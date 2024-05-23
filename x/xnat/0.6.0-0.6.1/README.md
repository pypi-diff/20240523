# Comparing `tmp/xnat-0.6.0.tar.gz` & `tmp/xnat-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xnat-0.6.0.tar", last modified: Tue May 14 16:26:10 2024, max compression
+gzip compressed data, was "dist/xnat-0.6.1.tar", last modified: Thu May 23 17:06:23 2024, max compression
```

## Comparing `xnat-0.6.0.tar` & `xnat-0.6.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:26:10.000000 xnat-0.6.0/
--rw-rw-rw-   0 root         (0) root         (0)    10349 2024-05-14 16:26:01.000000 xnat-0.6.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-14 16:26:01.000000 xnat-0.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3302 2024-05-14 16:26:10.000000 xnat-0.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2215 2024-05-14 16:26:01.000000 xnat-0.6.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-14 16:26:01.000000 xnat-0.6.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 16:26:10.000000 xnat-0.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3074 2024-05-14 16:26:01.000000 xnat-0.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:26:10.000000 xnat-0.6.0/xnat/
--rw-rw-rw-   0 root         (0) root         (0)    29831 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:26:10.000000 xnat-0.6.0/xnat/cli/
--rw-rw-rw-   0 root         (0) root         (0)     2212 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1588 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/cli/download.py
--rw-rw-rw-   0 root         (0) root         (0)     2463 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/cli/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1742 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/cli/importing.py
--rw-rw-rw-   0 root         (0) root         (0)     2331 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/cli/listings.py
--rw-rw-rw-   0 root         (0) root         (0)     5253 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/cli/prearchive.py
--rw-rw-rw-   0 root         (0) root         (0)     5282 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/cli/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     5312 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/cli/scripts.py
--rw-rw-rw-   0 root         (0) root         (0)       64 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/cli/search.py
--rw-rw-rw-   0 root         (0) root         (0)     4517 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    52743 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/convert_xsd.py
--rw-rw-rw-   0 root         (0) root         (0)    47814 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/core.py
--rw-rw-rw-   0 root         (0) root         (0)     5295 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/datatypes.py
--rw-rw-rw-   0 root         (0) root         (0)     2575 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6066 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/header.py
--rw-rw-rw-   0 root         (0) root         (0)     2567 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/inspect.py
--rw-rw-rw-   0 root         (0) root         (0)     4956 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/map.py
--rw-rw-rw-   0 root         (0) root         (0)    42165 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3365 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/plugins.py
--rw-rw-rw-   0 root         (0) root         (0)    18865 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/prearchive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:26:10.000000 xnat-0.6.0/xnat/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9501 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/scripts/copy_project.py
--rw-rw-rw-   0 root         (0) root         (0)    11540 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/scripts/data_integrity_check.py
--rw-rw-rw-   0 root         (0) root         (0)     1791 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/scripts/delete_project.py
--rw-rw-rw-   0 root         (0) root         (0)     2425 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/scripts/import_experiment_dir.py
--rw-rw-rw-   0 root         (0) root         (0)    11788 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/search.py
--rw-rw-rw-   0 root         (0) root         (0)    18611 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/services.py
--rw-rw-rw-   0 root         (0) root         (0)    51455 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/session.py
--rw-rw-rw-   0 root         (0) root         (0)      185 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/type_hints.py
--rw-rw-rw-   0 root         (0) root         (0)     2980 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/users.py
--rw-rw-rw-   0 root         (0) root         (0)     6559 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/utils.py
--rw-r--r--   0 root         (0) root         (0)       18 2024-05-14 16:26:10.000000 xnat-0.6.0/xnat/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:26:10.000000 xnat-0.6.0/xnat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3302 2024-05-14 16:26:10.000000 xnat-0.6.0/xnat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      878 2024-05-14 16:26:10.000000 xnat-0.6.0/xnat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 16:26:10.000000 xnat-0.6.0/xnat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      154 2024-05-14 16:26:10.000000 xnat-0.6.0/xnat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      155 2024-05-14 16:26:10.000000 xnat-0.6.0/xnat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-05-14 16:26:10.000000 xnat-0.6.0/xnat.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:06:23.000000 xnat-0.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)    10349 2024-05-23 17:06:14.000000 xnat-0.6.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-23 17:06:14.000000 xnat-0.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3302 2024-05-23 17:06:23.000000 xnat-0.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2215 2024-05-23 17:06:14.000000 xnat-0.6.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-23 17:06:14.000000 xnat-0.6.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 17:06:23.000000 xnat-0.6.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3074 2024-05-23 17:06:14.000000 xnat-0.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:06:23.000000 xnat-0.6.1/xnat/
+-rw-rw-rw-   0 root         (0) root         (0)    29831 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:06:23.000000 xnat-0.6.1/xnat/cli/
+-rw-rw-rw-   0 root         (0) root         (0)     2212 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1588 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/cli/download.py
+-rw-rw-rw-   0 root         (0) root         (0)     2463 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/cli/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/cli/importing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2331 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/cli/listings.py
+-rw-rw-rw-   0 root         (0) root         (0)     5253 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/cli/prearchive.py
+-rw-rw-rw-   0 root         (0) root         (0)     5282 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/cli/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5312 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/cli/scripts.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/cli/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     4517 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    52743 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/convert_xsd.py
+-rw-rw-rw-   0 root         (0) root         (0)    47814 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     5295 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/datatypes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2575 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6066 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     2567 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/inspect.py
+-rw-rw-rw-   0 root         (0) root         (0)     4956 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/map.py
+-rw-rw-rw-   0 root         (0) root         (0)    42165 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3365 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/plugins.py
+-rw-rw-rw-   0 root         (0) root         (0)    18865 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/prearchive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:06:23.000000 xnat-0.6.1/xnat/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9501 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/scripts/copy_project.py
+-rw-rw-rw-   0 root         (0) root         (0)    11540 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/scripts/data_integrity_check.py
+-rw-rw-rw-   0 root         (0) root         (0)     1791 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/scripts/delete_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     2425 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/scripts/import_experiment_dir.py
+-rw-rw-rw-   0 root         (0) root         (0)    11786 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/search.py
+-rw-rw-rw-   0 root         (0) root         (0)    18611 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/services.py
+-rw-rw-rw-   0 root         (0) root         (0)    51455 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/session.py
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/type_hints.py
+-rw-rw-rw-   0 root         (0) root         (0)     2980 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/users.py
+-rw-rw-rw-   0 root         (0) root         (0)     6559 2024-05-23 17:06:14.000000 xnat-0.6.1/xnat/utils.py
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-23 17:06:23.000000 xnat-0.6.1/xnat/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:06:23.000000 xnat-0.6.1/xnat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3302 2024-05-23 17:06:23.000000 xnat-0.6.1/xnat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      878 2024-05-23 17:06:23.000000 xnat-0.6.1/xnat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 17:06:23.000000 xnat-0.6.1/xnat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2024-05-23 17:06:23.000000 xnat-0.6.1/xnat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      155 2024-05-23 17:06:23.000000 xnat-0.6.1/xnat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-23 17:06:23.000000 xnat-0.6.1/xnat.egg-info/top_level.txt
```

### Comparing `xnat-0.6.0/LICENSE` & `xnat-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/PKG-INFO` & `xnat-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnat
-Version: 0.6.0
+Version: 0.6.1
 Summary: An XNAT client that exposes the XNAT REST interface as python objects. Part of the interface is automatically generated based on the servers data model as defined by the xnat schema.
 Home-page: https://gitlab.com/radiology/infrastructure/xnatpy
 Author: H.C. Achterberg
 Author-email: hakim.achterberg@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `xnat-0.6.0/README.rst` & `xnat-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/setup.py` & `xnat-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from __future__ import absolute_import
 from __future__ import unicode_literals
 import os
 from setuptools import setup
 
 # Get information about the version (polling mercurial if possible)
-version = '0.6.0'
+version = '0.6.1'
 
 # When building something else than a release (tag) append the job id to the version.
 if os.environ.get('CI_COMMIT_TAG'):
     pass
 elif os.environ.get('CI_JOB_ID'):
     version += ".{}".format(os.environ['CI_JOB_ID'])
```

### Comparing `xnat-0.6.0/xnat/__init__.py` & `xnat-0.6.1/xnat/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 from .convert_xsd import SchemaParser
 from .map import MappingLevel
 from .utils import JSessionAuth
 from .mixin import FilterFunctions
 
 GEN_MODULES = {}
 
-__version__ = '0.6.0'
+__version__ = '0.6.1'
 __all__ = ['connect', 'exceptions', 'MappingLevel', 'FilterFunctions']
 
 class StringLoader(importlib.abc.SourceLoader):
     def __init__(self, data):
         self.data = data
 
     def get_data(self, pathname):
```

### Comparing `xnat-0.6.0/xnat/cli/__init__.py` & `xnat-0.6.1/xnat/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/cli/download.py` & `xnat-0.6.1/xnat/cli/download.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/cli/helpers.py` & `xnat-0.6.1/xnat/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/cli/importing.py` & `xnat-0.6.1/xnat/cli/importing.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/cli/listings.py` & `xnat-0.6.1/xnat/cli/listings.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/cli/prearchive.py` & `xnat-0.6.1/xnat/cli/prearchive.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/cli/rest.py` & `xnat-0.6.1/xnat/cli/rest.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/cli/scripts.py` & `xnat-0.6.1/xnat/cli/scripts.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/constants.py` & `xnat-0.6.1/xnat/constants.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/convert_xsd.py` & `xnat-0.6.1/xnat/convert_xsd.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/core.py` & `xnat-0.6.1/xnat/core.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/datatypes.py` & `xnat-0.6.1/xnat/datatypes.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/exceptions.py` & `xnat-0.6.1/xnat/exceptions.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/header.py` & `xnat-0.6.1/xnat/header.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/inspect.py` & `xnat-0.6.1/xnat/inspect.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/map.py` & `xnat-0.6.1/xnat/map.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/mixin.py` & `xnat-0.6.1/xnat/mixin.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/plugins.py` & `xnat-0.6.1/xnat/plugins.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/prearchive.py` & `xnat-0.6.1/xnat/prearchive.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/scripts/copy_project.py` & `xnat-0.6.1/xnat/scripts/copy_project.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/scripts/data_integrity_check.py` & `xnat-0.6.1/xnat/scripts/data_integrity_check.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/scripts/delete_project.py` & `xnat-0.6.1/xnat/scripts/delete_project.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/scripts/import_experiment_dir.py` & `xnat-0.6.1/xnat/scripts/import_experiment_dir.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/search.py` & `xnat-0.6.1/xnat/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
     def to_xml(self):
         # Create main elements
         bundle = ElementTree.Element(ElementTree.QName(xdat_ns, "bundle"))
         root_elem_name = ElementTree.SubElement(bundle, ElementTree.QName(xdat_ns, "root_element_name"))
         root_elem_name.text = self.xsi_type
 
         # Add search fields
-        if self.fields is None and self.queried_class.DEFAULT_SEARCH_FIELDS:
+        if (not self.fields) and self.queried_class.DEFAULT_SEARCH_FIELDS:
             self.fields = tuple(getattr(self.queried_class, x) for x in self.queried_class.DEFAULT_SEARCH_FIELDS)
 
         if self.fields is not None:
             for idx, x in enumerate(self.fields):
                 search_where = ElementTree.SubElement(bundle, ElementTree.QName(xdat_ns, "search_field"))
                 element_name = ElementTree.SubElement(search_where, ElementTree.QName(xdat_ns, "element_name"))
                 element_name.text = x.xsi_type
```

### Comparing `xnat-0.6.0/xnat/services.py` & `xnat-0.6.1/xnat/services.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/session.py` & `xnat-0.6.1/xnat/session.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/users.py` & `xnat-0.6.1/xnat/users.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat/utils.py` & `xnat-0.6.1/xnat/utils.py`

 * *Files identical despite different names*

### Comparing `xnat-0.6.0/xnat.egg-info/PKG-INFO` & `xnat-0.6.1/xnat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnat
-Version: 0.6.0
+Version: 0.6.1
 Summary: An XNAT client that exposes the XNAT REST interface as python objects. Part of the interface is automatically generated based on the servers data model as defined by the xnat schema.
 Home-page: https://gitlab.com/radiology/infrastructure/xnatpy
 Author: H.C. Achterberg
 Author-email: hakim.achterberg@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `xnat-0.6.0/xnat.egg-info/SOURCES.txt` & `xnat-0.6.1/xnat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

