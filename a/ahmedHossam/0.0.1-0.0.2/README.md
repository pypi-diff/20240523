# Comparing `tmp/ahmedhossam-0.0.1.tar.gz` & `tmp/ahmedhossam-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahmedhossam-0.0.1.tar", last modified: Thu May 23 06:46:46 2024, max compression
+gzip compressed data, was "ahmedhossam-0.0.2.tar", last modified: Thu May 23 06:53:02 2024, max compression
```

## Comparing `ahmedhossam-0.0.1.tar` & `ahmedhossam-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0 ahossam   (6511) ahossam   (6500)        0 2024-05-23 06:46:46.294393 ahmedhossam-0.0.1/
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       78 2024-05-22 09:52:26.000000 ahmedhossam-0.0.1/CHANGELOG.txt
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)     1051 2024-05-22 09:52:26.000000 ahmedhossam-0.0.1/LICENCE.txt
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       26 2024-05-22 09:52:26.000000 ahmedhossam-0.0.1/MANIFEST.in
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)      544 2024-05-23 06:46:46.278386 ahmedhossam-0.0.1/PKG-INFO
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       20 2024-05-22 09:52:52.000000 ahmedhossam-0.0.1/README.txt
-drwxrwxrwx   0 ahossam   (6511) ahossam   (6500)        0 2024-05-23 06:46:46.155658 ahmedhossam-0.0.1/ahmed-hossam/
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       58 2024-05-22 09:49:53.000000 ahmedhossam-0.0.1/ahmed-hossam/__init__.py
-drwxrwxrwx   0 ahossam   (6511) ahossam   (6500)        0 2024-05-23 06:46:46.270702 ahmedhossam-0.0.1/ahmedHossam.egg-info/
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)      544 2024-05-23 06:46:45.000000 ahmedhossam-0.0.1/ahmedHossam.egg-info/PKG-INFO
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)      230 2024-05-23 06:46:46.000000 ahmedhossam-0.0.1/ahmedHossam.egg-info/SOURCES.txt
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)        1 2024-05-23 06:46:45.000000 ahmedhossam-0.0.1/ahmedHossam.egg-info/dependency_links.txt
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       13 2024-05-23 06:46:45.000000 ahmedhossam-0.0.1/ahmedHossam.egg-info/top_level.txt
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       38 2024-05-23 06:46:46.295907 ahmedhossam-0.0.1/setup.cfg
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)      633 2024-05-23 06:45:55.000000 ahmedhossam-0.0.1/setup.py
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       48 2024-05-22 11:39:16.000000 ahmedhossam-0.0.1/test.py
+drwxrwxrwx   0 ahossam   (6511) ahossam   (6500)        0 2024-05-23 06:53:02.809508 ahmedhossam-0.0.2/
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       78 2024-05-22 09:52:26.000000 ahmedhossam-0.0.2/CHANGELOG.txt
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)     1051 2024-05-22 09:52:26.000000 ahmedhossam-0.0.2/LICENCE.txt
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       26 2024-05-22 09:52:26.000000 ahmedhossam-0.0.2/MANIFEST.in
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)      544 2024-05-23 06:53:02.796507 ahmedhossam-0.0.2/PKG-INFO
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       20 2024-05-22 09:52:52.000000 ahmedhossam-0.0.2/README.txt
+drwxrwxrwx   0 ahossam   (6511) ahossam   (6500)        0 2024-05-23 06:53:02.635416 ahmedhossam-0.0.2/ahmed-hossam/
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       23 2024-05-23 06:52:24.000000 ahmedhossam-0.0.2/ahmed-hossam/__init__.py
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       40 2024-05-23 06:52:01.000000 ahmedhossam-0.0.2/ahmed-hossam/main.py
+drwxrwxrwx   0 ahossam   (6511) ahossam   (6500)        0 2024-05-23 06:53:02.781620 ahmedhossam-0.0.2/ahmedHossam.egg-info/
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)      544 2024-05-23 06:53:02.000000 ahmedhossam-0.0.2/ahmedHossam.egg-info/PKG-INFO
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)      251 2024-05-23 06:53:02.000000 ahmedhossam-0.0.2/ahmedHossam.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)        1 2024-05-23 06:53:02.000000 ahmedhossam-0.0.2/ahmedHossam.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       13 2024-05-23 06:53:02.000000 ahmedhossam-0.0.2/ahmedHossam.egg-info/top_level.txt
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       38 2024-05-23 06:53:02.810507 ahmedhossam-0.0.2/setup.cfg
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)      633 2024-05-23 06:51:24.000000 ahmedhossam-0.0.2/setup.py
+-rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       17 2024-05-23 06:49:27.000000 ahmedhossam-0.0.2/test.py
```

### Comparing `ahmedhossam-0.0.1/LICENCE.txt` & `ahmedhossam-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `ahmedhossam-0.0.1/PKG-INFO` & `ahmedhossam-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahmedHossam
-Version: 0.0.1
+Version: 0.0.2
 Summary: SABA7
 Home-page: 
 Author: Ahmed Hossam
 Author-email: 
 License: MIT
 Keywords: calculator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ahmedhossam-0.0.1/ahmedHossam.egg-info/PKG-INFO` & `ahmedhossam-0.0.2/ahmedHossam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahmedHossam
-Version: 0.0.1
+Version: 0.0.2
 Summary: SABA7
 Home-page: 
 Author: Ahmed Hossam
 Author-email: 
 License: MIT
 Keywords: calculator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ahmedhossam-0.0.1/setup.py` & `ahmedhossam-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='ahmedHossam',
-  version='0.0.1',
+  version='0.0.2',
   description='SABA7',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Ahmed Hossam',
   author_email='',
   license='MIT', 
   classifiers=classifiers,
```

