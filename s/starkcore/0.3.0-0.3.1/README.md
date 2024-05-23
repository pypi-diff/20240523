# Comparing `tmp/starkcore-0.3.0.tar.gz` & `tmp/starkcore-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starkcore-0.3.0.tar", last modified: Tue May 21 23:16:56 2024, max compression
+gzip compressed data, was "starkcore-0.3.1.tar", last modified: Thu May 23 17:32:26 2024, max compression
```

## Comparing `starkcore-0.3.0.tar` & `starkcore-0.3.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-21 23:16:56.053411 starkcore-0.3.0/
--rw-r--r--   0 caiodottori   (501) staff       (20)     1068 2022-05-11 20:37:59.000000 starkcore-0.3.0/LICENSE.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)       49 2022-05-11 20:37:59.000000 starkcore-0.3.0/MANIFEST.in
--rw-r--r--   0 caiodottori   (501) staff       (20)      804 2024-05-21 23:16:56.053246 starkcore-0.3.0/PKG-INFO
--rw-r--r--   0 caiodottori   (501) staff       (20)      458 2022-05-11 20:37:59.000000 starkcore-0.3.0/README.md
--rw-r--r--   0 caiodottori   (501) staff       (20)       38 2024-05-21 23:16:56.053477 starkcore-0.3.0/setup.cfg
--rw-r--r--   0 caiodottori   (501) staff       (20)      760 2022-05-11 20:37:59.000000 starkcore-0.3.0/setup.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-21 23:16:56.011342 starkcore-0.3.0/starkcore/
--rw-r--r--   0 caiodottori   (501) staff       (20)      198 2024-05-21 23:16:13.000000 starkcore-0.3.0/starkcore/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      120 2022-09-05 16:45:10.000000 starkcore-0.3.0/starkcore/environment.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      846 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/error.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      898 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/key.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-21 23:16:56.023490 starkcore-0.3.0/starkcore/user/
--rw-r--r--   0 caiodottori   (501) staff       (20)      134 2022-09-07 13:21:49.000000 starkcore-0.3.0/starkcore/user/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2842 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/user/__organization.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     1940 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/user/__project.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      161 2022-09-07 13:21:49.000000 starkcore-0.3.0/starkcore/user/__publicuser.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      452 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/user/__user.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-21 23:16:56.052862 starkcore-0.3.0/starkcore/utils/
--rw-r--r--   0 caiodottori   (501) staff       (20)       25 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/utils/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2015 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/utils/api.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       12 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/utils/cache.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      340 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/utils/case.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2613 2022-09-07 13:21:49.000000 starkcore-0.3.0/starkcore/utils/checks.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      166 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/utils/compatibility.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      264 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/utils/enum.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      105 2022-09-07 13:21:49.000000 starkcore-0.3.0/starkcore/utils/host.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2501 2022-09-07 16:26:14.000000 starkcore-0.3.0/starkcore/utils/parse.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2886 2024-05-21 23:14:22.000000 starkcore-0.3.0/starkcore/utils/request.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      311 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/utils/resource.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     9218 2024-05-21 23:14:22.000000 starkcore-0.3.0/starkcore/utils/rest.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      614 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/utils/subresource.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      600 2023-05-19 17:51:46.000000 starkcore-0.3.0/starkcore/utils/url.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-21 23:16:56.013517 starkcore-0.3.0/starkcore.egg-info/
--rw-r--r--   0 caiodottori   (501) staff       (20)      804 2024-05-21 23:16:55.000000 starkcore-0.3.0/starkcore.egg-info/PKG-INFO
--rw-r--r--   0 caiodottori   (501) staff       (20)      798 2024-05-21 23:16:55.000000 starkcore-0.3.0/starkcore.egg-info/SOURCES.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)        1 2024-05-21 23:16:55.000000 starkcore-0.3.0/starkcore.egg-info/dependency_links.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)       40 2024-05-21 23:16:55.000000 starkcore-0.3.0/starkcore.egg-info/requires.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)       16 2024-05-21 23:16:55.000000 starkcore-0.3.0/starkcore.egg-info/top_level.txt
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-23 17:32:26.605886 starkcore-0.3.1/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1068 2022-05-11 20:37:59.000000 starkcore-0.3.1/LICENSE.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)       49 2022-05-11 20:37:59.000000 starkcore-0.3.1/MANIFEST.in
+-rw-r--r--   0 caiodottori   (501) staff       (20)      804 2024-05-23 17:32:26.605676 starkcore-0.3.1/PKG-INFO
+-rw-r--r--   0 caiodottori   (501) staff       (20)      458 2022-05-11 20:37:59.000000 starkcore-0.3.1/README.md
+-rw-r--r--   0 caiodottori   (501) staff       (20)       38 2024-05-23 17:32:26.606121 starkcore-0.3.1/setup.cfg
+-rw-r--r--   0 caiodottori   (501) staff       (20)      760 2022-05-11 20:37:59.000000 starkcore-0.3.1/setup.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-23 17:32:26.565849 starkcore-0.3.1/starkcore/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      198 2024-05-23 17:31:54.000000 starkcore-0.3.1/starkcore/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      120 2022-09-05 16:45:10.000000 starkcore-0.3.1/starkcore/environment.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      846 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/error.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      898 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/key.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-23 17:32:26.573201 starkcore-0.3.1/starkcore/user/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      134 2022-09-07 13:21:49.000000 starkcore-0.3.1/starkcore/user/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2842 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/user/__organization.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1940 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/user/__project.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      161 2022-09-07 13:21:49.000000 starkcore-0.3.1/starkcore/user/__publicuser.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      452 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/user/__user.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-23 17:32:26.604874 starkcore-0.3.1/starkcore/utils/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       25 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/utils/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2015 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/utils/api.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       12 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/utils/cache.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      340 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/utils/case.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2613 2022-09-07 13:21:49.000000 starkcore-0.3.1/starkcore/utils/checks.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      166 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/utils/compatibility.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      264 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/utils/enum.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      105 2022-09-07 13:21:49.000000 starkcore-0.3.1/starkcore/utils/host.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2501 2022-09-07 16:26:14.000000 starkcore-0.3.1/starkcore/utils/parse.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2911 2024-05-23 17:31:07.000000 starkcore-0.3.1/starkcore/utils/request.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      311 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/utils/resource.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     9228 2024-05-23 17:31:07.000000 starkcore-0.3.1/starkcore/utils/rest.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      614 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/utils/subresource.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      600 2023-05-19 17:51:46.000000 starkcore-0.3.1/starkcore/utils/url.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-23 17:32:26.567179 starkcore-0.3.1/starkcore.egg-info/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      804 2024-05-23 17:32:26.000000 starkcore-0.3.1/starkcore.egg-info/PKG-INFO
+-rw-r--r--   0 caiodottori   (501) staff       (20)      798 2024-05-23 17:32:26.000000 starkcore-0.3.1/starkcore.egg-info/SOURCES.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)        1 2024-05-23 17:32:26.000000 starkcore-0.3.1/starkcore.egg-info/dependency_links.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)       40 2024-05-23 17:32:26.000000 starkcore-0.3.1/starkcore.egg-info/requires.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)       16 2024-05-23 17:32:26.000000 starkcore-0.3.1/starkcore.egg-info/top_level.txt
```

### Comparing `starkcore-0.3.0/LICENSE.txt` & `starkcore-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.0/PKG-INFO` & `starkcore-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starkcore
-Version: 0.3.0
+Version: 0.3.1
 Summary: Basic SDK functionalities for the starkbank and starkinfra SDKs
 Home-page: https://github.com/starkinfra/core-python
 Author: Stark Infra
 Author-email: developers@starkbank.com
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `starkcore-0.3.0/setup.py` & `starkcore-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.0/starkcore/error.py` & `starkcore-0.3.1/starkcore/error.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.0/starkcore/key.py` & `starkcore-0.3.1/starkcore/key.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.0/starkcore/user/__organization.py` & `starkcore-0.3.1/starkcore/user/__organization.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.0/starkcore/user/__project.py` & `starkcore-0.3.1/starkcore/user/__project.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.0/starkcore/utils/api.py` & `starkcore-0.3.1/starkcore/utils/api.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.0/starkcore/utils/checks.py` & `starkcore-0.3.1/starkcore/utils/checks.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.0/starkcore/utils/parse.py` & `starkcore-0.3.1/starkcore/utils/parse.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.0/starkcore/utils/request.py` & `starkcore-0.3.1/starkcore/utils/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             data=body,
             headers=headers,
             timeout=timeout,
         )
     except Exception as exception:
         raise UnknownError("{}: {}".format(exception.__class__.__name__, str(exception)))
 
-    response = Response(status=request.status_code, content=request.content)
+    response = Response(status=request.status_code, content=request.content, headers=request.headers)
 
     if response.status == 500:
         raise InternalServerError()
     if response.status == 400:
         raise InputErrors(response.json()["errors"])
     if response.status != 200:
         raise UnknownError(response.content)
```

### Comparing `starkcore-0.3.0/starkcore/utils/rest.py` & `starkcore-0.3.1/starkcore/utils/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,60 +204,60 @@
         language=language,
         timeout=timeout,
     ).json()
     entity = json[last_name(resource)]
     return from_api_json(resource, entity)
 
 
-def get_raw(sdk_version, host, api_version, path, user, language, timeout, query):
-    return _parse_response_data(fetch(
+def put_multi(sdk_version, host, api_version, user, resource, entities, language, timeout, **query):
+    json = fetch(
         host=host,
         sdk_version=sdk_version,
         user=user,
-        method=get,
-        path=path,
+        method=put,
+        path=endpoint(resource),
+        payload={last_name_plural(resource): [api_json(entity) for entity in entities]},
         query=query,
         api_version=api_version,
-        prefix="Joker",
         language=language,
         timeout=timeout,
-    ))
+    ).json()
+    entities = json[last_name_plural(resource)]
+    return [from_api_json(resource, entity) for entity in entities]
 
 
-def post_raw(sdk_version, host, api_version, path, payload, user, language, timeout, **query):
+def get_raw(sdk_version, host, api_version, path, user, language, timeout, query=None):
     return _parse_response_data(fetch(
         host=host,
         sdk_version=sdk_version,
         user=user,
-        method=post,
+        method=get,
         path=path,
-        payload=payload,
         query=query,
         api_version=api_version,
         prefix="Joker",
         language=language,
         timeout=timeout,
     ))
 
 
-def put_multi(sdk_version, host, api_version, user, resource, entities, language, timeout, **query):
-    json = fetch(
+def post_raw(sdk_version, host, api_version, path, payload, user, language, timeout, **query):
+    return _parse_response_data(fetch(
         host=host,
         sdk_version=sdk_version,
         user=user,
-        method=put,
-        path=endpoint(resource),
-        payload={last_name_plural(resource): [api_json(entity) for entity in entities]},
+        method=post,
+        path=path,
+        payload=payload,
         query=query,
         api_version=api_version,
+        prefix="Joker",
         language=language,
         timeout=timeout,
-    ).json()
-    entities = json[last_name_plural(resource)]
-    return [from_api_json(resource, entity) for entity in entities]
+    ))
 
 
 def patch_raw(sdk_version, host, api_version, path, payload, user, language, timeout, **query):
     return _parse_response_data(fetch(
         host=host,
         sdk_version=sdk_version,
         user=user,
@@ -284,15 +284,15 @@
         api_version=api_version,
         prefix="Joker",
         language=language,
         timeout=timeout,
     ))
 
 
-def delete_raw(sdk_version, host, api_version, path, payload, user, language, timeout, **query):
+def delete_raw(sdk_version, host, api_version, path, user, language, timeout, payload=None, **query):
     return _parse_response_data(fetch(
         host=host,
         sdk_version=sdk_version,
         user=user,
         method=delete,
         path=path,
         payload=payload,
```

### Comparing `starkcore-0.3.0/starkcore/utils/subresource.py` & `starkcore-0.3.1/starkcore/utils/subresource.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.0/starkcore/utils/url.py` & `starkcore-0.3.1/starkcore/utils/url.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.0/starkcore.egg-info/PKG-INFO` & `starkcore-0.3.1/starkcore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starkcore
-Version: 0.3.0
+Version: 0.3.1
 Summary: Basic SDK functionalities for the starkbank and starkinfra SDKs
 Home-page: https://github.com/starkinfra/core-python
 Author: Stark Infra
 Author-email: developers@starkbank.com
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `starkcore-0.3.0/starkcore.egg-info/SOURCES.txt` & `starkcore-0.3.1/starkcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

