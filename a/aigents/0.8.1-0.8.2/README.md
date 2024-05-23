# Comparing `tmp/aigents-0.8.1.tar.gz` & `tmp/aigents-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aigents-0.8.1.tar", max compression
+gzip compressed data, was "aigents-0.8.2.tar", max compression
```

## Comparing `aigents-0.8.1.tar` & `aigents-0.8.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35149 2024-02-29 18:27:57.056767 aigents-0.8.1/LICENSE
--rw-r--r--   0        0        0     7402 2024-05-06 13:16:01.219386 aigents-0.8.1/README.md
--rw-r--r--   0        0        0     1044 2024-05-22 15:55:18.290255 aigents-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      843 2024-05-06 12:53:46.596803 aigents-0.8.1/src/aigents/__init__.py
--rw-r--r--   0        0        0    19580 2024-05-17 17:53:53.908658 aigents-0.8.1/src/aigents/base.py
--rw-r--r--   0        0        0     1238 2024-05-17 18:41:32.446222 aigents-0.8.1/src/aigents/constants.py
--rw-r--r--   0        0        0      376 2024-05-05 20:28:48.665557 aigents-0.8.1/src/aigents/context/__init__.py
--rw-r--r--   0        0        0     2023 2024-05-06 17:26:15.624797 aigents-0.8.1/src/aigents/context/base.py
--rw-r--r--   0        0        0    13227 2024-05-15 19:26:29.333058 aigents-0.8.1/src/aigents/context/core.py
--rw-r--r--   0        0        0      337 2024-05-03 19:26:39.754455 aigents-0.8.1/src/aigents/context/errors.py
--rw-r--r--   0        0        0        0 2024-05-03 19:26:39.754455 aigents-0.8.1/src/aigents/context/nlp/__init__.py
--rw-r--r--   0        0        0     1098 2024-05-06 12:34:29.130871 aigents-0.8.1/src/aigents/context/nlp/base.py
--rw-r--r--   0        0        0      105 2024-05-03 19:26:39.754455 aigents-0.8.1/src/aigents/context/nlp/constants.py
--rw-r--r--   0        0        0      149 2024-05-03 19:26:39.754455 aigents-0.8.1/src/aigents/context/nlp/errors.py
--rw-r--r--   0        0        0    17637 2024-05-10 12:40:21.261161 aigents-0.8.1/src/aigents/context/nlp/processors.py
--rw-r--r--   0        0        0     3101 2024-05-09 19:39:39.988951 aigents-0.8.1/src/aigents/context/nlp/utils.py
--rw-r--r--   0        0        0     4020 2024-05-10 17:24:48.875825 aigents-0.8.1/src/aigents/context/utils.py
--rw-r--r--   0        0        0    32020 2024-05-22 15:54:28.277864 aigents-0.8.1/src/aigents/core.py
--rw-r--r--   0        0        0      188 2024-02-23 18:20:01.705095 aigents-0.8.1/src/aigents/data.py
--rw-r--r--   0        0        0      640 2024-02-29 13:47:18.770982 aigents-0.8.1/src/aigents/errors.py
--rw-r--r--   0        0        0    28395 2024-03-08 19:28:00.158179 aigents-0.8.1/src/aigents/prompts.py
--rw-r--r--   0        0        0     2822 2024-05-05 20:28:48.665557 aigents-0.8.1/src/aigents/settings.py
--rw-r--r--   0        0        0     6814 2024-05-03 19:26:39.754455 aigents-0.8.1/src/aigents/utils.py
--rw-r--r--   0        0        0     8712 1970-01-01 00:00:00.000000 aigents-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-29 18:27:57.056767 aigents-0.8.2/LICENSE
+-rw-r--r--   0        0        0     7402 2024-05-06 13:16:01.219386 aigents-0.8.2/README.md
+-rw-r--r--   0        0        0     1044 2024-05-23 12:00:23.462117 aigents-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0      843 2024-05-06 12:53:46.596803 aigents-0.8.2/src/aigents/__init__.py
+-rw-r--r--   0        0        0    19580 2024-05-17 17:53:53.908658 aigents-0.8.2/src/aigents/base.py
+-rw-r--r--   0        0        0     1238 2024-05-17 18:41:32.446222 aigents-0.8.2/src/aigents/constants.py
+-rw-r--r--   0        0        0      376 2024-05-05 20:28:48.665557 aigents-0.8.2/src/aigents/context/__init__.py
+-rw-r--r--   0        0        0     2023 2024-05-06 17:26:15.624797 aigents-0.8.2/src/aigents/context/base.py
+-rw-r--r--   0        0        0    13227 2024-05-15 19:26:29.333058 aigents-0.8.2/src/aigents/context/core.py
+-rw-r--r--   0        0        0      337 2024-05-03 19:26:39.754455 aigents-0.8.2/src/aigents/context/errors.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:26:39.754455 aigents-0.8.2/src/aigents/context/nlp/__init__.py
+-rw-r--r--   0        0        0     1098 2024-05-06 12:34:29.130871 aigents-0.8.2/src/aigents/context/nlp/base.py
+-rw-r--r--   0        0        0      105 2024-05-03 19:26:39.754455 aigents-0.8.2/src/aigents/context/nlp/constants.py
+-rw-r--r--   0        0        0      149 2024-05-03 19:26:39.754455 aigents-0.8.2/src/aigents/context/nlp/errors.py
+-rw-r--r--   0        0        0    17637 2024-05-10 12:40:21.261161 aigents-0.8.2/src/aigents/context/nlp/processors.py
+-rw-r--r--   0        0        0     3101 2024-05-09 19:39:39.988951 aigents-0.8.2/src/aigents/context/nlp/utils.py
+-rw-r--r--   0        0        0     4020 2024-05-10 17:24:48.875825 aigents-0.8.2/src/aigents/context/utils.py
+-rw-r--r--   0        0        0    33100 2024-05-23 12:00:23.462117 aigents-0.8.2/src/aigents/core.py
+-rw-r--r--   0        0        0      188 2024-02-23 18:20:01.705095 aigents-0.8.2/src/aigents/data.py
+-rw-r--r--   0        0        0      640 2024-02-29 13:47:18.770982 aigents-0.8.2/src/aigents/errors.py
+-rw-r--r--   0        0        0    28395 2024-03-08 19:28:00.158179 aigents-0.8.2/src/aigents/prompts.py
+-rw-r--r--   0        0        0     2822 2024-05-05 20:28:48.665557 aigents-0.8.2/src/aigents/settings.py
+-rw-r--r--   0        0        0     6814 2024-05-03 19:26:39.754455 aigents-0.8.2/src/aigents/utils.py
+-rw-r--r--   0        0        0     8712 1970-01-01 00:00:00.000000 aigents-0.8.2/PKG-INFO
```

### Comparing `aigents-0.8.1/LICENSE` & `aigents-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aigents-0.8.1/README.md` & `aigents-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `aigents-0.8.1/pyproject.toml` & `aigents-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aigents"
-version = "0.8.1"
+version = "0.8.2"
 description = "Adapters for Large Language Models and Generative Pre-trained Transformers APIs"
 authors = ["Vagner Bessa <bessavagner@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [{include = "aigents", from = "src"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `aigents-0.8.1/src/aigents/__init__.py` & `aigents-0.8.2/src/aigents/__init__.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.1/src/aigents/base.py` & `aigents-0.8.2/src/aigents/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.1/src/aigents/constants.py` & `aigents-0.8.2/src/aigents/constants.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.1/src/aigents/context/base.py` & `aigents-0.8.2/src/aigents/context/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.1/src/aigents/context/core.py` & `aigents-0.8.2/src/aigents/context/core.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.1/src/aigents/context/nlp/base.py` & `aigents-0.8.2/src/aigents/context/nlp/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.1/src/aigents/context/nlp/processors.py` & `aigents-0.8.2/src/aigents/context/nlp/processors.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.1/src/aigents/context/nlp/utils.py` & `aigents-0.8.2/src/aigents/context/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.1/src/aigents/context/utils.py` & `aigents-0.8.2/src/aigents/context/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.1/src/aigents/core.py` & `aigents-0.8.2/src/aigents/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-import os
+import time
 import logging
 import asyncio
 from pathlib import Path
 from typing import Union
 
 from dotenv import load_dotenv
 from PIL import Image
 
 import google.generativeai as genai
+from google.api_core.exceptions import ResourceExhausted
 from g4f.Provider.Bing import Tones
 
 from .base import BaseChatter
 from .base import OpenAIChatterMixin
 from .base import GoogleChatterMixin
 from .base import BingChatterMixin
 
@@ -301,14 +302,15 @@
                          **kwargs)
 
     def answer(self,
                prompt,
                use_agent=True,
                conversation=True,
                agent=None,
+               retry=2,
                **kwargs):
         if use_agent and agent is None:
             setup = (
                 "You are a very skilled writer that can summarize any text "
                 "while preserving the whole meaning of its content."
             )
             agent = GoogleChatter(setup=setup, api_key=self.api_key)
@@ -322,17 +324,29 @@
                 *self.messages[:2], self.messages[-1]
             ]
         else:
             messages = self.messages if conversation else self.messages[-2:]
 
         config = genai.types.GenerationConfig(temperature=self.temperature)
 
-        response = self.client.generate_content(
-            messages, generation_config=config,**kwargs
-        )
+        try:
+            response = self.client.generate_content(
+                messages, generation_config=config, **kwargs
+            )
+        except ResourceExhausted as err:
+            while retry:
+                logger.warning("%s. Sleeping for 5s", str(err))
+                time.sleep(5)
+                try:
+                    response = self.client.generate_content(
+                        messages, generation_config=config, **kwargs
+                    )
+                except ResourceExhausted:
+                    retry -= 1
+            raise AgentError from err
         self.last_response = response
         try:
             self._update(
                 ROLES[-1],
                 response.text,
                 use_agent=use_agent,
                 agent=agent
@@ -402,14 +416,15 @@
 
     async def answer(self,
                      prompt,
                      use_agent: bool = True,
                      conversation: bool = True,
                      agent: str = None,
                      generation_config_dict: dict = None,
+                     retry: int = 2,
                      **kwargs):
         if use_agent and agent is None:
             setup = (
                 "You are a very skilled writer that can summarize any text "
                 "while preserving the whole meaning of its content."
             )
             agent = GoogleChatter(setup=setup, api_key=self.api_key)
@@ -424,17 +439,29 @@
             ]
         else:
             messages = self.messages if conversation else self.messages[-2:]
         if generation_config_dict is None:
             generation_config_dict = {}
         generation_config_dict['temperature'] = self.temperature
         config = genai.types.GenerationConfig(**generation_config_dict)
-        response = await self.client.generate_content_async(
-            messages, generation_config=config, **kwargs
-        )
+        try:
+            response = await self.client.generate_content_async(
+                messages, generation_config=config, **kwargs
+            )
+        except ResourceExhausted as err:
+            while retry:
+                logger.warning("%s. Sleeping for 5s", str(err))
+                await asyncio.sleep(5)
+                try:
+                    response = await self.client.generate_content_async(
+                        messages, generation_config=config, **kwargs
+                    )
+                except ResourceExhausted:
+                    retry -= 1
+            raise AgentError from err
         self.last_response = response
         try:
             self._update(
                 ROLES[-1], response.text, use_agent=use_agent, agent=agent
             )
             return response.text
         except ValueError as err:
```

### Comparing `aigents-0.8.1/src/aigents/errors.py` & `aigents-0.8.2/src/aigents/errors.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.1/src/aigents/prompts.py` & `aigents-0.8.2/src/aigents/prompts.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.1/src/aigents/settings.py` & `aigents-0.8.2/src/aigents/settings.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.1/src/aigents/utils.py` & `aigents-0.8.2/src/aigents/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.1/PKG-INFO` & `aigents-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aigents
-Version: 0.8.1
+Version: 0.8.2
 Summary: Adapters for Large Language Models and Generative Pre-trained Transformers APIs
 Home-page: https://github.com/bessavagner/aigents.git
 License: GPL-3.0-only
 Author: Vagner Bessa
 Author-email: bessavagner@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

