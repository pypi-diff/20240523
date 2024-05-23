# Comparing `tmp/database_mysql_local-0.0.314.tar.gz` & `tmp/database_mysql_local-0.0.315.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.314.tar", last modified: Wed May 22 16:35:00 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.315.tar", last modified: Thu May 23 02:42:26 2024, max compression
```

## Comparing `database_mysql_local-0.0.314.tar` & `database_mysql_local-0.0.315.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:35:00.132812 database_mysql_local-0.0.314/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-22 16:35:00.132812 database_mysql_local-0.0.314/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:35:00.124812 database_mysql_local-0.0.314/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:35:00.132812 database_mysql_local-0.0.314/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    53465 2024-05-22 16:34:28.000000 database_mysql_local-0.0.314/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30389 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   630271 2024-05-22 16:34:28.000000 database_mysql_local-0.0.314/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:35:00.132812 database_mysql_local-0.0.314/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-22 16:35:00.000000 database_mysql_local-0.0.314/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-22 16:35:00.000000 database_mysql_local-0.0.314/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:35:00.000000 database_mysql_local-0.0.314/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-22 16:35:00.000000 database_mysql_local-0.0.314/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 16:35:00.000000 database_mysql_local-0.0.314/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-22 16:34:01.000000 database_mysql_local-0.0.314/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:35:00.132812 database_mysql_local-0.0.314/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-22 16:34:28.000000 database_mysql_local-0.0.314/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:42:26.320884 database_mysql_local-0.0.315/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 02:42:26.320884 database_mysql_local-0.0.315/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:42:26.312883 database_mysql_local-0.0.315/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:42:26.316884 database_mysql_local-0.0.315/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-05-23 02:41:52.000000 database_mysql_local-0.0.315/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53563 2024-05-23 02:41:52.000000 database_mysql_local-0.0.315/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30330 2024-05-23 02:41:52.000000 database_mysql_local-0.0.315/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   630271 2024-05-23 02:41:52.000000 database_mysql_local-0.0.315/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:42:26.316884 database_mysql_local-0.0.315/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 02:42:26.000000 database_mysql_local-0.0.315/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-23 02:42:26.000000 database_mysql_local-0.0.315/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 02:42:26.000000 database_mysql_local-0.0.315/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-23 02:42:26.000000 database_mysql_local-0.0.315/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 02:42:26.000000 database_mysql_local-0.0.315/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 02:42:26.320884 database_mysql_local-0.0.315/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 02:41:52.000000 database_mysql_local-0.0.315/setup.py
```

### Comparing `database_mysql_local-0.0.314/PKG-INFO` & `database_mysql_local-0.0.315/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.314
+Version: 0.0.315
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.314/README.md` & `database_mysql_local-0.0.315/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.314/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.315/database_mysql_local/src/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,39 +75,42 @@
         )
         self._cursor = self.cursor()
         self.set_schema(self.schema)
 
     def database_info(self):
         return f"host={self.host}, user={self.user}, schema={self.schema}"
 
+    def __del__(self):
+        self.close()
+
     def close(self) -> None:
         try:
             if self._cursor:
                 self._cursor.close()
                 logger.info(f"Cursor closed successfully for schema: {self.schema}")
         except Exception as exception:
             logger.error(f"connection.py close() {self.database_info()}", object={"exception": exception})
-
+        connections_pool.pop(self.schema, None)
         if self.connection and self.connection.is_connected():
             self.connection.close()
-            connections_pool.pop(self.schema, None)
             logger.info("Connection closed successfully.")
 
     def cursor(self, *, close_previous: bool = True, cache_previous: bool = False, dictionary: bool = None, buffered: bool = None, raw: bool = None,
                prepared: bool = None, named_tuple: bool = None, cursor_class=None) -> Cursor:
-        if cache_previous and self._cursor:
-            cursor_instance = self._cursor
-            return cursor_instance
+        # if cache_previous and self._cursor:
+        #     cursor_instance = self._cursor
+        #     return cursor_instance
+        # if close_previous and self._cursor:
+        #     self._cursor.close()
 
         cursor_instance = Cursor(self.connection.cursor(
             dictionary=dictionary, buffered=buffered, raw=raw, prepared=prepared,
             named_tuple=named_tuple, cursor_class=cursor_class))
-        if close_previous and self._cursor:
-            self._cursor.close()
-        self._cursor = cursor_instance
+
+        # self._cursor = cursor_instance
         return cursor_instance
 
     def commit(self) -> None:
         self.connection.commit()
 
     def set_schema(self, new_schema: Optional[str]) -> None:
         if not new_schema:
```

### Comparing `database_mysql_local-0.0.314/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.315/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.314/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.315/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.314/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.315/database_mysql_local/src/generic_crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,19 +97,18 @@
 
         columns, values, data_dict = process_insert_data_dict(data_dict=data_dict)
         # We removed the IGNORE from the SQL Statement as we want to return the id of the existing row
         insert_query = "INSERT " + \
                        f"INTO `{schema_name}`.`{table_name}` ({columns}) " \
                        f"VALUES ({values});"
         try:
-            cursor = self.cursor
-            cursor.execute(insert_query, tuple(data_dict.values()))
+            self.cursor.execute(insert_query, tuple(data_dict.values()))
             if commit_changes:
                 self.connection.commit()
-            inserted_id = cursor.lastrowid()
+            inserted_id = self.cursor.lastrowid()
         except mysql.connector.errors.IntegrityError as exception:
             if ignore_duplicate:
                 self.logger.warning("GenericCRUD.insert: existing record found, selecting it's id."
                                     f"(table_name={table_name}, data_dict={data_dict})")
                 inserted_id = self._get_existing_duplicate_id(schema_name, table_name, exception)
             else:
                 raise exception
@@ -156,16 +155,15 @@
         columns = ", ".join(f"`{key}`" for key in data_dict)
         values = ", ".join(["%s"] * len(data_dict))
         sql_statement = f"""
         INSERT INTO `{schema_name}`.`{table_name}` ({columns})
         VALUES ({values});
         """
         sql_parameters = list(zip(*data_dict.values()))
-        cursor = self.cursor
-        cursor.executemany(sql_statement=sql_statement, sql_parameters=sql_parameters)
+        self.cursor.executemany(sql_statement=sql_statement, sql_parameters=sql_parameters)
         if commit_changes:
             self.connection.commit()
 
     def upsert(self, *, schema_name: str = None, table_name: str = None, view_table_name: str = None,
                data_dict: dict = None, data_json: dict = None,
                data_dict_compare: dict = None, data_json_compare: dict = None,
                order_by: str = None, compare_with_or: bool = False) -> Optional[int]:
@@ -180,15 +178,16 @@
         view_table_name = view_table_name or self.default_view_table_name
         column_name = generate_column_name(table_name)
         self._validate_args(args=locals())
         if not data_dict:
             self.logger.warning(log_message="GenericCRUD.upsert: data_dict is empty")
             return
         if not data_dict_compare:
-            return self.insert(schema_name=schema_name, table_name=table_name, data_dict=data_dict)
+            inserted_id = self.insert(schema_name=schema_name, table_name=table_name, data_dict=data_dict)
+            return inserted_id
 
         columns, values, processed_data_dict_compare = process_insert_data_dict(data_dict=data_dict_compare)
         where_clauses = []
         params = []
         for key, value in processed_data_dict_compare.items():
             if isinstance(value, list):
                 where_clauses.append(f"({' OR '.join([f'{key}=%s' for _ in value])})")
@@ -197,15 +196,14 @@
                 where_clauses.append(f"{key}=%s")
                 params.append(value)
 
         where_clause = " OR " if compare_with_or else " AND "
         where_clause = where_clause.join(where_clauses)
 
         try:
-            cursor = self.cursor
             table_id = self.select_one_value_by_where(
                 schema_name=schema_name, view_table_name=view_table_name, select_clause_value=column_name,
                 where=where_clause, params=tuple(params), order_by=order_by)
             if table_id:
                 self.update_by_column_and_value(
                     schema_name=schema_name, table_name=table_name, column_name=column_name, column_value=table_id,
                     data_dict=data_dict, commit_changes=False)
@@ -237,33 +235,32 @@
         if duplicate_column_name.endswith("_UNIQUE"):
             duplicate_column_name = duplicate_column_name.split('_')[0]
 
         column_name = self.get_primary_key(schema_name=schema_name, table_name=table_name)
         if not column_name:
             raise error  # Column name for constraint not found
         select_query = f"SELECT {column_name} FROM `{schema_name}`.`{table_name}` WHERE {duplicate_column_name} = %s LIMIT 1;"
-        cursor = self.cursor
         self.connection.commit()
-        cursor.execute(select_query, (duplicate_value,))
-        existing_duplicate_id = (cursor.fetchone() or [None])[0]
+        self.cursor.execute(select_query, (duplicate_value,))
+        existing_duplicate_id = (self.cursor.fetchone() or [None])[0]
 
         self.logger.debug(object=locals())
         return existing_duplicate_id
 
     def update_by_id(
             self, *, schema_name: str = None, table_name: str = None, column_name: str = None, column_value: Any = None,
             id_column_name: str = None, id_column_value: Any = None, data_dict: dict = None, data_json: dict = None,
             limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None, commit_changes: bool = True) -> int or None:
         if datetime.now() > datetime(2024, 5, 25):
             self.logger.warning("GenericCRUD.update_by_id is deprecated, use update_by_column_and_value instead.")
-        return self.update_by_column_and_value(schema_name=schema_name, table_name=table_name,
-                                               column_name=column_name, column_value=column_value,
-                                               id_column_name=id_column_name, id_column_value=id_column_value,
-                                               data_dict=data_dict, data_json=data_json,
-                                               limit=limit, order_by=order_by, commit_changes=commit_changes)
+        updated_id = self.update_by_column_and_value(
+            schema_name=schema_name, table_name=table_name, column_name=column_name, column_value=column_value,
+            id_column_name=id_column_name, id_column_value=id_column_value, data_dict=data_dict, data_json=data_json,
+            limit=limit, order_by=order_by, commit_changes=commit_changes)
+        return updated_id
 
     def update_by_column_and_value(
             self, *, schema_name: str = None, table_name: str = None, column_name: str = None, column_value: Any = None,
             id_column_name: str = None, id_column_value: Any = None, data_dict: dict = None, data_json: dict = None,
             limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None, commit_changes: bool = True) -> int or None:
         """Updates data in the table by ID."""
         column_name = self._deprecated_id_column(id_column_name, column_name)
@@ -308,19 +305,19 @@
 
         update_query = f"UPDATE `{schema_name}`.`{table_name}` " \
                        f"SET {set_values} updated_timestamp=CURRENT_TIMESTAMP() " \
                        f"WHERE {where} " + \
                        (f"ORDER BY {order_by} " if order_by else "") + \
                        f"LIMIT {limit};"
         params = params or tuple()
-        cursor = self.cursor
-        cursor.execute(update_query, tuple(data_dict.values()) + params)
+
+        self.cursor.execute(update_query, tuple(data_dict.values()) + params)
         if commit_changes:
             self.connection.commit()
-        last_row_id = cursor.lastrowid()
+        last_row_id = self.cursor.lastrowid()
         return last_row_id
 
     def delete_by_id(self, *, schema_name: str = None, table_name: str = None,
                      column_name: str = None, column_value: Any = None,
                      id_column_name: str = None, id_column_value: Any = None) -> int:
         if datetime.now() > datetime(2024, 5, 25):
             self.logger.warning("GenericCRUD.delete_by_id is deprecated, use delete_by_column_and_value instead.")
@@ -353,18 +350,18 @@
         self._validate_args(args=locals())
         if not where:
             raise Exception("delete_by_where requires a 'where'")
 
         update_query = f"UPDATE `{schema_name}`.`{table_name}` " \
                        f"SET end_timestamp=CURRENT_TIMESTAMP() " \
                        f"WHERE {where};"
-        cursor = self.cursor
-        cursor.execute(update_query, params)
+
+        self.cursor.execute(update_query, params)
         self.connection.commit()
-        affected_rows = cursor.get_row_count()
+        affected_rows = self.cursor.get_row_count()
         return affected_rows
 
     # Main select function
     def select_multi_tuple_by_where(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             where: str = None, params: tuple = None, distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT,
             order_by: str = "") -> list:
@@ -375,58 +372,60 @@
         select_clause_value = select_clause_value or self.default_select_clause_value
         where = where or self.default_where
         where = self.__where_security(where=where, view_name=view_table_name)
         self._validate_args(args=locals())
 
         # TODO: add ` to column names if they are not reserved words (like COUNT, ST_X(point), etc.)
         # select_clause_value = ",".join([f"`{x.strip()}`" for x in select_clause_value.split(",") if x != "*"])
-        # TODO: If is_test_data exists in the table and is_test_data=False, add `AND is_test_data=0` to avoid users getting test data
-        #   (but the tests should be allowed to access real data)
+        # TODO: allow other tables too
         if (self.is_test_data and (view_table_name or "").replace("_view", "") ==
                 (self.default_table_name or "").replace("_table", "")):
             # test data does not appear in the view, but we still wants to access it in tests (partial solution).
             view_table_name = self.default_table_name
             if where:
                 where += " AND end_timestamp IS NULL "  # not deleted
         select_query = f"SELECT {'DISTINCT' if distinct else ''} {select_clause_value} " \
                        f"FROM `{schema_name}`.`{view_table_name}` " + \
                        (f"WHERE {where} " if where else "") + \
                        (f"ORDER BY {order_by} " if order_by else "") + \
                        f"LIMIT {limit};"
-        cursor = self.cursor
+
         self.connection.commit()  # https://bugs.mysql.com/bug.php?id=102053
-        cursor.execute(select_query, params)
-        result = cursor.fetchall()
+        self.cursor.execute(select_query, params)
+        result = self.cursor.fetchall()
 
         self.logger.debug(object=locals())
         return result
 
     def select_multi_dict_by_where(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             where: str = None, params: tuple = None, distinct: bool = False,
             limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
         """Selects multiple rows from the table based on a WHERE clause and returns them as a list of dictionaries."""
         result = self.select_multi_tuple_by_where(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
-        return self.convert_multi_to_dict(result, select_clause_value)
+        result_as_dicts = self.convert_multi_to_dict(result, select_clause_value)
+        return result_as_dicts
+
 
     # TODO: test distinct
     def select_one_tuple_by_id(self, *, schema_name: str = None, view_table_name: str = None,
                                select_clause_value: str = None,
                                column_name: str = None, column_value: Any = None,
                                id_column_name: str = None, id_column_value: Any = None,
                                distinct: bool = False, order_by: str = "") -> tuple:
         if datetime.now() > datetime(2024, 5, 25):
             self.logger.warning(
                 "GenericCRUD.select_one_tuple_by_id is deprecated, use select_one_tuple_by_column_and_value instead.")
-        return self.select_one_tuple_by_column_and_value(
+        result = self.select_one_tuple_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, order_by=order_by)
+        return result
 
     def select_one_tuple_by_column_and_value(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, order_by: str = "") -> tuple:
         """Selects one row from the table by ID and returns it as a tuple."""
         column_name = column_name or id_column_name
@@ -442,42 +441,45 @@
     def select_one_dict_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, order_by: str = "") -> dict:
         if datetime.now() > datetime(2024, 5, 25):
             self.logger.warning(
                 "GenericCRUD.select_one_dict_by_id is deprecated, use select_one_dict_by_column_and_value instead.")
-        return self.select_one_dict_by_column_and_value(
+        result = self.select_one_dict_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, order_by=order_by)
+        return result
 
     def select_one_dict_by_column_and_value(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, order_by: str = "") -> dict:
         """Selects one row from the table by ID and returns it as a dictionary (column_name: value)"""
         column_name = column_name or id_column_name
         column_value = column_value or id_column_value
         result = self.select_one_tuple_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, distinct=distinct, order_by=order_by)
-        return self.convert_to_dict(row=result, select_clause_value=select_clause_value)
+        result = self.convert_to_dict(row=result, select_clause_value=select_clause_value)
+        return result
 
     def select_one_value_by_id(
             self, *, select_clause_value: str, schema_name: str = None, view_table_name: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, order_by: str = "", skip_null_values: bool = True) -> Any:
         if datetime.now() > datetime(2024, 5, 25):
             self.logger.warning(
                 "GenericCRUD.select_one_value_by_id is deprecated, use select_one_value_by_column_and_value instead.")
-        return self.select_one_value_by_column_and_value(
+        result = self.select_one_value_by_column_and_value(
             select_clause_value=select_clause_value, schema_name=schema_name, view_table_name=view_table_name,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, order_by=order_by, skip_null_values=skip_null_values)
+        return result
 
     def select_one_value_by_column_and_value(
             self, *, select_clause_value: str, schema_name: str = None, view_table_name: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, order_by: str = "", skip_null_values: bool = True) -> Any:
         """Selects one value from the table by ID and returns it."""
         column_name = self._deprecated_id_column(id_column_name, column_name)
@@ -508,15 +510,16 @@
     def select_one_dict_by_where(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             where: str = None, params: tuple = None, distinct: bool = False, order_by: str = "") -> dict:
         """Selects one row from the table based on a WHERE clause and returns it as a dictionary."""
         result = self.select_one_tuple_by_where(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, order_by=order_by)
-        return self.convert_to_dict(row=result, select_clause_value=select_clause_value)
+        result = self.convert_to_dict(row=result, select_clause_value=select_clause_value)
+        return result
 
     def select_one_value_by_where(
             self, *, select_clause_value: str, schema_name: str = None, view_table_name: str = None,
             where: str = None, params: tuple = None, distinct: bool = False, order_by: str = "",
             skip_null_values: bool = True) -> Any:
         """Selects one value from the table based on a WHERE clause and returns it."""
         select_clause_value = select_clause_value or self.default_select_clause_value
@@ -532,19 +535,20 @@
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = "",
             skip_null_values: bool = True) -> list:
         if datetime.now() > datetime(2024, 5, 25):
             self.logger.warning(
                 "GenericCRUD.select_multi_value_by_id is deprecated, use select_multi_value_by_column_and_value instead.")
-        return self.select_multi_value_by_column_and_value(
+        result = self.select_multi_value_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, limit=limit, order_by=order_by,
             skip_null_values=skip_null_values)
+        return result
 
     def select_multi_value_by_column_and_value(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = "",
             skip_null_values: bool = True) -> list:
         """Selects multiple values from the table by ID and returns them as a list."""
@@ -575,18 +579,19 @@
     def select_multi_tuple_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
         if datetime.now() > datetime(2024, 5, 25):
             self.logger.warning(
                 "GenericCRUD.select_multi_tuple_by_id is deprecated, use select_multi_tuple_by_column_and_value instead.")
-        return self.select_multi_tuple_by_column_and_value(
+        result = self.select_multi_tuple_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, limit=limit, order_by=order_by)
+        return result
 
     def select_multi_tuple_by_column_and_value(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
         """Selects multiple rows from the table by ID and returns them as a
         list of tuples.
@@ -601,41 +606,44 @@
         else:
             if column_value is None:
                 where = f"`{column_name}` IS NULL"
                 params = None
             else:
                 where = f"`{column_name}`=%s"
                 params = (column_value,)
-        return self.select_multi_tuple_by_where(
+        result = self.select_multi_tuple_by_where(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
+        return result
 
     def select_multi_dict_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
         if datetime.now() > datetime(2024, 5, 25):
             self.logger.warning(
                 "GenericCRUD.select_multi_dict_by_id is deprecated, use select_multi_dict_by_column_and_value instead.")
-        return self.select_multi_dict_by_column_and_value(
+        result = self.select_multi_dict_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, limit=limit, order_by=order_by)
+        return result
 
     def select_multi_dict_by_column_and_value(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
         """Selects multiple rows from the table by ID and returns them as a list of dictionaries."""
         column_name = column_name or id_column_name
         column_value = column_value or id_column_value
         result = self.select_multi_tuple_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, distinct=distinct, limit=limit, order_by=order_by)
-        return self.convert_multi_to_dict(result, select_clause_value)
+        result = self.convert_multi_to_dict(result, select_clause_value)
+        return result
 
     def is_column_in_table(self, column_name: str, schema_name: str = None, table_name: str = None) -> bool:
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         if not column_name:
             raise Exception("is_column_in_table requires a column_name")
         table_columns = self.get_table_columns(schema_name=schema_name, table_name=table_name)
@@ -650,18 +658,18 @@
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         select_query = "SELECT column_name " \
                        "FROM information_schema.columns " \
                        "WHERE TABLE_SCHEMA = %s " \
                        "AND TABLE_NAME = %s;"
         params = (schema_name, table_name)
-        cursor = self.cursor
+
         self.connection.commit()
-        cursor.execute(select_query, params)
-        result = cursor.fetchall()
+        self.cursor.execute(select_query, params)
+        result = self.cursor.fetchall()
 
         columns_tuple = tuple(x[0] for x in result)
         self.logger.debug(object=locals())
         return columns_tuple
 
 
     @lru_cache
@@ -670,18 +678,18 @@
         table_name = table_name or self.default_table_name
         query = """
         SELECT COLUMN_NAME
         FROM INFORMATION_SCHEMA.KEY_COLUMN_USAGE
         WHERE TABLE_SCHEMA = %s AND TABLE_NAME = %s AND CONSTRAINT_NAME = "PRIMARY"
         LIMIT 1;
         """
-        cursor = self.cursor
+
         self.connection.commit()
-        cursor.execute(query, (schema_name, table_name))
-        column_name = (cursor.fetchone() or [None])[0]
+        self.cursor.execute(query, (schema_name, table_name))
+        column_name = (self.cursor.fetchone() or [None])[0]
         return column_name
 
     # helper functions:
     def convert_to_dict(self, row: tuple, select_clause_value: str = None) -> dict:
         """Returns a dictionary of the column names and their values."""
         select_clause_value = select_clause_value or self.default_select_clause_value
         if select_clause_value == "*":
@@ -733,16 +741,16 @@
         identifier = NumberGenerator.get_random_identifier(
             schema_name="identifier", view_name="identifier_view", identifier_column_name="identifier")
         data_dict["identifier"] = identifier
         # We can't use self.insert, as it would cause an infinite loop
         insert_query = "INSERT " + \
                        "INTO `identifier`.`identifier_table` (identifier, entity_type_id) " \
                        "VALUES (%s, %s);"
-        cursor = self.cursor
-        cursor.execute(insert_query, (identifier, identifier_entity_type_id))
+
+        self.cursor.execute(insert_query, (identifier, identifier_entity_type_id))
         self.connection.commit()
 
     # TODO: add warning logs
     def __add_create_updated_user_profile_ids(self, data_dict: dict, add_created_user_id: bool = False,
                                               schema_name: str = None, table_name: str = None) -> dict:
         """Adds created_user_id and updated_user_id to data_dict."""
         # if get_environment_name() not in (EnvironmentName.DVLP1.value, EnvironmentName.PROD1.value):
@@ -853,25 +861,34 @@
         In most cases you do not have to call this directly - you can pass schema_name to most functions"""
         if schema_name and self.default_schema_name != schema_name:
             self.connection.set_schema(schema_name)
             self.default_schema_name = schema_name
 
     def close(self) -> None:
         """Closes the connection to the database (we usually do not have to call this)"""
-        self.connection.close()
+        try:
+            self.connection.close()
+        except Exception as e:
+            self.logger.error(f"Error while closing the connection: {e}")
 
     def __del__(self):
         self.close()
 
     @property
     def cursor(self) -> Cursor:
         """Get a new cursor"""
         if self._cursor.is_closed():
             self._cursor = self.connection.cursor()
-        return self._cursor
+        cursor = self._cursor
+        return cursor
+
+    @cursor.setter
+    def cursor(self, value: Cursor) -> None:
+        """Set the cursor"""
+        self._cursor = value
 
     # TODO: test this method
     def get_test_entity_id(self, *, entity_name: str, insert_function: callable, insert_kwargs: dict = None,
                            entity_creator: callable = None, create_kwargs: dict = None,
                            schema_name: str = None, view_name: str = None) -> int:
         """
         1. Check if there's an entity with is `is_test_data=True`.
```

### Comparing `database_mysql_local-0.0.314/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.315/database_mysql_local/src/generic_crud_ml.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,20 @@
 # TODO If I understand, there are two things:
 # is_main in data_ml_dict
 # table_definition_table.is_main_column
 # I'm not sure we need additional parameter.
 class GenericCRUDML(GenericCRUD, metaclass=MetaLogger, object=LOGGER_CRUD_ML_CODE_OBJECT):
     """A class that provides generic CRUD functionality for tables with multi-language support."""
 
+    # TODO: allow overiding all default values in all methods
     def __init__(self, default_schema_name: str,
                  default_table_name: str = None, default_view_table_name: str = None,
                  default_ml_table_name: str = None, default_ml_view_table_name: str = None,
-                 default_column_name: str = None,
-                 default_id_column_name: str = None,
-                 is_main_column_name: str = IS_MAIN_COLUMN_NAME,
-                 is_test_data: bool = False) -> None:
+                 default_column_name: str = None, default_id_column_name: str = None,
+                 is_main_column_name: str = IS_MAIN_COLUMN_NAME, is_test_data: bool = False) -> None:
         """Initializes the GenericCRUDML class. If connection is not provided,
         a new connection will be created."""
         self.default_table_name = default_table_name or default_ml_table_name.replace("_ml", "")
         self.default_ml_table_name = default_ml_table_name or self.generate_ml_table_name(default_table_name)
         self.default_ml_view_table_name = default_ml_view_table_name or generate_view_name(self.default_ml_table_name)
         self.logger.info("GenericCRUDML.__init__", object={
             "default_ml_table_name": self.default_ml_table_name,
@@ -71,15 +70,17 @@
         data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
         lang_code_str = self._get_lang_code_str(lang_code=lang_code, data_ml_dict=data_ml_dict)
         table_name = table_name or self.default_table_name
         column_name = column_name or self.default_column_name
         ml_view_name = generate_view_name(ml_table_name) if ml_table_name else self.default_ml_view_table_name
         ml_table_name = ml_table_name or self.default_ml_table_name
 
+        old_cursor = self.cursor
         try:
+            self.cursor = self.connection.cursor()
             # if this is the first insert of this data, is_main should be True
             if is_main is not None:
                 if table_id is None:
                     is_main = True
                 elif is_main:
                     self._update_old_main_value_to_false(
                         schema_name=schema_name, table_name=table_name, table_id=table_id)
@@ -114,22 +115,24 @@
             ml_table_id = self.insert(schema_name=schema_name, data_dict=data_ml_dict, table_name=ml_table_name,
                                       ignore_duplicate=True, commit_changes=False)
 
             self.connection.commit()
         except Exception as e:
             self.connection.rollback()
             raise e
+        finally:
+            self.cursor.close()
+            self.cursor = old_cursor
         return table_id, ml_table_id
 
-    def add_value_if_not_exist(self, *, data_dict: dict = None, data_ml_dict: dict = None,
-                               data_json: dict = None, data_ml_json: dict = None,
-                               table_id: int = None, lang_code: LangCode = None,
-                               is_main: bool = False, table_name: str = None,
-                               ml_table_name: str = None, schema_name: str = None,
-                               order_by: str = None) -> tuple:
+    def add_value_if_not_exist(
+            self, *, data_dict: dict = None, data_ml_dict: dict = None, data_json: dict = None,
+            data_ml_json: dict = None, table_id: int = None, lang_code: LangCode = None,
+            is_main: bool = False, table_name: str = None, ml_table_name: str = None, schema_name: str = None,
+            order_by: str = None) -> (int, int):
         # TODO: after we delete data_ml_json parameter, make data_ml_dict without default value and we can delete the following raise
         if not data_ml_dict and not data_ml_json:
             raise ValueError("data_ml_dict or data_ml_json is required for add_value_if_not_exist")
         data_dict = data_json or self._data_json_to_dict(data_dict)
         data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
@@ -137,34 +140,31 @@
         column_name = generate_column_name(table_name)
         ml_column_name = generate_column_name(ml_table_name)
 
         # check if the row exists in the ml_table
         name = data_ml_dict.get("title") or data_ml_dict.get("name")
         if not name:
             raise ValueError("name or title is required for upsert_value")
-        table_id = table_id or self.get_id_by_name(schema_name=schema_name, table_name=table_name,
-                                                   ml_table_name=ml_table_name, name=name,
-                                                   lang_code=lang_code, column_name=column_name, order_by=order_by)
-        ml_table_id = self.get_ml_id_by_name(schema_name=schema_name, ml_table_name=ml_table_name, name=name,
-                                             lang_code=lang_code,
-                                             column_name=ml_column_name, order_by=order_by)
+        table_id = table_id or self.get_id_by_name(
+            schema_name=schema_name, table_name=table_name, ml_table_name=ml_table_name, name=name,
+            lang_code=lang_code, column_name=column_name, order_by=order_by)
+        ml_table_id = self.get_ml_id_by_name(
+            schema_name=schema_name, ml_table_name=ml_table_name, name=name, lang_code=lang_code,
+            column_name=ml_column_name, order_by=order_by)
         if not table_id:
-            return self.add_value(schema_name=schema_name, data_ml_dict=data_ml_dict, table_id=table_id,
-                                  lang_code=lang_code, is_main=is_main,
-                                  data_dict=data_dict, table_name=table_name, ml_table_name=ml_table_name)
-        else:
-            return table_id, ml_table_id
+            table_id, ml_table_id = self.add_value(
+                schema_name=schema_name, data_ml_dict=data_ml_dict, table_id=table_id, lang_code=lang_code,
+                is_main=is_main, data_dict=data_dict, table_name=table_name, ml_table_name=ml_table_name)
+        return table_id, ml_table_id
 
-    def update_value_by_id(self, *, data_dict: dict = None, data_ml_dict: dict = None,
-                           data_json: dict = None, data_ml_json: dict = None,
-                           ml_table_id: int, table_id: int,
-                           lang_code: LangCode = None, is_main: bool = False,
-                           table_name: str = None, ml_table_name: str = None,
-                           schema_name: str = None, limit: int = DEFAULT_SQL_SELECT_LIMIT,
-                           order_by: str = None) -> tuple:
+    def update_value_by_id(
+            self, *, data_dict: dict = None, data_ml_dict: dict = None, data_json: dict = None,
+            data_ml_json: dict = None, ml_table_id: int, table_id: int, lang_code: LangCode = None,
+            is_main: bool = False, table_name: str = None, ml_table_name: str = None, schema_name: str = None,
+            limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> (int, int):
         # TODO: after we delete data_ml_json parameter, make data_ml_dict without default value and we can delete the following raise
         if not data_ml_dict and not data_ml_json:
             raise ValueError("data_ml_dict or data_ml_json is required for update_value")
         data_dict = data_json or self._data_json_to_dict(data_dict)
         data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
         schema_name = schema_name or self.default_schema_name
         lang_code_str = self._get_lang_code_str(lang_code=lang_code, data_ml_dict=data_ml_dict)
@@ -172,15 +172,17 @@
         ml_table_name = ml_table_name or self.default_ml_table_name
         column_name = generate_column_name(table_name)
 
         if table_id is None:
             raise ValueError("table_id is required for update_value")
         if ml_table_id is None:
             raise ValueError("ml_table_id is required for update_value")
+        old_cursor = self.cursor
         try:
+            self.cursor = self.connection.cursor()
             if is_main is not None:
                 if is_main:
                     self._update_old_main_value_to_false(schema_name=schema_name, table_name=table_name,
                                                          table_id=table_id)
                 if data_dict:
                     self.update_by_id(schema_name=schema_name, table_name=table_name, column_name=column_name,
                                       column_value=table_id, data_dict=data_dict, limit=limit, order_by=order_by,
@@ -195,24 +197,25 @@
                               column_name=column_name, column_value=ml_table_id, limit=limit, order_by=order_by,
                               commit_changes=False)
 
             self.connection.commit()
         except Exception as e:
             self.connection.rollback()
             raise e
+        finally:
+            self.cursor.close()
+            self.cursor = old_cursor
         return table_id, ml_table_id
 
-    def upsert_value(self, *, data_dict: dict = None, data_ml_dict: dict = None,
-                     data_json: dict = None, data_ml_json: dict = None,
-                     data_json_compare: dict = None, data_dict_compare: dict = None,
-                     table_id: int = None, lang_code: LangCode = None,
-                     is_main: bool = False, table_name: str = None,
-                     ml_table_name: str = None, schema_name: str = None,
-                     compare_view_name: str = None,
-                     limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> tuple:
+    def upsert_value(
+            self, *, data_dict: dict = None, data_ml_dict: dict = None, data_json: dict = None,
+            data_ml_json: dict = None, data_json_compare: dict = None, data_dict_compare: dict = None,
+            table_id: int = None, lang_code: LangCode = None, is_main: bool = False, table_name: str = None,
+            ml_table_name: str = None, schema_name: str = None, compare_view_name: str = None,
+            limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> (int, int):
         # TODO: after we delete data_ml_json parameter, make data_ml_dict without default value and we can delete the following raise
         if not data_ml_dict and not data_ml_json:
             raise ValueError("data_ml_dict or data_ml_json is required for upsert_value")
         compare_view_name = compare_view_name or self.default_ml_view_table_name
         data_dict = data_json or self._data_json_to_dict(data_dict)
         data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
         data_dict_compare = data_json_compare or self._data_json_to_dict(data_dict_compare)
@@ -234,29 +237,29 @@
             schema_name=schema_name, table_name=table_name, ml_table_name=ml_table_name,
             name=name_compare, lang_code=lang_code, compare_view_name=compare_view_name,
             column_name=column_name, order_by=order_by)
         ml_table_id = self.get_ml_id_by_name(
             schema_name=schema_name, ml_table_name=ml_table_name, name=name_compare, lang_code=lang_code,
             compare_view_name=compare_view_name, column_name=ml_column_name, order_by=order_by)
         if not table_id:
-            return self.add_value(schema_name=schema_name, data_ml_dict=data_ml_dict, table_id=table_id,
-                                  lang_code=lang_code, is_main=is_main,
-                                  data_dict=data_dict, table_name=table_name, ml_table_name=ml_table_name)
+            table_id, ml_table_id = self.add_value(
+                schema_name=schema_name, data_ml_dict=data_ml_dict, table_id=table_id, lang_code=lang_code,
+                is_main=is_main, data_dict=data_dict, table_name=table_name, ml_table_name=ml_table_name)
         else:
-            return self.update_value_by_id(schema_name=schema_name, data_ml_dict=data_ml_dict, ml_table_id=ml_table_id,
-                                           table_id=table_id,
-                                           lang_code=lang_code, is_main=is_main, data_dict=data_dict,
-                                           table_name=table_name, ml_table_name=ml_table_name, limit=limit,
-                                           order_by=order_by)
+            table_id, ml_table_id = self.update_value_by_id(
+                schema_name=schema_name, data_ml_dict=data_ml_dict, ml_table_id=ml_table_id, table_id=table_id,
+                lang_code=lang_code, is_main=is_main, data_dict=data_dict, table_name=table_name,
+                ml_table_name=ml_table_name, limit=limit, order_by=order_by)
+        return table_id, ml_table_id
 
     def upsert_value_with_abbreviations(
             self, *, data_dict: dict = None, data_ml_dict: dict, data_json: dict = None, data_ml_json: dict = None,
-            data_json_compare: dict = None, data_dict_compare: dict = None, table_id: int = None, lang_code: LangCode = None,
-            table_name: str = None, ml_table_name: str = None, schema_name: str = None,
-            compare_view_name: str = None, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> tuple:
+            data_json_compare: dict = None, data_dict_compare: dict = None, table_id: int = None, order_by: str = None,
+            table_name: str = None, ml_table_name: str = None, schema_name: str = None, lang_code: LangCode = None,
+            compare_view_name: str = None, limit: int = DEFAULT_SQL_SELECT_LIMIT) -> (int, list[int]):
         # TODO: after we delete data_ml_json parameter, make data_ml_dict without default value and we can delete the following raise
         if not data_ml_dict and not data_ml_json:
             raise ValueError("data_ml_dict or data_ml_json is required for upsert_value")
         compare_view_name = compare_view_name or self.default_ml_view_table_name
         data_dict = data_json or self._data_json_to_dict(data_dict)
         data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
         data_dict_compare = data_json_compare or self._data_json_to_dict(data_dict_compare)
@@ -331,15 +334,15 @@
                         ml_table_name=ml_table_name)
                 ml_ids_list.append(ml_table_id)
             ml_ids_list.append(main_ml_table_id)
         return table_id, ml_ids_list
 
     def get_values_tuple(self, *, table_id: int, schema_name: str = None, ml_view_table_name: str = None,
                          lang_code: LangCode = None, column_name: str = None, id_column_name: str = None,
-                         select_clause_value: str = "*", order_by: str = None) -> tuple:
+                         select_clause_value: str = "*", order_by: str = None) -> (int, int):
         column_name = self._deprecated_id_column(id_column_name, column_name)
         lang_code_str = self._get_lang_code_str(lang_code=lang_code)
         ml_view_table_name = ml_view_table_name or self.default_ml_view_table_name
         column_name = column_name or self.default_column_name
         schema_name = schema_name or self.default_schema_name
         result = self.select_one_tuple_by_where(
             schema_name=schema_name, view_table_name=ml_view_table_name,
@@ -372,15 +375,16 @@
         result = self.select_multi_dict_by_where(
             schema_name=schema_name, view_table_name=self.default_ml_view_table_name,
             where=f"{column_name}=%s AND lang_code=%s", params=(table_id, lang_code_str),
             order_by=order_by)
         return result
 
     def get_main_values_tuple(self, *, table_id: int, column_name: str = None, id_column_name: str = None,
-                              select_clause_value: str = "*", order_by: str = None, schema_name: str = None) -> tuple:
+                              select_clause_value: str = "*", order_by: str = None, schema_name: str = None) -> (
+    int, int):
         schema_name = schema_name or self.default_schema_name
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_name = column_name or generate_column_name(
             self.default_table_name)
         result = self.select_one_tuple_by_where(
             schema_name=schema_name, view_table_name=self.default_ml_view_table_name,
             where=f"{column_name}=%s AND is_main=True", params=(table_id,),
@@ -452,36 +456,38 @@
         compare_view_name = compare_view_name or generate_view_name(ml_table_name)
         result = self.select_multi_value_by_where(
             schema_name=schema_name, view_table_name=compare_view_name,
             select_clause_value=ml_column_name, order_by=order_by,
             where=f"{column_name}=%s AND lang_code=%s", params=(table_id, lang_code_str))
         return result
 
-    def delete_by_name(self, *, name: str, lang_code: LangCode = None) -> None:
+    def delete_by_name(self, *, name: str, lang_code: LangCode = None) -> int:
         lang_code_str = self._get_lang_code_str(lang_code=lang_code, name=name)
         if GenericCRUD.is_column_in_table(self, table_name=self.default_ml_view_table_name, column_name="title"):
             where = "title=%s AND lang_code=%s"
         else:
             where = "`name`=%s AND lang_code=%s"
-        self.delete_by_where(table_name=self.default_ml_table_name, where=where,
-                             params=(name, lang_code_str))
+        deleted_id = self.delete_by_where(table_name=self.default_ml_table_name, where=where,
+                                          params=(name, lang_code_str))
+        return deleted_id
 
     @staticmethod
     def generate_ml_table_name(table_name: str) -> str:
         if table_name:
             ml_table_name = re.sub(r'(_table)$', '_ml_table', table_name)
             return ml_table_name
 
     # Change the old row with is_main=True to is_main=False
-    def _update_old_main_value_to_false(self, *, schema_name: str, table_id: int, table_name: str) -> None:
+    def _update_old_main_value_to_false(self, *, schema_name: str, table_id: int, table_name: str) -> int:
         data_ml_dict = {self.is_main_column_name: False}
         column_name = generate_column_name(table_name)
         where = f"{column_name}=%s AND {self.is_main_column_name} = True"
-        self.update_by_where(schema_name=schema_name, table_name=self.default_ml_table_name,
-                             data_dict=data_ml_dict, where=where, params=(table_id,))
+        updated_id = self.update_by_where(schema_name=schema_name, table_name=self.default_ml_table_name,
+                                          data_dict=data_ml_dict, where=where, params=(table_id,))
+        return updated_id
 
     def _get_lang_code_str(self, *, name: str = None, lang_code: LangCode = None,
                            data_ml_dict: dict = None, data_ml_json: dict = None) -> str:
         data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
         if lang_code is None and name is not None:
             lang_code_str = LangCode.detect_lang_code_str(name)
         elif lang_code is None and data_ml_dict is not None:
```

### Comparing `database_mysql_local-0.0.314/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.315/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.314/database_mysql_local/src/point.py` & `database_mysql_local-0.0.315/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.314/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.315/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.314/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.315/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.314/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.315/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.314/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.315/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.314/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.315/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.314/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.315/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.314
+Version: 0.0.315
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.314/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.315/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.314/pyproject.toml` & `database_mysql_local-0.0.315/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.314/setup.py` & `database_mysql_local-0.0.315/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.314',
+    version='0.0.315',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

