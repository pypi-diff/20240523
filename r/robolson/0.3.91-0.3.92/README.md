# Comparing `tmp/robolson-0.3.91.tar.gz` & `tmp/robolson-0.3.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robolson-0.3.91.tar", max compression
+gzip compressed data, was "robolson-0.3.92.tar", max compression
```

## Comparing `robolson-0.3.91.tar` & `robolson-0.3.92.tar`

### file list

```diff
@@ -1,60 +1,65 @@
--rw-r--r--   0        0        0      123 2024-01-23 01:31:29.797260 robolson-0.3.91/.autoenv
--rw-r--r--   0        0        0       56 2023-01-12 07:11:08.976913 robolson-0.3.91/.justfile
--rw-r--r--   0        0        0       24 2022-03-21 20:13:02.294495 robolson-0.3.91/__init__.py
--rw-r--r--   0        0        0       66 2022-03-21 23:26:56.141915 robolson-0.3.91/__main__.py
--rw-r--r--   0        0        0    21259 2024-01-23 01:31:29.798263 robolson-0.3.91/algebra.py
--rw-r--r--   0        0        0      829 2023-02-17 21:22:04.657577 robolson-0.3.91/anagram.py
--rw-r--r--   0        0        0    30059 2024-01-23 01:31:29.799261 robolson-0.3.91/clean.py
--rw-r--r--   0        0        0      489 2024-01-23 01:31:29.800262 robolson-0.3.91/config/algebra/config.toml
--rw-r--r--   0        0        0      642 2024-02-13 23:30:53.341876 robolson-0.3.91/config/algebra/latex_templates.toml
--rw-r--r--   0        0        0     1006 2023-01-18 09:41:39.545792 robolson-0.3.91/config/clean.toml
--rw-r--r--   0        0        0      675 2024-04-19 07:50:17.895146 robolson-0.3.91/config/english/config.toml
--rw-r--r--   0        0        0      570 2024-04-19 07:50:17.893117 robolson-0.3.91/config/english/latex_templates.toml
--rw-r--r--   0        0        0   568244 2024-04-16 02:57:22.162497 robolson-0.3.91/data/george orwell 1984.txt
--rw-r--r--   0        0        0   816591 2023-02-17 19:54:50.219010 robolson-0.3.91/data/word_list.txt
--rw-r--r--   0        0        0    11288 2024-04-16 02:59:58.700477 robolson-0.3.91/english.py
--rw-r--r--   0        0        0    10015 2023-05-10 16:31:41.064453 robolson-0.3.91/ffmpeg.py
--rw-r--r--   0        0        0     1079 2024-01-23 01:31:29.803259 robolson-0.3.91/help.py
--rw-r--r--   0        0        0    20235 2022-05-02 00:50:16.538685 robolson-0.3.91/hierarchy.py
--rw-r--r--   0        0        0    27535 2024-04-19 04:45:08.415412 robolson-0.3.91/homework.py
--rw-r--r--   0        0        0        0 2022-05-21 03:18:54.857385 robolson-0.3.91/loggers/__init__.py
--rw-r--r--   0        0        0     1021 2022-07-14 03:10:34.224571 robolson-0.3.91/loggers/tick_logger.py
--rw-r--r--   0        0        0     1976 2024-03-03 02:54:30.346789 robolson-0.3.91/night.py
--rw-r--r--   0        0        0    21895 2024-01-30 19:12:07.481429 robolson-0.3.91/old_clean.py
--rw-r--r--   0        0        0     5166 2024-01-23 01:31:29.806260 robolson-0.3.91/old_mail.py
--rw-r--r--   0        0        0        0 2022-05-21 03:18:36.761960 robolson-0.3.91/parser/__init__.py
--rw-r--r--   0        0        0     1119 2023-01-14 21:30:02.931167 robolson-0.3.91/parser/clean_parser.py
--rw-r--r--   0        0        0     1220 2022-07-08 10:11:15.790934 robolson-0.3.91/parser/email_parser.py
--rw-r--r--   0        0        0     1770 2022-04-08 02:11:14.941735 robolson-0.3.91/parser/ffmpeg_parser.py
--rw-r--r--   0        0        0     1509 2023-02-06 13:43:39.345746 robolson-0.3.91/parser/reddit_parser.py
--rw-r--r--   0        0        0      909 2022-07-04 01:50:11.624597 robolson-0.3.91/parser/tick_parser.py
--rw-r--r--   0        0        0    71203 2024-01-26 07:47:28.692623 robolson-0.3.91/poetry.lock
--rw-r--r--   0        0        0     1244 2024-02-14 01:20:51.194054 robolson-0.3.91/pyproject.toml
--rw-r--r--   0        0        0     8401 2023-02-06 13:44:14.394052 robolson-0.3.91/reddit_archive.py
--rw-r--r--   0        0        0     4153 2023-02-27 21:47:08.721554 robolson-0.3.91/robai.py
--rw-r--r--   0        0        0        0 2024-01-23 01:31:29.814265 robolson-0.3.91/tests/__init__.py
--rw-r--r--   0        0        0     1017 2024-01-23 01:31:29.815258 robolson-0.3.91/tests/test_algebra.py
--rw-r--r--   0        0        0      970 2024-01-23 01:31:29.815258 robolson-0.3.91/tests/test_clean.py
--rw-r--r--   0        0        0     5978 2023-02-08 17:22:46.858389 robolson-0.3.91/tick.py
--rw-r--r--   0        0        0        0 2022-04-07 19:21:12.560000 robolson-0.3.91/ticktick/__init__.py
--rw-r--r--   0        0        0    24751 2022-05-09 07:55:23.045790 robolson-0.3.91/ticktick/api.py
--rw-r--r--   0        0        0     1473 2022-05-02 00:50:17.516634 robolson-0.3.91/ticktick/cache.py
--rw-r--r--   0        0        0        0 2022-04-07 19:21:12.670000 robolson-0.3.91/ticktick/helpers/__init__.py
--rw-r--r--   0        0        0       68 2022-04-07 19:21:12.699905 robolson-0.3.91/ticktick/helpers/constants.py
--rw-r--r--   0        0        0     1184 2022-05-02 00:50:17.590600 robolson-0.3.91/ticktick/helpers/hex_color.py
--rw-r--r--   0        0        0     2787 2022-05-09 07:49:04.451389 robolson-0.3.91/ticktick/helpers/time_methods.py
--rw-r--r--   0        0        0     8805 2022-04-08 04:12:37.380147 robolson-0.3.91/ticktick/helpers/timezones.txt
--rw-r--r--   0        0        0        0 2022-04-07 19:21:12.804000 robolson-0.3.91/ticktick/managers/__init__.py
--rw-r--r--   0        0        0      444 2022-05-02 00:50:18.497442 robolson-0.3.91/ticktick/managers/check_logged_in.py
--rw-r--r--   0        0        0      408 2022-05-02 00:50:18.510446 robolson-0.3.91/ticktick/managers/focus.py
--rw-r--r--   0        0        0     4956 2022-05-02 00:50:18.524792 robolson-0.3.91/ticktick/managers/habits.py
--rw-r--r--   0        0        0      334 2022-05-02 00:50:18.547793 robolson-0.3.91/ticktick/managers/pomo.py
--rw-r--r--   0        0        0    43862 2022-06-11 04:09:26.134840 robolson-0.3.91/ticktick/managers/projects.py
--rw-r--r--   0        0        0      429 2022-05-02 00:50:18.617905 robolson-0.3.91/ticktick/managers/settings.py
--rw-r--r--   0        0        0    46804 2022-06-11 04:10:45.717520 robolson-0.3.91/ticktick/managers/tags.py
--rw-r--r--   0        0        0    54311 2022-06-11 04:08:26.998571 robolson-0.3.91/ticktick/managers/tasks.py
--rw-r--r--   0        0        0    13289 2022-05-09 07:54:06.826880 robolson-0.3.91/ticktick/oauth2.py
--rw-r--r--   0        0        0     1135 2024-01-23 01:31:29.816259 robolson-0.3.91/tomldict.py
--rw-r--r--   0        0        0      144 2024-02-13 23:10:05.116424 robolson-0.3.91/tomlshelve.py
--rw-r--r--   0        0        0       24 2022-04-19 17:39:25.252880 robolson-0.3.91/tox.ini
--rw-r--r--   0        0        0      927 1970-01-01 00:00:00.000000 robolson-0.3.91/PKG-INFO
+-rw-r--r--   0        0        0      123 2024-01-23 01:31:29.797260 robolson-0.3.92/.autoenv
+-rw-r--r--   0        0        0       56 2023-01-12 07:11:08.976913 robolson-0.3.92/.justfile
+-rw-r--r--   0        0        0       24 2022-03-21 20:13:02.294495 robolson-0.3.92/__init__.py
+-rw-r--r--   0        0        0       66 2022-03-21 23:26:56.141915 robolson-0.3.92/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:23:07.826613 robolson-0.3.92/algebra/__init__.py
+-rw-r--r--   0        0        0    24118 2024-05-23 02:06:56.099208 robolson-0.3.92/algebra/problems.py
+-rw-r--r--   0        0        0      829 2023-02-17 21:22:04.657577 robolson-0.3.92/anagram.py
+-rw-r--r--   0        0        0    30059 2024-01-23 01:31:29.799261 robolson-0.3.92/clean.py
+-rw-r--r--   0        0        0      489 2024-01-23 01:31:29.800262 robolson-0.3.92/config/algebra/config.toml
+-rw-r--r--   0        0        0      642 2024-02-13 23:30:53.341876 robolson-0.3.92/config/algebra/latex_templates.toml
+-rw-r--r--   0        0        0     1006 2023-01-18 09:41:39.545792 robolson-0.3.92/config/clean.toml
+-rw-r--r--   0        0        0      694 2024-05-08 00:04:20.817979 robolson-0.3.92/config/english/config.toml
+-rw-r--r--   0        0        0     1026 2024-05-08 00:01:44.828961 robolson-0.3.92/config/english/latex_templates.toml
+-rw-r--r--   0        0        0   816591 2023-02-17 19:54:50.219010 robolson-0.3.92/data/word_list.txt
+-rw-r--r--   0        0        0    28582 2024-05-23 02:06:17.351239 robolson-0.3.92/english.py
+-rw-r--r--   0        0        0    10015 2023-05-10 16:31:41.064453 robolson-0.3.92/ffmpeg.py
+-rw-r--r--   0        0        0     1079 2024-01-23 01:31:29.803259 robolson-0.3.92/help.py
+-rw-r--r--   0        0        0    20235 2022-05-02 00:50:16.538685 robolson-0.3.92/hierarchy.py
+-rw-r--r--   0        0        0    12729 2024-05-22 22:37:30.823400 robolson-0.3.92/homework.py
+-rw-r--r--   0        0        0        0 2022-05-21 03:18:54.857385 robolson-0.3.92/loggers/__init__.py
+-rw-r--r--   0        0        0     1118 2024-05-22 21:05:41.539436 robolson-0.3.92/loggers/tick_logger.py
+-rw-r--r--   0        0        0     1976 2024-03-03 02:54:30.346789 robolson-0.3.92/night.py
+-rw-r--r--   0        0        0    21259 2024-01-23 01:31:29.798263 robolson-0.3.92/old_algebra.py
+-rw-r--r--   0        0        0    21895 2024-01-30 19:12:07.481429 robolson-0.3.92/old_clean.py
+-rw-r--r--   0        0        0     5166 2024-01-23 01:31:29.806260 robolson-0.3.92/old_mail.py
+-rw-r--r--   0        0        0        0 2022-05-21 03:18:36.761960 robolson-0.3.92/parser/__init__.py
+-rw-r--r--   0        0        0     1119 2023-01-14 21:30:02.931167 robolson-0.3.92/parser/clean_parser.py
+-rw-r--r--   0        0        0     1220 2022-07-08 10:11:15.790934 robolson-0.3.92/parser/email_parser.py
+-rw-r--r--   0        0        0     1770 2022-04-08 02:11:14.941735 robolson-0.3.92/parser/ffmpeg_parser.py
+-rw-r--r--   0        0        0     1509 2023-02-06 13:43:39.345746 robolson-0.3.92/parser/reddit_parser.py
+-rw-r--r--   0        0        0      909 2022-07-04 01:50:11.624597 robolson-0.3.92/parser/tick_parser.py
+-rw-r--r--   0        0        0    71203 2024-01-26 07:47:28.692623 robolson-0.3.92/poetry.lock
+-rw-r--r--   0        0        0     1244 2024-05-23 02:22:31.447164 robolson-0.3.92/pyproject.toml
+-rw-r--r--   0        0        0     8401 2023-02-06 13:44:14.394052 robolson-0.3.92/reddit_archive.py
+-rw-r--r--   0        0        0     4153 2023-02-27 21:47:08.721554 robolson-0.3.92/robai.py
+-rw-r--r--   0        0        0        0 2024-01-23 01:31:29.814265 robolson-0.3.92/tests/__init__.py
+-rw-r--r--   0        0        0     1021 2024-04-23 05:40:47.039937 robolson-0.3.92/tests/test_algebra.py
+-rw-r--r--   0        0        0      970 2024-01-23 01:31:29.815258 robolson-0.3.92/tests/test_clean.py
+-rw-r--r--   0        0        0     5978 2023-02-08 17:22:46.858389 robolson-0.3.92/tick.py
+-rw-r--r--   0        0        0        0 2022-04-07 19:21:12.560000 robolson-0.3.92/ticktick/__init__.py
+-rw-r--r--   0        0        0    24751 2022-05-09 07:55:23.045790 robolson-0.3.92/ticktick/api.py
+-rw-r--r--   0        0        0     1473 2022-05-02 00:50:17.516634 robolson-0.3.92/ticktick/cache.py
+-rw-r--r--   0        0        0        0 2022-04-07 19:21:12.670000 robolson-0.3.92/ticktick/helpers/__init__.py
+-rw-r--r--   0        0        0       68 2022-04-07 19:21:12.699905 robolson-0.3.92/ticktick/helpers/constants.py
+-rw-r--r--   0        0        0     1184 2022-05-02 00:50:17.590600 robolson-0.3.92/ticktick/helpers/hex_color.py
+-rw-r--r--   0        0        0     2787 2022-05-09 07:49:04.451389 robolson-0.3.92/ticktick/helpers/time_methods.py
+-rw-r--r--   0        0        0     8805 2022-04-08 04:12:37.380147 robolson-0.3.92/ticktick/helpers/timezones.txt
+-rw-r--r--   0        0        0        0 2022-04-07 19:21:12.804000 robolson-0.3.92/ticktick/managers/__init__.py
+-rw-r--r--   0        0        0      444 2022-05-02 00:50:18.497442 robolson-0.3.92/ticktick/managers/check_logged_in.py
+-rw-r--r--   0        0        0      408 2022-05-02 00:50:18.510446 robolson-0.3.92/ticktick/managers/focus.py
+-rw-r--r--   0        0        0     4956 2022-05-02 00:50:18.524792 robolson-0.3.92/ticktick/managers/habits.py
+-rw-r--r--   0        0        0      334 2022-05-02 00:50:18.547793 robolson-0.3.92/ticktick/managers/pomo.py
+-rw-r--r--   0        0        0    43862 2022-06-11 04:09:26.134840 robolson-0.3.92/ticktick/managers/projects.py
+-rw-r--r--   0        0        0      429 2022-05-02 00:50:18.617905 robolson-0.3.92/ticktick/managers/settings.py
+-rw-r--r--   0        0        0    46804 2022-06-11 04:10:45.717520 robolson-0.3.92/ticktick/managers/tags.py
+-rw-r--r--   0        0        0    54311 2022-06-11 04:08:26.998571 robolson-0.3.92/ticktick/managers/tasks.py
+-rw-r--r--   0        0        0    13289 2022-05-09 07:54:06.826880 robolson-0.3.92/ticktick/oauth2.py
+-rw-r--r--   0        0        0     1135 2024-01-23 01:31:29.816259 robolson-0.3.92/tomldict.py
+-rw-r--r--   0        0        0      144 2024-02-13 23:10:05.116424 robolson-0.3.92/tomlshelve.py
+-rw-r--r--   0        0        0       24 2022-04-19 17:39:25.252880 robolson-0.3.92/tox.ini
+-rw-r--r--   0        0        0        0 2024-05-22 20:52:54.208516 robolson-0.3.92/utilities/__init__.py
+-rw-r--r--   0        0        0      381 2024-05-22 21:27:40.345662 robolson-0.3.92/utilities/perf_timer.py
+-rw-r--r--   0        0        0     1135 2024-01-23 01:31:29.816259 robolson-0.3.92/utilities/tomldict.py
+-rw-r--r--   0        0        0      144 2024-02-13 23:10:05.116424 robolson-0.3.92/utilities/tomlshelve.py
+-rw-r--r--   0        0        0      927 1970-01-01 00:00:00.000000 robolson-0.3.92/PKG-INFO
```

### Comparing `robolson-0.3.91/algebra.py` & `robolson-0.3.92/old_algebra.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/anagram.py` & `robolson-0.3.92/anagram.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/clean.py` & `robolson-0.3.92/clean.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/config/algebra/latex_templates.toml` & `robolson-0.3.92/config/algebra/latex_templates.toml`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/config/clean.toml` & `robolson-0.3.92/config/clean.toml`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/config/english/config.toml` & `robolson-0.3.92/config/english/config.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,7 @@
 [constants]
 weekdays = [ "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday",]
 months = [ "N/a", "Jan", "Feb", "March", "April", "May", "June", "July", "Aug", "Sept", "Oct", "Nov", "Dec",]
-instruction = """You are helping a student comprehend a passage by asking a few probing questions.  All questions should be one sentence at most.
 
-The first question begins:
-
-"Circle or highlight the section of the passage which ..."
-
-For the second question, pick an SAT style vocabulary word from the text and have the student define it.
-
-For 3rd and last question, ask a question that probes the reader's overall understanding of the passage."""
+[LLM]
+model = ""
+instruction = "You are helping a student comprehend a passage by asking a few probing questions.  All questions should be one sentence at most.\n\nThe first question begins:\n\n\"Circle or highlight the section of the passage which ...\"\n\nFor the second question, pick an SAT style vocabulary word from the text and have the student define it.\n\nFor 3rd and last question, ask a question that probes the reader's overall understanding of the passage."
```

### Comparing `robolson-0.3.91/data/word_list.txt` & `robolson-0.3.92/data/word_list.txt`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/english.py` & `robolson-0.3.92/homework.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,337 +1,398 @@
 import datetime
-import re
-from pathlib import Path
+import pathlib
+import random
+import sys
+import time
 
 import appdirs
 import survey
 import toml
 import typer
-from openai import OpenAI
 
-try:
-    from . import tomlshelve
+from .algebra.problems import *  # noqa: F403
 
-except ImportError:
-    import tomlshelve
+_DEBUG = True
+
+_typer_start = time.perf_counter()
 
 app = typer.Typer()
+algebra_app = typer.Typer()
 list_app = typer.Typer(no_args_is_help=True)
-app.add_typer(list_app, name="list")
+app.add_typer(algebra_app, name="algebra")
+algebra_app.add_typer(list_app, name="list")
 
-GPT_CLIENT = OpenAI()  # API key must be in environment as "OPENAI_API_KEY"
+if "english" in sys.argv:
+    import_english_start = time.perf_counter()
+    try:
+        from .english import app as english_app
+
+        # from .english import english_default
+    except ImportError:
+        from english import app as english_app
+
+        # from english import english_default
+
+    app.add_typer(
+        english_app,
+        name="english",
+        help="Prepare and generate English homework assignments.",
+    )
+    if _DEBUG:
+        import_english_stop = time.perf_counter()
+        print(
+            f"Finished importing english Typer app. ({import_english_stop - import_english_start:.3f}s)"
+        )
 
-_THIS_FILE = Path(__file__)
+_typer_stop = time.perf_counter()
 
-_BOOKS_FILE = (
-    Path(appdirs.user_data_dir(roaming=True)) / "robolson" / "english" / "data" / "books.toml"
-)
-_PROGRESS_FILE = (
-    Path(appdirs.user_data_dir(roaming=True)) / "robolson" / "english" / "data" / "progress.toml"
-)
-
-_BOOKS_FILE.parent.mkdir(parents=True, exist_ok=True)
-_PROGRESS_FILE.parent.mkdir(parents=True, exist_ok=True)
-
-_BOOKS_FILE.touch()
-_PROGRESS_FILE.touch()
-
-_LATEX_FILE = Path(_THIS_FILE.parent) / "config" / "english" / "latex_templates.toml"
-_LATEX_FILE.parent.mkdir(exist_ok=True)
-_LATEX_FILE.touch()
-LATEX_TEMPLATES = toml.loads(open(_LATEX_FILE.absolute(), "r").read())
-
-_LATEX_PAGE_HEADER = LATEX_TEMPLATES["page_header"]
-_LATEX_DOC_HEADER = LATEX_TEMPLATES["doc_header"]
-
-_CONFIG_FILE = Path(_THIS_FILE.parent) / "config" / "english" / "config.toml"
-_CONFIG_FILE.parent.mkdir(exist_ok=True)
-_CONFIG_FILE.touch()
-CONFIGURATION = toml.loads(open(_CONFIG_FILE.absolute(), "r").read())
-
-_WEEKDAYS = CONFIGURATION["constants"]["weekdays"]
-_MONTHS = CONFIGURATION["constants"]["months"]
-_SYSTEM_INSTRUCTION = CONFIGURATION["constants"]["instruction"]
-
-_LINES = r"""
-\\[12pt]
-\rule{\linewidth}{.5pt}
-\\[12pt]
-\rule{\linewidth}{.5pt}
-\\[12pt]
-\rule{\linewidth}{.5pt}
-\\[12pt]
-\rule{\linewidth}{.5pt}
-\\[12pt]
-\rule{\linewidth}{.5pt}
-\\
-Write a brief summary of the passage.
-\\[12pt]
-\rule{\linewidth}{.5pt}
-\\[12pt]
-\rule{\linewidth}{.5pt}
-\\[12pt]
-\rule{\linewidth}{.5pt}
-\\[12pt]
-\rule{\linewidth}{.5pt}
-\\[12pt]
-\rule{\linewidth}{.5pt}
-"""
-
-
-@app.command("ingest")
-def ingest_text_file(target: str, chars_per_page: int = 5_000, debug: bool = False):
-    """Import a (properly formatted) book.txt
-
-    line 1: Book Title
-    line 2: Book Author
-    CHAPTER 1 Optional Chapter Title
-    SUBSECTION IN ALL CAPS
-    One line of text per paragraph."""
-
-    target = Path(target).name
-
-    fp = open(target, "r", encoding="utf-8")
-    lines = fp.readlines()
-
-    title = lines[0].strip()
-    author = lines[1].strip()
-
-    text = "\n".join(lines[2:])
-
-    chapter_pattern = re.compile(r"( *CHAPTER (\d+) ?(.*))", re.IGNORECASE)
-    section_pattern = re.compile(r"\n[^a-z\n\.\?\]\)]+\??\n")
-    breakpoint()
-    book = []
-    for chapter in chapter_pattern.findall(text):
-        chapter_number = int(chapter[1])
-        chapter_name = chapter[2]
-        full_chapter = (
-            f"Chapter {chapter_number}{f': {chapter_name.title()}' if chapter_name else ''}"
-        )
-        split = text.split(str(chapter[0]))  # chapter[0] is the full match
-        chapter_text = split[1]
-        chapter_text = chapter_pattern.split(chapter_text)[0]
-        subsections = []
-
-        section_titles = section_pattern.findall(chapter_text)
-        section_titles = [e.strip() for e in section_titles]
-        section_titles.insert(0, full_chapter)
-        section_texts = section_pattern.sub(r"SPLIT_CHAPTER_HERE", chapter_text).split(
-            "SPLIT_CHAPTER_HERE"
-        )
+if _DEBUG:
+    print(f"Typer setup finished. ({_typer_stop - _typer_start:.3f} sec)")
 
-        for i, section_title in enumerate(section_titles):
-            subsections.append({"title": section_title, "text": section_texts[i].rstrip()})
 
-        for section in subsections:
-            section_length = len(section["text"])
-            page_count = section_length // chars_per_page + 1
-            if page_count > 1:
-                paragraphs = section["text"].split("\n")
-                paragraphs = [p for p in paragraphs if p]
-                paginated = []
-                page_counter = 0
-                while paragraphs:
-                    new_page = ""
-                    page_counter += 1
-                    while len(new_page) < section_length / page_count and paragraphs:
-                        new_page += f"\n\n \\indent {paragraphs[0]}"
-                        del paragraphs[0]
-
-                    # If remaining text is less than half the size of a normal excerpt
-                    # Then just append it to the penultimate excerpt
-                    if len("\n".join(paragraphs)) < chars_per_page / 2:
-                        while paragraphs:
-                            new_page += f"\n\n \\indent {paragraphs[0]}"
-                            del paragraphs[0]
-                    doc = {
-                        "title": section["title"] + f" (Part {page_counter})",
-                        "text": new_page,
-                    }
-
-                    paginated.append(doc)
-
-                for part in paginated:
-                    book.append(part)
-            else:
-                book.append(section)
+# @perf_timer(debug=_DEBUG)
+def prepare_disk_io():
+    start = time.perf_counter()
+    global _LATEX_FILE, _SAVE_FILE, _SAVE_DATA, _LATEX_TEMPLATES, _WEEKDAYS, _MONTHS, _VARIABLES, _START
+    _THIS_FILE = pathlib.Path(__file__)
+
+    _LATEX_FILE = _THIS_FILE.parent / "config" / "algebra" / "latex_templates.toml"
+    _LATEX_FILE.parent.mkdir(exist_ok=True)
+    _LATEX_TEMPLATES = toml.loads(open(_LATEX_FILE.absolute(), "r").read())
+
+    _SAVE_FILE = pathlib.Path(appdirs.user_data_dir()) / "robolson" / "algebra" / "config.toml"
+
+    if not _SAVE_FILE.exists():
+        # NEW_SAVE_FILE = pathlib.Path("data/algebra/save.toml")
+        NEW_SAVE_FILE = _THIS_FILE.parent / "config" / "algebra" / "config.toml"
+        _SAVE_DATA = toml.loads(open(NEW_SAVE_FILE.absolute(), "r").read())
+        _SAVE_FILE.parent.mkdir(exist_ok=True)
+        # _SAVE_FILE.touch()
+        toml.dump(o=_SAVE_DATA, f=open(_SAVE_FILE.name, "w"))
+
+    else:
+        _SAVE_DATA = toml.loads(open(_SAVE_FILE.absolute(), "r").read())
+
+    _WEEKDAYS = _SAVE_DATA["constants"]["weekdays"]
+    _MONTHS = _SAVE_DATA["constants"]["months"]
+    _VARIABLES = _SAVE_DATA["constants"]["variables"]
+
+    _START = datetime.datetime.today()
+    _DAYS = [_START + datetime.timedelta(days=i) for i in range(30)]
+    _DATES = [
+        f"{_WEEKDAYS[day.weekday()]} {_MONTHS[day.month]} {day.day}, {day.year}" for day in _DAYS
+    ]
+    stop = time.perf_counter()
+    if _DEBUG:
+        print(f"File i/o boilerplate executed. ({stop - start: .3f} sec)")
+
+
+class ProblemCategory:
+    """Represents a category of algebra problem.
+    Must supply the logic for generating a problem statement as a valid function.
+    Function must include a description of the problem type as the last line of its docstring.
+    """
+
+    def __init__(self, logic, weight: int):
+        self.name = logic.__name__
+        self.weight: int = weight
+        self.logic = logic
+        if logic.__doc__:
+            self.description = logic.__doc__.split("\n")[-1].strip()
+        else:
+            print(f"Problem generator requires docstring: {logic.__name__}")
+            exit(0)
+        self.long_description = f"{self.description} ({self.weight})"
 
-    breakpoint()
+    def generate(self):
+        """Return a tuple of strings ('problem statement', 'solution')"""
 
-    if not debug:
-        with tomlshelve.open(str(_BOOKS_FILE)) as db:
-            db[target] = {"book": book, "author": author, "title": title}
+        # return self.logic(self.weight)
 
-    # with tomlshelve.open(str(_BOOKS_FILE) + ".toml") as db:
-    #     breakpoint()
-    #     db[target] = {"book": book, "author": author, "title": title}
-
-
-@app.command("set-progress")
-def set_progress(target: str = None, progress: int = None):  # type: ignore
-    """Set progress for registered books.
-    Future generation will proceed from the progress point."""
-
-    with tomlshelve.open(str(_PROGRESS_FILE)) as progress_db:
-        if target and (progress is not None):
-            progress_db[target] = progress
-            return
-
-        with tomlshelve.open(_BOOKS_FILE) as db:
-            form = {
-                k: survey.widgets.Count(value=progress_db[k] if k in progress_db.keys() else 0)
-                for k in db.keys()
-            }
-        if form:
-            data = survey.routines.form("Set Progress:", form=form)
-            progress_db.update(data)
-        else:
-            print("No books have been ingested yet.  Aborting.")
-            exit(1)
+        problem, solution = self.logic(self.weight)
+        return Problem(problem, solution, self.name)
 
 
-@app.command("generate")
-def generate_pages(
-    target: str = None,  # type:ignore
-    n: int = 7,
-    debug: bool = True,
-    start_date: datetime.datetime = datetime.datetime.today(),
-):
-    if target is None:
-        with tomlshelve.open(_BOOKS_FILE) as db:
-            candidates = list(db.keys())
+class Problem:
+    """Represents a specific algebra problem and its solution."""
 
-            index = survey.routines.select(
-                "Select book to generate questions: ", options=candidates
-            )
-            if index is None:
-                print("No books ingested.  Aborting.")
-                exit(1)
+    def __init__(self, problem: str, solution: str, name: str):
+        self.problem = rf"\item {problem}"
+        self.solution = solution
+        self.name = name
 
-            target = candidates[index]
 
-    target = Path(target).name
+@list_app.command("weights")
+def list_weights() -> None:
+    """List the frequency weights for each problem type."""
+    prepare_globals()
 
-    with tomlshelve.open(str(_PROGRESS_FILE)) as db:
-        if target in db.keys():
-            PROGRESS_INDEX = db[target]
-        else:
-            db[target] = 0
-            PROGRESS_INDEX = 0
+    print(
+        "--------------------------------\nProblems start with 1000 weight.  \nWeight decreases exponentially with use.  \nProblems with smaller weight are less likely to appear in problem sets.  \nSome problem types will increase with difficulty as their weight decreases.  \n--------------------------------"
+    )
 
-    mytext = _LATEX_DOC_HEADER
-    # start = datetime.datetime.today()
-    days = [start_date + datetime.timedelta(days=i) for i in range(30)]
-    dates = [
-        f"{_WEEKDAYS[day.weekday()]} {_MONTHS[day.month]} {day.day}, {day.year}" for day in days
-    ]
+    for problem in _PROBLEM_GENERATORS:
+        statement = globals()[problem].__doc__.split("\n")[-1]
+        print(f"{statement}: {_SAVE_DATA['weights'][problem]}")
+
+
+@algebra_app.command("render")
+def render_latex(
+    assignment_count: int = 1,
+    problem_count: int = 4,
+    debug: bool = False,
+    threshold: int = 0,
+    problem_set=None,  # type: ignore Typer
+) -> None:
+    """Return a string coding for {assignment_count} pages of LaTeX algebra problems."""
+
+    prepare_globals()
+    prepare_disk_io()
+
+    if not problem_set or len(problem_set) == len(_ALL_PROBLEMS):
+        problem_set: list[ProblemCategory] = _ALL_PROBLEMS
+        problem_mass: int = 1000 * problem_count
+        filtered_set: list[ProblemCategory] = []
+        while problem_mass > 0 and len(filtered_set) < len(_ALL_PROBLEMS):
+            filtered_set.append(problem_set[0])
+            problem_set = problem_set[1:]
+            problem_mass -= filtered_set[-1].weight
+
+        problem_set = filtered_set
+
+    pages = []
+    solutions = []
+
+    doc_header = _LATEX_TEMPLATES["doc_header"]
+
+    for i in range(assignment_count):
+        solution_set = rf"{_DATES[i]}\\"
+        page_header = _LATEX_TEMPLATES["page_header"]
+        parts = page_header.split("INSERT_DATE_HERE")
+        page_header = _DATES[i].join(parts)
+
+        problem_statement = ""
+
+        problem_generators = random.sample(
+            problem_set,
+            k=problem_count,
+            counts=[problem.weight + problem_count + 1 for problem in problem_set],
+        )
 
-    # with shelve.open(_BOOKS_FILE.name) as db:
-    with tomlshelve.open(str(_BOOKS_FILE)) as db:
-        if target not in db.keys():
-            print(f"{target} not ingested.")
-            return
-
-        book = db[target]["book"]
-        title = db[target]["title"]
-        author = db[target]["author"]
-        book_size = len(book)
-        for index in range(n):
-            if not debug:
-                response = GPT_CLIENT.chat.completions.create(
-                    model="gpt-4",
-                    messages=[
-                        {"role": "system", "content": _SYSTEM_INSTRUCTION},
-                        {
-                            "role": "user",
-                            "content": book[(PROGRESS_INDEX + index) % book_size]["text"],
-                        },
-                    ],
-                )
-
-                questions = str(response.choices[0].message.content)
-                lines = questions.split("\n")
-
-                questions = [line for line in lines if len(line) > 0]
-                questions = [f"{i+1}.) {text}" for i, text in enumerate(questions)]
-                questions = "\n\n".join(questions)
-            else:
-                questions = "QUESTIONS GO HERE"
-            dated_header = re.sub("DATEGOESHERE", dates[index], _LATEX_PAGE_HEADER)
-            titled_header = re.sub("TITLEGOESHERE", title, dated_header)
-            authored_header = re.sub("AUTHORGOESHERE", author, titled_header)
-            mytext += f"{authored_header}\n\\section*{{{book[(PROGRESS_INDEX + index) % book_size]['title']}}}\n\n{book[(PROGRESS_INDEX + index) % book_size]['text']}\n\n{questions}{_LINES}\\newpage"
-
-        mytext = re.sub(pattern=r"&", repl=r"\\&", string=mytext)
-        if not debug:
-            fp = open(
-                f"English Reading {_MONTHS[datetime.datetime.now().month]} {datetime.datetime.now().day} {datetime.datetime.now().year}.tex",
-                "w",
-                encoding="utf-8",
+        problems: list[Problem] = [problem.generate() for problem in problem_generators]
+
+        for k, problem in enumerate(problems):
+            if k % 3 == 0 and k != 0:
+                problem_statement += r"\newpage"
+
+            problem_statement += problem.problem
+            solution_set += rf"{k+1}: {problem.solution}\;\;"
+
+            # _SAVE_DATA["weights"][problem.name] = int(_SAVE_DATA["weights"][problem.name] * 0.9)
+            _SAVE_DATA["weights"][problem.name] = int(
+                _SAVE_DATA["weights"].get(problem.name, 1000) * 0.9
             )
-            print(f"Writing English homework to {fp.name}")
-        else:
-            print("Use '--no-debug' to save progress.")
-            fp = open("English Sample.tex", "w", encoding="utf-8")
 
-        mytext += r"\end{document}"
+        page_footer = r"\end{enumerate}"
+        solutions.append(solution_set)
+        pages.append(page_header + problem_statement + page_footer)
 
-        fp.write(mytext)
-        fp.close()
+    doc_footer = r"\end{document}"
+
+    document = (
+        doc_header + r"\newpage".join(pages) + r"\newpage " + r"\\".join(solutions) + doc_footer
+    )
+
+    document_name = f"Algebra Homework {_MONTHS[datetime.datetime.now().month]} {datetime.datetime.now().day} {datetime.datetime.now().year}.tex"
+
+    print(f"Writing LaTeX document to '{document_name}")
+
+    fp = open(document_name, "w")
+    fp.write(document)
+    fp.close()
 
     if not debug:
-        with tomlshelve.open(str(_PROGRESS_FILE)) as db:
-            db[target] = PROGRESS_INDEX + n
+        toml.dump(o=_SAVE_DATA, f=open(_SAVE_FILE.absolute(), "w"))
 
 
-@list_app.command("books")
-def list_books():
-    """List available books and current progress."""
-    progress_db = tomlshelve.open(_PROGRESS_FILE)
-
-    with tomlshelve.open(_BOOKS_FILE) as db:
-        for book in db.keys():
-            try:
-                current_progress = progress_db[book]
-            except KeyError:
-                current_progress = 0
+@algebra_app.command("reset")
+def reset_weights(debug: bool = True):
+    """Reset problem frequency rates to default."""
 
-            print(f"{book} (Progress: {current_progress} / {len(db[book]['book'])})")
+    prepare_disk_io()
 
+    # weights: dict[str, int] = _SAVE_DATA["weights"]
+    for key in _SAVE_DATA["weights"].keys():
+        _SAVE_DATA["weights"][key] = 1000
+
+    if not debug:
+        toml.dump(o=_SAVE_DATA, f=open(_SAVE_FILE.absolute(), "w"))
+        print("Frequency weights reset to default (1000).")
+    else:
+        print("Invoke with --no-debug to save changes.")
+    exit(0)
+
+
+@algebra_app.command("config")
+def configure_problem_set():
+    """Configures the frequency rates of problems."""
+
+    prepare_globals()
+
+    form = {
+        _NAME_TO_DESCRIPTION[problem_type]: survey.widgets.Count(
+            value=_SAVE_DATA["weights"][problem_type]
+        )
+        for problem_type in _PROBLEM_GENERATORS
+    }
+
+    data = survey.routines.form("Frequency Weights (higher -> more frequent): ", form=form)
+
+    if not data:
+        return
+
+    data = {_DESCRIPTION_TO_NAME[desc]: data[desc] for desc in data.keys()}
+    _SAVE_DATA["weights"] = data
+    toml.dump(o=_SAVE_DATA, f=open(_SAVE_FILE.absolute(), "w"))
+    print(f"\nNew weights saved to {_SAVE_FILE.absolute()}")
+
+
+@algebra_app.callback(invoke_without_command=True)
+def algebra_default(ctx: typer.Context, debug: bool = False):
+    """Manage and generate algebra homework assignments."""
 
-@app.callback(invoke_without_command=True)
-def english_default(ctx: typer.Context):
     if ctx and ctx.invoked_subcommand:
         return
 
-    available_books = list(tomlshelve.open(_BOOKS_FILE).keys())
-    book_choice = survey.routines.select("Select a book: ", options=available_books)
-    book_choice = available_books[book_choice]
+    prepare_globals()
+
+    problem_indeces = survey.routines.basket(
+        "Select problem types to include.  (Numbers indicate relative frequency rate.)",
+        options=[problem.long_description for problem in _ALL_PROBLEMS],
+    )
+
+    selected_problems = [_ALL_PROBLEMS[i] for i in problem_indeces]  # type: ignore
 
     start_date = survey.routines.datetime(
         "Select assignment start date: ",
         attrs=("month", "day", "year"),
     )
-
     if not start_date:
         start_date = datetime.datetime.today()
 
     assignment_count = survey.routines.numeric(
-        "How many reading assignments to generate? ", decimal=False, value=5
+        "How many algebra assignments to generate? ", decimal=False, value=5
     )
 
-    debug_status = survey.routines.inquire("Debug? ", default=True)
+    if not assignment_count:
+        assignment_count = 5
 
-    generate_pages(
-        target=book_choice,
-        n=assignment_count,
-        start_date=start_date,
-        debug=debug_status,
+    problem_count = survey.routines.numeric(
+        "How many problems per assignment? ", decimal=False, value=4
     )
 
+    if not problem_count:
+        problem_count = 4
 
-if __name__ == "__main__":
+    days = [start_date + datetime.timedelta(days=i) for i in range(assignment_count + 1)]
+
+    global _DATES
+    _DATES = [
+        f"{_WEEKDAYS[day.weekday()]} {_MONTHS[day.month]} {day.day}, {day.year}" for day in days
+    ]
+
+    render_latex(
+        assignment_count=assignment_count,
+        problem_count=problem_count,
+        debug=debug,
+        problem_set=selected_problems,
+    )
+
+
+@list_app.callback(invoke_without_command=True)
+def list_default(ctx: typer.Context):
+    """List problem types, frequency weights, etc."""
+    if ctx.invoked_subcommand:
+        return
+
+    print("???")
+    list_app.rich_help_panel
+
+
+@app.callback(invoke_without_command=True)
+def default_homework(ctx: typer.Context):
+    if ctx and ctx.invoked_subcommand:
+        return
+
+    available_apps = ["algebra", "english"]
+
+    choice = survey.routines.select("Select the homework generation app: ", options=available_apps)
+
+    choice = available_apps[choice]
+
+    match choice:
+        case "algebra":
+            algebra_default(ctx=None)
+
+        case "english":
+            from .english import english_default
+
+            english_default(ctx=None)
+
+
+def main():
+    # default_homework(None)
     app()
-    # ingest_text_file(debug=False)
-    # generate_pages(7, debug=False)
-    # db = shelve.open(_BOOKS_FILE.name)
+
+
+_PROBLEM_GENERATORS = []
+_ALL_PROBLEMS = []
+_NAME_TO_DESCRIPTION = {}
+_DESCRIPTION_TO_NAME = {}
+
+
+def prepare_globals():
+    global _PROBLEM_GENERATORS, _ALL_PROBLEMS, _NAME_TO_DESCRIPTION, _DESCRIPTION_TO_NAME
+
+    prepare_disk_io()
+
+    _problem_dict = {k: v for k, v in globals().items() if k.startswith("generate") and callable(v)}
+    _PROBLEM_GENERATORS = [k for k in _problem_dict.keys()]
+
+    _ALL_PROBLEMS = [
+        ProblemCategory(logic=logic, weight=int(_SAVE_DATA["weights"].get(name, 1000)))
+        for name, logic in _problem_dict.items()
+    ]
+
+    for problem in _ALL_PROBLEMS:
+        if problem.weight is None:
+            problem.weight = 1000
+            _SAVE_DATA["weights"][problem.name] = 1000
+
+    # mapping of problem function name to problem description
+    _NAME_TO_DESCRIPTION = {
+        name: globals()[name].__doc__.split("\n")[-1].strip() for name in _PROBLEM_GENERATORS
+    }
+
+    # mapping of problem description to problem function name
+    _DESCRIPTION_TO_NAME = {
+        globals()[name].__doc__.split("\n")[-1].strip(): name for name in _PROBLEM_GENERATORS
+    }
+
+    removed_old_generator = False
+    for generator in list(_SAVE_DATA["weights"].keys()):
+        if generator not in globals().keys():
+            del _SAVE_DATA["weights"][generator]
+            removed_old_generator = True
+
+    if removed_old_generator:
+        _SAVE_DATA["constants"]["weekdays"] = _WEEKDAYS
+        _SAVE_DATA["constants"]["months"] = _MONTHS
+        _SAVE_DATA["constants"]["variables"] = _VARIABLES
+
+        toml.dump(o=_SAVE_DATA, f=open(_SAVE_FILE.absolute(), "w"))
+
+
+# _problem_dict = { =_SAVE_DATA, f=open(_SAVE_FILE.absolute(), "w"))
+
+if __name__ == "__main__":
+    main()
```

### Comparing `robolson-0.3.91/ffmpeg.py` & `robolson-0.3.92/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/help.py` & `robolson-0.3.92/help.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/hierarchy.py` & `robolson-0.3.92/hierarchy.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/loggers/tick_logger.py` & `robolson-0.3.92/loggers/tick_logger.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 import os
 from pathlib import Path
 
 import appdirs
 
 _LOG_FILE = Path(appdirs.user_data_dir()) / "robolson" / "tick" / "LOG.txt"
 
+
 if not _LOG_FILE.exists():
-    os.makedirs(_LOG_FILE.parent, exist_ok=True)
+    _LOG_FILE.parent.mkdir(parents=True, exist_ok=True)
+    _LOG_FILE.touch(exist_ok=True)
+    # os.makedirs(_LOG_FILE.parent, exist_ok=True)
 
 
 class StreamToLogger(object):
     """
     Fake file-like stream object that redirects writes to a logger instance.
     """
```

### Comparing `robolson-0.3.91/night.py` & `robolson-0.3.92/night.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/old_clean.py` & `robolson-0.3.92/old_clean.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/old_mail.py` & `robolson-0.3.92/old_mail.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/parser/clean_parser.py` & `robolson-0.3.92/parser/clean_parser.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/parser/email_parser.py` & `robolson-0.3.92/parser/email_parser.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/parser/ffmpeg_parser.py` & `robolson-0.3.92/parser/ffmpeg_parser.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/parser/reddit_parser.py` & `robolson-0.3.92/parser/reddit_parser.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/parser/tick_parser.py` & `robolson-0.3.92/parser/tick_parser.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/poetry.lock` & `robolson-0.3.92/poetry.lock`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/pyproject.toml` & `robolson-0.3.92/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robolson"
-version = "0.3.91"
+version = "0.3.92"
 description = "My collection of utilty scripts"
 authors = ["Rob L Olson <rob.louis@gmail.com>"]
 include = ["config/clean.toml", "config/english/latex_templates.toml", "config/english/config.toml", "config/algebra/config.toml", "config/english/latex_templates.toml", "pyproject.toml", "data/word_list.txt"]
 exclude = []
 packages = [
     {include="rob", from=".."},
     {include="parser"},
```

### Comparing `robolson-0.3.91/reddit_archive.py` & `robolson-0.3.92/reddit_archive.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/robai.py` & `robolson-0.3.92/robai.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/tests/test_algebra.py` & `robolson-0.3.92/tests/test_algebra.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 import pytest
 
-from ..algebra import Binomial, Term, UnlikeTermsError
+from ..old_algebra import Binomial, Term, UnlikeTermsError
 
 
 def test_Terms():
     assert Term(1)
     assert Term("2x^2")
     assert Term(2) + Term(2) == Term(4)
     assert Term(3) * Term(3) == Term(9)
```

### Comparing `robolson-0.3.91/tests/test_clean.py` & `robolson-0.3.92/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/tick.py` & `robolson-0.3.92/tick.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/ticktick/api.py` & `robolson-0.3.92/ticktick/api.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/ticktick/cache.py` & `robolson-0.3.92/ticktick/cache.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/ticktick/helpers/hex_color.py` & `robolson-0.3.92/ticktick/helpers/hex_color.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/ticktick/helpers/time_methods.py` & `robolson-0.3.92/ticktick/helpers/time_methods.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/ticktick/helpers/timezones.txt` & `robolson-0.3.92/ticktick/helpers/timezones.txt`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/ticktick/managers/habits.py` & `robolson-0.3.92/ticktick/managers/habits.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/ticktick/managers/projects.py` & `robolson-0.3.92/ticktick/managers/projects.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/ticktick/managers/tags.py` & `robolson-0.3.92/ticktick/managers/tags.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/ticktick/managers/tasks.py` & `robolson-0.3.92/ticktick/managers/tasks.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/ticktick/oauth2.py` & `robolson-0.3.92/ticktick/oauth2.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/tomldict.py` & `robolson-0.3.92/tomldict.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.91/PKG-INFO` & `robolson-0.3.92/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robolson
-Version: 0.3.91
+Version: 0.3.92
 Summary: My collection of utilty scripts
 Author: Rob L Olson
 Author-email: rob.louis@gmail.com
 Requires-Python: >=3.9.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

