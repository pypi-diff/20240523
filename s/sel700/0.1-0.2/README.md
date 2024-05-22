# Comparing `tmp/sel700-0.1.tar.gz` & `tmp/sel700-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sel700-0.1.tar", last modified: Wed May 22 21:00:15 2024, max compression
+gzip compressed data, was "sel700-0.2.tar", last modified: Wed May 22 21:51:02 2024, max compression
```

## Comparing `sel700-0.1.tar` & `sel700-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 21:00:15.800740 sel700-0.1/
--rw-rw-rw-   0        0        0     1093 2024-05-22 16:54:30.000000 sel700-0.1/LICENCE
--rw-rw-rw-   0        0        0      327 2024-05-22 21:00:15.793278 sel700-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-22 21:00:15.750919 sel700-0.1/sel700/
--rw-rw-rw-   0        0        0     7405 2024-05-22 20:41:57.000000 sel700-0.1/sel700/sel700.py
-drwxrwxrwx   0        0        0        0 2024-05-22 21:00:15.789364 sel700-0.1/sel700.egg-info/
--rw-rw-rw-   0        0        0      327 2024-05-22 21:00:15.000000 sel700-0.1/sel700.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      153 2024-05-22 21:00:15.000000 sel700-0.1/sel700.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 21:00:15.000000 sel700-0.1/sel700.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-22 21:00:15.000000 sel700-0.1/sel700.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 21:00:15.801411 sel700-0.1/setup.cfg
--rw-rw-rw-   0        0        0      417 2024-05-22 21:00:03.000000 sel700-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:51:02.202828 sel700-0.2/
+-rw-rw-rw-   0        0        0     1093 2024-05-22 16:54:30.000000 sel700-0.2/LICENCE
+-rw-rw-rw-   0        0        0      327 2024-05-22 21:51:02.197851 sel700-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 21:51:02.170568 sel700-0.2/sel700/
+-rw-rw-rw-   0        0        0     7405 2024-05-22 20:41:57.000000 sel700-0.2/sel700/sel700.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:51:02.192854 sel700-0.2/sel700.egg-info/
+-rw-rw-rw-   0        0        0      327 2024-05-22 21:51:02.000000 sel700-0.2/sel700.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      153 2024-05-22 21:51:02.000000 sel700-0.2/sel700.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 21:51:02.000000 sel700-0.2/sel700.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-22 21:51:02.000000 sel700-0.2/sel700.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 21:51:02.202828 sel700-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      417 2024-05-22 21:46:46.000000 sel700-0.2/setup.py
```

### Comparing `sel700-0.1/LICENCE` & `sel700-0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `sel700-0.1/sel700/sel700.py` & `sel700-0.2/sel700/sel700.py`

 * *Files identical despite different names*

