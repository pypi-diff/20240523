# Comparing `tmp/testwizard.web-3.8.1b4749.tar.gz` & `tmp/testwizard.web-3.8.1b4810.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testwizard.web-3.8.1b4749.tar", last modified: Tue Mar 19 15:01:50 2024, max compression
+gzip compressed data, was "testwizard.web-3.8.1b4810.tar", last modified: Wed Mar 27 12:56:37 2024, max compression
```

## Comparing `testwizard.web-3.8.1b4749.tar` & `testwizard.web-3.8.1b4810.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:50.620366 testwizard.web-3.8.1b4749/
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.web-3.8.1b4749/LICENSE.txt
--rw-rw-rw-   0        0        0     2211 2024-03-19 15:01:50.620366 testwizard.web-3.8.1b4749/PKG-INFO
--rw-rw-rw-   0        0        0     1680 2024-03-19 15:00:53.000000 testwizard.web-3.8.1b4749/README.md
--rw-rw-rw-   0        0        0       42 2024-03-19 15:01:50.620366 testwizard.web-3.8.1b4749/setup.cfg
--rw-rw-rw-   0        0        0      993 2024-03-19 15:01:50.000000 testwizard.web-3.8.1b4749/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:50.620366 testwizard.web-3.8.1b4749/testwizard/
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:50.620366 testwizard.web-3.8.1b4749/testwizard/web/
--rw-rw-rw-   0        0        0    22024 2024-03-19 15:00:53.000000 testwizard.web-3.8.1b4749/testwizard/web/Web.py
--rw-rw-rw-   0        0        0       20 2024-03-19 15:00:53.000000 testwizard.web-3.8.1b4749/testwizard/web/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:50.620366 testwizard.web-3.8.1b4749/testwizard.web.egg-info/
--rw-rw-rw-   0        0        0     2211 2024-03-19 15:01:50.000000 testwizard.web-3.8.1b4749/testwizard.web.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-03-19 15:01:50.000000 testwizard.web-3.8.1b4749/testwizard.web.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 15:01:50.000000 testwizard.web-3.8.1b4749/testwizard.web.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      180 2024-03-19 15:01:50.000000 testwizard.web-3.8.1b4749/testwizard.web.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 15:01:50.000000 testwizard.web-3.8.1b4749/testwizard.web.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:37.838621 testwizard.web-3.8.1b4810/
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.web-3.8.1b4810/LICENSE.txt
+-rw-rw-rw-   0        0        0     2211 2024-03-27 12:56:37.838621 testwizard.web-3.8.1b4810/PKG-INFO
+-rw-rw-rw-   0        0        0     1680 2024-03-27 12:55:37.000000 testwizard.web-3.8.1b4810/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-27 12:56:37.838621 testwizard.web-3.8.1b4810/setup.cfg
+-rw-rw-rw-   0        0        0      993 2024-03-27 12:56:37.000000 testwizard.web-3.8.1b4810/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:37.822998 testwizard.web-3.8.1b4810/testwizard/
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:37.822998 testwizard.web-3.8.1b4810/testwizard/web/
+-rw-rw-rw-   0        0        0    22024 2024-03-27 12:55:37.000000 testwizard.web-3.8.1b4810/testwizard/web/Web.py
+-rw-rw-rw-   0        0        0       20 2024-03-27 12:55:37.000000 testwizard.web-3.8.1b4810/testwizard/web/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:37.822998 testwizard.web-3.8.1b4810/testwizard.web.egg-info/
+-rw-rw-rw-   0        0        0     2211 2024-03-27 12:56:37.000000 testwizard.web-3.8.1b4810/testwizard.web.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-03-27 12:56:37.000000 testwizard.web-3.8.1b4810/testwizard.web.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-27 12:56:37.000000 testwizard.web-3.8.1b4810/testwizard.web.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      180 2024-03-27 12:56:37.000000 testwizard.web-3.8.1b4810/testwizard.web.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-27 12:56:37.000000 testwizard.web-3.8.1b4810/testwizard.web.egg-info/top_level.txt
```

### Comparing `testwizard.web-3.8.1b4749/PKG-INFO` & `testwizard.web-3.8.1b4810/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.web
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard for Web testobjects
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.web-3.8.1b4749/README.md` & `testwizard.web-3.8.1b4810/README.md`

 * *Files identical despite different names*

### Comparing `testwizard.web-3.8.1b4749/setup.py` & `testwizard.web-3.8.1b4810/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="testwizard.web",
-    version="3.8.1b4749",
+    version="3.8.1b4810",
     author="Resillion",
     author_email="testwizard-support@resillion.com",
     description="Testwizard for Web testobjects",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.resillion.com/services/software-testing/testing-tools/testwizard/",
     packages=['testwizard.web'],
     install_requires=[
-        'testwizard.test==3.8.1b4749',
-        'testwizard.testobjects-core==3.8.1b4749',
-        'testwizard.commands-audio==3.8.1b4749',
-        'testwizard.commands-video==3.8.1b4749',
-        'testwizard.commands-web==3.8.1b4749'
+        'testwizard.test==3.8.1b4810',
+        'testwizard.testobjects-core==3.8.1b4810',
+        'testwizard.commands-audio==3.8.1b4810',
+        'testwizard.commands-video==3.8.1b4810',
+        'testwizard.commands-web==3.8.1b4810'
     ],
     classifiers=[
         "Programming Language :: Python :: 3.3",
         "Development Status :: 5 - Production/Stable",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `testwizard.web-3.8.1b4749/testwizard/web/Web.py` & `testwizard.web-3.8.1b4810/testwizard/web/Web.py`

 * *Files identical despite different names*

### Comparing `testwizard.web-3.8.1b4749/testwizard.web.egg-info/PKG-INFO` & `testwizard.web-3.8.1b4810/testwizard.web.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.web
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard for Web testobjects
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

