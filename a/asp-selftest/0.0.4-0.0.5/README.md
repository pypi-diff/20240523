# Comparing `tmp/asp_selftest-0.0.4.tar.gz` & `tmp/asp_selftest-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asp_selftest-0.0.4.tar", last modified: Tue Apr 30 09:05:05 2024, max compression
+gzip compressed data, was "asp_selftest-0.0.5.tar", last modified: Thu May 23 14:13:09 2024, max compression
```

## Comparing `asp_selftest-0.0.4.tar` & `asp_selftest-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-04-30 09:05:05.672224 asp_selftest-0.0.4/
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)    35149 2024-02-19 08:25:44.000000 asp_selftest-0.0.4/LICENSE
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)       20 2024-04-25 13:29:32.000000 asp_selftest-0.0.4/MANIFEST.in
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)     3490 2024-04-30 09:05:05.671990 asp_selftest-0.0.4/PKG-INFO
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)     2878 2024-04-25 15:02:28.000000 asp_selftest-0.0.4/README.md
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)      789 2024-04-30 09:04:12.000000 asp_selftest-0.0.4/pyproject.toml
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)       38 2024-04-30 09:05:05.672269 asp_selftest-0.0.4/setup.cfg
-drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-04-30 09:05:05.668925 asp_selftest-0.0.4/src/
-drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-04-30 09:05:05.670887 asp_selftest-0.0.4/src/asp_selftest/
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)      703 2024-04-29 07:57:48.000000 asp_selftest-0.0.4/src/asp_selftest/__init__.py
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)      526 2024-03-01 15:10:30.000000 asp_selftest-0.0.4/src/asp_selftest/example.lp
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)     1277 2024-02-19 15:49:37.000000 asp_selftest-0.0.4/src/asp_selftest/queens.lp
--rwxr-xr-x   0 erikgroeneveld   (501) staff       (20)     4990 2024-04-29 08:01:23.000000 asp_selftest-0.0.4/src/asp_selftest/runasptests.py
-drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-04-30 09:05:05.671774 asp_selftest-0.0.4/src/asp_selftest.egg-info/
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)     3490 2024-04-30 09:05:05.000000 asp_selftest-0.0.4/src/asp_selftest.egg-info/PKG-INFO
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)      363 2024-04-30 09:05:05.000000 asp_selftest-0.0.4/src/asp_selftest.egg-info/SOURCES.txt
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)        1 2024-04-30 09:05:05.000000 asp_selftest-0.0.4/src/asp_selftest.egg-info/dependency_links.txt
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)       55 2024-04-30 09:05:05.000000 asp_selftest-0.0.4/src/asp_selftest.egg-info/entry_points.txt
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)       13 2024-04-30 09:05:05.000000 asp_selftest-0.0.4/src/asp_selftest.egg-info/top_level.txt
+drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-05-23 14:13:09.524746 asp_selftest-0.0.5/
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)    35149 2024-02-19 08:25:44.000000 asp_selftest-0.0.5/LICENSE
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)       20 2024-04-25 13:29:32.000000 asp_selftest-0.0.5/MANIFEST.in
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)     3490 2024-05-23 14:13:09.524549 asp_selftest-0.0.5/PKG-INFO
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)     2878 2024-04-25 15:02:28.000000 asp_selftest-0.0.5/README.md
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)      789 2024-05-23 14:12:30.000000 asp_selftest-0.0.5/pyproject.toml
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)       38 2024-05-23 14:13:09.524788 asp_selftest-0.0.5/setup.cfg
+drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-05-23 14:13:09.522519 asp_selftest-0.0.5/src/
+drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-05-23 14:13:09.523523 asp_selftest-0.0.5/src/asp_selftest/
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)      727 2024-05-08 16:37:36.000000 asp_selftest-0.0.5/src/asp_selftest/__init__.py
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)      526 2024-03-01 15:10:30.000000 asp_selftest-0.0.5/src/asp_selftest/example.lp
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)     1277 2024-02-19 15:49:37.000000 asp_selftest-0.0.5/src/asp_selftest/queens.lp
+-rwxr-xr-x   0 erikgroeneveld   (501) staff       (20)     9313 2024-05-09 17:21:55.000000 asp_selftest-0.0.5/src/asp_selftest/runasptests.py
+drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-05-23 14:13:09.524338 asp_selftest-0.0.5/src/asp_selftest.egg-info/
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)     3490 2024-05-23 14:13:09.000000 asp_selftest-0.0.5/src/asp_selftest.egg-info/PKG-INFO
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)      363 2024-05-23 14:13:09.000000 asp_selftest-0.0.5/src/asp_selftest.egg-info/SOURCES.txt
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)        1 2024-05-23 14:13:09.000000 asp_selftest-0.0.5/src/asp_selftest.egg-info/dependency_links.txt
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)       55 2024-05-23 14:13:09.000000 asp_selftest-0.0.5/src/asp_selftest.egg-info/entry_points.txt
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)       13 2024-05-23 14:13:09.000000 asp_selftest-0.0.5/src/asp_selftest.egg-info/top_level.txt
```

### Comparing `asp_selftest-0.0.4/LICENSE` & `asp_selftest-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `asp_selftest-0.0.4/PKG-INFO` & `asp_selftest-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asp_selftest
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool for running in-source unittests for Anwer Set Programming (ASP)
 Author-email: Erik Groeneveld <ejgroene@ieee.org>
 Project-URL: Homepage, https://github.com/ejgroene/asp-selftest
 Project-URL: Issues, https://github.com/ejgroene/asp-selftest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: ASP
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `asp_selftest-0.0.4/README.md` & `asp_selftest-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `asp_selftest-0.0.4/pyproject.toml` & `asp_selftest-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "asp_selftest"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Erik Groeneveld", email="ejgroene@ieee.org" },
 ]
 description = "A tool for running in-source unittests for Anwer Set Programming (ASP)"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `asp_selftest-0.0.4/src/asp_selftest/__init__.py` & `asp_selftest-0.0.5/src/asp_selftest/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 from .runasptests import runasptests, register
 
 
 
 @test
 def program_with_python():
-    """ test import of 'register'; here because runasptests modules must ve finished importing """
-    from .runasptests import do_tests
-    t = do_tests("""
+    """ test import of 'register'; here because runasptests modules must have finished importing """
+    from .runasptests import parse_and_run_tests
+    t = parse_and_run_tests("""
 #script (python)
 import clingo
 import asp_selftest
 def f():
     return clingo.String("aap")
 asp_selftest.register(f)
 #end.
```

### Comparing `asp_selftest-0.0.4/src/asp_selftest/example.lp` & `asp_selftest-0.0.5/src/asp_selftest/example.lp`

 * *Files identical despite different names*

### Comparing `asp_selftest-0.0.4/src/asp_selftest/queens.lp` & `asp_selftest-0.0.5/src/asp_selftest/queens.lp`

 * *Files identical despite different names*

### Comparing `asp_selftest-0.0.4/src/asp_selftest.egg-info/PKG-INFO` & `asp_selftest-0.0.5/src/asp_selftest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asp_selftest
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool for running in-source unittests for Anwer Set Programming (ASP)
 Author-email: Erik Groeneveld <ejgroene@ieee.org>
 Project-URL: Homepage, https://github.com/ejgroene/asp-selftest
 Project-URL: Issues, https://github.com/ejgroene/asp-selftest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: ASP
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

