# Comparing `tmp/profile_zoominfo_graphql_imp_local-0.0.17.tar.gz` & `tmp/profile_zoominfo_graphql_imp_local-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profile_zoominfo_graphql_imp_local-0.0.17.tar", last modified: Thu May 23 13:38:02 2024, max compression
+gzip compressed data, was "profile_zoominfo_graphql_imp_local-0.0.18.tar", last modified: Thu May 23 14:28:42 2024, max compression
```

## Comparing `profile_zoominfo_graphql_imp_local-0.0.17.tar` & `profile_zoominfo_graphql_imp_local-0.0.18.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:38:02.634307 profile_zoominfo_graphql_imp_local-0.0.17/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-23 13:38:02.634307 profile_zoominfo_graphql_imp_local-0.0.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-23 13:37:34.000000 profile_zoominfo_graphql_imp_local-0.0.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:38:02.630307 profile_zoominfo_graphql_imp_local-0.0.17/profile_zoominfo_graphql_imp_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:38:02.634307 profile_zoominfo_graphql_imp_local-0.0.17/profile_zoominfo_graphql_imp_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-05-23 13:37:34.000000 profile_zoominfo_graphql_imp_local-0.0.17/profile_zoominfo_graphql_imp_local/src/ZoomInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 13:37:34.000000 profile_zoominfo_graphql_imp_local-0.0.17/profile_zoominfo_graphql_imp_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-23 13:37:34.000000 profile_zoominfo_graphql_imp_local-0.0.17/profile_zoominfo_graphql_imp_local/src/constants_zoominfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:38:02.634307 profile_zoominfo_graphql_imp_local-0.0.17/profile_zoominfo_graphql_imp_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-23 13:38:02.000000 profile_zoominfo_graphql_imp_local-0.0.17/profile_zoominfo_graphql_imp_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-23 13:38:02.000000 profile_zoominfo_graphql_imp_local-0.0.17/profile_zoominfo_graphql_imp_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 13:38:02.000000 profile_zoominfo_graphql_imp_local-0.0.17/profile_zoominfo_graphql_imp_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-23 13:38:02.000000 profile_zoominfo_graphql_imp_local-0.0.17/profile_zoominfo_graphql_imp_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-23 13:38:02.000000 profile_zoominfo_graphql_imp_local-0.0.17/profile_zoominfo_graphql_imp_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-23 13:37:34.000000 profile_zoominfo_graphql_imp_local-0.0.17/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 13:38:02.634307 profile_zoominfo_graphql_imp_local-0.0.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-23 13:37:34.000000 profile_zoominfo_graphql_imp_local-0.0.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:28:42.637395 profile_zoominfo_graphql_imp_local-0.0.18/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-23 14:28:42.637395 profile_zoominfo_graphql_imp_local-0.0.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-23 14:28:18.000000 profile_zoominfo_graphql_imp_local-0.0.18/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:28:42.633395 profile_zoominfo_graphql_imp_local-0.0.18/profile_zoominfo_graphql_imp_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:28:42.633395 profile_zoominfo_graphql_imp_local-0.0.18/profile_zoominfo_graphql_imp_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-05-23 14:28:18.000000 profile_zoominfo_graphql_imp_local-0.0.18/profile_zoominfo_graphql_imp_local/src/ZoomInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:28:18.000000 profile_zoominfo_graphql_imp_local-0.0.18/profile_zoominfo_graphql_imp_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-23 14:28:18.000000 profile_zoominfo_graphql_imp_local-0.0.18/profile_zoominfo_graphql_imp_local/src/constants_zoominfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:28:42.637395 profile_zoominfo_graphql_imp_local-0.0.18/profile_zoominfo_graphql_imp_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-23 14:28:42.000000 profile_zoominfo_graphql_imp_local-0.0.18/profile_zoominfo_graphql_imp_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-23 14:28:42.000000 profile_zoominfo_graphql_imp_local-0.0.18/profile_zoominfo_graphql_imp_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:28:42.000000 profile_zoominfo_graphql_imp_local-0.0.18/profile_zoominfo_graphql_imp_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-23 14:28:42.000000 profile_zoominfo_graphql_imp_local-0.0.18/profile_zoominfo_graphql_imp_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-23 14:28:42.000000 profile_zoominfo_graphql_imp_local-0.0.18/profile_zoominfo_graphql_imp_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-23 14:28:18.000000 profile_zoominfo_graphql_imp_local-0.0.18/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 14:28:42.637395 profile_zoominfo_graphql_imp_local-0.0.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-23 14:28:18.000000 profile_zoominfo_graphql_imp_local-0.0.18/setup.py
```

### Comparing `profile_zoominfo_graphql_imp_local-0.0.17/PKG-INFO` & `profile_zoominfo_graphql_imp_local-0.0.18/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profile-zoominfo-graphql-imp-local
-Version: 0.0.17
+Version: 0.0.18
 Home-page: https://github.com/circles-zone/profile-zoominfo-graphql-imp-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `profile_zoominfo_graphql_imp_local-0.0.17/profile_zoominfo_graphql_imp_local/src/ZoomInfo.py` & `profile_zoominfo_graphql_imp_local-0.0.18/profile_zoominfo_graphql_imp_local/src/ZoomInfo.py`

 * *Files identical despite different names*

### Comparing `profile_zoominfo_graphql_imp_local-0.0.17/profile_zoominfo_graphql_imp_local/src/constants_zoominfo.py` & `profile_zoominfo_graphql_imp_local-0.0.18/profile_zoominfo_graphql_imp_local/src/constants_zoominfo.py`

 * *Files identical despite different names*

### Comparing `profile_zoominfo_graphql_imp_local-0.0.17/profile_zoominfo_graphql_imp_local.egg-info/PKG-INFO` & `profile_zoominfo_graphql_imp_local-0.0.18/profile_zoominfo_graphql_imp_local.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profile-zoominfo-graphql-imp-local
-Version: 0.0.17
+Version: 0.0.18
 Home-page: https://github.com/circles-zone/profile-zoominfo-graphql-imp-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `profile_zoominfo_graphql_imp_local-0.0.17/pyproject.toml` & `profile_zoominfo_graphql_imp_local-0.0.18/pyproject.toml`

 * *Files identical despite different names*

### Comparing `profile_zoominfo_graphql_imp_local-0.0.17/setup.py` & `profile_zoominfo_graphql_imp_local-0.0.18/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools  
 
 PACKAGE_NAME = "profile-zoominfo-graphql-imp-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/profile-zoominfo-graphql-imp-local
-    version='0.0.17',
+    version='0.0.18',
     author="Circles",
     author_email="info@circlez.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f"{package_dir}/src"},
     package_data={package_dir: ['*.py']},
     long_description="Profile ZoomInfo GraphQL Implementation Local Python Package",
```

