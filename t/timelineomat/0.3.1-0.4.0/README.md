# Comparing `tmp/timelineomat-0.3.1.tar.gz` & `tmp/timelineomat-0.4.0.tar.gz`

## Comparing `timelineomat-0.3.1.tar` & `timelineomat-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     8846 2020-02-02 00:00:00.000000 timelineomat-0.3.1/timelineomat.py
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 timelineomat-0.3.1/tests/test_basics.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 timelineomat-0.3.1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 timelineomat-0.3.1/LICENSE
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 timelineomat-0.3.1/README.md
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 timelineomat-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 timelineomat-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    12131 2020-02-02 00:00:00.000000 timelineomat-0.4.0/timelineomat.py
+-rw-r--r--   0        0        0    11775 2020-02-02 00:00:00.000000 timelineomat-0.4.0/tests/test_basics.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 timelineomat-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 timelineomat-0.4.0/LICENSE
+-rw-r--r--   0        0        0     8209 2020-02-02 00:00:00.000000 timelineomat-0.4.0/README.md
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 timelineomat-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 timelineomat-0.4.0/PKG-INFO
```

### Comparing `timelineomat-0.3.1/tests/test_basics.py` & `timelineomat-0.4.0/tests/test_basics.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,26 +18,26 @@
 
 @dataclass
 class Event2:
     begin: dt
     end: dt
 
 
+def _generate_time_tuple(faker, start):
+    return start, start + td(hours=faker.random_int(1, 48))
+
+
 def _generate_event_series(_type, _variant):
     faker = Faker()
     ts_start = faker.past_datetime(
         "-200d",
     )
-    ts_stop = faker.past_datetime(
-        "-200d",
-    )
     events = []
     for _i in range(1000):
-        while ts_stop < ts_start:
-            ts_stop += td(hours=faker.random_int(1, 48))
+        ts_stop = _generate_time_tuple(faker, ts_start)[1]
         if _variant == 1:
             events.append(_type(start=ts_start, stop=ts_stop))
         else:
             events.append(_type(begin=ts_start, end=ts_stop))
         ts_start += td(hours=faker.random_int(1, 48))
     return events
 
@@ -245,21 +245,97 @@
         timelineomat.TimeRangeTuple(start=dt(2024, 1, 4), stop=dt(2024, 1, 5)),
         timelineomat.TimeRangeTuple(start=dt(2024, 1, 3), stop=dt(2024, 1, 4)),
         timelineomat.TimeRangeTuple(start=dt(2024, 1, 2), stop=dt(2024, 1, 3)),
         timelineomat.TimeRangeTuple(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)),
     ]
 
 
+@pytest.mark.parametrize("direction", ["asc", "desc"])
+def test_ordered_insert_basic(direction):
+    timeline = [
+        Event1(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)),
+        # invalid event
+        {},
+        Event1(start=dt(2024, 1, 5), stop=dt(2024, 1, 6)),
+        Event1(start=dt(2024, 1, 10), stop=dt(2024, 1, 11)),
+        Event1(start=dt(2024, 1, 12), stop=dt(2024, 1, 13)),
+    ]
+    tm = timelineomat.TimelineOMat(direction=direction)
+    position_offset = tm.ordered_insert(
+        Event1(start=dt(2024, 1, 2), stop=dt(2024, 1, 3)), timeline, direction=direction
+    )
+    # invalid element is skipped
+    if direction == "asc":
+        assert position_offset == (2, 2)
+        position_offset = position_offset.offset
+    else:
+        assert position_offset == (1, 4)
+        # unset it for desc, we add asc events
+        position_offset = 0
+    # test stability
+    position_offset = tm.ordered_insert(
+        Event1(start=dt(2024, 1, 2), stop=dt(2024, 1, 3)), timeline, offset=position_offset
+    )
+    if direction == "asc":
+        assert position_offset == (3, 3)
+        position_offset = position_offset.offset
+    else:
+        assert position_offset == (1, 5)
+        position_offset = 0
+    # overlapping
+    position_offset = tm.ordered_insert(
+        Event1(start=dt(2024, 1, 7), stop=dt(2024, 1, 12)), timeline, offset=position_offset
+    )
+    if direction == "asc":
+        assert position_offset == (5, 5)
+        position_offset = position_offset.offset
+    else:
+        assert position_offset == (5, 2)
+        position_offset = 0
+
+
+def test_ordered_insert_desc():
+    # desc is more complicated
+    timeline = [
+        Event1(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)),
+        # invalid event
+        {},
+        Event1(start=dt(2024, 1, 5), stop=dt(2024, 1, 6)),
+        Event1(start=dt(2024, 1, 10), stop=dt(2024, 1, 11)),
+        Event1(start=dt(2024, 1, 12), stop=dt(2024, 1, 13)),
+    ]
+    tm = timelineomat.TimelineOMat(direction="desc")
+    # we need to insert descending
+    position, offset = tm.ordered_insert(Event1(start=dt(2024, 1, 12), stop=dt(2024, 1, 13)), timeline)
+    assert offset == 1
+    assert position == 4
+    # should work also for stop
+    position, offset = tm.ordered_insert(
+        Event1(start=dt(2024, 1, 12), stop=dt(2024, 1, 13)), timeline, extractor="stop", offset=offset
+    )
+    assert offset == 2
+    position, offset = tm.ordered_insert(Event1(start=dt(2024, 1, 7), stop=dt(2024, 1, 8)), timeline, offset=offset)
+    assert offset == 4
+    position = tm.ordered_insert(Event1(start=dt(2023, 1, 12), stop=dt(2023, 1, 13)), timeline, offset=offset).position
+    assert position == 0
+    # we are still descendend concerning the 2nd last insert and didn't updated the offset
+    position = tm.ordered_insert(Event1(start=dt(2024, 1, 2), stop=dt(2024, 1, 3)), timeline, offset=offset).position
+    assert position == 2
+
 
 def test_invalid_rejection():
     timeline = []
     new_event1 = Event1(stop=dt(2024, 1, 1), start=dt(2024, 1, 4))
     with pytest.raises(timelineomat.SkipEvent):
         timelineomat.streamline_event_times(new_event1, timeline)
     with pytest.raises(timelineomat.SkipEvent):
         timelineomat.streamline_event_times(new_event1)
+    with pytest.raises(timelineomat.SkipEvent):
+        timelineomat.ordered_insert(new_event1, timeline)
 
     tm = timelineomat.TimelineOMat()
     with pytest.raises(timelineomat.SkipEvent):
         tm.streamline_event_times(new_event1, timeline)
     with pytest.raises(timelineomat.SkipEvent):
         tm.streamline_event_times(new_event1)
+    with pytest.raises(timelineomat.SkipEvent):
+        tm.ordered_insert(new_event1, timeline)
```

### Comparing `timelineomat-0.3.1/.gitignore` & `timelineomat-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `timelineomat-0.3.1/LICENSE` & `timelineomat-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timelineomat-0.3.1/README.md` & `timelineomat-0.4.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -8,33 +8,43 @@
 ## Installation
 ``` sh
 pip install timelineomat
 ```
 
 ## Usage
 
-There are 3 different functions which also exist as methods of the TimelineOMat class
+There are 4 different functions which also exist as methods of the TimelineOMat class
 
-- streamline_event_times: checks how to short the given event to fit into the timelines
+- streamline_event_times: checks how to short the given event to fit into the timelines. Without a timeline the result can be used for sorting (see section later)
 - streamline_event: uses streamline_event_times plus setters to update the event and returns event
 - transform_events_to_times: transforms timelines to TimeRangeTuple for e.g. databases
+- ordered_insert: insert an event in a timeline so it stays ordered. By default an offset is returned. It can be used in case of ascending inserts to improve the performance
+
+ordered_insert also takes the parameters direction and offset (direction can be set on TimelineOMat). This allows performant inserts and collision checks.
+
+When ordered_insert is called with offset 0 or unset it is safe to call even when the insertion order is chaotic
+
+The timeline must be ordered anyway for ordered_insert
 
 
 ``` python
 from dataclasses import dataclass
 from datetime import datetime as dt
 from timelineomat import TimelineOMat, streamline_event_times, stream_line_event, TimeRangeTuple
 
 
 @dataclass
 class Event:
     start: dt
     stop: dt
 
-timeline = [Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)), Event(start=dt(2024, 1, 2), stop=dt(2024, 1, 3))]
+timeline = [
+    Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)),
+    Event(start=dt(2024, 1, 2), stop=dt(2024, 1, 3))
+]
 new_event = Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 4))
 # one time methods
 # get intermediate result of new times
 streamline_event_times(new_event, timeline) == TimeRangeTuple(start=dt(2024, 1, 3), stop=dt(2024, 1, 4))
 # update the event
 timeline.append(streamline_event(new_event, timeline))
 
@@ -96,15 +106,18 @@
 
 @dataclass
 class Event:
     start: dt
     stop: dt
 
 
-timeline = [Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)), Event(start=dt(2024, 1, 2), stop=dt(2024, 1, 3))]
+timeline = [
+    Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)),
+    Event(start=dt(2024, 1, 2), stop=dt(2024, 1, 3))
+]
 new_event1 = Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 4))
 new_event2 = dict(start=dt(2024, 1, 1), end=dt(2024, 1, 5))
 
 tm = TimelineOMat()
 ```
 
 it is possible to extract the data with
@@ -121,16 +134,14 @@
 timeline.append(tm.streamline_event(new_event1, timeline))
 #
 
 timeline.append(Event(**tm.streamline_event_times(new_event2, timeline, stop_extractor=one_time_overwrite_end)._asdict()))
 ```
 
 
-
-
 ## Tricks to improve the performance:
 
 ### Using TimelineOMat
  In case of the one time methods the extractors and setters are generated all the time when using string extractors or setters -> bad performance
 
 Building an TimelineOMat is more efficient or alternatively provide functions for extractors and setters
 
@@ -147,41 +158,96 @@
 
 
 @dataclass
 class Event:
     start: dt
     stop: dt
 
-ordered_timeline = [Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)), Event(start=dt(2024, 1, 2), stop=dt(2024, 1, 3))]
+ordered_timeline = [
+    Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)),
+    Event(start=dt(2024, 1, 2), stop=dt(2024, 1, 3))
+]
 new_event = Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 4))
 # here we generate the setters and extractors only onetime
 tm = TimelineOMat()
 tm.streamline_event_times(new_event, ordered_timeline[-1:])
-#
+
+```
+
+In case the inserts are not completely ordered there is a helper named ordered_insert. It returns and takes (optionally) an offset. As soon as a break in the monotonic ascending or descending is detected, the offset can be set to 0.
+
+Note: position and offset are in ascending orders the same.
+
+
+``` python
+from dataclasses import dataclass
+from datetime import datetime as dt
+from timelineomat import TimelineOMat
+
+
+@dataclass
+class Event:
+    start: dt
+    stop: dt
+
+ordered_timeline = [
+    Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)),
+    Event(start=dt(2024, 1, 2), stop=dt(2024, 1, 3))
+]
+new_event1 = Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 4))
+new_event2 = Event(start=dt(2023, 1, 1), stop=dt(2023, 1, 4))
+new_event3 = Event(start=dt(2025, 1, 1), stop=dt(2025, 1, 4))
+new_event4 = Event(start=dt(2025, 2, 1), stop=dt(2025, 2, 4))
+# here we generate the setters and extractors only onetime
+tm = TimelineOMat(direction="desc")
+position, offset = tm.ordered_insert(
+    tm.streamline_event(
+        new_event1, ordered_timeline[:len(ordered_timeline)-1-offset]
+    ),
+    ordered_timeline
+)
+position, offset = tm.ordered_insert(tm.streamline_event(new_event2, ordered_timeline[-1:]), ordered_timeline, offset=offset)
+# is stable
+position = tm.ordered_insert(tm.streamline_event(new_event2, ordered_timeline[-1:]), ordered_timeline, offset=offset).position
+# here is a break in the monotic order and we get ascending inserts
+offset = 0
+position, offset = tm.ordered_insert(tm.streamline_event(new_event3, ordered_timeline), ordered_timeline, offset=offset, direction="asc")
+position, offset = tm.ordered_insert(tm.streamline_event(new_event4, ordered_timeline[-1:]), ordered_timeline, offset=offset, direction="asc")
 
 ```
 
 
 ## How to integrate in db systems
 
 DB Systems like django support range queries, which receives two element tuples. TimelineOMat can convert the timelines into such tuples (TimeRangeTuple doubles as tuple)
 
 An example is in Usage
 
 
 ## How to use for sorting
 
-simple use the streamline_event_times(...) method of TimelineOMat without any timelines as key function. By using the TimelineOMat parameter can be preinitialized
+simple use the streamline_event_times(...) method of TimelineOMat without any timelines as key function. By using the TimelineOMat class parameters can be preinitialized
 
 The resulting tuple can be sorted
 
-
 ``` python
 
 tm = TimelineOMat()
 timeline.sort(key=tm.streamline_event_times)
 
 ```
 
+To compare only the start or stop timestamps
+
+``` python
+
+tm = TimelineOMat()
+timeline.sort(key=tm.start_extractor)
+
+```
+
+Another usage of the key function would be together with heapq to implement some kind of merge sort
+
 ## Changes
 
+0.4.0 rename NoCallAllowed to NoCallAllowedError
 0.3.0 rename NewTimesResult to TimeRangeTuple (the old name is still available)
```

### Comparing `timelineomat-0.3.1/pyproject.toml` & `timelineomat-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "timelineomat"
-version = "0.3.1"
+version = "0.4.0"
 description = "Squeeze events into timelines and other timeline manipulations"
 authors = [{name = "Alexander Kaftan", email="devkral@web.de"}]
 license = "MIT"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = [
     "event",
```

### Comparing `timelineomat-0.3.1/PKG-INFO` & `timelineomat-0.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: timelineomat
-Version: 0.3.1
+Version: 0.4.0
 Summary: Squeeze events into timelines and other timeline manipulations
 Author-email: Alexander Kaftan <devkral@web.de>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: database,event,time,timelines
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -30,33 +30,43 @@
 ## Installation
 ``` sh
 pip install timelineomat
 ```
 
 ## Usage
 
-There are 3 different functions which also exist as methods of the TimelineOMat class
+There are 4 different functions which also exist as methods of the TimelineOMat class
 
-- streamline_event_times: checks how to short the given event to fit into the timelines
+- streamline_event_times: checks how to short the given event to fit into the timelines. Without a timeline the result can be used for sorting (see section later)
 - streamline_event: uses streamline_event_times plus setters to update the event and returns event
 - transform_events_to_times: transforms timelines to TimeRangeTuple for e.g. databases
+- ordered_insert: insert an event in a timeline so it stays ordered. By default an offset is returned. It can be used in case of ascending inserts to improve the performance
+
+ordered_insert also takes the parameters direction and offset (direction can be set on TimelineOMat). This allows performant inserts and collision checks.
+
+When ordered_insert is called with offset 0 or unset it is safe to call even when the insertion order is chaotic
+
+The timeline must be ordered anyway for ordered_insert
 
 
 ``` python
 from dataclasses import dataclass
 from datetime import datetime as dt
 from timelineomat import TimelineOMat, streamline_event_times, stream_line_event, TimeRangeTuple
 
 
 @dataclass
 class Event:
     start: dt
     stop: dt
 
-timeline = [Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)), Event(start=dt(2024, 1, 2), stop=dt(2024, 1, 3))]
+timeline = [
+    Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)),
+    Event(start=dt(2024, 1, 2), stop=dt(2024, 1, 3))
+]
 new_event = Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 4))
 # one time methods
 # get intermediate result of new times
 streamline_event_times(new_event, timeline) == TimeRangeTuple(start=dt(2024, 1, 3), stop=dt(2024, 1, 4))
 # update the event
 timeline.append(streamline_event(new_event, timeline))
 
@@ -118,15 +128,18 @@
 
 @dataclass
 class Event:
     start: dt
     stop: dt
 
 
-timeline = [Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)), Event(start=dt(2024, 1, 2), stop=dt(2024, 1, 3))]
+timeline = [
+    Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)),
+    Event(start=dt(2024, 1, 2), stop=dt(2024, 1, 3))
+]
 new_event1 = Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 4))
 new_event2 = dict(start=dt(2024, 1, 1), end=dt(2024, 1, 5))
 
 tm = TimelineOMat()
 ```
 
 it is possible to extract the data with
@@ -143,16 +156,14 @@
 timeline.append(tm.streamline_event(new_event1, timeline))
 #
 
 timeline.append(Event(**tm.streamline_event_times(new_event2, timeline, stop_extractor=one_time_overwrite_end)._asdict()))
 ```
 
 
-
-
 ## Tricks to improve the performance:
 
 ### Using TimelineOMat
  In case of the one time methods the extractors and setters are generated all the time when using string extractors or setters -> bad performance
 
 Building an TimelineOMat is more efficient or alternatively provide functions for extractors and setters
 
@@ -169,41 +180,96 @@
 
 
 @dataclass
 class Event:
     start: dt
     stop: dt
 
-ordered_timeline = [Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)), Event(start=dt(2024, 1, 2), stop=dt(2024, 1, 3))]
+ordered_timeline = [
+    Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)),
+    Event(start=dt(2024, 1, 2), stop=dt(2024, 1, 3))
+]
 new_event = Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 4))
 # here we generate the setters and extractors only onetime
 tm = TimelineOMat()
 tm.streamline_event_times(new_event, ordered_timeline[-1:])
-#
+
+```
+
+In case the inserts are not completely ordered there is a helper named ordered_insert. It returns and takes (optionally) an offset. As soon as a break in the monotonic ascending or descending is detected, the offset can be set to 0.
+
+Note: position and offset are in ascending orders the same.
+
+
+``` python
+from dataclasses import dataclass
+from datetime import datetime as dt
+from timelineomat import TimelineOMat
+
+
+@dataclass
+class Event:
+    start: dt
+    stop: dt
+
+ordered_timeline = [
+    Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)),
+    Event(start=dt(2024, 1, 2), stop=dt(2024, 1, 3))
+]
+new_event1 = Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 4))
+new_event2 = Event(start=dt(2023, 1, 1), stop=dt(2023, 1, 4))
+new_event3 = Event(start=dt(2025, 1, 1), stop=dt(2025, 1, 4))
+new_event4 = Event(start=dt(2025, 2, 1), stop=dt(2025, 2, 4))
+# here we generate the setters and extractors only onetime
+tm = TimelineOMat(direction="desc")
+position, offset = tm.ordered_insert(
+    tm.streamline_event(
+        new_event1, ordered_timeline[:len(ordered_timeline)-1-offset]
+    ),
+    ordered_timeline
+)
+position, offset = tm.ordered_insert(tm.streamline_event(new_event2, ordered_timeline[-1:]), ordered_timeline, offset=offset)
+# is stable
+position = tm.ordered_insert(tm.streamline_event(new_event2, ordered_timeline[-1:]), ordered_timeline, offset=offset).position
+# here is a break in the monotic order and we get ascending inserts
+offset = 0
+position, offset = tm.ordered_insert(tm.streamline_event(new_event3, ordered_timeline), ordered_timeline, offset=offset, direction="asc")
+position, offset = tm.ordered_insert(tm.streamline_event(new_event4, ordered_timeline[-1:]), ordered_timeline, offset=offset, direction="asc")
 
 ```
 
 
 ## How to integrate in db systems
 
 DB Systems like django support range queries, which receives two element tuples. TimelineOMat can convert the timelines into such tuples (TimeRangeTuple doubles as tuple)
 
 An example is in Usage
 
 
 ## How to use for sorting
 
-simple use the streamline_event_times(...) method of TimelineOMat without any timelines as key function. By using the TimelineOMat parameter can be preinitialized
+simple use the streamline_event_times(...) method of TimelineOMat without any timelines as key function. By using the TimelineOMat class parameters can be preinitialized
 
 The resulting tuple can be sorted
 
-
 ``` python
 
 tm = TimelineOMat()
 timeline.sort(key=tm.streamline_event_times)
 
 ```
 
+To compare only the start or stop timestamps
+
+``` python
+
+tm = TimelineOMat()
+timeline.sort(key=tm.start_extractor)
+
+```
+
+Another usage of the key function would be together with heapq to implement some kind of merge sort
+
 ## Changes
 
+0.4.0 rename NoCallAllowed to NoCallAllowedError
 0.3.0 rename NewTimesResult to TimeRangeTuple (the old name is still available)
```

