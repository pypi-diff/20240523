# Comparing `tmp/mlab.py-0.2.1.tar.gz` & `tmp/mlab_py-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlab.py-0.2.1.tar", last modified: Wed May 22 22:03:37 2024, max compression
+gzip compressed data, was "mlab_py-0.2.2.tar", last modified: Wed May 22 22:19:22 2024, max compression
```

## Comparing `mlab.py-0.2.1.tar` & `mlab_py-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 disal      (501) staff       (20)        0 2024-05-22 22:03:37.742107 mlab.py-0.2.1/
--rw-r--r--   0 disal      (501) staff       (20)      597 2024-05-22 22:03:37.741472 mlab.py-0.2.1/PKG-INFO
--rw-r--r--   0 disal      (501) staff       (20)       42 2024-05-22 21:36:06.000000 mlab.py-0.2.1/README.md
-drwxr-xr-x   0 disal      (501) staff       (20)        0 2024-05-22 22:03:37.737182 mlab.py-0.2.1/mlab.py.egg-info/
--rw-r--r--   0 disal      (501) staff       (20)      597 2024-05-22 22:03:37.000000 mlab.py-0.2.1/mlab.py.egg-info/PKG-INFO
--rw-r--r--   0 disal      (501) staff       (20)      214 2024-05-22 22:03:37.000000 mlab.py-0.2.1/mlab.py.egg-info/SOURCES.txt
--rw-r--r--   0 disal      (501) staff       (20)        1 2024-05-22 22:03:37.000000 mlab.py-0.2.1/mlab.py.egg-info/dependency_links.txt
--rw-r--r--   0 disal      (501) staff       (20)        7 2024-05-22 22:03:37.000000 mlab.py-0.2.1/mlab.py.egg-info/top_level.txt
-drwxr-xr-x   0 disal      (501) staff       (20)        0 2024-05-22 22:03:37.740341 mlab.py-0.2.1/pymlab/
--rw-r--r--   0 disal      (501) staff       (20)      102 2024-05-22 22:03:04.000000 mlab.py-0.2.1/pymlab/__init__.py
--rw-r--r--   0 disal      (501) staff       (20)     2549 2024-05-22 22:02:59.000000 mlab.py-0.2.1/pymlab/__test.py
--rw-r--r--   0 disal      (501) staff       (20)     2348 2024-05-22 22:02:54.000000 mlab.py-0.2.1/pymlab/__train.py
--rw-r--r--   0 disal      (501) staff       (20)     2138 2024-05-22 21:05:42.000000 mlab.py-0.2.1/pymlab/__utils.py
--rw-r--r--   0 disal      (501) staff       (20)       38 2024-05-22 22:03:37.742278 mlab.py-0.2.1/setup.cfg
--rw-r--r--   0 disal      (501) staff       (20)     1108 2024-05-22 22:03:24.000000 mlab.py-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:22.243049 mlab_py-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-22 22:19:22.243049 mlab_py-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 22:19:18.000000 mlab_py-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:22.243049 mlab_py-0.2.2/mlab.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-22 22:19:22.000000 mlab_py-0.2.2/mlab.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-22 22:19:22.000000 mlab_py-0.2.2/mlab.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:19:22.000000 mlab_py-0.2.2/mlab.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 22:19:22.000000 mlab_py-0.2.2/mlab.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:22.239049 mlab_py-0.2.2/pymlab/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-22 22:19:18.000000 mlab_py-0.2.2/pymlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-22 22:19:18.000000 mlab_py-0.2.2/pymlab/__test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-22 22:19:18.000000 mlab_py-0.2.2/pymlab/__train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-22 22:19:18.000000 mlab_py-0.2.2/pymlab/__utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 22:19:22.243049 mlab_py-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-22 22:19:18.000000 mlab_py-0.2.2/setup.py
```

### Comparing `mlab.py-0.2.1/PKG-INFO` & `mlab_py-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mlab.py
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python packages for mlab ecosystem
 Author: Kelvin Nketia-Achiampong
 Author-email: <disal.bot@gmlcv.onmicrosoft.com>
 Keywords: python,mlab,mlab ecosystem,mlab python packages
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
-# This is the README file for the project.
+# pymlab
```

### Comparing `mlab.py-0.2.1/mlab.py.egg-info/PKG-INFO` & `mlab_py-0.2.2/mlab.py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mlab.py
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python packages for mlab ecosystem
 Author: Kelvin Nketia-Achiampong
 Author-email: <disal.bot@gmlcv.onmicrosoft.com>
 Keywords: python,mlab,mlab ecosystem,mlab python packages
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
-# This is the README file for the project.
+# pymlab
```

### Comparing `mlab.py-0.2.1/pymlab/__test.py` & `mlab_py-0.2.2/pymlab/__test.py`

 * *Files identical despite different names*

### Comparing `mlab.py-0.2.1/pymlab/__train.py` & `mlab_py-0.2.2/pymlab/__train.py`

 * *Files identical despite different names*

### Comparing `mlab.py-0.2.1/pymlab/__utils.py` & `mlab_py-0.2.2/pymlab/__utils.py`

 * *Files identical despite different names*

### Comparing `mlab.py-0.2.1/setup.py` & `mlab_py-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 DESCRIPTION = 'Python packages for mlab ecosystem'
 LONG_DESCRIPTION = 'This package contains supports the core functionalities for the mlab ecosystem'
 
 # Setting up
 setup(
     name="mlab.py",
     version=VERSION,
```

