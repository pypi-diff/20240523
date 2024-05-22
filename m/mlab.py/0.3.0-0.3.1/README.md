# Comparing `tmp/mlab_py-0.3.0.tar.gz` & `tmp/mlab_py-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlab_py-0.3.0.tar", last modified: Wed May 22 23:12:32 2024, max compression
+gzip compressed data, was "mlab_py-0.3.1.tar", last modified: Wed May 22 23:50:58 2024, max compression
```

## Comparing `mlab_py-0.3.0.tar` & `mlab_py-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:12:32.201881 mlab_py-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-22 23:12:32.201881 mlab_py-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 23:12:27.000000 mlab_py-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:12:32.201881 mlab_py-0.3.0/mlab.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-22 23:12:32.000000 mlab_py-0.3.0/mlab.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-22 23:12:32.000000 mlab_py-0.3.0/mlab.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 23:12:32.000000 mlab_py-0.3.0/mlab.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 23:12:32.000000 mlab_py-0.3.0/mlab.py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:12:32.201881 mlab_py-0.3.0/pymlab/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-22 23:12:27.000000 mlab_py-0.3.0/pymlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-22 23:12:27.000000 mlab_py-0.3.0/pymlab/__test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-22 23:12:27.000000 mlab_py-0.3.0/pymlab/__train.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-22 23:12:27.000000 mlab_py-0.3.0/pymlab/__utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 23:12:32.201881 mlab_py-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-22 23:12:27.000000 mlab_py-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:50:58.429010 mlab_py-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-22 23:50:58.429010 mlab_py-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 23:50:54.000000 mlab_py-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:50:58.429010 mlab_py-0.3.1/mlab.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-22 23:50:58.000000 mlab_py-0.3.1/mlab.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-22 23:50:58.000000 mlab_py-0.3.1/mlab.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 23:50:58.000000 mlab_py-0.3.1/mlab.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 23:50:58.000000 mlab_py-0.3.1/mlab.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:50:58.429010 mlab_py-0.3.1/pymlab/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-22 23:50:54.000000 mlab_py-0.3.1/pymlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-22 23:50:54.000000 mlab_py-0.3.1/pymlab/m_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-22 23:50:54.000000 mlab_py-0.3.1/pymlab/m_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-22 23:50:54.000000 mlab_py-0.3.1/pymlab/m_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 23:50:58.429010 mlab_py-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-22 23:50:54.000000 mlab_py-0.3.1/setup.py
```

### Comparing `mlab_py-0.3.0/PKG-INFO` & `mlab_py-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlab.py
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python packages for mlab ecosystem
 Author: Kelvin Nketia-Achiampong
 Author-email: <disal.bot@gmlcv.onmicrosoft.com>
 Keywords: python,mlab,mlab ecosystem,mlab python packages
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlab_py-0.3.0/mlab.py.egg-info/PKG-INFO` & `mlab_py-0.3.1/mlab.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlab.py
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python packages for mlab ecosystem
 Author: Kelvin Nketia-Achiampong
 Author-email: <disal.bot@gmlcv.onmicrosoft.com>
 Keywords: python,mlab,mlab ecosystem,mlab python packages
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlab_py-0.3.0/pymlab/__test.py` & `mlab_py-0.3.1/pymlab/m_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 Do not edit this file
 This is the file that will be used to test your model
 """
-import asyncio
 import os
 import json
 import requests
-from __utils import fetch_parameters,run_in_dir
+from .m_utils import fetch_parameters,run_in_dir
 
 class TestResults:
     """Results of testing."""
     def __init__(self, metrics: dict[str, float], files: [], predictions: []):
         self.metrics = metrics
         self.files = files
         self.predictions = predictions
```

### Comparing `mlab_py-0.3.0/pymlab/__train.py` & `mlab_py-0.3.1/pymlab/m_train.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import asyncio
 import os
 import json
 import requests
-from __utils import fetch_parameters,run_in_dir
+from .m_utils import fetch_parameters,run_in_dir
 
 class TrainResults:
     """Results of training."""
     def __init__(self, pretrained_model: str, metrics: dict[str, float], files: []):
         self.pretrained_model = pretrained_model
         self.metrics = metrics
         self.files = files
 
 def train(
     model_path:str,
     result_id: str,
     API_URL: str,
-) -> TrainResults:
+):
     """
     Train a model
     This function will provide the dataset path, parameters and result_id
     and will return the results of training.
     """
 
     parameters = fetch_parameters(config_path=f"{model_path}/config.txt")
```

### Comparing `mlab_py-0.3.0/pymlab/__utils.py` & `mlab_py-0.3.1/pymlab/m_utils.py`

 * *Files identical despite different names*

### Comparing `mlab_py-0.3.0/setup.py` & `mlab_py-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.3.0'
+VERSION = '0.3.1'
 DESCRIPTION = 'Python packages for mlab ecosystem'
 LONG_DESCRIPTION = 'This package contains supports the core functionalities for the mlab ecosystem'
 
 # Setting up
 setup(
     name="mlab.py",
     version=VERSION,
```

