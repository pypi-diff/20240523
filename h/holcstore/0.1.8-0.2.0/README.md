# Comparing `tmp/holcstore-0.1.8.tar.gz` & `tmp/holcstore-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holcstore-0.1.8.tar", last modified: Fri May  3 13:59:32 2024, max compression
+gzip compressed data, was "holcstore-0.2.0.tar", last modified: Thu May 23 14:49:22 2024, max compression
```

## Comparing `holcstore-0.1.8.tar` & `holcstore-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:59:32.965656 holcstore-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-03 13:59:29.000000 holcstore-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-03 13:59:29.000000 holcstore-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-03 13:59:32.965656 holcstore-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-03 13:59:29.000000 holcstore-0.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:59:32.961656 holcstore-0.1.8/holcstore/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:59:29.000000 holcstore-0.1.8/holcstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-03 13:59:29.000000 holcstore-0.1.8/holcstore/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-03 13:59:29.000000 holcstore-0.1.8/holcstore/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-03 13:59:29.000000 holcstore-0.1.8/holcstore/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-03 13:59:29.000000 holcstore-0.1.8/holcstore/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:59:32.965656 holcstore-0.1.8/holcstore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-03 13:59:32.000000 holcstore-0.1.8/holcstore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-03 13:59:32.000000 holcstore-0.1.8/holcstore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 13:59:32.000000 holcstore-0.1.8/holcstore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 13:59:32.000000 holcstore-0.1.8/holcstore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 13:59:32.000000 holcstore-0.1.8/holcstore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:59:32.961656 holcstore-0.1.8/hostore/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:59:32.965656 holcstore-0.1.8/hostore/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/migrations/0002_rename_store_testd_prm_91e86e_idx_hostore_tes_prm_897468_idx.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/migrations/0004_testdatastore_created_at.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:59:32.965656 holcstore-0.1.8/hostore/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/utils/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-03 13:59:29.000000 holcstore-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-03 13:59:32.965656 holcstore-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 13:59:29.000000 holcstore-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:49:22.965438 holcstore-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-23 14:49:19.000000 holcstore-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-23 14:49:19.000000 holcstore-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-23 14:49:22.965438 holcstore-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-23 14:49:19.000000 holcstore-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:49:22.965438 holcstore-0.2.0/holcstore/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:49:19.000000 holcstore-0.2.0/holcstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-23 14:49:19.000000 holcstore-0.2.0/holcstore/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-23 14:49:19.000000 holcstore-0.2.0/holcstore/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-23 14:49:19.000000 holcstore-0.2.0/holcstore/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-23 14:49:19.000000 holcstore-0.2.0/holcstore/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:49:22.965438 holcstore-0.2.0/holcstore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-23 14:49:22.000000 holcstore-0.2.0/holcstore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-23 14:49:22.000000 holcstore-0.2.0/holcstore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:49:22.000000 holcstore-0.2.0/holcstore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-23 14:49:22.000000 holcstore-0.2.0/holcstore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 14:49:22.000000 holcstore-0.2.0/holcstore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:49:22.965438 holcstore-0.2.0/hostore/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:49:19.000000 holcstore-0.2.0/hostore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-23 14:49:19.000000 holcstore-0.2.0/hostore/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-23 14:49:19.000000 holcstore-0.2.0/hostore/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-23 14:49:19.000000 holcstore-0.2.0/hostore/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:49:22.965438 holcstore-0.2.0/hostore/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-23 14:49:19.000000 holcstore-0.2.0/hostore/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-23 14:49:19.000000 holcstore-0.2.0/hostore/migrations/0002_rename_store_testd_prm_91e86e_idx_hostore_tes_prm_897468_idx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-23 14:49:19.000000 holcstore-0.2.0/hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-23 14:49:19.000000 holcstore-0.2.0/hostore/migrations/0004_testdatastore_created_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:49:19.000000 holcstore-0.2.0/hostore/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-05-23 14:49:19.000000 holcstore-0.2.0/hostore/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-05-23 14:49:19.000000 holcstore-0.2.0/hostore/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:49:22.965438 holcstore-0.2.0/hostore/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:49:19.000000 holcstore-0.2.0/hostore/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-05-23 14:49:19.000000 holcstore-0.2.0/hostore/utils/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-23 14:49:19.000000 holcstore-0.2.0/hostore/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-23 14:49:19.000000 holcstore-0.2.0/hostore/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-23 14:49:19.000000 holcstore-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-23 14:49:22.969438 holcstore-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-23 14:49:19.000000 holcstore-0.2.0/setup.py
```

### Comparing `holcstore-0.1.8/LICENSE` & `holcstore-0.2.0/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2024, JPierre
+Copyright (c) 2024, Jean-Pierre Lartigue
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `holcstore-0.1.8/PKG-INFO` & `holcstore-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holcstore
-Version: 0.1.8
+Version: 0.2.0
 Summary: A Django App to use a simple load curve store
 Home-page: 
 Author: Jean-Pierre Lartigue
 Author-email: 
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `holcstore-0.1.8/README.rst` & `holcstore-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.8/holcstore/settings.py` & `holcstore-0.2.0/holcstore/settings.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.8/holcstore/urls.py` & `holcstore-0.2.0/holcstore/urls.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.8/holcstore.egg-info/PKG-INFO` & `holcstore-0.2.0/holcstore.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holcstore
-Version: 0.1.8
+Version: 0.2.0
 Summary: A Django App to use a simple load curve store
 Home-page: 
 Author: Jean-Pierre Lartigue
 Author-email: 
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `holcstore-0.1.8/holcstore.egg-info/SOURCES.txt` & `holcstore-0.2.0/holcstore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.8/hostore/migrations/0001_initial.py` & `holcstore-0.2.0/hostore/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.8/hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py` & `holcstore-0.2.0/hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.8/hostore/models.py` & `holcstore-0.2.0/hostore/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import datetime as dt
 import pandas as pd
 from django.db import models
 from django.db.models import Max
 from pyarrow import BufferReader
 
 from .manager import StoreQuerySet
-from .utils.timeseries import ts_combine_first, find_constant_sequences, check_ts_completeness
+from .utils.timeseries import ts_combine_first, check_ts_completeness
 from .utils.utils import chunks
-from django.utils.timezone import now
+
 
 logger = logging.getLogger(__name__)
 
 
 class Store(models.Model):
     client_id = models.IntegerField()
     prm = models.CharField(max_length=30)
@@ -28,20 +28,22 @@
 
     class Meta:
         abstract = True
         unique_together = ('prm', 'client_id', 'version')
         indexes = [models.Index(fields=['prm', 'client_id']), ]
 
     @classmethod
-    def count(cls, client_id: int):
-        return cls.objects.filter(client_id=client_id).count()
+    def count(cls, client_id: int, custom_filters=None):
+        if custom_filters is None:
+            custom_filters = {}
+        return cls.objects.filter(client_id=client_id, **custom_filters).count()
 
     @classmethod
     def find_holes(cls, client_id: int, sd: dt.datetime, ed: dt.datetime, freq='30min', prms: List[str] = None, chunk_size=50,
-                   freq_margin=pd.Timedelta(minutes=0)) -> Dict[str, List]:
+                   freq_margin=pd.Timedelta(minutes=0), custom_filters=None) -> Dict[str, List]:
         """
         Find holes (missing data periods) for multiple prms within a specified datetime range.
 
         This method retrieves data from a database for each parameter associated with a client_id,
         checks each dataset for missing data within the specified datetime range, and identifies the start
         and end of each missing data period.
 
@@ -49,24 +51,27 @@
         :param sd: Start datetime of the range to check for holes.
         :param ed: End datetime of the range to check for holes.
         :param freq: Frequency at which the data is expected, defaulting to '30min'.
         :param prms: Optional list of prms to check; if None, all parameters for the client are checked.
         :param chunk_size: The size of chunks to break the parameter list into for batch processing.
                            This helps in managing memory and processing large datasets efficiently, defaulting to 50.
         :param freq_margin: Freq margin for null sequences
+        :param custom_filters: (optionnal) None or dict
         :return: A dictionary with prm as keys and a list of tuples (start, end) indicating
                  the missing data periods for each parameter. Start and end are included
         """
+        if custom_filters is None:
+            custom_filters = {}
         # If no prm are specified, retrieve all prm for the given client from the database
         if prms is None:
-            prms = list(cls.objects.filter(client_id=client_id).values_list('prm', flat=True))
+            prms = list(cls.objects.filter(client_id=client_id, **custom_filters).values_list('prm', flat=True))
 
         # Iterate over prms in chunks to manage memory usage and efficiency
         for prm_chunk in chunks(prms, chunk_size):
-            data_by_prm = cls.get_many_lc(prm_chunk, client_id, combined_versions=True)
+            data_by_prm = cls.get_many_lc(prm_chunk, client_id, combined_versions=True, **custom_filters)
 
             # Check each parameter's data for completeness
             for prm in prm_chunk:
                 nulls_seqs = []
                 data = data_by_prm[prm]
                 if len(data) == 0:
                     # If there's no data for a prm, the entire range is considered as a hole
@@ -77,27 +82,31 @@
                     nulls_seqs = check_ts_completeness(data[0]['data'], sd, ed, freq=freq, freq_margin=freq_margin)
 
                 # Yield the output for this prm
                 # This allows processing part by part without waiting for the entire operation to complete
                 yield prm, nulls_seqs
 
     @classmethod
-    def get_lc(cls, prm: str, client_id: int, combined_versions=True, version: int = None) -> List[Dict]:
+    def get_lc(cls, prm: str, client_id: int, combined_versions=True, version: int = None, custom_filters=None) -> List[Dict]:
         """
         Get the prm load curve
         Args:
             prm: str
             client_id: int, client's id
             combined_versions: bool, if multiple versions exists we combine them (default True)
             version: return only the selected version
+            custom_filters: (optionnal) None or dict
         Returns:
             List[Dict]
         """
         logger.info(f'Getting load curve with prm {prm} for client {client_id}')
-        qs = cls.objects.filter(prm=prm, client_id=client_id).order_by('-version')
+        if custom_filters is None:
+            custom_filters = {}
+
+        qs = cls.objects.filter(prm=prm, client_id=client_id, **custom_filters).order_by('-version')
         if version is not None:
             qs = qs.filter(version=version)
 
         entries = []
         for entry in qs:
             entry_dict = vars(entry)
             reader = BufferReader(entry_dict['data'])
@@ -113,25 +122,27 @@
         if len(entries) > 0 and combined_versions:
             ds_combined = ts_combine_first([e['data'] for e in entries])
             entries[0]['data'] = ds_combined
             return entries[0:1]
         return entries
 
     @classmethod
-    def get_many_lc(cls, prms: [str], client_id: int, combined_versions=True) -> Dict[str, List[Dict]]:
+    def get_many_lc(cls, prms: [str], client_id: int, combined_versions=True, custom_filters=None) -> Dict[str, List[Dict]]:
         """
         Get many prms from cache
         Args:
             prms: list of prms
             client_id: int, client's id
             combined_versions: bool, if multiple versions exists we combine them (default True)
         Returns:
             Dict[str, List[Dict]]
         """
-        qs = cls.objects.filter(prm__in=prms, client_id=client_id).order_by('-version')
+        if custom_filters is None:
+            custom_filters = {}
+        qs = cls.objects.filter(prm__in=prms, client_id=client_id, **custom_filters).order_by('-version')
         results = defaultdict(lambda: [])
         invalid_ids = []
         for entry in qs:
             reader = BufferReader(entry.data)
             ds = pd.read_feather(reader)
             try:
                 ds.set_index('index', inplace=True)
@@ -151,98 +162,110 @@
                 ds_combined = ts_combine_first([e['data'] for e in entries])
                 entries[0]['data'] = ds_combined
                 results[prm] = entries[0:1]
 
         return results
 
     @classmethod
-    def set_lc(cls, prm: str, value: pd.Series, client_id: int, versionning=False) -> None:
+    def set_lc(cls, prm: str, value: pd.Series, client_id: int, versionning=False, attributes_to_set=None) -> None:
         """
         Set one prm to cache
         Args:
             prm: str
             value: pd.Series
             client_id: int, client's id
             versionning: bool, if True, a new version will be saved else the load curve is replaced (default False)
-
+            attributes_to_set: (optionnal) None or dict
         Returns:
             None
         """
+        if attributes_to_set is None:
+            attributes_to_set = {}
         logger.info(f'SET key {prm} in cache')
         if isinstance(value, pd.Series):
             if value.isnull().all():
                 logger.warning(f'CACHE : Key {prm} is ignored because data is null')
                 return
             df = value.to_frame(name=prm)
             df.reset_index(inplace=True, names=['index'])
             buf = io.BytesIO()
             df.to_feather(buf, compression='lz4')
             v = buf.getvalue()
             if not versionning:
-                cls.objects.update_or_create(client_id=client_id, prm=prm, defaults=dict(data=v))
+                cls.objects.update_or_create(client_id=client_id, prm=prm, defaults=dict(data=v), **attributes_to_set)
             else:
-                latest_version = cls.objects.filter(client_id=client_id, prm=prm).aggregate(Max('version'))[
+                latest_version = cls.objects.filter(client_id=client_id, prm=prm, **attributes_to_set).aggregate(Max('version'))[
                     'version__max']
                 if latest_version is not None:
                     # If there's at least one object with the same prm, increment the version
                     version = latest_version + 1
                 else:
                     # If there are no objects with the same prm, start with version 0
                     version = 0
                 logger.info(f"version to insert {version}")
-                cls.objects.create(client_id=client_id, prm=prm, data=v, version=version)
+                cls.objects.create(client_id=client_id, prm=prm, data=v, version=version, **attributes_to_set)
             logger.info(f'SET prm {prm} in cache DONE')
         else:
             raise ValueError(f'Cannot cache value of type {type(value)}, only dataframe are accepted')
 
     @classmethod
-    def set_many_lc(cls, dataseries: Dict[str, pd.Series], client_id: int, versionning=False) -> None:
+    def set_many_lc(cls, dataseries: Dict[str, pd.Series], client_id: int, versionning=False, attributes_to_set=None) -> None:
         """
         Update prms contained in dataseries dict
         Args:
             dataseries: dict(key: pd.Series)
             client_id: int, client's id
             versionning: bool, if True, a new version will be saved for each prm else the load curve is replaced
+            attributes_to_set: (optionnal) None or dict
         Returns:
-            bool
+            None
         """
         if len(dataseries) > 0:
             logger.info(f'Updating cache for {list(dataseries.keys())}')
         for prm, data in dataseries.items():
             if data is not None and not data.empty:
-                cls.set_lc(prm, data, client_id, versionning=versionning)
+                cls.set_lc(prm, data, client_id, versionning=versionning, attributes_to_set=attributes_to_set)
 
     @classmethod
-    def clear(cls, prms: [str], client_id: int, version=None) -> None:
+    def clear(cls, prms: [str], client_id: int, version=None, custom_filters=None) -> None:
         """
         Method to clear multiple prm from cache
         Args:
             prms: list of prms
             client_id: client's id
             version: version id to delete
+            custom_filters: (optionnal) None or dict
         Returns:
             None
         """
-        qs = cls.objects.filter(prm__in=prms, client_id=client_id)
+        if custom_filters is None:
+            custom_filters = {}
+        qs = cls.objects.filter(prm__in=prms, client_id=client_id, **custom_filters)
         if version is not None:
             qs = qs.filter(version=version)
         qs.delete()
 
     @classmethod
-    def clear_all(cls, client_id: int = None) -> None:
+    def clear_all(cls, client_id: int = None, custom_filters=None) -> None:
         """
         Method to clear multiple prm from cache
         Args:
             client_id: client's id
+            custom_filters: (optionnal) None or dict
         Returns:
             None
         """
+        if custom_filters is None:
+            custom_filters = {}
+            qs = cls.objects.filter(**custom_filters)
+        else:
+            qs = cls.objects.all()
         if client_id is not None:
-            cls.objects.filter(client_id=client_id).delete()
+            qs.filter(client_id=client_id).delete()
         else:
-            cls.objects.all().delete()
+            qs.delete()
 
 
 class TestDataStore(Store):
     class Meta(Store.Meta):
         abstract = False
         app_label = 'hostore'
```

### Comparing `holcstore-0.1.8/hostore/tests.py` & `holcstore-0.2.0/hostore/tests.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.8/hostore/utils/timeseries.py` & `holcstore-0.2.0/hostore/utils/timeseries.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.8/setup.cfg` & `holcstore-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = holcstore
-version = 0.1.8
+version = 0.2.0
 description = A Django App to use a simple load curve store
 long_description = file: README.rst
 url = 
 author = Jean-Pierre Lartigue
 author_email = 
 license = BSD-3-Clause
 classifiers =
```

