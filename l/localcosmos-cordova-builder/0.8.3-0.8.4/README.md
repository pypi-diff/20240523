# Comparing `tmp/localcosmos_cordova_builder-0.8.3.tar.gz` & `tmp/localcosmos_cordova_builder-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localcosmos_cordova_builder-0.8.3.tar", last modified: Tue Dec  5 07:18:43 2023, max compression
+gzip compressed data, was "localcosmos_cordova_builder-0.8.4.tar", last modified: Thu May 23 07:32:41 2024, max compression
```

## Comparing `localcosmos_cordova_builder-0.8.3.tar` & `localcosmos_cordova_builder-0.8.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-12-05 07:18:43.184780 localcosmos_cordova_builder-0.8.3/
--rw-r--r--   0 tom       (1000) tom       (1000)     1070 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.8.3/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)       57 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.8.3/MANIFEST.in
--rw-r--r--   0 tom       (1000) tom       (1000)      916 2023-12-05 07:18:43.184780 localcosmos_cordova_builder-0.8.3/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      214 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.8.3/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-12-05 07:18:43.184780 localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/
--rw-r--r--   0 tom       (1000) tom       (1000)     9443 2023-09-20 06:56:37.000000 localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/AppImageCreator.py
--rw-r--r--   0 tom       (1000) tom       (1000)    31828 2023-09-20 07:21:39.000000 localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/CordovaAppBuilder.py
--rw-r--r--   0 tom       (1000) tom       (1000)    19819 2023-07-20 14:05:57.000000 localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/JobManager.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2102 2023-02-01 10:58:47.000000 localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/MetaAppDefinition.py
--rw-r--r--   0 tom       (1000) tom       (1000)       97 2023-01-31 12:39:35.000000 localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4601 2023-12-05 07:17:37.000000 localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/image_utils.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)      974 2022-12-08 09:26:06.000000 localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/logger.py
--rw-r--r--   0 tom       (1000) tom       (1000)      168 2023-01-31 12:38:43.000000 localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/required_assets.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-12-05 07:18:43.181446 localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/resources/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-12-05 07:18:43.184780 localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/resources/images/
--rw-r--r--   0 tom       (1000) tom       (1000)      283 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/resources/images/adaptive_launcher_background.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2154 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/resources/images/adaptive_launcher_background.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     4077 2023-04-26 15:23:50.000000 localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/resources/images/appLauncherIcon.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     2494 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/urllib_request_upload_files.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-12-05 07:18:43.184780 localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)      916 2023-12-05 07:18:43.000000 localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      927 2023-12-05 07:18:43.000000 localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-12-05 07:18:43.000000 localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       39 2023-12-05 07:18:43.000000 localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       28 2023-12-05 07:18:43.000000 localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-12-05 07:18:43.184780 localcosmos_cordova_builder-0.8.3/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)     1007 2023-12-05 07:18:26.000000 localcosmos_cordova_builder-0.8.3/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-23 07:32:41.919538 localcosmos_cordova_builder-0.8.4/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1070 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.8.4/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)       57 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.8.4/MANIFEST.in
+-rw-r--r--   0 tom       (1000) tom       (1000)      916 2024-05-23 07:32:41.919538 localcosmos_cordova_builder-0.8.4/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      214 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.8.4/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-23 07:32:41.919538 localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/
+-rw-r--r--   0 tom       (1000) tom       (1000)     9443 2023-09-20 06:56:37.000000 localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/AppImageCreator.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    31828 2024-05-22 11:53:19.000000 localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/CordovaAppBuilder.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    19819 2023-07-20 14:05:57.000000 localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/JobManager.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2102 2023-02-01 10:58:47.000000 localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/MetaAppDefinition.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       97 2023-01-31 12:39:35.000000 localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4601 2023-12-05 07:17:37.000000 localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/image_utils.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)      974 2022-12-08 09:26:06.000000 localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/logger.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      168 2023-01-31 12:38:43.000000 localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/required_assets.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-23 07:32:41.916204 localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/resources/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-23 07:32:41.919538 localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/resources/images/
+-rw-r--r--   0 tom       (1000) tom       (1000)      283 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/resources/images/adaptive_launcher_background.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2154 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/resources/images/adaptive_launcher_background.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     4077 2023-04-26 15:23:50.000000 localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/resources/images/appLauncherIcon.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     2494 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/urllib_request_upload_files.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-23 07:32:41.919538 localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)      916 2024-05-23 07:32:41.000000 localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      927 2024-05-23 07:32:41.000000 localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2024-05-23 07:32:41.000000 localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       39 2024-05-23 07:32:41.000000 localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       28 2024-05-23 07:32:41.000000 localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       38 2024-05-23 07:32:41.919538 localcosmos_cordova_builder-0.8.4/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)     1007 2024-05-23 07:32:22.000000 localcosmos_cordova_builder-0.8.4/setup.py
```

### Comparing `localcosmos_cordova_builder-0.8.3/LICENSE` & `localcosmos_cordova_builder-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.8.3/PKG-INFO` & `localcosmos_cordova_builder-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localcosmos_cordova_builder
-Version: 0.8.3
+Version: 0.8.4
 Summary: Create android and ios app packages for Local Cosmos apps.
 Home-page: https://github.com/SiSol-Systems/localcosmos-cordova-builder
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: localcosmos,app kit,cordova builder
 Platform: OS Independent
```

### Comparing `localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/AppImageCreator.py` & `localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/AppImageCreator.py`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/CordovaAppBuilder.py` & `localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/CordovaAppBuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 if not WORKDIR:
     raise ValueError('LOCALCOSMOS_CORDOVA_BUILDER_WORKDIR environment variable not found')
 
 CORDOVA_CLI_VERSION = '12.0.0'
 
 DEFAULT_CORDOVA_PLATFORM_VERSIONS = {
     "android" : "android@12.0.1",
-    "ios" : "ios@7.0.1",
+    "ios" : "ios@7.1.0",
     "browser" : "browser@7.0.0",
 }
 
 PLATFORM_IOS = 'ios'
 PLATFORM_ANDROID = 'android'
 PLATFORM_BROWSER = 'browser'
```

### Comparing `localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/JobManager.py` & `localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/JobManager.py`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/MetaAppDefinition.py` & `localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/MetaAppDefinition.py`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/image_utils.py` & `localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/image_utils.py`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/logger.py` & `localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/logger.py`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/resources/images/adaptive_launcher_background.svg` & `localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/resources/images/adaptive_launcher_background.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/resources/images/appLauncherIcon.svg` & `localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/resources/images/appLauncherIcon.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder/urllib_request_upload_files.py` & `localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder/urllib_request_upload_files.py`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder.egg-info/PKG-INFO` & `localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: localcosmos-cordova-builder
-Version: 0.8.3
+Name: localcosmos_cordova_builder
+Version: 0.8.4
 Summary: Create android and ios app packages for Local Cosmos apps.
 Home-page: https://github.com/SiSol-Systems/localcosmos-cordova-builder
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: localcosmos,app kit,cordova builder
 Platform: OS Independent
```

### Comparing `localcosmos_cordova_builder-0.8.3/localcosmos_cordova_builder.egg-info/SOURCES.txt` & `localcosmos_cordova_builder-0.8.4/localcosmos_cordova_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.8.3/setup.py` & `localcosmos_cordova_builder-0.8.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     'lxml>=4.3.4',
     'tendo',
     'Pillow',
 ]
 
 setup(
     name='localcosmos_cordova_builder',
-    version='0.8.3',
+    version='0.8.4',
     description='Create android and ios app packages for Local Cosmos apps.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='The MIT License',
     platforms=['OS Independent'],
     keywords='localcosmos, app kit, cordova builder',
     author='Thomas Uher',
```

