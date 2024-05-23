# Comparing `tmp/etl_m_ibrahim_khalil-0.0.1.tar.gz` & `tmp/etl_m_ibrahim_khalil-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_m_ibrahim_khalil-0.0.1.tar", max compression
+gzip compressed data, was "etl_m_ibrahim_khalil-0.0.2.tar", max compression
```

## Comparing `etl_m_ibrahim_khalil-0.0.1.tar` & `etl_m_ibrahim_khalil-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1099 2024-05-22 02:17:10.119933 etl_m_ibrahim_khalil-0.0.1/LICENSE
--rw-r--r--   0        0        0     1014 2024-05-22 02:34:58.321234 etl_m_ibrahim_khalil-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-22 02:05:12.572843 etl_m_ibrahim_khalil-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-05-22 02:05:12.572843 etl_m_ibrahim_khalil-0.0.1/src/etl_m_ibrahim_khalil/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 02:05:12.572843 etl_m_ibrahim_khalil-0.0.1/src/etl_m_ibrahim_khalil/common_utils/__init__.py
--rw-r--r--   0        0        0      824 2024-05-22 02:05:12.573843 etl_m_ibrahim_khalil-0.0.1/src/etl_m_ibrahim_khalil/common_utils/api_client.py
--rw-r--r--   0        0        0      327 2024-05-22 02:05:12.573843 etl_m_ibrahim_khalil-0.0.1/src/etl_m_ibrahim_khalil/common_utils/json_encoder.py
--rw-r--r--   0        0        0      690 2024-05-22 02:05:12.573843 etl_m_ibrahim_khalil-0.0.1/src/etl_m_ibrahim_khalil/config.py
--rw-r--r--   0        0        0        0 2024-05-22 02:05:12.573843 etl_m_ibrahim_khalil-0.0.1/src/etl_m_ibrahim_khalil/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 02:05:12.574842 etl_m_ibrahim_khalil-0.0.1/src/etl_m_ibrahim_khalil/data_sources/quotes/__init__.py
--rw-r--r--   0        0        0      195 2024-05-22 02:44:23.137767 etl_m_ibrahim_khalil-0.0.1/src/etl_m_ibrahim_khalil/data_sources/quotes/constants.py
--rw-r--r--   0        0        0     2520 2024-05-22 02:44:19.300451 etl_m_ibrahim_khalil-0.0.1/src/etl_m_ibrahim_khalil/data_sources/quotes/extractor.py
--rw-r--r--   0        0        0     1899 2024-05-22 02:05:12.575842 etl_m_ibrahim_khalil-0.0.1/src/etl_m_ibrahim_khalil/data_sources/quotes/normalizer.py
--rw-r--r--   0        0        0        0 2024-05-22 02:05:12.575842 etl_m_ibrahim_khalil-0.0.1/src/etl_m_ibrahim_khalil/data_sources/quotes/transformer.py
--rw-r--r--   0        0        0      480 2024-05-22 02:43:29.710740 etl_m_ibrahim_khalil-0.0.1/src/etl_m_ibrahim_khalil/models.py
--rw-r--r--   0        0        0     2094 2024-05-22 02:42:47.195412 etl_m_ibrahim_khalil-0.0.1/src/etl_m_ibrahim_khalil/supabase_repository.py
--rw-r--r--   0        0        0     1007 1970-01-01 00:00:00.000000 etl_m_ibrahim_khalil-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-22 02:05:12.572843 etl_m_ibrahim_khalil-0.0.2/etl_m_ibrahim_khalil/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 02:05:12.572843 etl_m_ibrahim_khalil-0.0.2/etl_m_ibrahim_khalil/common_utils/__init__.py
+-rw-r--r--   0        0        0      824 2024-05-22 02:05:12.573843 etl_m_ibrahim_khalil-0.0.2/etl_m_ibrahim_khalil/common_utils/api_client.py
+-rw-r--r--   0        0        0      327 2024-05-22 02:05:12.573843 etl_m_ibrahim_khalil-0.0.2/etl_m_ibrahim_khalil/common_utils/json_encoder.py
+-rw-r--r--   0        0        0      690 2024-05-22 02:05:12.573843 etl_m_ibrahim_khalil-0.0.2/etl_m_ibrahim_khalil/config.py
+-rw-r--r--   0        0        0        0 2024-05-22 02:05:12.573843 etl_m_ibrahim_khalil-0.0.2/etl_m_ibrahim_khalil/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 02:05:12.574842 etl_m_ibrahim_khalil-0.0.2/etl_m_ibrahim_khalil/data_sources/quotes/__init__.py
+-rw-r--r--   0        0        0      195 2024-05-23 12:24:23.914414 etl_m_ibrahim_khalil-0.0.2/etl_m_ibrahim_khalil/data_sources/quotes/constants.py
+-rw-r--r--   0        0        0     2520 2024-05-22 02:44:19.300451 etl_m_ibrahim_khalil-0.0.2/etl_m_ibrahim_khalil/data_sources/quotes/extractor.py
+-rw-r--r--   0        0        0     1933 2024-05-23 13:31:23.313345 etl_m_ibrahim_khalil-0.0.2/etl_m_ibrahim_khalil/data_sources/quotes/normalizer.py
+-rw-r--r--   0        0        0        0 2024-05-22 02:05:12.575842 etl_m_ibrahim_khalil-0.0.2/etl_m_ibrahim_khalil/data_sources/quotes/transformer.py
+-rw-r--r--   0        0        0      480 2024-05-22 02:43:29.710740 etl_m_ibrahim_khalil-0.0.2/etl_m_ibrahim_khalil/models.py
+-rw-r--r--   0        0        0     2094 2024-05-23 06:39:57.502266 etl_m_ibrahim_khalil-0.0.2/etl_m_ibrahim_khalil/supabase_repository.py
+-rw-r--r--   0        0        0     1099 2024-05-22 02:17:10.119933 etl_m_ibrahim_khalil-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1014 2024-05-23 13:36:57.677815 etl_m_ibrahim_khalil-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-22 02:05:12.572843 etl_m_ibrahim_khalil-0.0.2/README.md
+-rw-r--r--   0        0        0     1007 1970-01-01 00:00:00.000000 etl_m_ibrahim_khalil-0.0.2/PKG-INFO
```

### Comparing `etl_m_ibrahim_khalil-0.0.1/LICENSE` & `etl_m_ibrahim_khalil-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `etl_m_ibrahim_khalil-0.0.1/pyproject.toml` & `etl_m_ibrahim_khalil-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "etl-m-ibrahim-khalil"
-version = "0.0.1"
+version = "0.0.2"
 description = "A simple etl package to extract data from a website and load it to a database"
 authors = [
     "Md Ibrahim Khalil <bsse1009@iit.du.ac.bd>"
 ]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/m-ibrahim-khalil/ETL"
```

### Comparing `etl_m_ibrahim_khalil-0.0.1/src/etl_m_ibrahim_khalil/common_utils/api_client.py` & `etl_m_ibrahim_khalil-0.0.2/etl_m_ibrahim_khalil/common_utils/api_client.py`

 * *Files identical despite different names*

### Comparing `etl_m_ibrahim_khalil-0.0.1/src/etl_m_ibrahim_khalil/config.py` & `etl_m_ibrahim_khalil-0.0.2/etl_m_ibrahim_khalil/config.py`

 * *Files identical despite different names*

### Comparing `etl_m_ibrahim_khalil-0.0.1/src/etl_m_ibrahim_khalil/data_sources/quotes/extractor.py` & `etl_m_ibrahim_khalil-0.0.2/etl_m_ibrahim_khalil/data_sources/quotes/extractor.py`

 * *Files identical despite different names*

### Comparing `etl_m_ibrahim_khalil-0.0.1/src/etl_m_ibrahim_khalil/data_sources/quotes/normalizer.py` & `etl_m_ibrahim_khalil-0.0.2/etl_m_ibrahim_khalil/data_sources/quotes/normalizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 
 import pandas as pd
 
-from etl.data_sources.quotes.constants import NORMALIZED_TABLE_NAME, RAW_FILE_PATH
-from etl.supabase_repository import SupabaseRepository
+from etl_m_ibrahim_khalil.data_sources.quotes.constants import NORMALIZED_TABLE_NAME, RAW_FILE_PATH
+from etl_m_ibrahim_khalil.supabase_repository import SupabaseRepository
 
 
 class QuotesNormalizer:
     def __init__(self, repository: SupabaseRepository) -> None:
         self._repository = repository
 
     def _transform_quotes(self, quotes_df: pd.DataFrame) -> pd.DataFrame:
```

### Comparing `etl_m_ibrahim_khalil-0.0.1/src/etl_m_ibrahim_khalil/supabase_repository.py` & `etl_m_ibrahim_khalil-0.0.2/etl_m_ibrahim_khalil/supabase_repository.py`

 * *Files identical despite different names*

### Comparing `etl_m_ibrahim_khalil-0.0.1/PKG-INFO` & `etl_m_ibrahim_khalil-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl-m-ibrahim-khalil
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple etl package to extract data from a website and load it to a database
 Home-page: https://github.com/m-ibrahim-khalil/ETL
 License: MIT
 Keywords: etl,data,extraction,transformation,loading
 Author: Md Ibrahim Khalil
 Author-email: bsse1009@iit.du.ac.bd
 Requires-Python: >=3.11,<4.0
```

