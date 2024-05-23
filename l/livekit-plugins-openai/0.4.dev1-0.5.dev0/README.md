# Comparing `tmp/livekit_plugins_openai-0.4.dev1.tar.gz` & `tmp/livekit_plugins_openai-0.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit_plugins_openai-0.4.dev1.tar", last modified: Wed May  1 00:54:27 2024, max compression
+gzip compressed data, was "livekit_plugins_openai-0.5.dev0.tar", last modified: Thu May 23 15:59:32 2024, max compression
```

## Comparing `livekit_plugins_openai-0.4.dev1.tar` & `livekit_plugins_openai-0.5.dev0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:27.597602 livekit_plugins_openai-0.4.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-01 00:54:27.597602 livekit_plugins_openai-0.4.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-01 00:54:20.000000 livekit_plugins_openai-0.4.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:27.593602 livekit_plugins_openai-0.4.dev1/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:27.593602 livekit_plugins_openai-0.4.dev1/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:27.597602 livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-01 00:54:20.000000 livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8199 2024-05-01 00:54:20.000000 livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 00:54:20.000000 livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-01 00:54:20.000000 livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:20.000000 livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-01 00:54:20.000000 livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/stt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-01 00:54:20.000000 livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-01 00:54:20.000000 livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:27.597602 livekit_plugins_openai-0.4.dev1/livekit_plugins_openai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-01 00:54:27.000000 livekit_plugins_openai-0.4.dev1/livekit_plugins_openai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-01 00:54:27.000000 livekit_plugins_openai-0.4.dev1/livekit_plugins_openai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:54:27.000000 livekit_plugins_openai-0.4.dev1/livekit_plugins_openai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-01 00:54:27.000000 livekit_plugins_openai-0.4.dev1/livekit_plugins_openai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 00:54:27.000000 livekit_plugins_openai-0.4.dev1/livekit_plugins_openai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 00:54:20.000000 livekit_plugins_openai-0.4.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:54:27.597602 livekit_plugins_openai-0.4.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-01 00:54:20.000000 livekit_plugins_openai-0.4.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:32.203672 livekit_plugins_openai-0.5.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-23 15:59:32.203672 livekit_plugins_openai-0.5.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-23 15:59:24.000000 livekit_plugins_openai-0.5.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:32.203672 livekit_plugins_openai-0.5.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:32.203672 livekit_plugins_openai-0.5.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:32.203672 livekit_plugins_openai-0.5.dev0/livekit/plugins/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-23 15:59:24.000000 livekit_plugins_openai-0.5.dev0/livekit/plugins/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-05-23 15:59:24.000000 livekit_plugins_openai-0.5.dev0/livekit/plugins/openai/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-23 15:59:24.000000 livekit_plugins_openai-0.5.dev0/livekit/plugins/openai/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-23 15:59:24.000000 livekit_plugins_openai-0.5.dev0/livekit/plugins/openai/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:24.000000 livekit_plugins_openai-0.5.dev0/livekit/plugins/openai/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-23 15:59:24.000000 livekit_plugins_openai-0.5.dev0/livekit/plugins/openai/stt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-23 15:59:24.000000 livekit_plugins_openai-0.5.dev0/livekit/plugins/openai/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-23 15:59:24.000000 livekit_plugins_openai-0.5.dev0/livekit/plugins/openai/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:32.203672 livekit_plugins_openai-0.5.dev0/livekit_plugins_openai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-23 15:59:32.000000 livekit_plugins_openai-0.5.dev0/livekit_plugins_openai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-23 15:59:32.000000 livekit_plugins_openai-0.5.dev0/livekit_plugins_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:59:32.000000 livekit_plugins_openai-0.5.dev0/livekit_plugins_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-23 15:59:32.000000 livekit_plugins_openai-0.5.dev0/livekit_plugins_openai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 15:59:32.000000 livekit_plugins_openai-0.5.dev0/livekit_plugins_openai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 15:59:24.000000 livekit_plugins_openai-0.5.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:59:32.203672 livekit_plugins_openai-0.5.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-23 15:59:24.000000 livekit_plugins_openai-0.5.dev0/setup.py
```

### Comparing `livekit_plugins_openai-0.4.dev1/PKG-INFO` & `livekit_plugins_openai-0.5.dev0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-openai
-Version: 0.4.dev1
+Version: 0.5.dev0
 Summary: Agent Framework plugin for services from OpenAI
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Requires-Dist: livekit~=0.11
-Requires-Dist: livekit-agents~=0.6.dev1
+Requires-Dist: livekit-agents~=0.7.dev0
 Requires-Dist: openai>=1.0.0
 Requires-Dist: requests<3,>=2
 
 # LiveKit Plugins OpenAI
 
 Agent Framework plugin for services from OpenAI. Currently supports STT, TTS, and Dalle 3.
```

### Comparing `livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/__init__.py` & `livekit_plugins_openai-0.5.dev0/livekit/plugins/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/llm.py` & `livekit_plugins_openai-0.5.dev0/livekit/plugins/openai/llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import asyncio
 import enum
 import functools
 import inspect
 import json
 from typing import Any, Dict, MutableSet
 
@@ -19,15 +21,15 @@
     model: str | ChatModels
 
 
 class LLM(llm.LLM):
     def __init__(
         self,
         *,
-        model: str | ChatModels = "gpt-4-turbo",
+        model: str | ChatModels = "gpt-4o",
         client: openai.AsyncClient | None = None,
     ) -> None:
         self._opts = LLMOptions(model=model)
         self._client = client or openai.AsyncClient()
         self._running_fncs: MutableSet[asyncio.Task] = set()
 
     async def chat(
@@ -146,17 +148,21 @@
                 # TODO(theomonnom): Try to recover from invalid json
                 logger.exception(f"failed to decode arguments for tool call {name}")
                 return
 
         fnc = fncs[name]
         # validate args before calling fnc
         for arg in fnc.args.values():
-            if arg.default is inspect.Parameter.empty and arg.name not in args:
-                logger.error(f"missing required arg {arg.name} for ai_callable {name}")
-                return
+            if arg.name not in args:
+                if arg.default is inspect.Parameter.empty:
+                    logger.error(
+                        f"missing required arg {arg.name} for ai_callable {name}"
+                    )
+                    return
+                continue
 
             if arg.type is bool and args[arg.name] not in (True, False):
                 logger.error(f"invalid arg {arg.name} for ai_callable {name}")
                 return
 
             if arg.type is int and not isinstance(args[arg.name], int):
                 logger.error(f"invalid arg {arg.name} for ai_callable {name}")
@@ -166,17 +172,19 @@
                 logger.error(f"invalid arg {arg.name} for ai_callable {name}")
                 return
 
             if arg.type is str and not isinstance(args[arg.name], str):
                 logger.error(f"invalid arg {arg.name} for ai_callable {name}")
                 return
 
-            if issubclass(arg.type, enum.Enum) and args[arg.name] not in arg.type:
-                logger.error(f"invalid arg {arg.name} for ai_callable {name}")
-                return
+            if issubclass(arg.type, enum.Enum):
+                values = set(item.value for item in arg.type)
+                if args[arg.name] not in values:
+                    logger.error(f"invalid arg {arg.name} for ai_callable {name}")
+                    return
 
         logger.debug(f"calling function {name} with arguments {args}")
         self._called_functions.append(
             llm.CalledFunction(fnc_name=name, fnc=fnc.fnc, args=args)
         )
         func = functools.partial(fnc.fnc, **args)
         if asyncio.iscoroutinefunction(fnc.fnc):
```

### Comparing `livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/models.py` & `livekit_plugins_openai-0.5.dev0/livekit/plugins/openai/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Literal
 
 WhisperModels = Literal["whisper-1"]
 TTSModels = Literal["tts-1", "tts-1-hd"]
 TTSVoices = Literal["alloy", "echo", "fable", "onyx", "nova", "shimmer"]
 DalleModels = Literal["dall-e-2", "dall-e-3"]
 ChatModels = Literal[
+    "gpt-4o",
+    "gpt-4o-2024-05-13",
     "gpt-4-turbo",
     "gpt-4-turbo-2024-04-09",
     "gpt-4-turbo-preview",
     "gpt-4-0125-preview" "gpt-4-1106-preview",
     "gpt-4-vision-preview",
     "gpt-4-1106-vision-preview",
     "gpt-4",
```

### Comparing `livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/stt.py` & `livekit_plugins_openai-0.5.dev0/livekit/plugins/openai/stt.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,61 +16,70 @@
 
 import dataclasses
 import io
 import os
 import wave
 from dataclasses import dataclass
 
+import aiohttp
 from livekit import agents
-from livekit.agents import stt
+from livekit.agents import stt, utils
 from livekit.agents.utils import AudioBuffer
 
-import openai
-
 from .models import WhisperModels
 
+OPENAI_ENPOINT = "https://api.openai.com/v1/audio/transcriptions"
+
 
 @dataclass
-class STTOptions:
+class _STTOptions:
     language: str
     detect_language: bool
     model: WhisperModels
+    api_key: str
 
 
 class STT(stt.STT):
     def __init__(
         self,
         *,
         language: str = "en",
         detect_language: bool = False,
         model: WhisperModels = "whisper-1",
         api_key: str | None = None,
+        http_session: aiohttp.ClientSession | None = None,
     ):
         super().__init__(streaming_supported=False)
         api_key = api_key or os.environ.get("OPENAI_API_KEY")
         if not api_key:
             raise ValueError("OPENAI_API_KEY must be set")
 
-        self._client = openai.AsyncOpenAI(api_key=api_key)
-
         if detect_language:
             language = ""
 
-        self._config = STTOptions(
+        self._opts = _STTOptions(
             language=language,
             detect_language=detect_language,
             model=model,
+            api_key=api_key,
         )
+        self._session = http_session
+
+    def _ensure_session(self) -> aiohttp.ClientSession:
+        if not self._session:
+            self._session = utils.http_session()
+
+        return self._session
 
     def _sanitize_options(
         self,
         *,
         language: str | None = None,
-    ) -> STTOptions:
-        config = dataclasses.replace(self._config)
+    ) -> _STTOptions:
+        config = dataclasses.replace(self._opts)
         config.language = language or config.language
         return config
 
     async def recognize(
         self,
         *,
         buffer: AudioBuffer,
@@ -82,21 +91,33 @@
         io_buffer = io.BytesIO()
         with wave.open(io_buffer, "wb") as wav:
             wav.setnchannels(buffer.num_channels)
             wav.setsampwidth(2)  # 16-bit
             wav.setframerate(buffer.sample_rate)
             wav.writeframes(buffer.data)
 
-        resp = await self._client.audio.transcriptions.create(
-            file=("a.wav", io_buffer),
-            model=config.model,
-            language=config.language,
-            response_format="json",
-        )
-        return transcription_to_speech_event(resp, config.language)
+        form = aiohttp.FormData()
+        form.add_field("file", io_buffer.getvalue(), filename="my_file.wav")
+        form.add_field("model", config.model)
+
+        if config.language:
+            form.add_field("language", config.language)
+
+        form.add_field("response_format", "json")
+
+        async with self._ensure_session().post(
+            OPENAI_ENPOINT,
+            headers={"Authorization": f"Bearer {config.api_key}"},
+            data=form,
+        ) as resp:
+            data = await resp.json()
+            if "text" not in data or "error" in data:
+                raise ValueError(f"Unexpected response: {data}")
+
+            return _transcription_to_speech_event(data, config.language)
 
 
-def transcription_to_speech_event(transcription, language) -> stt.SpeechEvent:
+def _transcription_to_speech_event(transcription: dict, language) -> stt.SpeechEvent:
     return stt.SpeechEvent(
         type=stt.SpeechEventType.FINAL_TRANSCRIPT,
-        alternatives=[stt.SpeechData(text=transcription.text, language=language)],
+        alternatives=[stt.SpeechData(text=transcription["text"], language=language)],
     )
```

### Comparing `livekit_plugins_openai-0.4.dev1/livekit/plugins/openai/version.py` & `livekit_plugins_openai-0.5.dev0/livekit/plugins/openai/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.4.dev1"
+__version__ = "0.5.dev0"
```

### Comparing `livekit_plugins_openai-0.4.dev1/livekit_plugins_openai.egg-info/PKG-INFO` & `livekit_plugins_openai-0.5.dev0/livekit_plugins_openai.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-openai
-Version: 0.4.dev1
+Version: 0.5.dev0
 Summary: Agent Framework plugin for services from OpenAI
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Requires-Dist: livekit~=0.11
-Requires-Dist: livekit-agents~=0.6.dev1
+Requires-Dist: livekit-agents~=0.7.dev0
 Requires-Dist: openai>=1.0.0
 Requires-Dist: requests<3,>=2
 
 # LiveKit Plugins OpenAI
 
 Agent Framework plugin for services from OpenAI. Currently supports STT, TTS, and Dalle 3.
```

### Comparing `livekit_plugins_openai-0.4.dev1/livekit_plugins_openai.egg-info/SOURCES.txt` & `livekit_plugins_openai-0.5.dev0/livekit_plugins_openai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `livekit_plugins_openai-0.4.dev1/setup.py` & `livekit_plugins_openai-0.5.dev0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     ],
     keywords=["webrtc", "realtime", "audio", "video", "livekit"],
     license="Apache-2.0",
     packages=setuptools.find_namespace_packages(include=["livekit.*"]),
     python_requires=">=3.9.0",
     install_requires=[
         "livekit ~= 0.11",
-        "livekit-agents~=0.6.dev1",
+        "livekit-agents~=0.7.dev0",
         "openai >= 1.0.0",
         "requests >= 2, < 3",
     ],
     package_data={
         "livekit.plugins.openai": ["py.typed"],
     },
     project_urls={
```

