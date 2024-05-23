# Comparing `tmp/database_mysql_local-0.0.319.tar.gz` & `tmp/database_mysql_local-0.0.320.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.319.tar", last modified: Thu May 23 05:48:08 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.320.tar", last modified: Thu May 23 06:13:25 2024, max compression
```

## Comparing `database_mysql_local-0.0.319.tar` & `database_mysql_local-0.0.320.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:48:08.431249 database_mysql_local-0.0.319/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 05:48:08.431249 database_mysql_local-0.0.319/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:48:08.427250 database_mysql_local-0.0.319/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:48:08.431249 database_mysql_local-0.0.319/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    54266 2024-05-23 05:47:36.000000 database_mysql_local-0.0.319/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30330 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   238517 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   630215 2024-05-23 05:47:33.000000 database_mysql_local-0.0.319/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:48:08.431249 database_mysql_local-0.0.319/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 05:48:08.000000 database_mysql_local-0.0.319/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-23 05:48:08.000000 database_mysql_local-0.0.319/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 05:48:08.000000 database_mysql_local-0.0.319/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-23 05:48:08.000000 database_mysql_local-0.0.319/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 05:48:08.000000 database_mysql_local-0.0.319/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 05:48:08.431249 database_mysql_local-0.0.319/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 05:47:36.000000 database_mysql_local-0.0.319/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:13:25.939982 database_mysql_local-0.0.320/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 06:12:30.000000 database_mysql_local-0.0.320/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 06:13:25.939982 database_mysql_local-0.0.320/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-23 06:12:30.000000 database_mysql_local-0.0.320/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:13:25.931982 database_mysql_local-0.0.320/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:13:25.935982 database_mysql_local-0.0.320/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 06:12:30.000000 database_mysql_local-0.0.320/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-23 06:12:55.000000 database_mysql_local-0.0.320/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-23 06:12:30.000000 database_mysql_local-0.0.320/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-23 06:12:30.000000 database_mysql_local-0.0.320/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53155 2024-05-23 06:12:55.000000 database_mysql_local-0.0.320/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30338 2024-05-23 06:12:55.000000 database_mysql_local-0.0.320/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-23 06:12:30.000000 database_mysql_local-0.0.320/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-23 06:12:30.000000 database_mysql_local-0.0.320/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-23 06:12:30.000000 database_mysql_local-0.0.320/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-23 06:12:30.000000 database_mysql_local-0.0.320/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   238517 2024-05-23 06:12:30.000000 database_mysql_local-0.0.320/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   630215 2024-05-23 06:12:52.000000 database_mysql_local-0.0.320/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-23 06:12:30.000000 database_mysql_local-0.0.320/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-23 06:12:55.000000 database_mysql_local-0.0.320/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:13:25.935982 database_mysql_local-0.0.320/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 06:13:25.000000 database_mysql_local-0.0.320/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-23 06:13:25.000000 database_mysql_local-0.0.320/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 06:13:25.000000 database_mysql_local-0.0.320/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-23 06:13:25.000000 database_mysql_local-0.0.320/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 06:13:25.000000 database_mysql_local-0.0.320/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-23 06:12:30.000000 database_mysql_local-0.0.320/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 06:13:25.939982 database_mysql_local-0.0.320/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 06:12:55.000000 database_mysql_local-0.0.320/setup.py
```

### Comparing `database_mysql_local-0.0.319/PKG-INFO` & `database_mysql_local-0.0.320/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.319
+Version: 0.0.320
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.319/README.md` & `database_mysql_local-0.0.320/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.319/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.320/database_mysql_local/src/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations  # Required for type hinting in class methods
 
 from typing import Optional
 
 import mysql.connector
 from logger_local.LoggerLocal import Logger
 from logger_local.MetaLogger import MetaLogger
-from python_sdk_remote.utilities import get_sql_hostname, get_sql_username, get_sql_password
+from python_sdk_remote.utilities import (get_sql_hostname, get_sql_password,
+                                         get_sql_username)
 
 from .constants import LOGGER_CONNECTOR_CODE_OBJECT
 from .cursor import Cursor
 
 logger = Logger.create_logger(object=LOGGER_CONNECTOR_CODE_OBJECT)
 connections_pool = {}
 
@@ -87,15 +88,16 @@
         except Exception as exception:
             logger.error(f"connection.py close() {self.database_info()}", object={"exception": exception})
         connections_pool.pop(self.schema, None)
         if self.connection and self.connection.is_connected():
             self.connection.close()
             logger.info("Connection closed successfully.")
 
-    def cursor(self, *, close_previous: bool = True, cache_previous: bool = False, dictionary: bool = None, buffered: bool = None, raw: bool = None,
+    def cursor(self, *, close_previous: bool = True, cache_previous: bool = False, dictionary: bool = None,
+               buffered: bool = None, raw: bool = None,
                prepared: bool = None, named_tuple: bool = None, cursor_class=None) -> Cursor:
         # if cache_previous and self._cursor:
         #     cursor_instance = self._cursor
         #     return cursor_instance
         # if close_previous and self._cursor:
         #     self._cursor.close()
```

### Comparing `database_mysql_local-0.0.319/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.320/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.319/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.320/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.319/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.320/database_mysql_local/src/generic_crud.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,21 @@
 from user_context_remote.user_context import UserContext
 
 from .connector import Connector
 from .constants import DEFAULT_SQL_SELECT_LIMIT, LOGGER_CRUD_CODE_OBJECT
 from .cursor import Cursor
 from .table_columns import table_columns
 from .table_definition import table_definition
-from .utils import (process_insert_data_dict, process_update_data_dict, get_where_params, where_skip_null_values,
-                    validate_none_select_table_name, validate_single_clause_value,
-                    validate_select_table_name, detect_if_is_test_data, generate_table_name,
-                    generate_view_name, generate_column_name, get_entity_type_by_table_name)
+from .utils import (detect_if_is_test_data, generate_column_name,
+                    generate_table_name, generate_view_name,
+                    get_entity_type_by_table_name, get_where_params,
+                    process_insert_data_dict, process_update_data_dict,
+                    replace_view_with_table, validate_none_select_table_name,
+                    validate_select_table_name, validate_single_clause_value,
+                    where_skip_null_values)
 
 
 class GenericCRUD(metaclass=MetaLogger, object=LOGGER_CRUD_CODE_OBJECT):
     """A class that provides generic CRUD functionality.
     There are 4 main functions to create, read, update, and delete data from the database.
     The rest of the functions are helper functions or wrappers around the main functions."""
 
@@ -61,30 +64,29 @@
                 self.logger.warning(
                     "GenericCRUD: id_column_name and id_column_value are deprecated and scheduled to be removed by 12/06/2024, use column_name and column_value instead.")
             return id_column_name
         return column_name
 
     def insert(self, *, schema_name: str = None, table_name: str = None, data_dict: dict = None, data_json: dict = None,
                ignore_duplicate: bool = False, commit_changes: bool = True) -> int:
-               # TODO raise_if_database_raise: bool = True,
-               # get_id_of_existing_exact_match: bool = True) -> int:
+        # TODO raise_if_database_raise: bool = True,
+        # get_id_of_existing_exact_match: bool = True) -> int:
         """Inserts a new row into the table and returns the id of the new row or -1 if an error occurred.
         ignore_duplicate should be False as default, because for example if a user register with existing name,
             he should get an error and not existing id
         """
         # if ignore_duplicate is not None:
         #     self.logger.warning("GenericCRUD.insert: ignore_duplicate is deprecated")
         data_dict = data_json or self._data_json_to_dict(data_dict)
-        if ignore_duplicate:
-            self.logger.warning(f"GenericCRUD.insert({schema_name}.{table_name}) using ignore_duplicate, is it needed?",
-                                object={"data_dict": data_dict})
-
         table_name = table_name or self.default_table_name
         schema_name = schema_name or self.default_schema_name
         self._validate_args(args=locals())
+        if ignore_duplicate:
+            self.logger.warning(f"GenericCRUD.insert({schema_name}.{table_name}) using ignore_duplicate, is it needed?",
+                                object={"data_dict": data_dict})
 
         # if table_name in table_definition:
         #     if table_definition[table_name]["is_number_column"]:
         #         view_name = self._get_view_name(table_name)
         #         number = NumberGenerator.get_random_number(schema_name=schema_name, view_name=view_name)
         #         data_dict["number"] = number
         # else:
@@ -357,31 +359,14 @@
                        f"WHERE {where};"
 
         self.cursor.execute(update_query, params)
         self.connection.commit()
         affected_rows = self.cursor.get_row_count()
         return affected_rows
 
-    @lru_cache(maxsize=64)
-    @staticmethod
-    def _replace_view_with_table(view_table_name: str) -> str:
-        # test data does not appear in the view, but we still wants to access it in tests.
-        if not view_table_name:
-            return view_table_name
-        # Guess the table name from the view name:
-        table_name = view_table_name.replace("_view", "_table")
-        for table, values in table_definition.items():
-            if values["view_name"] == view_table_name:
-                table_name = table  # got a better guess
-                break
-        if table_name in table_columns and all(  # if all columns in the view present in the table.
-                col in table_columns.get(table_name, []) for col in table_columns.get(view_table_name, [])):
-            return table_name
-        return view_table_name  # appropriate table not found
-
     # Main select function
     def select_multi_tuple_by_where(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             where: str = None, params: tuple = None, distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT,
             order_by: str = "") -> list:
         """Selects multiple rows from the table based on a WHERE clause and returns them as a list of tuples."""
 
@@ -392,15 +377,15 @@
         where = self.__where_security(where=where, view_name=view_table_name)
         self._validate_args(args=locals())
 
         # TODO: add ` to column names if they are not reserved words (like COUNT, ST_X(point), etc.)
         # select_clause_value = ",".join([f"`{x.strip()}`" for x in select_clause_value.split(",") if x != "*"])
 
         if self.is_test_data:
-            view_table_name = self._replace_view_with_table(view_table_name)
+            view_table_name = replace_view_with_table(view_table_name)
 
         if where and "end_timestamp" not in where and "end_timestamp" in table_columns.get(view_table_name, []):
             where += " AND end_timestamp IS NULL "  # not deleted
         select_query = f"SELECT {'DISTINCT' if distinct else ''} {select_clause_value} " \
                        f"FROM `{schema_name}`.`{view_table_name}` " + \
                        (f"WHERE {where} " if where else "") + \
                        (f"ORDER BY {order_by} " if order_by else "") + \
@@ -420,15 +405,14 @@
         """Selects multiple rows from the table based on a WHERE clause and returns them as a list of dictionaries."""
         result = self.select_multi_tuple_by_where(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
         result_as_dicts = self.convert_multi_to_dict(result, select_clause_value)
         return result_as_dicts
 
-
     # TODO: test distinct
     def select_one_tuple_by_id(self, *, schema_name: str = None, view_table_name: str = None,
                                select_clause_value: str = None,
                                column_name: str = None, column_value: Any = None,
                                id_column_name: str = None, id_column_value: Any = None,
                                distinct: bool = False, order_by: str = "") -> tuple:
         if datetime.now() > datetime(2024, 5, 25):
@@ -684,25 +668,23 @@
         self.cursor.execute(select_query, params)
         result = self.cursor.fetchall()
 
         columns_tuple = tuple(x[0] for x in result)
         self.logger.debug(object=locals())
         return columns_tuple
 
-
     @lru_cache
     def get_primary_key(self, schema_name: str = None, table_name: str = None) -> str or None:
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         query = """
-        SELECT COLUMN_NAME
-        FROM INFORMATION_SCHEMA.KEY_COLUMN_USAGE
-        WHERE TABLE_SCHEMA = %s AND TABLE_NAME = %s AND CONSTRAINT_NAME = "PRIMARY"
-        LIMIT 1;
-        """
+            SELECT COLUMN_NAME
+            FROM INFORMATION_SCHEMA.KEY_COLUMN_USAGE
+            WHERE TABLE_SCHEMA = %s AND TABLE_NAME = %s AND CONSTRAINT_NAME = "PRIMARY"
+            LIMIT 1;"""
 
         self.connection.commit()
         self.cursor.execute(query, (schema_name, table_name))
         column_name = (self.cursor.fetchone() or [None])[0]
         return column_name
 
     # helper functions:
@@ -731,15 +713,15 @@
             if arg_name in ("self", "__class__"):
                 continue
             elif arg_name in required_args and not arg_value:
                 message = f"Invalid value for {arg_name}: {arg_value}"
             elif arg_name == "table_name":
                 validate_none_select_table_name(arg_value)
             elif arg_name == "view_table_name":
-                validate_select_table_name(arg_value, is_test_data=self.is_test_data)
+                validate_select_table_name(arg_value)
 
             # data_dict values are allowed to contain ';', as we use them with %s (TODO: unless it's ToSQLInterface)
             if ((arg_name.startswith("data_") and arg_value and any(
                     ";" in str(x) for x in arg_value.keys())) or  # check columns
                     (not arg_name.startswith("data_") and arg_name != "params" and ";" in str(arg_value))):
                 message = f"Invalid value for {arg_name}: {arg_value} (contains ';')"
 
@@ -748,17 +730,14 @@
 
     def __add_identifier(self, data_dict: dict, table_name: str) -> None:
         # If there's an "identifier" column in the table, we want to insert a random identifier
         #  to the identifier_table and use it in the data_dict.
         identifier_entity_type_id = get_entity_type_by_table_name(table_name)
         if not identifier_entity_type_id:
             return
-            # TODO Please add maximum infomation to any exception i.e. table_name, data_dict ...
-            # raise Exception("Could not find the entity_type_id1 for table " + table_name + " in database.table_definition_table")
-
         identifier = NumberGenerator.get_random_identifier(
             schema_name="identifier", view_name="identifier_view", identifier_column_name="identifier")
         data_dict["identifier"] = identifier
         # We can't use self.insert, as it would cause an infinite loop
         insert_query = "INSERT " + \
                        "INTO `identifier`.`identifier_table` (identifier, entity_type_id) " \
                        "VALUES (%s, %s);"
@@ -767,15 +746,14 @@
         self.connection.commit()
 
     # TODO: add warning logs
     def __add_create_updated_user_profile_ids(self, data_dict: dict, add_created_user_id: bool = False,
                                               schema_name: str = None, table_name: str = None) -> dict:
         """Adds created_user_id and updated_user_id to data_dict."""
         # if get_environment_name() not in (EnvironmentName.DVLP1.value, EnvironmentName.PROD1.value):
-        # TODO data_dict = data_dict.copy() ?
         data_dict = data_dict or {}
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         table_columns = self.get_table_columns(schema_name=schema_name, table_name=table_name)
         if add_created_user_id:
             if "created_user_id" in table_columns:
                 data_dict["created_user_id"] = self.user_context.get_effective_user_id()
```

### Comparing `database_mysql_local-0.0.319/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.320/database_mysql_local/src/generic_crud_ml.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 from language_remote.lang_code import LangCode
 from logger_local.MetaLogger import MetaLogger
 from user_context_remote.user_context import UserContext
 
 from .constants import DEFAULT_SQL_SELECT_LIMIT, LOGGER_CRUD_ML_CODE_OBJECT
 from .generic_crud import GenericCRUD
-from .utils import generate_column_name, generate_view_name
 from .table_definition import table_definition
+from .utils import generate_column_name, generate_view_name
 
 IS_MAIN_COLUMN_NAME = "is_main"
 
 
 # TODO If I understand, there are two things:
 # is_main in data_ml_dict
 # table_definition_table.is_main_column
@@ -376,15 +376,15 @@
             schema_name=schema_name, view_table_name=self.default_ml_view_table_name,
             where=f"{column_name}=%s AND lang_code=%s", params=(table_id, lang_code_str),
             order_by=order_by)
         return result
 
     def get_main_values_tuple(self, *, table_id: int, column_name: str = None, id_column_name: str = None,
                               select_clause_value: str = "*", order_by: str = None, schema_name: str = None) -> (
-    int, int):
+            int, int):
         schema_name = schema_name or self.default_schema_name
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_name = column_name or generate_column_name(
             self.default_table_name)
         result = self.select_one_tuple_by_where(
             schema_name=schema_name, view_table_name=self.default_ml_view_table_name,
             where=f"{column_name}=%s AND is_main=True", params=(table_id,),
```

### Comparing `database_mysql_local-0.0.319/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.320/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.319/database_mysql_local/src/point.py` & `database_mysql_local-0.0.320/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.319/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.320/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.319/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.320/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.319/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.320/database_mysql_local/src/table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.319/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.320/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.319/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.320/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.319/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.320/database_mysql_local/src/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 import os
 from functools import lru_cache
 from typing import Any, Optional
 
 from python_sdk_remote.utilities import get_environment_name
 from url_remote.environment_name_enum import EnvironmentName
 
+from .table_columns import table_columns
 from .table_definition import table_definition
 from .to_sql_interface import ToSQLInterface
 
 
-def validate_select_table_name(database_object_name: str, is_test_data: bool = False) -> None:
+def validate_select_table_name(database_object_name: str) -> None:
     if (get_environment_name() not in (EnvironmentName.DVLP1.value, EnvironmentName.PROD1.value)
-            and not database_object_name.endswith("_view") and not is_test_data):
+            and not database_object_name.endswith("_view")):
         raise Exception(
             f"View name must end with '_view' in this environment (got {database_object_name})")
 
 
 def validate_none_select_table_name(database_object_name: str) -> None:
     if (get_environment_name() not in (EnvironmentName.DVLP1.value, EnvironmentName.PROD1.value)
             and not database_object_name.endswith("_table")):
@@ -122,7 +123,24 @@
         validate_single_clause_value(select_clause_value)
         where_skip = f"`{select_clause_value}` IS NOT NULL"
         if where:
             where += f" AND {where_skip}"
         else:
             where = where_skip
     return where
+
+
+@lru_cache(maxsize=64)
+def replace_view_with_table(view_table_name: str) -> str:
+    # test data does not appear in the view, but we still wants to access it in tests.
+    if not view_table_name:
+        return view_table_name
+    # Guess the table name from the view name:
+    table_name = view_table_name.replace("_view", "_table")
+    for table, values in table_definition.items():
+        if values["view_name"] == view_table_name:
+            table_name = table  # got a better guess
+            break
+    if table_name in table_columns and all(  # if all columns in the view present in the table.
+            col in table_columns.get(table_name, []) for col in table_columns.get(view_table_name, [])):
+        return table_name
+    return view_table_name  # appropriate table not found
```

### Comparing `database_mysql_local-0.0.319/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.320/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.319
+Version: 0.0.320
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.319/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.320/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.319/pyproject.toml` & `database_mysql_local-0.0.320/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.319/setup.py` & `database_mysql_local-0.0.320/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.319',
+    version='0.0.320',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

