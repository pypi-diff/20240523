# Comparing `tmp/database_mysql_local-0.0.318.tar.gz` & `tmp/database_mysql_local-0.0.319.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.318.tar", last modified: Thu May 23 05:38:31 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.319.tar", last modified: Thu May 23 05:48:08 2024, max compression
```

## Comparing `database_mysql_local-0.0.318.tar` & `database_mysql_local-0.0.319.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:38:31.623654 database_mysql_local-0.0.318/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 05:37:31.000000 database_mysql_local-0.0.318/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 05:38:31.623654 database_mysql_local-0.0.318/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-23 05:37:31.000000 database_mysql_local-0.0.318/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:38:31.615654 database_mysql_local-0.0.318/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:38:31.623654 database_mysql_local-0.0.318/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 05:37:31.000000 database_mysql_local-0.0.318/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-23 05:37:31.000000 database_mysql_local-0.0.318/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-23 05:37:31.000000 database_mysql_local-0.0.318/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-23 05:37:31.000000 database_mysql_local-0.0.318/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    54256 2024-05-23 05:37:59.000000 database_mysql_local-0.0.318/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30330 2024-05-23 05:37:31.000000 database_mysql_local-0.0.318/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-23 05:37:31.000000 database_mysql_local-0.0.318/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-23 05:37:31.000000 database_mysql_local-0.0.318/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-23 05:37:31.000000 database_mysql_local-0.0.318/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-23 05:37:31.000000 database_mysql_local-0.0.318/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   238517 2024-05-23 05:37:31.000000 database_mysql_local-0.0.318/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   630215 2024-05-23 05:37:55.000000 database_mysql_local-0.0.318/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-23 05:37:31.000000 database_mysql_local-0.0.318/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-23 05:37:31.000000 database_mysql_local-0.0.318/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:38:31.623654 database_mysql_local-0.0.318/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 05:38:31.000000 database_mysql_local-0.0.318/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-23 05:38:31.000000 database_mysql_local-0.0.318/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 05:38:31.000000 database_mysql_local-0.0.318/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-23 05:38:31.000000 database_mysql_local-0.0.318/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 05:38:31.000000 database_mysql_local-0.0.318/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-23 05:37:31.000000 database_mysql_local-0.0.318/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 05:38:31.623654 database_mysql_local-0.0.318/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 05:37:59.000000 database_mysql_local-0.0.318/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:48:08.431249 database_mysql_local-0.0.319/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 05:48:08.431249 database_mysql_local-0.0.319/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:48:08.427250 database_mysql_local-0.0.319/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:48:08.431249 database_mysql_local-0.0.319/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54266 2024-05-23 05:47:36.000000 database_mysql_local-0.0.319/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30330 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   238517 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   630215 2024-05-23 05:47:33.000000 database_mysql_local-0.0.319/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:48:08.431249 database_mysql_local-0.0.319/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 05:48:08.000000 database_mysql_local-0.0.319/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-23 05:48:08.000000 database_mysql_local-0.0.319/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 05:48:08.000000 database_mysql_local-0.0.319/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-23 05:48:08.000000 database_mysql_local-0.0.319/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 05:48:08.000000 database_mysql_local-0.0.319/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-23 05:47:11.000000 database_mysql_local-0.0.319/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 05:48:08.431249 database_mysql_local-0.0.319/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 05:47:36.000000 database_mysql_local-0.0.319/setup.py
```

### Comparing `database_mysql_local-0.0.318/PKG-INFO` & `database_mysql_local-0.0.319/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.318
+Version: 0.0.319
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.318/README.md` & `database_mysql_local-0.0.319/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.318/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.319/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.318/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.319/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.318/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.319/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.318/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.319/database_mysql_local/src/generic_crud.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,29 +358,29 @@
 
         self.cursor.execute(update_query, params)
         self.connection.commit()
         affected_rows = self.cursor.get_row_count()
         return affected_rows
 
     @lru_cache(maxsize=64)
-    def _replace_view_with_table(self, view_table_name: str) -> str:
+    @staticmethod
+    def _replace_view_with_table(view_table_name: str) -> str:
         # test data does not appear in the view, but we still wants to access it in tests.
         if not view_table_name:
             return view_table_name
         # Guess the table name from the view name:
         table_name = view_table_name.replace("_view", "_table")
         for table, values in table_definition.items():
             if values["view_name"] == view_table_name:
                 table_name = table  # got a better guess
                 break
         if table_name in table_columns and all(  # if all columns in the view present in the table.
-                col in table_columns[table_name] for col in table_columns.get(view_table_name, [])):
-            view_table_name = table_name
-            return view_table_name
-        return table_name
+                col in table_columns.get(table_name, []) for col in table_columns.get(view_table_name, [])):
+            return table_name
+        return view_table_name  # appropriate table not found
 
     # Main select function
     def select_multi_tuple_by_where(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             where: str = None, params: tuple = None, distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT,
             order_by: str = "") -> list:
         """Selects multiple rows from the table based on a WHERE clause and returns them as a list of tuples."""
```

### Comparing `database_mysql_local-0.0.318/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.319/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.318/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.319/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.318/database_mysql_local/src/point.py` & `database_mysql_local-0.0.319/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.318/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.319/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.318/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.319/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.318/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.319/database_mysql_local/src/table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.318/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.319/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.318/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.319/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.318/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.319/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.318/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.319/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.318
+Version: 0.0.319
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.318/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.319/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.318/pyproject.toml` & `database_mysql_local-0.0.319/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.318/setup.py` & `database_mysql_local-0.0.319/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.318',
+    version='0.0.319',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

