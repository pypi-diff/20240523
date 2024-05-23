# Comparing `tmp/data_preprocessing_lib_byarat-1.4.0.tar.gz` & `tmp/data_preprocessing_lib_byarat-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_preprocessing_lib_byarat-1.4.0.tar", last modified: Thu May 23 11:23:11 2024, max compression
+gzip compressed data, was "data_preprocessing_lib_byarat-1.5.0.tar", last modified: Thu May 23 11:27:43 2024, max compression
```

## Comparing `data_preprocessing_lib_byarat-1.4.0.tar` & `data_preprocessing_lib_byarat-1.5.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 mehdiarat   (501) staff       (20)        0 2024-05-23 11:23:11.462678 data_preprocessing_lib_byarat-1.4.0/
--rw-r--r--   0 mehdiarat   (501) staff       (20)      286 2024-05-23 11:23:11.462550 data_preprocessing_lib_byarat-1.4.0/PKG-INFO
--rw-r--r--   0 mehdiarat   (501) staff       (20)      155 2024-05-19 19:01:55.000000 data_preprocessing_lib_byarat-1.4.0/README.md
-drwxr-xr-x   0 mehdiarat   (501) staff       (20)        0 2024-05-23 11:23:11.460110 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/
--rw-r--r--   0 mehdiarat   (501) staff       (20)      559 2024-05-22 22:05:31.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/__init__.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)     2334 2024-05-21 12:33:24.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/categorical_encoder.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)     1207 2024-05-21 12:38:26.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/data_type_converter.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)     5458 2024-05-21 12:52:14.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/datetime_handler.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)     8815 2024-05-21 13:00:54.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/feature_engineer.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)     4164 2024-05-21 13:02:30.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/missing_value_handler.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)     9624 2024-05-21 13:09:51.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/outlier_handler.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)     4430 2024-05-21 13:12:26.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/scaler.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)     6251 2024-05-21 13:19:19.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/text_cleaner.py
-drwxr-xr-x   0 mehdiarat   (501) staff       (20)        0 2024-05-23 11:23:11.460929 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat.egg-info/
--rw-r--r--   0 mehdiarat   (501) staff       (20)      286 2024-05-23 11:23:11.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat.egg-info/PKG-INFO
--rw-r--r--   0 mehdiarat   (501) staff       (20)      964 2024-05-23 11:23:11.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat.egg-info/SOURCES.txt
--rw-r--r--   0 mehdiarat   (501) staff       (20)        1 2024-05-23 11:23:11.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat.egg-info/dependency_links.txt
--rw-r--r--   0 mehdiarat   (501) staff       (20)       80 2024-05-23 11:23:11.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat.egg-info/requires.txt
--rw-r--r--   0 mehdiarat   (501) staff       (20)       30 2024-05-23 11:23:11.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat.egg-info/top_level.txt
--rw-r--r--   0 mehdiarat   (501) staff       (20)       38 2024-05-23 11:23:11.462739 data_preprocessing_lib_byarat-1.4.0/setup.cfg
--rw-r--r--   0 mehdiarat   (501) staff       (20)      904 2024-05-23 11:20:53.000000 data_preprocessing_lib_byarat-1.4.0/setup.py
-drwxr-xr-x   0 mehdiarat   (501) staff       (20)        0 2024-05-23 11:23:11.462284 data_preprocessing_lib_byarat-1.4.0/tests/
--rw-r--r--   0 mehdiarat   (501) staff       (20)     2214 2024-05-23 08:27:40.000000 data_preprocessing_lib_byarat-1.4.0/tests/test_categorical_encoder.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)     1215 2024-05-21 11:18:34.000000 data_preprocessing_lib_byarat-1.4.0/tests/test_data_type_converter.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)     3497 2024-05-21 11:19:37.000000 data_preprocessing_lib_byarat-1.4.0/tests/test_datetime_handler.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)     5368 2024-05-21 11:20:59.000000 data_preprocessing_lib_byarat-1.4.0/tests/test_feature_engineer.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)     2627 2024-05-21 11:30:27.000000 data_preprocessing_lib_byarat-1.4.0/tests/test_missing_value_handler.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)     4623 2024-05-23 08:27:40.000000 data_preprocessing_lib_byarat-1.4.0/tests/test_outlier_handler.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)     3177 2024-05-23 08:27:40.000000 data_preprocessing_lib_byarat-1.4.0/tests/test_scaler.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)     4643 2024-05-21 11:36:08.000000 data_preprocessing_lib_byarat-1.4.0/tests/test_text_cleaner.py
+drwxr-xr-x   0 mehdiarat   (501) staff       (20)        0 2024-05-23 11:27:43.941779 data_preprocessing_lib_byarat-1.5.0/
+-rw-r--r--   0 mehdiarat   (501) staff       (20)      286 2024-05-23 11:27:43.941640 data_preprocessing_lib_byarat-1.5.0/PKG-INFO
+-rw-r--r--   0 mehdiarat   (501) staff       (20)      155 2024-05-19 19:01:55.000000 data_preprocessing_lib_byarat-1.5.0/README.md
+drwxr-xr-x   0 mehdiarat   (501) staff       (20)        0 2024-05-23 11:27:43.939101 data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat/
+-rw-r--r--   0 mehdiarat   (501) staff       (20)      559 2024-05-22 22:05:31.000000 data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat/__init__.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     2342 2024-05-23 11:27:08.000000 data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat/categorical_encoder.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     1207 2024-05-21 12:38:26.000000 data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat/data_type_converter.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     5458 2024-05-21 12:52:14.000000 data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat/datetime_handler.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     8815 2024-05-21 13:00:54.000000 data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat/feature_engineer.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     4164 2024-05-21 13:02:30.000000 data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat/missing_value_handler.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     9624 2024-05-21 13:09:51.000000 data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat/outlier_handler.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     4430 2024-05-21 13:12:26.000000 data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat/scaler.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     6251 2024-05-21 13:19:19.000000 data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat/text_cleaner.py
+drwxr-xr-x   0 mehdiarat   (501) staff       (20)        0 2024-05-23 11:27:43.939955 data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat.egg-info/
+-rw-r--r--   0 mehdiarat   (501) staff       (20)      286 2024-05-23 11:27:43.000000 data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat.egg-info/PKG-INFO
+-rw-r--r--   0 mehdiarat   (501) staff       (20)      964 2024-05-23 11:27:43.000000 data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat.egg-info/SOURCES.txt
+-rw-r--r--   0 mehdiarat   (501) staff       (20)        1 2024-05-23 11:27:43.000000 data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat.egg-info/dependency_links.txt
+-rw-r--r--   0 mehdiarat   (501) staff       (20)       80 2024-05-23 11:27:43.000000 data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat.egg-info/requires.txt
+-rw-r--r--   0 mehdiarat   (501) staff       (20)       30 2024-05-23 11:27:43.000000 data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat.egg-info/top_level.txt
+-rw-r--r--   0 mehdiarat   (501) staff       (20)       38 2024-05-23 11:27:43.941835 data_preprocessing_lib_byarat-1.5.0/setup.cfg
+-rw-r--r--   0 mehdiarat   (501) staff       (20)      904 2024-05-23 11:27:17.000000 data_preprocessing_lib_byarat-1.5.0/setup.py
+drwxr-xr-x   0 mehdiarat   (501) staff       (20)        0 2024-05-23 11:27:43.941360 data_preprocessing_lib_byarat-1.5.0/tests/
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     2214 2024-05-23 08:27:40.000000 data_preprocessing_lib_byarat-1.5.0/tests/test_categorical_encoder.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     1215 2024-05-21 11:18:34.000000 data_preprocessing_lib_byarat-1.5.0/tests/test_data_type_converter.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     3497 2024-05-21 11:19:37.000000 data_preprocessing_lib_byarat-1.5.0/tests/test_datetime_handler.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     5368 2024-05-21 11:20:59.000000 data_preprocessing_lib_byarat-1.5.0/tests/test_feature_engineer.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     2627 2024-05-21 11:30:27.000000 data_preprocessing_lib_byarat-1.5.0/tests/test_missing_value_handler.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     4623 2024-05-23 08:27:40.000000 data_preprocessing_lib_byarat-1.5.0/tests/test_outlier_handler.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     3177 2024-05-23 08:27:40.000000 data_preprocessing_lib_byarat-1.5.0/tests/test_scaler.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     4643 2024-05-21 11:36:08.000000 data_preprocessing_lib_byarat-1.5.0/tests/test_text_cleaner.py
```

### Comparing `data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/__init__.py` & `data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat/__init__.py`

 * *Files identical despite different names*

### Comparing `data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/categorical_encoder.py` & `data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat/categorical_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas as pd
 from sklearn.preprocessing import LabelEncoder, OrdinalEncoder
 
 
 class CategoricalEncoder:
     @staticmethod
     def one_hot_encode(df, column):
-        return pd.get_dummies(df, columns=[column])
+     return pd.get_dummies(df, columns=[column], dtype=int)
 
     @staticmethod
     def label_encode(df, column):
         df[column] = df[column].astype('category').cat.codes
         return df
     @staticmethod
     def ordinal_encode(df, column, categories='auto'):
```

### Comparing `data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/data_type_converter.py` & `data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat/data_type_converter.py`

 * *Files identical despite different names*

### Comparing `data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/datetime_handler.py` & `data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat/datetime_handler.py`

 * *Files identical despite different names*

### Comparing `data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/feature_engineer.py` & `data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat/feature_engineer.py`

 * *Files identical despite different names*

### Comparing `data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/missing_value_handler.py` & `data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat/missing_value_handler.py`

 * *Files identical despite different names*

### Comparing `data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/outlier_handler.py` & `data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat/outlier_handler.py`

 * *Files identical despite different names*

### Comparing `data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/scaler.py` & `data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat/scaler.py`

 * *Files identical despite different names*

### Comparing `data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/text_cleaner.py` & `data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat/text_cleaner.py`

 * *Files identical despite different names*

### Comparing `data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat.egg-info/SOURCES.txt` & `data_preprocessing_lib_byarat-1.5.0/data_preprocessing_lib_byarat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_preprocessing_lib_byarat-1.4.0/setup.py` & `data_preprocessing_lib_byarat-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     """Post-installation for installation mode."""
     def run(self):
         install.run(self)
         subprocess.call(['python', 'download_nltk_data.py'])
 
 setup(
     name='data_preprocessing_lib_byarat',
-    version='1.4.0',
+    version='1.5.0',
     description='An easy peasy comprehensive library for data preprocessing tasks',
     author='Mehdi Miraç ARAT, Latif Şimşek',
     author_email='mehdimirac.arat@stu.fsm.edu.tr, latif.simsek@stu.fsm.edu.tr',
     packages=find_packages(),
     install_requires=[
         'pandas',
         'numpy',
```

### Comparing `data_preprocessing_lib_byarat-1.4.0/tests/test_categorical_encoder.py` & `data_preprocessing_lib_byarat-1.5.0/tests/test_categorical_encoder.py`

 * *Files identical despite different names*

### Comparing `data_preprocessing_lib_byarat-1.4.0/tests/test_data_type_converter.py` & `data_preprocessing_lib_byarat-1.5.0/tests/test_data_type_converter.py`

 * *Files identical despite different names*

### Comparing `data_preprocessing_lib_byarat-1.4.0/tests/test_datetime_handler.py` & `data_preprocessing_lib_byarat-1.5.0/tests/test_datetime_handler.py`

 * *Files identical despite different names*

### Comparing `data_preprocessing_lib_byarat-1.4.0/tests/test_feature_engineer.py` & `data_preprocessing_lib_byarat-1.5.0/tests/test_feature_engineer.py`

 * *Files identical despite different names*

### Comparing `data_preprocessing_lib_byarat-1.4.0/tests/test_missing_value_handler.py` & `data_preprocessing_lib_byarat-1.5.0/tests/test_missing_value_handler.py`

 * *Files identical despite different names*

### Comparing `data_preprocessing_lib_byarat-1.4.0/tests/test_outlier_handler.py` & `data_preprocessing_lib_byarat-1.5.0/tests/test_outlier_handler.py`

 * *Files identical despite different names*

### Comparing `data_preprocessing_lib_byarat-1.4.0/tests/test_scaler.py` & `data_preprocessing_lib_byarat-1.5.0/tests/test_scaler.py`

 * *Files identical despite different names*

### Comparing `data_preprocessing_lib_byarat-1.4.0/tests/test_text_cleaner.py` & `data_preprocessing_lib_byarat-1.5.0/tests/test_text_cleaner.py`

 * *Files identical despite different names*

