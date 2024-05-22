# Comparing `tmp/fleekapi-0.0.12.tar.gz` & `tmp/fleekapi-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleekapi-0.0.12.tar", last modified: Wed May 22 21:31:16 2024, max compression
+gzip compressed data, was "fleekapi-0.0.13.tar", last modified: Wed May 22 21:35:12 2024, max compression
```

## Comparing `fleekapi-0.0.12.tar` & `fleekapi-0.0.13.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-22 21:31:16.993317 fleekapi-0.0.12/
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-22 21:31:16.989317 fleekapi-0.0.12/FleekAPI.egg-info/
--rw-r--r--   0 hasan     (1002) hasan     (1002)     2415 2024-05-22 21:31:16.000000 fleekapi-0.0.12/FleekAPI.egg-info/PKG-INFO
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      285 2024-05-22 21:31:16.000000 fleekapi-0.0.12/FleekAPI.egg-info/SOURCES.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-22 21:31:16.000000 fleekapi-0.0.12/FleekAPI.egg-info/dependency_links.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      154 2024-05-22 21:31:16.000000 fleekapi-0.0.12/FleekAPI.egg-info/requires.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-22 21:31:16.000000 fleekapi-0.0.12/FleekAPI.egg-info/top_level.txt
--rw-r--r--   0 hasan     (1002) hasan     (1002)     2415 2024-05-22 21:31:16.993317 fleekapi-0.0.12/PKG-INFO
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-22 21:31:16.985317 fleekapi-0.0.12/fleekapi/
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-22 08:15:47.000000 fleekapi-0.0.12/fleekapi/__init__.py
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-22 21:31:16.989317 fleekapi-0.0.12/fleekapi/src/
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       69 2024-05-22 08:15:47.000000 fleekapi-0.0.12/fleekapi/src/__init__.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     3755 2024-05-22 21:20:57.000000 fleekapi-0.0.12/fleekapi/src/app.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      630 2024-05-22 08:15:47.000000 fleekapi-0.0.12/fleekapi/src/middleware.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      964 2024-05-22 08:15:47.000000 fleekapi-0.0.12/fleekapi/src/response.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-22 21:31:16.993317 fleekapi-0.0.12/setup.cfg
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     4036 2024-05-22 21:31:08.000000 fleekapi-0.0.12/setup.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-22 21:35:12.591179 fleekapi-0.0.13/
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-22 21:35:12.587179 fleekapi-0.0.13/FleekAPI.egg-info/
+-rw-r--r--   0 hasan     (1002) hasan     (1002)     2415 2024-05-22 21:35:12.000000 fleekapi-0.0.13/FleekAPI.egg-info/PKG-INFO
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      285 2024-05-22 21:35:12.000000 fleekapi-0.0.13/FleekAPI.egg-info/SOURCES.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-22 21:35:12.000000 fleekapi-0.0.13/FleekAPI.egg-info/dependency_links.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      154 2024-05-22 21:35:12.000000 fleekapi-0.0.13/FleekAPI.egg-info/requires.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-22 21:35:12.000000 fleekapi-0.0.13/FleekAPI.egg-info/top_level.txt
+-rw-r--r--   0 hasan     (1002) hasan     (1002)     2415 2024-05-22 21:35:12.587179 fleekapi-0.0.13/PKG-INFO
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-22 21:35:12.583178 fleekapi-0.0.13/fleekapi/
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       19 2024-05-22 21:35:04.000000 fleekapi-0.0.13/fleekapi/__init__.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-22 21:35:12.587179 fleekapi-0.0.13/fleekapi/src/
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       69 2024-05-22 08:15:47.000000 fleekapi-0.0.13/fleekapi/src/__init__.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     3755 2024-05-22 21:20:57.000000 fleekapi-0.0.13/fleekapi/src/app.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      630 2024-05-22 08:15:47.000000 fleekapi-0.0.13/fleekapi/src/middleware.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      964 2024-05-22 08:15:47.000000 fleekapi-0.0.13/fleekapi/src/response.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-22 21:35:12.591179 fleekapi-0.0.13/setup.cfg
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     4036 2024-05-22 21:35:04.000000 fleekapi-0.0.13/setup.py
```

### Comparing `fleekapi-0.0.12/FleekAPI.egg-info/PKG-INFO` & `fleekapi-0.0.13/FleekAPI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FleekAPI
-Version: 0.0.12
+Version: 0.0.13
 Summary: My short description for my project.
 Home-page: https://github.com/under-script/fleekapi
 Author: Yunusov Abdulmajid
 Author-email: abdulmajidyunusov18@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `fleekapi-0.0.12/PKG-INFO` & `fleekapi-0.0.13/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FleekAPI
-Version: 0.0.12
+Version: 0.0.13
 Summary: My short description for my project.
 Home-page: https://github.com/under-script/fleekapi
 Author: Yunusov Abdulmajid
 Author-email: abdulmajidyunusov18@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `fleekapi-0.0.12/fleekapi/src/app.py` & `fleekapi-0.0.13/fleekapi/src/app.py`

 * *Files identical despite different names*

### Comparing `fleekapi-0.0.12/fleekapi/src/middleware.py` & `fleekapi-0.0.13/fleekapi/src/middleware.py`

 * *Files identical despite different names*

### Comparing `fleekapi-0.0.12/fleekapi/src/response.py` & `fleekapi-0.0.13/fleekapi/src/response.py`

 * *Files identical despite different names*

### Comparing `fleekapi-0.0.12/setup.py` & `fleekapi-0.0.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'FleekAPI'
 DESCRIPTION = 'My short description for my project.'
 URL = 'https://github.com/under-script/fleekapi'
 EMAIL = 'abdulmajidyunusov18@gmail.com'
 AUTHOR = 'Yunusov Abdulmajid'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.0.12'
+VERSION = '0.0.13'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
     "gunicorn==22.0.0",
     "Jinja2==3.1.4",
     "parse==1.20.1",
```

