# Comparing `tmp/pylonparser-0.1.0.tar.gz` & `tmp/pylonparser-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylonparser-0.1.0.tar", max compression
+gzip compressed data, was "pylonparser-0.1.1.tar", max compression
```

## Comparing `pylonparser-0.1.0.tar` & `pylonparser-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2024-05-23 18:22:58.912425 pylonparser-0.1.0/LICENSE
--rw-r--r--   0        0        0      567 2024-05-23 18:16:47.772674 pylonparser-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-23 17:01:37.948193 pylonparser-0.1.0/pylonparser/__init__.py
--rw-r--r--   0        0        0     3490 2024-05-23 18:05:06.663205 pylonparser-0.1.0/pylonparser/parser.py
--rw-r--r--   0        0        0      694 2024-05-23 18:14:46.242756 pylonparser-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1438 1970-01-01 00:00:00.000000 pylonparser-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-23 18:22:58.912425 pylonparser-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1825 2024-05-23 18:42:24.501734 pylonparser-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 17:01:37.948193 pylonparser-0.1.1/pylonparser/__init__.py
+-rw-r--r--   0        0        0     3490 2024-05-23 18:05:06.663205 pylonparser-0.1.1/pylonparser/parser.py
+-rw-r--r--   0        0        0      694 2024-05-23 18:43:52.901683 pylonparser-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2696 1970-01-01 00:00:00.000000 pylonparser-0.1.1/PKG-INFO
```

### Comparing `pylonparser-0.1.0/LICENSE` & `pylonparser-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylonparser-0.1.0/pylonparser/parser.py` & `pylonparser-0.1.1/pylonparser/parser.py`

 * *Files identical despite different names*

### Comparing `pylonparser-0.1.0/pyproject.toml` & `pylonparser-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylonparser"
-version = "0.1.0"
+version = "0.1.1"
 description = "A tool to parse football game stats."
 authors = ["Your Name <your.email@example.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/traxxo/pylonparser"
 repository = "https://github.com/traxxo/pylonparser"
 documentation = "https://github.com/traxxo/pylonparser/wiki"
```

