# Comparing `tmp/nurtelecom_gras_library-1.3.5.tar.gz` & `tmp/nurtelecom_gras_library-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nurtelecom_gras_library-1.3.5.tar", last modified: Wed Mar 27 09:03:36 2024, max compression
+gzip compressed data, was "nurtelecom_gras_library-1.3.6.tar", last modified: Thu May 23 09:00:54 2024, max compression
```

## Comparing `nurtelecom_gras_library-1.3.5.tar` & `nurtelecom_gras_library-1.3.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 09:03:36.100648 nurtelecom_gras_library-1.3.5/
--rw-rw-rw-   0        0        0     1089 2023-09-22 10:27:00.000000 nurtelecom_gras_library-1.3.5/LICENSE
--rw-rw-rw-   0        0        0     3024 2024-03-27 09:03:36.100648 nurtelecom_gras_library-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0      709 2023-09-22 10:27:00.000000 nurtelecom_gras_library-1.3.5/README.md
--rw-rw-rw-   0        0        0     1089 2024-03-27 06:23:55.000000 nurtelecom_gras_library-1.3.5/pyproject.toml
--rw-rw-rw-   0        0        0      115 2024-03-27 09:03:36.105611 nurtelecom_gras_library-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1603 2024-01-30 04:48:12.000000 nurtelecom_gras_library-1.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-27 09:03:36.070506 nurtelecom_gras_library-1.3.5/src/
-drwxrwxrwx   0        0        0        0 2024-03-27 09:03:36.080020 nurtelecom_gras_library-1.3.5/src/nurtelecom_gras_library/
--rw-rw-rw-   0        0        0    16827 2024-02-01 03:30:08.000000 nurtelecom_gras_library-1.3.5/src/nurtelecom_gras_library/PLSQL_data_importer.py
--rw-rw-rw-   0        0        0     4179 2024-03-27 09:01:58.000000 nurtelecom_gras_library-1.3.5/src/nurtelecom_gras_library/PLSQL_geodata_importer.py
--rw-rw-rw-   0        0        0      392 2024-03-12 09:02:49.000000 nurtelecom_gras_library-1.3.5/src/nurtelecom_gras_library/__init__.py
--rw-rw-rw-   0        0        0    11586 2024-03-14 03:13:22.000000 nurtelecom_gras_library-1.3.5/src/nurtelecom_gras_library/additional_functions.py
--rw-rw-rw-   0        0        0     1981 2024-03-27 06:23:42.000000 nurtelecom_gras_library-1.3.5/src/nurtelecom_gras_library/updated_connection.py
-drwxrwxrwx   0        0        0        0 2024-03-27 09:03:36.099611 nurtelecom_gras_library-1.3.5/src/nurtelecom_gras_library.egg-info/
--rw-rw-rw-   0        0        0     3024 2024-03-27 09:03:36.000000 nurtelecom_gras_library-1.3.5/src/nurtelecom_gras_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2024-03-27 09:03:36.000000 nurtelecom_gras_library-1.3.5/src/nurtelecom_gras_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 09:03:36.000000 nurtelecom_gras_library-1.3.5/src/nurtelecom_gras_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-03-27 09:03:36.000000 nurtelecom_gras_library-1.3.5/src/nurtelecom_gras_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-03-27 09:03:36.000000 nurtelecom_gras_library-1.3.5/src/nurtelecom_gras_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 09:00:54.835205 nurtelecom_gras_library-1.3.6/
+-rw-rw-rw-   0        0        0     1089 2023-09-22 10:27:00.000000 nurtelecom_gras_library-1.3.6/LICENSE
+-rw-rw-rw-   0        0        0     3050 2024-05-23 09:00:54.834205 nurtelecom_gras_library-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0      709 2023-09-22 10:27:00.000000 nurtelecom_gras_library-1.3.6/README.md
+-rw-rw-rw-   0        0        0     1107 2024-05-23 09:00:32.000000 nurtelecom_gras_library-1.3.6/pyproject.toml
+-rw-rw-rw-   0        0        0      115 2024-05-23 09:00:54.836206 nurtelecom_gras_library-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2024-01-30 04:48:12.000000 nurtelecom_gras_library-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:00:54.801202 nurtelecom_gras_library-1.3.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 09:00:54.811202 nurtelecom_gras_library-1.3.6/src/nurtelecom_gras_library/
+-rw-rw-rw-   0        0        0    16214 2024-05-23 08:58:41.000000 nurtelecom_gras_library-1.3.6/src/nurtelecom_gras_library/PLSQL_data_importer.py
+-rw-rw-rw-   0        0        0     4179 2024-03-27 09:01:58.000000 nurtelecom_gras_library-1.3.6/src/nurtelecom_gras_library/PLSQL_geodata_importer.py
+-rw-rw-rw-   0        0        0      392 2024-03-12 09:02:49.000000 nurtelecom_gras_library-1.3.6/src/nurtelecom_gras_library/__init__.py
+-rw-rw-rw-   0        0        0    11586 2024-03-14 03:13:22.000000 nurtelecom_gras_library-1.3.6/src/nurtelecom_gras_library/additional_functions.py
+-rw-rw-rw-   0        0        0     1981 2024-03-27 06:23:42.000000 nurtelecom_gras_library-1.3.6/src/nurtelecom_gras_library/updated_connection.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:00:54.833204 nurtelecom_gras_library-1.3.6/src/nurtelecom_gras_library.egg-info/
+-rw-rw-rw-   0        0        0     3050 2024-05-23 09:00:54.000000 nurtelecom_gras_library-1.3.6/src/nurtelecom_gras_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2024-05-23 09:00:54.000000 nurtelecom_gras_library-1.3.6/src/nurtelecom_gras_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 09:00:54.000000 nurtelecom_gras_library-1.3.6/src/nurtelecom_gras_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-05-23 09:00:54.000000 nurtelecom_gras_library-1.3.6/src/nurtelecom_gras_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-23 09:00:54.000000 nurtelecom_gras_library-1.3.6/src/nurtelecom_gras_library.egg-info/top_level.txt
```

### Comparing `nurtelecom_gras_library-1.3.5/LICENSE` & `nurtelecom_gras_library-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nurtelecom_gras_library-1.3.5/PKG-INFO` & `nurtelecom_gras_library-1.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nurtelecom_gras_library
-Version: 1.3.5
+Version: 1.3.6
 Summary: Official Nurtelecom gras library
 Home-page: https://github.com/beksultantuleev/nurtelecom_gras_library.git
 Author: Beksultan Tuleev
 Author-email: Beksultan Tuleev <kazamabeks@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Beck Kazama
@@ -36,14 +36,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Requires-Dist: cx_Oracle
 Requires-Dist: pandas
+Requires-Dist: geopandas
 Requires-Dist: sqlalchemy
 Requires-Dist: openpyxl
 Requires-Dist: tabulate
 Requires-Dist: requests
 Requires-Dist: transliterate
 
 # nurtelecom_gras_library
```

### Comparing `nurtelecom_gras_library-1.3.5/README.md` & `nurtelecom_gras_library-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `nurtelecom_gras_library-1.3.5/pyproject.toml` & `nurtelecom_gras_library-1.3.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 
 [project]
 name = "nurtelecom_gras_library"
-version = "1.3.5"
+version = "1.3.6"
 description = "Official Nurtelecom gras library"
 readme = "README.md"
 authors = [
     { name = "Beksultan Tuleev", email = "kazamabeks@gmail.com" }
 ]
 license = { file="LICENSE" }
 classifiers = [
@@ -24,14 +24,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 urls = { "Homepage" = "https://github.com/beksultantuleev/nurtelecom_gras_library.git" }
 dependencies = [
     "cx_Oracle",
     "pandas",
+    "geopandas",
     "sqlalchemy",
     "openpyxl",
     "tabulate",
     "requests",
     "transliterate"
 ]
```

### Comparing `nurtelecom_gras_library-1.3.5/setup.py` & `nurtelecom_gras_library-1.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `nurtelecom_gras_library-1.3.5/src/nurtelecom_gras_library/PLSQL_data_importer.py` & `nurtelecom_gras_library-1.3.6/src/nurtelecom_gras_library/PLSQL_data_importer.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,28 +2,34 @@
 import pandas as pd
 import timeit
 from sqlalchemy.engine import create_engine
 from sqlalchemy import update
 from sqlalchemy import text
 from nurtelecom_gras_library.additional_functions import measure_time
 
+
 class PLSQL_data_importer():
 
     def __init__(self, user,
                  password,
                  host,
                  port='1521',
                  service_name='DWH') -> None:
 
         self.host = host
         self.port = port
         self.service_name = service_name
         self.user = user
         self.password = password
 
+        self.dsn_tns = cx_Oracle.makedsn(
+            self.host,
+            self.port,
+            service_name=self.service_name)
+
         self.ENGINE_PATH_WIN_AUTH = f'oracle://{self.user}:{self.password}@(DESCRIPTION=(ADDRESS=(PROTOCOL=TCP)(HOST={self.host})(PORT={self.port}))(CONNECT_DATA=(SERVICE_NAME={self.service_name})))'
 
     def get_engine(self):
         """
         Creates and returns a SQLAlchemy engine for database connections.
 
         Usage:
@@ -70,17 +76,17 @@
             return data
 
         except Exception as e:
             print(f"Error during data retrieval: {e}")
             raise
 
     def get_data_old(self, query,
-                 remove_column=[],
-                 remove_na=False,
-                 show_logs=False):
+                     remove_column=[],
+                     remove_na=False,
+                     show_logs=False):
         query = text(query)
         'establish connection and return data'
         start = timeit.default_timer()
 
         self.engine = create_engine(self.ENGINE_PATH_WIN_AUTH)
         self.conn = self.engine.connect()
         data = pd.read_sql(query, con=self.conn)
@@ -110,20 +116,22 @@
             query = text(query)
             engine = create_engine(self.ENGINE_PATH_WIN_AUTH)
 
             with engine.connect() as conn, open(path, 'w') as f:
                 for i, partial_df in enumerate(pd.read_sql(query, conn, chunksize=100000)):
                     print(f'Writing chunk "{i}" to "{path}"')
                     if is_csv:
-                        partial_df.to_csv(f, index=False, header=(i == 0), sep=sep)
+                        partial_df.to_csv(
+                            f, index=False, header=(i == 0), sep=sep)
                     else:
                         if i == 0:
                             partial_df.to_json(f, orient='records', lines=True)
                         else:
-                            partial_df.to_json(f, orient='records', lines=True, header=False)
+                            partial_df.to_json(
+                                f, orient='records', lines=True, header=False)
 
         except Exception as e:
             print(f"Error during export: {e}")
             raise
 
     def truncate_table(self, table_name):
         """
@@ -195,72 +203,27 @@
             conn.execute(query)  # text
             conn.close()
             if verbose:
                 print('Connection in execute is closed!')
         self.conn.close()
         self.engine.dispose()
 
-    def upload_pandas_df_to_oracle_experimental(self, pandas_df, table_name, geometry_cols=[], batch_size=15000):
-        # Prepare the values string for SQL statement
-        values_string_list = [
-            f":{i}" if col not in geometry_cols else f"SDO_UTIL.FROM_WKTGEOMETRY(:{i})"
-            for i, col in enumerate(pandas_df.columns, start=1)
-        ]
-        values_string = ', '.join(values_string_list)
-
-        # Convert geometry columns to string if necessary
-        if geometry_cols:
-            for geo_col in geometry_cols:
-                pandas_df[geo_col] = pandas_df[geo_col].astype(str)
-
-        # Prepare the data for insertion
-        pandas_tuple = [tuple(i) for i in pandas_df.to_numpy()]
-        sql_text = f"insert into {table_name} values({values_string})"
-
-        try:
-            # Use existing engine and connection management
-            self.engine = self.get_engine()
-            with self.engine.connect() as conn:
-                rowCount = 0
-                for start_pos in range(0, len(pandas_tuple), batch_size):
-                    data_batch = pandas_tuple[start_pos:start_pos + batch_size]
-                    conn.executemany(sql_text, data_batch)
-                    rowCount += len(data_batch)
-
-                # Update SDO_SRID for geometry columns if necessary
-                if geometry_cols:
-                    for geo_col in geometry_cols:
-                        update_sdo_srid = f"UPDATE {table_name} SET {geo_col}.SDO_SRID = 4326 WHERE {geo_col} IS NOT NULL"
-                        conn.execute(update_sdo_srid)
-                        print(f'SDO_SRID of "{geo_col}" is updated to "4326"')
-
-                print(
-                    f'Number of new added rows in "{table_name}": {rowCount}')
-                self.engine.dispose()
-        except Exception as e:
-            print(f'Error during insertion: {e}')
-            raise
-
     def upload_pandas_df_to_oracle(self, pandas_df, table_name, geometry_cols=[]):
         values_string_list = [
             f":{i}" if v not in geometry_cols else f"SDO_UTIL.FROM_WKTGEOMETRY(:{i})" for i, v in enumerate(pandas_df, start=1)]
         values_string = ', '.join(values_string_list)
         if len(geometry_cols) != 0:
             for geo_col in geometry_cols:
                 pandas_df.loc[:, geo_col] = pandas_df.loc[:,
                                                           geo_col].astype(str)
         try:
             # values_string = value_creator(pandas_df.shape[1])
             pandas_tuple = [tuple(i) for i in pandas_df.values]
             sql_text = f"insert into {table_name} values({values_string})"
             # print(sql_text)
-            self.dsn_tns = cx_Oracle.makedsn(
-                self.host,
-                self.port,
-                service_name=self.service_name)
 
             oracle_conn = cx_Oracle.connect(
                 user=self.user,
                 password=self.password,
                 dsn=self.dsn_tns
             )
             # oracle_cursor = oracle_conn.cursor()
@@ -291,67 +254,89 @@
             print('Error during insertion')
             if oracle_conn:
 
                 oracle_conn.close()
                 print('oracle connection is closed!')
             raise Exception
 
-    def upsert_from_pandas_df_experimental(self, pandas_df, table_name, list_of_keys, sum_update_columns=[], batch_size=15000):
-        # Column Lists
-        list_of_all_columns = list(pandas_df.columns)
-        list_regular_columns = list(
-            set(list_of_all_columns) - set(list_of_keys))
+    def upload_pandas_df_to_oracle_row(self, pandas_df, table_name, geometry_cols=[]):
+        'uploads row by row using clob'
+        # Prepare values string for the SQL insert statement
+        columns = pandas_df.columns
+        values_string = ', '.join([
+            f"SDO_UTIL.FROM_WKTGEOMETRY(:{i+1})" if col in geometry_cols else f":{i+1}"
+            for i, col in enumerate(columns)
+        ])
+        sql_text = f"INSERT INTO {table_name} ({', '.join(columns)}) VALUES ({values_string})"
+
+        # Convert geometry columns to WKT
+        for geo_col in geometry_cols:
+            pandas_df[geo_col] = pandas_df[geo_col].apply(
+                lambda geom: geom.wkt if geom else None)
 
-        # SQL Query Building
-        column_selection = ',\n'.join(
-            [f'\t:{col} AS {col}' for col in list_of_all_columns])
-        key_conditions = ' AND '.join(
-            [f"t.{key} = s.{key}" for key in list_of_keys])
-        update_selection = ',\n'.join(
-            [f"t.{col} = {'t.' + col + ' + ' if col in sum_update_columns else ''}s.{col}" for col in list_regular_columns])
-
-        merge_sql = f"""
-        MERGE INTO {table_name} t
-        USING (SELECT {column_selection} FROM dual) s
-        ON ({key_conditions})
-        WHEN MATCHED THEN UPDATE SET {update_selection}
-        WHEN NOT MATCHED THEN INSERT ({', '.join(list_of_all_columns)})
-        VALUES ({', '.join([f"s.{col}" for col in list_of_all_columns])})
-        """
-
-        # Execute Query in Batches
         try:
-            self.engine = self.get_engine()
-            with self.engine.connect() as conn:
-                data_list = pandas_df.to_dict(orient='records')
+            # Establish Oracle connection
+            oracle_conn = cx_Oracle.connect(
+                user=self.user,
+                password=self.password,
+                dsn=self.dsn_tns
+            )
+
+            with oracle_conn.cursor() as oracle_cursor:
                 rowCount = 0
-                for start_pos in range(0, len(data_list), batch_size):
-                    data_batch = data_list[start_pos:start_pos + batch_size]
-                    conn.execute(text(merge_sql), *data_batch)
-                    rowCount += len(data_batch)
+
+                for index, row in pandas_df.iterrows():
+                    bind_row = []
+                    input_sizes = []
+
+                    for col, value in zip(columns, row):
+                        if col in geometry_cols and value is not None:
+                            clob_var = oracle_cursor.var(cx_Oracle.CLOB)
+                            clob_var.setvalue(0, value)
+                            bind_row.append(clob_var)
+                            input_sizes.append(cx_Oracle.CLOB)
+                        else:
+                            bind_row.append(value)
+                            input_sizes.append(None)
+
+                    try:
+                        # Set input sizes for the row
+                        oracle_cursor.setinputsizes(*input_sizes)
+                        oracle_cursor.execute(sql_text, tuple(bind_row))
+                        rowCount += 1
+                        oracle_conn.commit()
+                        print(f'number of added rows so far> {rowCount}')
+                    except cx_Oracle.DatabaseError as e:
+                        error, = e.args
+                        print(
+                            f"Error at row {index}: Oracle-Error-Code: {error.code}, Oracle-Error-Message: {error.message}")
+                        continue
+                if len(geometry_cols) != 0:
+                    for geo_col in geometry_cols:
+                        update_sdo_srid = f'''UPDATE {table_name} T
+                                    SET T.{geo_col}.SDO_SRID = 4326
+                                    WHERE T.{geo_col} IS NOT NULL'''
+                        oracle_cursor.execute(update_sdo_srid)
+                        print(f'SDO_SRID of "{geo_col}" is updated to "4326" ')
+                    oracle_conn.commit()
                 print(
-                    f'Number of rows processed in "{table_name}": {rowCount}')
+                    f'Number of new added rows in "{table_name}": {rowCount}')
+
         except Exception as e:
-            print(f'Error during upsert: {e}')
+            print('Error during insertion')
+            print(str(e))
             raise
         finally:
-            self.engine.dispose()
+            if oracle_conn:
+                oracle_conn.close()
+                print('Oracle connection is closed!')
 
     def upsert_from_pandas_df(self, pandas_df, table_name, list_of_keys, sum_update_columns=[]):
         "connection"
-        self.dsn_tns = cx_Oracle.makedsn(
-            self.host,
-            self.port,
-            service_name=self.service_name)
 
-        oracle_conn = cx_Oracle.connect(
-            user=self.user,
-            password=self.password,
-            dsn=self.dsn_tns
-        )
         # dsn_tns = cx_Oracle.makedsn(host, port, service)
         # oracle_conn = cx_Oracle.connect(user=user, password=passwd, dsn=dsn_tns)
         "create query "
         list_of_all_columns = pandas_df.columns
         list_regular_columns = list(
             set(list_of_all_columns) - set(list_of_keys))
 
@@ -390,14 +375,19 @@
                     VALUES ({", ".join([f"s.{i}" for i in list_of_all_columns])})
         """
         # print(merge_sql)
         data_list = pandas_df.to_dict(orient='records')
         # cursor.executemany(merge_sql, data_list)
         ####
         try:
+            oracle_conn = cx_Oracle.connect(
+                user=self.user,
+                password=self.password,
+                dsn=self.dsn_tns
+            )
             with oracle_conn.cursor() as oracle_cursor:
                 rowCount = 0
                 start_pos = 0
                 batch_size = 15000
                 while start_pos < len(data_list):
                     data_ = data_list[start_pos:start_pos + batch_size]
                     start_pos += batch_size
```

### Comparing `nurtelecom_gras_library-1.3.5/src/nurtelecom_gras_library/PLSQL_geodata_importer.py` & `nurtelecom_gras_library-1.3.6/src/nurtelecom_gras_library/PLSQL_geodata_importer.py`

 * *Files identical despite different names*

### Comparing `nurtelecom_gras_library-1.3.5/src/nurtelecom_gras_library/additional_functions.py` & `nurtelecom_gras_library-1.3.6/src/nurtelecom_gras_library/additional_functions.py`

 * *Files identical despite different names*

### Comparing `nurtelecom_gras_library-1.3.5/src/nurtelecom_gras_library/updated_connection.py` & `nurtelecom_gras_library-1.3.6/src/nurtelecom_gras_library/updated_connection.py`

 * *Files identical despite different names*

### Comparing `nurtelecom_gras_library-1.3.5/src/nurtelecom_gras_library.egg-info/PKG-INFO` & `nurtelecom_gras_library-1.3.6/src/nurtelecom_gras_library.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nurtelecom_gras_library
-Version: 1.3.5
+Version: 1.3.6
 Summary: Official Nurtelecom gras library
 Home-page: https://github.com/beksultantuleev/nurtelecom_gras_library.git
 Author: Beksultan Tuleev
 Author-email: Beksultan Tuleev <kazamabeks@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Beck Kazama
@@ -36,14 +36,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Requires-Dist: cx_Oracle
 Requires-Dist: pandas
+Requires-Dist: geopandas
 Requires-Dist: sqlalchemy
 Requires-Dist: openpyxl
 Requires-Dist: tabulate
 Requires-Dist: requests
 Requires-Dist: transliterate
 
 # nurtelecom_gras_library
```

### Comparing `nurtelecom_gras_library-1.3.5/src/nurtelecom_gras_library.egg-info/SOURCES.txt` & `nurtelecom_gras_library-1.3.6/src/nurtelecom_gras_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

