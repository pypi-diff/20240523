# Comparing `tmp/modelsmith-0.3.0.tar.gz` & `tmp/modelsmith-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelsmith-0.3.0.tar", max compression
+gzip compressed data, was "modelsmith-0.4.0.tar", max compression
```

## Comparing `modelsmith-0.3.0.tar` & `modelsmith-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2024-03-22 19:22:37.844254 modelsmith-0.3.0/LICENSE
--rw-r--r--   0        0        0    11004 2024-03-23 10:40:18.119175 modelsmith-0.3.0/README.md
--rw-r--r--   0        0        0     1443 2024-04-08 08:36:55.409388 modelsmith-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      284 2024-04-08 08:36:55.409552 modelsmith-0.3.0/src/modelsmith/__init__.py
--rw-r--r--   0        0        0      256 2024-03-22 19:25:46.899419 modelsmith-0.3.0/src/modelsmith/enums.py
--rw-r--r--   0        0        0      639 2024-04-08 08:36:55.409707 modelsmith-0.3.0/src/modelsmith/exceptions.py
--rw-r--r--   0        0        0     6626 2024-03-25 09:47:21.501335 modelsmith-0.3.0/src/modelsmith/forge.py
--rw-r--r--   0        0        0     1860 2024-03-22 19:25:46.910176 modelsmith-0.3.0/src/modelsmith/language_model.py
--rw-r--r--   0        0        0     4682 2024-04-08 08:17:41.923420 modelsmith-0.3.0/src/modelsmith/prompt.py
--rw-r--r--   0        0        0     2556 2024-03-22 19:26:31.311149 modelsmith-0.3.0/src/modelsmith/response_model.py
--rw-r--r--   0        0        0      782 2024-03-22 19:25:46.915975 modelsmith-0.3.0/src/modelsmith/utilities.py
--rw-r--r--   0        0        0    11970 1970-01-01 00:00:00.000000 modelsmith-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-03-22 19:22:37.844254 modelsmith-0.4.0/LICENSE
+-rw-r--r--   0        0        0    11004 2024-03-23 10:40:18.119175 modelsmith-0.4.0/README.md
+-rw-r--r--   0        0        0     1443 2024-05-23 17:19:54.555899 modelsmith-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      284 2024-04-08 08:36:55.409552 modelsmith-0.4.0/src/modelsmith/__init__.py
+-rw-r--r--   0        0        0      256 2024-03-22 19:25:46.899419 modelsmith-0.4.0/src/modelsmith/enums.py
+-rw-r--r--   0        0        0      639 2024-04-08 08:36:55.409707 modelsmith-0.4.0/src/modelsmith/exceptions.py
+-rw-r--r--   0        0        0     6546 2024-05-23 17:18:19.216802 modelsmith-0.4.0/src/modelsmith/forge.py
+-rw-r--r--   0        0        0     1860 2024-03-22 19:25:46.910176 modelsmith-0.4.0/src/modelsmith/language_model.py
+-rw-r--r--   0        0        0     4924 2024-05-23 17:18:10.227450 modelsmith-0.4.0/src/modelsmith/prompt.py
+-rw-r--r--   0        0        0     2556 2024-03-22 19:26:31.311149 modelsmith-0.4.0/src/modelsmith/response_model.py
+-rw-r--r--   0        0        0      782 2024-03-22 19:25:46.915975 modelsmith-0.4.0/src/modelsmith/utilities.py
+-rw-r--r--   0        0        0    11970 1970-01-01 00:00:00.000000 modelsmith-0.4.0/PKG-INFO
```

### Comparing `modelsmith-0.3.0/LICENSE` & `modelsmith-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modelsmith-0.3.0/README.md` & `modelsmith-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `modelsmith-0.3.0/pyproject.toml` & `modelsmith-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelsmith"
-version = "0.3.0"
+version = "0.4.0"
 description = "Get Pydantic models and Python types as LLM responses from Google Vertex AI models."
 authors = ["Christo Olivier <mail@christoolivier.com>"]
 maintainers = ["Christo Olivier <mail@christoolivier.com>"]
 homepage = "https://github.com/christo-olivier/modelsmith"
 repository = "https://github.com/christo-olivier/modelsmith"
 keywords = ["vertexai", "pydantic", "models", "types", "llm"]
 license = "MIT"
```

### Comparing `modelsmith-0.3.0/src/modelsmith/exceptions.py` & `modelsmith-0.4.0/src/modelsmith/exceptions.py`

 * *Files identical despite different names*

### Comparing `modelsmith-0.3.0/src/modelsmith/forge.py` & `modelsmith-0.4.0/src/modelsmith/forge.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,14 @@
         )
 
         model_response = None
         try:
             for attempt in Retrying(stop=stop_after_attempt(self.max_retries)):
                 with attempt:
                     try:
-                        logger.debug(f"Prompt sent to LLM:\n{prepared_prompt}")
                         response = self.model.send(prepared_prompt, model_settings)
                         model_response = self._process_response(response)
                     except (CombinedException, PatternNotFound) as e:
                         prepared_prompt = (
                             prepared_prompt
                             + f"\nTry again and fix the errors that occurred: {e.args}"
                         )
```

### Comparing `modelsmith-0.3.0/src/modelsmith/language_model.py` & `modelsmith-0.4.0/src/modelsmith/language_model.py`

 * *Files identical despite different names*

### Comparing `modelsmith-0.3.0/src/modelsmith/prompt.py` & `modelsmith-0.4.0/src/modelsmith/prompt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import inspect
 import json
+import logging
 from typing import Any
 
 from jinja2 import BaseLoader, Environment, StrictUndefined, meta, select_autoescape
 from pydantic import BaseModel
 
+logger = logging.getLogger(__name__)
+
 RESPONSE_MODEL_TEXT = inspect.cleandoc("""
     Your output MUST be a JSON object that conforms to the JSON Schema below. All
     JSON object property names MUST be enclosed in double quotes.
 
     You MUST take the types of the OUTPUT SCHEMA into account and adjust your
     provided text to fit the required types.
 
@@ -108,15 +111,21 @@
             prompt_to_render += f"\n{RESPONSE_MODEL_TEXT}\n"
 
         # If the user_input is not specified in the prompt already then simply add it to
         # the end of the prompt.
         if "user_input" in prompt_kwargs and "user_input" not in self.prompt_variables:
             prompt_to_render += f"\n{prompt_kwargs['user_input']}\n"
 
-        return self._env.from_string(prompt_to_render).render(**prompt_kwargs)
+        # Render the prompt and log it for debugging purposes.
+        rendered_prompt = self._env.from_string(prompt_to_render).render(
+            **prompt_kwargs
+        )
+        logger.debug(f"Rendered prompt:\n{rendered_prompt}")
+
+        return rendered_prompt
 
     def _process_kwargs(self, prompt_values: dict[str, Any]) -> dict[str, Any]:
         """
         Process the prompt kwargs to handle cases around response_model.
 
         :param prompt_values: The keyword arguments to use to render the prompt.
         :return: Processed keyword arguments
```

### Comparing `modelsmith-0.3.0/src/modelsmith/response_model.py` & `modelsmith-0.4.0/src/modelsmith/response_model.py`

 * *Files identical despite different names*

### Comparing `modelsmith-0.3.0/src/modelsmith/utilities.py` & `modelsmith-0.4.0/src/modelsmith/utilities.py`

 * *Files identical despite different names*

### Comparing `modelsmith-0.3.0/PKG-INFO` & `modelsmith-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelsmith
-Version: 0.3.0
+Version: 0.4.0
 Summary: Get Pydantic models and Python types as LLM responses from Google Vertex AI models.
 Home-page: https://github.com/christo-olivier/modelsmith
 License: MIT
 Keywords: vertexai,pydantic,models,types,llm
 Author: Christo Olivier
 Author-email: mail@christoolivier.com
 Maintainer: Christo Olivier
```

