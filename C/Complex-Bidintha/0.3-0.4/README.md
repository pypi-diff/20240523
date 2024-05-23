# Comparing `tmp/Complex_Bidintha-0.3.tar.gz` & `tmp/Complex_Bidintha-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Complex_Bidintha-0.3.tar", last modified: Thu May 23 09:30:09 2024, max compression
+gzip compressed data, was "Complex_Bidintha-0.4.tar", last modified: Thu May 23 09:36:57 2024, max compression
```

## Comparing `Complex_Bidintha-0.3.tar` & `Complex_Bidintha-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 09:30:09.252948 Complex_Bidintha-0.3/
-drwxrwxrwx   0        0        0        0 2024-05-23 09:30:09.235875 Complex_Bidintha-0.3/Complex/
--rw-rw-rw-   0        0        0     1727 2024-05-23 08:41:16.000000 Complex_Bidintha-0.3/Complex/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 09:30:09.252948 Complex_Bidintha-0.3/Complex_Bidintha.egg-info/
--rw-rw-rw-   0        0        0      886 2024-05-23 09:30:09.000000 Complex_Bidintha-0.3/Complex_Bidintha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-05-23 09:30:09.000000 Complex_Bidintha-0.3/Complex_Bidintha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 09:30:09.000000 Complex_Bidintha-0.3/Complex_Bidintha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-23 09:30:09.000000 Complex_Bidintha-0.3/Complex_Bidintha.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2024-05-23 09:29:42.000000 Complex_Bidintha-0.3/License.txt
--rw-rw-rw-   0        0        0      886 2024-05-23 09:30:09.252948 Complex_Bidintha-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1276 2024-05-23 09:28:44.000000 Complex_Bidintha-0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 09:30:09.252948 Complex_Bidintha-0.3/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-05-23 09:29:53.000000 Complex_Bidintha-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:36:57.549197 Complex_Bidintha-0.4/
+drwxrwxrwx   0        0        0        0 2024-05-23 09:36:57.528554 Complex_Bidintha-0.4/Complex/
+-rw-rw-rw-   0        0        0     1727 2024-05-23 08:41:16.000000 Complex_Bidintha-0.4/Complex/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:36:57.546704 Complex_Bidintha-0.4/Complex_Bidintha.egg-info/
+-rw-rw-rw-   0        0        0      242 2024-05-23 09:36:57.000000 Complex_Bidintha-0.4/Complex_Bidintha.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-05-23 09:36:57.000000 Complex_Bidintha-0.4/Complex_Bidintha.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 09:36:57.000000 Complex_Bidintha-0.4/Complex_Bidintha.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-23 09:36:57.000000 Complex_Bidintha-0.4/Complex_Bidintha.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2024-05-23 09:29:42.000000 Complex_Bidintha-0.4/License.txt
+-rw-rw-rw-   0        0        0      242 2024-05-23 09:36:57.546704 Complex_Bidintha-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1276 2024-05-23 09:28:44.000000 Complex_Bidintha-0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 09:36:57.549197 Complex_Bidintha-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1157 2024-05-23 09:36:53.000000 Complex_Bidintha-0.4/setup.py
```

### Comparing `Complex_Bidintha-0.3/Complex/__init__.py` & `Complex_Bidintha-0.4/Complex/__init__.py`

 * *Files identical despite different names*

### Comparing `Complex_Bidintha-0.3/Complex_Bidintha.egg-info/PKG-INFO` & `Complex_Bidintha-0.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-Metadata-Version: 2.1
-Name: Complex-Bidintha
-Version: 0.3
-Summary: Complex Numbers
-Author: Bidintha Machahry
-Author-email: bidintha2006@gmail.com
-License-File: License.txt
+# ComplexNumbers
 
-Description:
-The ComplexNumbers package provides a simple implementation of complex numbers in Python. The package includes a Complex class with support for basic arithmetic operations such as addition, subtraction, multiplication, and division of complex numbers. Additionally, the class provides methods for calculating the absolute value (magnitude) of a complex number and comparing complex numbers for equality and inequality.
+[![PyPI version](https://img.shields.io/pypi/v/Complex_Bidintha.svg)](https://pypi.org/project/Complex_Bidintha/)
+[![License](https://img.shields.io/pypi/l/Complex_Bidintha.svg)](https://opensource.org/licenses/MIT)
+[![Python Versions](https://img.shields.io/pypi/pyversions/Complex_Bidintha.svg)](https://pypi.org/project/Complex_Bidintha/)
+[![Downloads](https://pepy.tech/badge/complex-bidintha)](https://pepy.tech/project/complex-bidintha)
 
-Features:
-Implements complex numbers with real and imaginary parts.
+The ComplexNumbers package provides a simple implementation of complex numbers in Python. It includes a `Complex` class with support for basic arithmetic operations such as addition, subtraction, multiplication, and division of complex numbers. Additionally, the class provides methods for calculating the absolute value (magnitude) of a complex number and comparing complex numbers for equality and inequality.
 
-Supports arithmetic operations: addition, subtraction, multiplication, and division.
+## Features
 
-Provides methods for absolute value calculation and comparison.
+- Implements complex numbers with real and imaginary parts.
+- Supports arithmetic operations: addition, subtraction, multiplication, and division.
+- Provides methods for absolute value calculation and comparison.
+- Designed for simplicity and ease of use.
 
-Designed for simplicity and ease of use.
+## Installation
+
+You can install the ComplexNumbers package using pip:
+
+```bash
+pip install Complex_Bidintha
```

### Comparing `Complex_Bidintha-0.3/License.txt` & `Complex_Bidintha-0.4/License.txt`

 * *Files identical despite different names*

### Comparing `Complex_Bidintha-0.3/setup.py` & `Complex_Bidintha-0.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from setuptools import setup,find_packages
+with open("README.md", "r") as fh:
+    long_description = fh.read()
 
 setup(
     name = "Complex_Bidintha",
-    version="0.3",
+    version="0.4",
     packages=find_packages(),
     author="Bidintha Machahry",
     author_email="bidintha2006@gmail.com",
     description="Complex Numbers",
-    long_description="""Description:
-The ComplexNumbers package provides a simple implementation of complex numbers in Python. The package includes a Complex class with support for basic arithmetic operations such as addition, subtraction, multiplication, and division of complex numbers. Additionally, the class provides methods for calculating the absolute value (magnitude) of a complex number and comparing complex numbers for equality and inequality.
+    license="License.txt",
+    long_description_content_type="text/markdown"
+)
+#     long_description="""
+# The ComplexNumbers package provides a simple implementation of complex numbers in Python. The package includes a Complex class with support for basic arithmetic operations such as addition, subtraction, multiplication, and division of complex numbers. Additionally, the class provides methods for calculating the absolute value (magnitude) of a complex number and comparing complex numbers for equality and inequality.
 
-Features:
-Implements complex numbers with real and imaginary parts.\n
-Supports arithmetic operations: addition, subtraction, multiplication, and division.\n
-Provides methods for absolute value calculation and comparison.\n
-Designed for simplicity and ease of use."""
-)
+# Features:\n
+# (*) Implements complex numbers with real and imaginary parts.\n
+# (*) Supports arithmetic operations: addition, subtraction, multiplication, and division.\n
+# (*) Provides methods for absolute value calculation and comparison.\n
+# (*) Designed for simplicity and ease of use."""
+# )
```
