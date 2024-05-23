# Comparing `tmp/data_preprocessing_lib_byarat-0.1.0.tar.gz` & `tmp/data_preprocessing_lib_byarat-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_preprocessing_lib_byarat-0.1.0.tar", last modified: Sun May 19 07:58:45 2024, max compression
+gzip compressed data, was "data_preprocessing_lib_byarat-1.4.0.tar", last modified: Thu May 23 11:23:11 2024, max compression
```

## Comparing `data_preprocessing_lib_byarat-0.1.0.tar` & `data_preprocessing_lib_byarat-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,30 @@
-drwxr-xr-x   0 mehdiarat   (501) staff       (20)        0 2024-05-19 07:58:45.874744 data_preprocessing_lib_byarat-0.1.0/
--rw-r--r--   0 mehdiarat   (501) staff       (20)      285 2024-05-19 07:58:45.874637 data_preprocessing_lib_byarat-0.1.0/PKG-INFO
--rw-r--r--   0 mehdiarat   (501) staff       (20)        0 2024-05-19 07:28:29.000000 data_preprocessing_lib_byarat-0.1.0/README.md
-drwxr-xr-x   0 mehdiarat   (501) staff       (20)        0 2024-05-19 07:58:45.873957 data_preprocessing_lib_byarat-0.1.0/data_preprocessing_lib_byarat/
--rw-r--r--   0 mehdiarat   (501) staff       (20)        0 2024-05-19 07:28:53.000000 data_preprocessing_lib_byarat-0.1.0/data_preprocessing_lib_byarat/__init__.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)        0 2024-05-19 07:29:43.000000 data_preprocessing_lib_byarat-0.1.0/data_preprocessing_lib_byarat/categorical_encoder.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)        0 2024-05-19 07:29:36.000000 data_preprocessing_lib_byarat-0.1.0/data_preprocessing_lib_byarat/data_type_converter.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)        0 2024-05-19 07:29:49.000000 data_preprocessing_lib_byarat-0.1.0/data_preprocessing_lib_byarat/datetime_handler.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)        0 2024-05-19 07:29:30.000000 data_preprocessing_lib_byarat-0.1.0/data_preprocessing_lib_byarat/feature_engineer.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)        0 2024-05-19 07:29:05.000000 data_preprocessing_lib_byarat-0.1.0/data_preprocessing_lib_byarat/missing_value_handler.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)        0 2024-05-19 07:29:12.000000 data_preprocessing_lib_byarat-0.1.0/data_preprocessing_lib_byarat/outlier_handler.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)        0 2024-05-19 07:29:17.000000 data_preprocessing_lib_byarat-0.1.0/data_preprocessing_lib_byarat/scaler.py
--rw-r--r--   0 mehdiarat   (501) staff       (20)        0 2024-05-19 07:29:23.000000 data_preprocessing_lib_byarat-0.1.0/data_preprocessing_lib_byarat/text_cleaner.py
-drwxr-xr-x   0 mehdiarat   (501) staff       (20)        0 2024-05-19 07:58:45.874493 data_preprocessing_lib_byarat-0.1.0/data_preprocessing_lib_byarat.egg-info/
--rw-r--r--   0 mehdiarat   (501) staff       (20)      285 2024-05-19 07:58:45.000000 data_preprocessing_lib_byarat-0.1.0/data_preprocessing_lib_byarat.egg-info/PKG-INFO
--rw-r--r--   0 mehdiarat   (501) staff       (20)      720 2024-05-19 07:58:45.000000 data_preprocessing_lib_byarat-0.1.0/data_preprocessing_lib_byarat.egg-info/SOURCES.txt
--rw-r--r--   0 mehdiarat   (501) staff       (20)        1 2024-05-19 07:58:45.000000 data_preprocessing_lib_byarat-0.1.0/data_preprocessing_lib_byarat.egg-info/dependency_links.txt
--rw-r--r--   0 mehdiarat   (501) staff       (20)       31 2024-05-19 07:58:45.000000 data_preprocessing_lib_byarat-0.1.0/data_preprocessing_lib_byarat.egg-info/requires.txt
--rw-r--r--   0 mehdiarat   (501) staff       (20)       30 2024-05-19 07:58:45.000000 data_preprocessing_lib_byarat-0.1.0/data_preprocessing_lib_byarat.egg-info/top_level.txt
--rw-r--r--   0 mehdiarat   (501) staff       (20)       38 2024-05-19 07:58:45.874793 data_preprocessing_lib_byarat-0.1.0/setup.cfg
--rw-r--r--   0 mehdiarat   (501) staff       (20)      491 2024-05-19 07:58:10.000000 data_preprocessing_lib_byarat-0.1.0/setup.py
+drwxr-xr-x   0 mehdiarat   (501) staff       (20)        0 2024-05-23 11:23:11.462678 data_preprocessing_lib_byarat-1.4.0/
+-rw-r--r--   0 mehdiarat   (501) staff       (20)      286 2024-05-23 11:23:11.462550 data_preprocessing_lib_byarat-1.4.0/PKG-INFO
+-rw-r--r--   0 mehdiarat   (501) staff       (20)      155 2024-05-19 19:01:55.000000 data_preprocessing_lib_byarat-1.4.0/README.md
+drwxr-xr-x   0 mehdiarat   (501) staff       (20)        0 2024-05-23 11:23:11.460110 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/
+-rw-r--r--   0 mehdiarat   (501) staff       (20)      559 2024-05-22 22:05:31.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/__init__.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     2334 2024-05-21 12:33:24.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/categorical_encoder.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     1207 2024-05-21 12:38:26.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/data_type_converter.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     5458 2024-05-21 12:52:14.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/datetime_handler.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     8815 2024-05-21 13:00:54.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/feature_engineer.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     4164 2024-05-21 13:02:30.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/missing_value_handler.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     9624 2024-05-21 13:09:51.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/outlier_handler.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     4430 2024-05-21 13:12:26.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/scaler.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     6251 2024-05-21 13:19:19.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat/text_cleaner.py
+drwxr-xr-x   0 mehdiarat   (501) staff       (20)        0 2024-05-23 11:23:11.460929 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat.egg-info/
+-rw-r--r--   0 mehdiarat   (501) staff       (20)      286 2024-05-23 11:23:11.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat.egg-info/PKG-INFO
+-rw-r--r--   0 mehdiarat   (501) staff       (20)      964 2024-05-23 11:23:11.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat.egg-info/SOURCES.txt
+-rw-r--r--   0 mehdiarat   (501) staff       (20)        1 2024-05-23 11:23:11.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat.egg-info/dependency_links.txt
+-rw-r--r--   0 mehdiarat   (501) staff       (20)       80 2024-05-23 11:23:11.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat.egg-info/requires.txt
+-rw-r--r--   0 mehdiarat   (501) staff       (20)       30 2024-05-23 11:23:11.000000 data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat.egg-info/top_level.txt
+-rw-r--r--   0 mehdiarat   (501) staff       (20)       38 2024-05-23 11:23:11.462739 data_preprocessing_lib_byarat-1.4.0/setup.cfg
+-rw-r--r--   0 mehdiarat   (501) staff       (20)      904 2024-05-23 11:20:53.000000 data_preprocessing_lib_byarat-1.4.0/setup.py
+drwxr-xr-x   0 mehdiarat   (501) staff       (20)        0 2024-05-23 11:23:11.462284 data_preprocessing_lib_byarat-1.4.0/tests/
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     2214 2024-05-23 08:27:40.000000 data_preprocessing_lib_byarat-1.4.0/tests/test_categorical_encoder.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     1215 2024-05-21 11:18:34.000000 data_preprocessing_lib_byarat-1.4.0/tests/test_data_type_converter.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     3497 2024-05-21 11:19:37.000000 data_preprocessing_lib_byarat-1.4.0/tests/test_datetime_handler.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     5368 2024-05-21 11:20:59.000000 data_preprocessing_lib_byarat-1.4.0/tests/test_feature_engineer.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     2627 2024-05-21 11:30:27.000000 data_preprocessing_lib_byarat-1.4.0/tests/test_missing_value_handler.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     4623 2024-05-23 08:27:40.000000 data_preprocessing_lib_byarat-1.4.0/tests/test_outlier_handler.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     3177 2024-05-23 08:27:40.000000 data_preprocessing_lib_byarat-1.4.0/tests/test_scaler.py
+-rw-r--r--   0 mehdiarat   (501) staff       (20)     4643 2024-05-21 11:36:08.000000 data_preprocessing_lib_byarat-1.4.0/tests/test_text_cleaner.py
```

### Comparing `data_preprocessing_lib_byarat-0.1.0/data_preprocessing_lib_byarat.egg-info/SOURCES.txt` & `data_preprocessing_lib_byarat-1.4.0/data_preprocessing_lib_byarat.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -9,8 +9,16 @@
 data_preprocessing_lib_byarat/outlier_handler.py
 data_preprocessing_lib_byarat/scaler.py
 data_preprocessing_lib_byarat/text_cleaner.py
 data_preprocessing_lib_byarat.egg-info/PKG-INFO
 data_preprocessing_lib_byarat.egg-info/SOURCES.txt
 data_preprocessing_lib_byarat.egg-info/dependency_links.txt
 data_preprocessing_lib_byarat.egg-info/requires.txt
-data_preprocessing_lib_byarat.egg-info/top_level.txt
+data_preprocessing_lib_byarat.egg-info/top_level.txt
+tests/test_categorical_encoder.py
+tests/test_data_type_converter.py
+tests/test_datetime_handler.py
+tests/test_feature_engineer.py
+tests/test_missing_value_handler.py
+tests/test_outlier_handler.py
+tests/test_scaler.py
+tests/test_text_cleaner.py
```

