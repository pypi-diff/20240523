# Comparing `tmp/dataprecf-0.6.0.tar.gz` & `tmp/dataprecf-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataprecf-0.6.0.tar", last modified: Thu May 23 16:28:08 2024, max compression
+gzip compressed data, was "dataprecf-0.7.0.tar", last modified: Thu May 23 16:41:06 2024, max compression
```

## Comparing `dataprecf-0.6.0.tar` & `dataprecf-0.7.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 16:28:08.109532 dataprecf-0.6.0/
--rw-rw-rw-   0        0        0     4335 2024-05-23 16:28:08.106303 dataprecf-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     3787 2024-05-23 15:59:58.000000 dataprecf-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 16:28:08.016041 dataprecf-0.6.0/dataprecf/
-drwxrwxrwx   0        0        0        0 2024-05-23 16:28:08.098966 dataprecf-0.6.0/dataprecf/dataprecf.egg-info/
--rw-rw-rw-   0        0        0     4335 2024-05-23 16:28:07.000000 dataprecf-0.6.0/dataprecf/dataprecf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-05-23 16:28:07.000000 dataprecf-0.6.0/dataprecf/dataprecf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 16:28:07.000000 dataprecf-0.6.0/dataprecf/dataprecf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-23 16:28:07.000000 dataprecf-0.6.0/dataprecf/dataprecf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 16:28:07.000000 dataprecf-0.6.0/dataprecf/dataprecf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      684 2024-05-23 16:28:08.115091 dataprecf-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0      529 2024-05-23 16:26:54.000000 dataprecf-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:41:06.861919 dataprecf-0.7.0/
+-rw-rw-rw-   0        0        0      354 2024-05-23 16:41:06.855966 dataprecf-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3777 2024-05-23 16:40:21.000000 dataprecf-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 16:41:06.787515 dataprecf-0.7.0/dataprecf/
+drwxrwxrwx   0        0        0        0 2024-05-23 16:41:06.851937 dataprecf-0.7.0/dataprecf/dataprecf.egg-info/
+-rw-rw-rw-   0        0        0      354 2024-05-23 16:41:06.000000 dataprecf-0.7.0/dataprecf/dataprecf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2024-05-23 16:41:06.000000 dataprecf-0.7.0/dataprecf/dataprecf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 16:41:06.000000 dataprecf-0.7.0/dataprecf/dataprecf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-23 16:41:06.000000 dataprecf-0.7.0/dataprecf/dataprecf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 16:41:06.000000 dataprecf-0.7.0/dataprecf/dataprecf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 16:41:06.862916 dataprecf-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      529 2024-05-23 16:40:34.000000 dataprecf-0.7.0/setup.py
```

### Comparing `dataprecf-0.6.0/PKG-INFO` & `dataprecf-0.7.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,17 @@
-Metadata-Version: 2.1
-Name: dataprecf
-Version: 0.6.0
-Summary: A data preprocessor for machine learning projects.
-Author: fatmanur caliskan, cihan yilmaz
-Author-email: fatmanur.caliskan@stu.fsm.edu.tr, cihan.yilmaz@stu.fsm.edu.tr
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Requires-Dist: pandas
-Requires-Dist: numpy
-Requires-Dist: scikit-learn
-Requires-Dist: nltk
-
 # cf_datapreprocessor
 
 cf_datapreprocessor is a Python package that simplifies data preprocessing steps for machine learning projects. This package provides various data preprocessing tools, including handling missing values, detecting and correcting outliers, data scaling, text cleaning, encoding categorical data, and more.
 
 ## Installation
 
 To install the package, follow these steps:
 
 ```sh
-pip install cf_datapreprocessor
+pip install dataprecf
 Usage
 1. Handling Missing Values (missing_value_handler)
 You can fill missing values with mean, median, or a constant value, or you can remove the missing data.
 
 from dataPreprocessor.missing_value_handler import missing_value_handler
 
 handler = missing_value_handler()
@@ -134,8 +118,8 @@
 nltk
 Contact
 If you have any questions or would like to contribute, please contact:
 
 Fatmanur Caliskan: fatmanur.caliskan@stu.fsm.edu.tr
 Cihan Yilmaz: cihan.yilmaz@stu.fsm.edu.tr
 
-Feel free to further customize the content as needed.
+Feel free to further customize the content as needed.
```

### Comparing `dataprecf-0.6.0/setup.py` & `dataprecf-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dataprecf',
-    version='0.6.0',
+    version='0.7.0',
     packages=find_packages(where='dataprecf'),
     install_requires=[
         'pandas',
         'numpy',
         'scikit-learn',
         'nltk',
     ],
```

