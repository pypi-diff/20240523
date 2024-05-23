# Comparing `tmp/music_kraken-2.0.0.tar.gz` & `tmp/music_kraken-2.0.1.dev3.tar.gz`

## Comparing `music_kraken-2.0.0.tar` & `music_kraken-2.0.1.dev3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/__init__.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/__main__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/_version.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/audio/__init__.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/audio/codec.py
--rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/audio/metadata.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/cli/__init__.py
--rw-r--r--   0        0        0    14401 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/cli/main_downloader.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/cli/utils.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/cli/informations/__init__.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/cli/informations/paths.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/cli/options/__init__.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/cli/options/cache.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/cli/options/first_config.py
--rw-r--r--   0        0        0     5838 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/cli/options/frontend.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/cli/options/settings.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/connection/__init__.py
--rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/connection/cache.py
--rw-r--r--   0        0        0    13408 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/connection/connection.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/connection/rotating.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/download/__init__.py
--rw-r--r--   0        0        0    12504 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/download/page_attributes.py
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/download/results.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/__init__.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/artwork.py
--rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/collection.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/contact.py
--rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/country.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/formatted_text.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/lint_default_factories.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/lyrics.py
--rw-r--r--   0        0        0    12675 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/metadata.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/option.py
--rw-r--r--   0        0        0    11281 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/parents.py
--rw-r--r--   0        0        0    23480 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/song.py
--rw-r--r--   0        0        0     7832 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/source.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/objects/target.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/pages/__init__.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/pages/abstract.py
--rw-r--r--   0        0        0    14081 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/pages/bandcamp.py
--rw-r--r--   0        0        0    30308 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/pages/encyclopaedia_metallum.py
--rw-r--r--   0        0        0    44109 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/pages/musify.py
--rw-r--r--   0        0        0    13074 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/pages/youtube.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/pages/youtube_music/__init__.py
--rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/pages/youtube_music/_list_render.py
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/pages/youtube_music/_music_object_render.py
--rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/pages/youtube_music/super_youtube.py
--rw-r--r--   0        0        0    27071 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/pages/youtube_music/youtube_music.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/__init__.py
--rw-r--r--   0        0        0     9851 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/hacking.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/shared.py
--rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/string_processing.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/config/__init__.py
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/config/config.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/config/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/config/attributes/__init__.py
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/config/attributes/attribute.py
--rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/config/attributes/special_attributes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/config/config_files/__init__.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/config/config_files/logging_config.py
--rw-r--r--   0        0        0     7956 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/config/config_files/main_config.py
--rw-r--r--   0        0        0     6296 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/config/config_files/youtube_config.py
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/enums/__init__.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/enums/album.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/enums/colors.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/enums/contact.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/exception/__init__.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/exception/config.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/exception/download.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/exception/objects.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/path_manager/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/path_manager/config_directory.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/path_manager/locations.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/path_manager/music_directory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/support_classes/__init__.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/support_classes/download_result.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 music_kraken-2.0.0/music_kraken/utils/support_classes/query.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 music_kraken-2.0.0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 music_kraken-2.0.0/LICENSE
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 music_kraken-2.0.0/README.md
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 music_kraken-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 music_kraken-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/__init__.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/__main__.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/_version.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/audio/__init__.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/audio/codec.py
+-rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/audio/metadata.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/cli/__init__.py
+-rw-r--r--   0        0        0    14401 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/cli/main_downloader.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/cli/utils.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/cli/informations/__init__.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/cli/informations/paths.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/cli/options/__init__.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/cli/options/cache.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/cli/options/first_config.py
+-rw-r--r--   0        0        0     5838 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/cli/options/frontend.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/cli/options/settings.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/connection/__init__.py
+-rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/connection/cache.py
+-rw-r--r--   0        0        0    13408 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/connection/connection.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/connection/rotating.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/download/__init__.py
+-rw-r--r--   0        0        0    12504 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/download/page_attributes.py
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/download/results.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/__init__.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/artwork.py
+-rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/collection.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/contact.py
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/country.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/formatted_text.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/lint_default_factories.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/lyrics.py
+-rw-r--r--   0        0        0    12675 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/metadata.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/option.py
+-rw-r--r--   0        0        0    11281 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/parents.py
+-rw-r--r--   0        0        0    23480 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/song.py
+-rw-r--r--   0        0        0     7832 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/source.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/target.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/pages/__init__.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/pages/abstract.py
+-rw-r--r--   0        0        0    14081 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/pages/bandcamp.py
+-rw-r--r--   0        0        0    30308 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/pages/encyclopaedia_metallum.py
+-rw-r--r--   0        0        0    44109 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/pages/musify.py
+-rw-r--r--   0        0        0    13074 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/pages/youtube.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/pages/youtube_music/__init__.py
+-rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/pages/youtube_music/_list_render.py
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/pages/youtube_music/_music_object_render.py
+-rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/pages/youtube_music/super_youtube.py
+-rw-r--r--   0        0        0    27173 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/pages/youtube_music/youtube_music.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/__init__.py
+-rw-r--r--   0        0        0     9851 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/hacking.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/shared.py
+-rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/string_processing.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/config/__init__.py
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/config/config.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/config/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/config/attributes/__init__.py
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/config/attributes/attribute.py
+-rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/config/attributes/special_attributes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/config/config_files/__init__.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/config/config_files/logging_config.py
+-rw-r--r--   0        0        0     7956 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/config/config_files/main_config.py
+-rw-r--r--   0        0        0     6296 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/config/config_files/youtube_config.py
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/enums/__init__.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/enums/album.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/enums/colors.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/enums/contact.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/exception/__init__.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/exception/config.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/exception/download.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/exception/objects.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/path_manager/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/path_manager/config_directory.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/path_manager/locations.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/path_manager/music_directory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/support_classes/__init__.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/support_classes/download_result.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/support_classes/query.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/LICENSE
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/README.md
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/pyproject.toml
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/PKG-INFO
```

### Comparing `music_kraken-2.0.0/music_kraken/__init__.py` & `music_kraken-2.0.1.dev3/music_kraken/__init__.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/__main__.py` & `music_kraken-2.0.1.dev3/music_kraken/__main__.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/audio/codec.py` & `music_kraken-2.0.1.dev3/music_kraken/audio/codec.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/audio/metadata.py` & `music_kraken-2.0.1.dev3/music_kraken/audio/metadata.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/cli/main_downloader.py` & `music_kraken-2.0.1.dev3/music_kraken/cli/main_downloader.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/cli/utils.py` & `music_kraken-2.0.1.dev3/music_kraken/cli/utils.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/cli/informations/paths.py` & `music_kraken-2.0.1.dev3/music_kraken/cli/informations/paths.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/cli/options/frontend.py` & `music_kraken-2.0.1.dev3/music_kraken/cli/options/frontend.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/cli/options/settings.py` & `music_kraken-2.0.1.dev3/music_kraken/cli/options/settings.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/connection/cache.py` & `music_kraken-2.0.1.dev3/music_kraken/connection/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pathlib import Path
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta
 from typing import List, Optional
 from functools import lru_cache
 import logging
 
+from ..utils import output, BColors
 from ..utils.config import main_settings
 from ..utils.string_processing import fit_to_file_system
 
 
 @dataclass
 class CacheAttribute:
     module: str
@@ -200,17 +201,20 @@
         delete every file in the cache directory
         :return:
         """
 
         for path in self._dir.iterdir():
             if path.is_dir():
                 for file in path.iterdir():
+                    output(f"Deleting file {file}", color=BColors.GREY)
                     file.unlink()
+                output(f"Deleting folder {path}", color=BColors.HEADER)
                 path.rmdir()
             else:
+                output(f"Deleting folder {path}", color=BColors.HEADER)
                 path.unlink()
 
         self.cached_attributes.clear()
         self._id_to_attribute.clear()
 
         self._write_index()
```

### Comparing `music_kraken-2.0.0/music_kraken/connection/connection.py` & `music_kraken-2.0.1.dev3/music_kraken/connection/connection.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/connection/rotating.py` & `music_kraken-2.0.1.dev3/music_kraken/connection/rotating.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/download/__init__.py` & `music_kraken-2.0.1.dev3/music_kraken/download/__init__.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/download/page_attributes.py` & `music_kraken-2.0.1.dev3/music_kraken/download/page_attributes.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/download/results.py` & `music_kraken-2.0.1.dev3/music_kraken/download/results.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/objects/artwork.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/artwork.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/objects/collection.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/collection.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/objects/contact.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/contact.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/objects/country.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/country.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/objects/formatted_text.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/formatted_text.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/objects/lint_default_factories.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/lint_default_factories.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/objects/lyrics.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/lyrics.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/objects/metadata.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/metadata.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/objects/option.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/option.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/objects/parents.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/parents.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/objects/song.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/song.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/objects/source.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/source.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/objects/target.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/target.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/pages/abstract.py` & `music_kraken-2.0.1.dev3/music_kraken/pages/abstract.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/pages/bandcamp.py` & `music_kraken-2.0.1.dev3/music_kraken/pages/bandcamp.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/pages/encyclopaedia_metallum.py` & `music_kraken-2.0.1.dev3/music_kraken/pages/encyclopaedia_metallum.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/pages/musify.py` & `music_kraken-2.0.1.dev3/music_kraken/pages/musify.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/pages/youtube.py` & `music_kraken-2.0.1.dev3/music_kraken/pages/youtube.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/pages/youtube_music/_list_render.py` & `music_kraken-2.0.1.dev3/music_kraken/pages/youtube_music/_list_render.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/pages/youtube_music/_music_object_render.py` & `music_kraken-2.0.1.dev3/music_kraken/pages/youtube_music/_music_object_render.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/pages/youtube_music/super_youtube.py` & `music_kraken-2.0.1.dev3/music_kraken/pages/youtube_music/super_youtube.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/pages/youtube_music/youtube_music.py` & `music_kraken-2.0.1.dev3/music_kraken/pages/youtube_music/youtube_music.py`

 * *Files 2% similar despite different names*

```diff
@@ -545,14 +545,19 @@
         for song in album.song_collection:
             for song_source in song.source_collection:
                 song_source.additional_data["playlist_id"] = browse_id
 
         return album
 
     def fetch_lyrics(self, video_id: str, playlist_id: str = None) -> str:
+        """
+        1. fetches the tabs of a song, to get the browse id
+        2. finds the browse id of the lyrics
+        3. fetches the lyrics with the browse id
+        """
         request_data = {
             "context": {**self.credentials.context, "adSignalsInfo": {"params": []}},
             "videoId": video_id,
         }
         if playlist_id is not None:
             request_data["playlistId"] = playlist_id
         
@@ -571,15 +576,16 @@
 
         tabs = traverse_json_path(tab_data, "contents.singleColumnMusicWatchNextResultsRenderer.tabbedRenderer.watchNextTabbedResultsRenderer.tabs", default=[])
         browse_id = None
         for tab in tabs:
             pageType = traverse_json_path(tab, "tabRenderer.endpoint.browseEndpoint.browseEndpointContextSupportedConfigs.browseEndpointContextMusicConfig.pageType", default="")
             if pageType in ("MUSIC_TAB_TYPE_LYRICS", "MUSIC_PAGE_TYPE_TRACK_LYRICS") or "lyrics" in pageType.lower():
                 browse_id = traverse_json_path(tab, "tabRenderer.endpoint.browseEndpoint.browseId", default=None)
-                break
+                if browse_id is not None:
+                    break
 
         if browse_id is None:
             return None
 
 
         r = self.yt_music_connection.post(
             url=get_youtube_url(path="/youtubei/v1/browse", query=f"prettyPrint=false"),
@@ -717,15 +723,14 @@
                 self.not_download[source.hash_url] = e
                 self.LOGGER.error(f"Couldn't fetch song from {source.url}. {e}")
                 return {"error": e}
         _best_format = _get_best_format(ydl_res.get("formats", [{}]))
 
         self.download_values_by_url[source.url] = {
             "url": _best_format.get("url"),
-            "chunk_size": _best_format.get("downloader_options", {}).get("http_chunk_size", main_settings["chunk_size"]),
             "headers": _best_format.get("http_headers", {}),
         }
 
         return self.download_values_by_url[source.url]
 
 
     def download_song_to_target(self, source: Source, target: Target, desc: str = None) -> DownloadResult:
```

### Comparing `music_kraken-2.0.0/music_kraken/utils/__init__.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/utils/hacking.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/hacking.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/utils/shared.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/shared.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/utils/string_processing.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/string_processing.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/utils/config/__init__.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/config/__init__.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/utils/config/config.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/config/config.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/utils/config/attributes/attribute.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/config/attributes/attribute.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/utils/config/attributes/special_attributes.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/config/attributes/special_attributes.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/utils/config/config_files/logging_config.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/config/config_files/logging_config.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/utils/config/config_files/main_config.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/config/config_files/main_config.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/utils/config/config_files/youtube_config.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/config/config_files/youtube_config.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/utils/enums/__init__.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/utils/enums/album.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/enums/album.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/utils/exception/config.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/exception/config.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/utils/path_manager/locations.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/path_manager/locations.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/utils/path_manager/music_directory.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/path_manager/music_directory.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/utils/support_classes/download_result.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/support_classes/download_result.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/music_kraken/utils/support_classes/query.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/support_classes/query.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/LICENSE` & `music_kraken-2.0.1.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/README.md` & `music_kraken-2.0.1.dev3/README.md`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/pyproject.toml` & `music_kraken-2.0.1.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.0/PKG-INFO` & `music_kraken-2.0.1.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: music-kraken
-Version: 2.0.0
+Version: 2.0.1.dev3
 Summary: An extensive music downloader crawling the internet. It gets its metadata from a couple of metadata providers, and it scrapes the audiofiles.
 Author-email: Hellow2 <hazel_is_cute@proton.me>
 License-Expression: AGPL-3.0-or-later
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

