# Comparing `tmp/digitalhub-0.5.0b1.tar.gz` & `tmp/digitalhub-0.5.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub-0.5.0b1.tar", last modified: Tue May 21 15:52:49 2024, max compression
+gzip compressed data, was "digitalhub-0.5.0b2.tar", last modified: Thu May 23 13:59:30 2024, max compression
```

## Comparing `digitalhub-0.5.0b1.tar` & `digitalhub-0.5.0b2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:52:49.192991 digitalhub-0.5.0b1/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub-0.5.0b1/LICENSE.txt
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14818 2024-05-21 15:52:49.192991 digitalhub-0.5.0b1/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      510 2024-04-23 09:36:04.000000 digitalhub-0.5.0b1/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:52:49.176991 digitalhub-0.5.0b1/digitalhub/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2218 2024-05-21 13:14:46.000000 digitalhub-0.5.0b1/digitalhub/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:52:49.184991 digitalhub-0.5.0b1/digitalhub.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14818 2024-05-21 15:52:49.000000 digitalhub-0.5.0b1/digitalhub.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      421 2024-05-21 15:52:49.000000 digitalhub-0.5.0b1/digitalhub.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-21 15:52:49.000000 digitalhub-0.5.0b1/digitalhub.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      194 2024-05-21 15:52:49.000000 digitalhub-0.5.0b1/digitalhub.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       35 2024-05-21 15:52:49.000000 digitalhub-0.5.0b1/digitalhub.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1575 2024-05-21 15:33:27.000000 digitalhub-0.5.0b1/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-21 15:52:49.192991 digitalhub-0.5.0b1/setup.cfg
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:52:49.184991 digitalhub-0.5.0b1/test/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2511 2024-05-09 07:33:31.000000 digitalhub-0.5.0b1/test/test_crud_artifacts.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2504 2024-05-09 07:33:31.000000 digitalhub-0.5.0b1/test/test_crud_dataitems.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2769 2024-05-09 07:33:31.000000 digitalhub-0.5.0b1/test/test_crud_functions.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2220 2024-05-09 07:33:31.000000 digitalhub-0.5.0b1/test/test_crud_runs.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2111 2024-05-09 07:33:31.000000 digitalhub-0.5.0b1/test/test_crud_tasks.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1269 2024-03-22 13:56:51.000000 digitalhub-0.5.0b1/test/test_imports.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1086 2024-03-25 07:51:29.000000 digitalhub-0.5.0b1/test/testkfp.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      619 2024-03-25 10:18:34.000000 digitalhub-0.5.0b1/test/testkfp_pipeline.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 13:59:30.806531 digitalhub-0.5.0b2/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub-0.5.0b2/LICENSE.txt
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14818 2024-05-23 13:59:30.802531 digitalhub-0.5.0b2/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      510 2024-04-23 09:36:04.000000 digitalhub-0.5.0b2/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 13:59:30.802531 digitalhub-0.5.0b2/digitalhub/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2218 2024-05-23 09:43:32.000000 digitalhub-0.5.0b2/digitalhub/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 13:59:30.802531 digitalhub-0.5.0b2/digitalhub.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14818 2024-05-23 13:59:30.000000 digitalhub-0.5.0b2/digitalhub.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      421 2024-05-23 13:59:30.000000 digitalhub-0.5.0b2/digitalhub.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-23 13:59:30.000000 digitalhub-0.5.0b2/digitalhub.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      194 2024-05-23 13:59:30.000000 digitalhub-0.5.0b2/digitalhub.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       35 2024-05-23 13:59:30.000000 digitalhub-0.5.0b2/digitalhub.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1575 2024-05-23 13:58:10.000000 digitalhub-0.5.0b2/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-23 13:59:30.806531 digitalhub-0.5.0b2/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 13:59:30.802531 digitalhub-0.5.0b2/test/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2511 2024-05-09 07:33:31.000000 digitalhub-0.5.0b2/test/test_crud_artifacts.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2504 2024-05-09 07:33:31.000000 digitalhub-0.5.0b2/test/test_crud_dataitems.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2769 2024-05-09 07:33:31.000000 digitalhub-0.5.0b2/test/test_crud_functions.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2220 2024-05-09 07:33:31.000000 digitalhub-0.5.0b2/test/test_crud_runs.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2111 2024-05-09 07:33:31.000000 digitalhub-0.5.0b2/test/test_crud_tasks.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1269 2024-03-22 13:56:51.000000 digitalhub-0.5.0b2/test/test_imports.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1086 2024-03-25 07:51:29.000000 digitalhub-0.5.0b2/test/testkfp.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      619 2024-03-25 10:18:34.000000 digitalhub-0.5.0b2/test/testkfp_pipeline.py
```

### Comparing `digitalhub-0.5.0b1/LICENSE.txt` & `digitalhub-0.5.0b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `digitalhub-0.5.0b1/PKG-INFO` & `digitalhub-0.5.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub
-Version: 0.5.0b1
+Version: 0.5.0b2
 Summary: Python SDK for DigitalHub
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -224,25 +224,25 @@
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: digitalhub-core==0.5.0b1
+Requires-Dist: digitalhub-core==0.5.0b2
 Provides-Extra: all
-Requires-Dist: digitalhub-data==0.5.0b1; extra == "all"
-Requires-Dist: digitalhub-ml==0.5.0b1; extra == "all"
-Requires-Dist: digitalhub-ai==0.5.0b1; extra == "all"
+Requires-Dist: digitalhub-data==0.5.0b2; extra == "all"
+Requires-Dist: digitalhub-ml==0.5.0b2; extra == "all"
+Requires-Dist: digitalhub-ai==0.5.0b2; extra == "all"
 Provides-Extra: ml
-Requires-Dist: digitalhub-ml==0.5.0b1; extra == "ml"
+Requires-Dist: digitalhub-ml==0.5.0b2; extra == "ml"
 Provides-Extra: ai
-Requires-Dist: digitalhub-ai==0.5.0b1; extra == "ai"
+Requires-Dist: digitalhub-ai==0.5.0b2; extra == "ai"
 Provides-Extra: data
-Requires-Dist: digitalhub-data==0.5.0b1; extra == "data"
+Requires-Dist: digitalhub-data==0.5.0b2; extra == "data"
 
 # Digitalhub Library
 
 The Digitalhub SDK library is used to manage entities and executions in Digitalhub from Python.
 It comes with a suite of tools to help you manage your projects and executions. It exposes CRUD methods to create, read, update and delete entities, and objects methods to excute functions or workflows, collect or store execution results and data.
 
 A more detailed description of the library can be found in the [official documentation](https://scc-digitalhub.github.io/docs/) of Digitalhub.
```

### Comparing `digitalhub-0.5.0b1/digitalhub/__init__.py` & `digitalhub-0.5.0b2/digitalhub/__init__.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.5.0b1/digitalhub.egg-info/PKG-INFO` & `digitalhub-0.5.0b2/digitalhub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub
-Version: 0.5.0b1
+Version: 0.5.0b2
 Summary: Python SDK for DigitalHub
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -224,25 +224,25 @@
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: digitalhub-core==0.5.0b1
+Requires-Dist: digitalhub-core==0.5.0b2
 Provides-Extra: all
-Requires-Dist: digitalhub-data==0.5.0b1; extra == "all"
-Requires-Dist: digitalhub-ml==0.5.0b1; extra == "all"
-Requires-Dist: digitalhub-ai==0.5.0b1; extra == "all"
+Requires-Dist: digitalhub-data==0.5.0b2; extra == "all"
+Requires-Dist: digitalhub-ml==0.5.0b2; extra == "all"
+Requires-Dist: digitalhub-ai==0.5.0b2; extra == "all"
 Provides-Extra: ml
-Requires-Dist: digitalhub-ml==0.5.0b1; extra == "ml"
+Requires-Dist: digitalhub-ml==0.5.0b2; extra == "ml"
 Provides-Extra: ai
-Requires-Dist: digitalhub-ai==0.5.0b1; extra == "ai"
+Requires-Dist: digitalhub-ai==0.5.0b2; extra == "ai"
 Provides-Extra: data
-Requires-Dist: digitalhub-data==0.5.0b1; extra == "data"
+Requires-Dist: digitalhub-data==0.5.0b2; extra == "data"
 
 # Digitalhub Library
 
 The Digitalhub SDK library is used to manage entities and executions in Digitalhub from Python.
 It comes with a suite of tools to help you manage your projects and executions. It exposes CRUD methods to create, read, update and delete entities, and objects methods to excute functions or workflows, collect or store execution results and data.
 
 A more detailed description of the library can be found in the [official documentation](https://scc-digitalhub.github.io/docs/) of Digitalhub.
```

### Comparing `digitalhub-0.5.0b1/test/test_crud_artifacts.py` & `digitalhub-0.5.0b2/test/test_crud_artifacts.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.5.0b1/test/test_crud_dataitems.py` & `digitalhub-0.5.0b2/test/test_crud_dataitems.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.5.0b1/test/test_crud_functions.py` & `digitalhub-0.5.0b2/test/test_crud_functions.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.5.0b1/test/test_crud_runs.py` & `digitalhub-0.5.0b2/test/test_crud_runs.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.5.0b1/test/test_crud_tasks.py` & `digitalhub-0.5.0b2/test/test_crud_tasks.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.5.0b1/test/test_imports.py` & `digitalhub-0.5.0b2/test/test_imports.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.5.0b1/test/testkfp.py` & `digitalhub-0.5.0b2/test/testkfp.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.5.0b1/test/testkfp_pipeline.py` & `digitalhub-0.5.0b2/test/testkfp_pipeline.py`

 * *Files identical despite different names*

