# Comparing `tmp/ls_cred_storage-0.1.3.tar.gz` & `tmp/ls_cred_storage-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ls_cred_storage-0.1.3.tar", last modified: Tue May  7 23:58:54 2024, max compression
+gzip compressed data, was "ls_cred_storage-0.1.4.tar", last modified: Thu May 23 11:45:16 2024, max compression
```

## Comparing `ls_cred_storage-0.1.3.tar` & `ls_cred_storage-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 23:58:54.642895 ls_cred_storage-0.1.3/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11350 2024-05-07 23:56:36.000000 ls_cred_storage-0.1.3/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      572 2024-05-07 23:58:54.642895 ls_cred_storage-0.1.3/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       79 2024-05-07 23:56:36.000000 ls_cred_storage-0.1.3/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 23:58:54.642895 ls_cred_storage-0.1.3/ls_cred_storage/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       57 2024-05-07 23:56:36.000000 ls_cred_storage-0.1.3/ls_cred_storage/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1983 2024-05-07 23:56:36.000000 ls_cred_storage-0.1.3/ls_cred_storage/ls_cred_storage.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 23:58:54.642895 ls_cred_storage-0.1.3/ls_cred_storage.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      572 2024-05-07 23:58:54.000000 ls_cred_storage-0.1.3/ls_cred_storage.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      289 2024-05-07 23:58:54.000000 ls_cred_storage-0.1.3/ls_cred_storage.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-07 23:58:54.000000 ls_cred_storage-0.1.3/ls_cred_storage.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-05-07 23:58:54.000000 ls_cred_storage-0.1.3/ls_cred_storage.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-05-07 23:58:54.000000 ls_cred_storage-0.1.3/ls_cred_storage.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      628 2024-05-07 23:58:51.000000 ls_cred_storage-0.1.3/pyproject.toml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-07 23:58:54.642895 ls_cred_storage-0.1.3/setup.cfg
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:45:16.289184 ls_cred_storage-0.1.4/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11350 2024-05-23 11:44:29.000000 ls_cred_storage-0.1.4/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      572 2024-05-23 11:45:16.289184 ls_cred_storage-0.1.4/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       79 2024-05-23 11:44:29.000000 ls_cred_storage-0.1.4/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:45:16.289184 ls_cred_storage-0.1.4/ls_cred_storage/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       57 2024-05-23 11:44:29.000000 ls_cred_storage-0.1.4/ls_cred_storage/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1983 2024-05-23 11:44:29.000000 ls_cred_storage-0.1.4/ls_cred_storage/ls_cred_storage.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:45:16.289184 ls_cred_storage-0.1.4/ls_cred_storage.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      572 2024-05-23 11:45:16.000000 ls_cred_storage-0.1.4/ls_cred_storage.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      289 2024-05-23 11:45:16.000000 ls_cred_storage-0.1.4/ls_cred_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-23 11:45:16.000000 ls_cred_storage-0.1.4/ls_cred_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-05-23 11:45:16.000000 ls_cred_storage-0.1.4/ls_cred_storage.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-05-23 11:45:16.000000 ls_cred_storage-0.1.4/ls_cred_storage.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      628 2024-05-23 11:45:08.000000 ls_cred_storage-0.1.4/pyproject.toml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-23 11:45:16.289184 ls_cred_storage-0.1.4/setup.cfg
```

### Comparing `ls_cred_storage-0.1.3/LICENSE` & `ls_cred_storage-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ls_cred_storage-0.1.3/PKG-INFO` & `ls_cred_storage-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ls-cred-storage
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package containing storage user credential
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://dev.lightsolver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ls_cred_storage-0.1.3/ls_cred_storage/ls_cred_storage.py` & `ls_cred_storage-0.1.4/ls_cred_storage/ls_cred_storage.py`

 * *Files identical despite different names*

### Comparing `ls_cred_storage-0.1.3/ls_cred_storage.egg-info/PKG-INFO` & `ls_cred_storage-0.1.4/ls_cred_storage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ls-cred-storage
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package containing storage user credential
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://dev.lightsolver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ls_cred_storage-0.1.3/pyproject.toml` & `ls_cred_storage-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ls-cred-storage"
-version = "0.1.3"
+version = "0.1.4"
 description = "A package containing storage user credential"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [ "keyring>=23.2.1",]
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "Assaf Kalinski"
```

