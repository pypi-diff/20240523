# Comparing `tmp/fuzzyset2-0.2.3.tar.gz` & `tmp/fuzzyset2-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzyset2-0.2.3.tar", last modified: Wed Mar  6 07:47:23 2024, max compression
+gzip compressed data, was "fuzzyset2-0.2.4.tar", last modified: Thu May 23 08:51:01 2024, max compression
```

## Comparing `fuzzyset2-0.2.3.tar` & `fuzzyset2-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 07:47:23.268430 fuzzyset2-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-06 07:47:10.000000 fuzzyset2-0.2.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-06 07:47:10.000000 fuzzyset2-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-03-06 07:47:23.268430 fuzzyset2-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-03-06 07:47:10.000000 fuzzyset2-0.2.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)   311326 2024-03-06 07:47:10.000000 fuzzyset2-0.2.3/cities.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 07:47:23.264430 fuzzyset2-0.2.3/fuzzyset/
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-03-06 07:47:10.000000 fuzzyset2-0.2.3/fuzzyset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-03-06 07:47:10.000000 fuzzyset2-0.2.3/fuzzyset/cfuzzyset.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 07:47:23.268430 fuzzyset2-0.2.3/fuzzyset2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-03-06 07:47:23.000000 fuzzyset2-0.2.3/fuzzyset2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-06 07:47:23.000000 fuzzyset2-0.2.3/fuzzyset2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 07:47:23.000000 fuzzyset2-0.2.3/fuzzyset2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-06 07:47:23.000000 fuzzyset2-0.2.3/fuzzyset2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-06 07:47:23.000000 fuzzyset2-0.2.3/fuzzyset2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-03-06 07:47:10.000000 fuzzyset2-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 07:47:23.268430 fuzzyset2-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-03-06 07:47:10.000000 fuzzyset2-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 07:47:23.268430 fuzzyset2-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-06 07:47:10.000000 fuzzyset2-0.2.3/tests/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-03-06 07:47:10.000000 fuzzyset2-0.2.3/tests/performance.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-06 07:47:10.000000 fuzzyset2-0.2.3/tests/profile_fuzzyset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-03-06 07:47:10.000000 fuzzyset2-0.2.3/tests/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:51:01.939084 fuzzyset2-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-23 08:50:50.000000 fuzzyset2-0.2.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-23 08:50:50.000000 fuzzyset2-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-05-23 08:51:01.939084 fuzzyset2-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-23 08:50:50.000000 fuzzyset2-0.2.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   311326 2024-05-23 08:50:50.000000 fuzzyset2-0.2.4/cities.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:51:01.939084 fuzzyset2-0.2.4/fuzzyset/
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-23 08:50:50.000000 fuzzyset2-0.2.4/fuzzyset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-23 08:50:50.000000 fuzzyset2-0.2.4/fuzzyset/cfuzzyset.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:51:01.939084 fuzzyset2-0.2.4/fuzzyset2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-05-23 08:51:01.000000 fuzzyset2-0.2.4/fuzzyset2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-23 08:51:01.000000 fuzzyset2-0.2.4/fuzzyset2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 08:51:01.000000 fuzzyset2-0.2.4/fuzzyset2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 08:51:01.000000 fuzzyset2-0.2.4/fuzzyset2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 08:51:01.000000 fuzzyset2-0.2.4/fuzzyset2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-23 08:50:50.000000 fuzzyset2-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 08:51:01.943084 fuzzyset2-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-23 08:50:50.000000 fuzzyset2-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:51:01.939084 fuzzyset2-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-23 08:50:50.000000 fuzzyset2-0.2.4/tests/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-23 08:50:50.000000 fuzzyset2-0.2.4/tests/performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-23 08:50:50.000000 fuzzyset2-0.2.4/tests/profile_fuzzyset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-23 08:50:50.000000 fuzzyset2-0.2.4/tests/test_simple.py
```

### Comparing `fuzzyset2-0.2.3/CHANGELOG.md` & `fuzzyset2-0.2.4/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 ## Changelog
 
+### [0.2.4] - 2024-05-23
+- fixed inconsistency between cfuzzyset and fuzzyset implementation (#30)
+- update ciwheelbuild to 2.18.1 
+- bump version of actions to latest versions
+
 ### [0.2.3] - 2024-03-05
 - add support to build wheels for py3.12 (macosx, win, linux)
 - drop support for py3.7 (EOL)
 - update ciwheelbuild from 2.12 to 2.16.5
 - bump version of actions to latest versions
 
 ### [0.2.2] - 2023-01-17
```

### Comparing `fuzzyset2-0.2.3/PKG-INFO` & `fuzzyset2-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzyset2
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple python fuzzyset implementation.
 Home-page: https://github.com/alpae/fuzzyset/
 Author: Michael Axiak, Adrian Altenhoff
 Author-email: adrian.altenhoff@inf.ethz.ch
 License: BSD
 Keywords: fuzzyset fuzzy data structure
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fuzzyset2-0.2.3/README.rst` & `fuzzyset2-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `fuzzyset2-0.2.3/cities.gz` & `fuzzyset2-0.2.4/cities.gz`

 * *Files identical despite different names*

### Comparing `fuzzyset2-0.2.3/fuzzyset/__init__.py` & `fuzzyset2-0.2.4/fuzzyset/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import math
 import operator
 import collections
 from rapidfuzz.distance import Levenshtein
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 __version_info__ = tuple(__version__.split("."))
 
 _non_word_re = re.compile(r'[^\w, ]+')
 
 __all__ = ('FuzzySet',)
```

### Comparing `fuzzyset2-0.2.3/fuzzyset/cfuzzyset.pyx` & `fuzzyset2-0.2.4/fuzzyset/cfuzzyset.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
             return [(score, self.exact_set[value])
                     for score, value in results
                     if score >= score_threshold]
         else:
             score_threshold = results[0][0] * self.rel_sim_cutoff
             return [(score / norm, self.exact_set[value])
                     for score, value in results
-                    if score == score_threshold]
+                    if score >= score_threshold]
 
     def __len__(self):
         return len(self.exact_set)
 
     def __nonzero__(self):
         return bool(self.exact_set)
```

### Comparing `fuzzyset2-0.2.3/fuzzyset2.egg-info/PKG-INFO` & `fuzzyset2-0.2.4/fuzzyset2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzyset2
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple python fuzzyset implementation.
 Home-page: https://github.com/alpae/fuzzyset/
 Author: Michael Axiak, Adrian Altenhoff
 Author-email: adrian.altenhoff@inf.ethz.ch
 License: BSD
 Keywords: fuzzyset fuzzy data structure
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fuzzyset2-0.2.3/pyproject.toml` & `fuzzyset2-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fuzzyset2-0.2.3/setup.py` & `fuzzyset2-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `fuzzyset2-0.2.3/tests/performance.py` & `fuzzyset2-0.2.4/tests/performance.py`

 * *Files identical despite different names*

### Comparing `fuzzyset2-0.2.3/tests/profile_fuzzyset.py` & `fuzzyset2-0.2.4/tests/profile_fuzzyset.py`

 * *Files identical despite different names*

### Comparing `fuzzyset2-0.2.3/tests/test_simple.py` & `fuzzyset2-0.2.4/tests/test_simple.py`

 * *Files identical despite different names*

