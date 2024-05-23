# Comparing `tmp/Complex_Bidintha-0.4.tar.gz` & `tmp/Complex_Bidintha-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Complex_Bidintha-0.4.tar", last modified: Thu May 23 09:36:57 2024, max compression
+gzip compressed data, was "Complex_Bidintha-0.5.tar", last modified: Thu May 23 09:47:56 2024, max compression
```

## Comparing `Complex_Bidintha-0.4.tar` & `Complex_Bidintha-0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 09:36:57.549197 Complex_Bidintha-0.4/
-drwxrwxrwx   0        0        0        0 2024-05-23 09:36:57.528554 Complex_Bidintha-0.4/Complex/
--rw-rw-rw-   0        0        0     1727 2024-05-23 08:41:16.000000 Complex_Bidintha-0.4/Complex/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 09:36:57.546704 Complex_Bidintha-0.4/Complex_Bidintha.egg-info/
--rw-rw-rw-   0        0        0      242 2024-05-23 09:36:57.000000 Complex_Bidintha-0.4/Complex_Bidintha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-05-23 09:36:57.000000 Complex_Bidintha-0.4/Complex_Bidintha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 09:36:57.000000 Complex_Bidintha-0.4/Complex_Bidintha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-23 09:36:57.000000 Complex_Bidintha-0.4/Complex_Bidintha.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2024-05-23 09:29:42.000000 Complex_Bidintha-0.4/License.txt
--rw-rw-rw-   0        0        0      242 2024-05-23 09:36:57.546704 Complex_Bidintha-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1276 2024-05-23 09:28:44.000000 Complex_Bidintha-0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 09:36:57.549197 Complex_Bidintha-0.4/setup.cfg
--rw-rw-rw-   0        0        0     1157 2024-05-23 09:36:53.000000 Complex_Bidintha-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:47:56.462754 Complex_Bidintha-0.5/
+drwxrwxrwx   0        0        0        0 2024-05-23 09:47:56.436321 Complex_Bidintha-0.5/Complex/
+-rw-rw-rw-   0        0        0     1727 2024-05-23 08:41:16.000000 Complex_Bidintha-0.5/Complex/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:47:56.459096 Complex_Bidintha-0.5/Complex_Bidintha.egg-info/
+-rw-rw-rw-   0        0        0     1575 2024-05-23 09:47:56.000000 Complex_Bidintha-0.5/Complex_Bidintha.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-05-23 09:47:56.000000 Complex_Bidintha-0.5/Complex_Bidintha.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 09:47:56.000000 Complex_Bidintha-0.5/Complex_Bidintha.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-23 09:47:56.000000 Complex_Bidintha-0.5/Complex_Bidintha.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2024-05-23 09:29:42.000000 Complex_Bidintha-0.5/License.txt
+-rw-rw-rw-   0        0        0     1575 2024-05-23 09:47:56.461987 Complex_Bidintha-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1276 2024-05-23 09:28:44.000000 Complex_Bidintha-0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 09:47:56.462754 Complex_Bidintha-0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1253 2024-05-23 09:47:06.000000 Complex_Bidintha-0.5/setup.py
```

### Comparing `Complex_Bidintha-0.4/Complex/__init__.py` & `Complex_Bidintha-0.5/Complex/__init__.py`

 * *Files identical despite different names*

### Comparing `Complex_Bidintha-0.4/License.txt` & `Complex_Bidintha-0.5/License.txt`

 * *Files identical despite different names*

### Comparing `Complex_Bidintha-0.4/README.md` & `Complex_Bidintha-0.5/README.md`

 * *Files identical despite different names*

### Comparing `Complex_Bidintha-0.4/setup.py` & `Complex_Bidintha-0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from setuptools import setup,find_packages
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "Complex_Bidintha",
-    version="0.4",
+    version="0.5",
     packages=find_packages(),
     author="Bidintha Machahry",
     author_email="bidintha2006@gmail.com",
     description="Complex Numbers",
     license="License.txt",
-    long_description_content_type="text/markdown"
+    url="https://github.com/MrS0lver/Complex_Number",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
 )
 #     long_description="""
 # The ComplexNumbers package provides a simple implementation of complex numbers in Python. The package includes a Complex class with support for basic arithmetic operations such as addition, subtraction, multiplication, and division of complex numbers. Additionally, the class provides methods for calculating the absolute value (magnitude) of a complex number and comparing complex numbers for equality and inequality.
 
 # Features:\n
 # (*) Implements complex numbers with real and imaginary parts.\n
 # (*) Supports arithmetic operations: addition, subtraction, multiplication, and division.\n
```

