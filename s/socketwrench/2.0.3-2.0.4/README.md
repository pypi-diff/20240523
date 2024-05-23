# Comparing `tmp/socketwrench-2.0.3.tar.gz` & `tmp/socketwrench-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketwrench-2.0.3.tar", last modified: Mon May 20 21:02:12 2024, max compression
+gzip compressed data, was "socketwrench-2.0.4.tar", last modified: Thu May 23 18:04:22 2024, max compression
```

## Comparing `socketwrench-2.0.3.tar` & `socketwrench-2.0.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:02:12.684836 socketwrench-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-20 21:02:08.000000 socketwrench-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 21:02:08.000000 socketwrench-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-05-20 21:02:12.684836 socketwrench-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14193 2024-05-20 21:02:08.000000 socketwrench-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-20 21:02:08.000000 socketwrench-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 21:02:12.684836 socketwrench-2.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:02:12.676836 socketwrench-2.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:02:12.680836 socketwrench-2.0.3/src/socketwrench/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:02:12.680836 socketwrench-2.0.3/src/socketwrench/fake_imports/
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/fake_imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/fake_imports/fake_argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/fake_imports/fake_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/fake_imports/fake_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/fake_imports/fake_functools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/fake_imports/fake_inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/fake_imports/fake_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/fake_imports/fake_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/fake_imports/fake_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/fake_imports/fake_tempfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/fake_imports/fake_traceback.py
--rw-r--r--   0 runner    (1001) docker     (127)    35292 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/public.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:02:12.680836 socketwrench-2.0.3/src/socketwrench/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/resources/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:02:12.680836 socketwrench-2.0.3/src/socketwrench/resources/playground/
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/resources/playground/panels.js
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/resources/playground/playground.html
--rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/resources/playground/playground.js
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/resources/swagger.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:02:12.684836 socketwrench-2.0.3/src/socketwrench/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/samples/file_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/samples/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/standardlib_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    33772 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:02:12.684836 socketwrench-2.0.3/src/socketwrench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-05-20 21:02:12.000000 socketwrench-2.0.3/src/socketwrench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-20 21:02:12.000000 socketwrench-2.0.3/src/socketwrench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:02:12.000000 socketwrench-2.0.3/src/socketwrench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 21:02:12.000000 socketwrench-2.0.3/src/socketwrench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:04:22.670690 socketwrench-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-23 18:04:18.000000 socketwrench-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 18:04:18.000000 socketwrench-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-05-23 18:04:22.670690 socketwrench-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14193 2024-05-23 18:04:18.000000 socketwrench-2.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-23 18:04:18.000000 socketwrench-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:04:22.670690 socketwrench-2.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:04:22.662690 socketwrench-2.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:04:22.666690 socketwrench-2.0.4/src/socketwrench/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:04:22.670690 socketwrench-2.0.4/src/socketwrench/fake_imports/
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/fake_imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/fake_imports/fake_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/fake_imports/fake_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/fake_imports/fake_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/fake_imports/fake_functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/fake_imports/fake_inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/fake_imports/fake_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/fake_imports/fake_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/fake_imports/fake_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/fake_imports/fake_tempfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/fake_imports/fake_traceback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35292 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8326 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/public.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:04:22.670690 socketwrench-2.0.4/src/socketwrench/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:04:22.670690 socketwrench-2.0.4/src/socketwrench/resources/playground/
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/resources/playground/panels.js
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/resources/playground/playground.html
+-rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/resources/playground/playground.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/resources/swagger.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:04:22.670690 socketwrench-2.0.4/src/socketwrench/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/samples/file_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/samples/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/standardlib_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33772 2024-05-23 18:04:18.000000 socketwrench-2.0.4/src/socketwrench/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:04:22.670690 socketwrench-2.0.4/src/socketwrench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-05-23 18:04:22.000000 socketwrench-2.0.4/src/socketwrench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-23 18:04:22.000000 socketwrench-2.0.4/src/socketwrench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:04:22.000000 socketwrench-2.0.4/src/socketwrench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 18:04:22.000000 socketwrench-2.0.4/src/socketwrench.egg-info/top_level.txt
```

### Comparing `socketwrench-2.0.3/LICENSE` & `socketwrench-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/PKG-INFO` & `socketwrench-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 2.0.3
+Version: 2.0.4
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `socketwrench-2.0.3/README.md` & `socketwrench-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/pyproject.toml` & `socketwrench-2.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketwrench"
-version = "2.0.3"
+version = "2.0.4"
 description = "A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger."
 readme = "README.md"
 authors = [{ name = "Torin Halsted", email = "modularizer@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
```

### Comparing `socketwrench-2.0.3/src/socketwrench/__init__.py` & `socketwrench-2.0.4/src/socketwrench/__init__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/__main__.py` & `socketwrench-2.0.4/src/socketwrench/__main__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/connection.py` & `socketwrench-2.0.4/src/socketwrench/connection.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/fake_imports/__init__.py` & `socketwrench-2.0.4/src/socketwrench/fake_imports/__init__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/fake_imports/fake_argparse.py` & `socketwrench-2.0.4/src/socketwrench/fake_imports/fake_argparse.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/fake_imports/fake_datetime.py` & `socketwrench-2.0.4/src/socketwrench/fake_imports/fake_datetime.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/fake_imports/fake_inspect.py` & `socketwrench-2.0.4/src/socketwrench/fake_imports/fake_inspect.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/fake_imports/fake_json.py` & `socketwrench-2.0.4/src/socketwrench/fake_imports/fake_json.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/fake_imports/fake_logging.py` & `socketwrench-2.0.4/src/socketwrench/fake_imports/fake_logging.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/fake_imports/fake_pathlib.py` & `socketwrench-2.0.4/src/socketwrench/fake_imports/fake_pathlib.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/fake_imports/fake_tempfile.py` & `socketwrench-2.0.4/src/socketwrench/fake_imports/fake_tempfile.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/handlers.py` & `socketwrench-2.0.4/src/socketwrench/handlers.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/openapi.py` & `socketwrench-2.0.4/src/socketwrench/openapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,62 +79,74 @@
                                 module = __import__("socketwrench.types", fromlist=[class_name])
                                 return_type = getattr(module, class_name)
                             except:
                                 return_type = Response
                 except:
                     pass
             if return_type is not inspect.Parameter.empty:
-                if return_type is None:
-                    route_info["responses"] = {
-                        "200": {
-                            "description": "Success",
-                            "content": {
-                                "application/json": {
-                                    "schema": {"type": "object"}
+                try:
+                    if return_type is None:
+                        route_info["responses"] = {
+                            "200": {
+                                "description": "Success",
+                                "content": {
+                                    "application/json": {
+                                        "schema": {"type": "object"}
+                                    }
                                 }
                             }
                         }
-                    }
-                elif return_type is Path or issubclass(return_type, Path) or return_type is FileResponse or issubclass(return_type, FileResponse):
-                    content_type = getattr(return_type, "default_content_type", "application/octet-stream")
-                    route_info["responses"] = {
-                        "200": {
-                            "description": "File response",
-                            "content": {
-                                content_type: {
-                                    "schema": {"type": "string", "format": "binary"}
+                    elif return_type is Path or issubclass(return_type, Path) or return_type is FileResponse or issubclass(return_type, FileResponse):
+                        content_type = getattr(return_type, "default_content_type", "application/octet-stream")
+                        route_info["responses"] = {
+                            "200": {
+                                "description": "File response",
+                                "content": {
+                                    content_type: {
+                                        "schema": {"type": "string", "format": "binary"}
+                                    }
                                 }
                             }
                         }
-                    }
-                elif return_type is str or issubclass(return_type, str):
-                    route_info["responses"] = {
-                        "200": {
-                            "description": "Success",
-                            "content": {
-                                "text/html": {
-                                    "schema": {"type": "string"}
+                    elif return_type is str or issubclass(return_type, str):
+                        route_info["responses"] = {
+                            "200": {
+                                "description": "Success",
+                                "content": {
+                                    "text/html": {
+                                        "schema": {"type": "string"}
+                                    }
                                 }
                             }
                         }
-                    }
-                elif return_type is bytes or issubclass(return_type, bytes) or return_type is memoryview or issubclass(return_type, memoryview) \
-                    or return_type is bytearray or issubclass(return_type, bytearray) or return_type is Response or issubclass(return_type, Response):
-                    content_type = getattr(return_type, "default_content_type", "application/octet-stream")
-                    route_info["responses"] = {
-                        "200": {
-                            "description": "Success",
-                            "content": {
-                                content_type: {
-                                    "schema": {"type": "string", "format": "binary"}
+                    elif return_type is bytes or issubclass(return_type, bytes) or return_type is memoryview or issubclass(return_type, memoryview) \
+                        or return_type is bytearray or issubclass(return_type, bytearray) or return_type is Response or issubclass(return_type, Response):
+                        content_type = getattr(return_type, "default_content_type", "application/octet-stream")
+                        route_info["responses"] = {
+                            "200": {
+                                "description": "Success",
+                                "content": {
+                                    content_type: {
+                                        "schema": {"type": "string", "format": "binary"}
+                                    }
                                 }
                             }
                         }
-                    }
-                else:
+                    else:
+                        route_info["responses"] = {
+                            "200": {
+                                "description": "Success",
+                                "content": {
+                                    "application/json": {
+                                        "schema": {"type": "object"}
+                                    }
+                                }
+                            }
+                        }
+                except:
                     route_info["responses"] = {
                         "200": {
                             "description": "Success",
                             "content": {
                                 "application/json": {
                                     "schema": {"type": "object"}
                                 }
```

### Comparing `socketwrench-2.0.3/src/socketwrench/public.py` & `socketwrench-2.0.4/src/socketwrench/public.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/resources/favicon.ico` & `socketwrench-2.0.4/src/socketwrench/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/resources/playground/panels.js` & `socketwrench-2.0.4/src/socketwrench/resources/playground/panels.js`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/resources/playground/playground.html` & `socketwrench-2.0.4/src/socketwrench/resources/playground/playground.html`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/resources/playground/playground.js` & `socketwrench-2.0.4/src/socketwrench/resources/playground/playground.js`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/resources/swagger.html` & `socketwrench-2.0.4/src/socketwrench/resources/swagger.html`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/samples/file_sample.py` & `socketwrench-2.0.4/src/socketwrench/samples/file_sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/samples/sample.py` & `socketwrench-2.0.4/src/socketwrench/samples/sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/server.py` & `socketwrench-2.0.4/src/socketwrench/server.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/settings.py` & `socketwrench-2.0.4/src/socketwrench/settings.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/standardlib_dependencies.py` & `socketwrench-2.0.4/src/socketwrench/standardlib_dependencies.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/tags.py` & `socketwrench-2.0.4/src/socketwrench/tags.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench/types.py` & `socketwrench-2.0.4/src/socketwrench/types.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.3/src/socketwrench.egg-info/PKG-INFO` & `socketwrench-2.0.4/src/socketwrench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 2.0.3
+Version: 2.0.4
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `socketwrench-2.0.3/src/socketwrench.egg-info/SOURCES.txt` & `socketwrench-2.0.4/src/socketwrench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

