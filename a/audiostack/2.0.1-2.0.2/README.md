# Comparing `tmp/audiostack-2.0.1.tar.gz` & `tmp/audiostack-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiostack-2.0.1.tar", max compression
+gzip compressed data, was "audiostack-2.0.2.tar", max compression
```

## Comparing `audiostack-2.0.1.tar` & `audiostack-2.0.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1061 2024-05-22 09:05:46.228890 audiostack-2.0.1/LICENSE
--rw-r--r--   0        0        0     4967 2024-05-22 09:05:46.228890 audiostack-2.0.1/README.md
--rw-r--r--   0        0        0      520 2024-05-22 09:05:49.336877 audiostack-2.0.1/audiostack/__init__.py
--rw-r--r--   0        0        0      819 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/content/__init__.py
--rw-r--r--   0        0        0     6430 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/content/file.py
--rw-r--r--   0        0        0     2321 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/content/media.py
--rw-r--r--   0        0        0     2178 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/content/recommend.py
--rw-r--r--   0        0        0     1029 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/content/root_functions.py
--rw-r--r--   0        0        0     4360 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/content/script.py
--rw-r--r--   0        0        0      120 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/delivery/__init__.py
--rw-r--r--   0        0        0     3620 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/delivery/encoder.py
--rw-r--r--   0        0        0     6216 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/delivery/video.py
--rw-r--r--   0        0        0       61 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/docs/__init__.py
--rw-r--r--   0        0        0      602 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/docs/docs.py
--rw-r--r--   0        0        0        0 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/helpers/__init__.py
--rw-r--r--   0        0        0      764 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/helpers/api_item.py
--rw-r--r--   0        0        0     1102 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/helpers/api_list.py
--rw-r--r--   0        0        0     4640 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/helpers/request_interface.py
--rw-r--r--   0        0        0      163 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/helpers/request_types.py
--rw-r--r--   0        0        0      388 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/helpers/response.py
--rw-r--r--   0        0        0      227 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/helpers/util.py
--rw-r--r--   0        0        0       58 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/orchestrator/__init__.py
--rw-r--r--   0        0        0      176 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/production/__init__.py
--rw-r--r--   0        0        0     5096 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/production/mix.py
--rw-r--r--   0        0        0     4542 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/production/sound.py
--rw-r--r--   0        0        0     4685 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/production/suite.py
--rw-r--r--   0        0        0      228 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/speech/__init__.py
--rw-r--r--   0        0        0     3179 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/speech/diction.py
--rw-r--r--   0        0        0     1294 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/speech/predict.py
--rw-r--r--   0        0        0     7902 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/speech/tts.py
--rw-r--r--   0        0        0     2325 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/speech/voice.py
--rw-r--r--   0        0        0     1200 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/content/test_file.py
--rw-r--r--   0        0        0      672 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/content/test_folder.py
--rw-r--r--   0        0        0     3832 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/content/test_recommend.py
--rw-r--r--   0        0        0      906 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/content/test_transfer.py
--rw-r--r--   0        0        0     2170 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/helpers/test_request_interface.py
--rw-r--r--   0        0        0      495 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/production/test_aes.py
--rw-r--r--   0        0        0      364 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/production/test_sound.py
--rw-r--r--   0        0        0      978 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/production/test_suite.py
--rw-r--r--   0        0        0     2385 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/production/test_video.py
--rw-r--r--   0        0        0     1292 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/test_script.py
--rw-r--r--   0        0        0     1071 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/tts/test_lexi.py
--rw-r--r--   0        0        0     1427 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/tts/test_predict.py
--rw-r--r--   0        0        0      488 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/tts/test_voice.py
--rw-r--r--   0        0        0     1819 2024-05-22 09:05:46.232890 audiostack-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     5715 1970-01-01 00:00:00.000000 audiostack-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-23 13:23:07.279255 audiostack-2.0.2/LICENSE
+-rw-r--r--   0        0        0     4967 2024-05-23 13:23:07.279255 audiostack-2.0.2/README.md
+-rw-r--r--   0        0        0      520 2024-05-23 13:23:11.419253 audiostack-2.0.2/audiostack/__init__.py
+-rw-r--r--   0        0        0      819 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/content/__init__.py
+-rw-r--r--   0        0        0     6430 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/content/file.py
+-rw-r--r--   0        0        0     2321 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/content/media.py
+-rw-r--r--   0        0        0     2178 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/content/recommend.py
+-rw-r--r--   0        0        0     1029 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/content/root_functions.py
+-rw-r--r--   0        0        0     4360 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/content/script.py
+-rw-r--r--   0        0        0      120 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/delivery/__init__.py
+-rw-r--r--   0        0        0     3620 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/delivery/encoder.py
+-rw-r--r--   0        0        0     6070 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/delivery/video.py
+-rw-r--r--   0        0        0       61 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/docs/__init__.py
+-rw-r--r--   0        0        0      602 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/docs/docs.py
+-rw-r--r--   0        0        0        0 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/helpers/__init__.py
+-rw-r--r--   0        0        0      764 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/helpers/api_item.py
+-rw-r--r--   0        0        0     1102 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/helpers/api_list.py
+-rw-r--r--   0        0        0     4640 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/helpers/request_interface.py
+-rw-r--r--   0        0        0      163 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/helpers/request_types.py
+-rw-r--r--   0        0        0      388 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/helpers/response.py
+-rw-r--r--   0        0        0      227 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/helpers/util.py
+-rw-r--r--   0        0        0       58 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/orchestrator/__init__.py
+-rw-r--r--   0        0        0      176 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/production/__init__.py
+-rw-r--r--   0        0        0     5096 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/production/mix.py
+-rw-r--r--   0        0        0     4542 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/production/sound.py
+-rw-r--r--   0        0        0     4685 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/production/suite.py
+-rw-r--r--   0        0        0      228 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/speech/__init__.py
+-rw-r--r--   0        0        0     3179 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/speech/diction.py
+-rw-r--r--   0        0        0     1294 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/speech/predict.py
+-rw-r--r--   0        0        0     7902 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/speech/tts.py
+-rw-r--r--   0        0        0     2325 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/speech/voice.py
+-rw-r--r--   0        0        0     1200 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/tests/content/test_file.py
+-rw-r--r--   0        0        0      672 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/tests/content/test_folder.py
+-rw-r--r--   0        0        0     3832 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/tests/content/test_recommend.py
+-rw-r--r--   0        0        0      906 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/tests/content/test_transfer.py
+-rw-r--r--   0        0        0     2170 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/tests/helpers/test_request_interface.py
+-rw-r--r--   0        0        0      495 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/tests/production/test_aes.py
+-rw-r--r--   0        0        0      364 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/tests/production/test_sound.py
+-rw-r--r--   0        0        0      978 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/tests/production/test_suite.py
+-rw-r--r--   0        0        0     2216 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/tests/production/test_video.py
+-rw-r--r--   0        0        0     1292 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/tests/test_script.py
+-rw-r--r--   0        0        0     1071 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/tests/tts/test_lexi.py
+-rw-r--r--   0        0        0     1427 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/tests/tts/test_predict.py
+-rw-r--r--   0        0        0      488 2024-05-23 13:23:07.279255 audiostack-2.0.2/audiostack/tests/tts/test_voice.py
+-rw-r--r--   0        0        0     1819 2024-05-23 13:23:07.287255 audiostack-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5715 1970-01-01 00:00:00.000000 audiostack-2.0.2/PKG-INFO
```

### Comparing `audiostack-2.0.1/LICENSE` & `audiostack-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/README.md` & `audiostack-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/__init__.py` & `audiostack-2.0.2/audiostack/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-sdk_version = "2.0.1"
+sdk_version = "2.0.2"
 api_base = "https://v2.api.audio"
 api_key = None
 assume_org_id = None
 app_info = None
 
 
 from audiostack import content as Content  # noqa: F401
```

### Comparing `audiostack-2.0.1/audiostack/content/__init__.py` & `audiostack-2.0.2/audiostack/content/__init__.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/content/file.py` & `audiostack-2.0.2/audiostack/content/file.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/content/media.py` & `audiostack-2.0.2/audiostack/content/media.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/content/recommend.py` & `audiostack-2.0.2/audiostack/content/recommend.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/content/root_functions.py` & `audiostack-2.0.2/audiostack/content/root_functions.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/content/script.py` & `audiostack-2.0.2/audiostack/content/script.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/delivery/encoder.py` & `audiostack-2.0.2/audiostack/delivery/encoder.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/delivery/video.py` & `audiostack-2.0.2/audiostack/delivery/video.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,30 +46,29 @@
             "productionId": productionId,
             "public": public,
         }
         r = Video.interface.send_request(
             rtype=RequestTypes.POST, route="video", json=body
         )
         retries = 0
-        max_retries = 10
+        max_retries = 30
         while r["statusCode"] == 202 and retries < max_retries:
             print("Response in progress please wait...")
             videoId = r["data"]["videoId"]
             r = Video.interface.send_request(
                 rtype=RequestTypes.GET, route="video", path_parameters=videoId
             )
             retries += 1
         return Video.Item(r)
 
     @staticmethod
     def create_from_production_and_video(
         productionId: str = "",
         productionItem: Optional[Any] = None,
         videoFileId: str = "",
-        format: str = "",
         mode: dict = {},
         public: bool = False,
     ) -> Item:
         if productionId and productionItem:
             raise Exception(
                 "productionId or productionItem should be supplied not both"
             )
@@ -87,71 +86,67 @@
             if not isinstance(productionId, str):
                 raise Exception("supplied productionId should be a uuid string.")
         body = {
             "productionId": productionId,
             "public": public,
             "videoFileId": videoFileId,
             "mode": mode,
-            "format": format,
+            "format": "",
         }
         r = Video.interface.send_request(
             rtype=RequestTypes.POST, route="video", json=body
         )
         retries = 0
-        max_retries = 10
+        max_retries = 30
         while r["statusCode"] == 202 and retries < max_retries:
             print("Response in progress please wait...")
             videoId = r["data"]["videoId"]
             r = Video.interface.send_request(
                 rtype=RequestTypes.GET, route="video", path_parameters=videoId
             )
             retries += 1
         return Video.Item(r)
 
     @staticmethod
     def create_from_file_and_video(
         fileId: str = "",
         videoFileId: str = "",
         mode: dict = {},
-        public: bool = False,
-        format: str = "",
     ) -> Item:
         interface = RequestInterface(family="production")
 
         if fileId and not videoFileId:
             raise Exception(
                 "if videoFileId is supplied, fileId should be supplied as well"
             )
 
         body = {
             "fileId": fileId,
             "videoFileId": videoFileId,
-            "public": public,
-            "outputFormat": format,
+            "public": False,
+            "outputFormat": "",
             "mode": mode,
         }
 
         r = interface.send_request(
             rtype=RequestTypes.POST, route="suite/file_to_video", json=body
         )
 
         item = Suite.PipelineInProgressItem(r)
         return Video.Item(_poll_video(r, item.pipelineId))
 
     @staticmethod
-    def create_from_file_and_image(
-        fileId: str = "", mode: dict = {}, public: bool = False, format: str = ""
-    ) -> Item:
+    def create_from_file_and_image(fileId: str = "") -> Item:
         interface = RequestInterface(family="production")
 
         body = {
             "fileId": fileId,
-            "public": public,
-            "outputFormat": format,
-            "mode": mode,
+            "public": False,
+            "outputFormat": "mp4",
+            "mode": {"setting": "default"},
         }
 
         r = interface.send_request(
             rtype=RequestTypes.POST, route="suite/file_to_video", json=body
         )
 
         item = Suite.PipelineInProgressItem(r)
```

### Comparing `audiostack-2.0.1/audiostack/docs/docs.py` & `audiostack-2.0.2/audiostack/docs/docs.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/helpers/api_item.py` & `audiostack-2.0.2/audiostack/helpers/api_item.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/helpers/api_list.py` & `audiostack-2.0.2/audiostack/helpers/api_list.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/helpers/request_interface.py` & `audiostack-2.0.2/audiostack/helpers/request_interface.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/production/mix.py` & `audiostack-2.0.2/audiostack/production/mix.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/production/sound.py` & `audiostack-2.0.2/audiostack/production/sound.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/production/suite.py` & `audiostack-2.0.2/audiostack/production/suite.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/speech/diction.py` & `audiostack-2.0.2/audiostack/speech/diction.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/speech/predict.py` & `audiostack-2.0.2/audiostack/speech/predict.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/speech/tts.py` & `audiostack-2.0.2/audiostack/speech/tts.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/speech/voice.py` & `audiostack-2.0.2/audiostack/speech/voice.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/tests/content/test_file.py` & `audiostack-2.0.2/audiostack/tests/content/test_file.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/tests/content/test_folder.py` & `audiostack-2.0.2/audiostack/tests/content/test_folder.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/tests/content/test_recommend.py` & `audiostack-2.0.2/audiostack/tests/content/test_recommend.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/tests/content/test_transfer.py` & `audiostack-2.0.2/audiostack/tests/content/test_transfer.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/tests/helpers/test_request_interface.py` & `audiostack-2.0.2/audiostack/tests/helpers/test_request_interface.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/tests/production/test_suite.py` & `audiostack-2.0.2/audiostack/tests/production/test_suite.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/tests/production/test_video.py` & `audiostack-2.0.2/audiostack/tests/production/test_video.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,41 +37,36 @@
 def test_create_from_production_and_video() -> None:
     script = audiostack.Content.Script.create(scriptText="hello lars")
     speech = audiostack.Speech.TTS.create(scriptItem=script, voice="sara")
     mix = audiostack.Production.Mix.create(speechItem=speech)
 
     videoFileId = FILE_IDS["video"]
     mode = {"setting": "low"}
-    format = "mp4"
 
     video = Video.create_from_production_and_video(
         productionItem=mix,
         videoFileId=videoFileId,
         public=True,
-        format=format,
         mode=mode,
     )
     print(video)
     assert video.status_code == 200, "Video from production and video Failed"
 
 
 def test_create_from_file_and_video() -> None:
     fileId = FILE_IDS["audio"]
     videoFileId = FILE_IDS["video"]
     mode = {"setting": "low"}
-    format = "mp4"
 
     video = Video.create_from_file_and_video(
-        fileId=fileId, videoFileId=videoFileId, mode=mode, format=format, public=False
+        fileId=fileId, videoFileId=videoFileId, mode=mode
     )
     print(video)
     assert video.status_code == 200, "Video from file and video Failed"
 
 
 def test_create_from_file_and_image() -> None:
     fileId = FILE_IDS["audio"]
-    mode = {"setting": "default"}
-    format = "mp4"
 
-    video = Video.create_from_file_and_image(fileId=fileId, mode=mode, format=format)
+    video = Video.create_from_file_and_image(fileId=fileId)
     print(video)
     assert video.status_code == 200, "Video from file and image"
```

### Comparing `audiostack-2.0.1/audiostack/tests/test_script.py` & `audiostack-2.0.2/audiostack/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/tests/tts/test_lexi.py` & `audiostack-2.0.2/audiostack/tests/tts/test_lexi.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/audiostack/tests/tts/test_predict.py` & `audiostack-2.0.2/audiostack/tests/tts/test_predict.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.1/pyproject.toml` & `audiostack-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "audiostack"
-version = "2.0.1"
+version = "2.0.2"
 description = "Python SDK for Audiostack API"
 authors = ["Aflorithmic <support@audiostack.ai>"]
 repository = "https://github.com/aflorithmic/audiostack-python"
 readme = "README.md"
 classifiers = [
    "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `audiostack-2.0.1/PKG-INFO` & `audiostack-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostack
-Version: 2.0.1
+Version: 2.0.2
 Summary: Python SDK for Audiostack API
 Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic
 Author-email: support@audiostack.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: audiostack Version: 2.0.1 Summary: Python SDK for
+Metadata-Version: 2.1 Name: audiostack Version: 2.0.2 Summary: Python SDK for
 Audiostack API Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic Author-email: support@audiostack.ai Requires-Python:
 >=3.8.1,<4.0.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: requests
```

