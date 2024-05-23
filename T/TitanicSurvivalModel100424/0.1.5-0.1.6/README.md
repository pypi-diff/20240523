# Comparing `tmp/titanicsurvivalmodel100424-0.1.5.tar.gz` & `tmp/titanicsurvivalmodel100424-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titanicsurvivalmodel100424-0.1.5.tar", last modified: Thu May 23 18:48:59 2024, max compression
+gzip compressed data, was "titanicsurvivalmodel100424-0.1.6.tar", last modified: Thu May 23 19:00:04 2024, max compression
```

## Comparing `titanicsurvivalmodel100424-0.1.5.tar` & `titanicsurvivalmodel100424-0.1.6.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 18:48:59.121671 titanicsurvivalmodel100424-0.1.5/
--rw-r--r--   0 ongzhicong   (501) staff       (20)      443 2024-05-20 06:43:12.000000 titanicsurvivalmodel100424-0.1.5/MANIFEST.in
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1138 2024-05-23 18:48:59.120746 titanicsurvivalmodel100424-0.1.5/PKG-INFO
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 18:48:59.119709 titanicsurvivalmodel100424-0.1.5/TitanicSurvivalModel100424.egg-info/
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1138 2024-05-23 18:48:59.000000 titanicsurvivalmodel100424-0.1.5/TitanicSurvivalModel100424.egg-info/PKG-INFO
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1022 2024-05-23 18:48:59.000000 titanicsurvivalmodel100424-0.1.5/TitanicSurvivalModel100424.egg-info/SOURCES.txt
--rw-r--r--   0 ongzhicong   (501) staff       (20)        1 2024-05-23 18:48:59.000000 titanicsurvivalmodel100424-0.1.5/TitanicSurvivalModel100424.egg-info/dependency_links.txt
--rw-r--r--   0 ongzhicong   (501) staff       (20)      188 2024-05-23 18:48:59.000000 titanicsurvivalmodel100424-0.1.5/TitanicSurvivalModel100424.egg-info/requires.txt
--rw-r--r--   0 ongzhicong   (501) staff       (20)       21 2024-05-23 18:48:59.000000 titanicsurvivalmodel100424-0.1.5/TitanicSurvivalModel100424.egg-info/top_level.txt
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 18:48:59.113671 titanicsurvivalmodel100424-0.1.5/classification_model/
--rw-r--r--   0 ongzhicong   (501) staff       (20)        6 2024-05-23 18:45:26.000000 titanicsurvivalmodel100424-0.1.5/classification_model/VERSION
--rw-r--r--   0 ongzhicong   (501) staff       (20)      862 2024-05-04 09:04:59.000000 titanicsurvivalmodel100424-0.1.5/classification_model/__init__.py
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 18:48:59.114469 titanicsurvivalmodel100424-0.1.5/classification_model/config/
--rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:23.000000 titanicsurvivalmodel100424-0.1.5/classification_model/config/__init__.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     2129 2024-05-20 00:42:53.000000 titanicsurvivalmodel100424-0.1.5/classification_model/config/core.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)      891 2024-05-23 10:57:47.000000 titanicsurvivalmodel100424-0.1.5/classification_model/config.yml
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 18:48:59.115014 titanicsurvivalmodel100424-0.1.5/classification_model/datasets/
--rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:51.000000 titanicsurvivalmodel100424-0.1.5/classification_model/datasets/__init__.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     2434 2024-05-17 06:12:30.000000 titanicsurvivalmodel100424-0.1.5/classification_model/pipeline.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1058 2024-05-18 07:00:50.000000 titanicsurvivalmodel100424-0.1.5/classification_model/predict.py
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 18:48:59.116620 titanicsurvivalmodel100424-0.1.5/classification_model/processing/
--rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:58.000000 titanicsurvivalmodel100424-0.1.5/classification_model/processing/__init__.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1751 2024-05-20 06:30:05.000000 titanicsurvivalmodel100424-0.1.5/classification_model/processing/data_manager.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     3575 2024-05-17 06:26:00.000000 titanicsurvivalmodel100424-0.1.5/classification_model/processing/features.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1763 2024-05-18 07:29:10.000000 titanicsurvivalmodel100424-0.1.5/classification_model/processing/validation.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)      831 2024-05-17 06:24:46.000000 titanicsurvivalmodel100424-0.1.5/classification_model/train_pipeline.py
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 18:48:59.117382 titanicsurvivalmodel100424-0.1.5/classification_model/trained_models/
--rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:09:07.000000 titanicsurvivalmodel100424-0.1.5/classification_model/trained_models/__init__.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     4110 2024-05-23 18:47:07.000000 titanicsurvivalmodel100424-0.1.5/classification_model/trained_models/classification_model_output_v0.1.5.pkl
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1914 2023-04-19 02:15:38.000000 titanicsurvivalmodel100424-0.1.5/pyproject.toml
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 18:48:59.107426 titanicsurvivalmodel100424-0.1.5/requirements/
--rw-r--r--   0 ongzhicong   (501) staff       (20)      225 2024-05-17 09:24:00.000000 titanicsurvivalmodel100424-0.1.5/requirements/requirements.txt
--rw-r--r--   0 ongzhicong   (501) staff       (20)       65 2023-04-19 02:15:38.000000 titanicsurvivalmodel100424-0.1.5/requirements/test_requirements.txt
--rw-r--r--   0 ongzhicong   (501) staff       (20)       38 2024-05-23 18:48:59.122265 titanicsurvivalmodel100424-0.1.5/setup.cfg
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1996 2024-05-23 17:39:04.000000 titanicsurvivalmodel100424-0.1.5/setup.py
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 18:48:59.118325 titanicsurvivalmodel100424-0.1.5/tests/
--rw-r--r--   0 ongzhicong   (501) staff       (20)      680 2024-05-14 08:58:22.000000 titanicsurvivalmodel100424-0.1.5/tests/test_features.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)      855 2024-05-14 08:58:29.000000 titanicsurvivalmodel100424-0.1.5/tests/test_prediction.py
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 19:00:04.045229 titanicsurvivalmodel100424-0.1.6/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      435 2024-05-23 18:56:35.000000 titanicsurvivalmodel100424-0.1.6/MANIFEST.in
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1138 2024-05-23 19:00:04.044807 titanicsurvivalmodel100424-0.1.6/PKG-INFO
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 19:00:04.044246 titanicsurvivalmodel100424-0.1.6/TitanicSurvivalModel100424.egg-info/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1138 2024-05-23 19:00:04.000000 titanicsurvivalmodel100424-0.1.6/TitanicSurvivalModel100424.egg-info/PKG-INFO
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1062 2024-05-23 19:00:04.000000 titanicsurvivalmodel100424-0.1.6/TitanicSurvivalModel100424.egg-info/SOURCES.txt
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        1 2024-05-23 19:00:04.000000 titanicsurvivalmodel100424-0.1.6/TitanicSurvivalModel100424.egg-info/dependency_links.txt
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      188 2024-05-23 19:00:04.000000 titanicsurvivalmodel100424-0.1.6/TitanicSurvivalModel100424.egg-info/requires.txt
+-rw-r--r--   0 ongzhicong   (501) staff       (20)       21 2024-05-23 19:00:04.000000 titanicsurvivalmodel100424-0.1.6/TitanicSurvivalModel100424.egg-info/top_level.txt
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 19:00:04.038188 titanicsurvivalmodel100424-0.1.6/classification_model/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        6 2024-05-23 18:57:10.000000 titanicsurvivalmodel100424-0.1.6/classification_model/VERSION
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      862 2024-05-04 09:04:59.000000 titanicsurvivalmodel100424-0.1.6/classification_model/__init__.py
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 19:00:04.039011 titanicsurvivalmodel100424-0.1.6/classification_model/config/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:23.000000 titanicsurvivalmodel100424-0.1.6/classification_model/config/__init__.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     2129 2024-05-20 00:42:53.000000 titanicsurvivalmodel100424-0.1.6/classification_model/config/core.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      891 2024-05-23 10:57:47.000000 titanicsurvivalmodel100424-0.1.6/classification_model/config.yml
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 19:00:04.039682 titanicsurvivalmodel100424-0.1.6/classification_model/datasets/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:51.000000 titanicsurvivalmodel100424-0.1.6/classification_model/datasets/__init__.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)    61194 2024-05-23 17:47:42.000000 titanicsurvivalmodel100424-0.1.6/classification_model/datasets/train.csv
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     2434 2024-05-17 06:12:30.000000 titanicsurvivalmodel100424-0.1.6/classification_model/pipeline.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1058 2024-05-18 07:00:50.000000 titanicsurvivalmodel100424-0.1.6/classification_model/predict.py
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 19:00:04.041985 titanicsurvivalmodel100424-0.1.6/classification_model/processing/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:58.000000 titanicsurvivalmodel100424-0.1.6/classification_model/processing/__init__.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1751 2024-05-20 06:30:05.000000 titanicsurvivalmodel100424-0.1.6/classification_model/processing/data_manager.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     3575 2024-05-17 06:26:00.000000 titanicsurvivalmodel100424-0.1.6/classification_model/processing/features.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1763 2024-05-18 07:29:10.000000 titanicsurvivalmodel100424-0.1.6/classification_model/processing/validation.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      831 2024-05-17 06:24:46.000000 titanicsurvivalmodel100424-0.1.6/classification_model/train_pipeline.py
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 19:00:04.042643 titanicsurvivalmodel100424-0.1.6/classification_model/trained_models/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:09:07.000000 titanicsurvivalmodel100424-0.1.6/classification_model/trained_models/__init__.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     4110 2024-05-23 18:59:28.000000 titanicsurvivalmodel100424-0.1.6/classification_model/trained_models/classification_model_output_v0.1.6.pkl
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1914 2023-04-19 02:15:38.000000 titanicsurvivalmodel100424-0.1.6/pyproject.toml
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 19:00:04.033887 titanicsurvivalmodel100424-0.1.6/requirements/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      225 2024-05-17 09:24:00.000000 titanicsurvivalmodel100424-0.1.6/requirements/requirements.txt
+-rw-r--r--   0 ongzhicong   (501) staff       (20)       65 2023-04-19 02:15:38.000000 titanicsurvivalmodel100424-0.1.6/requirements/test_requirements.txt
+-rw-r--r--   0 ongzhicong   (501) staff       (20)       38 2024-05-23 19:00:04.045298 titanicsurvivalmodel100424-0.1.6/setup.cfg
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1996 2024-05-23 17:39:04.000000 titanicsurvivalmodel100424-0.1.6/setup.py
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 19:00:04.043705 titanicsurvivalmodel100424-0.1.6/tests/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      680 2024-05-14 08:58:22.000000 titanicsurvivalmodel100424-0.1.6/tests/test_features.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      855 2024-05-14 08:58:29.000000 titanicsurvivalmodel100424-0.1.6/tests/test_prediction.py
```

### Comparing `titanicsurvivalmodel100424-0.1.5/PKG-INFO` & `titanicsurvivalmodel100424-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanicSurvivalModel100424
-Version: 0.1.5
+Version: 0.1.6
 Summary: sample Classification model package.
 Home-page: https://github.com/zong006/model_packaging
 Author: sample_author
 Author-email: sample_email@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `titanicsurvivalmodel100424-0.1.5/TitanicSurvivalModel100424.egg-info/PKG-INFO` & `titanicsurvivalmodel100424-0.1.6/TitanicSurvivalModel100424.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanicSurvivalModel100424
-Version: 0.1.5
+Version: 0.1.6
 Summary: sample Classification model package.
 Home-page: https://github.com/zong006/model_packaging
 Author: sample_author
 Author-email: sample_email@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `titanicsurvivalmodel100424-0.1.5/TitanicSurvivalModel100424.egg-info/SOURCES.txt` & `titanicsurvivalmodel100424-0.1.6/TitanicSurvivalModel100424.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 classification_model/config.yml
 classification_model/pipeline.py
 classification_model/predict.py
 classification_model/train_pipeline.py
 classification_model/config/__init__.py
 classification_model/config/core.py
 classification_model/datasets/__init__.py
+classification_model/datasets/train.csv
 classification_model/processing/__init__.py
 classification_model/processing/data_manager.py
 classification_model/processing/features.py
 classification_model/processing/validation.py
 classification_model/trained_models/__init__.py
-classification_model/trained_models/classification_model_output_v0.1.5.pkl
+classification_model/trained_models/classification_model_output_v0.1.6.pkl
 tests/test_features.py
 tests/test_prediction.py
```

### Comparing `titanicsurvivalmodel100424-0.1.5/classification_model/__init__.py` & `titanicsurvivalmodel100424-0.1.6/classification_model/__init__.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.5/classification_model/config/core.py` & `titanicsurvivalmodel100424-0.1.6/classification_model/config/core.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.5/classification_model/config.yml` & `titanicsurvivalmodel100424-0.1.6/classification_model/config.yml`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.5/classification_model/pipeline.py` & `titanicsurvivalmodel100424-0.1.6/classification_model/pipeline.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.5/classification_model/predict.py` & `titanicsurvivalmodel100424-0.1.6/classification_model/predict.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.5/classification_model/processing/data_manager.py` & `titanicsurvivalmodel100424-0.1.6/classification_model/processing/data_manager.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.5/classification_model/processing/features.py` & `titanicsurvivalmodel100424-0.1.6/classification_model/processing/features.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.5/classification_model/processing/validation.py` & `titanicsurvivalmodel100424-0.1.6/classification_model/processing/validation.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.5/classification_model/train_pipeline.py` & `titanicsurvivalmodel100424-0.1.6/classification_model/train_pipeline.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.5/classification_model/trained_models/classification_model_output_v0.1.5.pkl` & `titanicsurvivalmodel100424-0.1.6/classification_model/trained_models/classification_model_output_v0.1.6.pkl`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.5/pyproject.toml` & `titanicsurvivalmodel100424-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.5/setup.py` & `titanicsurvivalmodel100424-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.5/tests/test_features.py` & `titanicsurvivalmodel100424-0.1.6/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.5/tests/test_prediction.py` & `titanicsurvivalmodel100424-0.1.6/tests/test_prediction.py`

 * *Files identical despite different names*

