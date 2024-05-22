# Comparing `tmp/neon-nodes-0.0.1a8.tar.gz` & `tmp/neon-nodes-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-nodes-0.0.1a8.tar", last modified: Fri Apr  5 01:46:59 2024, max compression
+gzip compressed data, was "neon-nodes-0.0.2a1.tar", last modified: Wed May 22 23:52:25 2024, max compression
```

## Comparing `neon-nodes-0.0.1a8.tar` & `neon-nodes-0.0.2a1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:46:59.952230 neon-nodes-0.0.1a8/
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-05 01:46:54.000000 neon-nodes-0.0.1a8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-05 01:46:59.952230 neon-nodes-0.0.1a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-05 01:46:54.000000 neon-nodes-0.0.1a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:46:59.952230 neon-nodes-0.0.1a8/neon_nodes/
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-05 01:46:54.000000 neon-nodes-0.0.1a8/neon_nodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:46:59.952230 neon-nodes-0.0.1a8/neon_nodes/res/
--rw-r--r--   0 runner    (1001) docker     (127)   189942 2024-04-05 01:46:54.000000 neon-nodes-0.0.1a8/neon_nodes/res/error.wav
--rw-r--r--   0 runner    (1001) docker     (127)    67090 2024-04-05 01:46:54.000000 neon-nodes-0.0.1a8/neon_nodes/res/start_listening.wav
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-05 01:46:54.000000 neon-nodes-0.0.1a8/neon_nodes/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10836 2024-04-05 01:46:54.000000 neon-nodes-0.0.1a8/neon_nodes/voice_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:46:59.952230 neon-nodes-0.0.1a8/neon_nodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-05 01:46:59.000000 neon-nodes-0.0.1a8/neon_nodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-05 01:46:59.000000 neon-nodes-0.0.1a8/neon_nodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 01:46:59.000000 neon-nodes-0.0.1a8/neon_nodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-05 01:46:59.000000 neon-nodes-0.0.1a8/neon_nodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 01:46:59.000000 neon-nodes-0.0.1a8/neon_nodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 01:46:59.000000 neon-nodes-0.0.1a8/neon_nodes.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 01:46:59.952230 neon-nodes-0.0.1a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-05 01:46:54.000000 neon-nodes-0.0.1a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:52:25.602594 neon-nodes-0.0.2a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-22 23:52:22.000000 neon-nodes-0.0.2a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-22 23:52:25.602594 neon-nodes-0.0.2a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-22 23:52:22.000000 neon-nodes-0.0.2a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:52:25.602594 neon-nodes-0.0.2a1/neon_nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-22 23:52:22.000000 neon-nodes-0.0.2a1/neon_nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:52:25.602594 neon-nodes-0.0.2a1/neon_nodes/res/
+-rw-r--r--   0 runner    (1001) docker     (127)   189942 2024-05-22 23:52:22.000000 neon-nodes-0.0.2a1/neon_nodes/res/error.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    67090 2024-05-22 23:52:22.000000 neon-nodes-0.0.2a1/neon_nodes/res/start_listening.wav
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-22 23:52:22.000000 neon-nodes-0.0.2a1/neon_nodes/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10810 2024-05-22 23:52:22.000000 neon-nodes-0.0.2a1/neon_nodes/voice_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12437 2024-05-22 23:52:22.000000 neon-nodes-0.0.2a1/neon_nodes/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:52:25.602594 neon-nodes-0.0.2a1/neon_nodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-22 23:52:25.000000 neon-nodes-0.0.2a1/neon_nodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-22 23:52:25.000000 neon-nodes-0.0.2a1/neon_nodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 23:52:25.000000 neon-nodes-0.0.2a1/neon_nodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-22 23:52:25.000000 neon-nodes-0.0.2a1/neon_nodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 23:52:25.000000 neon-nodes-0.0.2a1/neon_nodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 23:52:25.000000 neon-nodes-0.0.2a1/neon_nodes.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 23:52:25.602594 neon-nodes-0.0.2a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-22 23:52:22.000000 neon-nodes-0.0.2a1/setup.py
```

### Comparing `neon-nodes-0.0.1a8/LICENSE.md` & `neon-nodes-0.0.2a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-nodes-0.0.1a8/PKG-INFO` & `neon-nodes-0.0.2a1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-Metadata-Version: 2.1
-Name: neon-nodes
-Version: 0.0.1a8
-Summary: Neon node clients for Hana
-Home-page: https://github.com/NeonGeckoCom/neon-nodes
-Author: NeonGecko
-Author-email: developers@neon.ai
-License: BSD-3-Clause
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-Provides-Extra: voice-client
-License-File: LICENSE.md
-
 # Neon Nodes
 Clients for connecting to a server running Hana. These are minimal classes that
 are responsible for collecting a user's input, sending it to a remote system for
 processing, and presenting a response to the user.
 
 ## Voice Client
 The voice client will start a service that listens for a wake word on the local
 system, sends recorded speech to a HANA endpoint for processing, and plays back
 the response.
+
+## Websocket Client
+The websocket client starts a local listener service and establishes a websocket
+connection to a remove HANA server. Compared to the Voice Client, this has 
+lower latency and allows for asynchronous messages from the HANA server.
+
+## Configuration
+This service is configured via `~/.config/neon/neon.yaml`.
+
+```yaml
+neon_node:
+  description: Neon Node  # Friendly description of the node
+  hana_address: https://hana.neonaiservices.com  # Hana server HTTP address
+  hana_username: node_user  # Hana node user username
+  hana_password: node_password  # Hana node user password
+```
```

### Comparing `neon-nodes-0.0.1a8/neon_nodes/__init__.py` & `neon-nodes-0.0.2a1/neon_nodes/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-# NEON AI (TM) SOFTWARE, Software Development Kit & Application Development System
+# NEON AI (TM) SOFTWARE, Software Development Kit & Application Framework
 # All trademark and other rights reserved by their respective owners
-# Copyright 2008-2021 Neongecko.com Inc.
-# BSD-3
+# Copyright 2008-2022 Neongecko.com Inc.
+# Contributors: Daniel McKnight, Guy Daniels, Elon Gasper, Richard Leeds,
+# Regina Bloomstine, Casimiro Ferreira, Andrii Pernatii, Kirill Hrymailo
+# BSD-3 License
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
 # 2. Redistributions in binary form must reproduce the above copyright notice,
 #    this list of conditions and the following disclaimer in the documentation
 #    and/or other materials provided with the distribution.
@@ -19,7 +21,9 @@
 # CONTRIBUTORS  BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+__version__ = "0.0.2a1"
```

### Comparing `neon-nodes-0.0.1a8/neon_nodes/res/error.wav` & `neon-nodes-0.0.2a1/neon_nodes/res/error.wav`

 * *Files identical despite different names*

### Comparing `neon-nodes-0.0.1a8/neon_nodes/res/start_listening.wav` & `neon-nodes-0.0.2a1/neon_nodes/res/start_listening.wav`

 * *Files identical despite different names*

### Comparing `neon-nodes-0.0.1a8/neon_nodes/version.py` & `neon-nodes-0.0.2a1/neon_nodes/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# NEON AI (TM) SOFTWARE, Software Development Kit & Application Framework
+# NEON AI (TM) SOFTWARE, Software Development Kit & Application Development System
 # All trademark and other rights reserved by their respective owners
-# Copyright 2008-2022 Neongecko.com Inc.
-# Contributors: Daniel McKnight, Guy Daniels, Elon Gasper, Richard Leeds,
-# Regina Bloomstine, Casimiro Ferreira, Andrii Pernatii, Kirill Hrymailo
-# BSD-3 License
+# Copyright 2008-2021 Neongecko.com Inc.
+# BSD-3
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
 # 2. Redistributions in binary form must reproduce the above copyright notice,
 #    this list of conditions and the following disclaimer in the documentation
 #    and/or other materials provided with the distribution.
@@ -22,8 +20,33 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.0.1a8"
+from mock import Mock
+from ovos_utils.log import LOG
+
+class MockTransformers(Mock):
+    def transform(self, chunk):
+        return chunk, dict()
+
+
+def on_ready():
+    LOG.info("ready")
+
+
+def on_stopping():
+    LOG.info("stopping")
+
+
+def on_error(e="unknown"):
+    LOG.error(e)
+
+
+def on_alive():
+    LOG.debug("alive")
+
+
+def on_started():
+    LOG.debug("started")
```

### Comparing `neon-nodes-0.0.1a8/neon_nodes/voice_client.py` & `neon-nodes-0.0.2a1/neon_nodes/voice_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,49 +43,28 @@
 from neon_utils.hana_utils import request_backend, ServerException
 from neon_utils.net_utils import get_adapter_info
 from neon_utils.user_utils import get_default_user_config
 from speech_recognition import AudioData
 from pydub import AudioSegment
 from pydub.playback import play
 
-
-class MockTransformers(Mock):
-    def transform(self, chunk):
-        return chunk, dict()
-
-
-def on_ready():
-    LOG.info("ready")
-
-
-def on_stopping():
-    LOG.info("stopping")
-
-
-def on_error(e="unknown"):
-    LOG.error(e)
-
-
-def on_alive():
-    LOG.debug("alive")
-
-
-def on_started():
-    LOG.debug("started")
+from neon_nodes import on_alive, on_error, on_ready, on_started, on_stopping, MockTransformers
 
 
 class NeonVoiceClient:
     def __init__(self, bus=None, ready_hook=on_ready, error_hook=on_error,
                  stopping_hook=on_stopping, alive_hook=on_alive,
                  started_hook=on_started):
         self.error_hook = error_hook
         self.stopping_hook = stopping_hook
         alive_hook()
         self.config = Configuration()
-        self._device_data = self.config.get('neon_node', {})
+        self._node_config = self.config.get('neon_node', {})
+        self._hana_address = self._node_config.get('hana_address')
+
         LOG.init(self.config.get("logging"))
         self.bus = bus or FakeBus()
         self.lang = self.config.get('lang') or "en-us"
         self._mic = OVOSMicrophoneFactory.create(self.config)
         self._mic.start()
         self._hotwords = HotwordContainer(self.bus)
         self._hotwords.load_hotword_engines()
@@ -104,15 +83,15 @@
         self._voice_thread = None
         self._watchdog_event = Event()
 
         self._listening_sound = None
         self._error_sound = None
 
         self._network_info = dict()
-        self._node_data = dict()
+        self._node_data = {"description": self._node_config.get("description")}
 
         started_hook()
         self.run()
         ready_hook()
 
     @property
     def listening_sound(self) -> AudioSegment:
@@ -236,26 +215,29 @@
         """
         Handle recorded audio input and get/speak a response.
         @param audio: bytes of STT audio
         """
         audio_data = b64encode(audio).decode("utf-8")
         transcript = request_backend("neon/get_stt",
                                      {"encoded_audio": audio_data,
-                                      "lang_code": self.lang})
+                                      "lang_code": self.lang},
+                                     server_url=self._hana_address)
         transcribed = transcript['transcripts'][0]
         LOG.info(transcribed)
         response = request_backend("neon/get_response",
                                    {"lang_code": self.lang,
                                     "user_profile": self.user_profile,
                                     "node_data": self.node_data,
-                                    "utterance": transcribed})
+                                    "utterance": transcribed},
+                                   server_url=self._hana_address)
         answer = response['answer']
         LOG.info(answer)
         audio = request_backend("neon/get_tts", {"lang_code": self.lang,
-                                                 "to_speak": answer})
+                                                 "to_speak": answer},
+                                server_url=self._hana_address)
         audio_bytes = b64decode(audio['encoded_audio'])
         play(AudioSegment.from_file(io.BytesIO(audio_bytes), format="wav"))
         LOG.info(f"Playback completed")
 
     def shutdown(self):
         """
         Cleanly stop all threads and shutdown this service
@@ -268,10 +250,8 @@
 
 def main(*args, **kwargs):
     client = NeonVoiceClient(*args, **kwargs)
     client.watchdog()
 
 
 if __name__ == "__main__":
-    # environ.setdefault("OVOS_CONFIG_BASE_FOLDER", "neon")
-    # environ.setdefault("OVOS_CONFIG_FILENAME", "diana.yaml")
     main()
```

### Comparing `neon-nodes-0.0.1a8/setup.py` & `neon-nodes-0.0.2a1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,16 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/NeonGeckoCom/neon-nodes',
     author='NeonGecko',
     author_email='developers@neon.ai',
     license='BSD-3-Clause',
     packages=find_packages(),
-    extras_require={"voice-client": get_requirements("voice_client.txt")},
+    extras_require={"voice-client": get_requirements("voice_client.txt"),
+                    "websocket-client": get_requirements("websocket_client.txt")},
     package_data={'neon_nodes': ['res/*']},
     zip_safe=True,
     classifiers=[
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
     ]
 )
```

