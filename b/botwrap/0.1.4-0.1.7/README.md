# Comparing `tmp/botwrap-0.1.4.tar.gz` & `tmp/botwrap-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botwrap-0.1.4.tar", last modified: Fri Apr  5 20:12:09 2024, max compression
+gzip compressed data, was "botwrap-0.1.7.tar", last modified: Thu May 23 00:53:11 2024, max compression
```

## Comparing `botwrap-0.1.4.tar` & `botwrap-0.1.7.tar`

### file list

```diff
@@ -1,36 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 20:12:09.077979 botwrap-0.1.4/
--rw-rw-rw-   0        0        0     3277 2024-04-05 20:12:09.074657 botwrap-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1513 2024-03-23 23:09:32.000000 botwrap-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 20:12:09.071651 botwrap-0.1.4/botwrap.egg-info/
--rw-rw-rw-   0        0        0     3277 2024-04-05 20:12:08.000000 botwrap-0.1.4/botwrap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      726 2024-04-05 20:12:08.000000 botwrap-0.1.4/botwrap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 20:12:08.000000 botwrap-0.1.4/botwrap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      222 2024-04-05 20:12:08.000000 botwrap-0.1.4/botwrap.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-05 20:12:08.000000 botwrap-0.1.4/botwrap.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 20:12:09.033403 botwrap-0.1.4/openaiwrapper/
--rw-rw-rw-   0        0        0        0 2024-03-22 23:19:35.000000 botwrap-0.1.4/openaiwrapper/__init__.py
--rw-rw-rw-   0        0        0     3860 2024-04-05 19:29:34.000000 botwrap-0.1.4/openaiwrapper/api_client.py
--rw-rw-rw-   0        0        0     3300 2024-04-04 06:28:29.000000 botwrap-0.1.4/openaiwrapper/assistants.py
--rw-rw-rw-   0        0        0     1400 2024-04-04 06:36:55.000000 botwrap-0.1.4/openaiwrapper/config.py
--rw-rw-rw-   0        0        0     1919 2024-04-05 20:09:31.000000 botwrap-0.1.4/openaiwrapper/exceptions.py
--rw-rw-rw-   0        0        0     4342 2024-04-04 06:26:25.000000 botwrap-0.1.4/openaiwrapper/files.py
--rw-rw-rw-   0        0        0     3046 2024-04-04 06:15:41.000000 botwrap-0.1.4/openaiwrapper/messages.py
--rw-rw-rw-   0        0        0    11316 2024-04-05 20:10:03.000000 botwrap-0.1.4/openaiwrapper/openai_wrapper.py
--rw-rw-rw-   0        0        0     2770 2024-04-04 06:21:44.000000 botwrap-0.1.4/openaiwrapper/runs.py
--rw-rw-rw-   0        0        0     2866 2024-04-04 06:18:54.000000 botwrap-0.1.4/openaiwrapper/threads.py
--rw-rw-rw-   0        0        0     3127 2024-04-04 06:39:51.000000 botwrap-0.1.4/openaiwrapper/tools.py
--rw-rw-rw-   0        0        0     3569 2024-04-04 06:44:47.000000 botwrap-0.1.4/openaiwrapper/utils.py
--rw-rw-rw-   0        0        0       42 2024-04-05 20:12:09.077979 botwrap-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1447 2024-04-05 20:11:57.000000 botwrap-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:12:09.069602 botwrap-0.1.4/tests/
--rw-rw-rw-   0        0        0        0 2024-03-22 23:19:35.000000 botwrap-0.1.4/tests/__init__.py
--rw-rw-rw-   0        0        0     2127 2024-04-05 19:32:00.000000 botwrap-0.1.4/tests/test_api_client.py
--rw-rw-rw-   0        0        0     2746 2024-04-05 19:00:48.000000 botwrap-0.1.4/tests/test_assistants.py
--rw-rw-rw-   0        0        0     2290 2024-04-05 19:07:26.000000 botwrap-0.1.4/tests/test_exceptions.py
--rw-rw-rw-   0        0        0     2085 2024-04-05 19:03:58.000000 botwrap-0.1.4/tests/test_files.py
--rw-rw-rw-   0        0        0     2427 2024-04-05 19:05:25.000000 botwrap-0.1.4/tests/test_messages.py
--rw-rw-rw-   0        0        0     2845 2024-04-05 19:21:07.000000 botwrap-0.1.4/tests/test_openai_wrapper.py
--rw-rw-rw-   0        0        0     2435 2024-04-05 19:07:10.000000 botwrap-0.1.4/tests/test_runs.py
--rw-rw-rw-   0        0        0     2858 2024-04-05 19:09:58.000000 botwrap-0.1.4/tests/test_threads.py
--rw-rw-rw-   0        0        0     2869 2024-04-05 19:16:17.000000 botwrap-0.1.4/tests/test_tools.py
--rw-rw-rw-   0        0        0     3376 2024-04-05 19:18:51.000000 botwrap-0.1.4/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 00:53:11.529975 botwrap-0.1.7/
+-rw-rw-rw-   0        0        0     5160 2024-05-23 00:53:11.526980 botwrap-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3829 2024-05-23 00:52:39.000000 botwrap-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 00:53:11.524464 botwrap-0.1.7/botwrap.egg-info/
+-rw-rw-rw-   0        0        0     5160 2024-05-23 00:53:11.000000 botwrap-0.1.7/botwrap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      919 2024-05-23 00:53:11.000000 botwrap-0.1.7/botwrap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 00:53:11.000000 botwrap-0.1.7/botwrap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-23 00:53:11.000000 botwrap-0.1.7/botwrap.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      243 2024-05-23 00:53:11.000000 botwrap-0.1.7/botwrap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-23 00:53:11.000000 botwrap-0.1.7/botwrap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 00:53:11.498035 botwrap-0.1.7/openaiwrapper/
+-rw-rw-rw-   0        0        0        0 2024-03-22 23:19:35.000000 botwrap-0.1.7/openaiwrapper/__init__.py
+-rw-rw-rw-   0        0        0     4558 2024-05-22 04:25:50.000000 botwrap-0.1.7/openaiwrapper/api_client.py
+-rw-rw-rw-   0        0        0     4022 2024-05-22 04:26:28.000000 botwrap-0.1.7/openaiwrapper/assistants.py
+-rw-rw-rw-   0        0        0     2369 2024-05-22 04:27:48.000000 botwrap-0.1.7/openaiwrapper/config.py
+-rw-rw-rw-   0        0        0      717 2024-05-22 04:37:27.000000 botwrap-0.1.7/openaiwrapper/decorators.py
+-rw-rw-rw-   0        0        0     1134 2024-05-22 04:28:08.000000 botwrap-0.1.7/openaiwrapper/error_logging.py
+-rw-rw-rw-   0        0        0     3050 2024-05-22 04:28:25.000000 botwrap-0.1.7/openaiwrapper/exceptions.py
+-rw-rw-rw-   0        0        0     3010 2024-05-22 04:52:00.000000 botwrap-0.1.7/openaiwrapper/files.py
+-rw-rw-rw-   0        0        0     4340 2024-05-22 04:54:22.000000 botwrap-0.1.7/openaiwrapper/messages.py
+-rw-rw-rw-   0        0        0     7328 2024-05-23 00:40:00.000000 botwrap-0.1.7/openaiwrapper/minimal_test_convo.py
+-rw-rw-rw-   0        0        0     6272 2024-05-22 04:29:24.000000 botwrap-0.1.7/openaiwrapper/openai_wrapper.py
+-rw-rw-rw-   0        0        0     3142 2024-05-22 04:29:37.000000 botwrap-0.1.7/openaiwrapper/profiles.py
+-rw-rw-rw-   0        0        0     3933 2024-05-23 00:09:00.000000 botwrap-0.1.7/openaiwrapper/runs.py
+-rw-rw-rw-   0        0        0     4329 2024-05-23 00:11:40.000000 botwrap-0.1.7/openaiwrapper/threads.py
+-rw-rw-rw-   0        0        0     3927 2024-05-22 04:54:39.000000 botwrap-0.1.7/openaiwrapper/tools.py
+-rw-rw-rw-   0        0        0     4699 2024-05-22 04:30:25.000000 botwrap-0.1.7/openaiwrapper/utils.py
+-rw-rw-rw-   0        0        0     3651 2024-05-22 04:55:48.000000 botwrap-0.1.7/openaiwrapper/vector_store_manager.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 00:53:11.530975 botwrap-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1608 2024-05-23 00:50:09.000000 botwrap-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 00:53:11.522477 botwrap-0.1.7/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-22 23:19:35.000000 botwrap-0.1.7/tests/__init__.py
+-rw-rw-rw-   0        0        0     2127 2024-04-05 19:32:00.000000 botwrap-0.1.7/tests/test_api_client.py
+-rw-rw-rw-   0        0        0     2746 2024-04-05 19:00:48.000000 botwrap-0.1.7/tests/test_assistants.py
+-rw-rw-rw-   0        0        0     2290 2024-04-05 19:07:26.000000 botwrap-0.1.7/tests/test_exceptions.py
+-rw-rw-rw-   0        0        0     2085 2024-04-05 19:03:58.000000 botwrap-0.1.7/tests/test_files.py
+-rw-rw-rw-   0        0        0     2427 2024-04-05 19:05:25.000000 botwrap-0.1.7/tests/test_messages.py
+-rw-rw-rw-   0        0        0     2845 2024-04-05 19:21:07.000000 botwrap-0.1.7/tests/test_openai_wrapper.py
+-rw-rw-rw-   0        0        0     2435 2024-04-05 19:07:10.000000 botwrap-0.1.7/tests/test_runs.py
+-rw-rw-rw-   0        0        0     2858 2024-04-05 19:09:58.000000 botwrap-0.1.7/tests/test_threads.py
+-rw-rw-rw-   0        0        0     2869 2024-04-05 19:16:17.000000 botwrap-0.1.7/tests/test_tools.py
+-rw-rw-rw-   0        0        0     3376 2024-04-05 19:18:51.000000 botwrap-0.1.7/tests/test_utils.py
```

### Comparing `botwrap-0.1.4/botwrap.egg-info/SOURCES.txt` & `botwrap-0.1.7/botwrap.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 README.md
 setup.py
 botwrap.egg-info/PKG-INFO
 botwrap.egg-info/SOURCES.txt
 botwrap.egg-info/dependency_links.txt
+botwrap.egg-info/entry_points.txt
 botwrap.egg-info/requires.txt
 botwrap.egg-info/top_level.txt
 openaiwrapper/__init__.py
 openaiwrapper/api_client.py
 openaiwrapper/assistants.py
 openaiwrapper/config.py
+openaiwrapper/decorators.py
+openaiwrapper/error_logging.py
 openaiwrapper/exceptions.py
 openaiwrapper/files.py
 openaiwrapper/messages.py
+openaiwrapper/minimal_test_convo.py
 openaiwrapper/openai_wrapper.py
+openaiwrapper/profiles.py
 openaiwrapper/runs.py
 openaiwrapper/threads.py
 openaiwrapper/tools.py
 openaiwrapper/utils.py
+openaiwrapper/vector_store_manager.py
 tests/__init__.py
 tests/test_api_client.py
 tests/test_assistants.py
 tests/test_exceptions.py
 tests/test_files.py
 tests/test_messages.py
 tests/test_openai_wrapper.py
```

### Comparing `botwrap-0.1.4/openaiwrapper/assistants.py` & `botwrap-0.1.7/openaiwrapper/assistants.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,78 @@
-##Path C:\Users\jamig\OneDrive\Desktop\botwrap\openaiwrapper\assistants.py
+# Path: C:\Users\jamig\OneDrive\Desktop\botwrap\openaiwrapper\assistants.py
 
 import logging
+from typing import List, Dict, Optional, Any
+from .profiles import ProfileManager
+from .decorators import log_error_decorator
 
 class AssistantManager:
-    def __init__(self, api_client, thread_manager=None, message_manager=None):
-        self.api_client = api_client
-        self.thread_manager = thread_manager
-        self.message_manager = message_manager
-        self.logger = logging.getLogger(__name__)
-
-    async def _validate_tools_config(self, tools):
-        if tools is not None and not all(isinstance(tool, dict) for tool in tools):
-            raise ValueError("Tools configuration must be a list of dictionaries.")
-
-    async def create(self, name, instructions, model, tools=None, **kwargs):
-        """Creates a new Assistant asynchronously."""
-        await self._validate_tools_config(tools)
-        data = {
-            "name": name,
-            "instructions": instructions,
-            "model": model,
-            "tools": tools or [],
-            **kwargs
-        }
-        self.logger.info(f"Creating new assistant with name: {name}")
-        return await self.api_client.make_api_call("assistants", method="POST", data=data)
-
-    async def start_conversation(self, assistant_id, initial_message=None):
-        if not self.thread_manager or not self.message_manager:
-            raise NotImplementedError("ThreadManager and Message Manager must be initialized.")
-
-        thread_response = await self.thread_manager.create()
-        thread_id = thread_response.get('id')
-        if initial_message:
-            await self.message_manager.create(thread_id, initial_message, role="user")
-        return thread_response
-
-    async def create_from_template(self, template_name, **overrides):
-        templates = self._load_templates()
-        if template_name not in templates:
-            raise ValueError(f"Template '{template_name}' not found.")
-
-        template_config = templates[template_name]
-        template_config.update(overrides)
-        return await self.create(**template_config)
-
-    def _load_templates(self):
-        templates = {
-            "basic_chat": {
-                "name": "Basic Chat Assistant",
-                "instructions": "You are a friendly chatbot.",
-                "model": "gpt-3.5-turbo",
-                "tools": [],
+    def __init__(self, make_api_call, logger: Optional[logging.Logger] = None):
+        self.make_api_call = make_api_call
+        self.logger = logger or self._setup_logger()
+        self.profile_manager = ProfileManager(logger)
+
+    def _setup_logger(self) -> logging.Logger:
+        logger = logging.getLogger(__name__)
+        if not logger.handlers:
+            handler = logging.StreamHandler()
+            formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+            handler.setFormatter(formatter)
+            logger.addHandler(handler)
+        logger.setLevel(logging.INFO)
+        return logger
+
+    @log_error_decorator(logger=None)
+    async def create_assistant(self, profile_name: Optional[str] = None, profile_path: Optional[str] = None, name: Optional[str] = None, instructions: Optional[str] = None, model: Optional[str] = None, tools: Optional[List[Dict[str, Any]]] = None, tool_resources: Optional[Dict[str, Any]] = None, **kwargs) -> Dict:
+        if profile_name:
+            profile = self.profile_manager.load_profile(profile_name)
+            self.logger.info(f"Creating new assistant with profile: {profile_name}")
+            data = {**profile, **kwargs}
+        elif profile_path:
+            profile = self.profile_manager.load_profile_from_path(profile_path)
+            self.logger.info(f"Creating new assistant with profile from path: {profile_path}")
+            data = {**profile, **kwargs}
+        else:
+            if not (name and instructions and model):
+                self.logger.error("Name, instructions, and model must be provided if no profile is used.")
+                raise ValueError("Name, instructions, and model must be provided if no profile is used.")
+            data = {
+                "name": name,
+                "instructions": instructions,
+                "model": model,
+                "tools": tools or [],
+                "tool_resources": tool_resources or {},
+                **kwargs
             }
-        }
-        return templates
+            self.logger.info(f"Creating new assistant with name: {name}")
 
-    async def retrieve(self, assistant_id):
+        return await self.make_api_call("assistants", method="POST", data=data)
+
+    @log_error_decorator(logger=None)
+    async def retrieve(self, assistant_id: str) -> Dict:
+        self._validate_input(assistant_id, "Assistant ID")
         self.logger.info(f"Retrieving assistant with ID: {assistant_id}")
-        return await self.api_client.make_api_call(f"assistants/{assistant_id}", method="GET")
+        return await self.make_api_call(f"assistants/{assistant_id}", method="GET")
 
-    async def update(self, assistant_id, **kwargs):
-        if 'tools' in kwargs:
-            await self._validate_tools_config(kwargs['tools'])
+    @log_error_decorator(logger=None)
+    async def update(self, assistant_id: str, updates: Dict[str, Any]) -> Dict:
+        if 'tools' in updates:
+            await self._validate_tools_config(updates['tools'])
         self.logger.info(f"Updating assistant with ID: {assistant_id}")
-        return await self.api_client.make_api_call(f"assistants/{assistant_id}", method="PATCH", data=kwargs)
+        return await self.make_api_call(f"assistants/{assistant_id}", method="PATCH", data=updates)
 
-    async def delete(self, assistant_id):
+    @log_error_decorator(logger=None)
+    async def delete(self, assistant_id: str) -> Dict:
+        self._validate_input(assistant_id, "Assistant ID")
         self.logger.info(f"Deleting assistant with ID: {assistant_id}")
-        return await self.api_client.make_api_call(f"assistants/{assistant_id}", method="DELETE")
+        return await self.make_api_call(f"assistants/{assistant_id}", method="DELETE")
 
-    async def list(self, **kwargs):
-        self.logger.info("Listing assistants")
-        return await self.api_client.make_api_call("assistants", method="GET", params=kwargs)
+    @log_error_decorator(logger=None)
+    async def list(self, **kwargs) -> List[Dict]:
+        self.logger.info("Listing all assistants")
+        response = await self.make_api_call("assistants", method="GET", params=kwargs)
+        return response.get("data", [])
+
+    def _validate_input(self, input_value: str, input_name: str):
+        if not input_value:
+            self.logger.error(f"{input_name} must be provided and cannot be empty.")
+            raise ValueError(f"{input_name} must be provided and cannot be empty.")
```

### Comparing `botwrap-0.1.4/openaiwrapper/exceptions.py` & `botwrap-0.1.7/openaiwrapper/exceptions.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,78 @@
-##Path C:\Users\jamig\OneDrive\Desktop\botwrap\openaiwrapper\exceptions.py
+# Path: C:\Users\jamig\OneDrive\Desktop\botwrap\openaiwrapper\exceptions.py
 
 import logging
 import aiohttp
+from typing import Optional
 
-logger = logging.getLogger(__name__)
+# Custom Base Exception
+class OpenAIWrapperError(Exception):
+    """Base exception class for OpenAI Wrapper related errors."""
+    pass
+
+# Specific Exception classes for different error categories
+class APIConnectionError(OpenAIWrapperError):
+    pass
+
+class APITimeoutError(OpenAIWrapperError):
+    pass
+
+class APIResponseError(OpenAIWrapperError):
+    def __init__(self, message, status_code, error_type='APIResponseError', details=None):
+        super().__init__(message)
+        self.status_code = status_code
+        self.error_type = error_type
+        self.details = details
+
+class BadRequestError(APIResponseError):
+    pass
+
+class UnauthorizedError(APIResponseError):
+    pass
 
-class OpenAIRequestError(Exception):
-    """Custom exception for handling OpenAI API request errors."""
-    def __init__(self, message=None, status_code=None, error_type=None, request_id=None):
-        self.message = message or "An error occurred with the OpenAI API request."
+class ServerError(APIResponseError):
+    pass
+
+class OpenAIRequestError(APIResponseError):
+    def __init__(self, message=None, status_code=None, error_type=None, request_id=None, details=None):
+        super().__init__(message, status_code, error_type, details)
+        self.message = message
         self.status_code = status_code
         self.error_type = error_type
-        self.request_id = request_id  # Useful for logging and support
-        super().__init__(self.message)
-    
-    def __str__(self):
-        return f"{self.error_type or 'Error'}: {self.message} (Status code: {self.status_code}) Request ID: {self.request_id or 'N/A'}"
+        self.request_id = request_id
 
-async def create_openai_request_error(response: aiohttp.ClientResponse):
-    """Utility function to create an OpenAIRequestError from an aiohttp HTTP response."""
+    def __str__(self):
+        return (f"Error Type: {self.error_type}, "
+                f"Message: {self.message}, Status Code: {self.status_code}, "
+                f"Request ID: {self.request_id}, Details: {self.details}")
+
+async def create_openai_request_error(response: aiohttp.ClientResponse, logger: Optional[logging.Logger] = None) -> OpenAIRequestError:
+    if not logger:
+        logger = logging.getLogger(__name__)
     try:
         error_details = await response.json()
         error_message = error_details.get('error', {}).get('message', 'No error message provided.')
-        error_type = error_details.get('error', {}).get('type', 'Unknown')
+        error_type = error_details.get('error', {}).get('type', 'Unknown Error Type')
     except aiohttp.ContentTypeError:
         text = await response.text()
         error_message = text or "Failed to decode JSON response."
         error_type = 'ContentTypeError'
 
     status_code = response.status
-    request_id = response.headers.get('X-Request-ID')
-
+    request_id = response.headers.get('X-Request-ID', 'Not provided')
+    logger.error(f"{error_type}: {error_message} (Request ID: {request_id})")
     return OpenAIRequestError(message=error_message, status_code=status_code, error_type=error_type, request_id=request_id)
 
-def log_openai_request_error(error: OpenAIRequestError):
-    """Logs detailed information from an OpenAIRequestError."""
-    logger.error(f"OpenAIRequestError encountered: {error.error_type or 'Error'} - {error.message} "
-                 f"(Status code: {error.status_code}, Request ID: {error.request_id or 'N/A'})")
+def log_error_decorator(logger: Optional[logging.Logger] = None):
+    """Decorator to automatically log errors when they are raised."""
+    if not logger:
+        logger = logging.getLogger(__name__)
+    def decorator(func):
+        @functools.wraps(func)
+        async def wrapper(*args, **kwargs):
+            try:
+                return await func(*args, **kwargs)
+            except OpenAIWrapperError as error:
+                logger.error(f"OpenAI Request Error Logged: {error}")
+                raise  # Re-raise to handle elsewhere
+        return wrapper
+    return decorator
```

### Comparing `botwrap-0.1.4/openaiwrapper/utils.py` & `botwrap-0.1.7/openaiwrapper/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,87 @@
-##Path C:\Users\jamig\OneDrive\Desktop\botwrap\openaiwrapper\utils.py
+# Path: C:\Users\jamig\OneDrive\Desktop\botwrap\openaiwrapper\utils.py
 
 import logging
-import asyncio
 import aiohttp
 import json
 from datetime import datetime
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Optional
 from .exceptions import OpenAIRequestError
 
-# Set up structured logging
-logger = logging.getLogger(__name__)
-
-async def handle_http_error(response: aiohttp.ClientResponse) -> None:
-    """Asynchronously handles HTTP errors by raising an OpenAIRequestError with detailed message."""
-    if response.status >= 400:
-        try:
-            json_response = await response.json()
-            error_message = json_response.get('error', {}).get('message', 'No error message provided.')
-            error_type = json_response.get('error', {}).get('type', 'APIError')
-            request_id = response.headers.get('X-Request-ID', 'N/A')
-        except Exception:
-            error_message = await response.text()
-            error_type = 'UnknownError'
-            request_id = 'N/A'
-        
-        raise OpenAIRequestError(message=error_message, status_code=response.status, error_type=error_type, request_id=request_id)
-
-def log_api_call(method: str, url: str, status_code: int = None, duration: float = None, data: Dict[str, Any] = None) -> None:
-    """Logs details of an API call including method, URL, status, duration, and data in a structured format."""
-    log_data = {
-        "event": "APIRequest",
-        "method": method,
-        "url": url,
-        "status_code": status_code,
-        "duration": f"{duration:.2f}s",
-        "data": data or {}
-    }
-    logger.info(json.dumps(log_data))
-
-def validate_response_content_type(response: aiohttp.ClientResponse, expected_content_type: str) -> None:
-    """Validates the Content-Type of the response asynchronously."""
-    content_type = response.headers.get('Content-Type', '')
-    if expected_content_type not in content_type:
-        raise ValueError(f"Unexpected Content-Type: {content_type}, expected {expected_content_type}.")
-
-def format_data_for_request(data: Dict[str, Any]) -> Dict[str, Any]:
-    """Formats data to be sent in an API request."""
-    return {k: v for k, v in data.items() if v is not None}
-
-def validate_list_of_dicts(items: List[Dict[str, Any]], required_keys: List[str]) -> bool:
-    """Validates that each dictionary in a list contains all required keys."""
-    return all(all(key in item for key in required_keys) for item in items)
-
-def datetime_to_iso(dt: datetime) -> str:
-    """Converts a datetime object to an ISO formatted string."""
-    return dt.isoformat()
-
-def sanitize_input(input_string: str) -> str:
-    """Sanitizes input strings to remove potentially harmful characters or patterns."""
-    # Implement specific sanitization rules as needed
-    return input_string.strip()
-
-async def fetch_all_pages(fetch_page_function, **params) -> List[Dict[str, Any]]:
-    """Utility function to fetch all pages of a paginated API response asynchronously."""
-    all_items = []
-    page_token = None
-
-    while True:
-        try:
-            response, next_page_token = await fetch_page_function(page_token=page_token, **params)
-        except OpenAIRequestError as e:
-            logger.warning(f"Encountered an error: {e}. Retrying...")
-            await asyncio.sleep(1)  # Simple backoff, adjust as needed
-            continue  # Retry the current page fetch
-
-        all_items.extend(response)
-        if not next_page_token:
-            break
-        page_token = next_page_token
-
-    return all_items
+class Utils:
+    def __init__(self, logger: Optional[logging.Logger] = None):
+        """Initializes utilities with a logger."""
+        self.logger = logger or logging.getLogger(__name__)
+        self._setup_logging()
+
+    def _setup_logging(self):
+        if not self.logger.handlers:
+            handler = logging.StreamHandler()
+            formatter = logging.Formatter('%(asctime)s - %(name)s - %(levellevelname)s - %(message)s')
+            handler.setFormatter(formatter)
+            self.logger.addHandler(handler)
+        self.logger.setLevel(logging.INFO)
+
+    async def handle_http_error(self, response: aiohttp.ClientResponse) -> None:
+        """Asynchronously handles HTTP errors by raising an OpenAIRequestError with detailed message."""
+        if response.status >= 400:
+            error_message, error_type, request_id = 'No error message provided.', 'APIError', 'N/A'
+            try:
+                json_response = await response.json()
+                error_message = json_response.get('error', {}).get('message', error_message)
+                error_type = json_response.get('error', {}).get('type', error_type)
+                request_id = response.headers.get('X-Request-ID', request_id)
+            except Exception as json_error:
+                self.logger.error("Failed to parse JSON response", exc_info=json_error)
+                error_message = str(json_error)
+
+            msg = f"{error_type}: {error_message} (Request ID: {request_id})"
+            self.logger.error(msg)
+            raise OpenAIRequestError(message=msg, status_code=response.status, error_type=error_type, request_id=request_id)
+
+    def log_api_call(self, method: str, url: str, status_code: Optional[int] = None, duration: Optional[float] = None, data: Optional[Dict[str, Any]] = None) -> None:
+        """Logs details of an API call including method, URL, status, duration, and data in a structured format."""
+        log_data = {
+            "event": "APIRequest",
+            "method": method,
+            "url": url,
+            "status_code": status_code,
+            "duration": f"{duration:.2f}s" if duration else None,
+            "request_data": json.dumps(data) if data else "{}"
+        }
+        self.logger.info("API call detail:", extra=log_data)
+
+    def validate_response_content_type(self, response: aiohttp.ClientResponse, expected_content_type: str) -> None:
+        """Validates the Content-Type of the response asynchronously."""
+        if expected_content_type not in response.headers.get('Content-Type', ''):
+            raise ValueError(f"Unexpected Content-Type. Expected {expected_content_type}.")
+
+    def format_data_for_request(self, data: Dict[str, Any]) -> Dict[str, Any]:
+        """Filters out None values from a dictionary for API request submission."""
+        return {k: v for k, v in data.items() if v is not None}
+
+    def validate_list_of_dicts(self, items: List[Dict[str, Any]], required_keys: List[str]) -> bool:
+        """Validates that each item in the list is a dict containing all required keys."""
+        return all(all(key in item for key in required_keys) for item in items)
+
+    def datetime_to_iso(self, dt: datetime) -> str:
+        """Converts a datetime object to an ISO formatted string."""
+        return dt.replace(microsecond=0).isoformat()
+
+    def sanitize_input(self, input_string: str) -> str:
+        """Sanitizes input strings by stripping leading and trailing whitespace."""
+        return input_string.strip()
+
+    async def fetch_all_pages(self, make_api_call, endpoint: str, **params) -> List[Dict[str, Any]]:
+        """Fetches all pages from a paginated API endpoint asynchronously using the provided API call function."""
+        all_items, page_token = [], None
+        while True:
+            response, next_page_token = await make_api_call(endpoint, params={**params, 'page_token': page_token})
+            all_items.extend(response)
+            if not next_page_token: break
+            page_token = next_page_token
+        return all_items
+
+    async def set_vector_store_expiration(self, make_api_call, vector_store_id: str, expires_after: Dict[str, Any]) -> Dict[str, Any]:
+        """Sets the expiration policy for a vector store."""
+        data = {"expires_after": expires_after}
+        return await make_api_call(f"beta/vector_stores/{vector_store_id}/update", method="POST", data=data)
```

### Comparing `botwrap-0.1.4/setup.py` & `botwrap-0.1.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='botwrap',
-    version='0.1.4',
+    version='0.1.7',
     author='BizPrincess',
     author_email='professionallyjami@gmail.com',
     description='A convenient wrapper for the OpenAI API.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/BizPrincess/botwrap',
     packages=find_packages(),
@@ -16,19 +16,25 @@
         'beautifulsoup4==4.12.3',
         'certifi==2023.11.17',
         'charset-normalizer==3.3.2',
         'click==8.1.7',
         'Flask==3.0.1',
         'httpx==0.26.0',
         'Jinja2==3.1.3',
-        'openai==1.10.0',
+        'openai==1.29.0',
         'psycopg2-binary==2.9.9',
         'requests==2.31.0',
-        'urllib3==2.1.0'
+        'urllib3==2.1.0',
+        'python-dotenv==1.0.0',
     ],
+    entry_points={
+        'console_scripts': [
+            'minimal_test_convo=minimal_test_convo:main',
+        ],
+    },
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
@@ -36,8 +42,7 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
 )
-
```

### Comparing `botwrap-0.1.4/tests/test_api_client.py` & `botwrap-0.1.7/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `botwrap-0.1.4/tests/test_assistants.py` & `botwrap-0.1.7/tests/test_assistants.py`

 * *Files identical despite different names*

### Comparing `botwrap-0.1.4/tests/test_exceptions.py` & `botwrap-0.1.7/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `botwrap-0.1.4/tests/test_files.py` & `botwrap-0.1.7/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `botwrap-0.1.4/tests/test_messages.py` & `botwrap-0.1.7/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `botwrap-0.1.4/tests/test_openai_wrapper.py` & `botwrap-0.1.7/tests/test_openai_wrapper.py`

 * *Files identical despite different names*

### Comparing `botwrap-0.1.4/tests/test_runs.py` & `botwrap-0.1.7/tests/test_runs.py`

 * *Files identical despite different names*

### Comparing `botwrap-0.1.4/tests/test_threads.py` & `botwrap-0.1.7/tests/test_threads.py`

 * *Files identical despite different names*

### Comparing `botwrap-0.1.4/tests/test_tools.py` & `botwrap-0.1.7/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `botwrap-0.1.4/tests/test_utils.py` & `botwrap-0.1.7/tests/test_utils.py`

 * *Files identical despite different names*

