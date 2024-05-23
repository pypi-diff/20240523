# Comparing `tmp/equivalent_llm-0.3.0.tar.gz` & `tmp/equivalent_llm-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equivalent_llm-0.3.0.tar", last modified: Mon May 20 05:52:51 2024, max compression
+gzip compressed data, was "equivalent_llm-0.3.2.tar", last modified: Thu May 23 09:25:57 2024, max compression
```

## Comparing `equivalent_llm-0.3.0.tar` & `equivalent_llm-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1469 2024-05-20 05:52:37.239201 equivalent_llm-0.3.0/LICENSE
--rw-r--r--   0        0        0     7297 2024-05-20 05:52:37.239201 equivalent_llm-0.3.0/README.md
--rw-r--r--   0        0        0     2050 2024-05-20 05:52:51.335234 equivalent_llm-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    13172 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/__init__.py
--rw-r--r--   0        0        0      194 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/engine/__init__.py
--rw-r--r--   0        0        0     1289 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/engine/openai.py
--rw-r--r--   0        0        0     2966 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/engine/pet.py
--rw-r--r--   0        0        0     5896 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/function/v1/__init__.py
--rw-r--r--   0        0        0     7402 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/function/v2/__init__.py
--rw-r--r--   0        0        0     7547 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/function_call/__init__.py
--rw-r--r--   0        0        0    13831 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/function_call/v1/__init__.py
--rw-r--r--   0        0        0    12430 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/function_call/v2/__init__.py
--rw-r--r--   0        0        0      571 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/parse/__init__.py
--rw-r--r--   0        0        0     8544 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/reservation.py
--rw-r--r--   0        0        0    13183 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/testers/__init__.py
--rw-r--r--   0        0        0     2667 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/user.py
--rw-r--r--   0        0        0        0 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     8182 1970-01-01 00:00:00.000000 equivalent_llm-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1469 2024-05-23 09:25:40.319812 equivalent_llm-0.3.2/LICENSE
+-rw-r--r--   0        0        0     7297 2024-05-23 09:25:40.319812 equivalent_llm-0.3.2/README.md
+-rw-r--r--   0        0        0     2050 2024-05-23 09:25:57.103871 equivalent_llm-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    13172 2024-05-23 09:25:40.343812 equivalent_llm-0.3.2/src/equivalent_llm/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-23 09:25:40.343812 equivalent_llm-0.3.2/src/equivalent_llm/engine/__init__.py
+-rw-r--r--   0        0        0     1289 2024-05-23 09:25:40.343812 equivalent_llm-0.3.2/src/equivalent_llm/engine/openai.py
+-rw-r--r--   0        0        0     3639 2024-05-23 09:25:40.343812 equivalent_llm-0.3.2/src/equivalent_llm/engine/pet.py
+-rw-r--r--   0        0        0     5896 2024-05-23 09:25:40.343812 equivalent_llm-0.3.2/src/equivalent_llm/function/v1/__init__.py
+-rw-r--r--   0        0        0     7402 2024-05-23 09:25:40.343812 equivalent_llm-0.3.2/src/equivalent_llm/function/v2/__init__.py
+-rw-r--r--   0        0        0     7599 2024-05-23 09:25:40.343812 equivalent_llm-0.3.2/src/equivalent_llm/function_call/__init__.py
+-rw-r--r--   0        0        0    13831 2024-05-23 09:25:40.343812 equivalent_llm-0.3.2/src/equivalent_llm/function_call/v1/__init__.py
+-rw-r--r--   0        0        0    12430 2024-05-23 09:25:40.343812 equivalent_llm-0.3.2/src/equivalent_llm/function_call/v2/__init__.py
+-rw-r--r--   0        0        0      571 2024-05-23 09:25:40.343812 equivalent_llm-0.3.2/src/equivalent_llm/parse/__init__.py
+-rw-r--r--   0        0        0     8544 2024-05-23 09:25:40.343812 equivalent_llm-0.3.2/src/equivalent_llm/reservation.py
+-rw-r--r--   0        0        0    13214 2024-05-23 09:25:40.343812 equivalent_llm-0.3.2/src/equivalent_llm/testers/__init__.py
+-rw-r--r--   0        0        0     2667 2024-05-23 09:25:40.343812 equivalent_llm-0.3.2/src/equivalent_llm/user.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:25:40.343812 equivalent_llm-0.3.2/tests/__init__.py
+-rw-r--r--   0        0        0     8182 1970-01-01 00:00:00.000000 equivalent_llm-0.3.2/PKG-INFO
```

### Comparing `equivalent_llm-0.3.0/LICENSE` & `equivalent_llm-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `equivalent_llm-0.3.0/README.md` & `equivalent_llm-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `equivalent_llm-0.3.0/pyproject.toml` & `equivalent_llm-0.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 max-complexity = 10
 
 [tool.pdm]
 distribution = true
 
 [project]
 name = "equivalent_llm"
-version = "0.3.0"
+version = "0.3.2"
 description = "Validation tool to compare a generated context by sLLM to reference context"
 authors = [
     { name = "Sung Gon Yi", email = "skonmeme@sk.com" },
 ]
 dependencies = [
     "langchain-core>=0.1.30",
     "langchain>=0.1.11",
```

### Comparing `equivalent_llm-0.3.0/src/equivalent_llm/__init__.py` & `equivalent_llm-0.3.2/src/equivalent_llm/__init__.py`

 * *Files identical despite different names*

### Comparing `equivalent_llm-0.3.0/src/equivalent_llm/engine/openai.py` & `equivalent_llm-0.3.2/src/equivalent_llm/engine/openai.py`

 * *Files identical despite different names*

### Comparing `equivalent_llm-0.3.0/src/equivalent_llm/engine/pet.py` & `equivalent_llm-0.3.2/src/equivalent_llm/engine/pet.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
+import logging
 import os
-from langchain_core.messages.function import FunctionMessage
+import re
 import requests
 from logging import Logger
 from typing import List, Union
 
 from langchain_core.messages import AIMessage, BaseMessage, FunctionMessage, SystemMessage
 
 from pydantic import BaseModel, Field
@@ -27,19 +28,21 @@
     state: int
     res: PETCompletionResponse
 
 class PET(PromptEngine):
     _DEFUALT_PET_URL = 'http://172.18.243.211:13100'
     _DEFAULT_PET_ID = '124102'
     _DEFAULT_PET_TIMEOUT = 60
+    _DEFAULT_RETRYT = 3
 
     def __init__(self, logger: Logger, **kwargs):
         self.pet_id = os.environ['PET_ID'] if 'PET_ID' in os.environ else self._DEFAULT_PET_ID
         self.pet_url = os.environ['PET_URL'] if 'PET_URL' in os.environ else self._DEFUALT_PET_URL
         self.pet_timeout = int(os.environ['PET_TIMEOUT']) if 'PET_TIMEOUT' in os.environ else self._DEFAULT_PET_TIMEOUT
+        self.retry = int(os.environ['PET_RETRY']) if 'PET_RETRY' in os.environ else self._DEFAULT_PET_TIMEOUT
 
         self.logger = logger
 
     def a(self) -> dict:
         return {}
 
     def _message_to_content(self, message: BaseMessage) -> dict:
@@ -64,17 +67,26 @@
         headers = {'Content-Type': 'application/json'}
         request_body = {
             'promptId': self.pet_id,
             'transactionId': 'movie-validation',
             'role': 'user',
             'requestTexts': [{'key': 'content', 'value': self.messages_to_contents(messages)}],
         }
-        response = requests.post(url=completion_url, headers=headers, data=json.dumps(request_body), timeout=self.pet_timeout)
 
+        response = requests.post(url=completion_url, headers=headers, data=json.dumps(request_body), timeout=self.pet_timeout)
+        count = self.retry - 1
+        while (response.status_code // 100) != 2 and count > 0:
+            response = requests.post(url=completion_url, headers=headers, data=json.dumps(request_body), timeout=self.pet_timeout)
+            count -= 1
+        if count <= 0:
+            logging.error(f"### PET request failed: {response.status_code}: {request_body}")
         parsed_response = PETResponse(**json_loads(response.content))
         self.logger.debug(f"### PET response: {parsed_response}")
 
         result = parsed_response.res.content
+        if not result.startswith("[") and not result.startswith("{"):
+            found = re.search(r"```json.+```", result, flags=re.DOTALL)
+            result = found.group() if found is not None else result
         if result.startswith("```json"):
             return json_loads(result.split("```json")[1].split("```")[0])
         else:
             return json_loads(result)
```

### Comparing `equivalent_llm-0.3.0/src/equivalent_llm/function/v1/__init__.py` & `equivalent_llm-0.3.2/src/equivalent_llm/function/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `equivalent_llm-0.3.0/src/equivalent_llm/function/v2/__init__.py` & `equivalent_llm-0.3.2/src/equivalent_llm/function/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `equivalent_llm-0.3.0/src/equivalent_llm/function_call/__init__.py` & `equivalent_llm-0.3.2/src/equivalent_llm/function_call/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,14 +157,16 @@
     reports['tests']['paired_arguments'] = paired_arguments_result
     etc_counter.count(paired_arguments_result)
 
     # value type
     logger.debug(f"FUNCTION_NAME: {function_name.upper()}")
     for name in reference['arguments']:
         definition = DEFINITION['parameters'].get(name)
+        if definition is None:
+            continue
 
         # equivalence tests
         equivalence_result = equivalence_test(
             generated['arguments'].get(name),
             reference['arguments'].get(name),
             instructions,
             definition['equivalence'],
```

### Comparing `equivalent_llm-0.3.0/src/equivalent_llm/function_call/v1/__init__.py` & `equivalent_llm-0.3.2/src/equivalent_llm/function_call/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `equivalent_llm-0.3.0/src/equivalent_llm/function_call/v2/__init__.py` & `equivalent_llm-0.3.2/src/equivalent_llm/function_call/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `equivalent_llm-0.3.0/src/equivalent_llm/parse/__init__.py` & `equivalent_llm-0.3.2/src/equivalent_llm/parse/__init__.py`

 * *Files identical despite different names*

### Comparing `equivalent_llm-0.3.0/src/equivalent_llm/reservation.py` & `equivalent_llm-0.3.2/src/equivalent_llm/reservation.py`

 * *Files identical despite different names*

### Comparing `equivalent_llm-0.3.0/src/equivalent_llm/testers/__init__.py` & `equivalent_llm-0.3.2/src/equivalent_llm/testers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         new_counter = TestCounter()
         new_counter.passed = self.passed + counter.passed
         new_counter.total = self.total + counter.total
         return new_counter
 
     def count(self, validation: dict):
         self.total += 1
-        if validation['passed']:
+        if validation is not None and validation.get('passed'):
             self.passed += 1
 
     def fully_passed(self):
         return self.passed == self.total
 
     def settlement(self):
         return {'passed': self.passed, 'total': self.total}
```

### Comparing `equivalent_llm-0.3.0/src/equivalent_llm/user.py` & `equivalent_llm-0.3.2/src/equivalent_llm/user.py`

 * *Files identical despite different names*

### Comparing `equivalent_llm-0.3.0/PKG-INFO` & `equivalent_llm-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equivalent_llm
-Version: 0.3.0
+Version: 0.3.2
 Summary: Validation tool to compare a generated context by sLLM to reference context
 Author-Email: Sung Gon Yi <skonmeme@sk.com>
 License: BSD-3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/sktaiflow/equivalent_llm
```

