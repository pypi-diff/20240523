# Comparing `tmp/database_mysql_local-0.0.322.tar.gz` & `tmp/database_mysql_local-0.0.323.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.322.tar", last modified: Thu May 23 13:22:32 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.323.tar", last modified: Thu May 23 17:35:36 2024, max compression
```

## Comparing `database_mysql_local-0.0.322.tar` & `database_mysql_local-0.0.323.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:22:32.814921 database_mysql_local-0.0.322/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 13:21:32.000000 database_mysql_local-0.0.322/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 13:22:32.814921 database_mysql_local-0.0.322/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-23 13:21:32.000000 database_mysql_local-0.0.322/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:22:32.810921 database_mysql_local-0.0.322/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:22:32.814921 database_mysql_local-0.0.322/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 13:21:32.000000 database_mysql_local-0.0.322/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-23 13:21:32.000000 database_mysql_local-0.0.322/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-23 13:21:32.000000 database_mysql_local-0.0.322/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-23 13:21:32.000000 database_mysql_local-0.0.322/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    53155 2024-05-23 13:21:32.000000 database_mysql_local-0.0.322/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30338 2024-05-23 13:21:32.000000 database_mysql_local-0.0.322/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-23 13:21:32.000000 database_mysql_local-0.0.322/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-23 13:21:32.000000 database_mysql_local-0.0.322/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-23 13:21:32.000000 database_mysql_local-0.0.322/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-23 13:21:32.000000 database_mysql_local-0.0.322/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   238517 2024-05-23 13:21:32.000000 database_mysql_local-0.0.322/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   630215 2024-05-23 13:21:56.000000 database_mysql_local-0.0.322/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-23 13:21:32.000000 database_mysql_local-0.0.322/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-23 13:21:32.000000 database_mysql_local-0.0.322/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:22:32.814921 database_mysql_local-0.0.322/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 13:22:32.000000 database_mysql_local-0.0.322/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-23 13:22:32.000000 database_mysql_local-0.0.322/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 13:22:32.000000 database_mysql_local-0.0.322/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-23 13:22:32.000000 database_mysql_local-0.0.322/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 13:22:32.000000 database_mysql_local-0.0.322/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-23 13:21:32.000000 database_mysql_local-0.0.322/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 13:22:32.814921 database_mysql_local-0.0.322/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 13:21:59.000000 database_mysql_local-0.0.322/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:35:36.701202 database_mysql_local-0.0.323/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:34:32.000000 database_mysql_local-0.0.323/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 17:35:36.701202 database_mysql_local-0.0.323/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-23 17:34:32.000000 database_mysql_local-0.0.323/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:35:36.693202 database_mysql_local-0.0.323/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:35:36.701202 database_mysql_local-0.0.323/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:34:32.000000 database_mysql_local-0.0.323/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-23 17:34:32.000000 database_mysql_local-0.0.323/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-23 17:34:32.000000 database_mysql_local-0.0.323/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-23 17:34:32.000000 database_mysql_local-0.0.323/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53208 2024-05-23 17:35:02.000000 database_mysql_local-0.0.323/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30338 2024-05-23 17:34:32.000000 database_mysql_local-0.0.323/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-23 17:34:32.000000 database_mysql_local-0.0.323/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-23 17:34:32.000000 database_mysql_local-0.0.323/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-23 17:34:32.000000 database_mysql_local-0.0.323/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-23 17:34:32.000000 database_mysql_local-0.0.323/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   238517 2024-05-23 17:34:32.000000 database_mysql_local-0.0.323/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   630215 2024-05-23 17:34:59.000000 database_mysql_local-0.0.323/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-23 17:34:32.000000 database_mysql_local-0.0.323/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-23 17:35:02.000000 database_mysql_local-0.0.323/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:35:36.701202 database_mysql_local-0.0.323/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 17:35:36.000000 database_mysql_local-0.0.323/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-23 17:35:36.000000 database_mysql_local-0.0.323/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 17:35:36.000000 database_mysql_local-0.0.323/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-23 17:35:36.000000 database_mysql_local-0.0.323/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 17:35:36.000000 database_mysql_local-0.0.323/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-23 17:35:02.000000 database_mysql_local-0.0.323/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 17:35:36.701202 database_mysql_local-0.0.323/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 17:35:02.000000 database_mysql_local-0.0.323/setup.py
```

### Comparing `database_mysql_local-0.0.322/PKG-INFO` & `database_mysql_local-0.0.323/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.322
+Version: 0.0.323
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.322/README.md` & `database_mysql_local-0.0.323/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.322/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.323/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.322/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.323/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.322/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.323/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.322/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.323/database_mysql_local/src/generic_crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -713,15 +713,15 @@
             if arg_name in ("self", "__class__"):
                 continue
             elif arg_name in required_args and not arg_value:
                 message = f"Invalid value for {arg_name}: {arg_value}"
             elif arg_name == "table_name":
                 validate_none_select_table_name(arg_value)
             elif arg_name == "view_table_name":
-                validate_select_table_name(arg_value)
+                validate_select_table_name(database_object_name=arg_value, is_test_data=self.is_test_data)
 
             # data_dict values are allowed to contain ';', as we use them with %s (TODO: unless it's ToSQLInterface)
             if ((arg_name.startswith("data_") and arg_value and any(
                     ";" in str(x) for x in arg_value.keys())) or  # check columns
                     (not arg_name.startswith("data_") and arg_name != "params" and ";" in str(arg_value))):
                 message = f"Invalid value for {arg_name}: {arg_value} (contains ';')"
```

### Comparing `database_mysql_local-0.0.322/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.323/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.322/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.323/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.322/database_mysql_local/src/point.py` & `database_mysql_local-0.0.323/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.322/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.323/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.322/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.323/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.322/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.323/database_mysql_local/src/table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.322/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.323/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.322/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.323/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.322/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.323/database_mysql_local/src/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from url_remote.environment_name_enum import EnvironmentName
 
 from .table_columns import table_columns
 from .table_definition import table_definition
 from .to_sql_interface import ToSQLInterface
 
 
-def validate_select_table_name(database_object_name: str) -> None:
+def validate_select_table_name(database_object_name: str, is_test_data: bool = False) -> None:
     if (get_environment_name() not in (EnvironmentName.DVLP1.value, EnvironmentName.PROD1.value)
-            and not database_object_name.endswith("_view")):
+            and not database_object_name.endswith("_view") and not is_test_data):
         raise Exception(
             f"View name must end with '_view' in this environment (got {database_object_name})")
 
 
 def validate_none_select_table_name(database_object_name: str) -> None:
     if (get_environment_name() not in (EnvironmentName.DVLP1.value, EnvironmentName.PROD1.value)
             and not database_object_name.endswith("_table")):
```

### Comparing `database_mysql_local-0.0.322/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.323/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.322
+Version: 0.0.323
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.322/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.323/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.322/pyproject.toml` & `database_mysql_local-0.0.323/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "database-mysql-local"
-version = "0.0.308" # https://pypi.org/project/database-mysql-local
+version = "0.0.323" # https://pypi.org/project/database-mysql-local
 description = "database-mysql-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
 
 # dephell deps convert --from pyproject.toml --from-format poetry --to setup.py --to-format setuppy
```

### Comparing `database_mysql_local-0.0.322/setup.py` & `database_mysql_local-0.0.323/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.322',
+    version='0.0.323',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

