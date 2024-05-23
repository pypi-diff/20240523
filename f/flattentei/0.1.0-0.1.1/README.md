# Comparing `tmp/flattentei-0.1.0.tar.gz` & `tmp/flattentei-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flattentei-0.1.0.tar", last modified: Mon Apr  8 12:21:08 2024, max compression
+gzip compressed data, was "flattentei-0.1.1.tar", last modified: Thu May 23 16:00:42 2024, max compression
```

## Comparing `flattentei-0.1.0.tar` & `flattentei-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 ottowg    (1004) ottowg    (1004)        0 2024-04-08 12:21:08.542394 flattentei-0.1.0/
--rw-rw-r--   0 ottowg    (1004) ottowg    (1004)      528 2024-04-08 12:21:08.542394 flattentei-0.1.0/PKG-INFO
--rw-rw-r--   0 ottowg    (1004) ottowg    (1004)      173 2023-10-11 08:22:08.000000 flattentei-0.1.0/README.md
-drwxrwxr-x   0 ottowg    (1004) ottowg    (1004)        0 2024-04-08 12:21:08.506394 flattentei-0.1.0/flattentei/
--rw-rw-r--   0 ottowg    (1004) ottowg    (1004)       97 2023-04-04 08:01:44.000000 flattentei-0.1.0/flattentei/__init__.py
--rw-rw-r--   0 ottowg    (1004) ottowg    (1004)     5971 2023-08-04 11:39:47.000000 flattentei-0.1.0/flattentei/extract_parts.py
--rw-rw-r--   0 ottowg    (1004) ottowg    (1004)     1023 2023-07-18 08:16:22.000000 flattentei-0.1.0/flattentei/loader.py
--rw-rw-r--   0 ottowg    (1004) ottowg    (1004)    12159 2024-03-19 13:37:34.000000 flattentei-0.1.0/flattentei/tei_to_text_and_standoff.py
-drwxrwxr-x   0 ottowg    (1004) ottowg    (1004)        0 2024-04-08 12:21:08.542394 flattentei-0.1.0/flattentei.egg-info/
--rw-r--r--   0 ottowg    (1004) ottowg    (1004)      528 2024-04-08 12:21:08.000000 flattentei-0.1.0/flattentei.egg-info/PKG-INFO
--rw-rw-r--   0 ottowg    (1004) ottowg    (1004)      298 2024-04-08 12:21:08.000000 flattentei-0.1.0/flattentei.egg-info/SOURCES.txt
--rw-rw-r--   0 ottowg    (1004) ottowg    (1004)        1 2024-04-08 12:21:08.000000 flattentei-0.1.0/flattentei.egg-info/dependency_links.txt
--rw-rw-r--   0 ottowg    (1004) ottowg    (1004)       12 2024-04-08 12:21:08.000000 flattentei-0.1.0/flattentei.egg-info/requires.txt
--rw-rw-r--   0 ottowg    (1004) ottowg    (1004)       11 2024-04-08 12:21:08.000000 flattentei-0.1.0/flattentei.egg-info/top_level.txt
--rw-rw-r--   0 ottowg    (1004) ottowg    (1004)       38 2024-04-08 12:21:08.542394 flattentei-0.1.0/setup.cfg
--rw-rw-r--   0 ottowg    (1004) ottowg    (1004)      673 2023-10-11 08:27:55.000000 flattentei-0.1.0/setup.py
+drwxrwxr-x   0 ottowg    (1004) ottowg    (1004)        0 2024-05-23 16:00:42.095612 flattentei-0.1.1/
+-rw-rw-r--   0 ottowg    (1004) ottowg    (1004)      557 2024-05-23 16:00:42.095612 flattentei-0.1.1/PKG-INFO
+-rw-rw-r--   0 ottowg    (1004) ottowg    (1004)      196 2024-05-23 15:41:48.000000 flattentei-0.1.1/README.md
+drwxrwxr-x   0 ottowg    (1004) ottowg    (1004)        0 2024-05-23 16:00:42.091612 flattentei-0.1.1/flattentei/
+-rw-rw-r--   0 ottowg    (1004) ottowg    (1004)      119 2024-05-23 15:45:00.000000 flattentei-0.1.1/flattentei/__init__.py
+-rw-rw-r--   0 ottowg    (1004) ottowg    (1004)     5971 2023-08-04 11:39:47.000000 flattentei-0.1.1/flattentei/extract_parts.py
+-rw-rw-r--   0 ottowg    (1004) ottowg    (1004)     1023 2023-07-18 08:16:22.000000 flattentei-0.1.1/flattentei/loader.py
+-rw-rw-r--   0 ottowg    (1004) ottowg    (1004)    12159 2024-04-08 12:40:59.000000 flattentei-0.1.1/flattentei/tei_to_text_and_standoff.py
+drwxrwxr-x   0 ottowg    (1004) ottowg    (1004)        0 2024-05-23 16:00:42.095612 flattentei-0.1.1/flattentei.egg-info/
+-rw-r--r--   0 ottowg    (1004) ottowg    (1004)      557 2024-05-23 16:00:41.000000 flattentei-0.1.1/flattentei.egg-info/PKG-INFO
+-rw-rw-r--   0 ottowg    (1004) ottowg    (1004)      335 2024-05-23 16:00:41.000000 flattentei-0.1.1/flattentei.egg-info/SOURCES.txt
+-rw-rw-r--   0 ottowg    (1004) ottowg    (1004)        1 2024-05-23 16:00:41.000000 flattentei-0.1.1/flattentei.egg-info/dependency_links.txt
+-rw-rw-r--   0 ottowg    (1004) ottowg    (1004)       83 2024-05-23 16:00:41.000000 flattentei-0.1.1/flattentei.egg-info/entry_points.txt
+-rw-rw-r--   0 ottowg    (1004) ottowg    (1004)       12 2024-05-23 16:00:41.000000 flattentei-0.1.1/flattentei.egg-info/requires.txt
+-rw-rw-r--   0 ottowg    (1004) ottowg    (1004)       11 2024-05-23 16:00:41.000000 flattentei-0.1.1/flattentei.egg-info/top_level.txt
+-rw-rw-r--   0 ottowg    (1004) ottowg    (1004)       38 2024-05-23 16:00:42.095612 flattentei-0.1.1/setup.cfg
+-rw-rw-r--   0 ottowg    (1004) ottowg    (1004)      843 2024-05-23 15:52:51.000000 flattentei-0.1.1/setup.py
```

### Comparing `flattentei-0.1.0/PKG-INFO` & `flattentei-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: flattentei
-Version: 0.1.0
+Version: 0.1.1
 Summary: Transform tei xml to a simple standoff format
-Home-page: https://
+Home-page: https://git.gesis.org/nlp/flatten-tei
 Author: Wolf Otto
 Author-email: wolfgang.otto@gesis.org
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `flattentei-0.1.0/flattentei/extract_parts.py` & `flattentei-0.1.1/flattentei/extract_parts.py`

 * *Files identical despite different names*

### Comparing `flattentei-0.1.0/flattentei/loader.py` & `flattentei-0.1.1/flattentei/loader.py`

 * *Files identical despite different names*

### Comparing `flattentei-0.1.0/flattentei/tei_to_text_and_standoff.py` & `flattentei-0.1.1/flattentei/tei_to_text_and_standoff.py`

 * *Files identical despite different names*

### Comparing `flattentei-0.1.0/flattentei.egg-info/PKG-INFO` & `flattentei-0.1.1/flattentei.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: flattentei
-Version: 0.1.0
+Version: 0.1.1
 Summary: Transform tei xml to a simple standoff format
-Home-page: https://
+Home-page: https://git.gesis.org/nlp/flatten-tei
 Author: Wolf Otto
 Author-email: wolfgang.otto@gesis.org
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `flattentei-0.1.0/setup.py` & `flattentei-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from setuptools import setup
 
 setup(
     name='flattentei',
-    version='0.1.0',    
+    version='0.1.1',    
     description='Transform tei xml to a simple standoff format',
-    url='https://',
+    url='https://git.gesis.org/nlp/flatten-tei',
     author='Wolf Otto',
     author_email='wolfgang.otto@gesis.org',
     license='BSD 2-clause',
     packages=['flattentei'],
     install_requires=[
         "lxml>=4.9.1",
     ],
-
+    entry_points={
+        'console_scripts': [
+            'flatten-tei-folder=flattentei.scripts.flatten_tei_folder:main',
+        ]
+    },
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',  
         'Operating System :: POSIX :: Linux',        
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
```

