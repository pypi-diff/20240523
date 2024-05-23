# Comparing `tmp/dagster_looker-0.23.6.tar.gz` & `tmp/dagster_looker-0.23.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_looker-0.23.6.tar", last modified: Thu May 16 20:15:40 2024, max compression
+gzip compressed data, was "dagster_looker-0.23.7.tar", last modified: Thu May 23 20:59:08 2024, max compression
```

## Comparing `dagster_looker-0.23.6.tar` & `dagster_looker-0.23.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:15:40.316416 dagster_looker-0.23.6/
--rw-r--r--   0 root         (0) root         (0)    11347 2024-05-16 20:06:23.000000 dagster_looker-0.23.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       66 2024-05-16 20:06:23.000000 dagster_looker-0.23.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      622 2024-05-16 20:15:40.316416 dagster_looker-0.23.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      129 2024-05-16 20:06:23.000000 dagster_looker-0.23.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:15:40.312416 dagster_looker-0.23.6/dagster_looker/
--rw-r--r--   0 root         (0) root         (0)      379 2024-05-16 20:06:23.000000 dagster_looker-0.23.6/dagster_looker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1366 2024-05-16 20:06:23.000000 dagster_looker-0.23.6/dagster_looker/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     3805 2024-05-16 20:06:23.000000 dagster_looker-0.23.6/dagster_looker/asset_utils.py
--rw-r--r--   0 root         (0) root         (0)    17128 2024-05-16 20:06:23.000000 dagster_looker-0.23.6/dagster_looker/dagster_looker_translator.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-16 20:06:23.000000 dagster_looker-0.23.6/dagster_looker/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-16 20:06:23.000000 dagster_looker-0.23.6/dagster_looker/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:15:40.316416 dagster_looker-0.23.6/dagster_looker.egg-info/
--rw-r--r--   0 root         (0) root         (0)      622 2024-05-16 20:15:40.000000 dagster_looker-0.23.6/dagster_looker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      459 2024-05-16 20:15:40.000000 dagster_looker-0.23.6/dagster_looker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:15:40.000000 dagster_looker-0.23.6/dagster_looker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:15:40.000000 dagster_looker-0.23.6/dagster_looker.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       28 2024-05-16 20:15:40.000000 dagster_looker-0.23.6/dagster_looker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-16 20:15:40.000000 dagster_looker-0.23.6/dagster_looker.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      161 2024-05-16 20:15:40.316416 dagster_looker-0.23.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1299 2024-05-16 20:06:23.000000 dagster_looker-0.23.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:59:08.939180 dagster_looker-0.23.7/
+-rw-r--r--   0 root         (0) root         (0)    11347 2024-05-23 20:50:32.000000 dagster_looker-0.23.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-23 20:50:32.000000 dagster_looker-0.23.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      622 2024-05-23 20:59:08.939180 dagster_looker-0.23.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      129 2024-05-23 20:50:32.000000 dagster_looker-0.23.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:59:08.939180 dagster_looker-0.23.7/dagster_looker/
+-rw-r--r--   0 root         (0) root         (0)      379 2024-05-23 20:50:32.000000 dagster_looker-0.23.7/dagster_looker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1366 2024-05-23 20:50:32.000000 dagster_looker-0.23.7/dagster_looker/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     3805 2024-05-23 20:50:32.000000 dagster_looker-0.23.7/dagster_looker/asset_utils.py
+-rw-r--r--   0 root         (0) root         (0)    17128 2024-05-23 20:50:32.000000 dagster_looker-0.23.7/dagster_looker/dagster_looker_translator.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-23 20:50:32.000000 dagster_looker-0.23.7/dagster_looker/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-23 20:50:32.000000 dagster_looker-0.23.7/dagster_looker/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:59:08.939180 dagster_looker-0.23.7/dagster_looker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      622 2024-05-23 20:59:08.000000 dagster_looker-0.23.7/dagster_looker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      459 2024-05-23 20:59:08.000000 dagster_looker-0.23.7/dagster_looker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:59:08.000000 dagster_looker-0.23.7/dagster_looker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:59:08.000000 dagster_looker-0.23.7/dagster_looker.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-23 20:59:08.000000 dagster_looker-0.23.7/dagster_looker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-23 20:59:08.000000 dagster_looker-0.23.7/dagster_looker.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2024-05-23 20:59:08.943180 dagster_looker-0.23.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1299 2024-05-23 20:50:32.000000 dagster_looker-0.23.7/setup.py
```

### Comparing `dagster_looker-0.23.6/LICENSE` & `dagster_looker-0.23.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster_looker-0.23.6/PKG-INFO` & `dagster_looker-0.23.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster_looker
-Version: 0.23.6
+Version: 0.23.7
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-looker
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dagster_looker-0.23.6/dagster_looker/asset_decorator.py` & `dagster_looker-0.23.7/dagster_looker/asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster_looker-0.23.6/dagster_looker/asset_utils.py` & `dagster_looker-0.23.7/dagster_looker/asset_utils.py`

 * *Files identical despite different names*

### Comparing `dagster_looker-0.23.6/dagster_looker/dagster_looker_translator.py` & `dagster_looker-0.23.7/dagster_looker/dagster_looker_translator.py`

 * *Files identical despite different names*

### Comparing `dagster_looker-0.23.6/dagster_looker.egg-info/PKG-INFO` & `dagster_looker-0.23.7/dagster_looker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-looker
-Version: 0.23.6
+Version: 0.23.7
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-looker
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dagster_looker-0.23.6/setup.py` & `dagster_looker-0.23.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,13 +33,13 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_looker_tests*"]),
     install_requires=[
-        "dagster==1.7.6",
+        "dagster==1.7.7",
         "lkml",
         "sqlglot",
     ],
     zip_safe=False,
 )
```

