# Comparing `tmp/balsamic-0.2.0.tar.gz` & `tmp/balsamic-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balsamic-0.2.0.tar", last modified: Thu May 23 21:45:06 2024, max compression
+gzip compressed data, was "balsamic-0.2.1.tar", last modified: Thu May 23 21:49:46 2024, max compression
```

## Comparing `balsamic-0.2.0.tar` & `balsamic-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-23 21:45:06.529498 balsamic-0.2.0/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2204 2024-05-23 21:45:06.529498 balsamic-0.2.0/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1670 2024-05-23 21:44:14.000000 balsamic-0.2.0/README.md
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-23 21:45:06.529498 balsamic-0.2.0/balsamic/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.2.0/balsamic/__innit__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2559 2024-05-23 21:43:15.000000 balsamic-0.2.0/balsamic/__main__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2499 2024-05-23 21:39:01.000000 balsamic-0.2.0/balsamic/balsamic.py
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-23 21:45:06.529498 balsamic-0.2.0/balsamic.egg-info/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2204 2024-05-23 21:45:06.000000 balsamic-0.2.0/balsamic.egg-info/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-23 21:45:06.000000 balsamic-0.2.0/balsamic.egg-info/SOURCES.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-23 21:45:06.000000 balsamic-0.2.0/balsamic.egg-info/dependency_links.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-23 21:45:06.000000 balsamic-0.2.0/balsamic.egg-info/requires.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-23 21:45:06.000000 balsamic-0.2.0/balsamic.egg-info/top_level.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-23 21:45:06.529498 balsamic-0.2.0/setup.cfg
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1143 2024-05-23 21:40:18.000000 balsamic-0.2.0/setup.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-23 21:49:46.905228 balsamic-0.2.1/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2204 2024-05-23 21:49:46.905228 balsamic-0.2.1/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1670 2024-05-23 21:44:14.000000 balsamic-0.2.1/README.md
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-23 21:49:46.905228 balsamic-0.2.1/balsamic/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.2.1/balsamic/__innit__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2582 2024-05-23 21:48:49.000000 balsamic-0.2.1/balsamic/__main__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2499 2024-05-23 21:39:01.000000 balsamic-0.2.1/balsamic/balsamic.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-23 21:49:46.905228 balsamic-0.2.1/balsamic.egg-info/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2204 2024-05-23 21:49:46.000000 balsamic-0.2.1/balsamic.egg-info/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-23 21:49:46.000000 balsamic-0.2.1/balsamic.egg-info/SOURCES.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-23 21:49:46.000000 balsamic-0.2.1/balsamic.egg-info/dependency_links.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-23 21:49:46.000000 balsamic-0.2.1/balsamic.egg-info/requires.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-23 21:49:46.000000 balsamic-0.2.1/balsamic.egg-info/top_level.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-23 21:49:46.905228 balsamic-0.2.1/setup.cfg
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-23 21:49:24.000000 balsamic-0.2.1/setup.py
```

### Comparing `balsamic-0.2.0/PKG-INFO` & `balsamic-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.2.0
+Version: 0.2.1
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.2.0/README.md` & `balsamic-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `balsamic-0.2.0/balsamic/__main__.py` & `balsamic-0.2.1/balsamic/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import balsamic
+from balsamic import balsamic
 if __name__ == "__main__":
     # Importing argparse
     import argparse
 
     # Define the parser function
     def parser():
         
@@ -37,15 +37,15 @@
         
         # Return parsed arguments
         args = parser.parse_args()
         return args
 
     args = parser()
     if args.command:
-        updatecmd(args.command)
+        balsamic.updatecmd(args.command)
 
     # Extract custom headers from the arguments
     try:
         custom_headers = dict([header.split(":") for header in args.headers.split(";")]) if args.headers else None
     except AttributeError:
         pass
     if args.attack == "webreq":
```

### Comparing `balsamic-0.2.0/balsamic/balsamic.py` & `balsamic-0.2.1/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `balsamic-0.2.0/balsamic.egg-info/PKG-INFO` & `balsamic-0.2.1/balsamic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.2.0
+Version: 0.2.1
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.2.0/setup.py` & `balsamic-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.0'
+VERSION = '0.2.01'
 DESCRIPTION = 'Send malicious pickles via requests or sockets'
 LONG_DESCRIPTION = 'A package that allows the user to easily send out malicious pickles, via web requests, or a malicious server or client(currently ipv4 only)'
 
 # Setting up
 setup(
     name="balsamic",
     version=VERSION,
```

