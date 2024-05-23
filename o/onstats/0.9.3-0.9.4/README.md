# Comparing `tmp/onstats-0.9.3.tar.gz` & `tmp/onstats-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onstats-0.9.3.tar", max compression
+gzip compressed data, was "onstats-0.9.4.tar", max compression
```

## Comparing `onstats-0.9.3.tar` & `onstats-0.9.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1901 2024-04-25 22:39:39.392368 onstats-0.9.3/README.md
--rw-r--r--   0        0        0        0 2024-04-25 18:47:55.240859 onstats-0.9.3/onstats/__init__.py
--rw-r--r--   0        0        0     7290 2024-04-25 22:40:38.136637 onstats-0.9.3/onstats/stats.py
--rw-r--r--   0        0        0     1375 2024-04-25 22:39:57.944453 onstats-0.9.3/onstats/util.py
--rw-r--r--   0        0        0      782 2024-04-25 22:41:16.880813 onstats-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 onstats-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     2368 2024-05-23 18:06:31.003253 onstats-0.9.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 18:47:55.240859 onstats-0.9.4/onstats/__init__.py
+-rw-r--r--   0        0        0     7188 2024-05-23 18:06:31.003253 onstats-0.9.4/onstats/stats.py
+-rw-r--r--   0        0        0     1387 2024-05-23 18:06:31.007253 onstats-0.9.4/onstats/util.py
+-rw-r--r--   0        0        0      920 2024-05-23 18:06:31.007253 onstats-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     3016 1970-01-01 00:00:00.000000 onstats-0.9.4/PKG-INFO
```

### Comparing `onstats-0.9.3/README.md` & `onstats-0.9.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: onstats
+Version: 0.9.4
+Summary: Online stats in python, based in generators with send
+Home-page: https://github.com/PabloRuizCuevas/onstats
+Author: Pablo Ruiz
+Author-email: pablo.r.c@live.com
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Project-URL: Repository, https://github.com/PabloRuizCuevas/onstats
+Description-Content-Type: text/markdown
+
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Tests Status](./reports/coverage/coverage-badge.svg?dummy=8484744)](./reports/junit/report.html)
 
 ## Generators Based Online Statistics
 
 This package implement online statistics written using python generators, with the only depencency of numpy.
@@ -19,33 +36,67 @@
 > pip install onstats
 
 ## How to use:
 
 Import the window / rolling statistic you want to compute and send the values to it:
 
 ```python
->>>  from onstats import ma # moving average
+>>>  from onstats.stats import ma # moving average
+>>>  from onstats.util import send
 
 >>>  gma = ma(2)  # with window 2
 >>>  gma.send(3)
 3
-
 >>>  gma.send(5)
 4
 >>>  gma.send(5)
 5
 ```
 
 If w = 0 the window is infinitelly large , we will compute the normal average.
 
+You can also feed all the iterator directly:
+
+
+```python
+>>>  gma = ma(2)  # with window 2
+>>>  send(gma, [3,5,5])
+5
+```
+
+Or as an iterator
+
+```python
+
+>>>  gma = ma(2)  # with window 2
+>>>  for d in isend(gma, [3,5,5]):
+>>>     print(d)
+3
+4
+5
+```
+
+You can also pass 2d np.arrays:
+
+```python
+
+>>>  gma = ma(2)  # with window 2
+>>>  for d in isend(gma, np.array([[0,0],[1,2],[1,4]])):
+>>>     print(d)
+[0,0]
+[0.5,1]
+[1,3]
+```
+
+
 ## Supported Stats:
 
 | rolling   | window | infinite | Ddoff | Description                |
 |-----------|--------|----------|-------|----------------------------|
 | ma        | ✅     | ✅       |       | Moving Average             |
 | ema       |        | ✅       |       | Exponential Moving Average |
 | var       | ✅     | ✅       | ✅    | Variance                   |
 | ath       |        | ✅       |       | All Time High              |
 | wsum      | ✅     | ✅       |       | Windowed Sum               |
 | cov_xy    | ✅     |          | ✅    | Covariance                 |
 | corr_xy   | ✅     |          | ✅    | Correlation                |
-| auto_corr | ✅     |          | ✅    | Correlation                |
+| auto_corr | ✅     |          | ✅    | Auto Correlation           |
```

### Comparing `onstats-0.9.3/onstats/stats.py` & `onstats-0.9.4/onstats/stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from typing import Callable, Deque, Generator, TypeVar
+from typing import Any, Callable, Deque, Generator, TypeVar
 from collections import deque
 import numpy as np
 
-from onstats.util import consumer
+from .util import consumer
 
 
 T = TypeVar("T", np.ndarray, float)
 
 GenStat = Generator[T, T, None]
 GenStats = list[GenStat]
 TupleGenStat = Generator[T, tuple[T, T], None]
@@ -179,32 +179,25 @@
     x_delay = delay(time)
     x = yield 0.0
     while True:
         x = yield corr.send((x, x_delay.send(x)))
 
 
 @consumer
-def delay(periods: int) -> GenStat:
+def delay(periods: int, default: Any = 0) -> GenStat:
     """Delays the iterator"""
     deq: Deque = deque()
-    deq.append((yield 0))
+    deq.append((yield default))
     for _ in range(periods):
-        deq.append((yield 0))
+        deq.append((yield default))
     while True:
         deq.append((yield deq.popleft()))
 
 
 @consumer
-def delay_it(periods: int, gen: Generator) -> GenStat:
-    for _ in range(periods):
-        yield 0
-    yield from gen
-
-
-@consumer
 def ema(alpha: float | None = None, com: float | None = None, halflife: float | None = None) -> GenStat:
     """
     TODO implement as well adjusted version based on https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.ewm.html
     """
     if alpha is None:
         if com is not None:
             alpha = 2 / (com + 1)
@@ -262,7 +255,8 @@
         last = yield (last - m)
     while True:
         if count % sample_freq == 0:
             m, v = avg_g.send(last), var_g.send(last)
             s_var = np.sqrt(v)
         last = yield (last - m) / s_var
         count += 1
+
```

### Comparing `onstats-0.9.3/onstats/util.py` & `onstats-0.9.4/onstats/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Callable, Generator, Iterable, Iterator
 
 
-def consumer(func):
+def consumer(func: Callable):
     """avoid priming the generator"""
 
     def wrapper(*args, **kw):
         gen = func(*args, **kw)
         next(gen)
         return gen
 
@@ -42,7 +42,9 @@
 
 def msend(data: Any, *generators: Generator) -> list[Generator]:
     return [gen.send(data) for gen in generators]
 
 
 def msendg(data: Iterator, *generators: Generator) -> Generator[list[Generator], None, None]:
     return (msend(d, *generators) for d in data)
+
+
```

### Comparing `onstats-0.9.3/pyproject.toml` & `onstats-0.9.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 [tool.poetry]
 name = "onstats"
-version = "0.9.3"
+version = "0.9.4"
 description = "Online stats in python, based in generators with send"
 authors = ["Pablo Ruiz <pablo.r.c@live.com>"]
 readme = "README.md"
 repository = "https://github.com/PabloRuizCuevas/onstats"
+packages = [
+    { include = "onstats" },
+]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.26.4"
-genbadge = "^1.1.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.0"
 black = "^24.2.0"
 pytest-cov = "^5.0.0"
 pandas = "^2.2.2"
 mypy = "^1.10.0"
 genbadge = {extras = ["all"], version = "^1.1.1"}
 pytest-html = "^4.1.1"
+pre-commit = "^3.7.0"
 
 [tool.black]
 line-length = 120
 
 [tool.pytest.ini_options]
 addopts = ["--import-mode=importlib",
      "--cov=src"]
@@ -31,8 +34,12 @@
 testpaths =['tests']
 
 
 [tool.mypy]
 exclude = [
     '^onstats/tests/.',
 ]
-ignore_missing_imports = true
+ignore_missing_imports = true
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `onstats-0.9.3/PKG-INFO` & `onstats-0.9.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: onstats
-Version: 0.9.3
-Summary: Online stats in python, based in generators with send
-Home-page: https://github.com/PabloRuizCuevas/onstats
-Author: Pablo Ruiz
-Author-email: pablo.r.c@live.com
-Requires-Python: >=3.9,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: genbadge (>=1.1.1,<2.0.0)
-Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Project-URL: Repository, https://github.com/PabloRuizCuevas/onstats
-Description-Content-Type: text/markdown
-
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Tests Status](./reports/coverage/coverage-badge.svg?dummy=8484744)](./reports/junit/report.html)
 
 ## Generators Based Online Statistics
 
 This package implement online statistics written using python generators, with the only depencency of numpy.
@@ -37,33 +19,67 @@
 > pip install onstats
 
 ## How to use:
 
 Import the window / rolling statistic you want to compute and send the values to it:
 
 ```python
->>>  from onstats import ma # moving average
+>>>  from onstats.stats import ma # moving average
+>>>  from onstats.util import send
 
 >>>  gma = ma(2)  # with window 2
 >>>  gma.send(3)
 3
-
 >>>  gma.send(5)
 4
 >>>  gma.send(5)
 5
 ```
 
 If w = 0 the window is infinitelly large , we will compute the normal average.
 
+You can also feed all the iterator directly:
+
+
+```python
+>>>  gma = ma(2)  # with window 2
+>>>  send(gma, [3,5,5])
+5
+```
+
+Or as an iterator
+
+```python
+
+>>>  gma = ma(2)  # with window 2
+>>>  for d in isend(gma, [3,5,5]):
+>>>     print(d)
+3
+4
+5
+```
+
+You can also pass 2d np.arrays:
+
+```python
+
+>>>  gma = ma(2)  # with window 2
+>>>  for d in isend(gma, np.array([[0,0],[1,2],[1,4]])):
+>>>     print(d)
+[0,0]
+[0.5,1]
+[1,3]
+```
+
+
 ## Supported Stats:
 
 | rolling   | window | infinite | Ddoff | Description                |
 |-----------|--------|----------|-------|----------------------------|
 | ma        | ✅     | ✅       |       | Moving Average             |
 | ema       |        | ✅       |       | Exponential Moving Average |
 | var       | ✅     | ✅       | ✅    | Variance                   |
 | ath       |        | ✅       |       | All Time High              |
 | wsum      | ✅     | ✅       |       | Windowed Sum               |
 | cov_xy    | ✅     |          | ✅    | Covariance                 |
 | corr_xy   | ✅     |          | ✅    | Correlation                |
-| auto_corr | ✅     |          | ✅    | Correlation                |
+| auto_corr | ✅     |          | ✅    | Auto Correlation           |
```

