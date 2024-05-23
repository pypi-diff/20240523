# Comparing `tmp/annetbox-0.1.0.tar.gz` & `tmp/annetbox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annetbox-0.1.0.tar", last modified: Wed May 22 15:58:52 2024, max compression
+gzip compressed data, was "annetbox-0.1.1.tar", last modified: Thu May 23 15:43:35 2024, max compression
```

## Comparing `annetbox-0.1.0.tar` & `annetbox-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-22 15:58:52.752632 annetbox-0.1.0/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1079 2024-05-22 15:57:41.000000 annetbox-0.1.0/LICENSE
--rw-r--r--   0 tishka17  (1000) tishka17  (1000)     2350 2024-05-22 15:58:52.752632 annetbox-0.1.0/PKG-INFO
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1320 2024-05-22 15:57:41.000000 annetbox-0.1.0/README.md
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1145 2024-05-22 15:57:57.000000 annetbox-0.1.0/pyproject.toml
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       38 2024-05-22 15:58:52.752632 annetbox-0.1.0/setup.cfg
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-22 15:58:52.752632 annetbox-0.1.0/src/
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-22 15:58:52.752632 annetbox-0.1.0/src/annetbox/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-05-16 11:58:16.000000 annetbox-0.1.0/src/annetbox/__init__.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-22 15:58:52.752632 annetbox-0.1.0/src/annetbox/base/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-05-16 12:24:00.000000 annetbox-0.1.0/src/annetbox/base/__init__.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3630 2024-05-22 15:57:41.000000 annetbox-0.1.0/src/annetbox/base/client_async.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3989 2024-05-22 15:57:41.000000 annetbox-0.1.0/src/annetbox/base/client_sync.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      312 2024-05-22 15:57:41.000000 annetbox-0.1.0/src/annetbox/base/models.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-22 15:58:52.752632 annetbox-0.1.0/src/annetbox/v24/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-05-16 12:00:46.000000 annetbox-0.1.0/src/annetbox/v24/__init__.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1471 2024-05-22 15:57:41.000000 annetbox-0.1.0/src/annetbox/v24/client_async.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1446 2024-05-22 15:57:41.000000 annetbox-0.1.0/src/annetbox/v24/client_sync.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1346 2024-05-16 13:08:04.000000 annetbox-0.1.0/src/annetbox/v24/models.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-22 15:58:52.752632 annetbox-0.1.0/src/annetbox/v37/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-05-16 12:00:51.000000 annetbox-0.1.0/src/annetbox/v37/__init__.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3457 2024-05-22 15:57:41.000000 annetbox-0.1.0/src/annetbox/v37/client_async.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3426 2024-05-22 15:57:41.000000 annetbox-0.1.0/src/annetbox/v37/client_sync.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3116 2024-05-22 15:57:41.000000 annetbox-0.1.0/src/annetbox/v37/models.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-22 15:58:52.752632 annetbox-0.1.0/src/annetbox.egg-info/
--rw-r--r--   0 tishka17  (1000) tishka17  (1000)     2350 2024-05-22 15:58:52.000000 annetbox-0.1.0/src/annetbox.egg-info/PKG-INFO
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      603 2024-05-22 15:58:52.000000 annetbox-0.1.0/src/annetbox.egg-info/SOURCES.txt
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        1 2024-05-22 15:58:52.000000 annetbox-0.1.0/src/annetbox.egg-info/dependency_links.txt
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       92 2024-05-22 15:58:52.000000 annetbox-0.1.0/src/annetbox.egg-info/requires.txt
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        9 2024-05-22 15:58:52.000000 annetbox-0.1.0/src/annetbox.egg-info/top_level.txt
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-23 15:43:35.954941 annetbox-0.1.1/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1079 2024-05-22 15:57:41.000000 annetbox-0.1.1/LICENSE
+-rw-r--r--   0 tishka17  (1000) tishka17  (1000)     2350 2024-05-23 15:43:35.954941 annetbox-0.1.1/PKG-INFO
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1320 2024-05-22 15:57:41.000000 annetbox-0.1.1/README.md
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1145 2024-05-23 15:43:09.000000 annetbox-0.1.1/pyproject.toml
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       38 2024-05-23 15:43:35.954941 annetbox-0.1.1/setup.cfg
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-23 15:43:35.954941 annetbox-0.1.1/src/
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-23 15:43:35.954941 annetbox-0.1.1/src/annetbox/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-05-16 11:58:16.000000 annetbox-0.1.1/src/annetbox/__init__.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-23 15:43:35.954941 annetbox-0.1.1/src/annetbox/base/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-05-16 12:24:00.000000 annetbox-0.1.1/src/annetbox/base/__init__.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3633 2024-05-23 15:43:03.000000 annetbox-0.1.1/src/annetbox/base/client_async.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3992 2024-05-23 15:43:03.000000 annetbox-0.1.1/src/annetbox/base/client_sync.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      312 2024-05-22 15:57:41.000000 annetbox-0.1.1/src/annetbox/base/models.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-23 15:43:35.954941 annetbox-0.1.1/src/annetbox/v24/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-05-16 12:00:46.000000 annetbox-0.1.1/src/annetbox/v24/__init__.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1471 2024-05-22 15:57:41.000000 annetbox-0.1.1/src/annetbox/v24/client_async.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1446 2024-05-22 15:57:41.000000 annetbox-0.1.1/src/annetbox/v24/client_sync.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1346 2024-05-16 13:08:04.000000 annetbox-0.1.1/src/annetbox/v24/models.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-23 15:43:35.954941 annetbox-0.1.1/src/annetbox/v37/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-05-16 12:00:51.000000 annetbox-0.1.1/src/annetbox/v37/__init__.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3457 2024-05-22 15:57:41.000000 annetbox-0.1.1/src/annetbox/v37/client_async.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3426 2024-05-23 14:46:58.000000 annetbox-0.1.1/src/annetbox/v37/client_sync.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3442 2024-05-23 15:43:03.000000 annetbox-0.1.1/src/annetbox/v37/models.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-23 15:43:35.954941 annetbox-0.1.1/src/annetbox.egg-info/
+-rw-r--r--   0 tishka17  (1000) tishka17  (1000)     2350 2024-05-23 15:43:35.000000 annetbox-0.1.1/src/annetbox.egg-info/PKG-INFO
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      603 2024-05-23 15:43:35.000000 annetbox-0.1.1/src/annetbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        1 2024-05-23 15:43:35.000000 annetbox-0.1.1/src/annetbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       92 2024-05-23 15:43:35.000000 annetbox-0.1.1/src/annetbox.egg-info/requires.txt
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        9 2024-05-23 15:43:35.000000 annetbox-0.1.1/src/annetbox.egg-info/top_level.txt
```

### Comparing `annetbox-0.1.0/LICENSE` & `annetbox-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `annetbox-0.1.0/PKG-INFO` & `annetbox-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annetbox
-Version: 0.1.0
+Version: 0.1.1
 Summary: Annet Netbox client
 Author-email: Andrey Tikhonov <tishka17@nebius.com>
 License: MIT
 Project-URL: Source, https://github.com/annetutil/annetbox
 Project-URL: Homepage, https://github.com/annetutil/annetbox
 Project-URL: Bug Tracker, https://github.com/annetutil/annetbox/issues
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `annetbox-0.1.0/README.md` & `annetbox-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `annetbox-0.1.0/pyproject.toml` & `annetbox-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "annetbox"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.md"
 authors = [
     { name = "Andrey Tikhonov", email = "tishka17@nebius.com" },
 ]
 license = { text = "MIT" }
 description = "Annet Netbox client"
 requires-python = ">=3.10"
```

### Comparing `annetbox-0.1.0/src/annetbox/base/client_async.py` & `annetbox-0.1.1/src/annetbox/base/client_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,19 +52,20 @@
     """
     func = _collect_by_pages(func)
     if not field:
         return func
 
     @wraps(func)
     async def wrapper(self, *args, **kwargs):
+        method = func.__get__(self, self.__class__)
+
         value = kwargs.get(field)
         if not value:
-            return await func(*args, **kwargs)
+            return await method(*args, **kwargs)
 
-        method = func.__get__(self, self.__class__)
         results = []
         for offset in range(0, len(value), batch_size):
             kwargs[field] = value[offset : offset + batch_size]
             page = await method(*args, **kwargs)
             results.extend(page.results)
         return PagingResponse(
             previous=None,
```

### Comparing `annetbox-0.1.0/src/annetbox/base/client_sync.py` & `annetbox-0.1.1/src/annetbox/base/client_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,19 +52,20 @@
     """
     func = _collect_by_pages(func)
     if not field:
         return func
 
     @wraps(func)
     def wrapper(self, *args, **kwargs):
+        method = func.__get__(self, self.__class__)
+
         value = kwargs.get(field)
         if not value:
-            return func(*args, **kwargs)
+            return method(*args, **kwargs)
 
-        method = func.__get__(self, self.__class__)
         results = []
         for offset in range(0, len(value), batch_size):
             kwargs[field] = value[offset : offset + batch_size]
             page = method(*args, **kwargs)
             results.extend(page.results)
         return PagingResponse(
             previous=None,
```

### Comparing `annetbox-0.1.0/src/annetbox/v24/client_async.py` & `annetbox-0.1.1/src/annetbox/v24/client_async.py`

 * *Files identical despite different names*

### Comparing `annetbox-0.1.0/src/annetbox/v24/client_sync.py` & `annetbox-0.1.1/src/annetbox/v24/client_sync.py`

 * *Files identical despite different names*

### Comparing `annetbox-0.1.0/src/annetbox/v24/models.py` & `annetbox-0.1.1/src/annetbox/v24/models.py`

 * *Files identical despite different names*

### Comparing `annetbox-0.1.0/src/annetbox/v37/client_async.py` & `annetbox-0.1.1/src/annetbox/v37/client_async.py`

 * *Files identical despite different names*

### Comparing `annetbox-0.1.0/src/annetbox/v37/client_sync.py` & `annetbox-0.1.1/src/annetbox/v37/client_sync.py`

 * *Files identical despite different names*

### Comparing `annetbox-0.1.0/src/annetbox/v37/models.py` & `annetbox-0.1.1/src/annetbox/v37/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from typing import Any
 
 
 @dataclass
 class Entity:
     id: int
     name: str
+    display: str
+    url: str
 
 
 @dataclass
 class Label:
     value: str
     label: str
 
@@ -28,18 +30,37 @@
     id: int
     display: str
     address: str
     family: int
 
 
 @dataclass
+class LinkPeer(Entity):
+    cable: int
+    device: Entity
+
+
+@dataclass
+class InterfaceCable:
+    id: int
+    label: str
+    display: str
+    url: str
+
+
+@dataclass
 class Interface(Entity):
+    cable: InterfaceCable | None
+    cable_end: str
     device: Entity
+    link_peers: list[LinkPeer]
+    link_peers_type: str | None
     enabled: bool
-    display: str = ""  # added in 3.x
+    created: datetime
+    last_updated: datetime
 
 
 @dataclass
 class Device(Entity):
     url: str
     display: str  # renamed in 3.x from display_name
     device_type: DeviceType
@@ -67,15 +88,15 @@
     value: int
     label: str
 
 
 @dataclass
 class IpAddress:
     id: int
-    assigned_object_id: int
+    assigned_object_id: int | None
     display: str
     family: IpFamily
     address: str
     status: Label
     tags: list[Entity]
     created: datetime
     last_updated: datetime
```

### Comparing `annetbox-0.1.0/src/annetbox.egg-info/PKG-INFO` & `annetbox-0.1.1/src/annetbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annetbox
-Version: 0.1.0
+Version: 0.1.1
 Summary: Annet Netbox client
 Author-email: Andrey Tikhonov <tishka17@nebius.com>
 License: MIT
 Project-URL: Source, https://github.com/annetutil/annetbox
 Project-URL: Homepage, https://github.com/annetutil/annetbox
 Project-URL: Bug Tracker, https://github.com/annetutil/annetbox/issues
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `annetbox-0.1.0/src/annetbox.egg-info/SOURCES.txt` & `annetbox-0.1.1/src/annetbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

