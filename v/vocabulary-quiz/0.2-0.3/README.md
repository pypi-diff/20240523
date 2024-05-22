# Comparing `tmp/vocabulary_quiz-0.2.tar.gz` & `tmp/vocabulary_quiz-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocabulary_quiz-0.2.tar", last modified: Wed May 22 22:58:00 2024, max compression
+gzip compressed data, was "vocabulary_quiz-0.3.tar", last modified: Wed May 22 23:11:05 2024, max compression
```

## Comparing `vocabulary_quiz-0.2.tar` & `vocabulary_quiz-0.3.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 song-yongchan   (501) staff       (20)        0 2024-05-22 22:58:00.055564 vocabulary_quiz-0.2/
-drwxr-xr-x   0 song-yongchan   (501) staff       (20)        0 2024-05-22 22:58:00.052585 vocabulary_quiz-0.2/App/
--rw-r--r--   0 song-yongchan   (501) staff       (20)      216 2024-05-22 14:33:11.000000 vocabulary_quiz-0.2/App/__init__.py
--rw-r--r--   0 song-yongchan   (501) staff       (20)     5448 2024-05-22 14:35:16.000000 vocabulary_quiz-0.2/App/app.py
--rw-r--r--   0 song-yongchan   (501) staff       (20)     2720 2024-05-22 14:43:13.000000 vocabulary_quiz-0.2/App/routes.py
-drwxr-xr-x   0 song-yongchan   (501) staff       (20)        0 2024-05-22 22:58:00.052797 vocabulary_quiz-0.2/App/static/
--rw-r--r--   0 song-yongchan   (501) staff       (20)      766 2024-05-22 14:24:58.000000 vocabulary_quiz-0.2/App/static/style.css
-drwxr-xr-x   0 song-yongchan   (501) staff       (20)        0 2024-05-22 22:58:00.054383 vocabulary_quiz-0.2/App/templates/
--rw-r--r--   0 song-yongchan   (501) staff       (20)     1259 2024-05-22 14:43:32.000000 vocabulary_quiz-0.2/App/templates/index.html
--rw-r--r--   0 song-yongchan   (501) staff       (20)      717 2024-05-22 14:24:42.000000 vocabulary_quiz-0.2/App/templates/quiz.html
--rw-r--r--   0 song-yongchan   (501) staff       (20)      250 2024-05-21 10:42:58.000000 vocabulary_quiz-0.2/App/templates/result.html
--rw-r--r--   0 song-yongchan   (501) staff       (20)      590 2024-05-22 14:24:48.000000 vocabulary_quiz-0.2/App/templates/scores.html
--rw-r--r--   0 song-yongchan   (501) staff       (20)      598 2024-05-22 14:13:42.000000 vocabulary_quiz-0.2/App/templates/start_quiz.html
--rw-r--r--   0 song-yongchan   (501) staff       (20)      113 2024-05-22 13:55:16.000000 vocabulary_quiz-0.2/App/templates/view_scores.html
--rw-r--r--   0 song-yongchan   (501) staff       (20)      102 2024-05-22 14:45:06.000000 vocabulary_quiz-0.2/MANIFEST.in
--rw-r--r--   0 song-yongchan   (501) staff       (20)       57 2024-05-22 22:58:00.055431 vocabulary_quiz-0.2/PKG-INFO
--rw-r--r--   0 song-yongchan   (501) staff       (20)       38 2024-05-22 22:58:00.055611 vocabulary_quiz-0.2/setup.cfg
--rw-r--r--   0 song-yongchan   (501) staff       (20)      399 2024-05-22 22:56:33.000000 vocabulary_quiz-0.2/setup.py
-drwxr-xr-x   0 song-yongchan   (501) staff       (20)        0 2024-05-22 22:58:00.055259 vocabulary_quiz-0.2/vocabulary_quiz.egg-info/
--rw-r--r--   0 song-yongchan   (501) staff       (20)       57 2024-05-22 22:58:00.000000 vocabulary_quiz-0.2/vocabulary_quiz.egg-info/PKG-INFO
--rw-r--r--   0 song-yongchan   (501) staff       (20)      490 2024-05-22 22:58:00.000000 vocabulary_quiz-0.2/vocabulary_quiz.egg-info/SOURCES.txt
--rw-r--r--   0 song-yongchan   (501) staff       (20)        1 2024-05-22 22:58:00.000000 vocabulary_quiz-0.2/vocabulary_quiz.egg-info/dependency_links.txt
--rw-r--r--   0 song-yongchan   (501) staff       (20)       48 2024-05-22 22:58:00.000000 vocabulary_quiz-0.2/vocabulary_quiz.egg-info/entry_points.txt
--rw-r--r--   0 song-yongchan   (501) staff       (20)       30 2024-05-22 22:58:00.000000 vocabulary_quiz-0.2/vocabulary_quiz.egg-info/requires.txt
--rw-r--r--   0 song-yongchan   (501) staff       (20)        4 2024-05-22 22:58:00.000000 vocabulary_quiz-0.2/vocabulary_quiz.egg-info/top_level.txt
--rw-r--r--   0 song-yongchan   (501) staff       (20)     3432 2024-05-21 10:17:30.000000 vocabulary_quiz-0.2/words.csv
+drwxr-xr-x   0 song-yongchan   (501) staff       (20)        0 2024-05-22 23:11:05.215991 vocabulary_quiz-0.3/
+drwxr-xr-x   0 song-yongchan   (501) staff       (20)        0 2024-05-22 23:11:05.213073 vocabulary_quiz-0.3/App/
+-rw-r--r--   0 song-yongchan   (501) staff       (20)      216 2024-05-22 14:33:11.000000 vocabulary_quiz-0.3/App/__init__.py
+-rw-r--r--   0 song-yongchan   (501) staff       (20)       61 2024-05-22 23:03:38.000000 vocabulary_quiz-0.3/App/__main__.py
+-rw-r--r--   0 song-yongchan   (501) staff       (20)     5461 2024-05-22 23:08:09.000000 vocabulary_quiz-0.3/App/app.py
+-rw-r--r--   0 song-yongchan   (501) staff       (20)     2720 2024-05-22 14:43:13.000000 vocabulary_quiz-0.3/App/routes.py
+drwxr-xr-x   0 song-yongchan   (501) staff       (20)        0 2024-05-22 23:11:05.213283 vocabulary_quiz-0.3/App/static/
+-rw-r--r--   0 song-yongchan   (501) staff       (20)      766 2024-05-22 14:24:58.000000 vocabulary_quiz-0.3/App/static/style.css
+drwxr-xr-x   0 song-yongchan   (501) staff       (20)        0 2024-05-22 23:11:05.214851 vocabulary_quiz-0.3/App/templates/
+-rw-r--r--   0 song-yongchan   (501) staff       (20)     1259 2024-05-22 14:43:32.000000 vocabulary_quiz-0.3/App/templates/index.html
+-rw-r--r--   0 song-yongchan   (501) staff       (20)      717 2024-05-22 14:24:42.000000 vocabulary_quiz-0.3/App/templates/quiz.html
+-rw-r--r--   0 song-yongchan   (501) staff       (20)      250 2024-05-21 10:42:58.000000 vocabulary_quiz-0.3/App/templates/result.html
+-rw-r--r--   0 song-yongchan   (501) staff       (20)      590 2024-05-22 14:24:48.000000 vocabulary_quiz-0.3/App/templates/scores.html
+-rw-r--r--   0 song-yongchan   (501) staff       (20)      598 2024-05-22 14:13:42.000000 vocabulary_quiz-0.3/App/templates/start_quiz.html
+-rw-r--r--   0 song-yongchan   (501) staff       (20)      113 2024-05-22 13:55:16.000000 vocabulary_quiz-0.3/App/templates/view_scores.html
+-rw-r--r--   0 song-yongchan   (501) staff       (20)      102 2024-05-22 14:45:06.000000 vocabulary_quiz-0.3/MANIFEST.in
+-rw-r--r--   0 song-yongchan   (501) staff       (20)       57 2024-05-22 23:11:05.215863 vocabulary_quiz-0.3/PKG-INFO
+-rw-r--r--   0 song-yongchan   (501) staff       (20)       38 2024-05-22 23:11:05.216036 vocabulary_quiz-0.3/setup.cfg
+-rw-r--r--   0 song-yongchan   (501) staff       (20)      400 2024-05-22 23:10:59.000000 vocabulary_quiz-0.3/setup.py
+drwxr-xr-x   0 song-yongchan   (501) staff       (20)        0 2024-05-22 23:11:05.215711 vocabulary_quiz-0.3/vocabulary_quiz.egg-info/
+-rw-r--r--   0 song-yongchan   (501) staff       (20)       57 2024-05-22 23:11:05.000000 vocabulary_quiz-0.3/vocabulary_quiz.egg-info/PKG-INFO
+-rw-r--r--   0 song-yongchan   (501) staff       (20)      506 2024-05-22 23:11:05.000000 vocabulary_quiz-0.3/vocabulary_quiz.egg-info/SOURCES.txt
+-rw-r--r--   0 song-yongchan   (501) staff       (20)        1 2024-05-22 23:11:05.000000 vocabulary_quiz-0.3/vocabulary_quiz.egg-info/dependency_links.txt
+-rw-r--r--   0 song-yongchan   (501) staff       (20)       49 2024-05-22 23:11:05.000000 vocabulary_quiz-0.3/vocabulary_quiz.egg-info/entry_points.txt
+-rw-r--r--   0 song-yongchan   (501) staff       (20)       30 2024-05-22 23:11:05.000000 vocabulary_quiz-0.3/vocabulary_quiz.egg-info/requires.txt
+-rw-r--r--   0 song-yongchan   (501) staff       (20)        4 2024-05-22 23:11:05.000000 vocabulary_quiz-0.3/vocabulary_quiz.egg-info/top_level.txt
+-rw-r--r--   0 song-yongchan   (501) staff       (20)     3432 2024-05-21 10:17:30.000000 vocabulary_quiz-0.3/words.csv
```

### Comparing `vocabulary_quiz-0.2/App/app.py` & `vocabulary_quiz-0.3/App/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import sys
 import random
 import requests
 from bs4 import BeautifulSoup
 import csv
 from flask import Flask, render_template, request, redirect, url_for, flash
 from datetime import datetime
 
@@ -153,9 +152,12 @@
     if not username:
         flash('Username cannot be empty')
         return redirect(url_for('index'))
 
     scores = view_scores(username)
     return render_template('scores.html', username=username, scores=scores)
 
-if __name__ == '__main__':
+def main():
     app.run(debug=True)
+
+if __name__ == '__main__':
+    main()
```

### Comparing `vocabulary_quiz-0.2/App/routes.py` & `vocabulary_quiz-0.3/App/routes.py`

 * *Files identical despite different names*

### Comparing `vocabulary_quiz-0.2/App/static/style.css` & `vocabulary_quiz-0.3/App/static/style.css`

 * *Files identical despite different names*

### Comparing `vocabulary_quiz-0.2/App/templates/index.html` & `vocabulary_quiz-0.3/App/templates/index.html`

 * *Files identical despite different names*

### Comparing `vocabulary_quiz-0.2/App/templates/quiz.html` & `vocabulary_quiz-0.3/App/templates/quiz.html`

 * *Files identical despite different names*

### Comparing `vocabulary_quiz-0.2/App/templates/scores.html` & `vocabulary_quiz-0.3/App/templates/scores.html`

 * *Files identical despite different names*

### Comparing `vocabulary_quiz-0.2/App/templates/start_quiz.html` & `vocabulary_quiz-0.3/App/templates/start_quiz.html`

 * *Files identical despite different names*

### Comparing `vocabulary_quiz-0.2/words.csv` & `vocabulary_quiz-0.3/words.csv`

 * *Files identical despite different names*

