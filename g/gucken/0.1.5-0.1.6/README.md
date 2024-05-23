# Comparing `tmp/gucken-0.1.5.tar.gz` & `tmp/gucken-0.1.6.tar.gz`

## Comparing `gucken-0.1.5.tar` & `gucken-0.1.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/__main__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/aniskip.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/custom_widgets.py
--rw-r--r--   0        0        0    32791 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/gucken.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/rome.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/settings.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/update.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/hoster/__init__.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/hoster/_hosters.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/hoster/common.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/hoster/doodstream.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/hoster/streamtape.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/hoster/veo.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/hoster/vidoza.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/player/__init__.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/player/_players.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/player/android.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/player/common.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/player/ffplay.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/player/flatpak.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/player/mpv.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/player/vlc.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/player/wmplayer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/provider/__init__.py
--rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/provider/aniworld.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/provider/burningseries.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/provider/common.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/provider/crunchyroll.py
--rw-r--r--   0        0        0    10844 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/provider/serienstream.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/provider/streamcloud.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/resources/default_settings.toml
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/resources/gucken.css
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/resources/mpv_skip.lua
--rwxr-xr-x   0        0        0     3912 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/resources/vlc_skip.lua
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/tracker/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/tracker/anilist.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/tracker/aniworld.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/tracker/common.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/tracker/myanimelist.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.5/src/gucken/tracker/serienstream.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gucken-0.1.5/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gucken-0.1.5/LICENSE.txt
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 gucken-0.1.5/README.md
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 gucken-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 gucken-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/__main__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/aniskip.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/custom_widgets.py
+-rw-r--r--   0        0        0    32791 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/gucken.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/rome.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/settings.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/update.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/hoster/__init__.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/hoster/_hosters.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/hoster/common.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/hoster/doodstream.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/hoster/streamtape.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/hoster/veo.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/hoster/vidoza.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/player/__init__.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/player/_players.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/player/android.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/player/common.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/player/ffplay.py
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/player/flatpak.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/player/mpv.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/player/vlc.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/player/wmplayer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/provider/__init__.py
+-rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/provider/aniworld.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/provider/burningseries.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/provider/common.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/provider/crunchyroll.py
+-rw-r--r--   0        0        0    10844 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/provider/serienstream.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/provider/streamcloud.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/resources/default_settings.toml
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/resources/gucken.css
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/resources/mpv_skip.lua
+-rwxr-xr-x   0        0        0     3912 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/resources/vlc_skip.lua
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/tracker/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/tracker/anilist.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/tracker/aniworld.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/tracker/common.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/tracker/myanimelist.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/tracker/serienstream.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gucken-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gucken-0.1.6/LICENSE.txt
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 gucken-0.1.6/README.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 gucken-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 gucken-0.1.6/PKG-INFO
```

### Comparing `gucken-0.1.5/src/gucken/aniskip.py` & `gucken-0.1.6/src/gucken/aniskip.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/custom_widgets.py` & `gucken-0.1.6/src/gucken/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/gucken.py` & `gucken-0.1.6/src/gucken/gucken.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/rome.py` & `gucken-0.1.6/src/gucken/rome.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/settings.py` & `gucken-0.1.6/src/gucken/settings.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/update.py` & `gucken-0.1.6/src/gucken/update.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/utils.py` & `gucken-0.1.6/src/gucken/utils.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/hoster/common.py` & `gucken-0.1.6/src/gucken/hoster/common.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/hoster/doodstream.py` & `gucken-0.1.6/src/gucken/hoster/doodstream.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/hoster/streamtape.py` & `gucken-0.1.6/src/gucken/hoster/streamtape.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/hoster/veo.py` & `gucken-0.1.6/src/gucken/hoster/veo.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/hoster/vidoza.py` & `gucken-0.1.6/src/gucken/hoster/vidoza.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/player/_players.py` & `gucken-0.1.6/src/gucken/player/_players.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/player/common.py` & `gucken-0.1.6/src/gucken/player/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     @abstractmethod
     def is_available(cls) -> bool:
         return cls.detect_executable() is not None
 
     @staticmethod
     @abstractmethod
     def detect_executable() -> str:
-        raise NotImplementedError
+        pass
 
     @abstractmethod
     def play(
         self,
         url: str,
         title: str,
         full_screen: bool,
```

### Comparing `gucken-0.1.5/src/gucken/player/ffplay.py` & `gucken-0.1.6/src/gucken/player/ffplay.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/player/flatpak.py` & `gucken-0.1.6/src/gucken/player/flatpak.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 from subprocess import DEVNULL, Popen
 
 from .common import Player
 from .mpv import CelluloidPlayer, MPVPlayer
 from .vlc import VLCPlayer
 
 
-# This is just that you can check if the player is a flatpak player
+# This is just that you can check if the player is a Flatpak player
 class FlatpakPlayer(Player):
-    @staticmethod
-    def detect_executable() -> str:
-        pass
+    pass
 
 
 # TODO: Dont use Popen, it will slow down
 
 
 class FlatpakMPVPlayer(MPVPlayer, FlatpakPlayer):
```

### Comparing `gucken-0.1.5/src/gucken/player/mpv.py` & `gucken-0.1.6/src/gucken/player/mpv.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/player/vlc.py` & `gucken-0.1.6/src/gucken/player/vlc.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/player/wmplayer.py` & `gucken-0.1.6/src/gucken/player/wmplayer.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/provider/aniworld.py` & `gucken-0.1.6/src/gucken/provider/aniworld.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/provider/common.py` & `gucken-0.1.6/src/gucken/provider/common.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/provider/serienstream.py` & `gucken-0.1.6/src/gucken/provider/serienstream.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/resources/default_settings.toml` & `gucken-0.1.6/src/gucken/resources/default_settings.toml`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/resources/gucken.css` & `gucken-0.1.6/src/gucken/resources/gucken.css`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/resources/mpv_skip.lua` & `gucken-0.1.6/src/gucken/resources/mpv_skip.lua`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/resources/vlc_skip.lua` & `gucken-0.1.6/src/gucken/resources/vlc_skip.lua`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/src/gucken/tracker/anilist.py` & `gucken-0.1.6/src/gucken/tracker/anilist.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/LICENSE.txt` & `gucken-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/README.md` & `gucken-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/pyproject.toml` & `gucken-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gucken-0.1.5/PKG-INFO` & `gucken-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gucken
-Version: 0.1.5
+Version: 0.1.6
 Summary: Gucken is a Terminal User Interface which allows you to browse and watch your favorite anime's with style.
 Project-URL: Repository, https://github.com/Commandcracker/gucken
 Author: Commandcracker
 Maintainer: Commandcracker
 License: MIT License
         
         Copyright (c) 2024 Commandcracker
```

