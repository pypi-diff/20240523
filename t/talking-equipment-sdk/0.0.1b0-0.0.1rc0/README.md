# Comparing `tmp/talking_equipment_sdk-0.0.1b0.tar.gz` & `tmp/talking_equipment_sdk-0.0.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talking_equipment_sdk-0.0.1b0.tar", last modified: Wed May 22 21:48:31 2024, max compression
+gzip compressed data, was "talking_equipment_sdk-0.0.1rc0.tar", last modified: Wed May 22 22:14:37 2024, max compression
```

## Comparing `talking_equipment_sdk-0.0.1b0.tar` & `talking_equipment_sdk-0.0.1rc0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:48:31.891247 talking_equipment_sdk-0.0.1b0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-22 21:48:31.891247 talking_equipment_sdk-0.0.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:48:31.887247 talking_equipment_sdk-0.0.1b0/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:48:31.887247 talking_equipment_sdk-0.0.1b0/api/data_source/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/api/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/api/data_source/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/api/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/api/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/api/responses.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:48:31.887247 talking_equipment_sdk-0.0.1b0/data/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:48:31.887247 talking_equipment_sdk-0.0.1b0/data/control/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/data/control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/data/control/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/data/control/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:48:31.891247 talking_equipment_sdk-0.0.1b0/data/counter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/data/counter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/data/counter/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/data/counter/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/data/entities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:48:31.891247 talking_equipment_sdk-0.0.1b0/data/temperature/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/data/temperature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/data/temperature/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/data/temperature/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:48:31.891247 talking_equipment_sdk-0.0.1b0/data/vibration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/data/vibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/data/vibration/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/data/vibration/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-22 21:48:31.891247 talking_equipment_sdk-0.0.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-22 21:48:22.000000 talking_equipment_sdk-0.0.1b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:48:31.891247 talking_equipment_sdk-0.0.1b0/talking_equipment_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-22 21:48:31.000000 talking_equipment_sdk-0.0.1b0/talking_equipment_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-22 21:48:31.000000 talking_equipment_sdk-0.0.1b0/talking_equipment_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 21:48:31.000000 talking_equipment_sdk-0.0.1b0/talking_equipment_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 21:48:31.000000 talking_equipment_sdk-0.0.1b0/talking_equipment_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:37.637177 talking_equipment_sdk-0.0.1rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-22 22:14:37.637177 talking_equipment_sdk-0.0.1rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:37.633177 talking_equipment_sdk-0.0.1rc0/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:37.633177 talking_equipment_sdk-0.0.1rc0/api/data_source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/api/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/api/data_source/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/api/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/api/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/api/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:37.637177 talking_equipment_sdk-0.0.1rc0/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:37.637177 talking_equipment_sdk-0.0.1rc0/data/control/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/data/control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/data/control/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/data/control/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:37.637177 talking_equipment_sdk-0.0.1rc0/data/counter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/data/counter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/data/counter/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/data/counter/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/data/entities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:37.637177 talking_equipment_sdk-0.0.1rc0/data/temperature/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/data/temperature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/data/temperature/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/data/temperature/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:37.637177 talking_equipment_sdk-0.0.1rc0/data/vibration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/data/vibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/data/vibration/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/data/vibration/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-22 22:14:37.637177 talking_equipment_sdk-0.0.1rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-22 22:14:29.000000 talking_equipment_sdk-0.0.1rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:37.637177 talking_equipment_sdk-0.0.1rc0/talking_equipment_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-22 22:14:37.000000 talking_equipment_sdk-0.0.1rc0/talking_equipment_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-22 22:14:37.000000 talking_equipment_sdk-0.0.1rc0/talking_equipment_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:14:37.000000 talking_equipment_sdk-0.0.1rc0/talking_equipment_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 22:14:37.000000 talking_equipment_sdk-0.0.1rc0/talking_equipment_sdk.egg-info/top_level.txt
```

### Comparing `talking_equipment_sdk-0.0.1b0/LICENSE.md` & `talking_equipment_sdk-0.0.1rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `talking_equipment_sdk-0.0.1b0/api/handlers.py` & `talking_equipment_sdk-0.0.1rc0/api/handlers.py`

 * *Files identical despite different names*

### Comparing `talking_equipment_sdk-0.0.1b0/api/requests.py` & `talking_equipment_sdk-0.0.1rc0/api/requests.py`

 * *Files identical despite different names*

### Comparing `talking_equipment_sdk-0.0.1b0/data/control/tests.py` & `talking_equipment_sdk-0.0.1rc0/data/control/tests.py`

 * *Files identical despite different names*

### Comparing `talking_equipment_sdk-0.0.1b0/data/entities.py` & `talking_equipment_sdk-0.0.1rc0/data/entities.py`

 * *Files identical despite different names*

### Comparing `talking_equipment_sdk-0.0.1b0/data/temperature/entities.py` & `talking_equipment_sdk-0.0.1rc0/data/temperature/entities.py`

 * *Files identical despite different names*

### Comparing `talking_equipment_sdk-0.0.1b0/data/temperature/tests.py` & `talking_equipment_sdk-0.0.1rc0/data/temperature/tests.py`

 * *Files identical despite different names*

### Comparing `talking_equipment_sdk-0.0.1b0/data/vibration/tests.py` & `talking_equipment_sdk-0.0.1rc0/data/vibration/tests.py`

 * *Files identical despite different names*

### Comparing `talking_equipment_sdk-0.0.1b0/setup.cfg` & `talking_equipment_sdk-0.0.1rc0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [metadata]
 name = talking-equipment-sdk
-version = 0.0.1b
+version = 0.0.1c
 author = Nathan Johnson
 author_email = nathanj@stratusadv.com
 description = Talking Equipment Standard Development Kit
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 include_package_data = True
 packages = find:
+package_dir = 
+	talking_equipment = .
 
 [options.packages.find]
 exclude = 
 	tests
 python_requires = >=3.9
 
 [egg_info]
```

### Comparing `talking_equipment_sdk-0.0.1b0/talking_equipment_sdk.egg-info/SOURCES.txt` & `talking_equipment_sdk-0.0.1rc0/talking_equipment_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

