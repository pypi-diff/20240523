# Comparing `tmp/livekit_plugins_deepgram-0.4.dev1.tar.gz` & `tmp/livekit_plugins_deepgram-0.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit_plugins_deepgram-0.4.dev1.tar", last modified: Wed May  1 00:54:08 2024, max compression
+gzip compressed data, was "livekit_plugins_deepgram-0.5.dev0.tar", last modified: Thu May 23 15:59:09 2024, max compression
```

## Comparing `livekit_plugins_deepgram-0.4.dev1.tar` & `livekit_plugins_deepgram-0.5.dev0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:08.143184 livekit_plugins_deepgram-0.4.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-01 00:54:08.143184 livekit_plugins_deepgram-0.4.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-01 00:54:04.000000 livekit_plugins_deepgram-0.4.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:08.139184 livekit_plugins_deepgram-0.4.dev1/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:08.139184 livekit_plugins_deepgram-0.4.dev1/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:08.139184 livekit_plugins_deepgram-0.4.dev1/livekit/plugins/deepgram/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-01 00:54:04.000000 livekit_plugins_deepgram-0.4.dev1/livekit/plugins/deepgram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-01 00:54:04.000000 livekit_plugins_deepgram-0.4.dev1/livekit/plugins/deepgram/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-01 00:54:04.000000 livekit_plugins_deepgram-0.4.dev1/livekit/plugins/deepgram/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:04.000000 livekit_plugins_deepgram-0.4.dev1/livekit/plugins/deepgram/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16441 2024-05-01 00:54:04.000000 livekit_plugins_deepgram-0.4.dev1/livekit/plugins/deepgram/stt.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-01 00:54:04.000000 livekit_plugins_deepgram-0.4.dev1/livekit/plugins/deepgram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:08.139184 livekit_plugins_deepgram-0.4.dev1/livekit_plugins_deepgram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-01 00:54:08.000000 livekit_plugins_deepgram-0.4.dev1/livekit_plugins_deepgram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-01 00:54:08.000000 livekit_plugins_deepgram-0.4.dev1/livekit_plugins_deepgram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:54:08.000000 livekit_plugins_deepgram-0.4.dev1/livekit_plugins_deepgram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-01 00:54:08.000000 livekit_plugins_deepgram-0.4.dev1/livekit_plugins_deepgram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 00:54:08.000000 livekit_plugins_deepgram-0.4.dev1/livekit_plugins_deepgram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 00:54:04.000000 livekit_plugins_deepgram-0.4.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:54:08.143184 livekit_plugins_deepgram-0.4.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-01 00:54:04.000000 livekit_plugins_deepgram-0.4.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:09.533347 livekit_plugins_deepgram-0.5.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-23 15:59:09.533347 livekit_plugins_deepgram-0.5.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-23 15:59:05.000000 livekit_plugins_deepgram-0.5.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:09.529346 livekit_plugins_deepgram-0.5.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:09.529346 livekit_plugins_deepgram-0.5.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:09.533347 livekit_plugins_deepgram-0.5.dev0/livekit/plugins/deepgram/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-23 15:59:05.000000 livekit_plugins_deepgram-0.5.dev0/livekit/plugins/deepgram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-23 15:59:05.000000 livekit_plugins_deepgram-0.5.dev0/livekit/plugins/deepgram/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-23 15:59:05.000000 livekit_plugins_deepgram-0.5.dev0/livekit/plugins/deepgram/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:05.000000 livekit_plugins_deepgram-0.5.dev0/livekit/plugins/deepgram/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-05-23 15:59:05.000000 livekit_plugins_deepgram-0.5.dev0/livekit/plugins/deepgram/stt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-23 15:59:05.000000 livekit_plugins_deepgram-0.5.dev0/livekit/plugins/deepgram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:09.533347 livekit_plugins_deepgram-0.5.dev0/livekit_plugins_deepgram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-23 15:59:09.000000 livekit_plugins_deepgram-0.5.dev0/livekit_plugins_deepgram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-23 15:59:09.000000 livekit_plugins_deepgram-0.5.dev0/livekit_plugins_deepgram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:59:09.000000 livekit_plugins_deepgram-0.5.dev0/livekit_plugins_deepgram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-23 15:59:09.000000 livekit_plugins_deepgram-0.5.dev0/livekit_plugins_deepgram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 15:59:09.000000 livekit_plugins_deepgram-0.5.dev0/livekit_plugins_deepgram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 15:59:05.000000 livekit_plugins_deepgram-0.5.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:59:09.533347 livekit_plugins_deepgram-0.5.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-23 15:59:05.000000 livekit_plugins_deepgram-0.5.dev0/setup.py
```

### Comparing `livekit_plugins_deepgram-0.4.dev1/PKG-INFO` & `livekit_plugins_deepgram-0.5.dev0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-deepgram
-Version: 0.4.dev1
+Version: 0.5.dev0
 Summary: Agent Framework plugin for services using DeepGram's API.
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
 Requires-Dist: aiohttp>=3.7.4
 
 # LiveKit Plugins DeepGram
 
 Agent Framework plugin for speech-to-text with [DeepGram](https://deepgram.com/)'s API. Currently supports speech-to-text.
 
 ## Installation
```

### Comparing `livekit_plugins_deepgram-0.4.dev1/livekit/plugins/deepgram/models.py` & `livekit_plugins_deepgram-0.5.dev0/livekit/plugins/deepgram/models.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_deepgram-0.4.dev1/livekit/plugins/deepgram/stt.py` & `livekit_plugins_deepgram-0.5.dev0/livekit/plugins/deepgram/stt.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 import dataclasses
 import io
 import json
 import os
 import wave
 from contextlib import suppress
 from dataclasses import dataclass
-from typing import List
+from typing import List, Optional, Union
 from urllib.parse import urlencode
 
 import aiohttp
 from livekit import rtc
-from livekit.agents import stt
+from livekit.agents import stt, utils
 from livekit.agents.utils import AudioBuffer, merge_frames
 
 from .log import logger
 from .models import DeepgramLanguages, DeepgramModels
 
 
 @dataclass
@@ -53,14 +53,15 @@
         detect_language: bool = False,
         interim_results: bool = True,
         punctuate: bool = True,
         smart_format: bool = True,
         model: DeepgramModels = "nova-2-general",
         api_key: str | None = None,
         min_silence_duration: int = 0,
+        http_session: aiohttp.ClientSession | None = None,
     ) -> None:
         super().__init__(streaming_supported=True)
         api_key = api_key or os.environ.get("DEEPGRAM_API_KEY")
         if api_key is None:
             raise ValueError("Deepgram API key is required")
         self._api_key = api_key
 
@@ -69,14 +70,21 @@
             detect_language=detect_language,
             interim_results=interim_results,
             punctuate=punctuate,
             model=model,
             smart_format=smart_format,
             endpointing=min_silence_duration,
         )
+        self._session = http_session
+
+    def _ensure_session(self) -> aiohttp.ClientSession:
+        if not self._session:
+            self._session = utils.http_session()
+
+        return self._session
 
     async def recognize(
         self,
         *,
         buffer: AudioBuffer,
         language: DeepgramLanguages | str | None = None,
     ) -> stt.SpeechEvent:
@@ -109,27 +117,26 @@
 
         headers = {
             "Authorization": f"Token {self._api_key}",
             "Accept": "application/json",
             "Content-Type": "audio/wav",
         }
 
-        async with aiohttp.ClientSession(headers=headers) as session:
-            async with session.post(url, data=data) as res:
-                return prerecorded_transcription_to_speech_event(
-                    config.language, await res.json()
-                )
+        async with self._ensure_session().post(url, data=data, headers=headers) as res:
+            return prerecorded_transcription_to_speech_event(
+                config.language, await res.json()
+            )
 
     def stream(
         self,
         *,
         language: DeepgramLanguages | str | None = None,
     ) -> "SpeechStream":
         config = self._sanitize_options(language=language)
-        return SpeechStream(config, api_key=self._api_key)
+        return SpeechStream(config, self._api_key, self._ensure_session())
 
     def _sanitize_options(
         self,
         *,
         language: str | None = None,
     ) -> STTOptions:
         config = dataclasses.replace(self._opts)
@@ -145,32 +152,32 @@
     _KEEPALIVE_MSG: str = json.dumps({"type": "KeepAlive"})
     _CLOSE_MSG: str = json.dumps({"type": "CloseStream"})
 
     def __init__(
         self,
         opts: STTOptions,
         api_key: str,
-        sample_rate: int = 16000,
+        http_session: aiohttp.ClientSession,
+        sample_rate: int = 48000,
         num_channels: int = 1,
         max_retry: int = 32,
     ) -> None:
         super().__init__()
 
         if opts.detect_language and opts.language is None:
             raise ValueError("language detection is not supported in streaming mode")
 
         self._opts = opts
         self._sample_rate = sample_rate
         self._num_channels = num_channels
         self._api_key = api_key
         self._speaking = False
-
-        self._session = aiohttp.ClientSession()
-        self._queue = asyncio.Queue[rtc.AudioFrame | str]()
-        self._event_queue = asyncio.Queue[stt.SpeechEvent | None]()
+        self._session = http_session
+        self._queue = asyncio.Queue[Union[rtc.AudioFrame, str]]()
+        self._event_queue = asyncio.Queue[Optional[stt.SpeechEvent]]()
         self._closed = False
         self._main_task = asyncio.create_task(self._run(max_retry))
 
         # keep a list of final transcripts to combine them inside the END_OF_SPEECH event
         self._final_events: List[stt.SpeechEvent] = []
 
     def push_frame(self, frame: rtc.AudioFrame) -> None:
@@ -272,14 +279,15 @@
 
                 if isinstance(data, rtc.AudioFrame):
                     # TODO(theomonnom): The remix_and_resample method is low quality
                     # and should be replaced with a continuous resampling
                     frame = data.remix_and_resample(
                         self._sample_rate, self._num_channels
                     )
+
                     await ws.send_bytes(frame.data.tobytes())
                 elif data == SpeechStream._CLOSE_MSG:
                     closing_ws = True
                     await ws.send_str(data)  # tell deepgram we are done with inputs
                     break
 
         async def recv_task():
```

### Comparing `livekit_plugins_deepgram-0.4.dev1/livekit/plugins/deepgram/version.py` & `livekit_plugins_deepgram-0.5.dev0/livekit/plugins/deepgram/version.py`

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

### Comparing `livekit_plugins_deepgram-0.4.dev1/livekit_plugins_deepgram.egg-info/PKG-INFO` & `livekit_plugins_deepgram-0.5.dev0/livekit_plugins_deepgram.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-deepgram
-Version: 0.4.dev1
+Version: 0.5.dev0
 Summary: Agent Framework plugin for services using DeepGram's API.
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
 Requires-Dist: aiohttp>=3.7.4
 
 # LiveKit Plugins DeepGram
 
 Agent Framework plugin for speech-to-text with [DeepGram](https://deepgram.com/)'s API. Currently supports speech-to-text.
 
 ## Installation
```

### Comparing `livekit_plugins_deepgram-0.4.dev1/setup.py` & `livekit_plugins_deepgram-0.5.dev0/setup.py`

 * *Files 4% similar despite different names*

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
         "aiohttp >= 3.7.4",
     ],
     package_data={
         "livekit.plugins.deepgram": ["py.typed"],
     },
     project_urls={
         "Documentation": "https://docs.livekit.io",
```

