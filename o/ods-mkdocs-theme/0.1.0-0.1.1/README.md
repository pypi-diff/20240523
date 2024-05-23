# Comparing `tmp/ods-mkdocs-theme-0.1.0.tar.gz` & `tmp/ods-mkdocs-theme-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ods-mkdocs-theme-0.1.0.tar", last modified: Wed Sep 27 12:39:16 2023, max compression
+gzip compressed data, was "ods-mkdocs-theme-0.1.1.tar", last modified: Thu May 23 14:26:06 2024, max compression
```

## Comparing `ods-mkdocs-theme-0.1.0.tar` & `ods-mkdocs-theme-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 ju         (501) staff       (20)        0 2023-09-27 12:39:16.309689 ods-mkdocs-theme-0.1.0/
--rw-r--r--   0 ju         (501) staff       (20)     1062 2023-09-27 10:29:14.000000 ods-mkdocs-theme-0.1.0/LICENSE
--rw-r--r--   0 ju         (501) staff       (20)      199 2023-09-27 11:44:50.000000 ods-mkdocs-theme-0.1.0/MANIFEST.in
--rw-r--r--   0 ju         (501) staff       (20)      811 2023-09-27 11:56:56.000000 ods-mkdocs-theme-0.1.0/NOTICE.txt
--rw-r--r--   0 ju         (501) staff       (20)      368 2023-09-27 12:39:16.309569 ods-mkdocs-theme-0.1.0/PKG-INFO
--rw-r--r--   0 ju         (501) staff       (20)     1505 2023-09-27 10:35:51.000000 ods-mkdocs-theme-0.1.0/README.md
-drwxr-xr-x   0 ju         (501) staff       (20)        0 2023-09-27 12:39:16.308254 ods-mkdocs-theme-0.1.0/ods_mkdocs_theme/
--rw-r--r--   0 ju         (501) staff       (20)        0 2023-09-27 11:50:18.000000 ods-mkdocs-theme-0.1.0/ods_mkdocs_theme/__init__.py
-drwxr-xr-x   0 ju         (501) staff       (20)        0 2023-09-27 12:39:16.307419 ods-mkdocs-theme-0.1.0/ods_mkdocs_theme/assets/
-drwxr-xr-x   0 ju         (501) staff       (20)        0 2023-09-27 12:39:16.309213 ods-mkdocs-theme-0.1.0/ods_mkdocs_theme/assets/images/
--rw-r--r--   0 ju         (501) staff       (20)     4286 2023-09-27 11:50:18.000000 ods-mkdocs-theme-0.1.0/ods_mkdocs_theme/assets/images/favicon.ico
--rw-r--r--   0 ju         (501) staff       (20)     1790 2023-09-27 11:50:18.000000 ods-mkdocs-theme-0.1.0/ods_mkdocs_theme/assets/images/orange-logo.svg
-drwxr-xr-x   0 ju         (501) staff       (20)        0 2023-09-27 12:39:16.309314 ods-mkdocs-theme-0.1.0/ods_mkdocs_theme/assets/stylesheets/
--rw-r--r--   0 ju         (501) staff       (20)    15914 2023-09-27 11:57:57.000000 ods-mkdocs-theme-0.1.0/ods_mkdocs_theme/assets/stylesheets/orange.css
--rw-r--r--   0 ju         (501) staff       (20)      224 2023-09-27 11:50:59.000000 ods-mkdocs-theme-0.1.0/ods_mkdocs_theme/mkdocs_theme.yml
-drwxr-xr-x   0 ju         (501) staff       (20)        0 2023-09-27 12:39:16.309429 ods-mkdocs-theme-0.1.0/ods_mkdocs_theme/partials/
--rw-r--r--   0 ju         (501) staff       (20)      328 2023-09-27 11:52:10.000000 ods-mkdocs-theme-0.1.0/ods_mkdocs_theme/partials/footer.html
-drwxr-xr-x   0 ju         (501) staff       (20)        0 2023-09-27 12:39:16.308997 ods-mkdocs-theme-0.1.0/ods_mkdocs_theme.egg-info/
--rw-r--r--   0 ju         (501) staff       (20)      368 2023-09-27 12:39:16.000000 ods-mkdocs-theme-0.1.0/ods_mkdocs_theme.egg-info/PKG-INFO
--rw-r--r--   0 ju         (501) staff       (20)      568 2023-09-27 12:39:16.000000 ods-mkdocs-theme-0.1.0/ods_mkdocs_theme.egg-info/SOURCES.txt
--rw-r--r--   0 ju         (501) staff       (20)        1 2023-09-27 12:39:16.000000 ods-mkdocs-theme-0.1.0/ods_mkdocs_theme.egg-info/dependency_links.txt
--rw-r--r--   0 ju         (501) staff       (20)       52 2023-09-27 12:39:16.000000 ods-mkdocs-theme-0.1.0/ods_mkdocs_theme.egg-info/entry_points.txt
--rw-r--r--   0 ju         (501) staff       (20)        1 2023-09-27 12:07:10.000000 ods-mkdocs-theme-0.1.0/ods_mkdocs_theme.egg-info/not-zip-safe
--rw-r--r--   0 ju         (501) staff       (20)       23 2023-09-27 12:39:16.000000 ods-mkdocs-theme-0.1.0/ods_mkdocs_theme.egg-info/requires.txt
--rw-r--r--   0 ju         (501) staff       (20)       17 2023-09-27 12:39:16.000000 ods-mkdocs-theme-0.1.0/ods_mkdocs_theme.egg-info/top_level.txt
--rw-r--r--   0 ju         (501) staff       (20)       38 2023-09-27 12:39:16.309720 ods-mkdocs-theme-0.1.0/setup.cfg
--rw-r--r--   0 ju         (501) staff       (20)      633 2023-09-27 12:23:22.000000 ods-mkdocs-theme-0.1.0/setup.py
+drwxr-xr-x   0 ju         (501) staff       (20)        0 2024-05-23 14:26:06.155381 ods-mkdocs-theme-0.1.1/
+-rw-r--r--   0 ju         (501) staff       (20)     1067 2024-01-02 06:08:27.000000 ods-mkdocs-theme-0.1.1/LICENSE
+-rw-r--r--   0 ju         (501) staff       (20)      199 2023-09-27 13:22:09.000000 ods-mkdocs-theme-0.1.1/MANIFEST.in
+-rw-r--r--   0 ju         (501) staff       (20)      782 2024-01-02 06:09:05.000000 ods-mkdocs-theme-0.1.1/NOTICE.txt
+-rw-r--r--   0 ju         (501) staff       (20)      406 2024-05-23 14:26:06.155184 ods-mkdocs-theme-0.1.1/PKG-INFO
+-rw-r--r--   0 ju         (501) staff       (20)     1505 2023-09-27 10:35:51.000000 ods-mkdocs-theme-0.1.1/README.md
+drwxr-xr-x   0 ju         (501) staff       (20)        0 2024-05-23 14:26:06.153505 ods-mkdocs-theme-0.1.1/ods_mkdocs_theme/
+-rw-r--r--   0 ju         (501) staff       (20)        0 2023-09-27 13:22:09.000000 ods-mkdocs-theme-0.1.1/ods_mkdocs_theme/__init__.py
+drwxr-xr-x   0 ju         (501) staff       (20)        0 2024-05-23 14:26:06.152698 ods-mkdocs-theme-0.1.1/ods_mkdocs_theme/assets/
+drwxr-xr-x   0 ju         (501) staff       (20)        0 2024-05-23 14:26:06.154511 ods-mkdocs-theme-0.1.1/ods_mkdocs_theme/assets/images/
+-rw-r--r--   0 ju         (501) staff       (20)     4286 2023-09-27 13:22:09.000000 ods-mkdocs-theme-0.1.1/ods_mkdocs_theme/assets/images/favicon.ico
+-rw-r--r--   0 ju         (501) staff       (20)     1790 2023-09-27 13:22:09.000000 ods-mkdocs-theme-0.1.1/ods_mkdocs_theme/assets/images/orange-logo.svg
+drwxr-xr-x   0 ju         (501) staff       (20)        0 2024-05-23 14:26:06.154617 ods-mkdocs-theme-0.1.1/ods_mkdocs_theme/assets/stylesheets/
+-rw-r--r--   0 ju         (501) staff       (20)    15919 2024-01-02 06:09:15.000000 ods-mkdocs-theme-0.1.1/ods_mkdocs_theme/assets/stylesheets/orange.css
+-rw-r--r--   0 ju         (501) staff       (20)      224 2023-09-27 13:22:09.000000 ods-mkdocs-theme-0.1.1/ods_mkdocs_theme/mkdocs_theme.yml
+drwxr-xr-x   0 ju         (501) staff       (20)        0 2024-05-23 14:26:06.154831 ods-mkdocs-theme-0.1.1/ods_mkdocs_theme/partials/
+-rw-r--r--   0 ju         (501) staff       (20)      333 2024-01-02 06:09:23.000000 ods-mkdocs-theme-0.1.1/ods_mkdocs_theme/partials/footer.html
+drwxr-xr-x   0 ju         (501) staff       (20)        0 2024-05-23 14:26:06.154985 ods-mkdocs-theme-0.1.1/ods_mkdocs_theme.egg-info/
+-rw-r--r--   0 ju         (501) staff       (20)      406 2024-05-23 14:26:06.000000 ods-mkdocs-theme-0.1.1/ods_mkdocs_theme.egg-info/PKG-INFO
+-rw-r--r--   0 ju         (501) staff       (20)      568 2024-05-23 14:26:06.000000 ods-mkdocs-theme-0.1.1/ods_mkdocs_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 ju         (501) staff       (20)        1 2024-05-23 14:26:06.000000 ods-mkdocs-theme-0.1.1/ods_mkdocs_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 ju         (501) staff       (20)       52 2024-05-23 14:26:06.000000 ods-mkdocs-theme-0.1.1/ods_mkdocs_theme.egg-info/entry_points.txt
+-rw-r--r--   0 ju         (501) staff       (20)        1 2023-09-27 12:07:10.000000 ods-mkdocs-theme-0.1.1/ods_mkdocs_theme.egg-info/not-zip-safe
+-rw-r--r--   0 ju         (501) staff       (20)       23 2024-05-23 14:26:06.000000 ods-mkdocs-theme-0.1.1/ods_mkdocs_theme.egg-info/requires.txt
+-rw-r--r--   0 ju         (501) staff       (20)       17 2024-05-23 14:26:06.000000 ods-mkdocs-theme-0.1.1/ods_mkdocs_theme.egg-info/top_level.txt
+-rw-r--r--   0 ju         (501) staff       (20)       38 2024-05-23 14:26:06.155418 ods-mkdocs-theme-0.1.1/setup.cfg
+-rw-r--r--   0 ju         (501) staff       (20)      633 2024-05-23 14:25:16.000000 ods-mkdocs-theme-0.1.1/setup.py
```

### Comparing `ods-mkdocs-theme-0.1.0/LICENSE` & `ods-mkdocs-theme-0.1.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Orange
+Copyright (c) 2023-2024 Orange
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ods-mkdocs-theme-0.1.0/NOTICE.txt` & `ods-mkdocs-theme-0.1.1/NOTICE.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Parts list under Orange SA Copyright
-Copyright (C) 2016 - 2023 Orange SA All rights reserved
+Copyright (C) 2023 - 2024 Orange SA All rights reserved
 
 The following parts are proprietary information of Orange.
 You shall not use or display any trade names, trademarks, service marks, products names, illustrations or designs used within the software
-or displayed on this website (https://boosted.orange.com) and owned by Orange SA and its subsidiaries,
+or displayed on this website and owned by Orange SA and its subsidiaries,
 in whole or part of, in any medium, except as required for reasonable and customary use in describing the origin of the software
 and reproducing the content of the NOTICE and DOCUMENTATION files.
 Any use or displaying shall constitute an infringement under intellectual property laws of France and international conventions.
 
 ods_mkdocs_theme/assets/images/favicon.ico
 ods_mkdocs_theme/assets/images/orange-logo.svg
```

### Comparing `ods-mkdocs-theme-0.1.0/README.md` & `ods-mkdocs-theme-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ods-mkdocs-theme-0.1.0/ods_mkdocs_theme/assets/images/favicon.ico` & `ods-mkdocs-theme-0.1.1/ods_mkdocs_theme/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `ods-mkdocs-theme-0.1.0/ods_mkdocs_theme/assets/images/orange-logo.svg` & `ods-mkdocs-theme-0.1.1/ods_mkdocs_theme/assets/images/orange-logo.svg`

 * *Files identical despite different names*

### Comparing `ods-mkdocs-theme-0.1.0/ods_mkdocs_theme/assets/stylesheets/orange.css` & `ods-mkdocs-theme-0.1.1/ods_mkdocs_theme/assets/stylesheets/orange.css`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*!
  * Orange Design System MkDocs Theme
- * Copyright 2023 Orange SA
+ * Copyright 2023-2024 Orange SA
  * Licensed under MIT (https://github.com/Orange-OpenSource/ods-mkdocs-theme/blob/main/LICENSE)
  */
 
 /* Orange colors */
 :root,
 [data-md-color-scheme="default"] {
   /* Primary color shades */
```

### Comparing `ods-mkdocs-theme-0.1.0/ods_mkdocs_theme.egg-info/SOURCES.txt` & `ods-mkdocs-theme-0.1.1/ods_mkdocs_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ods-mkdocs-theme-0.1.0/setup.py` & `ods-mkdocs-theme-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 
 setup(
   name='ods-mkdocs-theme',
   version=VERSION,
   url='https://github.com/Orange-OpenSource/ods-mkdocs-theme',
   license='MIT',
   description='Orange Design System MkDocs Theme provides a MkDocs theme for Orange.',
```

