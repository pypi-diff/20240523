# Comparing `tmp/user_context_remote-0.0.81.tar.gz` & `tmp/user_context_remote-0.0.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_context_remote-0.0.81.tar", last modified: Mon May 20 14:11:12 2024, max compression
+gzip compressed data, was "user_context_remote-0.0.82.tar", last modified: Thu May 23 00:27:02 2024, max compression
```

## Comparing `user_context_remote-0.0.81.tar` & `user_context_remote-0.0.82.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:11:12.557254 user_context_remote-0.0.81/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-20 14:11:12.557254 user_context_remote-0.0.81/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-20 14:10:57.000000 user_context_remote-0.0.81/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-20 14:10:57.000000 user_context_remote-0.0.81/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:11:12.557254 user_context_remote-0.0.81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-20 14:10:57.000000 user_context_remote-0.0.81/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:11:12.553254 user_context_remote-0.0.81/user_context_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:11:12.557254 user_context_remote-0.0.81/user_context_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:10:57.000000 user_context_remote-0.0.81/user_context_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18991 2024-05-20 14:10:57.000000 user_context_remote-0.0.81/user_context_remote/src/user_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:11:12.557254 user_context_remote-0.0.81/user_context_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-20 14:11:12.000000 user_context_remote-0.0.81/user_context_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-20 14:11:12.000000 user_context_remote-0.0.81/user_context_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:11:12.000000 user_context_remote-0.0.81/user_context_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-20 14:11:12.000000 user_context_remote-0.0.81/user_context_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-20 14:11:12.000000 user_context_remote-0.0.81/user_context_remote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:27:02.620931 user_context_remote-0.0.82/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-23 00:27:02.620931 user_context_remote-0.0.82/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-23 00:26:48.000000 user_context_remote-0.0.82/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-23 00:26:48.000000 user_context_remote-0.0.82/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 00:27:02.620931 user_context_remote-0.0.82/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-23 00:26:48.000000 user_context_remote-0.0.82/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:27:02.616931 user_context_remote-0.0.82/user_context_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:27:02.620931 user_context_remote-0.0.82/user_context_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 00:26:48.000000 user_context_remote-0.0.82/user_context_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18991 2024-05-23 00:26:48.000000 user_context_remote-0.0.82/user_context_remote/src/user_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:27:02.620931 user_context_remote-0.0.82/user_context_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-23 00:27:02.000000 user_context_remote-0.0.82/user_context_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-23 00:27:02.000000 user_context_remote-0.0.82/user_context_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 00:27:02.000000 user_context_remote-0.0.82/user_context_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 00:27:02.000000 user_context_remote-0.0.82/user_context_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-23 00:27:02.000000 user_context_remote-0.0.82/user_context_remote.egg-info/top_level.txt
```

### Comparing `user_context_remote-0.0.81/PKG-INFO` & `user_context_remote-0.0.82/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-context-remote
-Version: 0.0.81
+Version: 0.0.82
 Summary: PyPI Package for Circles User Context Local/Remote Python
 Home-page: https://github.com/circles-zone/user-context-remote-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `user_context_remote-0.0.81/README.md` & `user_context_remote-0.0.82/README.md`

 * *Files identical despite different names*

### Comparing `user_context_remote-0.0.81/pyproject.toml` & `user_context_remote-0.0.82/pyproject.toml`

 * *Files identical despite different names*

### Comparing `user_context_remote-0.0.81/setup.py` & `user_context_remote-0.0.82/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "user-context-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name='user-context-remote',
-    version='0.0.81',  # https://pypi.org/project/user-context-remote/
+    version='0.0.82',  # https://pypi.org/project/user-context-remote/
     author="Circles",
     author_email="info@circles.ai",
     description="PyPI Package for Circles User Context Local/Remote Python",
     long_description="This is a package for sharing common user-context-remote functions used in different repositories",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

### Comparing `user_context_remote-0.0.81/user_context_remote/src/user_context.py` & `user_context_remote-0.0.82/user_context_remote/src/user_context.py`

 * *Files identical despite different names*

### Comparing `user_context_remote-0.0.81/user_context_remote.egg-info/PKG-INFO` & `user_context_remote-0.0.82/user_context_remote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-context-remote
-Version: 0.0.81
+Version: 0.0.82
 Summary: PyPI Package for Circles User Context Local/Remote Python
 Home-page: https://github.com/circles-zone/user-context-remote-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

