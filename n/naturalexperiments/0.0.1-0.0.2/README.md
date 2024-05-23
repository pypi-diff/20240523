# Comparing `tmp/naturalexperiments-0.0.1.tar.gz` & `tmp/naturalexperiments-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naturalexperiments-0.0.1.tar", last modified: Wed May 22 21:05:27 2024, max compression
+gzip compressed data, was "naturalexperiments-0.0.2.tar", last modified: Thu May 23 00:37:44 2024, max compression
```

## Comparing `naturalexperiments-0.0.1.tar` & `naturalexperiments-0.0.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-22 21:05:27.569160 naturalexperiments-0.0.1/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1071 2024-05-22 20:16:39.000000 naturalexperiments-0.0.1/LICENSE
--rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-22 21:05:27.568996 naturalexperiments-0.0.1/PKG-INFO
--rw-r--r--   0 rtealwitter   (501) staff       (20)      101 2024-05-22 20:16:39.000000 naturalexperiments-0.0.1/README.md
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-22 21:05:27.562424 naturalexperiments-0.0.1/naturalexperiments/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      120 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)    11440 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/benchmark.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-22 21:05:27.563274 naturalexperiments-0.0.1/naturalexperiments/data/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      338 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/data/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-22 21:05:27.563566 naturalexperiments-0.0.1/naturalexperiments/data/acic/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1662 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/data/acic/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-22 21:05:27.563868 naturalexperiments-0.0.1/naturalexperiments/data/ihdp/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1274 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/data/ihdp/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-22 21:05:27.564903 naturalexperiments-0.0.1/naturalexperiments/data/jobs/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1033 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/data/jobs/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-22 21:05:27.565069 naturalexperiments-0.0.1/naturalexperiments/data/news/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1101 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/data/news/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-22 21:05:27.565374 naturalexperiments-0.0.1/naturalexperiments/data/rorco/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      880 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/data/rorco/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)    15534 2024-05-22 20:54:39.000000 naturalexperiments-0.0.1/naturalexperiments/data/rorco/rorco_preprocess.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-22 21:05:27.565702 naturalexperiments-0.0.1/naturalexperiments/data/twins/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1478 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/data/twins/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     5996 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/data_summary.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-22 21:05:27.568641 naturalexperiments-0.0.1/naturalexperiments/estimators/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1545 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/estimators/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      683 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/estimators/catenet.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      136 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/estimators/direct_difference.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      330 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/estimators/direct_prediction.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1750 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/estimators/double_double.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      629 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/estimators/doubly_robust.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      138 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/estimators/horvitz_thompson.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      234 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/estimators/learned_direct.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1419 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/estimators/off_policy.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      488 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/estimators/propensity_stratification.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      436 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/estimators/regression_discontinuity.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      872 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/estimators/tmle.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     3438 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/model.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      297 2024-05-22 20:57:12.000000 naturalexperiments-0.0.1/naturalexperiments/test.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1662 2024-05-22 20:42:14.000000 naturalexperiments-0.0.1/naturalexperiments/utils.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-22 21:05:27.568822 naturalexperiments-0.0.1/naturalexperiments.egg-info/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-22 21:05:27.000000 naturalexperiments-0.0.1/naturalexperiments.egg-info/PKG-INFO
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1285 2024-05-22 21:05:27.000000 naturalexperiments-0.0.1/naturalexperiments.egg-info/SOURCES.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)        1 2024-05-22 21:05:27.000000 naturalexperiments-0.0.1/naturalexperiments.egg-info/dependency_links.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)       19 2024-05-22 21:05:27.000000 naturalexperiments-0.0.1/naturalexperiments.egg-info/top_level.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)       38 2024-05-22 21:05:27.569198 naturalexperiments-0.0.1/setup.cfg
--rw-r--r--   0 rtealwitter   (501) staff       (20)      719 2024-05-22 20:20:14.000000 naturalexperiments-0.0.1/setup.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 00:37:44.224516 naturalexperiments-0.0.2/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1071 2024-05-22 20:16:39.000000 naturalexperiments-0.0.2/LICENSE
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-23 00:37:44.224299 naturalexperiments-0.0.2/PKG-INFO
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      101 2024-05-22 20:16:39.000000 naturalexperiments-0.0.2/README.md
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 00:37:44.217719 naturalexperiments-0.0.2/naturalexperiments/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      120 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)    11440 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/benchmark.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 00:37:44.218430 naturalexperiments-0.0.2/naturalexperiments/data/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      338 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/data/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 00:37:44.218644 naturalexperiments-0.0.2/naturalexperiments/data/acic/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1988 2024-05-22 21:47:02.000000 naturalexperiments-0.0.2/naturalexperiments/data/acic/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 00:37:44.218865 naturalexperiments-0.0.2/naturalexperiments/data/ihdp/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1553 2024-05-23 00:23:10.000000 naturalexperiments-0.0.2/naturalexperiments/data/ihdp/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 00:37:44.219090 naturalexperiments-0.0.2/naturalexperiments/data/jobs/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1356 2024-05-23 00:17:37.000000 naturalexperiments-0.0.2/naturalexperiments/data/jobs/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 00:37:44.219406 naturalexperiments-0.0.2/naturalexperiments/data/news/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1395 2024-05-23 00:31:31.000000 naturalexperiments-0.0.2/naturalexperiments/data/news/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 00:37:44.219949 naturalexperiments-0.0.2/naturalexperiments/data/rorco/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1215 2024-05-22 21:42:52.000000 naturalexperiments-0.0.2/naturalexperiments/data/rorco/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)    15535 2024-05-22 21:34:07.000000 naturalexperiments-0.0.2/naturalexperiments/data/rorco/rorco_preprocess.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 00:37:44.220263 naturalexperiments-0.0.2/naturalexperiments/data/twins/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1716 2024-05-23 00:20:25.000000 naturalexperiments-0.0.2/naturalexperiments/data/twins/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     5996 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/data_summary.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 00:37:44.223782 naturalexperiments-0.0.2/naturalexperiments/estimators/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1545 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      683 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/catenet.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      136 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/direct_difference.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      330 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/direct_prediction.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1750 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/double_double.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      629 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/doubly_robust.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      138 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/horvitz_thompson.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      234 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/learned_direct.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1419 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/off_policy.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      488 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/propensity_stratification.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      436 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/regression_discontinuity.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      872 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/tmle.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     3438 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/model.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      473 2024-05-23 00:24:10.000000 naturalexperiments-0.0.2/naturalexperiments/test.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1662 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/utils.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 00:37:44.223996 naturalexperiments-0.0.2/naturalexperiments.egg-info/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-23 00:37:44.000000 naturalexperiments-0.0.2/naturalexperiments.egg-info/PKG-INFO
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1285 2024-05-23 00:37:44.000000 naturalexperiments-0.0.2/naturalexperiments.egg-info/SOURCES.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)        1 2024-05-23 00:37:44.000000 naturalexperiments-0.0.2/naturalexperiments.egg-info/dependency_links.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)       19 2024-05-23 00:37:44.000000 naturalexperiments-0.0.2/naturalexperiments.egg-info/top_level.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)       38 2024-05-23 00:37:44.224569 naturalexperiments-0.0.2/setup.cfg
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      719 2024-05-23 00:36:11.000000 naturalexperiments-0.0.2/setup.py
```

### Comparing `naturalexperiments-0.0.1/LICENSE` & `naturalexperiments-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.1/PKG-INFO` & `naturalexperiments-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalexperiments
-Version: 0.0.1
+Version: 0.0.2
 Summary: Estimators and datasets for treatment effect estimation in natural experiments.
 Home-page: https://github.com/rtealwitter/naturalexperiments
 Author: R. Teal Witter
 Author-email: rtealwitter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `naturalexperiments-0.0.1/naturalexperiments/benchmark.py` & `naturalexperiments-0.0.2/naturalexperiments/benchmark.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.1/naturalexperiments/data/acic/__init__.py` & `naturalexperiments-0.0.2/naturalexperiments/data/acic/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 import pandas as pd
 import os
 import pickle as pkl
 import numpy as np
+import requests
 
 def load_acic():
     # Print absolute path
     # Get absolute path to this file
-    filename = __file__.replace('__init__.py', 'acic_data.pkl')
+    filename = __file__.replace('__init__.py', 'acic_data.csv')
 
-    data = pkl.load(open(filename, 'rb'))
+    if not os.path.exists(filename):
+        print('Downloading ACIC data...')
+        # Download the data 
+        url = 'https://raw.githubusercontent.com/rtealwitter/naturalexperiments/main/naturalexperiments/data/acic/acic_data.csv'
+
+        r = requests.get(url)
+        open(filename, 'wb').write(r.content)
+    
+    data = pd.read_csv(filename)
 
     # Remove string columns
     data = data.select_dtypes(include = ['int16', 'int32', 'int64', 'float16', 'float32', 'float64'])
     data = data.astype(np.float32)
 
     # Set data type of columns to float32
```

### Comparing `naturalexperiments-0.0.1/naturalexperiments/data/ihdp/__init__.py` & `naturalexperiments-0.0.2/naturalexperiments/data/ihdp/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import os
 import pickle as pkl
 import pandas as pd
+import requests
 
 def load_ihdp(num=1):
     assert num in range(1,11), "Invalid dataset number"
-    filename = __file__.replace('__init__.py', 'ihdp_data.pkl')
+    filename = __file__.replace('__init__.py', f'ihdp_data_{num}.csv')
 
-    datasets = pkl.load(open(filename, 'rb'))
+    if not os.path.exists(filename):
+        print('Downloading IHDP data...')
+        url = f'https://raw.githubusercontent.com/rtealwitter/naturalexperiments/main/naturalexperiments/data/ihdp/ihdp_data_{num}.csv'
 
-    data = datasets[num-1]
+        r = requests.get(url)
+        open(filename, 'wb').write(r.content)
+    
+    data = pd.read_csv(filename)
 
     z = data['treatment'].values
 
     y = pd.DataFrame({
         'y1' : data['y_cfactual'].values * z + data['y_factual'].values * (1-z),
         'y0' : data['y_cfactual'].values * (1-z) + data['y_factual'].values * z,
     }, dtype=float)
```

### Comparing `naturalexperiments-0.0.1/naturalexperiments/data/jobs/__init__.py` & `naturalexperiments-0.0.2/naturalexperiments/data/jobs/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 import pickle as pkl
 import pandas as pd
 import os
+import requests
 
 def load_jobs():
-    filename = __file__.replace('__init__.py', 'jobs_data.pkl')
+    filename = __file__.replace('__init__.py', 'jobs_data.csv')
 
-    data = pkl.load(open(filename, 'rb'))
+    if not os.path.exists(filename):
+        print('Downloading Jobs data...')
+        # Download the data 
+        url = 'https://raw.githubusercontent.com/rtealwitter/naturalexperiments/main/naturalexperiments/data/jobs/jobs_data.csv'
+
+        r = requests.get(url)
+        open(filename, 'wb').write(r.content)
+
+    data = pd.read_csv(filename) 
 
     z = data['treat'].values
     y = pd.DataFrame({
         'y1' : data['re78'].values * z,
         'y0' : data['re78'].values * (1-z)
     }, dtype=float)
```

### Comparing `naturalexperiments-0.0.1/naturalexperiments/data/news/__init__.py` & `naturalexperiments-0.0.2/naturalexperiments/data/news/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 import pickle as pkl
 import pandas as pd
 import os
+import requests
 
 def load_news(num=1):
     assert num in range(1, 51), 'Invalid dataset number'
-    filename = __file__.replace('__init__.py', 'news_data.pkl')
+    filename = __file__.replace('__init__.py', f'news_data_{num}.csv')
 
-    datasets = pkl.load(open(filename, 'rb'))
+    if not os.path.exists(filename):
+        print('Downloading News data...')
+        # Download the data 
+        url = 'https://raw.githubusercontent.com/rtealwitter/naturalexperiments/main/naturalexperiments/data/news/news_data.csv'
 
-    data = datasets[num-1]
+        r = requests.get(url)
+        open(filename, 'wb').write(r.content)
+
+    data = pd.read_csv(filename, header=None)
 
     z = data[0].values
 
     y = pd.DataFrame({
         'y1' : data[4].values * z,
         'y0' : data[4].values * (1-z)
     }, dtype=float)
@@ -20,19 +27,16 @@
     X = data.drop(columns=[0,4]).values
 
     return X, y, z
 
 
 if __name__ == '__main__':
     # Read filenames in csv folder
-    if os.path.exists('csv'):    
-        datasets = []
-        filenames = os.listdir('csv')
-        for filename in filenames:
-            if filename.endswith('.csv.y'):
-                data = pd.read_csv('csv/' + filename, header=None)
-                datasets += [data]
-        pkl.dump(datasets, open('news_data.pkl', 'wb'))
-    else:
+    try:
+        for seed_num in range(1, 51):
+            filename = __file__.replace('__init__.py', f'topic_doc_mean_n5000_k3477_seed_{seed_num}.csv.y')
+            data = pd.read_csv(filename, header=None)
+            data.to_csv(__file__.replace('__init__.py', f'news_data_{seed_num}.csv'))
+    except:
         print('Please download the news data from https://shubhanshu.com/awesome-causality/#data')
-        print('Extract the zip file and place the csv folder in the data folder')
+        print('Extract the zip file and place all csv files that end in .csv.y in the news folder')
         print('Then run this script again')
```

### Comparing `naturalexperiments-0.0.1/naturalexperiments/data/rorco/rorco_preprocess.py` & `naturalexperiments-0.0.2/naturalexperiments/data/rorco/rorco_preprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,8 +347,9 @@
 
     clinics_geom = load_clinic_data()
 
     school_geom = assign_visits_to_schools(school_geom, clinics_geom)
 
     school_geom = add_proximity(school_geom)
 
-    pickle.dump(school_geom, open('rorco_data.pkl', 'wb'))
+    # Write to csv
+    school_geom.to_csv('rorco_data.csv')
```

### Comparing `naturalexperiments-0.0.1/naturalexperiments/data/twins/__init__.py` & `naturalexperiments-0.0.2/naturalexperiments/data/twins/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import os
 import pickle as pkl
 import pandas as pd
 
 def load_twins():
-    filename = __file__.replace('__init__.py', 'twins_data.pkl')
+    filename = __file__.replace('__init__.py', 'twins_data.csv')
 
-    data = pkl.load(open(filename, 'rb'))
+    if not os.path.exists(filename):
+        print('Downloading twins data...')
+        # Download the data
+        url = 'https://raw.githubusercontent.com/rtealwitter/naturalexperiments/main/naturalexperiments/data/twins/twins_data.csv'
+
+    data = pd.read_csv(filename)
 
     # Drop cols with too many missing values
     nan_cols = data.isnull().sum() > 10000
     nan_cols = nan_cols[nan_cols].index
     data = data.drop(columns=nan_cols).dropna()
 
     z = None
@@ -17,15 +22,15 @@
     y = pd.DataFrame({
         'y1' : data['mort_1'].values,
         'y0' : data['mort_0'].values
     })
 
     cols_to_drop = [x for x in data.columns if '_0' in x or '_1' in x]
 
-    X = data.drop(columns=cols_to_drop)
+    X = data.drop(columns=cols_to_drop).values
 
     return X, y, z 
 
 if __name__ == '__main__':
     if not os.path.exists('twins_data.pkl'):
         url_weight = "https://raw.githubusercontent.com/AMLab-Amsterdam/CEVAE/9081f863e24ce21bd34c8d6a41bf0edc7d1b65dd/datasets/TWINS/twin_pairs_T_3years_samesex.csv"
```

### Comparing `naturalexperiments-0.0.1/naturalexperiments/data_summary.py` & `naturalexperiments-0.0.2/naturalexperiments/data_summary.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.1/naturalexperiments/estimators/__init__.py` & `naturalexperiments-0.0.2/naturalexperiments/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.1/naturalexperiments/estimators/catenet.py` & `naturalexperiments-0.0.2/naturalexperiments/estimators/catenet.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.1/naturalexperiments/estimators/double_double.py` & `naturalexperiments-0.0.2/naturalexperiments/estimators/double_double.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.1/naturalexperiments/estimators/doubly_robust.py` & `naturalexperiments-0.0.2/naturalexperiments/estimators/doubly_robust.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.1/naturalexperiments/estimators/off_policy.py` & `naturalexperiments-0.0.2/naturalexperiments/estimators/off_policy.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.1/naturalexperiments/estimators/tmle.py` & `naturalexperiments-0.0.2/naturalexperiments/estimators/tmle.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.1/naturalexperiments/model.py` & `naturalexperiments-0.0.2/naturalexperiments/model.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.1/naturalexperiments/utils.py` & `naturalexperiments-0.0.2/naturalexperiments/utils.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.1/naturalexperiments.egg-info/PKG-INFO` & `naturalexperiments-0.0.2/naturalexperiments.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalexperiments
-Version: 0.0.1
+Version: 0.0.2
 Summary: Estimators and datasets for treatment effect estimation in natural experiments.
 Home-page: https://github.com/rtealwitter/naturalexperiments
 Author: R. Teal Witter
 Author-email: rtealwitter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `naturalexperiments-0.0.1/naturalexperiments.egg-info/SOURCES.txt` & `naturalexperiments-0.0.2/naturalexperiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.1/setup.py` & `naturalexperiments-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="naturalexperiments",
-    version="0.0.1",
+    version="0.0.2",
     author="R. Teal Witter",
     author_email="rtealwitter@gmail.com",
     description="Estimators and datasets for treatment effect estimation in natural experiments.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rtealwitter/naturalexperiments",
     packages=setuptools.find_packages(),
```

