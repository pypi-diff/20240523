# Comparing `tmp/database_mysql_local-0.0.313.tar.gz` & `tmp/database_mysql_local-0.0.314.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.313.tar", last modified: Wed May 22 15:44:07 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.314.tar", last modified: Wed May 22 16:35:00 2024, max compression
```

## Comparing `database_mysql_local-0.0.313.tar` & `database_mysql_local-0.0.314.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:44:07.577252 database_mysql_local-0.0.313/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-22 15:44:07.577252 database_mysql_local-0.0.313/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:44:07.573252 database_mysql_local-0.0.313/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:44:07.577252 database_mysql_local-0.0.313/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-05-22 15:43:35.000000 database_mysql_local-0.0.313/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    53626 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30389 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   630271 2024-05-22 15:43:35.000000 database_mysql_local-0.0.313/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:44:07.577252 database_mysql_local-0.0.313/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-22 15:44:07.000000 database_mysql_local-0.0.313/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-22 15:44:07.000000 database_mysql_local-0.0.313/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:44:07.000000 database_mysql_local-0.0.313/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-22 15:44:07.000000 database_mysql_local-0.0.313/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 15:44:07.000000 database_mysql_local-0.0.313/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:44:07.577252 database_mysql_local-0.0.313/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-22 15:43:35.000000 database_mysql_local-0.0.313/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:35:00.132812 database_mysql_local-0.0.314/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-22 16:35:00.132812 database_mysql_local-0.0.314/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:35:00.124812 database_mysql_local-0.0.314/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:35:00.132812 database_mysql_local-0.0.314/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53465 2024-05-22 16:34:28.000000 database_mysql_local-0.0.314/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30389 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   630271 2024-05-22 16:34:28.000000 database_mysql_local-0.0.314/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:35:00.132812 database_mysql_local-0.0.314/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-22 16:35:00.000000 database_mysql_local-0.0.314/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-22 16:35:00.000000 database_mysql_local-0.0.314/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:35:00.000000 database_mysql_local-0.0.314/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-22 16:35:00.000000 database_mysql_local-0.0.314/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 16:35:00.000000 database_mysql_local-0.0.314/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:35:00.132812 database_mysql_local-0.0.314/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-22 16:34:28.000000 database_mysql_local-0.0.314/setup.py
```

### Comparing `database_mysql_local-0.0.313/PKG-INFO` & `database_mysql_local-0.0.314/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.313
+Version: 0.0.314
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.313/README.md` & `database_mysql_local-0.0.314/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.313/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.314/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.313/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.314/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.313/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.314/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.313/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.314/database_mysql_local/src/generic_crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def __init__(self, *, default_schema_name: str,
                  default_table_name: str = None, default_view_table_name: str = None,
                  default_column_name: str = None, default_id_column_name: str = None,
                  default_select_clause_value: str = "*", default_where: str = None, is_test_data: bool = False) -> None:
         """Initializes the GenericCRUD class. If a connection is not provided, a new connection will be created."""
         self.default_schema_name = default_schema_name
         self.connection = Connector.connect(schema_name=default_schema_name)
-        self.cursor = self.connection.cursor()
+        self._cursor = self.connection.cursor()
         column_name = self._deprecated_id_column(default_id_column_name, default_column_name)
         self.default_column_name = column_name or generate_column_name(default_table_name)
         self.default_table_name = default_table_name or generate_table_name(default_schema_name)
         self.default_view_table_name = default_view_table_name or generate_view_name(default_table_name)
         self.default_select_clause_value = default_select_clause_value
         self.default_where = default_where
         self.is_test_data = is_test_data or detect_if_is_test_data()
@@ -97,15 +97,15 @@
 
         columns, values, data_dict = process_insert_data_dict(data_dict=data_dict)
         # We removed the IGNORE from the SQL Statement as we want to return the id of the existing row
         insert_query = "INSERT " + \
                        f"INTO `{schema_name}`.`{table_name}` ({columns}) " \
                        f"VALUES ({values});"
         try:
-            cursor = self.get_cursor()
+            cursor = self.cursor
             cursor.execute(insert_query, tuple(data_dict.values()))
             if commit_changes:
                 self.connection.commit()
             inserted_id = cursor.lastrowid()
         except mysql.connector.errors.IntegrityError as exception:
             if ignore_duplicate:
                 self.logger.warning("GenericCRUD.insert: existing record found, selecting it's id."
@@ -156,15 +156,15 @@
         columns = ", ".join(f"`{key}`" for key in data_dict)
         values = ", ".join(["%s"] * len(data_dict))
         sql_statement = f"""
         INSERT INTO `{schema_name}`.`{table_name}` ({columns})
         VALUES ({values});
         """
         sql_parameters = list(zip(*data_dict.values()))
-        cursor = self.get_cursor()
+        cursor = self.cursor
         cursor.executemany(sql_statement=sql_statement, sql_parameters=sql_parameters)
         if commit_changes:
             self.connection.commit()
 
     def upsert(self, *, schema_name: str = None, table_name: str = None, view_table_name: str = None,
                data_dict: dict = None, data_json: dict = None,
                data_dict_compare: dict = None, data_json_compare: dict = None,
@@ -197,15 +197,15 @@
                 where_clauses.append(f"{key}=%s")
                 params.append(value)
 
         where_clause = " OR " if compare_with_or else " AND "
         where_clause = where_clause.join(where_clauses)
 
         try:
-            cursor = self.get_cursor()
+            cursor = self.cursor
             table_id = self.select_one_value_by_where(
                 schema_name=schema_name, view_table_name=view_table_name, select_clause_value=column_name,
                 where=where_clause, params=tuple(params), order_by=order_by)
             if table_id:
                 self.update_by_column_and_value(
                     schema_name=schema_name, table_name=table_name, column_name=column_name, column_value=table_id,
                     data_dict=data_dict, commit_changes=False)
@@ -237,15 +237,15 @@
         if duplicate_column_name.endswith("_UNIQUE"):
             duplicate_column_name = duplicate_column_name.split('_')[0]
 
         column_name = self.get_primary_key(schema_name=schema_name, table_name=table_name)
         if not column_name:
             raise error  # Column name for constraint not found
         select_query = f"SELECT {column_name} FROM `{schema_name}`.`{table_name}` WHERE {duplicate_column_name} = %s LIMIT 1;"
-        cursor = self.get_cursor()
+        cursor = self.cursor
         self.connection.commit()
         cursor.execute(select_query, (duplicate_value,))
         existing_duplicate_id = (cursor.fetchone() or [None])[0]
 
         self.logger.debug(object=locals())
         return existing_duplicate_id
 
@@ -308,15 +308,15 @@
 
         update_query = f"UPDATE `{schema_name}`.`{table_name}` " \
                        f"SET {set_values} updated_timestamp=CURRENT_TIMESTAMP() " \
                        f"WHERE {where} " + \
                        (f"ORDER BY {order_by} " if order_by else "") + \
                        f"LIMIT {limit};"
         params = params or tuple()
-        cursor = self.get_cursor()
+        cursor = self.cursor
         cursor.execute(update_query, tuple(data_dict.values()) + params)
         if commit_changes:
             self.connection.commit()
         last_row_id = cursor.lastrowid()
         return last_row_id
 
     def delete_by_id(self, *, schema_name: str = None, table_name: str = None,
@@ -353,15 +353,15 @@
         self._validate_args(args=locals())
         if not where:
             raise Exception("delete_by_where requires a 'where'")
 
         update_query = f"UPDATE `{schema_name}`.`{table_name}` " \
                        f"SET end_timestamp=CURRENT_TIMESTAMP() " \
                        f"WHERE {where};"
-        cursor = self.get_cursor()
+        cursor = self.cursor
         cursor.execute(update_query, params)
         self.connection.commit()
         affected_rows = cursor.get_row_count()
         return affected_rows
 
     # Main select function
     def select_multi_tuple_by_where(
@@ -388,15 +388,15 @@
             if where:
                 where += " AND end_timestamp IS NULL "  # not deleted
         select_query = f"SELECT {'DISTINCT' if distinct else ''} {select_clause_value} " \
                        f"FROM `{schema_name}`.`{view_table_name}` " + \
                        (f"WHERE {where} " if where else "") + \
                        (f"ORDER BY {order_by} " if order_by else "") + \
                        f"LIMIT {limit};"
-        cursor = self.get_cursor()
+        cursor = self.cursor
         self.connection.commit()  # https://bugs.mysql.com/bug.php?id=102053
         cursor.execute(select_query, params)
         result = cursor.fetchall()
 
         self.logger.debug(object=locals())
         return result
 
@@ -650,15 +650,15 @@
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         select_query = "SELECT column_name " \
                        "FROM information_schema.columns " \
                        "WHERE TABLE_SCHEMA = %s " \
                        "AND TABLE_NAME = %s;"
         params = (schema_name, table_name)
-        cursor = self.get_cursor()
+        cursor = self.cursor
         self.connection.commit()
         cursor.execute(select_query, params)
         result = cursor.fetchall()
 
         columns_tuple = tuple(x[0] for x in result)
         self.logger.debug(object=locals())
         return columns_tuple
@@ -670,15 +670,15 @@
         table_name = table_name or self.default_table_name
         query = """
         SELECT COLUMN_NAME
         FROM INFORMATION_SCHEMA.KEY_COLUMN_USAGE
         WHERE TABLE_SCHEMA = %s AND TABLE_NAME = %s AND CONSTRAINT_NAME = "PRIMARY"
         LIMIT 1;
         """
-        cursor = self.get_cursor()
+        cursor = self.cursor
         self.connection.commit()
         cursor.execute(query, (schema_name, table_name))
         column_name = (cursor.fetchone() or [None])[0]
         return column_name
 
     # helper functions:
     def convert_to_dict(self, row: tuple, select_clause_value: str = None) -> dict:
@@ -733,15 +733,15 @@
         identifier = NumberGenerator.get_random_identifier(
             schema_name="identifier", view_name="identifier_view", identifier_column_name="identifier")
         data_dict["identifier"] = identifier
         # We can't use self.insert, as it would cause an infinite loop
         insert_query = "INSERT " + \
                        "INTO `identifier`.`identifier_table` (identifier, entity_type_id) " \
                        "VALUES (%s, %s);"
-        cursor = self.get_cursor()
+        cursor = self.cursor
         cursor.execute(insert_query, (identifier, identifier_entity_type_id))
         self.connection.commit()
 
     # TODO: add warning logs
     def __add_create_updated_user_profile_ids(self, data_dict: dict, add_created_user_id: bool = False,
                                               schema_name: str = None, table_name: str = None) -> dict:
         """Adds created_user_id and updated_user_id to data_dict."""
@@ -858,21 +858,20 @@
     def close(self) -> None:
         """Closes the connection to the database (we usually do not have to call this)"""
         self.connection.close()
 
     def __del__(self):
         self.close()
 
-    def get_cursor(self, close_first: bool = False) -> Cursor:
+    @property
+    def cursor(self) -> Cursor:
         """Get a new cursor"""
-        if close_first and not self.cursor.is_closed():
-            self.cursor.close()
-        if self.cursor.is_closed():
-            self.cursor = self.connection.cursor()
-        return self.cursor
+        if self._cursor.is_closed():
+            self._cursor = self.connection.cursor()
+        return self._cursor
 
     # TODO: test this method
     def get_test_entity_id(self, *, entity_name: str, insert_function: callable, insert_kwargs: dict = None,
                            entity_creator: callable = None, create_kwargs: dict = None,
                            schema_name: str = None, view_name: str = None) -> int:
         """
         1. Check if there's an entity with is `is_test_data=True`.
```

### Comparing `database_mysql_local-0.0.313/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.314/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.313/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.314/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.313/database_mysql_local/src/point.py` & `database_mysql_local-0.0.314/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.313/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.314/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.313/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.314/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.313/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.314/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.313/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.314/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.313/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.314/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.313/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.314/database_mysql_local.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.313
+Version: 0.0.314
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.313/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.314/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.313/pyproject.toml` & `database_mysql_local-0.0.314/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.313/setup.py` & `database_mysql_local-0.0.314/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.313',
+    version='0.0.314',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

