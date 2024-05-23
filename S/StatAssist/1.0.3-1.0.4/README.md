# Comparing `tmp/StatAssist-1.0.3.tar.gz` & `tmp/StatAssist-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StatAssist-1.0.3.tar", last modified: Sun May 19 23:04:13 2024, max compression
+gzip compressed data, was "StatAssist-1.0.4.tar", last modified: Thu May 23 01:45:58 2024, max compression
```

## Comparing `StatAssist-1.0.3.tar` & `StatAssist-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 23:04:13.640415 StatAssist-1.0.3/
--rw-rw-rw-   0        0        0     2221 2024-05-19 23:04:13.640415 StatAssist-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1745 2024-05-19 20:02:54.000000 StatAssist-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 23:04:13.624819 StatAssist-1.0.3/StatAssist/
--rw-rw-rw-   0        0        0      285 2024-05-19 23:02:09.000000 StatAssist-1.0.3/StatAssist/__init__.py
--rw-rw-rw-   0        0        0     2358 2024-05-19 19:35:48.000000 StatAssist-1.0.3/StatAssist/algebra.py
--rw-rw-rw-   0        0        0    15935 2024-05-19 23:03:32.000000 StatAssist-1.0.3/StatAssist/stats.py
--rw-rw-rw-   0        0        0     7153 2024-05-19 19:46:17.000000 StatAssist-1.0.3/StatAssist/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-19 23:04:13.640415 StatAssist-1.0.3/StatAssist.egg-info/
--rw-rw-rw-   0        0        0     2221 2024-05-19 23:04:13.000000 StatAssist-1.0.3/StatAssist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-05-19 23:04:13.000000 StatAssist-1.0.3/StatAssist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 23:04:13.000000 StatAssist-1.0.3/StatAssist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-19 23:04:13.000000 StatAssist-1.0.3/StatAssist.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-19 23:04:13.000000 StatAssist-1.0.3/StatAssist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 23:04:13.640415 StatAssist-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      788 2024-05-19 23:01:58.000000 StatAssist-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:45:58.891928 StatAssist-1.0.4/
+-rw-rw-rw-   0        0        0     2253 2024-05-23 01:45:58.891928 StatAssist-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1745 2024-05-20 00:10:03.000000 StatAssist-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 01:45:58.876268 StatAssist-1.0.4/StatAssist/
+-rw-rw-rw-   0        0        0      285 2024-05-23 01:43:37.000000 StatAssist-1.0.4/StatAssist/__init__.py
+-rw-rw-rw-   0        0        0     2358 2024-05-19 19:35:48.000000 StatAssist-1.0.4/StatAssist/algebra.py
+-rw-rw-rw-   0        0        0    15935 2024-05-20 05:11:46.000000 StatAssist-1.0.4/StatAssist/stats.py
+-rw-rw-rw-   0        0        0    10009 2024-05-23 01:43:25.000000 StatAssist-1.0.4/StatAssist/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:45:58.891928 StatAssist-1.0.4/StatAssist.egg-info/
+-rw-rw-rw-   0        0        0     2253 2024-05-23 01:45:58.000000 StatAssist-1.0.4/StatAssist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-05-23 01:45:58.000000 StatAssist-1.0.4/StatAssist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 01:45:58.000000 StatAssist-1.0.4/StatAssist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-23 01:45:58.000000 StatAssist-1.0.4/StatAssist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-23 01:45:58.000000 StatAssist-1.0.4/StatAssist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 01:45:58.891928 StatAssist-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      816 2024-05-23 01:43:48.000000 StatAssist-1.0.4/setup.py
```

### Comparing `StatAssist-1.0.3/PKG-INFO` & `StatAssist-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: StatAssist
-Version: 1.0.3
+Version: 1.0.4
 Summary: Math tools for private or personal use.
 Author: Damion J. Quintanilla
 Author-email: djq314159@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.3.0
 Requires-Dist: pandas>=2.2.2
 Requires-Dist: scikit-learn>=1.4.2
+Requires-Dist: openpyxl>=3.1.2
 
 # StatAssist
 
 StatAssist is a python library that provides statistical and mathematical functions as well as built-in algorithms such
 as integration and linear regression.
 
 ## Installation
 
 You can install StatAssist using pip:
 
-pip install StatAssist==1.0.2
+pip install StatAssist==1.0.3
 
 ## Usage
 
 Example 1:
 
 ```python
 from StatAssist import statistics_ as stats
```

### Comparing `StatAssist-1.0.3/README.md` & `StatAssist-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 StatAssist is a python library that provides statistical and mathematical functions as well as built-in algorithms such
 as integration and linear regression.
 
 ## Installation
 
 You can install StatAssist using pip:
 
-pip install StatAssist==1.0.2
+pip install StatAssist==1.0.3
 
 ## Usage
 
 Example 1:
 
 ```python
 from StatAssist import statistics_ as stats
```

### Comparing `StatAssist-1.0.3/StatAssist/algebra.py` & `StatAssist-1.0.4/StatAssist/algebra.py`

 * *Files identical despite different names*

### Comparing `StatAssist-1.0.3/StatAssist/stats.py` & `StatAssist-1.0.4/StatAssist/stats.py`

 * *Files identical despite different names*

### Comparing `StatAssist-1.0.3/StatAssist.egg-info/PKG-INFO` & `StatAssist-1.0.4/StatAssist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: StatAssist
-Version: 1.0.3
+Version: 1.0.4
 Summary: Math tools for private or personal use.
 Author: Damion J. Quintanilla
 Author-email: djq314159@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.3.0
 Requires-Dist: pandas>=2.2.2
 Requires-Dist: scikit-learn>=1.4.2
+Requires-Dist: openpyxl>=3.1.2
 
 # StatAssist
 
 StatAssist is a python library that provides statistical and mathematical functions as well as built-in algorithms such
 as integration and linear regression.
 
 ## Installation
 
 You can install StatAssist using pip:
 
-pip install StatAssist==1.0.2
+pip install StatAssist==1.0.3
 
 ## Usage
 
 Example 1:
 
 ```python
 from StatAssist import statistics_ as stats
```

### Comparing `StatAssist-1.0.3/setup.py` & `StatAssist-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="StatAssist",
-    version="1.0.3",
+    version="1.0.4",
     license='MIT',
     author="Damion J. Quintanilla",
     author_email="djq314159@gmail.com",
     description="Math tools for private or personal use.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=[
         'torch>=2.3.0',
         'pandas>=2.2.2',
         'scikit-learn>=1.4.2',
+        'openpyxl>=3.1.2',
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_reqires='>=3.6',
```

