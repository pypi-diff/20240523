# Comparing `tmp/renone-0.5.4.tar.gz` & `tmp/renone-0.5.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renone-0.5.4.tar", last modified: Wed May 15 21:16:05 2024, max compression
+gzip compressed data, was "renone-0.5.6.1.tar", last modified: Thu May 23 21:10:40 2024, max compression
```

## Comparing `renone-0.5.4.tar` & `renone-0.5.6.1.tar`

### file list

```diff
@@ -1,12 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 21:16:05.194557 renone-0.5.4/
--rw-rw-rw-   0        0        0      304 2024-05-15 21:16:05.175918 renone-0.5.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-15 21:16:05.162374 renone-0.5.4/Renone.egg-info/
--rw-rw-rw-   0        0        0      304 2024-05-15 21:16:04.000000 renone-0.5.4/Renone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2024-05-15 21:16:04.000000 renone-0.5.4/Renone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 21:16:04.000000 renone-0.5.4/Renone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-15 21:16:04.000000 renone-0.5.4/Renone.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2024-05-15 21:16:04.000000 renone-0.5.4/Renone.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 21:16:04.000000 renone-0.5.4/Renone.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1103 2024-05-15 21:05:29.000000 renone-0.5.4/license
--rw-rw-rw-   0        0        0       42 2024-05-15 21:16:05.194557 renone-0.5.4/setup.cfg
--rw-rw-rw-   0        0        0      537 2024-05-15 21:14:11.000000 renone-0.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:10:40.494354 renone-0.5.6.1/
+-rw-rw-rw-   0        0        0      259 2024-05-23 21:10:40.491822 renone-0.5.6.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 21:10:40.487825 renone-0.5.6.1/Renone.egg-info/
+-rw-rw-rw-   0        0        0      259 2024-05-23 21:10:40.000000 renone-0.5.6.1/Renone.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2024-05-23 21:10:40.000000 renone-0.5.6.1/Renone.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 21:10:40.000000 renone-0.5.6.1/Renone.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-23 21:10:40.000000 renone-0.5.6.1/Renone.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 21:10:40.000000 renone-0.5.6.1/Renone.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 21:10:40.495369 renone-0.5.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      511 2024-05-23 21:10:26.000000 renone-0.5.6.1/setup.py
```

