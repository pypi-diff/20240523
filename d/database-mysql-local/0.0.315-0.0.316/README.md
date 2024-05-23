# Comparing `tmp/database_mysql_local-0.0.315.tar.gz` & `tmp/database_mysql_local-0.0.316.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.315.tar", last modified: Thu May 23 02:42:26 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.316.tar", last modified: Thu May 23 03:20:53 2024, max compression
```

## Comparing `database_mysql_local-0.0.315.tar` & `database_mysql_local-0.0.316.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:42:26.320884 database_mysql_local-0.0.315/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 02:42:26.320884 database_mysql_local-0.0.315/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:42:26.312883 database_mysql_local-0.0.315/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:42:26.316884 database_mysql_local-0.0.315/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-05-23 02:41:52.000000 database_mysql_local-0.0.315/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    53563 2024-05-23 02:41:52.000000 database_mysql_local-0.0.315/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30330 2024-05-23 02:41:52.000000 database_mysql_local-0.0.315/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   630271 2024-05-23 02:41:52.000000 database_mysql_local-0.0.315/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:42:26.316884 database_mysql_local-0.0.315/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 02:42:26.000000 database_mysql_local-0.0.315/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-23 02:42:26.000000 database_mysql_local-0.0.315/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 02:42:26.000000 database_mysql_local-0.0.315/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-23 02:42:26.000000 database_mysql_local-0.0.315/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 02:42:26.000000 database_mysql_local-0.0.315/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-23 02:41:26.000000 database_mysql_local-0.0.315/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 02:42:26.320884 database_mysql_local-0.0.315/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 02:41:52.000000 database_mysql_local-0.0.315/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:53.192987 database_mysql_local-0.0.316/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 03:20:53.192987 database_mysql_local-0.0.316/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:53.184987 database_mysql_local-0.0.316/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:53.192987 database_mysql_local-0.0.316/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-23 03:20:22.000000 database_mysql_local-0.0.316/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-23 03:20:22.000000 database_mysql_local-0.0.316/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53518 2024-05-23 03:20:22.000000 database_mysql_local-0.0.316/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30330 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   630215 2024-05-23 03:20:19.000000 database_mysql_local-0.0.316/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:53.192987 database_mysql_local-0.0.316/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 03:20:53.000000 database_mysql_local-0.0.316/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-23 03:20:53.000000 database_mysql_local-0.0.316/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 03:20:53.000000 database_mysql_local-0.0.316/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-23 03:20:53.000000 database_mysql_local-0.0.316/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 03:20:53.000000 database_mysql_local-0.0.316/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-23 03:19:56.000000 database_mysql_local-0.0.316/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 03:20:53.192987 database_mysql_local-0.0.316/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 03:20:22.000000 database_mysql_local-0.0.316/setup.py
```

### Comparing `database_mysql_local-0.0.315/PKG-INFO` & `database_mysql_local-0.0.316/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.315
+Version: 0.0.316
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.315/README.md` & `database_mysql_local-0.0.316/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.315/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.316/database_mysql_local/src/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,17 +75,14 @@
         )
         self._cursor = self.cursor()
         self.set_schema(self.schema)
 
     def database_info(self):
         return f"host={self.host}, user={self.user}, schema={self.schema}"
 
-    def __del__(self):
-        self.close()
-
     def close(self) -> None:
         try:
             if self._cursor:
                 self._cursor.close()
                 logger.info(f"Cursor closed successfully for schema: {self.schema}")
         except Exception as exception:
             logger.error(f"connection.py close() {self.database_info()}", object={"exception": exception})
```

### Comparing `database_mysql_local-0.0.315/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.316/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.315/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.316/database_mysql_local/src/cursor.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,13 +88,15 @@
 
     def get_last_executed_statement(self) -> str:
         return self.cursor.statement
 
     def close(self) -> None:
         if self.__is_closed:
             self.logger.warning('Cursor is already closed')
-            return
-        self.cursor.close()
-        self.__is_closed = True
+        try:
+            self.cursor.close()
+            self.__is_closed = True
+        except Exception as exception:
+            self.logger.error('Unable to close cursor', object={"exception": exception})
 
     def is_closed(self) -> bool:
         return self.__is_closed
```

### Comparing `database_mysql_local-0.0.315/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.316/database_mysql_local/src/generic_crud.py`

 * *Files 0% similar despite different names*

```diff
@@ -866,17 +866,14 @@
     def close(self) -> None:
         """Closes the connection to the database (we usually do not have to call this)"""
         try:
             self.connection.close()
         except Exception as e:
             self.logger.error(f"Error while closing the connection: {e}")
 
-    def __del__(self):
-        self.close()
-
     @property
     def cursor(self) -> Cursor:
         """Get a new cursor"""
         if self._cursor.is_closed():
             self._cursor = self.connection.cursor()
         cursor = self._cursor
         return cursor
```

### Comparing `database_mysql_local-0.0.315/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.316/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.315/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.316/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.315/database_mysql_local/src/point.py` & `database_mysql_local-0.0.316/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.315/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.316/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.315/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.316/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.315/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.316/database_mysql_local/src/table_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# from our database.table_definition_table with some properties about each table
+# Generated by SQL2Code
+
 table_definition = {
     'phone_table': {
         'table_definition_id': 1,
         'entity_type_id1': 26,
         'entity_type_id2': None,
         'schema': 'phone',
         'view_name': None,
```

### Comparing `database_mysql_local-0.0.315/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.316/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.315/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.316/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.315/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.316/database_mysql_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.315
+Version: 0.0.316
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.315/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.316/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.315/pyproject.toml` & `database_mysql_local-0.0.316/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.315/setup.py` & `database_mysql_local-0.0.316/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.315',
+    version='0.0.316',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

