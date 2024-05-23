# Comparing `tmp/caen_felib-1.1.0.tar.gz` & `tmp/caen_felib-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/software/frontend/py-caen-felib/dist/.tmp-enenl5fp/caen_felib-1.1.0.tar", last modified: Mon Dec 11 15:45:08 2023, max compression
+gzip compressed data, was "/builds/software/frontend/py-caen-felib/dist/.tmp-n02zkh_i/caen_felib-1.2.0.tar", last modified: Thu May 23 12:43:57 2024, max compression
```

## Comparing `caen_felib-1.1.0.tar` & `caen_felib-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 15:45:08.000000 caen_felib-1.1.0/
--rw-r--r--   0 root         (0) root         (0)     4445 2023-12-11 15:45:08.000000 caen_felib-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3357 2023-12-11 15:37:06.000000 caen_felib-1.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1152 2023-12-11 15:37:06.000000 caen_felib-1.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-11 15:45:08.000000 caen_felib-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-12-11 15:37:06.000000 caen_felib-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 15:45:08.000000 caen_felib-1.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 15:45:08.000000 caen_felib-1.1.0/src/caen_felib/
--rw-rw-rw-   0 root         (0) root         (0)      414 2023-12-11 15:37:06.000000 caen_felib-1.1.0/src/caen_felib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3413 2023-12-11 15:37:06.000000 caen_felib-1.1.0/src/caen_felib/_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    18695 2023-12-11 15:37:06.000000 caen_felib-1.1.0/src/caen_felib/device.py
--rw-rw-rw-   0 root         (0) root         (0)     1077 2023-12-11 15:37:06.000000 caen_felib-1.1.0/src/caen_felib/error.py
--rw-rw-rw-   0 root         (0) root         (0)     9818 2023-12-11 15:44:59.000000 caen_felib-1.1.0/src/caen_felib/lib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 15:45:08.000000 caen_felib-1.1.0/src/caen_felib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4445 2023-12-11 15:45:08.000000 caen_felib-1.1.0/src/caen_felib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      345 2023-12-11 15:45:08.000000 caen_felib-1.1.0/src/caen_felib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-11 15:45:08.000000 caen_felib-1.1.0/src/caen_felib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-12-11 15:45:08.000000 caen_felib-1.1.0/src/caen_felib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-12-11 15:45:08.000000 caen_felib-1.1.0/src/caen_felib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:43:57.000000 caen_felib-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)     4407 2024-05-23 12:43:57.000000 caen_felib-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3357 2024-05-23 12:43:44.000000 caen_felib-1.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1104 2024-05-23 12:43:44.000000 caen_felib-1.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 12:43:57.000000 caen_felib-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-23 12:43:44.000000 caen_felib-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:43:57.000000 caen_felib-1.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:43:57.000000 caen_felib-1.2.0/src/caen_felib/
+-rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-23 12:43:44.000000 caen_felib-1.2.0/src/caen_felib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3413 2024-05-23 12:43:44.000000 caen_felib-1.2.0/src/caen_felib/_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    18641 2024-05-23 12:43:44.000000 caen_felib-1.2.0/src/caen_felib/device.py
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2024-05-23 12:43:44.000000 caen_felib-1.2.0/src/caen_felib/error.py
+-rw-rw-rw-   0 root         (0) root         (0)     9818 2024-05-23 12:43:44.000000 caen_felib-1.2.0/src/caen_felib/lib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:43:57.000000 caen_felib-1.2.0/src/caen_felib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4407 2024-05-23 12:43:57.000000 caen_felib-1.2.0/src/caen_felib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      345 2024-05-23 12:43:57.000000 caen_felib-1.2.0/src/caen_felib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 12:43:57.000000 caen_felib-1.2.0/src/caen_felib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2024-05-23 12:43:57.000000 caen_felib-1.2.0/src/caen_felib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-23 12:43:57.000000 caen_felib-1.2.0/src/caen_felib.egg-info/top_level.txt
```

### Comparing `caen_felib-1.1.0/PKG-INFO` & `caen_felib-1.2.0/src/caen_felib.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
-Name: caen_felib
-Version: 1.1.0
+Name: caen-felib
+Version: 1.2.0
 Summary: Official Python wrapper for the CAEN FELib.
-Author-email: Giovanni Cerretani <g.cerretani@caen.it>, Daniele Ninci <d.ninci@caen.it>
-Project-URL: homepage, https://www.caen.it
-Project-URL: documentation, https://www.caen.it/products/caen-felib-library/
+Author: Giovanni Cerretani, Daniele Ninci
+Project-URL: Homepage, https://www.caen.it
+Project-URL: Documentation, https://www.caen.it/products/caen-felib-library/
+Project-URL: Support, https://www.caen.it/mycaen/support/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Typing :: Typed
```

### Comparing `caen_felib-1.1.0/README.md` & `caen_felib-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `caen_felib-1.1.0/pyproject.toml` & `caen_felib-1.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [project]
 name = "caen_felib"
 authors = [
-	{ name="Giovanni Cerretani", email="g.cerretani@caen.it" },
-	{ name="Daniele Ninci", email="d.ninci@caen.it" },
+	{ name="Giovanni Cerretani" },
+	{ name="Daniele Ninci" },
 ]
 description = "Official Python wrapper for the CAEN FELib."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
 	"Development Status :: 4 - Beta",
 	"Intended Audience :: Science/Research",
 	"License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
 	"Natural Language :: English",
 	"Operating System :: OS Independent",
 	"Programming Language :: Python :: 3",
-	"Programming Language :: Python :: 3.7",
 	"Programming Language :: Python :: 3.8",
 	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11",
 	"Programming Language :: Python :: 3.12",
 	"Topic :: Scientific/Engineering :: Physics",
 	"Typing :: Typed",
 ]
 dependencies = [
-	"numpy>=1.19",
+	"numpy>=1.20",
 	"typing-extensions>=4.0.0",
 ]
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = {attr = "caen_felib.__version__"}
 
 [project.urls]
-homepage = "https://www.caen.it"
-documentation = "https://www.caen.it/products/caen-felib-library/"
+Homepage = "https://www.caen.it"
+Documentation = "https://www.caen.it/products/caen-felib-library/"
+Support = "https://www.caen.it/mycaen/support/"
```

### Comparing `caen_felib-1.1.0/src/caen_felib/_utils.py` & `caen_felib-1.2.0/src/caen_felib/_utils.py`

 * *Files identical despite different names*

### Comparing `caen_felib-1.1.0/src/caen_felib/device.py` & `caen_felib-1.2.0/src/caen_felib/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 import ctypes as ct
 from enum import IntEnum, unique
 from functools import wraps
 from json import dumps, loads
 from typing import Any, Dict, Generator, List, Optional, Tuple, Type
 
 import numpy as np
+import numpy.typing as npt
 from typing_extensions import TypedDict, Self
 
 from caen_felib import lib, _utils
 
 # Comments on imports:
 # - TypedDict moved to typing on Python 3.8
 # - Self moved to typing on Python 3.11
-# - numpy.typing.typing.DTypeLike could be useful but requires numpy >= 1.20
+# - numpy.typing.DTypeLike requires numpy >= 1.20
 
 
-_type_map: Dict[str, Type] = {
-    # Generic Type could be replaced by numpy.typing.DTypeLike
+_type_map: Dict[str, npt.DTypeLike] = {
     'U8': ct.c_uint8,
     'U16': ct.c_uint16,
     'U32': ct.c_uint32,
     'U64': ct.c_uint64,
     'I8': ct.c_int8,
     'I16': ct.c_int16,
     'I32': ct.c_int32,
```

### Comparing `caen_felib-1.1.0/src/caen_felib/error.py` & `caen_felib-1.2.0/src/caen_felib/error.py`

 * *Files identical despite different names*

### Comparing `caen_felib-1.1.0/src/caen_felib/lib.py` & `caen_felib-1.2.0/src/caen_felib/lib.py`

 * *Files identical despite different names*

### Comparing `caen_felib-1.1.0/src/caen_felib.egg-info/PKG-INFO` & `caen_felib-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
-Name: caen-felib
-Version: 1.1.0
+Name: caen_felib
+Version: 1.2.0
 Summary: Official Python wrapper for the CAEN FELib.
-Author-email: Giovanni Cerretani <g.cerretani@caen.it>, Daniele Ninci <d.ninci@caen.it>
-Project-URL: homepage, https://www.caen.it
-Project-URL: documentation, https://www.caen.it/products/caen-felib-library/
+Author: Giovanni Cerretani, Daniele Ninci
+Project-URL: Homepage, https://www.caen.it
+Project-URL: Documentation, https://www.caen.it/products/caen-felib-library/
+Project-URL: Support, https://www.caen.it/mycaen/support/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Typing :: Typed
```

