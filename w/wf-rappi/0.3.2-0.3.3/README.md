# Comparing `tmp/wf_rappi-0.3.2.tar.gz` & `tmp/wf_rappi-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf_rappi-0.3.2.tar", last modified: Thu May 23 04:02:53 2024, max compression
+gzip compressed data, was "wf_rappi-0.3.3.tar", last modified: Thu May 23 04:08:31 2024, max compression
```

## Comparing `wf_rappi-0.3.2.tar` & `wf_rappi-0.3.3.tar`

### file list

```diff
@@ -1,29 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 04:02:53.074019 wf_rappi-0.3.2/
--rw-rw-rw-   0        0        0     2225 2024-05-23 04:02:53.072388 wf_rappi-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-23 04:02:53.076052 wf_rappi-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      974 2024-05-23 04:02:18.000000 wf_rappi-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 04:02:52.966264 wf_rappi-0.3.2/wf_rappi/
--rw-rw-rw-   0        0        0     6455 2024-05-22 23:36:42.000000 wf_rappi-0.3.2/wf_rappi/data_processing.py
--rw-rw-rw-   0        0        0     1396 2024-04-18 19:54:58.000000 wf_rappi-0.3.2/wf_rappi/dbconn.py
--rw-rw-rw-   0        0        0       70 2024-05-15 21:58:33.000000 wf_rappi-0.3.2/wf_rappi/export.py
--rw-rw-rw-   0        0        0    12003 2024-05-22 13:51:17.000000 wf_rappi-0.3.2/wf_rappi/fetch_data.py
--rw-rw-rw-   0        0        0     1610 2024-05-17 02:48:28.000000 wf_rappi-0.3.2/wf_rappi/modeling.py
--rw-rw-rw-   0        0        0     8092 2024-05-23 03:12:09.000000 wf_rappi-0.3.2/wf_rappi/order_distribution.py
--rw-rw-rw-   0        0        0     2748 2024-04-19 03:22:08.000000 wf_rappi-0.3.2/wf_rappi/wfm_functions.py
-drwxrwxrwx   0        0        0        0 2024-05-23 04:02:53.025936 wf_rappi-0.3.2/wf_rappi - copia/
--rw-rw-rw-   0        0        0       61 2024-05-23 03:46:28.000000 wf_rappi-0.3.2/wf_rappi - copia/__init__.py
--rw-rw-rw-   0        0        0     6455 2024-05-22 23:36:42.000000 wf_rappi-0.3.2/wf_rappi - copia/data_processing.py
--rw-rw-rw-   0        0        0     1396 2024-04-18 19:54:58.000000 wf_rappi-0.3.2/wf_rappi - copia/dbconn.py
--rw-rw-rw-   0        0        0       70 2024-05-15 21:58:33.000000 wf_rappi-0.3.2/wf_rappi - copia/export.py
--rw-rw-rw-   0        0        0    12003 2024-05-22 13:51:17.000000 wf_rappi-0.3.2/wf_rappi - copia/fetch_data.py
--rw-rw-rw-   0        0        0     2582 2024-05-22 15:27:04.000000 wf_rappi-0.3.2/wf_rappi - copia/main.py
--rw-rw-rw-   0        0        0     1610 2024-05-17 02:48:28.000000 wf_rappi-0.3.2/wf_rappi - copia/modeling.py
--rw-rw-rw-   0        0        0     8092 2024-05-23 03:12:09.000000 wf_rappi-0.3.2/wf_rappi - copia/order_distribution.py
--rw-rw-rw-   0        0        0     2748 2024-04-19 03:22:08.000000 wf_rappi-0.3.2/wf_rappi - copia/wfm_functions.py
-drwxrwxrwx   0        0        0        0 2024-05-23 04:02:53.065890 wf_rappi-0.3.2/wf_rappi.egg-info/
--rw-rw-rw-   0        0        0     2225 2024-05-23 04:02:52.000000 wf_rappi-0.3.2/wf_rappi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      646 2024-05-23 04:02:52.000000 wf_rappi-0.3.2/wf_rappi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 04:02:52.000000 wf_rappi-0.3.2/wf_rappi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2024-05-23 04:02:52.000000 wf_rappi-0.3.2/wf_rappi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      313 2024-05-23 04:02:52.000000 wf_rappi-0.3.2/wf_rappi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-23 04:02:52.000000 wf_rappi-0.3.2/wf_rappi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 04:08:31.717213 wf_rappi-0.3.3/
+-rw-rw-rw-   0        0        0     2225 2024-05-23 04:08:31.701588 wf_rappi-0.3.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 04:08:31.669976 wf_rappi-0.3.3/estawf_rappi copia/
+-rw-rw-rw-   0        0        0       61 2024-05-23 03:46:28.000000 wf_rappi-0.3.3/estawf_rappi copia/__init__.py
+-rw-rw-rw-   0        0        0     6455 2024-05-22 23:36:42.000000 wf_rappi-0.3.3/estawf_rappi copia/data_processing.py
+-rw-rw-rw-   0        0        0     1396 2024-04-18 19:54:58.000000 wf_rappi-0.3.3/estawf_rappi copia/dbconn.py
+-rw-rw-rw-   0        0        0       70 2024-05-15 21:58:33.000000 wf_rappi-0.3.3/estawf_rappi copia/export.py
+-rw-rw-rw-   0        0        0    12003 2024-05-22 13:51:17.000000 wf_rappi-0.3.3/estawf_rappi copia/fetch_data.py
+-rw-rw-rw-   0        0        0     2582 2024-05-22 15:27:04.000000 wf_rappi-0.3.3/estawf_rappi copia/main.py
+-rw-rw-rw-   0        0        0     1610 2024-05-17 02:48:28.000000 wf_rappi-0.3.3/estawf_rappi copia/modeling.py
+-rw-rw-rw-   0        0        0     8092 2024-05-23 03:12:09.000000 wf_rappi-0.3.3/estawf_rappi copia/order_distribution.py
+-rw-rw-rw-   0        0        0     2748 2024-04-19 03:22:08.000000 wf_rappi-0.3.3/estawf_rappi copia/wfm_functions.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 04:08:31.717213 wf_rappi-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      974 2024-05-23 04:08:10.000000 wf_rappi-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 04:08:31.701588 wf_rappi-0.3.3/wf_rappi.egg-info/
+-rw-rw-rw-   0        0        0     2225 2024-05-23 04:08:31.000000 wf_rappi-0.3.3/wf_rappi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      497 2024-05-23 04:08:31.000000 wf_rappi-0.3.3/wf_rappi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 04:08:31.000000 wf_rappi-0.3.3/wf_rappi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-05-23 04:08:31.000000 wf_rappi-0.3.3/wf_rappi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      313 2024-05-23 04:08:31.000000 wf_rappi-0.3.3/wf_rappi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-23 04:08:31.000000 wf_rappi-0.3.3/wf_rappi.egg-info/top_level.txt
```

### Comparing `wf_rappi-0.3.2/PKG-INFO` & `wf_rappi-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf_rappi
-Version: 0.3.2
+Version: 0.3.3
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.11.1
 Requires-Dist: pandas>=1.0
 Requires-Dist: matplotlib==3.8.3
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: packaging==23.2
 Requires-Dist: pillow==10.2.0
```

### Comparing `wf_rappi-0.3.2/setup.py` & `wf_rappi-0.3.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="wf_rappi",
-    version="0.3.2",
+    version="0.3.3",
     packages=find_packages(),
     install_requires=[
         'numpy>=1.11.1',
         'pandas>=1.0',
         'matplotlib==3.8.3',
         'openpyxl==3.1.2',
         'packaging==23.2',
```

### Comparing `wf_rappi-0.3.2/wf_rappi/data_processing.py` & `wf_rappi-0.3.3/estawf_rappi copia/data_processing.py`

 * *Files identical despite different names*

### Comparing `wf_rappi-0.3.2/wf_rappi/dbconn.py` & `wf_rappi-0.3.3/estawf_rappi copia/dbconn.py`

 * *Files identical despite different names*

### Comparing `wf_rappi-0.3.2/wf_rappi/fetch_data.py` & `wf_rappi-0.3.3/estawf_rappi copia/fetch_data.py`

 * *Files identical despite different names*

### Comparing `wf_rappi-0.3.2/wf_rappi/modeling.py` & `wf_rappi-0.3.3/estawf_rappi copia/modeling.py`

 * *Files identical despite different names*

### Comparing `wf_rappi-0.3.2/wf_rappi/order_distribution.py` & `wf_rappi-0.3.3/estawf_rappi copia/order_distribution.py`

 * *Files identical despite different names*

### Comparing `wf_rappi-0.3.2/wf_rappi/wfm_functions.py` & `wf_rappi-0.3.3/estawf_rappi copia/wfm_functions.py`

 * *Files identical despite different names*

### Comparing `wf_rappi-0.3.2/wf_rappi - copia/main.py` & `wf_rappi-0.3.3/estawf_rappi copia/main.py`

 * *Files identical despite different names*

### Comparing `wf_rappi-0.3.2/wf_rappi.egg-info/PKG-INFO` & `wf_rappi-0.3.3/wf_rappi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-rappi
-Version: 0.3.2
+Version: 0.3.3
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.11.1
 Requires-Dist: pandas>=1.0
 Requires-Dist: matplotlib==3.8.3
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: packaging==23.2
 Requires-Dist: pillow==10.2.0
```

