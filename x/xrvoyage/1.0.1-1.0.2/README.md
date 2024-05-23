# Comparing `tmp/xrvoyage-1.0.1.tar.gz` & `tmp/xrvoyage-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrvoyage-1.0.1.tar", max compression
+gzip compressed data, was "xrvoyage-1.0.2.tar", max compression
```

## Comparing `xrvoyage-1.0.1.tar` & `xrvoyage-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2024-05-23 14:33:39.451999 xrvoyage-1.0.1/LICENSE
--rw-r--r--   0        0        0      444 2024-05-23 14:33:51.196142 xrvoyage-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      167 2024-05-23 14:33:39.451999 xrvoyage-1.0.1/xrvoyage/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 14:33:39.451999 xrvoyage-1.0.1/xrvoyage/handlers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 14:33:39.451999 xrvoyage-1.0.1/xrvoyage/models/__init__.py
--rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 xrvoyage-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-23 14:45:14.472273 xrvoyage-1.0.2/LICENSE
+-rw-r--r--   0        0        0      444 2024-05-23 14:45:27.264326 xrvoyage-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      107 2024-05-23 14:45:14.472273 xrvoyage-1.0.2/xrvoyage/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 14:45:14.472273 xrvoyage-1.0.2/xrvoyage/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 14:45:14.472273 xrvoyage-1.0.2/xrvoyage/models/__init__.py
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 xrvoyage-1.0.2/PKG-INFO
```

### Comparing `xrvoyage-1.0.1/LICENSE` & `xrvoyage-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xrvoyage-1.0.1/PKG-INFO` & `xrvoyage-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrvoyage
-Version: 1.0.1
+Version: 1.0.2
 Summary: XR Voyage Python Package
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```

