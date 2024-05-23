# Comparing `tmp/silero-vad-0.0.3.tar.gz` & `tmp/silero-vad-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silero-vad-0.0.3.tar", last modified: Mon Apr 29 06:11:54 2024, max compression
+gzip compressed data, was "silero-vad-0.0.4.tar", last modified: Thu May 23 15:10:02 2024, max compression
```

## Comparing `silero-vad-0.0.3.tar` & `silero-vad-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:11:54.728680 silero-vad-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-29 06:11:50.000000 silero-vad-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-29 06:11:50.000000 silero-vad-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-29 06:11:54.728680 silero-vad-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-29 06:11:50.000000 silero-vad-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 06:11:51.000000 silero-vad-0.0.3/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-29 06:11:50.000000 silero-vad-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 06:11:54.728680 silero-vad-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-29 06:11:50.000000 silero-vad-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:11:54.728680 silero-vad-0.0.3/silero_vad/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-29 06:11:50.000000 silero-vad-0.0.3/silero_vad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-29 06:11:50.000000 silero-vad-0.0.3/silero_vad/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-29 06:11:50.000000 silero-vad-0.0.3/silero_vad/frame_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-29 06:11:50.000000 silero-vad-0.0.3/silero_vad/inference_session.py
--rw-r--r--   0 runner    (1001) docker     (127)  1807522 2024-04-29 06:11:50.000000 silero-vad-0.0.3/silero_vad/silero_vad.onnx
--rw-r--r--   0 runner    (1001) docker     (127)    14435 2024-04-29 06:11:50.000000 silero-vad-0.0.3/silero_vad/silero_vad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-29 06:11:50.000000 silero-vad-0.0.3/silero_vad/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:11:54.728680 silero-vad-0.0.3/silero_vad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-29 06:11:54.000000 silero-vad-0.0.3/silero_vad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-29 06:11:54.000000 silero-vad-0.0.3/silero_vad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 06:11:54.000000 silero-vad-0.0.3/silero_vad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-29 06:11:54.000000 silero-vad-0.0.3/silero_vad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-29 06:11:54.000000 silero-vad-0.0.3/silero_vad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 06:11:54.000000 silero-vad-0.0.3/silero_vad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:10:02.065923 silero-vad-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-23 15:10:01.000000 silero-vad-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-23 15:10:01.000000 silero-vad-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-23 15:10:02.065923 silero-vad-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-23 15:10:01.000000 silero-vad-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 15:10:01.000000 silero-vad-0.0.4/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 15:10:01.000000 silero-vad-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:10:02.065923 silero-vad-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-23 15:10:01.000000 silero-vad-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:10:02.065923 silero-vad-0.0.4/silero_vad/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-23 15:10:01.000000 silero-vad-0.0.4/silero_vad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-23 15:10:01.000000 silero-vad-0.0.4/silero_vad/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-23 15:10:01.000000 silero-vad-0.0.4/silero_vad/frame_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-23 15:10:01.000000 silero-vad-0.0.4/silero_vad/inference_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1807522 2024-05-23 15:10:01.000000 silero-vad-0.0.4/silero_vad/silero_vad.onnx
+-rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-23 15:10:01.000000 silero-vad-0.0.4/silero_vad/silero_vad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-23 15:10:01.000000 silero-vad-0.0.4/silero_vad/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:10:02.065923 silero-vad-0.0.4/silero_vad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-23 15:10:02.000000 silero-vad-0.0.4/silero_vad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-23 15:10:02.000000 silero-vad-0.0.4/silero_vad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:10:02.000000 silero-vad-0.0.4/silero_vad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 15:10:02.000000 silero-vad-0.0.4/silero_vad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 15:10:02.000000 silero-vad-0.0.4/silero_vad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 15:10:02.000000 silero-vad-0.0.4/silero_vad.egg-info/top_level.txt
```

### Comparing `silero-vad-0.0.3/LICENSE` & `silero-vad-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.3/PKG-INFO` & `silero-vad-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silero-vad
-Version: 0.0.3
+Version: 0.0.4
 Summary: Silero VAD
 Home-page: https://github.com/pengzhendong/silero-vad
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `silero-vad-0.0.3/setup.py` & `silero-vad-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.3/silero_vad/__init__.py` & `silero-vad-0.0.4/silero_vad/__init__.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.3/silero_vad/cli.py` & `silero-vad-0.0.4/silero_vad/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,18 @@
             out_wav.setnchannels(1)
             out_wav.setsampwidth(2)
             out_wav.setframerate(sr)
         # number of samples in a single audio chunk
         window_size_samples = 10 * sr // 1000
         for i in range(0, len(wav), window_size_samples):
             chunk = wav[i : i + window_size_samples]
-            for speech_dict, speech_samples in vad_iterator(chunk, return_seconds=True):
+            last = len(chunk) < window_size_samples
+            for speech_dict, speech_samples in vad_iterator(
+                chunk, last, return_seconds=True
+            ):
                 if speech_dict:
                     print(speech_dict, end=" ")
                 if save_path and speech_samples is not None:
                     out_wav.writeframes((speech_samples * 32768).astype(np.int16))
         # reset model states after each audio
         vad_iterator.reset_states()
```

### Comparing `silero-vad-0.0.3/silero_vad/frame_queue.py` & `silero-vad-0.0.4/silero_vad/frame_queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         if src_sr == dst_sr or dst_sr is None:
             self.step = 1.0
             self.resampler = None
             self.frame_size = frame_size_ms * src_sr // 1000
         else:
             self.step = src_sr / dst_sr
             self.frame_size = frame_size_ms * dst_sr // 1000
-            self.resampler = soxr.ResampleStream(src_sr, dst_sr, 1, dtype=np.float32)
+            self.resampler = soxr.ResampleStream(src_sr, dst_sr, 1)
 
     def add_chunk(self, chunk, last=False):
         # cache
         if self.cached_ms > 0:
             self.cache_start += len(chunk)
             self.cached_samples = np.roll(self.cached_samples, -len(chunk))
             self.cached_samples[-len(chunk) :] = chunk[-len(self.cached_samples) :]
```

### Comparing `silero-vad-0.0.3/silero_vad/inference_session.py` & `silero-vad-0.0.4/silero_vad/inference_session.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.3/silero_vad/silero_vad.onnx` & `silero-vad-0.0.4/silero_vad/silero_vad.onnx`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.3/silero_vad/silero_vad.py` & `silero-vad-0.0.4/silero_vad/silero_vad.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import math
 import os
+import warnings
 from functools import partial
 from pathlib import Path
 from typing import Union
-import warnings
 
 import numpy as np
 import soundfile as sf
+from tqdm import tqdm
 
 from .frame_queue import FrameQueue
 from .inference_session import PickableInferenceSession
 from .utils import get_energy
 
 
 class SileroVAD:
@@ -65,20 +67,20 @@
 
         speech_pad_samples = speech_pad_ms * sample_rate // 1000
         segment["start"] = max(segment["start"] - speech_pad_samples, 0)
         segment["end"] = min(segment["end"] + speech_pad_samples, len(wav))
         if save_path:
             wav = wav[segment["start"] : segment["end"]]
             if flat_layout:
-                sf.write(str(save_path) + f"_{idx:04d}.wav", wav, sample_rate)
+                sf.write(str(save_path) + f"_{idx:05d}.wav", wav, sample_rate)
             else:
                 save_path = Path(save_path)
                 if not save_path.exists():
                     save_path.mkdir(parents=True, exist_ok=True)
-                sf.write(str(save_path / f"{idx:04d}.wav"), wav, sample_rate)
+                sf.write(str(save_path / f"{idx:05d}.wav"), wav, sample_rate)
         if return_seconds:
             segment["start"] = round(segment["start"] / sample_rate, 3)
             segment["end"] = round(segment["end"] / sample_rate, 3)
         return segment
 
     def get_speech_timestamps(
         self,
@@ -133,20 +135,27 @@
         ----------
         speeches: list of dicts
             list containing ends and beginnings of speech chunks (samples or seconds
             based on return_seconds)
         """
 
         wav, sr = sf.read(Path(wav_path), dtype=np.float32)
+        dur_ms = len(wav) * 1000 / sr
         if len(wav.shape) > 1:
             raise ValueError("Only supported mono wav.")
-        if len(wav) / sr * 1000 < 32:
+        if dur_ms < 32:
             raise ValueError("Input audio is too short.")
         if window_size_ms not in [32, 64, 96]:
             warnings.warn("Supported window_size_ms: [32, 64, 96]")
+        progress_bar = tqdm(
+            total=math.ceil(dur_ms / window_size_ms),
+            desc="VAD processing",
+            unit="frames",
+            bar_format="{l_bar}{bar}{r_bar} | {percentage:.2f}%",
+        )
 
         if sr in self.sample_rates:
             vad_sr = sr
             queue = FrameQueue(window_size_ms, sr)
         else:
             vad_sr = 16000
             queue = FrameQueue(window_size_ms, src_sr=sr, dst_sr=vad_sr)
@@ -175,15 +184,16 @@
         neg_threshold = threshold - 0.15
         triggered = False
         # to save potential segment end (and tolerate some silence)
         temp_end = 0
         # to save potential segment limits in case of maximum segment size reached
         prev_end = 0
         next_start = 0
-        for frame_start, frame_end, frame in queue.add_chunk(wav):
+        for frame_start, frame_end, frame in queue.add_chunk(wav, True):
+            progress_bar.update(1)
             speech_prob = self(frame, vad_sr)
             # current frame is speech
             if speech_prob >= threshold:
                 if temp_end > 0 and next_start < prev_end:
                     next_start = frame_end
                 temp_end = 0
                 if not triggered:
@@ -303,25 +313,27 @@
 
     def reset_states(self):
         self.model.reset_states()
         self.triggered = False
         self.temp_end = 0
         self.queue.clear()
 
-    def __call__(self, chunk, use_energy=False, return_seconds=False):
+    def __call__(self, chunk, last=False, use_energy=False, return_seconds=False):
         """
         chunk: audio chunk
 
+        last: bool (default - False)
+            whether is the last audio chunk
         use_energy: bool (default - False)
             whether to use harmonic energy to suppress background vocals
         return_seconds: bool (default - False)
             whether return timestamps in seconds (default - samples)
         """
 
-        for frame_start, frame_end, frame in self.queue.add_chunk(chunk):
+        for frame_start, frame_end, frame in self.queue.add_chunk(chunk, last):
             speech_prob = self.model(frame, self.vad_sr)
             # Suppress background vocals by harmonic energy
             if use_energy:
                 energy = get_energy(frame, self.vad_sr, from_harmonic=4)
                 if speech_prob < 0.9 and energy < 500 * (1 - speech_prob):
                     speech_prob = 0
```

### Comparing `silero-vad-0.0.3/silero_vad/utils.py` & `silero-vad-0.0.4/silero_vad/utils.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.3/silero_vad.egg-info/PKG-INFO` & `silero-vad-0.0.4/silero_vad.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silero-vad
-Version: 0.0.3
+Version: 0.0.4
 Summary: Silero VAD
 Home-page: https://github.com/pengzhendong/silero-vad
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

