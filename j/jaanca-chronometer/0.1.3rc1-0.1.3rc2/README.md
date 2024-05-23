# Comparing `tmp/jaanca_chronometer-0.1.3rc1.tar.gz` & `tmp/jaanca_chronometer-0.1.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca_chronometer-0.1.3rc1.tar", last modified: Thu May 23 14:04:43 2024, max compression
+gzip compressed data, was "jaanca_chronometer-0.1.3rc2.tar", last modified: Thu May 23 14:19:34 2024, max compression
```

## Comparing `jaanca_chronometer-0.1.3rc1.tar` & `jaanca_chronometer-0.1.3rc2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 14:04:43.410712 jaanca_chronometer-0.1.3rc1/
--rw-rw-rw-   0        0        0     1092 2024-05-22 20:03:29.000000 jaanca_chronometer-0.1.3rc1/LICENSE.txt
--rw-rw-rw-   0        0        0     5066 2024-05-23 14:04:43.410712 jaanca_chronometer-0.1.3rc1/PKG-INFO
--rw-rw-rw-   0        0        0     3758 2024-05-23 14:03:04.000000 jaanca_chronometer-0.1.3rc1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 14:04:43.393047 jaanca_chronometer-0.1.3rc1/jaanca_chronometer/
--rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca_chronometer-0.1.3rc1/jaanca_chronometer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:04:43.403059 jaanca_chronometer-0.1.3rc1/jaanca_chronometer/utils/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.1.3rc1/jaanca_chronometer/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:04:43.406712 jaanca_chronometer-0.1.3rc1/jaanca_chronometer/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.1.3rc1/jaanca_chronometer/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     1651 2024-05-22 02:12:10.000000 jaanca_chronometer-0.1.3rc1/jaanca_chronometer/utils/helpers/chronometer.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:04:43.408713 jaanca_chronometer-0.1.3rc1/jaanca_chronometer.egg-info/
--rw-rw-rw-   0        0        0     5066 2024-05-23 14:04:43.000000 jaanca_chronometer-0.1.3rc1/jaanca_chronometer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2024-05-23 14:04:43.000000 jaanca_chronometer-0.1.3rc1/jaanca_chronometer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 14:04:43.000000 jaanca_chronometer-0.1.3rc1/jaanca_chronometer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-23 14:04:43.000000 jaanca_chronometer-0.1.3rc1/jaanca_chronometer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 14:04:43.412708 jaanca_chronometer-0.1.3rc1/setup.cfg
--rw-rw-rw-   0        0        0     1642 2024-05-23 14:04:08.000000 jaanca_chronometer-0.1.3rc1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:19:34.324462 jaanca_chronometer-0.1.3rc2/
+-rw-rw-rw-   0        0        0     1092 2024-05-22 20:03:29.000000 jaanca_chronometer-0.1.3rc2/LICENSE.txt
+-rw-rw-rw-   0        0        0     5335 2024-05-23 14:19:34.323463 jaanca_chronometer-0.1.3rc2/PKG-INFO
+-rw-rw-rw-   0        0        0     4027 2024-05-23 14:18:42.000000 jaanca_chronometer-0.1.3rc2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 14:19:34.305330 jaanca_chronometer-0.1.3rc2/jaanca_chronometer/
+-rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca_chronometer-0.1.3rc2/jaanca_chronometer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:19:34.316482 jaanca_chronometer-0.1.3rc2/jaanca_chronometer/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.1.3rc2/jaanca_chronometer/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:19:34.319698 jaanca_chronometer-0.1.3rc2/jaanca_chronometer/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.1.3rc2/jaanca_chronometer/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1651 2024-05-22 02:12:10.000000 jaanca_chronometer-0.1.3rc2/jaanca_chronometer/utils/helpers/chronometer.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:19:34.322464 jaanca_chronometer-0.1.3rc2/jaanca_chronometer.egg-info/
+-rw-rw-rw-   0        0        0     5335 2024-05-23 14:19:34.000000 jaanca_chronometer-0.1.3rc2/jaanca_chronometer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2024-05-23 14:19:34.000000 jaanca_chronometer-0.1.3rc2/jaanca_chronometer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 14:19:34.000000 jaanca_chronometer-0.1.3rc2/jaanca_chronometer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-23 14:19:34.000000 jaanca_chronometer-0.1.3rc2/jaanca_chronometer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 14:19:34.325467 jaanca_chronometer-0.1.3rc2/setup.cfg
+-rw-rw-rw-   0        0        0     1642 2024-05-23 14:18:59.000000 jaanca_chronometer-0.1.3rc2/setup.py
```

### Comparing `jaanca_chronometer-0.1.3rc1/LICENSE.txt` & `jaanca_chronometer-0.1.3rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca_chronometer-0.1.3rc1/PKG-INFO` & `jaanca_chronometer-0.1.3rc2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-chronometer
-Version: 0.1.3rc1
+Version: 0.1.3rc2
 Summary: A tool library created by jaanca that allows measuring the time between two moments in the source code.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-chronometer
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: timer stopwatch in interval format for databases
 Classifier: Development Status :: 4 - Beta
@@ -39,19 +39,23 @@
     <img src="https://img.shields.io/badge/Python-%5B%3E%3D3.8%2C%3C%3D3.11%5D-blue" alt="Python">
 </a>
 </p>
 
 
 ---
 
-# What libraries
+#  A tool library created by jaanca
 
 * **Python library**: A tool library created by jaanca that allows measuring the time between two moments in the source code.
 * **Analyze results in database**: The output format can be inserted in an INTERVAL attribute for example in PostgreSQL and add the time of several processes.
 
+[Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca-chronometer)
+| [Package (PyPI)](https://pypi.org/project/jaanca-chronometer/)
+| [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-chronometer/samples)
+
 ---
 
 # library installation
 ```console
 pip install jaanca-chronometer --upgrade
 ```
```

### Comparing `jaanca_chronometer-0.1.3rc1/README.md` & `jaanca_chronometer-0.1.3rc2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,19 +10,23 @@
     <img src="https://img.shields.io/badge/Python-%5B%3E%3D3.8%2C%3C%3D3.11%5D-blue" alt="Python">
 </a>
 </p>
 
 
 ---
 
-# What libraries
+#  A tool library created by jaanca
 
 * **Python library**: A tool library created by jaanca that allows measuring the time between two moments in the source code.
 * **Analyze results in database**: The output format can be inserted in an INTERVAL attribute for example in PostgreSQL and add the time of several processes.
 
+[Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca-chronometer)
+| [Package (PyPI)](https://pypi.org/project/jaanca-chronometer/)
+| [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-chronometer/samples)
+
 ---
 
 # library installation
 ```console
 pip install jaanca-chronometer --upgrade
 ```
```

### Comparing `jaanca_chronometer-0.1.3rc1/jaanca_chronometer/utils/helpers/chronometer.py` & `jaanca_chronometer-0.1.3rc2/jaanca_chronometer/utils/helpers/chronometer.py`

 * *Files identical despite different names*

### Comparing `jaanca_chronometer-0.1.3rc1/jaanca_chronometer.egg-info/PKG-INFO` & `jaanca_chronometer-0.1.3rc2/jaanca_chronometer.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-chronometer
-Version: 0.1.3rc1
+Version: 0.1.3rc2
 Summary: A tool library created by jaanca that allows measuring the time between two moments in the source code.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-chronometer
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: timer stopwatch in interval format for databases
 Classifier: Development Status :: 4 - Beta
@@ -39,19 +39,23 @@
     <img src="https://img.shields.io/badge/Python-%5B%3E%3D3.8%2C%3C%3D3.11%5D-blue" alt="Python">
 </a>
 </p>
 
 
 ---
 
-# What libraries
+#  A tool library created by jaanca
 
 * **Python library**: A tool library created by jaanca that allows measuring the time between two moments in the source code.
 * **Analyze results in database**: The output format can be inserted in an INTERVAL attribute for example in PostgreSQL and add the time of several processes.
 
+[Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca-chronometer)
+| [Package (PyPI)](https://pypi.org/project/jaanca-chronometer/)
+| [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-chronometer/samples)
+
 ---
 
 # library installation
 ```console
 pip install jaanca-chronometer --upgrade
 ```
```

### Comparing `jaanca_chronometer-0.1.3rc1/setup.py` & `jaanca_chronometer-0.1.3rc2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca-chronometer"
-VERSION = "0.1.3rc1"
+VERSION = "0.1.3rc2"
 
 install_requires = []
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'A tool library created by {COMPANY_NAME} that allows measuring the time between two moments in the source code.',
```

