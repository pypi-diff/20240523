# Comparing `tmp/dataprecf-0.7.0.tar.gz` & `tmp/dataprecf-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataprecf-0.7.0.tar", last modified: Thu May 23 16:41:06 2024, max compression
+gzip compressed data, was "dataprecf-0.8.0.tar", last modified: Thu May 23 16:49:43 2024, max compression
```

## Comparing `dataprecf-0.7.0.tar` & `dataprecf-0.8.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 16:41:06.861919 dataprecf-0.7.0/
--rw-rw-rw-   0        0        0      354 2024-05-23 16:41:06.855966 dataprecf-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     3777 2024-05-23 16:40:21.000000 dataprecf-0.7.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 16:41:06.787515 dataprecf-0.7.0/dataprecf/
-drwxrwxrwx   0        0        0        0 2024-05-23 16:41:06.851937 dataprecf-0.7.0/dataprecf/dataprecf.egg-info/
--rw-rw-rw-   0        0        0      354 2024-05-23 16:41:06.000000 dataprecf-0.7.0/dataprecf/dataprecf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2024-05-23 16:41:06.000000 dataprecf-0.7.0/dataprecf/dataprecf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 16:41:06.000000 dataprecf-0.7.0/dataprecf/dataprecf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-23 16:41:06.000000 dataprecf-0.7.0/dataprecf/dataprecf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 16:41:06.000000 dataprecf-0.7.0/dataprecf/dataprecf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 16:41:06.862916 dataprecf-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0      529 2024-05-23 16:40:34.000000 dataprecf-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:49:43.879874 dataprecf-0.8.0/
+-rw-rw-rw-   0        0        0     4325 2024-05-23 16:49:43.877884 dataprecf-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3777 2024-05-23 16:40:21.000000 dataprecf-0.8.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 16:49:43.846233 dataprecf-0.8.0/dataprecf/
+drwxrwxrwx   0        0        0        0 2024-05-23 16:49:43.875764 dataprecf-0.8.0/dataprecf/dataprecf.egg-info/
+-rw-rw-rw-   0        0        0     4325 2024-05-23 16:49:43.000000 dataprecf-0.8.0/dataprecf/dataprecf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-05-23 16:49:43.000000 dataprecf-0.8.0/dataprecf/dataprecf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 16:49:43.000000 dataprecf-0.8.0/dataprecf/dataprecf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-23 16:49:43.000000 dataprecf-0.8.0/dataprecf/dataprecf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 16:49:43.000000 dataprecf-0.8.0/dataprecf/dataprecf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      756 2024-05-23 16:49:43.884057 dataprecf-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0      561 2024-05-23 16:48:28.000000 dataprecf-0.8.0/setup.py
```

### Comparing `dataprecf-0.7.0/README.md` & `dataprecf-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `dataprecf-0.7.0/setup.py` & `dataprecf-0.8.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dataprecf',
-    version='0.7.0',
+    version='0.8.0',
     packages=find_packages(where='dataprecf'),
     install_requires=[
         'pandas',
         'numpy',
         'scikit-learn',
         'nltk',
     ],
     description='A data preprocessor for machine learning projects.',
     author='fatmanur caliskan, cihan yilmaz',
     author_email='fatmanur.caliskan@stu.fsm.edu.tr, cihan.yilmaz@stu.fsm.edu.tr',
     package_dir={'': 'dataprecf'},
+    include_package_data=True,
     python_requires='>=3.6',
 )
```

