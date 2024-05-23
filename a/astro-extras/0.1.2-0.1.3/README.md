# Comparing `tmp/astro_extras-0.1.2.tar.gz` & `tmp/astro_extras-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_extras-0.1.2.tar", last modified: Wed May 22 09:07:13 2024, max compression
+gzip compressed data, was "astro_extras-0.1.3.tar", last modified: Wed May 22 14:02:24 2024, max compression
```

## Comparing `astro_extras-0.1.2.tar` & `astro_extras-0.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 09:07:13.922525 astro_extras-0.1.2/
--rw-rw-r--   0 kol       (1000) kol       (1000)     1074 2023-11-17 10:43:31.000000 astro_extras-0.1.2/LICENSE
--rw-rw-r--   0 kol       (1000) kol       (1000)       24 2023-10-26 14:10:20.000000 astro_extras-0.1.2/MANIFEST.in
--rw-r--r--   0 kol       (1000) kol       (1000)     7920 2024-05-22 09:07:13.922525 astro_extras-0.1.2/PKG-INFO
--rw-rw-r--   0 kol       (1000) kol       (1000)     7444 2023-11-20 09:59:52.000000 astro_extras-0.1.2/README.md
--rw-rw-r--   0 kol       (1000) kol       (1000)      352 2023-10-26 14:10:20.000000 astro_extras-0.1.2/pyproject.toml
--rw-rw-r--   0 kol       (1000) kol       (1000)      288 2024-05-22 07:52:04.000000 astro_extras-0.1.2/requirements.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)       38 2024-05-22 09:07:13.922525 astro_extras-0.1.2/setup.cfg
--rw-rw-r--   0 kol       (1000) kol       (1000)     1193 2024-05-22 08:53:58.000000 astro_extras-0.1.2/setup.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 09:07:13.918525 astro_extras-0.1.2/src/
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 09:07:13.918525 astro_extras-0.1.2/src/astro_extras/
--rw-rw-r--   0 kol       (1000) kol       (1000)     1206 2024-05-22 08:53:06.000000 astro_extras-0.1.2/src/astro_extras/__init__.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 09:07:13.918525 astro_extras-0.1.2/src/astro_extras/hooks/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.2/src/astro_extras/hooks/__init__.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 09:07:13.918525 astro_extras-0.1.2/src/astro_extras/operators/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.2/src/astro_extras/operators/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     3861 2024-04-06 11:05:12.000000 astro_extras-0.1.2/src/astro_extras/operators/direct.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    18221 2024-05-22 07:52:04.000000 astro_extras-0.1.2/src/astro_extras/operators/session.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    53135 2024-05-22 09:05:03.000000 astro_extras-0.1.2/src/astro_extras/operators/table.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 09:07:13.918525 astro_extras-0.1.2/src/astro_extras/sensors/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2024-04-02 07:09:42.000000 astro_extras-0.1.2/src/astro_extras/sensors/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)      659 2024-04-23 14:51:38.000000 astro_extras-0.1.2/src/astro_extras/sensors/auto.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5536 2024-04-06 11:03:48.000000 astro_extras-0.1.2/src/astro_extras/sensors/file.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 09:07:13.918525 astro_extras-0.1.2/src/astro_extras/templates/
--rw-rw-r--   0 kol       (1000) kol       (1000)      121 2024-05-22 07:52:04.000000 astro_extras-0.1.2/src/astro_extras/templates/session_close.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)      269 2024-05-22 07:52:04.000000 astro_extras-0.1.2/src/astro_extras/templates/session_open.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)      545 2024-05-22 09:04:48.000000 astro_extras-0.1.2/src/astro_extras/templates/table_actuals_select.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)      138 2024-05-22 07:52:04.000000 astro_extras-0.1.2/src/astro_extras/templates/table_timed_update.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)       81 2024-05-22 07:52:04.000000 astro_extras-0.1.2/src/astro_extras/templates/table_transfer_nosess.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)      187 2024-05-22 07:52:04.000000 astro_extras-0.1.2/src/astro_extras/templates/table_transfer_sess.sql
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 09:07:13.918525 astro_extras-0.1.2/src/astro_extras/utils/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.2/src/astro_extras/utils/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    10671 2024-05-02 14:17:47.000000 astro_extras-0.1.2/src/astro_extras/utils/data_compare.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1675 2024-03-11 13:15:59.000000 astro_extras-0.1.2/src/astro_extras/utils/datetime_local.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     3707 2024-05-22 07:52:04.000000 astro_extras-0.1.2/src/astro_extras/utils/postgres_sql.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5818 2024-05-22 07:52:04.000000 astro_extras-0.1.2/src/astro_extras/utils/template.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     4032 2024-05-22 07:52:50.000000 astro_extras-0.1.2/src/astro_extras/utils/utils.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 09:07:13.922525 astro_extras-0.1.2/src/astro_extras.egg-info/
--rw-r--r--   0 kol       (1000) kol       (1000)     7920 2024-05-22 09:07:13.000000 astro_extras-0.1.2/src/astro_extras.egg-info/PKG-INFO
--rw-rw-r--   0 kol       (1000) kol       (1000)     1188 2024-05-22 09:07:13.000000 astro_extras-0.1.2/src/astro_extras.egg-info/SOURCES.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)        1 2024-05-22 09:07:13.000000 astro_extras-0.1.2/src/astro_extras.egg-info/dependency_links.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)      139 2024-05-22 09:07:13.000000 astro_extras-0.1.2/src/astro_extras.egg-info/requires.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)       13 2024-05-22 09:07:13.000000 astro_extras-0.1.2/src/astro_extras.egg-info/top_level.txt
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 09:07:13.922525 astro_extras-0.1.2/tests/
--rw-rw-r--   0 kol       (1000) kol       (1000)     4172 2023-11-17 09:41:29.000000 astro_extras-0.1.2/tests/test_session.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    28649 2024-05-22 07:52:04.000000 astro_extras-0.1.2/tests/test_table.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1295 2023-11-17 09:42:18.000000 astro_extras-0.1.2/tests/test_templates.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5772 2024-05-02 14:33:06.000000 astro_extras-0.1.2/tests/test_utils.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 14:02:24.512502 astro_extras-0.1.3/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1074 2023-11-17 10:43:31.000000 astro_extras-0.1.3/LICENSE
+-rw-rw-r--   0 kol       (1000) kol       (1000)       24 2023-10-26 14:10:20.000000 astro_extras-0.1.3/MANIFEST.in
+-rw-r--r--   0 kol       (1000) kol       (1000)     7920 2024-05-22 14:02:24.512502 astro_extras-0.1.3/PKG-INFO
+-rw-rw-r--   0 kol       (1000) kol       (1000)     7444 2023-11-20 09:59:52.000000 astro_extras-0.1.3/README.md
+-rw-rw-r--   0 kol       (1000) kol       (1000)      352 2023-10-26 14:10:20.000000 astro_extras-0.1.3/pyproject.toml
+-rw-rw-r--   0 kol       (1000) kol       (1000)      288 2024-05-22 07:52:04.000000 astro_extras-0.1.3/requirements.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)       38 2024-05-22 14:02:24.512502 astro_extras-0.1.3/setup.cfg
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1193 2024-05-22 11:56:41.000000 astro_extras-0.1.3/setup.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 14:02:24.504502 astro_extras-0.1.3/src/
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 14:02:24.504502 astro_extras-0.1.3/src/astro_extras/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1206 2024-05-22 11:56:32.000000 astro_extras-0.1.3/src/astro_extras/__init__.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 14:02:24.504502 astro_extras-0.1.3/src/astro_extras/hooks/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.3/src/astro_extras/hooks/__init__.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 14:02:24.508502 astro_extras-0.1.3/src/astro_extras/operators/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.3/src/astro_extras/operators/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     3861 2024-04-06 11:05:12.000000 astro_extras-0.1.3/src/astro_extras/operators/direct.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    18221 2024-05-22 07:52:04.000000 astro_extras-0.1.3/src/astro_extras/operators/session.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    54553 2024-05-22 13:08:41.000000 astro_extras-0.1.3/src/astro_extras/operators/table.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 14:02:24.508502 astro_extras-0.1.3/src/astro_extras/sensors/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2024-04-02 07:09:42.000000 astro_extras-0.1.3/src/astro_extras/sensors/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)      659 2024-04-23 14:51:38.000000 astro_extras-0.1.3/src/astro_extras/sensors/auto.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5536 2024-04-06 11:03:48.000000 astro_extras-0.1.3/src/astro_extras/sensors/file.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 14:02:24.508502 astro_extras-0.1.3/src/astro_extras/templates/
+-rw-rw-r--   0 kol       (1000) kol       (1000)      121 2024-05-22 07:52:04.000000 astro_extras-0.1.3/src/astro_extras/templates/session_close.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      269 2024-05-22 07:52:04.000000 astro_extras-0.1.3/src/astro_extras/templates/session_open.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      545 2024-05-22 09:04:48.000000 astro_extras-0.1.3/src/astro_extras/templates/table_actuals_select.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      138 2024-05-22 07:52:04.000000 astro_extras-0.1.3/src/astro_extras/templates/table_timed_update.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)       81 2024-05-22 07:52:04.000000 astro_extras-0.1.3/src/astro_extras/templates/table_transfer_nosess.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      187 2024-05-22 07:52:04.000000 astro_extras-0.1.3/src/astro_extras/templates/table_transfer_sess.sql
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 14:02:24.508502 astro_extras-0.1.3/src/astro_extras/utils/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.3/src/astro_extras/utils/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    10671 2024-05-02 14:17:47.000000 astro_extras-0.1.3/src/astro_extras/utils/data_compare.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1675 2024-03-11 13:15:59.000000 astro_extras-0.1.3/src/astro_extras/utils/datetime_local.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     3707 2024-05-22 07:52:04.000000 astro_extras-0.1.3/src/astro_extras/utils/postgres_sql.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5818 2024-05-22 07:52:04.000000 astro_extras-0.1.3/src/astro_extras/utils/template.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     4032 2024-05-22 07:52:50.000000 astro_extras-0.1.3/src/astro_extras/utils/utils.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 14:02:24.512502 astro_extras-0.1.3/src/astro_extras.egg-info/
+-rw-r--r--   0 kol       (1000) kol       (1000)     7920 2024-05-22 14:02:24.000000 astro_extras-0.1.3/src/astro_extras.egg-info/PKG-INFO
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1188 2024-05-22 14:02:24.000000 astro_extras-0.1.3/src/astro_extras.egg-info/SOURCES.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)        1 2024-05-22 14:02:24.000000 astro_extras-0.1.3/src/astro_extras.egg-info/dependency_links.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)      139 2024-05-22 14:02:24.000000 astro_extras-0.1.3/src/astro_extras.egg-info/requires.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)       13 2024-05-22 14:02:24.000000 astro_extras-0.1.3/src/astro_extras.egg-info/top_level.txt
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 14:02:24.512502 astro_extras-0.1.3/tests/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     4172 2023-11-17 09:41:29.000000 astro_extras-0.1.3/tests/test_session.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    28649 2024-05-22 07:52:04.000000 astro_extras-0.1.3/tests/test_table.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1295 2023-11-17 09:42:18.000000 astro_extras-0.1.3/tests/test_templates.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5772 2024-05-02 14:33:06.000000 astro_extras-0.1.3/tests/test_utils.py
```

### Comparing `astro_extras-0.1.2/LICENSE` & `astro_extras-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.2/PKG-INFO` & `astro_extras-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_extras
-Version: 0.1.2
+Version: 0.1.3
 Summary: Additional Astro SDK operators
 Home-page: https://github.com/skolchin/astro-extras
 Author: Kol
 Author-email: skolchin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
```

### Comparing `astro_extras-0.1.2/README.md` & `astro_extras-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.2/setup.py` & `astro_extras-0.1.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.readlines()
 
 setuptools.setup(
     name="astro_extras",
-    version="0.1.2",
+    version="0.1.3",
     author="Kol",
     author_email="skolchin@gmail.com",
     description="Additional Astro SDK operators",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/skolchin/astro-extras",
     classifiers=[
```

### Comparing `astro_extras-0.1.2/src/astro_extras/__init__.py` & `astro_extras-0.1.3/src/astro_extras/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Astro SDK Extras project
 # (c) kol, 2023-2024
 
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 
 from .operators.session import (
     open_session, 
     close_session,
     ETLSession,
     get_current_session,
     get_session_period,
```

### Comparing `astro_extras-0.1.2/src/astro_extras/operators/direct.py` & `astro_extras-0.1.3/src/astro_extras/operators/direct.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.2/src/astro_extras/operators/session.py` & `astro_extras-0.1.3/src/astro_extras/operators/session.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.2/src/astro_extras/operators/table.py` & `astro_extras-0.1.3/src/astro_extras/operators/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Astro SDK Extras project
 # (c) kol, 2023-2024
 
 """ Table operations """
 
 import logging
-import pandas as pd
 import warnings
-from sqlalchemy import text, Table as SqlaTable
+import numpy as np
+import pandas as pd
+from sqlalchemy import text, Table as SqlaTable, Integer, BigInteger, SmallInteger
 from sqlalchemy.engine.base import Connection as SqlaConnection
 
 from airflow.models.dag import DagContext
 from airflow.utils.context import Context
 from airflow.models.xcom_arg import XComArg
 from airflow.utils.task_group import TaskGroup
 from airflow.exceptions import AirflowFailException
@@ -26,15 +27,15 @@
 from ..utils.utils import ensure_table, schedule_ops, is_same_database_uri, adjust_table_name_case
 from ..utils.template import get_template, get_template_file, get_predefined_template
 from ..utils.data_compare import compare_datasets, compare_timed_dict
 from ..utils.postgres_sql import postgres_merge_tables
 
 from typing import Iterable, Type
 
-TOSQL_CHUNK_SIZE: int = 100000
+DEFAULT_CHUNK_SIZE: int = 10000
 """ Chunk size for `pd.to_sql()` calls. Set to value lesser than `DEFAULT_CHUNK_SIZE` in Astro SDK to avoid memory overload """
 
 class TableTransfer(GenericTransfer):
     """
     Table transfer operator to be used within `transfer_table` function.
     Implements 'bulk' data transfer without any extra conditioning.
     """
@@ -59,28 +60,32 @@
 
     destination: BaseTable
     """ Destination table object """
 
     destination_table: str
     """ Destination table fully-qualified name """
 
-    session: ETLSession | XComArg | None = None
+    session: ETLSession | XComArg | None
     """ ETL Session. Use `ensure_session` to cast to proper session type """
 
-    in_memory_transfer: bool = True
+    in_memory_transfer: bool
     """ Flag to use in-memory transfer (othewise it would be Airflow's cursor-based, which is several times slower) """
 
+    chunk_size: int
+    """ Chunk size for `pd.to_sql() calls """
+
     def __init__(
         self,
         *,
         source_table: BaseTable,
         destination_table: BaseTable,
         session: ETLSession | None = None,
         in_memory_transfer: bool = False,
         proper_case: bool = False,
+        chunk_size: int | None = DEFAULT_CHUNK_SIZE,
         **kwargs,
     ) -> None:
 
         # source and target databases
         self.source_db = create_database(source_table.conn_id)
         self.dest_db = create_database(destination_table.conn_id)
 
@@ -109,14 +114,15 @@
                          destination_table=self.dest_db.get_table_qualified_name(self.destination),
                          source_conn_id=self.source.conn_id,
                          destination_conn_id=self.destination.conn_id,
                          **kwargs)
 
         self.session = session
         self.in_memory_transfer = in_memory_transfer
+        self.chunk_size = chunk_size
 
         # flag to prevent multiple _pre_execute() calls
         self._pre_execute_called: bool = False
 
         # statistics for lineage
         self._row_count: int = 0
 
@@ -138,15 +144,15 @@
 
     def _pre_execute(self, context: Context):
         """ Internal - run before execution """
 
         if self._pre_execute_called:
             return
 
-        # Set debug level logging if requestedupon DAG start
+        # Set debug level logging if requested upon DAG start
         # Config is: {..., "debug": true}
         assert 'dag_run' in context
         if context['dag_run'].conf.get('debug'):
             self.log.setLevel(logging.DEBUG)
             logging.getLogger('airflow.task').setLevel(logging.DEBUG)
             self.log.debug('Log level set to DEBUG')
 
@@ -181,34 +187,58 @@
             raise AirflowFailException(f'Table {self.destination_table} does not exist on {self.destination_conn_id}')
         for c in dest_sqla_table.columns:
             self.destination.columns.append(c)
         self.log.info(f'Table {self.destination_table} columns: {",".join([f"{c.name} {c.type}" for c in self.destination.columns])}')
 
         self._pre_execute_called = True
 
+    def _adjust_dtypes(self, data: pd.DataFrame, table: BaseTable) -> pd.DataFrame:
+        """ Checks whether `data` column dtypes match given `table` ones and reset them to proper type.
+        This could happen if, for example, source has nulls in `int` columns which would have `float` type in dataframe.
+        """
+
+        for col in table.columns:
+            if col.name not in data.columns:
+                self.log.warning(f'Column {col.name} of table {table.name} was not found in dataset')
+                continue
+
+            match col.type:
+                case Integer() | SmallInteger() | BigInteger() if data.dtypes[col.name] == 'float':
+                    self.log.info(f'Correcting column {col.name} dtype from `float` to `int`')
+                    data[col.name] = data[col.name].astype('Int64')
+
+                case _:
+                    pass
+
+        return data
+
     def execute(self, context: Context):
         """ Execute operator """
         self._pre_execute(context)
         if not self.in_memory_transfer:
             return super().execute(context)
         
         # upload source data to memory (might need to use chunks)
+        self.log.info('Using in-memory transfer')
         data = pd.read_sql(self.sql, self.source_db.connection)
         if data is None or data.empty:
             self.log.info('No data to transfer')
-        else:
-            # save to target table
-            # TODO: cast integer NaNs to proper types
-            self._row_count = len(data)
-            self.log.info(f'{self._row_count} records to be transferred')
-            self.dest_db.load_pandas_dataframe_to_table(
-                data, 
-                self.destination, 
-                if_exists='append',
-                chunksize=TOSQL_CHUNK_SIZE)
+            return
+
+        # Adjust dtypes
+        data = self._adjust_dtypes(data, self.destination)
+
+        # save to target table
+        self._row_count = len(data)
+        self.log.info(f'{self._row_count} records to be transferred')
+        self.dest_db.load_pandas_dataframe_to_table(
+            data, 
+            self.destination, 
+            if_exists='append',
+            chunk_size=self.chunk_size)
 
     def get_openlineage_facets_on_complete(self, task_instance):  # skipcq: PYL-W0613
         """
         Collect the input, output, job and run facets for DataframeOperator
         """
         from airflow.providers.openlineage.extractors.base import OperatorLineage
         from openlineage.client.run import Dataset
@@ -351,22 +381,22 @@
                 data.insert(0, '_deleted', deleted)
                 data.insert(0, '_modified', modified)
                 data.insert(0, 'session_id', self.session.session_id)
             else:
                 data['_modified'] = modified
                 data['_deleted'] = deleted
 
-            self.log.info(f'Saving {data.shape[0]} {category} records to {self.destination_table}')
+            self.log.info(f'Saving {data.shape[0]} {category} records to {self.destination_table} (chunk size is {self.chunk_size})')
             data.to_sql(
                 self.destination.name,
                 con=conn,
                 schema=self.destination.metadata.schema if self.destination.metadata else None,
                 if_exists='append',
                 method='multi',
-                chunksize=TOSQL_CHUNK_SIZE,
+                chunksize=self.chunk_size,
                 index=False,
             )
             self._row_count += len(data)
 
     def execute(self, context: Context):
         """ Execute operator """
 
@@ -382,19 +412,20 @@
         if self.destination.columns[n_col].name.lower() != '_modified':
             raise AirflowFailException(f'Invalid ODS table {self.destination_table} structure: `_modified` column missing or at improper place')
         if self.destination.columns[n_col+1].name.lower() != '_deleted':
             raise AirflowFailException(f'Invalid ODS table {self.destination_table} structure: `_deleted` column missing or at improper place')
 
         # compare datasets and save delta frames to target (new/modified/deleted)
         self._row_count = 0
-        with self.source_db.connection as src_conn, self.dest_db.connection as dest_conn, dest_conn.begin():
+        with self.source_db.connection as src_conn, self.dest_db.connection as dest_conn:
             dfn, dfm, dfd = self._compare_datasets(src_conn, dest_conn, stop_on_first_diff=False)
-            self._save_data(dfn, dest_conn, pd.Timestamp.utcnow(), pd.NaT, 'new')
-            self._save_data(dfm, dest_conn, pd.Timestamp.utcnow(), pd.NaT, 'modified')
-            self._save_data(dfd, dest_conn, pd.Timestamp.utcnow(), pd.Timestamp.utcnow(), 'deleted')
+            with dest_conn.begin():
+                self._save_data(dfn, dest_conn, pd.Timestamp.utcnow(), pd.NaT, 'new')
+                self._save_data(dfm, dest_conn, pd.Timestamp.utcnow(), pd.NaT, 'modified')
+                self._save_data(dfd, dest_conn, pd.Timestamp.utcnow(), pd.Timestamp.utcnow(), 'deleted')
 
 class ActualsTableTransfer(TableTransfer):
     """
     Table transfer operator to be used within `transfer_actuals_table` function.
     Source and target table must have `_deleted` attribute of `timestamp` or `timestamptz` type.
     """
 
@@ -463,44 +494,44 @@
         sql = self.sql.replace('t.id', id_cols_str).replace('t.*', all_cols_str)
         self.log.info(f'Source extraction SQL:\n{sql}')
 
         # Check whether the hooks point to the same database
         same_db = is_same_database_uri(self.source_db.hook.get_uri(), self.dest_db.hook.get_uri())
 
         # Update/merge
-        with self.source_db.connection as src_conn, self.dest_db.connection as dest_conn, dest_conn.begin():
+        with self.source_db.connection as src_conn, self.dest_db.connection as dest_conn:
             if same_db:
                 # Source and destination tables are in the same database, 
                 self.log.info(f'Source and destination tables are in the same database')
+                with dest_conn.begin():
+                    # If `replace_data` is set, purge target table
+                    if self.replace_data:
+                        dest_conn.execute(text(f'delete from {self.destination_table}'))
 
-                # If `replace_data` is set, purge target table
-                if self.replace_data:
-                    dest_conn.execute(text(f'delete from {self.destination_table}'))
-
-                # Merge into target table directly from sql
-                self._row_count = postgres_merge_tables(
-                    conn=dest_conn,
-                    source_table=None,
-                    target_table=self.destination,
-                    source_to_target_columns_map=col_map,
-                    target_conflict_columns=id_cols,
-                    source_sql=sql,
-                    if_conflicts='update'
-                )
-                self.log.info(f'{self._row_count} records transferred')
+                    # Merge into target table directly using source sql
+                    self._row_count = postgres_merge_tables(
+                        conn=dest_conn,
+                        source_table=None,
+                        target_table=self.destination,
+                        source_to_target_columns_map=col_map,
+                        target_conflict_columns=id_cols,
+                        source_sql=sql,
+                        if_conflicts='update'
+                    )
+                    self.log.info(f'{self._row_count} records transferred')
 
             else:
                 # Source and destination tables are in different databases
                 temp_table = Table(metadata=self.destination.metadata, temp=True)
                 self.log.info(f'Source and destination tables are in different databases, transferring via temporary table')
 
                 # Load data from source table
                 data = pd.read_sql(sql, src_conn)
                 if data is None or data.empty:
-                    self.log.info('No records to transfer')
+                    self.log.info('No data to transfer')
                     return
                 
                 if self.session:
                     data['session_id'] = self.session.session_id
                     col_map['session_id'] = 'session_id'
 
                 # Temp table has to be created 1st, otherwise it might be column types mismatch
@@ -511,33 +542,34 @@
                     # Save data to temporary table
                     data.to_sql(
                         temp_table.name,
                         con=dest_conn,
                         schema=temp_table.metadata.schema if temp_table.metadata else None,
                         if_exists='append',
                         method='multi',
-                        chunksize=TOSQL_CHUNK_SIZE,
+                        chunksize=self.chunk_size,
                         index=False,
                     )
 
-                    # If `replace_data` is set, purge target table
-                    if self.replace_data:
-                        dest_conn.execute(text(f'delete from {self.destination_table}'))
-
-                    # Merge temporary and target tables
-                    self.log.info(f'Merging from {self.dest_db.get_table_qualified_name(temp_table)} to {self.destination_table}')
-                    self._row_count = postgres_merge_tables(
-                        conn=dest_conn,
-                        source_table=temp_table,
-                        target_table=self.destination,
-                        source_to_target_columns_map=col_map,
-                        target_conflict_columns=id_cols,
-                        if_conflicts='update'
-                    )
-                    self.log.info(f'{self._row_count} records transferred')
+                    with dest_conn.begin():
+                        # If `replace_data` is set, purge target table
+                        if self.replace_data:
+                            dest_conn.execute(text(f'delete from {self.destination_table}'))
+
+                        # Merge temporary and target tables
+                        self.log.info(f'Merging from {self.dest_db.get_table_qualified_name(temp_table)} to {self.destination_table}')
+                        self._row_count = postgres_merge_tables(
+                            conn=dest_conn,
+                            source_table=temp_table,
+                            target_table=self.destination,
+                            source_to_target_columns_map=col_map,
+                            target_conflict_columns=id_cols,
+                            if_conflicts='update'
+                        )
+                        self.log.info(f'{self._row_count} records transferred')
 
                 finally:
                     if not self.keep_temp_table:
                         self.dest_db.drop_table(temp_table)
 
 class TimedTableTransfer(ChangedTableTransfer):
     """
@@ -577,15 +609,15 @@
             if df_opening is not None and not df_opening.empty:
                 df_opening.to_sql(
                     self.destination.name,
                     con=dest_conn,
                     schema=self.destination.metadata.schema if self.destination.metadata else None,
                     if_exists='append',
                     method='multi',
-                    chunksize=TOSQL_CHUNK_SIZE,
+                    chunksize=self.chunk_size,
                     index=False,
                 )
 
 
 class CompareTableOperator(ChangedTableTransfer):
     """
     Table comparsion operator to be used within `compare_table` function.
```

### Comparing `astro_extras-0.1.2/src/astro_extras/sensors/auto.py` & `astro_extras-0.1.3/src/astro_extras/sensors/auto.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.2/src/astro_extras/sensors/file.py` & `astro_extras-0.1.3/src/astro_extras/sensors/file.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.2/src/astro_extras/templates/table_actuals_select.sql` & `astro_extras-0.1.3/src/astro_extras/templates/table_actuals_select.sql`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.2/src/astro_extras/utils/data_compare.py` & `astro_extras-0.1.3/src/astro_extras/utils/data_compare.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.2/src/astro_extras/utils/datetime_local.py` & `astro_extras-0.1.3/src/astro_extras/utils/datetime_local.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.2/src/astro_extras/utils/postgres_sql.py` & `astro_extras-0.1.3/src/astro_extras/utils/postgres_sql.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.2/src/astro_extras/utils/template.py` & `astro_extras-0.1.3/src/astro_extras/utils/template.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.2/src/astro_extras/utils/utils.py` & `astro_extras-0.1.3/src/astro_extras/utils/utils.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.2/src/astro_extras.egg-info/PKG-INFO` & `astro_extras-0.1.3/src/astro_extras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_extras
-Version: 0.1.2
+Version: 0.1.3
 Summary: Additional Astro SDK operators
 Home-page: https://github.com/skolchin/astro-extras
 Author: Kol
 Author-email: skolchin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
```

### Comparing `astro_extras-0.1.2/src/astro_extras.egg-info/SOURCES.txt` & `astro_extras-0.1.3/src/astro_extras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.2/tests/test_session.py` & `astro_extras-0.1.3/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.2/tests/test_table.py` & `astro_extras-0.1.3/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.2/tests/test_templates.py` & `astro_extras-0.1.3/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.2/tests/test_utils.py` & `astro_extras-0.1.3/tests/test_utils.py`

 * *Files identical despite different names*

