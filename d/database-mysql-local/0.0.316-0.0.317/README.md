# Comparing `tmp/database_mysql_local-0.0.316.tar.gz` & `tmp/database_mysql_local-0.0.317.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.316.tar", last modified: Thu May 23 03:20:53 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.317.tar", last modified: Thu May 23 05:30:53 2024, max compression
```

## Comparing `database_mysql_local-0.0.316.tar` & `database_mysql_local-0.0.317.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:53.192987 database_mysql_local-0.0.316/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 03:20:53.192987 database_mysql_local-0.0.316/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:53.184987 database_mysql_local-0.0.316/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:53.192987 database_mysql_local-0.0.316/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-23 03:20:22.000000 database_mysql_local-0.0.316/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-23 03:20:22.000000 database_mysql_local-0.0.316/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    53518 2024-05-23 03:20:22.000000 database_mysql_local-0.0.316/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30330 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   630215 2024-05-23 03:20:19.000000 database_mysql_local-0.0.316/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:53.192987 database_mysql_local-0.0.316/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 03:20:53.000000 database_mysql_local-0.0.316/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-23 03:20:53.000000 database_mysql_local-0.0.316/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 03:20:53.000000 database_mysql_local-0.0.316/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-23 03:20:53.000000 database_mysql_local-0.0.316/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 03:20:53.000000 database_mysql_local-0.0.316/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 03:20:53.192987 database_mysql_local-0.0.316/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 03:20:22.000000 database_mysql_local-0.0.316/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:30:53.773695 database_mysql_local-0.0.317/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 05:29:56.000000 database_mysql_local-0.0.317/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 05:30:53.773695 database_mysql_local-0.0.317/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-23 05:29:56.000000 database_mysql_local-0.0.317/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:30:53.769695 database_mysql_local-0.0.317/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:30:53.773695 database_mysql_local-0.0.317/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 05:29:56.000000 database_mysql_local-0.0.317/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-23 05:29:56.000000 database_mysql_local-0.0.317/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-23 05:29:56.000000 database_mysql_local-0.0.317/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-23 05:29:56.000000 database_mysql_local-0.0.317/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54232 2024-05-23 05:30:21.000000 database_mysql_local-0.0.317/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30330 2024-05-23 05:29:56.000000 database_mysql_local-0.0.317/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-23 05:29:56.000000 database_mysql_local-0.0.317/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-23 05:29:56.000000 database_mysql_local-0.0.317/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-23 05:29:56.000000 database_mysql_local-0.0.317/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-23 05:29:56.000000 database_mysql_local-0.0.317/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   238517 2024-05-23 05:30:21.000000 database_mysql_local-0.0.317/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   630215 2024-05-23 05:30:19.000000 database_mysql_local-0.0.317/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-23 05:29:56.000000 database_mysql_local-0.0.317/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-23 05:30:21.000000 database_mysql_local-0.0.317/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:30:53.773695 database_mysql_local-0.0.317/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 05:30:53.000000 database_mysql_local-0.0.317/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-23 05:30:53.000000 database_mysql_local-0.0.317/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 05:30:53.000000 database_mysql_local-0.0.317/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-23 05:30:53.000000 database_mysql_local-0.0.317/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 05:30:53.000000 database_mysql_local-0.0.317/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-23 05:29:56.000000 database_mysql_local-0.0.317/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 05:30:53.773695 database_mysql_local-0.0.317/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 05:29:56.000000 database_mysql_local-0.0.317/setup.py
```

### Comparing `database_mysql_local-0.0.316/PKG-INFO` & `database_mysql_local-0.0.317/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.316
+Version: 0.0.317
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.316/README.md` & `database_mysql_local-0.0.317/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.316/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.317/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.316/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.317/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.316/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.317/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.316/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.317/database_mysql_local/src/generic_crud.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from database_infrastructure_local.number_generator import NumberGenerator
 from logger_local.MetaLogger import MetaLogger
 from user_context_remote.user_context import UserContext
 
 from .connector import Connector
 from .constants import DEFAULT_SQL_SELECT_LIMIT, LOGGER_CRUD_CODE_OBJECT
 from .cursor import Cursor
+from .table_columns import table_columns
 from .table_definition import table_definition
 from .utils import (process_insert_data_dict, process_update_data_dict, get_where_params, where_skip_null_values,
                     validate_none_select_table_name, validate_single_clause_value,
                     validate_select_table_name, detect_if_is_test_data, generate_table_name,
                     generate_view_name, generate_column_name, get_entity_type_by_table_name)
 
 
@@ -356,14 +357,31 @@
                        f"WHERE {where};"
 
         self.cursor.execute(update_query, params)
         self.connection.commit()
         affected_rows = self.cursor.get_row_count()
         return affected_rows
 
+    @lru_cache(maxsize=64)
+    def _replace_view_with_table(self, view_table_name: str) -> str:
+        # test data does not appear in the view, but we still wants to access it in tests.
+        if not view_table_name:
+            return view_table_name
+        # Guess the table name from the view name:
+        table_name = view_table_name.replace("_view", "_table")
+        for table, values in table_definition.items():
+            if values["view_name"] == view_table_name:
+                table_name = table  # got a better guess
+                break
+        if all(  # if all columns in the view present in the table.
+                col in table_columns.get(table_name, []) for col in table_columns.get(view_table_name, [])):
+            view_table_name = table_name
+            return view_table_name
+        return table_name
+
     # Main select function
     def select_multi_tuple_by_where(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             where: str = None, params: tuple = None, distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT,
             order_by: str = "") -> list:
         """Selects multiple rows from the table based on a WHERE clause and returns them as a list of tuples."""
 
@@ -372,21 +390,20 @@
         select_clause_value = select_clause_value or self.default_select_clause_value
         where = where or self.default_where
         where = self.__where_security(where=where, view_name=view_table_name)
         self._validate_args(args=locals())
 
         # TODO: add ` to column names if they are not reserved words (like COUNT, ST_X(point), etc.)
         # select_clause_value = ",".join([f"`{x.strip()}`" for x in select_clause_value.split(",") if x != "*"])
-        # TODO: allow other tables too
-        if (self.is_test_data and (view_table_name or "").replace("_view", "") ==
-                (self.default_table_name or "").replace("_table", "")):
-            # test data does not appear in the view, but we still wants to access it in tests (partial solution).
-            view_table_name = self.default_table_name
-            if where:
-                where += " AND end_timestamp IS NULL "  # not deleted
+
+        if self.is_test_data:
+            view_table_name = self._replace_view_with_table(view_table_name)
+
+        if where and "end_timestamp" not in where and "end_timestamp" in table_columns.get(view_table_name, []):
+            where += " AND end_timestamp IS NULL "  # not deleted
         select_query = f"SELECT {'DISTINCT' if distinct else ''} {select_clause_value} " \
                        f"FROM `{schema_name}`.`{view_table_name}` " + \
                        (f"WHERE {where} " if where else "") + \
                        (f"ORDER BY {order_by} " if order_by else "") + \
                        f"LIMIT {limit};"
 
         self.connection.commit()  # https://bugs.mysql.com/bug.php?id=102053
```

### Comparing `database_mysql_local-0.0.316/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.317/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.316/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.317/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.316/database_mysql_local/src/point.py` & `database_mysql_local-0.0.317/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.316/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.317/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.316/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.317/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.316/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.317/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.316/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.317/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.316/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.317/database_mysql_local/src/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import inspect
 import os
-import re
 from functools import lru_cache
 from typing import Any, Optional
 
 from python_sdk_remote.utilities import get_environment_name
 from url_remote.environment_name_enum import EnvironmentName
 
 from .table_definition import table_definition
@@ -83,20 +82,23 @@
 def generate_table_name(schema_name: Optional[str]) -> Optional[str]:
     if schema_name:
         return schema_name + "_table"
 
 
 def generate_view_name(table_name: Optional[str]) -> Optional[str]:
     if table_name:
-        return re.sub(r'(_table)$', '_view', table_name)
+        view_name = table_name.replace("_table", "_view")
+        return view_name
+    return table_name
 
 
 def generate_column_name(table_name: Optional[str]) -> Optional[str]:
     if table_name:
-        return re.sub(r'(_table)$', '_id', table_name)
+        column_name = table_name.replace("_table", "_id")
+        return column_name
 
 
 def validate_single_clause_value(select_clause_value: str = None) -> None:
     if "," in select_clause_value or select_clause_value == "*":
         raise ValueError("select value requires a single column name")
```

### Comparing `database_mysql_local-0.0.316/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.317/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.316
+Version: 0.0.317
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.316/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.317/database_mysql_local.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,10 +13,11 @@
 database_mysql_local/src/cursor.py
 database_mysql_local/src/generic_crud.py
 database_mysql_local/src/generic_crud_ml.py
 database_mysql_local/src/generic_mapping.py
 database_mysql_local/src/point.py
 database_mysql_local/src/polygon.py
 database_mysql_local/src/sync_conflict_resolution.py
+database_mysql_local/src/table_columns.py
 database_mysql_local/src/table_definition.py
 database_mysql_local/src/to_sql_interface.py
 database_mysql_local/src/utils.py
```

### Comparing `database_mysql_local-0.0.316/pyproject.toml` & `database_mysql_local-0.0.317/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.316/setup.py` & `database_mysql_local-0.0.317/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.316',
+    version='0.0.317',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

