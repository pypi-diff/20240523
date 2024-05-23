# Comparing `tmp/jaanca_chronometer-0.1.2.tar.gz` & `tmp/jaanca_chronometer-0.1.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca_chronometer-0.1.2.tar", last modified: Wed May 22 20:06:30 2024, max compression
+gzip compressed data, was "jaanca_chronometer-0.1.3rc1.tar", last modified: Thu May 23 14:04:43 2024, max compression
```

## Comparing `jaanca_chronometer-0.1.2.tar` & `jaanca_chronometer-0.1.3rc1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 20:06:30.126216 jaanca_chronometer-0.1.2/
--rw-rw-rw-   0        0        0     1092 2024-05-22 20:03:29.000000 jaanca_chronometer-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0     4589 2024-05-22 20:06:30.125218 jaanca_chronometer-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3299 2024-05-22 20:04:49.000000 jaanca_chronometer-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 20:06:30.109316 jaanca_chronometer-0.1.2/jaanca_chronometer/
--rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca_chronometer-0.1.2/jaanca_chronometer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 20:06:30.118219 jaanca_chronometer-0.1.2/jaanca_chronometer/utils/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.1.2/jaanca_chronometer/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 20:06:30.121213 jaanca_chronometer-0.1.2/jaanca_chronometer/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.1.2/jaanca_chronometer/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     1651 2024-05-22 02:12:10.000000 jaanca_chronometer-0.1.2/jaanca_chronometer/utils/helpers/chronometer.py
-drwxrwxrwx   0        0        0        0 2024-05-22 20:06:30.123215 jaanca_chronometer-0.1.2/jaanca_chronometer.egg-info/
--rw-rw-rw-   0        0        0     4589 2024-05-22 20:06:30.000000 jaanca_chronometer-0.1.2/jaanca_chronometer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2024-05-22 20:06:30.000000 jaanca_chronometer-0.1.2/jaanca_chronometer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 20:06:30.000000 jaanca_chronometer-0.1.2/jaanca_chronometer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-22 20:06:30.000000 jaanca_chronometer-0.1.2/jaanca_chronometer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 20:06:30.127214 jaanca_chronometer-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1624 2024-05-22 20:05:36.000000 jaanca_chronometer-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:04:43.410712 jaanca_chronometer-0.1.3rc1/
+-rw-rw-rw-   0        0        0     1092 2024-05-22 20:03:29.000000 jaanca_chronometer-0.1.3rc1/LICENSE.txt
+-rw-rw-rw-   0        0        0     5066 2024-05-23 14:04:43.410712 jaanca_chronometer-0.1.3rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     3758 2024-05-23 14:03:04.000000 jaanca_chronometer-0.1.3rc1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 14:04:43.393047 jaanca_chronometer-0.1.3rc1/jaanca_chronometer/
+-rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca_chronometer-0.1.3rc1/jaanca_chronometer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:04:43.403059 jaanca_chronometer-0.1.3rc1/jaanca_chronometer/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.1.3rc1/jaanca_chronometer/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:04:43.406712 jaanca_chronometer-0.1.3rc1/jaanca_chronometer/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.1.3rc1/jaanca_chronometer/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1651 2024-05-22 02:12:10.000000 jaanca_chronometer-0.1.3rc1/jaanca_chronometer/utils/helpers/chronometer.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:04:43.408713 jaanca_chronometer-0.1.3rc1/jaanca_chronometer.egg-info/
+-rw-rw-rw-   0        0        0     5066 2024-05-23 14:04:43.000000 jaanca_chronometer-0.1.3rc1/jaanca_chronometer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2024-05-23 14:04:43.000000 jaanca_chronometer-0.1.3rc1/jaanca_chronometer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 14:04:43.000000 jaanca_chronometer-0.1.3rc1/jaanca_chronometer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-23 14:04:43.000000 jaanca_chronometer-0.1.3rc1/jaanca_chronometer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 14:04:43.412708 jaanca_chronometer-0.1.3rc1/setup.cfg
+-rw-rw-rw-   0        0        0     1642 2024-05-23 14:04:08.000000 jaanca_chronometer-0.1.3rc1/setup.py
```

### Comparing `jaanca_chronometer-0.1.2/LICENSE.txt` & `jaanca_chronometer-0.1.3rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca_chronometer-0.1.2/PKG-INFO` & `jaanca_chronometer-0.1.3rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: jaanca-chronometer
-Version: 0.1.2
+Version: 0.1.3rc1
 Summary: A tool library created by jaanca that allows measuring the time between two moments in the source code.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-chronometer
-Author: Andres Cardona
+Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: timer stopwatch in interval format for databases
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
@@ -23,14 +23,30 @@
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
+<p align="center">
+    <em>jaanca public libraries</em>
+</p>
+
+<p align="center">
+<a href="https://pypi.org/project/jaanca-chronometer" target="_blank">
+    <img src="https://img.shields.io/pypi/v/jaanca-chronometer?color=blue&label=PyPI%20Package" alt="Package version">
+</a>
+<a href="(https://www.python.org" target="_blank">
+    <img src="https://img.shields.io/badge/Python-%5B%3E%3D3.8%2C%3C%3D3.11%5D-blue" alt="Python">
+</a>
+</p>
+
+
+---
+
 # What libraries
 
 * **Python library**: A tool library created by jaanca that allows measuring the time between two moments in the source code.
 * **Analyze results in database**: The output format can be inserted in an INTERVAL attribute for example in PostgreSQL and add the time of several processes.
 
 ---
```

### Comparing `jaanca_chronometer-0.1.2/README.md` & `jaanca_chronometer-0.1.3rc1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+<p align="center">
+    <em>jaanca public libraries</em>
+</p>
+
+<p align="center">
+<a href="https://pypi.org/project/jaanca-chronometer" target="_blank">
+    <img src="https://img.shields.io/pypi/v/jaanca-chronometer?color=blue&label=PyPI%20Package" alt="Package version">
+</a>
+<a href="(https://www.python.org" target="_blank">
+    <img src="https://img.shields.io/badge/Python-%5B%3E%3D3.8%2C%3C%3D3.11%5D-blue" alt="Python">
+</a>
+</p>
+
+
+---
+
 # What libraries
 
 * **Python library**: A tool library created by jaanca that allows measuring the time between two moments in the source code.
 * **Analyze results in database**: The output format can be inserted in an INTERVAL attribute for example in PostgreSQL and add the time of several processes.
 
 ---
```

### Comparing `jaanca_chronometer-0.1.2/jaanca_chronometer/utils/helpers/chronometer.py` & `jaanca_chronometer-0.1.3rc1/jaanca_chronometer/utils/helpers/chronometer.py`

 * *Files identical despite different names*

### Comparing `jaanca_chronometer-0.1.2/jaanca_chronometer.egg-info/PKG-INFO` & `jaanca_chronometer-0.1.3rc1/jaanca_chronometer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: jaanca-chronometer
-Version: 0.1.2
+Version: 0.1.3rc1
 Summary: A tool library created by jaanca that allows measuring the time between two moments in the source code.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-chronometer
-Author: Andres Cardona
+Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: timer stopwatch in interval format for databases
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
@@ -23,14 +23,30 @@
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
+<p align="center">
+    <em>jaanca public libraries</em>
+</p>
+
+<p align="center">
+<a href="https://pypi.org/project/jaanca-chronometer" target="_blank">
+    <img src="https://img.shields.io/pypi/v/jaanca-chronometer?color=blue&label=PyPI%20Package" alt="Package version">
+</a>
+<a href="(https://www.python.org" target="_blank">
+    <img src="https://img.shields.io/badge/Python-%5B%3E%3D3.8%2C%3C%3D3.11%5D-blue" alt="Python">
+</a>
+</p>
+
+
+---
+
 # What libraries
 
 * **Python library**: A tool library created by jaanca that allows measuring the time between two moments in the source code.
 * **Analyze results in database**: The output format can be inserted in an INTERVAL attribute for example in PostgreSQL and add the time of several processes.
 
 ---
```

### Comparing `jaanca_chronometer-0.1.2/setup.py` & `jaanca_chronometer-0.1.3rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca-chronometer"
-VERSION = "0.1.2"
+VERSION = "0.1.3rc1"
 
 install_requires = []
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'A tool library created by {COMPANY_NAME} that allows measuring the time between two moments in the source code.',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     license='MIT License',
-    author='Andres Cardona',
+    author='Jaime Andres Cardona Carrillo',
     author_email='jacardona@outlook.com',
     url='https://github.com/jaanca/python-libraries/tree/main/jaanca-chronometer',
     keywords="timer stopwatch in interval format for databases",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
```

