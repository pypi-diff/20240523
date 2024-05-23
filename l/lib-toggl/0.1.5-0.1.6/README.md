# Comparing `tmp/lib_toggl-0.1.5.tar.gz` & `tmp/lib_toggl-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_toggl-0.1.5.tar", max compression
+gzip compressed data, was "lib_toggl-0.1.6.tar", max compression
```

## Comparing `lib_toggl-0.1.5.tar` & `lib_toggl-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-12-26 19:39:10.972800 lib_toggl-0.1.5/LICENSE
--rw-r--r--   0        0        0     3112 2024-05-22 17:50:45.128033 lib_toggl-0.1.5/README.md
--rw-r--r--   0        0        0       87 2024-01-18 17:19:23.942907 lib_toggl-0.1.5/lib_toggl/__init__.py
--rw-r--r--   0        0        0      758 2024-01-18 17:13:20.299494 lib_toggl-0.1.5/lib_toggl/account.py
--rw-r--r--   0        0        0    29959 2024-05-22 17:50:44.804704 lib_toggl-0.1.5/lib_toggl/client.py
--rw-r--r--   0        0        0      371 2023-12-26 19:39:10.972800 lib_toggl-0.1.5/lib_toggl/const.py
--rw-r--r--   0        0        0      559 2024-05-22 02:03:37.351411 lib_toggl-0.1.5/lib_toggl/organization.py
--rw-r--r--   0        0        0     1621 2024-05-22 02:03:37.351411 lib_toggl-0.1.5/lib_toggl/tags.py
--rw-r--r--   0        0        0     9195 2024-05-22 17:25:32.613801 lib_toggl-0.1.5/lib_toggl/time_entries.py
--rw-r--r--   0        0        0     5688 2024-05-22 02:03:37.351411 lib_toggl-0.1.5/lib_toggl/workspace.py
--rw-r--r--   0        0        0      628 2024-05-22 02:03:37.351411 lib_toggl-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3658 1970-01-01 00:00:00.000000 lib_toggl-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-12-26 19:39:10.972800 lib_toggl-0.1.6/LICENSE
+-rw-r--r--   0        0        0     3112 2024-05-22 17:50:45.128033 lib_toggl-0.1.6/README.md
+-rw-r--r--   0        0        0      168 2024-05-23 17:03:38.968701 lib_toggl-0.1.6/lib_toggl/__init__.py
+-rw-r--r--   0        0        0      918 2024-05-23 17:03:38.968701 lib_toggl-0.1.6/lib_toggl/account.py
+-rw-r--r--   0        0        0    30034 2024-05-23 17:03:38.968701 lib_toggl-0.1.6/lib_toggl/client.py
+-rw-r--r--   0        0        0      372 2024-05-23 17:03:38.968701 lib_toggl-0.1.6/lib_toggl/const.py
+-rw-r--r--   0        0        0      582 2024-05-23 17:03:38.968701 lib_toggl-0.1.6/lib_toggl/organization.py
+-rw-r--r--   0        0        0     1776 2024-05-23 17:03:38.968701 lib_toggl-0.1.6/lib_toggl/tags.py
+-rw-r--r--   0        0        0     9362 2024-05-23 17:03:38.968701 lib_toggl-0.1.6/lib_toggl/time_entries.py
+-rw-r--r--   0        0        0     5857 2024-05-23 17:03:38.972034 lib_toggl-0.1.6/lib_toggl/workspace.py
+-rw-r--r--   0        0        0      628 2024-05-23 17:03:38.972034 lib_toggl-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3658 1970-01-01 00:00:00.000000 lib_toggl-0.1.6/PKG-INFO
```

### Comparing `lib_toggl-0.1.5/LICENSE` & `lib_toggl-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_toggl-0.1.5/README.md` & `lib_toggl-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `lib_toggl-0.1.5/lib_toggl/account.py` & `lib_toggl-0.1.6/lib_toggl/account.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 """Account Information
 Parse/Coercion done by Pydantic
 """
+
 from datetime import datetime
 from typing import Optional
 
-from pydantic.v1 import BaseModel, SecretStr
+try:
+    # Pydantic v2 ships a copy of v1.
+    from pydantic.v1 import BaseModel, SecretStr
+except ImportError:
+    # Home Assistant does not yet support v2.
+    from pydantic import BaseModel, SecretStr
 
 from .const import BASE
 
 ENDPOINT = f"{BASE}/me"
 
 
 class Account(BaseModel):
```

### Comparing `lib_toggl-0.1.5/lib_toggl/client.py` & `lib_toggl-0.1.6/lib_toggl/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -692,12 +692,13 @@
 # TODO: General exceptions to handle and wrap
 # Trying to stop a TE that was deleted:
 #   aiohttp.client_exceptions.ClientResponseError: 404, message='Not Found',
 # Incorrect basic auth
 #   aiohttp.client_exceptions.ClientResponseError: 401, message='Unauthorized',
 # Trying to stop an entry on a workspace that's not mine
 #   aiohttp.client_exceptions.ClientResponseError: 403, message='Forbidden',
+#       409 when trying to stop a time entry that's already stopped... etc
 # When sending a request BODY with verb GET (or just a bad request in general)
 #   aiohttp.client_exceptions.ClientResponseError: 400, message='Bad Request',
 ##
 # TODO: can probably re-factor a bit and remove the do_$VERB_request functions and replace with
 #   a singular do_request which takes an aiohttp.request() object
```

### Comparing `lib_toggl-0.1.5/lib_toggl/tags.py` & `lib_toggl-0.1.6/lib_toggl/tags.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """Represents a Toggl Tag object."""
 
 import logging
 from datetime import datetime
 from typing import Optional
 
-from pydantic.v1 import BaseModel, Field
+try:
+    # Pydantic v2 ships a copy of v1.
+    from pydantic.v1 import BaseModel, Field
+except ImportError:
+    # Home Assistant does not yet support v2.
+    from pydantic import BaseModel, Field
 
 from .const import BASE
 
 log = logging.getLogger(__name__)
 
 
 @staticmethod
```

### Comparing `lib_toggl-0.1.5/lib_toggl/time_entries.py` & `lib_toggl-0.1.6/lib_toggl/time_entries.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 Parse/Coercion done by Pydantic
 """
 
 import logging
 from datetime import datetime
 from typing import Any, List, Optional
 
-from pydantic.v1 import BaseModel, Field, validator
+try:
+    # Pydantic v2 ships a copy of v1.
+    from pydantic.v1 import BaseModel, Field, validator
+except ImportError:
+    # Home Assistant does not yet support v2.
+    from pydantic import BaseModel, Field, validator
+
 from pyrfc3339 import generate
 
 from .const import BASE, DEFAULT_CREATED_BY
 
 log = logging.getLogger(__name__)
 
 ENDPOINT = f"{BASE}/me/time_entries"
```

### Comparing `lib_toggl-0.1.5/lib_toggl/workspace.py` & `lib_toggl-0.1.6/lib_toggl/workspace.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 Parse/Coercion done by Pydantic
 """
 
 import logging
 from datetime import datetime
 from typing import Any, Optional
 
-from pydantic import BaseModel, Field, SecretStr
+try:
+    # Pydantic v2 ships a copy of v1.
+    from pydantic.v1 import BaseModel, Field, SecretStr
+except ImportError:
+    # Home Assistant does not yet support v2.
+    from pydantic import BaseModel, Field, SecretStr
 
 from .const import BASE
 
 log = logging.getLogger(__name__)
 
 ENDPOINT = f"{BASE}/workspaces"
```

### Comparing `lib_toggl-0.1.5/pyproject.toml` & `lib_toggl-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib-toggl"
-version = "0.1.5"
+version = "0.1.6"
 description = "Asynchronous Python library for the Toggl API."
 authors = ["Karl Quinsalnd <karl@karlquinsland.com>"]
 readme = "README.md"
 packages = [{ include = "lib_toggl" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `lib_toggl-0.1.5/PKG-INFO` & `lib_toggl-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-toggl
-Version: 0.1.5
+Version: 0.1.6
 Summary: Asynchronous Python library for the Toggl API.
 Author: Karl Quinsalnd
 Author-email: karl@karlquinsland.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiodns (>=3.1.1,<4.0.0)
```

