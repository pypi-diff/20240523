# Comparing `tmp/metamath_py-0.0.5.tar.gz` & `tmp/metamath_py-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metamath_py-0.0.5.tar", last modified: Thu Apr 25 03:47:16 2024, max compression
+gzip compressed data, was "metamath_py-0.0.6.tar", last modified: Wed May 22 22:19:35 2024, max compression
```

## Comparing `metamath_py-0.0.5.tar` & `metamath_py-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-04-25 03:47:16.063389 metamath_py-0.0.5/
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     1088 2023-09-27 00:57:53.000000 metamath_py-0.0.5/LICENSE
--rw-r--r--   0 lightop   (1000) lightop   (1000)     5145 2024-04-25 03:47:16.063389 metamath_py-0.0.5/PKG-INFO
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     4633 2024-04-25 03:46:23.000000 metamath_py-0.0.5/README.md
--rw-rw-r--   0 lightop   (1000) lightop   (1000)      585 2024-04-25 03:47:03.000000 metamath_py-0.0.5/pyproject.toml
--rw-rw-r--   0 lightop   (1000) lightop   (1000)       38 2024-04-25 03:47:16.063389 metamath_py-0.0.5/setup.cfg
-drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-04-25 03:47:16.059389 metamath_py-0.0.5/src/
-drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-04-25 03:47:16.063389 metamath_py-0.0.5/src/metamath_py.egg-info/
--rw-r--r--   0 lightop   (1000) lightop   (1000)     5145 2024-04-25 03:47:16.000000 metamath_py-0.0.5/src/metamath_py.egg-info/PKG-INFO
--rw-rw-r--   0 lightop   (1000) lightop   (1000)      474 2024-04-25 03:47:16.000000 metamath_py-0.0.5/src/metamath_py.egg-info/SOURCES.txt
--rw-rw-r--   0 lightop   (1000) lightop   (1000)        1 2024-04-25 03:47:16.000000 metamath_py-0.0.5/src/metamath_py.egg-info/dependency_links.txt
--rw-rw-r--   0 lightop   (1000) lightop   (1000)       11 2024-04-25 03:47:16.000000 metamath_py-0.0.5/src/metamath_py.egg-info/top_level.txt
-drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-04-25 03:47:16.063389 metamath_py-0.0.5/src/metamathpy/
--rw-rw-r--   0 lightop   (1000) lightop   (1000)        1 2024-01-31 23:13:41.000000 metamath_py-0.0.5/src/metamathpy/__init__.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     6844 2024-03-24 20:58:34.000000 metamath_py-0.0.5/src/metamathpy/database.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     2940 2024-04-25 03:45:07.000000 metamath_py-0.0.5/src/metamathpy/environment.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     2521 2024-01-31 23:13:41.000000 metamath_py-0.0.5/src/metamathpy/obvious.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     7411 2024-01-31 23:13:41.000000 metamath_py-0.0.5/src/metamathpy/parse.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)    12437 2024-03-23 12:20:50.000000 metamath_py-0.0.5/src/metamathpy/proof.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     1012 2024-01-31 23:13:41.000000 metamath_py-0.0.5/src/metamathpy/scratch.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     6352 2024-01-31 23:13:41.000000 metamath_py-0.0.5/src/metamathpy/theory.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)      911 2024-01-31 23:24:22.000000 metamath_py-0.0.5/src/metamathpy/training_data.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     1513 2024-03-23 12:20:50.000000 metamath_py-0.0.5/src/metamathpy/unification.py
-drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-04-25 03:47:16.063389 metamath_py-0.0.5/tests/
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     3097 2023-09-27 01:27:35.000000 metamath_py-0.0.5/tests/tests.py
+drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-05-22 22:19:35.663277 metamath_py-0.0.6/
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     1088 2023-09-27 00:57:53.000000 metamath_py-0.0.6/LICENSE
+-rw-r--r--   0 lightop   (1000) lightop   (1000)     5145 2024-05-22 22:19:35.663277 metamath_py-0.0.6/PKG-INFO
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     4633 2024-04-25 03:46:23.000000 metamath_py-0.0.6/README.md
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)      585 2024-05-22 22:19:22.000000 metamath_py-0.0.6/pyproject.toml
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)       38 2024-05-22 22:19:35.663277 metamath_py-0.0.6/setup.cfg
+drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-05-22 22:19:35.655277 metamath_py-0.0.6/src/
+drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-05-22 22:19:35.663277 metamath_py-0.0.6/src/metamath_py.egg-info/
+-rw-r--r--   0 lightop   (1000) lightop   (1000)     5145 2024-05-22 22:19:35.000000 metamath_py-0.0.6/src/metamath_py.egg-info/PKG-INFO
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)      474 2024-05-22 22:19:35.000000 metamath_py-0.0.6/src/metamath_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)        1 2024-05-22 22:19:35.000000 metamath_py-0.0.6/src/metamath_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)       11 2024-05-22 22:19:35.000000 metamath_py-0.0.6/src/metamath_py.egg-info/top_level.txt
+drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-05-22 22:19:35.663277 metamath_py-0.0.6/src/metamathpy/
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)        1 2024-01-31 23:13:41.000000 metamath_py-0.0.6/src/metamathpy/__init__.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     6927 2024-05-22 21:54:40.000000 metamath_py-0.0.6/src/metamathpy/database.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     2940 2024-04-25 03:45:07.000000 metamath_py-0.0.6/src/metamathpy/environment.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     2521 2024-01-31 23:13:41.000000 metamath_py-0.0.6/src/metamathpy/obvious.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     7411 2024-01-31 23:13:41.000000 metamath_py-0.0.6/src/metamathpy/parse.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)    12437 2024-03-23 12:20:50.000000 metamath_py-0.0.6/src/metamathpy/proof.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     1012 2024-01-31 23:13:41.000000 metamath_py-0.0.6/src/metamathpy/scratch.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     6352 2024-01-31 23:13:41.000000 metamath_py-0.0.6/src/metamathpy/theory.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)      911 2024-01-31 23:24:22.000000 metamath_py-0.0.6/src/metamathpy/training_data.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     1513 2024-03-23 12:20:50.000000 metamath_py-0.0.6/src/metamathpy/unification.py
+drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-05-22 22:19:35.663277 metamath_py-0.0.6/tests/
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     3097 2023-09-27 01:27:35.000000 metamath_py-0.0.6/tests/tests.py
```

### Comparing `metamath_py-0.0.5/LICENSE` & `metamath_py-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `metamath_py-0.0.5/PKG-INFO` & `metamath_py-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamath-py
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python interface to Metamath
 Author-email: "Garrett E. Katz" <garrett.katz@gmail.com>
 Project-URL: Homepage, https://github.com/garrettkatz/mmpy
 Project-URL: Bug Tracker, https://github.com/garrettkatz/mmpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `metamath_py-0.0.5/README.md` & `metamath_py-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `metamath_py-0.0.5/pyproject.toml` & `metamath_py-0.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metamath-py"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Garrett E. Katz", email="garrett.katz@gmail.com" },
 ]
 description = "A Python interface to Metamath"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `metamath_py-0.0.5/src/metamath_py.egg-info/PKG-INFO` & `metamath_py-0.0.6/src/metamath_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamath-py
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python interface to Metamath
 Author-email: "Garrett E. Katz" <garrett.katz@gmail.com>
 Project-URL: Homepage, https://github.com/garrettkatz/mmpy
 Project-URL: Bug Tracker, https://github.com/garrettkatz/mmpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `metamath_py-0.0.5/src/metamathpy/database.py` & `metamath_py-0.0.6/src/metamathpy/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         if start < 0: start = len(self.rules) + start
         if stop <= 0: stop = len(self.rules) + stop
         for r, rule in enumerate(self.rules.values()):
             if not (start <= r < stop): continue
             print(rule)
 
 @profile
-def parse(fpath):
+def parse(fpath, max_rules=-1):
 
     db = Database()
 
     # parser state
     in_comment = False # whether currently in comment
     current_tag = None # most recent tag (excluding comments)
     label = None # most recent label
@@ -71,14 +71,16 @@
     frames = [new_frame()] # stack of frames in current scope
 
     # dbg = False
 
     with open(fpath, "r") as f:
         for n, line in enumerate(f):
 
+            if len(db.rules) == max_rules: break
+
             for token in line.strip().split():
 
                 # if label == "df-alsc": dbg = True
                 # if dbg:
                 #     db.print(start=-2)
                 #     print(f"token='{token}', label='{label}', tag='{current_tag}'")
                 #     print(statement)
@@ -174,19 +176,19 @@
 
     import os
 
     fpath = os.path.join(os.environ["HOME"], "metamath", "set.mm")
     # fpath = 'badparse.mm'
     # fpath = "p2.mm"
 
-    db = parse(fpath)
+    db = parse(fpath, max_rules=100)
 
     db.print(start=-6, stop=0)
-    # db.print()
-    print(f"{len(db.statements)} statements total, {len(db.rules)} rules total")
+    # # db.print()
+    # print(f"{len(db.statements)} statements total, {len(db.rules)} rules total")
 
     # for (label, stmt) in db.statements.items():
     #     print(label, stmt)
     
     # print(db.rules['df-alsc'])
     # print(db.rules['alsconv'])
```

### Comparing `metamath_py-0.0.5/src/metamathpy/environment.py` & `metamath_py-0.0.6/src/metamathpy/environment.py`

 * *Files identical despite different names*

### Comparing `metamath_py-0.0.5/src/metamathpy/obvious.py` & `metamath_py-0.0.6/src/metamathpy/obvious.py`

 * *Files identical despite different names*

### Comparing `metamath_py-0.0.5/src/metamathpy/parse.py` & `metamath_py-0.0.6/src/metamathpy/parse.py`

 * *Files identical despite different names*

### Comparing `metamath_py-0.0.5/src/metamathpy/proof.py` & `metamath_py-0.0.6/src/metamathpy/proof.py`

 * *Files identical despite different names*

### Comparing `metamath_py-0.0.5/src/metamathpy/scratch.py` & `metamath_py-0.0.6/src/metamathpy/scratch.py`

 * *Files identical despite different names*

### Comparing `metamath_py-0.0.5/src/metamathpy/theory.py` & `metamath_py-0.0.6/src/metamathpy/theory.py`

 * *Files identical despite different names*

### Comparing `metamath_py-0.0.5/src/metamathpy/training_data.py` & `metamath_py-0.0.6/src/metamathpy/training_data.py`

 * *Files identical despite different names*

### Comparing `metamath_py-0.0.5/src/metamathpy/unification.py` & `metamath_py-0.0.6/src/metamathpy/unification.py`

 * *Files identical despite different names*

### Comparing `metamath_py-0.0.5/tests/tests.py` & `metamath_py-0.0.6/tests/tests.py`

 * *Files identical despite different names*

