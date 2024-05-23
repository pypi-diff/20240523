# Comparing `tmp/midas_open_parser-0.1.12.tar.gz` & `tmp/midas_open_parser-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midas_open_parser-0.1.12.tar", last modified: Thu May 23 01:37:53 2024, max compression
+gzip compressed data, was "midas_open_parser-0.1.13.tar", last modified: Thu May 23 01:41:02 2024, max compression
```

## Comparing `midas_open_parser-0.1.12.tar` & `midas_open_parser-0.1.13.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:37:53.711532 midas_open_parser-0.1.12/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-23 01:37:43.000000 midas_open_parser-0.1.12/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-23 01:37:53.711532 midas_open_parser-0.1.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-23 01:37:43.000000 midas_open_parser-0.1.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:37:53.711532 midas_open_parser-0.1.12/midas_open_parser/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-23 01:37:43.000000 midas_open_parser-0.1.12/midas_open_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-23 01:37:43.000000 midas_open_parser-0.1.12/midas_open_parser/badc_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-05-23 01:37:43.000000 midas_open_parser-0.1.12/midas_open_parser/midas.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-23 01:37:43.000000 midas_open_parser-0.1.12/midas_open_parser/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:37:53.711532 midas_open_parser-0.1.12/midas_open_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-23 01:37:53.000000 midas_open_parser-0.1.12/midas_open_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-23 01:37:53.000000 midas_open_parser-0.1.12/midas_open_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:37:53.000000 midas_open_parser-0.1.12/midas_open_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 01:37:53.000000 midas_open_parser-0.1.12/midas_open_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-23 01:37:43.000000 midas_open_parser-0.1.12/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 01:37:53.711532 midas_open_parser-0.1.12/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:41:02.606037 midas_open_parser-0.1.13/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-23 01:40:53.000000 midas_open_parser-0.1.13/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-23 01:41:02.606037 midas_open_parser-0.1.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-23 01:40:53.000000 midas_open_parser-0.1.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:41:02.606037 midas_open_parser-0.1.13/midas_open_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-23 01:40:53.000000 midas_open_parser-0.1.13/midas_open_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-23 01:40:53.000000 midas_open_parser-0.1.13/midas_open_parser/badc_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-05-23 01:40:53.000000 midas_open_parser-0.1.13/midas_open_parser/midas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-23 01:40:53.000000 midas_open_parser-0.1.13/midas_open_parser/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:41:02.606037 midas_open_parser-0.1.13/midas_open_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-23 01:41:02.000000 midas_open_parser-0.1.13/midas_open_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-23 01:41:02.000000 midas_open_parser-0.1.13/midas_open_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:41:02.000000 midas_open_parser-0.1.13/midas_open_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 01:41:02.000000 midas_open_parser-0.1.13/midas_open_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-23 01:40:53.000000 midas_open_parser-0.1.13/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 01:41:02.606037 midas_open_parser-0.1.13/setup.cfg
```

### Comparing `midas_open_parser-0.1.12/LICENSE.txt` & `midas_open_parser-0.1.13/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `midas_open_parser-0.1.12/PKG-INFO` & `midas_open_parser-0.1.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas_open_parser
-Version: 0.1.12
+Version: 0.1.13
 Summary: A Python library for parsing BADC-CSV files from the MIDAS Open dataset
 Author-email: TempoTerra <vanuan+midasparser@gmail.com>
 Project-URL: Bug Tracker, https://github.com/tempoterra/midas_open_parser/issues
 Project-URL: Documentation, https://tempoterra.github.io/midas_open_parser
 Project-URL: Source Code, https://github.com/tempoterra/midas_open_parser
 Keywords: atmospheric-science,midas-open,badc-csv,parser,environmental-data
 Classifier: Programming Language :: Python :: 3
```

### Comparing `midas_open_parser-0.1.12/README.md` & `midas_open_parser-0.1.13/README.md`

 * *Files identical despite different names*

### Comparing `midas_open_parser-0.1.12/midas_open_parser/__init__.py` & `midas_open_parser-0.1.13/midas_open_parser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 A Python library for parsing BADC-CSV files from the MIDAS Open dataset.
 
 This library provides a flexible and extensible framework for handling various
 metadata labels and structures found in the MIDAS Open dataset.
 """
 
-__version__ = "0.1.12"
+__version__ = "0.1.13"
 __author__ = "Vanuan"
 __email__ = "vanuan+midasparser@gmail.com"
 
 from .badc_csv import parse_badc_csv, parse_badc_csv_metadata
 from .midas import extract_midas_metadata, UnknownMetadataLabelError
 
 __all__ = [
```

### Comparing `midas_open_parser-0.1.12/midas_open_parser/badc_csv.py` & `midas_open_parser-0.1.13/midas_open_parser/badc_csv.py`

 * *Files identical despite different names*

### Comparing `midas_open_parser-0.1.12/midas_open_parser/midas.py` & `midas_open_parser-0.1.13/midas_open_parser/midas.py`

 * *Files identical despite different names*

### Comparing `midas_open_parser-0.1.12/midas_open_parser/test.py` & `midas_open_parser-0.1.13/midas_open_parser/test.py`

 * *Files identical despite different names*

### Comparing `midas_open_parser-0.1.12/midas_open_parser.egg-info/PKG-INFO` & `midas_open_parser-0.1.13/midas_open_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas_open_parser
-Version: 0.1.12
+Version: 0.1.13
 Summary: A Python library for parsing BADC-CSV files from the MIDAS Open dataset
 Author-email: TempoTerra <vanuan+midasparser@gmail.com>
 Project-URL: Bug Tracker, https://github.com/tempoterra/midas_open_parser/issues
 Project-URL: Documentation, https://tempoterra.github.io/midas_open_parser
 Project-URL: Source Code, https://github.com/tempoterra/midas_open_parser
 Keywords: atmospheric-science,midas-open,badc-csv,parser,environmental-data
 Classifier: Programming Language :: Python :: 3
```

### Comparing `midas_open_parser-0.1.12/pyproject.toml` & `midas_open_parser-0.1.13/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "midas_open_parser"
-version = "0.1.12"
+version = "0.1.13"
 authors = [
     {name = "TempoTerra", email = "vanuan+midasparser@gmail.com"},
 ]
 description = "A Python library for parsing BADC-CSV files from the MIDAS Open dataset"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

