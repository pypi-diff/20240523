# Comparing `tmp/sqladaptor-0.1.0.tar.gz` & `tmp/sqladaptor-0.1.1.tar.gz`

## Comparing `sqladaptor-0.1.0.tar` & `sqladaptor-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 sqladaptor-0.1.0/.python-version
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 sqladaptor-0.1.0/.idea/.gitignore
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sqladaptor-0.1.0/.idea/misc.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 sqladaptor-0.1.0/.idea/modules.xml
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 sqladaptor-0.1.0/.idea/ruff.xml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 sqladaptor-0.1.0/.idea/sqladaptor.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 sqladaptor-0.1.0/.idea/vcs.xml
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 sqladaptor-0.1.0/.idea/workspace.xml
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 sqladaptor-0.1.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 sqladaptor-0.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 sqladaptor-0.1.0/example/db.sqlite
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 sqladaptor-0.1.0/example/quick_run.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqladaptor-0.1.0/src/sqladaptor/__init__.py
--rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 sqladaptor-0.1.0/src/sqladaptor/sqlite.py
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 sqladaptor-0.1.0/test/test_sqlite_adaptor.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sqladaptor-0.1.0/.gitignore
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 sqladaptor-0.1.0/README.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 sqladaptor-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 sqladaptor-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/.python-version
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/.idea/.gitignore
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/.idea/modules.xml
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/.idea/ruff.xml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/.idea/sqladaptor.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/.idea/workspace.xml
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/example/db.sqlite
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/example/quick_run.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/src/sqladaptor/__init__.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/src/sqladaptor/sqlite.py
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/test/test_sqlite_adaptor.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/README.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/PKG-INFO
```

### Comparing `sqladaptor-0.1.0/.idea/sqladaptor.iml` & `sqladaptor-0.1.1/.idea/sqladaptor.iml`

 * *Files identical despite different names*

### Comparing `sqladaptor-0.1.0/.idea/workspace.xml` & `sqladaptor-0.1.1/.idea/workspace.xml`

 * *Files 1% similar despite different names*

#### Comparing `sqladaptor-0.1.0/.idea/workspace.xml` & `sqladaptor-0.1.1/.idea/workspace.xml`

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="f543d5ca-4570-440d-bf15-99b5763dd321" name="Changes" comment="">
-      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/sqladaptor/sqlite.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/sqladaptor/sqlite.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
@@ -98,15 +98,15 @@
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="f543d5ca-4570-440d-bf15-99b5763dd321" name="Changes" comment=""/>
       <created>1716442147219</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1716442147219</updated>
-      <workItem from="1716442148490" duration="4374000"/>
+      <workItem from="1716442148490" duration="5081000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
```

### Comparing `sqladaptor-0.1.0/.idea/inspectionProfiles/Project_Default.xml` & `sqladaptor-0.1.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `sqladaptor-0.1.0/example/db.sqlite` & `sqladaptor-0.1.1/example/db.sqlite`

 * *Files identical despite different names*

### Comparing `sqladaptor-0.1.0/example/quick_run.py` & `sqladaptor-0.1.1/example/quick_run.py`

 * *Files identical despite different names*

### Comparing `sqladaptor-0.1.0/src/sqladaptor/sqlite.py` & `sqladaptor-0.1.1/src/sqladaptor/sqlite.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,47 +20,47 @@
 
     def make_conn(self):
         return sqlite3.connect(self.db_fname)
 
     def execute(self, *args):
         return self.cursor.execute(*args)
 
-    def execute_to_df(self, sql, params=None):
+    def execute_to_df(self, sql: str, params=None):
         return pandas.read_sql_query(sql, self.conn, params=params)
 
     def commit(self):
         self.conn.commit()
 
-    def set_from_df(self, table, df, index=False, if_exists="append"):
+    def set_from_df(self, table: str, df: pandas.DataFrame, index=False, if_exists="append"):
         """
         :param df: pandas.Dataframe
         :param if_exists: ["fail", "append", "replace"]
         """
         df.to_sql(con=self.conn, name=table, index=index, if_exists=if_exists)
         self.commit()
 
-    def replace_table_with_df(self, table, df, index=False):
+    def replace_table_with_df(self, table: str, df: pandas.DataFrame, index=False):
         self.set_from_df(table, df, index=index, if_exists="replace")
 
-    def add_column(self, name, col_type, table):
+    def add_column(self, table: str, name: str, col_type: str):
         self.execute(f"ALTER TABLE {table} ADD COLUMN '{name}' '{col_type}';")
         self.commit()
 
-    def get_columns(self, table):
+    def get_columns(self, table: str):
         queries = self.execute(f"PRAGMA table_info('{table}');").fetchall()
         return [r[1] for r in queries]
 
     def close(self):
         self.conn.close()
 
     def get_tables(self):
         rows = self.execute("SELECT name FROM sqlite_master;").fetchall()
         return [r[0] for r in rows]
 
-    def get_select_sql_and_params(self, table, where):
+    def get_select_sql_and_params(self, table: str, where: dict[str, [None, str, int, float]]):
         sql = f"SELECT * FROM {table} "
         params = []
         if where:
             for i, [k, v] in enumerate(where.items()):
                 sql += ("WHERE " if i == 0 else "AND ") + f"{k} = ? "
                 params.append(str(v))
         return sql, params
```

### Comparing `sqladaptor-0.1.0/test/test_sqlite_adaptor.py` & `sqladaptor-0.1.1/test/test_sqlite_adaptor.py`

 * *Files identical despite different names*

### Comparing `sqladaptor-0.1.0/README.md` & `sqladaptor-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sqladaptor-0.1.0/pyproject.toml` & `sqladaptor-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sqladaptor"
-version = "0.1.0"
+version = "0.1.1"
 description = "Starting adaptor for JSON/Pandas to SQL db"
 authors = [
     { name = "Bosco Ho", email = "apposite@gmail.com" }
 ]
 dependencies = [
     "path>=16.14.0",
     "pydash>=8.0.1",
```

### Comparing `sqladaptor-0.1.0/PKG-INFO` & `sqladaptor-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sqladaptor
-Version: 0.1.0
+Version: 0.1.1
 Summary: Starting adaptor for JSON/Pandas to SQL db
 Author-email: Bosco Ho <apposite@gmail.com>
 Requires-Python: >=3.8
 Requires-Dist: pandas>=2.2.2
 Requires-Dist: path>=16.14.0
 Requires-Dist: pydash>=8.0.1
 Requires-Dist: pytest>=8.2.1
```

