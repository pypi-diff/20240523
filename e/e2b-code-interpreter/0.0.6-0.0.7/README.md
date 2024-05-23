# Comparing `tmp/e2b_code_interpreter-0.0.6.tar.gz` & `tmp/e2b_code_interpreter-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2b_code_interpreter-0.0.6.tar", max compression
+gzip compressed data, was "e2b_code_interpreter-0.0.7.tar", max compression
```

## Comparing `e2b_code_interpreter-0.0.6.tar` & `e2b_code_interpreter-0.0.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2331 2024-05-14 23:43:53.442159 e2b_code_interpreter-0.0.6/README.md
--rw-r--r--   0        0        0      149 2024-05-14 23:43:53.442159 e2b_code_interpreter-0.0.6/e2b_code_interpreter/__init__.py
--rw-r--r--   0        0        0    11079 2024-05-14 23:43:53.442159 e2b_code_interpreter-0.0.6/e2b_code_interpreter/main.py
--rw-r--r--   0        0        0     8821 2024-05-14 23:43:53.446159 e2b_code_interpreter-0.0.6/e2b_code_interpreter/messaging.py
--rw-r--r--   0        0        0     7884 2024-05-14 23:43:53.446159 e2b_code_interpreter-0.0.6/e2b_code_interpreter/models.py
--rw-r--r--   0        0        0      766 2024-05-14 23:44:20.110434 e2b_code_interpreter-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3246 1970-01-01 00:00:00.000000 e2b_code_interpreter-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     2331 2024-05-23 09:16:43.243391 e2b_code_interpreter-0.0.7/README.md
+-rw-r--r--   0        0        0      149 2024-05-23 09:16:43.243391 e2b_code_interpreter-0.0.7/e2b_code_interpreter/__init__.py
+-rw-r--r--   0        0        0    11080 2024-05-23 09:16:43.243391 e2b_code_interpreter-0.0.7/e2b_code_interpreter/main.py
+-rw-r--r--   0        0        0     8759 2024-05-23 09:16:43.243391 e2b_code_interpreter-0.0.7/e2b_code_interpreter/messaging.py
+-rw-r--r--   0        0        0     7884 2024-05-23 09:16:43.243391 e2b_code_interpreter-0.0.7/e2b_code_interpreter/models.py
+-rw-r--r--   0        0        0      766 2024-05-23 09:17:15.003308 e2b_code_interpreter-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3246 1970-01-01 00:00:00.000000 e2b_code_interpreter-0.0.7/PKG-INFO
```

### Comparing `e2b_code_interpreter-0.0.6/README.md` & `e2b_code_interpreter-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `e2b_code_interpreter-0.0.6/e2b_code_interpreter/main.py` & `e2b_code_interpreter-0.0.7/e2b_code_interpreter/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         :param cwd: Sets the current working directory for the kernel. Defaults to "/home/user".
         :param kernel_name:
             Specifies which kernel should be used, useful if you have multiple kernel types.
             If not provided, the default kernel will be used.
         :param timeout: Timeout for the kernel creation request.
         :return: Kernel id of the created kernel
         """
-        data = {"cwd": cwd}
+        data = {"path": cwd}
         if kernel_name:
             data["kernel_name"] = kernel_name
         logger.debug(f"Creating kernel with data: {data}")
 
         response = requests.post(
             f"{self._sandbox.get_protocol()}://{self._sandbox.get_hostname(8888)}/api/kernels",
             json=data,
```

### Comparing `e2b_code_interpreter-0.0.6/e2b_code_interpreter/messaging.py` & `e2b_code_interpreter-0.0.7/e2b_code_interpreter/messaging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import json
 import logging
 import threading
 import time
 import uuid
 from concurrent.futures import Future
 from queue import Queue
-from typing import Callable, Dict, List, Any, Optional
+from typing import Callable, Dict, Any, Optional
 
 from e2b import ProcessMessage
 from e2b.constants import TIMEOUT
 from e2b.sandbox import TimeoutException
 from e2b.sandbox.websocket_client import WebSocket
 from e2b.utils.future import DeferredFuture
-from pydantic import ConfigDict, PrivateAttr, BaseModel
 
 from e2b_code_interpreter.models import Execution, Result, Error
 
 logger = logging.getLogger(__name__)
 
 
 class CellExecution:
```

### Comparing `e2b_code_interpreter-0.0.6/e2b_code_interpreter/models.py` & `e2b_code_interpreter-0.0.7/e2b_code_interpreter/models.py`

 * *Files identical despite different names*

### Comparing `e2b_code_interpreter-0.0.6/pyproject.toml` & `e2b_code_interpreter-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "e2b-code-interpreter"
-version = "0.0.6"
+version = "0.0.7"
 description = "E2B Code Interpreter - Stateful code execution"
 authors = ["e2b <hello@e2b.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://e2b.dev/"
 repository = "https://github.com/e2b-dev/e2b-code-interpreter/tree/python"
 packages = [{ include = "e2b_code_interpreter" }]
```

### Comparing `e2b_code_interpreter-0.0.6/PKG-INFO` & `e2b_code_interpreter-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2b-code-interpreter
-Version: 0.0.6
+Version: 0.0.7
 Summary: E2B Code Interpreter - Stateful code execution
 Home-page: https://e2b.dev/
 License: Apache-2.0
 Author: e2b
 Author-email: hello@e2b.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

