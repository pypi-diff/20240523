# Comparing `tmp/admin_auth0-0.2.8.tar.gz` & `tmp/admin_auth0-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "admin_auth0-0.2.8.tar", max compression
+gzip compressed data, was "admin_auth0-0.2.9.tar", max compression
```

## Comparing `admin_auth0-0.2.8.tar` & `admin_auth0-0.2.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      258 2024-04-12 15:38:57.001507 admin_auth0-0.2.8/README.md
--rw-r--r--   0        0        0        0 2024-04-12 15:38:57.001507 admin_auth0-0.2.8/admin_auth0/__init__.py
--rw-r--r--   0        0        0      632 2024-04-12 15:38:57.001507 admin_auth0-0.2.8/admin_auth0/auth0.py
--rw-r--r--   0        0        0     2127 2024-04-12 15:38:57.001507 admin_auth0-0.2.8/admin_auth0/authentication.py
--rw-r--r--   0        0        0      236 2024-04-12 15:38:57.001507 admin_auth0-0.2.8/admin_auth0/urls.py
--rw-r--r--   0        0        0     1344 2024-04-12 15:38:57.001507 admin_auth0-0.2.8/admin_auth0/views.py
--rw-r--r--   0        0        0      399 2024-04-12 15:38:57.001507 admin_auth0-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 admin_auth0-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      258 2024-04-17 16:49:05.185567 admin_auth0-0.2.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 16:49:05.189567 admin_auth0-0.2.9/admin_auth0/__init__.py
+-rw-r--r--   0        0        0      632 2024-04-17 16:49:05.189567 admin_auth0-0.2.9/admin_auth0/auth0.py
+-rw-r--r--   0        0        0     2127 2024-04-17 16:49:05.189567 admin_auth0-0.2.9/admin_auth0/authentication.py
+-rw-r--r--   0        0        0      236 2024-04-17 16:49:05.189567 admin_auth0-0.2.9/admin_auth0/urls.py
+-rw-r--r--   0        0        0     1344 2024-04-17 16:49:05.189567 admin_auth0-0.2.9/admin_auth0/views.py
+-rw-r--r--   0        0        0      398 2024-04-17 16:49:05.189567 admin_auth0-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 admin_auth0-0.2.9/PKG-INFO
```

### Comparing `admin_auth0-0.2.8/admin_auth0/auth0.py` & `admin_auth0-0.2.9/admin_auth0/auth0.py`

 * *Files identical despite different names*

### Comparing `admin_auth0-0.2.8/admin_auth0/authentication.py` & `admin_auth0-0.2.9/admin_auth0/authentication.py`

 * *Files identical despite different names*

### Comparing `admin_auth0-0.2.8/admin_auth0/views.py` & `admin_auth0-0.2.9/admin_auth0/views.py`

 * *Files identical despite different names*

### Comparing `admin_auth0-0.2.8/PKG-INFO` & `admin_auth0-0.2.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: admin_auth0
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 Author: Serhii Lakodei
 Author-email: serhii.lakodei@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: authlib (>=1.3.0)
 Requires-Dist: build (>=1.0.3)
 Requires-Dist: django (>=4.2.2)
 Requires-Dist: django-environ (>=0.10.0)
```

