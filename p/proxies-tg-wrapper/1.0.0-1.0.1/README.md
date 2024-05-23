# Comparing `tmp/proxies-tg-wrapper-1.0.0.tar.gz` & `tmp/proxies-tg-wrapper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxies-tg-wrapper-1.0.0.tar", last modified: Sun May 19 11:27:19 2024, max compression
+gzip compressed data, was "proxies-tg-wrapper-1.0.1.tar", last modified: Thu May 23 10:34:42 2024, max compression
```

## Comparing `proxies-tg-wrapper-1.0.0.tar` & `proxies-tg-wrapper-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-19 11:27:19.228614 proxies-tg-wrapper-1.0.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1072 2024-02-22 08:02:12.000000 proxies-tg-wrapper-1.0.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1114 2024-05-19 11:27:19.228614 proxies-tg-wrapper-1.0.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      569 2024-05-19 11:17:08.000000 proxies-tg-wrapper-1.0.0/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-19 11:27:19.228614 proxies-tg-wrapper-1.0.0/proxies_tg_wrapper/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       37 2024-05-19 11:09:58.000000 proxies-tg-wrapper-1.0.0/proxies_tg_wrapper/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6485 2024-05-19 11:08:32.000000 proxies-tg-wrapper-1.0.0/proxies_tg_wrapper/api_wrapper.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-19 11:27:19.228614 proxies-tg-wrapper-1.0.0/proxies_tg_wrapper.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1114 2024-05-19 11:27:19.000000 proxies-tg-wrapper-1.0.0/proxies_tg_wrapper.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      300 2024-05-19 11:27:19.000000 proxies-tg-wrapper-1.0.0/proxies_tg_wrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-19 11:27:19.000000 proxies-tg-wrapper-1.0.0/proxies_tg_wrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       24 2024-05-19 11:27:19.000000 proxies-tg-wrapper-1.0.0/proxies_tg_wrapper.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2024-05-19 11:27:19.000000 proxies-tg-wrapper-1.0.0/proxies_tg_wrapper.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-19 11:27:19.228614 proxies-tg-wrapper-1.0.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      774 2024-05-19 11:05:42.000000 proxies-tg-wrapper-1.0.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 10:34:42.079781 proxies-tg-wrapper-1.0.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1072 2024-02-22 08:02:12.000000 proxies-tg-wrapper-1.0.1/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1114 2024-05-23 10:34:42.079781 proxies-tg-wrapper-1.0.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      569 2024-05-19 11:17:08.000000 proxies-tg-wrapper-1.0.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 10:34:42.075781 proxies-tg-wrapper-1.0.1/proxies_tg_wrapper/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       37 2024-05-19 11:09:58.000000 proxies-tg-wrapper-1.0.1/proxies_tg_wrapper/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6485 2024-05-19 11:08:32.000000 proxies-tg-wrapper-1.0.1/proxies_tg_wrapper/api_wrapper.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 10:34:42.079781 proxies-tg-wrapper-1.0.1/proxies_tg_wrapper.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1114 2024-05-23 10:34:42.000000 proxies-tg-wrapper-1.0.1/proxies_tg_wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      300 2024-05-23 10:34:42.000000 proxies-tg-wrapper-1.0.1/proxies_tg_wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-23 10:34:42.000000 proxies-tg-wrapper-1.0.1/proxies_tg_wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       24 2024-05-23 10:34:42.000000 proxies-tg-wrapper-1.0.1/proxies_tg_wrapper.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2024-05-23 10:34:42.000000 proxies-tg-wrapper-1.0.1/proxies_tg_wrapper.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-23 10:34:42.079781 proxies-tg-wrapper-1.0.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      775 2024-05-23 10:33:56.000000 proxies-tg-wrapper-1.0.1/setup.py
```

### Comparing `proxies-tg-wrapper-1.0.0/LICENSE` & `proxies-tg-wrapper-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proxies-tg-wrapper-1.0.0/PKG-INFO` & `proxies-tg-wrapper-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxies-tg-wrapper
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package designed to facilitate interaction with the Telegram API, specifically for managing MTProto proxies.
 Home-page: https://github.com/Ilia-Abolhasani/proxies-tg-wrapper
 Author: Ilia Abolhasani
 Author-email: abolhasani.eliya@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `proxies-tg-wrapper-1.0.0/README.md` & `proxies-tg-wrapper-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `proxies-tg-wrapper-1.0.0/proxies_tg_wrapper/api_wrapper.py` & `proxies-tg-wrapper-1.0.1/proxies_tg_wrapper/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `proxies-tg-wrapper-1.0.0/proxies_tg_wrapper.egg-info/PKG-INFO` & `proxies-tg-wrapper-1.0.1/proxies_tg_wrapper.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxies-tg-wrapper
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package designed to facilitate interaction with the Telegram API, specifically for managing MTProto proxies.
 Home-page: https://github.com/Ilia-Abolhasani/proxies-tg-wrapper
 Author: Ilia Abolhasani
 Author-email: abolhasani.eliya@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `proxies-tg-wrapper-1.0.0/setup.py` & `proxies-tg-wrapper-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name="proxies-tg-wrapper",
-    version="1.0.0",
+    version="1.0.1",
     packages=find_packages(),
     install_requires=[
-        'python-telegram==1.18.0'        
+        'python-telegram==0.18.0'        
     ],
     author="Ilia Abolhasani",
     author_email="abolhasani.eliya@gmail.com",
     description="A package designed to facilitate interaction with the Telegram API, specifically for managing MTProto proxies.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/Ilia-Abolhasani/proxies-tg-wrapper",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-)
+)
```

