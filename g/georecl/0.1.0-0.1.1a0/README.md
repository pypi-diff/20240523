# Comparing `tmp/georecl-0.1.0.tar.gz` & `tmp/georecl-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "georecl-0.1.0.tar", max compression
+gzip compressed data, was "georecl-0.1.1a0.tar", max compression
```

## Comparing `georecl-0.1.0.tar` & `georecl-0.1.1a0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-05-23 14:14:32.010214 georecl-0.1.0/georecl/__init__.py
--rw-r--r--   0        0        0     1686 2024-05-23 14:24:37.948198 georecl-0.1.0/georecl/geoserver.py
--rw-r--r--   0        0        0      333 2024-05-21 17:30:14.880592 georecl-0.1.0/georecl/main.py
--rw-r--r--   0        0        0      455 2024-05-23 14:26:54.724319 georecl-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-23 14:14:32.010214 georecl-0.1.0/README.md
--rw-r--r--   0        0        0      393 1970-01-01 00:00:00.000000 georecl-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-23 14:14:32.010214 georecl-0.1.1a0/georecl/__init__.py
+-rw-r--r--   0        0        0     1686 2024-05-23 14:24:37.948198 georecl-0.1.1a0/georecl/geoserver.py
+-rw-r--r--   0        0        0      333 2024-05-21 17:30:14.880592 georecl-0.1.1a0/georecl/main.py
+-rw-r--r--   0        0        0      457 2024-05-23 15:14:14.811827 georecl-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0      382 2024-05-23 15:03:49.287126 georecl-0.1.1a0/README.md
+-rw-r--r--   0        0        0      772 1970-01-01 00:00:00.000000 georecl-0.1.1a0/PKG-INFO
```

### Comparing `georecl-0.1.0/georecl/geoserver.py` & `georecl-0.1.1a0/georecl/geoserver.py`

 * *Files identical despite different names*

