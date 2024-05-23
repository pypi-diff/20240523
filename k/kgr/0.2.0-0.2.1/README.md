# Comparing `tmp/kgr-0.2.0.tar.gz` & `tmp/kgr-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgr-0.2.0.tar", last modified: Mon May 13 15:55:40 2024, max compression
+gzip compressed data, was "kgr-0.2.1.tar", last modified: Thu May 23 19:52:03 2024, max compression
```

## Comparing `kgr-0.2.0.tar` & `kgr-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2024-04-13 20:46:37.220586 kgr-0.2.0/LICENSE
--rw-r--r--   0        0        0       73 2024-04-13 20:46:37.220754 kgr-0.2.0/README.md
--rw-r--r--   0        0        0      876 2024-05-13 15:55:40.880263 kgr-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       94 2024-05-13 11:07:57.892389 kgr-0.2.0/src/kgr/__init__.py
--rw-r--r--   0        0        0      645 2024-05-13 15:45:03.297572 kgr-0.2.0/src/kgr/__main__.py
--rw-r--r--   0        0        0     3096 2024-05-13 15:49:06.693947 kgr-0.2.0/src/kgr/convert.py
--rw-r--r--   0        0        0     3430 2024-05-13 15:49:00.117401 kgr-0.2.0/src/kgr/geocode.py
--rw-r--r--   0        0        0     1302 2024-05-13 15:42:53.776396 kgr-0.2.0/src/kgr/lib.py
--rw-r--r--   0        0        0     2781 2024-05-13 15:46:54.378388 kgr-0.2.0/src/kgr/prepare.py
--rw-r--r--   0        0        0     2042 1970-01-01 00:00:00.000000 kgr-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-13 20:46:37.220586 kgr-0.2.1/LICENSE
+-rw-r--r--   0        0        0       73 2024-04-13 20:46:37.220754 kgr-0.2.1/README.md
+-rw-r--r--   0        0        0      876 2024-05-23 19:52:03.482235 kgr-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-05-13 11:07:57.892389 kgr-0.2.1/src/kgr/__init__.py
+-rw-r--r--   0        0        0      645 2024-05-13 15:45:03.297572 kgr-0.2.1/src/kgr/__main__.py
+-rw-r--r--   0        0        0     3096 2024-05-13 15:49:06.693947 kgr-0.2.1/src/kgr/convert.py
+-rw-r--r--   0        0        0     3396 2024-05-23 19:50:12.189075 kgr-0.2.1/src/kgr/geocode.py
+-rw-r--r--   0        0        0     1302 2024-05-13 15:42:53.776396 kgr-0.2.1/src/kgr/lib.py
+-rw-r--r--   0        0        0     2781 2024-05-13 15:46:54.378388 kgr-0.2.1/src/kgr/prepare.py
+-rw-r--r--   0        0        0     2042 1970-01-01 00:00:00.000000 kgr-0.2.1/PKG-INFO
```

### Comparing `kgr-0.2.0/LICENSE` & `kgr-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kgr-0.2.0/pyproject.toml` & `kgr-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "kgr"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
     "requests",
     "geopy",
     "bs4",
 ]
 authors = [
     { name = "Dmitry Luschan", email = "dluschan@gmail.com" },
```

### Comparing `kgr-0.2.0/src/kgr/__main__.py` & `kgr-0.2.1/src/kgr/__main__.py`

 * *Files identical despite different names*

### Comparing `kgr-0.2.0/src/kgr/convert.py` & `kgr-0.2.1/src/kgr/convert.py`

 * *Files identical despite different names*

### Comparing `kgr-0.2.0/src/kgr/geocode.py` & `kgr-0.2.1/src/kgr/geocode.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,10 +79,10 @@
 	
 	data = read_data(args)
 	if not data or not check_columns(data[0].keys(), "ФИО", "city"):
 		return
 	errors = translate_city_to_geocode(data, args)
 	if not args.quiet:
 		print(f"Не найдено и пропущено адресов: {errors}.")
-	write_data(data, headings + ["lon", "lat", "WKT"], args)
+	write_data(data, args)
```

### Comparing `kgr-0.2.0/src/kgr/lib.py` & `kgr-0.2.1/src/kgr/lib.py`

 * *Files identical despite different names*

### Comparing `kgr-0.2.0/src/kgr/prepare.py` & `kgr-0.2.1/src/kgr/prepare.py`

 * *Files identical despite different names*

### Comparing `kgr-0.2.0/PKG-INFO` & `kgr-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kgr
-Version: 0.2.0
+Version: 0.2.1
 Summary: Miltitool for convert data from https://memopzk.org to Google Maps
 Author-Email: Dmitry Luschan <dluschan@gmail.com>
 Maintainer-Email: Dmitry Luschan <dluschan@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Dmitry Luschan
```

