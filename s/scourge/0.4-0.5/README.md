# Comparing `tmp/scourge-0.4.tar.gz` & `tmp/scourge-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scourge-0.4.tar", last modified: Thu Feb 22 15:36:47 2024, max compression
+gzip compressed data, was "scourge-0.5.tar", last modified: Thu May 23 03:12:36 2024, max compression
```

## Comparing `scourge-0.4.tar` & `scourge-0.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-02-22 15:36:47.818956 scourge-0.4/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1071 2023-02-27 16:18:38.000000 scourge-0.4/LICENSE
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       82 2023-02-27 16:18:38.000000 scourge-0.4/MANIFEST.in
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2389 2024-02-22 15:36:47.818956 scourge-0.4/PKG-INFO
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      814 2023-02-27 16:18:38.000000 scourge-0.4/README.md
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       81 2023-12-20 08:09:13.000000 scourge-0.4/dev.txt
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-02-22 15:36:47.818956 scourge-0.4/scourge/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-27 16:18:38.000000 scourge-0.4/scourge/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      214 2023-02-27 16:18:38.000000 scourge-0.4/scourge/debug.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     5334 2023-02-27 16:18:38.000000 scourge-0.4/scourge/fedex.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1676 2024-02-22 15:36:16.000000 scourge-0.4/scourge/metro.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2538 2024-02-22 15:36:02.000000 scourge-0.4/scourge/metro_orders.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4491 2023-11-30 08:12:42.000000 scourge-0.4/scourge/pilot.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     5802 2023-09-08 15:56:21.000000 scourge-0.4/scourge/ups.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        3 2024-02-22 15:36:41.000000 scourge-0.4/scourge/version.txt
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-02-22 15:36:47.818956 scourge-0.4/scourge.egg-info/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2389 2024-02-22 15:36:47.000000 scourge-0.4/scourge.egg-info/PKG-INFO
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      347 2024-02-22 15:36:47.000000 scourge-0.4/scourge.egg-info/SOURCES.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2024-02-22 15:36:47.000000 scourge-0.4/scourge.egg-info/dependency_links.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       99 2024-02-22 15:36:47.000000 scourge-0.4/scourge.egg-info/requires.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        8 2024-02-22 15:36:47.000000 scourge-0.4/scourge.egg-info/top_level.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       38 2024-02-22 15:36:47.818956 scourge-0.4/setup.cfg
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2397 2023-12-19 16:00:48.000000 scourge-0.4/setup.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-05-23 03:12:36.099181 scourge-0.5/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1071 2023-02-27 16:18:38.000000 scourge-0.5/LICENSE
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       82 2023-02-27 16:18:38.000000 scourge-0.5/MANIFEST.in
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2385 2024-05-23 03:12:36.099181 scourge-0.5/PKG-INFO
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      810 2024-05-23 02:04:09.000000 scourge-0.5/README.md
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       81 2023-12-20 08:09:13.000000 scourge-0.5/dev.txt
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-05-23 03:12:36.089181 scourge-0.5/scourge/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-27 16:18:38.000000 scourge-0.5/scourge/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      214 2023-02-27 16:18:38.000000 scourge-0.5/scourge/debug.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     5334 2023-02-27 16:18:38.000000 scourge-0.5/scourge/fedex.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1416 2024-05-23 01:43:31.000000 scourge-0.5/scourge/metro.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2562 2024-05-23 01:50:28.000000 scourge-0.5/scourge/metro_orders.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     8825 2024-05-23 01:41:19.000000 scourge-0.5/scourge/non_stop_delivery.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4491 2023-11-30 08:12:42.000000 scourge-0.5/scourge/pilot.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     5802 2023-09-08 15:56:21.000000 scourge-0.5/scourge/ups.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        3 2024-05-23 03:12:28.000000 scourge-0.5/scourge/version.txt
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-05-23 03:12:36.099181 scourge-0.5/scourge.egg-info/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2385 2024-05-23 03:12:35.000000 scourge-0.5/scourge.egg-info/PKG-INFO
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      376 2024-05-23 03:12:35.000000 scourge-0.5/scourge.egg-info/SOURCES.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2024-05-23 03:12:35.000000 scourge-0.5/scourge.egg-info/dependency_links.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       99 2024-05-23 03:12:35.000000 scourge-0.5/scourge.egg-info/requires.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        8 2024-05-23 03:12:35.000000 scourge-0.5/scourge.egg-info/top_level.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       38 2024-05-23 03:12:36.099181 scourge-0.5/setup.cfg
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2397 2023-12-19 16:00:48.000000 scourge-0.5/setup.py
```

### Comparing `scourge-0.4/LICENSE` & `scourge-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scourge-0.4/PKG-INFO` & `scourge-0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scourge
-Version: 0.4
+Version: 0.5
 Summary: scourge
 Home-page: https://bitbucket.org/dbuy/scourge
 Author: dev
 Author-email: developers@directbuy.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -42,20 +42,17 @@
 # scourge
 
 scourge, named after a group of starlings, lets you get summary tracking
 information from various carriers.  currently supported carriers:
 
 * ups
 * fedex
-
-coming soon
-
-* tuscany
 * pilot
 * metropolitan
+* non-stop delivery
 
 used for wismo and wigmo.  powered by angry penguins.
 
 # notes
 
 * the summary tracking results are limited to dates because the ups api 
   only provides localized date/time information and does not provide time
```

### Comparing `scourge-0.4/README.md` & `scourge-0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 # scourge
 
 scourge, named after a group of starlings, lets you get summary tracking
 information from various carriers.  currently supported carriers:
 
 * ups
 * fedex
-
-coming soon
-
-* tuscany
 * pilot
 * metropolitan
+* non-stop delivery
 
 used for wismo and wigmo.  powered by angry penguins.
 
 # notes
 
 * the summary tracking results are limited to dates because the ups api 
   only provides localized date/time information and does not provide time
```

### Comparing `scourge-0.4/scourge/fedex.py` & `scourge-0.5/scourge/fedex.py`

 * *Files identical despite different names*

### Comparing `scourge-0.4/scourge/metro.py` & `scourge-0.5/scourge/metro.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,20 +33,13 @@
         route = 'GetTransitHistory'
         json_data = {
             'trackingNumber': tracking_number,
             'timezone': timezone
         }
         return self.post(route, json_data=json_data, **kwargs)
 
-    def invoice_data(self, tracking_number, **kwargs):
-        url = 'https://api.gomwd.com/order/GetOrderInvoiceData'
-        json_data = {
-            'trackingNumber': tracking_number,
-        }
-        return self.post(url, json_data=json_data, **kwargs)
-
     def tracking_details(self, tracking_number, **kwargs):
         route = 'GetTrackingDetails'
         json_data = {
             'trackingNumber': tracking_number,
         }
         return self.post(route, json_data=json_data, **kwargs)
```

### Comparing `scourge-0.4/scourge/metro_orders.py` & `scourge-0.5/scourge/metro_orders.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import time
 from deceit.api_client import ApiClient
 from deceit.exceptions import ApiException
-import time
+
 
 class MetroApiException(ApiException):
     pass
 
+
 class MetroApiOrders(ApiClient):
     def __init__(self, conf, *args, base_url=None, password=None, client_id=None,
                  username=None, default_timeout=None, **kwargs):
         base_url = base_url or conf.get('base_url')
         super().__init__(*args, base_url=base_url or conf.get('base_url'),
                          default_timeout=default_timeout or conf.get('default_timeout'),
                          exception_class=MetroApiException, **kwargs)
@@ -32,17 +34,18 @@
         }
 
         # Set headers directly for authentication to avoid recursion
         headers = {
             'Content-Type': 'application/x-www-form-urlencoded'
         }
 
-        # Use the session's post method directly for authentication to bypass the custom headers logic
+        # Use the session's post method directly for authentication to bypass
+        # the custom headers logic
         response = self.session.post(route, data=form_data, headers=headers)
-        print(f'response: {response.status_code}')
+        self.log.info('response: %s', response.status_code)
         if response.status_code == 200:
             response_data = response.json()
             self.token = response_data['access_token']
             self.token_expiry = time.time() + response_data['expires_in']
         else:
             raise MetroApiException(f"Authentication failed: {response.text}")
```

### Comparing `scourge-0.4/scourge/pilot.py` & `scourge-0.5/scourge/pilot.py`

 * *Files identical despite different names*

### Comparing `scourge-0.4/scourge/ups.py` & `scourge-0.5/scourge/ups.py`

 * *Files identical despite different names*

### Comparing `scourge-0.4/scourge.egg-info/PKG-INFO` & `scourge-0.5/scourge.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scourge
-Version: 0.4
+Version: 0.5
 Summary: scourge
 Home-page: https://bitbucket.org/dbuy/scourge
 Author: dev
 Author-email: developers@directbuy.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -42,20 +42,17 @@
 # scourge
 
 scourge, named after a group of starlings, lets you get summary tracking
 information from various carriers.  currently supported carriers:
 
 * ups
 * fedex
-
-coming soon
-
-* tuscany
 * pilot
 * metropolitan
+* non-stop delivery
 
 used for wismo and wigmo.  powered by angry penguins.
 
 # notes
 
 * the summary tracking results are limited to dates because the ups api 
   only provides localized date/time information and does not provide time
```

### Comparing `scourge-0.4/setup.py` & `scourge-0.5/setup.py`

 * *Files identical despite different names*

