# Comparing `tmp/vocabulary_quiz-0.4.tar.gz` & `tmp/vocabulary_quiz-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocabulary_quiz-0.4.tar", last modified: Wed May 22 23:14:10 2024, max compression
+gzip compressed data, was "vocabulary_quiz-0.5.tar", last modified: Wed May 22 23:33:38 2024, max compression
```

## Comparing `vocabulary_quiz-0.4.tar` & `vocabulary_quiz-0.5.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 song-yongchan   (501) staff       (20)        0 2024-05-22 23:14:10.333807 vocabulary_quiz-0.4/
-drwxr-xr-x   0 song-yongchan   (501) staff       (20)        0 2024-05-22 23:14:10.330062 vocabulary_quiz-0.4/App/
--rw-r--r--   0 song-yongchan   (501) staff       (20)      216 2024-05-22 14:33:11.000000 vocabulary_quiz-0.4/App/__init__.py
--rw-r--r--   0 song-yongchan   (501) staff       (20)       61 2024-05-22 23:03:38.000000 vocabulary_quiz-0.4/App/__main__.py
--rw-r--r--   0 song-yongchan   (501) staff       (20)     5461 2024-05-22 23:08:09.000000 vocabulary_quiz-0.4/App/app.py
--rw-r--r--   0 song-yongchan   (501) staff       (20)     2720 2024-05-22 14:43:13.000000 vocabulary_quiz-0.4/App/routes.py
-drwxr-xr-x   0 song-yongchan   (501) staff       (20)        0 2024-05-22 23:14:10.330317 vocabulary_quiz-0.4/App/static/
--rw-r--r--   0 song-yongchan   (501) staff       (20)      766 2024-05-22 14:24:58.000000 vocabulary_quiz-0.4/App/static/style.css
-drwxr-xr-x   0 song-yongchan   (501) staff       (20)        0 2024-05-22 23:14:10.332356 vocabulary_quiz-0.4/App/templates/
--rw-r--r--   0 song-yongchan   (501) staff       (20)     1259 2024-05-22 14:43:32.000000 vocabulary_quiz-0.4/App/templates/index.html
--rw-r--r--   0 song-yongchan   (501) staff       (20)      717 2024-05-22 14:24:42.000000 vocabulary_quiz-0.4/App/templates/quiz.html
--rw-r--r--   0 song-yongchan   (501) staff       (20)      250 2024-05-21 10:42:58.000000 vocabulary_quiz-0.4/App/templates/result.html
--rw-r--r--   0 song-yongchan   (501) staff       (20)      590 2024-05-22 14:24:48.000000 vocabulary_quiz-0.4/App/templates/scores.html
--rw-r--r--   0 song-yongchan   (501) staff       (20)      598 2024-05-22 14:13:42.000000 vocabulary_quiz-0.4/App/templates/start_quiz.html
--rw-r--r--   0 song-yongchan   (501) staff       (20)      113 2024-05-22 13:55:16.000000 vocabulary_quiz-0.4/App/templates/view_scores.html
--rw-r--r--   0 song-yongchan   (501) staff       (20)      102 2024-05-22 14:45:06.000000 vocabulary_quiz-0.4/MANIFEST.in
--rw-r--r--   0 song-yongchan   (501) staff       (20)       57 2024-05-22 23:14:10.333656 vocabulary_quiz-0.4/PKG-INFO
--rw-r--r--   0 song-yongchan   (501) staff       (20)       38 2024-05-22 23:14:10.333875 vocabulary_quiz-0.4/setup.cfg
--rw-r--r--   0 song-yongchan   (501) staff       (20)      400 2024-05-22 23:14:03.000000 vocabulary_quiz-0.4/setup.py
-drwxr-xr-x   0 song-yongchan   (501) staff       (20)        0 2024-05-22 23:14:10.333433 vocabulary_quiz-0.4/vocabulary_quiz.egg-info/
--rw-r--r--   0 song-yongchan   (501) staff       (20)       57 2024-05-22 23:14:10.000000 vocabulary_quiz-0.4/vocabulary_quiz.egg-info/PKG-INFO
--rw-r--r--   0 song-yongchan   (501) staff       (20)      506 2024-05-22 23:14:10.000000 vocabulary_quiz-0.4/vocabulary_quiz.egg-info/SOURCES.txt
--rw-r--r--   0 song-yongchan   (501) staff       (20)        1 2024-05-22 23:14:10.000000 vocabulary_quiz-0.4/vocabulary_quiz.egg-info/dependency_links.txt
--rw-r--r--   0 song-yongchan   (501) staff       (20)       49 2024-05-22 23:14:10.000000 vocabulary_quiz-0.4/vocabulary_quiz.egg-info/entry_points.txt
--rw-r--r--   0 song-yongchan   (501) staff       (20)       30 2024-05-22 23:14:10.000000 vocabulary_quiz-0.4/vocabulary_quiz.egg-info/requires.txt
--rw-r--r--   0 song-yongchan   (501) staff       (20)        4 2024-05-22 23:14:10.000000 vocabulary_quiz-0.4/vocabulary_quiz.egg-info/top_level.txt
--rw-r--r--   0 song-yongchan   (501) staff       (20)     3432 2024-05-21 10:17:30.000000 vocabulary_quiz-0.4/words.csv
+drwxr-xr-x   0 song-yongchan   (501) staff       (20)        0 2024-05-22 23:33:38.022000 vocabulary_quiz-0.5/
+drwxr-xr-x   0 song-yongchan   (501) staff       (20)        0 2024-05-22 23:33:38.018860 vocabulary_quiz-0.5/App/
+-rw-r--r--   0 song-yongchan   (501) staff       (20)      215 2024-05-22 23:28:05.000000 vocabulary_quiz-0.5/App/__init__.py
+-rw-r--r--   0 song-yongchan   (501) staff       (20)       61 2024-05-22 23:03:38.000000 vocabulary_quiz-0.5/App/__main__.py
+-rw-r--r--   0 song-yongchan   (501) staff       (20)     5461 2024-05-22 23:08:09.000000 vocabulary_quiz-0.5/App/app.py
+-rw-r--r--   0 song-yongchan   (501) staff       (20)     5288 2024-05-22 23:27:52.000000 vocabulary_quiz-0.5/App/routes.py
+drwxr-xr-x   0 song-yongchan   (501) staff       (20)        0 2024-05-22 23:33:38.019173 vocabulary_quiz-0.5/App/static/
+-rw-r--r--   0 song-yongchan   (501) staff       (20)      766 2024-05-22 14:24:58.000000 vocabulary_quiz-0.5/App/static/style.css
+drwxr-xr-x   0 song-yongchan   (501) staff       (20)        0 2024-05-22 23:33:38.020773 vocabulary_quiz-0.5/App/templates/
+-rw-r--r--   0 song-yongchan   (501) staff       (20)     1259 2024-05-22 14:43:32.000000 vocabulary_quiz-0.5/App/templates/index.html
+-rw-r--r--   0 song-yongchan   (501) staff       (20)      717 2024-05-22 14:24:42.000000 vocabulary_quiz-0.5/App/templates/quiz.html
+-rw-r--r--   0 song-yongchan   (501) staff       (20)      250 2024-05-21 10:42:58.000000 vocabulary_quiz-0.5/App/templates/result.html
+-rw-r--r--   0 song-yongchan   (501) staff       (20)      590 2024-05-22 14:24:48.000000 vocabulary_quiz-0.5/App/templates/scores.html
+-rw-r--r--   0 song-yongchan   (501) staff       (20)      598 2024-05-22 14:13:42.000000 vocabulary_quiz-0.5/App/templates/start_quiz.html
+-rw-r--r--   0 song-yongchan   (501) staff       (20)      113 2024-05-22 13:55:16.000000 vocabulary_quiz-0.5/App/templates/view_scores.html
+-rw-r--r--   0 song-yongchan   (501) staff       (20)      102 2024-05-22 14:45:06.000000 vocabulary_quiz-0.5/MANIFEST.in
+-rw-r--r--   0 song-yongchan   (501) staff       (20)       57 2024-05-22 23:33:38.021865 vocabulary_quiz-0.5/PKG-INFO
+-rw-r--r--   0 song-yongchan   (501) staff       (20)      869 2024-05-22 23:30:52.000000 vocabulary_quiz-0.5/README.md
+-rw-r--r--   0 song-yongchan   (501) staff       (20)       38 2024-05-22 23:33:38.022041 vocabulary_quiz-0.5/setup.cfg
+-rw-r--r--   0 song-yongchan   (501) staff       (20)      431 2024-05-22 23:33:27.000000 vocabulary_quiz-0.5/setup.py
+drwxr-xr-x   0 song-yongchan   (501) staff       (20)        0 2024-05-22 23:33:38.021676 vocabulary_quiz-0.5/vocabulary_quiz.egg-info/
+-rw-r--r--   0 song-yongchan   (501) staff       (20)       57 2024-05-22 23:33:37.000000 vocabulary_quiz-0.5/vocabulary_quiz.egg-info/PKG-INFO
+-rw-r--r--   0 song-yongchan   (501) staff       (20)      573 2024-05-22 23:33:37.000000 vocabulary_quiz-0.5/vocabulary_quiz.egg-info/SOURCES.txt
+-rw-r--r--   0 song-yongchan   (501) staff       (20)        1 2024-05-22 23:33:37.000000 vocabulary_quiz-0.5/vocabulary_quiz.egg-info/dependency_links.txt
+-rw-r--r--   0 song-yongchan   (501) staff       (20)       54 2024-05-22 23:33:37.000000 vocabulary_quiz-0.5/vocabulary_quiz.egg-info/entry_points.txt
+-rw-r--r--   0 song-yongchan   (501) staff       (20)       30 2024-05-22 23:33:37.000000 vocabulary_quiz-0.5/vocabulary_quiz.egg-info/requires.txt
+-rw-r--r--   0 song-yongchan   (501) staff       (20)        4 2024-05-22 23:33:37.000000 vocabulary_quiz-0.5/vocabulary_quiz.egg-info/top_level.txt
+-rw-r--r--   0 song-yongchan   (501) staff       (20)     3432 2024-05-22 23:28:40.000000 vocabulary_quiz-0.5/words.csv
```

### Comparing `vocabulary_quiz-0.4/App/app.py` & `vocabulary_quiz-0.5/App/app.py`

 * *Files identical despite different names*

### Comparing `vocabulary_quiz-0.4/App/static/style.css` & `vocabulary_quiz-0.5/App/static/style.css`

 * *Files identical despite different names*

### Comparing `vocabulary_quiz-0.4/App/templates/index.html` & `vocabulary_quiz-0.5/App/templates/index.html`

 * *Files identical despite different names*

### Comparing `vocabulary_quiz-0.4/App/templates/quiz.html` & `vocabulary_quiz-0.5/App/templates/quiz.html`

 * *Files identical despite different names*

### Comparing `vocabulary_quiz-0.4/App/templates/scores.html` & `vocabulary_quiz-0.5/App/templates/scores.html`

 * *Files identical despite different names*

### Comparing `vocabulary_quiz-0.4/App/templates/start_quiz.html` & `vocabulary_quiz-0.5/App/templates/start_quiz.html`

 * *Files identical despite different names*

### Comparing `vocabulary_quiz-0.4/words.csv` & `vocabulary_quiz-0.5/words.csv`

 * *Files identical despite different names*

