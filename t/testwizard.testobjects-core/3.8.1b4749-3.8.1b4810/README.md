# Comparing `tmp/testwizard.testobjects-core-3.8.1b4749.tar.gz` & `tmp/testwizard.testobjects-core-3.8.1b4810.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testwizard.testobjects-core-3.8.1b4749.tar", last modified: Tue Mar 19 15:01:47 2024, max compression
+gzip compressed data, was "testwizard.testobjects-core-3.8.1b4810.tar", last modified: Wed Mar 27 12:56:34 2024, max compression
```

## Comparing `testwizard.testobjects-core-3.8.1b4749.tar` & `testwizard.testobjects-core-3.8.1b4810.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:47.119397 testwizard.testobjects-core-3.8.1b4749/
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.testobjects-core-3.8.1b4749/LICENSE.txt
--rw-rw-rw-   0        0        0      560 2024-03-19 15:01:47.119397 testwizard.testobjects-core-3.8.1b4749/PKG-INFO
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.testobjects-core-3.8.1b4749/README.md
--rw-rw-rw-   0        0        0       42 2024-03-19 15:01:47.119397 testwizard.testobjects-core-3.8.1b4749/setup.cfg
--rw-rw-rw-   0        0        0      863 2024-03-19 15:01:46.000000 testwizard.testobjects-core-3.8.1b4749/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:47.103776 testwizard.testobjects-core-3.8.1b4749/testwizard/
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:47.103776 testwizard.testobjects-core-3.8.1b4749/testwizard/testobjects_core/
--rw-rw-rw-   0        0        0     2923 2024-03-19 15:00:53.000000 testwizard.testobjects-core-3.8.1b4749/testwizard/testobjects_core/TestObjectBase.py
--rw-rw-rw-   0        0        0       42 2024-03-19 15:00:53.000000 testwizard.testobjects-core-3.8.1b4749/testwizard/testobjects_core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:47.119397 testwizard.testobjects-core-3.8.1b4749/testwizard/testobjects_core/models/
--rw-rw-rw-   0        0        0      185 2024-03-19 15:00:53.000000 testwizard.testobjects-core-3.8.1b4749/testwizard/testobjects_core/models/AudioInfo.py
--rw-rw-rw-   0        0        0      595 2024-03-19 15:00:53.000000 testwizard.testobjects-core-3.8.1b4749/testwizard/testobjects_core/models/CustomProperties.py
--rw-rw-rw-   0        0        0      782 2024-03-19 15:00:53.000000 testwizard.testobjects-core-3.8.1b4749/testwizard/testobjects_core/models/DeviceInfo.py
--rw-rw-rw-   0        0        0      192 2024-03-19 15:00:53.000000 testwizard.testobjects-core-3.8.1b4749/testwizard/testobjects_core/models/MobileInfo.py
--rw-rw-rw-   0        0        0      324 2024-03-19 15:00:53.000000 testwizard.testobjects-core-3.8.1b4749/testwizard/testobjects_core/models/RemoteControlInfo.py
--rw-rw-rw-   0        0        0     1545 2024-03-19 15:00:53.000000 testwizard.testobjects-core-3.8.1b4749/testwizard/testobjects_core/models/TestObjectInfo.py
--rw-rw-rw-   0        0        0      412 2024-03-19 15:00:53.000000 testwizard.testobjects-core-3.8.1b4749/testwizard/testobjects_core/models/VendorInfo.py
--rw-rw-rw-   0        0        0      185 2024-03-19 15:00:53.000000 testwizard.testobjects-core-3.8.1b4749/testwizard/testobjects_core/models/VideoInfo.py
--rw-rw-rw-   0        0        0      189 2024-03-19 15:00:53.000000 testwizard.testobjects-core-3.8.1b4749/testwizard/testobjects_core/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:47.103776 testwizard.testobjects-core-3.8.1b4749/testwizard.testobjects_core.egg-info/
--rw-rw-rw-   0        0        0      560 2024-03-19 15:01:47.000000 testwizard.testobjects-core-3.8.1b4749/testwizard.testobjects_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      824 2024-03-19 15:01:47.000000 testwizard.testobjects-core-3.8.1b4749/testwizard.testobjects_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 15:01:47.000000 testwizard.testobjects-core-3.8.1b4749/testwizard.testobjects_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-03-19 15:01:47.000000 testwizard.testobjects-core-3.8.1b4749/testwizard.testobjects_core.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 15:01:47.000000 testwizard.testobjects-core-3.8.1b4749/testwizard.testobjects_core.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:34.384367 testwizard.testobjects-core-3.8.1b4810/
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.testobjects-core-3.8.1b4810/LICENSE.txt
+-rw-rw-rw-   0        0        0      560 2024-03-27 12:56:34.384367 testwizard.testobjects-core-3.8.1b4810/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.testobjects-core-3.8.1b4810/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-27 12:56:34.384367 testwizard.testobjects-core-3.8.1b4810/setup.cfg
+-rw-rw-rw-   0        0        0      863 2024-03-27 12:56:34.000000 testwizard.testobjects-core-3.8.1b4810/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:34.368743 testwizard.testobjects-core-3.8.1b4810/testwizard/
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:34.384367 testwizard.testobjects-core-3.8.1b4810/testwizard/testobjects_core/
+-rw-rw-rw-   0        0        0     2923 2024-03-27 12:55:37.000000 testwizard.testobjects-core-3.8.1b4810/testwizard/testobjects_core/TestObjectBase.py
+-rw-rw-rw-   0        0        0       42 2024-03-27 12:55:37.000000 testwizard.testobjects-core-3.8.1b4810/testwizard/testobjects_core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:34.384367 testwizard.testobjects-core-3.8.1b4810/testwizard/testobjects_core/models/
+-rw-rw-rw-   0        0        0      185 2024-03-27 12:55:37.000000 testwizard.testobjects-core-3.8.1b4810/testwizard/testobjects_core/models/AudioInfo.py
+-rw-rw-rw-   0        0        0      595 2024-03-27 12:55:37.000000 testwizard.testobjects-core-3.8.1b4810/testwizard/testobjects_core/models/CustomProperties.py
+-rw-rw-rw-   0        0        0      782 2024-03-27 12:55:37.000000 testwizard.testobjects-core-3.8.1b4810/testwizard/testobjects_core/models/DeviceInfo.py
+-rw-rw-rw-   0        0        0      192 2024-03-27 12:55:37.000000 testwizard.testobjects-core-3.8.1b4810/testwizard/testobjects_core/models/MobileInfo.py
+-rw-rw-rw-   0        0        0      324 2024-03-27 12:55:37.000000 testwizard.testobjects-core-3.8.1b4810/testwizard/testobjects_core/models/RemoteControlInfo.py
+-rw-rw-rw-   0        0        0     1545 2024-03-27 12:55:37.000000 testwizard.testobjects-core-3.8.1b4810/testwizard/testobjects_core/models/TestObjectInfo.py
+-rw-rw-rw-   0        0        0      412 2024-03-27 12:55:37.000000 testwizard.testobjects-core-3.8.1b4810/testwizard/testobjects_core/models/VendorInfo.py
+-rw-rw-rw-   0        0        0      185 2024-03-27 12:55:37.000000 testwizard.testobjects-core-3.8.1b4810/testwizard/testobjects_core/models/VideoInfo.py
+-rw-rw-rw-   0        0        0      189 2024-03-27 12:55:37.000000 testwizard.testobjects-core-3.8.1b4810/testwizard/testobjects_core/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:34.384367 testwizard.testobjects-core-3.8.1b4810/testwizard.testobjects_core.egg-info/
+-rw-rw-rw-   0        0        0      560 2024-03-27 12:56:34.000000 testwizard.testobjects-core-3.8.1b4810/testwizard.testobjects_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      824 2024-03-27 12:56:34.000000 testwizard.testobjects-core-3.8.1b4810/testwizard.testobjects_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-27 12:56:34.000000 testwizard.testobjects-core-3.8.1b4810/testwizard.testobjects_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-03-27 12:56:34.000000 testwizard.testobjects-core-3.8.1b4810/testwizard.testobjects_core.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-27 12:56:34.000000 testwizard.testobjects-core-3.8.1b4810/testwizard.testobjects_core.egg-info/top_level.txt
```

### Comparing `testwizard.testobjects-core-3.8.1b4749/PKG-INFO` & `testwizard.testobjects-core-3.8.1b4810/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.testobjects-core
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard core components for testobjects
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.testobjects-core-3.8.1b4749/setup.py` & `testwizard.testobjects-core-3.8.1b4810/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_namespace_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="testwizard.testobjects-core",
-    version="3.8.1b4749",
+    version="3.8.1b4810",
     author="Resillion",
     author_email="testwizard-support@resillion.com",
     description="Testwizard core components for testobjects",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.resillion.com/services/software-testing/testing-tools/testwizard/",
     packages=find_namespace_packages(),
     install_requires=[
-        'testwizard.commands-services==3.8.1b4749'
+        'testwizard.commands-services==3.8.1b4810'
     ],
     classifiers=[
         "Programming Language :: Python :: 3.3",
         "Development Status :: 5 - Production/Stable",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `testwizard.testobjects-core-3.8.1b4749/testwizard/testobjects_core/TestObjectBase.py` & `testwizard.testobjects-core-3.8.1b4810/testwizard/testobjects_core/TestObjectBase.py`

 * *Files identical despite different names*

### Comparing `testwizard.testobjects-core-3.8.1b4749/testwizard/testobjects_core/models/CustomProperties.py` & `testwizard.testobjects-core-3.8.1b4810/testwizard/testobjects_core/models/CustomProperties.py`

 * *Files identical despite different names*

### Comparing `testwizard.testobjects-core-3.8.1b4749/testwizard/testobjects_core/models/DeviceInfo.py` & `testwizard.testobjects-core-3.8.1b4810/testwizard/testobjects_core/models/DeviceInfo.py`

 * *Files identical despite different names*

### Comparing `testwizard.testobjects-core-3.8.1b4749/testwizard/testobjects_core/models/TestObjectInfo.py` & `testwizard.testobjects-core-3.8.1b4810/testwizard/testobjects_core/models/TestObjectInfo.py`

 * *Files identical despite different names*

### Comparing `testwizard.testobjects-core-3.8.1b4749/testwizard.testobjects_core.egg-info/PKG-INFO` & `testwizard.testobjects-core-3.8.1b4810/testwizard.testobjects_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.testobjects-core
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard core components for testobjects
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.testobjects-core-3.8.1b4749/testwizard.testobjects_core.egg-info/SOURCES.txt` & `testwizard.testobjects-core-3.8.1b4810/testwizard.testobjects_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

