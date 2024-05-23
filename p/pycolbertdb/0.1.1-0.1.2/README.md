# Comparing `tmp/pycolbertdb-0.1.1.tar.gz` & `tmp/pycolbertdb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycolbertdb-0.1.1.tar", max compression
+gzip compressed data, was "pycolbertdb-0.1.2.tar", max compression
```

## Comparing `pycolbertdb-0.1.1.tar` & `pycolbertdb-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1085 2024-05-18 17:33:37.213828 pycolbertdb-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-18 17:33:37.213828 pycolbertdb-0.1.1/pycolbertdb/__init__.py
--rw-r--r--   0        0        0     9622 2024-05-18 17:33:37.213828 pycolbertdb-0.1.1/pycolbertdb/client.py
--rw-r--r--   0        0        0     2229 2024-05-18 17:33:37.213828 pycolbertdb-0.1.1/pycolbertdb/models.py
--rw-r--r--   0        0        0      518 2024-05-18 17:33:37.213828 pycolbertdb-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1666 1970-01-01 00:00:00.000000 pycolbertdb-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-05-23 12:52:20.521684 pycolbertdb-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 12:52:20.521684 pycolbertdb-0.1.2/pycolbertdb/__init__.py
+-rw-r--r--   0        0        0     9622 2024-05-23 12:52:20.521684 pycolbertdb-0.1.2/pycolbertdb/client.py
+-rw-r--r--   0        0        0     2229 2024-05-23 12:52:20.525684 pycolbertdb-0.1.2/pycolbertdb/models.py
+-rw-r--r--   0        0        0      518 2024-05-23 12:52:20.525684 pycolbertdb-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 pycolbertdb-0.1.2/PKG-INFO
```

### Comparing `pycolbertdb-0.1.1/README.md` & `pycolbertdb-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ## Installation
 ```
 pip install pycolbertdb
 ```
 
 ## Usage
 ```python
-from colbertdb import Colbertdb
+from colbertdb.client import Colbertdb
 from llama_index.readers.web import SimpleWebPageReader
 
 client = Colbertdb(url="http://localhost:8080")
 client.connect()
 
 docs = SimpleWebPageReader(html_to_text=True).load_data(
     ["https://www.radar.com/documentation/api"]
```

### Comparing `pycolbertdb-0.1.1/pycolbertdb/client.py` & `pycolbertdb-0.1.2/pycolbertdb/client.py`

 * *Files identical despite different names*

### Comparing `pycolbertdb-0.1.1/pycolbertdb/models.py` & `pycolbertdb-0.1.2/pycolbertdb/models.py`

 * *Files identical despite different names*

### Comparing `pycolbertdb-0.1.1/pyproject.toml` & `pycolbertdb-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycolbertdb"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python client for colbertdb"
 authors = ["Ryan Sloan <rysloan4@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
```

### Comparing `pycolbertdb-0.1.1/PKG-INFO` & `pycolbertdb-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycolbertdb
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python client for colbertdb
 License: MIT
 Author: Ryan Sloan
 Author-email: rysloan4@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -26,15 +26,15 @@
 ## Installation
 ```
 pip install pycolbertdb
 ```
 
 ## Usage
 ```python
-from colbertdb import Colbertdb
+from colbertdb.client import Colbertdb
 from llama_index.readers.web import SimpleWebPageReader
 
 client = Colbertdb(url="http://localhost:8080")
 client.connect()
 
 docs = SimpleWebPageReader(html_to_text=True).load_data(
     ["https://www.radar.com/documentation/api"]
```

