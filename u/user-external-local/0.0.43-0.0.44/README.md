# Comparing `tmp/user_external_local-0.0.43.tar.gz` & `tmp/user_external_local-0.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_external_local-0.0.43.tar", last modified: Sun May 12 15:18:50 2024, max compression
+gzip compressed data, was "user_external_local-0.0.44.tar", last modified: Thu May 23 18:52:42 2024, max compression
```

## Comparing `user_external_local-0.0.43.tar` & `user_external_local-0.0.44.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:18:50.310273 user_external_local-0.0.43/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-12 15:18:50.310273 user_external_local-0.0.43/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-12 15:18:30.000000 user_external_local-0.0.43/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-12 15:18:30.000000 user_external_local-0.0.43/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 15:18:50.310273 user_external_local-0.0.43/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-12 15:18:30.000000 user_external_local-0.0.43/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:18:50.310273 user_external_local-0.0.43/user_external_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:18:50.310273 user_external_local-0.0.43/user_external_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 15:18:30.000000 user_external_local-0.0.43/user_external_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11279 2024-05-12 15:18:30.000000 user_external_local-0.0.43/user_external_local/src/user_externals_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:18:50.310273 user_external_local-0.0.43/user_external_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-12 15:18:50.000000 user_external_local-0.0.43/user_external_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-12 15:18:50.000000 user_external_local-0.0.43/user_external_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 15:18:50.000000 user_external_local-0.0.43/user_external_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-12 15:18:50.000000 user_external_local-0.0.43/user_external_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-12 15:18:50.000000 user_external_local-0.0.43/user_external_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:52:42.418931 user_external_local-0.0.44/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-23 18:52:42.418931 user_external_local-0.0.44/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-23 18:52:21.000000 user_external_local-0.0.44/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-23 18:52:21.000000 user_external_local-0.0.44/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:52:42.418931 user_external_local-0.0.44/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-23 18:52:21.000000 user_external_local-0.0.44/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:52:42.414931 user_external_local-0.0.44/user_external_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:52:42.418931 user_external_local-0.0.44/user_external_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:52:21.000000 user_external_local-0.0.44/user_external_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-05-23 18:52:21.000000 user_external_local-0.0.44/user_external_local/src/user_externals_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:52:42.418931 user_external_local-0.0.44/user_external_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-23 18:52:42.000000 user_external_local-0.0.44/user_external_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-23 18:52:42.000000 user_external_local-0.0.44/user_external_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:52:42.000000 user_external_local-0.0.44/user_external_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-23 18:52:42.000000 user_external_local-0.0.44/user_external_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-23 18:52:42.000000 user_external_local-0.0.44/user_external_local.egg-info/top_level.txt
```

### Comparing `user_external_local-0.0.43/PKG-INFO` & `user_external_local-0.0.44/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-external-local
-Version: 0.0.43
+Version: 0.0.44
 Home-page: https://github.com/circles-zone/user-external-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `user_external_local-0.0.43/README.md` & `user_external_local-0.0.44/README.md`

 * *Files identical despite different names*

### Comparing `user_external_local-0.0.43/setup.py` & `user_external_local-0.0.44/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "user-external-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/user-external-local
-    version='0.0.43',
+    version='0.0.44',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="user-external-local",
```

### Comparing `user_external_local-0.0.43/user_external_local/src/user_externals_local.py` & `user_external_local-0.0.44/user_external_local/src/user_externals_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,31 +22,30 @@
 
 class UserExternalsLocal(GenericCRUD):
     def __init__(self, is_test_data: bool = False):
         super().__init__(default_schema_name=DEFAULT_SCHEMA_NAME, default_table_name=DEFAULT_TABLE_NAME,
                          default_view_table_name=DEFAULT_VIEW_NAME, default_id_column_name=DEFAULT_ID_COLUMN_NAME,
                          is_test_data=is_test_data)
 
-    # TODO change the order of the parameters: system_id, username, profile_id ..
-    def insert_or_update_user_external_access_token(self, username: str, profile_id: int, system_id: int, access_token: str,
+    def insert_or_update_user_external_access_token(self, *, system_id: int, username: str, access_token: str, profile_id: int,
                                                     expiry=None, refresh_token: str = None) -> None:
         object_start = {
             'username': username,
             'profile_id': profile_id,
             'system_id': system_id,
             'access_token': access_token,
             'expiry': expiry,
             'refresh_token': refresh_token
         }
         logger.start(object=object_start)
         try:
-            current_token = self.get_access_token(username, profile_id, system_id)
+            current_token = self.get_access_token(system_id=system_id, username=username, profile_id=profile_id)
             if current_token is not None:
                 self.delete_access_token(
-                    username, system_id, profile_id)
+                    system_id=system_id, username=username, profile_id=profile_id)
 
             connection = Connector.connect('user_external')
             if (expiry is None):
                 expiry = ""
             if (refresh_token is None):
                 refresh_token = ""
             query_insert_external = (
@@ -75,15 +74,15 @@
             logger.info("external user inserted", object=object_info)
         except Exception as error:
             logger.exception(object=error)
             logger.end()
             raise
         logger.end(object={})
 
-    def get_access_token_by_username_and_system_id(self, username: str, system_id: int) -> str:
+    def get_access_token_by_username_and_system_id(self, *, username: str, system_id: int) -> str:
         access_token = None
         try:
             object_start = {
                 'username': username,
                 'system_id': system_id
             }
             logger.start(object=object_start)
@@ -96,17 +95,16 @@
         except Exception as error:
             logger.exception(object=error)
             logger.end()
             raise
         logger.end(object={'access_token': access_token})
         return access_token
 
-    # TODO I think think the order of the paramters should be system_id, username and profile_id
     # TODO Shall we default the profile_id to profile_id from User Context?
-    def get_access_token(self, username: str, profile_id: int, system_id: int) -> str:
+    def get_access_token(self, *, system_id: int, username: str, profile_id: int) -> str:
         access_token = None
         try:
             object_start = {
                 'username': username,
                 'profile_id': profile_id,
                 'system_id': system_id
             }
@@ -123,15 +121,15 @@
         except Exception as error:
             logger.exception(object=error)
             logger.end()
             raise
         logger.end(object={'access_token': access_token})
         return access_token
 
-    def update_user_external_access_token(self, username: str, system_id: int, profile_id: int, access_token, expiry=None,
+    def update_user_external_access_token(self, *, system_id: int, username: str, profile_id: int, access_token, expiry=None,
                                           refresh_token: str = None) -> None:
         try:
             object_start = {
                 'username': username,
                 'system_id': system_id,
                 'profile_id': profile_id,
                 'access_token': access_token,
@@ -156,15 +154,15 @@
             logger.info("external user updated", object=object_info)
         except Exception as error:
             logger.exception(object=error)
             logger.end()
             raise
         logger.end(object={})
 
-    def delete_access_token(self, username: str, system_id: int, profile_id: int):
+    def delete_access_token(self, *, system_id: int, username: str, profile_id: int):
         try:
             object_start = {
                 'username': username,
                 'system_id': system_id,
                 'profile_id': profile_id,
             }
             logger.start(object=object_start)
@@ -186,15 +184,15 @@
             logger.info("external user updated", object=object_info)
         except Exception as error:
             logger.exception(object=error)
             logger.end()
             raise
         logger.end(object={})
 
-    def get_auth_details_by_system_id_and_profile_id(self, system_id: int, profile_id: int) -> tuple:
+    def get_auth_details_by_system_id_and_profile_id(self, *, system_id: int, profile_id: int) -> tuple:
         try:
             object_start = {
                 'system_id': system_id,
                 "profile_id": profile_id
             }
             logger.warning(
                 log_message="This static method is deprecated, "
@@ -213,16 +211,15 @@
         except Exception as error:
             logger.exception(object=error)
             logger.end()
             raise
         logger.end(object={'auth_details': auth_details})
         return auth_details
 
-    # TODO Change the order of the parameters to system_id, username, profile_id
-    def get_auth_details(self, username: str, system_id: int, profile_id: int) -> None:
+    def get_auth_details(self, *, system_id: int, username: str, profile_id: int) -> None:
         auth_details = None
         try:
             object_start = {
                 "username": username,
                 'system_id': system_id,
                 "profile_id": profile_id,
             }
```

### Comparing `user_external_local-0.0.43/user_external_local.egg-info/PKG-INFO` & `user_external_local-0.0.44/user_external_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-external-local
-Version: 0.0.43
+Version: 0.0.44
 Home-page: https://github.com/circles-zone/user-external-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

