# Comparing `tmp/mercapy-0.3.0.tar.gz` & `tmp/mercapy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercapy-0.3.0.tar", last modified: Tue May 21 12:56:56 2024, max compression
+gzip compressed data, was "mercapy-1.0.0.tar", last modified: Wed May 22 09:22:10 2024, max compression
```

## Comparing `mercapy-0.3.0.tar` & `mercapy-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:56:56.835744 mercapy-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-21 12:56:51.000000 mercapy-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-21 12:56:56.835744 mercapy-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-21 12:56:51.000000 mercapy-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:56:56.831743 mercapy-0.3.0/mercapy/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:56:56.831743 mercapy-0.3.0/mercapy/elements/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/elements/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/elements/photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7802 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/elements/product.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/elements/season.py
--rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/merca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:56:56.835744 mercapy-0.3.0/mercapy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/utils/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/utils/warehouses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:56:56.835744 mercapy-0.3.0/mercapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-21 12:56:56.000000 mercapy-0.3.0/mercapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-21 12:56:56.000000 mercapy-0.3.0/mercapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 12:56:56.000000 mercapy-0.3.0/mercapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 12:56:56.000000 mercapy-0.3.0/mercapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 12:56:56.000000 mercapy-0.3.0/mercapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 12:56:56.835744 mercapy-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-21 12:56:51.000000 mercapy-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:22:10.148579 mercapy-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-22 09:22:00.000000 mercapy-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-22 09:22:10.148579 mercapy-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-22 09:22:00.000000 mercapy-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:22:10.148579 mercapy-1.0.0/mercapy/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:22:10.148579 mercapy-1.0.0/mercapy/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/elements/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/elements/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/elements/photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/elements/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/elements/season.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/merca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:22:10.148579 mercapy-1.0.0/mercapy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/utils/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-22 09:22:00.000000 mercapy-1.0.0/mercapy/utils/warehouses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:22:10.148579 mercapy-1.0.0/mercapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-22 09:22:10.000000 mercapy-1.0.0/mercapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-22 09:22:10.000000 mercapy-1.0.0/mercapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 09:22:10.000000 mercapy-1.0.0/mercapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 09:22:10.000000 mercapy-1.0.0/mercapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 09:22:10.000000 mercapy-1.0.0/mercapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 09:22:10.148579 mercapy-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-22 09:22:00.000000 mercapy-1.0.0/setup.py
```

### Comparing `mercapy-0.3.0/LICENSE` & `mercapy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mercapy-0.3.0/PKG-INFO` & `mercapy-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercapy
-Version: 0.3.0
+Version: 1.0.0
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
-Metadata-Version: 2.1 Name: mercapy Version: 0.3.0 Summary: A Mercadona
+Metadata-Version: 2.1 Name: mercapy Version: 1.0.0 Summary: A Mercadona
 interface for Python to track product prices, amounts, and more. Author: Joel
 Taylor Author-email: contact@joeltaylor.business License: MIT Keywords:
 mercadona,api,sdk,data science,prices,information Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.12 Classifier: Programming Language ::
 Python :: Implementation :: CPython Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: requests
```

### Comparing `mercapy-0.3.0/README.md` & `mercapy-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mercapy-0.3.0/mercapy/constants.py` & `mercapy-1.0.0/mercapy/constants.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 WAREHOUSES = [
     "mad1",
     "mad2",
     "bcn1",
     "alc1",
     "vlc1",
+    "svq1",
     "4115",
     "3532",
     "2183",
     "4483",
     "4421",
     "3684",
     "3968",
@@ -26,10 +27,23 @@
     "2623",
     "4416",
     "4028",
     "2343",
     "4436",
     "4281",
     "4308",
+    "2749",
+    "3947",
+    "3951",
+    "3996",
+    "4068",
+    "4069",
+    "4230",
+    "4267",
+    "4354",
+    "4385",
+    "4472",
+    "4558",
+    "4697",
 ]
 
 MAD1 = WAREHOUSES[0]
```

### Comparing `mercapy-0.3.0/mercapy/elements/category.py` & `mercapy-1.0.0/mercapy/elements/category.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-from dataclasses import dataclass, field
-from urllib.parse import urljoin
 from typing import Literal
 
-from ..constants import MAD1, API_URL
-from ..utils.api import fetch_json
+from .base import MercadonaItem, lazy_load_property
 
+class Category(MercadonaItem):
+    def __init__(
+        self,
+        id: str | dict,
+        name: str,
+        warehouse: str = "mad1",
+        language: Literal["es", "en"] = "es",
+    ):
+        self.name = name
+
+        if isinstance(id, dict):
+            endpoint = f"/api/categories/{id.get("id")}/"
+        else:
+            endpoint = f"/api/categories/{id}/"
 
-@dataclass
-class Category:
-    id: str
-    name: str = None
-    warehouse: str = MAD1
-    language: Literal["es", "en"] = "es"
-    _endpoint: str = field(init=False, repr=False)
-    _response: dict = field(default=None, init=False, repr=False)
+        super().__init__(id, endpoint, warehouse, language)
 
-    def get_products(self):
+    @lazy_load_property
+    def products(self):
         from .product import Product
 
-        url = urljoin(API_URL, f"/api/categories/{self.id}/")
-        response = fetch_json(url, {"lang": self.language, "wh": self.warehouse})
-
         category_products = []
-        subcategories = response.get("categories", [])
+        subcategories = self._data.get("categories", [])
         for subcategory in subcategories:
             products = subcategory.get("products", [])
 
             for product_data in products:
                 product = Product(product_data, self.warehouse, self.language)
                 category_products.append(product)
```

### Comparing `mercapy-0.3.0/mercapy/elements/photo.py` & `mercapy-1.0.0/mercapy/elements/photo.py`

 * *Files identical despite different names*

### Comparing `mercapy-0.3.0/mercapy/merca.py` & `mercapy-1.0.0/mercapy/merca.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,17 +62,15 @@
         """
         response = query_algolia(query, self.warehouse, self.language)
         hits = response.get("hits", [])
 
         products = []
         for h in hits:
             product = Product(h["id"], self.warehouse, self.language)
-
-            if product.exists():
-                products.append(product)
+            products.append(product)
 
         return products
 
     def get_home_recommendations(self) -> dict:
         """
         Retrieves product recommendations for the home page grouped by sections.
 
@@ -90,23 +88,22 @@
         for section in sections:
             section_name = section.get("layout")
 
             items = section.get("content", {}).get("items", [])
 
             for item in items:
                 if item.get("bg_colors", None):
-                    parsed_item = Season(item["id"], self.warehouse, self.language)
+                    parsed_item = Season(str(item["id"]), self.warehouse, self.language)
                 else:
                     parsed_item = Product(item, self.warehouse, self.language)
 
-                if parsed_item.exists():
-                    if section_products.get(section_name, None):
-                        section_products[section_name].append(parsed_item)
-                    else:
-                        section_products[section_name] = [parsed_item]
+                if section_products.get(section_name, None):
+                    section_products[section_name].append(parsed_item)
+                else:
+                    section_products[section_name] = [parsed_item]
 
         return section_products
 
     def get_new_arrivals(self) -> list[Product]:
         """
         New product arrivals at Mercadona
 
@@ -117,17 +114,16 @@
             list[Product]: List of new product arrivals.
         """
         url = urljoin(API_URL, f"/api/home/new-arrivals/")
         response = self._get_with_context(url)
 
         products = []
         for item in response.get("items", []):
-            product = Product(item)
-            if product.exists():
-                products.append(product)
+            product = Product(item, self.warehouse, self.language)
+            products.append(product)
 
         return products
 
     def get_categories(self) -> list[Category]:
         url = urljoin(API_URL, "/api/categories/")
         response = self._get_with_context(url)
```

### Comparing `mercapy-0.3.0/mercapy/utils/api.py` & `mercapy-1.0.0/mercapy/utils/api.py`

 * *Files identical despite different names*

### Comparing `mercapy-0.3.0/mercapy/utils/warehouses.py` & `mercapy-1.0.0/mercapy/utils/warehouses.py`

 * *Files identical despite different names*

### Comparing `mercapy-0.3.0/mercapy.egg-info/PKG-INFO` & `mercapy-1.0.0/mercapy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercapy
-Version: 0.3.0
+Version: 1.0.0
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
-Metadata-Version: 2.1 Name: mercapy Version: 0.3.0 Summary: A Mercadona
+Metadata-Version: 2.1 Name: mercapy Version: 1.0.0 Summary: A Mercadona
 interface for Python to track product prices, amounts, and more. Author: Joel
 Taylor Author-email: contact@joeltaylor.business License: MIT Keywords:
 mercadona,api,sdk,data science,prices,information Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.12 Classifier: Programming Language ::
 Python :: Implementation :: CPython Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: requests
```

### Comparing `mercapy-0.3.0/setup.py` & `mercapy-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
 # Read version from VERSION file
 here = path.abspath(path.dirname(__file__))
 
-VERSION = "0.3.0"
+VERSION = "1.0.0"
 DESCRIPTION = (
     "A Mercadona interface for Python to track product prices, amounts, and more."
 )
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
```

