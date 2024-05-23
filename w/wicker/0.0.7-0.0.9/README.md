# Comparing `tmp/wicker-0.0.7.tar.gz` & `tmp/wicker-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wicker-0.0.7.tar", last modified: Fri Sep  8 01:08:12 2023, max compression
+gzip compressed data, was "wicker-0.0.9.tar", last modified: Mon Sep 25 15:23:27 2023, max compression
```

## Comparing `wicker-0.0.7.tar` & `wicker-0.0.9.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 01:08:12.188828 wicker-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-09-08 01:08:04.000000 wicker-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-09-08 01:08:04.000000 wicker-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2023-09-08 01:08:12.188828 wicker-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2023-09-08 01:08:04.000000 wicker-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-09-08 01:08:04.000000 wicker-0.0.7/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      206 2023-09-08 01:08:04.000000 wicker-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      866 2023-09-08 01:08:12.188828 wicker-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-09-08 01:08:04.000000 wicker-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 01:08:12.188828 wicker-0.0.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 01:08:12.180828 wicker-0.0.7/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 01:08:04.000000 wicker-0.0.7/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2023-09-08 01:08:04.000000 wicker-0.0.7/tests/core/test_persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)    21017 2023-09-08 01:08:04.000000 wicker-0.0.7/tests/test_avro_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7784 2023-09-08 01:08:04.000000 wicker-0.0.7/tests/test_column_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     7157 2023-09-08 01:08:04.000000 wicker-0.0.7/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2023-09-08 01:08:04.000000 wicker-0.0.7/tests/test_filelock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2023-09-08 01:08:04.000000 wicker-0.0.7/tests/test_numpy_codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     7314 2023-09-08 01:08:04.000000 wicker-0.0.7/tests/test_s3_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     9718 2023-09-08 01:08:04.000000 wicker-0.0.7/tests/test_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2023-09-08 01:08:04.000000 wicker-0.0.7/tests/test_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2023-09-08 01:08:04.000000 wicker-0.0.7/tests/test_wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 01:08:12.180828 wicker-0.0.7/wicker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 01:08:12.184828 wicker-0.0.7/wicker/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/core/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    12544 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/core/column_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8926 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/core/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/core/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/core/filelock.py
--rw-r--r--   0 runner    (1001) docker     (127)    11063 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/core/persistance.py
--rw-r--r--   0 runner    (1001) docker     (127)    10410 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/core/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)    10680 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/core/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10994 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/core/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 01:08:12.184828 wicker-0.0.7/wicker/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/plugins/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (127)    11960 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/plugins/flyte.py
--rw-r--r--   0 runner    (1001) docker     (127)    11310 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/plugins/spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/plugins/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 01:08:12.184828 wicker-0.0.7/wicker/schema/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/schema/codecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/schema/dataloading.py
--rw-r--r--   0 runner    (1001) docker     (127)     7328 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/schema/dataparsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    18946 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    11466 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/schema/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/schema/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 01:08:12.184828 wicker-0.0.7/wicker/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/testing/codecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2023-09-08 01:08:04.000000 wicker-0.0.7/wicker/testing/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 01:08:12.188828 wicker-0.0.7/wicker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2023-09-08 01:08:12.000000 wicker-0.0.7/wicker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2023-09-08 01:08:12.000000 wicker-0.0.7/wicker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 01:08:12.000000 wicker-0.0.7/wicker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-09-08 01:08:12.000000 wicker-0.0.7/wicker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-09-08 01:08:12.000000 wicker-0.0.7/wicker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 15:23:27.517513 wicker-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-09-25 15:23:19.000000 wicker-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-09-25 15:23:19.000000 wicker-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2023-09-25 15:23:27.517513 wicker-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2023-09-25 15:23:19.000000 wicker-0.0.9/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)        5 2023-09-25 15:23:19.000000 wicker-0.0.9/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2023-09-25 15:23:19.000000 wicker-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2023-09-25 15:23:27.517513 wicker-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2023-09-25 15:23:19.000000 wicker-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 15:23:27.517513 wicker-0.0.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 15:23:27.513513 wicker-0.0.9/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-25 15:23:19.000000 wicker-0.0.9/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2023-09-25 15:23:19.000000 wicker-0.0.9/tests/core/test_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21017 2023-09-25 15:23:19.000000 wicker-0.0.9/tests/test_avro_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7784 2023-09-25 15:23:19.000000 wicker-0.0.9/tests/test_column_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7157 2023-09-25 15:23:19.000000 wicker-0.0.9/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2023-09-25 15:23:19.000000 wicker-0.0.9/tests/test_filelock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2023-09-25 15:23:19.000000 wicker-0.0.9/tests/test_numpy_codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7704 2023-09-25 15:23:19.000000 wicker-0.0.9/tests/test_s3_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9718 2023-09-25 15:23:19.000000 wicker-0.0.9/tests/test_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2023-09-25 15:23:19.000000 wicker-0.0.9/tests/test_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2023-09-25 15:23:19.000000 wicker-0.0.9/tests/test_wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 15:23:27.513513 wicker-0.0.9/wicker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 15:23:27.513513 wicker-0.0.9/wicker/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/core/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12544 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/core/column_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8926 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/core/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/core/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/core/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11063 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/core/persistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10410 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/core/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11911 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/core/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10994 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/core/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 15:23:27.513513 wicker-0.0.9/wicker/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/plugins/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11960 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/plugins/flyte.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11310 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/plugins/spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/plugins/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 15:23:27.513513 wicker-0.0.9/wicker/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/schema/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/schema/dataloading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7328 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/schema/dataparsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18946 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11466 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/schema/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/schema/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 15:23:27.517513 wicker-0.0.9/wicker/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/testing/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2023-09-25 15:23:19.000000 wicker-0.0.9/wicker/testing/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 15:23:27.517513 wicker-0.0.9/wicker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2023-09-25 15:23:27.000000 wicker-0.0.9/wicker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2023-09-25 15:23:27.000000 wicker-0.0.9/wicker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 15:23:27.000000 wicker-0.0.9/wicker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2023-09-25 15:23:27.000000 wicker-0.0.9/wicker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-09-25 15:23:27.000000 wicker-0.0.9/wicker.egg-info/top_level.txt
```

### Comparing `wicker-0.0.7/LICENSE` & `wicker-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/PKG-INFO` & `wicker-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wicker
-Version: 0.0.7
+Version: 0.0.9
 Summary: An open source framework for Machine Learning dataset storage and serving
 Home-page: https://github.com/woven-planet/Wicker
 Author: Jay Chia
 Author-email: jaychia94@gmail.com
 Project-URL: Bug Tracker, https://github.com/woven-planet/Wicker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `wicker-0.0.7/README.md` & `wicker-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/setup.cfg` & `wicker-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/tests/core/test_persistence.py` & `wicker-0.0.9/tests/core/test_persistence.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/tests/test_avro_schema.py` & `wicker-0.0.9/tests/test_avro_schema.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/tests/test_column_files.py` & `wicker-0.0.9/tests/test_column_files.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/tests/test_datasets.py` & `wicker-0.0.9/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/tests/test_filelock.py` & `wicker-0.0.9/tests/test_filelock.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/tests/test_numpy_codec.py` & `wicker-0.0.9/tests/test_numpy_codec.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/tests/test_s3_storage.py` & `wicker-0.0.9/tests/test_s3_storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -143,15 +143,23 @@
         """Unit test for the S3PathFactory get_column_concatenated_bytes_files_path
         function"""
         # If store_concatenated_bytes_files_in_dataset is False, return the default path
         dummy_config: Dict[str, Any] = {
             "aws_s3_config": {
                 "s3_datasets_path": "s3://dummy_bucket/wicker/",
                 "region": "us-east-1",
-            }
+                "boto_config": {"max_pool_connections": 10, "read_timeout_s": 140, "connect_timeout_s": 140},
+            },
+            "dynamodb_config": {"table_name": "fake-table-name", "region": "us-west-2"},
+            "storage_download_config": {
+                "retries": 2,
+                "timeout": 150,
+                "retry_backoff": 5,
+                "retry_delay_s": 4,
+            },
         }
         mock_get_config.return_value = WickerConfig.from_json(dummy_config)
 
         path_factory = S3PathFactory()
         self.assertEqual(
             path_factory.get_column_concatenated_bytes_files_path(),
             "s3://dummy_bucket/wicker/__COLUMN_CONCATENATED_FILES__",
```

### Comparing `wicker-0.0.7/tests/test_shuffle.py` & `wicker-0.0.9/tests/test_shuffle.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/tests/test_spark.py` & `wicker-0.0.9/tests/test_spark.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/tests/test_wandb.py` & `wicker-0.0.9/tests/test_wandb.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/wicker/core/column_files.py` & `wicker-0.0.9/wicker/core/column_files.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/wicker/core/config.py` & `wicker-0.0.9/wicker/core/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,40 +20,76 @@
         return cls(
             wandb_api_key=data.get("wandb_api_key", None),
             wandb_base_url=data.get("wandb_base_url", None),
         )
 
 
 @dataclasses.dataclass(frozen=True)
+class BotoS3Config:
+    max_pool_connections: int
+    read_timeout_s: int
+    connect_timeout_s: int
+
+    @classmethod
+    def from_json(cls, data: Dict[str, Any]) -> BotoS3Config:
+        return cls(
+            max_pool_connections=data["max_pool_connections"],
+            read_timeout_s=data["read_timeout_s"],
+            connect_timeout_s=data["connect_timeout_s"],
+        )
+
+
+@dataclasses.dataclass(frozen=True)
 class WickerAwsS3Config:
     s3_datasets_path: str
     region: str
+    boto_config: BotoS3Config
     store_concatenated_bytes_files_in_dataset: bool = False
 
     @classmethod
     def from_json(cls, data: Dict[str, Any]) -> WickerAwsS3Config:
         return cls(
             s3_datasets_path=data["s3_datasets_path"],
             region=data["region"],
+            boto_config=BotoS3Config.from_json(data["boto_config"]),
             store_concatenated_bytes_files_in_dataset=data.get("store_concatenated_bytes_files_in_dataset", False),
         )
 
 
 @dataclasses.dataclass(frozen=True)
+class StorageDownloadConfig:
+    retries: int
+    timeout: int
+    retry_backoff: int
+    retry_delay_s: int
+
+    @classmethod
+    def from_json(cls, data: Dict[str, Any]) -> StorageDownloadConfig:
+        return cls(
+            retries=data["retries"],
+            timeout=data["timeout"],
+            retry_backoff=data["retry_backoff"],
+            retry_delay_s=data["retry_delay_s"],
+        )
+
+
+@dataclasses.dataclass(frozen=True)
 class WickerConfig:
     raw: Dict[str, Any]
     aws_s3_config: WickerAwsS3Config
     wandb_config: WickerWandBConfig
+    storage_download_config: StorageDownloadConfig
 
     @classmethod
     def from_json(cls, data: Dict[str, Any]) -> WickerConfig:
         return cls(
             raw=data,
             aws_s3_config=WickerAwsS3Config.from_json(data["aws_s3_config"]),
             wandb_config=WickerWandBConfig.from_json(data.get("wandb_config", {})),
+            storage_download_config=StorageDownloadConfig.from_json(data["storage_download_config"]),
         )
 
 
 def get_config() -> WickerConfig:
     """Retrieves the Wicker config for the current process"""
 
     wicker_config_path = os.getenv("WICKER_CONFIG_PATH", os.path.expanduser("~/wickerconfig.json"))
```

### Comparing `wicker-0.0.7/wicker/core/datasets.py` & `wicker-0.0.9/wicker/core/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from wicker.core.definitions import DatasetDefinition, DatasetID, DatasetPartition
 from wicker.core.shuffle import ShuffleWorker
 from wicker.core.storage import S3DataStorage, S3PathFactory
 from wicker.schema import dataloading, serialization
 from wicker.schema.schema import DatasetSchema
 
 # How long to wait before timing out on filelocks in seconds
-FILE_LOCK_TIMEOUT_SECONDS = 240
+FILE_LOCK_TIMEOUT_SECONDS = 300
 
 
 class AbstractDataset(abc.ABC):
     """Interface for a Map-style (non-streaming) Dataset"""
 
     @abc.abstractmethod
     def __getitem__(self, idx: int) -> Dict[str, Any]:
```

### Comparing `wicker-0.0.7/wicker/core/definitions.py` & `wicker-0.0.9/wicker/core/definitions.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/wicker/core/filelock.py` & `wicker-0.0.9/wicker/core/filelock.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/wicker/core/persistance.py` & `wicker-0.0.9/wicker/core/persistance.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/wicker/core/shuffle.py` & `wicker-0.0.9/wicker/core/shuffle.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/wicker/core/storage.py` & `wicker-0.0.9/wicker/core/storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,35 +11,45 @@
 import os
 import uuid
 from typing import Any, Dict, Optional, Tuple
 from urllib.parse import urlparse
 
 import boto3
 import boto3.session
+import botocore  # type: ignore
 from botocore.exceptions import ClientError  # type: ignore
+from retry import retry
 
 from wicker.core.config import get_config
 from wicker.core.definitions import DatasetID, DatasetPartition
 from wicker.core.filelock import SimpleUnixFileLock
+from wicker.core.utils import time_limit
 
 logger = logging.getLogger(__name__)
 
 
 class S3DataStorage:
     """Storage routines for reading and writing objects in S3"""
 
     def __init__(self, session: Optional[boto3.session.Session] = None) -> None:
         """Constructor for an S3Storage instance
 
         Part of the reason to structure S3 routines as a class rather utility functions is to enable
         unit tests to easily mock / patch the S3 client or to utilize the S3 Stubber. Unit tests
         might also find it convenient to mock or patch member functions on instances of this class.
         """
+        boto_config = get_config().aws_s3_config.boto_config
+        boto_client_config = botocore.config.Config(
+            max_pool_connections=boto_config.max_pool_connections,
+            read_timeout=boto_config.read_timeout_s,
+            connect_timeout=boto_config.connect_timeout_s,
+        )
         self.session = boto3.session.Session() if session is None else session
-        self.client = self.session.client("s3")
+        self.client = self.session.client("s3", config=boto_client_config)
+        self.read_timeout = get_config().storage_download_config.timeout
 
     def __getstate__(self) -> Dict[Any, Any]:
         return {}
 
     def __setstate__(self, state: Dict[Any, Any]) -> None:
         self.session = boto3.session.Session()
         self.client = self.session.client("s3")
@@ -68,14 +78,31 @@
         bucket, key = self.bucket_key_from_s3_path(input_path)
         try:
             self.client.head_object(Bucket=bucket, Key=key)
             return True
         except ClientError:
             return False
 
+    @retry(
+        Exception,
+        tries=get_config().storage_download_config.retries,
+        backoff=get_config().storage_download_config.retry_backoff,
+        delay=get_config().storage_download_config.retry_delay_s,
+        logger=logger,
+    )
+    def download_with_retries(self, bucket: str, key: str, local_path: str):
+        try:
+            with time_limit(
+                self.read_timeout, f"Timing out in trying to download object for bucket: {bucket}, key: {key}"
+            ):
+                self.client.download_file(bucket, key, local_path)
+        except Exception as e:
+            logging.error(f"Failed to download s3 object in bucket: {bucket}, key: {key}")
+            raise e
+
     def fetch_file_s3(self, input_path: str, local_prefix: str, timeout_seconds: int = 120) -> str:
         """Fetches a file from S3 to the local machine and skips it if it already exists. This function
         is safe to call concurrently from multiple processes and utilizes a local filelock to block
         parallel downloads such that only one process will perform the download.
 
         This function assumes the input_path is a valid file in S3.
 
@@ -95,16 +122,15 @@
             with SimpleUnixFileLock(lock_path, timeout_seconds=timeout_seconds):
                 if not os.path.isfile(success_marker):
 
                     # For now, we will only download the file if it has not already been downloaded already.
                     # Long term, we would also add a size check or md5sum comparison against the object in S3.
                     filedir = os.path.split(local_path)[0]
                     os.makedirs(filedir, exist_ok=True)
-                    self.client.download_file(bucket, key, local_path)
-
+                    self.download_with_retries(bucket=bucket, key=key, local_path=local_path)
                     with open(success_marker, "w"):
                         pass
 
         return local_path
 
     def fetch_obj_s3(self, input_path: str) -> bytes:
         """Fetches an object from S3 as bytes in memory
```

### Comparing `wicker-0.0.7/wicker/core/writer.py` & `wicker-0.0.9/wicker/core/writer.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/wicker/plugins/dynamodb.py` & `wicker-0.0.9/wicker/plugins/dynamodb.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/wicker/plugins/flyte.py` & `wicker-0.0.9/wicker/plugins/flyte.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/wicker/plugins/spark.py` & `wicker-0.0.9/wicker/plugins/spark.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/wicker/plugins/wandb.py` & `wicker-0.0.9/wicker/plugins/wandb.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/wicker/schema/codecs.py` & `wicker-0.0.9/wicker/schema/codecs.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/wicker/schema/dataloading.py` & `wicker-0.0.9/wicker/schema/dataloading.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/wicker/schema/dataparsing.py` & `wicker-0.0.9/wicker/schema/dataparsing.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/wicker/schema/schema.py` & `wicker-0.0.9/wicker/schema/schema.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/wicker/schema/serialization.py` & `wicker-0.0.9/wicker/schema/serialization.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/wicker/schema/validation.py` & `wicker-0.0.9/wicker/schema/validation.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/wicker/testing/codecs.py` & `wicker-0.0.9/wicker/testing/codecs.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/wicker/testing/storage.py` & `wicker-0.0.9/wicker/testing/storage.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.7/wicker.egg-info/PKG-INFO` & `wicker-0.0.9/wicker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wicker
-Version: 0.0.7
+Version: 0.0.9
 Summary: An open source framework for Machine Learning dataset storage and serving
 Home-page: https://github.com/woven-planet/Wicker
 Author: Jay Chia
 Author-email: jaychia94@gmail.com
 Project-URL: Bug Tracker, https://github.com/woven-planet/Wicker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `wicker-0.0.7/wicker.egg-info/SOURCES.txt` & `wicker-0.0.9/wicker.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 ./wicker/core/datasets.py
 ./wicker/core/definitions.py
 ./wicker/core/errors.py
 ./wicker/core/filelock.py
 ./wicker/core/persistance.py
 ./wicker/core/shuffle.py
 ./wicker/core/storage.py
+./wicker/core/utils.py
 ./wicker/core/writer.py
 ./wicker/plugins/__init__.py
 ./wicker/plugins/dynamodb.py
 ./wicker/plugins/flyte.py
 ./wicker/plugins/spark.py
 ./wicker/plugins/wandb.py
 ./wicker/schema/__init__.py
```

