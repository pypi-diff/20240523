# Comparing `tmp/gritql-0.1.0.tar.gz` & `tmp/gritql-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gritql-0.1.0.tar", max compression
+gzip compressed data, was "gritql-0.1.1.tar", max compression
```

## Comparing `gritql-0.1.0.tar` & `gritql-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      840 2024-05-22 23:23:34.117195 gritql-0.1.0/README.md
--rw-r--r--   0        0        0      179 2024-05-19 05:47:58.201419 gritql-0.1.0/gritql/README.md
--rw-r--r--   0        0        0        0 2024-05-19 05:47:58.201448 gritql-0.1.0/gritql/__init__.py
--rw-r--r--   0        0        0     3795 2024-05-19 08:35:11.769286 gritql-0.1.0/gritql/installer.py
--rw-r--r--   0        0        0       31 2024-05-19 05:47:58.201875 gritql-0.1.0/gritql/requirements.txt
--rw-r--r--   0        0        0      624 2024-05-19 08:36:12.951556 gritql-0.1.0/gritql/run.py
--rw-r--r--   0        0        0      554 2024-05-22 23:22:56.238150 gritql-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 gritql-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      840 2024-05-22 23:23:34.117195 gritql-0.1.1/README.md
+-rw-r--r--   0        0        0      179 2024-05-19 05:47:58.201419 gritql-0.1.1/gritql/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 05:47:58.201448 gritql-0.1.1/gritql/__init__.py
+-rw-r--r--   0        0        0     3795 2024-05-19 08:35:11.769286 gritql-0.1.1/gritql/installer.py
+-rw-r--r--   0        0        0       31 2024-05-19 05:47:58.201875 gritql-0.1.1/gritql/requirements.txt
+-rw-r--r--   0        0        0      624 2024-05-19 08:36:12.951556 gritql-0.1.1/gritql/run.py
+-rw-r--r--   0        0        0      554 2024-05-22 23:31:21.155657 gritql-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1407 1970-01-01 00:00:00.000000 gritql-0.1.1/PKG-INFO
```

### Comparing `gritql-0.1.0/README.md` & `gritql-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gritql-0.1.0/gritql/installer.py` & `gritql-0.1.1/gritql/installer.py`

 * *Files identical despite different names*

### Comparing `gritql-0.1.0/gritql/run.py` & `gritql-0.1.1/gritql/run.py`

 * *Files identical despite different names*

### Comparing `gritql-0.1.0/pyproject.toml` & `gritql-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,20 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 version = "0.1.0"
 
 [tool.poetry]
 name = "gritql"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python bindings for GritQL"
 authors = ["Grit <developers@grit.io>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gritql-0.1.0/PKG-INFO` & `gritql-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: gritql
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python bindings for GritQL
 License: MIT
 Author: Grit
 Author-email: developers@grit.io
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 GritQL is a declarative query language for searching and modifying source code.
```

