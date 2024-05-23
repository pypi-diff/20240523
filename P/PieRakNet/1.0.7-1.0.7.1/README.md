# Comparing `tmp/pieraknet-1.0.7.tar.gz` & `tmp/pieraknet-1.0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pieraknet-1.0.7.tar", last modified: Sun Apr 28 12:31:35 2024, max compression
+gzip compressed data, was "pieraknet-1.0.7.1.tar", last modified: Thu May 23 19:07:50 2024, max compression
```

## Comparing `pieraknet-1.0.7.tar` & `pieraknet-1.0.7.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:31:35.974782 pieraknet-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 12:31:31.000000 pieraknet-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-28 12:31:35.974782 pieraknet-1.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:31:35.974782 pieraknet-1.0.7/PieRakNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-28 12:31:35.000000 pieraknet-1.0.7/PieRakNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-28 12:31:35.000000 pieraknet-1.0.7/PieRakNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:31:35.000000 pieraknet-1.0.7/PieRakNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:31:35.000000 pieraknet-1.0.7/PieRakNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-28 12:31:31.000000 pieraknet-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 12:31:35.974782 pieraknet-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-28 12:31:31.000000 pieraknet-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:07:50.293843 pieraknet-1.0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 19:07:46.000000 pieraknet-1.0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-23 19:07:50.293843 pieraknet-1.0.7.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:07:50.293843 pieraknet-1.0.7.1/PieRakNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-23 19:07:50.000000 pieraknet-1.0.7.1/PieRakNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-23 19:07:50.000000 pieraknet-1.0.7.1/PieRakNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:07:50.000000 pieraknet-1.0.7.1/PieRakNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:07:50.000000 pieraknet-1.0.7.1/PieRakNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-23 19:07:46.000000 pieraknet-1.0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 19:07:50.293843 pieraknet-1.0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-23 19:07:46.000000 pieraknet-1.0.7.1/setup.py
```

### Comparing `pieraknet-1.0.7/LICENSE` & `pieraknet-1.0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pieraknet-1.0.7/PKG-INFO` & `pieraknet-1.0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PieRakNet
-Version: 1.0.7
+Version: 1.0.7.1
 Summary: RakNet implementation, written in Python. Created for PieMC.
 Home-page: https://github.com/PieMC-Dev/PieRakNet
 Author: lapismyt
 Author-email: PieMC.Developers@gmail.com
 Project-URL: Example, https://github.com/PieMC-Dev/PieRakNet/tree/main/EXAMPLE.md
 Project-URL: Developer, https://github.com/PieMC-Dev
 Keywords: python python3 raknet rak-net mcpe bedrock rak_net piemc pieraknet
```

### Comparing `pieraknet-1.0.7/PieRakNet.egg-info/PKG-INFO` & `pieraknet-1.0.7.1/PieRakNet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PieRakNet
-Version: 1.0.7
+Version: 1.0.7.1
 Summary: RakNet implementation, written in Python. Created for PieMC.
 Home-page: https://github.com/PieMC-Dev/PieRakNet
 Author: lapismyt
 Author-email: PieMC.Developers@gmail.com
 Project-URL: Example, https://github.com/PieMC-Dev/PieRakNet/tree/main/EXAMPLE.md
 Project-URL: Developer, https://github.com/PieMC-Dev
 Keywords: python python3 raknet rak-net mcpe bedrock rak_net piemc pieraknet
```

### Comparing `pieraknet-1.0.7/README.md` & `pieraknet-1.0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pieraknet-1.0.7/setup.py` & `pieraknet-1.0.7.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from setuptools import setup, find_packages
 
-
 def readme():
     with open('README.md', 'r', encoding='utf-8') as f:
         return f.read()
 
-
 setup(
     name='PieRakNet',
-    version='1.0.7',
+    version='1.0.7.1',
     author='lapismyt',
     author_email='PieMC.Developers@gmail.com',
     description='RakNet implementation, written in Python. Created for PieMC.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/PieMC-Dev/PieRakNet',
     packages=find_packages(),
-    # install_requires=[],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3.11',
         'Topic :: Internet',
         'Topic :: Games/Entertainment',
         'Topic :: Software Development :: Libraries :: Python Modules',
```

