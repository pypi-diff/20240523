# Comparing `tmp/pgscatalog_utils-1.0.1.tar.gz` & `tmp/pgscatalog_utils-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgscatalog_utils-1.0.1.tar", max compression
+gzip compressed data, was "pgscatalog_utils-1.0.2.tar", max compression
```

## Comparing `pgscatalog_utils-1.0.1.tar` & `pgscatalog_utils-1.0.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2171 2024-04-09 09:33:40.152724 pgscatalog_utils-1.0.1/README.md
--rw-r--r--   0        0        0      593 2024-04-09 09:33:40.152724 pgscatalog_utils-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       92 2024-04-09 09:33:40.152724 pgscatalog_utils-1.0.1/src/pgscatalog/utils/__init__.py
--rw-r--r--   0        0        0     2812 1970-01-01 00:00:00.000000 pgscatalog_utils-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2171 2024-05-23 15:24:34.253965 pgscatalog_utils-1.0.2/README.md
+-rw-r--r--   0        0        0      593 2024-05-23 15:24:34.253965 pgscatalog_utils-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      110 2024-05-23 15:24:34.253965 pgscatalog_utils-1.0.2/src/pgscatalog/utils/__init__.py
+-rw-r--r--   0        0        0     2812 1970-01-01 00:00:00.000000 pgscatalog_utils-1.0.2/PKG-INFO
```

### Comparing `pgscatalog_utils-1.0.1/README.md` & `pgscatalog_utils-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pgscatalog_utils-1.0.1/pyproject.toml` & `pgscatalog_utils-1.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "pgscatalog-utils"
-version = "1.0.1"
+version = "1.0.2"
 description = "Utilities for working with PGS Catalog API and scoring files"
 authors = ["Benjamin Wingfield <bwingfield@ebi.ac.uk>", "Samuel Lambert <sl925@medschl.cam.ac.uk>", "Laurent Gil <lg10@sanger.ac.uk>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "pgscatalog", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-"pgscatalog.calc" = "^0.1.0"
-"pgscatalog.core" = "^0.1.1"
-"pgscatalog.match" = "^0.1.0"
+"pgscatalog.calc" = "^0.1.1"
+"pgscatalog.core" = "^0.1.2"
+"pgscatalog.match" = "^0.1.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pgscatalog_utils-1.0.1/PKG-INFO` & `pgscatalog_utils-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pgscatalog-utils
-Version: 1.0.1
+Version: 1.0.2
 Summary: Utilities for working with PGS Catalog API and scoring files
 License: Apache-2.0
 Author: Benjamin Wingfield
 Author-email: bwingfield@ebi.ac.uk
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pgscatalog.calc (>=0.1.0,<0.2.0)
-Requires-Dist: pgscatalog.core (>=0.1.1,<0.2.0)
-Requires-Dist: pgscatalog.match (>=0.1.0,<0.2.0)
+Requires-Dist: pgscatalog.calc (>=0.1.1,<0.2.0)
+Requires-Dist: pgscatalog.core (>=0.1.2,<0.2.0)
+Requires-Dist: pgscatalog.match (>=0.1.1,<0.2.0)
 Description-Content-Type: text/markdown
 
 # `pgscatalog-utils`
 
 This convenience package bundles every PGS Catalog application, including:
 
 | Application                  | Description                                                            | Link                                                                                |
```

