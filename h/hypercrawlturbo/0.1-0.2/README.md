# Comparing `tmp/hypercrawlturbo-0.1.tar.gz` & `tmp/hypercrawlturbo-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypercrawlturbo-0.1.tar", last modified: Wed May 22 12:13:03 2024, max compression
+gzip compressed data, was "hypercrawlturbo-0.2.tar", last modified: Thu May 23 13:08:32 2024, max compression
```

## Comparing `hypercrawlturbo-0.1.tar` & `hypercrawlturbo-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-05-22 12:13:03.675072 hypercrawlturbo-0.1/
--rw-r--r--   0 akhouriudit   (501) staff       (20)      486 2024-05-22 12:13:03.674933 hypercrawlturbo-0.1/PKG-INFO
--rw-r--r--   0 akhouriudit   (501) staff       (20)      197 2024-05-22 12:09:14.000000 hypercrawlturbo-0.1/README.md
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-05-22 12:13:03.673220 hypercrawlturbo-0.1/hypercrawlturbo/
--rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-05-22 12:07:57.000000 hypercrawlturbo-0.1/hypercrawlturbo/__init__.py
--rw-r--r--   0 akhouriudit   (501) staff       (20)      877 2024-05-22 12:10:07.000000 hypercrawlturbo-0.1/hypercrawlturbo/scraper.py
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-05-22 12:13:03.674668 hypercrawlturbo-0.1/hypercrawlturbo.egg-info/
--rw-r--r--   0 akhouriudit   (501) staff       (20)      486 2024-05-22 12:13:03.000000 hypercrawlturbo-0.1/hypercrawlturbo.egg-info/PKG-INFO
--rw-r--r--   0 akhouriudit   (501) staff       (20)      309 2024-05-22 12:13:03.000000 hypercrawlturbo-0.1/hypercrawlturbo.egg-info/SOURCES.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)        1 2024-05-22 12:13:03.000000 hypercrawlturbo-0.1/hypercrawlturbo.egg-info/dependency_links.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       65 2024-05-22 12:13:03.000000 hypercrawlturbo-0.1/hypercrawlturbo.egg-info/entry_points.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       24 2024-05-22 12:13:03.000000 hypercrawlturbo-0.1/hypercrawlturbo.egg-info/requires.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       16 2024-05-22 12:13:03.000000 hypercrawlturbo-0.1/hypercrawlturbo.egg-info/top_level.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       38 2024-05-22 12:13:03.675135 hypercrawlturbo-0.1/setup.cfg
--rw-r--r--   0 akhouriudit   (501) staff       (20)      636 2024-05-22 12:10:07.000000 hypercrawlturbo-0.1/setup.py
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-05-23 13:08:32.561969 hypercrawlturbo-0.2/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      486 2024-05-23 13:08:32.561813 hypercrawlturbo-0.2/PKG-INFO
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      197 2024-05-22 12:09:14.000000 hypercrawlturbo-0.2/README.md
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-05-23 13:08:32.560290 hypercrawlturbo-0.2/hypercrawlturbo/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-05-22 12:07:57.000000 hypercrawlturbo-0.2/hypercrawlturbo/__init__.py
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      877 2024-05-22 12:10:07.000000 hypercrawlturbo-0.2/hypercrawlturbo/scraper.py
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-05-23 13:08:32.561369 hypercrawlturbo-0.2/hypercrawlturbo.egg-info/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      486 2024-05-23 13:08:32.000000 hypercrawlturbo-0.2/hypercrawlturbo.egg-info/PKG-INFO
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      309 2024-05-23 13:08:32.000000 hypercrawlturbo-0.2/hypercrawlturbo.egg-info/SOURCES.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        1 2024-05-23 13:08:32.000000 hypercrawlturbo-0.2/hypercrawlturbo.egg-info/dependency_links.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       65 2024-05-23 13:08:32.000000 hypercrawlturbo-0.2/hypercrawlturbo.egg-info/entry_points.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       24 2024-05-23 13:08:32.000000 hypercrawlturbo-0.2/hypercrawlturbo.egg-info/requires.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       16 2024-05-23 13:08:32.000000 hypercrawlturbo-0.2/hypercrawlturbo.egg-info/top_level.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       38 2024-05-23 13:08:32.562024 hypercrawlturbo-0.2/setup.cfg
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      636 2024-05-23 13:07:15.000000 hypercrawlturbo-0.2/setup.py
```

### Comparing `hypercrawlturbo-0.1/hypercrawlturbo/scraper.py` & `hypercrawlturbo-0.2/hypercrawlturbo/scraper.py`

 * *Files identical despite different names*

### Comparing `hypercrawlturbo-0.1/setup.py` & `hypercrawlturbo-0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hypercrawlturbo',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     install_requires=[
         'requests',
         'beautifulsoup4',
     ],
     entry_points={
         'console_scripts': [
```

