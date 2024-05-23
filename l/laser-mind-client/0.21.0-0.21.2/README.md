# Comparing `tmp/laser_mind_client-0.21.0.tar.gz` & `tmp/laser_mind_client-0.21.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laser_mind_client-0.21.0.tar", last modified: Tue May  7 14:49:46 2024, max compression
+gzip compressed data, was "laser_mind_client-0.21.2.tar", last modified: Thu May 23 09:42:19 2024, max compression
```

## Comparing `laser_mind_client-0.21.0.tar` & `laser_mind_client-0.21.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 14:49:46.517714 laser_mind_client-0.21.0/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11350 2024-05-07 14:48:49.000000 laser_mind_client-0.21.0/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8772 2024-05-07 14:49:46.517714 laser_mind_client-0.21.0/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8152 2024-05-07 14:48:49.000000 laser_mind_client-0.21.0/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 14:49:46.513714 laser_mind_client-0.21.0/laser_mind_client/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       57 2024-05-07 14:48:49.000000 laser_mind_client-0.21.0/laser_mind_client/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7918 2024-05-07 14:48:49.000000 laser_mind_client-0.21.0/laser_mind_client/laser_mind_client.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 14:49:46.513714 laser_mind_client-0.21.0/laser_mind_client.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8772 2024-05-07 14:49:46.000000 laser_mind_client-0.21.0/laser_mind_client.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      305 2024-05-07 14:49:46.000000 laser_mind_client-0.21.0/laser_mind_client.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-07 14:49:46.000000 laser_mind_client-0.21.0/laser_mind_client.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       84 2024-05-07 14:49:46.000000 laser_mind_client-0.21.0/laser_mind_client.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-07 14:49:46.000000 laser_mind_client-0.21.0/laser_mind_client.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      722 2024-05-07 14:49:42.000000 laser_mind_client-0.21.0/pyproject.toml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-07 14:49:46.517714 laser_mind_client-0.21.0/setup.cfg
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 09:42:19.912034 laser_mind_client-0.21.2/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11350 2024-05-23 09:36:06.000000 laser_mind_client-0.21.2/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8772 2024-05-23 09:42:19.908034 laser_mind_client-0.21.2/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8152 2024-05-23 09:36:06.000000 laser_mind_client-0.21.2/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 09:42:19.908034 laser_mind_client-0.21.2/laser_mind_client/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       57 2024-05-23 09:36:06.000000 laser_mind_client-0.21.2/laser_mind_client/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7918 2024-05-23 09:36:06.000000 laser_mind_client-0.21.2/laser_mind_client/laser_mind_client.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 09:42:19.908034 laser_mind_client-0.21.2/laser_mind_client.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8772 2024-05-23 09:42:19.000000 laser_mind_client-0.21.2/laser_mind_client.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      305 2024-05-23 09:42:19.000000 laser_mind_client-0.21.2/laser_mind_client.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-23 09:42:19.000000 laser_mind_client-0.21.2/laser_mind_client.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       84 2024-05-23 09:42:19.000000 laser_mind_client-0.21.2/laser_mind_client.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-23 09:42:19.000000 laser_mind_client-0.21.2/laser_mind_client.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      722 2024-05-23 09:42:13.000000 laser_mind_client-0.21.2/pyproject.toml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-23 09:42:19.912034 laser_mind_client-0.21.2/setup.cfg
```

### Comparing `laser_mind_client-0.21.0/LICENSE` & `laser_mind_client-0.21.2/LICENSE`

 * *Files identical despite different names*

### Comparing `laser_mind_client-0.21.0/PKG-INFO` & `laser_mind_client-0.21.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laser-mind-client
-Version: 0.21.0
+Version: 0.21.2
 Summary: A client python API for accessing LightSolver's capabilities
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://lightsolver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `laser_mind_client-0.21.0/README.md` & `laser_mind_client-0.21.2/README.md`

 * *Files identical despite different names*

### Comparing `laser_mind_client-0.21.0/laser_mind_client/laser_mind_client.py` & `laser_mind_client-0.21.2/laser_mind_client/laser_mind_client.py`

 * *Files identical despite different names*

### Comparing `laser_mind_client-0.21.0/laser_mind_client.egg-info/PKG-INFO` & `laser_mind_client-0.21.2/laser_mind_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laser-mind-client
-Version: 0.21.0
+Version: 0.21.2
 Summary: A client python API for accessing LightSolver's capabilities
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://lightsolver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `laser_mind_client-0.21.0/pyproject.toml` & `laser_mind_client-0.21.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "laser-mind-client"
-version = "0.21.0"
+version = "0.21.2"
 description = "A client python API for accessing LightSolver's capabilities"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [ "numpy>=1.21.5", "laser-mind-client-meta>=0.0.9", "ls_api_clients>=0.4.6", "ls-packers>=0.2.0",]
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "Assaf Kalinski"
```

