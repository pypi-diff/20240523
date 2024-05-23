# Comparing `tmp/testwizard.smart-tv-3.8.1b4749.tar.gz` & `tmp/testwizard.smart-tv-3.8.1b4810.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testwizard.smart-tv-3.8.1b4749.tar", last modified: Tue Mar 19 15:01:51 2024, max compression
+gzip compressed data, was "testwizard.smart-tv-3.8.1b4810.tar", last modified: Wed Mar 27 12:56:38 2024, max compression
```

## Comparing `testwizard.smart-tv-3.8.1b4749.tar` & `testwizard.smart-tv-3.8.1b4810.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:51.511371 testwizard.smart-tv-3.8.1b4749/
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.smart-tv-3.8.1b4749/LICENSE.txt
--rw-rw-rw-   0        0        0     1997 2024-03-19 15:01:51.511371 testwizard.smart-tv-3.8.1b4749/PKG-INFO
--rw-rw-rw-   0        0        0     1456 2024-03-19 15:00:53.000000 testwizard.smart-tv-3.8.1b4749/README.md
--rw-rw-rw-   0        0        0       42 2024-03-19 15:01:51.511371 testwizard.smart-tv-3.8.1b4749/setup.cfg
--rw-rw-rw-   0        0        0     1176 2024-03-19 15:01:51.000000 testwizard.smart-tv-3.8.1b4749/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:51.511371 testwizard.smart-tv-3.8.1b4749/testwizard/
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:51.511371 testwizard.smart-tv-3.8.1b4749/testwizard/smart_tv/
--rw-rw-rw-   0        0        0    21663 2024-03-19 15:00:53.000000 testwizard.smart-tv-3.8.1b4749/testwizard/smart_tv/SmartTv.py
--rw-rw-rw-   0        0        0       28 2024-03-19 15:00:53.000000 testwizard.smart-tv-3.8.1b4749/testwizard/smart_tv/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:51.511371 testwizard.smart-tv-3.8.1b4749/testwizard.smart_tv.egg-info/
--rw-rw-rw-   0        0        0     1997 2024-03-19 15:01:51.000000 testwizard.smart-tv-3.8.1b4749/testwizard.smart_tv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2024-03-19 15:01:51.000000 testwizard.smart-tv-3.8.1b4749/testwizard.smart_tv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 15:01:51.000000 testwizard.smart-tv-3.8.1b4749/testwizard.smart_tv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      312 2024-03-19 15:01:51.000000 testwizard.smart-tv-3.8.1b4749/testwizard.smart_tv.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 15:01:51.000000 testwizard.smart-tv-3.8.1b4749/testwizard.smart_tv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:38.682659 testwizard.smart-tv-3.8.1b4810/
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.smart-tv-3.8.1b4810/LICENSE.txt
+-rw-rw-rw-   0        0        0     1997 2024-03-27 12:56:38.682659 testwizard.smart-tv-3.8.1b4810/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2024-03-27 12:55:37.000000 testwizard.smart-tv-3.8.1b4810/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-27 12:56:38.682659 testwizard.smart-tv-3.8.1b4810/setup.cfg
+-rw-rw-rw-   0        0        0     1176 2024-03-27 12:56:38.000000 testwizard.smart-tv-3.8.1b4810/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:38.682659 testwizard.smart-tv-3.8.1b4810/testwizard/
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:38.682659 testwizard.smart-tv-3.8.1b4810/testwizard/smart_tv/
+-rw-rw-rw-   0        0        0    21725 2024-03-27 12:55:37.000000 testwizard.smart-tv-3.8.1b4810/testwizard/smart_tv/SmartTv.py
+-rw-rw-rw-   0        0        0       28 2024-03-27 12:55:37.000000 testwizard.smart-tv-3.8.1b4810/testwizard/smart_tv/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:38.682659 testwizard.smart-tv-3.8.1b4810/testwizard.smart_tv.egg-info/
+-rw-rw-rw-   0        0        0     1997 2024-03-27 12:56:38.000000 testwizard.smart-tv-3.8.1b4810/testwizard.smart_tv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2024-03-27 12:56:38.000000 testwizard.smart-tv-3.8.1b4810/testwizard.smart_tv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-27 12:56:38.000000 testwizard.smart-tv-3.8.1b4810/testwizard.smart_tv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      312 2024-03-27 12:56:38.000000 testwizard.smart-tv-3.8.1b4810/testwizard.smart_tv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-27 12:56:38.000000 testwizard.smart-tv-3.8.1b4810/testwizard.smart_tv.egg-info/top_level.txt
```

### Comparing `testwizard.smart-tv-3.8.1b4749/PKG-INFO` & `testwizard.smart-tv-3.8.1b4810/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.smart-tv
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard for Smart TV testobjects
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.smart-tv-3.8.1b4749/README.md` & `testwizard.smart-tv-3.8.1b4810/README.md`

 * *Files identical despite different names*

### Comparing `testwizard.smart-tv-3.8.1b4749/setup.py` & `testwizard.smart-tv-3.8.1b4810/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="testwizard.smart-tv",
-    version="3.8.1b4749",
+    version="3.8.1b4810",
     author="Resillion",
     author_email="testwizard-support@resillion.com",
     description="Testwizard for Smart TV testobjects",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.resillion.com/services/software-testing/testing-tools/testwizard/",
     packages=['testwizard.smart_tv'],
     install_requires=[
-        'testwizard.test==3.8.1b4749',
-        'testwizard.testobjects-core==3.8.1b4749',
-        'testwizard.commands-audio==3.8.1b4749',
-        'testwizard.commands-mobile==3.8.1b4749',
-        'testwizard.commands-powerswitch==3.8.1b4749',
-        'testwizard.commands-remotecontrol==3.8.1b4749',
-        'testwizard.commands-video==3.8.1b4749',
-        'testwizard.commands-camera==3.8.1b4749'
+        'testwizard.test==3.8.1b4810',
+        'testwizard.testobjects-core==3.8.1b4810',
+        'testwizard.commands-audio==3.8.1b4810',
+        'testwizard.commands-mobile==3.8.1b4810',
+        'testwizard.commands-powerswitch==3.8.1b4810',
+        'testwizard.commands-remotecontrol==3.8.1b4810',
+        'testwizard.commands-video==3.8.1b4810',
+        'testwizard.commands-camera==3.8.1b4810'
     ],
     classifiers=[
         "Programming Language :: Python :: 3.3",
         "Development Status :: 5 - Production/Stable",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `testwizard.smart-tv-3.8.1b4749/testwizard/smart_tv/SmartTv.py` & `testwizard.smart-tv-3.8.1b4810/testwizard/smart_tv/SmartTv.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,17 +179,17 @@
         self.throwIfDisposed()
         return InitDriverCommand(self).execute(appPath)
     
     def quitDriver(self):
         self.throwIfDisposed()
         return QuitDriverCommand(self).execute()
 
-    def closeApp(self):
+    def closeApp(self, appId):
         self.throwIfDisposed()
-        return CloseAppCommand(self).execute()
+        return CloseAppCommand(self).execute(appId)
     
     def addCapability(self, name, value):
         self.throwIfDisposed()
         return AddCapabilityCommand(self).execute(name, value)
     
     def android_SendKeyCode(self, keyCode):
         self.throwIfDisposed()
@@ -235,17 +235,17 @@
         self.throwIfDisposed()
         return HideKeyboardCommand(self).execute(iOS_Key)
     
     def inputText(self, selector, text):
         self.throwIfDisposed()
         return InputTextCommand(self).execute(selector, text)
     
-    def launchApp(self):
+    def launchApp(self, appId = None, activityId = None):
         self.throwIfDisposed()
-        return LaunchAppCommand(self).execute()
+        return LaunchAppCommand(self).execute(appId, activityId)
     
     def multiTouch_Add(self):
         self.throwIfDisposed()
         return MultiTouch_AddCommand(self).execute()   
     
     def multiTouch_New(self):
         self.throwIfDisposed()
```

### Comparing `testwizard.smart-tv-3.8.1b4749/testwizard.smart_tv.egg-info/PKG-INFO` & `testwizard.smart-tv-3.8.1b4810/testwizard.smart_tv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.smart-tv
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard for Smart TV testobjects
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

