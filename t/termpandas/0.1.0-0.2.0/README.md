# Comparing `tmp/termpandas-0.1.0.tar.gz` & `tmp/termpandas-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termpandas-0.1.0.tar", last modified: Sun Apr 14 23:17:49 2024, max compression
+gzip compressed data, was "termpandas-0.2.0.tar", last modified: Wed May 22 22:35:30 2024, max compression
```

## Comparing `termpandas-0.1.0.tar` & `termpandas-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxr-x   0 juanesh   (1000) juanesh   (1000)        0 2024-04-14 23:17:49.118673 termpandas-0.1.0/
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)      100 2024-04-14 23:16:45.000000 termpandas-0.1.0/CHANGELOG.txt
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)     1076 2024-04-11 15:26:31.000000 termpandas-0.1.0/LICENSE
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)       75 2024-04-11 16:34:42.000000 termpandas-0.1.0/MANIFEST.in
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)     1453 2024-04-14 23:17:49.118673 termpandas-0.1.0/PKG-INFO
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)      679 2024-04-14 23:12:39.000000 termpandas-0.1.0/README.md
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)       38 2024-04-14 23:17:49.118673 termpandas-0.1.0/setup.cfg
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)     1138 2024-04-14 23:16:31.000000 termpandas-0.1.0/setup.py
-drwxrwxr-x   0 juanesh   (1000) juanesh   (1000)        0 2024-04-14 23:17:49.114673 termpandas-0.1.0/termpandas/
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)       31 2024-04-11 15:57:50.000000 termpandas-0.1.0/termpandas/__init__.py
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)     6032 2024-04-14 17:19:41.000000 termpandas-0.1.0/termpandas/scrollable.py
-drwxrwxr-x   0 juanesh   (1000) juanesh   (1000)        0 2024-04-14 23:17:49.118673 termpandas-0.1.0/termpandas.egg-info/
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)     1453 2024-04-14 23:17:48.000000 termpandas-0.1.0/termpandas.egg-info/PKG-INFO
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)      269 2024-04-14 23:17:49.000000 termpandas-0.1.0/termpandas.egg-info/SOURCES.txt
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)        1 2024-04-14 23:17:48.000000 termpandas-0.1.0/termpandas.egg-info/dependency_links.txt
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)       45 2024-04-14 23:17:48.000000 termpandas-0.1.0/termpandas.egg-info/requires.txt
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)       11 2024-04-14 23:17:48.000000 termpandas-0.1.0/termpandas.egg-info/top_level.txt
+drwxr-xr-x   0 juanesh   (1000) juanesh   (1000)        0 2024-05-22 22:35:30.372501 termpandas-0.2.0/
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)      312 2024-05-22 22:10:51.000000 termpandas-0.2.0/CHANGELOG.txt
+-rw-rw-r--   0 juanesh   (1000) juanesh   (1000)     1076 2024-04-11 15:26:31.000000 termpandas-0.2.0/LICENSE
+-rw-rw-r--   0 juanesh   (1000) juanesh   (1000)       75 2024-04-11 16:34:42.000000 termpandas-0.2.0/MANIFEST.in
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)     2241 2024-05-22 22:35:30.372501 termpandas-0.2.0/PKG-INFO
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)     1414 2024-05-22 22:10:51.000000 termpandas-0.2.0/README.md
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)       38 2024-05-22 22:35:30.372501 termpandas-0.2.0/setup.cfg
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)     1138 2024-05-22 22:10:51.000000 termpandas-0.2.0/setup.py
+drwxr-xr-x   0 juanesh   (1000) juanesh   (1000)        0 2024-05-22 22:35:30.369168 termpandas-0.2.0/termpandas/
+-rw-rw-r--   0 juanesh   (1000) juanesh   (1000)       31 2024-04-11 15:57:50.000000 termpandas-0.2.0/termpandas/__init__.py
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)    16509 2024-05-22 22:10:51.000000 termpandas-0.2.0/termpandas/scrollable.py
+drwxr-xr-x   0 juanesh   (1000) juanesh   (1000)        0 2024-05-22 22:35:30.369168 termpandas-0.2.0/termpandas.egg-info/
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)     2241 2024-05-22 22:35:30.000000 termpandas-0.2.0/termpandas.egg-info/PKG-INFO
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)      284 2024-05-22 22:35:30.000000 termpandas-0.2.0/termpandas.egg-info/SOURCES.txt
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)        1 2024-05-22 22:35:30.000000 termpandas-0.2.0/termpandas.egg-info/dependency_links.txt
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)       45 2024-05-22 22:35:30.000000 termpandas-0.2.0/termpandas.egg-info/requires.txt
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)       11 2024-05-22 22:35:30.000000 termpandas-0.2.0/termpandas.egg-info/top_level.txt
+drwxr-xr-x   0 juanesh   (1000) juanesh   (1000)        0 2024-05-22 22:35:30.369168 termpandas-0.2.0/tests/
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)     3048 2024-05-22 22:10:51.000000 termpandas-0.2.0/tests/tests.py
```

### Comparing `termpandas-0.1.0/LICENSE` & `termpandas-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `termpandas-0.1.0/setup.py` & `termpandas-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Load the README file and use it as the long_description.
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='termpandas',
-    version='0.1.0',
+    version='0.2.0',
     url='https://github.com/juan-esteban-berger/termpandas',
     author='Juan Esteban Berger',
     author_email='juanestebanberger@gmail.com',
     description='Scrollable pandas dataframes in the terminal.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

