# Comparing `tmp/zermelo_api_vogk-1.0.4.tar.gz` & `tmp/zermelo_api_vogk-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zermelo_api_vogk-1.0.4.tar", last modified: Wed May 22 15:32:27 2024, max compression
+gzip compressed data, was "zermelo_api_vogk-1.0.5.tar", last modified: Wed May 22 15:42:05 2024, max compression
```

## Comparing `zermelo_api_vogk-1.0.4.tar` & `zermelo_api_vogk-1.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-22 15:32:27.789367 zermelo_api_vogk-1.0.4/
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1068 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.4/LICENSE
--rw-r--r--   0 klaas     (1000) klaas     (1000)     3969 2024-05-22 15:32:27.785366 zermelo_api_vogk-1.0.4/PKG-INFO
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3397 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.4/README.md
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-22 15:32:27.769366 zermelo_api_vogk-1.0.4/app/
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-22 15:32:27.773366 zermelo_api_vogk-1.0.4/app/zermelo_api/
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      563 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/__init__.py
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-22 15:32:27.781366 zermelo_api_vogk-1.0.4/app/zermelo_api/src/
--rw-rw-r--   0 klaas     (1000) klaas     (1000)        0 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/__init__.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3138 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/appointments.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3771 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/branches.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1437 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/config.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      618 2024-05-17 10:07:35.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/credentials.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1556 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/groepen.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      674 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/io_json.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1136 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/leerjaren.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     6089 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/lesgroepen.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      812 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/lokalen.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      446 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/time_utils.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3786 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/users.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1806 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/vakdoclok.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     2291 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/vakken.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     5831 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/vaklessen.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3612 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/zermelo_api.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1523 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/zermelo_collection.py
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-22 15:32:27.785366 zermelo_api_vogk-1.0.4/app/zermelo_api_vogk.egg-info/
--rw-r--r--   0 klaas     (1000) klaas     (1000)     3969 2024-05-22 15:32:27.000000 zermelo_api_vogk-1.0.4/app/zermelo_api_vogk.egg-info/PKG-INFO
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      834 2024-05-22 15:32:27.000000 zermelo_api_vogk-1.0.4/app/zermelo_api_vogk.egg-info/SOURCES.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)        1 2024-05-22 15:32:27.000000 zermelo_api_vogk-1.0.4/app/zermelo_api_vogk.egg-info/dependency_links.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)       15 2024-05-22 15:32:27.000000 zermelo_api_vogk-1.0.4/app/zermelo_api_vogk.egg-info/requires.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)       12 2024-05-22 15:32:27.000000 zermelo_api_vogk-1.0.4/app/zermelo_api_vogk.egg-info/top_level.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)       38 2024-05-22 15:32:27.789367 zermelo_api_vogk-1.0.4/setup.cfg
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      874 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.4/setup.py
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-22 15:42:05.400684 zermelo_api_vogk-1.0.5/
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1068 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.5/LICENSE
+-rw-r--r--   0 klaas     (1000) klaas     (1000)     4001 2024-05-22 15:42:05.400684 zermelo_api_vogk-1.0.5/PKG-INFO
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3429 2024-05-22 15:42:04.000000 zermelo_api_vogk-1.0.5/README.md
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-22 15:42:05.380684 zermelo_api_vogk-1.0.5/app/
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-22 15:42:05.380684 zermelo_api_vogk-1.0.5/app/zermelo_api/
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      552 2024-05-22 15:42:04.000000 zermelo_api_vogk-1.0.5/app/zermelo_api/__init__.py
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-22 15:42:05.396684 zermelo_api_vogk-1.0.5/app/zermelo_api/src/
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)        0 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.5/app/zermelo_api/src/__init__.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3138 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.5/app/zermelo_api/src/appointments.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3771 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.5/app/zermelo_api/src/branches.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1437 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.5/app/zermelo_api/src/config.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      618 2024-05-17 10:07:35.000000 zermelo_api_vogk-1.0.5/app/zermelo_api/src/credentials.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1556 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.5/app/zermelo_api/src/groepen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      674 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.5/app/zermelo_api/src/io_json.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1136 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.5/app/zermelo_api/src/leerjaren.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     6089 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.5/app/zermelo_api/src/lesgroepen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      812 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.5/app/zermelo_api/src/lokalen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      446 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.5/app/zermelo_api/src/time_utils.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3786 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.5/app/zermelo_api/src/users.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1806 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.5/app/zermelo_api/src/vakdoclok.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     2291 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.5/app/zermelo_api/src/vakken.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     5831 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.5/app/zermelo_api/src/vaklessen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3612 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.5/app/zermelo_api/src/zermelo_api.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1523 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.5/app/zermelo_api/src/zermelo_collection.py
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-22 15:42:05.400684 zermelo_api_vogk-1.0.5/app/zermelo_api_vogk.egg-info/
+-rw-r--r--   0 klaas     (1000) klaas     (1000)     4001 2024-05-22 15:42:05.000000 zermelo_api_vogk-1.0.5/app/zermelo_api_vogk.egg-info/PKG-INFO
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      834 2024-05-22 15:42:05.000000 zermelo_api_vogk-1.0.5/app/zermelo_api_vogk.egg-info/SOURCES.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)        1 2024-05-22 15:42:05.000000 zermelo_api_vogk-1.0.5/app/zermelo_api_vogk.egg-info/dependency_links.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)       15 2024-05-22 15:42:05.000000 zermelo_api_vogk-1.0.5/app/zermelo_api_vogk.egg-info/requires.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)       12 2024-05-22 15:42:05.000000 zermelo_api_vogk-1.0.5/app/zermelo_api_vogk.egg-info/top_level.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)       38 2024-05-22 15:42:05.400684 zermelo_api_vogk-1.0.5/setup.cfg
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      874 2024-05-22 15:42:04.000000 zermelo_api_vogk-1.0.5/setup.py
```

### Comparing `zermelo_api_vogk-1.0.4/LICENSE` & `zermelo_api_vogk-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.4/PKG-INFO` & `zermelo_api_vogk-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zermelo_api_vogk
-Version: 1.0.4
+Version: 1.0.5
 Summary: A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 Home-page: https://github.com/KlaasVogel/zermelo_api_vogk
 Author: Klaas Vogel
 Author-email: zermelo_api@klaasvogel.nl
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
@@ -14,17 +14,18 @@
 License-File: LICENSE
 Requires-Dist: aiohttp
 Provides-Extra: dev
 
 ## zermelo_api_vogk
 A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 
-# V1.0.4
+# V1.0.5
  - async loading lesgroepen done
  - async loading appointments done
+ - enabled packages in __init__
 
 # V1.0.2
  - replacement of request for working with asyncio
  - first rough test if asyncio is working
  - TODO: refactor leerlingen (sort should be done later)
  - loading branches seems done.
  - Next check Lesgroepen en vakdocloks
```

### Comparing `zermelo_api_vogk-1.0.4/README.md` & `zermelo_api_vogk-1.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ## zermelo_api_vogk
 A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 
-# V1.0.4
+# V1.0.5
  - async loading lesgroepen done
  - async loading appointments done
+ - enabled packages in __init__
 
 # V1.0.2
  - replacement of request for working with asyncio
  - first rough test if asyncio is working
  - TODO: refactor leerlingen (sort should be done later)
  - loading branches seems done.
  - Next check Lesgroepen en vakdocloks
```

### Comparing `zermelo_api_vogk-1.0.4/app/zermelo_api/__init__.py` & `zermelo_api_vogk-1.0.5/app/zermelo_api/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .src.zermelo_api import ZermeloAPI, loadAPI
 # from .src.collections import ZermeloCollection
 from .src.branches import Branch, Branches
 from .src.time_utils import *
-# from .src.users import Leerling, Medewerker, Leerlingen, Personeel
-# from .src.lesgroepen import Lesgroepen, Lesgroep
-# from .src.leerjaren import Leerjaar, Leerjaren
-# from .src.appointments import get_user_appointments, get_department_updates, Appointment
-# from .src.vakken import Vakken, Vak
-# from .src.lokalen import Lokalen, Lokaal
+from .src.users import Leerling, Medewerker, Leerlingen, Personeel
+from .src.lesgroepen import Lesgroepen, Lesgroep
+from .src.leerjaren import Leerjaar, Leerjaren
+from .src.appointments import get_user_appointments, get_department_updates, Appointment
+from .src.vakken import Vakken, Vak
+from .src.lokalen import Lokalen, Lokaal
+
 # from .src.vakdoclok import VakDocLoks, VakDocLok
```

### Comparing `zermelo_api_vogk-1.0.4/app/zermelo_api/src/appointments.py` & `zermelo_api_vogk-1.0.5/app/zermelo_api/src/appointments.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.4/app/zermelo_api/src/branches.py` & `zermelo_api_vogk-1.0.5/app/zermelo_api/src/branches.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.4/app/zermelo_api/src/config.py` & `zermelo_api_vogk-1.0.5/app/zermelo_api/src/config.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.4/app/zermelo_api/src/credentials.py` & `zermelo_api_vogk-1.0.5/app/zermelo_api/src/credentials.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.4/app/zermelo_api/src/groepen.py` & `zermelo_api_vogk-1.0.5/app/zermelo_api/src/groepen.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.4/app/zermelo_api/src/io_json.py` & `zermelo_api_vogk-1.0.5/app/zermelo_api/src/io_json.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.4/app/zermelo_api/src/leerjaren.py` & `zermelo_api_vogk-1.0.5/app/zermelo_api/src/leerjaren.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.4/app/zermelo_api/src/lesgroepen.py` & `zermelo_api_vogk-1.0.5/app/zermelo_api/src/lesgroepen.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.4/app/zermelo_api/src/lokalen.py` & `zermelo_api_vogk-1.0.5/app/zermelo_api/src/lokalen.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.4/app/zermelo_api/src/users.py` & `zermelo_api_vogk-1.0.5/app/zermelo_api/src/users.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.4/app/zermelo_api/src/vakdoclok.py` & `zermelo_api_vogk-1.0.5/app/zermelo_api/src/vakdoclok.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.4/app/zermelo_api/src/vakken.py` & `zermelo_api_vogk-1.0.5/app/zermelo_api/src/vakken.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.4/app/zermelo_api/src/vaklessen.py` & `zermelo_api_vogk-1.0.5/app/zermelo_api/src/vaklessen.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.4/app/zermelo_api/src/zermelo_api.py` & `zermelo_api_vogk-1.0.5/app/zermelo_api/src/zermelo_api.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.4/app/zermelo_api/src/zermelo_collection.py` & `zermelo_api_vogk-1.0.5/app/zermelo_api/src/zermelo_collection.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.4/app/zermelo_api_vogk.egg-info/PKG-INFO` & `zermelo_api_vogk-1.0.5/app/zermelo_api_vogk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zermelo_api_vogk
-Version: 1.0.4
+Version: 1.0.5
 Summary: A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 Home-page: https://github.com/KlaasVogel/zermelo_api_vogk
 Author: Klaas Vogel
 Author-email: zermelo_api@klaasvogel.nl
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
@@ -14,17 +14,18 @@
 License-File: LICENSE
 Requires-Dist: aiohttp
 Provides-Extra: dev
 
 ## zermelo_api_vogk
 A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 
-# V1.0.4
+# V1.0.5
  - async loading lesgroepen done
  - async loading appointments done
+ - enabled packages in __init__
 
 # V1.0.2
  - replacement of request for working with asyncio
  - first rough test if asyncio is working
  - TODO: refactor leerlingen (sort should be done later)
  - loading branches seems done.
  - Next check Lesgroepen en vakdocloks
```

### Comparing `zermelo_api_vogk-1.0.4/app/zermelo_api_vogk.egg-info/SOURCES.txt` & `zermelo_api_vogk-1.0.5/app/zermelo_api_vogk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.4/setup.py` & `zermelo_api_vogk-1.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="zermelo_api_vogk",
-    version="1.0.4",
+    version="1.0.5",
     description="A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/KlaasVogel/zermelo_api_vogk",
     author="Klaas Vogel",
```

