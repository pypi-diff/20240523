# Comparing `tmp/Complex_Bidintha-0.2.tar.gz` & `tmp/Complex_Bidintha-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Complex_Bidintha-0.2.tar", last modified: Thu May 23 09:24:56 2024, max compression
+gzip compressed data, was "Complex_Bidintha-0.3.tar", last modified: Thu May 23 09:30:09 2024, max compression
```

## Comparing `Complex_Bidintha-0.2.tar` & `Complex_Bidintha-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 09:24:56.102589 Complex_Bidintha-0.2/
-drwxrwxrwx   0        0        0        0 2024-05-23 09:24:56.093032 Complex_Bidintha-0.2/Complex/
--rw-rw-rw-   0        0        0     1727 2024-05-23 08:41:16.000000 Complex_Bidintha-0.2/Complex/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 09:24:56.102589 Complex_Bidintha-0.2/Complex_Bidintha.egg-info/
--rw-rw-rw-   0        0        0      880 2024-05-23 09:24:55.000000 Complex_Bidintha-0.2/Complex_Bidintha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-05-23 09:24:56.000000 Complex_Bidintha-0.2/Complex_Bidintha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 09:24:55.000000 Complex_Bidintha-0.2/Complex_Bidintha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-23 09:24:55.000000 Complex_Bidintha-0.2/Complex_Bidintha.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-05-23 08:08:20.000000 Complex_Bidintha-0.2/License.txt
--rw-rw-rw-   0        0        0      880 2024-05-23 09:24:56.102589 Complex_Bidintha-0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-23 08:08:09.000000 Complex_Bidintha-0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 09:24:56.102589 Complex_Bidintha-0.2/setup.cfg
--rw-rw-rw-   0        0        0      977 2024-05-23 09:20:44.000000 Complex_Bidintha-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:30:09.252948 Complex_Bidintha-0.3/
+drwxrwxrwx   0        0        0        0 2024-05-23 09:30:09.235875 Complex_Bidintha-0.3/Complex/
+-rw-rw-rw-   0        0        0     1727 2024-05-23 08:41:16.000000 Complex_Bidintha-0.3/Complex/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:30:09.252948 Complex_Bidintha-0.3/Complex_Bidintha.egg-info/
+-rw-rw-rw-   0        0        0      886 2024-05-23 09:30:09.000000 Complex_Bidintha-0.3/Complex_Bidintha.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-05-23 09:30:09.000000 Complex_Bidintha-0.3/Complex_Bidintha.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 09:30:09.000000 Complex_Bidintha-0.3/Complex_Bidintha.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-23 09:30:09.000000 Complex_Bidintha-0.3/Complex_Bidintha.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2024-05-23 09:29:42.000000 Complex_Bidintha-0.3/License.txt
+-rw-rw-rw-   0        0        0      886 2024-05-23 09:30:09.252948 Complex_Bidintha-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1276 2024-05-23 09:28:44.000000 Complex_Bidintha-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 09:30:09.252948 Complex_Bidintha-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-05-23 09:29:53.000000 Complex_Bidintha-0.3/setup.py
```

### Comparing `Complex_Bidintha-0.2/Complex/__init__.py` & `Complex_Bidintha-0.3/Complex/__init__.py`

 * *Files identical despite different names*

### Comparing `Complex_Bidintha-0.2/Complex_Bidintha.egg-info/PKG-INFO` & `Complex_Bidintha-0.3/Complex_Bidintha.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: Complex-Bidintha
-Version: 0.2
+Version: 0.3
 Summary: Complex Numbers
 Author: Bidintha Machahry
 Author-email: bidintha2006@gmail.com
 License-File: License.txt
 
 Description:
 The ComplexNumbers package provides a simple implementation of complex numbers in Python. The package includes a Complex class with support for basic arithmetic operations such as addition, subtraction, multiplication, and division of complex numbers. Additionally, the class provides methods for calculating the absolute value (magnitude) of a complex number and comparing complex numbers for equality and inequality.
 
 Features:
 Implements complex numbers with real and imaginary parts.
+
 Supports arithmetic operations: addition, subtraction, multiplication, and division.
+
 Provides methods for absolute value calculation and comparison.
+
 Designed for simplicity and ease of use.
```

### Comparing `Complex_Bidintha-0.2/PKG-INFO` & `Complex_Bidintha-0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: Complex_Bidintha
-Version: 0.2
+Version: 0.3
 Summary: Complex Numbers
 Author: Bidintha Machahry
 Author-email: bidintha2006@gmail.com
 License-File: License.txt
 
 Description:
 The ComplexNumbers package provides a simple implementation of complex numbers in Python. The package includes a Complex class with support for basic arithmetic operations such as addition, subtraction, multiplication, and division of complex numbers. Additionally, the class provides methods for calculating the absolute value (magnitude) of a complex number and comparing complex numbers for equality and inequality.
 
 Features:
 Implements complex numbers with real and imaginary parts.
+
 Supports arithmetic operations: addition, subtraction, multiplication, and division.
+
 Provides methods for absolute value calculation and comparison.
+
 Designed for simplicity and ease of use.
```

### Comparing `Complex_Bidintha-0.2/setup.py` & `Complex_Bidintha-0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup,find_packages
 
 setup(
     name = "Complex_Bidintha",
-    version="0.2",
+    version="0.3",
     packages=find_packages(),
     author="Bidintha Machahry",
     author_email="bidintha2006@gmail.com",
     description="Complex Numbers",
     long_description="""Description:
 The ComplexNumbers package provides a simple implementation of complex numbers in Python. The package includes a Complex class with support for basic arithmetic operations such as addition, subtraction, multiplication, and division of complex numbers. Additionally, the class provides methods for calculating the absolute value (magnitude) of a complex number and comparing complex numbers for equality and inequality.
 
 Features:
-Implements complex numbers with real and imaginary parts.
-Supports arithmetic operations: addition, subtraction, multiplication, and division.
-Provides methods for absolute value calculation and comparison.
+Implements complex numbers with real and imaginary parts.\n
+Supports arithmetic operations: addition, subtraction, multiplication, and division.\n
+Provides methods for absolute value calculation and comparison.\n
 Designed for simplicity and ease of use."""
 )
```

