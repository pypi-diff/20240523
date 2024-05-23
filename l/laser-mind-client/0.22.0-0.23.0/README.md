# Comparing `tmp/laser_mind_client-0.22.0.tar.gz` & `tmp/laser_mind_client-0.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laser_mind_client-0.22.0.tar", last modified: Thu May 23 10:47:47 2024, max compression
+gzip compressed data, was "laser_mind_client-0.23.0.tar", last modified: Thu May 23 11:27:02 2024, max compression
```

## Comparing `laser_mind_client-0.22.0.tar` & `laser_mind_client-0.23.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 10:47:47.107981 laser_mind_client-0.22.0/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11350 2024-05-23 10:46:36.000000 laser_mind_client-0.22.0/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8914 2024-05-23 10:47:47.103981 laser_mind_client-0.22.0/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8294 2024-05-23 10:46:36.000000 laser_mind_client-0.22.0/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 10:47:47.103981 laser_mind_client-0.22.0/laser_mind_client/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       57 2024-05-23 10:46:36.000000 laser_mind_client-0.22.0/laser_mind_client/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8587 2024-05-23 10:46:36.000000 laser_mind_client-0.22.0/laser_mind_client/laser_mind_client.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 10:47:47.103981 laser_mind_client-0.22.0/laser_mind_client.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8914 2024-05-23 10:47:47.000000 laser_mind_client-0.22.0/laser_mind_client.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      415 2024-05-23 10:47:47.000000 laser_mind_client-0.22.0/laser_mind_client.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-23 10:47:47.000000 laser_mind_client-0.22.0/laser_mind_client.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       84 2024-05-23 10:47:47.000000 laser_mind_client-0.22.0/laser_mind_client.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-23 10:47:47.000000 laser_mind_client-0.22.0/laser_mind_client.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      722 2024-05-23 10:47:40.000000 laser_mind_client-0.22.0/pyproject.toml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-23 10:47:47.107981 laser_mind_client-0.22.0/setup.cfg
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 10:47:47.103981 laser_mind_client-0.22.0/tests/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      453 2024-05-23 10:46:36.000000 laser_mind_client-0.22.0/tests/test_solve_qubo_adjacency_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      529 2024-05-23 10:46:36.000000 laser_mind_client-0.22.0/tests/test_solve_qubo_matrix.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      992 2024-05-23 10:46:36.000000 laser_mind_client-0.22.0/tests/test_solve_qubo_matrix_async.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:27:02.305035 laser_mind_client-0.23.0/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11350 2024-05-23 10:46:36.000000 laser_mind_client-0.23.0/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8914 2024-05-23 11:27:02.305035 laser_mind_client-0.23.0/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8294 2024-05-23 10:46:36.000000 laser_mind_client-0.23.0/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:27:02.301035 laser_mind_client-0.23.0/laser_mind_client/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       57 2024-05-23 10:46:36.000000 laser_mind_client-0.23.0/laser_mind_client/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8587 2024-05-23 10:46:36.000000 laser_mind_client-0.23.0/laser_mind_client/laser_mind_client.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:27:02.305035 laser_mind_client-0.23.0/laser_mind_client.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8914 2024-05-23 11:27:02.000000 laser_mind_client-0.23.0/laser_mind_client.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      415 2024-05-23 11:27:02.000000 laser_mind_client-0.23.0/laser_mind_client.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-23 11:27:02.000000 laser_mind_client-0.23.0/laser_mind_client.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       84 2024-05-23 11:27:02.000000 laser_mind_client-0.23.0/laser_mind_client.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-23 11:27:02.000000 laser_mind_client-0.23.0/laser_mind_client.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      722 2024-05-23 11:26:53.000000 laser_mind_client-0.23.0/pyproject.toml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-23 11:27:02.305035 laser_mind_client-0.23.0/setup.cfg
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:27:02.305035 laser_mind_client-0.23.0/tests/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      453 2024-05-23 10:46:36.000000 laser_mind_client-0.23.0/tests/test_solve_qubo_adjacency_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      529 2024-05-23 10:46:36.000000 laser_mind_client-0.23.0/tests/test_solve_qubo_matrix.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      992 2024-05-23 10:46:36.000000 laser_mind_client-0.23.0/tests/test_solve_qubo_matrix_async.py
```

### Comparing `laser_mind_client-0.22.0/LICENSE` & `laser_mind_client-0.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `laser_mind_client-0.22.0/PKG-INFO` & `laser_mind_client-0.23.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laser-mind-client
-Version: 0.22.0
+Version: 0.23.0
 Summary: A client python API for accessing LightSolver's capabilities
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://lightsolver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `laser_mind_client-0.22.0/README.md` & `laser_mind_client-0.23.0/README.md`

 * *Files identical despite different names*

### Comparing `laser_mind_client-0.22.0/laser_mind_client/laser_mind_client.py` & `laser_mind_client-0.23.0/laser_mind_client/laser_mind_client.py`

 * *Files identical despite different names*

### Comparing `laser_mind_client-0.22.0/laser_mind_client.egg-info/PKG-INFO` & `laser_mind_client-0.23.0/laser_mind_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laser-mind-client
-Version: 0.22.0
+Version: 0.23.0
 Summary: A client python API for accessing LightSolver's capabilities
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://lightsolver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `laser_mind_client-0.22.0/pyproject.toml` & `laser_mind_client-0.23.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "laser-mind-client"
-version = "0.22.0"
+version = "0.23.0"
 description = "A client python API for accessing LightSolver's capabilities"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [ "numpy>=1.21.5", "laser-mind-client-meta>=0.0.9", "ls_api_clients>=0.4.6", "ls-packers>=0.2.0",]
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "Assaf Kalinski"
```

### Comparing `laser_mind_client-0.22.0/tests/test_solve_qubo_matrix.py` & `laser_mind_client-0.23.0/tests/test_solve_qubo_matrix.py`

 * *Files identical despite different names*

### Comparing `laser_mind_client-0.22.0/tests/test_solve_qubo_matrix_async.py` & `laser_mind_client-0.23.0/tests/test_solve_qubo_matrix_async.py`

 * *Files identical despite different names*

