# Comparing `tmp/inherit_docstring-0.1.3.tar.gz` & `tmp/inherit_docstring-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inherit_docstring-0.1.3.tar", max compression
+gzip compressed data, was "inherit_docstring-0.1.4.tar", max compression
```

## Comparing `inherit_docstring-0.1.3.tar` & `inherit_docstring-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11337 2023-10-29 06:52:59.111205 inherit_docstring-0.1.3/LICENSE
--rw-r--r--   0        0        0     4103 2023-11-08 17:46:12.224793 inherit_docstring-0.1.3/README.md
--rw-r--r--   0        0        0     2497 2023-11-21 02:59:20.397949 inherit_docstring-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      126 2023-10-29 11:10:11.723063 inherit_docstring-0.1.3/src/inherit_docstring/__init__.py
--rw-r--r--   0        0        0       93 2023-10-29 06:34:23.099244 inherit_docstring-0.1.3/src/inherit_docstring/__version__.py
--rw-r--r--   0        0        0      862 2023-11-08 03:17:51.815215 inherit_docstring-0.1.3/src/inherit_docstring/decorator.py
--rw-r--r--   0        0        0     4356 2023-11-21 02:59:20.393288 inherit_docstring-0.1.3/src/inherit_docstring/utils.py
--rw-r--r--   0        0        0     5122 1970-01-01 00:00:00.000000 inherit_docstring-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-10-29 06:52:59.111205 inherit_docstring-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4103 2023-11-08 17:46:12.224793 inherit_docstring-0.1.4/README.md
+-rw-r--r--   0        0        0     2497 2024-05-22 23:47:18.533120 inherit_docstring-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      126 2023-10-29 11:10:11.723063 inherit_docstring-0.1.4/src/inherit_docstring/__init__.py
+-rw-r--r--   0        0        0       93 2023-10-29 06:34:23.099244 inherit_docstring-0.1.4/src/inherit_docstring/__version__.py
+-rw-r--r--   0        0        0      862 2023-11-08 03:17:51.815215 inherit_docstring-0.1.4/src/inherit_docstring/decorator.py
+-rw-r--r--   0        0        0        0 2024-05-22 23:45:09.802788 inherit_docstring-0.1.4/src/inherit_docstring/py.typed
+-rw-r--r--   0        0        0     4356 2023-11-21 02:59:20.393288 inherit_docstring-0.1.4/src/inherit_docstring/utils.py
+-rw-r--r--   0        0        0     5122 1970-01-01 00:00:00.000000 inherit_docstring-0.1.4/PKG-INFO
```

### Comparing `inherit_docstring-0.1.3/LICENSE` & `inherit_docstring-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `inherit_docstring-0.1.3/README.md` & `inherit_docstring-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `inherit_docstring-0.1.3/pyproject.toml` & `inherit_docstring-0.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inherit-docstring"
-version = "0.1.3"
+version = "0.1.4"
 description = "A python decorator to inherit docstring."
 authors = ["rcmdnk <rcmdnk@gmail.com>"]
 repository = "https://github.com/rcmdnk/inherit-docstring"
 homepage = "https://github.com/rcmdnk/inherit-docstring"
 readme = "README.md"
 license = "apache-2.0"
 keywords = ["docstring", "inherit", "decorator"]
```

### Comparing `inherit_docstring-0.1.3/src/inherit_docstring/decorator.py` & `inherit_docstring-0.1.4/src/inherit_docstring/decorator.py`

 * *Files identical despite different names*

### Comparing `inherit_docstring-0.1.3/src/inherit_docstring/utils.py` & `inherit_docstring-0.1.4/src/inherit_docstring/utils.py`

 * *Files identical despite different names*

### Comparing `inherit_docstring-0.1.3/PKG-INFO` & `inherit_docstring-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inherit-docstring
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python decorator to inherit docstring.
 Home-page: https://github.com/rcmdnk/inherit-docstring
 License: Apache-2.0
 Keywords: docstring,inherit,decorator
 Author: rcmdnk
 Author-email: rcmdnk@gmail.com
 Requires-Python: >=3.9,<4.0
```

