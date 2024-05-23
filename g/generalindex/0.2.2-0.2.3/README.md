# Comparing `tmp/generalindex-0.2.2.tar.gz` & `tmp/generalindex-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generalindex-0.2.2.tar", last modified: Wed May 22 11:00:24 2024, max compression
+gzip compressed data, was "generalindex-0.2.3.tar", last modified: Thu May 23 10:53:28 2024, max compression
```

## Comparing `generalindex-0.2.2.tar` & `generalindex-0.2.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 11:00:24.567203 generalindex-0.2.2/
--rw-rw-rw-   0 root         (0) root         (0)     1055 2024-05-22 11:00:11.000000 generalindex-0.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    17501 2024-05-22 11:00:24.567203 generalindex-0.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    16900 2024-05-22 11:00:11.000000 generalindex-0.2.2/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 11:00:24.563203 generalindex-0.2.2/generalindex/
--rw-rw-rw-   0 root         (0) root         (0)     1324 2024-05-22 11:00:11.000000 generalindex-0.2.2/generalindex/Authenticator.py
--rw-rw-rw-   0 root         (0) root         (0)     9789 2024-05-22 11:00:11.000000 generalindex-0.2.2/generalindex/DatalakeHandler.py
--rw-rw-rw-   0 root         (0) root         (0)     7696 2024-05-22 11:00:11.000000 generalindex-0.2.2/generalindex/GxApi.py
--rw-rw-rw-   0 root         (0) root         (0)     7126 2024-05-22 11:00:11.000000 generalindex-0.2.2/generalindex/HTTPCaller.py
--rw-rw-rw-   0 root         (0) root         (0)     2154 2024-05-22 11:00:11.000000 generalindex-0.2.2/generalindex/StatusHandler.py
--rw-rw-rw-   0 root         (0) root         (0)     8962 2024-05-22 11:00:11.000000 generalindex-0.2.2/generalindex/TaskHandler.py
--rw-rw-rw-   0 root         (0) root         (0)    28639 2024-05-22 11:00:11.000000 generalindex-0.2.2/generalindex/Timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2024-05-22 11:00:11.000000 generalindex-0.2.2/generalindex/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       96 2024-05-22 11:00:11.000000 generalindex-0.2.2/generalindex/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      551 2024-05-22 11:00:11.000000 generalindex-0.2.2/generalindex/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1779 2024-05-22 11:00:11.000000 generalindex-0.2.2/generalindex/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 11:00:24.567203 generalindex-0.2.2/generalindex.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17501 2024-05-22 11:00:24.000000 generalindex-0.2.2/generalindex.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      616 2024-05-22 11:00:24.000000 generalindex-0.2.2/generalindex.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-22 11:00:24.000000 generalindex-0.2.2/generalindex.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-22 11:00:24.000000 generalindex-0.2.2/generalindex.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       13 2024-05-22 11:00:24.000000 generalindex-0.2.2/generalindex.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-22 11:00:24.567203 generalindex-0.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1205 2024-05-22 11:00:13.000000 generalindex-0.2.2/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 11:00:24.567203 generalindex-0.2.2/test/
--rw-rw-rw-   0 root         (0) root         (0)     1631 2024-05-22 11:00:11.000000 generalindex-0.2.2/test/test_datalakehandler.py
--rw-rw-rw-   0 root         (0) root         (0)     8088 2024-05-22 11:00:11.000000 generalindex-0.2.2/test/test_gxapi.py
--rw-rw-rw-   0 root         (0) root         (0)     7987 2024-05-22 11:00:11.000000 generalindex-0.2.2/test/test_httpcaller.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2024-05-22 11:00:11.000000 generalindex-0.2.2/test/test_timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)     1716 2024-05-22 11:00:11.000000 generalindex-0.2.2/test/test_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 10:53:28.662369 generalindex-0.2.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1055 2024-05-23 10:53:15.000000 generalindex-0.2.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    17501 2024-05-23 10:53:28.662369 generalindex-0.2.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    16900 2024-05-23 10:53:15.000000 generalindex-0.2.3/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 10:53:28.658369 generalindex-0.2.3/generalindex/
+-rw-rw-rw-   0 root         (0) root         (0)     1324 2024-05-23 10:53:15.000000 generalindex-0.2.3/generalindex/Authenticator.py
+-rw-rw-rw-   0 root         (0) root         (0)     9789 2024-05-23 10:53:15.000000 generalindex-0.2.3/generalindex/DatalakeHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)     7728 2024-05-23 10:53:15.000000 generalindex-0.2.3/generalindex/GxApi.py
+-rw-rw-rw-   0 root         (0) root         (0)     7126 2024-05-23 10:53:15.000000 generalindex-0.2.3/generalindex/HTTPCaller.py
+-rw-rw-rw-   0 root         (0) root         (0)     2154 2024-05-23 10:53:15.000000 generalindex-0.2.3/generalindex/StatusHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)     8962 2024-05-23 10:53:15.000000 generalindex-0.2.3/generalindex/TaskHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)    28639 2024-05-23 10:53:15.000000 generalindex-0.2.3/generalindex/Timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)      271 2024-05-23 10:53:15.000000 generalindex-0.2.3/generalindex/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       96 2024-05-23 10:53:15.000000 generalindex-0.2.3/generalindex/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      551 2024-05-23 10:53:15.000000 generalindex-0.2.3/generalindex/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1779 2024-05-23 10:53:15.000000 generalindex-0.2.3/generalindex/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 10:53:28.662369 generalindex-0.2.3/generalindex.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17501 2024-05-23 10:53:28.000000 generalindex-0.2.3/generalindex.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      616 2024-05-23 10:53:28.000000 generalindex-0.2.3/generalindex.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-23 10:53:28.000000 generalindex-0.2.3/generalindex.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-23 10:53:28.000000 generalindex-0.2.3/generalindex.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       13 2024-05-23 10:53:28.000000 generalindex-0.2.3/generalindex.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-23 10:53:28.662369 generalindex-0.2.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1205 2024-05-23 10:53:17.000000 generalindex-0.2.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 10:53:28.662369 generalindex-0.2.3/test/
+-rw-rw-rw-   0 root         (0) root         (0)     1631 2024-05-23 10:53:15.000000 generalindex-0.2.3/test/test_datalakehandler.py
+-rw-rw-rw-   0 root         (0) root         (0)     8088 2024-05-23 10:53:15.000000 generalindex-0.2.3/test/test_gxapi.py
+-rw-rw-rw-   0 root         (0) root         (0)     7987 2024-05-23 10:53:15.000000 generalindex-0.2.3/test/test_httpcaller.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2024-05-23 10:53:15.000000 generalindex-0.2.3/test/test_timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1716 2024-05-23 10:53:15.000000 generalindex-0.2.3/test/test_utils.py
```

### Comparing `generalindex-0.2.2/LICENSE` & `generalindex-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.2/PKG-INFO` & `generalindex-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generalindex
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python SDK for the General Index platform
 Home-page: https://www.general-index.com/
 Author: General Index
 Author-email: info@general-index.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `generalindex-0.2.2/README.md` & `generalindex-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.2/generalindex/Authenticator.py` & `generalindex-0.2.3/generalindex/Authenticator.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.2/generalindex/DatalakeHandler.py` & `generalindex-0.2.3/generalindex/DatalakeHandler.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.2/generalindex/GxApi.py` & `generalindex-0.2.3/generalindex/GxApi.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         :param headers: Additional headers, which will be sent with request for symbols e.g. {"Example-Header":"Example_header_value"}
 
         :return: _ApiRequest
         """
         sig, method_locals = inspect.signature(self.index), locals()
         query_params_dict = {self._to_camel_case(param.name): self._concatenate(method_locals[param.name]) for param in
                              sig.parameters.values() if
-                             (method_locals[param.name] is not None)}
+                             (method_locals[param.name] is not None and not param.name != 'headers')}
         query_params_dict = self._create_query_params(query_params_dict)
         return _ApiRequest(path='/index', query_params=query_params_dict, headers=headers)
 
     def catalogue(self, code: list = None, no_module: bool = None, module: str = None,
                   fields: dict = None, limit_fields: list = None):
         """
         The method retrieves the data from Gx Api based on provided parameters.
```

### Comparing `generalindex-0.2.2/generalindex/HTTPCaller.py` & `generalindex-0.2.3/generalindex/HTTPCaller.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.2/generalindex/StatusHandler.py` & `generalindex-0.2.3/generalindex/StatusHandler.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.2/generalindex/TaskHandler.py` & `generalindex-0.2.3/generalindex/TaskHandler.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.2/generalindex/Timeseries.py` & `generalindex-0.2.3/generalindex/Timeseries.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.2/generalindex/exceptions.py` & `generalindex-0.2.3/generalindex/exceptions.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.2/generalindex/utils.py` & `generalindex-0.2.3/generalindex/utils.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.2/generalindex.egg-info/PKG-INFO` & `generalindex-0.2.3/generalindex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generalindex
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python SDK for the General Index platform
 Home-page: https://www.general-index.com/
 Author: General Index
 Author-email: info@general-index.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `generalindex-0.2.2/generalindex.egg-info/SOURCES.txt` & `generalindex-0.2.3/generalindex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.2/setup.py` & `generalindex-0.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open('requirements.txt') as fin:
     requirements = fin.read()
 
 setuptools.setup(
     name="generalindex",
-    version="0.2.2",
+    version="0.2.3",
     author="General Index",
     author_email="info@general-index.com",
     description="Python SDK for the General Index platform",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.general-index.com/",
     packages=setuptools.find_packages(exclude=["test"]),
```

### Comparing `generalindex-0.2.2/test/test_datalakehandler.py` & `generalindex-0.2.3/test/test_datalakehandler.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.2/test/test_gxapi.py` & `generalindex-0.2.3/test/test_gxapi.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.2/test/test_httpcaller.py` & `generalindex-0.2.3/test/test_httpcaller.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.2/test/test_timeseries.py` & `generalindex-0.2.3/test/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.2/test/test_utils.py` & `generalindex-0.2.3/test/test_utils.py`

 * *Files identical despite different names*

