# Comparing `tmp/preprocessinglib_tonga_gumustakim-0.2.tar.gz` & `tmp/preprocessinglib_tonga_gumustakim-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preprocessinglib_tonga_gumustakim-0.2.tar", last modified: Thu May 23 09:37:45 2024, max compression
+gzip compressed data, was "preprocessinglib_tonga_gumustakim-0.3.tar", last modified: Thu May 23 09:39:12 2024, max compression
```

## Comparing `preprocessinglib_tonga_gumustakim-0.2.tar` & `preprocessinglib_tonga_gumustakim-0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 09:37:45.055498 preprocessinglib_tonga_gumustakim-0.2/
--rw-rw-rw-   0        0        0     3230 2024-05-23 09:37:45.054501 preprocessinglib_tonga_gumustakim-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2546 2024-05-21 20:13:01.000000 preprocessinglib_tonga_gumustakim-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 09:37:45.021352 preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim/
--rw-rw-rw-   0        0        0      664 2024-05-21 15:21:25.000000 preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim/CategoricalEncoder.py
--rw-rw-rw-   0        0        0      459 2024-05-21 15:31:42.000000 preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim/DataTypeConverter.py
--rw-rw-rw-   0        0        0      380 2024-05-21 17:04:39.000000 preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim/DateTimeHandler.py
--rw-rw-rw-   0        0        0      212 2024-05-21 15:39:43.000000 preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim/FeatureEngineer.py
--rw-rw-rw-   0        0        0      920 2024-05-21 15:41:03.000000 preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim/MissingValueHandler.py
--rw-rw-rw-   0        0        0      711 2024-05-21 16:01:47.000000 preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim/OutlierHandler.py
--rw-rw-rw-   0        0        0      510 2024-05-21 15:31:42.000000 preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim/Scaler.py
--rw-rw-rw-   0        0        0     4903 2024-05-23 09:29:07.000000 preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim/TestDataPreprocessing.py
--rw-rw-rw-   0        0        0      665 2024-05-21 15:42:19.000000 preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim/TextCleaner.py
--rw-rw-rw-   0        0        0      255 2024-05-23 09:29:07.000000 preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 09:37:45.053000 preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim.egg-info/
--rw-rw-rw-   0        0        0     3230 2024-05-23 09:37:44.000000 preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      826 2024-05-23 09:37:44.000000 preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 09:37:44.000000 preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-23 09:37:44.000000 preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2024-05-23 09:37:44.000000 preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 09:37:45.056494 preprocessinglib_tonga_gumustakim-0.2/setup.cfg
--rw-rw-rw-   0        0        0      898 2024-05-23 09:29:07.000000 preprocessinglib_tonga_gumustakim-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:39:12.126339 preprocessinglib_tonga_gumustakim-0.3/
+-rw-rw-rw-   0        0        0     3230 2024-05-23 09:39:12.124848 preprocessinglib_tonga_gumustakim-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2546 2024-05-21 20:13:01.000000 preprocessinglib_tonga_gumustakim-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 09:39:12.102228 preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim/
+-rw-rw-rw-   0        0        0      664 2024-05-21 15:21:25.000000 preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim/CategoricalEncoder.py
+-rw-rw-rw-   0        0        0      459 2024-05-21 15:31:42.000000 preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim/DataTypeConverter.py
+-rw-rw-rw-   0        0        0      380 2024-05-21 17:04:39.000000 preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim/DateTimeHandler.py
+-rw-rw-rw-   0        0        0      212 2024-05-21 15:39:43.000000 preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim/FeatureEngineer.py
+-rw-rw-rw-   0        0        0      920 2024-05-21 15:41:03.000000 preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim/MissingValueHandler.py
+-rw-rw-rw-   0        0        0      711 2024-05-21 16:01:47.000000 preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim/OutlierHandler.py
+-rw-rw-rw-   0        0        0      510 2024-05-21 15:31:42.000000 preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim/Scaler.py
+-rw-rw-rw-   0        0        0     4903 2024-05-23 09:29:07.000000 preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim/TestDataPreprocessing.py
+-rw-rw-rw-   0        0        0      665 2024-05-21 15:42:19.000000 preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim/TextCleaner.py
+-rw-rw-rw-   0        0        0      255 2024-05-23 09:29:07.000000 preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:39:12.124848 preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim.egg-info/
+-rw-rw-rw-   0        0        0     3230 2024-05-23 09:39:12.000000 preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      826 2024-05-23 09:39:12.000000 preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 09:39:12.000000 preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-23 09:39:12.000000 preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2024-05-23 09:39:12.000000 preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 09:39:12.126339 preprocessinglib_tonga_gumustakim-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      898 2024-05-23 09:39:08.000000 preprocessinglib_tonga_gumustakim-0.3/setup.py
```

### Comparing `preprocessinglib_tonga_gumustakim-0.2/PKG-INFO` & `preprocessinglib_tonga_gumustakim-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preprocessinglib_tonga_gumustakim
-Version: 0.2
+Version: 0.3
 Summary: A comprehensive data preprocessing library for Python
 Home-page: https://github.com/Fzehzeh/mypreprocessinglib , https://github.com/ayserragm/mypreprocessinglib
 Author: Zehra Tonga-Ayse Serra Gumustakim
 Author-email: tongafatmazehra@gmail.com-ayseserra.gumustakim@stu.fsm.edu.tr 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `preprocessinglib_tonga_gumustakim-0.2/README.md` & `preprocessinglib_tonga_gumustakim-0.3/README.md`

 * *Files identical despite different names*

### Comparing `preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim/CategoricalEncoder.py` & `preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim/CategoricalEncoder.py`

 * *Files identical despite different names*

### Comparing `preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim/MissingValueHandler.py` & `preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim/MissingValueHandler.py`

 * *Files identical despite different names*

### Comparing `preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim/OutlierHandler.py` & `preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim/OutlierHandler.py`

 * *Files identical despite different names*

### Comparing `preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim/TestDataPreprocessing.py` & `preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim/TestDataPreprocessing.py`

 * *Files identical despite different names*

### Comparing `preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim/TextCleaner.py` & `preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim/TextCleaner.py`

 * *Files identical despite different names*

### Comparing `preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim.egg-info/PKG-INFO` & `preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preprocessinglib_tonga_gumustakim
-Version: 0.2
+Version: 0.3
 Summary: A comprehensive data preprocessing library for Python
 Home-page: https://github.com/Fzehzeh/mypreprocessinglib , https://github.com/ayserragm/mypreprocessinglib
 Author: Zehra Tonga-Ayse Serra Gumustakim
 Author-email: tongafatmazehra@gmail.com-ayseserra.gumustakim@stu.fsm.edu.tr 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `preprocessinglib_tonga_gumustakim-0.2/preprocessinglib_tonga_gumustakim.egg-info/SOURCES.txt` & `preprocessinglib_tonga_gumustakim-0.3/preprocessinglib_tonga_gumustakim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `preprocessinglib_tonga_gumustakim-0.2/setup.py` & `preprocessinglib_tonga_gumustakim-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='preprocessinglib_tonga_gumustakim',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     install_requires=[
         'pandas',
         'numpy',
         'scikit-learn',
         'nltk'
     ],
```

