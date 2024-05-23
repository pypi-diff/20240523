# Comparing `tmp/utbot_executor-1.9.8.tar.gz` & `tmp/utbot_executor-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utbot_executor-1.9.8.tar", max compression
+gzip compressed data, was "utbot_executor-1.9.9.tar", max compression
```

## Comparing `utbot_executor-1.9.8.tar` & `utbot_executor-1.9.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     3501 2023-11-24 05:51:01.489618 utbot_executor-1.9.8/README.md
--rw-r--r--   0        0        0      450 2023-11-30 11:06:26.474859 utbot_executor-1.9.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-13 11:46:22.950058 utbot_executor-1.9.8/utbot_executor/__init__.py
--rw-r--r--   0        0        0     2012 2023-11-27 11:37:43.174368 utbot_executor-1.9.8/utbot_executor/__main__.py
--rw-r--r--   0        0        0      491 2023-11-27 11:16:40.470272 utbot_executor-1.9.8/utbot_executor/config.py
--rw-r--r--   0        0        0        0 2023-10-13 11:46:22.950058 utbot_executor-1.9.8/utbot_executor/deep_serialization/__init__.py
--rw-r--r--   0        0        0       96 2023-10-13 11:46:22.950058 utbot_executor-1.9.8/utbot_executor/deep_serialization/config.py
--rw-r--r--   0        0        0     2090 2023-10-13 11:46:22.950058 utbot_executor-1.9.8/utbot_executor/deep_serialization/deep_serialization.py
--rw-r--r--   0        0        0     2358 2023-10-13 11:46:22.950058 utbot_executor-1.9.8/utbot_executor/deep_serialization/example.py
--rw-r--r--   0        0        0     1703 2023-11-24 05:51:01.492952 utbot_executor-1.9.8/utbot_executor/deep_serialization/iterator_wrapper.py
--rw-r--r--   0        0        0    11243 2023-11-24 05:51:01.492952 utbot_executor-1.9.8/utbot_executor/deep_serialization/json_converter.py
--rw-r--r--   0        0        0    16907 2023-11-30 10:48:35.579995 utbot_executor-1.9.8/utbot_executor/deep_serialization/memory_objects.py
--rw-r--r--   0        0        0     3866 2023-10-13 11:46:22.950058 utbot_executor-1.9.8/utbot_executor/deep_serialization/test_json.json
--rw-r--r--   0        0        0     5500 2023-10-13 11:46:22.950058 utbot_executor-1.9.8/utbot_executor/deep_serialization/utils.py
--rw-r--r--   0        0        0        0 2023-10-13 11:46:22.950058 utbot_executor-1.9.8/utbot_executor/example/__init__.py
--rw-r--r--   0        0        0     2008 2023-11-24 05:51:01.492952 utbot_executor-1.9.8/utbot_executor/example/example.py
--rw-r--r--   0        0        0      186 2023-10-13 11:46:22.950058 utbot_executor-1.9.8/utbot_executor/example/my_func.py
--rw-r--r--   0        0        0    12420 2023-11-28 09:30:47.369454 utbot_executor-1.9.8/utbot_executor/executor.py
--rw-r--r--   0        0        0     3324 2023-11-27 11:16:40.656937 utbot_executor-1.9.8/utbot_executor/listener.py
--rw-r--r--   0        0        0      654 2023-11-24 05:51:01.496285 utbot_executor-1.9.8/utbot_executor/memory_compressor.py
--rw-r--r--   0        0        0     3013 2023-11-30 10:11:13.088412 utbot_executor-1.9.8/utbot_executor/parser.py
--rw-r--r--   0        0        0     4514 2023-10-26 07:03:57.933969 utbot_executor-1.9.8/utbot_executor/ut_tracer.py
--rw-r--r--   0        0        0     1418 2023-11-24 05:51:01.496285 utbot_executor-1.9.8/utbot_executor/utils.py
--rw-r--r--   0        0        0     3959 1970-01-01 00:00:00.000000 utbot_executor-1.9.8/PKG-INFO
+-rw-r--r--   0        0        0     3501 2023-11-24 05:51:01.489618 utbot_executor-1.9.9/README.md
+-rw-r--r--   0        0        0      450 2023-12-01 07:47:41.368565 utbot_executor-1.9.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-10-13 11:46:22.950058 utbot_executor-1.9.9/utbot_executor/__init__.py
+-rw-r--r--   0        0        0     2012 2023-11-27 11:37:43.174368 utbot_executor-1.9.9/utbot_executor/__main__.py
+-rw-r--r--   0        0        0      491 2023-11-27 11:16:40.470272 utbot_executor-1.9.9/utbot_executor/config.py
+-rw-r--r--   0        0        0        0 2023-10-13 11:46:22.950058 utbot_executor-1.9.9/utbot_executor/deep_serialization/__init__.py
+-rw-r--r--   0        0        0       96 2023-10-13 11:46:22.950058 utbot_executor-1.9.9/utbot_executor/deep_serialization/config.py
+-rw-r--r--   0        0        0     2090 2023-10-13 11:46:22.950058 utbot_executor-1.9.9/utbot_executor/deep_serialization/deep_serialization.py
+-rw-r--r--   0        0        0     2358 2023-10-13 11:46:22.950058 utbot_executor-1.9.9/utbot_executor/deep_serialization/example.py
+-rw-r--r--   0        0        0     1703 2023-11-24 05:51:01.492952 utbot_executor-1.9.9/utbot_executor/deep_serialization/iterator_wrapper.py
+-rw-r--r--   0        0        0    11243 2023-11-24 05:51:01.492952 utbot_executor-1.9.9/utbot_executor/deep_serialization/json_converter.py
+-rw-r--r--   0        0        0    16881 2023-12-01 07:47:15.764463 utbot_executor-1.9.9/utbot_executor/deep_serialization/memory_objects.py
+-rw-r--r--   0        0        0     3866 2023-10-13 11:46:22.950058 utbot_executor-1.9.9/utbot_executor/deep_serialization/test_json.json
+-rw-r--r--   0        0        0     5504 2023-12-01 07:47:29.321537 utbot_executor-1.9.9/utbot_executor/deep_serialization/utils.py
+-rw-r--r--   0        0        0        0 2023-10-13 11:46:22.950058 utbot_executor-1.9.9/utbot_executor/example/__init__.py
+-rw-r--r--   0        0        0     2008 2023-11-24 05:51:01.492952 utbot_executor-1.9.9/utbot_executor/example/example.py
+-rw-r--r--   0        0        0      186 2023-10-13 11:46:22.950058 utbot_executor-1.9.9/utbot_executor/example/my_func.py
+-rw-r--r--   0        0        0    12420 2023-11-28 09:30:47.369454 utbot_executor-1.9.9/utbot_executor/executor.py
+-rw-r--r--   0        0        0     3324 2023-11-27 11:16:40.656937 utbot_executor-1.9.9/utbot_executor/listener.py
+-rw-r--r--   0        0        0      654 2023-11-24 05:51:01.496285 utbot_executor-1.9.9/utbot_executor/memory_compressor.py
+-rw-r--r--   0        0        0     3013 2023-11-30 10:11:13.088412 utbot_executor-1.9.9/utbot_executor/parser.py
+-rw-r--r--   0        0        0     4514 2023-10-26 07:03:57.933969 utbot_executor-1.9.9/utbot_executor/ut_tracer.py
+-rw-r--r--   0        0        0     1418 2023-11-24 05:51:01.496285 utbot_executor-1.9.9/utbot_executor/utils.py
+-rw-r--r--   0        0        0     3959 1970-01-01 00:00:00.000000 utbot_executor-1.9.9/PKG-INFO
```

### Comparing `utbot_executor-1.9.8/README.md` & `utbot_executor-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.9.8/utbot_executor/__main__.py` & `utbot_executor-1.9.9/utbot_executor/__main__.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.9.8/utbot_executor/deep_serialization/deep_serialization.py` & `utbot_executor-1.9.9/utbot_executor/deep_serialization/deep_serialization.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.9.8/utbot_executor/deep_serialization/example.py` & `utbot_executor-1.9.9/utbot_executor/deep_serialization/example.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.9.8/utbot_executor/deep_serialization/iterator_wrapper.py` & `utbot_executor-1.9.9/utbot_executor/deep_serialization/iterator_wrapper.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.9.8/utbot_executor/deep_serialization/json_converter.py` & `utbot_executor-1.9.9/utbot_executor/deep_serialization/json_converter.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.9.8/utbot_executor/deep_serialization/memory_objects.py` & `utbot_executor-1.9.9/utbot_executor/deep_serialization/memory_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from __future__ import annotations
 
-import copyreg
 import inspect
 import logging
+import pickle
 import re
 import sys
 import typing
 from itertools import zip_longest
-import pickle
-from typing import Any, Callable, Dict, List, Optional, Set, Type, Iterator, Iterable
-
+from typing import Any, Callable, Dict, List, Optional, Set, Type, Iterable
 from utbot_executor.deep_serialization.config import PICKLE_PROTO
 from utbot_executor.deep_serialization.iterator_wrapper import IteratorWrapper
 from utbot_executor.deep_serialization.utils import (
     PythonId,
     get_kind,
     has_reduce,
     check_comparability,
```

### Comparing `utbot_executor-1.9.8/utbot_executor/deep_serialization/test_json.json` & `utbot_executor-1.9.9/utbot_executor/deep_serialization/test_json.json`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.9.8/utbot_executor/deep_serialization/utils.py` & `utbot_executor-1.9.9/utbot_executor/deep_serialization/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         result = TypeInfo("builtins", "object.__new__")
     elif constructor is None:
         result = TypeInfo("types", "NoneType")
     else:
         result = TypeInfo(constructor.__module__, constructor.__qualname__)
 
     if result.kind == "object.__new__" and obj.__new__.__module__ is None:
-        result = TypeInfo(obj.__module__, f"{obj.__class__.__name__}.__new__")
+        result = TypeInfo(obj.__module__, f"{obj.__class__.__qualname__}.__new__")
     return result
 
 
 def has_reduce(py_object: object) -> bool:
     reduce = getattr(py_object, "__reduce__", None)
     if reduce is None:
         return False
```

### Comparing `utbot_executor-1.9.8/utbot_executor/example/example.py` & `utbot_executor-1.9.9/utbot_executor/example/example.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.9.8/utbot_executor/executor.py` & `utbot_executor-1.9.9/utbot_executor/executor.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.9.8/utbot_executor/listener.py` & `utbot_executor-1.9.9/utbot_executor/listener.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.9.8/utbot_executor/memory_compressor.py` & `utbot_executor-1.9.9/utbot_executor/memory_compressor.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.9.8/utbot_executor/parser.py` & `utbot_executor-1.9.9/utbot_executor/parser.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.9.8/utbot_executor/ut_tracer.py` & `utbot_executor-1.9.9/utbot_executor/ut_tracer.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.9.8/utbot_executor/utils.py` & `utbot_executor-1.9.9/utbot_executor/utils.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.9.8/PKG-INFO` & `utbot_executor-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utbot-executor
-Version: 1.9.8
+Version: 1.9.9
 Summary: 
 Author: Vyacheslav Tamarin
 Author-email: vyacheslav.tamarin@yandex.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

