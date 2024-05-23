# Comparing `tmp/testwizard.set-top-box-3.8.1b4749.tar.gz` & `tmp/testwizard.set-top-box-3.8.1b4810.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testwizard.set-top-box-3.8.1b4749.tar", last modified: Tue Mar 19 15:01:49 2024, max compression
+gzip compressed data, was "testwizard.set-top-box-3.8.1b4810.tar", last modified: Wed Mar 27 12:56:36 2024, max compression
```

## Comparing `testwizard.set-top-box-3.8.1b4749.tar` & `testwizard.set-top-box-3.8.1b4810.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:49.713627 testwizard.set-top-box-3.8.1b4749/
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.set-top-box-3.8.1b4749/LICENSE.txt
--rw-rw-rw-   0        0        0     2033 2024-03-19 15:01:49.713627 testwizard.set-top-box-3.8.1b4749/PKG-INFO
--rw-rw-rw-   0        0        0     1486 2024-03-19 15:00:53.000000 testwizard.set-top-box-3.8.1b4749/README.md
--rw-rw-rw-   0        0        0       42 2024-03-19 15:01:49.713627 testwizard.set-top-box-3.8.1b4749/setup.cfg
--rw-rw-rw-   0        0        0     1134 2024-03-19 15:01:49.000000 testwizard.set-top-box-3.8.1b4749/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:49.713627 testwizard.set-top-box-3.8.1b4749/testwizard/
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:49.713627 testwizard.set-top-box-3.8.1b4749/testwizard/set_top_box/
--rw-rw-rw-   0        0        0    10531 2024-03-19 15:00:53.000000 testwizard.set-top-box-3.8.1b4749/testwizard/set_top_box/SetTopBox.py
--rw-rw-rw-   0        0        0       32 2024-03-19 15:00:53.000000 testwizard.set-top-box-3.8.1b4749/testwizard/set_top_box/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:49.713627 testwizard.set-top-box-3.8.1b4749/testwizard.set_top_box.egg-info/
--rw-rw-rw-   0        0        0     2033 2024-03-19 15:01:49.000000 testwizard.set-top-box-3.8.1b4749/testwizard.set_top_box.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2024-03-19 15:01:49.000000 testwizard.set-top-box-3.8.1b4749/testwizard.set_top_box.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 15:01:49.000000 testwizard.set-top-box-3.8.1b4749/testwizard.set_top_box.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      273 2024-03-19 15:01:49.000000 testwizard.set-top-box-3.8.1b4749/testwizard.set_top_box.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 15:01:49.000000 testwizard.set-top-box-3.8.1b4749/testwizard.set_top_box.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:36.978963 testwizard.set-top-box-3.8.1b4810/
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.set-top-box-3.8.1b4810/LICENSE.txt
+-rw-rw-rw-   0        0        0     2033 2024-03-27 12:56:36.978963 testwizard.set-top-box-3.8.1b4810/PKG-INFO
+-rw-rw-rw-   0        0        0     1486 2024-03-27 12:55:37.000000 testwizard.set-top-box-3.8.1b4810/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-27 12:56:36.978963 testwizard.set-top-box-3.8.1b4810/setup.cfg
+-rw-rw-rw-   0        0        0     1134 2024-03-27 12:56:36.000000 testwizard.set-top-box-3.8.1b4810/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:36.978963 testwizard.set-top-box-3.8.1b4810/testwizard/
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:36.978963 testwizard.set-top-box-3.8.1b4810/testwizard/set_top_box/
+-rw-rw-rw-   0        0        0    10531 2024-03-27 12:55:37.000000 testwizard.set-top-box-3.8.1b4810/testwizard/set_top_box/SetTopBox.py
+-rw-rw-rw-   0        0        0       32 2024-03-27 12:55:37.000000 testwizard.set-top-box-3.8.1b4810/testwizard/set_top_box/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:36.978963 testwizard.set-top-box-3.8.1b4810/testwizard.set_top_box.egg-info/
+-rw-rw-rw-   0        0        0     2033 2024-03-27 12:56:36.000000 testwizard.set-top-box-3.8.1b4810/testwizard.set_top_box.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2024-03-27 12:56:36.000000 testwizard.set-top-box-3.8.1b4810/testwizard.set_top_box.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-27 12:56:36.000000 testwizard.set-top-box-3.8.1b4810/testwizard.set_top_box.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      273 2024-03-27 12:56:36.000000 testwizard.set-top-box-3.8.1b4810/testwizard.set_top_box.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-27 12:56:36.000000 testwizard.set-top-box-3.8.1b4810/testwizard.set_top_box.egg-info/top_level.txt
```

### Comparing `testwizard.set-top-box-3.8.1b4749/PKG-INFO` & `testwizard.set-top-box-3.8.1b4810/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.set-top-box
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard for set-top box testobjects
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.set-top-box-3.8.1b4749/README.md` & `testwizard.set-top-box-3.8.1b4810/README.md`

 * *Files identical despite different names*

### Comparing `testwizard.set-top-box-3.8.1b4749/setup.py` & `testwizard.set-top-box-3.8.1b4810/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="testwizard.set-top-box",
-    version="3.8.1b4749",
+    version="3.8.1b4810",
     author="Resillion",
     author_email="testwizard-support@resillion.com",
     description="Testwizard for set-top box testobjects",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.resillion.com/services/software-testing/testing-tools/testwizard/",
     packages=['testwizard.set_top_box'],
     install_requires=[
-        'testwizard.test==3.8.1b4749',
-        'testwizard.testobjects-core==3.8.1b4749',
-        'testwizard.commands-audio==3.8.1b4749',
-        'testwizard.commands-mobile==3.8.1b4749',
-        'testwizard.commands-powerswitch==3.8.1b4749',
-        'testwizard.commands-remotecontrol==3.8.1b4749',
-        'testwizard.commands-video==3.8.1b4749'
+        'testwizard.test==3.8.1b4810',
+        'testwizard.testobjects-core==3.8.1b4810',
+        'testwizard.commands-audio==3.8.1b4810',
+        'testwizard.commands-mobile==3.8.1b4810',
+        'testwizard.commands-powerswitch==3.8.1b4810',
+        'testwizard.commands-remotecontrol==3.8.1b4810',
+        'testwizard.commands-video==3.8.1b4810'
     ],
     classifiers=[
         "Programming Language :: Python :: 3.3",
         "Development Status :: 5 - Production/Stable",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `testwizard.set-top-box-3.8.1b4749/testwizard/set_top_box/SetTopBox.py` & `testwizard.set-top-box-3.8.1b4810/testwizard/set_top_box/SetTopBox.py`

 * *Files identical despite different names*

### Comparing `testwizard.set-top-box-3.8.1b4749/testwizard.set_top_box.egg-info/PKG-INFO` & `testwizard.set-top-box-3.8.1b4810/testwizard.set_top_box.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.set-top-box
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard for set-top box testobjects
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

