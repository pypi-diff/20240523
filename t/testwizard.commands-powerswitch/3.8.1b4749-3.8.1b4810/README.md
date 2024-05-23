# Comparing `tmp/testwizard.commands-powerswitch-3.8.1b4749.tar.gz` & `tmp/testwizard.commands-powerswitch-3.8.1b4810.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testwizard.commands-powerswitch-3.8.1b4749.tar", last modified: Tue Mar 19 15:01:41 2024, max compression
+gzip compressed data, was "testwizard.commands-powerswitch-3.8.1b4810.tar", last modified: Wed Mar 27 12:56:28 2024, max compression
```

## Comparing `testwizard.commands-powerswitch-3.8.1b4749.tar` & `testwizard.commands-powerswitch-3.8.1b4810.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:41.647498 testwizard.commands-powerswitch-3.8.1b4749/
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.commands-powerswitch-3.8.1b4749/LICENSE.txt
--rw-rw-rw-   0        0        0      553 2024-03-19 15:01:41.631876 testwizard.commands-powerswitch-3.8.1b4749/PKG-INFO
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.commands-powerswitch-3.8.1b4749/README.md
--rw-rw-rw-   0        0        0       42 2024-03-19 15:01:41.647498 testwizard.commands-powerswitch-3.8.1b4749/setup.cfg
--rw-rw-rw-   0        0        0      923 2024-03-19 15:01:41.000000 testwizard.commands-powerswitch-3.8.1b4749/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:41.631876 testwizard.commands-powerswitch-3.8.1b4749/testwizard/
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:41.631876 testwizard.commands-powerswitch-3.8.1b4749/testwizard/commands_powerswitch/
--rw-rw-rw-   0        0        0      529 2024-03-19 15:00:53.000000 testwizard.commands-powerswitch-3.8.1b4749/testwizard/commands_powerswitch/GetPowerSwitchStatusCommand.py
--rw-rw-rw-   0        0        0      329 2024-03-19 15:00:53.000000 testwizard.commands-powerswitch-3.8.1b4749/testwizard/commands_powerswitch/GetPowerSwitchStatusResult.py
--rw-rw-rw-   0        0        0      485 2024-03-19 15:00:53.000000 testwizard.commands-powerswitch-3.8.1b4749/testwizard/commands_powerswitch/SwitchPowerCommand.py
--rw-rw-rw-   0        0        0      491 2024-03-19 15:00:53.000000 testwizard.commands-powerswitch-3.8.1b4749/testwizard/commands_powerswitch/SwitchPowerOffCommand.py
--rw-rw-rw-   0        0        0      487 2024-03-19 15:00:53.000000 testwizard.commands-powerswitch-3.8.1b4749/testwizard/commands_powerswitch/SwitchPowerOnCommand.py
--rw-rw-rw-   0        0        0      234 2024-03-19 15:00:53.000000 testwizard.commands-powerswitch-3.8.1b4749/testwizard/commands_powerswitch/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:41.631876 testwizard.commands-powerswitch-3.8.1b4749/testwizard.commands_powerswitch.egg-info/
--rw-rw-rw-   0        0        0      553 2024-03-19 15:01:41.000000 testwizard.commands-powerswitch-3.8.1b4749/testwizard.commands_powerswitch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      640 2024-03-19 15:01:41.000000 testwizard.commands-powerswitch-3.8.1b4749/testwizard.commands_powerswitch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 15:01:41.000000 testwizard.commands-powerswitch-3.8.1b4749/testwizard.commands_powerswitch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-03-19 15:01:41.000000 testwizard.commands-powerswitch-3.8.1b4749/testwizard.commands_powerswitch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 15:01:41.000000 testwizard.commands-powerswitch-3.8.1b4749/testwizard.commands_powerswitch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:28.255512 testwizard.commands-powerswitch-3.8.1b4810/
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.commands-powerswitch-3.8.1b4810/LICENSE.txt
+-rw-rw-rw-   0        0        0      553 2024-03-27 12:56:28.255512 testwizard.commands-powerswitch-3.8.1b4810/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.commands-powerswitch-3.8.1b4810/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-27 12:56:28.255512 testwizard.commands-powerswitch-3.8.1b4810/setup.cfg
+-rw-rw-rw-   0        0        0      923 2024-03-27 12:56:27.000000 testwizard.commands-powerswitch-3.8.1b4810/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:28.239889 testwizard.commands-powerswitch-3.8.1b4810/testwizard/
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:28.255512 testwizard.commands-powerswitch-3.8.1b4810/testwizard/commands_powerswitch/
+-rw-rw-rw-   0        0        0      529 2024-03-27 12:55:37.000000 testwizard.commands-powerswitch-3.8.1b4810/testwizard/commands_powerswitch/GetPowerSwitchStatusCommand.py
+-rw-rw-rw-   0        0        0      329 2024-03-27 12:55:37.000000 testwizard.commands-powerswitch-3.8.1b4810/testwizard/commands_powerswitch/GetPowerSwitchStatusResult.py
+-rw-rw-rw-   0        0        0      485 2024-03-27 12:55:37.000000 testwizard.commands-powerswitch-3.8.1b4810/testwizard/commands_powerswitch/SwitchPowerCommand.py
+-rw-rw-rw-   0        0        0      491 2024-03-27 12:55:37.000000 testwizard.commands-powerswitch-3.8.1b4810/testwizard/commands_powerswitch/SwitchPowerOffCommand.py
+-rw-rw-rw-   0        0        0      487 2024-03-27 12:55:37.000000 testwizard.commands-powerswitch-3.8.1b4810/testwizard/commands_powerswitch/SwitchPowerOnCommand.py
+-rw-rw-rw-   0        0        0      234 2024-03-27 12:55:37.000000 testwizard.commands-powerswitch-3.8.1b4810/testwizard/commands_powerswitch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:28.255512 testwizard.commands-powerswitch-3.8.1b4810/testwizard.commands_powerswitch.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-03-27 12:56:28.000000 testwizard.commands-powerswitch-3.8.1b4810/testwizard.commands_powerswitch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      640 2024-03-27 12:56:28.000000 testwizard.commands-powerswitch-3.8.1b4810/testwizard.commands_powerswitch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-27 12:56:28.000000 testwizard.commands-powerswitch-3.8.1b4810/testwizard.commands_powerswitch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-03-27 12:56:28.000000 testwizard.commands-powerswitch-3.8.1b4810/testwizard.commands_powerswitch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-27 12:56:28.000000 testwizard.commands-powerswitch-3.8.1b4810/testwizard.commands_powerswitch.egg-info/top_level.txt
```

### Comparing `testwizard.commands-powerswitch-3.8.1b4749/PKG-INFO` & `testwizard.commands-powerswitch-3.8.1b4810/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.commands-powerswitch
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard Powerswitch commands
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.commands-powerswitch-3.8.1b4749/setup.py` & `testwizard.commands-powerswitch-3.8.1b4810/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="testwizard.commands-powerswitch",
-    version="3.8.1b4749",
+    version="3.8.1b4810",
     author="Resillion",
     author_email="testwizard-support@resillion.com",
     description="Testwizard Powerswitch commands",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.resillion.com/services/software-testing/testing-tools/testwizard/",
     packages=['testwizard.commands_powerswitch'],
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

### Comparing `testwizard.commands-powerswitch-3.8.1b4749/testwizard/commands_powerswitch/GetPowerSwitchStatusCommand.py` & `testwizard.commands-powerswitch-3.8.1b4810/testwizard/commands_powerswitch/GetPowerSwitchStatusCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-powerswitch-3.8.1b4749/testwizard.commands_powerswitch.egg-info/PKG-INFO` & `testwizard.commands-powerswitch-3.8.1b4810/testwizard.commands_powerswitch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.commands-powerswitch
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard Powerswitch commands
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.commands-powerswitch-3.8.1b4749/testwizard.commands_powerswitch.egg-info/SOURCES.txt` & `testwizard.commands-powerswitch-3.8.1b4810/testwizard.commands_powerswitch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

