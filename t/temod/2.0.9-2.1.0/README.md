# Comparing `tmp/temod-2.0.9.tar.gz` & `tmp/temod-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temod-2.0.9.tar", last modified: Tue Apr  2 10:06:42 2024, max compression
+gzip compressed data, was "temod-2.1.0.tar", last modified: Thu May 23 09:46:20 2024, max compression
```

## Comparing `temod-2.0.9.tar` & `temod-2.1.0.tar`

### file list

```diff
@@ -1,54 +1,58 @@
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.456259 temod-2.0.9/
--rw-rw-r--   0 oem      (29999) oem      (29999)     1069 2023-07-16 09:53:35.000000 temod-2.0.9/LICENSE.txt
--rw-r--r--   0 oem      (29999) oem      (29999)      703 2024-04-02 10:06:42.456259 temod-2.0.9/PKG-INFO
--rw-rw-r--   0 oem      (29999) oem      (29999)       67 2023-07-16 09:51:01.000000 temod-2.0.9/README.md
--rw-rw-r--   0 oem      (29999) oem      (29999)      704 2024-04-02 10:06:23.000000 temod-2.0.9/pyproject.toml
--rw-rw-r--   0 oem      (29999) oem      (29999)       38 2024-04-02 10:06:42.456259 temod-2.0.9/setup.cfg
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.452259 temod-2.0.9/src/
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.452259 temod-2.0.9/src/temod/
--rw-rw-r--   0 oem      (29999) oem      (29999)       27 2023-07-15 13:43:54.000000 temod-2.0.9/src/temod/__init__.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.452259 temod-2.0.9/src/temod/base/
--rw-rw-r--   0 oem      (29999) oem      (29999)      145 2023-07-15 13:44:09.000000 temod-2.0.9/src/temod/base/__init__.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     9973 2024-03-24 12:34:15.000000 temod-2.0.9/src/temod/base/attribute.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     1697 2023-07-15 13:44:06.000000 temod-2.0.9/src/temod/base/cluster.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     2900 2023-07-15 13:44:09.000000 temod-2.0.9/src/temod/base/condition.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     1986 2023-07-15 13:44:10.000000 temod-2.0.9/src/temod/base/constraint.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     6238 2023-07-15 13:44:09.000000 temod-2.0.9/src/temod/base/entity.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     1481 2023-07-15 13:44:09.000000 temod-2.0.9/src/temod/base/exceptions.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     2557 2023-07-15 13:44:10.000000 temod-2.0.9/src/temod/base/join.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.452259 temod-2.0.9/src/temod/ext/
--rw-rw-r--   0 oem      (29999) oem      (29999)    11228 2023-07-15 13:43:55.000000 temod-2.0.9/src/temod/ext/holders.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.452259 temod-2.0.9/src/temod/operators/
--rw-rw-r--   0 oem      (29999) oem      (29999)      451 2023-07-15 13:43:22.000000 temod-2.0.9/src/temod/operators/aggregation.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.452259 temod-2.0.9/src/temod/storage/
--rw-rw-r--   0 oem      (29999) oem      (29999)      201 2023-07-15 13:43:59.000000 temod-2.0.9/src/temod/storage/__init__.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.452259 temod-2.0.9/src/temod/storage/directory/
--rw-rw-r--   0 oem      (29999) oem      (29999)       59 2023-07-15 13:43:57.000000 temod-2.0.9/src/temod/storage/directory/__init__.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     5004 2023-07-15 13:43:57.000000 temod-2.0.9/src/temod/storage/directory/directoryStorage.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     2835 2023-07-15 13:43:55.000000 temod-2.0.9/src/temod/storage/directory/yamlStorage.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.456259 temod-2.0.9/src/temod/storage/exceptions/
--rw-rw-r--   0 oem      (29999) oem      (29999)      774 2023-07-15 13:43:58.000000 temod-2.0.9/src/temod/storage/exceptions/entities.py
--rw-rw-r--   0 oem      (29999) oem      (29999)      541 2023-07-15 13:43:58.000000 temod-2.0.9/src/temod/storage/exceptions/joins.py
--rw-rw-r--   0 oem      (29999) oem      (29999)      418 2023-07-15 13:43:58.000000 temod-2.0.9/src/temod/storage/exceptions/translators.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.456259 temod-2.0.9/src/temod/storage/influxdb/
--rw-rw-r--   0 oem      (29999) oem      (29999)     9803 2024-02-25 20:41:24.000000 temod-2.0.9/src/temod/storage/influxdb/influxEntityStorage.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     2363 2024-02-25 20:41:37.000000 temod-2.0.9/src/temod/storage/influxdb/influxStorage.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     6019 2023-07-15 13:43:59.000000 temod-2.0.9/src/temod/storage/influxdb/influxTranslators.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.456259 temod-2.0.9/src/temod/storage/mysql/
--rw-rw-r--   0 oem      (29999) oem      (29999)      131 2023-07-15 13:44:05.000000 temod-2.0.9/src/temod/storage/mysql/__init__.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     2416 2023-07-15 13:44:01.000000 temod-2.0.9/src/temod/storage/mysql/mysqlAttributesTranslator.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     6604 2024-02-25 20:41:49.000000 temod-2.0.9/src/temod/storage/mysql/mysqlClusterStorage.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     4235 2023-07-15 13:44:05.000000 temod-2.0.9/src/temod/storage/mysql/mysqlConditionsTranslator.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     9775 2024-03-27 20:27:49.000000 temod-2.0.9/src/temod/storage/mysql/mysqlEntityStorage.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     9497 2024-03-24 11:58:47.000000 temod-2.0.9/src/temod/storage/mysql/mysqlJoinStorage.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     2148 2024-03-24 12:33:38.000000 temod-2.0.9/src/temod/storage/mysql/mysqlStorage.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.456259 temod-2.0.9/src/temod/utils/
--rw-rw-r--   0 oem      (29999) oem      (29999)     2073 2023-07-15 13:43:23.000000 temod-2.0.9/src/temod/utils/decorators.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     2373 2023-07-15 13:43:23.000000 temod-2.0.9/src/temod/utils/exoskeleton.py
--rw-rw-r--   0 oem      (29999) oem      (29999)      547 2023-07-15 13:43:24.000000 temod-2.0.9/src/temod/utils/graphs.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.456259 temod-2.0.9/src/temod.egg-info/
--rw-r--r--   0 oem      (29999) oem      (29999)      703 2024-04-02 10:06:42.000000 temod-2.0.9/src/temod.egg-info/PKG-INFO
--rw-rw-r--   0 oem      (29999) oem      (29999)     1329 2024-04-02 10:06:42.000000 temod-2.0.9/src/temod.egg-info/SOURCES.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)        1 2024-04-02 10:06:42.000000 temod-2.0.9/src/temod.egg-info/dependency_links.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)       49 2024-04-02 10:06:42.000000 temod-2.0.9/src/temod.egg-info/requires.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)        6 2024-04-02 10:06:42.000000 temod-2.0.9/src/temod.egg-info/top_level.txt
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-23 09:46:20.097818 temod-2.1.0/
+-rw-rw-r--   0 oem      (29999) oem      (29999)     1069 2023-07-16 09:53:35.000000 temod-2.1.0/LICENSE.txt
+-rw-r--r--   0 oem      (29999) oem      (29999)      739 2024-05-23 09:46:20.097818 temod-2.1.0/PKG-INFO
+-rw-rw-r--   0 oem      (29999) oem      (29999)       67 2023-07-16 09:51:01.000000 temod-2.1.0/README.md
+-rw-rw-r--   0 oem      (29999) oem      (29999)      734 2024-05-23 09:46:15.000000 temod-2.1.0/pyproject.toml
+-rw-rw-r--   0 oem      (29999) oem      (29999)       38 2024-05-23 09:46:20.097818 temod-2.1.0/setup.cfg
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-23 09:46:20.093818 temod-2.1.0/src/
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-23 09:46:20.097818 temod-2.1.0/src/temod/
+-rw-rw-r--   0 oem      (29999) oem      (29999)       27 2023-07-15 13:43:54.000000 temod-2.1.0/src/temod/__init__.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-23 09:46:20.097818 temod-2.1.0/src/temod/base/
+-rw-rw-r--   0 oem      (29999) oem      (29999)      145 2023-07-15 13:44:09.000000 temod-2.1.0/src/temod/base/__init__.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)    14485 2024-05-23 09:35:56.000000 temod-2.1.0/src/temod/base/attribute.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     1697 2023-07-15 13:44:06.000000 temod-2.1.0/src/temod/base/cluster.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     2900 2023-07-15 13:44:09.000000 temod-2.1.0/src/temod/base/condition.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     1986 2023-07-15 13:44:10.000000 temod-2.1.0/src/temod/base/constraint.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     7248 2024-04-11 15:21:33.000000 temod-2.1.0/src/temod/base/entity.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     1803 2024-04-18 14:32:45.000000 temod-2.1.0/src/temod/base/exceptions.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     2557 2023-07-15 13:44:10.000000 temod-2.1.0/src/temod/base/join.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-23 09:46:20.097818 temod-2.1.0/src/temod/ext/
+-rw-rw-r--   0 oem      (29999) oem      (29999)    11228 2023-07-15 13:43:55.000000 temod-2.1.0/src/temod/ext/holders.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-23 09:46:20.097818 temod-2.1.0/src/temod/operators/
+-rw-rw-r--   0 oem      (29999) oem      (29999)      451 2023-07-15 13:43:22.000000 temod-2.1.0/src/temod/operators/aggregation.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-23 09:46:20.097818 temod-2.1.0/src/temod/storage/
+-rw-rw-r--   0 oem      (29999) oem      (29999)      201 2023-07-15 13:43:59.000000 temod-2.1.0/src/temod/storage/__init__.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-23 09:46:20.097818 temod-2.1.0/src/temod/storage/directory/
+-rw-rw-r--   0 oem      (29999) oem      (29999)       59 2023-07-15 13:43:57.000000 temod-2.1.0/src/temod/storage/directory/__init__.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     5004 2023-07-15 13:43:57.000000 temod-2.1.0/src/temod/storage/directory/directoryStorage.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     7554 2024-05-22 15:50:04.000000 temod-2.1.0/src/temod/storage/directory/yamlStorage.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-23 09:46:20.097818 temod-2.1.0/src/temod/storage/exceptions/
+-rw-rw-r--   0 oem      (29999) oem      (29999)      774 2023-07-15 13:43:58.000000 temod-2.1.0/src/temod/storage/exceptions/entities.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)      541 2023-07-15 13:43:58.000000 temod-2.1.0/src/temod/storage/exceptions/joins.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)      418 2023-07-15 13:43:58.000000 temod-2.1.0/src/temod/storage/exceptions/translators.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-23 09:46:20.097818 temod-2.1.0/src/temod/storage/influxdb/
+-rw-rw-r--   0 oem      (29999) oem      (29999)     9803 2024-02-25 20:41:24.000000 temod-2.1.0/src/temod/storage/influxdb/influxEntityStorage.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     2363 2024-02-25 20:41:37.000000 temod-2.1.0/src/temod/storage/influxdb/influxStorage.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     6019 2023-07-15 13:43:59.000000 temod-2.1.0/src/temod/storage/influxdb/influxTranslators.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-23 09:46:20.097818 temod-2.1.0/src/temod/storage/mysql/
+-rw-rw-r--   0 oem      (29999) oem      (29999)      131 2023-07-15 13:44:05.000000 temod-2.1.0/src/temod/storage/mysql/__init__.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     2596 2024-05-23 09:35:36.000000 temod-2.1.0/src/temod/storage/mysql/mysqlAttributesTranslator.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     6604 2024-02-25 20:41:49.000000 temod-2.1.0/src/temod/storage/mysql/mysqlClusterStorage.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     4235 2023-07-15 13:44:05.000000 temod-2.1.0/src/temod/storage/mysql/mysqlConditionsTranslator.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     9847 2024-04-02 13:14:31.000000 temod-2.1.0/src/temod/storage/mysql/mysqlEntityStorage.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)    10186 2024-05-21 19:46:44.000000 temod-2.1.0/src/temod/storage/mysql/mysqlJoinStorage.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     2148 2024-03-24 12:33:38.000000 temod-2.1.0/src/temod/storage/mysql/mysqlStorage.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-23 09:46:20.097818 temod-2.1.0/src/temod/utils/
+-rw-rw-r--   0 oem      (29999) oem      (29999)     2073 2023-07-15 13:43:23.000000 temod-2.1.0/src/temod/utils/decorators.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     2373 2023-07-15 13:43:23.000000 temod-2.1.0/src/temod/utils/exoskeleton.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)      547 2023-07-15 13:43:24.000000 temod-2.1.0/src/temod/utils/graphs.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-23 09:46:20.097818 temod-2.1.0/src/temod/utils/synchronizer/
+-rw-rw-r--   0 oem      (29999) oem      (29999)       90 2024-05-22 16:03:41.000000 temod-2.1.0/src/temod/utils/synchronizer/__init__.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     1709 2024-05-22 15:49:56.000000 temod-2.1.0/src/temod/utils/synchronizer/simple.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     1905 2024-05-22 16:07:45.000000 temod-2.1.0/src/temod/utils/synchronizer/unidirectional.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-23 09:46:20.097818 temod-2.1.0/src/temod.egg-info/
+-rw-r--r--   0 oem      (29999) oem      (29999)      739 2024-05-23 09:46:20.000000 temod-2.1.0/src/temod.egg-info/PKG-INFO
+-rw-rw-r--   0 oem      (29999) oem      (29999)     1456 2024-05-23 09:46:20.000000 temod-2.1.0/src/temod.egg-info/SOURCES.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)        1 2024-05-23 09:46:20.000000 temod-2.1.0/src/temod.egg-info/dependency_links.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)       70 2024-05-23 09:46:20.000000 temod-2.1.0/src/temod.egg-info/requires.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)        6 2024-05-23 09:46:20.000000 temod-2.1.0/src/temod.egg-info/top_level.txt
```

### Comparing `temod-2.0.9/LICENSE.txt` & `temod-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `temod-2.0.9/PKG-INFO` & `temod-2.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: temod
-Version: 2.0.9
+Version: 2.1.0
 Summary: Data management abstraction layer for your python programs
 Author-email: PyAxolotl <abdellatifzied.saada@gmail.com>
 Project-URL: Homepage, https://github.com/TuburboMajus/temod
 Project-URL: Bug Tracker, https://github.com/TuburboMajus/temod/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: networkx>=3.1
-Requires-Dist: mysql.connector>=2.2.9
+Requires-Dist: mysql-connector-python>=8.3.0
 Requires-Dist: PyYaml>=6.0
+Requires-Dist: bcrypt>=4.1.3
 
 # temod
 Data management abstraction layer for your python programs
```

### Comparing `temod-2.0.9/pyproject.toml` & `temod-2.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "temod"
-version = "2.0.9"
+version = "2.1.0"
 authors = [
   { name="PyAxolotl", email="abdellatifzied.saada@gmail.com" },
 ]
 description = "Data management abstraction layer for your python programs"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.7"
 dependencies = [
     "networkx >= 3.1",
-    "mysql.connector >= 2.2.9",
-    "PyYaml >= 6.0"
+    "mysql-connector-python >= 8.3.0",
+    "PyYaml >= 6.0",
+    "bcrypt >= 4.1.3"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TuburboMajus/temod"
 "Bug Tracker" = "https://github.com/TuburboMajus/temod/issues"
```

### Comparing `temod-2.0.9/src/temod/base/attribute.py` & `temod-2.1.0/src/temod/base/attribute.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from datetime import datetime, date
 from temod.base.exceptions import *
 
 import traceback
+import bcrypt
 import random
 import base64
 import uuid
+import re
 
 ASCII_ALPHABET =  "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ"
 BASE16_ALPHABET = "abcdef0123456789"
 BASE64_ALPHABET = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789+/="
+EMAIL_FORMAT = r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,7}\b'
+PHONE_NUNBER_FORMAT = r'^(\+|00)(?:[0-9] ?){6,14}[0-9]$'
 		
 class Attribute(object):
 	"""docstring for Attribute"""
 	def __init__(self, name, value_type, value=None, is_id=False,is_auto=False,is_nullable=True,default_value=None,force_cast=None,
 		owner=None,owner_name=None,owner_type=None,no_check=False):
 		super(Attribute, self).__init__()
 		self.name = name
@@ -88,14 +92,74 @@
 	def generate_random_value(length):
 		str_ = ""
 		for i in range(length):
 			str_ += ASCII_ALPHABET[random.randint(0,len(ASCII_ALPHABET)-1)]
 		return str_
 
 
+class EmailAttribute(StringAttribute):
+	"""docstring for EmailAttribute"""
+	def __init__(self, *args, **kwargs):
+		super(EmailAttribute, self).__init__(
+			*args, force_lower_case=kwargs.pop("force_lower_case",True), non_empty=kwargs.pop('non_empty',True), 
+			max_length=kwargs.pop("max_length",320),
+			**kwargs
+		)
+		self.check_value()
+
+	def check_value(self):
+		if super(EmailAttribute,self).check_value() is False:
+			return False
+		if self.value is not None:
+			if not re.fullmatch(EMAIL_FORMAT,self.value):
+				raise WrongEmailFormat(self,f"Value of EmailAttribute doesn't comply with email formats (email :{self.value})")
+
+	def set_value(self,value):
+		self.value = value
+		self.check_value()
+
+
+class PhoneNumberAttribute(StringAttribute):
+	"""docstring for PhoneNumberAttribute"""
+	def __init__(self, *args, default_country_code=None, **kwargs):
+		default_country_code = default_country_code.replace('+','') if type(default_country_code) is str else default_country_code
+		super(PhoneNumberAttribute, self).__init__(
+			*args, non_empty=kwargs.pop('non_empty',True), 
+			max_length=kwargs.pop("max_length",16),
+			force_cast=PhoneNumberAttribute.number_transformer(default_country_code),
+			**kwargs
+		)
+		self.check_value()
+
+	def check_value(self):
+		if super(PhoneNumberAttribute,self).check_value() is False:
+			return False
+		if self.value is not None:
+			if not re.fullmatch(PHONE_NUNBER_FORMAT,self.value):
+				raise WrongPhoneNumberFormat(self,f"Value of PhoneNumberAttribute doesn't comply with phone number formats (number :{self.value})")
+
+	def set_value(self,value):
+		self.value = value
+		self.check_value()
+
+	def number_transform(number,default_country_code=None):
+		if number is None:
+			return 
+		n = number.replace(' ','')
+		if n.startswith('00'):
+			n = "+"+n[2:]
+		if not n.startswith('+') and default_country_code is not None:
+			n = "+"+str(default_country_code)+n
+		return n
+
+	def number_transformer(country_code):
+		return lambda x:PhoneNumberAttribute.number_transform(default_country_code=country_code)
+
+
+
 class UUID4Attribute(StringAttribute):
 	"""docstring for UUID4Attribute"""
 	def __init__(self, *args, **kwargs):
 		super(UUID4Attribute, self).__init__(*args, non_empty=kwargs.pop('non_empty',True), **kwargs)
 		self.check_value()
 
 	def check_value(self):
@@ -290,8 +354,64 @@
 		return self.value
 
 	def cast(value):
 		if not value is None:
 			try:
 				return int(value)
 			except:
-				return self.reversed[value]
+				return self.reversed[value]
+
+
+class BytesAttribute(Attribute):
+	"""docstring for BytesAttribute"""
+	def __init__(self, name, non_empty=False,force_lower_case=False,length=None,max_length=None,min_length=None,**kwargs):
+		super(BytesAttribute, self).__init__(name, bytearray, **kwargs)
+		self.length = length
+		self.max_length = max_length if length is None else length
+		self.min_length = min_length if length is None else length
+		self.non_empty = non_empty
+		self.force_lower_case = force_lower_case
+		self.check_value()
+		if force_lower_case and self.value is not None:
+			self.value = self.value.lower()
+
+	def check_value(self):
+		if super(BytesAttribute,self).check_value() is False:
+			return False
+		if self.non_empty and self.value == b"":
+			raise EmptyStringError(self,"Value of non empty BytesAttribute set to null or empty bytes")
+		if self.value is not None and self.max_length is not None:
+			if len(self.value) > self.max_length:
+				raise OverMaxLengthError(
+					self,f"Value of BytesAttribute exceeds the max_length allowed. (value: {self.value}, max_length: {self.max_length})"
+				)
+		if self.value is not None and self.min_length is not None:
+			if len(self.value) < self.min_length:
+				raise BelowMinLengthError(
+					self,f"Value of BytesAttribute doesn't comply with the min_length needed. (value: {self.value}, max_length: {self.min_length})"
+				)
+
+
+class BCryptedAttribute(BytesAttribute):
+	"""docstring for BCryptedAttribute"""
+	def __init__(self, name, salt=None, encoding="utf-8", **kwargs):
+		super(BCryptedAttribute, self).__init__(name, **kwargs)
+		self.encoding = encoding
+		self.salt = salt
+
+	def set_value(self,value):
+		if type(value) is str:
+			if self.salt is None:
+				self.salt = bcrypt.gensalt()
+			self.value = bytearray(bcrypt.hashpw(value.encode(self.encoding), self.salt))
+		else:
+			self.value = value
+		self.check_value()
+
+	def __eq__(self, value):
+		if value is None:
+			return self.value is None
+		if type(value) is str:
+			return bcrypt.checkpw(value.encode(self.encoding), bytes(self.value))
+		elif issubclass(type(value),StringAttribute):
+			return (self.value is None and value.value is None) or bcrypt.checkpw(value.encode(self.encoding), bytes(self.value))
+		return False
```

### Comparing `temod-2.0.9/src/temod/base/cluster.py` & `temod-2.1.0/src/temod/base/cluster.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.9/src/temod/base/condition.py` & `temod-2.1.0/src/temod/base/condition.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.9/src/temod/base/constraint.py` & `temod-2.1.0/src/temod/base/constraint.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.9/src/temod/base/entity.py` & `temod-2.1.0/src/temod/base/entity.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from .attribute import Attribute
 
+class DuplicateNameError(Exception):
+	pass
+
 class MalformedEntityException(Exception):
-	"""docstring for MalformedEntityException"""
-	def __init__(self, *args, **kwargs):
-		super(MalformedEntityException, self).__init__(*args, **kwargs)
+	pass
 
 class MissingRequiredAttributeError(Exception):
-	"""docstring for MissingRequiredAttributeError"""
-	def __init__(self, *args, **kwargs):
-		super(MissingRequiredAttributeError, self).__init__(*args, **kwargs)
+	pass
 
 
 class Entity(object):
 	"""docstring for Entity"""
 	def __init__(self, *attributes,**kwargs):
 		super(Entity, self).__init__()
 		self.attributes = {}
+		self.complements = {}
 		self.snapshot = None
 		for i,attribute in enumerate(attributes):
 			if issubclass(type(attribute),Attribute):
 				self.attributes[attribute.name] = attribute
 			else:
 				self.attributes[self.ATTRIBUTES[i]['name']] = self.ATTRIBUTES[i]['type'](
 					self.ATTRIBUTES[i]['name'],value=attribute,
@@ -49,16 +49,45 @@
 	def setAttribute(self,attribute: str,value):
 		self.attributes[attribute].set_value(value)
 
 	def setAttributes(self,**kwargs):
 		for k,v in kwargs.items():
 			self.attributes[k].set_value(v)
 
+	def setInfo(self, info: str, value):
+		if info in self.attributes:
+			raise DuplicateNameError("Complementary infos cannot share names with base attributes.")
+		self.complements[info] = value
+
+	def setInfos(self, **complements):
+		for complement, value in complements.items():
+			self.setInfo(complement, value)
+
+	def scalarizeInfo(self, value, complements=False):
+		if value is None:
+			return None
+		if(type(value) in [dict, str, int, float, bool]):
+			return value
+		if type(value) in [list, set]:
+			return [self.scalarizeInfo(element, complements=complements) for element in value]
+		if (issubclass(type(value), Attribute)):
+			return value.to_scalar()
+		if (issubclass(type(value), Entity)):
+			return value.to_dict(complements=complements)
+		raise Exception(f"Cannot scalarize info of type {type(value)}")
+
 	def __getitem__(self,name):
-		return self.attributes[name].value
+		try:
+			return self.attributes[name].value
+		except Exception as e:
+			try:
+				return self.complements[name]
+			except:
+				pass
+			raise e
 
 	def __setitem__(self,name,value): 
 		return self.setAttribute(name,value)
 
 	#####################################################
 
 	def takeSnapshot(self):
@@ -66,19 +95,25 @@
 			name:type(attribute)(attribute.name,value=attribute.value)
 			for name,attribute in self.attributes.items()
 		}
 		return self
 
 	#####################################################
 
-	def to_dict(self,include=None):
-		return {
+	def to_dict(self,include=None, complements=False, translator=None):
+		dct = {}
+		if complements:
+			dct = {complement: self.scalarizeInfo(value, complements=True) for complement, value in self.complements.items()}
+		dct.update({
 			name:attr.to_scalar() if attr.value is not None else None
 			for name,attr in self.attributes.items() if include is None or name in include
-		}
+		})
+		if translator is not None:
+			return {translator.get(k,k):v for k,v in dct.items()}
+		return dct
 
 	def name(self):
 		return getattr(self,'ENTITY_NAME',type(self).__name__)
 
 	def __repr__(self):
 		attributes = [f"{attr.name} ({type(attr).__name__}): {attr.value} ({type(attr.value).__name__})" for attr in self.attributes.values()]
 		return f"""Entity {self.ENTITY_NAME}"""+((":\n\t"+"\n\t".join(attributes)) if len(self.attributes) > 0 else "")
@@ -164,8 +199,7 @@
 		return dct
 
 	def __repr__(self):
 		attributes = [f"{attr.name} ({type(attr).__name__}): {attr.value} ({type(attr.value).__name__})" for attr in self.attributes.values()]
 		return f"""Auto Completed Entity {self.ENTITY_NAME}"""+((":\n\t"+"\n\t".join(attributes)) if len(self.attributes) > 0 else "")
 
 	#####################################################
-
```

### Comparing `temod-2.0.9/src/temod/base/exceptions.py` & `temod-2.1.0/src/temod/base/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -52,8 +52,24 @@
 DATE_ERROR_CODE = "0x3"
 
 class DateOverBoundError(AttributeValueException):
 	CODE = DATE_ERROR_CODE+"0"
 
 class DateBelowBoundError(AttributeValueException):
 	CODE = DATE_ERROR_CODE+"1"
+
+
+""" EmailAttribute Exceptions"""
+
+EMAIL_ERROR_CODE = "0x4"
+
+class WrongEmailFormat(AttributeValueException):
+	CODE = EMAIL_ERROR_CODE+"0"
+
+
+""" PhoneNumberAttribute Exceptions"""
+
+PHONE_NUMBER_ERROR_CODE = "0x5"
+
+class WrongPhoneNumberFormat(AttributeValueException):
+	CODE = PHONE_NUMBER_ERROR_CODE+"0"
```

### Comparing `temod-2.0.9/src/temod/base/join.py` & `temod-2.1.0/src/temod/base/join.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.9/src/temod/ext/holders.py` & `temod-2.1.0/src/temod/ext/holders.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.9/src/temod/storage/directory/directoryStorage.py` & `temod-2.1.0/src/temod/storage/directory/directoryStorage.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.9/src/temod/storage/exceptions/entities.py` & `temod-2.1.0/src/temod/storage/exceptions/entities.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.9/src/temod/storage/exceptions/joins.py` & `temod-2.1.0/src/temod/storage/exceptions/joins.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.9/src/temod/storage/influxdb/influxEntityStorage.py` & `temod-2.1.0/src/temod/storage/influxdb/influxEntityStorage.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.9/src/temod/storage/influxdb/influxStorage.py` & `temod-2.1.0/src/temod/storage/influxdb/influxStorage.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.9/src/temod/storage/influxdb/influxTranslators.py` & `temod-2.1.0/src/temod/storage/influxdb/influxTranslators.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.9/src/temod/storage/mysql/mysqlAttributesTranslator.py` & `temod-2.1.0/src/temod/storage/mysql/mysqlAttributesTranslator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from temod.base.attribute import *
 
+import binascii
 import base64
 
 STRING_ESCAPE = str.maketrans({'"':  r'\"'})
 
 class MysqlAttributeException(Exception):
 	"""docstring for MysqlAttributeException"""
 	def __init__(self, *args, **kwargs):
@@ -11,42 +12,45 @@
 
 class MysqlAttributesTranslator(object):
 	"""docstring for MysqlAttributesTranslator"""
 
 	def translate(attribute):
 		if attribute.value is None:
 			return "null"
-		if type(attribute) is StringAttribute:
+		if type(attribute) in [StringAttribute, EmailAttribute, PhoneNumberAttribute, UUID4Attribute]:
 			return MysqlAttributesTranslator.translateString(attribute)
+		if type(attribute) in [BytesAttribute, BCryptedAttribute]:
+			return MysqlAttributesTranslator.translateBytes(attribute)
 		elif type(attribute) is IntegerAttribute:
 			return MysqlAttributesTranslator.translateInteger(attribute)
 		elif type(attribute) is RealAttribute:
 			return MysqlAttributesTranslator.translateReal(attribute)
 		elif type(attribute) is BooleanAttribute:
 			return MysqlAttributesTranslator.translateBool(attribute)
 		elif type(attribute) is DateAttribute:
 			return MysqlAttributesTranslator.translateDate(attribute)
 		elif type(attribute) is DateTimeAttribute:
 			return MysqlAttributesTranslator.translateDatetime(attribute)
-		elif type(attribute) is UUID4Attribute:
-			return MysqlAttributesTranslator.translateString(attribute)
 		elif type(attribute) is UTF8BASE64Attribute:
 			return MysqlAttributesTranslator.translateBase64UTF8(attribute)
 		elif type(attribute) is RangeAttribute:
 			return MysqlAttributesTranslator.translateInteger(attribute)
 		else:
 			raise MysqlAttributeException(f"Can't translate attribute of type {type(attribute).__name__}")
 
 	####################################
 	# BASIC TRANSLATORS
 	####################################
 
 	def translateString(attribute):
 		return f'"{attribute.value.translate(STRING_ESCAPE)}"'
 
+	def translateBytes(attribute):
+		return f'0x{binascii.hexlify(attribute.value).decode()}'
+
 	def translateInteger(attribute):
 		return str(attribute.value)
 
 	def translateReal(attribute):
 		return str(attribute.value)
 
 	def translateBool(attribute):
@@ -59,10 +63,8 @@
 	def translateDate(attribute):
 		return f'"{attribute.value.strftime("%Y-%m-%d")}"'
 
 	def translateDatetime(attribute):
 		return f'"{attribute.value.strftime("%Y-%m-%d %H:%M:%S")}"'
 
 	def translateBase64UTF8(attribute):
-		return f'"{base64.b64encode(attribute.value.encode()).decode("utf-8")}"'
-
-		
+		return f'"{base64.b64encode(attribute.value.encode()).decode("utf-8")}"'
```

### Comparing `temod-2.0.9/src/temod/storage/mysql/mysqlClusterStorage.py` & `temod-2.1.0/src/temod/storage/mysql/mysqlClusterStorage.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.9/src/temod/storage/mysql/mysqlConditionsTranslator.py` & `temod-2.1.0/src/temod/storage/mysql/mysqlConditionsTranslator.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.9/src/temod/storage/mysql/mysqlEntityStorage.py` & `temod-2.1.0/src/temod/storage/mysql/mysqlEntityStorage.py`

 * *Files 5% similar despite different names*

```diff
@@ -191,20 +191,23 @@
 	def update(self,updates,*conditions,limit=None,skip=None,updateID=False,**kwargs):
 		condition = self._build_condition(*conditions,**kwargs)
 		try:
 			assert(updates is not None and len(updates) > 0)
 		except:
 			raise EntityStorageException("At least one attribute to update is necessary")
 		if type(updates) is dict:
-			updates = [
+			attributes = [
 				attr['type'](name,value=updates[name],**{k:v for k,v in attr.items() if not k in ['type','required']})
 				for name,attr in self.entity_attributes.items() if name in updates
 			]
-		toUpdate = [Equals(update) if not issubclass(type(update),Equals) else update for update in updates]
-		query = f"UPDATE {self.entity_name} SET {','.join([MysqlAttributeTranslator.translate(update) for update in toUpdate])}"
+		elif issubclass(type(updates),Attribute):
+			attributes = [updates]
+		else:
+			raise Exception("Updates must be a dict or an Attribute")
+		query = f"UPDATE {self.entity_name} SET {','.join([attribute.name+' = '+MysqlAttributesTranslator.translate(attribute) for attribute in attributes])}"
 		if condition is not None:
 			query +=  f" WHERE {MysqlConditionsTranslator.translate(condition)}"
 		if skip is not None:
 			query += f" SKIP {skip}"
 		if limit is not None:
 			query += f" LIMIT {limit}"
 		return self.executeAndCommit(query).lastrowid
```

### Comparing `temod-2.0.9/src/temod/storage/mysql/mysqlJoinStorage.py` & `temod-2.1.0/src/temod/storage/mysql/mysqlJoinStorage.py`

 * *Files 4% similar despite different names*

```diff
@@ -225,14 +225,28 @@
 				except:
 					# Check if this might be caused by a left or right join
 					if i == 0 or list_[i][2] == "":
 						raise
 				i += 1
 			yield self.join_type(*to_join,**getattr(self.join_type,'SHORTCUTS',{}))
 
+
+	def count(self,*conditions,skip=None,entry=None,**kwargs):
+		entry = self.default_entry if (entry is None) else entry
+		condition = self._build_condition(entry, *conditions,**kwargs)
+		list_ = self._build_entities_list(entry)
+		entities = [list_[0]]+[entity[0] for entity in list_[1:]]
+		entities_names = [(entity.ENTITY_NAME if hasattr(entity,"ENTITY_NAME") else entity.__name__) for entity in entities]
+
+		query = f"SELECT count(*) as counted FROM {getattr(list_[0],'ENTITY_NAME',list_[0].__name__)} {self._build_join(list_[1:])}"
+		if condition is not None:
+			query += f" WHERE {MysqlConditionsTranslator.translate(condition)}"
+
+		return self.getOne(query)['counted']
+
 	#############################################
 
 	def updateOnSnapshot(self,join,updateID=False):
 		if not type(join) is self.join_type:
 			raise JoinStorageException(f'Cannot store {type(join)} into a MysqlJoinStorage of {self.join_type}')
 
 		if any([not hasattr(entity,"snapshot") for entity in join.entities.values()]):
```

### Comparing `temod-2.0.9/src/temod/storage/mysql/mysqlStorage.py` & `temod-2.1.0/src/temod/storage/mysql/mysqlStorage.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.9/src/temod/utils/decorators.py` & `temod-2.1.0/src/temod/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.9/src/temod/utils/exoskeleton.py` & `temod-2.1.0/src/temod/utils/exoskeleton.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.9/src/temod/utils/graphs.py` & `temod-2.1.0/src/temod/utils/graphs.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.9/src/temod.egg-info/PKG-INFO` & `temod-2.1.0/src/temod.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: temod
-Version: 2.0.9
+Version: 2.1.0
 Summary: Data management abstraction layer for your python programs
 Author-email: PyAxolotl <abdellatifzied.saada@gmail.com>
 Project-URL: Homepage, https://github.com/TuburboMajus/temod
 Project-URL: Bug Tracker, https://github.com/TuburboMajus/temod/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: networkx>=3.1
-Requires-Dist: mysql.connector>=2.2.9
+Requires-Dist: mysql-connector-python>=8.3.0
 Requires-Dist: PyYaml>=6.0
+Requires-Dist: bcrypt>=4.1.3
 
 # temod
 Data management abstraction layer for your python programs
```

### Comparing `temod-2.0.9/src/temod.egg-info/SOURCES.txt` & `temod-2.1.0/src/temod.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -32,8 +32,11 @@
 src/temod/storage/mysql/mysqlClusterStorage.py
 src/temod/storage/mysql/mysqlConditionsTranslator.py
 src/temod/storage/mysql/mysqlEntityStorage.py
 src/temod/storage/mysql/mysqlJoinStorage.py
 src/temod/storage/mysql/mysqlStorage.py
 src/temod/utils/decorators.py
 src/temod/utils/exoskeleton.py
-src/temod/utils/graphs.py
+src/temod/utils/graphs.py
+src/temod/utils/synchronizer/__init__.py
+src/temod/utils/synchronizer/simple.py
+src/temod/utils/synchronizer/unidirectional.py
```

