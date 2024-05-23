# Comparing `tmp/testwizard.commands-remotecontrol-3.8.1b4749.tar.gz` & `tmp/testwizard.commands-remotecontrol-3.8.1b4810.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testwizard.commands-remotecontrol-3.8.1b4749.tar", last modified: Tue Mar 19 15:01:42 2024, max compression
+gzip compressed data, was "testwizard.commands-remotecontrol-3.8.1b4810.tar", last modified: Wed Mar 27 12:56:29 2024, max compression
```

## Comparing `testwizard.commands-remotecontrol-3.8.1b4749.tar` & `testwizard.commands-remotecontrol-3.8.1b4810.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:42.507650 testwizard.commands-remotecontrol-3.8.1b4749/
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.commands-remotecontrol-3.8.1b4749/LICENSE.txt
--rw-rw-rw-   0        0        0      558 2024-03-19 15:01:42.507650 testwizard.commands-remotecontrol-3.8.1b4749/PKG-INFO
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.commands-remotecontrol-3.8.1b4749/README.md
--rw-rw-rw-   0        0        0       42 2024-03-19 15:01:42.507650 testwizard.commands-remotecontrol-3.8.1b4749/setup.cfg
--rw-rw-rw-   0        0        0      930 2024-03-19 15:01:42.000000 testwizard.commands-remotecontrol-3.8.1b4749/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:42.492026 testwizard.commands-remotecontrol-3.8.1b4749/testwizard/
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:42.507650 testwizard.commands-remotecontrol-3.8.1b4749/testwizard/commands_remotecontrol/
--rw-rw-rw-   0        0        0      472 2024-03-19 15:00:53.000000 testwizard.commands-remotecontrol-3.8.1b4749/testwizard/commands_remotecontrol/SendRCKeyCommand.py
--rw-rw-rw-   0        0        0      468 2024-03-19 15:00:53.000000 testwizard.commands-remotecontrol-3.8.1b4749/testwizard/commands_remotecontrol/SendRCKeyResult.py
--rw-rw-rw-   0        0        0       46 2024-03-19 15:00:53.000000 testwizard.commands-remotecontrol-3.8.1b4749/testwizard/commands_remotecontrol/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:42.492026 testwizard.commands-remotecontrol-3.8.1b4749/testwizard.commands_remotecontrol.egg-info/
--rw-rw-rw-   0        0        0      558 2024-03-19 15:01:42.000000 testwizard.commands-remotecontrol-3.8.1b4749/testwizard.commands_remotecontrol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      467 2024-03-19 15:01:42.000000 testwizard.commands-remotecontrol-3.8.1b4749/testwizard.commands_remotecontrol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 15:01:42.000000 testwizard.commands-remotecontrol-3.8.1b4749/testwizard.commands_remotecontrol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-03-19 15:01:42.000000 testwizard.commands-remotecontrol-3.8.1b4749/testwizard.commands_remotecontrol.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 15:01:42.000000 testwizard.commands-remotecontrol-3.8.1b4749/testwizard.commands_remotecontrol.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:29.131000 testwizard.commands-remotecontrol-3.8.1b4810/
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.commands-remotecontrol-3.8.1b4810/LICENSE.txt
+-rw-rw-rw-   0        0        0      558 2024-03-27 12:56:29.131000 testwizard.commands-remotecontrol-3.8.1b4810/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.commands-remotecontrol-3.8.1b4810/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-27 12:56:29.131000 testwizard.commands-remotecontrol-3.8.1b4810/setup.cfg
+-rw-rw-rw-   0        0        0      930 2024-03-27 12:56:28.000000 testwizard.commands-remotecontrol-3.8.1b4810/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:29.131000 testwizard.commands-remotecontrol-3.8.1b4810/testwizard/
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:29.131000 testwizard.commands-remotecontrol-3.8.1b4810/testwizard/commands_remotecontrol/
+-rw-rw-rw-   0        0        0      472 2024-03-27 12:55:37.000000 testwizard.commands-remotecontrol-3.8.1b4810/testwizard/commands_remotecontrol/SendRCKeyCommand.py
+-rw-rw-rw-   0        0        0      468 2024-03-27 12:55:37.000000 testwizard.commands-remotecontrol-3.8.1b4810/testwizard/commands_remotecontrol/SendRCKeyResult.py
+-rw-rw-rw-   0        0        0       46 2024-03-27 12:55:37.000000 testwizard.commands-remotecontrol-3.8.1b4810/testwizard/commands_remotecontrol/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:29.131000 testwizard.commands-remotecontrol-3.8.1b4810/testwizard.commands_remotecontrol.egg-info/
+-rw-rw-rw-   0        0        0      558 2024-03-27 12:56:29.000000 testwizard.commands-remotecontrol-3.8.1b4810/testwizard.commands_remotecontrol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      467 2024-03-27 12:56:29.000000 testwizard.commands-remotecontrol-3.8.1b4810/testwizard.commands_remotecontrol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-27 12:56:29.000000 testwizard.commands-remotecontrol-3.8.1b4810/testwizard.commands_remotecontrol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-03-27 12:56:29.000000 testwizard.commands-remotecontrol-3.8.1b4810/testwizard.commands_remotecontrol.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-27 12:56:29.000000 testwizard.commands-remotecontrol-3.8.1b4810/testwizard.commands_remotecontrol.egg-info/top_level.txt
```

### Comparing `testwizard.commands-remotecontrol-3.8.1b4749/PKG-INFO` & `testwizard.commands-remotecontrol-3.8.1b4810/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.commands-remotecontrol
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard Remote control commands
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.commands-remotecontrol-3.8.1b4749/setup.py` & `testwizard.commands-remotecontrol-3.8.1b4810/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="testwizard.commands-remotecontrol",
-    version="3.8.1b4749",
+    version="3.8.1b4810",
     author="Resillion",
     author_email="testwizard-support@resillion.com",
     description="Testwizard Remote control commands",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.resillion.com/services/software-testing/testing-tools/testwizard/",
     packages=['testwizard.commands_remotecontrol'],
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

### Comparing `testwizard.commands-remotecontrol-3.8.1b4749/testwizard.commands_remotecontrol.egg-info/PKG-INFO` & `testwizard.commands-remotecontrol-3.8.1b4810/testwizard.commands_remotecontrol.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.commands-remotecontrol
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard Remote control commands
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

