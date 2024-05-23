# Comparing `tmp/testwizard.commands-services-3.8.1b4749.tar.gz` & `tmp/testwizard.commands-services-3.8.1b4810.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testwizard.commands-services-3.8.1b4749.tar", last modified: Tue Mar 19 15:01:46 2024, max compression
+gzip compressed data, was "testwizard.commands-services-3.8.1b4810.tar", last modified: Wed Mar 27 12:56:33 2024, max compression
```

## Comparing `testwizard.commands-services-3.8.1b4749.tar` & `testwizard.commands-services-3.8.1b4810.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:46.259330 testwizard.commands-services-3.8.1b4749/
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.commands-services-3.8.1b4749/LICENSE.txt
--rw-rw-rw-   0        0        0      547 2024-03-19 15:01:46.259330 testwizard.commands-services-3.8.1b4749/PKG-INFO
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.commands-services-3.8.1b4749/README.md
--rw-rw-rw-   0        0        0       42 2024-03-19 15:01:46.259330 testwizard.commands-services-3.8.1b4749/setup.cfg
--rw-rw-rw-   0        0        0      828 2024-03-19 15:01:45.000000 testwizard.commands-services-3.8.1b4749/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:46.259330 testwizard.commands-services-3.8.1b4749/testwizard/
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:46.259330 testwizard.commands-services-3.8.1b4749/testwizard/commands_services/
--rw-rw-rw-   0        0        0      576 2024-03-19 15:00:53.000000 testwizard.commands-services-3.8.1b4749/testwizard/commands_services/SendNotificationCommand.py
--rw-rw-rw-   0        0        0      327 2024-03-19 15:00:53.000000 testwizard.commands-services-3.8.1b4749/testwizard/commands_services/SendNotificationResult.py
--rw-rw-rw-   0        0        0       60 2024-03-19 15:00:53.000000 testwizard.commands-services-3.8.1b4749/testwizard/commands_services/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:46.259330 testwizard.commands-services-3.8.1b4749/testwizard.commands_services.egg-info/
--rw-rw-rw-   0        0        0      547 2024-03-19 15:01:46.000000 testwizard.commands-services-3.8.1b4749/testwizard.commands_services.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      441 2024-03-19 15:01:46.000000 testwizard.commands-services-3.8.1b4749/testwizard.commands_services.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 15:01:46.000000 testwizard.commands-services-3.8.1b4749/testwizard.commands_services.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-03-19 15:01:46.000000 testwizard.commands-services-3.8.1b4749/testwizard.commands_services.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 15:01:46.000000 testwizard.commands-services-3.8.1b4749/testwizard.commands_services.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:33.383380 testwizard.commands-services-3.8.1b4810/
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.commands-services-3.8.1b4810/LICENSE.txt
+-rw-rw-rw-   0        0        0      547 2024-03-27 12:56:33.383380 testwizard.commands-services-3.8.1b4810/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.commands-services-3.8.1b4810/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-27 12:56:33.383380 testwizard.commands-services-3.8.1b4810/setup.cfg
+-rw-rw-rw-   0        0        0      828 2024-03-27 12:56:33.000000 testwizard.commands-services-3.8.1b4810/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:33.367756 testwizard.commands-services-3.8.1b4810/testwizard/
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:33.367756 testwizard.commands-services-3.8.1b4810/testwizard/commands_services/
+-rw-rw-rw-   0        0        0      576 2024-03-27 12:55:37.000000 testwizard.commands-services-3.8.1b4810/testwizard/commands_services/SendNotificationCommand.py
+-rw-rw-rw-   0        0        0      327 2024-03-27 12:55:37.000000 testwizard.commands-services-3.8.1b4810/testwizard/commands_services/SendNotificationResult.py
+-rw-rw-rw-   0        0        0       60 2024-03-27 12:55:37.000000 testwizard.commands-services-3.8.1b4810/testwizard/commands_services/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:33.367756 testwizard.commands-services-3.8.1b4810/testwizard.commands_services.egg-info/
+-rw-rw-rw-   0        0        0      547 2024-03-27 12:56:33.000000 testwizard.commands-services-3.8.1b4810/testwizard.commands_services.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      441 2024-03-27 12:56:33.000000 testwizard.commands-services-3.8.1b4810/testwizard.commands_services.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-27 12:56:33.000000 testwizard.commands-services-3.8.1b4810/testwizard.commands_services.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-03-27 12:56:33.000000 testwizard.commands-services-3.8.1b4810/testwizard.commands_services.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-27 12:56:33.000000 testwizard.commands-services-3.8.1b4810/testwizard.commands_services.egg-info/top_level.txt
```

### Comparing `testwizard.commands-services-3.8.1b4749/PKG-INFO` & `testwizard.commands-services-3.8.1b4810/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.commands-services
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard Services commands
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.commands-services-3.8.1b4749/setup.py` & `testwizard.commands-services-3.8.1b4810/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="testwizard.commands-services",
-    version="3.8.1b4749",
+    version="3.8.1b4810",
     author="Resillion",
     author_email="testwizard-support@resillion.com",
     description="Testwizard Services commands",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.resillion.com/services/software-testing/testing-tools/testwizard/",
     packages=['testwizard.commands_services'],
     install_requires=[
-        'testwizard.commands-core==3.8.1b4749'
+        'testwizard.commands-core==3.8.1b4810'
     ],
     classifiers=[
         "Programming Language :: Python :: 3.3",
         "Development Status :: 5 - Production/Stable",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `testwizard.commands-services-3.8.1b4749/testwizard/commands_services/SendNotificationCommand.py` & `testwizard.commands-services-3.8.1b4810/testwizard/commands_services/SendNotificationCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-services-3.8.1b4749/testwizard.commands_services.egg-info/PKG-INFO` & `testwizard.commands-services-3.8.1b4810/testwizard.commands_services.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.commands-services
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard Services commands
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

