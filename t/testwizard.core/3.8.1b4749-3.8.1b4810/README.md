# Comparing `tmp/testwizard.core-3.8.1b4749.tar.gz` & `tmp/testwizard.core-3.8.1b4810.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testwizard.core-3.8.1b4749.tar", last modified: Tue Mar 19 15:01:37 2024, max compression
+gzip compressed data, was "testwizard.core-3.8.1b4810.tar", last modified: Wed Mar 27 12:56:23 2024, max compression
```

## Comparing `testwizard.core-3.8.1b4749.tar` & `testwizard.core-3.8.1b4810.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:37.020967 testwizard.core-3.8.1b4749/
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/LICENSE.txt
--rw-rw-rw-   0        0        0      521 2024-03-19 15:01:37.020967 testwizard.core-3.8.1b4749/PKG-INFO
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/README.md
--rw-rw-rw-   0        0        0       42 2024-03-19 15:01:37.020967 testwizard.core-3.8.1b4749/setup.cfg
--rw-rw-rw-   0        0        0      816 2024-03-19 15:01:35.000000 testwizard.core-3.8.1b4749/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:37.005343 testwizard.core-3.8.1b4749/testwizard/
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:37.020967 testwizard.core-3.8.1b4749/testwizard/core/
--rw-rw-rw-   0        0        0      595 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/CustomProperties.py
--rw-rw-rw-   0        0        0      688 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/EnvironmentInfo.py
--rw-rw-rw-   0        0        0       90 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/Errors.py
--rw-rw-rw-   0        0        0      454 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/ManagerSessionInfo.py
--rw-rw-rw-   0        0        0      593 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/Parameters.py
--rw-rw-rw-   0        0        0     4240 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/RestClient.py
--rw-rw-rw-   0        0        0      155 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/ResultCodes.py
--rw-rw-rw-   0        0        0     1900 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/RobotClient.py
--rw-rw-rw-   0        0        0     5253 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/Session.py
--rw-rw-rw-   0        0        0     1171 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/SessionInfo.py
--rw-rw-rw-   0        0        0      201 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/SideCarFileReader.py
--rw-rw-rw-   0        0        0     2707 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/TestWizard.py
--rw-rw-rw-   0        0        0       72 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:37.020967 testwizard.core-3.8.1b4749/testwizard/core/commands/
--rw-rw-rw-   0        0        0      551 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/commands/AddCustomDataCommand.py
--rw-rw-rw-   0        0        0      623 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/commands/AddPerformanceDataCommand.py
--rw-rw-rw-   0        0        0      517 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/commands/BeginStepCommand.py
--rw-rw-rw-   0        0        0      519 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/commands/CancelCommandsCommand.py
--rw-rw-rw-   0        0        0      555 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/commands/EndStepCommand.py
--rw-rw-rw-   0        0        0      734 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/commands/EndStepResult.py
--rw-rw-rw-   0        0        0      140 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/commands/StepExecutionResult.py
--rw-rw-rw-   0        0        0      527 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/commands/StringCompareCommand.py
--rw-rw-rw-   0        0        0      761 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/commands/StringCompareResult.py
--rw-rw-rw-   0        0        0      580 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/commands/WaitForCommandCompletionCommand.py
--rw-rw-rw-   0        0        0      399 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:37.020967 testwizard.core-3.8.1b4749/testwizard/core/models/
--rw-rw-rw-   0        0        0     1060 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/models/CreateTestRunRequest.py
--rw-rw-rw-   0        0        0      283 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/models/TestResult.py
--rw-rw-rw-   0        0        0       60 2024-03-19 15:00:53.000000 testwizard.core-3.8.1b4749/testwizard/core/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:37.005343 testwizard.core-3.8.1b4749/testwizard.core.egg-info/
--rw-rw-rw-   0        0        0      521 2024-03-19 15:01:36.000000 testwizard.core-3.8.1b4749/testwizard.core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1278 2024-03-19 15:01:36.000000 testwizard.core-3.8.1b4749/testwizard.core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 15:01:36.000000 testwizard.core-3.8.1b4749/testwizard.core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-03-19 15:01:36.000000 testwizard.core-3.8.1b4749/testwizard.core.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 15:01:36.000000 testwizard.core-3.8.1b4749/testwizard.core.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:23.378349 testwizard.core-3.8.1b4810/
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/LICENSE.txt
+-rw-rw-rw-   0        0        0      521 2024-03-27 12:56:23.378349 testwizard.core-3.8.1b4810/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-27 12:56:23.378349 testwizard.core-3.8.1b4810/setup.cfg
+-rw-rw-rw-   0        0        0      816 2024-03-27 12:56:20.000000 testwizard.core-3.8.1b4810/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:23.356315 testwizard.core-3.8.1b4810/testwizard/
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:23.364450 testwizard.core-3.8.1b4810/testwizard/core/
+-rw-rw-rw-   0        0        0      595 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/CustomProperties.py
+-rw-rw-rw-   0        0        0      688 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/EnvironmentInfo.py
+-rw-rw-rw-   0        0        0       90 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/Errors.py
+-rw-rw-rw-   0        0        0      454 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/ManagerSessionInfo.py
+-rw-rw-rw-   0        0        0      593 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/Parameters.py
+-rw-rw-rw-   0        0        0     4240 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/RestClient.py
+-rw-rw-rw-   0        0        0      155 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/ResultCodes.py
+-rw-rw-rw-   0        0        0     1900 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/RobotClient.py
+-rw-rw-rw-   0        0        0     5253 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/Session.py
+-rw-rw-rw-   0        0        0     1171 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/SessionInfo.py
+-rw-rw-rw-   0        0        0      201 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/SideCarFileReader.py
+-rw-rw-rw-   0        0        0     2707 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/TestWizard.py
+-rw-rw-rw-   0        0        0       72 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:23.375337 testwizard.core-3.8.1b4810/testwizard/core/commands/
+-rw-rw-rw-   0        0        0      551 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/commands/AddCustomDataCommand.py
+-rw-rw-rw-   0        0        0      623 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/commands/AddPerformanceDataCommand.py
+-rw-rw-rw-   0        0        0      517 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/commands/BeginStepCommand.py
+-rw-rw-rw-   0        0        0      519 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/commands/CancelCommandsCommand.py
+-rw-rw-rw-   0        0        0      555 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/commands/EndStepCommand.py
+-rw-rw-rw-   0        0        0      734 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/commands/EndStepResult.py
+-rw-rw-rw-   0        0        0      140 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/commands/StepExecutionResult.py
+-rw-rw-rw-   0        0        0      527 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/commands/StringCompareCommand.py
+-rw-rw-rw-   0        0        0      761 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/commands/StringCompareResult.py
+-rw-rw-rw-   0        0        0      580 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/commands/WaitForCommandCompletionCommand.py
+-rw-rw-rw-   0        0        0      399 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:23.378349 testwizard.core-3.8.1b4810/testwizard/core/models/
+-rw-rw-rw-   0        0        0     1060 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/models/CreateTestRunRequest.py
+-rw-rw-rw-   0        0        0      283 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/models/TestResult.py
+-rw-rw-rw-   0        0        0       60 2024-03-27 12:55:37.000000 testwizard.core-3.8.1b4810/testwizard/core/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:23.364450 testwizard.core-3.8.1b4810/testwizard.core.egg-info/
+-rw-rw-rw-   0        0        0      521 2024-03-27 12:56:23.000000 testwizard.core-3.8.1b4810/testwizard.core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1278 2024-03-27 12:56:23.000000 testwizard.core-3.8.1b4810/testwizard.core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-27 12:56:23.000000 testwizard.core-3.8.1b4810/testwizard.core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-03-27 12:56:23.000000 testwizard.core-3.8.1b4810/testwizard.core.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-27 12:56:23.000000 testwizard.core-3.8.1b4810/testwizard.core.egg-info/top_level.txt
```

### Comparing `testwizard.core-3.8.1b4749/PKG-INFO` & `testwizard.core-3.8.1b4810/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.core
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard core
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.core-3.8.1b4749/setup.py` & `testwizard.core-3.8.1b4810/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_namespace_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="testwizard.core",
-    version="3.8.1b4749",
+    version="3.8.1b4810",
     author="Resillion",
     author_email="testwizard-support@resillion.com",
     description="Testwizard core",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.resillion.com/services/software-testing/testing-tools/testwizard/",
     packages=find_namespace_packages(),
     install_requires=[
           'jsons',
-          'testwizard.commands-core==3.8.1b4749'
+          'testwizard.commands-core==3.8.1b4810'
     ],
     classifiers=[
         "Programming Language :: Python :: 3.3",
         "Development Status :: 5 - Production/Stable",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `testwizard.core-3.8.1b4749/testwizard/core/CustomProperties.py` & `testwizard.core-3.8.1b4810/testwizard/core/CustomProperties.py`

 * *Files identical despite different names*

### Comparing `testwizard.core-3.8.1b4749/testwizard/core/EnvironmentInfo.py` & `testwizard.core-3.8.1b4810/testwizard/core/EnvironmentInfo.py`

 * *Files identical despite different names*

### Comparing `testwizard.core-3.8.1b4749/testwizard/core/Parameters.py` & `testwizard.core-3.8.1b4810/testwizard/core/Parameters.py`

 * *Files identical despite different names*

### Comparing `testwizard.core-3.8.1b4749/testwizard/core/RestClient.py` & `testwizard.core-3.8.1b4810/testwizard/core/RestClient.py`

 * *Files identical despite different names*

### Comparing `testwizard.core-3.8.1b4749/testwizard/core/RobotClient.py` & `testwizard.core-3.8.1b4810/testwizard/core/RobotClient.py`

 * *Files identical despite different names*

### Comparing `testwizard.core-3.8.1b4749/testwizard/core/Session.py` & `testwizard.core-3.8.1b4810/testwizard/core/Session.py`

 * *Files identical despite different names*

### Comparing `testwizard.core-3.8.1b4749/testwizard/core/SessionInfo.py` & `testwizard.core-3.8.1b4810/testwizard/core/SessionInfo.py`

 * *Files identical despite different names*

### Comparing `testwizard.core-3.8.1b4749/testwizard/core/TestWizard.py` & `testwizard.core-3.8.1b4810/testwizard/core/TestWizard.py`

 * *Files identical despite different names*

### Comparing `testwizard.core-3.8.1b4749/testwizard/core/commands/AddCustomDataCommand.py` & `testwizard.core-3.8.1b4810/testwizard/core/commands/AddCustomDataCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.core-3.8.1b4749/testwizard/core/commands/AddPerformanceDataCommand.py` & `testwizard.core-3.8.1b4810/testwizard/core/commands/AddPerformanceDataCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.core-3.8.1b4749/testwizard/core/commands/BeginStepCommand.py` & `testwizard.core-3.8.1b4810/testwizard/core/commands/BeginStepCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.core-3.8.1b4749/testwizard/core/commands/CancelCommandsCommand.py` & `testwizard.core-3.8.1b4810/testwizard/core/commands/CancelCommandsCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.core-3.8.1b4749/testwizard/core/commands/EndStepCommand.py` & `testwizard.core-3.8.1b4810/testwizard/core/commands/EndStepCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.core-3.8.1b4749/testwizard/core/commands/EndStepResult.py` & `testwizard.core-3.8.1b4810/testwizard/core/commands/EndStepResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.core-3.8.1b4749/testwizard/core/commands/StringCompareCommand.py` & `testwizard.core-3.8.1b4810/testwizard/core/commands/StringCompareCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.core-3.8.1b4749/testwizard/core/commands/StringCompareResult.py` & `testwizard.core-3.8.1b4810/testwizard/core/commands/StringCompareResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.core-3.8.1b4749/testwizard/core/commands/WaitForCommandCompletionCommand.py` & `testwizard.core-3.8.1b4810/testwizard/core/commands/WaitForCommandCompletionCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.core-3.8.1b4749/testwizard/core/models/CreateTestRunRequest.py` & `testwizard.core-3.8.1b4810/testwizard/core/models/CreateTestRunRequest.py`

 * *Files identical despite different names*

### Comparing `testwizard.core-3.8.1b4749/testwizard.core.egg-info/PKG-INFO` & `testwizard.core-3.8.1b4810/testwizard.core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.core
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard core
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.core-3.8.1b4749/testwizard.core.egg-info/SOURCES.txt` & `testwizard.core-3.8.1b4810/testwizard.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

