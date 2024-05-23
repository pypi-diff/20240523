# Comparing `tmp/llama_index_tools_cassandra-0.1.0.tar.gz` & `tmp/llama_index_tools_cassandra-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_tools_cassandra-0.1.0.tar", max compression
+gzip compressed data, was "llama_index_tools_cassandra-0.1.1.tar", max compression
```

## Comparing `llama_index_tools_cassandra-0.1.0.tar` & `llama_index_tools_cassandra-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2354 2024-05-22 00:56:40.041637 llama_index_tools_cassandra-0.1.0/README.md
--rw-r--r--   0        0        0       17 2024-05-22 00:56:40.041637 llama_index_tools_cassandra-0.1.0/llama_index/tools/cassandra/BUILD
--rw-r--r--   0        0        0      113 2024-05-22 00:56:40.041637 llama_index_tools_cassandra-0.1.0/llama_index/tools/cassandra/__init__.py
--rw-r--r--   0        0        0     3103 2024-05-22 00:56:40.041637 llama_index_tools_cassandra-0.1.0/llama_index/tools/cassandra/base.py
--rw-r--r--   0        0        0    24546 2024-05-22 00:56:40.041637 llama_index_tools_cassandra-0.1.0/llama_index/tools/cassandra/cassandra_database_wrapper.py
--rw-r--r--   0        0        0     1418 2024-05-22 00:56:40.041637 llama_index_tools_cassandra-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2968 1970-01-01 00:00:00.000000 llama_index_tools_cassandra-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2354 2024-05-23 15:33:20.448286 llama_index_tools_cassandra-0.1.1/README.md
+-rw-r--r--   0        0        0       17 2024-05-23 15:33:20.448286 llama_index_tools_cassandra-0.1.1/llama_index/tools/cassandra/BUILD
+-rw-r--r--   0        0        0      113 2024-05-23 15:33:20.448286 llama_index_tools_cassandra-0.1.1/llama_index/tools/cassandra/__init__.py
+-rw-r--r--   0        0        0     3055 2024-05-23 15:33:20.448286 llama_index_tools_cassandra-0.1.1/llama_index/tools/cassandra/base.py
+-rw-r--r--   0        0        0    24853 2024-05-23 15:33:20.448286 llama_index_tools_cassandra-0.1.1/llama_index/tools/cassandra/cassandra_database_wrapper.py
+-rw-r--r--   0        0        0     1418 2024-05-23 15:33:20.448286 llama_index_tools_cassandra-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2968 1970-01-01 00:00:00.000000 llama_index_tools_cassandra-0.1.1/PKG-INFO
```

### Comparing `llama_index_tools_cassandra-0.1.0/README.md` & `llama_index_tools_cassandra-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,8 +34,8 @@
 
 - **`cassandra_db_schema`**: Fetches schema information, essential for the agent’s operation.
 - **`cassandra_db_select_table_data`**: Allows selection of data from a specific keyspace and table.
 - **`cassandra_db_query`**: An experimental tool that accepts fully formed query strings from the agent.
 
 ## Example Usage
 
-Initialize the CassandraDatabase and set up the agent with the tools provided. Query the database by interacting with the agent as shown in the example [notebook](https://docs.llamaindex.ai/en/latest/examples/tools/cassandra/).
+Initialize the CassandraDatabase and set up the agent with the tools provided. Query the database by interacting with the agent as shown in the example [notebook](https://docs.llamaindex.ai/en/stable/examples/tools/cassandra/).
```

### Comparing `llama_index_tools_cassandra-0.1.0/llama_index/tools/cassandra/base.py` & `llama_index_tools_cassandra-0.1.1/llama_index/tools/cassandra/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
         Args:
             keyspace (str): The name of the keyspace for which to return the schema.
 
         Returns:
             List[Document]: A list of Document objects, each containing a table description.
         """
-        return [Document(text=self.db.get_keyspace_tables_str_no_throw(keyspace))]
+        return [Document(text=self.db.get_keyspace_tables_str(keyspace))]
 
     def cassandra_db_select_table_data(
         self, keyspace: str, table: str, predicate: str, limit: int
     ) -> List[Document]:
         """Tool for getting data from a table in an Apache Cassandra database.
             Use the WHERE clause to specify the predicate for the query that uses the
             primary key. A blank predicate will return all rows. Avoid this if possible.
@@ -71,11 +71,9 @@
             predicate (str): The predicate for the query that uses the primary key.
             limit (int): The maximum number of rows to return.
 
         Returns:
             List[Document]: A list of Document objects, each containing a row of data.
         """
         return [
-            Document(
-                text=self.db.get_table_data_no_throw(keyspace, table, predicate, limit)
-            )
+            Document(text=self.db.get_table_data(keyspace, table, predicate, limit))
         ]
```

### Comparing `llama_index_tools_cassandra-0.1.0/llama_index/tools/cassandra/cassandra_database_wrapper.py` & `llama_index_tools_cassandra-0.1.1/llama_index/tools/cassandra/cassandra_database_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,29 +38,40 @@
         self._exclude_tables = exclude_tables or []
         self._include_tables = include_tables or []
 
     def run(
         self,
         query: str,
         fetch: str = "all",
-        include_columns: bool = False,
         **kwargs: Any,
     ) -> Union[str, Sequence[Dict[str, Any]], ResultSet]:
         """Execute a CQL query and return the results."""
         clean_query = self._validate_cql(query, "SELECT")
         result = self._session.execute(clean_query, **kwargs)
         if fetch == "all":
             return list(result)
         elif fetch == "one":
             return result.one()._asdict() if result else {}
         elif fetch == "cursor":
             return result
         else:
             raise ValueError("Fetch parameter must be either 'one', 'all', or 'cursor'")
 
+    def run_no_throw(
+        self,
+        query: str,
+        fetch: str = "all",
+        **kwargs: Any,
+    ) -> Union[str, Sequence[Dict[str, Any]], ResultSet]:
+        """Execute a CQL query and return the results."""
+        try:
+            return self.run(query, fetch, **kwargs)
+        except Exception as e:
+            return str(e)
+
     def get_keyspace_tables_str(self, keyspace: str) -> str:
         """Get the tables for the specified keyspace."""
         try:
             tables = self.get_keyspace_tables(keyspace)
             schema_string = ""
             for table in tables:
                 schema_string += table.as_markdown() + "\n\n"
```

### Comparing `llama_index_tools_cassandra-0.1.0/pyproject.toml` & `llama_index_tools_cassandra-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Patrick McFadin <patrick@datastax.com>"]
 description = "llama-index tools Apache Cassandra® integration"
 license = "MIT"
 name = "llama-index-tools-cassandra"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.0"
 cassio = "^0.1.7"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_tools_cassandra-0.1.0/PKG-INFO` & `llama_index_tools_cassandra-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-tools-cassandra
-Version: 0.1.0
+Version: 0.1.1
 Summary: llama-index tools Apache Cassandra® integration
 License: MIT
 Author: Patrick McFadin
 Author-email: patrick@datastax.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -51,9 +51,9 @@
 
 - **`cassandra_db_schema`**: Fetches schema information, essential for the agent’s operation.
 - **`cassandra_db_select_table_data`**: Allows selection of data from a specific keyspace and table.
 - **`cassandra_db_query`**: An experimental tool that accepts fully formed query strings from the agent.
 
 ## Example Usage
 
-Initialize the CassandraDatabase and set up the agent with the tools provided. Query the database by interacting with the agent as shown in the example [notebook](https://docs.llamaindex.ai/en/latest/examples/tools/cassandra/).
+Initialize the CassandraDatabase and set up the agent with the tools provided. Query the database by interacting with the agent as shown in the example [notebook](https://docs.llamaindex.ai/en/stable/examples/tools/cassandra/).
```

