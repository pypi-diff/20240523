# Comparing `tmp/vipas-0.1.4.tar.gz` & `tmp/vipas-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vipas-0.1.4.tar", last modified: Wed May 22 15:11:13 2024, max compression
+gzip compressed data, was "vipas-0.1.5.tar", last modified: Thu May 23 11:20:00 2024, max compression
```

## Comparing `vipas-0.1.4.tar` & `vipas-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-22 15:11:13.808755 vipas-0.1.4/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2487 2024-04-30 05:46:43.000000 vipas-0.1.4/LICENSE.md
--rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-22 15:11:13.808755 vipas-0.1.4/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1598 2024-05-01 12:56:58.000000 vipas-0.1.4/README.md
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       91 2024-05-14 08:16:21.000000 vipas-0.1.4/pyproject.toml
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      443 2024-05-22 15:11:13.808755 vipas-0.1.4/setup.cfg
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1273 2024-05-22 14:39:02.000000 vipas-0.1.4/setup.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-22 15:11:13.804755 vipas-0.1.4/test/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2818 2024-05-14 08:16:21.000000 vipas-0.1.4/test/test_model_client.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-22 15:11:13.804755 vipas-0.1.4/vipas/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      725 2024-04-30 15:42:34.000000 vipas-0.1.4/vipas/__init__.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2084 2024-05-02 09:27:49.000000 vipas-0.1.4/vipas/_rest.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     4145 2024-05-15 18:08:55.000000 vipas-0.1.4/vipas/config.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     3809 2024-05-16 15:16:24.000000 vipas-0.1.4/vipas/exceptions.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     6870 2024-05-17 09:04:05.000000 vipas-0.1.4/vipas/model.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2463 2024-05-22 14:37:58.000000 vipas-0.1.4/vipas/vipas_logger.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-22 15:11:13.804755 vipas-0.1.4/vipas.egg-info/
--rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-22 15:11:13.000000 vipas-0.1.4/vipas.egg-info/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      330 2024-05-22 15:11:13.000000 vipas-0.1.4/vipas.egg-info/SOURCES.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2024-05-22 15:11:13.000000 vipas-0.1.4/vipas.egg-info/dependency_links.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       65 2024-05-22 15:11:13.000000 vipas-0.1.4/vipas.egg-info/requires.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        6 2024-05-22 15:11:13.000000 vipas-0.1.4/vipas.egg-info/top_level.txt
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-23 11:20:00.127206 vipas-0.1.5/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2487 2024-04-30 05:46:43.000000 vipas-0.1.5/LICENSE.md
+-rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-23 11:20:00.127206 vipas-0.1.5/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1598 2024-05-01 12:56:58.000000 vipas-0.1.5/README.md
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       91 2024-05-14 08:16:21.000000 vipas-0.1.5/pyproject.toml
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      443 2024-05-23 11:20:00.127206 vipas-0.1.5/setup.cfg
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1273 2024-05-23 11:13:43.000000 vipas-0.1.5/setup.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-23 11:20:00.127206 vipas-0.1.5/test/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2818 2024-05-14 08:16:21.000000 vipas-0.1.5/test/test_model_client.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-23 11:20:00.127206 vipas-0.1.5/vipas/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      725 2024-04-30 15:42:34.000000 vipas-0.1.5/vipas/__init__.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2381 2024-05-23 10:06:07.000000 vipas-0.1.5/vipas/_rest.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     4145 2024-05-15 18:08:55.000000 vipas-0.1.5/vipas/config.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1270 2024-05-23 11:11:09.000000 vipas-0.1.5/vipas/error_suggestions.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     4046 2024-05-23 11:16:54.000000 vipas-0.1.5/vipas/exceptions.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     6870 2024-05-17 09:04:05.000000 vipas-0.1.5/vipas/model.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2463 2024-05-22 14:37:58.000000 vipas-0.1.5/vipas/vipas_logger.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-23 11:20:00.127206 vipas-0.1.5/vipas.egg-info/
+-rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-23 11:20:00.000000 vipas-0.1.5/vipas.egg-info/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      357 2024-05-23 11:20:00.000000 vipas-0.1.5/vipas.egg-info/SOURCES.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2024-05-23 11:20:00.000000 vipas-0.1.5/vipas.egg-info/dependency_links.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       65 2024-05-23 11:20:00.000000 vipas-0.1.5/vipas.egg-info/requires.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        6 2024-05-23 11:20:00.000000 vipas-0.1.5/vipas.egg-info/top_level.txt
```

### Comparing `vipas-0.1.4/LICENSE.md` & `vipas-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vipas-0.1.4/README.md` & `vipas-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `vipas-0.1.4/setup.py` & `vipas-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "vipas"
-VERSION = "0.1.4"
+VERSION = "0.1.5"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3",
     "pydantic",
     "typing-extensions",
     "ratelimit",
     "pybreaker",
```

### Comparing `vipas-0.1.4/test/test_model_client.py` & `vipas-0.1.5/test/test_model_client.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.4/vipas/__init__.py` & `vipas-0.1.5/vipas/__init__.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.4/vipas/_rest.py` & `vipas-0.1.5/vipas/_rest.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,13 +44,19 @@
             body = json.dumps(body)
 
         # Make the HTTP request using the session
         try:
             response = self.session.request(method, url, headers=headers, data=body)
             response.raise_for_status()
         except requests.exceptions.HTTPError as e:
-            raise ClientException.from_response(http_resp=response, body=response.text, data=None)
+            error_detail = response.text
+            try:
+                # Attempt to parse the response text as JSON and extract the 'detail' field
+                error_detail = json.loads(response.text).get('detail', response.text)
+            except json.JSONDecodeError:
+                pass
+            raise ClientException.from_response(http_resp=response, body=error_detail, data=None)
         except requests.exceptions.RequestException as e:
             # Handle any errors that occur while making the request
             raise ClientException(status=500, reason=str(e))
         
         return json.loads(response.content.decode('utf-8'))
```

### Comparing `vipas-0.1.4/vipas/config.py` & `vipas-0.1.5/vipas/config.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.4/vipas/model.py` & `vipas-0.1.5/vipas/model.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.4/vipas/vipas_logger.py` & `vipas-0.1.5/vipas/vipas_logger.py`

 * *Files identical despite different names*

