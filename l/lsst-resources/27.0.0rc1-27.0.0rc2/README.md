# Comparing `tmp/lsst_resources-27.0.0rc1.tar.gz` & `tmp/lsst_resources-27.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst_resources-27.0.0rc1.tar", last modified: Wed May  1 21:17:10 2024, max compression
+gzip compressed data, was "lsst_resources-27.0.0rc2.tar", last modified: Thu May 23 01:52:46 2024, max compression
```

## Comparing `lsst_resources-27.0.0rc1.tar` & `lsst_resources-27.0.0rc2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:10.747386 lsst_resources-27.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-01 21:17:10.743386 lsst_resources-27.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:10.735386 lsst_resources-27.0.0rc1/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:10.739386 lsst_resources-27.0.0rc1/doc/lsst.resources/
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/doc/lsst.resources/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/doc/lsst.resources/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/doc/lsst.resources/internal-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:10.735386 lsst_resources-27.0.0rc1/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:10.739386 lsst_resources-27.0.0rc1/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:10.739386 lsst_resources-27.0.0rc1/python/lsst/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:10.743386 lsst_resources-27.0.0rc1/python/lsst/resources/_resourceHandles/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/_resourceHandles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/_resourceHandles/_baseResourceHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/_resourceHandles/_fileResourceHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/_resourceHandles/_httpResourceHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)    12552 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/_resourceHandles/_s3ResourceHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)    57619 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/_resourcePath.py
--rw-r--r--   0 runner    (1001) docker     (127)    21878 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    12576 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/gs.py
--rw-r--r--   0 runner    (1001) docker     (127)    70041 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/location.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/packageresource.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21622 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)    15172 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/s3utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/schemeless.py
--rw-r--r--   0 runner    (1001) docker     (127)    36780 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 21:17:10.000000 lsst_resources-27.0.0rc1/python/lsst/resources/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:10.743386 lsst_resources-27.0.0rc1/python/lsst_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-01 21:17:10.000000 lsst_resources-27.0.0rc1/python/lsst_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-01 21:17:10.000000 lsst_resources-27.0.0rc1/python/lsst_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:17:10.000000 lsst_resources-27.0.0rc1/python/lsst_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-01 21:17:10.000000 lsst_resources-27.0.0rc1/python/lsst_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 21:17:10.000000 lsst_resources-27.0.0rc1/python/lsst_resources.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:17:10.000000 lsst_resources-27.0.0rc1/python/lsst_resources.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-01 21:17:10.747386 lsst_resources-27.0.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:10.743386 lsst_resources-27.0.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/tests/test_gs.py
--rw-r--r--   0 runner    (1001) docker     (127)    40077 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (127)    17060 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/tests/test_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/tests/test_mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/tests/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/tests/test_s3utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/tests/test_schemeless.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:46.952604 lsst_resources-27.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-23 01:52:46.952604 lsst_resources-27.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:46.940604 lsst_resources-27.0.0rc2/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:46.944604 lsst_resources-27.0.0rc2/doc/lsst.resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/doc/lsst.resources/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/doc/lsst.resources/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/doc/lsst.resources/internal-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:46.940604 lsst_resources-27.0.0rc2/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:46.944604 lsst_resources-27.0.0rc2/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:46.948604 lsst_resources-27.0.0rc2/python/lsst/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/python/lsst/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:46.948604 lsst_resources-27.0.0rc2/python/lsst/resources/_resourceHandles/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/python/lsst/resources/_resourceHandles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/python/lsst/resources/_resourceHandles/_baseResourceHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/python/lsst/resources/_resourceHandles/_fileResourceHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/python/lsst/resources/_resourceHandles/_httpResourceHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12552 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/python/lsst/resources/_resourceHandles/_s3ResourceHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57619 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/python/lsst/resources/_resourcePath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21878 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/python/lsst/resources/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12576 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/python/lsst/resources/gs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70041 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/python/lsst/resources/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/python/lsst/resources/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/python/lsst/resources/mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/python/lsst/resources/packageresource.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/python/lsst/resources/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21622 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/python/lsst/resources/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15172 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/python/lsst/resources/s3utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/python/lsst/resources/schemeless.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36780 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/python/lsst/resources/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/python/lsst/resources/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 01:52:46.000000 lsst_resources-27.0.0rc2/python/lsst/resources/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:46.952604 lsst_resources-27.0.0rc2/python/lsst_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-23 01:52:46.000000 lsst_resources-27.0.0rc2/python/lsst_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-23 01:52:46.000000 lsst_resources-27.0.0rc2/python/lsst_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:52:46.000000 lsst_resources-27.0.0rc2/python/lsst_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-23 01:52:46.000000 lsst_resources-27.0.0rc2/python/lsst_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 01:52:46.000000 lsst_resources-27.0.0rc2/python/lsst_resources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:52:46.000000 lsst_resources-27.0.0rc2/python/lsst_resources.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-23 01:52:46.952604 lsst_resources-27.0.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:46.952604 lsst_resources-27.0.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/tests/test_gs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40077 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17060 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/tests/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/tests/test_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/tests/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/tests/test_s3utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-23 01:52:35.000000 lsst_resources-27.0.0rc2/tests/test_schemeless.py
```

### Comparing `lsst_resources-27.0.0rc1/LICENSE` & `lsst_resources-27.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/PKG-INFO` & `lsst_resources-27.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-resources
-Version: 27.0.0rc1
+Version: 27.0.0rc2
 Summary: An abstraction layer for reading and writing from URI file resources.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/resources
 Keywords: lsst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_resources-27.0.0rc1/README.md` & `lsst_resources-27.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/doc/lsst.resources/CHANGES.rst` & `lsst_resources-27.0.0rc2/doc/lsst.resources/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/doc/lsst.resources/index.rst` & `lsst_resources-27.0.0rc2/doc/lsst.resources/index.rst`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/pyproject.toml` & `lsst_resources-27.0.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/python/lsst/resources/__init__.py` & `lsst_resources-27.0.0rc2/python/lsst/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/python/lsst/resources/_resourceHandles/_baseResourceHandle.py` & `lsst_resources-27.0.0rc2/python/lsst/resources/_resourceHandles/_baseResourceHandle.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/python/lsst/resources/_resourceHandles/_fileResourceHandle.py` & `lsst_resources-27.0.0rc2/python/lsst/resources/_resourceHandles/_fileResourceHandle.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/python/lsst/resources/_resourceHandles/_httpResourceHandle.py` & `lsst_resources-27.0.0rc2/python/lsst/resources/_resourceHandles/_httpResourceHandle.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/python/lsst/resources/_resourceHandles/_s3ResourceHandle.py` & `lsst_resources-27.0.0rc2/python/lsst/resources/_resourceHandles/_s3ResourceHandle.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/python/lsst/resources/_resourcePath.py` & `lsst_resources-27.0.0rc2/python/lsst/resources/_resourcePath.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/python/lsst/resources/file.py` & `lsst_resources-27.0.0rc2/python/lsst/resources/file.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/python/lsst/resources/gs.py` & `lsst_resources-27.0.0rc2/python/lsst/resources/gs.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/python/lsst/resources/http.py` & `lsst_resources-27.0.0rc2/python/lsst/resources/http.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/python/lsst/resources/location.py` & `lsst_resources-27.0.0rc2/python/lsst/resources/location.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/python/lsst/resources/mem.py` & `lsst_resources-27.0.0rc2/python/lsst/resources/mem.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/python/lsst/resources/packageresource.py` & `lsst_resources-27.0.0rc2/python/lsst/resources/packageresource.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/python/lsst/resources/s3.py` & `lsst_resources-27.0.0rc2/python/lsst/resources/s3.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/python/lsst/resources/s3utils.py` & `lsst_resources-27.0.0rc2/python/lsst/resources/s3utils.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/python/lsst/resources/schemeless.py` & `lsst_resources-27.0.0rc2/python/lsst/resources/schemeless.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/python/lsst/resources/tests.py` & `lsst_resources-27.0.0rc2/python/lsst/resources/tests.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/python/lsst/resources/utils.py` & `lsst_resources-27.0.0rc2/python/lsst/resources/utils.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/python/lsst_resources.egg-info/PKG-INFO` & `lsst_resources-27.0.0rc2/python/lsst_resources.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-resources
-Version: 27.0.0rc1
+Version: 27.0.0rc2
 Summary: An abstraction layer for reading and writing from URI file resources.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/resources
 Keywords: lsst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_resources-27.0.0rc1/python/lsst_resources.egg-info/SOURCES.txt` & `lsst_resources-27.0.0rc2/python/lsst_resources.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/tests/test_file.py` & `lsst_resources-27.0.0rc2/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/tests/test_gs.py` & `lsst_resources-27.0.0rc2/tests/test_gs.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/tests/test_http.py` & `lsst_resources-27.0.0rc2/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/tests/test_location.py` & `lsst_resources-27.0.0rc2/tests/test_location.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/tests/test_mem.py` & `lsst_resources-27.0.0rc2/tests/test_mem.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/tests/test_resource.py` & `lsst_resources-27.0.0rc2/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/tests/test_s3.py` & `lsst_resources-27.0.0rc2/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/tests/test_s3utils.py` & `lsst_resources-27.0.0rc2/tests/test_s3utils.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.0.0rc1/tests/test_schemeless.py` & `lsst_resources-27.0.0rc2/tests/test_schemeless.py`

 * *Files identical despite different names*

