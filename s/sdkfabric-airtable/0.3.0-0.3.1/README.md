# Comparing `tmp/sdkfabric_airtable-0.3.0.tar.gz` & `tmp/sdkfabric_airtable-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkfabric_airtable-0.3.0.tar", last modified: Sun May 19 21:53:21 2024, max compression
+gzip compressed data, was "sdkfabric_airtable-0.3.1.tar", last modified: Thu May 23 21:19:14 2024, max compression
```

## Comparing `sdkfabric_airtable-0.3.0.tar` & `sdkfabric_airtable-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:53:21.174533 sdkfabric_airtable-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-19 21:53:21.174533 sdkfabric_airtable-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 21:53:21.174533 sdkfabric_airtable-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:53:21.170533 sdkfabric_airtable-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:53:21.174533 sdkfabric_airtable-0.3.0/src/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/src/sdk/bulk_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/src/sdk/bulk_update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/src/sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/src/sdk/field.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/src/sdk/field_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/src/sdk/fields_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/src/sdk/meta_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/src/sdk/record.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/src/sdk/record_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/src/sdk/records_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/src/sdk/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:53:21.174533 sdkfabric_airtable-0.3.0/src/sdkfabric_airtable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-19 21:53:21.000000 sdkfabric_airtable-0.3.0/src/sdkfabric_airtable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-19 21:53:21.000000 sdkfabric_airtable-0.3.0/src/sdkfabric_airtable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 21:53:21.000000 sdkfabric_airtable-0.3.0/src/sdkfabric_airtable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 21:53:21.000000 sdkfabric_airtable-0.3.0/src/sdkfabric_airtable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 21:53:21.000000 sdkfabric_airtable-0.3.0/src/sdkfabric_airtable.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:19:14.414676 sdkfabric_airtable-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-23 21:19:14.414676 sdkfabric_airtable-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:19:14.414676 sdkfabric_airtable-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:19:14.406676 sdkfabric_airtable-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:19:14.410676 sdkfabric_airtable-0.3.1/src/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/bulk_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/bulk_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/field_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/fields_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/meta_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/record_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/records_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/table_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-23 21:19:07.000000 sdkfabric_airtable-0.3.1/src/sdk/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:19:14.414676 sdkfabric_airtable-0.3.1/src/sdkfabric_airtable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-23 21:19:14.000000 sdkfabric_airtable-0.3.1/src/sdkfabric_airtable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-23 21:19:14.000000 sdkfabric_airtable-0.3.1/src/sdkfabric_airtable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:19:14.000000 sdkfabric_airtable-0.3.1/src/sdkfabric_airtable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 21:19:14.000000 sdkfabric_airtable-0.3.1/src/sdkfabric_airtable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-23 21:19:14.000000 sdkfabric_airtable-0.3.1/src/sdkfabric_airtable.egg-info/top_level.txt
```

### Comparing `sdkfabric_airtable-0.3.0/LICENSE` & `sdkfabric_airtable-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.3.0/PKG-INFO` & `sdkfabric_airtable-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-airtable
-Version: 0.3.0
+Version: 0.3.1
 Summary: Airtable Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/airtable-python
 Project-URL: Issues, https://github.com/sdk-fabric/airtable-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkfabric_airtable-0.3.0/README.md` & `sdkfabric_airtable-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.3.0/pyproject.toml` & `sdkfabric_airtable-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sdkfabric-airtable"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "Airtable Python SDK managed by SDK Fabric"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `sdkfabric_airtable-0.3.0/src/sdk/bulk_update_request.py` & `sdkfabric_airtable-0.3.1/src/sdk/bulk_update_request.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.3.0/src/sdk/bulk_update_response.py` & `sdkfabric_airtable-0.3.1/src/sdk/bulk_update_response.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.3.0/src/sdk/client.py` & `sdkfabric_airtable-0.3.1/src/sdk/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import sdkgen
 from requests import RequestException
 from typing import List
 
 from .meta_tag import MetaTag
 from .records_tag import RecordsTag
 from .fields_tag import FieldsTag
+from .table_tag import TableTag
 
 class Client(sdkgen.ClientAbstract):
     def __init__(self, base_url: str, credentials: sdkgen.CredentialsInterface):
         super().__init__(base_url, credentials)
 
     def meta(self) -> MetaTag:
         return MetaTag(
@@ -30,13 +31,19 @@
 
     def fields(self) -> FieldsTag:
         return FieldsTag(
             self.http_client,
             self.parser
         )
 
+    def table(self) -> TableTag:
+        return TableTag(
+            self.http_client,
+            self.parser
+        )
+
 
 
     @staticmethod
     def build(token: str):
         return Client("https://api.airtable.com/", sdkgen.HttpBearer(token))
```

### Comparing `sdkfabric_airtable-0.3.0/src/sdk/field.py` & `sdkfabric_airtable-0.3.1/src/sdk/field.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.3.0/src/sdk/field_options.py` & `sdkfabric_airtable-0.3.1/src/sdk/field_options.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.3.0/src/sdk/fields_tag.py` & `sdkfabric_airtable-0.3.1/src/sdk/fields_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.3.0/src/sdk/meta_tag.py` & `sdkfabric_airtable-0.3.1/src/sdk/meta_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.3.0/src/sdk/record.py` & `sdkfabric_airtable-0.3.1/src/sdk/record.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.3.0/src/sdk/records_tag.py` & `sdkfabric_airtable-0.3.1/src/sdk/records_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.3.0/src/sdkfabric_airtable.egg-info/PKG-INFO` & `sdkfabric_airtable-0.3.1/src/sdkfabric_airtable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-airtable
-Version: 0.3.0
+Version: 0.3.1
 Summary: Airtable Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/airtable-python
 Project-URL: Issues, https://github.com/sdk-fabric/airtable-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkfabric_airtable-0.3.0/src/sdkfabric_airtable.egg-info/SOURCES.txt` & `sdkfabric_airtable-0.3.1/src/sdkfabric_airtable.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,13 +8,15 @@
 src/sdk/field.py
 src/sdk/field_options.py
 src/sdk/fields_tag.py
 src/sdk/meta_tag.py
 src/sdk/record.py
 src/sdk/record_collection.py
 src/sdk/records_tag.py
+src/sdk/table.py
+src/sdk/table_tag.py
 src/sdk/user.py
 src/sdkfabric_airtable.egg-info/PKG-INFO
 src/sdkfabric_airtable.egg-info/SOURCES.txt
 src/sdkfabric_airtable.egg-info/dependency_links.txt
 src/sdkfabric_airtable.egg-info/requires.txt
 src/sdkfabric_airtable.egg-info/top_level.txt
```

