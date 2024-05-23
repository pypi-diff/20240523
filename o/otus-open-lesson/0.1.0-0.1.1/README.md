# Comparing `tmp/otus_open_lesson-0.1.0.tar.gz` & `tmp/otus_open_lesson-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otus_open_lesson-0.1.0.tar", last modified: Thu May 23 15:12:37 2024, max compression
+gzip compressed data, was "otus_open_lesson-0.1.1.tar", last modified: Thu May 23 15:17:41 2024, max compression
```

## Comparing `otus_open_lesson-0.1.0.tar` & `otus_open_lesson-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:12:37.295402 otus_open_lesson-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-23 15:12:27.000000 otus_open_lesson-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-23 15:12:37.295402 otus_open_lesson-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-23 15:12:27.000000 otus_open_lesson-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:12:37.295402 otus_open_lesson-0.1.0/otus_open_lesson/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:12:27.000000 otus_open_lesson-0.1.0/otus_open_lesson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:12:27.000000 otus_open_lesson-0.1.0/otus_open_lesson/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 15:12:27.000000 otus_open_lesson-0.1.0/otus_open_lesson/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:12:37.295402 otus_open_lesson-0.1.0/otus_open_lesson/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:12:27.000000 otus_open_lesson-0.1.0/otus_open_lesson/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-23 15:12:27.000000 otus_open_lesson-0.1.0/otus_open_lesson/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 15:12:27.000000 otus_open_lesson-0.1.0/otus_open_lesson/package.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-23 15:12:27.000000 otus_open_lesson-0.1.0/otus_open_lesson/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:12:27.000000 otus_open_lesson-0.1.0/otus_open_lesson/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:12:37.295402 otus_open_lesson-0.1.0/otus_open_lesson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-23 15:12:37.000000 otus_open_lesson-0.1.0/otus_open_lesson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-23 15:12:37.000000 otus_open_lesson-0.1.0/otus_open_lesson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:12:37.000000 otus_open_lesson-0.1.0/otus_open_lesson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 15:12:37.000000 otus_open_lesson-0.1.0/otus_open_lesson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:12:37.295402 otus_open_lesson-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-23 15:12:27.000000 otus_open_lesson-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:17:41.078920 otus_open_lesson-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-23 15:17:37.000000 otus_open_lesson-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-23 15:17:41.078920 otus_open_lesson-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-23 15:17:37.000000 otus_open_lesson-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:17:41.078920 otus_open_lesson-0.1.1/otus_open_lesson/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:17:37.000000 otus_open_lesson-0.1.1/otus_open_lesson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:17:37.000000 otus_open_lesson-0.1.1/otus_open_lesson/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 15:17:37.000000 otus_open_lesson-0.1.1/otus_open_lesson/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:17:41.078920 otus_open_lesson-0.1.1/otus_open_lesson/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:17:37.000000 otus_open_lesson-0.1.1/otus_open_lesson/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-23 15:17:37.000000 otus_open_lesson-0.1.1/otus_open_lesson/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 15:17:37.000000 otus_open_lesson-0.1.1/otus_open_lesson/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-23 15:17:37.000000 otus_open_lesson-0.1.1/otus_open_lesson/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:17:37.000000 otus_open_lesson-0.1.1/otus_open_lesson/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:17:41.078920 otus_open_lesson-0.1.1/otus_open_lesson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-23 15:17:41.000000 otus_open_lesson-0.1.1/otus_open_lesson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-23 15:17:41.000000 otus_open_lesson-0.1.1/otus_open_lesson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:17:41.000000 otus_open_lesson-0.1.1/otus_open_lesson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 15:17:41.000000 otus_open_lesson-0.1.1/otus_open_lesson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:17:41.078920 otus_open_lesson-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-23 15:17:37.000000 otus_open_lesson-0.1.1/setup.py
```

### Comparing `otus_open_lesson-0.1.0/LICENSE` & `otus_open_lesson-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `otus_open_lesson-0.1.0/PKG-INFO` & `otus_open_lesson-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otus-open-lesson
-Version: 0.1.0
+Version: 0.1.1
 Summary: Django test package
 Home-page: https://github.com/danteonline/otus-open-lesson
 Author: DanteOnline
 Author-email: iamdanteonline@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/danteonline/otus-open-lesson
 Project-URL: Tracker, https://github.com/danteonline/otus-open-lesson/issues
@@ -35,15 +35,14 @@
 - [Mission](#mission)
 - [Open Source Project](#open-source-project)
 - [Features](#features)
 - [Requirements](#requirements)
 - [Development Status](#development-status)
 - [Install](#install)
 - [Quickstart](#quickstart)
-- [Contributing](#contributing)
 
 ## Mission
 
 To demonstrate how to create python-django package with test cases
 
 ## Features
```

### Comparing `otus_open_lesson-0.1.0/README.md` & `otus_open_lesson-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 - [Mission](#mission)
 - [Open Source Project](#open-source-project)
 - [Features](#features)
 - [Requirements](#requirements)
 - [Development Status](#development-status)
 - [Install](#install)
 - [Quickstart](#quickstart)
-- [Contributing](#contributing)
 
 ## Mission
 
 To demonstrate how to create python-django package with test cases
 
 ## Features
```

### Comparing `otus_open_lesson-0.1.0/otus_open_lesson.egg-info/PKG-INFO` & `otus_open_lesson-0.1.1/otus_open_lesson.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otus-open-lesson
-Version: 0.1.0
+Version: 0.1.1
 Summary: Django test package
 Home-page: https://github.com/danteonline/otus-open-lesson
 Author: DanteOnline
 Author-email: iamdanteonline@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/danteonline/otus-open-lesson
 Project-URL: Tracker, https://github.com/danteonline/otus-open-lesson/issues
@@ -35,15 +35,14 @@
 - [Mission](#mission)
 - [Open Source Project](#open-source-project)
 - [Features](#features)
 - [Requirements](#requirements)
 - [Development Status](#development-status)
 - [Install](#install)
 - [Quickstart](#quickstart)
-- [Contributing](#contributing)
 
 ## Mission
 
 To demonstrate how to create python-django package with test cases
 
 ## Features
```

### Comparing `otus_open_lesson-0.1.0/setup.py` & `otus_open_lesson-0.1.1/setup.py`

 * *Files identical despite different names*

