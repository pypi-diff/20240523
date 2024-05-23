# Comparing `tmp/types-Flask-Cors-4.0.0.20240405.tar.gz` & `tmp/types-Flask-Cors-4.0.0.20240523.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-Flask-Cors-4.0.0.20240405.tar", last modified: Fri Apr  5 02:14:54 2024, max compression
+gzip compressed data, was "types-Flask-Cors-4.0.0.20240523.tar", last modified: Thu May 23 02:22:02 2024, max compression
```

## Comparing `types-Flask-Cors-4.0.0.20240405.tar` & `types-Flask-Cors-4.0.0.20240523.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:14:54.714166 types-Flask-Cors-4.0.0.20240405/
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-05 02:14:54.000000 types-Flask-Cors-4.0.0.20240405/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 02:14:54.000000 types-Flask-Cors-4.0.0.20240405/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-05 02:14:54.714166 types-Flask-Cors-4.0.0.20240405/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:14:54.714166 types-Flask-Cors-4.0.0.20240405/flask_cors-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-05 02:14:54.000000 types-Flask-Cors-4.0.0.20240405/flask_cors-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-05 02:14:36.000000 types-Flask-Cors-4.0.0.20240405/flask_cors-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-05 02:14:36.000000 types-Flask-Cors-4.0.0.20240405/flask_cors-stubs/core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-05 02:14:36.000000 types-Flask-Cors-4.0.0.20240405/flask_cors-stubs/decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-05 02:14:36.000000 types-Flask-Cors-4.0.0.20240405/flask_cors-stubs/extension.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 02:14:54.000000 types-Flask-Cors-4.0.0.20240405/flask_cors-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 02:14:36.000000 types-Flask-Cors-4.0.0.20240405/flask_cors-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:14:54.714166 types-Flask-Cors-4.0.0.20240405/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-05 02:14:54.000000 types-Flask-Cors-4.0.0.20240405/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:14:54.714166 types-Flask-Cors-4.0.0.20240405/types_Flask_Cors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-05 02:14:54.000000 types-Flask-Cors-4.0.0.20240405/types_Flask_Cors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-05 02:14:54.000000 types-Flask-Cors-4.0.0.20240405/types_Flask_Cors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:14:54.000000 types-Flask-Cors-4.0.0.20240405/types_Flask_Cors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 02:14:54.000000 types-Flask-Cors-4.0.0.20240405/types_Flask_Cors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 02:14:54.000000 types-Flask-Cors-4.0.0.20240405/types_Flask_Cors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:22:02.714237 types-Flask-Cors-4.0.0.20240523/
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-23 02:22:02.000000 types-Flask-Cors-4.0.0.20240523/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 02:22:02.000000 types-Flask-Cors-4.0.0.20240523/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-23 02:22:02.714237 types-Flask-Cors-4.0.0.20240523/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:22:02.714237 types-Flask-Cors-4.0.0.20240523/flask_cors-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-23 02:22:02.000000 types-Flask-Cors-4.0.0.20240523/flask_cors-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-23 02:21:41.000000 types-Flask-Cors-4.0.0.20240523/flask_cors-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-23 02:21:41.000000 types-Flask-Cors-4.0.0.20240523/flask_cors-stubs/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-23 02:21:41.000000 types-Flask-Cors-4.0.0.20240523/flask_cors-stubs/decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-23 02:21:41.000000 types-Flask-Cors-4.0.0.20240523/flask_cors-stubs/extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 02:22:02.000000 types-Flask-Cors-4.0.0.20240523/flask_cors-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 02:21:41.000000 types-Flask-Cors-4.0.0.20240523/flask_cors-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 02:22:02.714237 types-Flask-Cors-4.0.0.20240523/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-23 02:22:02.000000 types-Flask-Cors-4.0.0.20240523/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:22:02.714237 types-Flask-Cors-4.0.0.20240523/types_Flask_Cors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-23 02:22:02.000000 types-Flask-Cors-4.0.0.20240523/types_Flask_Cors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-23 02:22:02.000000 types-Flask-Cors-4.0.0.20240523/types_Flask_Cors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 02:22:02.000000 types-Flask-Cors-4.0.0.20240523/types_Flask_Cors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 02:22:02.000000 types-Flask-Cors-4.0.0.20240523/types_Flask_Cors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 02:22:02.000000 types-Flask-Cors-4.0.0.20240523/types_Flask_Cors.egg-info/top_level.txt
```

### Comparing `types-Flask-Cors-4.0.0.20240405/CHANGELOG.md` & `types-Flask-Cors-4.0.0.20240523/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 4.0.0.20240523 (2024-05-23)
+
+[Flask-Cors] accepts flask blueprints (#11995)
+
 ## 4.0.0.20240405 (2024-04-05)
 
 Improve `flask-cors` stubs (#11708)
 
 ## 4.0.0.20240106 (2024-01-06)
 
 Update typing_extensions imports in third-party stubs (#11245)
```

### Comparing `types-Flask-Cors-4.0.0.20240405/PKG-INFO` & `types-Flask-Cors-4.0.0.20240523/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Flask-Cors
-Version: 4.0.0.20240405
+Version: 4.0.0.20240523
 Summary: Typing stubs for Flask-Cors
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Cors.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -32,10 +32,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `130a04905c0cab48604ac7be1f3d18ce96567c68` and was tested
-with mypy 1.9.0, pyright 1.1.357, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `f7c03486ee01c8ea74823db75e017341bf3c2ad0` and was tested
+with mypy 1.10.0, pyright 1.1.364, and
+pytype 2024.4.11.
```

### Comparing `types-Flask-Cors-4.0.0.20240405/flask_cors-stubs/core.pyi` & `types-Flask-Cors-4.0.0.20240523/flask_cors-stubs/core.pyi`

 * *Files identical despite different names*

### Comparing `types-Flask-Cors-4.0.0.20240405/flask_cors-stubs/decorator.pyi` & `types-Flask-Cors-4.0.0.20240523/flask_cors-stubs/decorator.pyi`

 * *Files identical despite different names*

### Comparing `types-Flask-Cors-4.0.0.20240405/flask_cors-stubs/extension.pyi` & `types-Flask-Cors-4.0.0.20240523/flask_cors-stubs/extension.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import flask
 
 LOG: Logger
 
 class CORS:
     def __init__(
         self,
-        app: flask.Flask | None = None,
+        app: flask.Flask | flask.Blueprint | None = None,
         *,
         resources: dict[str, dict[str, Any]] | list[str] | str | None = ...,
         origins: str | list[str] | None = ...,
         methods: str | list[str] | None = ...,
         expose_headers: str | list[str] | None = ...,
         allow_headers: str | list[str] | None = ...,
         supports_credentials: bool | None = ...,
```

### Comparing `types-Flask-Cors-4.0.0.20240405/setup.py` & `types-Flask-Cors-4.0.0.20240523/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `130a04905c0cab48604ac7be1f3d18ce96567c68` and was tested
-with mypy 1.9.0, pyright 1.1.357, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `f7c03486ee01c8ea74823db75e017341bf3c2ad0` and was tested
+with mypy 1.10.0, pyright 1.1.364, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="4.0.0.20240405",
+      version="4.0.0.20240523",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Cors.md",
```

### Comparing `types-Flask-Cors-4.0.0.20240405/types_Flask_Cors.egg-info/PKG-INFO` & `types-Flask-Cors-4.0.0.20240523/types_Flask_Cors.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Flask-Cors
-Version: 4.0.0.20240405
+Version: 4.0.0.20240523
 Summary: Typing stubs for Flask-Cors
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Cors.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -32,10 +32,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `130a04905c0cab48604ac7be1f3d18ce96567c68` and was tested
-with mypy 1.9.0, pyright 1.1.357, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `f7c03486ee01c8ea74823db75e017341bf3c2ad0` and was tested
+with mypy 1.10.0, pyright 1.1.364, and
+pytype 2024.4.11.
```

