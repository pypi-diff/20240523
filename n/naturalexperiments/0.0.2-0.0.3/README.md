# Comparing `tmp/naturalexperiments-0.0.2.tar.gz` & `tmp/naturalexperiments-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naturalexperiments-0.0.2.tar", last modified: Thu May 23 00:37:44 2024, max compression
+gzip compressed data, was "naturalexperiments-0.0.3.tar", last modified: Thu May 23 11:51:10 2024, max compression
```

## Comparing `naturalexperiments-0.0.2.tar` & `naturalexperiments-0.0.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 00:37:44.224516 naturalexperiments-0.0.2/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1071 2024-05-22 20:16:39.000000 naturalexperiments-0.0.2/LICENSE
--rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-23 00:37:44.224299 naturalexperiments-0.0.2/PKG-INFO
--rw-r--r--   0 rtealwitter   (501) staff       (20)      101 2024-05-22 20:16:39.000000 naturalexperiments-0.0.2/README.md
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 00:37:44.217719 naturalexperiments-0.0.2/naturalexperiments/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      120 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)    11440 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/benchmark.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 00:37:44.218430 naturalexperiments-0.0.2/naturalexperiments/data/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      338 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/data/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 00:37:44.218644 naturalexperiments-0.0.2/naturalexperiments/data/acic/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1988 2024-05-22 21:47:02.000000 naturalexperiments-0.0.2/naturalexperiments/data/acic/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 00:37:44.218865 naturalexperiments-0.0.2/naturalexperiments/data/ihdp/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1553 2024-05-23 00:23:10.000000 naturalexperiments-0.0.2/naturalexperiments/data/ihdp/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 00:37:44.219090 naturalexperiments-0.0.2/naturalexperiments/data/jobs/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1356 2024-05-23 00:17:37.000000 naturalexperiments-0.0.2/naturalexperiments/data/jobs/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 00:37:44.219406 naturalexperiments-0.0.2/naturalexperiments/data/news/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1395 2024-05-23 00:31:31.000000 naturalexperiments-0.0.2/naturalexperiments/data/news/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 00:37:44.219949 naturalexperiments-0.0.2/naturalexperiments/data/rorco/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1215 2024-05-22 21:42:52.000000 naturalexperiments-0.0.2/naturalexperiments/data/rorco/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)    15535 2024-05-22 21:34:07.000000 naturalexperiments-0.0.2/naturalexperiments/data/rorco/rorco_preprocess.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 00:37:44.220263 naturalexperiments-0.0.2/naturalexperiments/data/twins/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1716 2024-05-23 00:20:25.000000 naturalexperiments-0.0.2/naturalexperiments/data/twins/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     5996 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/data_summary.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 00:37:44.223782 naturalexperiments-0.0.2/naturalexperiments/estimators/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1545 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      683 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/catenet.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      136 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/direct_difference.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      330 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/direct_prediction.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1750 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/double_double.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      629 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/doubly_robust.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      138 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/horvitz_thompson.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      234 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/learned_direct.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1419 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/off_policy.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      488 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/propensity_stratification.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      436 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/regression_discontinuity.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      872 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/estimators/tmle.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     3438 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/model.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      473 2024-05-23 00:24:10.000000 naturalexperiments-0.0.2/naturalexperiments/test.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1662 2024-05-22 20:42:14.000000 naturalexperiments-0.0.2/naturalexperiments/utils.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 00:37:44.223996 naturalexperiments-0.0.2/naturalexperiments.egg-info/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-23 00:37:44.000000 naturalexperiments-0.0.2/naturalexperiments.egg-info/PKG-INFO
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1285 2024-05-23 00:37:44.000000 naturalexperiments-0.0.2/naturalexperiments.egg-info/SOURCES.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)        1 2024-05-23 00:37:44.000000 naturalexperiments-0.0.2/naturalexperiments.egg-info/dependency_links.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)       19 2024-05-23 00:37:44.000000 naturalexperiments-0.0.2/naturalexperiments.egg-info/top_level.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)       38 2024-05-23 00:37:44.224569 naturalexperiments-0.0.2/setup.cfg
--rw-r--r--   0 rtealwitter   (501) staff       (20)      719 2024-05-23 00:36:11.000000 naturalexperiments-0.0.2/setup.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:51:10.747783 naturalexperiments-0.0.3/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1071 2024-05-22 20:16:39.000000 naturalexperiments-0.0.3/LICENSE
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-23 11:51:10.747352 naturalexperiments-0.0.3/PKG-INFO
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      101 2024-05-22 20:16:39.000000 naturalexperiments-0.0.3/README.md
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:51:10.740476 naturalexperiments-0.0.3/naturalexperiments/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      120 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)    11440 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/benchmark.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:51:10.741175 naturalexperiments-0.0.3/naturalexperiments/data/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      338 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/data/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:51:10.741402 naturalexperiments-0.0.3/naturalexperiments/data/acic/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1988 2024-05-22 21:47:02.000000 naturalexperiments-0.0.3/naturalexperiments/data/acic/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:51:10.741635 naturalexperiments-0.0.3/naturalexperiments/data/ihdp/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1553 2024-05-23 00:23:10.000000 naturalexperiments-0.0.3/naturalexperiments/data/ihdp/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:51:10.741855 naturalexperiments-0.0.3/naturalexperiments/data/jobs/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1356 2024-05-23 00:17:37.000000 naturalexperiments-0.0.3/naturalexperiments/data/jobs/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:51:10.742089 naturalexperiments-0.0.3/naturalexperiments/data/news/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1429 2024-05-23 11:48:46.000000 naturalexperiments-0.0.3/naturalexperiments/data/news/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:51:10.742595 naturalexperiments-0.0.3/naturalexperiments/data/rorco/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1215 2024-05-22 21:42:52.000000 naturalexperiments-0.0.3/naturalexperiments/data/rorco/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)    15535 2024-05-22 21:34:07.000000 naturalexperiments-0.0.3/naturalexperiments/data/rorco/rorco_preprocess.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:51:10.742908 naturalexperiments-0.0.3/naturalexperiments/data/twins/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1716 2024-05-23 00:20:25.000000 naturalexperiments-0.0.3/naturalexperiments/data/twins/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     5996 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/data_summary.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:51:10.746595 naturalexperiments-0.0.3/naturalexperiments/estimators/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1545 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      683 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/catenet.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      136 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/direct_difference.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      330 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/direct_prediction.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1750 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/double_double.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      629 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/doubly_robust.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      138 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/horvitz_thompson.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      234 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/learned_direct.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1419 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/off_policy.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      488 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/propensity_stratification.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      436 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/regression_discontinuity.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      872 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/estimators/tmle.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     3438 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/model.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      473 2024-05-23 11:45:15.000000 naturalexperiments-0.0.3/naturalexperiments/test.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1662 2024-05-22 20:42:14.000000 naturalexperiments-0.0.3/naturalexperiments/utils.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 11:51:10.746850 naturalexperiments-0.0.3/naturalexperiments.egg-info/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-23 11:51:10.000000 naturalexperiments-0.0.3/naturalexperiments.egg-info/PKG-INFO
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1285 2024-05-23 11:51:10.000000 naturalexperiments-0.0.3/naturalexperiments.egg-info/SOURCES.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)        1 2024-05-23 11:51:10.000000 naturalexperiments-0.0.3/naturalexperiments.egg-info/dependency_links.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)       19 2024-05-23 11:51:10.000000 naturalexperiments-0.0.3/naturalexperiments.egg-info/top_level.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)       38 2024-05-23 11:51:10.747841 naturalexperiments-0.0.3/setup.cfg
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      719 2024-05-23 11:50:25.000000 naturalexperiments-0.0.3/setup.py
```

### Comparing `naturalexperiments-0.0.2/LICENSE` & `naturalexperiments-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.2/PKG-INFO` & `naturalexperiments-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalexperiments
-Version: 0.0.2
+Version: 0.0.3
 Summary: Estimators and datasets for treatment effect estimation in natural experiments.
 Home-page: https://github.com/rtealwitter/naturalexperiments
 Author: R. Teal Witter
 Author-email: rtealwitter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `naturalexperiments-0.0.2/naturalexperiments/benchmark.py` & `naturalexperiments-0.0.3/naturalexperiments/benchmark.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.2/naturalexperiments/data/acic/__init__.py` & `naturalexperiments-0.0.3/naturalexperiments/data/acic/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.2/naturalexperiments/data/ihdp/__init__.py` & `naturalexperiments-0.0.3/naturalexperiments/data/ihdp/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.2/naturalexperiments/data/jobs/__init__.py` & `naturalexperiments-0.0.3/naturalexperiments/data/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.2/naturalexperiments/data/news/__init__.py` & `naturalexperiments-0.0.3/naturalexperiments/data/news/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,14 @@
     return X, y, z
 
 
 if __name__ == '__main__':
     # Read filenames in csv folder
     try:
         for seed_num in range(1, 51):
-            filename = __file__.replace('__init__.py', f'topic_doc_mean_n5000_k3477_seed_{seed_num}.csv.y')
+            filename = __file__.replace('__init__.py', f'csv/topic_doc_mean_n5000_k3477_seed_{seed_num}.csv.y')
             data = pd.read_csv(filename, header=None)
-            data.to_csv(__file__.replace('__init__.py', f'news_data_{seed_num}.csv'))
-    except:
+            data.to_csv(__file__.replace('__init__.py', f'news_data_{seed_num}.csv'), index=False, header=False)
+    except FileNotFoundError:
         print('Please download the news data from https://shubhanshu.com/awesome-causality/#data')
-        print('Extract the zip file and place all csv files that end in .csv.y in the news folder')
+        print('Extract the zip file and place the csv folder in the news directory')
         print('Then run this script again')
```

### Comparing `naturalexperiments-0.0.2/naturalexperiments/data/rorco/__init__.py` & `naturalexperiments-0.0.3/naturalexperiments/data/rorco/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.2/naturalexperiments/data/rorco/rorco_preprocess.py` & `naturalexperiments-0.0.3/naturalexperiments/data/rorco/rorco_preprocess.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.2/naturalexperiments/data/twins/__init__.py` & `naturalexperiments-0.0.3/naturalexperiments/data/twins/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.2/naturalexperiments/data_summary.py` & `naturalexperiments-0.0.3/naturalexperiments/data_summary.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.2/naturalexperiments/estimators/__init__.py` & `naturalexperiments-0.0.3/naturalexperiments/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.2/naturalexperiments/estimators/catenet.py` & `naturalexperiments-0.0.3/naturalexperiments/estimators/catenet.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.2/naturalexperiments/estimators/double_double.py` & `naturalexperiments-0.0.3/naturalexperiments/estimators/double_double.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.2/naturalexperiments/estimators/doubly_robust.py` & `naturalexperiments-0.0.3/naturalexperiments/estimators/doubly_robust.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.2/naturalexperiments/estimators/off_policy.py` & `naturalexperiments-0.0.3/naturalexperiments/estimators/off_policy.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.2/naturalexperiments/estimators/tmle.py` & `naturalexperiments-0.0.3/naturalexperiments/estimators/tmle.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.2/naturalexperiments/model.py` & `naturalexperiments-0.0.3/naturalexperiments/model.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.2/naturalexperiments/utils.py` & `naturalexperiments-0.0.3/naturalexperiments/utils.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.2/naturalexperiments.egg-info/PKG-INFO` & `naturalexperiments-0.0.3/naturalexperiments.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalexperiments
-Version: 0.0.2
+Version: 0.0.3
 Summary: Estimators and datasets for treatment effect estimation in natural experiments.
 Home-page: https://github.com/rtealwitter/naturalexperiments
 Author: R. Teal Witter
 Author-email: rtealwitter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `naturalexperiments-0.0.2/naturalexperiments.egg-info/SOURCES.txt` & `naturalexperiments-0.0.3/naturalexperiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.2/setup.py` & `naturalexperiments-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="naturalexperiments",
-    version="0.0.2",
+    version="0.0.3",
     author="R. Teal Witter",
     author_email="rtealwitter@gmail.com",
     description="Estimators and datasets for treatment effect estimation in natural experiments.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rtealwitter/naturalexperiments",
     packages=setuptools.find_packages(),
```

