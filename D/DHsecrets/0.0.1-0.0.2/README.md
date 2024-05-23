# Comparing `tmp/DHsecrets-0.0.1.tar.gz` & `tmp/DHsecrets-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DHsecrets-0.0.1.tar", last modified: Thu Sep  8 12:19:57 2022, max compression
+gzip compressed data, was "DHsecrets-0.0.2.tar", last modified: Thu May 23 19:36:39 2024, max compression
```

## Comparing `DHsecrets-0.0.1.tar` & `DHsecrets-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-09-08 12:19:57.131911 DHsecrets-0.0.1/
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-09-08 12:19:57.131911 DHsecrets-0.0.1/DHsecrets.egg-info/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     3525 2022-09-08 12:19:56.000000 DHsecrets-0.0.1/DHsecrets.egg-info/PKG-INFO
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      294 2022-09-08 12:19:57.000000 DHsecrets-0.0.1/DHsecrets.egg-info/SOURCES.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        1 2022-09-08 12:19:56.000000 DHsecrets-0.0.1/DHsecrets.egg-info/dependency_links.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)       41 2022-09-08 12:19:56.000000 DHsecrets-0.0.1/DHsecrets.egg-info/entry_points.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)       17 2022-09-08 12:19:56.000000 DHsecrets-0.0.1/DHsecrets.egg-info/requires.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)       18 2022-09-08 12:19:56.000000 DHsecrets-0.0.1/DHsecrets.egg-info/top_level.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1072 2022-05-13 12:53:32.000000 DHsecrets-0.0.1/LICENSE
--rw-rw-r--   0 valerio   (1000) valerio   (1000)       16 2022-09-07 19:35:16.000000 DHsecrets-0.0.1/MANIFEST.in
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     3525 2022-09-08 12:19:57.131911 DHsecrets-0.0.1/PKG-INFO
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     3100 2022-09-08 11:28:31.000000 DHsecrets-0.0.1/README.md
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     3123 2022-09-08 08:14:07.000000 DHsecrets-0.0.1/dhs_cli.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-09-08 12:19:57.131911 DHsecrets-0.0.1/dhsecrets/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2022-09-08 08:14:18.000000 DHsecrets-0.0.1/dhsecrets/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     5848 2022-09-07 19:57:04.000000 DHsecrets-0.0.1/dhsecrets/dhsecrets.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)       38 2022-09-08 12:19:57.131911 DHsecrets-0.0.1/setup.cfg
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      921 2022-09-08 12:19:22.000000 DHsecrets-0.0.1/setup.py
+drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2024-05-23 19:36:39.359767 DHsecrets-0.0.2/
+drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2024-05-23 19:36:39.359767 DHsecrets-0.0.2/DHsecrets.egg-info/
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     3525 2024-05-23 19:36:39.000000 DHsecrets-0.0.2/DHsecrets.egg-info/PKG-INFO
+-rw-r--r--   0 valerio   (1000) valerio   (1000)      294 2024-05-23 19:36:39.000000 DHsecrets-0.0.2/DHsecrets.egg-info/SOURCES.txt
+-rw-r--r--   0 valerio   (1000) valerio   (1000)        1 2024-05-23 19:36:39.000000 DHsecrets-0.0.2/DHsecrets.egg-info/dependency_links.txt
+-rw-r--r--   0 valerio   (1000) valerio   (1000)       41 2024-05-23 19:36:39.000000 DHsecrets-0.0.2/DHsecrets.egg-info/entry_points.txt
+-rw-r--r--   0 valerio   (1000) valerio   (1000)       17 2024-05-23 19:36:39.000000 DHsecrets-0.0.2/DHsecrets.egg-info/requires.txt
+-rw-r--r--   0 valerio   (1000) valerio   (1000)       18 2024-05-23 19:36:39.000000 DHsecrets-0.0.2/DHsecrets.egg-info/top_level.txt
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     1072 2024-05-23 19:30:04.000000 DHsecrets-0.0.2/LICENSE
+-rw-r--r--   0 valerio   (1000) valerio   (1000)       16 2024-05-23 19:30:04.000000 DHsecrets-0.0.2/MANIFEST.in
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     3525 2024-05-23 19:36:39.359767 DHsecrets-0.0.2/PKG-INFO
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     3100 2024-05-23 19:30:04.000000 DHsecrets-0.0.2/README.md
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     3123 2024-05-23 19:30:04.000000 DHsecrets-0.0.2/dhs_cli.py
+drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2024-05-23 19:36:39.359767 DHsecrets-0.0.2/dhsecrets/
+-rw-r--r--   0 valerio   (1000) valerio   (1000)        0 2024-05-23 19:30:04.000000 DHsecrets-0.0.2/dhsecrets/__init__.py
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     5848 2024-05-23 19:30:04.000000 DHsecrets-0.0.2/dhsecrets/dhsecrets.py
+-rw-r--r--   0 valerio   (1000) valerio   (1000)       38 2024-05-23 19:36:39.359767 DHsecrets-0.0.2/setup.cfg
+-rw-r--r--   0 valerio   (1000) valerio   (1000)      921 2024-05-23 19:34:17.000000 DHsecrets-0.0.2/setup.py
```

### Comparing `DHsecrets-0.0.1/DHsecrets.egg-info/PKG-INFO` & `DHsecrets-0.0.2/DHsecrets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DHsecrets
-Version: 0.0.1
+Version: 0.0.2
 Summary: Diffie-Hellman based secret secure exchange.
 Home-page: https://github.com/valerio-vaccaro/DH-secrets
 Author: Valerio Vaccaro
 Author-email: valerio.vaccaro@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
```

### Comparing `DHsecrets-0.0.1/LICENSE` & `DHsecrets-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DHsecrets-0.0.1/PKG-INFO` & `DHsecrets-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DHsecrets
-Version: 0.0.1
+Version: 0.0.2
 Summary: Diffie-Hellman based secret secure exchange.
 Home-page: https://github.com/valerio-vaccaro/DH-secrets
 Author: Valerio Vaccaro
 Author-email: valerio.vaccaro@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
```

### Comparing `DHsecrets-0.0.1/README.md` & `DHsecrets-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `DHsecrets-0.0.1/dhs_cli.py` & `DHsecrets-0.0.2/dhs_cli.py`

 * *Files identical despite different names*

### Comparing `DHsecrets-0.0.1/dhsecrets/dhsecrets.py` & `DHsecrets-0.0.2/dhsecrets/dhsecrets.py`

 * *Files identical despite different names*

### Comparing `DHsecrets-0.0.1/setup.py` & `DHsecrets-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name='DHsecrets',
-    version='0.0.1',
+    version='0.0.2',
     author='Valerio Vaccaro',
     author_email='valerio.vaccaro@gmail.com',
     license='MIT',
     description='Diffie-Hellman based secret secure exchange.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/valerio-vaccaro/DH-secrets',
```

