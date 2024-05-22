# Comparing `tmp/talking_equipment_sdk-0.0.2.tar.gz` & `tmp/talking_equipment_sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talking_equipment_sdk-0.0.2.tar", last modified: Wed May 22 22:56:40 2024, max compression
+gzip compressed data, was "talking_equipment_sdk-0.0.3.tar", last modified: Wed May 22 23:25:21 2024, max compression
```

## Comparing `talking_equipment_sdk-0.0.2.tar` & `talking_equipment_sdk-0.0.3.tar`

### file list

```diff
@@ -1,40 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:56:40.673871 talking_equipment_sdk-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-22 22:56:40.673871 talking_equipment_sdk-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:56:40.665871 talking_equipment_sdk-0.0.2/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:56:40.669871 talking_equipment_sdk-0.0.2/api/data_source/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/api/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/api/data_source/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/api/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/api/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/api/responses.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:56:40.669871 talking_equipment_sdk-0.0.2/data/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:56:40.669871 talking_equipment_sdk-0.0.2/data/control/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/data/control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/data/control/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/data/control/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:56:40.669871 talking_equipment_sdk-0.0.2/data/counter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/data/counter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/data/counter/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/data/counter/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/data/entities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:56:40.669871 talking_equipment_sdk-0.0.2/data/temperature/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/data/temperature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/data/temperature/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/data/temperature/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:56:40.669871 talking_equipment_sdk-0.0.2/data/vibration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/data/vibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/data/vibration/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/data/vibration/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 22:56:40.673871 talking_equipment_sdk-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-22 22:56:30.000000 talking_equipment_sdk-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:56:40.673871 talking_equipment_sdk-0.0.2/talking_equipment_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-22 22:56:40.000000 talking_equipment_sdk-0.0.2/talking_equipment_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 22:56:40.000000 talking_equipment_sdk-0.0.2/talking_equipment_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:56:40.000000 talking_equipment_sdk-0.0.2/talking_equipment_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 22:56:40.000000 talking_equipment_sdk-0.0.2/talking_equipment_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:25:21.474391 talking_equipment_sdk-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 23:25:21.470391 talking_equipment_sdk-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 23:25:21.474391 talking_equipment_sdk-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:25:21.466391 talking_equipment_sdk-0.0.3/talking_equipment/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:25:21.466391 talking_equipment_sdk-0.0.3/talking_equipment/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/talking_equipment/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:25:21.466391 talking_equipment_sdk-0.0.3/talking_equipment/api/data_source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/talking_equipment/api/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/talking_equipment/api/data_source/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/talking_equipment/api/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/talking_equipment/api/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/talking_equipment/api/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/talking_equipment/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:25:21.470391 talking_equipment_sdk-0.0.3/talking_equipment/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/talking_equipment/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:25:21.470391 talking_equipment_sdk-0.0.3/talking_equipment/data/control/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/talking_equipment/data/control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/talking_equipment/data/control/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/talking_equipment/data/control/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:25:21.470391 talking_equipment_sdk-0.0.3/talking_equipment/data/counter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/talking_equipment/data/counter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/talking_equipment/data/counter/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/talking_equipment/data/counter/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/talking_equipment/data/entities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:25:21.470391 talking_equipment_sdk-0.0.3/talking_equipment/data/temperature/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/talking_equipment/data/temperature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/talking_equipment/data/temperature/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/talking_equipment/data/temperature/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:25:21.470391 talking_equipment_sdk-0.0.3/talking_equipment/data/vibration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/talking_equipment/data/vibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/talking_equipment/data/vibration/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-22 23:25:12.000000 talking_equipment_sdk-0.0.3/talking_equipment/data/vibration/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:25:21.470391 talking_equipment_sdk-0.0.3/talking_equipment/talking_equipment_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 23:25:21.000000 talking_equipment_sdk-0.0.3/talking_equipment/talking_equipment_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-22 23:25:21.000000 talking_equipment_sdk-0.0.3/talking_equipment/talking_equipment_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 23:25:21.000000 talking_equipment_sdk-0.0.3/talking_equipment/talking_equipment_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 23:25:21.000000 talking_equipment_sdk-0.0.3/talking_equipment/talking_equipment_sdk.egg-info/top_level.txt
```

### Comparing `talking_equipment_sdk-0.0.2/api/handlers.py` & `talking_equipment_sdk-0.0.3/talking_equipment/api/handlers.py`

 * *Files identical despite different names*

### Comparing `talking_equipment_sdk-0.0.2/api/requests.py` & `talking_equipment_sdk-0.0.3/talking_equipment/api/requests.py`

 * *Files identical despite different names*

### Comparing `talking_equipment_sdk-0.0.2/data/control/tests.py` & `talking_equipment_sdk-0.0.3/talking_equipment/data/control/tests.py`

 * *Files identical despite different names*

### Comparing `talking_equipment_sdk-0.0.2/data/entities.py` & `talking_equipment_sdk-0.0.3/talking_equipment/data/entities.py`

 * *Files identical despite different names*

### Comparing `talking_equipment_sdk-0.0.2/data/temperature/entities.py` & `talking_equipment_sdk-0.0.3/talking_equipment/data/temperature/entities.py`

 * *Files identical despite different names*

### Comparing `talking_equipment_sdk-0.0.2/data/temperature/tests.py` & `talking_equipment_sdk-0.0.3/talking_equipment/data/temperature/tests.py`

 * *Files identical despite different names*

### Comparing `talking_equipment_sdk-0.0.2/data/vibration/tests.py` & `talking_equipment_sdk-0.0.3/talking_equipment/data/vibration/tests.py`

 * *Files identical despite different names*

### Comparing `talking_equipment_sdk-0.0.2/talking_equipment_sdk.egg-info/SOURCES.txt` & `talking_equipment_sdk-0.0.3/talking_equipment/talking_equipment_sdk.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-LICENSE.md
-README.md
 pyproject.toml
 setup.py
-api/__init__.py
-api/handlers.py
-api/requests.py
-api/responses.py
-api/utils.py
-api/data_source/__init__.py
-api/data_source/handlers.py
-data/__init__.py
-data/entities.py
-data/control/__init__.py
-data/control/entities.py
-data/control/tests.py
-data/counter/__init__.py
-data/counter/entities.py
-data/counter/tests.py
-data/temperature/__init__.py
-data/temperature/entities.py
-data/temperature/tests.py
-data/vibration/__init__.py
-data/vibration/entities.py
-data/vibration/tests.py
-talking_equipment_sdk.egg-info/PKG-INFO
-talking_equipment_sdk.egg-info/SOURCES.txt
-talking_equipment_sdk.egg-info/dependency_links.txt
-talking_equipment_sdk.egg-info/top_level.txt
+talking_equipment/api/__init__.py
+talking_equipment/api/handlers.py
+talking_equipment/api/requests.py
+talking_equipment/api/responses.py
+talking_equipment/api/utils.py
+talking_equipment/api/data_source/__init__.py
+talking_equipment/api/data_source/handlers.py
+talking_equipment/data/__init__.py
+talking_equipment/data/entities.py
+talking_equipment/data/control/__init__.py
+talking_equipment/data/control/entities.py
+talking_equipment/data/control/tests.py
+talking_equipment/data/counter/__init__.py
+talking_equipment/data/counter/entities.py
+talking_equipment/data/counter/tests.py
+talking_equipment/data/temperature/__init__.py
+talking_equipment/data/temperature/entities.py
+talking_equipment/data/temperature/tests.py
+talking_equipment/data/vibration/__init__.py
+talking_equipment/data/vibration/entities.py
+talking_equipment/data/vibration/tests.py
+talking_equipment/talking_equipment_sdk.egg-info/PKG-INFO
+talking_equipment/talking_equipment_sdk.egg-info/SOURCES.txt
+talking_equipment/talking_equipment_sdk.egg-info/dependency_links.txt
+talking_equipment/talking_equipment_sdk.egg-info/top_level.txt
```

