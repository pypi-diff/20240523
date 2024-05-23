# Comparing `tmp/music_kraken-1.9.0.tar.gz` & `tmp/music_kraken-2.0.0.tar.gz`

## Comparing `music_kraken-1.9.0.tar` & `music_kraken-2.0.0.tar`

### file list

```diff
@@ -1,7 +1,82 @@
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 music_kraken-1.9.0/music_kraken/__init__.py
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 music_kraken-1.9.0/music_kraken/__main__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 music_kraken-1.9.0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 music_kraken-1.9.0/LICENSE
--rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 music_kraken-1.9.0/README.md
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 music_kraken-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     7998 2020-02-02 00:00:00.000000 music_kraken-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/__init__.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/__main__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/_version.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/audio/__init__.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/audio/codec.py
+-rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/audio/metadata.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/cli/__init__.py
+-rw-r--r--   0        0        0    14401 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/cli/main_downloader.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/cli/utils.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/cli/informations/__init__.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/cli/informations/paths.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/cli/options/__init__.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/cli/options/cache.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/cli/options/first_config.py
+-rw-r--r--   0        0        0     5838 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/cli/options/frontend.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/cli/options/settings.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/connection/__init__.py
+-rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/connection/cache.py
+-rw-r--r--   0        0        0    13408 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/connection/connection.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/connection/rotating.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/download/__init__.py
+-rw-r--r--   0        0        0    12504 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/download/page_attributes.py
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/download/results.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/__init__.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/artwork.py
+-rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/collection.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/contact.py
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/country.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/formatted_text.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/lint_default_factories.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/lyrics.py
+-rw-r--r--   0        0        0    12675 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/metadata.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/option.py
+-rw-r--r--   0        0        0    11281 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/parents.py
+-rw-r--r--   0        0        0    23480 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/song.py
+-rw-r--r--   0        0        0     7832 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/source.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/target.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/pages/__init__.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/pages/abstract.py
+-rw-r--r--   0        0        0    14081 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/pages/bandcamp.py
+-rw-r--r--   0        0        0    30308 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/pages/encyclopaedia_metallum.py
+-rw-r--r--   0        0        0    44109 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/pages/musify.py
+-rw-r--r--   0        0        0    13074 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/pages/youtube.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/pages/youtube_music/__init__.py
+-rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/pages/youtube_music/_list_render.py
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/pages/youtube_music/_music_object_render.py
+-rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/pages/youtube_music/super_youtube.py
+-rw-r--r--   0        0        0    27071 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/pages/youtube_music/youtube_music.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/__init__.py
+-rw-r--r--   0        0        0     9851 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/hacking.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/shared.py
+-rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/string_processing.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/config/__init__.py
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/config/config.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/config/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/config/attributes/__init__.py
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/config/attributes/attribute.py
+-rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/config/attributes/special_attributes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/config/config_files/__init__.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/config/config_files/logging_config.py
+-rw-r--r--   0        0        0     7956 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/config/config_files/main_config.py
+-rw-r--r--   0        0        0     6296 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/config/config_files/youtube_config.py
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/enums/__init__.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/enums/album.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/enums/colors.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/enums/contact.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/exception/__init__.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/exception/config.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/exception/download.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/exception/objects.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/path_manager/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/path_manager/config_directory.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/path_manager/locations.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/path_manager/music_directory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/support_classes/__init__.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/support_classes/download_result.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/support_classes/query.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 music_kraken-2.0.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 music_kraken-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 music_kraken-2.0.0/README.md
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 music_kraken-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 music_kraken-2.0.0/PKG-INFO
```

### Comparing `music_kraken-1.9.0/music_kraken/__init__.py` & `music_kraken-2.0.0/music_kraken/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 
 from rich.logging import RichHandler
 from rich.console import Console
 
 from .utils.shared import DEBUG, DEBUG_LOGGING
 from .utils.config import logging_settings, main_settings, read_config
 
-__version__ = "1.9.0"
-
 read_config()
 
 console: Console = Console()
 def init_logging():
     log_file = main_settings['log_file']
 
     if log_file.is_file():
@@ -42,15 +40,15 @@
     )
 
 init_logging()
 
 from . import cli
 
 if DEBUG:
-    sys.setrecursionlimit(100)
+    sys.setrecursionlimit(300)
 
 
 if main_settings['modify_gc']:
     """
     At the start I modify the garbage collector to run a bit fewer times.
     This should increase speed:
     https://mkennedy.codes/posts/python-gc-settings-change-this-and-make-your-app-go-20pc-faster/
```

### Comparing `music_kraken-1.9.0/music_kraken/__main__.py` & `music_kraken-2.0.0/music_kraken/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,13 +140,13 @@
     if arguments.test:
         genre = "test"
 
     cli.download(
         genre=genre,
         download_all=arguments.all,
         direct_download_url=arguments.url,
-        process_metadata_anyway=arguments.force_post_process or arguments.test
+        process_metadata_anyway=True or arguments.test
     )
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `music_kraken-1.9.0/LICENSE` & `music_kraken-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `music_kraken-1.9.0/pyproject.toml` & `music_kraken-2.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 [build-system]
-requires = ["hatchling", "hatch-requirements-txt" ]
+requires = ["hatchling", "hatch-requirements-txt", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 directory = "dist"
 
 [tool.hatch.build.targets.sdist]
-include = ["music_kraken/*.py" ]
+include = ["music_kraken/*.py", "music_kraken/**/*.py" ]
 
 [tool.hatch.build.targets.wheel]
 packages = ["music_kraken"]
 
 [project.scripts]
 music-kraken = "music_kraken.__main__:cli" 
 
 [tool.hatch.version]
-path = "music_kraken/__init__.py"
+source = "vcs"
+path = "music_kraken/_version.py"
+fallback-version = "0.0.0"
+
+[tool.hatch.version.raw-options]
+local_scheme = "no-local-version"
+
+[tool.hatch.build.hooks.vcs]
+version-file = "music_kraken/_version.py"
 
 [project]
 name = "music-kraken"
 description = "An extensive music downloader crawling the internet. It gets its metadata from a couple of metadata providers, and it scrapes the audiofiles."
 authors = [{ name = "Hellow2", email = "hazel_is_cute@proton.me" }]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
@@ -37,30 +45,33 @@
     "Topic :: Utilities",
 ]
 dependencies = [
     "requests~=2.31.0",
     "responses~=0.24.1",
     "beautifulsoup4~=4.11.1",
 
-    "ffmpeg-python~=0.2.0",
+    "pyffmpeg~=2.4.2.18.1",
     "ffmpeg-progress-yield~=0.7.8",
     "mutagen~=1.46.0",
+    "pillow~=10.3.0",
 
+    "rich~=13.7.1",
     "mistune~=3.0.2",
+    "markdownify~=0.12.1",
     "html2markdown~=0.1.7",
     "jellyfish~=0.9.0",
     "transliterate~=1.10.2",
-    "pycountry~=24.0.1",
+    "pycountry~=23.12.11",
     
     "python-dotenv~=1.0.1",
     "tqdm~=4.65.0",
     "platformdirs~=4.2.0",
     "pathvalidate~=2.5.2",
     "toml~=0.10.2",
     "typing_extensions~=4.7.1",
 
-    "sponsorblock~=0.1.3",
+    "python-sponsorblock~=0.1",
     "youtube_dl",
 ]
 dynamic = [
     "version"
 ]
```

