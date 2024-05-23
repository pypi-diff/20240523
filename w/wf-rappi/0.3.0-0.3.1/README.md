# Comparing `tmp/wf_rappi-0.3.0.tar.gz` & `tmp/wf_rappi-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf_rappi-0.3.0.tar", last modified: Thu May 23 03:48:47 2024, max compression
+gzip compressed data, was "wf_rappi-0.3.1.tar", last modified: Thu May 23 03:57:20 2024, max compression
```

## Comparing `wf_rappi-0.3.0.tar` & `wf_rappi-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 03:48:47.606948 wf_rappi-0.3.0/
--rw-rw-rw-   0        0        0     2225 2024-05-23 03:48:47.593437 wf_rappi-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-23 03:48:47.608814 wf_rappi-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      960 2024-05-23 03:46:22.000000 wf_rappi-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 03:48:47.562580 wf_rappi-0.3.0/wf_rappi/
--rw-rw-rw-   0        0        0       61 2024-05-23 03:46:28.000000 wf_rappi-0.3.0/wf_rappi/__init__.py
--rw-rw-rw-   0        0        0     6455 2024-05-22 23:36:42.000000 wf_rappi-0.3.0/wf_rappi/data_processing.py
--rw-rw-rw-   0        0        0     1396 2024-04-18 19:54:58.000000 wf_rappi-0.3.0/wf_rappi/dbconn.py
--rw-rw-rw-   0        0        0       70 2024-05-15 21:58:33.000000 wf_rappi-0.3.0/wf_rappi/export.py
--rw-rw-rw-   0        0        0    12003 2024-05-22 13:51:17.000000 wf_rappi-0.3.0/wf_rappi/fetch_data.py
--rw-rw-rw-   0        0        0     2582 2024-05-22 15:27:04.000000 wf_rappi-0.3.0/wf_rappi/main.py
--rw-rw-rw-   0        0        0     1610 2024-05-17 02:48:28.000000 wf_rappi-0.3.0/wf_rappi/modeling.py
--rw-rw-rw-   0        0        0     8092 2024-05-23 03:12:09.000000 wf_rappi-0.3.0/wf_rappi/order_distribution.py
--rw-rw-rw-   0        0        0     2748 2024-04-19 03:22:08.000000 wf_rappi-0.3.0/wf_rappi/wfm_functions.py
-drwxrwxrwx   0        0        0        0 2024-05-23 03:48:47.593437 wf_rappi-0.3.0/wf_rappi.egg-info/
--rw-rw-rw-   0        0        0     2225 2024-05-23 03:48:47.000000 wf_rappi-0.3.0/wf_rappi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2024-05-23 03:48:47.000000 wf_rappi-0.3.0/wf_rappi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 03:48:47.000000 wf_rappi-0.3.0/wf_rappi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-05-23 03:48:47.000000 wf_rappi-0.3.0/wf_rappi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      313 2024-05-23 03:48:47.000000 wf_rappi-0.3.0/wf_rappi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-23 03:48:47.000000 wf_rappi-0.3.0/wf_rappi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 03:57:20.906164 wf_rappi-0.3.1/
+-rw-rw-rw-   0        0        0     2225 2024-05-23 03:57:20.906164 wf_rappi-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-23 03:57:20.906164 wf_rappi-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      937 2024-05-23 03:56:52.000000 wf_rappi-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:57:20.792459 wf_rappi-0.3.1/wf_rappi/
+-rw-rw-rw-   0        0        0     6455 2024-05-22 23:36:42.000000 wf_rappi-0.3.1/wf_rappi/data_processing.py
+-rw-rw-rw-   0        0        0     1396 2024-04-18 19:54:58.000000 wf_rappi-0.3.1/wf_rappi/dbconn.py
+-rw-rw-rw-   0        0        0       70 2024-05-15 21:58:33.000000 wf_rappi-0.3.1/wf_rappi/export.py
+-rw-rw-rw-   0        0        0    12003 2024-05-22 13:51:17.000000 wf_rappi-0.3.1/wf_rappi/fetch_data.py
+-rw-rw-rw-   0        0        0     1610 2024-05-17 02:48:28.000000 wf_rappi-0.3.1/wf_rappi/modeling.py
+-rw-rw-rw-   0        0        0     8092 2024-05-23 03:12:09.000000 wf_rappi-0.3.1/wf_rappi/order_distribution.py
+-rw-rw-rw-   0        0        0     2748 2024-04-19 03:22:08.000000 wf_rappi-0.3.1/wf_rappi/wfm_functions.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:57:20.862199 wf_rappi-0.3.1/wf_rappi - copia/
+-rw-rw-rw-   0        0        0       61 2024-05-23 03:46:28.000000 wf_rappi-0.3.1/wf_rappi - copia/__init__.py
+-rw-rw-rw-   0        0        0     6455 2024-05-22 23:36:42.000000 wf_rappi-0.3.1/wf_rappi - copia/data_processing.py
+-rw-rw-rw-   0        0        0     1396 2024-04-18 19:54:58.000000 wf_rappi-0.3.1/wf_rappi - copia/dbconn.py
+-rw-rw-rw-   0        0        0       70 2024-05-15 21:58:33.000000 wf_rappi-0.3.1/wf_rappi - copia/export.py
+-rw-rw-rw-   0        0        0    12003 2024-05-22 13:51:17.000000 wf_rappi-0.3.1/wf_rappi - copia/fetch_data.py
+-rw-rw-rw-   0        0        0     2582 2024-05-22 15:27:04.000000 wf_rappi-0.3.1/wf_rappi - copia/main.py
+-rw-rw-rw-   0        0        0     1610 2024-05-17 02:48:28.000000 wf_rappi-0.3.1/wf_rappi - copia/modeling.py
+-rw-rw-rw-   0        0        0     8092 2024-05-23 03:12:09.000000 wf_rappi-0.3.1/wf_rappi - copia/order_distribution.py
+-rw-rw-rw-   0        0        0     2748 2024-04-19 03:22:08.000000 wf_rappi-0.3.1/wf_rappi - copia/wfm_functions.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:57:20.898623 wf_rappi-0.3.1/wf_rappi.egg-info/
+-rw-rw-rw-   0        0        0     2225 2024-05-23 03:57:20.000000 wf_rappi-0.3.1/wf_rappi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      646 2024-05-23 03:57:20.000000 wf_rappi-0.3.1/wf_rappi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 03:57:20.000000 wf_rappi-0.3.1/wf_rappi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-23 03:57:20.000000 wf_rappi-0.3.1/wf_rappi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      313 2024-05-23 03:57:20.000000 wf_rappi-0.3.1/wf_rappi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-23 03:57:20.000000 wf_rappi-0.3.1/wf_rappi.egg-info/top_level.txt
```

### Comparing `wf_rappi-0.3.0/PKG-INFO` & `wf_rappi-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf_rappi
-Version: 0.3.0
+Version: 0.3.1
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.11.1
 Requires-Dist: pandas>=1.0
 Requires-Dist: matplotlib==3.8.3
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: packaging==23.2
 Requires-Dist: pillow==10.2.0
```

### Comparing `wf_rappi-0.3.0/setup.py` & `wf_rappi-0.3.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="wf_rappi",
-    version="0.3.0",
+    version="0.3.1",
     packages=find_packages(),
     install_requires=[
         'numpy>=1.11.1',
         'pandas>=1.0',
         'matplotlib==3.8.3',
         'openpyxl==3.1.2',
         'packaging==23.2',
@@ -24,13 +24,13 @@
         'snowflake-snowpark-python==1.13.0',
         'SQLAlchemy==1.4.51',
         'twine==5.1.0',
         'xgboost==2.0.3'
     ],
     entry_points={
         "console_scripts": [
-            "wf-rappi = wf_rappi.main:distribute_orders",
+            "wf-rappi = wf_rappi",
         ],
     },
     long_description=description,
     long_description_content_type="text/markdown",
 )
```

### Comparing `wf_rappi-0.3.0/wf_rappi/data_processing.py` & `wf_rappi-0.3.1/wf_rappi/data_processing.py`

 * *Files identical despite different names*

### Comparing `wf_rappi-0.3.0/wf_rappi/dbconn.py` & `wf_rappi-0.3.1/wf_rappi/dbconn.py`

 * *Files identical despite different names*

### Comparing `wf_rappi-0.3.0/wf_rappi/fetch_data.py` & `wf_rappi-0.3.1/wf_rappi/fetch_data.py`

 * *Files identical despite different names*

### Comparing `wf_rappi-0.3.0/wf_rappi/main.py` & `wf_rappi-0.3.1/wf_rappi - copia/main.py`

 * *Files identical despite different names*

### Comparing `wf_rappi-0.3.0/wf_rappi/modeling.py` & `wf_rappi-0.3.1/wf_rappi/modeling.py`

 * *Files identical despite different names*

### Comparing `wf_rappi-0.3.0/wf_rappi/order_distribution.py` & `wf_rappi-0.3.1/wf_rappi/order_distribution.py`

 * *Files identical despite different names*

### Comparing `wf_rappi-0.3.0/wf_rappi/wfm_functions.py` & `wf_rappi-0.3.1/wf_rappi/wfm_functions.py`

 * *Files identical despite different names*

### Comparing `wf_rappi-0.3.0/wf_rappi.egg-info/PKG-INFO` & `wf_rappi-0.3.1/wf_rappi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-rappi
-Version: 0.3.0
+Version: 0.3.1
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.11.1
 Requires-Dist: pandas>=1.0
 Requires-Dist: matplotlib==3.8.3
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: packaging==23.2
 Requires-Dist: pillow==10.2.0
```

