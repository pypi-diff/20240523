# Comparing `tmp/profile_zoominfo_graphql_imp_local-0.0.12.tar.gz` & `tmp/profile_zoominfo_graphql_imp_local-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profile_zoominfo_graphql_imp_local-0.0.12.tar", last modified: Tue May 21 14:07:39 2024, max compression
+gzip compressed data, was "profile_zoominfo_graphql_imp_local-0.0.13.tar", last modified: Thu May 23 04:56:58 2024, max compression
```

## Comparing `profile_zoominfo_graphql_imp_local-0.0.12.tar` & `profile_zoominfo_graphql_imp_local-0.0.13.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:07:39.786642 profile_zoominfo_graphql_imp_local-0.0.12/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-21 14:07:39.786642 profile_zoominfo_graphql_imp_local-0.0.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-21 14:07:08.000000 profile_zoominfo_graphql_imp_local-0.0.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:07:39.782642 profile_zoominfo_graphql_imp_local-0.0.12/profile_zoominfo_graphql_imp_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:07:39.786642 profile_zoominfo_graphql_imp_local-0.0.12/profile_zoominfo_graphql_imp_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)    10594 2024-05-21 14:07:08.000000 profile_zoominfo_graphql_imp_local-0.0.12/profile_zoominfo_graphql_imp_local/src/ZoomInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 14:07:08.000000 profile_zoominfo_graphql_imp_local-0.0.12/profile_zoominfo_graphql_imp_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-21 14:07:08.000000 profile_zoominfo_graphql_imp_local-0.0.12/profile_zoominfo_graphql_imp_local/src/constants_zoominfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:07:39.786642 profile_zoominfo_graphql_imp_local-0.0.12/profile_zoominfo_graphql_imp_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-21 14:07:39.000000 profile_zoominfo_graphql_imp_local-0.0.12/profile_zoominfo_graphql_imp_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-21 14:07:39.000000 profile_zoominfo_graphql_imp_local-0.0.12/profile_zoominfo_graphql_imp_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 14:07:39.000000 profile_zoominfo_graphql_imp_local-0.0.12/profile_zoominfo_graphql_imp_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-21 14:07:39.000000 profile_zoominfo_graphql_imp_local-0.0.12/profile_zoominfo_graphql_imp_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-21 14:07:39.000000 profile_zoominfo_graphql_imp_local-0.0.12/profile_zoominfo_graphql_imp_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-21 14:07:08.000000 profile_zoominfo_graphql_imp_local-0.0.12/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 14:07:39.786642 profile_zoominfo_graphql_imp_local-0.0.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-21 14:07:08.000000 profile_zoominfo_graphql_imp_local-0.0.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:56:58.407223 profile_zoominfo_graphql_imp_local-0.0.13/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-23 04:56:58.407223 profile_zoominfo_graphql_imp_local-0.0.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-23 04:56:25.000000 profile_zoominfo_graphql_imp_local-0.0.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:56:58.403223 profile_zoominfo_graphql_imp_local-0.0.13/profile_zoominfo_graphql_imp_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:56:58.407223 profile_zoominfo_graphql_imp_local-0.0.13/profile_zoominfo_graphql_imp_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-05-23 04:56:25.000000 profile_zoominfo_graphql_imp_local-0.0.13/profile_zoominfo_graphql_imp_local/src/ZoomInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 04:56:25.000000 profile_zoominfo_graphql_imp_local-0.0.13/profile_zoominfo_graphql_imp_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-23 04:56:25.000000 profile_zoominfo_graphql_imp_local-0.0.13/profile_zoominfo_graphql_imp_local/src/constants_zoominfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:56:58.407223 profile_zoominfo_graphql_imp_local-0.0.13/profile_zoominfo_graphql_imp_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-23 04:56:58.000000 profile_zoominfo_graphql_imp_local-0.0.13/profile_zoominfo_graphql_imp_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-23 04:56:58.000000 profile_zoominfo_graphql_imp_local-0.0.13/profile_zoominfo_graphql_imp_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 04:56:58.000000 profile_zoominfo_graphql_imp_local-0.0.13/profile_zoominfo_graphql_imp_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-23 04:56:58.000000 profile_zoominfo_graphql_imp_local-0.0.13/profile_zoominfo_graphql_imp_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-23 04:56:58.000000 profile_zoominfo_graphql_imp_local-0.0.13/profile_zoominfo_graphql_imp_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-23 04:56:25.000000 profile_zoominfo_graphql_imp_local-0.0.13/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 04:56:58.407223 profile_zoominfo_graphql_imp_local-0.0.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-23 04:56:25.000000 profile_zoominfo_graphql_imp_local-0.0.13/setup.py
```

### Comparing `profile_zoominfo_graphql_imp_local-0.0.12/PKG-INFO` & `profile_zoominfo_graphql_imp_local-0.0.13/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profile-zoominfo-graphql-imp-local
-Version: 0.0.12
+Version: 0.0.13
 Home-page: https://github.com/circles-zone/profile-zoominfo-graphql-imp-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `profile_zoominfo_graphql_imp_local-0.0.12/profile_zoominfo_graphql_imp_local/src/ZoomInfo.py` & `profile_zoominfo_graphql_imp_local-0.0.13/profile_zoominfo_graphql_imp_local/src/ZoomInfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,14 +250,15 @@
     def generate_compatible_dict(user_info: dict) -> dict:
         plan_type_dict = {
             1: "Basic",
             2: "Licensed",
             99: "None (can only be set with ssoCreate)"
         }
 
+        # TODO Please add _dict suffix to all those objects
         person = {}
 
         profile = {
             'name': user_info['display_name'],
             'title_approved': True,
             'lang_code': user_info['language'],
             'user_id': user_info['id'],
```

### Comparing `profile_zoominfo_graphql_imp_local-0.0.12/profile_zoominfo_graphql_imp_local/src/constants_zoominfo.py` & `profile_zoominfo_graphql_imp_local-0.0.13/profile_zoominfo_graphql_imp_local/src/constants_zoominfo.py`

 * *Files identical despite different names*

### Comparing `profile_zoominfo_graphql_imp_local-0.0.12/profile_zoominfo_graphql_imp_local.egg-info/PKG-INFO` & `profile_zoominfo_graphql_imp_local-0.0.13/profile_zoominfo_graphql_imp_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profile-zoominfo-graphql-imp-local
-Version: 0.0.12
+Version: 0.0.13
 Home-page: https://github.com/circles-zone/profile-zoominfo-graphql-imp-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `profile_zoominfo_graphql_imp_local-0.0.12/pyproject.toml` & `profile_zoominfo_graphql_imp_local-0.0.13/pyproject.toml`

 * *Files identical despite different names*

### Comparing `profile_zoominfo_graphql_imp_local-0.0.12/setup.py` & `profile_zoominfo_graphql_imp_local-0.0.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 PACKAGE_NAME = "profile-zoominfo-graphql-imp-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/profile-zoominfo-graphql-imp-local
-    version='0.0.12',
+    version='0.0.13',
     author="Circles",
     author_email="info@circlez.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f"{package_dir}/src"},
     package_data={package_dir: ['*.py']},
     long_description="Profile ZoomInfo GraphQL Implementation Local Python Package",
```

