# Comparing `tmp/billzio_api-1.0.6.tar.gz` & `tmp/billzio_api-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "billzio_api-1.0.6.tar", max compression
+gzip compressed data, was "billzio_api-1.0.7.tar", max compression
```

## Comparing `billzio_api-1.0.6.tar` & `billzio_api-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-08-22 15:09:19.640175 billzio_api-1.0.6/LICENSE
--rw-r--r--   0        0        0     1287 2023-08-22 15:09:19.640175 billzio_api-1.0.6/README.md
--rw-r--r--   0        0        0      565 2023-08-22 15:09:19.640175 billzio_api-1.0.6/billzio_api/__init__.py
--rw-r--r--   0        0        0      273 2023-08-22 15:09:19.640175 billzio_api-1.0.6/billzio_api/__version__.py
--rw-r--r--   0        0        0      188 2023-08-22 15:09:19.640175 billzio_api-1.0.6/billzio_api/exceptions.py
--rw-r--r--   0        0        0        0 2023-08-22 15:09:19.640175 billzio_api-1.0.6/billzio_api/handlers/__init__.py
--rw-r--r--   0        0        0     8507 2023-08-22 15:09:19.640175 billzio_api-1.0.6/billzio_api/handlers/async_handler.py
--rw-r--r--   0        0        0     2692 2023-08-22 15:09:19.640175 billzio_api-1.0.6/billzio_api/handlers/base.py
--rw-r--r--   0        0        0     7895 2023-08-22 15:09:19.640175 billzio_api-1.0.6/billzio_api/handlers/handler.py
--rw-r--r--   0        0        0      151 2023-08-22 15:09:19.640175 billzio_api-1.0.6/billzio_api/models/auth.py
--rw-r--r--   0        0        0      361 2023-08-22 15:09:19.640175 billzio_api-1.0.6/billzio_api/models/brands.py
--rw-r--r--   0        0        0      831 2023-08-22 15:09:19.640175 billzio_api-1.0.6/billzio_api/models/categories.py
--rw-r--r--   0        0        0     1183 2023-08-22 15:09:19.640175 billzio_api-1.0.6/billzio_api/models/clients.py
--rw-r--r--   0        0        0      495 2023-08-22 15:09:19.640175 billzio_api-1.0.6/billzio_api/models/currencies.py
--rw-r--r--   0        0        0      376 2023-08-22 15:09:19.640175 billzio_api-1.0.6/billzio_api/models/orders.py
--rw-r--r--   0        0        0      374 2023-08-22 15:09:19.640175 billzio_api-1.0.6/billzio_api/models/payment_types.py
--rw-r--r--   0        0        0     1438 2023-08-22 15:09:19.640175 billzio_api-1.0.6/billzio_api/models/products.py
--rw-r--r--   0        0        0      698 2023-08-22 15:09:19.640175 billzio_api-1.0.6/billzio_api/models/shops.py
--rw-r--r--   0        0        0      395 2023-08-22 15:09:19.640175 billzio_api-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     1840 1970-01-01 00:00:00.000000 billzio_api-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-23 09:02:33.964650 billzio_api-1.0.7/LICENSE
+-rw-r--r--   0        0        0     1287 2024-05-23 09:02:33.964650 billzio_api-1.0.7/README.md
+-rw-r--r--   0        0        0      565 2024-05-23 09:02:33.964650 billzio_api-1.0.7/billzio_api/__init__.py
+-rw-r--r--   0        0        0      273 2024-05-23 09:02:33.964650 billzio_api-1.0.7/billzio_api/__version__.py
+-rw-r--r--   0        0        0      188 2024-05-23 09:02:33.964650 billzio_api-1.0.7/billzio_api/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:02:33.964650 billzio_api-1.0.7/billzio_api/handlers/__init__.py
+-rw-r--r--   0        0        0     8704 2024-05-23 09:02:33.964650 billzio_api-1.0.7/billzio_api/handlers/async_handler.py
+-rw-r--r--   0        0        0     2692 2024-05-23 09:02:33.964650 billzio_api-1.0.7/billzio_api/handlers/base.py
+-rw-r--r--   0        0        0     8088 2024-05-23 09:02:33.964650 billzio_api-1.0.7/billzio_api/handlers/handler.py
+-rw-r--r--   0        0        0      151 2024-05-23 09:02:33.964650 billzio_api-1.0.7/billzio_api/models/auth.py
+-rw-r--r--   0        0        0      361 2024-05-23 09:02:33.964650 billzio_api-1.0.7/billzio_api/models/brands.py
+-rw-r--r--   0        0        0      831 2024-05-23 09:02:33.964650 billzio_api-1.0.7/billzio_api/models/categories.py
+-rw-r--r--   0        0        0     1183 2024-05-23 09:02:33.968649 billzio_api-1.0.7/billzio_api/models/clients.py
+-rw-r--r--   0        0        0      495 2024-05-23 09:02:33.968649 billzio_api-1.0.7/billzio_api/models/currencies.py
+-rw-r--r--   0        0        0      396 2024-05-23 09:02:33.968649 billzio_api-1.0.7/billzio_api/models/orders.py
+-rw-r--r--   0        0        0      374 2024-05-23 09:02:33.968649 billzio_api-1.0.7/billzio_api/models/payment_types.py
+-rw-r--r--   0        0        0     1513 2024-05-23 09:02:33.968649 billzio_api-1.0.7/billzio_api/models/products.py
+-rw-r--r--   0        0        0      698 2024-05-23 09:02:33.968649 billzio_api-1.0.7/billzio_api/models/shops.py
+-rw-r--r--   0        0        0      395 2024-05-23 09:02:33.968649 billzio_api-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1891 1970-01-01 00:00:00.000000 billzio_api-1.0.7/PKG-INFO
```

### Comparing `billzio_api-1.0.6/LICENSE` & `billzio_api-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `billzio_api-1.0.6/README.md` & `billzio_api-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `billzio_api-1.0.6/billzio_api/__init__.py` & `billzio_api-1.0.7/billzio_api/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.6"
+__version__ = "1.0.7"
 
 from .handlers.async_handler import AsyncBillzHandler
 from .handlers.handler import BillzHandler
 from .models.shops import ShopsListFilters, ShopsListData
 from .models.products import ProductsListFilters, ProductListData
 from .models.categories import CategoriesListFilters, CategoriesListData
 from .models.currencies import CurrenciesListData
```

### Comparing `billzio_api-1.0.6/billzio_api/handlers/async_handler.py` & `billzio_api-1.0.7/billzio_api/handlers/async_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,22 +93,25 @@
                                           json=data.model_dump(exclude_unset=True, exclude_none=True),
                                           headers=self._request_auth_headers())
         if resp.is_success:
             return True
         else:
             raise ContentUpdateError
 
-    async def create_order(self, data: NewOrderData) -> Optional[str]:
+    async def create_order(self, data: NewOrderData, finish=True) -> Optional[str]:
+        """ Creates a new draft order and attaches products and customer to it.
+            And if :finish is True then it will be marked as paid (finish) """
         await self._auth()
         order_id = await self._create_draft_order(data.shop_id)
         if order_id:
             for p in data.products:
                 await self._add_product_to_draft_order(order_id, p)
             await self._add_customer_to_draft_order(order_id, data.customer_id)
-            await self._finish_draft_order(order_id, data.payments)
+            if finish:
+                await self.finish_draft_order(order_id, data.payments)
         return order_id
 
     async def _create_draft_order(self, shop_id: str) -> Optional[str]:
         data = {
             "method": "order.create",
             "params": {
                 "shop_id": shop_id
@@ -158,15 +161,15 @@
 
         if resp.is_success:
             return True
         else:
             error = resp.json()
             raise ContentCreateError(error["error"]["message"])
 
-    async def _finish_draft_order(self, order_id: str, payments: List[NewOrderPayment]):
+    async def finish_draft_order(self, order_id: str, payments: List[NewOrderPayment]):
         data = {
             "method": "order.make_payment",
             "params": {
                 "payments": [p.model_dump() for p in payments],
                 "order_id": order_id
             }
         }
```

### Comparing `billzio_api-1.0.6/billzio_api/handlers/base.py` & `billzio_api-1.0.7/billzio_api/handlers/base.py`

 * *Files identical despite different names*

### Comparing `billzio_api-1.0.6/billzio_api/handlers/handler.py` & `billzio_api-1.0.7/billzio_api/handlers/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,21 +85,24 @@
                                     json=data.model_dump(exclude_unset=True, exclude_none=True),
                                     headers=self._request_auth_headers())
         if resp.is_success:
             return True
         else:
             raise ContentUpdateError
 
-    def create_order(self, data: NewOrderData) -> Optional[str]:
+    def create_order(self, data: NewOrderData, finish=True) -> Optional[str]:
+        """ Creates a new draft order and attaches products and customer to it.
+        And if :finish is True then it will be marked as paid (finish) """
         order_id = self._create_draft_order(data.shop_id)
         if order_id:
             for p in data.products:
                 self._add_product_to_draft_order(order_id, p)
             self._add_customer_to_draft_order(order_id, data.customer_id)
-            self._finish_draft_order(order_id, data.payments)
+            if finish:
+                self.finish_draft_order(order_id, data.payments)
         return order_id
 
     def _create_draft_order(self, shop_id: str) -> Optional[str]:
         data = {
             "method": "order.create",
             "params": {
                 "shop_id": shop_id
@@ -149,15 +152,15 @@
 
         if resp.is_success:
             return True
         else:
             error = resp.json()
             raise ContentCreateError(error["error"]["message"])
 
-    def _finish_draft_order(self, order_id: str, payments: List[NewOrderPayment]):
+    def finish_draft_order(self, order_id: str, payments: List[NewOrderPayment]):
         data = {
             "method": "order.make_payment",
             "params": {
                 "payments": [p.model_dump() for p in payments],
                 "order_id": order_id
             }
         }
```

### Comparing `billzio_api-1.0.6/billzio_api/models/categories.py` & `billzio_api-1.0.7/billzio_api/models/categories.py`

 * *Files identical despite different names*

### Comparing `billzio_api-1.0.6/billzio_api/models/clients.py` & `billzio_api-1.0.7/billzio_api/models/clients.py`

 * *Files identical despite different names*

### Comparing `billzio_api-1.0.6/billzio_api/models/products.py` & `billzio_api-1.0.7/billzio_api/models/products.py`

 * *Files 9% similar despite different names*

```diff
@@ -67,8 +67,9 @@
     products: List[Product]
 
 
 class ProductsListFilters(BaseModel):
     page: Optional[int] = None
     limit: Optional[int] = None
     search: Optional[str] = None
+    last_updated_date: Optional[str] = None  # format: yyyy-mm-dd 00:00:00
```

### Comparing `billzio_api-1.0.6/billzio_api/models/shops.py` & `billzio_api-1.0.7/billzio_api/models/shops.py`

 * *Files identical despite different names*

### Comparing `billzio_api-1.0.6/PKG-INFO` & `billzio_api-1.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: billzio-api
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python wrapper for Billz.io Public API
 License: Apache 2.0
 Author: Sirojiddin Mustafayev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: pydantic (>=2.1.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # billzio-api
 Asynchronous Python wrapper for [Billz.io](https://billz.io) Public API (v2)
```

