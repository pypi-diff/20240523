# Comparing `tmp/celus_nibbler-11.1.1.tar.gz` & `tmp/celus_nibbler-11.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celus_nibbler-11.1.1.tar", max compression
+gzip compressed data, was "celus_nibbler-11.1.2.tar", max compression
```

## Comparing `celus_nibbler-11.1.1.tar` & `celus_nibbler-11.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1057 2022-06-17 07:35:22.867507 celus_nibbler-11.1.1/LICENSE
--rw-r--r--   0        0        0      644 2024-05-02 20:46:59.314165 celus_nibbler-11.1.1/celus_nibbler/__init__.py
--rw-r--r--   0        0        0     8253 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/__main__.py
--rw-r--r--   0        0        0     5480 2023-11-22 12:21:31.240892 celus_nibbler-11.1.1/celus_nibbler/aggregator.py
--rw-r--r--   0        0        0     6946 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/conditions.py
--rw-r--r--   0        0        0     6096 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/coordinates.py
--rw-r--r--   0        0        0    14359 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/data_headers.py
--rw-r--r--   0        0        0     2117 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/definitions/__init__.py
--rw-r--r--   0        0        0     1717 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/definitions/base.py
--rw-r--r--   0        0        0     4238 2023-10-27 12:46:00.516284 celus_nibbler-11.1.1/celus_nibbler/definitions/celus_format.py
--rw-r--r--   0        0        0    15825 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/definitions/counter.py
--rw-r--r--   0        0        0     4561 2023-10-27 12:46:00.520284 celus_nibbler-11.1.1/celus_nibbler/definitions/date_based.py
--rw-r--r--   0        0        0     4472 2023-10-27 12:46:00.520284 celus_nibbler-11.1.1/celus_nibbler/definitions/date_metric_based.py
--rw-r--r--   0        0        0     4726 2023-10-27 12:46:00.520284 celus_nibbler-11.1.1/celus_nibbler/definitions/generic.py
--rw-r--r--   0        0        0     4381 2023-10-27 12:46:00.520284 celus_nibbler-11.1.1/celus_nibbler/definitions/metric_based.py
--rw-r--r--   0        0        0    14563 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/eat_and_poop.py
--rw-r--r--   0        0        0     6074 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/errors.py
--rw-r--r--   0        0        0     2785 2022-11-01 15:22:27.669687 celus_nibbler-11.1.1/celus_nibbler/parsers/__init__.py
--rw-r--r--   0        0        0    15190 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/parsers/base.py
--rw-r--r--   0        0        0    13122 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/parsers/counter/__init__.py
--rw-r--r--   0        0        0    11529 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/parsers/counter/c4.py
--rw-r--r--   0        0        0    10694 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/parsers/counter/c5.py
--rw-r--r--   0        0        0     3803 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/parsers/counter/c5json.py
--rw-r--r--   0        0        0      156 2023-08-15 12:26:51.461995 celus_nibbler-11.1.1/celus_nibbler/parsers/dynamic.py
--rw-r--r--   0        0        0        0 2022-10-21 20:55:53.099727 celus_nibbler-11.1.1/celus_nibbler/parsers/non_counter/__init__.py
--rw-r--r--   0        0        0      194 2022-11-04 15:01:01.540828 celus_nibbler-11.1.1/celus_nibbler/parsers/non_counter/base.py
--rw-r--r--   0        0        0     5683 2023-07-29 08:57:05.293613 celus_nibbler-11.1.1/celus_nibbler/parsers/non_counter/celus_format.py
--rw-r--r--   0        0        0      322 2023-07-19 09:21:05.347414 celus_nibbler-11.1.1/celus_nibbler/parsers/non_counter/date_based.py
--rw-r--r--   0        0        0     2547 2023-07-19 09:21:05.347414 celus_nibbler-11.1.1/celus_nibbler/parsers/non_counter/date_metric_based.py
--rw-r--r--   0        0        0      774 2023-07-19 09:21:05.347414 celus_nibbler-11.1.1/celus_nibbler/parsers/non_counter/generic.py
--rw-r--r--   0        0        0     2478 2023-07-19 09:21:05.347414 celus_nibbler-11.1.1/celus_nibbler/parsers/non_counter/metric_based.py
--rw-r--r--   0        0        0    14940 2024-05-02 20:46:59.322165 celus_nibbler-11.1.1/celus_nibbler/reader.py
--rw-r--r--   0        0        0    15482 2024-05-02 20:46:59.322165 celus_nibbler-11.1.1/celus_nibbler/sources.py
--rw-r--r--   0        0        0     1624 2023-10-27 12:46:00.524284 celus_nibbler-11.1.1/celus_nibbler/utils.py
--rw-r--r--   0        0        0     9468 2024-05-02 20:46:59.322165 celus_nibbler-11.1.1/celus_nibbler/validators.py
--rw-r--r--   0        0        0     3311 2024-05-02 20:47:55.618084 celus_nibbler-11.1.1/pyproject.toml
--rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 celus_nibbler-11.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1057 2022-06-17 07:35:22.867507 celus_nibbler-11.1.2/LICENSE
+-rw-r--r--   0        0        0      644 2024-05-10 12:09:17.061009 celus_nibbler-11.1.2/celus_nibbler/__init__.py
+-rw-r--r--   0        0        0     8253 2024-05-10 12:09:17.061009 celus_nibbler-11.1.2/celus_nibbler/__main__.py
+-rw-r--r--   0        0        0     5480 2023-11-22 12:21:31.240892 celus_nibbler-11.1.2/celus_nibbler/aggregator.py
+-rw-r--r--   0        0        0     6946 2024-05-10 12:09:17.061009 celus_nibbler-11.1.2/celus_nibbler/conditions.py
+-rw-r--r--   0        0        0     6096 2024-05-10 12:09:17.061009 celus_nibbler-11.1.2/celus_nibbler/coordinates.py
+-rw-r--r--   0        0        0    14359 2024-05-10 12:09:17.061009 celus_nibbler-11.1.2/celus_nibbler/data_headers.py
+-rw-r--r--   0        0        0     2117 2024-05-10 12:09:17.061009 celus_nibbler-11.1.2/celus_nibbler/definitions/__init__.py
+-rw-r--r--   0        0        0     1717 2024-05-10 12:09:17.061009 celus_nibbler-11.1.2/celus_nibbler/definitions/base.py
+-rw-r--r--   0        0        0     4238 2023-10-27 12:46:00.516284 celus_nibbler-11.1.2/celus_nibbler/definitions/celus_format.py
+-rw-r--r--   0        0        0    15825 2024-05-10 12:09:17.061009 celus_nibbler-11.1.2/celus_nibbler/definitions/counter.py
+-rw-r--r--   0        0        0     4561 2023-10-27 12:46:00.520284 celus_nibbler-11.1.2/celus_nibbler/definitions/date_based.py
+-rw-r--r--   0        0        0     4472 2023-10-27 12:46:00.520284 celus_nibbler-11.1.2/celus_nibbler/definitions/date_metric_based.py
+-rw-r--r--   0        0        0     4726 2023-10-27 12:46:00.520284 celus_nibbler-11.1.2/celus_nibbler/definitions/generic.py
+-rw-r--r--   0        0        0     4381 2023-10-27 12:46:00.520284 celus_nibbler-11.1.2/celus_nibbler/definitions/metric_based.py
+-rw-r--r--   0        0        0    14563 2024-05-10 12:09:17.069009 celus_nibbler-11.1.2/celus_nibbler/eat_and_poop.py
+-rw-r--r--   0        0        0     6074 2024-05-10 12:09:17.069009 celus_nibbler-11.1.2/celus_nibbler/errors.py
+-rw-r--r--   0        0        0     2785 2022-11-01 15:22:27.669687 celus_nibbler-11.1.2/celus_nibbler/parsers/__init__.py
+-rw-r--r--   0        0        0    15190 2024-05-10 12:09:17.069009 celus_nibbler-11.1.2/celus_nibbler/parsers/base.py
+-rw-r--r--   0        0        0    13122 2024-05-10 12:09:17.069009 celus_nibbler-11.1.2/celus_nibbler/parsers/counter/__init__.py
+-rw-r--r--   0        0        0    11529 2024-05-10 12:09:17.069009 celus_nibbler-11.1.2/celus_nibbler/parsers/counter/c4.py
+-rw-r--r--   0        0        0    10694 2024-05-10 12:09:17.069009 celus_nibbler-11.1.2/celus_nibbler/parsers/counter/c5.py
+-rw-r--r--   0        0        0     3803 2024-05-10 12:09:17.069009 celus_nibbler-11.1.2/celus_nibbler/parsers/counter/c5json.py
+-rw-r--r--   0        0        0      156 2023-08-15 12:26:51.461995 celus_nibbler-11.1.2/celus_nibbler/parsers/dynamic.py
+-rw-r--r--   0        0        0        0 2022-10-21 20:55:53.099727 celus_nibbler-11.1.2/celus_nibbler/parsers/non_counter/__init__.py
+-rw-r--r--   0        0        0      194 2022-11-04 15:01:01.540828 celus_nibbler-11.1.2/celus_nibbler/parsers/non_counter/base.py
+-rw-r--r--   0        0        0     5683 2023-07-29 08:57:05.293613 celus_nibbler-11.1.2/celus_nibbler/parsers/non_counter/celus_format.py
+-rw-r--r--   0        0        0      322 2023-07-19 09:21:05.347414 celus_nibbler-11.1.2/celus_nibbler/parsers/non_counter/date_based.py
+-rw-r--r--   0        0        0     2547 2023-07-19 09:21:05.347414 celus_nibbler-11.1.2/celus_nibbler/parsers/non_counter/date_metric_based.py
+-rw-r--r--   0        0        0      774 2023-07-19 09:21:05.347414 celus_nibbler-11.1.2/celus_nibbler/parsers/non_counter/generic.py
+-rw-r--r--   0        0        0     2478 2023-07-19 09:21:05.347414 celus_nibbler-11.1.2/celus_nibbler/parsers/non_counter/metric_based.py
+-rw-r--r--   0        0        0    14940 2024-05-10 12:09:17.069009 celus_nibbler-11.1.2/celus_nibbler/reader.py
+-rw-r--r--   0        0        0    15482 2024-05-10 12:09:17.069009 celus_nibbler-11.1.2/celus_nibbler/sources.py
+-rw-r--r--   0        0        0     1624 2023-10-27 12:46:00.524284 celus_nibbler-11.1.2/celus_nibbler/utils.py
+-rw-r--r--   0        0        0     9468 2024-05-10 12:09:17.069009 celus_nibbler-11.1.2/celus_nibbler/validators.py
+-rw-r--r--   0        0        0     3311 2024-05-10 12:13:52.465975 celus_nibbler-11.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 celus_nibbler-11.1.2/PKG-INFO
```

### Comparing `celus_nibbler-11.1.1/LICENSE` & `celus_nibbler-11.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/__init__.py` & `celus_nibbler-11.1.2/celus_nibbler/__init__.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/__main__.py` & `celus_nibbler-11.1.2/celus_nibbler/__main__.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/aggregator.py` & `celus_nibbler-11.1.2/celus_nibbler/aggregator.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/conditions.py` & `celus_nibbler-11.1.2/celus_nibbler/conditions.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/coordinates.py` & `celus_nibbler-11.1.2/celus_nibbler/coordinates.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/data_headers.py` & `celus_nibbler-11.1.2/celus_nibbler/data_headers.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/definitions/__init__.py` & `celus_nibbler-11.1.2/celus_nibbler/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/definitions/base.py` & `celus_nibbler-11.1.2/celus_nibbler/definitions/base.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/definitions/celus_format.py` & `celus_nibbler-11.1.2/celus_nibbler/definitions/celus_format.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/definitions/counter.py` & `celus_nibbler-11.1.2/celus_nibbler/definitions/counter.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/definitions/date_based.py` & `celus_nibbler-11.1.2/celus_nibbler/definitions/date_based.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/definitions/date_metric_based.py` & `celus_nibbler-11.1.2/celus_nibbler/definitions/date_metric_based.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/definitions/generic.py` & `celus_nibbler-11.1.2/celus_nibbler/definitions/generic.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/definitions/metric_based.py` & `celus_nibbler-11.1.2/celus_nibbler/definitions/metric_based.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/eat_and_poop.py` & `celus_nibbler-11.1.2/celus_nibbler/eat_and_poop.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/errors.py` & `celus_nibbler-11.1.2/celus_nibbler/errors.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/parsers/__init__.py` & `celus_nibbler-11.1.2/celus_nibbler/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/parsers/base.py` & `celus_nibbler-11.1.2/celus_nibbler/parsers/base.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/parsers/counter/__init__.py` & `celus_nibbler-11.1.2/celus_nibbler/parsers/counter/__init__.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/parsers/counter/c4.py` & `celus_nibbler-11.1.2/celus_nibbler/parsers/counter/c4.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/parsers/counter/c5.py` & `celus_nibbler-11.1.2/celus_nibbler/parsers/counter/c5.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/parsers/counter/c5json.py` & `celus_nibbler-11.1.2/celus_nibbler/parsers/counter/c5json.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/parsers/non_counter/celus_format.py` & `celus_nibbler-11.1.2/celus_nibbler/parsers/non_counter/celus_format.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/parsers/non_counter/date_metric_based.py` & `celus_nibbler-11.1.2/celus_nibbler/parsers/non_counter/date_metric_based.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/parsers/non_counter/generic.py` & `celus_nibbler-11.1.2/celus_nibbler/parsers/non_counter/generic.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/parsers/non_counter/metric_based.py` & `celus_nibbler-11.1.2/celus_nibbler/parsers/non_counter/metric_based.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/reader.py` & `celus_nibbler-11.1.2/celus_nibbler/reader.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/sources.py` & `celus_nibbler-11.1.2/celus_nibbler/sources.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/utils.py` & `celus_nibbler-11.1.2/celus_nibbler/utils.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/celus_nibbler/validators.py` & `celus_nibbler-11.1.2/celus_nibbler/validators.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.1/pyproject.toml` & `celus_nibbler-11.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 plugins = "pydantic.mypy"
 
 [tool.pytest.ini_options]
 testpaths = "tests/"
 
 [tool.poetry]
 name = "celus-nibbler"
-version = "11.1.1"
+version = "11.1.2"
 description = "Counter-like data reader and processor."
 authors = ["Stepan Henek <stepan@bigdigdata.com>", "Zbynek Vyhlas <zbyneksmail@gmail.com>"]
 license = "MIT"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"Topic :: Software Development :: Libraries"
 ]
@@ -44,15 +44,15 @@
 
 [tool.poetry.scripts]
 nibbler-eat = 'celus_nibbler.__main__:main'
 
 [tool.poetry.dependencies]
 python = "^3.8.9"
 
-celus-nigiri = "~2.1.0"
+celus-nigiri = "~2.2.0"
 diskcache = "~5.6.0"
 nltk = "~3.8.1"
 pydantic = "~2.6.4"
 python-dateutil = "~2.9.0"
 openpyxl = "~3.1.2"
 unidecode = "~1.3.7"
 isbnlib = "~3.10.14"
```

### Comparing `celus_nibbler-11.1.1/PKG-INFO` & `celus_nibbler-11.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: celus-nibbler
-Version: 11.1.1
+Version: 11.1.2
 Summary: Counter-like data reader and processor.
 License: MIT
 Keywords: parsing,counter5
 Author: Stepan Henek
 Author-email: stepan@bigdigdata.com
 Requires-Python: >=3.8.9,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: xls
-Requires-Dist: celus-nigiri (>=2.1.0,<2.2.0)
+Requires-Dist: celus-nigiri (>=2.2.0,<2.3.0)
 Requires-Dist: diskcache (>=5.6.0,<5.7.0)
 Requires-Dist: isbnlib (>=3.10.14,<3.11.0)
 Requires-Dist: nltk (>=3.8.1,<3.9.0)
 Requires-Dist: openpyxl (>=3.1.2,<3.2.0)
 Requires-Dist: pydantic (>=2.6.4,<2.7.0)
 Requires-Dist: python-dateutil (>=2.9.0,<2.10.0)
 Requires-Dist: typing-extensions (>=4.10.0,<4.11.0)
```

