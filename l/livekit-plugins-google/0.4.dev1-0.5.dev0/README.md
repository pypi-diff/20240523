# Comparing `tmp/livekit_plugins_google-0.4.dev1.tar.gz` & `tmp/livekit_plugins_google-0.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit_plugins_google-0.4.dev1.tar", last modified: Wed May  1 00:54:18 2024, max compression
+gzip compressed data, was "livekit_plugins_google-0.5.dev0.tar", last modified: Thu May 23 15:59:24 2024, max compression
```

## Comparing `livekit_plugins_google-0.4.dev1.tar` & `livekit_plugins_google-0.5.dev0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:18.102965 livekit_plugins_google-0.4.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-01 00:54:18.102965 livekit_plugins_google-0.4.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-01 00:54:09.000000 livekit_plugins_google-0.4.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:18.098965 livekit_plugins_google-0.4.dev1/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:18.098965 livekit_plugins_google-0.4.dev1/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:18.098965 livekit_plugins_google-0.4.dev1/livekit/plugins/google/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-01 00:54:09.000000 livekit_plugins_google-0.4.dev1/livekit/plugins/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 00:54:09.000000 livekit_plugins_google-0.4.dev1/livekit/plugins/google/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-01 00:54:09.000000 livekit_plugins_google-0.4.dev1/livekit/plugins/google/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:09.000000 livekit_plugins_google-0.4.dev1/livekit/plugins/google/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-05-01 00:54:09.000000 livekit_plugins_google-0.4.dev1/livekit/plugins/google/stt.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-01 00:54:09.000000 livekit_plugins_google-0.4.dev1/livekit/plugins/google/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:54:18.102965 livekit_plugins_google-0.4.dev1/livekit_plugins_google.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-01 00:54:18.000000 livekit_plugins_google-0.4.dev1/livekit_plugins_google.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-01 00:54:18.000000 livekit_plugins_google-0.4.dev1/livekit_plugins_google.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:54:18.000000 livekit_plugins_google-0.4.dev1/livekit_plugins_google.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-01 00:54:18.000000 livekit_plugins_google-0.4.dev1/livekit_plugins_google.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 00:54:18.000000 livekit_plugins_google-0.4.dev1/livekit_plugins_google.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 00:54:09.000000 livekit_plugins_google-0.4.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:54:18.102965 livekit_plugins_google-0.4.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-01 00:54:09.000000 livekit_plugins_google-0.4.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:24.257817 livekit_plugins_google-0.5.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-23 15:59:24.257817 livekit_plugins_google-0.5.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-23 15:59:17.000000 livekit_plugins_google-0.5.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:24.253816 livekit_plugins_google-0.5.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:24.253816 livekit_plugins_google-0.5.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:24.257817 livekit_plugins_google-0.5.dev0/livekit/plugins/google/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-23 15:59:17.000000 livekit_plugins_google-0.5.dev0/livekit/plugins/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-23 15:59:17.000000 livekit_plugins_google-0.5.dev0/livekit/plugins/google/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-23 15:59:17.000000 livekit_plugins_google-0.5.dev0/livekit/plugins/google/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:17.000000 livekit_plugins_google-0.5.dev0/livekit/plugins/google/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-05-23 15:59:17.000000 livekit_plugins_google-0.5.dev0/livekit/plugins/google/stt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-23 15:59:17.000000 livekit_plugins_google-0.5.dev0/livekit/plugins/google/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-23 15:59:17.000000 livekit_plugins_google-0.5.dev0/livekit/plugins/google/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:24.257817 livekit_plugins_google-0.5.dev0/livekit_plugins_google.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-23 15:59:24.000000 livekit_plugins_google-0.5.dev0/livekit_plugins_google.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-23 15:59:24.000000 livekit_plugins_google-0.5.dev0/livekit_plugins_google.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:59:24.000000 livekit_plugins_google-0.5.dev0/livekit_plugins_google.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-23 15:59:24.000000 livekit_plugins_google-0.5.dev0/livekit_plugins_google.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 15:59:24.000000 livekit_plugins_google-0.5.dev0/livekit_plugins_google.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 15:59:17.000000 livekit_plugins_google-0.5.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:59:24.257817 livekit_plugins_google-0.5.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-23 15:59:17.000000 livekit_plugins_google-0.5.dev0/setup.py
```

### Comparing `livekit_plugins_google-0.4.dev1/PKG-INFO` & `livekit_plugins_google-0.5.dev0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-google
-Version: 0.4.dev1
+Version: 0.5.dev0
 Summary: Agent Framework plugin for services from Google Cloud
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -26,15 +26,15 @@
 Requires-Dist: google-auth<3,>=2
 Requires-Dist: google-cloud-core<3,>=2
 Requires-Dist: google-cloud-speech<3,>=2
 Requires-Dist: google-cloud-texttospeech<3,>=2
 Requires-Dist: google-cloud-translate<4,>=3
 Requires-Dist: googleapis-common-protos<2,>=1
 Requires-Dist: livekit~=0.11
-Requires-Dist: livekit-agents~=0.6.dev1
+Requires-Dist: livekit-agents~=0.7.dev0
 
 # LiveKit Plugins Google
 
 Agent Framework plugin for services from Google Cloud. Currently supporting Google's [Speech-to-Text](https://cloud.google.com/speech-to-text) API.
 
 ## Installation
```

### Comparing `livekit_plugins_google-0.4.dev1/README.md` & `livekit_plugins_google-0.5.dev0/README.md`

 * *Files identical despite different names*

### Comparing `livekit_plugins_google-0.4.dev1/livekit/plugins/google/__init__.py` & `livekit_plugins_google-0.5.dev0/livekit/plugins/google/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .stt import STT, SpeechStream
+from .tts import TTS
 from .version import __version__
 
-__all__ = ["STT", "SpeechStream", "__version__"]
+__all__ = ["STT", "TTS", "SpeechStream", "__version__"]
 
 from livekit.agents import Plugin
 
 
 class GooglePlugin(Plugin):
     def __init__(self):
         super().__init__(__name__, __version__, __package__)
```

### Comparing `livekit_plugins_google-0.4.dev1/livekit/plugins/google/models.py` & `livekit_plugins_google-0.5.dev0/livekit/plugins/google/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,7 +79,11 @@
     "es-US",
     "th-TH",
     "tr-TR",
     "uk-UA",
     "vi-VN",
     "da-DK",
 ]
+
+Gender = Literal["male", "female", "neutral"]
+
+AudioEncoding = Literal["wav", "mp3", "ogg", "mulaw", "alaw", "linear16"]
```

### Comparing `livekit_plugins_google-0.4.dev1/livekit/plugins/google/stt.py` & `livekit_plugins_google-0.5.dev0/livekit/plugins/google/stt.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import dataclasses
+import os
 from dataclasses import dataclass
-from typing import Any, AsyncIterable, Dict, List
+from typing import AsyncIterable, List, Optional, Union
 
 from livekit import agents, rtc
 from livekit.agents import stt
 from livekit.agents.utils import AudioBuffer
 
-from google.auth import credentials  # type: ignore
 from google.cloud.speech_v2 import SpeechAsyncClient
 from google.cloud.speech_v2.types import cloud_speech
 
 from .log import logger
 from .models import SpeechLanguages, SpeechModels
 
-LgType = SpeechLanguages | str
-LanguageCode = LgType | List[LgType]
+LgType = Union[SpeechLanguages, str]
+LanguageCode = Union[LgType, List[LgType]]
 
 
 # This class is only be used internally to encapsulate the options
 @dataclass
 class STTOptions:
     languages: List[LgType]
     detect_language: bool
@@ -52,48 +52,69 @@
         *,
         languages: LanguageCode = "en-US",  # Google STT can accept multiple languages
         detect_language: bool = True,
         interim_results: bool = True,
         punctuate: bool = True,
         spoken_punctuation: bool = True,
         model: SpeechModels = "long",
-        credentials_info: Dict[str, Any] | None = None,
+        credentials_info: dict | None = None,
         credentials_file: str | None = None,
     ):
         """
         if no credentials is provided, it will use the credentials on the environment
-        GOOGLE_APPLICATION_CREDENTIALS (Default behavior of Google SpeechAsyncClient)
+        GOOGLE_APPLICATION_CREDENTIALS (default behavior of Google SpeechAsyncClient)
         """
         super().__init__(streaming_supported=True)
 
-        if credentials_info:
-            self._client = SpeechAsyncClient.from_service_account_info(credentials_info)
-        elif credentials_file:
-            self._client = SpeechAsyncClient.from_service_account_file(credentials_file)
-        else:
-            self._client = SpeechAsyncClient()
+        self._client: SpeechAsyncClient | None = None
+        self._credentials_info = credentials_info
+        self._credentials_file = credentials_file
+
+        if credentials_file is None and credentials_info is None:
+            creds = os.environ.get("GOOGLE_APPLICATION_CREDENTIALS")
+            if not creds:
+                raise ValueError(
+                    "GOOGLE_APPLICATION_CREDENTIALS must be set if no credentials is provided"
+                )
 
         if isinstance(languages, str):
             languages = [languages]
 
         self._config = STTOptions(
             languages=languages,
             detect_language=detect_language,
             interim_results=interim_results,
             punctuate=punctuate,
             spoken_punctuation=spoken_punctuation,
             model=model,
         )
-        self._creds = self._client.transport._credentials
+
+    def _ensure_client(self) -> SpeechAsyncClient:
+        if self._credentials_info:
+            self._client = SpeechAsyncClient.from_service_account_info(
+                self._credentials_info
+            )
+        elif self._credentials_file:
+            self._client = SpeechAsyncClient.from_service_account_file(
+                self._credentials_file
+            )
+        else:
+            self._client = SpeechAsyncClient()
+
+        assert self._client is not None
+        return self._client
 
     @property
     def _recognizer(self) -> str:
         # TODO(theomonnom): should we use recognizers?
-        # Recognizers may improve latency https://cloud.google.com/speech-to-text/v2/docs/recognizers#understand_recognizers
-        return f"projects/{self._creds.project_id}/locations/global/recognizers/_"  # type: ignore
+        # recognizers may improve latency https://cloud.google.com/speech-to-text/v2/docs/recognizers#understand_recognizers
+
+        # TODO(theomonnom): find a better way to access the project_id
+        project_id = self._ensure_client().transport._credentials.project_id  # type: ignore
+        return f"projects/{project_id}/locations/global/recognizers/_"
 
     def _sanitize_options(
         self,
         *,
         language: str | None = None,
     ) -> STTOptions:
         config = dataclasses.replace(self._config)
@@ -115,93 +136,92 @@
     async def recognize(
         self,
         *,
         buffer: AudioBuffer,
         language: SpeechLanguages | str | None = None,
     ) -> stt.SpeechEvent:
         config = self._sanitize_options(language=language)
-        buffer = agents.utils.merge_frames(buffer)
+        frame = agents.utils.merge_frames(buffer)
 
         config = cloud_speech.RecognitionConfig(
             explicit_decoding_config=cloud_speech.ExplicitDecodingConfig(
                 encoding=cloud_speech.ExplicitDecodingConfig.AudioEncoding.LINEAR16,
-                sample_rate_hertz=buffer.sample_rate,
-                audio_channel_count=buffer.num_channels,
+                sample_rate_hertz=frame.sample_rate,
+                audio_channel_count=frame.num_channels,
             ),
             features=cloud_speech.RecognitionFeatures(
                 enable_automatic_punctuation=config.punctuate,
                 enable_spoken_punctuation=config.spoken_punctuation,
+                enable_word_time_offsets=True,
             ),
             model=config.model,
             language_codes=config.languages,
         )
 
-        return recognize_response_to_speech_event(
-            await self._client.recognize(
-                cloud_speech.RecognizeRequest(
-                    recognizer=self._recognizer,
-                    config=config,
-                    content=buffer.data.tobytes(),
-                )
+        raw = await self._ensure_client().recognize(
+            cloud_speech.RecognizeRequest(
+                recognizer=self._recognizer,
+                config=config,
+                content=frame.data.tobytes(),
             )
         )
+        return _recognize_response_to_speech_event(raw)
 
     def stream(
         self,
         *,
         language: SpeechLanguages | str | None = None,
     ) -> "SpeechStream":
         config = self._sanitize_options(language=language)
         return SpeechStream(
-            self._client,
-            self._creds,
+            self._ensure_client(),
             self._recognizer,
             config,
         )
 
 
 class SpeechStream(stt.SpeechStream):
     def __init__(
         self,
         client: SpeechAsyncClient,
-        creds: credentials.Credentials,
         recognizer: str,
         config: STTOptions,
-        sample_rate: int = 24000,
+        sample_rate: int = 48000,
         num_channels: int = 1,
         max_retry: int = 32,
     ) -> None:
         super().__init__()
 
         self._client = client
-        self._creds = creds
         self._recognizer = recognizer
         self._config = config
         self._sample_rate = sample_rate
         self._num_channels = num_channels
 
-        self._queue = asyncio.Queue[rtc.AudioFrame | None]()
-        self._event_queue = asyncio.Queue[stt.SpeechEvent | None]()
+        self._queue = asyncio.Queue[Optional[rtc.AudioFrame]]()
+        self._event_queue = asyncio.Queue[Optional[stt.SpeechEvent]]()
         self._closed = False
         self._main_task = asyncio.create_task(self._run(max_retry=max_retry))
 
         self._final_events: List[stt.SpeechEvent] = []
-        self._speaking = False
+        self._need_bos = True
+        self._need_eos = False
 
         self._streaming_config = cloud_speech.StreamingRecognitionConfig(
             config=cloud_speech.RecognitionConfig(
                 explicit_decoding_config=cloud_speech.ExplicitDecodingConfig(
                     encoding=cloud_speech.ExplicitDecodingConfig.AudioEncoding.LINEAR16,
                     sample_rate_hertz=self._sample_rate,
                     audio_channel_count=self._num_channels,
                 ),
                 language_codes=self._config.languages,
                 model=self._config.model,
                 features=cloud_speech.RecognitionFeatures(
                     enable_automatic_punctuation=self._config.punctuate,
+                    enable_word_time_offsets=True,
                 ),
             ),
             streaming_features=cloud_speech.StreamingRecognitionFeatures(
                 enable_voice_activity_events=True,
                 interim_results=self._config.interim_results,
             ),
         )
@@ -214,189 +234,230 @@
 
     def push_frame(self, frame: rtc.AudioFrame) -> None:
         if self._closed:
             raise ValueError("cannot push frame to closed stream")
 
         self._queue.put_nowait(frame)
 
-    async def aclose(self, wait: bool = True) -> None:
+    async def aclose(self, *, wait: bool = True) -> None:
         self._closed = True
         if not wait:
             self._main_task.cancel()
 
         self._queue.put_nowait(None)
         with contextlib.suppress(asyncio.CancelledError):
             await self._main_task
 
     async def _run(self, max_retry: int) -> None:
         retry_count = 0
-        try:
-            while not self._closed:
-                try:
-                    # google requires a async generator when calling streaming_recognize
-                    # this function basically convert the queue into a async generator
-                    async def input_generator():
-                        try:
-                            # first request should contain the config
-                            yield cloud_speech.StreamingRecognizeRequest(
-                                recognizer=self._recognizer,
-                                streaming_config=self._streaming_config,
+        while not self._closed:
+            try:
+                # google requires a async generator when calling streaming_recognize
+                # this function basically convert the queue into a async generator
+                async def input_generator():
+                    try:
+                        # first request should contain the config
+                        yield cloud_speech.StreamingRecognizeRequest(
+                            recognizer=self._recognizer,
+                            streaming_config=self._streaming_config,
+                        )
+                        while True:
+                            frame = await self._queue.get()
+                            if frame is None:
+                                break
+
+                            frame = frame.remix_and_resample(
+                                self._sample_rate, self._num_channels
                             )
-                            while True:
-                                frame = (
-                                    await self._queue.get()
-                                )  # wait for a new rtc.AudioFrame
-                                if frame is None:
-                                    break  # None is sent inside aclose
-
-                                self._queue.task_done()
-                                frame = frame.remix_and_resample(
-                                    self._sample_rate, self._num_channels
-                                )
-                                yield cloud_speech.StreamingRecognizeRequest(
-                                    audio=frame.data.tobytes(),
-                                )
-                        except Exception as e:
-                            logger.error(
-                                f"an error occurred while streaming inputs: {e}"
+                            yield cloud_speech.StreamingRecognizeRequest(
+                                audio=frame.data.tobytes(),
                             )
+                    except Exception as e:
+                        logger.error(f"an error occurred while streaming inputs: {e}")
 
-                    # try to connect
-                    stream = await self._client.streaming_recognize(
-                        requests=input_generator()
-                    )
-                    retry_count = 0  # connection successful, reset retry count
-
-                    await self._run_stream(stream)
-                except Exception as e:
-                    if retry_count >= max_retry:
-                        logger.error(
-                            f"failed to connect to google stt after {max_retry} tries",
-                            exc_info=e,
-                        )
-                        break
+                # try to connect
+                stream = await self._client.streaming_recognize(
+                    requests=input_generator()
+                )
+                retry_count = 0  # connection successful, reset retry count
 
-                    retry_delay = min(retry_count * 2, 10)  # max 10s
-                    retry_count += 1
-                    logger.warning(
-                        f"google stt connection failed, retrying in {retry_delay}s",
+                await self._run_stream(stream)
+            except Exception as e:
+                if retry_count >= max_retry:
+                    logger.error(
+                        f"failed to connect to google stt after {max_retry} tries",
                         exc_info=e,
                     )
-                    await asyncio.sleep(retry_delay)
-        finally:
-            self._event_queue.put_nowait(None)
+                    break
+
+                retry_delay = min(retry_count * 2, 5)  # max 5s
+                retry_count += 1
+                logger.warning(
+                    f"google stt connection failed, retrying in {retry_delay}s",
+                    exc_info=e,
+                )
+                await asyncio.sleep(retry_delay)
+
+        self._event_queue.put_nowait(None)
 
     async def _run_stream(
         self, stream: AsyncIterable[cloud_speech.StreamingRecognizeResponse]
     ):
         async for resp in stream:
             if (
                 resp.speech_event_type
                 == cloud_speech.StreamingRecognizeResponse.SpeechEventType.SPEECH_ACTIVITY_BEGIN
             ):
-                self._speaking = True
-                start_event = stt.SpeechEvent(
-                    type=stt.SpeechEventType.START_OF_SPEECH,
-                )
-                self._event_queue.put_nowait(start_event)
+                if self._need_eos:
+                    self._send_eos()
+
+            if self._need_bos:
+                self._send_bos()
 
             if (
                 resp.speech_event_type
                 == cloud_speech.StreamingRecognizeResponse.SpeechEventType.SPEECH_EVENT_TYPE_UNSPECIFIED
             ):
                 result = resp.results[0]
                 if not result.is_final:
-                    # interim results
                     iterim_event = stt.SpeechEvent(
                         type=stt.SpeechEventType.INTERIM_TRANSCRIPT,
-                        alternatives=streaming_recognize_response_to_speech_data(resp),
+                        alternatives=[
+                            _streaming_recognize_response_to_speech_data(resp)
+                        ],
                     )
                     self._event_queue.put_nowait(iterim_event)
 
                 else:
                     final_event = stt.SpeechEvent(
                         type=stt.SpeechEventType.FINAL_TRANSCRIPT,
-                        alternatives=streaming_recognize_response_to_speech_data(resp),
+                        alternatives=[
+                            _streaming_recognize_response_to_speech_data(resp)
+                        ],
                     )
                     self._final_events.append(final_event)
                     self._event_queue.put_nowait(final_event)
 
-                    if not self._speaking:
-                        # With Google STT, we receive the final event after the END_OF_SPEECH event
-                        sentence = ""
-                        confidence = 0.0
-                        for alt in self._final_events:
-                            sentence += f"{alt.alternatives[0].text.strip()} "
-                            confidence += alt.alternatives[0].confidence
-
-                        sentence = sentence.rstrip()
-                        confidence /= len(self._final_events)  # avg. of confidence
-
-                        end_event = stt.SpeechEvent(
-                            type=stt.SpeechEventType.END_OF_SPEECH,
-                            alternatives=[
-                                stt.SpeechData(
-                                    language=result.language_code,
-                                    start_time=self._final_events[0]
-                                    .alternatives[0]
-                                    .start_time,
-                                    end_time=self._final_events[-1]
-                                    .alternatives[0]
-                                    .end_time,
-                                    confidence=confidence,
-                                    text=sentence,
-                                )
-                            ],
-                        )
-
-                        self._final_events = []
-                        self._event_queue.put_nowait(end_event)
+            if self._need_eos:
+                self._send_eos()
 
             if (
                 resp.speech_event_type
                 == cloud_speech.StreamingRecognizeResponse.SpeechEventType.SPEECH_ACTIVITY_END
             ):
-                self._speaking = False
+                self._need_eos = True
+
+        if not self._need_bos:
+            self._send_eos()
+
+    def _send_bos(self) -> None:
+        self._need_bos = False
+        start_event = stt.SpeechEvent(
+            type=stt.SpeechEventType.START_OF_SPEECH,
+        )
+        self._event_queue.put_nowait(start_event)
+
+    def _send_eos(self) -> None:
+        self._need_eos = False
+        self._need_bos = True
+
+        if self._final_events:
+            lg = self._final_events[0].alternatives[0].language
+
+            sentence = ""
+            confidence = 0.0
+            for alt in self._final_events:
+                sentence += f"{alt.alternatives[0].text.strip()} "
+                confidence += alt.alternatives[0].confidence
+
+            sentence = sentence.rstrip()
+            confidence /= len(self._final_events)  # avg. of confidence
+
+            end_event = stt.SpeechEvent(
+                type=stt.SpeechEventType.END_OF_SPEECH,
+                alternatives=[
+                    stt.SpeechData(
+                        language=lg,
+                        start_time=self._final_events[0].alternatives[0].start_time,
+                        end_time=self._final_events[-1].alternatives[0].end_time,
+                        confidence=confidence,
+                        text=sentence,
+                    )
+                ],
+            )
+
+            self._final_events = []
+            self._event_queue.put_nowait(end_event)
+        else:
+            end_event = stt.SpeechEvent(
+                type=stt.SpeechEventType.END_OF_SPEECH,
+                alternatives=[
+                    stt.SpeechData(
+                        language="",
+                        start_time=0,
+                        end_time=0,
+                        confidence=0,
+                        text="",
+                    )
+                ],
+            )
+
+            self._event_queue.put_nowait(end_event)
 
     async def __anext__(self) -> stt.SpeechEvent:
         evt = await self._event_queue.get()
         if evt is None:
             raise StopAsyncIteration
 
         return evt
 
 
-def recognize_response_to_speech_event(
+def _recognize_response_to_speech_event(
     resp: cloud_speech.RecognizeResponse,
 ) -> stt.SpeechEvent:
-    result = resp.results[0]
-    gg_alts = result.alternatives
+    text = ""
+    confidence = 0.0
+    for result in resp.results:
+        text += result.alternatives[0].transcript
+        confidence += result.alternatives[0].confidence
+
+    # not sure why start_offset and end_offset returns a timedelta
+    start_offset = resp.results[0].alternatives[0].words[0].start_offset
+    end_offset = resp.results[-1].alternatives[0].words[-1].end_offset
+
+    confidence /= len(resp.results)
+    lg = resp.results[0].language_code
     return stt.SpeechEvent(
         type=stt.SpeechEventType.FINAL_TRANSCRIPT,
         alternatives=[
             stt.SpeechData(
-                language=result.language_code,
-                start_time=alt.words[0].start_offset.seconds if alt.words else 0,
-                end_time=alt.words[-1].end_offset.seconds if alt.words else 0,
-                confidence=alt.confidence,
-                text=alt.transcript,
+                language=lg,
+                start_time=start_offset.total_seconds(),  # type: ignore
+                end_time=end_offset.total_seconds(),  # type: ignore
+                confidence=confidence,
+                text=text,
             )
-            for alt in gg_alts
         ],
     )
 
 
-def streaming_recognize_response_to_speech_data(
+def _streaming_recognize_response_to_speech_data(
     resp: cloud_speech.StreamingRecognizeResponse,
-) -> List[stt.SpeechData]:
-    result = resp.results[0]
-    gg_alts = result.alternatives
-    return [
-        stt.SpeechData(
-            language=result.language_code,
-            start_time=alt.words[0].start_offset.seconds if alt.words else 0,
-            end_time=alt.words[-1].end_offset.seconds if alt.words else 0,
-            confidence=alt.confidence,
-            text=alt.transcript,
-        )
-        for alt in gg_alts
-    ]
+) -> stt.SpeechData:
+    text = ""
+    confidence = 0.0
+    for result in resp.results:
+        text += result.alternatives[0].transcript
+        confidence += result.alternatives[0].confidence
+
+    confidence /= len(resp.results)
+    lg = resp.results[0].language_code
+
+    data = stt.SpeechData(
+        language=lg,
+        start_time=0,
+        end_time=0,
+        confidence=confidence,
+        text=text,
+    )
+
+    return data
```

### Comparing `livekit_plugins_google-0.4.dev1/livekit/plugins/google/version.py` & `livekit_plugins_google-0.5.dev0/livekit/plugins/google/version.py`

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

### Comparing `livekit_plugins_google-0.4.dev1/livekit_plugins_google.egg-info/PKG-INFO` & `livekit_plugins_google-0.5.dev0/livekit_plugins_google.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-google
-Version: 0.4.dev1
+Version: 0.5.dev0
 Summary: Agent Framework plugin for services from Google Cloud
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -26,15 +26,15 @@
 Requires-Dist: google-auth<3,>=2
 Requires-Dist: google-cloud-core<3,>=2
 Requires-Dist: google-cloud-speech<3,>=2
 Requires-Dist: google-cloud-texttospeech<3,>=2
 Requires-Dist: google-cloud-translate<4,>=3
 Requires-Dist: googleapis-common-protos<2,>=1
 Requires-Dist: livekit~=0.11
-Requires-Dist: livekit-agents~=0.6.dev1
+Requires-Dist: livekit-agents~=0.7.dev0
 
 # LiveKit Plugins Google
 
 Agent Framework plugin for services from Google Cloud. Currently supporting Google's [Speech-to-Text](https://cloud.google.com/speech-to-text) API.
 
 ## Installation
```

### Comparing `livekit_plugins_google-0.4.dev1/setup.py` & `livekit_plugins_google-0.5.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         "google-auth >= 2, < 3",
         "google-cloud-core >= 2, < 3",
         "google-cloud-speech >= 2, < 3",
         "google-cloud-texttospeech >= 2, < 3",
         "google-cloud-translate >= 3, < 4",
         "googleapis-common-protos >= 1, < 2",
         "livekit ~= 0.11",
-        "livekit-agents~=0.6.dev1",
+        "livekit-agents~=0.7.dev0",
     ],
     package_data={
         "livekit.plugins.google": ["py.typed"],
     },
     project_urls={
         "Documentation": "https://docs.livekit.io",
         "Website": "https://livekit.io/",
```

