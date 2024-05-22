# Comparing `tmp/mlab_py-0.3.1.tar.gz` & `tmp/mlab.py-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlab_py-0.3.1.tar", last modified: Wed May 22 23:50:58 2024, max compression
+gzip compressed data, was "mlab.py-0.3.2.tar", last modified: Wed May 22 23:56:58 2024, max compression
```

## Comparing `mlab_py-0.3.1.tar` & `mlab.py-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:50:58.429010 mlab_py-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-22 23:50:58.429010 mlab_py-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 23:50:54.000000 mlab_py-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:50:58.429010 mlab_py-0.3.1/mlab.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-22 23:50:58.000000 mlab_py-0.3.1/mlab.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-22 23:50:58.000000 mlab_py-0.3.1/mlab.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 23:50:58.000000 mlab_py-0.3.1/mlab.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 23:50:58.000000 mlab_py-0.3.1/mlab.py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:50:58.429010 mlab_py-0.3.1/pymlab/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-22 23:50:54.000000 mlab_py-0.3.1/pymlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-22 23:50:54.000000 mlab_py-0.3.1/pymlab/m_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-22 23:50:54.000000 mlab_py-0.3.1/pymlab/m_train.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-22 23:50:54.000000 mlab_py-0.3.1/pymlab/m_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 23:50:58.429010 mlab_py-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-22 23:50:54.000000 mlab_py-0.3.1/setup.py
+drwxr-xr-x   0 disal      (501) staff       (20)        0 2024-05-22 23:56:58.322013 mlab.py-0.3.2/
+-rw-r--r--   0 disal      (501) staff       (20)      563 2024-05-22 23:56:58.320757 mlab.py-0.3.2/PKG-INFO
+-rw-r--r--   0 disal      (501) staff       (20)        8 2024-05-22 22:06:07.000000 mlab.py-0.3.2/README.md
+drwxr-xr-x   0 disal      (501) staff       (20)        0 2024-05-22 23:56:58.317196 mlab.py-0.3.2/mlab.py.egg-info/
+-rw-r--r--   0 disal      (501) staff       (20)      563 2024-05-22 23:56:58.000000 mlab.py-0.3.2/mlab.py.egg-info/PKG-INFO
+-rw-r--r--   0 disal      (501) staff       (20)      229 2024-05-22 23:56:58.000000 mlab.py-0.3.2/mlab.py.egg-info/SOURCES.txt
+-rw-r--r--   0 disal      (501) staff       (20)        1 2024-05-22 23:56:58.000000 mlab.py-0.3.2/mlab.py.egg-info/dependency_links.txt
+-rw-r--r--   0 disal      (501) staff       (20)        7 2024-05-22 23:56:58.000000 mlab.py-0.3.2/mlab.py.egg-info/top_level.txt
+drwxr-xr-x   0 disal      (501) staff       (20)        0 2024-05-22 23:56:58.319605 mlab.py-0.3.2/pymlab/
+-rw-r--r--   0 disal      (501) staff       (20)      183 2024-05-22 23:41:07.000000 mlab.py-0.3.2/pymlab/__init__.py
+-rw-r--r--   0 disal      (501) staff       (20)     2628 2024-05-22 23:41:33.000000 mlab.py-0.3.2/pymlab/m_test.py
+-rw-r--r--   0 disal      (501) staff       (20)     2426 2024-05-22 23:42:11.000000 mlab.py-0.3.2/pymlab/m_train.py
+-rw-r--r--   0 disal      (501) staff       (20)     2291 2024-05-22 23:00:18.000000 mlab.py-0.3.2/pymlab/m_utils.py
+-rw-r--r--   0 disal      (501) staff       (20)      317 2024-05-22 23:56:13.000000 mlab.py-0.3.2/pyproject.toml
+-rw-r--r--   0 disal      (501) staff       (20)       38 2024-05-22 23:56:58.322281 mlab.py-0.3.2/setup.cfg
+-rw-r--r--   0 disal      (501) staff       (20)     1108 2024-05-22 23:56:56.000000 mlab.py-0.3.2/setup.py
```

### Comparing `mlab_py-0.3.1/PKG-INFO` & `mlab.py-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlab.py
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python packages for mlab ecosystem
 Author: Kelvin Nketia-Achiampong
 Author-email: <disal.bot@gmlcv.onmicrosoft.com>
 Keywords: python,mlab,mlab ecosystem,mlab python packages
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlab_py-0.3.1/mlab.py.egg-info/PKG-INFO` & `mlab.py-0.3.2/mlab.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlab.py
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python packages for mlab ecosystem
 Author: Kelvin Nketia-Achiampong
 Author-email: <disal.bot@gmlcv.onmicrosoft.com>
 Keywords: python,mlab,mlab ecosystem,mlab python packages
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlab_py-0.3.1/pymlab/m_test.py` & `mlab.py-0.3.2/pymlab/m_test.py`

 * *Files identical despite different names*

### Comparing `mlab_py-0.3.1/pymlab/m_train.py` & `mlab.py-0.3.2/pymlab/m_train.py`

 * *Files identical despite different names*

### Comparing `mlab_py-0.3.1/pymlab/m_utils.py` & `mlab.py-0.3.2/pymlab/m_utils.py`

 * *Files identical despite different names*

### Comparing `mlab_py-0.3.1/setup.py` & `mlab.py-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.3.1'
+VERSION = '0.3.2'
 DESCRIPTION = 'Python packages for mlab ecosystem'
 LONG_DESCRIPTION = 'This package contains supports the core functionalities for the mlab ecosystem'
 
 # Setting up
 setup(
     name="mlab.py",
     version=VERSION,
```

