# Comparing `tmp/packmanager-1.0.5.tar.gz` & `tmp/packmanager-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packmanager-1.0.5.tar", last modified: Thu May 23 07:11:43 2024, max compression
+gzip compressed data, was "packmanager-1.0.6.tar", last modified: Thu May 23 07:20:08 2024, max compression
```

## Comparing `packmanager-1.0.5.tar` & `packmanager-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 07:11:43.430146 packmanager-1.0.5/
--rw-rw-rw-   0        0        0       85 2024-05-22 12:41:47.000000 packmanager-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      810 2024-05-23 07:11:43.427146 packmanager-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-05-22 08:13:58.000000 packmanager-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 07:11:43.384136 packmanager-1.0.5/packManager/
--rw-rw-rw-   0        0        0     1251 2024-05-23 07:10:40.000000 packmanager-1.0.5/packManager/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 07:11:43.424145 packmanager-1.0.5/packManager.egg-info/
--rw-rw-rw-   0        0        0      810 2024-05-23 07:11:43.000000 packmanager-1.0.5/packManager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-05-23 07:11:43.000000 packmanager-1.0.5/packManager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 07:11:43.000000 packmanager-1.0.5/packManager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-23 07:11:43.000000 packmanager-1.0.5/packManager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2024-05-22 12:42:05.000000 packmanager-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-23 07:11:43.431146 packmanager-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      855 2024-05-23 07:10:31.000000 packmanager-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:20:08.266245 packmanager-1.0.6/
+-rw-rw-rw-   0        0        0       85 2024-05-22 12:41:47.000000 packmanager-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      810 2024-05-23 07:20:08.264251 packmanager-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-05-22 08:13:58.000000 packmanager-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 07:20:08.223526 packmanager-1.0.6/packManager/
+-rw-rw-rw-   0        0        0     1427 2024-05-23 07:18:59.000000 packmanager-1.0.6/packManager/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:20:08.261244 packmanager-1.0.6/packManager.egg-info/
+-rw-rw-rw-   0        0        0      810 2024-05-23 07:20:08.000000 packmanager-1.0.6/packManager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-05-23 07:20:08.000000 packmanager-1.0.6/packManager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 07:20:08.000000 packmanager-1.0.6/packManager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-23 07:20:08.000000 packmanager-1.0.6/packManager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2024-05-22 12:42:05.000000 packmanager-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 07:20:08.266245 packmanager-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      855 2024-05-23 07:19:39.000000 packmanager-1.0.6/setup.py
```

### Comparing `packmanager-1.0.5/PKG-INFO` & `packmanager-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packManager
-Version: 1.0.5
+Version: 1.0.6
 Summary: A package manager for python
 Home-page: https://chicken-muggets.github.io/packManager/
 Author: Chicken Muggets
 License: MIT
 Project-URL: Documentation, https://github.com/chicken-muggets/PackInst/wiki
 Project-URL: Source, https://github.com/chicken-muggets/PackInst
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `packmanager-1.0.5/packManager/__init__.py` & `packmanager-1.0.6/packManager/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,8 +20,15 @@
         else:
             os.system('pip uninstall ' + package)
         print(package + ' uninstalled successfully')
     if consCall == 0 or consCall == False:
         if hasInput == False or hasInput == 0:
             os.system('pip uninstall ' + package + ' ' + '-q -q -q ' + '-y')
         else:
-            os.system('pip uninstall ' + package + ' ' + '-q -q -q ')
+            os.system('pip uninstall ' + package + ' ' + '-q -q -q ')
+def testInstall(package):
+    import importlib.util
+    spec = importlib.util.find_spec(package)
+    if spec is None:
+        return False
+    else:
+        return True
```

### Comparing `packmanager-1.0.5/packManager.egg-info/PKG-INFO` & `packmanager-1.0.6/packManager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packManager
-Version: 1.0.5
+Version: 1.0.6
 Summary: A package manager for python
 Home-page: https://chicken-muggets.github.io/packManager/
 Author: Chicken Muggets
 License: MIT
 Project-URL: Documentation, https://github.com/chicken-muggets/PackInst/wiki
 Project-URL: Source, https://github.com/chicken-muggets/PackInst
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `packmanager-1.0.5/setup.py` & `packmanager-1.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 
 import setuptools
 
 setuptools.setup(
     name="packManager",
-    version="1.0.5",
+    version="1.0.6",
     description="A package manager for python",
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://chicken-muggets.github.io/packManager/",
     author="Chicken Muggets",
     license="MIT",
     project_urls={
```

