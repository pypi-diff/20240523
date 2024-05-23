# Comparing `tmp/livekit_plugins_elevenlabs-0.4.dev2.tar.gz` & `tmp/livekit_plugins_elevenlabs-0.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit_plugins_elevenlabs-0.4.dev2.tar", last modified: Sun May  5 16:56:20 2024, max compression
+gzip compressed data, was "livekit_plugins_elevenlabs-0.5.dev0.tar", last modified: Thu May 23 15:59:15 2024, max compression
```

## Comparing `livekit_plugins_elevenlabs-0.4.dev2.tar` & `livekit_plugins_elevenlabs-0.5.dev0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:56:20.065905 livekit_plugins_elevenlabs-0.4.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-05 16:56:20.065905 livekit_plugins_elevenlabs-0.4.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-05 16:56:16.000000 livekit_plugins_elevenlabs-0.4.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:56:20.061905 livekit_plugins_elevenlabs-0.4.dev2/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:56:20.061905 livekit_plugins_elevenlabs-0.4.dev2/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:56:20.061905 livekit_plugins_elevenlabs-0.4.dev2/livekit/plugins/elevenlabs/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-05 16:56:16.000000 livekit_plugins_elevenlabs-0.4.dev2/livekit/plugins/elevenlabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-05 16:56:16.000000 livekit_plugins_elevenlabs-0.4.dev2/livekit/plugins/elevenlabs/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-05 16:56:16.000000 livekit_plugins_elevenlabs-0.4.dev2/livekit/plugins/elevenlabs/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 16:56:16.000000 livekit_plugins_elevenlabs-0.4.dev2/livekit/plugins/elevenlabs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-05-05 16:56:16.000000 livekit_plugins_elevenlabs-0.4.dev2/livekit/plugins/elevenlabs/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-05 16:56:16.000000 livekit_plugins_elevenlabs-0.4.dev2/livekit/plugins/elevenlabs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:56:20.065905 livekit_plugins_elevenlabs-0.4.dev2/livekit_plugins_elevenlabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-05 16:56:20.000000 livekit_plugins_elevenlabs-0.4.dev2/livekit_plugins_elevenlabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-05 16:56:20.000000 livekit_plugins_elevenlabs-0.4.dev2/livekit_plugins_elevenlabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 16:56:20.000000 livekit_plugins_elevenlabs-0.4.dev2/livekit_plugins_elevenlabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-05 16:56:20.000000 livekit_plugins_elevenlabs-0.4.dev2/livekit_plugins_elevenlabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-05 16:56:20.000000 livekit_plugins_elevenlabs-0.4.dev2/livekit_plugins_elevenlabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-05 16:56:16.000000 livekit_plugins_elevenlabs-0.4.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 16:56:20.065905 livekit_plugins_elevenlabs-0.4.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-05 16:56:16.000000 livekit_plugins_elevenlabs-0.4.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:15.325023 livekit_plugins_elevenlabs-0.5.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-23 15:59:15.321023 livekit_plugins_elevenlabs-0.5.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-23 15:59:11.000000 livekit_plugins_elevenlabs-0.5.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:15.321023 livekit_plugins_elevenlabs-0.5.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:15.321023 livekit_plugins_elevenlabs-0.5.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:15.321023 livekit_plugins_elevenlabs-0.5.dev0/livekit/plugins/elevenlabs/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-23 15:59:11.000000 livekit_plugins_elevenlabs-0.5.dev0/livekit/plugins/elevenlabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-23 15:59:11.000000 livekit_plugins_elevenlabs-0.5.dev0/livekit/plugins/elevenlabs/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 15:59:11.000000 livekit_plugins_elevenlabs-0.5.dev0/livekit/plugins/elevenlabs/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:11.000000 livekit_plugins_elevenlabs-0.5.dev0/livekit/plugins/elevenlabs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-05-23 15:59:11.000000 livekit_plugins_elevenlabs-0.5.dev0/livekit/plugins/elevenlabs/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-23 15:59:11.000000 livekit_plugins_elevenlabs-0.5.dev0/livekit/plugins/elevenlabs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:15.321023 livekit_plugins_elevenlabs-0.5.dev0/livekit_plugins_elevenlabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-23 15:59:15.000000 livekit_plugins_elevenlabs-0.5.dev0/livekit_plugins_elevenlabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-23 15:59:15.000000 livekit_plugins_elevenlabs-0.5.dev0/livekit_plugins_elevenlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:59:15.000000 livekit_plugins_elevenlabs-0.5.dev0/livekit_plugins_elevenlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-23 15:59:15.000000 livekit_plugins_elevenlabs-0.5.dev0/livekit_plugins_elevenlabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 15:59:15.000000 livekit_plugins_elevenlabs-0.5.dev0/livekit_plugins_elevenlabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 15:59:11.000000 livekit_plugins_elevenlabs-0.5.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:59:15.325023 livekit_plugins_elevenlabs-0.5.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-23 15:59:11.000000 livekit_plugins_elevenlabs-0.5.dev0/setup.py
```

### Comparing `livekit_plugins_elevenlabs-0.4.dev2/PKG-INFO` & `livekit_plugins_elevenlabs-0.5.dev0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-elevenlabs
-Version: 0.4.dev2
+Version: 0.5.dev0
 Summary: Agent Framework plugin for voice synthesis with ElevenLabs' API.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,elevenlabs
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
 Requires-Dist: aiohttp>=3.8.5
 
 # LiveKit Plugins Elevenlabs
 
 Agent Framework plugin for voice synthesis with [ElevenLabs](https://elevenlabs.io/) API.
 
 ## Installation
```

### Comparing `livekit_plugins_elevenlabs-0.4.dev2/livekit/plugins/elevenlabs/__init__.py` & `livekit_plugins_elevenlabs-0.5.dev0/livekit/plugins/elevenlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_elevenlabs-0.4.dev2/livekit/plugins/elevenlabs/version.py` & `livekit_plugins_elevenlabs-0.5.dev0/livekit/plugins/elevenlabs/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.4.dev2"
+__version__ = "0.5.dev0"
```

### Comparing `livekit_plugins_elevenlabs-0.4.dev2/livekit_plugins_elevenlabs.egg-info/PKG-INFO` & `livekit_plugins_elevenlabs-0.5.dev0/livekit_plugins_elevenlabs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-elevenlabs
-Version: 0.4.dev2
+Version: 0.5.dev0
 Summary: Agent Framework plugin for voice synthesis with ElevenLabs' API.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,elevenlabs
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
 Requires-Dist: aiohttp>=3.8.5
 
 # LiveKit Plugins Elevenlabs
 
 Agent Framework plugin for voice synthesis with [ElevenLabs](https://elevenlabs.io/) API.
 
 ## Installation
```

### Comparing `livekit_plugins_elevenlabs-0.4.dev2/setup.py` & `livekit_plugins_elevenlabs-0.5.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     ],
     keywords=["webrtc", "realtime", "audio", "video", "livekit", "elevenlabs"],
     license="Apache-2.0",
     packages=setuptools.find_namespace_packages(include=["livekit.*"]),
     python_requires=">=3.9.0",
     install_requires=[
         "livekit ~= 0.11",
-        "livekit-agents~=0.6.dev1",
+        "livekit-agents~=0.7.dev0",
         "aiohttp >= 3.8.5",
     ],
     package_data={
         "livekit.plugins.elevenlabs": ["py.typed"],
     },
     project_urls={
         "Documentation": "https://docs.livekit.io",
```

