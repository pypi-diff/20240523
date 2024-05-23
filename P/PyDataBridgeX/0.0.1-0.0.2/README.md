# Comparing `tmp/PyDataBridgeX-0.0.1.tar.gz` & `tmp/PyDataBridgeX-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDataBridgeX-0.0.1.tar", last modified: Wed May 22 18:03:07 2024, max compression
+gzip compressed data, was "PyDataBridgeX-0.0.2.tar", last modified: Thu May 23 10:21:46 2024, max compression
```

## Comparing `PyDataBridgeX-0.0.1.tar` & `PyDataBridgeX-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ranuga    (1000) ranuga    (1000)        0 2024-05-22 18:03:07.581344 PyDataBridgeX-0.0.1/
--rw-rw-r--   0 ranuga    (1000) ranuga    (1000)    11357 2024-05-22 17:03:05.000000 PyDataBridgeX-0.0.1/LICENSE
--rw-r--r--   0 ranuga    (1000) ranuga    (1000)      892 2024-05-22 18:03:07.581344 PyDataBridgeX-0.0.1/PKG-INFO
-drwxrwxr-x   0 ranuga    (1000) ranuga    (1000)        0 2024-05-22 18:03:07.581344 PyDataBridgeX-0.0.1/PyDataBridgeX.egg-info/
--rw-r--r--   0 ranuga    (1000) ranuga    (1000)      892 2024-05-22 18:03:07.000000 PyDataBridgeX-0.0.1/PyDataBridgeX.egg-info/PKG-INFO
--rw-rw-r--   0 ranuga    (1000) ranuga    (1000)      210 2024-05-22 18:03:07.000000 PyDataBridgeX-0.0.1/PyDataBridgeX.egg-info/SOURCES.txt
--rw-rw-r--   0 ranuga    (1000) ranuga    (1000)        1 2024-05-22 18:03:07.000000 PyDataBridgeX-0.0.1/PyDataBridgeX.egg-info/dependency_links.txt
--rw-rw-r--   0 ranuga    (1000) ranuga    (1000)       16 2024-05-22 18:03:07.000000 PyDataBridgeX-0.0.1/PyDataBridgeX.egg-info/requires.txt
--rw-rw-r--   0 ranuga    (1000) ranuga    (1000)        1 2024-05-22 18:03:07.000000 PyDataBridgeX-0.0.1/PyDataBridgeX.egg-info/top_level.txt
--rw-rw-r--   0 ranuga    (1000) ranuga    (1000)      310 2024-05-22 17:03:05.000000 PyDataBridgeX-0.0.1/README.md
--rw-rw-r--   0 ranuga    (1000) ranuga    (1000)       38 2024-05-22 18:03:07.581344 PyDataBridgeX-0.0.1/setup.cfg
--rw-rw-r--   0 ranuga    (1000) ranuga    (1000)     1195 2024-05-22 18:02:37.000000 PyDataBridgeX-0.0.1/setup.py
+drwxrwxr-x   0 ranuga    (1000) ranuga    (1000)        0 2024-05-23 10:21:46.385785 PyDataBridgeX-0.0.2/
+-rw-rw-r--   0 ranuga    (1000) ranuga    (1000)    11357 2024-05-22 17:03:05.000000 PyDataBridgeX-0.0.2/LICENSE
+-rw-r--r--   0 ranuga    (1000) ranuga    (1000)      873 2024-05-23 10:21:46.385785 PyDataBridgeX-0.0.2/PKG-INFO
+drwxrwxr-x   0 ranuga    (1000) ranuga    (1000)        0 2024-05-23 10:21:46.385785 PyDataBridgeX-0.0.2/PyDataBridgeX.egg-info/
+-rw-r--r--   0 ranuga    (1000) ranuga    (1000)      873 2024-05-23 10:21:46.000000 PyDataBridgeX-0.0.2/PyDataBridgeX.egg-info/PKG-INFO
+-rw-rw-r--   0 ranuga    (1000) ranuga    (1000)      210 2024-05-23 10:21:46.000000 PyDataBridgeX-0.0.2/PyDataBridgeX.egg-info/SOURCES.txt
+-rw-rw-r--   0 ranuga    (1000) ranuga    (1000)        1 2024-05-23 10:21:46.000000 PyDataBridgeX-0.0.2/PyDataBridgeX.egg-info/dependency_links.txt
+-rw-rw-r--   0 ranuga    (1000) ranuga    (1000)       16 2024-05-23 10:21:46.000000 PyDataBridgeX-0.0.2/PyDataBridgeX.egg-info/requires.txt
+-rw-rw-r--   0 ranuga    (1000) ranuga    (1000)        1 2024-05-23 10:21:46.000000 PyDataBridgeX-0.0.2/PyDataBridgeX.egg-info/top_level.txt
+-rw-rw-r--   0 ranuga    (1000) ranuga    (1000)     1366 2024-05-23 06:59:01.000000 PyDataBridgeX-0.0.2/README.md
+-rw-rw-r--   0 ranuga    (1000) ranuga    (1000)       38 2024-05-23 10:21:46.385785 PyDataBridgeX-0.0.2/setup.cfg
+-rw-rw-r--   0 ranuga    (1000) ranuga    (1000)     1176 2024-05-23 10:21:40.000000 PyDataBridgeX-0.0.2/setup.py
```

### Comparing `PyDataBridgeX-0.0.1/LICENSE` & `PyDataBridgeX-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDataBridgeX-0.0.1/PKG-INFO` & `PyDataBridgeX-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: PyDataBridgeX
-Version: 0.0.1
-Summary: Your go-to solution for database connectivity in Python
+Version: 0.0.2
+Summary: Bridging Innovation, Connecting Data
 Author: Ranuga Disansa Gamage
 Author-email: go2ranuga@gmail.com
 Keywords: python,database,connectivity,firebase,backend,development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PyDataBridgeX-0.0.1/PyDataBridgeX.egg-info/PKG-INFO` & `PyDataBridgeX-0.0.2/PyDataBridgeX.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: PyDataBridgeX
-Version: 0.0.1
-Summary: Your go-to solution for database connectivity in Python
+Version: 0.0.2
+Summary: Bridging Innovation, Connecting Data
 Author: Ranuga Disansa Gamage
 Author-email: go2ranuga@gmail.com
 Keywords: python,database,connectivity,firebase,backend,development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PyDataBridgeX-0.0.1/setup.py` & `PyDataBridgeX-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.1"
-DESCRIPTION = "Your go-to solution for database connectivity in Python"
+VERSION = "0.0.2"
+DESCRIPTION = "Bridging Innovation, Connecting Data"
 LONG_DESCRIPTION = """PyDataBridge is your go-to solution for database connectivity in Python. Whether you're working with Firebase or other databases, PyDataBridge offers a versatile and intuitive package for seamless integration. Simplify your backend development and unleash the power of Python with PyDataBridge."""
 
 # Setting up
 setup(
     name="PyDataBridgeX",
     version=VERSION,
     author="Ranuga Disansa Gamage",
```

