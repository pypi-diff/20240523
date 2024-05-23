# Comparing `tmp/dagster-duckdb-0.23.6.tar.gz` & `tmp/dagster-duckdb-0.23.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-0.23.6.tar", last modified: Thu May 16 20:13:40 2024, max compression
+gzip compressed data, was "dagster-duckdb-0.23.7.tar", last modified: Thu May 23 20:57:11 2024, max compression
```

## Comparing `dagster-duckdb-0.23.6.tar` & `dagster-duckdb-0.23.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:13:40.484081 dagster-duckdb-0.23.6/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-16 20:06:23.000000 dagster-duckdb-0.23.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       48 2024-05-16 20:06:23.000000 dagster-duckdb-0.23.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      678 2024-05-16 20:13:40.484081 dagster-duckdb-0.23.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2024-05-16 20:06:23.000000 dagster-duckdb-0.23.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:13:40.484081 dagster-duckdb-0.23.6/dagster_duckdb/
--rw-r--r--   0 root         (0) root         (0)      336 2024-05-16 20:06:23.000000 dagster-duckdb-0.23.6/dagster_duckdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12026 2024-05-16 20:06:23.000000 dagster-duckdb-0.23.6/dagster_duckdb/io_manager.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-16 20:06:23.000000 dagster-duckdb-0.23.6/dagster_duckdb/py.typed
--rw-r--r--   0 root         (0) root         (0)     1716 2024-05-16 20:06:23.000000 dagster-duckdb-0.23.6/dagster_duckdb/resource.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-16 20:06:23.000000 dagster-duckdb-0.23.6/dagster_duckdb/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:13:40.484081 dagster-duckdb-0.23.6/dagster_duckdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      678 2024-05-16 20:13:40.000000 dagster-duckdb-0.23.6/dagster_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      407 2024-05-16 20:13:40.000000 dagster-duckdb-0.23.6/dagster_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:13:40.000000 dagster-duckdb-0.23.6/dagster_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:13:40.000000 dagster-duckdb-0.23.6/dagster_duckdb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       61 2024-05-16 20:13:40.000000 dagster-duckdb-0.23.6/dagster_duckdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-16 20:13:40.000000 dagster-duckdb-0.23.6/dagster_duckdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      125 2024-05-16 20:13:40.484081 dagster-duckdb-0.23.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1399 2024-05-16 20:06:23.000000 dagster-duckdb-0.23.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:57:11.488172 dagster-duckdb-0.23.7/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-23 20:50:32.000000 dagster-duckdb-0.23.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-23 20:50:32.000000 dagster-duckdb-0.23.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      678 2024-05-23 20:57:11.488172 dagster-duckdb-0.23.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2024-05-23 20:50:32.000000 dagster-duckdb-0.23.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:57:11.488172 dagster-duckdb-0.23.7/dagster_duckdb/
+-rw-r--r--   0 root         (0) root         (0)      336 2024-05-23 20:50:32.000000 dagster-duckdb-0.23.7/dagster_duckdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12026 2024-05-23 20:50:32.000000 dagster-duckdb-0.23.7/dagster_duckdb/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-23 20:50:32.000000 dagster-duckdb-0.23.7/dagster_duckdb/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-05-23 20:50:32.000000 dagster-duckdb-0.23.7/dagster_duckdb/resource.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-23 20:50:32.000000 dagster-duckdb-0.23.7/dagster_duckdb/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:57:11.488172 dagster-duckdb-0.23.7/dagster_duckdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      678 2024-05-23 20:57:11.000000 dagster-duckdb-0.23.7/dagster_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      407 2024-05-23 20:57:11.000000 dagster-duckdb-0.23.7/dagster_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:57:11.000000 dagster-duckdb-0.23.7/dagster_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:57:11.000000 dagster-duckdb-0.23.7/dagster_duckdb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       61 2024-05-23 20:57:11.000000 dagster-duckdb-0.23.7/dagster_duckdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-23 20:57:11.000000 dagster-duckdb-0.23.7/dagster_duckdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      125 2024-05-23 20:57:11.488172 dagster-duckdb-0.23.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1399 2024-05-23 20:50:32.000000 dagster-duckdb-0.23.7/setup.py
```

### Comparing `dagster-duckdb-0.23.6/LICENSE` & `dagster-duckdb-0.23.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.23.6/PKG-INFO` & `dagster-duckdb-0.23.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb
-Version: 0.23.6
+Version: 0.23.7
 Summary: Package for DuckDB-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-0.23.6/dagster_duckdb/io_manager.py` & `dagster-duckdb-0.23.7/dagster_duckdb/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.23.6/dagster_duckdb/resource.py` & `dagster-duckdb-0.23.7/dagster_duckdb/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.23.6/dagster_duckdb.egg-info/PKG-INFO` & `dagster-duckdb-0.23.7/dagster_duckdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb
-Version: 0.23.6
+Version: 0.23.7
 Summary: Package for DuckDB-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-0.23.6/setup.py` & `dagster-duckdb-0.23.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
         "duckdb",
-        "dagster==1.7.6",
+        "dagster==1.7.7",
     ],
     extras_require={
         "pandas": [
             "pandas",
         ],
         "pyspark": ["pyspark>=3"],
     },
```

