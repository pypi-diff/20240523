# Comparing `tmp/lancedb_tables-0.1.1.tar.gz` & `tmp/lancedb_tables-0.1.2.tar.gz`

## Comparing `lancedb_tables-0.1.1.tar` & `lancedb_tables-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 lancedb_tables-0.1.1/.python-version
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 lancedb_tables-0.1.1/requirements-dev.lock
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 lancedb_tables-0.1.1/requirements.lock
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 lancedb_tables-0.1.1/src/lancedb_tables/__init__.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 lancedb_tables-0.1.1/src/lancedb_tables/lance_table.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 lancedb_tables-0.1.1/.gitignore
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 lancedb_tables-0.1.1/README.md
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 lancedb_tables-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 lancedb_tables-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 lancedb_tables-0.1.2/.python-version
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 lancedb_tables-0.1.2/requirements-dev.lock
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 lancedb_tables-0.1.2/requirements.lock
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 lancedb_tables-0.1.2/src/lancedb_tables/__init__.py
+-rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 lancedb_tables-0.1.2/src/lancedb_tables/lance_table.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 lancedb_tables-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 lancedb_tables-0.1.2/README.md
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 lancedb_tables-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 lancedb_tables-0.1.2/PKG-INFO
```

### Comparing `lancedb_tables-0.1.1/src/lancedb_tables/lance_table.py` & `lancedb_tables-0.1.2/src/lancedb_tables/lance_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,14 +54,17 @@
                 datetime.timedelta(seconds=self.CLEANUP_TIME))
 
             # merge insert data into table
             lance_tbl.merge_insert(merge_on) \
                 .when_not_matched_insert_all() \
                 .execute(data)
 
+            # create scalar index
+            lance_tbl.create_scalar_index(column=merge_on)
+
         except FileNotFoundError:
             # Handle the case where the table does not exist
             print(f"Creating table {table}")
             lance_tbl = db.create_table(name=table, data=data)
 
     def open_table(self, uri: str, table: str, conn_params: dict[str, any] = None):
         """
```

### Comparing `lancedb_tables-0.1.1/README.md` & `lancedb_tables-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lancedb_tables-0.1.1/pyproject.toml` & `lancedb_tables-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lancedb-tables"
-version = "0.1.1"
+version = "0.1.2"
 description = "An embedded streaming OLAP data pipeline with LanceDB"
 authors = [{ name = "Evan K", email = "ekcopersonal@gmail.com" }]
 dependencies = ["lancedb==0.6.13"]
 readme = "README.md"
 requires-python = ">= 3.12"
 
 [build-system]
```

### Comparing `lancedb_tables-0.1.1/PKG-INFO` & `lancedb_tables-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: lancedb-tables
-Version: 0.1.1
+Version: 0.1.2
 Summary: An embedded streaming OLAP data pipeline with LanceDB
 Author-email: Evan K <ekcopersonal@gmail.com>
 Requires-Python: >=3.12
 Requires-Dist: lancedb==0.6.13
 Description-Content-Type: text/markdown
 
 # lancedb-tables
```

