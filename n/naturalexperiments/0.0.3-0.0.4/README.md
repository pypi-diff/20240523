# Comparing `tmp/naturalexperiments-0.0.3.tar.gz` & `tmp/naturalexperiments-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naturalexperiments-0.0.3.tar", last modified: Thu May 23 11:51:10 2024, max compression
+gzip compressed data, was "naturalexperiments-0.0.4.tar", last modified: Thu May 23 11:57:53 2024, max compression
```

## Comparing `naturalexperiments-0.0.3.tar` & `naturalexperiments-0.0.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:51:10.747783 naturalexperiments-0.0.3/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1071 2024-05-22 20:16:39.000000 naturalexperiments-0.0.3/LICENSE
--rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-23 11:51:10.747352 naturalexperiments-0.0.3/PKG-INFO
--rw-r--r--   0 rtealwitter   (501) staff       (20)      101 2024-05-22 20:16:39.000000 naturalexperiments-0.0.3/README.md
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:51:10.740476 naturalexperiments-0.0.3/naturalexperiments/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      120 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)    11440 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/benchmark.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:51:10.741175 naturalexperiments-0.0.3/naturalexperiments/data/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      338 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/data/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:51:10.741402 naturalexperiments-0.0.3/naturalexperiments/data/acic/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1988 2024-05-22 21:47:02.000000 naturalexperiments-0.0.3/naturalexperiments/data/acic/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:51:10.741635 naturalexperiments-0.0.3/naturalexperiments/data/ihdp/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1553 2024-05-23 00:23:10.000000 naturalexperiments-0.0.3/naturalexperiments/data/ihdp/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:51:10.741855 naturalexperiments-0.0.3/naturalexperiments/data/jobs/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1356 2024-05-23 00:17:37.000000 naturalexperiments-0.0.3/naturalexperiments/data/jobs/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:51:10.742089 naturalexperiments-0.0.3/naturalexperiments/data/news/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1429 2024-05-23 11:48:46.000000 naturalexperiments-0.0.3/naturalexperiments/data/news/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:51:10.742595 naturalexperiments-0.0.3/naturalexperiments/data/rorco/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1215 2024-05-22 21:42:52.000000 naturalexperiments-0.0.3/naturalexperiments/data/rorco/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)    15535 2024-05-22 21:34:07.000000 naturalexperiments-0.0.3/naturalexperiments/data/rorco/rorco_preprocess.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:51:10.742908 naturalexperiments-0.0.3/naturalexperiments/data/twins/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1716 2024-05-23 00:20:25.000000 naturalexperiments-0.0.3/naturalexperiments/data/twins/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     5996 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/data_summary.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:51:10.746595 naturalexperiments-0.0.3/naturalexperiments/estimators/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1545 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      683 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/catenet.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      136 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/direct_difference.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      330 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/direct_prediction.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1750 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/double_double.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      629 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/doubly_robust.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      138 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/horvitz_thompson.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      234 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/learned_direct.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1419 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/off_policy.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      488 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/propensity_stratification.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      436 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/regression_discontinuity.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      872 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/tmle.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     3438 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/model.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      473 2024-05-23 11:45:15.000000 naturalexperiments-0.0.3/naturalexperiments/test.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1662 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/utils.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:51:10.746850 naturalexperiments-0.0.3/naturalexperiments.egg-info/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-23 11:51:10.000000 naturalexperiments-0.0.3/naturalexperiments.egg-info/PKG-INFO
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1285 2024-05-23 11:51:10.000000 naturalexperiments-0.0.3/naturalexperiments.egg-info/SOURCES.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)        1 2024-05-23 11:51:10.000000 naturalexperiments-0.0.3/naturalexperiments.egg-info/dependency_links.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)       19 2024-05-23 11:51:10.000000 naturalexperiments-0.0.3/naturalexperiments.egg-info/top_level.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)       38 2024-05-23 11:51:10.747841 naturalexperiments-0.0.3/setup.cfg
--rw-r--r--   0 rtealwitter   (501) staff       (20)      719 2024-05-23 11:50:25.000000 naturalexperiments-0.0.3/setup.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:57:53.107369 naturalexperiments-0.0.4/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1071 2024-05-22 20:16:39.000000 naturalexperiments-0.0.4/LICENSE
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-23 11:57:53.107183 naturalexperiments-0.0.4/PKG-INFO
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      101 2024-05-22 20:16:39.000000 naturalexperiments-0.0.4/README.md
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:57:53.101127 naturalexperiments-0.0.4/naturalexperiments/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      120 2024-05-22 20:42:14.000000 naturalexperiments-0.0.4/naturalexperiments/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)    11440 2024-05-22 20:42:14.000000 naturalexperiments-0.0.4/naturalexperiments/benchmark.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:57:53.101856 naturalexperiments-0.0.4/naturalexperiments/data/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      338 2024-05-22 20:42:14.000000 naturalexperiments-0.0.4/naturalexperiments/data/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:57:53.102081 naturalexperiments-0.0.4/naturalexperiments/data/acic/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1988 2024-05-22 21:47:02.000000 naturalexperiments-0.0.4/naturalexperiments/data/acic/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:57:53.102296 naturalexperiments-0.0.4/naturalexperiments/data/ihdp/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1553 2024-05-23 00:23:10.000000 naturalexperiments-0.0.4/naturalexperiments/data/ihdp/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:57:53.102506 naturalexperiments-0.0.4/naturalexperiments/data/jobs/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1356 2024-05-23 00:17:37.000000 naturalexperiments-0.0.4/naturalexperiments/data/jobs/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:57:53.102737 naturalexperiments-0.0.4/naturalexperiments/data/news/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1436 2024-05-23 11:56:32.000000 naturalexperiments-0.0.4/naturalexperiments/data/news/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:57:53.103233 naturalexperiments-0.0.4/naturalexperiments/data/rorco/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1215 2024-05-22 21:42:52.000000 naturalexperiments-0.0.4/naturalexperiments/data/rorco/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)    15535 2024-05-22 21:34:07.000000 naturalexperiments-0.0.4/naturalexperiments/data/rorco/rorco_preprocess.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:57:53.103478 naturalexperiments-0.0.4/naturalexperiments/data/twins/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1716 2024-05-23 00:20:25.000000 naturalexperiments-0.0.4/naturalexperiments/data/twins/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     5996 2024-05-22 20:42:14.000000 naturalexperiments-0.0.4/naturalexperiments/data_summary.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:57:53.106672 naturalexperiments-0.0.4/naturalexperiments/estimators/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1545 2024-05-22 20:42:14.000000 naturalexperiments-0.0.4/naturalexperiments/estimators/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      683 2024-05-22 20:42:14.000000 naturalexperiments-0.0.4/naturalexperiments/estimators/catenet.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      136 2024-05-22 20:42:14.000000 naturalexperiments-0.0.4/naturalexperiments/estimators/direct_difference.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      330 2024-05-22 20:42:14.000000 naturalexperiments-0.0.4/naturalexperiments/estimators/direct_prediction.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1750 2024-05-22 20:42:14.000000 naturalexperiments-0.0.4/naturalexperiments/estimators/double_double.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      629 2024-05-22 20:42:14.000000 naturalexperiments-0.0.4/naturalexperiments/estimators/doubly_robust.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      138 2024-05-22 20:42:14.000000 naturalexperiments-0.0.4/naturalexperiments/estimators/horvitz_thompson.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      234 2024-05-22 20:42:14.000000 naturalexperiments-0.0.4/naturalexperiments/estimators/learned_direct.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1419 2024-05-22 20:42:14.000000 naturalexperiments-0.0.4/naturalexperiments/estimators/off_policy.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      488 2024-05-22 20:42:14.000000 naturalexperiments-0.0.4/naturalexperiments/estimators/propensity_stratification.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      436 2024-05-22 20:42:14.000000 naturalexperiments-0.0.4/naturalexperiments/estimators/regression_discontinuity.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      872 2024-05-22 20:42:14.000000 naturalexperiments-0.0.4/naturalexperiments/estimators/tmle.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     3438 2024-05-22 20:42:14.000000 naturalexperiments-0.0.4/naturalexperiments/model.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      473 2024-05-23 11:45:15.000000 naturalexperiments-0.0.4/naturalexperiments/test.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1662 2024-05-22 20:42:14.000000 naturalexperiments-0.0.4/naturalexperiments/utils.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:57:53.106872 naturalexperiments-0.0.4/naturalexperiments.egg-info/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-23 11:57:53.000000 naturalexperiments-0.0.4/naturalexperiments.egg-info/PKG-INFO
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1285 2024-05-23 11:57:53.000000 naturalexperiments-0.0.4/naturalexperiments.egg-info/SOURCES.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)        1 2024-05-23 11:57:53.000000 naturalexperiments-0.0.4/naturalexperiments.egg-info/dependency_links.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)       19 2024-05-23 11:57:53.000000 naturalexperiments-0.0.4/naturalexperiments.egg-info/top_level.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)       38 2024-05-23 11:57:53.107420 naturalexperiments-0.0.4/setup.cfg
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      719 2024-05-23 11:57:06.000000 naturalexperiments-0.0.4/setup.py
```

### Comparing `naturalexperiments-0.0.3/LICENSE` & `naturalexperiments-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.3/PKG-INFO` & `naturalexperiments-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalexperiments
-Version: 0.0.3
+Version: 0.0.4
 Summary: Estimators and datasets for treatment effect estimation in natural experiments.
 Home-page: https://github.com/rtealwitter/naturalexperiments
 Author: R. Teal Witter
 Author-email: rtealwitter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `naturalexperiments-0.0.3/naturalexperiments/benchmark.py` & `naturalexperiments-0.0.4/naturalexperiments/benchmark.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.3/naturalexperiments/data/acic/__init__.py` & `naturalexperiments-0.0.4/naturalexperiments/data/acic/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.3/naturalexperiments/data/ihdp/__init__.py` & `naturalexperiments-0.0.4/naturalexperiments/data/ihdp/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.3/naturalexperiments/data/jobs/__init__.py` & `naturalexperiments-0.0.4/naturalexperiments/data/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.3/naturalexperiments/data/news/__init__.py` & `naturalexperiments-0.0.4/naturalexperiments/data/news/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def load_news(num=1):
     assert num in range(1, 51), 'Invalid dataset number'
     filename = __file__.replace('__init__.py', f'news_data_{num}.csv')
 
     if not os.path.exists(filename):
         print('Downloading News data...')
         # Download the data 
-        url = 'https://raw.githubusercontent.com/rtealwitter/naturalexperiments/main/naturalexperiments/data/news/news_data.csv'
+        url = f'https://raw.githubusercontent.com/rtealwitter/naturalexperiments/main/naturalexperiments/data/news/news_data_{num}.csv'
 
         r = requests.get(url)
         open(filename, 'wb').write(r.content)
 
     data = pd.read_csv(filename, header=None)
 
     z = data[0].values
```

### Comparing `naturalexperiments-0.0.3/naturalexperiments/data/rorco/__init__.py` & `naturalexperiments-0.0.4/naturalexperiments/data/rorco/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.3/naturalexperiments/data/rorco/rorco_preprocess.py` & `naturalexperiments-0.0.4/naturalexperiments/data/rorco/rorco_preprocess.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.3/naturalexperiments/data/twins/__init__.py` & `naturalexperiments-0.0.4/naturalexperiments/data/twins/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.3/naturalexperiments/data_summary.py` & `naturalexperiments-0.0.4/naturalexperiments/data_summary.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.3/naturalexperiments/estimators/__init__.py` & `naturalexperiments-0.0.4/naturalexperiments/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.3/naturalexperiments/estimators/catenet.py` & `naturalexperiments-0.0.4/naturalexperiments/estimators/catenet.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.3/naturalexperiments/estimators/double_double.py` & `naturalexperiments-0.0.4/naturalexperiments/estimators/double_double.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.3/naturalexperiments/estimators/doubly_robust.py` & `naturalexperiments-0.0.4/naturalexperiments/estimators/doubly_robust.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.3/naturalexperiments/estimators/off_policy.py` & `naturalexperiments-0.0.4/naturalexperiments/estimators/off_policy.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.3/naturalexperiments/estimators/tmle.py` & `naturalexperiments-0.0.4/naturalexperiments/estimators/tmle.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.3/naturalexperiments/model.py` & `naturalexperiments-0.0.4/naturalexperiments/model.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.3/naturalexperiments/utils.py` & `naturalexperiments-0.0.4/naturalexperiments/utils.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.3/naturalexperiments.egg-info/PKG-INFO` & `naturalexperiments-0.0.4/naturalexperiments.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalexperiments
-Version: 0.0.3
+Version: 0.0.4
 Summary: Estimators and datasets for treatment effect estimation in natural experiments.
 Home-page: https://github.com/rtealwitter/naturalexperiments
 Author: R. Teal Witter
 Author-email: rtealwitter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `naturalexperiments-0.0.3/naturalexperiments.egg-info/SOURCES.txt` & `naturalexperiments-0.0.4/naturalexperiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.3/setup.py` & `naturalexperiments-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="naturalexperiments",
-    version="0.0.3",
+    version="0.0.4",
     author="R. Teal Witter",
     author_email="rtealwitter@gmail.com",
     description="Estimators and datasets for treatment effect estimation in natural experiments.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rtealwitter/naturalexperiments",
     packages=setuptools.find_packages(),
```

