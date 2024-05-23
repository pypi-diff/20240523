# Comparing `tmp/ahmedhossam-0.0.3.tar.gz` & `tmp/ahmedhossam-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahmedhossam-0.0.3.tar", last modified: Thu May 23 07:05:47 2024, max compression
+gzip compressed data, was "ahmedhossam-0.0.4.tar", last modified: Thu May 23 07:32:35 2024, max compression
```

## Comparing `ahmedhossam-0.0.3.tar` & `ahmedhossam-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 ahossam   (6511) ahossam   (6500)        0 2024-05-23 07:05:47.329380 ahmedhossam-0.0.3/
-drwxrwxrwx   0 ahossam   (6511) ahossam   (6500)        0 2024-05-23 07:05:47.190230 ahmedhossam-0.0.3/AhmedHossam/
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       23 2024-05-23 07:02:12.000000 ahmedhossam-0.0.3/AhmedHossam/__init__.py
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       40 2024-05-23 06:52:01.000000 ahmedhossam-0.0.3/AhmedHossam/main.py
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       78 2024-05-22 09:52:26.000000 ahmedhossam-0.0.3/CHANGELOG.txt
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)     1051 2024-05-22 09:52:26.000000 ahmedhossam-0.0.3/LICENCE.txt
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       26 2024-05-22 09:52:26.000000 ahmedhossam-0.0.3/MANIFEST.in
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)      544 2024-05-23 07:05:47.319253 ahmedhossam-0.0.3/PKG-INFO
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       20 2024-05-22 09:52:52.000000 ahmedhossam-0.0.3/README.txt
-drwxrwxrwx   0 ahossam   (6511) ahossam   (6500)        0 2024-05-23 07:05:47.306618 ahmedhossam-0.0.3/ahmedHossam.egg-info/
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)      544 2024-05-23 07:05:46.000000 ahmedhossam-0.0.3/ahmedHossam.egg-info/PKG-INFO
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)      249 2024-05-23 07:05:47.000000 ahmedhossam-0.0.3/ahmedHossam.egg-info/SOURCES.txt
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)        1 2024-05-23 07:05:46.000000 ahmedhossam-0.0.3/ahmedHossam.egg-info/dependency_links.txt
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       12 2024-05-23 07:05:46.000000 ahmedhossam-0.0.3/ahmedHossam.egg-info/top_level.txt
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       38 2024-05-23 07:05:47.330394 ahmedhossam-0.0.3/setup.cfg
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)      633 2024-05-23 07:05:31.000000 ahmedhossam-0.0.3/setup.py
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       39 2024-05-23 07:04:49.000000 ahmedhossam-0.0.3/test.py
+drwxrwxrwx   0 ahossam   (6511) ahossam   (6500)        0 2024-05-23 07:32:35.140103 ahmedhossam-0.0.4/
+drwxrwxrwx   0 ahossam   (6511) ahossam   (6500)        0 2024-05-23 07:32:34.985148 ahmedhossam-0.0.4/AhmedHossam/
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       23 2024-05-23 07:02:12.000000 ahmedhossam-0.0.4/AhmedHossam/__init__.py
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       48 2024-05-23 07:29:23.000000 ahmedhossam-0.0.4/AhmedHossam/main.py
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       78 2024-05-22 09:52:26.000000 ahmedhossam-0.0.4/CHANGELOG.txt
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)     1051 2024-05-22 09:52:26.000000 ahmedhossam-0.0.4/LICENCE.txt
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       26 2024-05-22 09:52:26.000000 ahmedhossam-0.0.4/MANIFEST.in
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)      544 2024-05-23 07:32:35.125855 ahmedhossam-0.0.4/PKG-INFO
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       20 2024-05-22 09:52:52.000000 ahmedhossam-0.0.4/README.txt
+drwxrwxrwx   0 ahossam   (6511) ahossam   (6500)        0 2024-05-23 07:32:35.108918 ahmedhossam-0.0.4/ahmedHossam.egg-info/
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)      544 2024-05-23 07:32:34.000000 ahmedhossam-0.0.4/ahmedHossam.egg-info/PKG-INFO
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)      249 2024-05-23 07:32:34.000000 ahmedhossam-0.0.4/ahmedHossam.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)        1 2024-05-23 07:32:34.000000 ahmedhossam-0.0.4/ahmedHossam.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       12 2024-05-23 07:32:34.000000 ahmedhossam-0.0.4/ahmedHossam.egg-info/top_level.txt
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       38 2024-05-23 07:32:35.141103 ahmedhossam-0.0.4/setup.cfg
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)      633 2024-05-23 07:32:30.000000 ahmedhossam-0.0.4/setup.py
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       45 2024-05-23 07:06:49.000000 ahmedhossam-0.0.4/test.py
```

### Comparing `ahmedhossam-0.0.3/LICENCE.txt` & `ahmedhossam-0.0.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `ahmedhossam-0.0.3/PKG-INFO` & `ahmedhossam-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahmedHossam
-Version: 0.0.3
+Version: 0.0.4
 Summary: SABA7
 Home-page: 
 Author: Ahmed Hossam
 Author-email: 
 License: MIT
 Keywords: calculator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ahmedhossam-0.0.3/ahmedHossam.egg-info/PKG-INFO` & `ahmedhossam-0.0.4/ahmedHossam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahmedHossam
-Version: 0.0.3
+Version: 0.0.4
 Summary: SABA7
 Home-page: 
 Author: Ahmed Hossam
 Author-email: 
 License: MIT
 Keywords: calculator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ahmedhossam-0.0.3/setup.py` & `ahmedhossam-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='ahmedHossam',
-  version='0.0.3',
+  version='0.0.4',
   description='SABA7',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Ahmed Hossam',
   author_email='',
   license='MIT', 
   classifiers=classifiers,
```

