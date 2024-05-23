# Comparing `tmp/fastapi_tarpit-1.0.3.tar.gz` & `tmp/fastapi_tarpit-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_tarpit-1.0.3.tar", last modified: Wed May  8 19:19:37 2024, max compression
+gzip compressed data, was "fastapi_tarpit-1.0.4.tar", last modified: Thu May 23 20:35:25 2024, max compression
```

## Comparing `fastapi_tarpit-1.0.3.tar` & `fastapi_tarpit-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 mats      (1000) mats      (1000)        0 2024-05-08 19:19:37.276832 fastapi_tarpit-1.0.3/
--rw-rw-r--   0 mats      (1000) mats      (1000)     1071 2024-04-16 21:29:58.000000 fastapi_tarpit-1.0.3/LICENSE
--rw-r--r--   0 mats      (1000) mats      (1000)     1703 2024-05-08 19:19:37.276832 fastapi_tarpit-1.0.3/PKG-INFO
--rw-rw-r--   0 mats      (1000) mats      (1000)     1084 2024-04-25 19:23:39.000000 fastapi_tarpit-1.0.3/README.md
-drwxrwxr-x   0 mats      (1000) mats      (1000)        0 2024-05-08 19:19:37.276832 fastapi_tarpit-1.0.3/fastapi_tarpit/
--rw-rw-r--   0 mats      (1000) mats      (1000)       87 2024-05-08 19:09:42.000000 fastapi_tarpit-1.0.3/fastapi_tarpit/__init__.py
--rw-rw-r--   0 mats      (1000) mats      (1000)     3300 2024-05-08 19:15:16.000000 fastapi_tarpit-1.0.3/fastapi_tarpit/client.py
--rw-rw-r--   0 mats      (1000) mats      (1000)      519 2024-05-08 19:02:19.000000 fastapi_tarpit-1.0.3/fastapi_tarpit/config.py
--rw-rw-r--   0 mats      (1000) mats      (1000)     2221 2024-05-08 19:14:04.000000 fastapi_tarpit-1.0.3/fastapi_tarpit/middleware.py
-drwxrwxr-x   0 mats      (1000) mats      (1000)        0 2024-05-08 19:19:37.276832 fastapi_tarpit-1.0.3/fastapi_tarpit.egg-info/
--rw-r--r--   0 mats      (1000) mats      (1000)     1703 2024-05-08 19:19:37.000000 fastapi_tarpit-1.0.3/fastapi_tarpit.egg-info/PKG-INFO
--rw-rw-r--   0 mats      (1000) mats      (1000)      327 2024-05-08 19:19:37.000000 fastapi_tarpit-1.0.3/fastapi_tarpit.egg-info/SOURCES.txt
--rw-rw-r--   0 mats      (1000) mats      (1000)        1 2024-05-08 19:19:37.000000 fastapi_tarpit-1.0.3/fastapi_tarpit.egg-info/dependency_links.txt
--rw-rw-r--   0 mats      (1000) mats      (1000)        8 2024-05-08 19:19:37.000000 fastapi_tarpit-1.0.3/fastapi_tarpit.egg-info/requires.txt
--rw-rw-r--   0 mats      (1000) mats      (1000)       15 2024-05-08 19:19:37.000000 fastapi_tarpit-1.0.3/fastapi_tarpit.egg-info/top_level.txt
--rw-rw-r--   0 mats      (1000) mats      (1000)      693 2024-05-08 19:17:04.000000 fastapi_tarpit-1.0.3/pyproject.toml
--rw-rw-r--   0 mats      (1000) mats      (1000)       38 2024-05-08 19:19:37.276832 fastapi_tarpit-1.0.3/setup.cfg
+drwxrwxr-x   0 mats      (1000) mats      (1000)        0 2024-05-23 20:35:25.191217 fastapi_tarpit-1.0.4/
+-rw-rw-r--   0 mats      (1000) mats      (1000)     1071 2024-04-16 21:29:58.000000 fastapi_tarpit-1.0.4/LICENSE
+-rw-r--r--   0 mats      (1000) mats      (1000)     1704 2024-05-23 20:35:25.191217 fastapi_tarpit-1.0.4/PKG-INFO
+-rw-rw-r--   0 mats      (1000) mats      (1000)     1084 2024-04-25 19:23:39.000000 fastapi_tarpit-1.0.4/README.md
+drwxrwxr-x   0 mats      (1000) mats      (1000)        0 2024-05-23 20:35:25.191217 fastapi_tarpit-1.0.4/fastapi_tarpit/
+-rw-rw-r--   0 mats      (1000) mats      (1000)       87 2024-05-08 19:09:42.000000 fastapi_tarpit-1.0.4/fastapi_tarpit/__init__.py
+-rw-rw-r--   0 mats      (1000) mats      (1000)     4506 2024-05-23 20:23:07.000000 fastapi_tarpit-1.0.4/fastapi_tarpit/client.py
+-rw-rw-r--   0 mats      (1000) mats      (1000)      702 2024-05-10 21:52:07.000000 fastapi_tarpit-1.0.4/fastapi_tarpit/config.py
+-rw-rw-r--   0 mats      (1000) mats      (1000)     2186 2024-05-09 20:02:54.000000 fastapi_tarpit-1.0.4/fastapi_tarpit/middleware.py
+drwxrwxr-x   0 mats      (1000) mats      (1000)        0 2024-05-23 20:35:25.191217 fastapi_tarpit-1.0.4/fastapi_tarpit.egg-info/
+-rw-r--r--   0 mats      (1000) mats      (1000)     1704 2024-05-23 20:35:25.000000 fastapi_tarpit-1.0.4/fastapi_tarpit.egg-info/PKG-INFO
+-rw-rw-r--   0 mats      (1000) mats      (1000)      327 2024-05-23 20:35:25.000000 fastapi_tarpit-1.0.4/fastapi_tarpit.egg-info/SOURCES.txt
+-rw-rw-r--   0 mats      (1000) mats      (1000)        1 2024-05-23 20:35:25.000000 fastapi_tarpit-1.0.4/fastapi_tarpit.egg-info/dependency_links.txt
+-rw-rw-r--   0 mats      (1000) mats      (1000)        8 2024-05-23 20:35:25.000000 fastapi_tarpit-1.0.4/fastapi_tarpit.egg-info/requires.txt
+-rw-rw-r--   0 mats      (1000) mats      (1000)       15 2024-05-23 20:35:25.000000 fastapi_tarpit-1.0.4/fastapi_tarpit.egg-info/top_level.txt
+-rw-rw-r--   0 mats      (1000) mats      (1000)      694 2024-05-23 20:34:36.000000 fastapi_tarpit-1.0.4/pyproject.toml
+-rw-rw-r--   0 mats      (1000) mats      (1000)       38 2024-05-23 20:35:25.191217 fastapi_tarpit-1.0.4/setup.cfg
```

### Comparing `fastapi_tarpit-1.0.3/LICENSE` & `fastapi_tarpit-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_tarpit-1.0.3/PKG-INFO` & `fastapi_tarpit-1.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: fastapi-tarpit
-Version: 1.0.3
+Version: 1.0.4
 Summary: FastAPI middleware that purposely delays incoming connections on unused routes
 Author-email: Mats Klepsland <mats.klepsland@gmail.com>
 Project-URL: Homepage, https://github.com/thus/fastapi-tarpit
 Project-URL: Issues, https://github.com/thus/fastapi-tarpit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: FastAPI
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastapi
 
 # FastAPI Tarpit
 
 [FastAPI](https://fastapi.tiangolo.com/) middleware that purposely delays
```

### Comparing `fastapi_tarpit-1.0.3/README.md` & `fastapi_tarpit-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_tarpit-1.0.3/fastapi_tarpit/client.py` & `fastapi_tarpit-1.0.4/fastapi_tarpit/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+import json
+from asyncio import sleep
 from datetime import datetime, timedelta
+from enum import Enum
 from random import randrange
 from typing import List
 
 from fastapi import Request
 from starlette.datastructures import Address
 
 from .config import TarpitConfig
@@ -36,54 +39,93 @@
                             f"{'minutes' if minutes > 1 else 'minute'}")
     if seconds or not duration_str:
         duration_str.append(f"{seconds} "
                             f"{'second' if seconds == 1 else 'seconds'}")
     return " ".join(duration_str)
 
 
+class TarpitState(Enum):
+    NEW = 1
+    TRAPPED = 2
+    CLOSED = 3
+
+
 class TarpitClient:
     def __init__(self: "TarpitClient", request: Request,
                  config: TarpitConfig) -> None:
         if isinstance(request.client, Address):
-            self.host = f"{request.client.host}:{request.client.port}"
+            self.client = f"{request.client.host}:{request.client.port}"
         else:
-            self.host = "<undefined>"
+            self.client = "<undefined>"
         self.request = request
         self.config = config
         self.start_time = datetime.now()
         self.log_next = self.start_time + timedelta(seconds=log_interval[0])
         self.log_interval_idx = 0
         self.logging_enabled = True
-        self.log(f"'{self.host}' got stuck in the tarpit visiting "
-                 f"'{request.url.path}'")
+        self.log(TarpitState.NEW)
+
+    def log(self: "TarpitClient", state: TarpitState) -> None:
+        duration = duration_pretty_string(datetime.now() - self.start_time)
+
+        if self.config.log_as_json:
+            data = {
+                "client": self.client,
+                "path": self.request.url.path,
+                "duration": duration
+            }
+
+        match state:
+            case TarpitState.NEW:
+                if self.config.log_as_json:
+                    data["state"] = "NEW"
+                else:
+                    msg = (f"'{self.client}' got stuck in the tarpit visiting "
+                           f"'{self.request.url.path}'")
+            case TarpitState.TRAPPED:
+                if self.config.log_as_json:
+                    data["state"] = "TRAPPED"
+                else:
+                    msg = (f"'{self.client}' is still stuck in the tarpit "
+                           f"after {duration} visiting "
+                           f"'{self.request.url.path}'")
+            case TarpitState.CLOSED:
+                if self.config.log_as_json:
+                    data["state"] = "CLOSED"
+                else:
+                    msg = (f"Trapped '{self.client} in the tarpit for "
+                           f"{duration} visiting '{self.request.url.path}'")
+
+        if self.config.log_as_json:
+            msg = json.dumps(data)
 
-    def log(self: "TarpitClient", msg: str) -> None:
         self.config.logger.info(msg)
 
     def close(self: "TarpitClient") -> None:
-        duration = duration_pretty_string(datetime.now() - self.start_time)
-        self.log(f"Trapped '{self.host} in the tarpit for {duration} "
-                 f"visiting '{self.request.url.path}'")
+        self.log(TarpitState.CLOSED)
 
     def tick(self: "TarpitClient") -> None:
-        """Used to log how long a host has been stuck in the tarpit at
+        """Used to log how long a client has been stuck in the tarpit at
            different time intervals (minute, hour, day, etc)."""
         if not self.logging_enabled or datetime.now() < self.log_next:
             return
 
-        duration = duration_pretty_string(datetime.now() - self.start_time)
-        self.log(f"'{self.host}' is still stuck in the tarpit after "
-                 f"{duration} visiting '{self.request.url.path}'")
+        self.log(TarpitState.TRAPPED)
 
         self.log_interval_idx += 1
         try:
             seconds = log_interval[self.log_interval_idx]
         except IndexError:
             # This is unlikely to ever happen, but if it does, then just
             # disable logging.
             self.logging_enabled = False
         self.log_next = self.start_time + timedelta(seconds=seconds)
 
-    def generate_bytes(self: "TarpitClient") -> bytes:
-        length = randrange(self.config.output_length_min,  # noqa: S311
-                           self.config.output_length_max)
+    def generate_chunk(self: "TarpitClient") -> bytes:
+        length = randrange(self.config.chunk_length_min,  # noqa: S311
+                           self.config.chunk_length_max)
         return b'.' * length
+
+    async def wait(self: "TarpitClient") -> None:
+        wait = randrange(self.config.chunk_wait_min,  # noqa: S311
+                         self.config.chunk_wait_max)
+        await sleep(wait)
```

### Comparing `fastapi_tarpit-1.0.3/fastapi_tarpit/middleware.py` & `fastapi_tarpit-1.0.4/fastapi_tarpit/middleware.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from asyncio import sleep
 from contextlib import contextmanager
 from signal import SIGINT, getsignal, signal
 from types import FrameType
 from typing import Any, AsyncIterator, Dict, Iterator, Optional
 
 from fastapi import FastAPI, Request
 from fastapi.responses import StreamingResponse
@@ -25,17 +24,17 @@
         client.close()
 
 
 async def tarpit_stream(request: Request,
                         config: TarpitConfig) -> AsyncIterator[bytes]:
     with tarpit_connection(request, config) as client:
         while tarpit_running:
-            await sleep(config.interval)
+            await client.wait()
             client.tick()
-            yield client.generate_bytes()
+            yield client.generate_chunk()
 
 
 class HTTPTarpitMiddleware(BaseHTTPMiddleware):
     def __init__(self: "HTTPTarpitMiddleware", app: FastAPI,
                  **kwargs: Any) -> None:
         self.config: TarpitConfig = TarpitConfig(**kwargs)
         self.routes: Dict[str, int] = {}
```

### Comparing `fastapi_tarpit-1.0.3/fastapi_tarpit.egg-info/PKG-INFO` & `fastapi_tarpit-1.0.4/fastapi_tarpit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: fastapi-tarpit
-Version: 1.0.3
+Version: 1.0.4
 Summary: FastAPI middleware that purposely delays incoming connections on unused routes
 Author-email: Mats Klepsland <mats.klepsland@gmail.com>
 Project-URL: Homepage, https://github.com/thus/fastapi-tarpit
 Project-URL: Issues, https://github.com/thus/fastapi-tarpit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: FastAPI
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastapi
 
 # FastAPI Tarpit
 
 [FastAPI](https://fastapi.tiangolo.com/) middleware that purposely delays
```

### Comparing `fastapi_tarpit-1.0.3/pyproject.toml` & `fastapi_tarpit-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastapi-tarpit"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Mats Klepsland", email="mats.klepsland@gmail.com" },
 ]
 dependencies = [
   "fastapi",
 ]
 description = "FastAPI middleware that purposely delays incoming connections on unused routes"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Framework :: FastAPI",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

