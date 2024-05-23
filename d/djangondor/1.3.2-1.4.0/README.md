# Comparing `tmp/djangondor-1.3.2.tar.gz` & `tmp/djangondor-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangondor-1.3.2.tar", last modified: Wed May 22 18:17:00 2024, max compression
+gzip compressed data, was "djangondor-1.4.0.tar", last modified: Wed May 22 18:31:42 2024, max compression
```

## Comparing `djangondor-1.3.2.tar` & `djangondor-1.4.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dalitso   (1000) dalitso   (1000)        0 2024-05-22 18:17:00.606989 djangondor-1.3.2/
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1103 2023-10-14 14:58:56.000000 djangondor-1.3.2/LICENSE
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1348 2024-05-22 18:17:00.606989 djangondor-1.3.2/PKG-INFO
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)      349 2023-10-14 14:58:56.000000 djangondor-1.3.2/README.rst
-drwxr-xr-x   0 dalitso   (1000) dalitso   (1000)        0 2024-05-22 18:17:00.606989 djangondor-1.3.2/djangondor/
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)        0 2023-10-14 14:58:56.000000 djangondor-1.3.2/djangondor/__init__.py
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)       63 2023-10-14 14:58:56.000000 djangondor-1.3.2/djangondor/admin.py
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)      152 2023-10-14 14:58:56.000000 djangondor-1.3.2/djangondor/apps.py
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1251 2023-10-14 14:58:56.000000 djangondor-1.3.2/djangondor/collections.py
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1636 2023-10-21 16:21:10.000000 djangondor-1.3.2/djangondor/models.py
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)     3417 2023-10-14 14:58:56.000000 djangondor-1.3.2/djangondor/processing.py
-drwxr-xr-x   0 dalitso   (1000) dalitso   (1000)        0 2024-05-22 18:17:00.606989 djangondor-1.3.2/djangondor/templatetags/
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)        0 2023-10-14 14:58:56.000000 djangondor-1.3.2/djangondor/templatetags/__init__.py
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)      410 2023-10-14 14:58:56.000000 djangondor-1.3.2/djangondor/templatetags/djangondor_collection_tags.py
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1601 2023-10-14 14:58:56.000000 djangondor-1.3.2/djangondor/templatetags/djangondor_path_tags.py
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)       60 2023-10-14 14:58:56.000000 djangondor-1.3.2/djangondor/tests.py
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)      909 2023-10-14 14:58:56.000000 djangondor-1.3.2/djangondor/time.py
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)       63 2023-10-14 14:58:56.000000 djangondor-1.3.2/djangondor/views.py
-drwxr-xr-x   0 dalitso   (1000) dalitso   (1000)        0 2024-05-22 18:17:00.606989 djangondor-1.3.2/djangondor.egg-info/
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1348 2024-05-22 18:17:00.000000 djangondor-1.3.2/djangondor.egg-info/PKG-INFO
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)      552 2024-05-22 18:17:00.000000 djangondor-1.3.2/djangondor.egg-info/SOURCES.txt
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)        1 2024-05-22 18:17:00.000000 djangondor-1.3.2/djangondor.egg-info/dependency_links.txt
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)       54 2024-05-22 18:17:00.000000 djangondor-1.3.2/djangondor.egg-info/requires.txt
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)       11 2024-05-22 18:17:00.000000 djangondor-1.3.2/djangondor.egg-info/top_level.txt
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)       89 2023-10-14 14:58:56.000000 djangondor-1.3.2/pyproject.toml
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)      945 2024-05-22 18:17:00.606989 djangondor-1.3.2/setup.cfg
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)      106 2023-10-14 14:58:56.000000 djangondor-1.3.2/setup.py
+drwxr-xr-x   0 dalitso   (1000) dalitso   (1000)        0 2024-05-22 18:31:42.866885 djangondor-1.4.0/
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1103 2023-10-14 14:58:56.000000 djangondor-1.4.0/LICENSE
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1348 2024-05-22 18:31:42.866885 djangondor-1.4.0/PKG-INFO
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)      349 2023-10-14 14:58:56.000000 djangondor-1.4.0/README.rst
+drwxr-xr-x   0 dalitso   (1000) dalitso   (1000)        0 2024-05-22 18:31:42.866885 djangondor-1.4.0/djangondor/
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)        0 2023-10-14 14:58:56.000000 djangondor-1.4.0/djangondor/__init__.py
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)       63 2023-10-14 14:58:56.000000 djangondor-1.4.0/djangondor/admin.py
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)      152 2023-10-14 14:58:56.000000 djangondor-1.4.0/djangondor/apps.py
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1251 2023-10-14 14:58:56.000000 djangondor-1.4.0/djangondor/collections.py
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1693 2024-05-22 18:30:27.000000 djangondor-1.4.0/djangondor/models.py
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)     3417 2023-10-14 14:58:56.000000 djangondor-1.4.0/djangondor/processing.py
+drwxr-xr-x   0 dalitso   (1000) dalitso   (1000)        0 2024-05-22 18:31:42.866885 djangondor-1.4.0/djangondor/templatetags/
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)        0 2023-10-14 14:58:56.000000 djangondor-1.4.0/djangondor/templatetags/__init__.py
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)      410 2023-10-14 14:58:56.000000 djangondor-1.4.0/djangondor/templatetags/djangondor_collection_tags.py
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1601 2023-10-14 14:58:56.000000 djangondor-1.4.0/djangondor/templatetags/djangondor_path_tags.py
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)       60 2023-10-14 14:58:56.000000 djangondor-1.4.0/djangondor/tests.py
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)      909 2023-10-14 14:58:56.000000 djangondor-1.4.0/djangondor/time.py
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)       63 2023-10-14 14:58:56.000000 djangondor-1.4.0/djangondor/views.py
+drwxr-xr-x   0 dalitso   (1000) dalitso   (1000)        0 2024-05-22 18:31:42.866885 djangondor-1.4.0/djangondor.egg-info/
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1348 2024-05-22 18:31:42.000000 djangondor-1.4.0/djangondor.egg-info/PKG-INFO
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)      552 2024-05-22 18:31:42.000000 djangondor-1.4.0/djangondor.egg-info/SOURCES.txt
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)        1 2024-05-22 18:31:42.000000 djangondor-1.4.0/djangondor.egg-info/dependency_links.txt
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)       54 2024-05-22 18:31:42.000000 djangondor-1.4.0/djangondor.egg-info/requires.txt
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)       11 2024-05-22 18:31:42.000000 djangondor-1.4.0/djangondor.egg-info/top_level.txt
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)       89 2023-10-14 14:58:56.000000 djangondor-1.4.0/pyproject.toml
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)      945 2024-05-22 18:31:42.866885 djangondor-1.4.0/setup.cfg
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)      106 2023-10-14 14:58:56.000000 djangondor-1.4.0/setup.py
```

### Comparing `djangondor-1.3.2/LICENSE` & `djangondor-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djangondor-1.3.2/PKG-INFO` & `djangondor-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangondor
-Version: 1.3.2
+Version: 1.4.0
 Summary: A collection of django utilities.
 Home-page: https://github.com/dalitsosakala/djangondor
 Author: Dalitso Sakala
 Author-email: dalitso.1sc@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `djangondor-1.3.2/djangondor/collections.py` & `djangondor-1.4.0/djangondor/collections.py`

 * *Files identical despite different names*

### Comparing `djangondor-1.3.2/djangondor/models.py` & `djangondor-1.4.0/djangondor/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from django.db import models
+from django.db.models import CASCADE
 import uuid
 
 # Create your models here.
 
 
 # NULLABLE
 # USAGE
 # =====
 # description = models.CharField(max_length=200,**NULLABLE)
 # # is the same as:
 # description = models.CharField(max_length=200,null=True,default=None,blank=True)
 NULLABLE = {"null": True, "default": None, "blank": True}
 NULLABLE_CHARFIELD = {**NULLABLE, "max_length": 250}
+NULLABLE_FK = {**NULLABLE, "on_delete": CASCADE}
 NON_NULL_BLANK_CHARFIELD = {"blank":True, "max_length": 225}
 
 
 # UUID_PK
 # USAGE
 # =====
 # id=models.UUIDField(**UUID_PK)
```

### Comparing `djangondor-1.3.2/djangondor/processing.py` & `djangondor-1.4.0/djangondor/processing.py`

 * *Files identical despite different names*

### Comparing `djangondor-1.3.2/djangondor/templatetags/djangondor_path_tags.py` & `djangondor-1.4.0/djangondor/templatetags/djangondor_path_tags.py`

 * *Files identical despite different names*

### Comparing `djangondor-1.3.2/djangondor/time.py` & `djangondor-1.4.0/djangondor/time.py`

 * *Files identical despite different names*

### Comparing `djangondor-1.3.2/djangondor.egg-info/PKG-INFO` & `djangondor-1.4.0/djangondor.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangondor
-Version: 1.3.2
+Version: 1.4.0
 Summary: A collection of django utilities.
 Home-page: https://github.com/dalitsosakala/djangondor
 Author: Dalitso Sakala
 Author-email: dalitso.1sc@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `djangondor-1.3.2/djangondor.egg-info/SOURCES.txt` & `djangondor-1.4.0/djangondor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangondor-1.3.2/setup.cfg` & `djangondor-1.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djangondor
-version = 1.3.2
+version = 1.4.0
 description = A collection of django utilities.
 long_description = file: README.rst
 url = https://github.com/dalitsosakala/djangondor
 author = Dalitso Sakala
 author_email = dalitso.1sc@gmail.com
 license = MIT License
 classifiers =
```

