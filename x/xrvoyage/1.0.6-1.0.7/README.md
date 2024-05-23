# Comparing `tmp/xrvoyage-1.0.6.tar.gz` & `tmp/xrvoyage-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrvoyage-1.0.6.tar", max compression
+gzip compressed data, was "xrvoyage-1.0.7.tar", max compression
```

## Comparing `xrvoyage-1.0.6.tar` & `xrvoyage-1.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2024-05-23 15:06:22.447919 xrvoyage-1.0.6/LICENSE
--rw-r--r--   0        0        0      444 2024-05-23 15:06:48.083930 xrvoyage-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      107 2024-05-23 15:06:22.447919 xrvoyage-1.0.6/xrvoyage/__init__.py
--rw-r--r--   0        0        0       40 2024-05-23 15:06:52.039932 xrvoyage-1.0.6/xrvoyage/_version.py
--rw-r--r--   0        0        0        0 2024-05-23 15:06:22.447919 xrvoyage-1.0.6/xrvoyage/handlers/__init__.py
--rw-r--r--   0        0        0      209 2024-05-23 15:06:22.447919 xrvoyage-1.0.6/xrvoyage/handlers/static.py
--rw-r--r--   0        0        0        0 2024-05-23 15:06:22.447919 xrvoyage-1.0.6/xrvoyage/models/__init__.py
--rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 xrvoyage-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-23 15:14:44.783079 xrvoyage-1.0.7/LICENSE
+-rw-r--r--   0        0        0      444 2024-05-23 15:14:56.427133 xrvoyage-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      107 2024-05-23 15:14:44.783079 xrvoyage-1.0.7/xrvoyage/__init__.py
+-rw-r--r--   0        0        0       18 2024-05-23 15:14:56.475134 xrvoyage-1.0.7/xrvoyage/_version.py
+-rw-r--r--   0        0        0        0 2024-05-23 15:14:44.783079 xrvoyage-1.0.7/xrvoyage/handlers/__init__.py
+-rw-r--r--   0        0        0      209 2024-05-23 15:14:44.783079 xrvoyage-1.0.7/xrvoyage/handlers/static.py
+-rw-r--r--   0        0        0        0 2024-05-23 15:14:44.783079 xrvoyage-1.0.7/xrvoyage/models/__init__.py
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 xrvoyage-1.0.7/PKG-INFO
```

### Comparing `xrvoyage-1.0.6/LICENSE` & `xrvoyage-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xrvoyage-1.0.6/PKG-INFO` & `xrvoyage-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrvoyage
-Version: 1.0.6
+Version: 1.0.7
 Summary: XR Voyage Python Package
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```

