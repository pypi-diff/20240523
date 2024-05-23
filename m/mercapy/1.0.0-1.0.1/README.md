# Comparing `tmp/mercapy-1.0.0.tar.gz` & `tmp/mercapy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercapy-1.0.0.tar", last modified: Wed May 22 09:22:10 2024, max compression
+gzip compressed data, was "mercapy-1.0.1.tar", last modified: Thu May 23 07:26:41 2024, max compression
```

## Comparing `mercapy-1.0.0.tar` & `mercapy-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:22:10.148579 mercapy-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-22 09:22:00.000000 mercapy-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-22 09:22:10.148579 mercapy-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-22 09:22:00.000000 mercapy-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:22:10.148579 mercapy-1.0.0/mercapy/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:22:10.148579 mercapy-1.0.0/mercapy/elements/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/elements/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/elements/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/elements/photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/elements/product.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/elements/season.py
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/merca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:22:10.148579 mercapy-1.0.0/mercapy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/utils/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/utils/warehouses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:22:10.148579 mercapy-1.0.0/mercapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-22 09:22:10.000000 mercapy-1.0.0/mercapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-22 09:22:10.000000 mercapy-1.0.0/mercapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 09:22:10.000000 mercapy-1.0.0/mercapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 09:22:10.000000 mercapy-1.0.0/mercapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 09:22:10.000000 mercapy-1.0.0/mercapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 09:22:10.148579 mercapy-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-22 09:22:00.000000 mercapy-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:26:41.726110 mercapy-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-23 07:26:36.000000 mercapy-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-23 07:26:41.726110 mercapy-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-23 07:26:36.000000 mercapy-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:26:41.722110 mercapy-1.0.1/mercapy/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-23 07:26:36.000000 mercapy-1.0.1/mercapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-23 07:26:36.000000 mercapy-1.0.1/mercapy/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:26:41.722110 mercapy-1.0.1/mercapy/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-23 07:26:36.000000 mercapy-1.0.1/mercapy/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-23 07:26:36.000000 mercapy-1.0.1/mercapy/elements/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-23 07:26:36.000000 mercapy-1.0.1/mercapy/elements/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-23 07:26:36.000000 mercapy-1.0.1/mercapy/elements/photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-05-23 07:26:36.000000 mercapy-1.0.1/mercapy/elements/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-23 07:26:36.000000 mercapy-1.0.1/mercapy/elements/season.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-23 07:26:36.000000 mercapy-1.0.1/mercapy/merca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:26:41.722110 mercapy-1.0.1/mercapy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:26:36.000000 mercapy-1.0.1/mercapy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-23 07:26:36.000000 mercapy-1.0.1/mercapy/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-23 07:26:36.000000 mercapy-1.0.1/mercapy/utils/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-23 07:26:36.000000 mercapy-1.0.1/mercapy/utils/warehouses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:26:41.726110 mercapy-1.0.1/mercapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-23 07:26:41.000000 mercapy-1.0.1/mercapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-23 07:26:41.000000 mercapy-1.0.1/mercapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 07:26:41.000000 mercapy-1.0.1/mercapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 07:26:41.000000 mercapy-1.0.1/mercapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 07:26:41.000000 mercapy-1.0.1/mercapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 07:26:41.726110 mercapy-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-23 07:26:36.000000 mercapy-1.0.1/setup.py
```

### Comparing `mercapy-1.0.0/LICENSE` & `mercapy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mercapy-1.0.0/PKG-INFO` & `mercapy-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercapy
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Mercadona interface for Python to track product prices, amounts, and more.
 Author: Joel Taylor
 Author-email: contact@joeltaylor.business
 License: MIT
 Keywords: mercadona,api,sdk,data science,prices,information
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mercapy Version: 1.0.0 Summary: A Mercadona
+Metadata-Version: 2.1 Name: mercapy Version: 1.0.1 Summary: A Mercadona
 interface for Python to track product prices, amounts, and more. Author: Joel
 Taylor Author-email: contact@joeltaylor.business License: MIT Keywords:
 mercadona,api,sdk,data science,prices,information Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.12 Classifier: Programming Language ::
 Python :: Implementation :: CPython Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: requests
```

### Comparing `mercapy-1.0.0/README.md` & `mercapy-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mercapy-1.0.0/mercapy/constants.py` & `mercapy-1.0.1/mercapy/constants.py`

 * *Files identical despite different names*

### Comparing `mercapy-1.0.0/mercapy/elements/base.py` & `mercapy-1.0.1/mercapy/elements/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
 
 def lazy_load_property(func):
     @property
     def wrapper(self):
         if self._is_empty():
             self._fetch_data()
+        
+        if self.not_found():
+            return None
+        
         return func(self)
 
     return wrapper
 
 
 @dataclass
 class MercadonaItem:
@@ -29,21 +33,28 @@
         language (str): Language for the API response. Defaults to "es".
     """
 
     id: str | dict
     endpoint: str = field(repr=False)
     warehouse: str = "mad1"
     language: Literal["es", "en"] = field(default="es", init=True, repr=False)
-    _data: dict = field(init=False, default=None, repr=False)
 
     def __post_init__(self):
+        self._data = {}
+
         if isinstance(self.id, dict):
             self._data = self.id
             self.id = self._data.get("id")
 
+    def not_found(self):
+        if self._is_empty():
+            self._fetch_data()
+
+        return bool(self._data.get("err_code"))
+
     def _fetch_with_context(self, endpoint: str) -> dict:
         url = urljoin(API_URL, endpoint)
         return fetch_json(url, {"lang": self.language, "wh": self.warehouse})
 
     def _fetch_data(self, retry_attempts: int = 3, retry_delay: int = 20) -> None:
         attempt = 0
         while attempt <= retry_attempts:
@@ -60,20 +71,18 @@
                 print(
                     f"[{attempt}/{retry_attempts}]: Retrying to fetch {self} in {calculated_delay} seconds..."
                 )
                 time.sleep(calculated_delay)
             elif err_code == 404:
                 # Not Found, no need to retry
                 print(f"Couldn't find {self} :(")
-                self._data = None
                 break
             else:
                 # Other errors, stop retrying
                 print(f"Error fetching data for {self}.")
-                self._data = None
                 break
 
     def _is_empty(self):
         return not bool(self._data)
 
     def __dict__(self):
         if self._is_empty():
```

### Comparing `mercapy-1.0.0/mercapy/elements/category.py` & `mercapy-1.0.1/mercapy/elements/category.py`

 * *Files identical despite different names*

### Comparing `mercapy-1.0.0/mercapy/elements/photo.py` & `mercapy-1.0.1/mercapy/elements/photo.py`

 * *Files identical despite different names*

### Comparing `mercapy-1.0.0/mercapy/elements/product.py` & `mercapy-1.0.1/mercapy/elements/product.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,19 @@
             endpoint = f"/api/products/{id.get("id")}/"
         else:
             endpoint = f"/api/products/{id}/"
 
         super().__init__(id, endpoint, warehouse, language)
 
     def _is_data_incomplete(self):
-        details = self._data.get("details", None)
-        if not details:
-            self._fetch_data()
+        if self._data is None:
+            return True
+        
+        details = self._data.get("details", {})
+        return not details
 
     @lazy_load_property
     @require_complete_data
     def ean(self) -> str:
         return self._data.get("ean")
 
     @lazy_load_property
```

### Comparing `mercapy-1.0.0/mercapy/elements/season.py` & `mercapy-1.0.1/mercapy/elements/season.py`

 * *Files identical despite different names*

### Comparing `mercapy-1.0.0/mercapy/merca.py` & `mercapy-1.0.1/mercapy/merca.py`

 * *Files identical despite different names*

### Comparing `mercapy-1.0.0/mercapy/utils/api.py` & `mercapy-1.0.1/mercapy/utils/api.py`

 * *Files identical despite different names*

### Comparing `mercapy-1.0.0/mercapy/utils/warehouses.py` & `mercapy-1.0.1/mercapy/utils/warehouses.py`

 * *Files identical despite different names*

### Comparing `mercapy-1.0.0/mercapy.egg-info/PKG-INFO` & `mercapy-1.0.1/mercapy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercapy
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Mercadona interface for Python to track product prices, amounts, and more.
 Author: Joel Taylor
 Author-email: contact@joeltaylor.business
 License: MIT
 Keywords: mercadona,api,sdk,data science,prices,information
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mercapy Version: 1.0.0 Summary: A Mercadona
+Metadata-Version: 2.1 Name: mercapy Version: 1.0.1 Summary: A Mercadona
 interface for Python to track product prices, amounts, and more. Author: Joel
 Taylor Author-email: contact@joeltaylor.business License: MIT Keywords:
 mercadona,api,sdk,data science,prices,information Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.12 Classifier: Programming Language ::
 Python :: Implementation :: CPython Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: requests
```

### Comparing `mercapy-1.0.0/setup.py` & `mercapy-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
 # Read version from VERSION file
 here = path.abspath(path.dirname(__file__))
 
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 DESCRIPTION = (
     "A Mercadona interface for Python to track product prices, amounts, and more."
 )
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
```

