# Comparing `tmp/dagster-gcp-pandas-0.23.6.tar.gz` & `tmp/dagster-gcp-pandas-0.23.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-gcp-pandas-0.23.6.tar", last modified: Thu May 16 20:17:46 2024, max compression
+gzip compressed data, was "dagster-gcp-pandas-0.23.7.tar", last modified: Thu May 23 21:41:32 2024, max compression
```

## Comparing `dagster-gcp-pandas-0.23.6.tar` & `dagster-gcp-pandas-0.23.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:17:46.796784 dagster-gcp-pandas-0.23.6/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-16 20:06:23.000000 dagster-gcp-pandas-0.23.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-16 20:06:23.000000 dagster-gcp-pandas-0.23.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      735 2024-05-16 20:17:46.796784 dagster-gcp-pandas-0.23.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      140 2024-05-16 20:06:23.000000 dagster-gcp-pandas-0.23.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:17:46.796784 dagster-gcp-pandas-0.23.6/dagster_gcp_pandas/
--rw-r--r--   0 root         (0) root         (0)      394 2024-05-16 20:06:23.000000 dagster-gcp-pandas-0.23.6/dagster_gcp_pandas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:17:46.796784 dagster-gcp-pandas-0.23.6/dagster_gcp_pandas/bigquery/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:23.000000 dagster-gcp-pandas-0.23.6/dagster_gcp_pandas/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11335 2024-05-16 20:06:23.000000 dagster-gcp-pandas-0.23.6/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-16 20:06:23.000000 dagster-gcp-pandas-0.23.6/dagster_gcp_pandas/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-16 20:06:23.000000 dagster-gcp-pandas-0.23.6/dagster_gcp_pandas/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:17:46.796784 dagster-gcp-pandas-0.23.6/dagster_gcp_pandas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      735 2024-05-16 20:17:46.000000 dagster-gcp-pandas-0.23.6/dagster_gcp_pandas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      487 2024-05-16 20:17:46.000000 dagster-gcp-pandas-0.23.6/dagster_gcp_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:17:46.000000 dagster-gcp-pandas-0.23.6/dagster_gcp_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:17:46.000000 dagster-gcp-pandas-0.23.6/dagster_gcp_pandas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       61 2024-05-16 20:17:46.000000 dagster-gcp-pandas-0.23.6/dagster_gcp_pandas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-05-16 20:17:46.000000 dagster-gcp-pandas-0.23.6/dagster_gcp_pandas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      165 2024-05-16 20:17:46.800784 dagster-gcp-pandas-0.23.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1448 2024-05-16 20:06:23.000000 dagster-gcp-pandas-0.23.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:41:32.805880 dagster-gcp-pandas-0.23.7/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-23 21:36:17.000000 dagster-gcp-pandas-0.23.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-23 21:36:17.000000 dagster-gcp-pandas-0.23.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      735 2024-05-23 21:41:32.805880 dagster-gcp-pandas-0.23.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      140 2024-05-23 21:36:17.000000 dagster-gcp-pandas-0.23.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:41:32.805880 dagster-gcp-pandas-0.23.7/dagster_gcp_pandas/
+-rw-r--r--   0 root         (0) root         (0)      394 2024-05-23 21:36:17.000000 dagster-gcp-pandas-0.23.7/dagster_gcp_pandas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:41:32.805880 dagster-gcp-pandas-0.23.7/dagster_gcp_pandas/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 21:36:17.000000 dagster-gcp-pandas-0.23.7/dagster_gcp_pandas/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11335 2024-05-23 21:36:17.000000 dagster-gcp-pandas-0.23.7/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-23 21:36:17.000000 dagster-gcp-pandas-0.23.7/dagster_gcp_pandas/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-23 21:36:17.000000 dagster-gcp-pandas-0.23.7/dagster_gcp_pandas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:41:32.805880 dagster-gcp-pandas-0.23.7/dagster_gcp_pandas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      735 2024-05-23 21:41:32.000000 dagster-gcp-pandas-0.23.7/dagster_gcp_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      487 2024-05-23 21:41:32.000000 dagster-gcp-pandas-0.23.7/dagster_gcp_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 21:41:32.000000 dagster-gcp-pandas-0.23.7/dagster_gcp_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 21:41:32.000000 dagster-gcp-pandas-0.23.7/dagster_gcp_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       61 2024-05-23 21:41:32.000000 dagster-gcp-pandas-0.23.7/dagster_gcp_pandas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-23 21:41:32.000000 dagster-gcp-pandas-0.23.7/dagster_gcp_pandas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      165 2024-05-23 21:41:32.809880 dagster-gcp-pandas-0.23.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1448 2024-05-23 21:36:17.000000 dagster-gcp-pandas-0.23.7/setup.py
```

### Comparing `dagster-gcp-pandas-0.23.6/LICENSE` & `dagster-gcp-pandas-0.23.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-gcp-pandas-0.23.6/PKG-INFO` & `dagster-gcp-pandas-0.23.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-gcp-pandas
-Version: 0.23.6
+Version: 0.23.7
 Summary: Package for storing Pandas DataFrames in GCP.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pandas
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-gcp-pandas-0.23.6/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py` & `dagster-gcp-pandas-0.23.7/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-pandas-0.23.6/dagster_gcp_pandas.egg-info/PKG-INFO` & `dagster-gcp-pandas-0.23.7/dagster_gcp_pandas.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-gcp-pandas
-Version: 0.23.6
+Version: 0.23.7
 Summary: Package for storing Pandas DataFrames in GCP.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pandas
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-gcp-pandas-0.23.6/setup.py` & `dagster-gcp-pandas-0.23.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,14 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_gcp_pandas_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.6",
-        "dagster-gcp==0.23.6",
+        "dagster==1.7.7",
+        "dagster-gcp==0.23.7",
         "pandas",
     ],
     extras_require={"test": ["pandas-gbq"]},
     zip_safe=False,
 )
```

