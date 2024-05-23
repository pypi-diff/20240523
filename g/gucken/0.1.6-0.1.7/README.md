# Comparing `tmp/gucken-0.1.6.tar.gz` & `tmp/gucken-0.1.7.tar.gz`

## Comparing `gucken-0.1.6.tar` & `gucken-0.1.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/__main__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/aniskip.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/custom_widgets.py
--rw-r--r--   0        0        0    32791 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/gucken.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/rome.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/settings.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/update.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/hoster/__init__.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/hoster/_hosters.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/hoster/common.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/hoster/doodstream.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/hoster/streamtape.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/hoster/veo.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/hoster/vidoza.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/player/__init__.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/player/_players.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/player/android.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/player/common.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/player/ffplay.py
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/player/flatpak.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/player/mpv.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/player/vlc.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/player/wmplayer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/provider/__init__.py
--rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/provider/aniworld.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/provider/burningseries.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/provider/common.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/provider/crunchyroll.py
--rw-r--r--   0        0        0    10844 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/provider/serienstream.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/provider/streamcloud.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/resources/default_settings.toml
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/resources/gucken.css
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/resources/mpv_skip.lua
--rwxr-xr-x   0        0        0     3912 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/resources/vlc_skip.lua
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/tracker/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/tracker/anilist.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/tracker/aniworld.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/tracker/common.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/tracker/myanimelist.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.6/src/gucken/tracker/serienstream.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gucken-0.1.6/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gucken-0.1.6/LICENSE.txt
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 gucken-0.1.6/README.md
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 gucken-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 gucken-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/__main__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/aniskip.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/custom_widgets.py
+-rw-r--r--   0        0        0    32797 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/gucken.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/rome.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/settings.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/update.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/hoster/__init__.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/hoster/_hosters.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/hoster/common.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/hoster/doodstream.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/hoster/streamtape.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/hoster/veo.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/hoster/vidoza.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/player/__init__.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/player/_players.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/player/android.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/player/common.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/player/ffplay.py
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/player/flatpak.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/player/mpv.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/player/vlc.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/player/wmplayer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/provider/__init__.py
+-rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/provider/aniworld.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/provider/burningseries.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/provider/common.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/provider/crunchyroll.py
+-rw-r--r--   0        0        0    10844 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/provider/serienstream.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/provider/streamcloud.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/resources/default_settings.toml
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/resources/gucken.css
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/resources/mpv_skip.lua
+-rwxr-xr-x   0        0        0     3912 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/resources/vlc_skip.lua
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/tracker/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/tracker/anilist.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/tracker/aniworld.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/tracker/common.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/tracker/myanimelist.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.7/src/gucken/tracker/serienstream.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gucken-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gucken-0.1.7/LICENSE.txt
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 gucken-0.1.7/README.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 gucken-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 gucken-0.1.7/PKG-INFO
```

### Comparing `gucken-0.1.6/src/gucken/aniskip.py` & `gucken-0.1.7/src/gucken/aniskip.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/custom_widgets.py` & `gucken-0.1.7/src/gucken/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/gucken.py` & `gucken-0.1.7/src/gucken/gucken.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
     # TODO: color theme https://textual.textualize.io/guide/design/#designing-with-colors
 
     CSS_PATH = [join("resources", "gucken.css")]
     custom_css = user_config_path("gucken").joinpath("custom.css")
     if custom_css.exists():
         CSS_PATH.append(custom_css)
     BINDINGS: ClassVar[list[BindingType]] = [
-        Binding("q", "quit", "Quit", show=True, priority=False),
+        Binding("q", "quit", "Quit", show=False, priority=False),
     ]
 
     def __init__(self, debug: bool, search: str):
         super().__init__(watch_css=debug)
         self._debug = debug
         self._search = search
 
@@ -324,17 +324,17 @@
                             value=settings["ani_skip"]["skip_ending"],
                         )
                         yield RadioButton(
                             "Get chapters (only MPV)",
                             id="ani_skip_chapters",
                             value=settings["ani_skip"]["chapters"],
                         )
-        with Footer():
-            with Center():
-                yield Label("Made by Commandcracker with [red]:heart:[/red]")
+        # yield Footer()
+        with Center(id="footer"):
+            yield Label("Made by Commandcracker with [red]:heart:[/red]")
 
     @on(Input.Changed)
     async def input_changed(self, event: Input.Changed):
         id = event.control.id
         value = event.value
 
         if id == "input":
```

### Comparing `gucken-0.1.6/src/gucken/rome.py` & `gucken-0.1.7/src/gucken/rome.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/settings.py` & `gucken-0.1.7/src/gucken/settings.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/update.py` & `gucken-0.1.7/src/gucken/update.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/utils.py` & `gucken-0.1.7/src/gucken/utils.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/hoster/common.py` & `gucken-0.1.7/src/gucken/hoster/common.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/hoster/doodstream.py` & `gucken-0.1.7/src/gucken/hoster/doodstream.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/hoster/streamtape.py` & `gucken-0.1.7/src/gucken/hoster/streamtape.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/hoster/veo.py` & `gucken-0.1.7/src/gucken/hoster/veo.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/hoster/vidoza.py` & `gucken-0.1.7/src/gucken/hoster/vidoza.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/player/_players.py` & `gucken-0.1.7/src/gucken/player/_players.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/player/android.py` & `gucken-0.1.7/src/gucken/player/android.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/player/common.py` & `gucken-0.1.7/src/gucken/player/common.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/player/ffplay.py` & `gucken-0.1.7/src/gucken/player/ffplay.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/player/flatpak.py` & `gucken-0.1.7/src/gucken/player/flatpak.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/player/mpv.py` & `gucken-0.1.7/src/gucken/player/mpv.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/player/vlc.py` & `gucken-0.1.7/src/gucken/player/vlc.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/player/wmplayer.py` & `gucken-0.1.7/src/gucken/player/wmplayer.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/provider/aniworld.py` & `gucken-0.1.7/src/gucken/provider/aniworld.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/provider/common.py` & `gucken-0.1.7/src/gucken/provider/common.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/provider/serienstream.py` & `gucken-0.1.7/src/gucken/provider/serienstream.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/resources/default_settings.toml` & `gucken-0.1.7/src/gucken/resources/default_settings.toml`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/resources/gucken.css` & `gucken-0.1.7/src/gucken/resources/gucken.css`

 * *Files 7% similar despite different names*

```diff
@@ -56,8 +56,15 @@
 
 ClickableListItem {
     padding-bottom: -1;
     padding-left: -2;
     padding-right: -2;
 }
 
+#footer {
+    background: $accent;
+    color: $text;
+    dock: bottom;
+    height: 1;
+}
+
 /*$accent: lime;*/
```

### Comparing `gucken-0.1.6/src/gucken/resources/mpv_skip.lua` & `gucken-0.1.7/src/gucken/resources/mpv_skip.lua`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/resources/vlc_skip.lua` & `gucken-0.1.7/src/gucken/resources/vlc_skip.lua`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/src/gucken/tracker/anilist.py` & `gucken-0.1.7/src/gucken/tracker/anilist.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/LICENSE.txt` & `gucken-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/README.md` & `gucken-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/pyproject.toml` & `gucken-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gucken-0.1.6/PKG-INFO` & `gucken-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gucken
-Version: 0.1.6
+Version: 0.1.7
 Summary: Gucken is a Terminal User Interface which allows you to browse and watch your favorite anime's with style.
 Project-URL: Repository, https://github.com/Commandcracker/gucken
 Author: Commandcracker
 Maintainer: Commandcracker
 License: MIT License
         
         Copyright (c) 2024 Commandcracker
```

