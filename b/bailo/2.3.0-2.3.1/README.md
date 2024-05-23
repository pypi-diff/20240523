# Comparing `tmp/bailo-2.3.0.tar.gz` & `tmp/bailo-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bailo-2.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "bailo-2.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `bailo-2.3.0.tar` & `bailo-2.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2241 2024-05-21 16:08:28.781113 bailo-2.3.0/README.md
--rw-r--r--   0        0        0     4889 2024-05-21 16:08:28.785113 bailo-2.3.0/pyproject.toml
--rw-r--r--   0        0        0      685 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/__init__.py
--rw-r--r--   0        0        0      153 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/core/__init__.py
--rw-r--r--   0        0        0     3594 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/core/agent.py
--rw-r--r--   0        0        0    19238 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/core/client.py
--rw-r--r--   0        0        0      672 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/core/enums.py
--rw-r--r--   0        0        0      221 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/core/exceptions.py
--rw-r--r--   0        0        0     1072 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/core/utils.py
--rw-r--r--   0        0        0      521 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/helper/__init__.py
--rw-r--r--   0        0        0     3923 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/helper/access_request.py
--rw-r--r--   0        0        0     3833 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/helper/datacard.py
--rw-r--r--   0        0        0     3367 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/helper/entry.py
--rw-r--r--   0        0        0    13134 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/helper/model.py
--rw-r--r--   0        0        0     9816 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/helper/release.py
--rw-r--r--   0        0        0     2976 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/helper/schema.py
--rw-r--r--   0        0        0     3674 1970-01-01 00:00:00.000000 bailo-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2241 2024-05-23 16:23:35.505535 bailo-2.3.1/README.md
+-rw-r--r--   0        0        0     4889 2024-05-23 16:23:35.505535 bailo-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0      685 2024-05-23 16:23:35.505535 bailo-2.3.1/src/bailo/__init__.py
+-rw-r--r--   0        0        0      153 2024-05-23 16:23:35.505535 bailo-2.3.1/src/bailo/core/__init__.py
+-rw-r--r--   0        0        0     4083 2024-05-23 16:23:35.505535 bailo-2.3.1/src/bailo/core/agent.py
+-rw-r--r--   0        0        0    19238 2024-05-23 16:23:35.505535 bailo-2.3.1/src/bailo/core/client.py
+-rw-r--r--   0        0        0      672 2024-05-23 16:23:35.505535 bailo-2.3.1/src/bailo/core/enums.py
+-rw-r--r--   0        0        0      221 2024-05-23 16:23:35.505535 bailo-2.3.1/src/bailo/core/exceptions.py
+-rw-r--r--   0        0        0     1072 2024-05-23 16:23:35.505535 bailo-2.3.1/src/bailo/core/utils.py
+-rw-r--r--   0        0        0      521 2024-05-23 16:23:35.505535 bailo-2.3.1/src/bailo/helper/__init__.py
+-rw-r--r--   0        0        0     3923 2024-05-23 16:23:35.505535 bailo-2.3.1/src/bailo/helper/access_request.py
+-rw-r--r--   0        0        0     3833 2024-05-23 16:23:35.509535 bailo-2.3.1/src/bailo/helper/datacard.py
+-rw-r--r--   0        0        0     3367 2024-05-23 16:23:35.509535 bailo-2.3.1/src/bailo/helper/entry.py
+-rw-r--r--   0        0        0    13134 2024-05-23 16:23:35.509535 bailo-2.3.1/src/bailo/helper/model.py
+-rw-r--r--   0        0        0     9816 2024-05-23 16:23:35.509535 bailo-2.3.1/src/bailo/helper/release.py
+-rw-r--r--   0        0        0     2976 2024-05-23 16:23:35.509535 bailo-2.3.1/src/bailo/helper/schema.py
+-rw-r--r--   0        0        0     3674 1970-01-01 00:00:00.000000 bailo-2.3.1/PKG-INFO
```

### Comparing `bailo-2.3.0/README.md` & `bailo-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `bailo-2.3.0/pyproject.toml` & `bailo-2.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bailo-2.3.0/src/bailo/__init__.py` & `bailo-2.3.1/src/bailo/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 ===================
 
 Bailo is a ecosystem for managing the lifecycle of managing machine learning models. This package provides support for interacting with models within Bailo.
 """
 from __future__ import annotations
 
 
-# Package Version 2.3.0
-__version__ = "2.3.0"
+# Package Version 2.3.1
+__version__ = "2.3.1"
 
 
 from bailo.core.agent import Agent, PkiAgent, TokenAgent
 from bailo.core.client import Client
 from bailo.core.enums import EntryKind, ModelVisibility, Role, SchemaKind
 from bailo.helper.access_request import AccessRequest
 from bailo.helper.datacard import Datacard
```

### Comparing `bailo-2.3.0/src/bailo/core/agent.py` & `bailo-2.3.1/src/bailo/core/agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 from json import JSONDecodeError
 
 import requests
+import os
+import getpass
 from requests.auth import HTTPBasicAuth
 from bailo.core.exceptions import BailoException, ResponseException
 
 
 class Agent:
     """Base API Agent for talking with Bailo.
 
@@ -91,22 +93,36 @@
     def delete(self, *args, **kwargs):
         return super().delete(*args, cert=(self.cert, self.key), **kwargs)
 
 
 class TokenAgent(Agent):
     def __init__(
         self,
-        access_key: str,
-        secret_key: str,
+        access_key: str | None = None,
+        secret_key: str | None = None,
     ):
         """Initiate an agent for API token authentication.
 
         :param access_key: Access key
         :param secret_key: Secret key
         """
+        super().__init__()
+
+        if access_key is None:
+            try:
+                access_key = os.environ["BAILO_ACCESS_KEY"]
+            except KeyError:
+                access_key = getpass.getpass("BAILO ACCESS KEY:")
+
+        if secret_key is None:
+            try:
+                secret_key = os.environ["BAILO_SECRET_KEY"]
+            except KeyError:
+                secret_key = getpass.getpass("BAILO SECRET KEY:")
+
         self.access_key = access_key
         self.secret_key = secret_key
         self.basic = HTTPBasicAuth(access_key, secret_key)
 
     def get(self, *args, **kwargs):
         return super().get(*args, auth=self.basic, **kwargs)
```

### Comparing `bailo-2.3.0/src/bailo/core/client.py` & `bailo-2.3.1/src/bailo/core/client.py`

 * *Files identical despite different names*

### Comparing `bailo-2.3.0/src/bailo/core/enums.py` & `bailo-2.3.1/src/bailo/core/enums.py`

 * *Files identical despite different names*

### Comparing `bailo-2.3.0/src/bailo/core/utils.py` & `bailo-2.3.1/src/bailo/core/utils.py`

 * *Files identical despite different names*

### Comparing `bailo-2.3.0/src/bailo/helper/__init__.py` & `bailo-2.3.1/src/bailo/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `bailo-2.3.0/src/bailo/helper/access_request.py` & `bailo-2.3.1/src/bailo/helper/access_request.py`

 * *Files identical despite different names*

### Comparing `bailo-2.3.0/src/bailo/helper/datacard.py` & `bailo-2.3.1/src/bailo/helper/datacard.py`

 * *Files identical despite different names*

### Comparing `bailo-2.3.0/src/bailo/helper/entry.py` & `bailo-2.3.1/src/bailo/helper/entry.py`

 * *Files identical despite different names*

### Comparing `bailo-2.3.0/src/bailo/helper/model.py` & `bailo-2.3.1/src/bailo/helper/model.py`

 * *Files identical despite different names*

### Comparing `bailo-2.3.0/src/bailo/helper/release.py` & `bailo-2.3.1/src/bailo/helper/release.py`

 * *Files identical despite different names*

### Comparing `bailo-2.3.0/src/bailo/helper/schema.py` & `bailo-2.3.1/src/bailo/helper/schema.py`

 * *Files identical despite different names*

### Comparing `bailo-2.3.0/PKG-INFO` & `bailo-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bailo
-Version: 2.3.0
+Version: 2.3.1
 Summary: Simplifies interacting with Bailo
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bailo Version: 2.3.0 Summary: Simplifies
+Metadata-Version: 2.1 Name: bailo Version: 2.3.1 Summary: Simplifies
 interacting with Bailo Requires-Python: >=3.8.1 Description-Content-Type: text/
 markdown Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: semantic-version==2.10.0 Requires-Dist: requests>=2.22 Requires-
 Dist: tqdm>=4.66.2 Requires-Dist: black==23.3.0 ; extra == "test" Requires-
```

