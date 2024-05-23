# Comparing `tmp/sophisticate-1.0.1.tar.gz` & `tmp/sophisticate-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sophisticate-1.0.1.tar", last modified: Tue May 21 23:48:09 2024, max compression
+gzip compressed data, was "sophisticate-1.0.2.tar", last modified: Thu May 23 16:45:56 2024, max compression
```

## Comparing `sophisticate-1.0.1.tar` & `sophisticate-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-21 23:48:09.511675 sophisticate-1.0.1/
--rw-r--r--   0 khiat     (1000) khiat     (1000)     1141 2024-05-21 23:48:09.511675 sophisticate-1.0.1/PKG-INFO
--rw-rw-r--   0 khiat     (1000) khiat     (1000)      715 2024-05-21 23:24:21.000000 sophisticate-1.0.1/README.md
--rw-r--r--   0 khiat     (1000) khiat     (1000)       38 2024-05-21 23:48:09.511675 sophisticate-1.0.1/setup.cfg
--rw-rw-r--   0 khiat     (1000) khiat     (1000)      741 2024-05-21 23:46:55.000000 sophisticate-1.0.1/setup.py
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-21 23:48:09.507675 sophisticate-1.0.1/sophisticate/
--rw-r--r--   0 khiat     (1000) khiat     (1000)       60 2024-05-21 22:25:03.000000 sophisticate-1.0.1/sophisticate/__init__.py
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-21 23:48:09.511675 sophisticate-1.0.1/sophisticate.egg-info/
--rw-r--r--   0 khiat     (1000) khiat     (1000)     1141 2024-05-21 23:48:09.000000 sophisticate-1.0.1/sophisticate.egg-info/PKG-INFO
--rw-r--r--   0 khiat     (1000) khiat     (1000)      222 2024-05-21 23:48:09.000000 sophisticate-1.0.1/sophisticate.egg-info/SOURCES.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)        1 2024-05-21 23:48:09.000000 sophisticate-1.0.1/sophisticate.egg-info/dependency_links.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)       60 2024-05-21 23:48:09.000000 sophisticate-1.0.1/sophisticate.egg-info/requires.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)       13 2024-05-21 23:48:09.000000 sophisticate-1.0.1/sophisticate.egg-info/top_level.txt
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-23 16:45:56.651929 sophisticate-1.0.2/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)     1141 2024-05-23 16:45:56.651929 sophisticate-1.0.2/PKG-INFO
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)      715 2024-05-21 23:24:20.000000 sophisticate-1.0.2/README.md
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       38 2024-05-23 16:45:56.651929 sophisticate-1.0.2/setup.cfg
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)      741 2024-05-23 16:42:52.000000 sophisticate-1.0.2/setup.py
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-23 16:45:56.651929 sophisticate-1.0.2/sophisticate/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       60 2024-05-21 22:25:02.000000 sophisticate-1.0.2/sophisticate/__init__.py
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-23 16:45:56.651929 sophisticate-1.0.2/sophisticate.egg-info/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)     1141 2024-05-23 16:45:56.000000 sophisticate-1.0.2/sophisticate.egg-info/PKG-INFO
+-rw-r--r--   0 khiat     (1000) khiat     (1000)      222 2024-05-23 16:45:56.000000 sophisticate-1.0.2/sophisticate.egg-info/SOURCES.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)        1 2024-05-23 16:45:56.000000 sophisticate-1.0.2/sophisticate.egg-info/dependency_links.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       60 2024-05-23 16:45:56.000000 sophisticate-1.0.2/sophisticate.egg-info/requires.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       13 2024-05-23 16:45:56.000000 sophisticate-1.0.2/sophisticate.egg-info/top_level.txt
```

### Comparing `sophisticate-1.0.1/PKG-INFO` & `sophisticate-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sophisticate
-Version: 1.0.1
+Version: 1.0.2
 Summary: Sophisticate Libraries Collection
 Home-page: https://pypi.org/project/sophisticate/
 Author: khiat Mohammed Abderrezzak
 Author-email: khiat.abderrezzak@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `sophisticate-1.0.1/README.md` & `sophisticate-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sophisticate-1.0.1/sophisticate.egg-info/PKG-INFO` & `sophisticate-1.0.2/sophisticate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sophisticate
-Version: 1.0.1
+Version: 1.0.2
 Summary: Sophisticate Libraries Collection
 Home-page: https://pypi.org/project/sophisticate/
 Author: khiat Mohammed Abderrezzak
 Author-email: khiat.abderrezzak@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

