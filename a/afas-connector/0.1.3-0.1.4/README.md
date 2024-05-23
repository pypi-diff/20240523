# Comparing `tmp/afas_connector-0.1.3.tar.gz` & `tmp/afas_connector-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afas_connector-0.1.3.tar", last modified: Wed Apr 10 08:25:52 2024, max compression
+gzip compressed data, was "afas_connector-0.1.4.tar", last modified: Thu May 23 11:58:43 2024, max compression
```

## Comparing `afas_connector-0.1.3.tar` & `afas_connector-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:25:52.498058 afas_connector-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-10 08:25:36.000000 afas_connector-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-10 08:25:52.498058 afas_connector-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-10 08:25:36.000000 afas_connector-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:25:52.498058 afas_connector-0.1.3/afas_connector/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-10 08:25:36.000000 afas_connector-0.1.3/afas_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-10 08:25:36.000000 afas_connector-0.1.3/afas_connector/afas_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-10 08:25:36.000000 afas_connector-0.1.3/afas_connector/afas_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-10 08:25:36.000000 afas_connector-0.1.3/afas_connector/afas_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:25:52.498058 afas_connector-0.1.3/afas_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-10 08:25:52.000000 afas_connector-0.1.3/afas_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-10 08:25:52.000000 afas_connector-0.1.3/afas_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 08:25:52.000000 afas_connector-0.1.3/afas_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 08:25:52.000000 afas_connector-0.1.3/afas_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-10 08:25:52.000000 afas_connector-0.1.3/afas_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 08:25:52.498058 afas_connector-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-10 08:25:38.000000 afas_connector-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:58:43.444871 afas_connector-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-23 11:58:37.000000 afas_connector-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-05-23 11:58:43.444871 afas_connector-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-23 11:58:37.000000 afas_connector-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:58:43.444871 afas_connector-0.1.4/afas_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-23 11:58:37.000000 afas_connector-0.1.4/afas_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-23 11:58:37.000000 afas_connector-0.1.4/afas_connector/afas_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-05-23 11:58:37.000000 afas_connector-0.1.4/afas_connector/afas_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-23 11:58:37.000000 afas_connector-0.1.4/afas_connector/afas_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:58:43.444871 afas_connector-0.1.4/afas_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-05-23 11:58:43.000000 afas_connector-0.1.4/afas_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-23 11:58:43.000000 afas_connector-0.1.4/afas_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:58:43.000000 afas_connector-0.1.4/afas_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 11:58:43.000000 afas_connector-0.1.4/afas_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 11:58:43.000000 afas_connector-0.1.4/afas_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 11:58:43.444871 afas_connector-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-23 11:58:40.000000 afas_connector-0.1.4/setup.py
```

### Comparing `afas_connector-0.1.3/LICENSE` & `afas_connector-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `afas_connector-0.1.3/PKG-INFO` & `afas_connector-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afas_connector
-Version: 0.1.3
+Version: 0.1.4
 Summary: AfasConnector is a Python package that simplifies interacting with AFAS Connectors via HTTP requests. It provides classes for making GET, POST, and PUT requests to AFAS Connectors and handling their responses.
 Home-page: https://github.com/bakeable/afas-connector
 Author: Robin Bakker
 Author-email: robin@bakeable.nl
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `afas_connector-0.1.3/README.md` & `afas_connector-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `afas_connector-0.1.3/afas_connector/afas_connector.py` & `afas_connector-0.1.4/afas_connector/afas_connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,24 @@
             tuple: A tuple containing the status code and the JSON response from the AFAS Connector.
         """
         # Check if endpoint starts with "/"
         if endpoint[0] != "/":
             endpoint = "/" + endpoint
 
         # Create the URL
-        url = self.AFAS_CONNECTORS_URL + endpoint + f'?take={take}&skip={skip}'
+        url = self.AFAS_CONNECTORS_URL + endpoint
+
+        # Add query parameters
+        if '?' in url:
+            url += '&'
+        else:
+            url += '?'
+        
+        # Add take and skip
+        url += f'take={take}&skip={skip}'
 
         # Add ordering
         if order_by is not None:
             if ascending:
                 url += f'&orderbyfieldids={order_by}'
             else:
                 url += f'&orderbyfieldids=-{order_by}'
```

### Comparing `afas_connector-0.1.3/afas_connector/afas_filter.py` & `afas_connector-0.1.4/afas_connector/afas_filter.py`

 * *Files identical despite different names*

### Comparing `afas_connector-0.1.3/afas_connector/afas_object.py` & `afas_connector-0.1.4/afas_connector/afas_object.py`

 * *Files identical despite different names*

### Comparing `afas_connector-0.1.3/afas_connector.egg-info/PKG-INFO` & `afas_connector-0.1.4/afas_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afas_connector
-Version: 0.1.3
+Version: 0.1.4
 Summary: AfasConnector is a Python package that simplifies interacting with AFAS Connectors via HTTP requests. It provides classes for making GET, POST, and PUT requests to AFAS Connectors and handling their responses.
 Home-page: https://github.com/bakeable/afas-connector
 Author: Robin Bakker
 Author-email: robin@bakeable.nl
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `afas_connector-0.1.3/setup.py` & `afas_connector-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="afas_connector",
-    version="0.1.3",
+    version="0.1.4",
     packages=find_packages(),
     install_requires=[
         'requests >= 2.31.0',
         'python-dotenv >= 1.0.1'
     ],
     author="Robin Bakker",
     author_email="robin@bakeable.nl",
```

