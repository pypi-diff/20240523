# Comparing `tmp/ndpprep-0.0.5.tar.gz` & `tmp/ndpprep-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndpprep-0.0.5.tar", last modified: Mon May 20 11:52:59 2024, max compression
+gzip compressed data, was "ndpprep-0.0.8.tar", last modified: Thu May 23 09:01:34 2024, max compression
```

## Comparing `ndpprep-0.0.5.tar` & `ndpprep-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:52:59.220123 ndpprep-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-20 11:52:59.220123 ndpprep-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-20 11:52:55.000000 ndpprep-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-20 11:52:55.000000 ndpprep-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 11:52:59.220123 ndpprep-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:52:59.216123 ndpprep-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:52:59.220123 ndpprep-0.0.5/src/ndpprep/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:52:55.000000 ndpprep-0.0.5/src/ndpprep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-20 11:52:55.000000 ndpprep-0.0.5/src/ndpprep/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:52:59.220123 ndpprep-0.0.5/src/ndpprep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-20 11:52:59.000000 ndpprep-0.0.5/src/ndpprep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-20 11:52:59.000000 ndpprep-0.0.5/src/ndpprep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:52:59.000000 ndpprep-0.0.5/src/ndpprep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 11:52:59.000000 ndpprep-0.0.5/src/ndpprep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 11:52:59.000000 ndpprep-0.0.5/src/ndpprep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 11:52:59.000000 ndpprep-0.0.5/src/ndpprep.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:34.500280 ndpprep-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-23 09:01:34.500280 ndpprep-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-23 09:01:30.000000 ndpprep-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-23 09:01:30.000000 ndpprep-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 09:01:34.500280 ndpprep-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:34.492281 ndpprep-0.0.8/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:34.496281 ndpprep-0.0.8/src/ndpprep/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:34.496281 ndpprep-0.0.8/src/ndpprep/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/cli/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:34.496281 ndpprep-0.0.8/src/ndpprep/decryption/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/decryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/decryption/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:34.496281 ndpprep-0.0.8/src/ndpprep/encryption/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/encryption/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:34.496281 ndpprep-0.0.8/src/ndpprep/inventory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/inventory/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:34.496281 ndpprep-0.0.8/src/ndpprep/masked/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/masked/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/masked/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:34.496281 ndpprep-0.0.8/src/ndpprep/process_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/process_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10080 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/process_data/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:34.500280 ndpprep-0.0.8/src/ndpprep/save_sftp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/save_sftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/save_sftp/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:34.500280 ndpprep-0.0.8/src/ndpprep/secret_key/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/secret_key/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/secret_key/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:34.500280 ndpprep-0.0.8/src/ndpprep/shp_file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/shp_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/shp_file/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13630 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/shp_file/mygeospatial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:34.500280 ndpprep-0.0.8/src/ndpprep/target_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/target_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   117931 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/target_schema/granite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22583 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/target_schema/neps.py
+-rw-r--r--   0 runner    (1001) docker     (127)   171975 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/target_schema/nis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:34.500280 ndpprep-0.0.8/src/ndpprep/unmask/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/unmask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-23 09:01:30.000000 ndpprep-0.0.8/src/ndpprep/unmask/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:01:34.500280 ndpprep-0.0.8/src/ndpprep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-23 09:01:34.000000 ndpprep-0.0.8/src/ndpprep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-23 09:01:34.000000 ndpprep-0.0.8/src/ndpprep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:01:34.000000 ndpprep-0.0.8/src/ndpprep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 09:01:34.000000 ndpprep-0.0.8/src/ndpprep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-23 09:01:34.000000 ndpprep-0.0.8/src/ndpprep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-23 09:01:34.000000 ndpprep-0.0.8/src/ndpprep.egg-info/top_level.txt
```

### Comparing `ndpprep-0.0.5/PKG-INFO` & `ndpprep-0.0.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
 Name: ndpprep
-Version: 0.0.5
+Version: 0.0.8
 Summary: A command line tool to prepare high-quality data in Parquet
 Author-email: Mohd Zaid Waqiyuddin Mohd Zulkifli <zaidwaqi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/zaidwaqi/ndpprep
 Project-URL: Issues, https://github.com/pypa/zaidwaqi/ndpprep/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: pyarrow>=14.0.0
+Requires-Dist: Click
+Requires-Dist: pandas
+Requires-Dist: geopandas
+Requires-Dist: paramiko
 
 # ndpprep
 
 `ndpprep` is a data prep tool that simplifies use of custom Python data processing within a data pipeline focusing on application in Network Data Platform (NDP) project.
+
+`ndpprep` is to be used both in on-premise CDSW and Azure Function in the cloud.
```

### Comparing `ndpprep-0.0.5/src/ndpprep.egg-info/PKG-INFO` & `ndpprep-0.0.8/src/ndpprep.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
 Name: ndpprep
-Version: 0.0.5
+Version: 0.0.8
 Summary: A command line tool to prepare high-quality data in Parquet
 Author-email: Mohd Zaid Waqiyuddin Mohd Zulkifli <zaidwaqi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/zaidwaqi/ndpprep
 Project-URL: Issues, https://github.com/pypa/zaidwaqi/ndpprep/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: pyarrow>=14.0.0
+Requires-Dist: Click
+Requires-Dist: pandas
+Requires-Dist: geopandas
+Requires-Dist: paramiko
 
 # ndpprep
 
 `ndpprep` is a data prep tool that simplifies use of custom Python data processing within a data pipeline focusing on application in Network Data Platform (NDP) project.
+
+`ndpprep` is to be used both in on-premise CDSW and Azure Function in the cloud.
```

