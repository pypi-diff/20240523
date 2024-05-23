# Comparing `tmp/s3_reader-0.3.1.tar.gz` & `tmp/s3_reader-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3_reader-0.3.1.tar", max compression
+gzip compressed data, was "s3_reader-0.3.2.tar", max compression
```

## Comparing `s3_reader-0.3.1.tar` & `s3_reader-0.3.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0    11337 2023-09-23 03:40:43.847301 s3_reader-0.3.1/LICENSE
--rw-r--r--   0        0        0     1073 2023-12-26 08:59:47.832085 s3_reader-0.3.1/README.md
--rw-r--r--   0        0        0     2010 2024-05-13 05:20:42.009595 s3_reader-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       95 2023-09-23 03:40:43.848692 s3_reader-0.3.1/src/s3_reader/__init__.py
--rw-r--r--   0        0        0       93 2023-09-23 03:40:43.848794 s3_reader-0.3.1/src/s3_reader/__version__.py
--rw-r--r--   0        0        0     4652 2024-05-13 05:19:51.935652 s3_reader-0.3.1/src/s3_reader/file.py
--rw-r--r--   0        0        0     1785 1970-01-01 00:00:00.000000 s3_reader-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-09-23 03:40:43.847301 s3_reader-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1073 2023-12-26 08:59:47.832085 s3_reader-0.3.2/README.md
+-rw-r--r--   0        0        0     2010 2024-05-23 00:38:33.122938 s3_reader-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0       95 2023-09-23 03:40:43.848692 s3_reader-0.3.2/src/s3_reader/__init__.py
+-rw-r--r--   0        0        0       93 2023-09-23 03:40:43.848794 s3_reader-0.3.2/src/s3_reader/__version__.py
+-rw-r--r--   0        0        0     4652 2024-05-13 05:19:51.935652 s3_reader-0.3.2/src/s3_reader/file.py
+-rw-r--r--   0        0        0        0 2024-05-23 00:37:55.574019 s3_reader-0.3.2/src/s3_reader/py.typed
+-rw-r--r--   0        0        0     1785 1970-01-01 00:00:00.000000 s3_reader-0.3.2/PKG-INFO
```

### Comparing `s3_reader-0.3.1/LICENSE` & `s3_reader-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `s3_reader-0.3.1/README.md` & `s3_reader-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `s3_reader-0.3.1/pyproject.toml` & `s3_reader-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "s3-reader"
-version = "0.3.1"
+version = "0.3.2"
 description = "Python library to read S3 file as local file."
 authors = ["rcmdnk <rcmdnk@gmail.com>"]
 repository = "https://github.com/rcmdnk/s3-reader"
 homepage = "https://github.com/rcmdnk/s3-reader"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = []
```

### Comparing `s3_reader-0.3.1/src/s3_reader/file.py` & `s3_reader-0.3.2/src/s3_reader/file.py`

 * *Files identical despite different names*

### Comparing `s3_reader-0.3.1/PKG-INFO` & `s3_reader-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3-reader
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python library to read S3 file as local file.
 Home-page: https://github.com/rcmdnk/s3-reader
 License: Apache-2.0
 Author: rcmdnk
 Author-email: rcmdnk@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

