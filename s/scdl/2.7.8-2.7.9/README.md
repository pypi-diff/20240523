# Comparing `tmp/scdl-2.7.8.tar.gz` & `tmp/scdl-2.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/scdl/scdl/dist/.tmp-z3hlvkhp/scdl-2.7.8.tar", last modified: Mon May 20 17:31:29 2024, max compression
+gzip compressed data, was "/home/runner/work/scdl/scdl/dist/.tmp-xwp810x_/scdl-2.7.9.tar", last modified: Thu May 23 01:11:12 2024, max compression
```

## Comparing `scdl-2.7.8.tar` & `scdl-2.7.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:31:29.000000 scdl-2.7.8/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-20 17:31:13.000000 scdl-2.7.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    18027 2024-05-20 17:31:13.000000 scdl-2.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-20 17:31:13.000000 scdl-2.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-05-20 17:31:29.000000 scdl-2.7.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     4954 2024-05-20 17:31:13.000000 scdl-2.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:31:29.000000 scdl-2.7.8/scdl/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-20 17:31:13.000000 scdl-2.7.8/scdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-20 17:31:13.000000 scdl-2.7.8/scdl/scdl.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)    38901 2024-05-20 17:31:13.000000 scdl-2.7.8/scdl/scdl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-20 17:31:13.000000 scdl-2.7.8/scdl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:31:29.000000 scdl-2.7.8/scdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-05-20 17:31:29.000000 scdl-2.7.8/scdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-20 17:31:29.000000 scdl-2.7.8/scdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 17:31:29.000000 scdl-2.7.8/scdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-20 17:31:29.000000 scdl-2.7.8/scdl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-20 17:31:29.000000 scdl-2.7.8/scdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-20 17:31:29.000000 scdl-2.7.8/scdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 17:31:29.000000 scdl-2.7.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1594 2024-05-20 17:31:13.000000 scdl-2.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:11:12.000000 scdl-2.7.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-23 01:10:56.000000 scdl-2.7.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    18027 2024-05-23 01:10:56.000000 scdl-2.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 01:10:56.000000 scdl-2.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-05-23 01:11:12.000000 scdl-2.7.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4954 2024-05-23 01:10:56.000000 scdl-2.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:11:12.000000 scdl-2.7.9/scdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-23 01:10:56.000000 scdl-2.7.9/scdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-23 01:10:56.000000 scdl-2.7.9/scdl/scdl.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38901 2024-05-23 01:10:56.000000 scdl-2.7.9/scdl/scdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-23 01:10:56.000000 scdl-2.7.9/scdl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:11:12.000000 scdl-2.7.9/scdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-05-23 01:11:12.000000 scdl-2.7.9/scdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-23 01:11:12.000000 scdl-2.7.9/scdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:11:12.000000 scdl-2.7.9/scdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-23 01:11:12.000000 scdl-2.7.9/scdl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-23 01:11:12.000000 scdl-2.7.9/scdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 01:11:12.000000 scdl-2.7.9/scdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 01:11:12.000000 scdl-2.7.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1594 2024-05-23 01:10:56.000000 scdl-2.7.9/setup.py
```

### Comparing `scdl-2.7.8/LICENSE` & `scdl-2.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scdl-2.7.8/PKG-INFO` & `scdl-2.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdl
-Version: 2.7.8
+Version: 2.7.9
 Summary: Download Music from Souncloud
 Home-page: https://github.com/flyingrub/scdl
 Author: FlyinGrub
 Author-email: flyinggrub@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `scdl-2.7.8/README.md` & `scdl-2.7.9/README.md`

 * *Files identical despite different names*

### Comparing `scdl-2.7.8/scdl/scdl.cfg` & `scdl-2.7.9/scdl/scdl.cfg`

 * *Files identical despite different names*

### Comparing `scdl-2.7.8/scdl/scdl.py` & `scdl-2.7.9/scdl/scdl.py`

 * *Files identical despite different names*

### Comparing `scdl-2.7.8/scdl/utils.py` & `scdl-2.7.9/scdl/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     units = {
         'k': 1024,
         'm': 1024 ** 2,
         'g': 1024 ** 3,
         't': 1024 ** 4,
         'p': 1024 ** 5,
     }
-    match = re.search('^\s*([0-9\.]+)\s*([kmgtp])?', insize, re.I)
+    match = re.search(r'^\s*([0-9\.]+)\s*([kmgtp])?', insize, re.I)
 
     if match is None:
         raise ValueError('match not found')
 
     size, unit = match.groups()
 
     if size:
```

### Comparing `scdl-2.7.8/scdl.egg-info/PKG-INFO` & `scdl-2.7.9/scdl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdl
-Version: 2.7.8
+Version: 2.7.9
 Summary: Download Music from Souncloud
 Home-page: https://github.com/flyingrub/scdl
 Author: FlyinGrub
 Author-email: flyinggrub@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `scdl-2.7.8/setup.py` & `scdl-2.7.9/setup.py`

 * *Files identical despite different names*

