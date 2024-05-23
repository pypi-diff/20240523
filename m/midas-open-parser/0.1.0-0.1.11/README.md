# Comparing `tmp/midas_open_parser-0.1.0.tar.gz` & `tmp/midas_open_parser-0.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midas_open_parser-0.1.0.tar", last modified: Sun May 19 17:10:06 2024, max compression
+gzip compressed data, was "midas_open_parser-0.1.11.tar", last modified: Thu May 23 01:23:00 2024, max compression
```

## Comparing `midas_open_parser-0.1.0.tar` & `midas_open_parser-0.1.11.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-19 17:10:06.660018 midas_open_parser-0.1.0/
--rw-rw-r--   0 john      (1000) john      (1000)     1067 2024-05-17 19:56:11.000000 midas_open_parser-0.1.0/LICENSE.txt
--rw-r--r--   0 john      (1000) john      (1000)     4351 2024-05-19 17:10:06.660018 midas_open_parser-0.1.0/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)     3377 2024-05-16 17:48:27.000000 midas_open_parser-0.1.0/README.md
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-19 17:10:06.659018 midas_open_parser-0.1.0/midas_open_parser/
--rw-rw-r--   0 john      (1000) john      (1000)      613 2024-05-16 16:08:42.000000 midas_open_parser-0.1.0/midas_open_parser/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     2029 2024-05-16 16:10:07.000000 midas_open_parser-0.1.0/midas_open_parser/badc_csv.py
--rw-rw-r--   0 john      (1000) john      (1000)     7271 2024-05-16 16:14:37.000000 midas_open_parser-0.1.0/midas_open_parser/midas.py
--rw-rw-r--   0 john      (1000) john      (1000)      984 2024-05-15 10:53:25.000000 midas_open_parser-0.1.0/midas_open_parser/test.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-19 17:10:06.659018 midas_open_parser-0.1.0/midas_open_parser.egg-info/
--rw-r--r--   0 john      (1000) john      (1000)     4351 2024-05-19 17:10:06.000000 midas_open_parser-0.1.0/midas_open_parser.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)      321 2024-05-19 17:10:06.000000 midas_open_parser-0.1.0/midas_open_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2024-05-19 17:10:06.000000 midas_open_parser-0.1.0/midas_open_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1000) john      (1000)       18 2024-05-19 17:10:06.000000 midas_open_parser-0.1.0/midas_open_parser.egg-info/top_level.txt
--rw-rw-r--   0 john      (1000) john      (1000)     1389 2024-05-19 17:10:02.000000 midas_open_parser-0.1.0/pyproject.toml
--rw-rw-r--   0 john      (1000) john      (1000)       38 2024-05-19 17:10:06.660018 midas_open_parser-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:23:00.867593 midas_open_parser-0.1.11/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-23 01:22:51.000000 midas_open_parser-0.1.11/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-23 01:23:00.867593 midas_open_parser-0.1.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-23 01:22:51.000000 midas_open_parser-0.1.11/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:23:00.863593 midas_open_parser-0.1.11/midas_open_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-23 01:22:51.000000 midas_open_parser-0.1.11/midas_open_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-23 01:22:51.000000 midas_open_parser-0.1.11/midas_open_parser/badc_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-05-23 01:22:51.000000 midas_open_parser-0.1.11/midas_open_parser/midas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-23 01:22:51.000000 midas_open_parser-0.1.11/midas_open_parser/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:23:00.867593 midas_open_parser-0.1.11/midas_open_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-23 01:23:00.000000 midas_open_parser-0.1.11/midas_open_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-23 01:23:00.000000 midas_open_parser-0.1.11/midas_open_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:23:00.000000 midas_open_parser-0.1.11/midas_open_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 01:23:00.000000 midas_open_parser-0.1.11/midas_open_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-23 01:22:51.000000 midas_open_parser-0.1.11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 01:23:00.867593 midas_open_parser-0.1.11/setup.cfg
```

### Comparing `midas_open_parser-0.1.0/LICENSE.txt` & `midas_open_parser-0.1.11/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `midas_open_parser-0.1.0/PKG-INFO` & `midas_open_parser-0.1.11/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas_open_parser
-Version: 0.1.0
+Version: 0.1.11
 Summary: A Python library for parsing BADC-CSV files from the MIDAS Open dataset
 Author-email: TempoTerra <vanuan+midasparser@gmail.com>
 Project-URL: Bug Tracker, https://github.com/tempoterra/midas_open_parser/issues
 Project-URL: Documentation, https://tempoterra.github.io/midas_open_parser
 Project-URL: Source Code, https://github.com/tempoterra/midas_open_parser
 Keywords: atmospheric-science,midas-open,badc-csv,parser,environmental-data
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,17 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # MIDAS Open parser
 
+[![PyPI Version](https://img.shields.io/pypi/v/midas-open-parser)](https://pypi.org/project/midas-open-parser/)
+
+
 `midas_open_parser` is a Python library specifically designed to parse BADC-CSV files from the MIDAS Open dataset.
 
 It provides a tailored and extensible framework for handling the metadata labels and structures found in the MIDAS Open dataset.
 
 The main goal of the `midas_open_parser` project is to provide tools to ingest the MIDAS Open dataset into various destinations.
 
 ## About MIDAS Open and BADC-CSV
```

### Comparing `midas_open_parser-0.1.0/README.md` & `midas_open_parser-0.1.11/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # MIDAS Open parser
 
+[![PyPI Version](https://img.shields.io/pypi/v/midas-open-parser)](https://pypi.org/project/midas-open-parser/)
+
+
 `midas_open_parser` is a Python library specifically designed to parse BADC-CSV files from the MIDAS Open dataset.
 
 It provides a tailored and extensible framework for handling the metadata labels and structures found in the MIDAS Open dataset.
 
 The main goal of the `midas_open_parser` project is to provide tools to ingest the MIDAS Open dataset into various destinations.
 
 ## About MIDAS Open and BADC-CSV
```

### Comparing `midas_open_parser-0.1.0/midas_open_parser/__init__.py` & `midas_open_parser-0.1.11/midas_open_parser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 A Python library for parsing BADC-CSV files from the MIDAS Open dataset.
 
 This library provides a flexible and extensible framework for handling various
 metadata labels and structures found in the MIDAS Open dataset.
 """
 
-__version__ = "0.1.0"
+__version__ = "0.1.11"
 __author__ = "Vanuan"
 __email__ = "vanuan+midasparser@gmail.com"
 
 from .badc_csv import parse_badc_csv, parse_badc_csv_metadata
 from .midas import extract_midas_metadata, UnknownMetadataLabelError
 
 __all__ = [
```

### Comparing `midas_open_parser-0.1.0/midas_open_parser/badc_csv.py` & `midas_open_parser-0.1.11/midas_open_parser/badc_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 This module provides functions for parsing BADC-CSV files and extracting data
 records and metadata.
 """
 import csv
 import sys
 
-from midas import extract_midas_metadata, UnknownMetadataLabelError
+from .midas import extract_midas_metadata, UnknownMetadataLabelError
 
 def parse_badc_csv(file_path):
     """Parse a BADC-CSV file and extract data records.
 
     Args:
         file_path (str): The path to the BADC-CSV file.
```

### Comparing `midas_open_parser-0.1.0/midas_open_parser/midas.py` & `midas_open_parser-0.1.11/midas_open_parser/midas.py`

 * *Files identical despite different names*

### Comparing `midas_open_parser-0.1.0/midas_open_parser/test.py` & `midas_open_parser-0.1.11/midas_open_parser/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # test.py
 import csv
 import sys
 
-from midas import extract_midas_metadata, UnknownMetadataLabelError
-from badc_csv import  parse_badc_csv, parse_badc_csv_metadata
+from .midas import extract_midas_metadata, UnknownMetadataLabelError
+from .badc_csv import  parse_badc_csv, parse_badc_csv_metadata
 
 if __name__ == '__main__':
     print('hello')
 
     try:
         filename = sys.argv[1]
     except IndexError:
```

### Comparing `midas_open_parser-0.1.0/midas_open_parser.egg-info/PKG-INFO` & `midas_open_parser-0.1.11/midas_open_parser.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas_open_parser
-Version: 0.1.0
+Version: 0.1.11
 Summary: A Python library for parsing BADC-CSV files from the MIDAS Open dataset
 Author-email: TempoTerra <vanuan+midasparser@gmail.com>
 Project-URL: Bug Tracker, https://github.com/tempoterra/midas_open_parser/issues
 Project-URL: Documentation, https://tempoterra.github.io/midas_open_parser
 Project-URL: Source Code, https://github.com/tempoterra/midas_open_parser
 Keywords: atmospheric-science,midas-open,badc-csv,parser,environmental-data
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,17 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # MIDAS Open parser
 
+[![PyPI Version](https://img.shields.io/pypi/v/midas-open-parser)](https://pypi.org/project/midas-open-parser/)
+
+
 `midas_open_parser` is a Python library specifically designed to parse BADC-CSV files from the MIDAS Open dataset.
 
 It provides a tailored and extensible framework for handling the metadata labels and structures found in the MIDAS Open dataset.
 
 The main goal of the `midas_open_parser` project is to provide tools to ingest the MIDAS Open dataset into various destinations.
 
 ## About MIDAS Open and BADC-CSV
```

### Comparing `midas_open_parser-0.1.0/pyproject.toml` & `midas_open_parser-0.1.11/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "midas_open_parser"
-version = "0.1.0"
+version = "0.1.11"
 authors = [
     {name = "TempoTerra", email = "vanuan+midasparser@gmail.com"},
 ]
 description = "A Python library for parsing BADC-CSV files from the MIDAS Open dataset"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

