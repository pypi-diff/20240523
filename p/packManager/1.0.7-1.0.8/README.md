# Comparing `tmp/packmanager-1.0.7.tar.gz` & `tmp/packmanager-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packmanager-1.0.7.tar", last modified: Thu May 23 07:28:47 2024, max compression
+gzip compressed data, was "packmanager-1.0.8.tar", last modified: Thu May 23 12:11:44 2024, max compression
```

## Comparing `packmanager-1.0.7.tar` & `packmanager-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 07:28:47.707238 packmanager-1.0.7/
--rw-rw-rw-   0        0        0       85 2024-05-22 12:41:47.000000 packmanager-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      810 2024-05-23 07:28:47.705244 packmanager-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-05-22 08:13:58.000000 packmanager-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 07:28:47.670231 packmanager-1.0.7/packManager/
--rw-rw-rw-   0        0        0     1427 2024-05-23 07:27:00.000000 packmanager-1.0.7/packManager/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 07:28:47.703238 packmanager-1.0.7/packManager.egg-info/
--rw-rw-rw-   0        0        0      810 2024-05-23 07:28:47.000000 packmanager-1.0.7/packManager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-05-23 07:28:47.000000 packmanager-1.0.7/packManager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 07:28:47.000000 packmanager-1.0.7/packManager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-23 07:28:47.000000 packmanager-1.0.7/packManager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2024-05-22 12:42:05.000000 packmanager-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-23 07:28:47.707238 packmanager-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      855 2024-05-23 07:28:19.000000 packmanager-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:44.187701 packmanager-1.0.8/
+-rw-rw-rw-   0        0        0       85 2024-05-22 12:41:47.000000 packmanager-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      810 2024-05-23 12:11:44.183699 packmanager-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-05-22 08:13:58.000000 packmanager-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:44.123346 packmanager-1.0.8/packManager/
+-rw-rw-rw-   0        0        0     1231 2024-05-23 12:06:35.000000 packmanager-1.0.8/packManager/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:44.180702 packmanager-1.0.8/packManager.egg-info/
+-rw-rw-rw-   0        0        0      810 2024-05-23 12:11:43.000000 packmanager-1.0.8/packManager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-05-23 12:11:43.000000 packmanager-1.0.8/packManager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 12:11:43.000000 packmanager-1.0.8/packManager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-23 12:11:43.000000 packmanager-1.0.8/packManager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2024-05-22 12:42:05.000000 packmanager-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 12:11:44.187701 packmanager-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      855 2024-05-23 12:02:33.000000 packmanager-1.0.8/setup.py
```

### Comparing `packmanager-1.0.7/PKG-INFO` & `packmanager-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packManager
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package manager for python
 Home-page: https://chicken-muggets.github.io/packManager/
 Author: Chicken Muggets
 License: MIT
 Project-URL: Documentation, https://github.com/chicken-muggets/PackInst/wiki
 Project-URL: Source, https://github.com/chicken-muggets/PackInst
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `packmanager-1.0.7/packManager/__init__.py` & `packmanager-1.0.8/packManager/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import os
 def install(package,consCall, hasInput):
     if consCall == 1 or consCall == True:
-        print('installing package ' + package)
         if hasInput == False or hasInput == 0:
-            os.system('pip install ' + package)
-        else:
             os.system('pip install ' + package + ' --no-input')
-        print(package + ' installed successfully')
+        else:
+            os.system('pip install ' + package)
+    
     if consCall == 0 or consCall == False:
         if hasInput == False or hasInput == 0:
-            os.system('pip install ' + package + ' ' + '-q -q -q ')
-        else:
             os.system('pip install ' + package + ' ' + '-q -q -q ' + '--no-input')
+        else:
+            os.system('pip install ' + package + ' ' + '-q -q -q ')
+
 def uninstall(package,consCall, hasInput):
     if consCall == 1 or consCall == True:
-        print('uninstalling package ' + package)
         if hasInput == False or hasInput == 0:
             os.system('pip uninstall ' + package + ' -y')
         else:
             os.system('pip uninstall ' + package)
-        print(package + ' uninstalled successfully')
     if consCall == 0 or consCall == False:
         if hasInput == False or hasInput == 0:
             os.system('pip uninstall ' + package + ' ' + '-q -q -q ' + '-y')
         else:
             os.system('pip uninstall ' + package + ' ' + '-q -q -q ')
 def testInstall(package):
     import importlib.util
```

### Comparing `packmanager-1.0.7/packManager.egg-info/PKG-INFO` & `packmanager-1.0.8/packManager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packManager
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package manager for python
 Home-page: https://chicken-muggets.github.io/packManager/
 Author: Chicken Muggets
 License: MIT
 Project-URL: Documentation, https://github.com/chicken-muggets/PackInst/wiki
 Project-URL: Source, https://github.com/chicken-muggets/PackInst
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `packmanager-1.0.7/setup.py` & `packmanager-1.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 
 import setuptools
 
 setuptools.setup(
     name="packManager",
-    version="1.0.7",
+    version="1.0.8",
     description="A package manager for python",
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://chicken-muggets.github.io/packManager/",
     author="Chicken Muggets",
     license="MIT",
     project_urls={
```

