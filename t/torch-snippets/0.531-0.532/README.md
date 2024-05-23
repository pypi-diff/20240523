# Comparing `tmp/torch_snippets-0.531.tar.gz` & `tmp/torch_snippets-0.532.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_snippets-0.531.tar", last modified: Tue May  7 08:15:31 2024, max compression
+gzip compressed data, was "torch_snippets-0.532.tar", last modified: Thu May 23 10:47:04 2024, max compression
```

## Comparing `torch_snippets-0.531.tar` & `torch_snippets-0.532.tar`

### file list

```diff
@@ -1,55 +1,54 @@
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-07 08:15:31.334568 torch_snippets-0.531/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11357 2021-12-31 15:06:08.000000 torch_snippets-0.531/LICENSE
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1062 2023-01-17 16:58:23.000000 torch_snippets-0.531/LICENSE.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      111 2021-12-31 15:06:08.000000 torch_snippets-0.531/MANIFEST.in
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5711 2024-05-07 08:15:31.334918 torch_snippets-0.531/PKG-INFO
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4999 2023-01-17 16:58:23.000000 torch_snippets-0.531/README.md
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      871 2024-05-07 08:12:44.000000 torch_snippets-0.531/settings.ini
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       79 2024-05-07 08:15:31.337021 torch_snippets-0.531/setup.cfg
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2001 2024-01-08 09:24:32.000000 torch_snippets-0.531/setup.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-07 08:15:31.319326 torch_snippets-0.531/torch_snippets/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      401 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    57057 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/_modidx.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4482 2023-01-17 16:58:25.000000 torch_snippets-0.531/torch_snippets/_nbdev.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8846 2024-05-07 08:15:27.000000 torch_snippets-0.531/torch_snippets/adapters.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    17079 2024-05-07 08:15:27.000000 torch_snippets-0.531/torch_snippets/bb_utils.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2026 2024-05-07 08:15:27.000000 torch_snippets-0.531/torch_snippets/bokeh_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    19042 2024-05-07 08:15:27.000000 torch_snippets-0.531/torch_snippets/charts.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1866 2023-12-28 06:40:32.000000 torch_snippets-0.531/torch_snippets/dates.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2056 2024-05-07 08:15:27.000000 torch_snippets-0.531/torch_snippets/decorators.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       73 2022-05-07 11:30:59.000000 torch_snippets-0.531/torch_snippets/fastcores.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11427 2023-11-28 11:52:35.000000 torch_snippets-0.531/torch_snippets/icecream.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8479 2024-05-07 08:15:27.000000 torch_snippets-0.531/torch_snippets/imgaug_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3429 2024-05-07 08:15:27.000000 torch_snippets-0.531/torch_snippets/inspector.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8386 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/interactive_show.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5727 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/ipython.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      597 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/load_defaults.py
--rwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    23434 2024-05-05 12:47:54.000000 torch_snippets-0.531/torch_snippets/loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8480 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/logger.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    14683 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/markup.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    17692 2024-05-07 08:11:34.000000 torch_snippets-0.531/torch_snippets/markup2.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2054 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/misc.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11039 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/paths.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1465 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/pdf_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      822 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/registry.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3234 2024-05-05 12:47:53.000000 torch_snippets-0.531/torch_snippets/scp.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6144 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/sklegos.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    14202 2024-03-28 08:34:42.000000 torch_snippets-0.531/torch_snippets/text_utils.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-07 08:15:31.326416 torch_snippets-0.531/torch_snippets/thinc_parser/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/thinc_parser/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1082 2022-10-16 17:20:20.000000 torch_snippets-0.531/torch_snippets/thinc_parser/parser.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    31250 2024-02-29 09:58:55.000000 torch_snippets-0.531/torch_snippets/torch_loader.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-07 08:15:31.333427 torch_snippets-0.531/torch_snippets/trainer/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       23 2024-05-07 08:15:28.000000 torch_snippets-0.531/torch_snippets/trainer/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6882 2024-05-07 08:15:27.000000 torch_snippets-0.531/torch_snippets/trainer/capsule.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2432 2024-05-07 08:15:27.000000 torch_snippets-0.531/torch_snippets/trainer/config.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5801 2024-04-24 06:16:19.000000 torch_snippets-0.531/torch_snippets/trainer/hooks.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2137 2024-02-14 10:01:57.000000 torch_snippets-0.531/torch_snippets/video.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-07 08:15:31.325037 torch_snippets-0.531/torch_snippets.egg-info/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5711 2024-05-07 08:15:31.000000 torch_snippets-0.531/torch_snippets.egg-info/PKG-INFO
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1337 2024-05-07 08:15:31.000000 torch_snippets-0.531/torch_snippets.egg-info/SOURCES.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        1 2024-05-07 08:15:31.000000 torch_snippets-0.531/torch_snippets.egg-info/dependency_links.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       20 2024-05-07 08:15:31.000000 torch_snippets-0.531/torch_snippets.egg-info/entry_points.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-01-17 16:58:23.000000 torch_snippets-0.531/torch_snippets.egg-info/not-zip-safe
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      281 2024-05-07 08:15:31.000000 torch_snippets-0.531/torch_snippets.egg-info/requires.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       15 2024-05-07 08:15:31.000000 torch_snippets-0.531/torch_snippets.egg-info/top_level.txt
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-23 10:47:04.065409 torch_snippets-0.532/
+-rw-r--r--   0 apple      (501) staff       (20)    11357 2024-05-16 14:23:49.000000 torch_snippets-0.532/LICENSE
+-rw-r--r--   0 apple      (501) staff       (20)     1062 2024-05-16 14:23:49.000000 torch_snippets-0.532/LICENSE.txt
+-rw-r--r--   0 apple      (501) staff       (20)      111 2024-05-16 14:23:49.000000 torch_snippets-0.532/MANIFEST.in
+-rw-r--r--   0 apple      (501) staff       (20)     6437 2024-05-23 10:47:04.065328 torch_snippets-0.532/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)     4999 2024-05-16 14:23:49.000000 torch_snippets-0.532/README.md
+-rw-r--r--   0 apple      (501) staff       (20)      871 2024-05-23 10:33:02.000000 torch_snippets-0.532/settings.ini
+-rw-r--r--   0 apple      (501) staff       (20)       79 2024-05-23 10:47:04.065621 torch_snippets-0.532/setup.cfg
+-rw-r--r--   0 apple      (501) staff       (20)     2001 2024-05-16 14:23:49.000000 torch_snippets-0.532/setup.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-23 10:47:04.062721 torch_snippets-0.532/torch_snippets/
+-rw-r--r--   0 apple      (501) staff       (20)      401 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    57057 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/_modidx.py
+-rw-r--r--   0 apple      (501) staff       (20)     4482 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets/_nbdev.py
+-rw-r--r--   0 apple      (501) staff       (20)     8846 2024-05-23 10:33:25.000000 torch_snippets-0.532/torch_snippets/adapters.py
+-rw-r--r--   0 apple      (501) staff       (20)    17079 2024-05-23 10:33:25.000000 torch_snippets-0.532/torch_snippets/bb_utils.py
+-rw-r--r--   0 apple      (501) staff       (20)     2026 2024-05-23 10:33:25.000000 torch_snippets-0.532/torch_snippets/bokeh_loader.py
+-rw-r--r--   0 apple      (501) staff       (20)    19042 2024-05-23 10:33:25.000000 torch_snippets-0.532/torch_snippets/charts.py
+-rw-r--r--   0 apple      (501) staff       (20)     1866 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets/dates.py
+-rw-r--r--   0 apple      (501) staff       (20)     2056 2024-05-23 10:33:25.000000 torch_snippets-0.532/torch_snippets/decorators.py
+-rw-r--r--   0 apple      (501) staff       (20)       73 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets/fastcores.py
+-rw-r--r--   0 apple      (501) staff       (20)    11427 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets/icecream.py
+-rw-r--r--   0 apple      (501) staff       (20)     8479 2024-05-23 10:33:25.000000 torch_snippets-0.532/torch_snippets/imgaug_loader.py
+-rw-r--r--   0 apple      (501) staff       (20)     3429 2024-05-23 10:33:25.000000 torch_snippets-0.532/torch_snippets/inspector.py
+-rw-r--r--   0 apple      (501) staff       (20)     8386 2024-05-23 10:33:25.000000 torch_snippets-0.532/torch_snippets/interactive_show.py
+-rw-r--r--   0 apple      (501) staff       (20)     5727 2024-05-23 10:33:25.000000 torch_snippets-0.532/torch_snippets/ipython.py
+-rw-r--r--   0 apple      (501) staff       (20)      597 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/load_defaults.py
+-rwxr-xr-x   0 apple      (501) staff       (20)    23434 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets/loader.py
+-rw-r--r--   0 apple      (501) staff       (20)     8480 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/logger.py
+-rw-r--r--   0 apple      (501) staff       (20)    15588 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/markup.py
+-rw-r--r--   0 apple      (501) staff       (20)    17741 2024-05-23 10:32:45.000000 torch_snippets-0.532/torch_snippets/markup2.py
+-rw-r--r--   0 apple      (501) staff       (20)     2054 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/misc.py
+-rw-r--r--   0 apple      (501) staff       (20)    11039 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/paths.py
+-rw-r--r--   0 apple      (501) staff       (20)     1465 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/pdf_loader.py
+-rw-r--r--   0 apple      (501) staff       (20)      822 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/registry.py
+-rw-r--r--   0 apple      (501) staff       (20)     3234 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets/scp.py
+-rw-r--r--   0 apple      (501) staff       (20)     6144 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/sklegos.py
+-rw-r--r--   0 apple      (501) staff       (20)    14202 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets/text_utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-23 10:47:04.063714 torch_snippets-0.532/torch_snippets/thinc_parser/
+-rw-r--r--   0 apple      (501) staff       (20)        0 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/thinc_parser/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     1082 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets/thinc_parser/parser.py
+-rw-r--r--   0 apple      (501) staff       (20)    31250 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets/torch_loader.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-23 10:47:04.064574 torch_snippets-0.532/torch_snippets/trainer/
+-rw-r--r--   0 apple      (501) staff       (20)       23 2024-05-23 10:33:26.000000 torch_snippets-0.532/torch_snippets/trainer/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     6882 2024-05-23 10:33:25.000000 torch_snippets-0.532/torch_snippets/trainer/capsule.py
+-rw-r--r--   0 apple      (501) staff       (20)     2432 2024-05-23 10:33:25.000000 torch_snippets-0.532/torch_snippets/trainer/config.py
+-rw-r--r--   0 apple      (501) staff       (20)     5801 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets/trainer/hooks.py
+-rw-r--r--   0 apple      (501) staff       (20)     2137 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets/video.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-23 10:47:04.064933 torch_snippets-0.532/torch_snippets.egg-info/
+-rw-r--r--   0 apple      (501) staff       (20)     6437 2024-05-23 10:47:04.000000 torch_snippets-0.532/torch_snippets.egg-info/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)     1296 2024-05-23 10:47:04.000000 torch_snippets-0.532/torch_snippets.egg-info/SOURCES.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2024-05-23 10:47:04.000000 torch_snippets-0.532/torch_snippets.egg-info/dependency_links.txt
+-rw-r--r--   0 apple      (501) staff       (20)        0 2024-05-16 14:23:49.000000 torch_snippets-0.532/torch_snippets.egg-info/not-zip-safe
+-rw-r--r--   0 apple      (501) staff       (20)      281 2024-05-23 10:47:04.000000 torch_snippets-0.532/torch_snippets.egg-info/requires.txt
+-rw-r--r--   0 apple      (501) staff       (20)       15 2024-05-23 10:47:04.000000 torch_snippets-0.532/torch_snippets.egg-info/top_level.txt
```

### Comparing `torch_snippets-0.531/LICENSE` & `torch_snippets-0.532/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/LICENSE.txt` & `torch_snippets-0.532/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/README.md` & `torch_snippets-0.532/README.md`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/settings.ini` & `torch_snippets-0.532/settings.ini`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = sizhky
 description = One line functions for common tasks
 keywords = snippets, torch
 author = Yeshwanth Reddy
 author_email = 1992chinna@gmail.com
 copyright = sizhky
 branch = master
-version = 0.531
+version = 0.532
 min_python = 3.7
 audience = Developers
 language = English
 custom_sidebar = False
 license = apache2
 status = 2
 requirements = fastcore matplotlib Pillow altair dill ipython loguru numpy pandas tqdm rich PyYAML catalogue confection pydantic typing srsly typing_extensions wasabi jsonlines imgaug>=0.4.0 xmltodict fuzzywuzzy scikit-learn nltk python-Levenshtein pre-commit pymupdf nbconvert nbformat icecream
```

### Comparing `torch_snippets-0.531/setup.py` & `torch_snippets-0.532/setup.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/_modidx.py` & `torch_snippets-0.532/torch_snippets/_modidx.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/_nbdev.py` & `torch_snippets-0.532/torch_snippets/_nbdev.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/adapters.py` & `torch_snippets-0.532/torch_snippets/adapters.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/bb_utils.py` & `torch_snippets-0.532/torch_snippets/bb_utils.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/bokeh_loader.py` & `torch_snippets-0.532/torch_snippets/bokeh_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/charts.py` & `torch_snippets-0.532/torch_snippets/charts.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/dates.py` & `torch_snippets-0.532/torch_snippets/dates.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/decorators.py` & `torch_snippets-0.532/torch_snippets/decorators.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/icecream.py` & `torch_snippets-0.532/torch_snippets/icecream.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/imgaug_loader.py` & `torch_snippets-0.532/torch_snippets/imgaug_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/inspector.py` & `torch_snippets-0.532/torch_snippets/inspector.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/interactive_show.py` & `torch_snippets-0.532/torch_snippets/interactive_show.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/ipython.py` & `torch_snippets-0.532/torch_snippets/ipython.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/load_defaults.py` & `torch_snippets-0.532/torch_snippets/load_defaults.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/loader.py` & `torch_snippets-0.532/torch_snippets/loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/logger.py` & `torch_snippets-0.532/torch_snippets/logger.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/markup.py` & `torch_snippets-0.532/torch_snippets/markup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/markups.ipynb.
 
 # %% auto 0
 __all__ = ['AD', 'Config', 'isnamedtupleinstance', 'unpack', 'AttrDict', 'pretty_json', 'read_json', 'write_json', 'write_jsonl',
            'read_jsonl', 'read_yaml', 'write_yaml', 'read_xml', 'write_xml']
 
 # %% ../nbs/markups.ipynb 2
-import json
+import json, os
 from json import JSONEncoder
 import jsonlines
 import yaml
 
+
 from .loader import BB, L, np
 from .paths import *
 from .logger import *
 import xmltodict
 from typing import Union
 from .thinc_parser.parser import Config
 
@@ -147,14 +148,15 @@
     def __iter__(self):
         return iter(self.keys())
 
     def __len__(self):
         return len(self.keys())
 
     def __repr__(self):
+        return self.summary()
         return "{%s}" % str(
             ", ".join("'%s': %s" % (k, repr(v)) for (k, v) in self.__dict__.items())
         )
 
     def __dir__(self):
         return self.__dict__.keys()
 
@@ -231,62 +233,90 @@
 
             elif isinstance(self[k], (L, tuple, list, set, frozenset)):
                 for i, item in enumerate(self[k]):
                     if isinstance(item, AttrDict):
                         addresses.extend(item.find_address(key, f"{new_path}.{i}"))
         return addresses
 
-    def summary(self, current_path="", summary_str="", depth=0, sep="\t"):
-        tab = sep * depth
-        for k in self.keys():
-            if current_path:
-                new_path = f"{current_path}.{k}"
-            else:
-                new_path = k
+    def summary(self, current_path="", depth=0, sep="  ", max_items=10):
+        max_items = int(os.environ.get("AD_MAX_ITEMS", max_items))
+        sep = os.environ.get("AD_SEP", sep)
+
+        def format_path(path, key):
+            return f"{path}.{key}" if path else key
+
+        def format_item(key, item, path, depth, sep):
+            import numpy as np
+            import pandas as pd
+
+            try:
+                import torch
+            except ModuleNotFoundError:
+
+                class Torch:
+                    Tensor = type(None)
+
+                torch = Torch()
+
+            if isinstance(item, (pd.DataFrame,)):
+                return f"{sep * depth}{key} - {type(item).__name__} - shape {item.shape} - columns {item.columns} - {hash_pandas_dataframe(item)}\n"
+            if isinstance(item, AttrDict) or hasattr(item, "keys"):
+                item = AttrDict(**item)
+                return f"{sep*depth}{key}\n" + item.summary(path, depth + 1, sep)
+            elif isinstance(item, (list, tuple, set, frozenset, L)):
+                return summarize_collection(key, item, path, depth + 1, sep)
+            elif isinstance(item, (torch.Tensor, np.ndarray)):
+                is_np = False
+                if isinstance(item, np.ndarray):
+                    is_np = True
+                    item = torch.tensor(item)
+                is_np = "🔦" if not is_np else "np."
+                return f"{sep * depth}{key} - {is_np}{item} - {hash_tensor(item)}\n"
 
-            if isinstance(self[k], AttrDict):
-                summary_str += f"{tab}{k}\n"
-                summary_str = self[k].summary(new_path, summary_str, depth + 1, sep=sep)
-            elif isinstance(self[k], (list, tuple, set, frozenset)):
-                summary_str += f"{tab}{k}\n"
-                for i, item in enumerate(self[k]):
-                    summary_str += f"{tab}{sep}{i}\n"
-                    if isinstance(item, AttrDict):
-                        summary_str = item.summary(
-                            f"{new_path}.{i}", summary_str, depth + 2, sep=sep
-                        )
-                    elif isinstance(item, (list, tuple, set, frozenset)):
-                        nested_path = f"{new_path}.{i}"
-                        nested_summary_str = ""
-                        for j, nested_item in enumerate(item):
-                            summary_str += f"{tab}{sep}{sep}{j}\n"
-                            if isinstance(nested_item, AttrDict):
-                                nested_summary_str = nested_item.summary(
-                                    f"{nested_path}.{j}",
-                                    nested_summary_str,
-                                    depth + 3,
-                                    sep=sep,
-                                )
-                            elif isinstance(nested_item, (list, tuple, set, frozenset)):
-                                nested_list_path = f"{nested_path}.{j}"
-                                for idx, nested_list_item in enumerate(nested_item):
-                                    if isinstance(nested_list_item, AttrDict):
-                                        nested_summary_str = nested_list_item.summary(
-                                            f"{nested_list_path}.{idx}",
-                                            nested_summary_str,
-                                            depth + 4,
-                                            sep=sep,
-                                        )
-                        if nested_summary_str:
-                            summary_str += nested_summary_str
-                    else:
-                        summary_str += f"{tab}{sep}{k} - {type(self[k]).__name__}\n"
             else:
-                summary_str += f"{tab}{k} - {type(self[k]).__name__}\n"
-
+                if isinstance(item, (int, float, complex, str)):
+                    is_multiline = False
+                    if isinstance(item, str):
+                        is_multiline = "\n" in item
+                        _sep = (
+                            " ...\n...\n...\n...\n... " if is_multiline else "........."
+                        )
+                        if len(item) > 250:
+                            item = item[:100] + _sep + item[-100:]
+                        if is_multiline:
+                            _item = item.split("\n")
+                            _item = "\n".join([f"{sep*(depth+1)}{l}" for l in _item])
+                            item = f"↓\n{sep*(depth+1)}```\n{_item}\n{sep*(depth+1)}```"
+                    multiline = "" if not is_multiline else "Multiline "
+                    return f"{sep * depth}{key} - {item} ({multiline}{type(item).__name__})\n"
+                else:
+                    return f"{sep * depth}{key} - {type(item).__name__}\n"
+
+        def summarize_collection(key, collection, path, d, s):
+            summary_str = f"{s * (d - 1)}{key}\n"
+            for i, item in enumerate(collection):
+                item_path = format_path(path, i)
+                if i < max_items:
+                    summary_str += format_item(i, item, item_path, d, s)
+                else:
+                    summary_str += (
+                        f"{s*d}... {len(collection) - max_items} more items ...\n"
+                    )
+                    break
+            return summary_str
+
+        summary_str = ""
+        for ix, key in enumerate(self.keys()):
+            if ix >= max_items:
+                summary_str += (
+                    f"{sep*depth} ... {len(self.keys()) - max_items} more keys ...\n"
+                )
+                break
+            new_path = format_path(current_path, key)
+            summary_str += format_item(key, self[key], new_path, depth, sep)
         return summary_str
 
     def write_summary(self, to, **kwargs):
         writelines(self.summary(**kwargs).split("\n"), to, "w")
 
     def fetch(self, addr):
         if isinstance(addr, (list, L)):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `torch_snippets-0.531/torch_snippets/markup2.py` & `torch_snippets-0.532/torch_snippets/markup2.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,16 +183,16 @@
                 value = L(value)
             return value
         else:
             return (
                 AttrDict(given_input_to_ad=value) if isinstance(value, dict) else value
             )
 
-    __getitem__ = (
-        lambda self, x: AttrDict({_x: self[_x] for _x in x})
+    __getitem__ = lambda self, x: (
+        AttrDict({_x: self[_x] for _x in x})
         if isinstance(x, (list, L))
         else getattr(self, str(x))
     )
     __setitem__ = lambda self, k, v: setattr(self, str(k), self._wrap(v))
 
     def update(self, dict):
         for k, v in dict.items():
@@ -288,15 +288,16 @@
             elif isinstance(self[k], (L, tuple, list, set, frozenset)):
                 for i, item in enumerate(self[k]):
                     if isinstance(item, AttrDict):
                         addresses.extend(item.find_address(key, f"{new_path}.{i}"))
         return addresses
 
     def summary(self, current_path="", depth=0, sep="  ", max_items=10):
-        max_items = os.environ.get("AD_MAX_ITEMS", max_items)
+        max_items = int(os.environ.get("AD_MAX_ITEMS", max_items))
+        sep = os.environ.get("AD_SEP", sep)
 
         def format_path(path, key):
             return f"{path}.{key}" if path else key
 
         def format_item(key, item, path, depth, sep):
             import numpy as np
             import pandas as pd
```

### Comparing `torch_snippets-0.531/torch_snippets/misc.py` & `torch_snippets-0.532/torch_snippets/misc.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/paths.py` & `torch_snippets-0.532/torch_snippets/paths.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/pdf_loader.py` & `torch_snippets-0.532/torch_snippets/pdf_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/registry.py` & `torch_snippets-0.532/torch_snippets/registry.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/scp.py` & `torch_snippets-0.532/torch_snippets/scp.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/sklegos.py` & `torch_snippets-0.532/torch_snippets/sklegos.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/text_utils.py` & `torch_snippets-0.532/torch_snippets/text_utils.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/thinc_parser/parser.py` & `torch_snippets-0.532/torch_snippets/thinc_parser/parser.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/torch_loader.py` & `torch_snippets-0.532/torch_snippets/torch_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/trainer/capsule.py` & `torch_snippets-0.532/torch_snippets/trainer/capsule.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/trainer/config.py` & `torch_snippets-0.532/torch_snippets/trainer/config.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/trainer/hooks.py` & `torch_snippets-0.532/torch_snippets/trainer/hooks.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets/video.py` & `torch_snippets-0.532/torch_snippets/video.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.531/torch_snippets.egg-info/SOURCES.txt` & `torch_snippets-0.532/torch_snippets.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 torch_snippets/sklegos.py
 torch_snippets/text_utils.py
 torch_snippets/torch_loader.py
 torch_snippets/video.py
 torch_snippets.egg-info/PKG-INFO
 torch_snippets.egg-info/SOURCES.txt
 torch_snippets.egg-info/dependency_links.txt
-torch_snippets.egg-info/entry_points.txt
 torch_snippets.egg-info/not-zip-safe
 torch_snippets.egg-info/requires.txt
 torch_snippets.egg-info/top_level.txt
 torch_snippets/thinc_parser/__init__.py
 torch_snippets/thinc_parser/parser.py
 torch_snippets/trainer/__init__.py
 torch_snippets/trainer/capsule.py
```

