# Comparing `tmp/papers_dl-0.0.5.tar.gz` & `tmp/papers_dl-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papers_dl-0.0.5.tar", last modified: Tue May  7 19:27:27 2024, max compression
+gzip compressed data, was "papers_dl-0.0.6.tar", last modified: Wed May 22 22:55:18 2024, max compression
```

## Comparing `papers_dl-0.0.5.tar` & `papers_dl-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-07 19:27:27.596951 papers_dl-0.0.5/
--rw-r--r--   0 ben        (501) staff       (20)     1070 2024-03-23 22:45:07.000000 papers_dl-0.0.5/LICENSE
--rw-r--r--   0 ben        (501) staff       (20)     2615 2024-05-07 19:27:27.596624 papers_dl-0.0.5/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     1296 2024-05-04 19:26:22.000000 papers_dl-0.0.5/README.md
--rw-r--r--   0 ben        (501) staff       (20)     1206 2024-05-07 19:25:50.000000 papers_dl-0.0.5/pyproject.toml
--rw-r--r--   0 ben        (501) staff       (20)       38 2024-05-07 19:27:27.597014 papers_dl-0.0.5/setup.cfg
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-07 19:27:27.593840 papers_dl-0.0.5/src/
--rw-r--r--   0 ben        (501) staff       (20)        1 2024-05-06 22:49:47.000000 papers_dl-0.0.5/src/__init__.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-07 19:27:27.596167 papers_dl-0.0.5/src/papers_dl.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     2615 2024-05-07 19:27:27.000000 papers_dl-0.0.5/src/papers_dl.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      374 2024-05-07 19:27:27.000000 papers_dl-0.0.5/src/papers_dl.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2024-05-07 19:27:27.000000 papers_dl-0.0.5/src/papers_dl.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       45 2024-05-07 19:27:27.000000 papers_dl-0.0.5/src/papers_dl.egg-info/entry_points.txt
--rw-r--r--   0 ben        (501) staff       (20)      411 2024-05-07 19:27:27.000000 papers_dl-0.0.5/src/papers_dl.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)       32 2024-05-07 19:27:27.000000 papers_dl-0.0.5/src/papers_dl.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)     3562 2024-05-04 19:19:41.000000 papers_dl-0.0.5/src/papers_dl.py
--rw-r--r--   0 ben        (501) staff       (20)     2384 2024-05-04 19:19:49.000000 papers_dl-0.0.5/src/parse.py
--rw-r--r--   0 ben        (501) staff       (20)     7881 2024-05-04 19:19:49.000000 papers_dl-0.0.5/src/scihub.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-07 19:27:27.595889 papers_dl-0.0.5/tests/
--rw-r--r--   0 ben        (501) staff       (20)     1714 2024-05-04 19:19:41.000000 papers_dl-0.0.5/tests/test_cli.py
--rw-r--r--   0 ben        (501) staff       (20)      825 2024-05-04 19:19:41.000000 papers_dl-0.0.5/tests/test_fetch.py
--rw-r--r--   0 ben        (501) staff       (20)     2347 2024-05-04 19:19:41.000000 papers_dl-0.0.5/tests/test_parse.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-22 22:55:18.022138 papers_dl-0.0.6/
+-rw-r--r--   0 ben        (501) staff       (20)     1070 2024-03-23 22:45:07.000000 papers_dl-0.0.6/LICENSE
+-rw-r--r--   0 ben        (501) staff       (20)     2615 2024-05-22 22:55:18.021824 papers_dl-0.0.6/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     1296 2024-05-04 19:26:22.000000 papers_dl-0.0.6/README.md
+-rw-r--r--   0 ben        (501) staff       (20)     1276 2024-05-07 21:38:53.000000 papers_dl-0.0.6/pyproject.toml
+-rw-r--r--   0 ben        (501) staff       (20)       38 2024-05-22 22:55:18.022201 papers_dl-0.0.6/setup.cfg
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-22 22:55:18.018788 papers_dl-0.0.6/src/
+-rw-r--r--   0 ben        (501) staff       (20)        1 2024-05-06 22:49:47.000000 papers_dl-0.0.6/src/__init__.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-22 22:55:18.021375 papers_dl-0.0.6/src/papers_dl.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     2615 2024-05-22 22:55:18.000000 papers_dl-0.0.6/src/papers_dl.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      389 2024-05-22 22:55:18.000000 papers_dl-0.0.6/src/papers_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2024-05-22 22:55:18.000000 papers_dl-0.0.6/src/papers_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)       45 2024-05-22 22:55:18.000000 papers_dl-0.0.6/src/papers_dl.egg-info/entry_points.txt
+-rw-r--r--   0 ben        (501) staff       (20)      411 2024-05-22 22:55:18.000000 papers_dl-0.0.6/src/papers_dl.egg-info/requires.txt
+-rw-r--r--   0 ben        (501) staff       (20)       40 2024-05-22 22:55:18.000000 papers_dl-0.0.6/src/papers_dl.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)     3735 2024-05-07 21:14:52.000000 papers_dl-0.0.6/src/papers_dl.py
+-rw-r--r--   0 ben        (501) staff       (20)     2384 2024-05-04 19:19:49.000000 papers_dl-0.0.6/src/parse.py
+-rw-r--r--   0 ben        (501) staff       (20)     7881 2024-05-04 19:19:49.000000 papers_dl-0.0.6/src/scihub.py
+-rw-r--r--   0 ben        (501) staff       (20)       20 2024-05-07 21:05:21.000000 papers_dl-0.0.6/src/version.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-22 22:55:18.020750 papers_dl-0.0.6/tests/
+-rw-r--r--   0 ben        (501) staff       (20)     1714 2024-05-04 19:19:41.000000 papers_dl-0.0.6/tests/test_cli.py
+-rw-r--r--   0 ben        (501) staff       (20)      825 2024-05-04 19:19:41.000000 papers_dl-0.0.6/tests/test_fetch.py
+-rw-r--r--   0 ben        (501) staff       (20)     2347 2024-05-04 19:19:41.000000 papers_dl-0.0.6/tests/test_parse.py
```

### Comparing `papers_dl-0.0.5/LICENSE` & `papers_dl-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.5/PKG-INFO` & `papers_dl-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papers-dl
-Version: 0.0.5
+Version: 0.0.6
 Summary: A command line application for downloading scientific papers
 Author-email: Ben Muthalaly <benmuthalaly@gmail.com>
 Project-URL: Homepage, https://github.com/benmuth/papers-dl
 Project-URL: Issues, https://github.com/benmuth/papers-dl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `papers_dl-0.0.5/README.md` & `papers_dl-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.5/pyproject.toml` & `papers_dl-0.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "papers-dl"
-version = "0.0.5"
 authors = [
   { name="Ben Muthalaly", email="benmuthalaly@gmail.com" },
 ]
 description = "A command line application for downloading scientific papers"
 readme = "README.md"
 requires-python = ">=3.8"
+dynamic=["version"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "beautifulsoup4==4.12.3",
@@ -46,7 +46,10 @@
 
 [project.scripts]
 papers-dl = "papers_dl:main"
 
 [project.urls]
 Homepage = "https://github.com/benmuth/papers-dl"
 Issues = "https://github.com/benmuth/papers-dl/issues"
+
+[tool.setuptools.dynamic]
+version = {attr = "version.__version__"}
```

### Comparing `papers_dl-0.0.5/src/papers_dl.egg-info/PKG-INFO` & `papers_dl-0.0.6/src/papers_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papers-dl
-Version: 0.0.5
+Version: 0.0.6
 Summary: A command line application for downloading scientific papers
 Author-email: Ben Muthalaly <benmuthalaly@gmail.com>
 Project-URL: Homepage, https://github.com/benmuth/papers-dl
 Project-URL: Issues, https://github.com/benmuth/papers-dl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `papers_dl-0.0.5/src/papers_dl.py` & `papers_dl-0.0.6/src/papers_dl.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 DEFAULT_USER_AGENT = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.3 Safari/605.1.15"
 
 
 def save_scihub(identifier: str, out: str, user_agent: str, name: str | None = None):
     """
-    find a paper with the given identifier and download it to the output 
+    find a paper with the given identifier and download it to the output
     directory. If given, name will be the name of the output file. otherwise
     we attempt to find a title from the PDF contents.
     """
 
     sh = SciHub(user_agent)
     print(f"Attempting to download from {identifier}")
 
@@ -49,18 +49,23 @@
         file_name += ".pdf"
         new_path = os.path.join(out, file_name)
         os.rename(result_path, new_path)
         print(f"File downloaded to {new_path}")
 
 
 def main():
+    name = "papers-dl"
     parser = argparse.ArgumentParser(
-        description="Download scientific papers from the command line"
+        prog=name,
+        description="Download scientific papers from the command line",
     )
 
+    from version import __version__
+    parser.add_argument("--version", "-v", action="version", version=f"{name} {__version__}")
+
     subparsers = parser.add_subparsers()
 
     # FETCH
     parser_fetch = subparsers.add_parser(
         "fetch", help="try to download a paper with the given identifier"
     )
```

### Comparing `papers_dl-0.0.5/src/parse.py` & `papers_dl-0.0.6/src/parse.py`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.5/src/scihub.py` & `papers_dl-0.0.6/src/scihub.py`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.5/tests/test_cli.py` & `papers_dl-0.0.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.5/tests/test_fetch.py` & `papers_dl-0.0.6/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.5/tests/test_parse.py` & `papers_dl-0.0.6/tests/test_parse.py`

 * *Files identical despite different names*

