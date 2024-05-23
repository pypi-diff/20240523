# Comparing `tmp/ls_packers-0.5.3.tar.gz` & `tmp/ls_packers-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ls_packers-0.5.3.tar", last modified: Thu May 23 11:41:25 2024, max compression
+gzip compressed data, was "ls_packers-0.6.0.tar", last modified: Thu May 23 11:42:03 2024, max compression
```

## Comparing `ls_packers-0.5.3.tar` & `ls_packers-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:41:25.872317 ls_packers-0.5.3/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2024-05-23 11:40:43.000000 ls_packers-0.5.3/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      598 2024-05-23 11:41:25.872317 ls_packers-0.5.3/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       68 2024-05-23 11:40:43.000000 ls_packers-0.5.3/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:41:25.872317 ls_packers-0.5.3/ls_packers/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      493 2024-05-23 11:40:43.000000 ls_packers-0.5.3/ls_packers/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1152 2024-05-23 11:40:43.000000 ls_packers-0.5.3/ls_packers/converters.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      561 2024-05-23 11:40:43.000000 ls_packers-0.5.3/ls_packers/packers.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:41:25.872317 ls_packers-0.5.3/ls_packers.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      598 2024-05-23 11:41:25.000000 ls_packers-0.5.3/ls_packers.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      335 2024-05-23 11:41:25.000000 ls_packers-0.5.3/ls_packers.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-23 11:41:25.000000 ls_packers-0.5.3/ls_packers.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       22 2024-05-23 11:41:25.000000 ls_packers-0.5.3/ls_packers.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       11 2024-05-23 11:41:25.000000 ls_packers-0.5.3/ls_packers.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      649 2024-05-23 11:41:11.000000 ls_packers-0.5.3/pyproject.toml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-23 11:41:25.872317 ls_packers-0.5.3/setup.cfg
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:41:25.872317 ls_packers-0.5.3/tests/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      797 2024-05-23 11:40:43.000000 ls_packers-0.5.3/tests/test_float_array_packers.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      747 2024-05-23 11:40:43.000000 ls_packers-0.5.3/tests/test_triu_conversion.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:42:03.088458 ls_packers-0.6.0/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2024-05-23 11:40:43.000000 ls_packers-0.6.0/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      598 2024-05-23 11:42:03.088458 ls_packers-0.6.0/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       68 2024-05-23 11:40:43.000000 ls_packers-0.6.0/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:42:03.088458 ls_packers-0.6.0/ls_packers/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      493 2024-05-23 11:40:43.000000 ls_packers-0.6.0/ls_packers/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1152 2024-05-23 11:40:43.000000 ls_packers-0.6.0/ls_packers/converters.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      561 2024-05-23 11:40:43.000000 ls_packers-0.6.0/ls_packers/packers.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:42:03.088458 ls_packers-0.6.0/ls_packers.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      598 2024-05-23 11:42:03.000000 ls_packers-0.6.0/ls_packers.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      335 2024-05-23 11:42:03.000000 ls_packers-0.6.0/ls_packers.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-23 11:42:03.000000 ls_packers-0.6.0/ls_packers.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       22 2024-05-23 11:42:03.000000 ls_packers-0.6.0/ls_packers.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       11 2024-05-23 11:42:03.000000 ls_packers-0.6.0/ls_packers.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      649 2024-05-23 11:41:58.000000 ls_packers-0.6.0/pyproject.toml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-23 11:42:03.088458 ls_packers-0.6.0/setup.cfg
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:42:03.088458 ls_packers-0.6.0/tests/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      797 2024-05-23 11:40:43.000000 ls_packers-0.6.0/tests/test_float_array_packers.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      747 2024-05-23 11:40:43.000000 ls_packers-0.6.0/tests/test_triu_conversion.py
```

### Comparing `ls_packers-0.5.3/LICENSE` & `ls_packers-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ls_packers-0.5.3/PKG-INFO` & `ls_packers-0.6.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ls-packers
-Version: 0.5.3
+Version: 0.6.0
 Summary: An internal client python API for accessing LightSolver's capabilities
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://lightsolver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ls_packers-0.5.3/ls_packers/converters.py` & `ls_packers-0.6.0/ls_packers/converters.py`

 * *Files identical despite different names*

### Comparing `ls_packers-0.5.3/ls_packers/packers.py` & `ls_packers-0.6.0/ls_packers/packers.py`

 * *Files identical despite different names*

### Comparing `ls_packers-0.5.3/ls_packers.egg-info/PKG-INFO` & `ls_packers-0.6.0/ls_packers.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ls-packers
-Version: 0.5.3
+Version: 0.6.0
 Summary: An internal client python API for accessing LightSolver's capabilities
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://lightsolver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ls_packers-0.5.3/pyproject.toml` & `ls_packers-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ls-packers"
-version = "0.5.3"
+version = "0.6.0"
 description = "An internal client python API for accessing LightSolver's capabilities"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [ "numpy>=1.21.5", "msgpack",]
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "Assaf Kalinski"
```

### Comparing `ls_packers-0.5.3/tests/test_float_array_packers.py` & `ls_packers-0.6.0/tests/test_float_array_packers.py`

 * *Files identical despite different names*

### Comparing `ls_packers-0.5.3/tests/test_triu_conversion.py` & `ls_packers-0.6.0/tests/test_triu_conversion.py`

 * *Files identical despite different names*

