# Comparing `tmp/fleekapi-0.0.13.tar.gz` & `tmp/fleekapi-0.0.131.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleekapi-0.0.13.tar", last modified: Wed May 22 21:35:12 2024, max compression
+gzip compressed data, was "fleekapi-0.0.131.tar", last modified: Wed May 22 22:03:26 2024, max compression
```

## Comparing `fleekapi-0.0.13.tar` & `fleekapi-0.0.131.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-22 21:35:12.591179 fleekapi-0.0.13/
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-22 21:35:12.587179 fleekapi-0.0.13/FleekAPI.egg-info/
--rw-r--r--   0 hasan     (1002) hasan     (1002)     2415 2024-05-22 21:35:12.000000 fleekapi-0.0.13/FleekAPI.egg-info/PKG-INFO
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      285 2024-05-22 21:35:12.000000 fleekapi-0.0.13/FleekAPI.egg-info/SOURCES.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-22 21:35:12.000000 fleekapi-0.0.13/FleekAPI.egg-info/dependency_links.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      154 2024-05-22 21:35:12.000000 fleekapi-0.0.13/FleekAPI.egg-info/requires.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-22 21:35:12.000000 fleekapi-0.0.13/FleekAPI.egg-info/top_level.txt
--rw-r--r--   0 hasan     (1002) hasan     (1002)     2415 2024-05-22 21:35:12.587179 fleekapi-0.0.13/PKG-INFO
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-22 21:35:12.583178 fleekapi-0.0.13/fleekapi/
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       19 2024-05-22 21:35:04.000000 fleekapi-0.0.13/fleekapi/__init__.py
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-22 21:35:12.587179 fleekapi-0.0.13/fleekapi/src/
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       69 2024-05-22 08:15:47.000000 fleekapi-0.0.13/fleekapi/src/__init__.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     3755 2024-05-22 21:20:57.000000 fleekapi-0.0.13/fleekapi/src/app.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      630 2024-05-22 08:15:47.000000 fleekapi-0.0.13/fleekapi/src/middleware.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      964 2024-05-22 08:15:47.000000 fleekapi-0.0.13/fleekapi/src/response.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-22 21:35:12.591179 fleekapi-0.0.13/setup.cfg
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     4036 2024-05-22 21:35:04.000000 fleekapi-0.0.13/setup.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-22 22:03:26.919855 fleekapi-0.0.131/
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-22 22:03:26.915855 fleekapi-0.0.131/FleekAPI.egg-info/
+-rw-r--r--   0 hasan     (1002) hasan     (1002)     2416 2024-05-22 22:03:26.000000 fleekapi-0.0.131/FleekAPI.egg-info/PKG-INFO
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      285 2024-05-22 22:03:26.000000 fleekapi-0.0.131/FleekAPI.egg-info/SOURCES.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-22 22:03:26.000000 fleekapi-0.0.131/FleekAPI.egg-info/dependency_links.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      154 2024-05-22 22:03:26.000000 fleekapi-0.0.131/FleekAPI.egg-info/requires.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-22 22:03:26.000000 fleekapi-0.0.131/FleekAPI.egg-info/top_level.txt
+-rw-r--r--   0 hasan     (1002) hasan     (1002)     2416 2024-05-22 22:03:26.915855 fleekapi-0.0.131/PKG-INFO
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-22 22:03:26.867855 fleekapi-0.0.131/fleekapi/
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       19 2024-05-22 21:35:04.000000 fleekapi-0.0.131/fleekapi/__init__.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-22 22:03:26.911855 fleekapi-0.0.131/fleekapi/src/
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       69 2024-05-22 08:15:47.000000 fleekapi-0.0.131/fleekapi/src/__init__.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     4030 2024-05-22 22:03:16.000000 fleekapi-0.0.131/fleekapi/src/app.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      630 2024-05-22 08:15:47.000000 fleekapi-0.0.131/fleekapi/src/middleware.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      964 2024-05-22 08:15:47.000000 fleekapi-0.0.131/fleekapi/src/response.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-22 22:03:26.919855 fleekapi-0.0.131/setup.cfg
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     4037 2024-05-22 22:03:16.000000 fleekapi-0.0.131/setup.py
```

### Comparing `fleekapi-0.0.13/FleekAPI.egg-info/PKG-INFO` & `fleekapi-0.0.131/FleekAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FleekAPI
-Version: 0.0.13
+Version: 0.0.131
 Summary: My short description for my project.
 Home-page: https://github.com/under-script/fleekapi
 Author: Yunusov Abdulmajid
 Author-email: abdulmajidyunusov18@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `fleekapi-0.0.13/PKG-INFO` & `fleekapi-0.0.131/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FleekAPI
-Version: 0.0.13
+Version: 0.0.131
 Summary: My short description for my project.
 Home-page: https://github.com/under-script/fleekapi
 Author: Yunusov Abdulmajid
 Author-email: abdulmajidyunusov18@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `fleekapi-0.0.13/fleekapi/src/app.py` & `fleekapi-0.0.131/fleekapi/src/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os.path
 
 import requests
 import wsgiadapter
 from jinja2 import Environment, FileSystemLoader
 from parse import parse
 from webob import Request
+from werkzeug.serving import run_simple
 from whitenoise import WhiteNoise
 
 from .middleware import Middleware
 from .response import Response
 
 
 def default_response(resp):
@@ -121,12 +122,18 @@
 
     def add_middleware(self, middleware_cls):
         self.middleware.add(middleware_cls)
 
     def include_router(self, router):
         self.routes.update(**router.routes)
 
+    def run(self, debug=False):
+        if debug:
+            run_simple("localhost", 8000, self, use_reloader=True, use_debugger=True, use_evalex=True)
+        else:
+            run_simple("localhost", 8000, self, use_reloader=True)
+
 
 class Router(FleekAPI):
     def __init__(self):
         super().__init__()
         self.routes = dict()
```

### Comparing `fleekapi-0.0.13/fleekapi/src/middleware.py` & `fleekapi-0.0.131/fleekapi/src/middleware.py`

 * *Files identical despite different names*

### Comparing `fleekapi-0.0.13/fleekapi/src/response.py` & `fleekapi-0.0.131/fleekapi/src/response.py`

 * *Files identical despite different names*

### Comparing `fleekapi-0.0.13/setup.py` & `fleekapi-0.0.131/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'FleekAPI'
 DESCRIPTION = 'My short description for my project.'
 URL = 'https://github.com/under-script/fleekapi'
 EMAIL = 'abdulmajidyunusov18@gmail.com'
 AUTHOR = 'Yunusov Abdulmajid'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.0.13'
+VERSION = '0.0.131'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
     "gunicorn==22.0.0",
     "Jinja2==3.1.4",
     "parse==1.20.1",
```

