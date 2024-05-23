# Comparing `tmp/plg-0.0.2.tar.gz` & `tmp/plg-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plg-0.0.2.tar", last modified: Fri Mar 15 08:17:17 2024, max compression
+gzip compressed data, was "plg-0.1.0.tar", last modified: Thu May 23 02:59:07 2024, max compression
```

## Comparing `plg-0.0.2.tar` & `plg-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,9 @@
-drwxrwxrwx   0        0        0        0 2024-03-15 08:17:17.124178 plg-0.0.2/
--rw-rw-rw-   0        0        0      259 2024-03-15 08:17:17.124178 plg-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-15 08:17:17.120176 plg-0.0.2/plg.egg-info/
--rw-rw-rw-   0        0        0      259 2024-03-15 08:17:16.000000 plg-0.0.2/plg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      153 2024-03-15 08:17:16.000000 plg-0.0.2/plg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-15 08:17:16.000000 plg-0.0.2/plg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-03-15 08:17:16.000000 plg-0.0.2/plg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-15 08:17:17.130180 plg-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      535 2024-03-15 08:15:55.000000 plg-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-15 08:17:17.123183 plg-0.0.2/src/
--rw-rw-rw-   0        0        0        0 2019-09-19 05:18:53.000000 plg-0.0.2/src/__init__.py
--rw-rw-rw-   0        0        0       40 2019-09-19 05:18:53.000000 plg-0.0.2/src/plg.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:59:07.703545 plg-0.1.0/
+-rw-rw-rw-   0        0        0      472 2024-05-23 02:59:07.702558 plg-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 02:59:07.700553 plg-0.1.0/plg.egg-info/
+-rw-rw-rw-   0        0        0      472 2024-05-23 02:59:07.000000 plg-0.1.0/plg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2024-05-23 02:59:07.000000 plg-0.1.0/plg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 02:59:07.000000 plg-0.1.0/plg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 02:59:07.000000 plg-0.1.0/plg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 02:59:07.703545 plg-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      614 2024-05-23 02:58:10.000000 plg-0.1.0/setup.py
```

