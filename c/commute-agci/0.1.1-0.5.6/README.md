# Comparing `tmp/commute_agci-0.1.1.tar.gz` & `tmp/commute_agci-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commute_agci-0.1.1.tar", last modified: Thu May 23 04:05:01 2024, max compression
+gzip compressed data, was "commute_agci-0.5.6.tar", last modified: Thu May 23 04:18:45 2024, max compression
```

## Comparing `commute_agci-0.1.1.tar` & `commute_agci-0.5.6.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 kishimotosakaiyasushi   (501) staff       (20)        0 2024-05-23 04:05:01.637345 commute_agci-0.1.1/
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)      146 2024-05-23 04:05:01.637134 commute_agci-0.1.1/PKG-INFO
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       61 2024-05-23 03:55:15.000000 commute_agci-0.1.1/README.md
-drwxr-xr-x   0 kishimotosakaiyasushi   (501) staff       (20)        0 2024-05-23 04:05:01.635978 commute_agci-0.1.1/commute_agci/
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       40 2024-05-23 04:04:02.000000 commute_agci-0.1.1/commute_agci/__init__.py
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     1458 2024-05-23 04:02:05.000000 commute_agci-0.1.1/commute_agci/commute_agci.py
-drwxr-xr-x   0 kishimotosakaiyasushi   (501) staff       (20)        0 2024-05-23 04:05:01.636874 commute_agci-0.1.1/commute_agci.egg-info/
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)      146 2024-05-23 04:05:01.000000 commute_agci-0.1.1/commute_agci.egg-info/PKG-INFO
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)      290 2024-05-23 04:05:01.000000 commute_agci-0.1.1/commute_agci.egg-info/SOURCES.txt
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)        1 2024-05-23 04:05:01.000000 commute_agci-0.1.1/commute_agci.egg-info/dependency_links.txt
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       35 2024-05-23 04:05:01.000000 commute_agci-0.1.1/commute_agci.egg-info/entry_points.txt
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       30 2024-05-23 04:05:01.000000 commute_agci-0.1.1/commute_agci.egg-info/requires.txt
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       13 2024-05-23 04:05:01.000000 commute_agci-0.1.1/commute_agci.egg-info/top_level.txt
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       38 2024-05-23 04:05:01.637389 commute_agci-0.1.1/setup.cfg
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)      346 2024-05-23 04:01:01.000000 commute_agci-0.1.1/setup.py
+drwxr-xr-x   0 kishimotosakaiyasushi   (501) staff       (20)        0 2024-05-23 04:18:45.659565 commute_agci-0.5.6/
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     5456 2024-05-23 04:18:45.659364 commute_agci-0.5.6/PKG-INFO
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     4758 2024-05-23 04:09:34.000000 commute_agci-0.5.6/README.md
+drwxr-xr-x   0 kishimotosakaiyasushi   (501) staff       (20)        0 2024-05-23 04:18:45.658256 commute_agci-0.5.6/commute_agci/
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       69 2024-05-23 04:15:20.000000 commute_agci-0.5.6/commute_agci/__init__.py
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     1458 2024-05-23 04:02:05.000000 commute_agci-0.5.6/commute_agci/commute_agci.py
+drwxr-xr-x   0 kishimotosakaiyasushi   (501) staff       (20)        0 2024-05-23 04:18:45.659082 commute_agci-0.5.6/commute_agci.egg-info/
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     5456 2024-05-23 04:18:45.000000 commute_agci-0.5.6/commute_agci.egg-info/PKG-INFO
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)      251 2024-05-23 04:18:45.000000 commute_agci-0.5.6/commute_agci.egg-info/SOURCES.txt
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)        1 2024-05-23 04:18:45.000000 commute_agci-0.5.6/commute_agci.egg-info/dependency_links.txt
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       30 2024-05-23 04:18:45.000000 commute_agci-0.5.6/commute_agci.egg-info/requires.txt
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       13 2024-05-23 04:18:45.000000 commute_agci-0.5.6/commute_agci.egg-info/top_level.txt
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       38 2024-05-23 04:18:45.659602 commute_agci-0.5.6/setup.cfg
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     1626 2024-05-23 04:18:18.000000 commute_agci-0.5.6/setup.py
```

### Comparing `commute_agci-0.1.1/commute_agci/commute_agci.py` & `commute_agci-0.5.6/commute_agci/commute_agci.py`

 * *Files identical despite different names*

