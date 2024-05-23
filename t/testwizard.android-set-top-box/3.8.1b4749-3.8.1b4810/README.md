# Comparing `tmp/testwizard.android-set-top-box-3.8.1b4749.tar.gz` & `tmp/testwizard.android-set-top-box-3.8.1b4810.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testwizard.android-set-top-box-3.8.1b4749.tar", last modified: Tue Mar 19 15:01:47 2024, max compression
+gzip compressed data, was "testwizard.android-set-top-box-3.8.1b4810.tar", last modified: Wed Mar 27 12:56:35 2024, max compression
```

## Comparing `testwizard.android-set-top-box-3.8.1b4749.tar` & `testwizard.android-set-top-box-3.8.1b4810.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:47.994591 testwizard.android-set-top-box-3.8.1b4749/
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.android-set-top-box-3.8.1b4749/LICENSE.txt
--rw-rw-rw-   0        0        0     2131 2024-03-19 15:01:47.994591 testwizard.android-set-top-box-3.8.1b4749/PKG-INFO
--rw-rw-rw-   0        0        0     1568 2024-03-19 15:00:53.000000 testwizard.android-set-top-box-3.8.1b4749/README.md
--rw-rw-rw-   0        0        0       42 2024-03-19 15:01:47.994591 testwizard.android-set-top-box-3.8.1b4749/setup.cfg
--rw-rw-rw-   0        0        0     1158 2024-03-19 15:01:47.000000 testwizard.android-set-top-box-3.8.1b4749/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:47.978968 testwizard.android-set-top-box-3.8.1b4749/testwizard/
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:47.994591 testwizard.android-set-top-box-3.8.1b4749/testwizard/android_set_top_box/
--rw-rw-rw-   0        0        0    19638 2024-03-19 15:00:53.000000 testwizard.android-set-top-box-3.8.1b4749/testwizard/android_set_top_box/AndroidSetTopBox.py
--rw-rw-rw-   0        0        0       46 2024-03-19 15:00:53.000000 testwizard.android-set-top-box-3.8.1b4749/testwizard/android_set_top_box/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:47.994591 testwizard.android-set-top-box-3.8.1b4749/testwizard.android_set_top_box.egg-info/
--rw-rw-rw-   0        0        0     2131 2024-03-19 15:01:47.000000 testwizard.android-set-top-box-3.8.1b4749/testwizard.android_set_top_box.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2024-03-19 15:01:47.000000 testwizard.android-set-top-box-3.8.1b4749/testwizard.android_set_top_box.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 15:01:47.000000 testwizard.android-set-top-box-3.8.1b4749/testwizard.android_set_top_box.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      273 2024-03-19 15:01:47.000000 testwizard.android-set-top-box-3.8.1b4749/testwizard.android_set_top_box.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 15:01:47.000000 testwizard.android-set-top-box-3.8.1b4749/testwizard.android_set_top_box.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:35.259601 testwizard.android-set-top-box-3.8.1b4810/
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.android-set-top-box-3.8.1b4810/LICENSE.txt
+-rw-rw-rw-   0        0        0     2131 2024-03-27 12:56:35.259601 testwizard.android-set-top-box-3.8.1b4810/PKG-INFO
+-rw-rw-rw-   0        0        0     1568 2024-03-27 12:55:37.000000 testwizard.android-set-top-box-3.8.1b4810/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-27 12:56:35.259601 testwizard.android-set-top-box-3.8.1b4810/setup.cfg
+-rw-rw-rw-   0        0        0     1158 2024-03-27 12:56:34.000000 testwizard.android-set-top-box-3.8.1b4810/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:35.243975 testwizard.android-set-top-box-3.8.1b4810/testwizard/
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:35.259601 testwizard.android-set-top-box-3.8.1b4810/testwizard/android_set_top_box/
+-rw-rw-rw-   0        0        0    19700 2024-03-27 12:55:37.000000 testwizard.android-set-top-box-3.8.1b4810/testwizard/android_set_top_box/AndroidSetTopBox.py
+-rw-rw-rw-   0        0        0       46 2024-03-27 12:55:37.000000 testwizard.android-set-top-box-3.8.1b4810/testwizard/android_set_top_box/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:35.243975 testwizard.android-set-top-box-3.8.1b4810/testwizard.android_set_top_box.egg-info/
+-rw-rw-rw-   0        0        0     2131 2024-03-27 12:56:35.000000 testwizard.android-set-top-box-3.8.1b4810/testwizard.android_set_top_box.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2024-03-27 12:56:35.000000 testwizard.android-set-top-box-3.8.1b4810/testwizard.android_set_top_box.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-27 12:56:35.000000 testwizard.android-set-top-box-3.8.1b4810/testwizard.android_set_top_box.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      273 2024-03-27 12:56:35.000000 testwizard.android-set-top-box-3.8.1b4810/testwizard.android_set_top_box.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-27 12:56:35.000000 testwizard.android-set-top-box-3.8.1b4810/testwizard.android_set_top_box.egg-info/top_level.txt
```

### Comparing `testwizard.android-set-top-box-3.8.1b4749/PKG-INFO` & `testwizard.android-set-top-box-3.8.1b4810/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.android-set-top-box
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard for Android set-top box testobjects
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.android-set-top-box-3.8.1b4749/README.md` & `testwizard.android-set-top-box-3.8.1b4810/README.md`

 * *Files identical despite different names*

### Comparing `testwizard.android-set-top-box-3.8.1b4749/setup.py` & `testwizard.android-set-top-box-3.8.1b4810/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="testwizard.android-set-top-box",
-    version="3.8.1b4749",
+    version="3.8.1b4810",
     author="Resillion",
     author_email="testwizard-support@resillion.com",
     description="Testwizard for Android set-top box testobjects",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.resillion.com/services/software-testing/testing-tools/testwizard/",
     packages=['testwizard.android_set_top_box'],
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

### Comparing `testwizard.android-set-top-box-3.8.1b4749/testwizard/android_set_top_box/AndroidSetTopBox.py` & `testwizard.android-set-top-box-3.8.1b4810/testwizard/android_set_top_box/AndroidSetTopBox.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,17 +141,17 @@
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
@@ -197,17 +197,17 @@
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

### Comparing `testwizard.android-set-top-box-3.8.1b4749/testwizard.android_set_top_box.egg-info/PKG-INFO` & `testwizard.android-set-top-box-3.8.1b4810/testwizard.android_set_top_box.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.android-set-top-box
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard for Android set-top box testobjects
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

