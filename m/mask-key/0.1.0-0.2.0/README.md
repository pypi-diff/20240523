# Comparing `tmp/mask_key-0.1.0.tar.gz` & `tmp/mask_key-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mask_key-0.1.0.tar", last modified: Thu May 23 04:10:34 2024, max compression
+gzip compressed data, was "mask_key-0.2.0.tar", last modified: Thu May 23 04:51:46 2024, max compression
```

## Comparing `mask_key-0.1.0.tar` & `mask_key-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 04:10:34.812785 mask_key-0.1.0/
--rw-rw-rw-   0        0        0        0 2024-05-23 03:49:20.000000 mask_key-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       34 2024-05-23 04:03:50.000000 mask_key-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      528 2024-05-23 04:10:34.809145 mask_key-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-23 03:49:07.000000 mask_key-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 04:10:34.740333 mask_key-0.1.0/mask_key/
--rw-rw-rw-   0        0        0       47 2024-05-23 03:48:11.000000 mask_key-0.1.0/mask_key/__init__.py
--rw-rw-rw-   0        0        0      378 2024-05-23 03:50:50.000000 mask_key-0.1.0/mask_key/api.py
--rw-rw-rw-   0        0        0     1174 2024-05-23 03:51:09.000000 mask_key-0.1.0/mask_key/main.py
--rw-rw-rw-   0        0        0       94 2024-05-23 03:50:36.000000 mask_key-0.1.0/mask_key/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 04:10:34.807153 mask_key-0.1.0/mask_key.egg-info/
--rw-rw-rw-   0        0        0      528 2024-05-23 04:10:34.000000 mask_key-0.1.0/mask_key.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2024-05-23 04:10:34.000000 mask_key-0.1.0/mask_key.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 04:10:34.000000 mask_key-0.1.0/mask_key.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-23 04:10:34.000000 mask_key-0.1.0/mask_key.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       23 2024-05-23 04:10:34.000000 mask_key-0.1.0/mask_key.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-23 04:10:34.000000 mask_key-0.1.0/mask_key.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 04:10:34.813809 mask_key-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      832 2024-05-23 04:07:04.000000 mask_key-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 04:51:46.162118 mask_key-0.2.0/
+-rw-rw-rw-   0        0        0        0 2024-05-23 03:49:20.000000 mask_key-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-05-23 04:03:50.000000 mask_key-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      528 2024-05-23 04:51:46.159764 mask_key-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-23 03:49:07.000000 mask_key-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 04:51:46.118320 mask_key-0.2.0/mask_key/
+-rw-rw-rw-   0        0        0       47 2024-05-23 03:48:11.000000 mask_key-0.2.0/mask_key/__init__.py
+-rw-rw-rw-   0        0        0      392 2024-05-23 04:47:54.000000 mask_key-0.2.0/mask_key/api.py
+-rw-rw-rw-   0        0        0     1174 2024-05-23 03:51:09.000000 mask_key-0.2.0/mask_key/main.py
+-rw-rw-rw-   0        0        0       94 2024-05-23 03:50:36.000000 mask_key-0.2.0/mask_key/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 04:51:46.157768 mask_key-0.2.0/mask_key.egg-info/
+-rw-rw-rw-   0        0        0      528 2024-05-23 04:51:46.000000 mask_key-0.2.0/mask_key.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2024-05-23 04:51:46.000000 mask_key-0.2.0/mask_key.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 04:51:46.000000 mask_key-0.2.0/mask_key.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-23 04:51:46.000000 mask_key-0.2.0/mask_key.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       23 2024-05-23 04:51:46.000000 mask_key-0.2.0/mask_key.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-23 04:51:46.000000 mask_key-0.2.0/mask_key.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 04:51:46.163474 mask_key-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      832 2024-05-23 04:51:40.000000 mask_key-0.2.0/setup.py
```

### Comparing `mask_key-0.1.0/PKG-INFO` & `mask_key-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mask_key
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python package to generate mask keys.
 Home-page: https://github.com/krishnaagarwal781/mask_keys_server
 Author: krishna agarwal
 Author-email: krishnacool781@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mask_key-0.1.0/mask_key/main.py` & `mask_key-0.2.0/mask_key/main.py`

 * *Files identical despite different names*

### Comparing `mask_key-0.1.0/mask_key.egg-info/PKG-INFO` & `mask_key-0.2.0/mask_key.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mask_key
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python package to generate mask keys.
 Home-page: https://github.com/krishnaagarwal781/mask_keys_server
 Author: krishna agarwal
 Author-email: krishnacool781@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mask_key-0.1.0/setup.py` & `mask_key-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mask_key',
-    version='0.1.0',
+    version='0.2.0',
     author='krishna agarwal',
     author_email='krishnacool781@gmail.com',
     description='A Python package to generate mask keys.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/krishnaagarwal781/mask_keys_server',
     packages=find_packages(),
```

