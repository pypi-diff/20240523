# Comparing `tmp/testwizard.mobile-3.8.1b4749.tar.gz` & `tmp/testwizard.mobile-3.8.1b4810.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testwizard.mobile-3.8.1b4749.tar", last modified: Tue Mar 19 15:01:48 2024, max compression
+gzip compressed data, was "testwizard.mobile-3.8.1b4810.tar", last modified: Wed Mar 27 12:56:36 2024, max compression
```

## Comparing `testwizard.mobile-3.8.1b4749.tar` & `testwizard.mobile-3.8.1b4810.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:48.854297 testwizard.mobile-3.8.1b4749/
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.mobile-3.8.1b4749/LICENSE.txt
--rw-rw-rw-   0        0        0     2164 2024-03-19 15:01:48.854297 testwizard.mobile-3.8.1b4749/PKG-INFO
--rw-rw-rw-   0        0        0     1627 2024-03-19 15:00:53.000000 testwizard.mobile-3.8.1b4749/README.md
--rw-rw-rw-   0        0        0       42 2024-03-19 15:01:48.854297 testwizard.mobile-3.8.1b4749/setup.cfg
--rw-rw-rw-   0        0        0     1005 2024-03-19 15:01:48.000000 testwizard.mobile-3.8.1b4749/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:48.854297 testwizard.mobile-3.8.1b4749/testwizard/
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:48.854297 testwizard.mobile-3.8.1b4749/testwizard/mobile/
--rw-rw-rw-   0        0        0    19929 2024-03-19 15:00:53.000000 testwizard.mobile-3.8.1b4749/testwizard/mobile/Mobile.py
--rw-rw-rw-   0        0        0       26 2024-03-19 15:00:53.000000 testwizard.mobile-3.8.1b4749/testwizard/mobile/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:48.854297 testwizard.mobile-3.8.1b4749/testwizard.mobile.egg-info/
--rw-rw-rw-   0        0        0     2164 2024-03-19 15:01:48.000000 testwizard.mobile-3.8.1b4749/testwizard.mobile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-03-19 15:01:48.000000 testwizard.mobile-3.8.1b4749/testwizard.mobile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 15:01:48.000000 testwizard.mobile-3.8.1b4749/testwizard.mobile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      183 2024-03-19 15:01:48.000000 testwizard.mobile-3.8.1b4749/testwizard.mobile.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 15:01:48.000000 testwizard.mobile-3.8.1b4749/testwizard.mobile.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:36.134828 testwizard.mobile-3.8.1b4810/
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.mobile-3.8.1b4810/LICENSE.txt
+-rw-rw-rw-   0        0        0     2164 2024-03-27 12:56:36.134828 testwizard.mobile-3.8.1b4810/PKG-INFO
+-rw-rw-rw-   0        0        0     1627 2024-03-27 12:55:37.000000 testwizard.mobile-3.8.1b4810/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-27 12:56:36.134828 testwizard.mobile-3.8.1b4810/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2024-03-27 12:56:35.000000 testwizard.mobile-3.8.1b4810/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:36.134828 testwizard.mobile-3.8.1b4810/testwizard/
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:36.134828 testwizard.mobile-3.8.1b4810/testwizard/mobile/
+-rw-rw-rw-   0        0        0    19917 2024-03-27 12:55:37.000000 testwizard.mobile-3.8.1b4810/testwizard/mobile/Mobile.py
+-rw-rw-rw-   0        0        0       26 2024-03-27 12:55:37.000000 testwizard.mobile-3.8.1b4810/testwizard/mobile/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:36.134828 testwizard.mobile-3.8.1b4810/testwizard.mobile.egg-info/
+-rw-rw-rw-   0        0        0     2164 2024-03-27 12:56:36.000000 testwizard.mobile-3.8.1b4810/testwizard.mobile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-03-27 12:56:36.000000 testwizard.mobile-3.8.1b4810/testwizard.mobile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-27 12:56:36.000000 testwizard.mobile-3.8.1b4810/testwizard.mobile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      183 2024-03-27 12:56:36.000000 testwizard.mobile-3.8.1b4810/testwizard.mobile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-27 12:56:36.000000 testwizard.mobile-3.8.1b4810/testwizard.mobile.egg-info/top_level.txt
```

### Comparing `testwizard.mobile-3.8.1b4749/PKG-INFO` & `testwizard.mobile-3.8.1b4810/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.mobile
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard for Mobile testobjects
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.mobile-3.8.1b4749/README.md` & `testwizard.mobile-3.8.1b4810/README.md`

 * *Files identical despite different names*

### Comparing `testwizard.mobile-3.8.1b4749/setup.py` & `testwizard.mobile-3.8.1b4810/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="testwizard.mobile",
-    version="3.8.1b4749",
+    version="3.8.1b4810",
     author="Resillion",
     author_email="testwizard-support@resillion.com",
     description="Testwizard for Mobile testobjects",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.resillion.com/services/software-testing/testing-tools/testwizard/",
     packages=['testwizard.mobile'],
     install_requires=[
-        'testwizard.test==3.8.1b4749',
-        'testwizard.testobjects-core==3.8.1b4749',
-        'testwizard.commands-audio==3.8.1b4749',
-        'testwizard.commands-mobile==3.8.1b4749',
-        'testwizard.commands-video==3.8.1b4749'
+        'testwizard.test==3.8.1b4810',
+        'testwizard.testobjects-core==3.8.1b4810',
+        'testwizard.commands-audio==3.8.1b4810',
+        'testwizard.commands-mobile==3.8.1b4810',
+        'testwizard.commands-video==3.8.1b4810'
     ],
     classifiers=[
         "Programming Language :: Python :: 3.3",
         "Development Status :: 5 - Production/Stable",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `testwizard.mobile-3.8.1b4749/testwizard/mobile/Mobile.py` & `testwizard.mobile-3.8.1b4810/testwizard/mobile/Mobile.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,17 +110,17 @@
         self.throwIfDisposed()
         return QuitDriverCommand(self).execute()
     
     def activateApp(self, bundleId = None):
         self.throwIfDisposed()
         return ActivateAppCommand(self).execute(bundleId)
     
-    def closeApp(self, bundleId):
+    def closeApp(self, appId):
         self.throwIfDisposed()
-        return CloseAppCommand(self).execute(bundleId)    
+        return CloseAppCommand(self).execute(appId)
     
     def addCapability(self, name, value):
         self.throwIfDisposed()
         return AddCapabilityCommand(self).execute(name, value)
     
     def android_SendKeyCode(self, keyCode):
         self.throwIfDisposed()
@@ -190,17 +190,17 @@
         self.throwIfDisposed()
         return InstallAppCommand(self).execute(ipaPath)
     
     def isAppInstalled(self, bundleId = None):
         self.throwIfDisposed()
         return IsAppInstalledCommand(self).execute(bundleId)
     
-    def launchApp(self, bundleId = None):
+    def launchApp(self, appId = None, activityId = None):
         self.throwIfDisposed()
-        return LaunchAppCommand(self).execute(bundleId)
+        return LaunchAppCommand(self).execute(appId, activityId)
     
     def multiTouch_Add(self):
         self.throwIfDisposed()
         return MultiTouch_AddCommand(self).execute()   
     
     def multiTouch_New(self):
         self.throwIfDisposed()
@@ -218,17 +218,17 @@
         self.throwIfDisposed()
         return PinchElementCommand(self).execute(selector)
     
     def queryAppState(self, bundleId = None):
         self.throwIfDisposed()
         return QueryAppStateCommand(self).execute(bundleId)
 
-    def resetApp(self, bundleId = None):
+    def resetApp(self):
         self.throwIfDisposed()
-        return ResetAppCommand(self, bundleId).execute()
+        return ResetAppCommand(self).execute()
 
     def removeApp(self, appId):
         self.throwIfDisposed()
         return RemoveAppCommand(self).execute(appId)          
     
     def runAppInBackground(self, seconds = None):
         self.throwIfDisposed()
```

### Comparing `testwizard.mobile-3.8.1b4749/testwizard.mobile.egg-info/PKG-INFO` & `testwizard.mobile-3.8.1b4810/testwizard.mobile.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.mobile
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard for Mobile testobjects
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

