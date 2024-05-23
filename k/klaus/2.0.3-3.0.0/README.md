# Comparing `tmp/klaus-2.0.3.tar.gz` & `tmp/klaus-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klaus-2.0.3.tar", last modified: Sat Jun  3 15:15:02 2023, max compression
+gzip compressed data, was "klaus-3.0.0.tar", last modified: Thu May 23 20:03:59 2024, max compression
```

## Comparing `klaus-2.0.3.tar` & `klaus-3.0.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 j          (501) wheel        (0)        0 2023-06-03 15:15:02.889720 klaus-2.0.3/
--rw-r--r--   0 j          (501) wheel        (0)     1130 2023-06-03 15:11:57.000000 klaus-2.0.3/LICENSE
--rw-r--r--   0 j          (501) wheel        (0)       85 2023-06-03 15:11:57.000000 klaus-2.0.3/MANIFEST.in
--rw-r--r--   0 j          (501) wheel        (0)     4902 2023-06-03 15:15:02.889603 klaus-2.0.3/PKG-INFO
--rw-r--r--   0 j          (501) wheel        (0)     4151 2023-06-03 15:11:57.000000 klaus-2.0.3/README.rst
-drwxr-xr-x   0 j          (501) wheel        (0)        0 2023-06-03 15:15:02.886407 klaus-2.0.3/klaus/
--rw-r--r--   0 j          (501) wheel        (0)     9728 2023-06-03 15:14:33.000000 klaus-2.0.3/klaus/__init__.py
--rw-r--r--   0 j          (501) wheel        (0)     4279 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/cli.py
-drwxr-xr-x   0 j          (501) wheel        (0)        0 2023-06-03 15:15:02.887559 klaus-2.0.3/klaus/contrib/
--rw-r--r--   0 j          (501) wheel        (0)        0 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/contrib/__init__.py
--rw-r--r--   0 j          (501) wheel        (0)      789 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/contrib/app_args.py
--rw-r--r--   0 j          (501) wheel        (0)      317 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/contrib/wsgi.py
--rw-r--r--   0 j          (501) wheel        (0)      804 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/contrib/wsgi_autoreload.py
--rw-r--r--   0 j          (501) wheel        (0)     1466 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/contrib/wsgi_autoreloading.py
--rw-r--r--   0 j          (501) wheel        (0)     7559 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/ctagscache.py
--rw-r--r--   0 j          (501) wheel        (0)     1404 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/ctagsutils.py
--rw-r--r--   0 j          (501) wheel        (0)     2605 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/diff.py
--rw-r--r--   0 j          (501) wheel        (0)     4728 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/highlighting.py
--rw-r--r--   0 j          (501) wheel        (0)     1329 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/markup.py
--rw-r--r--   0 j          (501) wheel        (0)    14878 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/repo.py
-drwxr-xr-x   0 j          (501) wheel        (0)        0 2023-06-03 15:15:02.888007 klaus-2.0.3/klaus/static/
--rw-r--r--   0 j          (501) wheel        (0)     2876 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/static/favicon.png
--rw-r--r--   0 j          (501) wheel        (0)     9557 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/static/klaus.css
--rw-r--r--   0 j          (501) wheel        (0)     1912 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/static/klaus.js
--rw-r--r--   0 j          (501) wheel        (0)     3422 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/static/pygments.css
--rw-r--r--   0 j          (501) wheel        (0)      201 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/static/robots.txt
-drwxr-xr-x   0 j          (501) wheel        (0)        0 2023-06-03 15:15:02.888957 klaus-2.0.3/klaus/templates/
--rw-r--r--   0 j          (501) wheel        (0)     1362 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/templates/base.html
--rw-r--r--   0 j          (501) wheel        (0)     1254 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/templates/blame_blob.html
--rw-r--r--   0 j          (501) wheel        (0)      448 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/templates/history.html
--rw-r--r--   0 j          (501) wheel        (0)     2146 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/templates/history.inc.html
--rw-r--r--   0 j          (501) wheel        (0)      395 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/templates/index.html
--rw-r--r--   0 j          (501) wheel        (0)     1887 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/templates/repo_list.html
--rw-r--r--   0 j          (501) wheel        (0)      945 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/templates/skeleton.html
--rw-r--r--   0 j          (501) wheel        (0)      503 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/templates/submodule.html
--rw-r--r--   0 j          (501) wheel        (0)      884 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/templates/tree.inc.html
--rw-r--r--   0 j          (501) wheel        (0)     1722 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/templates/view_blob.html
--rw-r--r--   0 j          (501) wheel        (0)     5966 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/templates/view_commit.html
--rw-r--r--   0 j          (501) wheel        (0)     8779 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/utils.py
--rw-r--r--   0 j          (501) wheel        (0)    18137 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus/views.py
--rw-r--r--   0 j          (501) wheel        (0)     1435 2023-06-03 15:11:57.000000 klaus-2.0.3/klaus.1
-drwxr-xr-x   0 j          (501) wheel        (0)        0 2023-06-03 15:15:02.887125 klaus-2.0.3/klaus.egg-info/
--rw-r--r--   0 j          (501) wheel        (0)     4902 2023-06-03 15:15:02.000000 klaus-2.0.3/klaus.egg-info/PKG-INFO
--rw-r--r--   0 j          (501) wheel        (0)     1156 2023-06-03 15:15:02.000000 klaus-2.0.3/klaus.egg-info/SOURCES.txt
--rw-r--r--   0 j          (501) wheel        (0)        1 2023-06-03 15:15:02.000000 klaus-2.0.3/klaus.egg-info/dependency_links.txt
--rw-r--r--   0 j          (501) wheel        (0)       41 2023-06-03 15:15:02.000000 klaus-2.0.3/klaus.egg-info/entry_points.txt
--rw-r--r--   0 j          (501) wheel        (0)        1 2023-06-03 15:15:02.000000 klaus-2.0.3/klaus.egg-info/not-zip-safe
--rw-r--r--   0 j          (501) wheel        (0)      143 2023-06-03 15:15:02.000000 klaus-2.0.3/klaus.egg-info/requires.txt
--rw-r--r--   0 j          (501) wheel        (0)        6 2023-06-03 15:15:02.000000 klaus-2.0.3/klaus.egg-info/top_level.txt
--rw-r--r--   0 j          (501) wheel        (0)       81 2023-06-03 15:11:57.000000 klaus-2.0.3/pyproject.toml
--rw-r--r--   0 j          (501) wheel        (0)       38 2023-06-03 15:15:02.889749 klaus-2.0.3/setup.cfg
--rw-r--r--   0 j          (501) wheel        (0)     1756 2023-06-03 15:14:26.000000 klaus-2.0.3/setup.py
-drwxr-xr-x   0 j          (501) wheel        (0)        0 2023-06-03 15:15:02.889465 klaus-2.0.3/tests/
--rw-r--r--   0 j          (501) wheel        (0)     1011 2023-06-03 15:11:57.000000 klaus-2.0.3/tests/test_blame.py
--rw-r--r--   0 j          (501) wheel        (0)     4552 2023-06-03 15:11:57.000000 klaus-2.0.3/tests/test_contrib.py
--rw-r--r--   0 j          (501) wheel        (0)     5937 2023-06-03 15:11:57.000000 klaus-2.0.3/tests/test_make_app.py
--rw-r--r--   0 j          (501) wheel        (0)     1095 2023-06-03 15:11:57.000000 klaus-2.0.3/tests/test_manpage.py
--rw-r--r--   0 j          (501) wheel        (0)     1222 2023-06-03 15:11:57.000000 klaus-2.0.3/tests/test_utils.py
--rw-r--r--   0 j          (501) wheel        (0)     2906 2023-06-03 15:11:57.000000 klaus-2.0.3/tests/test_views.py
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2024-05-23 20:03:59.393556 klaus-3.0.0/
+-rw-r--r--   0 j          (501) wheel        (0)     1130 2024-05-23 19:48:58.000000 klaus-3.0.0/LICENSE
+-rw-r--r--   0 j          (501) wheel        (0)       85 2024-05-23 19:48:58.000000 klaus-3.0.0/MANIFEST.in
+-rw-r--r--   0 j          (501) wheel        (0)     5086 2024-05-23 20:03:59.393394 klaus-3.0.0/PKG-INFO
+-rw-r--r--   0 j          (501) wheel        (0)     4151 2024-05-23 19:48:58.000000 klaus-3.0.0/README.rst
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2024-05-23 20:03:59.389060 klaus-3.0.0/klaus/
+-rw-r--r--   0 j          (501) wheel        (0)     9719 2024-05-23 19:51:12.000000 klaus-3.0.0/klaus/__init__.py
+-rw-r--r--   0 j          (501) wheel        (0)     4210 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/cli.py
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2024-05-23 20:03:59.390420 klaus-3.0.0/klaus/contrib/
+-rw-r--r--   0 j          (501) wheel        (0)        0 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/contrib/__init__.py
+-rw-r--r--   0 j          (501) wheel        (0)      789 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/contrib/app_args.py
+-rw-r--r--   0 j          (501) wheel        (0)      318 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/contrib/wsgi.py
+-rw-r--r--   0 j          (501) wheel        (0)      800 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/contrib/wsgi_autoreload.py
+-rw-r--r--   0 j          (501) wheel        (0)     1428 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/contrib/wsgi_autoreloading.py
+-rw-r--r--   0 j          (501) wheel        (0)     7552 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/ctagscache.py
+-rw-r--r--   0 j          (501) wheel        (0)     1449 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/ctagsutils.py
+-rw-r--r--   0 j          (501) wheel        (0)     2635 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/diff.py
+-rw-r--r--   0 j          (501) wheel        (0)     4634 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/highlighting.py
+-rw-r--r--   0 j          (501) wheel        (0)     1616 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/markup.py
+-rw-r--r--   0 j          (501) wheel        (0)    15043 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/repo.py
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2024-05-23 20:03:59.391104 klaus-3.0.0/klaus/static/
+-rw-r--r--   0 j          (501) wheel        (0)     2876 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/static/favicon.png
+-rw-r--r--   0 j          (501) wheel        (0)     9557 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/static/klaus.css
+-rw-r--r--   0 j          (501) wheel        (0)     1912 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/static/klaus.js
+-rw-r--r--   0 j          (501) wheel        (0)     3422 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/static/pygments.css
+-rw-r--r--   0 j          (501) wheel        (0)      201 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/static/robots.txt
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2024-05-23 20:03:59.392366 klaus-3.0.0/klaus/templates/
+-rw-r--r--   0 j          (501) wheel        (0)     1362 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/templates/base.html
+-rw-r--r--   0 j          (501) wheel        (0)     1254 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/templates/blame_blob.html
+-rw-r--r--   0 j          (501) wheel        (0)      448 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/templates/history.html
+-rw-r--r--   0 j          (501) wheel        (0)     2146 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/templates/history.inc.html
+-rw-r--r--   0 j          (501) wheel        (0)      395 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/templates/index.html
+-rw-r--r--   0 j          (501) wheel        (0)     1886 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/templates/repo_list.html
+-rw-r--r--   0 j          (501) wheel        (0)      945 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/templates/skeleton.html
+-rw-r--r--   0 j          (501) wheel        (0)      503 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/templates/submodule.html
+-rw-r--r--   0 j          (501) wheel        (0)      884 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/templates/tree.inc.html
+-rw-r--r--   0 j          (501) wheel        (0)     1722 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/templates/view_blob.html
+-rw-r--r--   0 j          (501) wheel        (0)     5966 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/templates/view_commit.html
+-rw-r--r--   0 j          (501) wheel        (0)     8678 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/utils.py
+-rw-r--r--   0 j          (501) wheel        (0)    17985 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus/views.py
+-rw-r--r--   0 j          (501) wheel        (0)     1435 2024-05-23 19:48:58.000000 klaus-3.0.0/klaus.1
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2024-05-23 20:03:59.393209 klaus-3.0.0/klaus.egg-info/
+-rw-r--r--   0 j          (501) wheel        (0)     5086 2024-05-23 20:03:59.000000 klaus-3.0.0/klaus.egg-info/PKG-INFO
+-rw-r--r--   0 j          (501) wheel        (0)     1156 2024-05-23 20:03:59.000000 klaus-3.0.0/klaus.egg-info/SOURCES.txt
+-rw-r--r--   0 j          (501) wheel        (0)        1 2024-05-23 20:03:59.000000 klaus-3.0.0/klaus.egg-info/dependency_links.txt
+-rw-r--r--   0 j          (501) wheel        (0)       41 2024-05-23 20:03:59.000000 klaus-3.0.0/klaus.egg-info/entry_points.txt
+-rw-r--r--   0 j          (501) wheel        (0)        1 2024-05-23 20:03:59.000000 klaus-3.0.0/klaus.egg-info/not-zip-safe
+-rw-r--r--   0 j          (501) wheel        (0)       71 2024-05-23 20:03:59.000000 klaus-3.0.0/klaus.egg-info/requires.txt
+-rw-r--r--   0 j          (501) wheel        (0)        6 2024-05-23 20:03:59.000000 klaus-3.0.0/klaus.egg-info/top_level.txt
+-rw-r--r--   0 j          (501) wheel        (0)      243 2024-05-23 19:48:58.000000 klaus-3.0.0/pyproject.toml
+-rw-r--r--   0 j          (501) wheel        (0)       38 2024-05-23 20:03:59.393585 klaus-3.0.0/setup.cfg
+-rw-r--r--   0 j          (501) wheel        (0)     1701 2024-05-23 19:51:01.000000 klaus-3.0.0/setup.py
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2024-05-23 20:03:59.393057 klaus-3.0.0/tests/
+-rw-r--r--   0 j          (501) wheel        (0)     1012 2024-05-23 19:48:58.000000 klaus-3.0.0/tests/test_blame.py
+-rw-r--r--   0 j          (501) wheel        (0)     4552 2024-05-23 19:48:58.000000 klaus-3.0.0/tests/test_contrib.py
+-rw-r--r--   0 j          (501) wheel        (0)     5974 2024-05-23 19:48:58.000000 klaus-3.0.0/tests/test_make_app.py
+-rw-r--r--   0 j          (501) wheel        (0)     1051 2024-05-23 19:48:58.000000 klaus-3.0.0/tests/test_manpage.py
+-rw-r--r--   0 j          (501) wheel        (0)     1173 2024-05-23 19:48:58.000000 klaus-3.0.0/tests/test_utils.py
+-rw-r--r--   0 j          (501) wheel        (0)     2908 2024-05-23 19:48:58.000000 klaus-3.0.0/tests/test_views.py
```

### Comparing `klaus-2.0.3/LICENSE` & `klaus-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `klaus-2.0.3/PKG-INFO` & `klaus-3.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 Metadata-Version: 2.1
 Name: klaus
-Version: 2.0.3
+Version: 3.0.0
 Summary: The first Git web viewer that Just Works™.
 Home-page: https://github.com/jonashaag/klaus
 Author: Jonas Haag
 Author-email: jonas@lophus.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
 License-File: LICENSE
+Requires-Dist: flask
+Requires-Dist: Werkzeug>=0.15.0
+Requires-Dist: pygments
+Requires-Dist: httpauth>=0.4
+Requires-Dist: humanize
+Requires-Dist: dulwich>=0.19.3
 
 |travis-badge| |gitter-badge|
 
 .. |travis-badge| image:: https://travis-ci.org/jonashaag/klaus.svg?branch=master
     :target: https://travis-ci.org/jonashaag/klaus
 
 .. |gitter-badge| image:: https://badges.gitter.im/Join%20Chat.svg
```

### Comparing `klaus-2.0.3/README.rst` & `klaus-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `klaus-2.0.3/klaus/__init__.py` & `klaus-3.0.0/klaus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import jinja2
+
 try:
     import jinja2.ext.autoescape
+
     jinja2_autoescape_builtin = False
 except ImportError:
     jinja2_autoescape_builtin = True
+import dulwich.web
 import flask
 import httpauth
-import dulwich.web
 from dulwich.errors import NotGitRepository
-from klaus import views, utils
-from klaus.repo import FancyRepo, InvalidRepo
 
+from klaus import utils, views
+from klaus.repo import FancyRepo, InvalidRepo
 
-KLAUS_VERSION = utils.guess_git_revision() or "2.0.3"
+KLAUS_VERSION = utils.guess_git_revision() or "3.0.0"
 
 
 class Klaus(flask.Flask):
     jinja_options = {
         "extensions": [] if jinja2_autoescape_builtin else ["jinja2.ext.autoescape"],
         "undefined": jinja2.StrictUndefined,
     }
@@ -33,15 +35,15 @@
 
         flask.Flask.__init__(self, __name__)
 
         self.setup_routes()
 
     def create_jinja_environment(self):
         """Called by Flask.__init__"""
-        env = super(Klaus, self).create_jinja_environment()
+        env = super().create_jinja_environment()
         for func in [
             "force_unicode",
             "timesince",
             "shorten_sha1",
             "shorten_message",
             "extract_author_name",
             "formattimestamp",
```

### Comparing `klaus-2.0.3/klaus/cli.py` & `klaus-3.0.0/klaus/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-# coding: utf-8
-from __future__ import print_function
-
-import sys
-import os
 import argparse
+import os
+import sys
 import webbrowser
 
 from dulwich.errors import NotGitRepository
 from dulwich.repo import Repo
 
-from klaus import make_app, KLAUS_VERSION
+from klaus import KLAUS_VERSION, make_app
 from klaus.utils import force_unicode
 
 
 def git_repository(path):
     path = os.path.abspath(path)
     if not os.path.exists(path):
         raise argparse.ArgumentTypeError("%r: No such directory" % path)
@@ -110,15 +107,15 @@
         if not check_have_exuberant_ctags():
             print(
                 "ERROR: Exuberant ctags not installed (or 'ctags' binary isn't *Exuberant* ctags)",
                 file=sys.stderr,
             )
             return 1
         try:
-            import ctags
+            pass
         except ImportError:
             raise ImportError("Please install 'python-ctags3' to enable ctags support.")
 
     app = make_app(
         args.repos,
         force_unicode(args.site_name or args.host),
         args.smarthttp,
@@ -139,12 +136,12 @@
     # losing the simplicity of the code. In the Real World (TM) it'll take
     # longer for the browser to start than it will for us to start
     # serving, so we'll be OK.
     if args.with_browser is None:
         opener = webbrowser.open
     else:
         opener = webbrowser.get(args.with_browser).open
-    opener("http://%s:%s" % (args.host, args.port))
+    opener(f"http://{args.host}:{args.port}")
 
 
 if __name__ == "__main__":
     exit(main())
```

### Comparing `klaus-2.0.3/klaus/contrib/app_args.py` & `klaus-3.0.0/klaus/contrib/app_args.py`

 * *Files identical despite different names*

### Comparing `klaus-2.0.3/klaus/contrib/wsgi_autoreload.py` & `klaus-3.0.0/klaus/contrib/wsgi_autoreload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
+import io
 import os
 import warnings
-import io
 
 from .app_args import get_args_from_env
 from .wsgi_autoreloading import make_autoreloading_app
 
-
 if "KLAUS_REPOS" in os.environ:
     warnings.warn(
         "use KLAUS_REPOS_ROOT instead of KLAUS_REPOS for the autoreloader apps",
         DeprecationWarning,
     )
 
 args, kwargs = get_args_from_env()
 repos_root = os.environ.get("KLAUS_REPOS_ROOT") or os.environ["KLAUS_REPOS"]
 args = (repos_root,) + args[1:]
 
 if kwargs["htdigest_file"]:
     # Cache the contents of the htdigest file, the application will not read
     # the file like object until later when called.
-    with io.open(kwargs["htdigest_file"], encoding="utf-8") as htdigest_file:
+    with open(kwargs["htdigest_file"], encoding="utf-8") as htdigest_file:
         kwargs["htdigest_file"] = io.StringIO(htdigest_file.read())
 
 application = make_autoreloading_app(*args, **kwargs)
```

### Comparing `klaus-2.0.3/klaus/contrib/wsgi_autoreloading.py` & `klaus-3.0.0/klaus/contrib/wsgi_autoreloading.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from __future__ import print_function
 import glob
-import time
 import threading
+import time
 
 from klaus import make_app
 
 
 # Shared state between poller and application wrapper
 class S:
     #: the real WSGI app
```

### Comparing `klaus-2.0.3/klaus/ctagscache.py` & `klaus-3.0.0/klaus/ctagscache.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,23 +22,24 @@
 on each request, we keep the tagsfiles that are most likely to be used (**) in
 uncompressed form.
 
 (*) We always create a clone in the current implementation;
     this could be optimized in the future.
 (**) "most likely": currently implemented as "most recently used"
 """
+import atexit
+import gzip
 import os
 import shutil
 import tempfile
 import threading
-import gzip
-import atexit
+
 from dulwich.lru_cache import LRUSizeCache
-from klaus.ctagsutils import create_tagsfile, delete_tagsfile
 
+from klaus.ctagsutils import create_tagsfile, delete_tagsfile
 
 # Good compression while taking only 10% more time than level 1
 COMPRESSION_LEVEL = 4
 
 
 def compress_tagsfile(uncompressed_tagsfile_path):
     """Compress an uncompressed tagsfile.
@@ -63,15 +64,15 @@
             shutil.copyfileobj(compressed, uncompressed)
     return uncompressed_tagsfile_path
 
 
 MiB = 1024 * 1024
 
 
-class CTagsCache(object):
+class CTagsCache:
     """A ctags cache. Both uncompressed and compressed entries are kept in
     temporary files created by `tempfile.mkstemp` which are deleted from disk
     when the Python interpreter is shut down.
 
     :param uncompressed_max_bytes: Maximum size of the uncompressed cache sector
     :param compressed_max_bytes:   Maximum size of the compressed cache sector
```

### Comparing `klaus-2.0.3/klaus/ctagsutils.py` & `klaus-3.0.0/klaus/ctagsutils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 import os
-import subprocess
 import shutil
-import tempfile
 import subprocess
+import tempfile
 
 
-def check_have_exuberant_ctags():
-    """Check that the 'ctags' binary is *Exuberant* ctags (not etags etc)"""
+def check_have_compatible_ctags():
+    """Check that the 'ctags' binary is a compatible ctags (Universal or Exuberant, not etags etc)"""
     try:
-        return b"Exuberant" in subprocess.check_output(
-            ["ctags", "--version"], stderr=subprocess.PIPE
-        )
+        out = subprocess.check_output(["ctags", "--version"], stderr=subprocess.PIPE)
+        return b"Universal" in out or b"Exuberant" in out
     except subprocess.CalledProcessError:
         return False
 
 
 def create_tagsfile(git_repo_path, git_rev):
     """Create a ctags tagsfile for the given Git repository and revision.
 
     This creates a temporary clone of the repository, checks out the revision,
     runs 'ctags -R' and deletes the temporary clone.
 
     :return: path to the generated tagsfile
     """
     assert (
-        check_have_exuberant_ctags()
-    ), "'ctags' binary is missing or not *Exuberant* ctags"
+        check_have_compatible_ctags()
+    ), "'ctags' binary is missing or not *Universal* (or *Exuberant*) ctags"
 
     _, target_tagsfile = tempfile.mkstemp()
     checkout_tmpdir = tempfile.mkdtemp()
     try:
         subprocess.check_call(
             ["git", "clone", "-q", "--shared", git_repo_path, checkout_tmpdir]
         )
```

### Comparing `klaus-2.0.3/klaus/diff.py` & `klaus-3.0.0/klaus/diff.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# -*- coding: utf-8 -*-
 """
     lodgeit.lib.diff
     ~~~~~~~~~~~~~~~~
 
     Render a nice diff between two things.
 
     :copyright: 2007 by Armin Ronacher.
     :license: BSD
 """
 
 from difflib import SequenceMatcher
+
 from klaus.utils import escape_html as e
 
 
 def highlight_line(old_line, new_line):
     """Highlight inline changes in both lines."""
     start = 0
     limit = min(len(old_line), len(new_line))
@@ -22,36 +22,40 @@
     end = -1
     limit -= start
     while -end <= limit and old_line[end] == new_line[end]:
         end -= 1
     end += 1
     if start or end:
 
-        def do(l, tag):
-            last = end + len(l)
+        def do(line, tag):
+            last = end + len(line)
             return b"".join(
-                [l[:start], b"<", tag, b">", l[start:last], b"</", tag, b">", l[last:]]
+                [
+                    line[:start],
+                    b"<",
+                    tag,
+                    b">",
+                    line[start:last],
+                    b"</",
+                    tag,
+                    b">",
+                    line[last:],
+                ]
             )
 
         old_line = do(old_line, b"del")
         new_line = do(new_line, b"ins")
     return old_line, new_line
 
 
 def render_diff(a, b, n=3):
     """Parse the diff an return data for the template."""
     actions = []
     chunks = []
     for group in SequenceMatcher(None, a, b).get_grouped_opcodes(n):
-        old_line, old_end, new_line, new_end = (
-            group[0][1],
-            group[-1][2],
-            group[0][3],
-            group[-1][4],
-        )
         lines = []
 
         def add_line(old_lineno, new_lineno, action, line):
             actions.append(action)
             lines.append(
                 {
                     "old_lineno": old_lineno,
```

### Comparing `klaus-2.0.3/klaus/highlighting.py` & `klaus-3.0.0/klaus/highlighting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,39 @@
-try:
-    # Python < 3
-    from itertools import ifilter as filter
-except ImportError:
-    pass
-
 from pygments import highlight
+from pygments.formatters import HtmlFormatter
 from pygments.lexers import (
+    ClassNotFound,
+    TextLexer,
     get_lexer_by_name,
     get_lexer_for_filename,
     guess_lexer,
-    ClassNotFound,
-    TextLexer,
 )
-from pygments.formatters import HtmlFormatter
 
 from klaus import markup
 
-
 CTAGS_SUPPORTED_LANGUAGES = (
     "Asm Awk Basic C C# C++ Cobol DosBatch Eiffel Erlang Fortran HTML Java "
     "JavaScript Lisp Lua Make Makefile MatLab OCaml PHP Pascal Perl Python "
     "REXX Ruby SML SQL Scheme Sh Tcl Tex VHDL Verilog Vim"
     # Not supported by Pygments: Asp Ant BETA Flex SLang Vera YACC
 ).split()
 PYGMENTS_CTAGS_LANGUAGE_MAP = dict(
-    (get_lexer_by_name(l).name, l) for l in CTAGS_SUPPORTED_LANGUAGES
+    (get_lexer_by_name(lexer).name, lexer) for lexer in CTAGS_SUPPORTED_LANGUAGES  # type: ignore
 )
 
 
 class KlausDefaultFormatter(HtmlFormatter):
     def __init__(self, language, ctags, **kwargs):
         HtmlFormatter.__init__(
             self,
             linenos="table",
             lineanchors="L",
             linespans="L",
             anchorlinenos=True,
-            **kwargs
+            **kwargs,
         )
         self.language = language
         if ctags:
             # Use Pygments' ctags system but provide our own CTags instance
             self.tagsfile = True  # some trueish object
             self._ctags = ctags
 
@@ -89,15 +82,15 @@
         # the "real" definition of the tag.  Import matches aren't very helpful:
         # In the best case, we are brought to the line where the tag is imported
         # in the same file. But it may also bring us to some completely unrelated
         # import of the tag in some other file.  We change the tag lookup mechanics
         # so that non-import matches are always preferred over import matches.
         return filter(
             lambda match: match["kind"] != b"i",
-            super(KlausPythonFormatter, self).get_best_ctags_matches(matches),
+            super().get_best_ctags_matches(matches),
         )
 
 
 def highlight_or_render(
     code, filename, render_markup=True, ctags=None, ctags_baseurl=None
 ):
     """Render code using Pygments, markup (markdown, rst, ...) using the
```

### Comparing `klaus-2.0.3/klaus/repo.py` & `klaus-3.0.0/klaus/repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 import functools
 import io
 import os
 import stat
 import subprocess
 import threading
 
-from dulwich.objects import S_ISGITLINK
-from dulwich.object_store import tree_lookup_path
-from dulwich.objects import Blob
+import dulwich
+import dulwich.patch
 from dulwich.errors import NotTreeError
-import dulwich, dulwich.patch
+from dulwich.object_store import tree_lookup_path
+from dulwich.objects import S_ISGITLINK, Blob
 
 try:
     from dulwich.refs import SymrefLoop
 except ImportError:  # dulwich < 0.20.46
-    InaccessibleRef = KeyError
+    InaccessibleRef = KeyError  # type: ignore
 else:
-    InaccessibleRef = (SymrefLoop, KeyError)
+    InaccessibleRef = (SymrefLoop, KeyError)  # type: ignore
 
 
+from klaus.diff import render_diff
 from klaus.utils import (
+    decode_from_git,
+    encode_for_git,
     force_unicode,
     parent_directory,
     repo_human_name,
-    encode_for_git,
-    decode_from_git,
 )
-from klaus.diff import render_diff
-
 
 NOT_SET = "__not_set__"
 
 
 def cached_call(key, validator, producer, _cache={}):
     data, old_validator = _cache.get(key, (None, NOT_SET))
     if old_validator != validator:
@@ -41,52 +40,54 @@
 
 
 def synchronized(func, lock=threading.RLock()):
     @functools.wraps(func)
     def synchronized_func(*args, **kwargs):
         with lock:
             return func(*args, **kwargs)
+
     return synchronized_func
 
 
-class FancyRepo(object):
+class FancyRepo:
     """A wrapper around Dulwich's Repo that adds some helper methods."""
 
     def __init__(self, path, namespace):
         self.dulwich_repo = dulwich.repo.Repo(path)
         self.namespace = namespace
 
-    @property
-    def path(self):
-        return self.dulwich_repo.path
+    @synchronized
+    def __getattr__(self, attr):
+        return getattr(self.dulwich_repo, attr)
+
+    @synchronized
+    def __getitem__(self, key):
+        return self.dulwich_repo[key]
 
     @property
     def name(self):
         return repo_human_name(self.path)
 
     @property
     def namespaced_name(self):
         if self.namespace:
-            return "~{}/{}".format(self.namespace, self.name)
+            return f"~{self.namespace}/{self.name}"
         else:
             return self.name
 
-    @synchronized
-    def __getitem__(self, key):
-        return self.dulwich_repo[key]
-
     # TODO: factor out stuff into dulwich
     @synchronized
     def get_last_updated_at(self):
         """Get datetime of last commit to this repository.
 
         Caches the result to speed up the repo_list page.
         Cache is invalidated if one of the ref targets changes,
         eg. a new commit has been made and 'refs/heads/master' was changed.
         """
+
         def _get_commit_time_cached(ref_id):
             return cached_call(
                 key=(ref_id, "_get_commit_time"),
                 validator=None,
                 producer=lambda: _get_commit_time(ref_id),
             )
 
@@ -298,14 +299,15 @@
             elif stat.S_ISDIR(entry_abs.mode):
                 dirs.append(item)
             else:
                 files.append(item)
 
         def keyfunc(tpl):
             return tpl[0].lower()
+
         submodules.sort(key=keyfunc)
         files.sort(key=keyfunc)
         dirs.sort(key=keyfunc)
 
         if path:
             dirs.insert(0, ("..", parent_directory(path)))
 
@@ -320,24 +322,34 @@
             parent_tree = self[commit.parents[0]].tree
         else:
             parent_tree = None
 
         summary = {"nfiles": 0, "nadditions": 0, "ndeletions": 0}
         file_changes = []  # the changes in detail
 
-        dulwich_changes = self.dulwich_repo.object_store.tree_changes(parent_tree, commit.tree)
+        dulwich_changes = self.dulwich_repo.object_store.tree_changes(
+            parent_tree, commit.tree
+        )
         for (oldpath, newpath), (oldmode, newmode), (oldsha, newsha) in dulwich_changes:
             summary["nfiles"] += 1
             try:
-                oldblob = self.dulwich_repo.object_store[oldsha] if oldsha else Blob.from_string(b"")
+                oldblob = (
+                    self.dulwich_repo.object_store[oldsha]
+                    if oldsha
+                    else Blob.from_string(b"")
+                )
             except KeyError:
                 # probably related to submodules; Dulwich will handle that.
                 oldblob = Blob.from_string(b"")
             try:
-                newblob = self.dulwich_repo.object_store[newsha] if newsha else Blob.from_string(b"")
+                newblob = (
+                    self.dulwich_repo.object_store[newsha]
+                    if newsha
+                    else Blob.from_string(b"")
+                )
             except KeyError:
                 # probably related to submodules; Dulwich will handle that.
                 newblob = Blob.from_string(b"")
 
             # Check for binary files -- can't show diffs for these
             if guess_is_binary(newblob) or guess_is_binary(oldblob):
                 file_changes.append(
@@ -379,27 +391,27 @@
         )
         return bytesio.getvalue()
 
     def freeze(self):
         return FrozenFancyRepo(self)
 
 
-class FrozenFancyRepo(object):
+class FrozenFancyRepo:
     """A special version of FancyRepo that assumes the underlying Git
     repository does not change.  Used for performance optimizations.
     """
 
     def __init__(self, repo):
         self.__repo = repo
         self.__last_updated_at = NOT_SET
 
     def __setattr__(self, name, value):
         if not name.startswith("_FrozenFancyRepo__"):
             raise TypeError("Can't set %s attribute on FrozenFancyRepo" % name)
-        super(FrozenFancyRepo, self).__setattr__(name, value)
+        super().__setattr__(name, value)
 
     def __getattr__(self, name):
         return getattr(self.__repo, name)
 
     def fast_get_last_updated_at(self):
         if self.__last_updated_at is NOT_SET:
             self.__last_updated_at = self.__repo.get_last_updated_at()
@@ -416,10 +428,10 @@
     @property
     def name(self):
         return repo_human_name(self.path)
 
     @property
     def namespaced_name(self):
         if self.namespace:
-            return "~{}/{}".format(self.namespace, self.name)
+            return f"~{self.namespace}/{self.name}"
         else:
             return self.name
```

### Comparing `klaus-2.0.3/klaus/static/favicon.png` & `klaus-3.0.0/klaus/static/favicon.png`

 * *Files identical despite different names*

### Comparing `klaus-2.0.3/klaus/static/klaus.css` & `klaus-3.0.0/klaus/static/klaus.css`

 * *Files identical despite different names*

### Comparing `klaus-2.0.3/klaus/static/klaus.js` & `klaus-3.0.0/klaus/static/klaus.js`

 * *Files identical despite different names*

### Comparing `klaus-2.0.3/klaus/static/pygments.css` & `klaus-3.0.0/klaus/static/pygments.css`

 * *Files identical despite different names*

### Comparing `klaus-2.0.3/klaus/templates/base.html` & `klaus-3.0.0/klaus/templates/base.html`

 * *Files identical despite different names*

### Comparing `klaus-2.0.3/klaus/templates/blame_blob.html` & `klaus-3.0.0/klaus/templates/blame_blob.html`

 * *Files identical despite different names*

### Comparing `klaus-2.0.3/klaus/templates/history.inc.html` & `klaus-3.0.0/klaus/templates/history.inc.html`

 * *Files identical despite different names*

### Comparing `klaus-2.0.3/klaus/templates/repo_list.html` & `klaus-3.0.0/klaus/templates/repo_list.html`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     <label for="order_by_name">Name</label>
   </div>
   <br>
   <label for="search_query">Search repos:</label>
   <input type="search" id="search_query" name="q" value="{{ search_query|default }}">
   <button type="submit">Search</button>
 </form>
- 
+
 <ul class=repolist>
   {% for repo in repos %}
     {% set last_updated_at = repo.fast_get_last_updated_at() %}
     {% set description = repo.get_description() %}
     <li>
       <a
         {% if last_updated_at %}
```

### Comparing `klaus-2.0.3/klaus/templates/skeleton.html` & `klaus-3.0.0/klaus/templates/skeleton.html`

 * *Files identical despite different names*

### Comparing `klaus-2.0.3/klaus/templates/tree.inc.html` & `klaus-3.0.0/klaus/templates/tree.inc.html`

 * *Files identical despite different names*

### Comparing `klaus-2.0.3/klaus/templates/view_blob.html` & `klaus-3.0.0/klaus/templates/view_blob.html`

 * *Files identical despite different names*

### Comparing `klaus-2.0.3/klaus/templates/view_commit.html` & `klaus-3.0.0/klaus/templates/view_commit.html`

 * *Files identical despite different names*

### Comparing `klaus-2.0.3/klaus/utils.py` & `klaus-3.0.0/klaus/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# encoding: utf-8
 import binascii
+import datetime
+import locale
+import mimetypes
 import os
 import re
+import subprocess
 import time
-import datetime
-import mimetypes
-import locale
 import warnings
-import subprocess
+from typing import Union
 
 try:
     import chardet
 except ImportError:
-    chardet = None
+    chardet = None  # type: ignore
 
-from werkzeug.middleware.proxy_fix import ProxyFix as WerkzeugProxyFix
 from humanize import naturaltime
+from werkzeug.middleware.proxy_fix import ProxyFix as WerkzeugProxyFix
 
 
 class ProxyFix(WerkzeugProxyFix):
     """This middleware can be applied to add HTTP (reverse) proxy support to a
     WSGI application (klaus), making it possible to:
 
     * Mount it under a sub-URL (http://example.com/git/...)
@@ -55,18 +55,18 @@
             if script_name.endswith("/"):
                 warnings.warn(
                     "'X-Script-Name' header should not end in '/' (found: %r). "
                     "Please fix your proxy's configuration." % script_name
                 )
                 script_name = script_name.rstrip("/")
             environ["SCRIPT_NAME"] = script_name
-        return super(ProxyFix, self).__call__(environ, start_response)
+        return super().__call__(environ, start_response)
 
 
-class SubUri(object):
+class SubUri:
     """WSGI middleware to tweak the WSGI environ so that it's possible to serve
     the wrapped app (klaus) under a sub-URL and/or to use a different HTTP
     scheme (http:// vs. https://) for proxy communication.
 
     This is done by making your proxy pass appropriate HTTP_X_SCRIPT_NAME and
     HTTP_X_SCHEME headers.
 
@@ -128,23 +128,18 @@
 
 
 def decode_from_git(b):
     # XXX This assumes everything to be UTF-8 encoded
     return b.decode("utf8")
 
 
-def force_unicode(s):
+def force_unicode(s: Union[str, bytes]) -> str:
     """Do all kinds of magic to turn `s` into unicode"""
     # It's already unicode, don't do anything:
-    try:
-        # Python < 3
-        text_type = unicode
-    except NameError:
-        text_type = str
-    if isinstance(s, text_type):
+    if isinstance(s, str):
         return s
 
     # Try some default encodings:
     try:
         return s.decode("utf-8")
     except UnicodeDecodeError:
         pass
@@ -155,19 +150,19 @@
         pass
 
     if chardet is not None:
         # Try chardet, if available
         encoding = chardet.detect(s)["encoding"]
         if encoding is not None:
             try:
-                return s.decode(encoding, 'replace')
+                return s.decode(encoding, "replace")
             except LookupError:
                 pass
 
-    return s.decode('latin1', 'replace')
+    return s.decode("latin1", "replace")
 
 
 def extract_author_name(email):
     """Extract the name from an email address --
     >>> extract_author_name("John <john@example.com>")
     "John"
 
@@ -275,20 +270,20 @@
     if rev.startswith(repo_name + "-"):
         # If the rev is a tag name that already starts with the repo name,
         # skip it.
         return rev
     elif len(rev) >= 2 and rev[0] == "v" and not rev[1].isalpha():
         # If the rev is a tag name prefixed by a 'v', skip the 'v'.
         # So, v-1.0 -> 1.0, v1.0 -> 1.0, but vanilla -> vanilla.
-        return "%s-%s" % (repo_name, rev[1:])
+        return f"{repo_name}-{rev[1:]}"
     elif len(rev) == 40 and is_hex_prefix(rev):
         # If the rev is a commit hash, simply use that.
-        return "%s@%s" % (repo_name, rev)
+        return f"{repo_name}@{rev}"
     else:
-        return "%s-%s" % (repo_name, rev)
+        return f"{repo_name}-{rev}"
 
 
 def repo_human_name(path):
     """Get repository name from path.
 
     1. /x/y.git -> /x/y  and  /x/y/.git/ -> /x/y//
     2. /x/y/ -> /x/y
```

### Comparing `klaus-2.0.3/klaus/views.py` & `klaus-3.0.0/klaus/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,50 @@
-from io import BytesIO
 import os
 import sys
+from io import BytesIO
 
-from flask import request, render_template, current_app, url_for
-from flask.views import View
-
-from werkzeug.wrappers import Response
-from werkzeug.exceptions import NotFound
-
-import dulwich.objects
 import dulwich.archive
 import dulwich.config
+import dulwich.objects
 from dulwich.object_store import tree_lookup_path
+from flask import current_app, render_template, request, url_for
+from flask.views import View
+from werkzeug.exceptions import NotFound
+from werkzeug.wrappers import Response
 
 try:
     from dulwich.refs import SymrefLoop
-except ImportError:   # dulwich < 0.20.46
-    class SymrefLoop(Exception):
+except ImportError:  # dulwich < 0.20.46
+
+    class SymrefLoop(Exception):  # type: ignore
         """Dummy exception."""
 
+
 try:
     import ctags
 except ImportError:
     ctags = None
 else:
     from klaus import ctagscache
 
     CTAGS_CACHE = ctagscache.CTagsCache()
 
 from klaus import markup
 from klaus.highlighting import highlight_or_render
 from klaus.utils import (
-    parent_directory,
-    subpaths,
+    encode_for_git,
     force_unicode,
     guess_is_binary,
     guess_is_image,
+    parent_directory,
     replace_dupes,
     sanitize_branch_name,
-    encode_for_git,
+    subpaths,
 )
 
-
 README_FILENAMES = [
     b"README",
     b"README.md",
     b"README.mkdn",
     b"README.mdwn",
     b"README.markdown",
     b"README.rst",
@@ -65,17 +64,20 @@
         invalid_repos = [
             r
             for r in invalid_repos
             if search_query.lower() in r.namespaced_name.lower()
         ]
 
     if order_by == "name":
+
         def sort_key(repo):
             return repo.namespaced_name
+
     else:
+
         def sort_key(repo):
             return -(repo.fast_get_last_updated_at() or -1), repo.namespaced_name
 
     repos = sorted(repos, key=sort_key)
     invalid_repos = sorted(invalid_repos, key=lambda repo: repo.namespaced_name)
 
     return render_template(
@@ -94,15 +96,15 @@
 
 
 def _get_repo_and_rev(repo, namespace=None, rev=None, path=None):
     if path and rev:
         rev += "/" + path.rstrip("/")
 
     if namespace:
-        repo_key = "~{}/{}".format(namespace, repo)
+        repo_key = f"~{namespace}/{repo}"
     else:
         repo_key = repo
     try:
         repo = current_app.valid_repos[repo_key]
     except KeyError:
         raise NotFound("No such repository %r" % repo)
 
@@ -117,20 +119,18 @@
 
     i = len(rev)
     while i > 0:
         try:
             commit = repo.get_commit(rev[:i])
             path = rev[i:].strip("/")
             rev = rev[:i]
-        except (KeyError, IOError):
+        except (OSError, KeyError):
             i = rev.rfind("/", 0, i)
         except SymrefLoop as e:
-            raise NotFound(
-                "symref loop for %s at depth %d"
-                % (e.ref, e.depth))
+            raise NotFound("symref loop for %s at depth %d" % (e.ref, e.depth))
         else:
             break
     else:
         raise NotFound("No such commit %r" % rev)
 
     return repo, rev, path, commit
 
@@ -214,47 +214,48 @@
     def get_response(self):
         return Response(
             self.context["repo"].raw_commit_diff(self.context["commit"]),
             mimetype="text/plain",
         )
 
 
-class TreeViewMixin(object):
+class TreeViewMixin:
     """The logic required for displaying the current directory in the sidebar."""
 
     def make_template_context(self, *args):
-        super(TreeViewMixin, self).make_template_context(*args)
+        super().make_template_context(*args)
         self.context["root_tree"] = self.listdir()
 
     def listdir(self):
         """Return a list of directories and files in the current path of the selected commit."""
         root_directory = self.get_root_directory()
         return self.context["repo"].listdir(self.context["commit"], root_directory)
 
     def get_root_directory(self):
         root_directory = self.context["path"]
         if isinstance(self.context["blob_or_tree"], dulwich.objects.Blob):
             # 'path' is a file (not folder) name
             root_directory = parent_directory(root_directory)
         return root_directory
 
-class ReadmeMixin(object):
+
+class ReadmeMixin:
     """The logic required for finding and displaying README files."""
 
     def _get_readme(self):
         commit, path = self.context["commit"], self.context["path"]
         tree = self.context["repo"].get_blob_or_tree(commit, path)
 
         if not isinstance(tree, dulwich.objects.Tree):
             raise KeyError
 
         for name in README_FILENAMES:
             if name.lower() in [t.lower() for t in tree]:
                 obj = self.context["repo"][tree[name][1]]
-                if obj.type_name == b'blob':
+                if obj.type_name == b"blob":
                     readme_data = obj.data
                     readme_filename = name
                     return (readme_filename, readme_data)
         else:
             raise KeyError
 
     def get_readme_context(self):
@@ -278,15 +279,15 @@
     """Show commits of a branch + path, just like `git log`. With pagination.
 
     Also, README, if available."""
 
     template_name = "history.html"
 
     def make_template_context(self, *args):
-        super(HistoryView, self).make_template_context(*args)
+        super().make_template_context(*args)
 
         try:
             page = int(request.args.get("page"))
         except (TypeError, ValueError):
             page = 0
 
         self.context["page"] = page
@@ -328,15 +329,15 @@
     """Show commits of a branch, just like `git log`.
 
     Also, README, if available."""
 
     template_name = "index.html"
 
     def make_template_context(self, *args):
-        super(IndexView, self).make_template_context(*args)
+        super().make_template_context(*args)
 
         self.context["base_href"] = url_for(
             "blob",
             repo=self.context["repo"].namespaced_name,
             rev=self.context["rev"],
             path="",
         )
@@ -365,15 +366,15 @@
         )
 
         self.context.update(self.get_readme_context())
 
 
 class BaseBlobView(BaseRepoView):
     def make_template_context(self, *args):
-        super(BaseBlobView, self).make_template_context(*args)
+        super().make_template_context(*args)
         if not isinstance(self.context["blob_or_tree"], dulwich.objects.Blob):
             raise NotFound("Not a blob")
         self.context["filename"] = os.path.basename(self.context["path"])
 
 
 class SubmoduleView(BaseRepoView):
     """Show an information page about a submodule."""
@@ -446,19 +447,19 @@
         else:
             ctags_args = {}
 
         return highlight_or_render(
             force_unicode(self.context["blob_or_tree"].data),
             self.context["filename"],
             render_markup,
-            **ctags_args
+            **ctags_args,
         )
 
     def make_template_context(self, *args):
-        super(BaseFileView, self).make_template_context(*args)
+        super().make_template_context(*args)
         self.context.update(
             {
                 "can_render": True,
                 "is_binary": False,
                 "too_large": False,
                 "is_markup": False,
             }
@@ -485,15 +486,15 @@
 
 class FileView(BaseFileView):
     """Shows a file rendered using ``pygmentize``."""
 
     template_name = "view_blob.html"
 
     def make_template_context(self, *args):
-        super(FileView, self).make_template_context(*args)
+        super().make_template_context(*args)
         if self.context["can_render"]:
             render_markup = "markup" not in request.args
             self.context.update(
                 {
                     "is_markup": markup.can_render(self.context["filename"]),
                     "render_markup": render_markup,
                     "rendered_code": self.render_code(render_markup),
@@ -501,15 +502,15 @@
             )
 
 
 class BlameView(BaseFileView):
     template_name = "blame_blob.html"
 
     def make_template_context(self, *args):
-        super(BlameView, self).make_template_context(*args)
+        super().make_template_context(*args)
         if self.context["can_render"]:
             line_commits = self.context["repo"].blame(
                 self.context["commit"], self.context["path"]
             )
             replace_dupes(line_commits, None)
             self.context.update(
                 {
@@ -531,15 +532,15 @@
         return Response(self.context["blob_or_tree"].chunked, mimetype="")
 
 
 class DownloadView(BaseRepoView):
     """Download a repo as a tar.gz file."""
 
     def get_response(self):
-        basename = "%s@%s" % (
+        basename = "{}@{}".format(
             self.context["repo"].name,
             sanitize_branch_name(self.context["rev"]),
         )
         tarname = basename + ".tar.gz"
         headers = {
             "Content-Disposition": "attachment; filename=%s" % tarname,
             "Cache-Control": "no-store",  # Disables browser caching
```

### Comparing `klaus-2.0.3/klaus.1` & `klaus-3.0.0/klaus.1`

 * *Files identical despite different names*

### Comparing `klaus-2.0.3/klaus.egg-info/PKG-INFO` & `klaus-3.0.0/klaus.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 Metadata-Version: 2.1
 Name: klaus
-Version: 2.0.3
+Version: 3.0.0
 Summary: The first Git web viewer that Just Works™.
 Home-page: https://github.com/jonashaag/klaus
 Author: Jonas Haag
 Author-email: jonas@lophus.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
 License-File: LICENSE
+Requires-Dist: flask
+Requires-Dist: Werkzeug>=0.15.0
+Requires-Dist: pygments
+Requires-Dist: httpauth>=0.4
+Requires-Dist: humanize
+Requires-Dist: dulwich>=0.19.3
 
 |travis-badge| |gitter-badge|
 
 .. |travis-badge| image:: https://travis-ci.org/jonashaag/klaus.svg?branch=master
     :target: https://travis-ci.org/jonashaag/klaus
 
 .. |gitter-badge| image:: https://badges.gitter.im/Join%20Chat.svg
```

### Comparing `klaus-2.0.3/klaus.egg-info/SOURCES.txt` & `klaus-3.0.0/klaus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `klaus-2.0.3/setup.py` & `klaus-3.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# encoding: utf-8
-
 import os
+
 from setuptools import setup
 
 long_description = open(os.path.join(os.path.dirname(__file__), "README.rst")).read()
 
+
 def install_data_files_hack():
     # This is a clever hack to circumvent distutil's data_files
     # policy "install once, find never". Definitely a TODO!
     # -- https://groups.google.com/group/comp.lang.python/msg/2105ee4d9e8042cb
     from distutils.command.install import INSTALL_SCHEMES
 
     for scheme in INSTALL_SCHEMES.values():
@@ -17,23 +17,22 @@
 
 install_data_files_hack()
 
 requires = [
     "flask",
     "Werkzeug>=0.15.0",
     "pygments",
-    "httpauth",
+    "httpauth>=0.4",
     "humanize",
-    'dulwich>=0.19.3;python_version>="3.5"',
-    'dulwich>=0.19.3,<0.20;python_version<"3.5"',
+    "dulwich>=0.19.3",
 ]
 
 setup(
     name="klaus",
-    version="2.0.3",
+    version="3.0.0",
     author="Jonas Haag",
     author_email="jonas@lophus.org",
     packages=["klaus", "klaus.contrib"],
     include_package_data=True,
     zip_safe=False,
     url="https://github.com/jonashaag/klaus",
     description="The first Git web viewer that Just Works™.",
@@ -46,12 +45,13 @@
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: ISC License (ISCL)",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
     ],
+    python_requires=">=3.7",
     install_requires=requires,
     entry_points={
         "console_scripts": ["klaus=klaus.cli:main"],
     },
 )
```

### Comparing `klaus-2.0.3/tests/test_blame.py` & `klaus-3.0.0/tests/test_blame.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import requests
+
 from .utils import *
 
 
 def test_blame():
     with serve():
         response = requests.get(UNAUTH_TEST_REPO_URL + "blame/HEAD/test.c")
         assert response.status_code == 200
```

### Comparing `klaus-2.0.3/tests/test_contrib.py` & `klaus-3.0.0/tests/test_contrib.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     pass
 
 import subprocess
 
 import pytest
 import requests
 
-
 from klaus.contrib import app_args
+
 from .utils import *
 
 
 def check_env(env, expected_args, expected_kwargs):
     os.environ.update(env)
     args, kwargs = app_args.get_args_from_env()
     assert args == expected_args
```

### Comparing `klaus-2.0.3/tests/test_make_app.py` & `klaus-3.0.0/tests/test_make_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import re
+import shutil
 import subprocess
 import tempfile
-import shutil
-import klaus
 
 import pytest
 import requests
 import requests.auth
 
+import klaus
+
 from .utils import *
 
 
 def test_make_app_using_list():
     app = klaus.make_app(REPOS, TEST_SITE_NAME)
     with serve_app(app):
         response = requests.get(UNAUTH_TEST_SERVER).text
@@ -136,15 +137,15 @@
 def can_clone_auth():
     return _can_clone(_GET_auth, AUTH_TEST_REPO_URL)
 
 
 def _can_clone(http_get, url):
     tmp = tempfile.mkdtemp()
     try:
-        return any(
+        return all(
             [
                 "git clone" in http_get(TEST_REPO_BASE_URL).text,
                 _check_http200(
                     http_get, TEST_REPO_BASE_URL + "info/refs?service=git-upload-pack"
                 ),
                 subprocess.call(["git", "clone", url, tmp]) == 0,
             ]
@@ -159,20 +160,22 @@
 
 
 def can_push_auth():
     return _can_push(_GET_auth, AUTH_TEST_REPO_URL)
 
 
 def _can_push(http_get, url):
-    return any(
+    return all(
         [
-            _check_http200(
-                http_get, TEST_REPO_BASE_URL + "info/refs?service=git-receive-pack"
-            ),
-            _check_http200(http_get, TEST_REPO_BASE_URL + "git-receive-pack"),
+            any([
+                _check_http200(
+                    http_get, TEST_REPO_BASE_URL + "info/refs?service=git-receive-pack"
+                ),
+                _check_http200(http_get, TEST_REPO_BASE_URL + "git-receive-pack"),
+            ]),
             subprocess.call(["git", "push", url, "master"], cwd=TEST_REPO) == 0,
         ]
     )
 
 
 # Ctags
 def ctags_tags_and_branches():
@@ -190,17 +193,17 @@
     assert len(all_refs) == 3
     return all(
         _ctags_enabled(ref, f) for ref in all_refs for f in ["test.c", "test.js"]
     )
 
 
 def _ctags_enabled(ref, filename):
-    response = requests.get(UNAUTH_TEST_REPO_URL + "blob/%s/%s" % (ref, filename))
+    response = requests.get(UNAUTH_TEST_REPO_URL + f"blob/{ref}/{filename}")
     assert response.status_code == 200, response.text
-    href = '<a href="/%sblob/%s/%s#L-1">' % (TEST_REPO_BASE_URL, ref, filename)
+    href = f'<a href="/{TEST_REPO_BASE_URL}blob/{ref}/{filename}#L-1">'
     return href in response.text
 
 
 def _GET_unauth(url=""):
     return requests.get(
         UNAUTH_TEST_SERVER + url,
         auth=requests.auth.HTTPDigestAuth("invalid", "password"),
```

### Comparing `klaus-2.0.3/tests/test_manpage.py` & `klaus-3.0.0/tests/test_manpage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import re
-import subprocess
 import shutil
+import subprocess
+from unittest import mock
 
-try:
-    from unittest import mock
-except ImportError:
-    import mock
 from klaus.utils import force_unicode
 
 
 def test_covers_all_cli_options():
     if hasattr(shutil, "which") and not shutil.which("man"):
         return
 
     import klaus.cli
 
     manpage = force_unicode(subprocess.check_output(["man", "./klaus.1"]))
 
     def assert_in_manpage(s):
         def clean(x):
             return re.sub("(.\\x08)|\\s", "", x)
+
         assert clean(s) in clean(manpage), "%r not found in manpage" % s
 
     mock_parser = mock.Mock()
     with mock.patch("argparse.ArgumentParser") as mock_cls:
         mock_cls.return_value = mock_parser
         klaus.cli.make_parser()
```

### Comparing `klaus-2.0.3/tests/test_utils.py` & `klaus-3.0.0/tests/test_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 import sys
 import unittest
-
-try:
-    from unittest import mock
-except ImportError:
-    import mock
+from unittest import mock
 
 from klaus import utils
 
 
 class ForceUnicodeTests(unittest.TestCase):
     def test_ascii(self):
-        self.assertEqual(u"foo", utils.force_unicode(b"foo"))
+        self.assertEqual("foo", utils.force_unicode(b"foo"))
 
     def test_utf8(self):
         if sys.version_info[0] < 3:
             return
         self.assertEqual(eval(r'"f\xce"'), utils.force_unicode(eval(r'b"f\xc3\x8e"')))
 
     def test_invalid(self):
@@ -33,9 +29,9 @@
             ("0.1", "klaus-0.1"),
             (
                 "b3e70e08344ca3f83cc7033ecdbefa90443d7d2e",
                 "klaus@b3e70e08344ca3f83cc7033ecdbefa90443d7d2e",
             ),
             ("vanilla", "klaus-vanilla"),
         ]
-        for (rev, basename) in examples:
+        for rev, basename in examples:
             self.assertEqual(utils.tarball_basename("klaus", rev), basename)
```

### Comparing `klaus-2.0.3/tests/test_views.py` & `klaus-3.0.0/tests/test_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import contextlib
+import tarfile
 from io import BytesIO
+
 import requests
-import tarfile
-import contextlib
+
 from .utils import *
 
 
 def test_repo_list():
     with serve():
         response = requests.get(UNAUTH_TEST_SERVER).text
         assert TEST_REPO_BASE_URL in response
```

