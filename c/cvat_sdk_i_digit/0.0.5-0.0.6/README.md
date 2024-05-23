# Comparing `tmp/cvat_sdk_i_digit-0.0.5.tar.gz` & `tmp/cvat_sdk_i_digit-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvat_sdk_i_digit-0.0.5.tar", last modified: Thu May 23 03:33:00 2024, max compression
+gzip compressed data, was "cvat_sdk_i_digit-0.0.6.tar", last modified: Thu May 23 03:39:50 2024, max compression
```

## Comparing `cvat_sdk_i_digit-0.0.5.tar` & `cvat_sdk_i_digit-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1073 2024-05-23 02:59:28.391193 cvat_sdk_i_digit-0.0.5/LICENSE
--rw-r--r--   0        0        0     1599 2024-05-23 03:32:20.586871 cvat_sdk_i_digit-0.0.5/README.md
--rw-r--r--   0        0        0      658 2024-05-23 03:33:00.435335 cvat_sdk_i_digit-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-22 11:19:44.471973 cvat_sdk_i_digit-0.0.5/src/cvat_sdk_i_digit/__init__.py
--rw-r--r--   0        0        0     6031 2024-05-23 03:06:00.080006 cvat_sdk_i_digit-0.0.5/src/cvat_sdk_i_digit/config.py
--rw-r--r--   0        0        0     3499 2024-05-23 03:18:38.841234 cvat_sdk_i_digit-0.0.5/src/cvat_sdk_i_digit/cvat_api.py
--rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 cvat_sdk_i_digit-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-23 02:59:28.391193 cvat_sdk_i_digit-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1599 2024-05-23 03:32:20.586871 cvat_sdk_i_digit-0.0.6/README.md
+-rw-r--r--   0        0        0     1599 2024-05-23 03:32:20.586871 cvat_sdk_i_digit-0.0.6/README.md
+-rw-r--r--   0        0        0      679 2024-05-23 03:39:50.535889 cvat_sdk_i_digit-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-22 11:19:44.471973 cvat_sdk_i_digit-0.0.6/src/cvat_sdk_i_digit/__init__.py
+-rw-r--r--   0        0        0     6031 2024-05-23 03:06:00.080006 cvat_sdk_i_digit-0.0.6/src/cvat_sdk_i_digit/config.py
+-rw-r--r--   0        0        0     3499 2024-05-23 03:18:38.841234 cvat_sdk_i_digit-0.0.6/src/cvat_sdk_i_digit/cvat_api.py
+-rw-r--r--   0        0        0     1968 1970-01-01 00:00:00.000000 cvat_sdk_i_digit-0.0.6/PKG-INFO
```

### Comparing `cvat_sdk_i_digit-0.0.5/LICENSE` & `cvat_sdk_i_digit-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cvat_sdk_i_digit-0.0.5/README.md` & `cvat_sdk_i_digit-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cvat_sdk_i_digit-0.0.5/pyproject.toml` & `cvat_sdk_i_digit-0.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [project]
 name = "cvat_sdk_i_digit"
-version = "0.0.5"
+version = "0.0.6"
 description = ""
 authors = [
     { name = "Шумелев Дмитрий Игоревич", email = "cmit.dima@gmail.com" },
 ]
+readme = "README.md"
 dependencies = [
     "cvat-sdk>=2.13.0",
     "pydantic-settings>=2.0.2",
     "passlib>=1.7.4",
     "pandas>=2.2.2",
 ]
 requires-python = ">=3.11"
```

### Comparing `cvat_sdk_i_digit-0.0.5/src/cvat_sdk_i_digit/config.py` & `cvat_sdk_i_digit-0.0.6/src/cvat_sdk_i_digit/config.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk_i_digit-0.0.5/src/cvat_sdk_i_digit/cvat_api.py` & `cvat_sdk_i_digit-0.0.6/src/cvat_sdk_i_digit/cvat_api.py`

 * *Files identical despite different names*

