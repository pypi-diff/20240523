# Comparing `tmp/lazy_schema-0.2.6.tar.gz` & `tmp/lazy_schema-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_schema-0.2.6.tar", max compression
+gzip compressed data, was "lazy_schema-0.3.0.tar", max compression
```

## Comparing `lazy_schema-0.2.6.tar` & `lazy_schema-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2948 2024-03-08 00:37:24.160180 lazy_schema-0.2.6/README.md
--rw-r--r--   0        0        0       71 2024-04-16 07:03:59.348863 lazy_schema-0.2.6/lazy_schema/__init__.py
--rw-r--r--   0        0        0     5028 2024-04-17 00:36:54.834012 lazy_schema-0.2.6/lazy_schema/schema.py
--rw-r--r--   0        0        0     2509 2024-04-16 08:27:40.001220 lazy_schema-0.2.6/lazy_schema/schema_pool.py
--rw-r--r--   0        0        0      278 2024-04-17 00:37:06.926692 lazy_schema-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     3447 1970-01-01 00:00:00.000000 lazy_schema-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     4137 2024-05-23 01:52:28.879909 lazy_schema-0.3.0/README.md
+-rw-r--r--   0        0        0       71 2024-05-23 01:52:28.619910 lazy_schema-0.3.0/lazy_schema/__init__.py
+-rw-r--r--   0        0        0     5229 2024-05-23 01:52:28.619910 lazy_schema-0.3.0/lazy_schema/schema.py
+-rw-r--r--   0        0        0     2669 2024-05-23 01:52:28.619910 lazy_schema-0.3.0/lazy_schema/schema_pool.py
+-rw-r--r--   0        0        0      278 2024-05-23 01:52:28.855909 lazy_schema-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4636 1970-01-01 00:00:00.000000 lazy_schema-0.3.0/PKG-INFO
```

### Comparing `lazy_schema-0.2.6/lazy_schema/schema.py` & `lazy_schema-0.3.0/lazy_schema/schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import json
-from typing import Any, NamedTuple, Union, Dict
+from typing import Any, NamedTuple, Union, Dict, TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from schema_pool import SchemaPool
 
 
 def _null_coalesce(*args):
     for arg in args:
         if arg != None:
             return arg
 
@@ -81,14 +84,21 @@
                 if not __no_null__ or value != None:
                     result[key] = value
             else:
                 raise Exception(f"Key '{key}' does not exist!")
 
         return result
 
+    def add_to(
+        self,
+        name: str,
+        pool: "SchemaPool",
+    ):
+        return pool.add_schema(name, self)
+
     @staticmethod
     def new(
         *args: Union[str, dict],
         __discrete__=False,
         __no_default__=False,
         __no_null__=False,
         **kwargs,
```

### Comparing `lazy_schema-0.2.6/lazy_schema/schema_pool.py` & `lazy_schema-0.3.0/lazy_schema/schema_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,61 +25,69 @@
 
     def __getitem__(self, key: str) -> Schema:
         raise Exception(f"Schema '{key}' does not exist!")
 
     def pymongo(
         self,
         mongo_collection,
-        name: str,
+        field_value: str,
         field_name="__name__",
         *args: Union[str, dict],
         __discrete__=False,
         __no_default__=False,
         __no_null__=False,
         **kwargs,
     ):
         return self.pymongo_query(
             mongo_collection,
-            name,
             {
-                field_name: name,
+                field_name: field_value,
             },
             *args,
             __discrete__=__discrete__,
             __no_default__=__no_default__,
             __no_null__=__no_null__,
             **kwargs,
         )
 
     def pymongo_query(
         self,
         mongo_collection,
-        name: str,
         query,
         *args: Union[str, dict],
         __discrete__=False,
         __no_default__=False,
         __no_null__=False,
         **kwargs,
     ):
         document = _load_document(mongo_collection, query)
 
         if document == None:
-            raise Exception(f"Failed to retrieve schema '{name}'!")
+            raise Exception(
+                f"Failed to retrieve schema from MongoDB!",
+            )
 
-        return self.set(
-            name,
+        return Schema.new(
             document,
             *args,
             __discrete__=__discrete__,
             __no_default__=__no_default__,
             __no_null__=__no_null__,
             **kwargs,
         )
 
+    def add_schema(
+        self,
+        name: str,
+        schema: Schema,
+    ):
+        setattr(self, name, schema)
+
+        return schema
+
     def set(
         self,
         name: str,
         *args: Union[str, dict],
         __discrete__=False,
         __no_default__=False,
         __no_null__=False,
@@ -88,18 +96,17 @@
         """
         :__discrete__: When `true`, excludes fields with a `null` default value. Explicitly setting the value to `null` will include it.
 
         :__no_default__: When `true`, default values are excluded.
 
         :__no_null__: When `true`, `null` values will never be included.
         """
-        schema = Schema.new(
-            *args,
-            __discrete__=__discrete__,
-            __no_default__=__no_default__,
-            __no_null__=__no_null__,
-            **kwargs,
+        return self.add_schema(
+            name,
+            Schema.new(
+                *args,
+                __discrete__=__discrete__,
+                __no_default__=__no_default__,
+                __no_null__=__no_null__,
+                **kwargs,
+            ),
         )
-
-        setattr(self, name, schema)
-
-        return schema
```

### Comparing `lazy_schema-0.2.6/PKG-INFO` & `lazy_schema-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,21 @@
-Metadata-Version: 2.1
-Name: lazy-schema
-Version: 0.2.6
-Summary: 
-Author: MisterNyan
-Author-email: michael.edmund.wong@gmail.com
-Requires-Python: >=3.8,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-
 # Lazy Schema
 Quick and simple schema validator.
 
 # Installation
 ```
 pip install lazy-schema
 ```
 
 # How to Use
 
 ```py
 from lazy_schema import schema
 from datetime import datetime
+from bson import ObjectId
 
 exampleSchema = schema(
     stringField="Hello World!",
     numberField=123,
     booleanField=True,
     lambdaField=lambda: datetime.utcnow(),
 )
@@ -76,14 +62,101 @@
     "stringField": "Hi World!",
     "numberField": 123,
     "booleanField": True,
     "lambdaField": [datetime Object]
 }
 ```
 
+## SchemaPool
+
+Just a collection where you can keep all your schemas.
+
+```py
+from lazy_schema import SchemaPool
+
+schemas = SchemaPool()
+
+schemas.set(
+    "my_schema",
+    hello="world!",
+    number=123,
+)
+
+schemas.set(
+    "my_other_schema",
+    hello="there!",
+    number=456,
+)
+
+print(schemas.my_schema())
+print(schemas.my_other_schema())
+```
+
+```json
+{
+    "hello": "world!",
+    "number": 123
+}
+
+{
+    "hello": "there!",
+    "number": 456
+}
+```
+
+## Loading from MongoDB with SchemaPool
+
+You can load MongoDB documents with `SchemaPool`!
+
+### MongoDB Document
+```json
+{
+    "_id": [ObjectId],
+    "__im_a_comment__": null,
+    "hello": "world!",
+    "number": 123
+}
+```
+
+### Script
+```py
+from pymongo import MongoClient
+from lazy_schema import SchemaPool
+
+mongo = MongoClient(...)
+collection = mongo.my_database.my_schemas
+
+schemas = SchemaPool()
+
+schema = schemas.pymongo(
+    collection,
+    query={
+        "_id": ObjectId(...),
+    },
+)
+
+print(schema())
+```
+
+### Result
+```json
+{
+    // `_id` is always excluded.
+    "hello": "world!",
+    "number": 123
+}
+```
+
+You can also add it into the `SchemaPool`.
+
+```py
+...
+schema.add_to("my_schema", schemas)
+```
+
 ## Special Keywords
 
 Field names that are enclosed with double underscores `_`
 are special keywords.
 They are not included in the schema.
 
 These can be used when creating a schema,
@@ -208,8 +281,8 @@
 ```
 ```
 {
     "fieldA": "Hello World!",
     "fieldB": None,
     "fieldC": "Hi World!"
 }
-```
+```
```

