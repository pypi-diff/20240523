# Comparing `tmp/ls_cred_storage-0.2.0.tar.gz` & `tmp/ls_cred_storage-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ls_cred_storage-0.2.0.tar", last modified: Thu May 23 11:47:46 2024, max compression
+gzip compressed data, was "ls_cred_storage-0.3.0.tar", last modified: Thu May 23 15:39:14 2024, max compression
```

## Comparing `ls_cred_storage-0.2.0.tar` & `ls_cred_storage-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:47:46.549755 ls_cred_storage-0.2.0/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11350 2024-05-23 11:44:29.000000 ls_cred_storage-0.2.0/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      572 2024-05-23 11:47:46.549755 ls_cred_storage-0.2.0/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       79 2024-05-23 11:44:29.000000 ls_cred_storage-0.2.0/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:47:46.549755 ls_cred_storage-0.2.0/ls_cred_storage/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       57 2024-05-23 11:44:29.000000 ls_cred_storage-0.2.0/ls_cred_storage/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1983 2024-05-23 11:44:29.000000 ls_cred_storage-0.2.0/ls_cred_storage/ls_cred_storage.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:47:46.549755 ls_cred_storage-0.2.0/ls_cred_storage.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      572 2024-05-23 11:47:46.000000 ls_cred_storage-0.2.0/ls_cred_storage.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      289 2024-05-23 11:47:46.000000 ls_cred_storage-0.2.0/ls_cred_storage.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-23 11:47:46.000000 ls_cred_storage-0.2.0/ls_cred_storage.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-05-23 11:47:46.000000 ls_cred_storage-0.2.0/ls_cred_storage.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-05-23 11:47:46.000000 ls_cred_storage-0.2.0/ls_cred_storage.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      628 2024-05-23 11:47:39.000000 ls_cred_storage-0.2.0/pyproject.toml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-23 11:47:46.549755 ls_cred_storage-0.2.0/setup.cfg
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 15:39:14.922809 ls_cred_storage-0.3.0/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11350 2024-05-23 15:38:03.000000 ls_cred_storage-0.3.0/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      572 2024-05-23 15:39:14.922809 ls_cred_storage-0.3.0/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       79 2024-05-23 15:38:03.000000 ls_cred_storage-0.3.0/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 15:39:14.922809 ls_cred_storage-0.3.0/ls_cred_storage/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       57 2024-05-23 15:38:03.000000 ls_cred_storage-0.3.0/ls_cred_storage/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1988 2024-05-23 15:38:03.000000 ls_cred_storage-0.3.0/ls_cred_storage/ls_cred_storage.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 15:39:14.922809 ls_cred_storage-0.3.0/ls_cred_storage.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      572 2024-05-23 15:39:14.000000 ls_cred_storage-0.3.0/ls_cred_storage.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      289 2024-05-23 15:39:14.000000 ls_cred_storage-0.3.0/ls_cred_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-23 15:39:14.000000 ls_cred_storage-0.3.0/ls_cred_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-05-23 15:39:14.000000 ls_cred_storage-0.3.0/ls_cred_storage.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-05-23 15:39:14.000000 ls_cred_storage-0.3.0/ls_cred_storage.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      628 2024-05-23 15:39:07.000000 ls_cred_storage-0.3.0/pyproject.toml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-23 15:39:14.922809 ls_cred_storage-0.3.0/setup.cfg
```

### Comparing `ls_cred_storage-0.2.0/LICENSE` & `ls_cred_storage-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ls_cred_storage-0.2.0/PKG-INFO` & `ls_cred_storage-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ls-cred-storage
-Version: 0.2.0
+Version: 0.3.0
 Summary: A package containing storage user credential
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://dev.lightsolver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ls_cred_storage-0.2.0/ls_cred_storage/ls_cred_storage.py` & `ls_cred_storage-0.3.0/ls_cred_storage/ls_cred_storage.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import keyring
 import time
 import json
 import os
 
 
 class LSCredStorage():
-    USER_KEY = 'user'
+    USER_KEY = 'userToken'
     TIMESTAMP_KEY = 'timestamp'
     USER_ID_KEY = 'userId'
     SESSION_TOKEN_KEY = 'sessionToken'
     ACCESS_TOKEN_KEY = 'accessToken'
     MAX_TOKEN_RETENTION_TIME_SECS = 3500
     APP_SERVICE_NAME = 'LightSolverClient'
```

### Comparing `ls_cred_storage-0.2.0/ls_cred_storage.egg-info/PKG-INFO` & `ls_cred_storage-0.3.0/ls_cred_storage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ls-cred-storage
-Version: 0.2.0
+Version: 0.3.0
 Summary: A package containing storage user credential
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://dev.lightsolver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ls_cred_storage-0.2.0/pyproject.toml` & `ls_cred_storage-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ls-cred-storage"
-version = "0.2.0"
+version = "0.3.0"
 description = "A package containing storage user credential"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [ "keyring>=23.2.1",]
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "Assaf Kalinski"
```

