# Comparing `tmp/JustDeepIt-0.2.2.tar.gz` & `tmp/JustDeepIt-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JustDeepIt-0.2.2.tar", last modified: Thu May 16 06:15:03 2024, max compression
+gzip compressed data, was "JustDeepIt-0.2.3.tar", last modified: Thu May 23 01:54:21 2024, max compression
```

## Comparing `JustDeepIt-0.2.2.tar` & `JustDeepIt-0.2.3.tar`

### file list

```diff
@@ -1,53 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:15:03.257052 JustDeepIt-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:15:03.253052 JustDeepIt-0.2.2/JustDeepIt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-16 06:15:03.000000 JustDeepIt-0.2.2/JustDeepIt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-16 06:15:03.000000 JustDeepIt-0.2.2/JustDeepIt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 06:15:03.000000 JustDeepIt-0.2.2/JustDeepIt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-16 06:15:03.000000 JustDeepIt-0.2.2/JustDeepIt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-16 06:15:03.000000 JustDeepIt-0.2.2/JustDeepIt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 06:15:03.000000 JustDeepIt-0.2.2/JustDeepIt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 06:15:03.000000 JustDeepIt-0.2.2/JustDeepIt.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-16 06:15:03.257052 JustDeepIt-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:15:03.253052 JustDeepIt-0.2.2/justdeepit/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:15:03.253052 JustDeepIt-0.2.2/justdeepit/app/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25983 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/appbase.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/appis.py
--rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/appod.py
--rw-r--r--   0 runner    (1001) docker     (127)    22300 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/appsod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:15:03.253052 JustDeepIt-0.2.2/justdeepit/app/static/
--rw-r--r--   0 runner    (1001) docker     (127)    89501 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/static/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   137972 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/static/jquery-3.6.0.min.map
--rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/static/styles.css
--rw-r--r--   0 runner    (1001) docker     (127)    58702 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/static/tree.jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)   174878 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/static/tree.jquery.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    22813 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/static/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:15:03.253052 JustDeepIt-0.2.2/justdeepit/app/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    17293 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/templates/module.html
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/templates/shutdown.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:15:03.257052 JustDeepIt-0.2.2/justdeepit/models/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    12931 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/models/instance_segment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/models/object_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/models/salient_object_detect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:15:03.257052 JustDeepIt-0.2.2/justdeepit/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/models/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    13883 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/models/utils/mmdetbase.py
--rw-r--r--   0 runner    (1001) docker     (127)    36052 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/models/utils/u2net.py
--rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/models/utils/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:15:03.249052 JustDeepIt-0.2.2/justdeepit/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:15:03.257052 JustDeepIt-0.2.2/justdeepit/src/font/
--rw-r--r--   0 runner    (1001) docker     (127)   555264 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/src/font/NotoSans-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/src/font/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)    56860 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 06:15:03.257052 JustDeepIt-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.725402 JustDeepIt-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.717402 JustDeepIt-0.2.3/JustDeepIt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-23 01:54:21.000000 JustDeepIt-0.2.3/JustDeepIt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-23 01:54:21.000000 JustDeepIt-0.2.3/JustDeepIt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:54:21.000000 JustDeepIt-0.2.3/JustDeepIt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 01:54:21.000000 JustDeepIt-0.2.3/JustDeepIt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-23 01:54:21.000000 JustDeepIt-0.2.3/JustDeepIt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 01:54:21.000000 JustDeepIt-0.2.3/JustDeepIt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:54:21.000000 JustDeepIt-0.2.3/JustDeepIt.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-23 01:54:21.725402 JustDeepIt-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.717402 JustDeepIt-0.2.3/justdeepit/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.717402 JustDeepIt-0.2.3/justdeepit/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24123 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/appbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/appis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/appod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22300 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/appsod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.717402 JustDeepIt-0.2.3/justdeepit/app/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    89501 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   137972 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jquery-3.6.0.min.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.717402 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.721402 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      464 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/application.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      603 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/code.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      618 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/css.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      579 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/db.png
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/directory-lock.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      537 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/directory.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      651 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/doc.png
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/file-lock.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      294 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/file.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      653 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/film.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      582 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/flash.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      583 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/folder_open.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      734 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/html.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      633 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/java.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      668 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/linux.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      385 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/music.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      591 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/pdf.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      538 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/php.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      606 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/picture.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      588 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/ppt.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      856 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/psd.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      626 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/ruby.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      859 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/script.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2530 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/spinner.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      342 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/txt.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      663 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/xls.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      386 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/zip.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/jQueryFileTree.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7361 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/jQueryFileTree.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)    20646 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.721402 JustDeepIt-0.2.3/justdeepit/app/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    17454 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/templates/module.html
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/templates/shutdown.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.721402 JustDeepIt-0.2.3/justdeepit/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12931 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/models/instance_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/models/object_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/models/salient_object_detect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.725402 JustDeepIt-0.2.3/justdeepit/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/models/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13883 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/models/utils/mmdetbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36052 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/models/utils/u2net.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/models/utils/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.713402 JustDeepIt-0.2.3/justdeepit/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.725402 JustDeepIt-0.2.3/justdeepit/src/font/
+-rw-r--r--   0 runner    (1001) docker     (127)   555264 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/src/font/NotoSans-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/src/font/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    56860 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 01:54:21.725402 JustDeepIt-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/setup.py
```

### Comparing `JustDeepIt-0.2.2/JustDeepIt.egg-info/PKG-INFO` & `JustDeepIt-0.2.3/JustDeepIt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JustDeepIt
-Version: 0.2.2
+Version: 0.2.3
 Summary: a GUI tool for object detection and segmentation based on deep learning
 Home-page: https://github.com/biunit/JustDeepIt
 Author: Jianqiang Sun
 Author-email: sun@biunit.dev
 License: MIT
 Keywords: object detection,object segmentation
 Platform: UNKNOWN
@@ -14,9 +14,9 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 License-File: LICENSE
 
-Deep learning has been applied to solve various problems, especially in image recognition, across many fields including the life sciences and agriculture. Many studies have reported the use of deep learning to identify plant and insect species, detect flowers and fruits, segment plant individuals from fixed-point observation cameras or drone images, and other applications. Programming languages such as Python and its libraries including PyTorch, MMDetection, and Detectron2 have made deep learning easier and more accessible to researchers. However, it remains difficult for many researchers without advanced programming skills to use deep learning and environments such as the character user interface (CUI) through keyboard input. JustDeepIt aims to support researchers by facilitating the use of deep learning for object detection and segmentation by providing both graphical user interface (GUI) and CUI operations. JustDeepIt can be used for plant detection, pest detection, and a variety of tasks in life sciences, agriculture, and other fields.
+Deep learning has been applied to solve various problems, especially in image recognition, across many fields including the life sciences and agriculture. Many studies have reported the use of deep learning to identify plant and insect species, detect flowers and fruits, segment plant individuals from fixed-point observation cameras or drone images, and other applications. Programming languages such as Python and its libraries including PyTorch and MMDetection have made deep learning easier and more accessible to researchers. However, it remains difficult for many researchers without advanced programming skills to use deep learning and environments such as the character user interface (CUI) through keyboard input. JustDeepIt aims to support researchers by facilitating the use of deep learning for object detection and segmentation by providing both graphical user interface (GUI) and CUI operations. JustDeepIt can be used for plant detection, pest detection, and a variety of tasks in life sciences, agriculture, and other fields.
```

### Comparing `JustDeepIt-0.2.2/LICENSE` & `JustDeepIt-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.2/PKG-INFO` & `JustDeepIt-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JustDeepIt
-Version: 0.2.2
+Version: 0.2.3
 Summary: a GUI tool for object detection and segmentation based on deep learning
 Home-page: https://github.com/biunit/JustDeepIt
 Author: Jianqiang Sun
 Author-email: sun@biunit.dev
 License: MIT
 Keywords: object detection,object segmentation
 Platform: UNKNOWN
@@ -14,9 +14,9 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 License-File: LICENSE
 
-Deep learning has been applied to solve various problems, especially in image recognition, across many fields including the life sciences and agriculture. Many studies have reported the use of deep learning to identify plant and insect species, detect flowers and fruits, segment plant individuals from fixed-point observation cameras or drone images, and other applications. Programming languages such as Python and its libraries including PyTorch, MMDetection, and Detectron2 have made deep learning easier and more accessible to researchers. However, it remains difficult for many researchers without advanced programming skills to use deep learning and environments such as the character user interface (CUI) through keyboard input. JustDeepIt aims to support researchers by facilitating the use of deep learning for object detection and segmentation by providing both graphical user interface (GUI) and CUI operations. JustDeepIt can be used for plant detection, pest detection, and a variety of tasks in life sciences, agriculture, and other fields.
+Deep learning has been applied to solve various problems, especially in image recognition, across many fields including the life sciences and agriculture. Many studies have reported the use of deep learning to identify plant and insect species, detect flowers and fruits, segment plant individuals from fixed-point observation cameras or drone images, and other applications. Programming languages such as Python and its libraries including PyTorch and MMDetection have made deep learning easier and more accessible to researchers. However, it remains difficult for many researchers without advanced programming skills to use deep learning and environments such as the character user interface (CUI) through keyboard input. JustDeepIt aims to support researchers by facilitating the use of deep learning for object detection and segmentation by providing both graphical user interface (GUI) and CUI operations. JustDeepIt can be used for plant detection, pest detection, and a variety of tasks in life sciences, agriculture, and other fields.
```

### Comparing `JustDeepIt-0.2.2/README.md` & `JustDeepIt-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.2/justdeepit/app/app.py` & `JustDeepIt-0.2.3/justdeepit/app/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -556,95 +556,40 @@
                     log_record = '<p class="log-newpage"></p>'
                 else:
                     log_record = f'<p>{log_record}</p>'
                 log_records += log_record
     return log_records
 
 
-
-@app.get('/api/dirtree')
-def get_dirtree(request: Request, dirpath=None, include_file=1):
-    if dirpath is None:
+@app.post('/api/dirtree')
+async def get_dirtree(request: Request):
+    form = await request.form()    
+    dirpath = form.get('dir')
+    if dirpath is None or dirpath == 'null':
         dirpath = APP_ROOT_PATH
     else:
         dirpath = os.path.join(APP_ROOT_PATH, dirpath)
     
-    def __get_filetree(dirpath, idx_start, include_file, n_files_cutoff=20):
-        filetree_dict = []
-        n_files = [0, 0] # (directories, files)
-        
-        # check #files
-        for fpath in sorted(os.listdir(dirpath)):
-            if fpath.startswith('.'):
-                continue
-            fpath = os.path.join(dirpath, fpath)
-            if  os.path.isdir(os.path.join(dirpath, fpath)):
-                n_files[0] += 1
-            if os.path.isfile(fpath):
-                n_files[1] += 1
-            
-        # walk directories
-        for fpath in sorted(os.listdir(dirpath)):
-            if fpath.startswith('.'):
-                continue
-            fpath = os.path.join(dirpath, fpath)
+    ftree = ['<ul class="jqueryFileTree" style="display: none;">']
+    try:
+        ftree = ['<ul class="jqueryFileTree" style="display: none;">']
+        for fname in os.listdir(dirpath):
+            fpath =os.path.join(dirpath, fname)
             if os.path.isdir(fpath):
-                idx_start[0] += 1
-                filetree_dict.append({
-                    'id': idx_start[0],
-                    'name': os.path.basename(fpath),
-                    'children': __get_filetree(fpath, idx_start, include_file),
-                })
-            elif os.path.isfile(fpath):
-                if include_file == 1 and n_files[1] <= n_files_cutoff:
-                    idx_start[0] += 1
-                    filetree_dict.append({
-                        'id': idx_start[0],
-                        'name': os.path.basename(fpath),
-                    })
-                
-        # if #files is larger than the cutoff, set '...' to represent files.
-        if include_file == 1 and n_files[1] > n_files_cutoff:
-            idx_start[0] += 1
-            filetree_dict.append({
-                'id': idx_start[0],
-                'name': '...',
-            })
-
-        return filetree_dict
-    
-    if os.path.exists(dirpath):
-        idx_start = [0]
-        filetree_dict = [{
-            'id': 0,
-            'name': dirpath,
-            'children': __get_filetree(dirpath, idx_start, include_file)
-        }]
-    else:
-        filetree_dict = []
-    
-    return JSONResponse(content=filetree_dict)
-
-
-
-
-#@app.get('/api/modelconfig')
-#def get_modelconfig(config_fpath):
-#    response_data = {'data': '', 'status': ''}
-#    if os.path.exists(config_fpath):
-#        with open(config_fpath, 'r') as configfh:
-#            for line in configfh:
-#                response_data['data'] += line
-#        response_data['status'] = '[{}]     SUCCESS: The config file has been loaded.'.format(datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S'))
-#    else:
-#        response_data['status'] = '[{}]     ERROR: FileNotFound, check the file path to the config file.'.format(datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S'))
-#    return JSONResponse(content=response_data)
+                ftree.append(f'<li class="directory collapsed"><a rel="{fpath}/">{fname}</a></li>')
+            else:
+                e = os.path.splitext(fname)[1][1:]
+                ftree.append(f'<li class="file ext_{e}"><a rel="{fpath}">{fname}</a></li>')
+        ftree.append('</ul>')
+    except Exception(e):
+        ftree.append(f'Could not load directory: {str(e)}')
+    ftree.append('</ul>')
+    return HTMLResponse(''.join(ftree))
 
 
- 
 @app.post('/api/modelconfig')
 async def update_modelconfig(request: Request):
     form = await request.form()
     config_fpath = form.get('file_path')
     config_data = form.get('data')
     response_data = {'data': config_data, 'status': ''}
     if os.path.exists(config_fpath):
@@ -684,16 +629,18 @@
     global server
     server.keep_running = False
     
 
 @app.post("/app/shutdown")
 async def shutdown_server(request: Request, background_tasks: BackgroundTasks):
     background_tasks.add_task(__shutdown_server)
-    return templates.TemplateResponse('shutdown.html', {'request': request,
-        'justdeepit_version': justdeepit.__version__})
+    return templates.TemplateResponse('shutdown.html', {
+        'request': request,
+        'version': justdeepit.__version__
+    })
 
 
 def run_app():
     with server.run_in_thread():
         while server.keep_running:
             time.sleep(1)
```

### Comparing `JustDeepIt-0.2.2/justdeepit/app/appbase.py` & `JustDeepIt-0.2.3/justdeepit/app/appbase.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.2/justdeepit/app/appis.py` & `JustDeepIt-0.2.3/justdeepit/app/appis.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.2/justdeepit/app/appod.py` & `JustDeepIt-0.2.3/justdeepit/app/appod.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.2/justdeepit/app/appsod.py` & `JustDeepIt-0.2.3/justdeepit/app/appsod.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.2/justdeepit/app/static/jquery-3.6.0.min.js` & `JustDeepIt-0.2.3/justdeepit/app/static/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.2/justdeepit/app/static/jquery-3.6.0.min.map` & `JustDeepIt-0.2.3/justdeepit/app/static/jquery-3.6.0.min.map`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.2/justdeepit/app/static/styles.css` & `JustDeepIt-0.2.3/justdeepit/app/static/styles.css`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.2/justdeepit/app/static/utils.js` & `JustDeepIt-0.2.3/justdeepit/app/static/utils.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -125,15 +125,14 @@
 function setSelectedFile(selectFieldId = 'filetree-selected') {
     selectedFilePath = $('#' + selectFieldId).val();
     if (focusedInputField == 'module--TRAIN--model_weight') {
         if (selectedFilePath.slice((selectedFilePath.lastIndexOf(".") - 1 >>> 0) + 2) !== 'pth') {
             selectedFilePath = selectedFilePath + '.pth';
         }
     }
-    console.log(selectedFilePath);
     $('#' + focusedInputField).val(selectedFilePath);
     focusedInputField = null;
     refreshExecuteButtons();
     $('#select-file-popup').fadeOut();
 }
 
 
@@ -416,55 +415,38 @@
     // open sub-window to select file/folder when clicking Select buttons
     $('button.select-file').on('click', function() {
         let _ = $(this).val().split('+');
         focusedInputField = _[0];
         let selectType = _[1];
         let btn_id = $(this).attr('id');
 
-        $.ajax({
-            type: 'GET',
-            url: '/api/dirtree',
-            dataType: 'json',
-            cache: false,
-        }).done(function(dirtree, textStatus, jqXHR) {
-            $('#filetree').tree('destroy');
-            $('#filetree').tree({
-                openedIcon: '&#x0229F;',
-                closedIcon: '&#x0229E;',
-                showEmptyFolder: true,
-                autoOpen: 0,
-                selectable: true,
-                data: dirtree,
-            });
-            if (selectType === 'any') {
-                selectType = 'folder';
-                if ($('#module--TRAIN--trainannfmt').val() === 'COCO' && btn_id === 'module--TRAIN--trainann--button') {
-                    selectType = 'file';
-                }
-                if ($('#module--TRAIN--validannfmt').val() === 'COCO' && btn_id === 'module--TRAIN--validann--button') {
-                    selectType = 'file';
-                }
-                if ($('#module--TRAIN--testannfmt').val() === 'COCO' && btn_id === 'module--TRAIN--testann--button') {
-                    selectType = 'file';
-                }
+        $('#filetree').fileTree();
+
+        if (selectType === 'any') {
+            selectType = 'folder';
+            if ($('#module--TRAIN--trainannfmt').val() === 'COCO' && btn_id === 'module--TRAIN--trainann--button') {
+                selectType = 'file';
             }
-            console.log(selectType);
-            $('#filetree-required-filetype').val(selectType);
-            if (selectType === 'file') {
-                $('#filetree-select-msgbox').text(msgSelectFile);
-            } else {
-                $('#filetree-select-msgbox').text(msgSelectFolder);
+            if ($('#module--TRAIN--validannfmt').val() === 'COCO' && btn_id === 'module--TRAIN--validann--button') {
+                selectType = 'file';
             }
-            $('#filetree-selected').val($('#' + focusedInputField).val());
-            $('#select-file-popup').fadeIn();
-        }).fail(function(XMLHttpRequest, textStatus, errorThrown) {
-            console.log("XMLHttpRequest : " + XMLHttpRequest.status);
-            console.log("textStatus     : " + textStatus);
-            console.log("errorThrown    : " + errorThrown.message);
-        });
+            if ($('#module--TRAIN--testannfmt').val() === 'COCO' && btn_id === 'module--TRAIN--testann--button') {
+                selectType = 'file';
+            }
+        }
+
+        $('#filetree-required-filetype').val(selectType);
+        if (selectType === 'file') {
+            $('#filetree-select-msgbox').text(msgSelectFile);
+        } else {
+            $('#filetree-select-msgbox').text(msgSelectFolder);
+        }
+        $('#filetree-selected').val($('#' + focusedInputField).val());
+        $('#select-file-popup').fadeIn();
+
     });
     // close select-file-popup window
     $('body').on('click', '#select-file-popup', function(e) {
         if (!$(e.target).closest('#select-file-manager').length) {
             $('#select-file-popup').fadeOut();
         }
     });
@@ -472,35 +454,28 @@
         $('#select-file-popup').fadeOut();
     });
     // set the selected path
     $('body').on('click', '#selectFile', function() {
         setSelectedFile();
     });
 
-
     $('body').on('click', '#filetree', function() {
-        // wait for JqTree to set up the selected file
-        setTimeout(function() {
-            $('#filetree-selected').val(node2path($('#filetree').tree('getSelectedNode')).slice(1));
-            $('#filetree-selected').data('val', node2path($('#filetree').tree('getSelectedNode')).slice(1));
-            $('#filetree-selected-filetype').val(node2filetype($('#filetree').tree('getSelectedNode')));
-
-            if ($('#filetree-required-filetype').val() === $('#filetree-selected-filetype').val()) {
-                $('#selectFile').removeClass('button-disable');
-                $('#selectFile').attr('disabled', false);
-            } else {
-                $('#selectFile').addClass('button-disable');
-                $('#selectFile').attr('disabled', true);
-                if (($('#filetree-required-filetype').val() === 'file') && ($('#filetree-selected-filetype').val() === 'folder')) {
-                    $('#filetree-select-msgbox').text(msgSelectFile);
-                } else if (($('#filetree-required-filetype').val() === 'folder') && ($('#filetree-selected-filetype').val() === 'file')) {
-                    $('#filetree-select-msgbox').text(msgSelectFolder);
-                }
+        if ($('#filetree-required-filetype').val() === $('#filetree-selected-filetype').val()) {
+            $('#selectFile').removeClass('button-disable');
+            $('#selectFile').attr('disabled', false);
+        } else {
+            $('#selectFile').addClass('button-disable');
+            $('#selectFile').attr('disabled', true);
+            if (($('#filetree-required-filetype').val() === 'file') && ($('#filetree-selected-filetype').val() === 'folder')) {
+                $('#filetree-select-msgbox').text(msgSelectFile);
+            } else if (($('#filetree-required-filetype').val() === 'folder') && ($('#filetree-selected-filetype').val() === 'file')) {
+                $('#filetree-select-msgbox').text(msgSelectFolder);
             }
-        }, 300);
+        }
+
     });
     // check users whether write file name or not
     $('body').on('keyup keypress blur change', '#filetree-selected', function(e) {
         if ($('#filetree-required-filetype').val() === 'file' && $('#filetree-selected-filetype').val() === 'folder') {
             if (($(this).data('val') === $(this).val()) | ($(this).val().slice(-1)) === '/') {
                 $('#selectFile').addClass('button-disable');
                 $('#selectFile').attr('disabled', true);
@@ -511,34 +486,14 @@
                     setSelectedFile();
                 }
             }
         }
     });
 
 
-    /*
-    $('button#config-edition-open').on('click', function() {
-        $.ajax({
-            type: 'GET',
-            url: '/api/modelconfig',
-            data: {config_fpath: $('#module--BASE--config').val()},
-            dataType: 'json',
-            cache: false,
-        }).done(function(config_content, textStatus, jqXHR) {
-            $('#config-edition-msgbox').text(config_content['status']);
-            $('#config-edition-content').val(config_content['data']);
-            $('#config-edition-popup').fadeIn();
-        }).fail(function(XMLHttpRequest, textStatus, errorThrown) {
-                console.log("XMLHttpRequest : " + XMLHttpRequest.status);
-                console.log("textStatus     : " + textStatus);
-                console.log("errorThrown    : " + errorThrown.message);
-        });
-    });
-    */
-
     $('body').on('click', '#config-edition-popup', function(e) {
         if (!$(e.target).closest('#config-edition-manager').length) {
             $('#config-edition-popup').fadeOut();
         }
     });
     $('body').on('click', '#config-edition-close', function() {
         $('#config-edition-popup').fadeOut();
@@ -598,14 +553,17 @@
         'mouseenter': function() {
             $(this).attr('placeholder', msgLeftBank.replace('____', 'test'));
         },
         'mouseleave': function() {
             $(this).removeAttr('placeholder');
         }
     });
+
+    $('#filetree-2').fileTree();
+
 });
 
 
 // check the running status and update logs
 refreshModule(true);
 window.setInterval(function() {
     refreshModule();
```

### Comparing `JustDeepIt-0.2.2/justdeepit/app/templates/index.html` & `JustDeepIt-0.2.3/justdeepit/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.2/justdeepit/app/templates/module.html` & `JustDeepIt-0.2.3/justdeepit/app/templates/module.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 <html>
 <head>
     <title>JustDeepIt</title>
     <link href="{{ url_for('static', path='/styles.css') }}" rel="stylesheet">
+    <link href="{{ url_for('static', path='/jqueryfiletree/jQueryFileTree.css') }}" rel="stylesheet">
     <script src="{{ url_for('static', path='/jquery-3.6.0.min.js') }}"></script>
-    <script src="{{ url_for('static', path='/tree.jquery.js') }}"></script>
+    <script src="{{ url_for('static', path='/jqueryfiletree/jQueryFileTree.js') }}"></script>
     <script src="{{ url_for('static', path='/utils.js') }}"></script>
 </head>
 <body>
     <div id="app-module-panel">
     
     <!-- JustDeepIt -->
     <table id="app-menu">
@@ -315,14 +316,15 @@
         </div>
         </div>
     </div>
     
     <div id="select-file-popup">
         <div id="select-file-manager">
             <div id="filetree-select-msgbox">&nbsp;</div>
+            <!-- div id="filetree"></div -->
             <div id="filetree"></div>
             <div>
                 <input id="filetree-selected" value=""></input>
                 <input id="filetree-selected-filetype" value="" type="hidden"></input>
                 <input id="filetree-required-filetype" value="" type="hidden"></input>
             </div>
             <div class="popup-ctrl-buttons">
@@ -341,12 +343,12 @@
             <div id="config-edition-msgbox">&nbsp;</div>
             <div class="popup-ctrl-buttons">
                 <button id="config-edition-save" type="button">SAVE</button>
                 <button id="config-edition-close" type="button">CLOSSE</button>
             </div>
         </div>
     </div>
-    
+
     <div id="version">JustDeepIt v{{version}}</div>
     </div>
 </body> 
 </html>
```

### Comparing `JustDeepIt-0.2.2/justdeepit/app/templates/shutdown.html` & `JustDeepIt-0.2.3/justdeepit/app/templates/shutdown.html`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.2/justdeepit/models/instance_segment.py` & `JustDeepIt-0.2.3/justdeepit/models/instance_segment.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.2/justdeepit/models/object_detect.py` & `JustDeepIt-0.2.3/justdeepit/models/object_detect.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.2/justdeepit/models/salient_object_detect.py` & `JustDeepIt-0.2.3/justdeepit/models/salient_object_detect.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.2/justdeepit/models/utils/data.py` & `JustDeepIt-0.2.3/justdeepit/models/utils/data.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.2/justdeepit/models/utils/mmdetbase.py` & `JustDeepIt-0.2.3/justdeepit/models/utils/mmdetbase.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.2/justdeepit/models/utils/u2net.py` & `JustDeepIt-0.2.3/justdeepit/models/utils/u2net.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.2/justdeepit/models/utils/unet.py` & `JustDeepIt-0.2.3/justdeepit/models/utils/unet.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.2/justdeepit/src/font/NotoSans-Medium.ttf` & `JustDeepIt-0.2.3/justdeepit/src/font/NotoSans-Medium.ttf`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.2/justdeepit/src/font/OFL.txt` & `JustDeepIt-0.2.3/justdeepit/src/font/OFL.txt`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.2/justdeepit/utils.py` & `JustDeepIt-0.2.3/justdeepit/utils.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.2/setup.py` & `JustDeepIt-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 package_desc = 'Deep learning has been applied to solve various problems, especially in image recognition, '\
     'across many fields including the life sciences and agriculture. '\
     'Many studies have reported the use of deep learning to identify plant and insect species, '\
     'detect flowers and fruits, segment plant individuals from fixed-point observation cameras or drone images, '\
     'and other applications. '\
-    'Programming languages such as Python and its libraries including PyTorch, MMDetection, and Detectron2 ' \
+    'Programming languages such as Python and its libraries including PyTorch and MMDetection ' \
     'have made deep learning easier and more accessible to researchers. '\
     'However, it remains difficult for many researchers without advanced programming skills '\
     'to use deep learning and environments such as the character user interface (CUI) through keyboard input. '\
     'JustDeepIt aims to support researchers by facilitating the use of deep learning for object detection and segmentation '\
     'by providing both graphical user interface (GUI) and CUI operations. '\
     'JustDeepIt can be used for plant detection, pest detection, '\
     'and a variety of tasks in life sciences, agriculture, and other fields.'
```

