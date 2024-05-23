# Comparing `tmp/pypods-0.1.1.tar.gz` & `tmp/pypods-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypods-0.1.1.tar", last modified: Thu May 23 06:03:04 2024, max compression
+gzip compressed data, was "pypods-0.1.2.tar", last modified: Thu May 23 06:27:32 2024, max compression
```

## Comparing `pypods-0.1.1.tar` & `pypods-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 rohandeshpande   (501) staff       (20)        0 2024-05-23 06:03:04.457578 pypods-0.1.1/
--rw-r--r--   0 rohandeshpande   (501) staff       (20)     1058 2024-05-19 02:45:24.000000 pypods-0.1.1/LICENSE
--rw-r--r--   0 rohandeshpande   (501) staff       (20)     4624 2024-05-23 06:03:04.457449 pypods-0.1.1/PKG-INFO
--rw-r--r--   0 rohandeshpande   (501) staff       (20)     4105 2024-05-23 05:57:54.000000 pypods-0.1.1/README.md
-drwxr-xr-x   0 rohandeshpande   (501) staff       (20)        0 2024-05-23 06:03:04.456418 pypods-0.1.1/pypods/
--rw-r--r--   0 rohandeshpande   (501) staff       (20)       53 2024-05-23 06:02:29.000000 pypods-0.1.1/pypods/__init__.py
--rw-r--r--   0 rohandeshpande   (501) staff       (20)      414 2024-05-20 17:24:37.000000 pypods-0.1.1/pypods/errors.py
--rw-r--r--   0 rohandeshpande   (501) staff       (20)     1624 2024-05-20 20:52:13.000000 pypods-0.1.1/pypods/ns.py
--rw-r--r--   0 rohandeshpande   (501) staff       (20)     8193 2024-05-23 05:39:22.000000 pypods-0.1.1/pypods/pods.py
-drwxr-xr-x   0 rohandeshpande   (501) staff       (20)        0 2024-05-23 06:03:04.457223 pypods-0.1.1/pypods.egg-info/
--rw-r--r--   0 rohandeshpande   (501) staff       (20)     4624 2024-05-23 06:03:04.000000 pypods-0.1.1/pypods.egg-info/PKG-INFO
--rw-r--r--   0 rohandeshpande   (501) staff       (20)      239 2024-05-23 06:03:04.000000 pypods-0.1.1/pypods.egg-info/SOURCES.txt
--rw-r--r--   0 rohandeshpande   (501) staff       (20)        1 2024-05-23 06:03:04.000000 pypods-0.1.1/pypods.egg-info/dependency_links.txt
--rw-r--r--   0 rohandeshpande   (501) staff       (20)        5 2024-05-23 06:03:04.000000 pypods-0.1.1/pypods.egg-info/requires.txt
--rw-r--r--   0 rohandeshpande   (501) staff       (20)        7 2024-05-23 06:03:04.000000 pypods-0.1.1/pypods.egg-info/top_level.txt
--rw-r--r--   0 rohandeshpande   (501) staff       (20)       38 2024-05-23 06:03:04.457639 pypods-0.1.1/setup.cfg
--rw-r--r--   0 rohandeshpande   (501) staff       (20)      824 2024-05-23 06:02:31.000000 pypods-0.1.1/setup.py
+drwxr-xr-x   0 rohandeshpande   (501) staff       (20)        0 2024-05-23 06:27:32.237585 pypods-0.1.2/
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)     1058 2024-05-19 02:45:24.000000 pypods-0.1.2/LICENSE
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)     4624 2024-05-23 06:27:32.237458 pypods-0.1.2/PKG-INFO
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)     4105 2024-05-23 05:57:54.000000 pypods-0.1.2/README.md
+drwxr-xr-x   0 rohandeshpande   (501) staff       (20)        0 2024-05-23 06:27:32.236364 pypods-0.1.2/pypods/
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)       53 2024-05-23 06:26:12.000000 pypods-0.1.2/pypods/__init__.py
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)      414 2024-05-20 17:24:37.000000 pypods-0.1.2/pypods/errors.py
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)     1624 2024-05-20 20:52:13.000000 pypods-0.1.2/pypods/ns.py
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)     8193 2024-05-23 05:39:22.000000 pypods-0.1.2/pypods/pods.py
+drwxr-xr-x   0 rohandeshpande   (501) staff       (20)        0 2024-05-23 06:27:32.237220 pypods-0.1.2/pypods/template/
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)     1386 2024-05-20 20:56:47.000000 pypods-0.1.2/pypods/template/pod.py
+drwxr-xr-x   0 rohandeshpande   (501) staff       (20)        0 2024-05-23 06:27:32.237078 pypods-0.1.2/pypods.egg-info/
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)     4624 2024-05-23 06:27:32.000000 pypods-0.1.2/pypods.egg-info/PKG-INFO
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)      262 2024-05-23 06:27:32.000000 pypods-0.1.2/pypods.egg-info/SOURCES.txt
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)        1 2024-05-23 06:27:32.000000 pypods-0.1.2/pypods.egg-info/dependency_links.txt
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)        5 2024-05-23 06:27:32.000000 pypods-0.1.2/pypods.egg-info/requires.txt
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)        7 2024-05-23 06:27:32.000000 pypods-0.1.2/pypods.egg-info/top_level.txt
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)       38 2024-05-23 06:27:32.237633 pypods-0.1.2/setup.cfg
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)      823 2024-05-23 06:25:43.000000 pypods-0.1.2/setup.py
```

### Comparing `pypods-0.1.1/LICENSE` & `pypods-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypods-0.1.1/PKG-INFO` & `pypods-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypods
-Version: 0.1.1
+Version: 0.1.2
 Summary: A lightweight solution to execute Python dependencies in an isolated fashion.
 Home-page: https://github.com/Rohan2002/pypods
 Author: Rohan Deshpande
 Author-email: rohandeshpande832@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pypods-0.1.1/README.md` & `pypods-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pypods-0.1.1/pypods/ns.py` & `pypods-0.1.2/pypods/ns.py`

 * *Files identical despite different names*

### Comparing `pypods-0.1.1/pypods/pods.py` & `pypods-0.1.2/pypods/pods.py`

 * *Files identical despite different names*

### Comparing `pypods-0.1.1/pypods.egg-info/PKG-INFO` & `pypods-0.1.2/pypods.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypods
-Version: 0.1.1
+Version: 0.1.2
 Summary: A lightweight solution to execute Python dependencies in an isolated fashion.
 Home-page: https://github.com/Rohan2002/pypods
 Author: Rohan Deshpande
 Author-email: rohandeshpande832@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pypods-0.1.1/setup.py` & `pypods-0.1.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 from pypods import __version__
 def read_requirements():
     with open('requirements.txt') as req:
         return req.read().splitlines()
 
 setup(
     name='pypods',
     version=__version__,
-    packages=find_packages(),
+    packages=["pypods", "pypods.template"],
     install_requires=read_requirements(),
     author='Rohan Deshpande',
     author_email='rohandeshpande832@gmail.com',
     description='A lightweight solution to execute Python dependencies in an isolated fashion.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Rohan2002/pypods',
```

