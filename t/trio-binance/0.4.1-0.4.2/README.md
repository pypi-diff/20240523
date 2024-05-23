# Comparing `tmp/trio_binance-0.4.1.tar.gz` & `tmp/trio_binance-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trio_binance-0.4.1.tar", max compression
+gzip compressed data, was "trio_binance-0.4.2.tar", max compression
```

## Comparing `trio_binance-0.4.1.tar` & `trio_binance-0.4.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2021-11-18 07:43:08.000000 trio_binance-0.4.1/LICENSE
--rwxr-xr-x   0        0        0     1143 2022-01-12 05:13:36.000000 trio_binance-0.4.1/README.rst
--rw-r--r--   0        0        0     1080 2024-05-20 01:43:11.707867 trio_binance-0.4.1/pyproject.toml
--rwxr-xr-x   0        0        0       67 2024-05-20 01:43:15.853942 trio_binance-0.4.1/trio_binance/__init__.py
--rwxr-xr-x   0        0        0    79811 2024-05-16 06:18:42.288051 trio_binance-0.4.1/trio_binance/client.py
--rw-r--r--   0        0        0     1891 2024-04-23 01:56:20.850456 trio_binance-0.4.1/trio_binance/enums.py
--rw-r--r--   0        0        0     2260 2024-04-23 02:07:31.211547 trio_binance-0.4.1/trio_binance/exceptions.py
--rw-r--r--   0        0        0     1493 2024-04-23 02:07:31.211671 trio_binance-0.4.1/trio_binance/helpers.py
--rw-r--r--   0        0        0     3780 2024-04-23 05:34:24.595456 trio_binance-0.4.1/trio_binance/streams.py
--rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 trio_binance-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2021-11-18 07:43:08.000000 trio_binance-0.4.2/LICENSE
+-rwxr-xr-x   0        0        0     1143 2022-01-12 05:13:36.000000 trio_binance-0.4.2/README.rst
+-rw-r--r--   0        0        0     1080 2024-05-23 07:51:39.029096 trio_binance-0.4.2/pyproject.toml
+-rwxr-xr-x   0        0        0       67 2024-05-23 07:51:30.830255 trio_binance-0.4.2/trio_binance/__init__.py
+-rwxr-xr-x   0        0        0    79952 2024-05-23 07:45:39.337411 trio_binance-0.4.2/trio_binance/client.py
+-rw-r--r--   0        0        0     1891 2024-04-23 01:56:20.850456 trio_binance-0.4.2/trio_binance/enums.py
+-rw-r--r--   0        0        0     2260 2024-04-23 02:07:31.211547 trio_binance-0.4.2/trio_binance/exceptions.py
+-rw-r--r--   0        0        0     1493 2024-04-23 02:07:31.211671 trio_binance-0.4.2/trio_binance/helpers.py
+-rw-r--r--   0        0        0     3780 2024-04-23 05:34:24.595456 trio_binance-0.4.2/trio_binance/streams.py
+-rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 trio_binance-0.4.2/PKG-INFO
```

### Comparing `trio_binance-0.4.1/LICENSE` & `trio_binance-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trio_binance-0.4.1/README.rst` & `trio_binance-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `trio_binance-0.4.1/pyproject.toml` & `trio_binance-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trio-binance"
-version = "0.4.1"
+version = "0.4.2"
 description = "trio based asynchronous binance SDK"
 authors = ["Shu Wang <halfelf.ronin@gmail.com>"]
 keywords = ["binance", "python-trio"]
 readme = "README.rst"
 license = "MIT"
 homepage = "https://github.com/halfelf/trio-binance"
 repository = "https://github.com/halfelf/trio-binance"
```

### Comparing `trio_binance-0.4.1/trio_binance/client.py` & `trio_binance-0.4.2/trio_binance/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -654,14 +654,17 @@
 
     async def get_account_api_permissions(self, **params):
         return await self._request_margin_api("get", "account/apiRestrictions", True, data=params)
 
     async def get_dust_log(self, **params):
         return await self._request_margin_api("get", "asset/dribblet", True, data=params)
 
+    async def get_dustable_list(self, **params):
+        return await self._request_margin_api("post", "asset/dust-btc", True, data=params)
+
     async def transfer_dust(self, **params):
         return await self._request_margin_api("post", "asset/dust", True, data=params)
 
     async def get_asset_dividend_history(self, **params):
         return await self._request_margin_api("get", "asset/assetDividend", True, data=params)
 
     async def make_universal_transfer(self, **params):
```

### Comparing `trio_binance-0.4.1/trio_binance/enums.py` & `trio_binance-0.4.2/trio_binance/enums.py`

 * *Files identical despite different names*

### Comparing `trio_binance-0.4.1/trio_binance/exceptions.py` & `trio_binance-0.4.2/trio_binance/exceptions.py`

 * *Files identical despite different names*

### Comparing `trio_binance-0.4.1/trio_binance/helpers.py` & `trio_binance-0.4.2/trio_binance/helpers.py`

 * *Files identical despite different names*

### Comparing `trio_binance-0.4.1/trio_binance/streams.py` & `trio_binance-0.4.2/trio_binance/streams.py`

 * *Files identical despite different names*

### Comparing `trio_binance-0.4.1/PKG-INFO` & `trio_binance-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trio-binance
-Version: 0.4.1
+Version: 0.4.2
 Summary: trio based asynchronous binance SDK
 Home-page: https://github.com/halfelf/trio-binance
 License: MIT
 Keywords: binance,python-trio
 Author: Shu Wang
 Author-email: halfelf.ronin@gmail.com
 Requires-Python: >=3.11,<4.0
```

