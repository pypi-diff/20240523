# Comparing `tmp/aguasgaia-0.0.14.tar.gz` & `tmp/aguasgaia-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aguasgaia-0.0.14.tar", last modified: Thu May 16 19:33:29 2024, max compression
+gzip compressed data, was "aguasgaia-0.0.17.tar", last modified: Wed May 22 22:14:13 2024, max compression
```

## Comparing `aguasgaia-0.0.14.tar` & `aguasgaia-0.0.17.tar`

### file list

```diff
@@ -1,23 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:33:29.586027 aguasgaia-0.0.14/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-16 19:33:25.000000 aguasgaia-0.0.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-16 19:33:29.586027 aguasgaia-0.0.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-16 19:33:25.000000 aguasgaia-0.0.14/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:33:29.582027 aguasgaia-0.0.14/aguasgaia/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 19:33:25.000000 aguasgaia-0.0.14/aguasgaia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-16 19:33:25.000000 aguasgaia-0.0.14/aguasgaia/aguasgaia.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-16 19:33:25.000000 aguasgaia-0.0.14/aguasgaia/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:33:29.582027 aguasgaia-0.0.14/aguasgaia/models/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-16 19:33:25.000000 aguasgaia-0.0.14/aguasgaia/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-16 19:33:25.000000 aguasgaia-0.0.14/aguasgaia/models/consumption.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-16 19:33:25.000000 aguasgaia-0.0.14/aguasgaia/models/invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:33:29.586027 aguasgaia-0.0.14/aguasgaia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-16 19:33:29.000000 aguasgaia-0.0.14/aguasgaia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-16 19:33:29.000000 aguasgaia-0.0.14/aguasgaia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:33:29.000000 aguasgaia-0.0.14/aguasgaia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 19:33:29.000000 aguasgaia-0.0.14/aguasgaia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 19:33:29.000000 aguasgaia-0.0.14/aguasgaia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-16 19:33:25.000000 aguasgaia-0.0.14/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 19:33:29.586027 aguasgaia-0.0.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-16 19:33:25.000000 aguasgaia-0.0.14/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:33:29.586027 aguasgaia-0.0.14/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-05-16 19:33:25.000000 aguasgaia-0.0.14/tests/aguasgaia_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:13.773187 aguasgaia-0.0.17/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-22 22:14:09.000000 aguasgaia-0.0.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-22 22:14:13.773187 aguasgaia-0.0.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-22 22:14:09.000000 aguasgaia-0.0.17/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:13.769187 aguasgaia-0.0.17/aguasgaia/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 22:14:09.000000 aguasgaia-0.0.17/aguasgaia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-22 22:14:09.000000 aguasgaia-0.0.17/aguasgaia/aguasgaia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-22 22:14:09.000000 aguasgaia-0.0.17/aguasgaia/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:13.769187 aguasgaia-0.0.17/aguasgaia/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-22 22:14:09.000000 aguasgaia-0.0.17/aguasgaia/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-22 22:14:09.000000 aguasgaia-0.0.17/aguasgaia/models/consumption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-22 22:14:09.000000 aguasgaia-0.0.17/aguasgaia/models/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-22 22:14:09.000000 aguasgaia-0.0.17/aguasgaia/models/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:13.769187 aguasgaia-0.0.17/aguasgaia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-22 22:14:13.000000 aguasgaia-0.0.17/aguasgaia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-22 22:14:13.000000 aguasgaia-0.0.17/aguasgaia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:14:13.000000 aguasgaia-0.0.17/aguasgaia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 22:14:13.000000 aguasgaia-0.0.17/aguasgaia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 22:14:13.000000 aguasgaia-0.0.17/aguasgaia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-22 22:14:09.000000 aguasgaia-0.0.17/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 22:14:13.773187 aguasgaia-0.0.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-22 22:14:09.000000 aguasgaia-0.0.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:13.765187 aguasgaia-0.0.17/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:13.769187 aguasgaia-0.0.17/src/aguasgaia/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 22:14:09.000000 aguasgaia-0.0.17/src/aguasgaia/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:13.769187 aguasgaia-0.0.17/src/aguasgaia/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-22 22:14:09.000000 aguasgaia-0.0.17/src/aguasgaia/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-22 22:14:09.000000 aguasgaia-0.0.17/src/aguasgaia/models/consumption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-22 22:14:09.000000 aguasgaia-0.0.17/src/aguasgaia/models/invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:14:13.769187 aguasgaia-0.0.17/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-22 22:14:09.000000 aguasgaia-0.0.17/tests/aguasgaia_test.py
```

### Comparing `aguasgaia-0.0.14/LICENSE` & `aguasgaia-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `aguasgaia-0.0.14/PKG-INFO` & `aguasgaia-0.0.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aguasgaia
-Version: 0.0.14
+Version: 0.0.17
 Summary: Python library to retrieve information from "Aguas de Gaia" portal
 Author-email: Jose Rolo <ze.p.rolo@gmail.com>
 License: Apache-2.0
 Keywords: api,aguasgaia
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `aguasgaia-0.0.14/README.md` & `aguasgaia-0.0.17/README.md`

 * *Files identical despite different names*

### Comparing `aguasgaia-0.0.14/aguasgaia/aguasgaia.py` & `aguasgaia-0.0.17/aguasgaia/aguasgaia.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,68 @@
 import logging
 from datetime import datetime
+
 from dateutil.relativedelta import relativedelta
 
 from .const import DEFAULT_HEADERS, ENDPOINT, INVOICEHISTORY_ENDDATE_PARAM, INVOICEHISTORY_PATH, \
     INVOICEHISTORY_STARTDATE_PARAM, INVOICEHISTORY_SUBSCRIPTION_PARAM, JSON_CONTENT, LASTDOC_PATH, \
-    LASTDOC_SUBSCRIPTION_PARAM, LOGIN_PATH, PWD_PARAM, SUBSCRIPTIONS_PATH, USER_PARAM, LASTCONSUMPTION_PATH, \
+    LOGIN_PATH, PWD_PARAM, SUBSCRIPTIONS_PATH, USER_PARAM, LASTCONSUMPTION_PATH, \
     LASTCONSUMPTION_SUBSCRIPTION_PARAM
-from .models import Consumption, Invoice
+from .models import Consumption, Invoice, Subscription
 
 _LOGGER = logging.getLogger(__name__)
 _LOGGER.setLevel(logging.DEBUG)
 
 
 class AguasGaia:
 
-    def __init__(self, websession, username, password, subscription_id):
+    def __init__(self, websession, username, password, subscription_id=None):
         self._last_invoice = None
         self._last_consumption = None
         self._invoice_history = None
         self._selected_subscription_id = subscription_id
         self._subscriptions = None
         self._session_cookies = None
         self._token = None
         self._websession = websession
         self._username = username
         self._password = password
 
-    async def __api_request(self, url: str, method="get", data=None, return_cookies=False):
-        async with getattr(self._websession, method)(url, headers=self.__get_auth_headers(), json=data) as response:
+    async def __api_request(self, url: str, method="get", data=None, return_cookies=False, params=None):
+        async with getattr(self._websession, method)(url, headers=self.__get_auth_headers(), json=data,
+                                                     params=params) as response:
             try:
                 if response.status == 200 and response.content_type == JSON_CONTENT:
                     json_response = await response.json()
                     if return_cookies:
                         return {
                             "response": json_response,
                             "cookies": response.cookies
                         }
                     return json_response
                 else:
-                    raise Exception("HTTP Request Error: %s", str(response.status)+" "+str(response.content_type))
+                    raise Exception(f"HTTP Request Error: %s", str(response.status) + " " + str(response.content_type))
             except Exception as err:
-                _LOGGER.error("API request error: %s", err)
+                _LOGGER.error(f"API request error: %s", err)
                 return None
 
     def __get_auth_headers(self):
         _LOGGER.debug("AguasGaia API AuthHeaders")
         headers = {**DEFAULT_HEADERS}
         if self._token is not None:
             headers["X-Auth-Token"] = self._token
         if self._session_cookies is not None:
             headers["Cookie"] = self._session_cookies
         return headers
 
-    def get_subscription(self):
-        return self._selected_subscription_id
+    def get_selected_subscription(self):
+        return str(self._selected_subscription_id)
+
+    def set_selected_subscription(self, sub: Subscription):
+        self._selected_subscription_id = sub.subscription_id
 
     async def login(self):
         _LOGGER.debug("AguasGaia API Login")
         url = ENDPOINT + LOGIN_PATH
 
         data = {
             USER_PARAM: self._username,
@@ -65,80 +70,81 @@
         }
 
         res = await self.__api_request(url, method="post", data=data, return_cookies=True)
         if res is not None:
             self._token = res.get("response", {}).get("token", {}).get("token", None)
             cookies = res.get("cookies", [])
             self._session_cookies = "".join([cookies[x].key + "=" + cookies[x].value + ";" for x in cookies])
-            if self._token is not None and self._session_cookies is not None:
-                return True
-        return False
+            if self._token is None or self._session_cookies is None:
+                return False
+
+        if self._selected_subscription_id is None:
+            subscriptions = await self.get_subscriptions()
+            if subscriptions is None or len(subscriptions) == 0:
+                return False
+            self.set_selected_subscription(subscriptions.pop())
+        return True
 
-    async def get_subscriptions(self):
+    async def get_subscriptions(self) -> list[Subscription]:
         _LOGGER.debug("AguasGaia API Subscriptions")
 
         url = ENDPOINT + SUBSCRIPTIONS_PATH
-
-        self._subscriptions = await self.__api_request(url)
+        subscription_payload = await self.__api_request(url)
+        self._subscriptions = [Subscription(sub) for sub in await self.__api_request(url)]
         return self._subscriptions
 
     async def get_last_invoice(self, subscription_id=None) -> Invoice:
         _LOGGER.debug("AguasGaia API LastDocData")
 
         subscription_id = subscription_id or self._selected_subscription_id
 
-        url = ENDPOINT + LASTDOC_PATH + "?" + LASTDOC_SUBSCRIPTION_PARAM + "=" + subscription_id
+        url = ENDPOINT + LASTDOC_PATH
 
-        invoice = await self.__api_request(url)
+        invoice_payload = await self.__api_request(url, params={LASTCONSUMPTION_SUBSCRIPTION_PARAM: subscription_id})
 
-        self._last_invoice = Invoice(
-            invoice_value=invoice[0]["dadosPagamento"]["valor"],
-            invoice_attributes=invoice[0]
-        )
+        self._last_invoice = Invoice(invoice_payload)
         return self._last_invoice
 
     async def get_invoice_history(self, subscription_id=None):
         _LOGGER.debug("AguasGaia API Invoice History")
 
         subscription_id = subscription_id or self._selected_subscription_id
 
         today = datetime.now()
         year_ago = today - relativedelta(years=1)
-        url = "{url}?{param1}={param1_value}&{param2}={param2_value}&{param3}={param3_value}".format(
-            url=ENDPOINT + INVOICEHISTORY_PATH,
-            param1=INVOICEHISTORY_ENDDATE_PARAM,
-            param1_value="{year}-{month}-{day}".format(
-                year=today.year,
-                month=today.month,
-                day=today.day
-            ),
-            param2=INVOICEHISTORY_STARTDATE_PARAM,
-            param2_value="{year}-{month}-{day}".format(
-                year=year_ago.year,
-                month=year_ago.month,
-                day=year_ago.day
-            ),
-            param3=INVOICEHISTORY_SUBSCRIPTION_PARAM,
-            param3_value=subscription_id
-        )
+        url = ENDPOINT + INVOICEHISTORY_PATH
 
-        self._invoice_history = await self.__api_request(url)
+        self._invoice_history = await self.__api_request(
+            url,
+            params={
+                INVOICEHISTORY_ENDDATE_PARAM: "{year}-{month}-{day}".format(
+                    year=today.year,
+                    month=today.month,
+                    day=today.day
+                ),
+                INVOICEHISTORY_STARTDATE_PARAM: "{year}-{month}-{day}".format(
+                    year=year_ago.year,
+                    month=year_ago.month,
+                    day=year_ago.day
+                ),
+                INVOICEHISTORY_SUBSCRIPTION_PARAM: subscription_id
+            }
+        )
         return self._invoice_history
 
     async def get_last_consumption(self, subscription_id=None) -> Consumption:
         _LOGGER.debug("AguasGaia API Last Consumption")
 
         subscription_id = subscription_id or self._selected_subscription_id
 
-        url = ENDPOINT + LASTCONSUMPTION_PATH + "?" + LASTCONSUMPTION_SUBSCRIPTION_PARAM + "=" + subscription_id
+        url = ENDPOINT + LASTCONSUMPTION_PATH
 
-        self._last_consumption = await self.__api_request(url)
+        last_consumption_payload = await self.__api_request(
+            url,
+            params={LASTCONSUMPTION_SUBSCRIPTION_PARAM: subscription_id})
 
-        if len(self._last_consumption[0]["funcoesContador"]) != 0:
-            return Consumption(
-                consumption_value=self._last_consumption[0]["funcoesContador"][0]["ultimaLeitura"],
-                consumption_attributes=self._last_consumption[0]
-            )
-        else:
-            raise Exception("No consumption data found")
+        self._last_consumption = Consumption(last_consumption_payload)
 
+        if self._last_consumption.consumption_value == 0 and self._last_consumption.consumption_attributes == {}:
+            raise Exception("No consumption data found")
 
+        return self._last_consumption
```

### Comparing `aguasgaia-0.0.14/aguasgaia/const.py` & `aguasgaia-0.0.17/aguasgaia/const.py`

 * *Files identical despite different names*

### Comparing `aguasgaia-0.0.14/aguasgaia.egg-info/PKG-INFO` & `aguasgaia-0.0.17/aguasgaia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aguasgaia
-Version: 0.0.14
+Version: 0.0.17
 Summary: Python library to retrieve information from "Aguas de Gaia" portal
 Author-email: Jose Rolo <ze.p.rolo@gmail.com>
 License: Apache-2.0
 Keywords: api,aguasgaia
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `aguasgaia-0.0.14/tests/aguasgaia_test.py` & `aguasgaia-0.0.17/tests/aguasgaia_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pytest
 import aiohttp
 from unittest.mock import MagicMock
 from http.cookies import SimpleCookie
 
 from aguasgaia import AguasGaia
+from aguasgaia.models import Subscription
 
 
 def create_mock(status_code, get_json_response, post_json_response, cookies):
     mock = aiohttp.ClientSession()
     mock.post = MagicMock()
     mock.post.return_value.__aenter__.return_value.status = status_code
     mock.post.return_value.__aenter__.return_value.content_type = "application/json"
@@ -31,17 +32,28 @@
         }
     }
     token_no_response = {
         "no_token": {
             "no_token": "my_token"
         }
     }
-    subscriptions_response = {
-        "subscriptions": ["SUB1", "SUB2"]
-    }
+    subscriptions_response = [
+        {
+            "subscriptionId": "456454",
+            "clientAddress": "PT",
+            "activationDate": "today",
+            "isActive": True
+        },
+        {
+            "subscriptionId": "1236453",
+            "clientAddress": "PT",
+            "activationDate": "tomorrow",
+            "isActive": False
+        }
+    ]
     invoice_response = [
         {
             "dadosPagamento": {
                 "valor": "999"
             }
         }
     ]
@@ -60,89 +72,67 @@
     cookies.__setitem__("COOKIE2", "B")
 
     mock_post_get_subscriptions = create_mock(200, subscriptions_response, token_response, cookies)
     mock_post_get_last_invoice = create_mock(200, invoice_response, token_response, cookies)
     mock_post_get_last_consumption = create_mock(200, consumption_response, token_response, cookies)
     mock_post_failure = create_mock(200, subscriptions_response, token_no_response, cookies)
 
-    '''
-    mock_post_success = aiohttp.ClientSession()
-    mock_post_success.post = MagicMock()
-    mock_post_success.post.return_value.__aenter__.return_value.status = 200
-    mock_post_success.post.return_value.__aenter__.return_value.content_type = "application/json"
-    mock_post_success.post.return_value.__aenter__.return_value.json.return_value = {
-        "token": {
-            "token": "my_token"
-        }
-    }
-    
-    
-    mock_post_failure = aiohttp.ClientSession()
-    mock_post_failure.post = MagicMock()
-    mock_post_failure.post.return_value.__aenter__.return_value.status = 200
-    mock_post_failure.post.return_value.__aenter__.return_value.content_type = "application/json"
-    mock_post_failure.post.return_value.__aenter__.return_value.json.return_value = {
-        "no_token": {
-            "no_token": "my_token"
-        }
-    }
-    '''
-
     yield {
         "post_get_success": mock_post_get_subscriptions,
         "mock_post_get_last_invoice": mock_post_get_last_invoice,
         "mock_post_get_last_consumption": mock_post_get_last_consumption,
         "post_failure": mock_post_failure
     }
 
 
 @pytest.mark.asyncio
 async def test_login_success(setup_mocks):
     mock = setup_mocks.get("post_get_success")
 
-    aguas = AguasGaia(mock, "", "", "123")
+    aguas = AguasGaia(mock, "", "")
     response = await aguas.login()
 
     assert response
 
     await mock.close()
 
 
 @pytest.mark.asyncio
 async def test_login_failed(setup_mocks):
     mock = setup_mocks.get("post_failure")
 
-    aguas = AguasGaia(mock, "", "", "")
+    aguas = AguasGaia(mock, "", "")
     response = await aguas.login()
 
     assert not response
 
     await mock.close()
 
 
 @pytest.mark.asyncio
 async def test_get_subscriptions_success(setup_mocks):
     mock_post_get_success = setup_mocks.get("post_get_success")
 
-    aguas = AguasGaia(mock_post_get_success, "", "", "")
+    aguas = AguasGaia(mock_post_get_success, "", "")
 
     response = await aguas.login()
     assert response
 
     subscriptions = await aguas.get_subscriptions()
-    assert subscriptions.get("subscriptions", None) == ["SUB1", "SUB2"]
+    assert len(subscriptions) == 2
+    assert subscriptions[0].subscription_id == "456454" or subscriptions[0].subscription_id == "1236453"
 
     await mock_post_get_success.close()
 
 
 @pytest.mark.asyncio
 async def test_get_last_invoice_success(setup_mocks):
     mock_post_get_last_invoice = setup_mocks.get("mock_post_get_last_invoice")
 
-    aguas = AguasGaia(mock_post_get_last_invoice, "", "", "")
+    aguas = AguasGaia(mock_post_get_last_invoice, "", "")
 
     response = await aguas.login()
     assert response
 
     invoice = await aguas.get_last_invoice()
 
     assert invoice is not None
@@ -151,15 +141,15 @@
     await mock_post_get_last_invoice.close()
 
 
 @pytest.mark.asyncio
 async def test_get_invoice_history_success(setup_mocks):
     mock_post_get_last_invoice = setup_mocks.get("mock_post_get_last_invoice")
 
-    aguas = AguasGaia(mock_post_get_last_invoice, "", "", "")
+    aguas = AguasGaia(mock_post_get_last_invoice, "", "")
 
     response = await aguas.login()
     assert response
 
     invoices = await aguas.get_invoice_history()
 
     assert invoices is not None
@@ -167,15 +157,15 @@
     await mock_post_get_last_invoice.close()
 
 
 @pytest.mark.asyncio
 async def test_get_last_consumption_success(setup_mocks):
     mock_post_get_last_consumption = setup_mocks.get("mock_post_get_last_consumption")
 
-    aguas = AguasGaia(mock_post_get_last_consumption, "", "", "")
+    aguas = AguasGaia(mock_post_get_last_consumption, "", "")
 
     response = await aguas.login()
     assert response
 
     consumption = await aguas.get_last_consumption()
 
     assert consumption is not None
```

