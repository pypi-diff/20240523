# Comparing `tmp/reversinglabs_sdk_py3-2.5.5.tar.gz` & `tmp/reversinglabs_sdk_py3-2.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reversinglabs_sdk_py3-2.5.5.tar", last modified: Wed May 15 12:28:01 2024, max compression
+gzip compressed data, was "reversinglabs_sdk_py3-2.5.6.tar", last modified: Thu May 23 15:05:56 2024, max compression
```

## Comparing `reversinglabs_sdk_py3-2.5.5.tar` & `reversinglabs_sdk_py3-2.5.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:28:01.767688 reversinglabs_sdk_py3-2.5.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11004 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    46144 2024-05-15 12:28:01.767688 reversinglabs_sdk_py3-2.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    44788 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:28:01.763688 reversinglabs_sdk_py3-2.5.5/ReversingLabs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:28:01.763688 reversinglabs_sdk_py3-2.5.5/ReversingLabs/SDK/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/ReversingLabs/SDK/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    96422 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/ReversingLabs/SDK/a1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/ReversingLabs/SDK/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)   250906 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/ReversingLabs/SDK/ticloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    16866 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/ReversingLabs/SDK/tiscale.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/ReversingLabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:28:01.767688 reversinglabs_sdk_py3-2.5.5/reversinglabs_sdk_py3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    46144 2024-05-15 12:28:01.000000 reversinglabs_sdk_py3-2.5.5/reversinglabs_sdk_py3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-15 12:28:01.000000 reversinglabs_sdk_py3-2.5.5/reversinglabs_sdk_py3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:28:01.000000 reversinglabs_sdk_py3-2.5.5/reversinglabs_sdk_py3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:28:01.000000 reversinglabs_sdk_py3-2.5.5/reversinglabs_sdk_py3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-15 12:28:01.000000 reversinglabs_sdk_py3-2.5.5/reversinglabs_sdk_py3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 12:28:01.000000 reversinglabs_sdk_py3-2.5.5/reversinglabs_sdk_py3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-15 12:28:01.767688 reversinglabs_sdk_py3-2.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:28:01.767688 reversinglabs_sdk_py3-2.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/tests/test_a1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/tests/test_ticloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/tests/test_tiscale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:05:56.177977 reversinglabs_sdk_py3-2.5.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-05-23 15:05:52.000000 reversinglabs_sdk_py3-2.5.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-23 15:05:52.000000 reversinglabs_sdk_py3-2.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 15:05:52.000000 reversinglabs_sdk_py3-2.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    46144 2024-05-23 15:05:56.177977 reversinglabs_sdk_py3-2.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    44788 2024-05-23 15:05:52.000000 reversinglabs_sdk_py3-2.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:05:56.173977 reversinglabs_sdk_py3-2.5.6/ReversingLabs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:05:56.173977 reversinglabs_sdk_py3-2.5.6/ReversingLabs/SDK/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-23 15:05:52.000000 reversinglabs_sdk_py3-2.5.6/ReversingLabs/SDK/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102315 2024-05-23 15:05:52.000000 reversinglabs_sdk_py3-2.5.6/ReversingLabs/SDK/a1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-05-23 15:05:52.000000 reversinglabs_sdk_py3-2.5.6/ReversingLabs/SDK/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)   250906 2024-05-23 15:05:52.000000 reversinglabs_sdk_py3-2.5.6/ReversingLabs/SDK/ticloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16866 2024-05-23 15:05:52.000000 reversinglabs_sdk_py3-2.5.6/ReversingLabs/SDK/tiscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:05:52.000000 reversinglabs_sdk_py3-2.5.6/ReversingLabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-23 15:05:52.000000 reversinglabs_sdk_py3-2.5.6/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:05:56.177977 reversinglabs_sdk_py3-2.5.6/reversinglabs_sdk_py3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    46144 2024-05-23 15:05:56.000000 reversinglabs_sdk_py3-2.5.6/reversinglabs_sdk_py3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-23 15:05:56.000000 reversinglabs_sdk_py3-2.5.6/reversinglabs_sdk_py3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:05:56.000000 reversinglabs_sdk_py3-2.5.6/reversinglabs_sdk_py3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:05:56.000000 reversinglabs_sdk_py3-2.5.6/reversinglabs_sdk_py3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-23 15:05:56.000000 reversinglabs_sdk_py3-2.5.6/reversinglabs_sdk_py3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 15:05:56.000000 reversinglabs_sdk_py3-2.5.6/reversinglabs_sdk_py3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-23 15:05:56.177977 reversinglabs_sdk_py3-2.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-23 15:05:52.000000 reversinglabs_sdk_py3-2.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:05:56.177977 reversinglabs_sdk_py3-2.5.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-23 15:05:52.000000 reversinglabs_sdk_py3-2.5.6/tests/test_a1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-23 15:05:52.000000 reversinglabs_sdk_py3-2.5.6/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-23 15:05:52.000000 reversinglabs_sdk_py3-2.5.6/tests/test_ticloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-23 15:05:52.000000 reversinglabs_sdk_py3-2.5.6/tests/test_tiscale.py
```

### Comparing `reversinglabs_sdk_py3-2.5.5/CHANGELOG.md` & `reversinglabs_sdk_py3-2.5.6/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -267,7 +267,15 @@
 
 2.5.5 (2024-05-15)
 -------------------
 
 #### Bugfixes
 - **a1000** module:
   - Changed the `risk_score` parameter's type hint from `str` to `int` in `set_classification` method's docstring.
+
+
+2.5.6 (2024-05-23)
+-------------------
+
+#### Improvements
+- **a1000** module:
+  - Reintroduced the `a1000.A1000.advanced_search_v2` method. This method will remain in the DEPRECATED state until its permanent removal from the SDK. The permanent removal date will be announced in the CHANGELOG's "Scheduled removals" section. In the meantime, the use of `a1000.A1000.advanced_search_v3` is highly advised.
```

### Comparing `reversinglabs_sdk_py3-2.5.5/LICENSE` & `reversinglabs_sdk_py3-2.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.5/PKG-INFO` & `reversinglabs_sdk_py3-2.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reversinglabs-sdk-py3
-Version: 2.5.5
+Version: 2.5.6
 Summary: Python SDK for using ReversingLabs services.
 Home-page: https://github.com/reversinglabs/reversinglabs-sdk-py3
 Author: ReversingLabs
 Author-email: support@reversinglabs.com
 License: MIT
 Project-URL: Documentation, https://github.com/reversinglabs/reversinglabs-sdk-py3/blob/main/README.md
 Project-URL: Source, https://github.com/reversinglabs/reversinglabs-sdk-py3
```

### Comparing `reversinglabs_sdk_py3-2.5.5/README.md` & `reversinglabs_sdk_py3-2.5.6/README.md`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.5/ReversingLabs/SDK/a1000.py` & `reversinglabs_sdk_py3-2.5.6/ReversingLabs/SDK/a1000.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 A Python module for the ReversingLabs A1000 appliance REST API.
 """
 
 import datetime
 import requests
 import time
 from urllib import parse
+from warnings import warn
 
 from ReversingLabs.SDK.helper import ADVANCED_SEARCH_SORTING_CRITERIA, DEFAULT_USER_AGENT, RESPONSE_CODE_ERROR_MAP, \
     MD5, SHA1, SHA256, SHA512, \
     RequestTimeoutError, WrongInputError, \
     validate_hashes
 
 
@@ -1591,14 +1592,139 @@
 
         response = self.__get_request(url=url)
 
         self.__raise_on_error(response)
 
         return response
 
+    def advanced_search_v2(self, query_string, ticloud=False, page_number=1, records_per_page=20, sorting_criteria=None,
+                           sorting_order="desc"):
+        """THIS METHOD IS DEPRECATED. Use advanced_search_v3 instead.
+
+        Sends a query string to the A1000 Advanced Search API v2.
+        The query string must be composed of key-value pairs separated by space.
+        A key is separated from its value by a colon symbol and no spaces.
+        For directions on how to write advanced search queries, consult the A1000 documentation.
+        If a page number is not provided, the first page of results will be returned.
+            Query string example:
+            'av-count:5 available:TRUE'
+
+            :param query_string: query string
+            :type query_string: str
+            :param ticloud: show only cloud results
+            :type ticloud: bool
+            :param page_number: page number
+            :type page_number: int
+            :param records_per_page: number of records returned per page; maximum value is 100
+            :type records_per_page: int
+            :param sorting_criteria: define the criteria used in sorting; possible values are 'sha1', 'firstseen',
+            'threatname', 'sampletype', 'filecount', 'size'
+            :type sorting_criteria: str
+            :param sorting_order: sorting order; possible values are 'desc', 'asc'
+            :type sorting_order: str
+            :return: response
+            :rtype: requests.Response
+        """
+        warn("This method is deprecated. Use advanced_search_v3 instead.", DeprecationWarning)
+
+        if not isinstance(query_string, str):
+            raise WrongInputError("The search query must be a string.")
+
+        if not isinstance(ticloud, bool):
+            raise WrongInputError("ticloud parameter must be boolean.")
+
+        if not isinstance(records_per_page, int) or not 1 <= records_per_page <= 100:
+            raise WrongInputError("records_per_page parameter must be an integer with a value "
+                                  "between 1 and 100 (included).")
+
+        url = self._url.format(endpoint=self.__ADVANCED_SEARCH_ENDPOINT_V2)
+
+        post_json = {"query": query_string, "ticloud": ticloud, "page": page_number,
+                     "records_per_page": records_per_page}
+
+        if sorting_criteria:
+            if sorting_criteria not in ADVANCED_SEARCH_SORTING_CRITERIA or sorting_order not in ("desc", "asc"):
+                raise WrongInputError("Sorting criteria must be one of the following options: {criteria}. "
+                                      "Sorting order needs to be 'desc' or 'asc'.".format(
+                    criteria=ADVANCED_SEARCH_SORTING_CRITERIA
+                ))
+            sorting_expression = "{criteria} {order}".format(
+                criteria=sorting_criteria,
+                order=sorting_order
+            )
+
+            post_json["sort"] = sorting_expression
+
+        response = self.__post_request(url=url, post_json=post_json)
+
+        self.__raise_on_error(response)
+
+        return response
+
+    def advanced_search_v2_aggregated(self, query_string, ticloud=False, max_results=5000, sorting_criteria=None,
+                                      sorting_order="desc"):
+        """THIS METHOD IS DEPRECATED. Use advanced_search_v3_aggregated instead.
+
+        Sends a query string to the A1000 Advanced Search API v2.
+        The query string must be composed of key-value pairs separated by space.
+        A key is separated from its value by a colon symbol and no spaces.
+        For directions on how to write advanced search queries, consult the A1000 documentation.
+        Paging is done automatically and results from individual
+        responses aggregated into one list and returned`.
+        The 'max_results' parameter defines the maximum desired number of results to be returned.
+            Query string example:
+            'av-count:5 available:TRUE'
+
+            :param query_string: search query - see API documentation for details on writing search queries
+            :type query_string: str
+            :param ticloud: show only cloud results
+            :type ticloud: bool
+            :param max_results: maximum results to be returned in a list; default value is 5000
+            :type max_results: int
+            :param sorting_criteria: define the criteria used in sorting; possible values are 'sha1', 'firstseen',
+            'threatname', 'sampletype', 'filecount', 'size'
+            :type sorting_criteria: str
+            :param sorting_order: sorting order; possible values are 'desc', 'asc'
+            :type sorting_order: str
+            :return: list of results
+            :rtype: list
+        """
+        warn("This method is deprecated. Use advanced_search_v3_aggregated instead.", DeprecationWarning)
+
+        if not isinstance(max_results, int):
+            raise WrongInputError("max_results parameter must be integer.")
+
+        results = []
+        next_page = 1
+        more_pages = True
+
+        while more_pages:
+            response = self.advanced_search_v2(
+                query_string=query_string,
+                ticloud=ticloud,
+                page_number=next_page,
+                records_per_page=100,
+                sorting_criteria=sorting_criteria,
+                sorting_order=sorting_order
+            )
+
+            response_json = response.json()
+
+            entries = response_json.get("rl").get("web_search_api").get("entries", [])
+            results.extend(entries)
+
+            if len(results) > max_results:
+                results = results[:max_results]
+                return results
+
+            next_page = response_json.get("rl").get("web_search_api").get("next_page", None)
+            more_pages = response_json.get("rl").get("web_search_api").get("more_pages", False)
+
+        return results
+
     def advanced_search_v3(self, query_string, ticloud=False, start_search_date=None, end_search_date=None,
                            page_number=1, records_per_page=20, sorting_criteria=None, sorting_order="desc"):
         """Sends a query string to the A1000 Advanced Search API v3.
         The query string must be composed of key-value pairs separated by space.
         A key is separated from its value by a colon symbol and no spaces.
         For directions on how to write advanced search queries, consult the A1000 documentation.
         If a page number is not provided, the first page of results will be returned.
```

### Comparing `reversinglabs_sdk_py3-2.5.5/ReversingLabs/SDK/helper.py` & `reversinglabs_sdk_py3-2.5.6/ReversingLabs/SDK/helper.py`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.5/ReversingLabs/SDK/ticloud.py` & `reversinglabs_sdk_py3-2.5.6/ReversingLabs/SDK/ticloud.py`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.5/ReversingLabs/SDK/tiscale.py` & `reversinglabs_sdk_py3-2.5.6/ReversingLabs/SDK/tiscale.py`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.5/logo.png` & `reversinglabs_sdk_py3-2.5.6/logo.png`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.5/reversinglabs_sdk_py3.egg-info/PKG-INFO` & `reversinglabs_sdk_py3-2.5.6/reversinglabs_sdk_py3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reversinglabs-sdk-py3
-Version: 2.5.5
+Version: 2.5.6
 Summary: Python SDK for using ReversingLabs services.
 Home-page: https://github.com/reversinglabs/reversinglabs-sdk-py3
 Author: ReversingLabs
 Author-email: support@reversinglabs.com
 License: MIT
 Project-URL: Documentation, https://github.com/reversinglabs/reversinglabs-sdk-py3/blob/main/README.md
 Project-URL: Source, https://github.com/reversinglabs/reversinglabs-sdk-py3
```

### Comparing `reversinglabs_sdk_py3-2.5.5/reversinglabs_sdk_py3.egg-info/SOURCES.txt` & `reversinglabs_sdk_py3-2.5.6/reversinglabs_sdk_py3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.5/setup.py` & `reversinglabs_sdk_py3-2.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.5/tests/test_a1000.py` & `reversinglabs_sdk_py3-2.5.6/tests/test_a1000.py`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.5/tests/test_helper.py` & `reversinglabs_sdk_py3-2.5.6/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.5/tests/test_ticloud.py` & `reversinglabs_sdk_py3-2.5.6/tests/test_ticloud.py`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.5/tests/test_tiscale.py` & `reversinglabs_sdk_py3-2.5.6/tests/test_tiscale.py`

 * *Files identical despite different names*

