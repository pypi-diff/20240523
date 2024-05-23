# Comparing `tmp/timelineomat-0.4.0.tar.gz` & `tmp/timelineomat-0.5.0.tar.gz`

## Comparing `timelineomat-0.4.0.tar` & `timelineomat-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    12131 2020-02-02 00:00:00.000000 timelineomat-0.4.0/timelineomat.py
--rw-r--r--   0        0        0    11775 2020-02-02 00:00:00.000000 timelineomat-0.4.0/tests/test_basics.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 timelineomat-0.4.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 timelineomat-0.4.0/LICENSE
--rw-r--r--   0        0        0     8209 2020-02-02 00:00:00.000000 timelineomat-0.4.0/README.md
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 timelineomat-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 timelineomat-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 timelineomat-0.5.0/timelineomat.py
+-rw-r--r--   0        0        0    12337 2020-02-02 00:00:00.000000 timelineomat-0.5.0/tests/test_basics.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 timelineomat-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 timelineomat-0.5.0/LICENSE
+-rw-r--r--   0        0        0     8340 2020-02-02 00:00:00.000000 timelineomat-0.5.0/README.md
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 timelineomat-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     9221 2020-02-02 00:00:00.000000 timelineomat-0.5.0/PKG-INFO
```

### Comparing `timelineomat-0.4.0/timelineomat.py` & `timelineomat-0.5.0/timelineomat.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 __all__ = [
     "streamline_event_times",
     "streamline_event",
     "ordered_insert",
     "TimelineOMat",
     "SkipEvent",
+    "SkipInvalidEvent",
+    "SkipOccludedEvent",
     "NoCallAllowedError",
     "PositionOffsetTuple",
     "TimeRangeTuple",
 ]
 
-from collections.abc import Callable, MutableSequence
+from collections.abc import Callable, Iterable, MutableSequence
 from datetime import datetime as dt
 from datetime import timezone as tz
 from functools import lru_cache
 from itertools import chain
 from typing import Literal, NamedTuple, Optional, TypeVar, Union
 
 Event = TypeVar("Event")
@@ -23,47 +25,60 @@
 FilterFunction = Callable[[Event], bool]
 CallableExtractor = Callable[[Event], ExtractionResult]
 Extractor = Union[str, CallableExtractor]
 CallableSetter = Callable[[Event, dt], None]
 Setter = Union[str, CallableSetter]
 
 
+class TimeRangeTuple(NamedTuple):
+    start: dt
+    stop: dt
+
+
+class PositionOffsetTuple(NamedTuple):
+    position: Position
+    offset: Offset
+
+
 class SkipEvent(BaseException):
     pass
 
 
-class NoCallAllowedError(Exception):
+class SkipInvalidEvent(SkipEvent):
     pass
 
 
-class TimeRangeTuple(NamedTuple):
-    start: dt
-    stop: dt
+class SkipOccludedEvent(SkipEvent):
+    original: TimeRangeTuple
 
+    def __init__(self, *args, original: TimeRangeTuple, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.original = original
 
-class PositionOffsetTuple(NamedTuple):
-    position: Position
-    offset: Offset
+
+class NoCallAllowedError(Exception):
+    pass
 
 
 # old name
 NewTimesResult = TimeRangeTuple
+_empty = frozenset()
 
 
 def create_extractor(extractor: Extractor) -> CallableExtractor:
     if not isinstance(extractor, str):
         return extractor
 
     def _extractor(event: Event) -> ExtractionResult:
         try:
             if isinstance(event, dict):
                 return event[extractor]
             return getattr(event, extractor)
-        except (KeyError, AttributeError):
-            raise SkipEvent from None
+        except (KeyError, AttributeError) as exc:
+            raise SkipInvalidEvent from exc
 
     return _extractor
 
 
 def create_setter(
     setter: Setter,
     *,
@@ -109,44 +124,70 @@
     start_extractor: CallableExtractor,
     stop_extractor: CallableExtractor,
     fallback_timezone: Optional[tz] = None,
 ) -> TimeRangeTuple:
     start = handle_result(start_extractor(event), fallback_timezone=fallback_timezone)
     stop = handle_result(stop_extractor(event), fallback_timezone=fallback_timezone)
     if stop <= start:
-        raise SkipEvent
+        raise SkipInvalidEvent("duration <= 0")
     return TimeRangeTuple(start=start, stop=stop)
 
 
-def streamline_event_times(
+def _streamline_event_times(
     event: Event,
-    *timelines,
+    timeline: Iterable[Event],
     start_extractor: Extractor = "start",
     stop_extractor: Extractor = "stop",
     filter_fn: Optional[FilterFunction] = None,
     fallback_timezone: Optional[tz] = None,
     **kwargs,
-) -> TimeRangeTuple:
+) -> tuple[TimeRangeTuple, TimeRangeTuple]:
     start_extractor = create_extractor(start_extractor)
     stop_extractor = create_extractor(stop_extractor)
-    start, stop = extract_tuple_from_event(event, start_extractor, stop_extractor, fallback_timezone)
-    if timelines:
-        for ev in chain.from_iterable(timelines):
-            if filter_fn and not filter_fn(ev):
-                continue
+    start, stop = orig_tuple = extract_tuple_from_event(event, start_extractor, stop_extractor, fallback_timezone)
+    if not timeline:
+        return orig_tuple, orig_tuple
+    for ev in timeline:
+        if filter_fn and not filter_fn(ev):
+            continue
+        try:
             ev_start, ev_stop = extract_tuple_from_event(ev, start_extractor, stop_extractor, fallback_timezone)
-            if ev_start <= start and ev_stop >= stop:
-                raise SkipEvent
-            if ev_start <= start and ev_stop > start:
-                start = ev_stop
-            if ev_start < stop and ev_stop >= stop:
-                stop = ev_start
-            if stop <= start:
-                raise SkipEvent
-    return TimeRangeTuple(start=start, stop=stop)
+        except SkipEvent:
+            continue
+        if ev_start <= start and ev_stop >= stop:
+            raise SkipOccludedEvent(original=orig_tuple)
+        if ev_start <= start and ev_stop > start:
+            start = ev_stop
+        if ev_start < stop and ev_stop >= stop:
+            stop = ev_start
+        if stop <= start:
+            raise SkipOccludedEvent(original=orig_tuple)
+    return TimeRangeTuple(start=start, stop=stop), orig_tuple
+
+
+def streamline_event_times(
+    event: Event,
+    *timelines,
+    occlusions: Optional[list[TimeRangeTuple]] = None,
+    **kwargs,
+) -> TimeRangeTuple:
+    try:
+        new_tuple, orig_tuple = _streamline_event_times(
+            event, chain.from_iterable(timelines) if timelines else _empty, **kwargs
+        )
+    except SkipOccludedEvent as exc:
+        if occlusions is not None:
+            occlusions.append(exc.original)
+        raise exc
+    if new_tuple != orig_tuple and occlusions is not None:
+        if orig_tuple.start != new_tuple.start:
+            occlusions.append(TimeRangeTuple(start=orig_tuple.start, stop=new_tuple.start))
+        if orig_tuple.stop != new_tuple.stop:
+            occlusions.append(TimeRangeTuple(start=new_tuple.stop, stop=orig_tuple.stop))
+    return new_tuple
 
 
 def streamline_event(
     event: Event,
     *timelines,
     start_extractor: Extractor = "start",
     stop_extractor: Extractor = "stop",
@@ -160,34 +201,35 @@
         start_setter = create_setter(start_setter)
     else:
         start_setter = create_setter(start_extractor, disallow_call_instant=True)
     if stop_setter is not None:
         stop_setter = create_setter(stop_setter)
     else:
         stop_setter = create_setter(stop_extractor, disallow_call_instant=True)
-    result = streamline_event_times(
+    new_tuple = streamline_event_times(
         event,
         chain.from_iterable(timelines),
         start_extractor=start_extractor,
         stop_extractor=stop_extractor,
         **kwargs,
     )
-    start_setter(event, result.start)
-    stop_setter(event, result.stop)
+    start_setter(event, new_tuple.start)
+    stop_setter(event, new_tuple.stop)
     return event
 
 
 def transform_events_to_times(
     *timelines,
     start_extractor: Extractor = "start",
     stop_extractor: Extractor = "stop",
     filter_fn: Optional[FilterFunction] = None,
     fallback_timezone: Optional[tz] = None,
     **kwargs,
 ) -> list[TimeRangeTuple]:
+    assert "occlusions" not in kwargs, "occlusions not supported for this function"
     start_extractor = create_extractor(start_extractor)
     stop_extractor = create_extractor(stop_extractor)
     transformed = []
     if not timelines:
         return transformed
     for ev in chain.from_iterable(timelines):
         if filter_fn and not filter_fn(ev):
@@ -247,14 +289,15 @@
 def ordered_insert(
     event: Event,
     timeline: MutableSequence[Event],
     *,
     direction: Literal["asc", "desc"] = "asc",
     **kwargs,
 ) -> PositionOffsetTuple:
+    assert "occlusions" not in kwargs, "occlusions not supported for this function"
     position = _ordered_insert(event, timeline, direction=direction, **kwargs)
     if direction == "desc":
         return PositionOffsetTuple(position=position, offset=len(timeline) - position - 1)
     return PositionOffsetTuple(position=position, offset=position)
 
 
 class TimelineOMat:
@@ -296,39 +339,43 @@
             return streamline_event_times(
                 event,
                 chain.from_iterable(timelines),
                 start_extractor=kwargs.get("start_extractor", self.start_extractor),
                 stop_extractor=kwargs.get("stop_extractor", self.stop_extractor),
                 filter_fn=kwargs.get("filter_fn", self.filter_fn),
                 fallback_timezone=kwargs.get("fallback_timezone", self.fallback_timezone),
+                occlusions=kwargs.get("occlusions", None),
             )
         else:
             return streamline_event_times(
                 event,
                 start_extractor=kwargs.get("start_extractor", self.start_extractor),
                 stop_extractor=kwargs.get("stop_extractor", self.stop_extractor),
                 filter_fn=kwargs.get("filter_fn", self.filter_fn),
                 fallback_timezone=kwargs.get("fallback_timezone", self.fallback_timezone),
+                occlusions=kwargs.get("occlusions", None),
             )
 
     def streamline_event(self, event: Event, *timelines, **kwargs) -> Event:
         if not timelines:
             return event
         return streamline_event(
             event,
             chain.from_iterable(timelines),
             start_extractor=kwargs.get("start_extractor", self.start_extractor),
             stop_extractor=kwargs.get("stop_extractor", self.stop_extractor),
             filter_fn=kwargs.get("filter_fn", self.filter_fn),
             fallback_timezone=kwargs.get("fallback_timezone", self.fallback_timezone),
             start_setter=kwargs.get("start_setter", self.start_setter),
             stop_setter=kwargs.get("stop_setter", self.stop_setter),
+            occlusions=kwargs.get("occlusions", None),
         )
 
     def transform_events_to_times(self, *timelines, **kwargs) -> list[TimeRangeTuple]:
+        assert "occlusions" not in kwargs, "occlusions not supported for this function"
         if not timelines:
             return []
         return transform_events_to_times(
             chain.from_iterable(timelines),
             start_extractor=kwargs.get("start_extractor", self.start_extractor),
             stop_extractor=kwargs.get("stop_extractor", self.stop_extractor),
             filter_fn=kwargs.get("filter_fn", self.filter_fn),
@@ -339,14 +386,15 @@
         self,
         event: Event,
         timeline: MutableSequence[Event],
         *,
         offset: Offset = 0,
         **kwargs,
     ) -> PositionOffsetTuple:
+        assert "occlusions" not in kwargs, "occlusions not supported for this function"
         return ordered_insert(
             event,
             timeline,
             offset=offset,
             start_extractor=kwargs.get("start_extractor", self.start_extractor),
             stop_extractor=kwargs.get("stop_extractor", self.stop_extractor),
             direction=kwargs.get("direction", self.direction),
```

### Comparing `timelineomat-0.4.0/tests/test_basics.py` & `timelineomat-0.5.0/tests/test_basics.py`

 * *Files 5% similar despite different names*

```diff
@@ -183,31 +183,43 @@
     events = []
     with pytest.raises(timelineomat.SkipEvent):
         timelineomat.streamline_event_times(Event1(start=dt(2024, 3, 2), stop=dt(2024, 2, 1)), events)
 
 
 def test_event_within_event():
     events = [Event1(start=dt(2024, 1, 1), stop=dt(2024, 3, 1))]
+    new_event = Event1(start=dt(2024, 1, 2), stop=dt(2024, 2, 1))
+    occlusions = []
     with pytest.raises(timelineomat.SkipEvent):
-        timelineomat.streamline_event_times(Event1(start=dt(2024, 1, 2), stop=dt(2024, 2, 1)), events)
+        timelineomat.streamline_event_times(new_event, events, occlusions=occlusions)
+    assert new_event.start == occlusions[0].start
+    assert new_event.stop == occlusions[0].stop
 
 
 def test_result():
     timeline = [Event1(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)), Event1(start=dt(2024, 1, 2), stop=dt(2024, 1, 3))]
     new_event = Event1(start=dt(2024, 1, 1), stop=dt(2024, 1, 4))
     # one time methods
-    assert timelineomat.streamline_event_times(new_event, timeline) == timelineomat.TimeRangeTuple(
+    occlusions = []
+    assert timelineomat.streamline_event_times(
+        new_event, timeline, occlusions=occlusions
+    ) == timelineomat.TimeRangeTuple(start=dt(2024, 1, 3), stop=dt(2024, 1, 4))
+    assert occlusions[0] == timelineomat.TimeRangeTuple(start=dt(2024, 1, 1), stop=dt(2024, 1, 3))
+    # TimelineOMat method
+    tm = timelineomat.TimelineOMat()
+    occlusions = []
+    assert tm.streamline_event_times(new_event, timeline, occlusions=occlusions) == timelineomat.TimeRangeTuple(
         start=dt(2024, 1, 3), stop=dt(2024, 1, 4)
     )
 
 
 def test_result_fallback_utc():
     timeline = [Event1(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)), Event1(start=dt(2024, 1, 2), stop=dt(2024, 1, 3))]
     new_event = Event1(start=dt(2024, 1, 1), stop=dt(2024, 1, 4))
-    # one time methods
+    # one time function
     assert timelineomat.streamline_event_times(
         new_event, timeline, fallback_timezone=timezone.utc
     ) == timelineomat.TimeRangeTuple(
         start=dt(2024, 1, 3, tzinfo=timezone.utc), stop=dt(2024, 1, 4, tzinfo=timezone.utc)
     )
```

### Comparing `timelineomat-0.4.0/.gitignore` & `timelineomat-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `timelineomat-0.4.0/LICENSE` & `timelineomat-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timelineomat-0.4.0/README.md` & `timelineomat-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
 ordered_insert also takes the parameters direction and offset (direction can be set on TimelineOMat). This allows performant inserts and collision checks.
 
 When ordered_insert is called with offset 0 or unset it is safe to call even when the insertion order is chaotic
 
 The timeline must be ordered anyway for ordered_insert
 
+There is a new argument occlusions which must be of type list. It receives the 
+occluded time ranges
 
 ``` python
 from dataclasses import dataclass
 from datetime import datetime as dt
 from timelineomat import TimelineOMat, streamline_event_times, stream_line_event, TimeRangeTuple
 
 
@@ -245,9 +247,10 @@
 
 ```
 
 Another usage of the key function would be together with heapq to implement some kind of merge sort
 
 ## Changes
 
+0.5.0 add occlusions argument
 0.4.0 rename NoCallAllowed to NoCallAllowedError
 0.3.0 rename NewTimesResult to TimeRangeTuple (the old name is still available)
```

### Comparing `timelineomat-0.4.0/pyproject.toml` & `timelineomat-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "timelineomat"
-version = "0.4.0"
+version = "0.5.0"
 description = "Squeeze events into timelines and other timeline manipulations"
 authors = [{name = "Alexander Kaftan", email="devkral@web.de"}]
 license = "MIT"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = [
     "event",
```

### Comparing `timelineomat-0.4.0/PKG-INFO` & `timelineomat-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: timelineomat
-Version: 0.4.0
+Version: 0.5.0
 Summary: Squeeze events into timelines and other timeline manipulations
 Author-email: Alexander Kaftan <devkral@web.de>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: database,event,time,timelines
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -43,14 +43,16 @@
 
 ordered_insert also takes the parameters direction and offset (direction can be set on TimelineOMat). This allows performant inserts and collision checks.
 
 When ordered_insert is called with offset 0 or unset it is safe to call even when the insertion order is chaotic
 
 The timeline must be ordered anyway for ordered_insert
 
+There is a new argument occlusions which must be of type list. It receives the 
+occluded time ranges
 
 ``` python
 from dataclasses import dataclass
 from datetime import datetime as dt
 from timelineomat import TimelineOMat, streamline_event_times, stream_line_event, TimeRangeTuple
 
 
@@ -267,9 +269,10 @@
 
 ```
 
 Another usage of the key function would be together with heapq to implement some kind of merge sort
 
 ## Changes
 
+0.5.0 add occlusions argument
 0.4.0 rename NoCallAllowed to NoCallAllowedError
 0.3.0 rename NewTimesResult to TimeRangeTuple (the old name is still available)
```

