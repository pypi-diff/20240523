# Comparing `tmp/interactions-lavalink-2.0.0.tar.gz` & `tmp/interactions_lavalink-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interactions-lavalink-2.0.0.tar", last modified: Thu May 18 14:59:55 2023, max compression
+gzip compressed data, was "interactions_lavalink-3.0.0.tar", last modified: Thu May 23 10:20:39 2024, max compression
```

## Comparing `interactions-lavalink-2.0.0.tar` & `interactions_lavalink-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:59:55.198724 interactions-lavalink-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 14:59:44.000000 interactions-lavalink-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-18 14:59:44.000000 interactions-lavalink-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-18 14:59:55.198724 interactions-lavalink-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-18 14:59:44.000000 interactions-lavalink-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:59:55.194724 interactions-lavalink-2.0.0/interactions_lavalink/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-18 14:59:44.000000 interactions-lavalink-2.0.0/interactions_lavalink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-18 14:59:44.000000 interactions-lavalink-2.0.0/interactions_lavalink/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-05-18 14:59:44.000000 interactions-lavalink-2.0.0/interactions_lavalink/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-18 14:59:44.000000 interactions-lavalink-2.0.0/interactions_lavalink/player.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:59:55.198724 interactions-lavalink-2.0.0/interactions_lavalink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-18 14:59:55.000000 interactions-lavalink-2.0.0/interactions_lavalink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-18 14:59:55.000000 interactions-lavalink-2.0.0/interactions_lavalink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 14:59:55.000000 interactions-lavalink-2.0.0/interactions_lavalink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-18 14:59:55.000000 interactions-lavalink-2.0.0/interactions_lavalink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 14:59:55.000000 interactions-lavalink-2.0.0/interactions_lavalink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-18 14:59:44.000000 interactions-lavalink-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 14:59:55.198724 interactions-lavalink-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-18 14:59:44.000000 interactions-lavalink-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:20:39.770024 interactions_lavalink-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 10:20:35.000000 interactions_lavalink-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-23 10:20:35.000000 interactions_lavalink-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-23 10:20:39.770024 interactions_lavalink-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-23 10:20:35.000000 interactions_lavalink-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:20:39.766024 interactions_lavalink-3.0.0/interactions_lavalink/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-23 10:20:35.000000 interactions_lavalink-3.0.0/interactions_lavalink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-23 10:20:35.000000 interactions_lavalink-3.0.0/interactions_lavalink/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-23 10:20:35.000000 interactions_lavalink-3.0.0/interactions_lavalink/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-23 10:20:35.000000 interactions_lavalink-3.0.0/interactions_lavalink/player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:20:39.770024 interactions_lavalink-3.0.0/interactions_lavalink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-23 10:20:39.000000 interactions_lavalink-3.0.0/interactions_lavalink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-23 10:20:39.000000 interactions_lavalink-3.0.0/interactions_lavalink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:20:39.000000 interactions_lavalink-3.0.0/interactions_lavalink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 10:20:39.000000 interactions_lavalink-3.0.0/interactions_lavalink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-23 10:20:39.000000 interactions_lavalink-3.0.0/interactions_lavalink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-23 10:20:35.000000 interactions_lavalink-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 10:20:39.770024 interactions_lavalink-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-23 10:20:35.000000 interactions_lavalink-3.0.0/setup.py
```

### Comparing `interactions-lavalink-2.0.0/LICENSE` & `interactions_lavalink-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `interactions-lavalink-2.0.0/PKG-INFO` & `interactions_lavalink-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interactions-lavalink
-Version: 2.0.0
+Version: 3.0.0
 Summary: Lavalink support for interactions.py
 Home-page: https://github.com/interactions-py/lavalink
 Author: Damego
 Author-email: damego.dev@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,16 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: interactions.py<6.0.0,>=5.0.0
+Requires-Dist: lavalink<6.0.0,>=5.0.0
 
 # interactions-lavalink
 
 ## Installation
 
 Download ext via `pip install --upgrade interactions-lavalink`
```

### Comparing `interactions-lavalink-2.0.0/README.md` & `interactions_lavalink-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `interactions-lavalink-2.0.0/interactions_lavalink/events.py` & `interactions_lavalink-3.0.0/interactions_lavalink/events.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import attrs
 from interactions.api.events.base import BaseEvent
 from lavalink.events import (
     Event,
+    IncomingWebSocketMessage,
     NodeChangedEvent,
     NodeConnectedEvent,
+    NodeReadyEvent,
     NodeDisconnectedEvent,
     PlayerUpdateEvent,
     QueueEndEvent,
     TrackEndEvent,
     TrackExceptionEvent,
     TrackLoadFailedEvent,
     TrackStartEvent,
@@ -33,14 +35,18 @@
 @attrs.define(eq=False, order=False, hash=False, slots=False, kw_only=False)
 class CursedLavalinkEvent(BaseEvent):
     lavalink_event: Event = attrs.field(repr=False)
 
     def __getattr__(self, name: str):
         return getattr(self.lavalink_event, name)
 
+@attrs.define(eq=False, order=False, hash=False, slots=False, kw_only=False)
+class IncomingWebSocketMessage(CursedLavalinkEvent, IncomingWebSocketMessage):
+    ...
+
 
 @attrs.define(eq=False, order=False, hash=False, slots=False, kw_only=False)
 class TrackStart(CursedLavalinkEvent, TrackStartEvent):
     ...
 
 
 @attrs.define(eq=False, order=False, hash=False, slots=False, kw_only=False)
@@ -73,14 +79,18 @@
     ...
 
 
 @attrs.define(eq=False, order=False, hash=False, slots=False, kw_only=False)
 class NodeConnected(CursedLavalinkEvent, NodeConnectedEvent):
     ...
 
+@attrs.define(eq=False, order=False, hash=False, slots=False, kw_only=False)
+class NodeReady(CursedLavalinkEvent, NodeReadyEvent):
+    ...
+
 
 @attrs.define(eq=False, order=False, hash=False, slots=False, kw_only=False)
 class NodeDisconnected(CursedLavalinkEvent, NodeDisconnectedEvent):
     ...
 
 
 @attrs.define(eq=False, order=False, hash=False, slots=False, kw_only=False)
```

### Comparing `interactions-lavalink-2.0.0/interactions_lavalink/extension.py` & `interactions_lavalink-3.0.0/interactions_lavalink/extension.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,34 +26,26 @@
 
     def add_node(
         self,
         host: str,
         port: int,
         password: str,
         region: str,
-        resume_key: str = None,
-        resume_timeout: int = 60,
         name: str = None,
-        reconnect_attempts: int = 3,
-        filters: bool = True,
         ssl: bool = False,
     ):
         if self.client is None:
             self.__init_lavalink()
 
         return self.client.add_node(
             host=host,
             port=port,
             password=password,
             region=region,
-            resume_key=resume_key,
-            resume_timeout=resume_timeout,
             name=name,
-            reconnect_attempts=reconnect_attempts,
-            filters=filters,
             ssl=ssl,
         )
 
     def __init_lavalink(self):
         self.client = LavalinkClient(int(self._bot.user.id), player=Player)
         self.client.add_event_hook(self._dispatch_lavalink_event)
```

### Comparing `interactions-lavalink-2.0.0/interactions_lavalink/player.py` & `interactions_lavalink-3.0.0/interactions_lavalink/player.py`

 * *Files identical despite different names*

### Comparing `interactions-lavalink-2.0.0/interactions_lavalink.egg-info/PKG-INFO` & `interactions_lavalink-3.0.0/interactions_lavalink.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interactions-lavalink
-Version: 2.0.0
+Version: 3.0.0
 Summary: Lavalink support for interactions.py
 Home-page: https://github.com/interactions-py/lavalink
 Author: Damego
 Author-email: damego.dev@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,16 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: interactions.py<6.0.0,>=5.0.0
+Requires-Dist: lavalink<6.0.0,>=5.0.0
 
 # interactions-lavalink
 
 ## Installation
 
 Download ext via `pip install --upgrade interactions-lavalink`
```

### Comparing `interactions-lavalink-2.0.0/pyproject.toml` & `interactions_lavalink-3.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 [tool.isort]
 profile = "black"
 line_length = 100
 
 [tool.poetry]
 name = "interactions-lavalink"
-version = "2.0.0"
+version = "3.0.0"
 description = "Lavalink support for interactions.py"
 authors = ["Damego <damego.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "interactions_lavalink"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 tomli = "^2.0.1"
-lavalink = "^4.0.0"
+lavalink = "^5.0.0"
 interactions-py = "^5.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.0.4"
 
 [build-system]
 requires = [
```

### Comparing `interactions-lavalink-2.0.0/setup.py` & `interactions_lavalink-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 setup(
     name=pyproject["tool"]["poetry"]["name"],
     version=pyproject["tool"]["poetry"]["version"],
     author="Damego",
     author_email="damego.dev@gmail.com",
     description=pyproject["tool"]["poetry"]["description"],
     include_package_data=True,
-    install_requires=["interactions.py>=5.0.0,<6.0.0", "lavalink>=4.0.0,<5.0.0"],
+    install_requires=["interactions.py>=5.0.0,<6.0.0", "lavalink>=5.0.0,<6.0.0"],
     license=pyproject["tool"]["poetry"]["license"],
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/interactions-py/lavalink",
     packages=find_packages(),
     python_requires=">=3.10",
     classifiers=[
```

