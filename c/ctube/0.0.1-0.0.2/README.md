# Comparing `tmp/ctube-0.0.1.tar.gz` & `tmp/ctube-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctube-0.0.1.tar", max compression
+gzip compressed data, was "ctube-0.0.2.tar", max compression
```

## Comparing `ctube-0.0.1.tar` & `ctube-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1058 2024-05-21 18:00:19.544353 ctube-0.0.1/LICENSE
--rw-r--r--   0        0        0        8 2024-05-21 18:12:37.447875 ctube-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-05-21 18:10:22.007715 ctube-0.0.1/ctube/__init__.py
--rw-r--r--   0        0        0     9115 2024-05-21 18:08:00.247958 ctube-0.0.1/ctube/app.py
--rw-r--r--   0        0        0      486 2024-05-21 18:08:14.988229 ctube-0.0.1/ctube/cli.py
--rw-r--r--   0        0        0      348 2024-05-20 21:16:10.094478 ctube-0.0.1/ctube/colors.py
--rw-r--r--   0        0        0      506 2024-05-21 18:08:23.355057 ctube-0.0.1/ctube/config.py
--rw-r--r--   0        0        0      397 2024-05-20 21:34:33.134572 ctube-0.0.1/ctube/containers.py
--rw-r--r--   0        0        0     1252 2024-05-21 18:08:31.471884 ctube-0.0.1/ctube/decorators.py
--rw-r--r--   0        0        0     3926 2024-05-21 18:08:38.065350 ctube-0.0.1/ctube/download.py
--rw-r--r--   0        0        0      173 2024-05-21 18:08:51.782302 ctube-0.0.1/ctube/errors.py
--rw-r--r--   0        0        0     1722 2024-05-21 18:08:57.179084 ctube-0.0.1/ctube/extractors.py
--rw-r--r--   0        0        0      247 2024-05-21 18:00:19.574354 ctube-0.0.1/ctube/paths.py
--rw-r--r--   0        0        0     1981 2024-05-21 18:09:01.955854 ctube-0.0.1/ctube/terminal.py
--rw-r--r--   0        0        0      602 2024-05-21 18:19:38.669566 ctube-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 ctube-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-05-21 18:00:19.544353 ctube-0.0.2/LICENSE
+-rw-r--r--   0        0        0        8 2024-05-21 18:12:37.447875 ctube-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-21 18:10:22.007715 ctube-0.0.2/ctube/__init__.py
+-rw-r--r--   0        0        0     6703 2024-05-21 22:28:30.102105 ctube-0.0.2/ctube/app.py
+-rw-r--r--   0        0        0      511 2024-05-21 22:28:30.102105 ctube-0.0.2/ctube/cli.py
+-rw-r--r--   0        0        0     2004 2024-05-21 20:56:10.230755 ctube-0.0.2/ctube/cmds.py
+-rw-r--r--   0        0        0      658 2024-05-21 21:21:21.916025 ctube-0.0.2/ctube/colors.py
+-rw-r--r--   0        0        0      397 2024-05-20 21:34:33.134572 ctube-0.0.2/ctube/containers.py
+-rw-r--r--   0        0        0     1364 2024-05-21 22:28:30.102105 ctube-0.0.2/ctube/decorators.py
+-rw-r--r--   0        0        0     4172 2024-05-21 21:47:45.472668 ctube-0.0.2/ctube/download.py
+-rw-r--r--   0        0        0      325 2024-05-21 21:08:14.245466 ctube-0.0.2/ctube/errors.py
+-rw-r--r--   0        0        0     1722 2024-05-21 18:08:57.179084 ctube-0.0.2/ctube/extractors.py
+-rw-r--r--   0        0        0     2885 2024-05-21 22:00:49.146238 ctube-0.0.2/ctube/helpers.py
+-rw-r--r--   0        0        0      247 2024-05-21 18:00:19.574354 ctube-0.0.2/ctube/paths.py
+-rw-r--r--   0        0        0     1903 2024-05-21 22:28:30.102105 ctube-0.0.2/ctube/printers.py
+-rw-r--r--   0        0        0     2068 2024-05-21 21:41:27.800799 ctube-0.0.2/ctube/terminal.py
+-rw-r--r--   0        0        0      622 2024-05-23 07:36:38.694868 ctube-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 ctube-0.0.2/PKG-INFO
```

### Comparing `ctube-0.0.1/LICENSE` & `ctube-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ctube-0.0.1/ctube/decorators.py` & `ctube-0.0.2/ctube/decorators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,12 @@
-from signal import signal, SIGINT
 from typing import Callable, Any
+from signal import signal, SIGINT
+from ctube.cmds import Commands
 from ctube.colors import Color, color
-from ctube.errors import InvalidSyntax, InvalidIndexSyntax
-
-
-def handle_main_function(func: Callable) -> Callable:
-    def inner(*args, **kwargs) -> None:
-        signal(SIGINT, lambda signum, _: exit())
-        try:
-            func(*args, **kwargs)
-        except Exception as error:
-            print(color(str(error), Color.RED))
-            raise
-        exit()
-    return inner
-
-
-def handle_invalid_syntax(func: Callable) -> Callable:
-    def inner(*args, **kwargs) -> None:
-        try:
-            return func(*args, **kwargs)
-        except InvalidSyntax:
-            print(color("Invalid syntax", Color.RED))
-    return inner
+from ctube.errors import InvalidIndexSyntax
 
 
 def handle_invalid_index_syntax(func: Callable) -> Callable:
     def inner(*args, **kwargs) -> None:
         try:
             return func(*args, **kwargs)
         except InvalidIndexSyntax:
@@ -37,7 +17,23 @@
 def handle_extraction(func: Callable) -> Callable:
     def inner(*args, **kwargs) -> Any:
         try:
             return func(*args, **kwargs)
         except (KeyError, IndexError, TypeError, ValueError):
             pass
     return inner
+
+
+def handle_invalid_cmd_args(cmd: Commands) -> Callable:
+    accepted_args = cmd.value.accepted_args
+    if not accepted_args:
+        raise ValueError("Invalid usage")
+    def wrapper(func: Callable) -> Callable:
+        def inner(*cmd_args: str) -> Any:
+            invalid_args = {cmd_arg for cmd_arg in cmd_args[1:] if cmd_arg not in accepted_args}
+            if invalid_args:
+                print(color(f"Invalid arguments for command '{cmd.value.name}': {invalid_args}", Color.RED))
+                print(color(f"Accepted arguments are {accepted_args}", Color.RED))
+            else:
+                return func(*cmd_args)
+        return inner
+    return wrapper
```

### Comparing `ctube-0.0.1/ctube/download.py` & `ctube-0.0.2/ctube/download.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
+from pathvalidate import sanitize_filename
 from enum import Enum
 from urllib import request
-from typing import Callable, Optional, List, Optional
+from typing import Callable, List
 from dataclasses import dataclass
 from ctube.containers import MusicItem
 from pytubefix import Playlist, Stream, YouTube
 from pytubefix.exceptions import (
         MembersOnly, 
         RecordingUnavailable, 
         VideoPrivate, 
@@ -51,34 +52,37 @@
             os.makedirs(output_path, exist_ok=True)
         if not os.path.isdir(output_path):
             raise NotADirectoryError
         if not os.access(path=output_path, mode=os.W_OK):
             raise NotADirectoryError
         self._output_path = output_path
 
-    def _on_complete_callback(self, data: Data, filepath: Optional[str]) -> None:
-        if filepath:
-            data.filepath = filepath
-            self.on_complete_callback(data)
-        else:
-            raise RuntimeError
+    def _on_complete_callback(self, data: Data, filepath: str) -> None:
+        data.filepath = filepath
+        self.on_complete_callback(data)
 
     def _on_progress_callback(self, data: Data, bytes_remaining: int, stream: Stream) -> None:
         filesize = stream.filesize
         bytes_received = filesize - bytes_remaining
         self.on_progress_callback(data, filesize, bytes_received)
 
     def download(self, item: MusicItem, artist: str) -> List[YouTube]:
         playlist = Playlist(url=f"{BaseURL.PLAYLIST.value}{item.playlist_id}")
         failed_downloads: List[YouTube] = []
 
         response = request.urlopen(item.thumbanail_url)
         image_data = response.read()
 
-        final_destination = os.path.join(os.path.join(self.output_path, artist), item.title)
+        final_destination = os.path.join(
+            os.path.join(
+                self.output_path, sanitize_filename(artist)
+            ), 
+            sanitize_filename(item.title)
+        )
+
         os.makedirs(final_destination, exist_ok=True)
 
         for i, url in enumerate(playlist):
             youtube = YouTube(url=url)
 
             try:
                 stream = youtube.streams
@@ -88,15 +92,15 @@
                     VideoPrivate, 
                     VideoUnavailable,
                     KeyError  # This is a bug in pytubefix I think.
             ):
                 failed_downloads.append(youtube)
                 continue
 
-            audio_stream = stream.get_audio_only()
+            audio_stream = stream.get_audio_only(subtype="mp4")
 
             if not audio_stream:
                 failed_downloads.append(youtube)
                 continue
 
             data = Data(
                 title=youtube.title,
@@ -110,15 +114,20 @@
 
             youtube.register_on_progress_callback(
                 lambda stream, _, bytes_remaining: self._on_progress_callback(
                     data, bytes_remaining, stream
                 )
             )
             youtube.register_on_complete_callback(
-                lambda _, filepath: self._on_complete_callback(data, filepath)
+                lambda _, filepath: self._on_complete_callback(
+                    data, 
+                    filepath  # type: ignore
+                    # pytubefix says that 'filepath' can be None, 
+                    # but this is not possible.
+                )
             )
 
             audio_stream.download(
                 output_path=final_destination,
                 skip_existing=self.skip_existing
             )
```

### Comparing `ctube-0.0.1/ctube/extractors.py` & `ctube-0.0.2/ctube/extractors.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.1/ctube/terminal.py` & `ctube-0.0.2/ctube/terminal.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import sys, tty, termios
 from typing import List, Optional
+from ctube.colors import Color, color
 
 
 class Prompt:
-    def __init__(self, prompt_char: str = ">"):
-        self.prompt_char = prompt_char
+    def __init__(self, char: str = "❯", color: Color = Color.GREEN):
+
+        self.char = char
+        self.color = color
 
     def get_input(self):
-        return input(f"{self.prompt_char} ")
+        return input(f"{color(self.char, self.color)} ")
 
 
 class Buffer:
     def __init__(self, infinite_scroll: bool = True):
         self.infinite_scroll = infinite_scroll
         self._index = 0
         self._buffer: List[str] = []
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ctube-0.0.1/pyproject.toml` & `ctube-0.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "ctube"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["Simone Gentili <gensydev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://pypi.org/project/ctube/"
 repository = "https://github.com/g3nsy/ctube"
 keywords = ["innertube", "youtube", "youtube-music", "python", "download", "music", "client"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydub = "^0.25.1"
 eyed3 = "^0.9.7"
 innertube = "^2.1.16"
 pytubefix = "^5.4.2"
+pathvalidate = "^3.2.0"
 
 [tool.poetry.scripts]
-my-script = "ctube.cli:main"
+ctube = "ctube.cli:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ctube-0.0.1/PKG-INFO` & `ctube-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctube
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Home-page: https://pypi.org/project/ctube/
 License: MIT
 Keywords: innertube,youtube,youtube-music,python,download,music,client
 Author: Simone Gentili
 Author-email: gensydev@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: eyed3 (>=0.9.7,<0.10.0)
 Requires-Dist: innertube (>=2.1.16,<3.0.0)
+Requires-Dist: pathvalidate (>=3.2.0,<4.0.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0)
 Requires-Dist: pytubefix (>=5.4.2,<6.0.0)
 Project-URL: Repository, https://github.com/g3nsy/ctube
 Description-Content-Type: text/markdown
 
 # ctube
```

