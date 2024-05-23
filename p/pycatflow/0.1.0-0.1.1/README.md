# Comparing `tmp/pycatflow-0.1.0.tar.gz` & `tmp/pycatflow-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatflow-0.1.0.tar", last modified: Thu May 23 19:50:40 2024, max compression
+gzip compressed data, was "pycatflow-0.1.1.tar", last modified: Thu May 23 19:59:03 2024, max compression
```

## Comparing `pycatflow-0.1.0.tar` & `pycatflow-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 bumatic    (501) staff       (20)        0 2024-05-23 19:50:40.580853 pycatflow-0.1.0/
--rw-rw-r--   0 bumatic    (501) staff       (20)     1077 2021-10-03 11:41:14.000000 pycatflow-0.1.0/LICENSE
--rw-r--r--   0 bumatic    (501) staff       (20)     3302 2024-05-23 19:50:40.564371 pycatflow-0.1.0/PKG-INFO
--rw-rw-r--   0 bumatic    (501) staff       (20)     2844 2021-10-03 11:41:14.000000 pycatflow-0.1.0/README.md
-drwxr-xr-x   0 bumatic    (501) staff       (20)        0 2024-05-23 19:50:40.522210 pycatflow-0.1.0/pycatflow/
--rw-rw-r--   0 bumatic    (501) staff       (20)       40 2021-10-03 11:41:14.000000 pycatflow-0.1.0/pycatflow/__init__.py
--rw-rw-r--   0 bumatic    (501) staff       (20)     9068 2021-10-03 11:41:14.000000 pycatflow-0.1.0/pycatflow/input.py
--rw-rw-r--   0 bumatic    (501) staff       (20)    27937 2021-10-03 11:41:14.000000 pycatflow-0.1.0/pycatflow/viz.py
-drwxr-xr-x   0 bumatic    (501) staff       (20)        0 2024-05-23 19:50:40.562580 pycatflow-0.1.0/pycatflow.egg-info/
--rw-r--r--   0 bumatic    (501) staff       (20)     3302 2024-05-23 19:50:40.000000 pycatflow-0.1.0/pycatflow.egg-info/PKG-INFO
--rw-r--r--   0 bumatic    (501) staff       (20)      263 2024-05-23 19:50:40.000000 pycatflow-0.1.0/pycatflow.egg-info/SOURCES.txt
--rw-r--r--   0 bumatic    (501) staff       (20)        1 2024-05-23 19:50:40.000000 pycatflow-0.1.0/pycatflow.egg-info/dependency_links.txt
--rw-r--r--   0 bumatic    (501) staff       (20)       23 2024-05-23 19:50:40.000000 pycatflow-0.1.0/pycatflow.egg-info/requires.txt
--rw-r--r--   0 bumatic    (501) staff       (20)       10 2024-05-23 19:50:40.000000 pycatflow-0.1.0/pycatflow.egg-info/top_level.txt
--rw-rw-r--   0 bumatic    (501) staff       (20)      108 2021-10-03 11:41:14.000000 pycatflow-0.1.0/pyproject.toml
--rw-r--r--   0 bumatic    (501) staff       (20)       38 2024-05-23 19:50:40.581160 pycatflow-0.1.0/setup.cfg
--rw-rw-r--   0 bumatic    (501) staff       (20)      788 2024-05-23 19:43:31.000000 pycatflow-0.1.0/setup.py
+drwxr-xr-x   0 bumatic    (501) staff       (20)        0 2024-05-23 19:59:03.403694 pycatflow-0.1.1/
+-rw-rw-r--   0 bumatic    (501) staff       (20)     1077 2021-10-03 11:41:14.000000 pycatflow-0.1.1/LICENSE
+-rw-r--r--   0 bumatic    (501) staff       (20)     3302 2024-05-23 19:59:03.399579 pycatflow-0.1.1/PKG-INFO
+-rw-rw-r--   0 bumatic    (501) staff       (20)     2844 2021-10-03 11:41:14.000000 pycatflow-0.1.1/README.md
+drwxr-xr-x   0 bumatic    (501) staff       (20)        0 2024-05-23 19:59:03.341055 pycatflow-0.1.1/pycatflow/
+-rw-rw-r--   0 bumatic    (501) staff       (20)       40 2021-10-03 11:41:14.000000 pycatflow-0.1.1/pycatflow/__init__.py
+-rw-rw-r--   0 bumatic    (501) staff       (20)     9068 2021-10-03 11:41:14.000000 pycatflow-0.1.1/pycatflow/input.py
+-rw-rw-r--   0 bumatic    (501) staff       (20)    27937 2021-10-03 11:41:14.000000 pycatflow-0.1.1/pycatflow/viz.py
+drwxr-xr-x   0 bumatic    (501) staff       (20)        0 2024-05-23 19:59:03.395072 pycatflow-0.1.1/pycatflow.egg-info/
+-rw-r--r--   0 bumatic    (501) staff       (20)     3302 2024-05-23 19:59:03.000000 pycatflow-0.1.1/pycatflow.egg-info/PKG-INFO
+-rw-r--r--   0 bumatic    (501) staff       (20)      263 2024-05-23 19:59:03.000000 pycatflow-0.1.1/pycatflow.egg-info/SOURCES.txt
+-rw-r--r--   0 bumatic    (501) staff       (20)        1 2024-05-23 19:59:03.000000 pycatflow-0.1.1/pycatflow.egg-info/dependency_links.txt
+-rw-r--r--   0 bumatic    (501) staff       (20)       23 2024-05-23 19:59:03.000000 pycatflow-0.1.1/pycatflow.egg-info/requires.txt
+-rw-r--r--   0 bumatic    (501) staff       (20)       10 2024-05-23 19:59:03.000000 pycatflow-0.1.1/pycatflow.egg-info/top_level.txt
+-rw-rw-r--   0 bumatic    (501) staff       (20)      108 2021-10-03 11:41:14.000000 pycatflow-0.1.1/pyproject.toml
+-rw-r--r--   0 bumatic    (501) staff       (20)       38 2024-05-23 19:59:03.404068 pycatflow-0.1.1/setup.cfg
+-rw-rw-r--   0 bumatic    (501) staff       (20)      788 2024-05-23 19:58:25.000000 pycatflow-0.1.1/setup.py
```

### Comparing `pycatflow-0.1.0/LICENSE` & `pycatflow-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycatflow-0.1.0/PKG-INFO` & `pycatflow-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatflow
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool for visualizing categorical data over time.
 Home-page: https://github.com/bumatic/PyCatFlow
 Author: Marcus Burkhardt
 Author-email: marcus.burkhardt@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pycatflow-0.1.0/README.md` & `pycatflow-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pycatflow-0.1.0/pycatflow/input.py` & `pycatflow-0.1.1/pycatflow/input.py`

 * *Files identical despite different names*

### Comparing `pycatflow-0.1.0/pycatflow/viz.py` & `pycatflow-0.1.1/pycatflow/viz.py`

 * *Files identical despite different names*

### Comparing `pycatflow-0.1.0/pycatflow.egg-info/PKG-INFO` & `pycatflow-0.1.1/pycatflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatflow
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool for visualizing categorical data over time.
 Home-page: https://github.com/bumatic/PyCatFlow
 Author: Marcus Burkhardt
 Author-email: marcus.burkhardt@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pycatflow-0.1.0/setup.py` & `pycatflow-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pycatflow", 
-    version="0.1.0",
+    version="0.1.1",
     author="Marcus Burkhardt",
     author_email="marcus.burkhardt@gmail.com",
     description="A tool for visualizing categorical data over time.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bumatic/PyCatFlow",
     license="MIT",
```

