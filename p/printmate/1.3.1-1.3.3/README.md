# Comparing `tmp/printmate-1.3.1.tar.gz` & `tmp/printmate-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "printmate-1.3.1.tar", last modified: Wed May 22 20:50:33 2024, max compression
+gzip compressed data, was "printmate-1.3.3.tar", last modified: Thu May 23 21:33:07 2024, max compression
```

## Comparing `printmate-1.3.1.tar` & `printmate-1.3.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 20:50:33.475888 printmate-1.3.1/
--rw-rw-rw-   0        0        0      308 2024-05-22 20:50:33.471368 printmate-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1103 2024-05-15 21:05:01.000000 printmate-1.3.1/license
-drwxrwxrwx   0        0        0        0 2024-05-22 20:50:33.471368 printmate-1.3.1/printmate.egg-info/
--rw-rw-rw-   0        0        0      308 2024-05-22 20:50:33.000000 printmate-1.3.1/printmate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2024-05-22 20:50:33.000000 printmate-1.3.1/printmate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 20:50:33.000000 printmate-1.3.1/printmate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-22 20:50:33.000000 printmate-1.3.1/printmate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-22 20:50:33.000000 printmate-1.3.1/printmate.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 20:50:33.000000 printmate-1.3.1/printmate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 20:50:33.475888 printmate-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      536 2024-05-22 20:50:21.000000 printmate-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:33:07.335690 printmate-1.3.3/
+-rw-rw-rw-   0        0        0      819 2024-05-23 21:33:07.332197 printmate-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2024-05-23 21:30:50.000000 printmate-1.3.3/README.md
+-rw-rw-rw-   0        0        0     1103 2024-05-15 21:05:01.000000 printmate-1.3.3/license
+drwxrwxrwx   0        0        0        0 2024-05-23 21:33:07.328184 printmate-1.3.3/printmate.egg-info/
+-rw-rw-rw-   0        0        0      819 2024-05-23 21:33:06.000000 printmate-1.3.3/printmate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-23 21:33:07.000000 printmate-1.3.3/printmate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 21:33:06.000000 printmate-1.3.3/printmate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-23 21:33:06.000000 printmate-1.3.3/printmate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 21:33:06.000000 printmate-1.3.3/printmate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 21:33:07.335690 printmate-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      760 2024-05-23 21:32:52.000000 printmate-1.3.3/setup.py
```

### Comparing `printmate-1.3.1/license` & `printmate-1.3.3/license`

 * *Files identical despite different names*

