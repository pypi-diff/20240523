# Comparing `tmp/timelineomat-0.3.0.tar.gz` & `tmp/timelineomat-0.3.1.tar.gz`

## Comparing `timelineomat-0.3.0.tar` & `timelineomat-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     8093 2020-02-02 00:00:00.000000 timelineomat-0.3.0/timelineomat.py
--rw-r--r--   0        0        0     7585 2020-02-02 00:00:00.000000 timelineomat-0.3.0/tests/test_basics.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 timelineomat-0.3.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 timelineomat-0.3.0/LICENSE
--rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 timelineomat-0.3.0/README.md
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 timelineomat-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 timelineomat-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     8846 2020-02-02 00:00:00.000000 timelineomat-0.3.1/timelineomat.py
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 timelineomat-0.3.1/tests/test_basics.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 timelineomat-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 timelineomat-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 timelineomat-0.3.1/README.md
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 timelineomat-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 timelineomat-0.3.1/PKG-INFO
```

### Comparing `timelineomat-0.3.0/timelineomat.py` & `timelineomat-0.3.1/timelineomat.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,44 +95,47 @@
 ) -> TimeRangeTuple:
     start_extractor = create_extractor(start_extractor)
     stop_extractor = create_extractor(stop_extractor)
     start = handle_result(start_extractor(event), fallback_timezone=fallback_timezone)
     stop = handle_result(stop_extractor(event), fallback_timezone=fallback_timezone)
     if stop <= start:
         raise SkipEvent
-    for ev in chain.from_iterable(timelines):
-        if filter_fn and not filter_fn(ev):
-            continue
-        try:
-            ev_start = handle_result(start_extractor(ev), fallback_timezone=fallback_timezone)
-            ev_stop = handle_result(stop_extractor(ev), fallback_timezone=fallback_timezone)
-        except SkipEvent:
-            continue
-        if ev_stop <= ev_start:
-            continue
-        if ev_start <= start and ev_stop >= stop:
-            raise SkipEvent
-        if ev_start <= start and ev_stop > start:
-            start = ev_stop
-        if ev_start < stop and ev_stop >= stop:
-            stop = ev_start
-        if stop <= start:
-            raise SkipEvent
+    if timelines:
+        for ev in chain.from_iterable(timelines):
+            if filter_fn and not filter_fn(ev):
+                continue
+            try:
+                ev_start = handle_result(start_extractor(ev), fallback_timezone=fallback_timezone)
+                ev_stop = handle_result(stop_extractor(ev), fallback_timezone=fallback_timezone)
+            except SkipEvent:
+                continue
+            if ev_stop <= ev_start:
+                continue
+            if ev_start <= start and ev_stop >= stop:
+                raise SkipEvent
+            if ev_start <= start and ev_stop > start:
+                start = ev_stop
+            if ev_start < stop and ev_stop >= stop:
+                stop = ev_start
+            if stop <= start:
+                raise SkipEvent
     return TimeRangeTuple(start=start, stop=stop)
 
 
 def streamline_event(
     event: Any,
     *timelines,
     start_extractor: Extractor = "start",
     stop_extractor: Extractor = "stop",
     start_setter: Optional[Setter] = None,
     stop_setter: Optional[Setter] = None,
     **kwargs,
 ) -> Any:
+    if not timelines:
+        return event
     if start_setter is not None:
         start_setter = create_setter(start_setter)
     else:
         start_setter = create_setter(start_extractor, disallow_call_instant=True)
     if stop_setter is not None:
         stop_setter = create_setter(stop_setter)
     else:
@@ -156,14 +159,16 @@
     filter_fn: Optional[Callable[[Any], bool]] = None,
     fallback_timezone: Optional[tz] = None,
     **kwargs,
 ) -> list[TimeRangeTuple]:
     start_extractor = create_extractor(start_extractor)
     stop_extractor = create_extractor(stop_extractor)
     transformed = []
+    if not timelines:
+        return transformed
     for ev in chain.from_iterable(timelines):
         if filter_fn and not filter_fn(ev):
             continue
         try:
             ev_start = handle_result(start_extractor(ev), fallback_timezone=fallback_timezone)
             ev_stop = handle_result(stop_extractor(ev), fallback_timezone=fallback_timezone)
         except SkipEvent:
@@ -194,36 +199,49 @@
             self.start_setter = create_setter(start_extractor, disallow_call=True)
         if stop_setter is not None:
             self.stop_setter = create_setter(stop_setter)
         else:
             self.stop_setter = create_setter(stop_extractor, disallow_call=True)
 
     def streamline_event_times(self, event: Any, *timelines, **kwargs) -> TimeRangeTuple:
-        return streamline_event_times(
-            event,
-            chain.from_iterable(timelines),
-            start_extractor=kwargs.get("start_extractor", self.start_extractor),
-            stop_extractor=kwargs.get("stop_extractor", self.stop_extractor),
-            filter_fn=kwargs.get("filter_fn", self.filter_fn),
-            fallback_timezone=kwargs.get("fallback_timezone", self.fallback_timezone),
-        )
-
-    def streamline_event(self, event: Any, *timelines, **kwargs) -> None:
+        if timelines:
+            return streamline_event_times(
+                event,
+                chain.from_iterable(timelines),
+                start_extractor=kwargs.get("start_extractor", self.start_extractor),
+                stop_extractor=kwargs.get("stop_extractor", self.stop_extractor),
+                filter_fn=kwargs.get("filter_fn", self.filter_fn),
+                fallback_timezone=kwargs.get("fallback_timezone", self.fallback_timezone),
+            )
+        else:
+            return streamline_event_times(
+                event,
+                start_extractor=kwargs.get("start_extractor", self.start_extractor),
+                stop_extractor=kwargs.get("stop_extractor", self.stop_extractor),
+                filter_fn=kwargs.get("filter_fn", self.filter_fn),
+                fallback_timezone=kwargs.get("fallback_timezone", self.fallback_timezone),
+            )
+
+    def streamline_event(self, event: Any, *timelines, **kwargs) -> Any:
+        if not timelines:
+            return event
         return streamline_event(
             event,
             chain.from_iterable(timelines),
             start_extractor=kwargs.get("start_extractor", self.start_extractor),
             stop_extractor=kwargs.get("stop_extractor", self.stop_extractor),
             filter_fn=kwargs.get("filter_fn", self.filter_fn),
             fallback_timezone=kwargs.get("fallback_timezone", self.fallback_timezone),
             start_setter=kwargs.get("start_setter", self.start_setter),
             stop_setter=kwargs.get("stop_setter", self.stop_setter),
         )
 
     def transform_events_to_times(self, *timelines, **kwargs) -> list[TimeRangeTuple]:
+        if not timelines:
+            return []
         return transform_events_to_times(
             chain.from_iterable(timelines),
             start_extractor=kwargs.get("start_extractor", self.start_extractor),
             stop_extractor=kwargs.get("stop_extractor", self.stop_extractor),
             filter_fn=kwargs.get("filter_fn", self.filter_fn),
             fallback_timezone=kwargs.get("fallback_timezone", self.fallback_timezone),
         )
```

### Comparing `timelineomat-0.3.0/tests/test_basics.py` & `timelineomat-0.3.1/tests/test_basics.py`

 * *Files 10% similar despite different names*

```diff
@@ -228,13 +228,38 @@
     assert timeline[-1].stop == dt(2024, 1, 4)
     assert timeline[-1].start == dt(2024, 1, 3)
     timeline.append(
         Event1(**tm.streamline_event_times(new_event2, timeline, stop_extractor=one_time_overwrite_end)._asdict())
     )
     assert timeline[-1].stop == dt(2024, 1, 5)
     assert timeline[-1].start == dt(2024, 1, 4)
+    # test conversion in TimeRangeTuple array
     assert tm.transform_events_to_times(timeline) == [
         timelineomat.TimeRangeTuple(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)),
         timelineomat.TimeRangeTuple(start=dt(2024, 1, 2), stop=dt(2024, 1, 3)),
         timelineomat.TimeRangeTuple(start=dt(2024, 1, 3), stop=dt(2024, 1, 4)),
         timelineomat.TimeRangeTuple(start=dt(2024, 1, 4), stop=dt(2024, 1, 5)),
     ]
+    # test sorting
+
+    assert tm.transform_events_to_times(sorted(timeline, key=tm.streamline_event_times, reverse=True)) == [
+        timelineomat.TimeRangeTuple(start=dt(2024, 1, 4), stop=dt(2024, 1, 5)),
+        timelineomat.TimeRangeTuple(start=dt(2024, 1, 3), stop=dt(2024, 1, 4)),
+        timelineomat.TimeRangeTuple(start=dt(2024, 1, 2), stop=dt(2024, 1, 3)),
+        timelineomat.TimeRangeTuple(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)),
+    ]
+
+
+
+def test_invalid_rejection():
+    timeline = []
+    new_event1 = Event1(stop=dt(2024, 1, 1), start=dt(2024, 1, 4))
+    with pytest.raises(timelineomat.SkipEvent):
+        timelineomat.streamline_event_times(new_event1, timeline)
+    with pytest.raises(timelineomat.SkipEvent):
+        timelineomat.streamline_event_times(new_event1)
+
+    tm = timelineomat.TimelineOMat()
+    with pytest.raises(timelineomat.SkipEvent):
+        tm.streamline_event_times(new_event1, timeline)
+    with pytest.raises(timelineomat.SkipEvent):
+        tm.streamline_event_times(new_event1)
```

### Comparing `timelineomat-0.3.0/.gitignore` & `timelineomat-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `timelineomat-0.3.0/LICENSE` & `timelineomat-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `timelineomat-0.3.0/README.md` & `timelineomat-0.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -164,10 +164,24 @@
 ## How to integrate in db systems
 
 DB Systems like django support range queries, which receives two element tuples. TimelineOMat can convert the timelines into such tuples (TimeRangeTuple doubles as tuple)
 
 An example is in Usage
 
 
+## How to use for sorting
+
+simple use the streamline_event_times(...) method of TimelineOMat without any timelines as key function. By using the TimelineOMat parameter can be preinitialized
+
+The resulting tuple can be sorted
+
+
+``` python
+
+tm = TimelineOMat()
+timeline.sort(key=tm.streamline_event_times)
+
+```
+
 ## Changes
 
 0.3.0 rename NewTimesResult to TimeRangeTuple (the old name is still available)
```

### Comparing `timelineomat-0.3.0/pyproject.toml` & `timelineomat-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "timelineomat"
-version = "0.3.0"
+version = "0.3.1"
 description = "Squeeze events into timelines and other timeline manipulations"
 authors = [{name = "Alexander Kaftan", email="devkral@web.de"}]
 license = "MIT"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = [
     "event",
```

### Comparing `timelineomat-0.3.0/PKG-INFO` & `timelineomat-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: timelineomat
-Version: 0.3.0
+Version: 0.3.1
 Summary: Squeeze events into timelines and other timeline manipulations
 Author-email: Alexander Kaftan <devkral@web.de>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: database,event,time,timelines
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -186,10 +186,24 @@
 ## How to integrate in db systems
 
 DB Systems like django support range queries, which receives two element tuples. TimelineOMat can convert the timelines into such tuples (TimeRangeTuple doubles as tuple)
 
 An example is in Usage
 
 
+## How to use for sorting
+
+simple use the streamline_event_times(...) method of TimelineOMat without any timelines as key function. By using the TimelineOMat parameter can be preinitialized
+
+The resulting tuple can be sorted
+
+
+``` python
+
+tm = TimelineOMat()
+timeline.sort(key=tm.streamline_event_times)
+
+```
+
 ## Changes
 
 0.3.0 rename NewTimesResult to TimeRangeTuple (the old name is still available)
```

