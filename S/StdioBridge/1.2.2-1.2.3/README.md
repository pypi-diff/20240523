# Comparing `tmp/StdioBridge-1.2.2.tar.gz` & `tmp/StdioBridge-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StdioBridge-1.2.2.tar", last modified: Sat May 18 18:57:04 2024, max compression
+gzip compressed data, was "StdioBridge-1.2.3.tar", last modified: Thu May 23 18:21:22 2024, max compression
```

## Comparing `StdioBridge-1.2.2.tar` & `StdioBridge-1.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:57:04.069894 StdioBridge-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-18 18:56:56.000000 StdioBridge-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-18 18:57:04.069894 StdioBridge-1.2.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:57:04.065894 StdioBridge-1.2.2/StdioBridge/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-18 18:56:56.000000 StdioBridge-1.2.2/StdioBridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-18 18:56:56.000000 StdioBridge-1.2.2/StdioBridge/_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:57:04.065894 StdioBridge-1.2.2/StdioBridge/api/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-18 18:56:56.000000 StdioBridge-1.2.2/StdioBridge/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-18 18:56:56.000000 StdioBridge-1.2.2/StdioBridge/api/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-18 18:56:56.000000 StdioBridge-1.2.2/StdioBridge/api/_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-05-18 18:56:56.000000 StdioBridge-1.2.2/StdioBridge/api/_router.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-18 18:56:56.000000 StdioBridge-1.2.2/StdioBridge/api/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:57:04.069894 StdioBridge-1.2.2/StdioBridge/client/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-18 18:56:56.000000 StdioBridge-1.2.2/StdioBridge/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-18 18:56:56.000000 StdioBridge-1.2.2/StdioBridge/client/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-18 18:56:56.000000 StdioBridge-1.2.2/StdioBridge/client/_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:57:04.065894 StdioBridge-1.2.2/StdioBridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-18 18:57:04.000000 StdioBridge-1.2.2/StdioBridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-18 18:57:04.000000 StdioBridge-1.2.2/StdioBridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 18:57:04.000000 StdioBridge-1.2.2/StdioBridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-18 18:57:04.000000 StdioBridge-1.2.2/StdioBridge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-18 18:57:04.000000 StdioBridge-1.2.2/StdioBridge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 18:57:04.069894 StdioBridge-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-18 18:56:56.000000 StdioBridge-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:21:22.245226 StdioBridge-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-23 18:21:22.245226 StdioBridge-1.2.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:21:22.241226 StdioBridge-1.2.3/StdioBridge/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/StdioBridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/StdioBridge/_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:21:22.245226 StdioBridge-1.2.3/StdioBridge/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/StdioBridge/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/StdioBridge/api/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/StdioBridge/api/_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/StdioBridge/api/_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/StdioBridge/api/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:21:22.245226 StdioBridge-1.2.3/StdioBridge/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/StdioBridge/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/StdioBridge/client/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/StdioBridge/client/_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:21:22.241226 StdioBridge-1.2.3/StdioBridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-23 18:21:22.000000 StdioBridge-1.2.3/StdioBridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-23 18:21:22.000000 StdioBridge-1.2.3/StdioBridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:21:22.000000 StdioBridge-1.2.3/StdioBridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 18:21:22.000000 StdioBridge-1.2.3/StdioBridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 18:21:22.000000 StdioBridge-1.2.3/StdioBridge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:21:22.245226 StdioBridge-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/setup.py
```

### Comparing `StdioBridge-1.2.2/LICENSE` & `StdioBridge-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.2.2/PKG-INFO` & `StdioBridge-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StdioBridge
-Version: 1.2.2
+Version: 1.2.3
 Summary: A StdioBridge package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) 2024 SergeiKrivko
```

### Comparing `StdioBridge-1.2.2/StdioBridge/api/_api.py` & `StdioBridge-1.2.3/StdioBridge/api/_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from aioconsole import ainput
 
 from StdioBridge.api._response import Response, StreamResponse
 from StdioBridge.api._router import Router
 from StdioBridge.api.errors import *
 
 
-class Api:
+class BridgeAPI:
     def __init__(self):
         self._root_router = Router()
 
     def get(self, url: str):
         return self._root_router.get(url)
 
     def post(self, url: str):
```

### Comparing `StdioBridge-1.2.2/StdioBridge/api/_response.py` & `StdioBridge-1.2.3/StdioBridge/api/_response.py`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.2.2/StdioBridge/api/_router.py` & `StdioBridge-1.2.3/StdioBridge/api/_router.py`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.2.2/StdioBridge/api/errors.py` & `StdioBridge-1.2.3/StdioBridge/api/errors.py`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.2.2/StdioBridge/client/_client.py` & `StdioBridge-1.2.3/StdioBridge/client/_client.py`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.2.2/StdioBridge/client/_response.py` & `StdioBridge-1.2.3/StdioBridge/client/_response.py`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.2.2/StdioBridge.egg-info/PKG-INFO` & `StdioBridge-1.2.3/StdioBridge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StdioBridge
-Version: 1.2.2
+Version: 1.2.3
 Summary: A StdioBridge package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) 2024 SergeiKrivko
```

### Comparing `StdioBridge-1.2.2/setup.py` & `StdioBridge-1.2.3/setup.py`

 * *Files identical despite different names*

