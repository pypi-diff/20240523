# Comparing `tmp/testwizard.commands-camera-3.8.1b4749.tar.gz` & `tmp/testwizard.commands-camera-3.8.1b4810.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testwizard.commands-camera-3.8.1b4749.tar", last modified: Tue Mar 19 15:01:45 2024, max compression
+gzip compressed data, was "testwizard.commands-camera-3.8.1b4810.tar", last modified: Wed Mar 27 12:56:32 2024, max compression
```

## Comparing `testwizard.commands-camera-3.8.1b4749.tar` & `testwizard.commands-camera-3.8.1b4810.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:45.415232 testwizard.commands-camera-3.8.1b4749/
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.commands-camera-3.8.1b4749/LICENSE.txt
--rw-rw-rw-   0        0        0      543 2024-03-19 15:01:45.415232 testwizard.commands-camera-3.8.1b4749/PKG-INFO
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.commands-camera-3.8.1b4749/README.md
--rw-rw-rw-   0        0        0       42 2024-03-19 15:01:45.415232 testwizard.commands-camera-3.8.1b4749/setup.cfg
--rw-rw-rw-   0        0        0      840 2024-03-19 15:01:45.000000 testwizard.commands-camera-3.8.1b4749/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:45.399611 testwizard.commands-camera-3.8.1b4749/testwizard/
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:45.415232 testwizard.commands-camera-3.8.1b4749/testwizard/commands_camera/
--rw-rw-rw-   0        0        0      736 2024-03-19 15:00:53.000000 testwizard.commands-camera-3.8.1b4749/testwizard/commands_camera/CameraDetectMotionCommand.py
--rw-rw-rw-   0        0        0      558 2024-03-19 15:00:53.000000 testwizard.commands-camera-3.8.1b4749/testwizard/commands_camera/CameraDetectMotionResult.py
--rw-rw-rw-   0        0        0      547 2024-03-19 15:00:53.000000 testwizard.commands-camera-3.8.1b4749/testwizard/commands_camera/CameraInitializeNetworkCommand.py
--rw-rw-rw-   0        0        0      512 2024-03-19 15:00:53.000000 testwizard.commands-camera-3.8.1b4749/testwizard/commands_camera/CameraSnapShotCommand.py
--rw-rw-rw-   0        0        0      322 2024-03-19 15:00:53.000000 testwizard.commands-camera-3.8.1b4749/testwizard/commands_camera/CameraSnapShotResult.py
--rw-rw-rw-   0        0        0      760 2024-03-19 15:00:53.000000 testwizard.commands-camera-3.8.1b4749/testwizard/commands_camera/CameraWaitForPatternCommand.py
--rw-rw-rw-   0        0        0      788 2024-03-19 15:00:53.000000 testwizard.commands-camera-3.8.1b4749/testwizard/commands_camera/CameraWaitForPatternNoMatchCommand.py
--rw-rw-rw-   0        0        0      726 2024-03-19 15:00:53.000000 testwizard.commands-camera-3.8.1b4749/testwizard/commands_camera/CameraWaitForSampleCommand.py
--rw-rw-rw-   0        0        0      754 2024-03-19 15:00:53.000000 testwizard.commands-camera-3.8.1b4749/testwizard/commands_camera/CameraWaitForSampleNoMatchCommand.py
--rw-rw-rw-   0        0        0      543 2024-03-19 15:00:53.000000 testwizard.commands-camera-3.8.1b4749/testwizard/commands_camera/CameraWaitForSampleResult.py
--rw-rw-rw-   0        0        0      502 2024-03-19 15:00:53.000000 testwizard.commands-camera-3.8.1b4749/testwizard/commands_camera/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:45.415232 testwizard.commands-camera-3.8.1b4749/testwizard.commands_camera.egg-info/
--rw-rw-rw-   0        0        0      543 2024-03-19 15:01:45.000000 testwizard.commands-camera-3.8.1b4749/testwizard.commands_camera.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      893 2024-03-19 15:01:45.000000 testwizard.commands-camera-3.8.1b4749/testwizard.commands_camera.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 15:01:45.000000 testwizard.commands-camera-3.8.1b4749/testwizard.commands_camera.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-03-19 15:01:45.000000 testwizard.commands-camera-3.8.1b4749/testwizard.commands_camera.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 15:01:45.000000 testwizard.commands-camera-3.8.1b4749/testwizard.commands_camera.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:32.507399 testwizard.commands-camera-3.8.1b4810/
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.commands-camera-3.8.1b4810/LICENSE.txt
+-rw-rw-rw-   0        0        0      543 2024-03-27 12:56:32.491775 testwizard.commands-camera-3.8.1b4810/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.commands-camera-3.8.1b4810/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-27 12:56:32.507399 testwizard.commands-camera-3.8.1b4810/setup.cfg
+-rw-rw-rw-   0        0        0      840 2024-03-27 12:56:32.000000 testwizard.commands-camera-3.8.1b4810/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:32.491775 testwizard.commands-camera-3.8.1b4810/testwizard/
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:32.491775 testwizard.commands-camera-3.8.1b4810/testwizard/commands_camera/
+-rw-rw-rw-   0        0        0      736 2024-03-27 12:55:37.000000 testwizard.commands-camera-3.8.1b4810/testwizard/commands_camera/CameraDetectMotionCommand.py
+-rw-rw-rw-   0        0        0      558 2024-03-27 12:55:37.000000 testwizard.commands-camera-3.8.1b4810/testwizard/commands_camera/CameraDetectMotionResult.py
+-rw-rw-rw-   0        0        0      547 2024-03-27 12:55:37.000000 testwizard.commands-camera-3.8.1b4810/testwizard/commands_camera/CameraInitializeNetworkCommand.py
+-rw-rw-rw-   0        0        0      512 2024-03-27 12:55:37.000000 testwizard.commands-camera-3.8.1b4810/testwizard/commands_camera/CameraSnapShotCommand.py
+-rw-rw-rw-   0        0        0      322 2024-03-27 12:55:37.000000 testwizard.commands-camera-3.8.1b4810/testwizard/commands_camera/CameraSnapShotResult.py
+-rw-rw-rw-   0        0        0      760 2024-03-27 12:55:37.000000 testwizard.commands-camera-3.8.1b4810/testwizard/commands_camera/CameraWaitForPatternCommand.py
+-rw-rw-rw-   0        0        0      788 2024-03-27 12:55:37.000000 testwizard.commands-camera-3.8.1b4810/testwizard/commands_camera/CameraWaitForPatternNoMatchCommand.py
+-rw-rw-rw-   0        0        0      726 2024-03-27 12:55:37.000000 testwizard.commands-camera-3.8.1b4810/testwizard/commands_camera/CameraWaitForSampleCommand.py
+-rw-rw-rw-   0        0        0      754 2024-03-27 12:55:37.000000 testwizard.commands-camera-3.8.1b4810/testwizard/commands_camera/CameraWaitForSampleNoMatchCommand.py
+-rw-rw-rw-   0        0        0      543 2024-03-27 12:55:37.000000 testwizard.commands-camera-3.8.1b4810/testwizard/commands_camera/CameraWaitForSampleResult.py
+-rw-rw-rw-   0        0        0      502 2024-03-27 12:55:37.000000 testwizard.commands-camera-3.8.1b4810/testwizard/commands_camera/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:32.491775 testwizard.commands-camera-3.8.1b4810/testwizard.commands_camera.egg-info/
+-rw-rw-rw-   0        0        0      543 2024-03-27 12:56:32.000000 testwizard.commands-camera-3.8.1b4810/testwizard.commands_camera.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      893 2024-03-27 12:56:32.000000 testwizard.commands-camera-3.8.1b4810/testwizard.commands_camera.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-27 12:56:32.000000 testwizard.commands-camera-3.8.1b4810/testwizard.commands_camera.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-03-27 12:56:32.000000 testwizard.commands-camera-3.8.1b4810/testwizard.commands_camera.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-27 12:56:32.000000 testwizard.commands-camera-3.8.1b4810/testwizard.commands_camera.egg-info/top_level.txt
```

### Comparing `testwizard.commands-camera-3.8.1b4749/PKG-INFO` & `testwizard.commands-camera-3.8.1b4810/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.commands-camera
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard camera commands
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.commands-camera-3.8.1b4749/setup.py` & `testwizard.commands-camera-3.8.1b4810/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="testwizard.commands-camera",
-    version="3.8.1b4749",
+    version="3.8.1b4810",
     author="Resillion",
     author_email="testwizard-support@resillion.com",
     description="Testwizard camera commands",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.resillion.com/services/software-testing/testing-tools/testwizard/",
     packages=['testwizard.commands_camera'],
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

### Comparing `testwizard.commands-camera-3.8.1b4749/testwizard/commands_camera/CameraDetectMotionCommand.py` & `testwizard.commands-camera-3.8.1b4810/testwizard/commands_camera/CameraDetectMotionCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-camera-3.8.1b4749/testwizard/commands_camera/CameraDetectMotionResult.py` & `testwizard.commands-camera-3.8.1b4810/testwizard/commands_camera/CameraDetectMotionResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-camera-3.8.1b4749/testwizard/commands_camera/CameraInitializeNetworkCommand.py` & `testwizard.commands-camera-3.8.1b4810/testwizard/commands_camera/CameraInitializeNetworkCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-camera-3.8.1b4749/testwizard/commands_camera/CameraSnapShotCommand.py` & `testwizard.commands-camera-3.8.1b4810/testwizard/commands_camera/CameraSnapShotCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-camera-3.8.1b4749/testwizard/commands_camera/CameraWaitForPatternCommand.py` & `testwizard.commands-camera-3.8.1b4810/testwizard/commands_camera/CameraWaitForPatternCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-camera-3.8.1b4749/testwizard/commands_camera/CameraWaitForPatternNoMatchCommand.py` & `testwizard.commands-camera-3.8.1b4810/testwizard/commands_camera/CameraWaitForPatternNoMatchCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-camera-3.8.1b4749/testwizard/commands_camera/CameraWaitForSampleCommand.py` & `testwizard.commands-camera-3.8.1b4810/testwizard/commands_camera/CameraWaitForSampleCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-camera-3.8.1b4749/testwizard/commands_camera/CameraWaitForSampleNoMatchCommand.py` & `testwizard.commands-camera-3.8.1b4810/testwizard/commands_camera/CameraWaitForSampleNoMatchCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-camera-3.8.1b4749/testwizard/commands_camera/CameraWaitForSampleResult.py` & `testwizard.commands-camera-3.8.1b4810/testwizard/commands_camera/CameraWaitForSampleResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-camera-3.8.1b4749/testwizard.commands_camera.egg-info/PKG-INFO` & `testwizard.commands-camera-3.8.1b4810/testwizard.commands_camera.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.commands-camera
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard camera commands
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.commands-camera-3.8.1b4749/testwizard.commands_camera.egg-info/SOURCES.txt` & `testwizard.commands-camera-3.8.1b4810/testwizard.commands_camera.egg-info/SOURCES.txt`

 * *Files identical despite different names*

