# Comparing `tmp/anything_world-0.1.6.tar.gz` & `tmp/anything_world-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anything_world-0.1.6.tar", last modified: Fri May 10 08:29:13 2024, max compression
+gzip compressed data, was "anything_world-0.1.7.tar", last modified: Thu May 23 08:23:58 2024, max compression
```

## Comparing `anything_world-0.1.6.tar` & `anything_world-0.1.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-10 08:29:13.720955 anything_world-0.1.6/
--rw-rw-r--   0 vilson    (1000) vilson    (1001)     1071 2024-05-10 08:20:41.000000 anything_world-0.1.6/LICENSE
--rw-rw-r--   0 vilson    (1000) vilson    (1001)      241 2024-05-10 08:20:41.000000 anything_world-0.1.6/MANIFEST.in
--rw-r--r--   0 vilson    (1000) vilson    (1001)     4545 2024-05-10 08:29:13.720955 anything_world-0.1.6/PKG-INFO
--rw-rw-r--   0 vilson    (1000) vilson    (1001)     3913 2024-05-10 08:21:23.000000 anything_world-0.1.6/README.md
-drwxrwxr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-10 08:29:13.710955 anything_world-0.1.6/anything_world/
--rw-rw-r--   0 vilson    (1000) vilson    (1001)        0 2024-05-10 08:20:41.000000 anything_world-0.1.6/anything_world/__init__.py
-drwxrwxr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-10 08:29:13.710955 anything_world-0.1.6/anything_world/async_api/
--rw-rw-r--   0 vilson    (1000) vilson    (1001)       32 2024-05-10 08:20:41.000000 anything_world-0.1.6/anything_world/async_api/__init__.py
--rw-rw-r--   0 vilson    (1000) vilson    (1001)    12407 2024-05-10 08:20:41.000000 anything_world-0.1.6/anything_world/async_api/api_client.py
--rw-rw-r--   0 vilson    (1000) vilson    (1001)     3163 2024-05-10 08:20:41.000000 anything_world-0.1.6/anything_world/async_api/utils.py
-drwxrwxr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-10 08:29:13.710955 anything_world-0.1.6/anything_world/sync_api/
--rw-rw-r--   0 vilson    (1000) vilson    (1001)       32 2024-05-10 08:20:41.000000 anything_world-0.1.6/anything_world/sync_api/__init__.py
--rw-rw-r--   0 vilson    (1000) vilson    (1001)    12250 2024-05-10 08:20:41.000000 anything_world-0.1.6/anything_world/sync_api/api_client.py
--rw-rw-r--   0 vilson    (1000) vilson    (1001)     2755 2024-05-10 08:20:41.000000 anything_world-0.1.6/anything_world/sync_api/utils.py
-drwxrwxr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-10 08:29:13.710955 anything_world-0.1.6/anything_world/utils/
--rw-rw-r--   0 vilson    (1000) vilson    (1001)     2872 2024-05-10 08:20:41.000000 anything_world-0.1.6/anything_world/utils/__init__.py
-drwxrwxr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-10 08:29:13.710955 anything_world-0.1.6/anything_world.egg-info/
--rw-r--r--   0 vilson    (1000) vilson    (1001)     4545 2024-05-10 08:29:13.000000 anything_world-0.1.6/anything_world.egg-info/PKG-INFO
--rw-rw-r--   0 vilson    (1000) vilson    (1001)      634 2024-05-10 08:29:13.000000 anything_world-0.1.6/anything_world.egg-info/SOURCES.txt
--rw-rw-r--   0 vilson    (1000) vilson    (1001)        1 2024-05-10 08:29:13.000000 anything_world-0.1.6/anything_world.egg-info/dependency_links.txt
--rw-rw-r--   0 vilson    (1000) vilson    (1001)       46 2024-05-10 08:29:13.000000 anything_world-0.1.6/anything_world.egg-info/entry_points.txt
--rw-rw-r--   0 vilson    (1000) vilson    (1001)      119 2024-05-10 08:29:13.000000 anything_world-0.1.6/anything_world.egg-info/requires.txt
--rw-rw-r--   0 vilson    (1000) vilson    (1001)       23 2024-05-10 08:29:13.000000 anything_world-0.1.6/anything_world.egg-info/top_level.txt
--rw-rw-r--   0 vilson    (1000) vilson    (1001)      132 2024-05-10 08:20:41.000000 anything_world-0.1.6/env.example
--rw-rw-r--   0 vilson    (1000) vilson    (1001)      829 2024-05-10 08:26:56.000000 anything_world-0.1.6/pyproject.toml
-drwxrwxr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-10 08:29:13.710955 anything_world-0.1.6/scripts/
--rw-rw-r--   0 vilson    (1000) vilson    (1001)       95 2024-05-10 08:20:41.000000 anything_world-0.1.6/scripts/cli.py
--rw-rw-r--   0 vilson    (1000) vilson    (1001)       38 2024-05-10 08:29:13.720955 anything_world-0.1.6/setup.cfg
--rw-rw-r--   0 vilson    (1000) vilson    (1001)       91 2024-05-10 08:20:41.000000 anything_world-0.1.6/setup.py
-drwxrwxr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-10 08:29:13.710955 anything_world-0.1.6/tests/
--rw-rw-r--   0 vilson    (1000) vilson    (1001)     2110 2024-05-10 08:20:41.000000 anything_world-0.1.6/tests/test_async_api.py
--rw-rw-r--   0 vilson    (1000) vilson    (1001)     2006 2024-05-10 08:20:41.000000 anything_world-0.1.6/tests/test_sync_api.py
+drwxr-xr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-23 08:23:58.440232 anything_world-0.1.7/
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)     1071 2024-05-10 08:20:41.000000 anything_world-0.1.7/LICENSE
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)      241 2024-05-10 08:20:41.000000 anything_world-0.1.7/MANIFEST.in
+-rw-r--r--   0 vilson    (1000) vilson    (1001)     4545 2024-05-23 08:23:58.440232 anything_world-0.1.7/PKG-INFO
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)     3913 2024-05-10 08:21:23.000000 anything_world-0.1.7/README.md
+drwxr-xr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-23 08:23:58.440232 anything_world-0.1.7/anything_world/
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)        0 2024-05-10 08:20:41.000000 anything_world-0.1.7/anything_world/__init__.py
+drwxr-xr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-23 08:23:58.440232 anything_world-0.1.7/anything_world/async_api/
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)       32 2024-05-10 08:20:41.000000 anything_world-0.1.7/anything_world/async_api/__init__.py
+-rw-r--r--   0 vilson    (1000) vilson    (1001)    12437 2024-05-23 08:23:08.000000 anything_world-0.1.7/anything_world/async_api/api_client.py
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)     3163 2024-05-10 08:20:41.000000 anything_world-0.1.7/anything_world/async_api/utils.py
+drwxr-xr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-23 08:23:58.440232 anything_world-0.1.7/anything_world/sync_api/
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)       32 2024-05-10 08:20:41.000000 anything_world-0.1.7/anything_world/sync_api/__init__.py
+-rw-r--r--   0 vilson    (1000) vilson    (1001)    12280 2024-05-23 08:23:08.000000 anything_world-0.1.7/anything_world/sync_api/api_client.py
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)     2755 2024-05-10 08:20:41.000000 anything_world-0.1.7/anything_world/sync_api/utils.py
+drwxr-xr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-23 08:23:58.440232 anything_world-0.1.7/anything_world/utils/
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)     2872 2024-05-10 08:20:41.000000 anything_world-0.1.7/anything_world/utils/__init__.py
+drwxr-xr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-23 08:23:58.440232 anything_world-0.1.7/anything_world.egg-info/
+-rw-r--r--   0 vilson    (1000) vilson    (1001)     4545 2024-05-23 08:23:58.000000 anything_world-0.1.7/anything_world.egg-info/PKG-INFO
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)      634 2024-05-23 08:23:58.000000 anything_world-0.1.7/anything_world.egg-info/SOURCES.txt
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)        1 2024-05-23 08:23:58.000000 anything_world-0.1.7/anything_world.egg-info/dependency_links.txt
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)       46 2024-05-23 08:23:58.000000 anything_world-0.1.7/anything_world.egg-info/entry_points.txt
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)      119 2024-05-23 08:23:58.000000 anything_world-0.1.7/anything_world.egg-info/requires.txt
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)       23 2024-05-23 08:23:58.000000 anything_world-0.1.7/anything_world.egg-info/top_level.txt
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)      132 2024-05-10 08:20:41.000000 anything_world-0.1.7/env.example
+-rw-r--r--   0 vilson    (1000) vilson    (1001)      829 2024-05-23 08:23:08.000000 anything_world-0.1.7/pyproject.toml
+drwxr-xr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-23 08:23:58.440232 anything_world-0.1.7/scripts/
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)       95 2024-05-10 08:20:41.000000 anything_world-0.1.7/scripts/cli.py
+-rw-r--r--   0 vilson    (1000) vilson    (1001)       38 2024-05-23 08:23:58.440232 anything_world-0.1.7/setup.cfg
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)       91 2024-05-10 08:20:41.000000 anything_world-0.1.7/setup.py
+drwxr-xr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-23 08:23:58.440232 anything_world-0.1.7/tests/
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)     2110 2024-05-10 08:20:41.000000 anything_world-0.1.7/tests/test_async_api.py
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)     2006 2024-05-10 08:20:41.000000 anything_world-0.1.7/tests/test_sync_api.py
```

### Comparing `anything_world-0.1.6/LICENSE` & `anything_world-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `anything_world-0.1.6/PKG-INFO` & `anything_world-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anything_world
-Version: 0.1.6
+Version: 0.1.7
 Summary: Anything World API wrapper library and CLI
 Author-email: Anything World <support@anything.world>
 License: MIT
 Project-URL: Homepage, https://anything.world
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `anything_world-0.1.6/README.md` & `anything_world-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `anything_world-0.1.6/anything_world/async_api/api_client.py` & `anything_world-0.1.7/anything_world/async_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,18 +92,19 @@
         :param model_name: str, the name of the model to be animated.
         :param model_type: str, the type of the model to be animated.
         :param is_symmetric: bool, optional, a flag indicating whether the model is symmetric. Defaults to True.
 
         :return: dict, the JSON response from the API decoded as a dict.
         """
         data = {
-            "api_key": self.api_key,
+            "key": self.api_key,
             "model_name": model_name,
             "model_type": model_type,
-            "symmetry": "true" if is_symmetric else "false"
+            "symmetry": "true" if is_symmetric else "false",
+            "platform": "python"
         }
         form_data = create_form_data(read_files(files_dir), data)
         params = {"staging": "true"} if self.is_staging else {}
         return await send_request(
             url=f"{self.api_url}/animate",
             method="POST",
             data=form_data,
```

### Comparing `anything_world-0.1.6/anything_world/async_api/utils.py` & `anything_world-0.1.7/anything_world/async_api/utils.py`

 * *Files identical despite different names*

### Comparing `anything_world-0.1.6/anything_world/sync_api/api_client.py` & `anything_world-0.1.7/anything_world/sync_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,18 +93,19 @@
         :param model_name: str, the name of the model to be animated.
         :param model_type: str, the type of the model to be animated.
         :param is_symmetric: bool, optional, a flag indicating whether the model is symmetric. Defaults to True.
 
         :return: dict, the JSON response from the API decoded as a dict.
         """
         data = {
-            "api_key": self.api_key,
+            "key": self.api_key,
             "model_name": model_name,
             "model_type": model_type,
-            "symmetry": "true" if is_symmetric else "false"
+            "symmetry": "true" if is_symmetric else "false",
+            "platform": "python"
         }
         form_data = create_form_data(read_files(files_dir), {})
         params = {"staging": "true"} if self.is_staging else {}
         return send_request(
             url=f"{self.api_url}/animate",
             method="POST",
             data=data,
```

### Comparing `anything_world-0.1.6/anything_world/sync_api/utils.py` & `anything_world-0.1.7/anything_world/sync_api/utils.py`

 * *Files identical despite different names*

### Comparing `anything_world-0.1.6/anything_world/utils/__init__.py` & `anything_world-0.1.7/anything_world/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anything_world-0.1.6/anything_world.egg-info/PKG-INFO` & `anything_world-0.1.7/anything_world.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anything_world
-Version: 0.1.6
+Version: 0.1.7
 Summary: Anything World API wrapper library and CLI
 Author-email: Anything World <support@anything.world>
 License: MIT
 Project-URL: Homepage, https://anything.world
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `anything_world-0.1.6/anything_world.egg-info/SOURCES.txt` & `anything_world-0.1.7/anything_world.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anything_world-0.1.6/pyproject.toml` & `anything_world-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "anything_world"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
     {name = "Anything World", email = "support@anything.world"},
 ]
 description = "Anything World API wrapper library and CLI"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT"}
```

### Comparing `anything_world-0.1.6/tests/test_async_api.py` & `anything_world-0.1.7/tests/test_async_api.py`

 * *Files identical despite different names*

### Comparing `anything_world-0.1.6/tests/test_sync_api.py` & `anything_world-0.1.7/tests/test_sync_api.py`

 * *Files identical despite different names*

