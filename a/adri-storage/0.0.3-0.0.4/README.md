# Comparing `tmp/adri_storage-0.0.3.tar.gz` & `tmp/adri_storage-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adri_storage-0.0.3.tar", last modified: Mon May 20 12:48:59 2024, max compression
+gzip compressed data, was "adri_storage-0.0.4.tar", last modified: Thu May 23 05:39:00 2024, max compression
```

## Comparing `adri_storage-0.0.3.tar` & `adri_storage-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 12:48:59.439649 adri_storage-0.0.3/
--rw-rw-rw-   0        0        0      450 2024-05-20 12:48:59.437646 adri_storage-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-20 12:48:59.377810 adri_storage-0.0.3/adri_storage/
--rw-rw-rw-   0        0        0        0 2024-05-20 11:27:28.000000 adri_storage-0.0.3/adri_storage/__init__.py
--rw-rw-rw-   0        0        0     1098 2024-05-20 11:18:27.000000 adri_storage-0.0.3/adri_storage/client.py
--rw-rw-rw-   0        0        0       88 2024-05-19 11:03:38.000000 adri_storage-0.0.3/adri_storage/client_enums.py
--rw-rw-rw-   0        0        0     7692 2024-05-20 12:48:07.000000 adri_storage-0.0.3/adri_storage/local_client.py
--rw-rw-rw-   0        0        0     2000 2024-05-20 12:48:24.000000 adri_storage-0.0.3/adri_storage/main.py
--rw-rw-rw-   0        0        0     4775 2024-05-20 12:48:30.000000 adri_storage-0.0.3/adri_storage/s3_client.py
-drwxrwxrwx   0        0        0        0 2024-05-20 12:48:59.432453 adri_storage-0.0.3/adri_storage.egg-info/
--rw-rw-rw-   0        0        0      450 2024-05-20 12:48:59.000000 adri_storage-0.0.3/adri_storage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-05-20 12:48:59.000000 adri_storage-0.0.3/adri_storage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 12:48:59.000000 adri_storage-0.0.3/adri_storage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-20 12:48:59.000000 adri_storage-0.0.3/adri_storage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-20 12:48:59.000000 adri_storage-0.0.3/adri_storage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      592 2024-05-20 12:42:53.000000 adri_storage-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-20 12:48:59.440649 adri_storage-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 05:39:00.307902 adri_storage-0.0.4/
+-rw-rw-rw-   0        0        0      450 2024-05-23 05:39:00.297641 adri_storage-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 05:39:00.271042 adri_storage-0.0.4/adri_storage/
+-rw-rw-rw-   0        0        0        0 2024-05-20 11:27:28.000000 adri_storage-0.0.4/adri_storage/__init__.py
+-rw-rw-rw-   0        0        0     1098 2024-05-20 11:18:27.000000 adri_storage-0.0.4/adri_storage/client.py
+-rw-rw-rw-   0        0        0       88 2024-05-19 11:03:38.000000 adri_storage-0.0.4/adri_storage/client_enums.py
+-rw-rw-rw-   0        0        0     2000 2024-05-20 12:48:24.000000 adri_storage-0.0.4/adri_storage/client_factory.py
+-rw-rw-rw-   0        0        0     7692 2024-05-20 12:48:07.000000 adri_storage-0.0.4/adri_storage/local_client.py
+-rw-rw-rw-   0        0        0     4775 2024-05-20 12:48:30.000000 adri_storage-0.0.4/adri_storage/s3_client.py
+drwxrwxrwx   0        0        0        0 2024-05-23 05:39:00.297641 adri_storage-0.0.4/adri_storage.egg-info/
+-rw-rw-rw-   0        0        0      450 2024-05-23 05:39:00.000000 adri_storage-0.0.4/adri_storage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2024-05-23 05:39:00.000000 adri_storage-0.0.4/adri_storage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 05:39:00.000000 adri_storage-0.0.4/adri_storage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-23 05:39:00.000000 adri_storage-0.0.4/adri_storage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-23 05:39:00.000000 adri_storage-0.0.4/adri_storage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      592 2024-05-23 05:38:21.000000 adri_storage-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 05:39:00.308627 adri_storage-0.0.4/setup.cfg
```

### Comparing `adri_storage-0.0.3/adri_storage/client.py` & `adri_storage-0.0.4/adri_storage/client.py`

 * *Files identical despite different names*

### Comparing `adri_storage-0.0.3/adri_storage/local_client.py` & `adri_storage-0.0.4/adri_storage/local_client.py`

 * *Files identical despite different names*

### Comparing `adri_storage-0.0.3/adri_storage/main.py` & `adri_storage-0.0.4/adri_storage/client_factory.py`

 * *Files identical despite different names*

### Comparing `adri_storage-0.0.3/adri_storage/s3_client.py` & `adri_storage-0.0.4/adri_storage/s3_client.py`

 * *Files identical despite different names*

### Comparing `adri_storage-0.0.3/pyproject.toml` & `adri_storage-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "adri_storage"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Khalid Rasool", email="khalid.rasool@adri.nz" },
   { name="Eslam Allam", email="eslam.allam@adri.nz" }
 ]
 description = "ADRI Storage Python SDK"
 requires-python = ">=3.8"
 classifiers = [
```

