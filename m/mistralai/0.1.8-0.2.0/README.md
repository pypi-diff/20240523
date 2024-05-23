# Comparing `tmp/mistralai-0.1.8.tar.gz` & `tmp/mistralai-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistralai-0.1.8.tar", max compression
+gzip compressed data, was "mistralai-0.2.0.tar", max compression
```

## Comparing `mistralai-0.1.8.tar` & `mistralai-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2024-03-26 15:00:33.063484 mistralai-0.1.8/LICENSE
--rw-r--r--   0        0        0     1286 2024-03-26 15:00:33.063484 mistralai-0.1.8/README.md
--rw-r--r--   0        0        0      783 2024-03-26 15:00:44.115496 mistralai-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-26 15:00:33.063484 mistralai-0.1.8/src/mistralai/__init__.py
--rw-r--r--   0        0        0    11411 2024-03-26 15:00:33.063484 mistralai-0.1.8/src/mistralai/async_client.py
--rw-r--r--   0        0        0    11164 2024-03-26 15:00:33.063484 mistralai-0.1.8/src/mistralai/client.py
--rw-r--r--   0        0        0     4645 2024-03-26 15:00:44.163497 mistralai-0.1.8/src/mistralai/client_base.py
--rw-r--r--   0        0        0       86 2024-03-26 15:00:33.063484 mistralai-0.1.8/src/mistralai/constants.py
--rw-r--r--   0        0        0     1664 2024-03-26 15:00:33.063484 mistralai-0.1.8/src/mistralai/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-26 15:00:33.063484 mistralai-0.1.8/src/mistralai/models/__init__.py
--rw-r--r--   0        0        0     1845 2024-03-26 15:00:33.067484 mistralai-0.1.8/src/mistralai/models/chat_completion.py
--rw-r--r--   0        0        0      172 2024-03-26 15:00:33.067484 mistralai-0.1.8/src/mistralai/models/common.py
--rw-r--r--   0        0        0      331 2024-03-26 15:00:33.067484 mistralai-0.1.8/src/mistralai/models/embeddings.py
--rw-r--r--   0        0        0      713 2024-03-26 15:00:33.067484 mistralai-0.1.8/src/mistralai/models/models.py
--rw-r--r--   0        0        0        0 2024-03-26 15:00:33.067484 mistralai-0.1.8/src/mistralai/py.typed
--rw-r--r--   0        0        0     1836 1970-01-01 00:00:00.000000 mistralai-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-23 16:38:56.123877 mistralai-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1286 2024-05-23 16:38:56.123877 mistralai-0.2.0/README.md
+-rw-r--r--   0        0        0      790 2024-05-23 16:38:56.127877 mistralai-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/__init__.py
+-rw-r--r--   0        0        0    11378 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/async_client.py
+-rw-r--r--   0        0        0    11119 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/client.py
+-rw-r--r--   0        0        0     4710 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/client_base.py
+-rw-r--r--   0        0        0       84 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/constants.py
+-rw-r--r--   0        0        0     1652 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/models/__init__.py
+-rw-r--r--   0        0        0     1884 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/models/chat_completion.py
+-rw-r--r--   0        0        0      172 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/models/common.py
+-rw-r--r--   0        0        0      331 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/models/embeddings.py
+-rw-r--r--   0        0        0      714 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/models/models.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/py.typed
+-rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 mistralai-0.2.0/PKG-INFO
```

### Comparing `mistralai-0.1.8/LICENSE` & `mistralai-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mistralai-0.1.8/README.md` & `mistralai-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mistralai-0.1.8/pyproject.toml` & `mistralai-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mistralai"
-version = "0.1.8"
+version = "0.2.0"
 description = ""
 authors = ["Bam4d <bam4d@mistral.ai>"]
 readme = "README.md"
 
 [tool.ruff]
 select = ["E", "F", "W", "Q", "I"]
 ignore = ["E203"]
@@ -22,15 +22,15 @@
 exclude = ["docs", "tests", "examples", "tools", "build"]
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 orjson = "^3.9.10"
 pydantic = "^2.5.2"
-httpx = "^0.25.2"
+httpx = ">= 0.25.2, < 1"
 
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.1.6"
 mypy = "^1.7.1"
 types-requests = "^2.31.0.10"
 pytest = "^7.4.3"
```

### Comparing `mistralai-0.1.8/src/mistralai/async_client.py` & `mistralai-0.2.0/src/mistralai/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import os
+import asyncio
 import posixpath
-import time
 from json import JSONDecodeError
 from typing import Any, AsyncGenerator, Dict, List, Optional, Union
 
 from httpx import (
     AsyncClient,
     AsyncHTTPTransport,
     ConnectError,
@@ -30,15 +29,15 @@
 from mistralai.models.embeddings import EmbeddingResponse
 from mistralai.models.models import ModelList
 
 
 class MistralAsyncClient(ClientBase):
     def __init__(
         self,
-        api_key: Optional[str] = os.environ.get("MISTRAL_API_KEY", None),
+        api_key: Optional[str] = None,
         endpoint: str = ENDPOINT,
         max_retries: int = 5,
         timeout: int = 120,
         max_concurrent_requests: int = 64,
     ):
         super().__init__(endpoint, api_key, max_retries, timeout)
 
@@ -147,15 +146,15 @@
                 message=f"Failed to decode json body: {response.text}",
             ) from e
         except MistralAPIStatusException as e:
             attempt += 1
             if attempt > self._max_retries:
                 raise MistralAPIStatusException.from_response(response, message=str(e)) from e
             backoff = 2.0**attempt  # exponential backoff
-            time.sleep(backoff)
+            await asyncio.sleep(backoff)
 
             # Retry as a generator
             async for r in self._request(method, json, path, stream=stream, attempt=attempt):
                 yield r
 
     async def chat(
         self,
```

### Comparing `mistralai-0.1.8/src/mistralai/client.py` & `mistralai-0.2.0/src/mistralai/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import posixpath
 import time
 from json import JSONDecodeError
 from typing import Any, Dict, Iterable, Iterator, List, Optional, Union
 
 from httpx import Client, ConnectError, HTTPTransport, RequestError, Response
 
@@ -27,15 +26,15 @@
 class MistralClient(ClientBase):
     """
     Synchronous wrapper around the async client
     """
 
     def __init__(
         self,
-        api_key: Optional[str] = os.environ.get("MISTRAL_API_KEY", None),
+        api_key: Optional[str] = None,
         endpoint: str = ENDPOINT,
         max_retries: int = 5,
         timeout: int = 120,
     ):
         super().__init__(endpoint, api_key, max_retries, timeout)
 
         self._client = Client(
```

### Comparing `mistralai-0.1.8/src/mistralai/client_base.py` & `mistralai-0.2.0/src/mistralai/client_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,41 +6,41 @@
 import orjson
 
 from mistralai.exceptions import (
     MistralException,
 )
 from mistralai.models.chat_completion import ChatMessage, Function, ResponseFormat, ToolChoice
 
-logging.basicConfig(
-    format="%(asctime)s %(levelname)s %(name)s: %(message)s",
-    level=os.getenv("LOG_LEVEL", "ERROR"),
-)
+CLIENT_VERSION = "0.2.0"
 
 
 class ClientBase(ABC):
     def __init__(
         self,
         endpoint: str,
         api_key: Optional[str] = None,
         max_retries: int = 5,
         timeout: int = 120,
     ):
         self._max_retries = max_retries
         self._timeout = timeout
 
-        self._endpoint = endpoint
+        if api_key is None:
+            api_key = os.environ.get("MISTRAL_API_KEY")
+        if api_key is None:
+            raise MistralException(message="API key not provided. Please set MISTRAL_API_KEY environment variable.")
         self._api_key = api_key
+        self._endpoint = endpoint
         self._logger = logging.getLogger(__name__)
 
         # For azure endpoints, we default to the mistral model
         if "inference.azure.com" in self._endpoint:
             self._default_model = "mistral"
 
-        # This should be automatically updated by the deploy script
-        self._version = "0.1.8"
+        self._version = CLIENT_VERSION
 
     def _parse_tools(self, tools: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
         parsed_tools: List[Dict[str, Any]] = []
         for tool in tools:
             if tool["type"] == "function":
                 parsed_function = {}
                 parsed_function["type"] = tool["type"]
```

### Comparing `mistralai-0.1.8/src/mistralai/exceptions.py` & `mistralai-0.2.0/src/mistralai/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,24 +31,24 @@
         headers: Optional[Dict[str, Any]] = None,
     ) -> None:
         super().__init__(message)
         self.http_status = http_status
         self.headers = headers or {}
 
     @classmethod
-    def from_response(
-        cls, response: Response, message: Optional[str] = None
-    ) -> MistralAPIException:
+    def from_response(cls, response: Response, message: Optional[str] = None) -> MistralAPIException:
         return cls(
             message=message or response.text,
             http_status=response.status_code,
             headers=dict(response.headers),
         )
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(message={str(self)}, http_status={self.http_status})"
 
+
 class MistralAPIStatusException(MistralAPIException):
     """Returned when we receive a non-200 response from the API that we should retry"""
 
+
 class MistralConnectionException(MistralException):
     """Returned when the SDK can not reach the API server for any reason"""
```

### Comparing `mistralai-0.1.8/src/mistralai/models/chat_completion.py` & `mistralai-0.2.0/src/mistralai/models/chat_completion.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
 
 class ChatMessage(BaseModel):
     role: str
     content: Union[str, List[str]]
     name: Optional[str] = None
     tool_calls: Optional[List[ToolCall]] = None
+    tool_call_id: Optional[str] = None
 
 
 class DeltaMessage(BaseModel):
     role: Optional[str] = None
     content: Optional[str] = None
     tool_calls: Optional[List[ToolCall]] = None
```

### Comparing `mistralai-0.1.8/src/mistralai/models/models.py` & `mistralai-0.2.0/src/mistralai/models/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     allow_search_indices: bool = False
     allow_view: bool = True
     allow_fine_tuning: bool = False
     organization: str = "*"
     group: Optional[str] = None
     is_blocking: bool = False
 
+
 class ModelCard(BaseModel):
     id: str
     object: str
     created: int
     owned_by: str
     root: Optional[str] = None
     parent: Optional[str] = None
```

### Comparing `mistralai-0.1.8/PKG-INFO` & `mistralai-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: mistralai
-Version: 0.1.8
+Version: 0.2.0
 Summary: 
 Author: Bam4d
 Author-email: bam4d@mistral.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: httpx (>=0.25.2,<0.26.0)
+Requires-Dist: httpx (>=0.25.2,<1)
 Requires-Dist: orjson (>=3.9.10,<4.0.0)
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Mistral Python Client
 
 This client is inspired from [cohere-python](https://github.com/cohere-ai/cohere-python)
```

