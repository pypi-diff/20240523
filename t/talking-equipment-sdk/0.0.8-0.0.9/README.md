# Comparing `tmp/talking_equipment_sdk-0.0.8.tar.gz` & `tmp/talking_equipment_sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talking_equipment_sdk-0.0.8.tar", last modified: Wed May 22 23:52:06 2024, max compression
+gzip compressed data, was "talking_equipment_sdk-0.0.9.tar", last modified: Thu May 23 01:31:06 2024, max compression
```

## Comparing `talking_equipment_sdk-0.0.8.tar` & `talking_equipment_sdk-0.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:52:06.919311 talking_equipment_sdk-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 23:52:06.919311 talking_equipment_sdk-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 23:52:06.919311 talking_equipment_sdk-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:52:06.915311 talking_equipment_sdk-0.0.8/talking_equipment/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:52:06.915311 talking_equipment_sdk-0.0.8/talking_equipment/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/talking_equipment/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:52:06.915311 talking_equipment_sdk-0.0.8/talking_equipment/api/data_source/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/talking_equipment/api/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/talking_equipment/api/data_source/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/talking_equipment/api/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/talking_equipment/api/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/talking_equipment/api/responses.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/talking_equipment/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:52:06.919311 talking_equipment_sdk-0.0.8/talking_equipment/data/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/talking_equipment/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:52:06.919311 talking_equipment_sdk-0.0.8/talking_equipment/data/control/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/talking_equipment/data/control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/talking_equipment/data/control/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/talking_equipment/data/control/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:52:06.919311 talking_equipment_sdk-0.0.8/talking_equipment/data/counter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/talking_equipment/data/counter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/talking_equipment/data/counter/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/talking_equipment/data/counter/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/talking_equipment/data/entities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:52:06.919311 talking_equipment_sdk-0.0.8/talking_equipment/data/temperature/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/talking_equipment/data/temperature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/talking_equipment/data/temperature/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/talking_equipment/data/temperature/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:52:06.919311 talking_equipment_sdk-0.0.8/talking_equipment/data/vibration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/talking_equipment/data/vibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/talking_equipment/data/vibration/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-22 23:51:58.000000 talking_equipment_sdk-0.0.8/talking_equipment/data/vibration/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:52:06.919311 talking_equipment_sdk-0.0.8/talking_equipment/talking_equipment_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 23:52:06.000000 talking_equipment_sdk-0.0.8/talking_equipment/talking_equipment_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-22 23:52:06.000000 talking_equipment_sdk-0.0.8/talking_equipment/talking_equipment_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 23:52:06.000000 talking_equipment_sdk-0.0.8/talking_equipment/talking_equipment_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 23:52:06.000000 talking_equipment_sdk-0.0.8/talking_equipment/talking_equipment_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:31:06.801159 talking_equipment_sdk-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 01:31:06.801159 talking_equipment_sdk-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 01:31:06.801159 talking_equipment_sdk-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:31:06.797159 talking_equipment_sdk-0.0.9/talking_equipment/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:31:06.797159 talking_equipment_sdk-0.0.9/talking_equipment/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/talking_equipment/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:31:06.797159 talking_equipment_sdk-0.0.9/talking_equipment/api/data_source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/talking_equipment/api/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/talking_equipment/api/data_source/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/talking_equipment/api/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/talking_equipment/api/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/talking_equipment/api/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/talking_equipment/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:31:06.797159 talking_equipment_sdk-0.0.9/talking_equipment/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/talking_equipment/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:31:06.797159 talking_equipment_sdk-0.0.9/talking_equipment/data/control/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/talking_equipment/data/control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/talking_equipment/data/control/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/talking_equipment/data/control/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:31:06.801159 talking_equipment_sdk-0.0.9/talking_equipment/data/counter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/talking_equipment/data/counter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/talking_equipment/data/counter/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/talking_equipment/data/counter/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/talking_equipment/data/entities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:31:06.801159 talking_equipment_sdk-0.0.9/talking_equipment/data/temperature/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/talking_equipment/data/temperature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/talking_equipment/data/temperature/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/talking_equipment/data/temperature/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:31:06.801159 talking_equipment_sdk-0.0.9/talking_equipment/data/vibration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/talking_equipment/data/vibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/talking_equipment/data/vibration/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-23 01:30:52.000000 talking_equipment_sdk-0.0.9/talking_equipment/data/vibration/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:31:06.801159 talking_equipment_sdk-0.0.9/talking_equipment/talking_equipment_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 01:31:06.000000 talking_equipment_sdk-0.0.9/talking_equipment/talking_equipment_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-23 01:31:06.000000 talking_equipment_sdk-0.0.9/talking_equipment/talking_equipment_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:31:06.000000 talking_equipment_sdk-0.0.9/talking_equipment/talking_equipment_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 01:31:06.000000 talking_equipment_sdk-0.0.9/talking_equipment/talking_equipment_sdk.egg-info/top_level.txt
```

### Comparing `talking_equipment_sdk-0.0.8/setup.py` & `talking_equipment_sdk-0.0.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 module_directory = 'talking_equipment'
 
 setup(
     name="talking-equipment-sdk",
-    version="0.0.8",
+    version="0.0.9",
     author="Nathan Johnson",
     author_email="nathanj@stratusadv.com",
     description="Talking Equipment Standard Development Kit",
     long_description=open(f"{module_directory}/README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `talking_equipment_sdk-0.0.8/talking_equipment/api/handlers.py` & `talking_equipment_sdk-0.0.9/talking_equipment/api/handlers.py`

 * *Files identical despite different names*

### Comparing `talking_equipment_sdk-0.0.8/talking_equipment/api/requests.py` & `talking_equipment_sdk-0.0.9/talking_equipment/api/requests.py`

 * *Files identical despite different names*

### Comparing `talking_equipment_sdk-0.0.8/talking_equipment/data/control/tests.py` & `talking_equipment_sdk-0.0.9/talking_equipment/data/control/tests.py`

 * *Files identical despite different names*

### Comparing `talking_equipment_sdk-0.0.8/talking_equipment/data/entities.py` & `talking_equipment_sdk-0.0.9/talking_equipment/data/entities.py`

 * *Files identical despite different names*

### Comparing `talking_equipment_sdk-0.0.8/talking_equipment/data/temperature/entities.py` & `talking_equipment_sdk-0.0.9/talking_equipment/data/temperature/entities.py`

 * *Files identical despite different names*

### Comparing `talking_equipment_sdk-0.0.8/talking_equipment/data/temperature/tests.py` & `talking_equipment_sdk-0.0.9/talking_equipment/data/temperature/tests.py`

 * *Files identical despite different names*

### Comparing `talking_equipment_sdk-0.0.8/talking_equipment/data/vibration/tests.py` & `talking_equipment_sdk-0.0.9/talking_equipment/data/vibration/tests.py`

 * *Files identical despite different names*

### Comparing `talking_equipment_sdk-0.0.8/talking_equipment/talking_equipment_sdk.egg-info/SOURCES.txt` & `talking_equipment_sdk-0.0.9/talking_equipment/talking_equipment_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

