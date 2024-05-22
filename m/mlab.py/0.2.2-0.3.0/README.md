# Comparing `tmp/mlab_py-0.2.2.tar.gz` & `tmp/mlab_py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlab_py-0.2.2.tar", last modified: Wed May 22 22:19:22 2024, max compression
+gzip compressed data, was "mlab_py-0.3.0.tar", last modified: Wed May 22 23:12:32 2024, max compression
```

## Comparing `mlab_py-0.2.2.tar` & `mlab_py-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:22.243049 mlab_py-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-22 22:19:22.243049 mlab_py-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 22:19:18.000000 mlab_py-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:22.243049 mlab_py-0.2.2/mlab.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-22 22:19:22.000000 mlab_py-0.2.2/mlab.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-22 22:19:22.000000 mlab_py-0.2.2/mlab.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:19:22.000000 mlab_py-0.2.2/mlab.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 22:19:22.000000 mlab_py-0.2.2/mlab.py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:22.239049 mlab_py-0.2.2/pymlab/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-22 22:19:18.000000 mlab_py-0.2.2/pymlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-22 22:19:18.000000 mlab_py-0.2.2/pymlab/__test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-22 22:19:18.000000 mlab_py-0.2.2/pymlab/__train.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-22 22:19:18.000000 mlab_py-0.2.2/pymlab/__utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 22:19:22.243049 mlab_py-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-22 22:19:18.000000 mlab_py-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:12:32.201881 mlab_py-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-22 23:12:32.201881 mlab_py-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 23:12:27.000000 mlab_py-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:12:32.201881 mlab_py-0.3.0/mlab.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-22 23:12:32.000000 mlab_py-0.3.0/mlab.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-22 23:12:32.000000 mlab_py-0.3.0/mlab.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 23:12:32.000000 mlab_py-0.3.0/mlab.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 23:12:32.000000 mlab_py-0.3.0/mlab.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:12:32.201881 mlab_py-0.3.0/pymlab/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-22 23:12:27.000000 mlab_py-0.3.0/pymlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-22 23:12:27.000000 mlab_py-0.3.0/pymlab/__test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-22 23:12:27.000000 mlab_py-0.3.0/pymlab/__train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-22 23:12:27.000000 mlab_py-0.3.0/pymlab/__utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 23:12:32.201881 mlab_py-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-22 23:12:27.000000 mlab_py-0.3.0/setup.py
```

### Comparing `mlab_py-0.2.2/PKG-INFO` & `mlab_py-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlab.py
-Version: 0.2.2
+Version: 0.3.0
 Summary: Python packages for mlab ecosystem
 Author: Kelvin Nketia-Achiampong
 Author-email: <disal.bot@gmlcv.onmicrosoft.com>
 Keywords: python,mlab,mlab ecosystem,mlab python packages
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlab_py-0.2.2/mlab.py.egg-info/PKG-INFO` & `mlab_py-0.3.0/mlab.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlab.py
-Version: 0.2.2
+Version: 0.3.0
 Summary: Python packages for mlab ecosystem
 Author: Kelvin Nketia-Achiampong
 Author-email: <disal.bot@gmlcv.onmicrosoft.com>
 Keywords: python,mlab,mlab ecosystem,mlab python packages
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlab_py-0.2.2/pymlab/__test.py` & `mlab_py-0.3.0/pymlab/__test.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Do not edit this file
 This is the file that will be used to test your model
 """
 import asyncio
 import os
 import json
 import requests
-from __utils import fetch_parameters
+from __utils import fetch_parameters,run_in_dir
 
 class TestResults:
     """Results of testing."""
     def __init__(self, metrics: dict[str, float], files: [], predictions: []):
         self.metrics = metrics
         self.files = files
         self.predictions = predictions
@@ -48,15 +48,15 @@
 
 
             response = requests.post(API_URL+f"?error={False}", data=data, files=files,timeout=120, verify=False)
 
             if response.status_code != 200:
                 raise requests.HTTPError(f"Error uploading results. Status code: {response.status_code}, error: {response.text}")
             
-        asyncio.run(main())
+        run_in_dir(model_path, [f"source {model_path}/venv/bin/activate", f"python -m asyncio.run {main()}"])
 
     except Exception as e:
         # Append error in error.txt file
         # First check if error.txt file exists
         print("Error: ", e)
         if not os.path.exists(f"{result_id}/error.txt"):
             os.mkdir(result_id)
```

### Comparing `mlab_py-0.2.2/pymlab/__train.py` & `mlab_py-0.3.0/pymlab/__train.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import os
 import json
 import requests
-from __utils import fetch_parameters
+from __utils import fetch_parameters,run_in_dir
 
 class TrainResults:
     """Results of training."""
     def __init__(self, pretrained_model: str, metrics: dict[str, float], files: []):
         self.pretrained_model = pretrained_model
         self.metrics = metrics
         self.files = files
@@ -46,15 +46,15 @@
 
 
             response = requests.post(API_URL, data=data, files=files,timeout=120, verify=False)
 
             if response.status_code != 200:
                 raise requests.HTTPError(f"Error uploading results. Status code: {response.status_code}, error: {response.text}")
 
-        asyncio.run(main())
+        run_in_dir(model_path, [f"source {model_path}/venv/bin/activate", f"python -m asyncio.run {main()}"])
     except Exception as e:
         # Append error in error.txt file
         # First check if error.txt file exists
         if not os.path.exists(f"{result_id}/error.txt"):
             os.mkdir(result_id)
             with open(f"{result_id}/error.txt", "w", encoding="utf-8") as f:
                 f.write(str(e))
```

### Comparing `mlab_py-0.2.2/pymlab/__utils.py` & `mlab_py-0.3.0/pymlab/__utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import os
+
+
 def parse_list(value):
     # Check if the value is a list
     if value.startswith('[') and value.endswith(']'):
         # Remove brackets
         value = value[1:-1]
         result = []
         nested_level = 0
@@ -56,7 +59,12 @@
                         parameters[param_name] = float(param_value)
                     elif param_type == 'bool':
                         parameters[param_name] = param_value.lower() == 'true'
                     else:
                         parameters[param_name] = str(param_value)
 
     return parameters
+
+def run_in_dir(directory: str, commands: list[str]) -> None:
+    os.chdir(directory)
+    for command in commands:
+        os.system(command)
```

### Comparing `mlab_py-0.2.2/setup.py` & `mlab_py-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.2'
+VERSION = '0.3.0'
 DESCRIPTION = 'Python packages for mlab ecosystem'
 LONG_DESCRIPTION = 'This package contains supports the core functionalities for the mlab ecosystem'
 
 # Setting up
 setup(
     name="mlab.py",
     version=VERSION,
```

