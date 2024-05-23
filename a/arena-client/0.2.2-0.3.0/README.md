# Comparing `tmp/arena_client-0.2.2.tar.gz` & `tmp/arena_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arena_client-0.2.2.tar", max compression
+gzip compressed data, was "arena_client-0.3.0.tar", max compression
```

## Comparing `arena_client-0.2.2.tar` & `arena_client-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      570 2024-05-22 09:26:09.375372 arena_client-0.2.2/README.md
--rw-r--r--   0        0        0     1348 2024-05-22 09:26:09.375372 arena_client-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      154 2024-05-22 09:26:09.375372 arena_client-0.2.2/src/arena/__init__.py
--rw-r--r--   0        0        0    12669 2024-05-22 09:26:09.375372 arena_client-0.2.2/src/arena/client.py
--rw-r--r--   0        0        0     1018 2024-05-22 09:26:09.375372 arena_client-0.2.2/src/arena/models/__init__.py
--rw-r--r--   0        0        0     4009 2024-05-22 09:26:09.375372 arena_client-0.2.2/src/arena/models/anthropic.py
--rw-r--r--   0        0        0     4364 2024-05-22 09:26:09.375372 arena_client-0.2.2/src/arena/models/chat_completion.py
--rw-r--r--   0        0        0      281 2024-05-22 09:26:09.375372 arena_client-0.2.2/src/arena/models/evaluation.py
--rw-r--r--   0        0        0     2287 2024-05-22 09:26:09.375372 arena_client-0.2.2/src/arena/models/mistral.py
--rw-r--r--   0        0        0     1444 2024-05-22 09:26:09.375372 arena_client-0.2.2/src/arena/models/openai.py
--rw-r--r--   0        0        0      237 2024-05-22 09:26:09.375372 arena_client-0.2.2/src/arena/models/settings.py
--rw-r--r--   0        0        0     1195 1970-01-01 00:00:00.000000 arena_client-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      123 2024-05-23 15:50:43.500275 arena_client-0.3.0/README.md
+-rw-r--r--   0        0        0     1387 2024-05-23 15:50:43.500275 arena_client-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      154 2024-05-23 15:50:43.500275 arena_client-0.3.0/src/arena/__init__.py
+-rw-r--r--   0        0        0    15342 2024-05-23 15:50:43.500275 arena_client-0.3.0/src/arena/client.py
+-rw-r--r--   0        0        0     1018 2024-05-23 15:50:43.500275 arena_client-0.3.0/src/arena/models/__init__.py
+-rw-r--r--   0        0        0     4009 2024-05-23 15:50:43.500275 arena_client-0.3.0/src/arena/models/anthropic.py
+-rw-r--r--   0        0        0     4364 2024-05-23 15:50:43.500275 arena_client-0.3.0/src/arena/models/chat_completion.py
+-rw-r--r--   0        0        0      281 2024-05-23 15:50:43.500275 arena_client-0.3.0/src/arena/models/evaluation.py
+-rw-r--r--   0        0        0     2287 2024-05-23 15:50:43.500275 arena_client-0.3.0/src/arena/models/mistral.py
+-rw-r--r--   0        0        0     1444 2024-05-23 15:50:43.500275 arena_client-0.3.0/src/arena/models/openai.py
+-rw-r--r--   0        0        0      237 2024-05-23 15:50:43.500275 arena_client-0.3.0/src/arena/models/settings.py
+-rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 arena_client-0.3.0/PKG-INFO
```

### Comparing `arena_client-0.2.2/pyproject.toml` & `arena_client-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "arena-client"
-version = "0.2.2"
+version = "0.3.0"
 description = "A client to use arena AI"
 authors = ["Nicolas Grislain <ng@sarus.tech>"]
 license = "Apache-2"
 readme = "README.md"
 packages = [{from = "src", include = "arena"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 httpx = "^0.25"
 openai = "^1.23"
 anthropic = "^0.21"
 mistralai = "^0.1"
 anyio = {extras = ["trio"], version = "^4.3.0"}
+pyarrow = "^16.1.0"
+parquet = "^1.3.1"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.10.0"
 pytest = "^8.1.1"
 ruff = "^0.2.2"
 python-dotenv = "^1.0.1"
 rich = "^13.7.1"
```

### Comparing `arena_client-0.2.2/src/arena/client.py` & `arena_client-0.3.0/src/arena/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,17 +4,21 @@
 from arena.models import ChatCompletionRequest, ChatCompletionResponse, Evaluation, Score, LMConfig, EventOut, ChatCompletionRequestEventResponse
 import arena.models.openai as oai
 import arena.models.mistral as mis
 import arena.models.anthropic as ant
 import openai
 import mistralai
 import anthropic
+import pyarrow as pa
+import pyarrow.parquet as pq
+
 
 BASE_URL = "https://arena.sarus.app/api/v1"
 
+
 class Client:
     def __init__(self, username: str | None = None, password: str | None = None, api_key: str | None = None, base_url: str = BASE_URL):
         self.username = username
         self.password = password
         self.api_key = api_key
         self.base_url = base_url
         self.timeout = 30.0
@@ -201,14 +205,88 @@
             )
         if resp.status_code == 200:
             return resp.json()["id"]
         else:
             raise RuntimeError(resp)
     
 
+    def event(self, name: str, content: str, parent_id: int | None = None, native_identifier: str | None = None) -> int:
+        """Create an event"""
+        with httpx.Client(timeout=self.timeout) as client:
+            resp = client.post(
+                url = f"{self.base_url}/events/",
+                headers = {
+                    "Authorization": f"Bearer {self.api_key}"
+                },
+                json={
+                    "name": name,
+                    "content": content,
+                    "parent_id": parent_id
+                },
+            )
+        if resp.status_code == 200:
+            if native_identifier:
+                self.identifier(resp.json()["id"], native_identifier)
+            return resp.json()["id"]
+        else:
+            raise RuntimeError(resp)
+    
+
+    def identifier(self, event_id: int, native_identifier: str) -> int:
+        """Create an event"""
+        with httpx.Client(timeout=self.timeout) as client:
+            resp = client.post(
+                url = f"{self.base_url}/events/identifier",
+                headers = {
+                    "Authorization": f"Bearer {self.api_key}"
+                },
+                json={
+                    "id": native_identifier,
+                    "event_id": event_id
+                },
+            )
+        if resp.status_code == 200:
+            return resp.json()["id"]
+        else:
+            raise RuntimeError(resp)
+
+
+    def events(self) -> list[EventOut]:
+        """download all events as an arrow file"""
+        with httpx.Client(timeout=self.timeout) as client:
+            resp = client.get(
+                url = f"{self.base_url}/events/?skip=0&limit=1000000",
+                headers = {
+                    "Authorization": f"Bearer {self.api_key}"
+                },
+            )
+        if resp.status_code == 200:
+            return [EventOut.model_validate(event) for event in resp.json()["data"]]
+        else:
+            raise RuntimeError(resp)
+
+
+    def download_events(self) -> pa.Table:
+        """download all events as an arrow file"""
+        with httpx.Client(timeout=self.timeout) as client:
+            resp = client.get(
+                url = f"{self.base_url}/events/download/parquet",
+                headers = {
+                    "Authorization": f"Bearer {self.api_key}"
+                },
+            )
+        if resp.status_code == 200:
+            buffer = pa.py_buffer(resp.content)
+            input_stream = pa.input_stream(buffer)
+            table = pq.read_table(input_stream)
+            return table
+        else:
+            raise RuntimeError(resp)
+
+
     def decorate(self, client: Type, mode: Literal['proxy', 'instrument'] = 'proxy'):
         """Decorate the client"""
         if not hasattr(client, "_arena_decorated_"):
             client._arena_decorated_ = mode
             if client == openai.OpenAI:
                 if mode == 'proxy':
                     self.decorate_openai_proxy(client)
```

### Comparing `arena_client-0.2.2/src/arena/models/__init__.py` & `arena_client-0.3.0/src/arena/models/__init__.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.2.2/src/arena/models/anthropic.py` & `arena_client-0.3.0/src/arena/models/anthropic.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.2.2/src/arena/models/chat_completion.py` & `arena_client-0.3.0/src/arena/models/chat_completion.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.2.2/src/arena/models/mistral.py` & `arena_client-0.3.0/src/arena/models/mistral.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.2.2/src/arena/models/openai.py` & `arena_client-0.3.0/src/arena/models/openai.py`

 * *Files identical despite different names*

