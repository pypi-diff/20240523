# Comparing `tmp/tulona-0.8.1.tar.gz` & `tmp/tulona-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulona-0.8.1.tar", last modified: Sat May 18 01:54:41 2024, max compression
+gzip compressed data, was "tulona-0.8.2.tar", last modified: Thu May 23 15:30:08 2024, max compression
```

## Comparing `tulona-0.8.1.tar` & `tulona-0.8.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:40.994581 tulona-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-18 01:54:33.000000 tulona-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14812 2024-05-18 01:54:40.994581 tulona-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-05-18 01:54:33.000000 tulona-0.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:40.986581 tulona-0.8.1/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:40.986581 tulona-0.8.1/core/tulona/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:40.990581 tulona-0.8.1/core/tulona/adapter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:40.990581 tulona-0.8.1/core/tulona/adapter/base/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/adapter/base/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/adapter/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/adapter/mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/adapter/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/adapter/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/adapter/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:40.990581 tulona-0.8.1/core/tulona/cli/
--rw-r--r--   0 runner    (1001) docker     (127)    18678 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/cli/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:40.990581 tulona-0.8.1/core/tulona/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/config/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:40.990581 tulona-0.8.1/core/tulona/task/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    25257 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/task/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/task/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/task/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/task/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    16803 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/task/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:40.994581 tulona-0.8.1/core/tulona/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/util/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/util/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/util/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/util/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/util/profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/util/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-18 01:54:33.000000 tulona-0.8.1/core/tulona/util/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:54:40.994581 tulona-0.8.1/core/tulona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14812 2024-05-18 01:54:40.000000 tulona-0.8.1/core/tulona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-18 01:54:40.000000 tulona-0.8.1/core/tulona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 01:54:40.000000 tulona-0.8.1/core/tulona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-18 01:54:40.000000 tulona-0.8.1/core/tulona.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-18 01:54:40.000000 tulona-0.8.1/core/tulona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-18 01:54:40.000000 tulona-0.8.1/core/tulona.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-18 01:54:33.000000 tulona-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 01:54:40.994581 tulona-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:30:08.333631 tulona-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-23 15:29:58.000000 tulona-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15585 2024-05-23 15:30:08.333631 tulona-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13878 2024-05-23 15:29:58.000000 tulona-0.8.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:30:08.325631 tulona-0.8.2/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:30:08.329631 tulona-0.8.2/core/tulona/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:30:08.329631 tulona-0.8.2/core/tulona/adapter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:30:08.329631 tulona-0.8.2/core/tulona/adapter/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/adapter/base/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/adapter/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/adapter/mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/adapter/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/adapter/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/adapter/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:30:08.329631 tulona-0.8.2/core/tulona/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    18676 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/cli/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:30:08.333631 tulona-0.8.2/core/tulona/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:30:08.333631 tulona-0.8.2/core/tulona/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25257 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/task/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/task/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/task/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9626 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/task/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16803 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/task/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:30:08.333631 tulona-0.8.2/core/tulona/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/util/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/util/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/util/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/util/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/util/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/util/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-23 15:29:58.000000 tulona-0.8.2/core/tulona/util/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:30:08.333631 tulona-0.8.2/core/tulona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15585 2024-05-23 15:30:08.000000 tulona-0.8.2/core/tulona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-23 15:30:08.000000 tulona-0.8.2/core/tulona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:30:08.000000 tulona-0.8.2/core/tulona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-23 15:30:08.000000 tulona-0.8.2/core/tulona.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-23 15:30:08.000000 tulona-0.8.2/core/tulona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 15:30:08.000000 tulona-0.8.2/core/tulona.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-23 15:29:58.000000 tulona-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:30:08.333631 tulona-0.8.2/setup.cfg
```

### Comparing `tulona-0.8.1/LICENSE` & `tulona-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tulona-0.8.1/PKG-INFO` & `tulona-0.8.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.8.1
+Version: 0.8.2
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
@@ -114,34 +114,35 @@
 
 .. code-block:: yaml
 
   version: '2.0'
   name: integration_project
   config_version: 1
 
-  outdir: output # the folder comparison result is written into
+  outdir: output # optional
 
   # Datasource names must be unique
   datasources:
     employee_postgres:
       connection_profile: pgdb
       database: postgresdb
       schema: corporate
       table: employee
       primary_key: Employee_ID
       exclude_columns:
-        - name
+        - Email
+        - Name
       compare_column: Employee_ID
     employee_mysql:
       connection_profile: mydb
       schema: corporate
       table: employee
       primary_key: Employee_ID
       exclude_columns:
-        - phone_number
+        - Phone_Number
       compare_column: Employee_ID
     person_postgres:
       connection_profile: pgdb
       database: postgresdb
       schema: corporate
       table: people_composite_key
       primary_key:
@@ -189,14 +190,34 @@
       connection_profile: mydb
       schema: corporate
       query: select * from corporate.employee
       primary_key: Employee_ID
       exclude_columns:
         - phone_number
       compare_column: Employee_ID
+    employee_postgres_query_tab:
+      connection_profile: pgdb
+      database: postgresdb
+      schema: corporate
+      table: employee
+      query: select * from postgresdb.corporate.employee
+      primary_key: Employee_ID
+      exclude_columns:
+        - name
+      compare_column: Employee_ID
+    employee_mysql_query_tab:
+      connection_profile: mydb
+      schema: corporate
+      table: employee
+      query: select * from corporate.employee
+      primary_key: Employee_ID
+      exclude_columns:
+        - phone_number
+      compare_column: Employee_ID
+
 
   # List of task configs(Dict)
   # Depending on the accepted params, task config can have different params
   # The value for that `task` key is the name of the command you want to run
   task_config:
     - task: ping
       datasources:
@@ -204,20 +225,20 @@
         - none_mysql
         - employee_mysql_query
 
     - task: profile
       datasources:
         - employee_postgres
         - employee_mysql
+      compare: true
 
     - task: profile
       datasources:
         - person_postgres
         - person_mysql
-      compare: true
 
     - task: compare-row
       datasources:
         - employee_postgres
         - employee_mysql
       sample_count: 30
 
@@ -278,14 +299,18 @@
       compare: true
 
     - task: scan
       datasources:
         - postgresdb_postgres
         - none_mysql
       compare: true
+    - task: compare
+      datasources:
+        - employee_postgres_query_tab
+        - employee_mysql_query_tab
 
 
 Features
 --------
 Executing `tulona` or `tulona -h` or `tulona --help` returns available commands.
 If you don't setup `task_config`, all commands take one mandatory parameter, `--datasources`, a comma separated list of names of datasources from project config file (`tulona-project.yml`).
 
@@ -301,15 +326,15 @@
 
     ``tulona ping --datasources employee_postgres,employee_mysql``
 
   * To ping all the datasources, just skip the `--datasources` parameter:
 
     ``tulona ping``
 
-* **profile**: To extract and compare metadata of two sources/tables. It includes metadata from `information_schema` related to the tables and some column level metrics (min, max, average, count & distinct_count). Sample commands:
+* **profile**: To extract and compare metadata of two sources/tables. It includes metadata from `information_schema` related to the tables and some column level metrics (min, max, average, count & distinct_count). Note that specifying `database`, `schema` and `table` is required for `profile` to work regardless the use of `query`. Sample commands:
 
   * Profiling without `--compare` flag. It will write metadata and metrics about different sources/tables in different sheets/tabs in the excel file (not a comparison view):
 
     ``tulona profile --datasources employee_postgres,employee_mysql``
 
   * Profiling with `--compare` flag. It will produce a comparison view (side by side):
```

### Comparing `tulona-0.8.1/README.rst` & `tulona-0.8.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -70,34 +70,35 @@
 
 .. code-block:: yaml
 
   version: '2.0'
   name: integration_project
   config_version: 1
 
-  outdir: output # the folder comparison result is written into
+  outdir: output # optional
 
   # Datasource names must be unique
   datasources:
     employee_postgres:
       connection_profile: pgdb
       database: postgresdb
       schema: corporate
       table: employee
       primary_key: Employee_ID
       exclude_columns:
-        - name
+        - Email
+        - Name
       compare_column: Employee_ID
     employee_mysql:
       connection_profile: mydb
       schema: corporate
       table: employee
       primary_key: Employee_ID
       exclude_columns:
-        - phone_number
+        - Phone_Number
       compare_column: Employee_ID
     person_postgres:
       connection_profile: pgdb
       database: postgresdb
       schema: corporate
       table: people_composite_key
       primary_key:
@@ -145,14 +146,34 @@
       connection_profile: mydb
       schema: corporate
       query: select * from corporate.employee
       primary_key: Employee_ID
       exclude_columns:
         - phone_number
       compare_column: Employee_ID
+    employee_postgres_query_tab:
+      connection_profile: pgdb
+      database: postgresdb
+      schema: corporate
+      table: employee
+      query: select * from postgresdb.corporate.employee
+      primary_key: Employee_ID
+      exclude_columns:
+        - name
+      compare_column: Employee_ID
+    employee_mysql_query_tab:
+      connection_profile: mydb
+      schema: corporate
+      table: employee
+      query: select * from corporate.employee
+      primary_key: Employee_ID
+      exclude_columns:
+        - phone_number
+      compare_column: Employee_ID
+
 
   # List of task configs(Dict)
   # Depending on the accepted params, task config can have different params
   # The value for that `task` key is the name of the command you want to run
   task_config:
     - task: ping
       datasources:
@@ -160,20 +181,20 @@
         - none_mysql
         - employee_mysql_query
 
     - task: profile
       datasources:
         - employee_postgres
         - employee_mysql
+      compare: true
 
     - task: profile
       datasources:
         - person_postgres
         - person_mysql
-      compare: true
 
     - task: compare-row
       datasources:
         - employee_postgres
         - employee_mysql
       sample_count: 30
 
@@ -234,14 +255,18 @@
       compare: true
 
     - task: scan
       datasources:
         - postgresdb_postgres
         - none_mysql
       compare: true
+    - task: compare
+      datasources:
+        - employee_postgres_query_tab
+        - employee_mysql_query_tab
 
 
 Features
 --------
 Executing `tulona` or `tulona -h` or `tulona --help` returns available commands.
 If you don't setup `task_config`, all commands take one mandatory parameter, `--datasources`, a comma separated list of names of datasources from project config file (`tulona-project.yml`).
 
@@ -257,15 +282,15 @@
 
     ``tulona ping --datasources employee_postgres,employee_mysql``
 
   * To ping all the datasources, just skip the `--datasources` parameter:
 
     ``tulona ping``
 
-* **profile**: To extract and compare metadata of two sources/tables. It includes metadata from `information_schema` related to the tables and some column level metrics (min, max, average, count & distinct_count). Sample commands:
+* **profile**: To extract and compare metadata of two sources/tables. It includes metadata from `information_schema` related to the tables and some column level metrics (min, max, average, count & distinct_count). Note that specifying `database`, `schema` and `table` is required for `profile` to work regardless the use of `query`. Sample commands:
 
   * Profiling without `--compare` flag. It will write metadata and metrics about different sources/tables in different sheets/tabs in the excel file (not a comparison view):
 
     ``tulona profile --datasources employee_postgres,employee_mysql``
 
   * Profiling with `--compare` flag. It will produce a comparison view (side by side):
```

### Comparing `tulona-0.8.1/core/tulona/adapter/connection.py` & `tulona-0.8.2/core/tulona/adapter/connection.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.1/core/tulona/adapter/mssql.py` & `tulona-0.8.2/core/tulona/adapter/mssql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.1/core/tulona/adapter/mysql.py` & `tulona-0.8.2/core/tulona/adapter/mysql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.1/core/tulona/adapter/postgres.py` & `tulona-0.8.2/core/tulona/adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.1/core/tulona/adapter/snowflake.py` & `tulona-0.8.2/core/tulona/adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.1/core/tulona/cli/base.py` & `tulona-0.8.2/core/tulona/cli/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 @p.datasources
 def ping(ctx, **kwargs):
     """Test connectivity to datasources"""
 
     ping_tasks = []
     if kwargs["datasources"]:
         task_config = {
-            "task": "compare",
+            "task": "ping",
             "datasources": kwargs["datasources"].split(","),
         }
         ping_tasks.append(task_config)
     else:
         ping_tasks = [t for t in ctx.obj["project"]["task_config"] if t["task"] == "ping"]
 
     if len(ping_tasks) == 0:
@@ -102,15 +102,15 @@
 @p.composite
 @p.case_insensitive
 def scan(ctx, **kwargs):
     """Scan data sources to collect metadata"""
     scan_tasks = []
     if kwargs["datasources"]:
         task_config = {
-            "task": "compare",
+            "task": "scan",
             "datasources": kwargs["datasources"].split(","),
         }
         if kwargs["compare"]:
             task_config["compare"] = kwargs["compare"]
         if kwargs["sample_count"]:
             task_config["sample_count"] = kwargs["sample_count"]
         if kwargs["composite"]:
@@ -157,15 +157,15 @@
 @p.datasources
 @p.compare
 def profile(ctx, **kwargs):
     """Profile data sources to collect metadata [row count, column min/max/mean etc.]"""
     profile_tasks = []
     if kwargs["datasources"]:
         task_config = {
-            "task": "compare",
+            "task": "profile",
             "datasources": kwargs["datasources"].split(","),
         }
         if kwargs["compare"]:
             task_config["compare"] = kwargs["compare"]
         profile_tasks.append(task_config)
     else:
         profile_tasks = [
@@ -205,15 +205,15 @@
 @p.sample_count
 @p.case_insensitive
 def compare_row(ctx, **kwargs):
     """Compares rows from two data entities"""
     compare_row_tasks = []
     if kwargs["datasources"]:
         task_config = {
-            "task": "compare",
+            "task": "compare-row",
             "datasources": kwargs["datasources"].split(","),
         }
         if kwargs["sample_count"]:
             task_config["sample_count"] = kwargs["sample_count"]
         if kwargs["case_insensitive"]:
             task_config["case_insensitive"] = kwargs["case_insensitive"]
         compare_row_tasks.append(task_config)
```

### Comparing `tulona-0.8.1/core/tulona/cli/params.py` & `tulona-0.8.2/core/tulona/cli/params.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.1/core/tulona/config/profile.py` & `tulona-0.8.2/core/tulona/config/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.1/core/tulona/config/project.py` & `tulona-0.8.2/core/tulona/config/project.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.1/core/tulona/exceptions.py` & `tulona-0.8.2/core/tulona/exceptions.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.1/core/tulona/task/base.py` & `tulona-0.8.2/core/tulona/task/base.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.1/core/tulona/task/compare.py` & `tulona-0.8.2/core/tulona/task/compare.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.1/core/tulona/task/ping.py` & `tulona-0.8.2/core/tulona/task/ping.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.1/core/tulona/task/scan.py` & `tulona-0.8.2/core/tulona/task/scan.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.1/core/tulona/util/database.py` & `tulona-0.8.2/core/tulona/util/database.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.1/core/tulona/util/dataframe.py` & `tulona-0.8.2/core/tulona/util/dataframe.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.1/core/tulona/util/excel.py` & `tulona-0.8.2/core/tulona/util/excel.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.1/core/tulona/util/filesystem.py` & `tulona-0.8.2/core/tulona/util/filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
 from pathlib import Path
-from typing import Union
+from typing import Dict, Union
 
 
 def path_exists(p: Union[str, Path]) -> bool:
     return Path(p).exists()
 
 
 def recursive_rmdir(directory):
@@ -34,15 +34,15 @@
 def get_run_result_dir(basedir: str):
     out_timestamp = datetime.now().strftime("%Y_%m_%d_%H_%M_%S_%f")
     run_dir = Path(basedir, f"runid__{out_timestamp}")
     return run_dir
 
 
 # TODO: Testable - pull current timestamp from caller
-def get_task_outdir(run_dir: str, task_conf: str):
+def get_task_outdir(run_dir: str, task_conf: Dict):
     task = task_conf["task"].replace("-", "")
     ds_list = [ds.split(":")[0].replace("_", "") for ds in task_conf["datasources"]]
     extra_params = []
     for p in task_conf:
         if p not in ["task", "datasources"]:
             if isinstance(task_conf[p], int):
                 extra_params.extend([p.replace("_", ""), str(task_conf[p])])
```

### Comparing `tulona-0.8.1/core/tulona/util/profiles.py` & `tulona-0.8.2/core/tulona/util/profiles.py`

 * *Files identical despite different names*

### Comparing `tulona-0.8.1/core/tulona/util/sql.py` & `tulona-0.8.2/core/tulona/util/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         select * from information_schema.columns
         where upper(table_schema) = '{schema.upper()}'
         and upper(table_name) = '{table.upper()}'
         """
     return query
 
 
-def get_metric_query(table_fqn, columns_dtype: Dict, metrics: list, quoted=False):
+def get_metric_query(data_container, columns_dtype: Dict, metrics: list, quoted=False):
     numeric_types = [
         "smallint",
         "integer",
         "bigint",
         "decimal",
         "numeric",
         "real",
@@ -171,15 +171,15 @@
             else:
                 qp.append(f"'NA' as {col}_{m.lower()}")
         call_funcs.extend(qp)
 
     query = f"""
     select
         {", ".join(call_funcs)}
-    from {table_fqn}
+    from {data_container}
     """
 
     return query
 
 
 def get_table_data_query(
     dbtype, data_container, sample_count, query_expr: Optional[str] = None
```

### Comparing `tulona-0.8.1/core/tulona.egg-info/PKG-INFO` & `tulona-0.8.2/core/tulona.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.8.1
+Version: 0.8.2
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
@@ -114,34 +114,35 @@
 
 .. code-block:: yaml
 
   version: '2.0'
   name: integration_project
   config_version: 1
 
-  outdir: output # the folder comparison result is written into
+  outdir: output # optional
 
   # Datasource names must be unique
   datasources:
     employee_postgres:
       connection_profile: pgdb
       database: postgresdb
       schema: corporate
       table: employee
       primary_key: Employee_ID
       exclude_columns:
-        - name
+        - Email
+        - Name
       compare_column: Employee_ID
     employee_mysql:
       connection_profile: mydb
       schema: corporate
       table: employee
       primary_key: Employee_ID
       exclude_columns:
-        - phone_number
+        - Phone_Number
       compare_column: Employee_ID
     person_postgres:
       connection_profile: pgdb
       database: postgresdb
       schema: corporate
       table: people_composite_key
       primary_key:
@@ -189,14 +190,34 @@
       connection_profile: mydb
       schema: corporate
       query: select * from corporate.employee
       primary_key: Employee_ID
       exclude_columns:
         - phone_number
       compare_column: Employee_ID
+    employee_postgres_query_tab:
+      connection_profile: pgdb
+      database: postgresdb
+      schema: corporate
+      table: employee
+      query: select * from postgresdb.corporate.employee
+      primary_key: Employee_ID
+      exclude_columns:
+        - name
+      compare_column: Employee_ID
+    employee_mysql_query_tab:
+      connection_profile: mydb
+      schema: corporate
+      table: employee
+      query: select * from corporate.employee
+      primary_key: Employee_ID
+      exclude_columns:
+        - phone_number
+      compare_column: Employee_ID
+
 
   # List of task configs(Dict)
   # Depending on the accepted params, task config can have different params
   # The value for that `task` key is the name of the command you want to run
   task_config:
     - task: ping
       datasources:
@@ -204,20 +225,20 @@
         - none_mysql
         - employee_mysql_query
 
     - task: profile
       datasources:
         - employee_postgres
         - employee_mysql
+      compare: true
 
     - task: profile
       datasources:
         - person_postgres
         - person_mysql
-      compare: true
 
     - task: compare-row
       datasources:
         - employee_postgres
         - employee_mysql
       sample_count: 30
 
@@ -278,14 +299,18 @@
       compare: true
 
     - task: scan
       datasources:
         - postgresdb_postgres
         - none_mysql
       compare: true
+    - task: compare
+      datasources:
+        - employee_postgres_query_tab
+        - employee_mysql_query_tab
 
 
 Features
 --------
 Executing `tulona` or `tulona -h` or `tulona --help` returns available commands.
 If you don't setup `task_config`, all commands take one mandatory parameter, `--datasources`, a comma separated list of names of datasources from project config file (`tulona-project.yml`).
 
@@ -301,15 +326,15 @@
 
     ``tulona ping --datasources employee_postgres,employee_mysql``
 
   * To ping all the datasources, just skip the `--datasources` parameter:
 
     ``tulona ping``
 
-* **profile**: To extract and compare metadata of two sources/tables. It includes metadata from `information_schema` related to the tables and some column level metrics (min, max, average, count & distinct_count). Sample commands:
+* **profile**: To extract and compare metadata of two sources/tables. It includes metadata from `information_schema` related to the tables and some column level metrics (min, max, average, count & distinct_count). Note that specifying `database`, `schema` and `table` is required for `profile` to work regardless the use of `query`. Sample commands:
 
   * Profiling without `--compare` flag. It will write metadata and metrics about different sources/tables in different sheets/tabs in the excel file (not a comparison view):
 
     ``tulona profile --datasources employee_postgres,employee_mysql``
 
   * Profiling with `--compare` flag. It will produce a comparison view (side by side):
```

### Comparing `tulona-0.8.1/core/tulona.egg-info/SOURCES.txt` & `tulona-0.8.2/core/tulona.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tulona-0.8.1/pyproject.toml` & `tulona-0.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tulona"
-version = "0.8.1"
+version = "0.8.2"
 description = "A tool to compare data from different sources."
 dependencies = [
   "click~=8.1",
   "ruamel.yaml~=0.18",
   "psycopg2-binary~=2.9",
   "pymysql~=1.1",
   "cryptography~=42.0",
@@ -125,15 +125,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 90
 skip = [".gitignore"]
 
 [tool.bumpversion]
-current_version = "0.8.1"
+current_version = "0.8.2"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 tag = false
```

