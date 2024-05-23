# Comparing `tmp/halina_mypackage-0.0.1.tar.gz` & `tmp/halina_mypackage-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halina_mypackage-0.0.1.tar", last modified: Wed May 22 05:24:06 2024, max compression
+gzip compressed data, was "halina_mypackage-0.0.2.tar", last modified: Wed May 22 05:35:03 2024, max compression
```

## Comparing `halina_mypackage-0.0.1.tar` & `halina_mypackage-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 prashantsood   (501) staff       (20)        0 2024-05-22 05:24:06.261930 halina_mypackage-0.0.1/
--rw-r--r--   0 prashantsood   (501) staff       (20)      189 2024-05-22 05:24:06.261707 halina_mypackage-0.0.1/PKG-INFO
-drwxr-xr-x   0 prashantsood   (501) staff       (20)        0 2024-05-22 05:24:06.260630 halina_mypackage-0.0.1/halina_mypackage/
--rw-r--r--   0 prashantsood   (501) staff       (20)       26 2024-05-22 04:38:48.000000 halina_mypackage-0.0.1/halina_mypackage/__init__.py
--rw-r--r--   0 prashantsood   (501) staff       (20)      104 2024-05-22 04:57:43.000000 halina_mypackage-0.0.1/halina_mypackage/calculator.py
-drwxr-xr-x   0 prashantsood   (501) staff       (20)        0 2024-05-22 05:24:06.261416 halina_mypackage-0.0.1/halina_mypackage.egg-info/
--rw-r--r--   0 prashantsood   (501) staff       (20)      189 2024-05-22 05:24:06.000000 halina_mypackage-0.0.1/halina_mypackage.egg-info/PKG-INFO
--rw-r--r--   0 prashantsood   (501) staff       (20)      228 2024-05-22 05:24:06.000000 halina_mypackage-0.0.1/halina_mypackage.egg-info/SOURCES.txt
--rw-r--r--   0 prashantsood   (501) staff       (20)        1 2024-05-22 05:24:06.000000 halina_mypackage-0.0.1/halina_mypackage.egg-info/dependency_links.txt
--rw-r--r--   0 prashantsood   (501) staff       (20)       17 2024-05-22 05:24:06.000000 halina_mypackage-0.0.1/halina_mypackage.egg-info/top_level.txt
--rw-r--r--   0 prashantsood   (501) staff       (20)       38 2024-05-22 05:24:06.262023 halina_mypackage-0.0.1/setup.cfg
--rw-r--r--   0 prashantsood   (501) staff       (20)      203 2024-05-22 05:23:06.000000 halina_mypackage-0.0.1/setup.py
+drwxr-xr-x   0 prashantsood   (501) staff       (20)        0 2024-05-22 05:35:03.538693 halina_mypackage-0.0.2/
+-rw-r--r--   0 prashantsood   (501) staff       (20)      189 2024-05-22 05:35:03.538457 halina_mypackage-0.0.2/PKG-INFO
+drwxr-xr-x   0 prashantsood   (501) staff       (20)        0 2024-05-22 05:35:03.537361 halina_mypackage-0.0.2/halina_mypackage/
+-rw-r--r--   0 prashantsood   (501) staff       (20)       26 2024-05-22 04:38:48.000000 halina_mypackage-0.0.2/halina_mypackage/__init__.py
+-rw-r--r--   0 prashantsood   (501) staff       (20)      138 2024-05-22 05:34:35.000000 halina_mypackage-0.0.2/halina_mypackage/calculator.py
+drwxr-xr-x   0 prashantsood   (501) staff       (20)        0 2024-05-22 05:35:03.538155 halina_mypackage-0.0.2/halina_mypackage.egg-info/
+-rw-r--r--   0 prashantsood   (501) staff       (20)      189 2024-05-22 05:35:03.000000 halina_mypackage-0.0.2/halina_mypackage.egg-info/PKG-INFO
+-rw-r--r--   0 prashantsood   (501) staff       (20)      228 2024-05-22 05:35:03.000000 halina_mypackage-0.0.2/halina_mypackage.egg-info/SOURCES.txt
+-rw-r--r--   0 prashantsood   (501) staff       (20)        1 2024-05-22 05:35:03.000000 halina_mypackage-0.0.2/halina_mypackage.egg-info/dependency_links.txt
+-rw-r--r--   0 prashantsood   (501) staff       (20)       17 2024-05-22 05:35:03.000000 halina_mypackage-0.0.2/halina_mypackage.egg-info/top_level.txt
+-rw-r--r--   0 prashantsood   (501) staff       (20)       38 2024-05-22 05:35:03.538774 halina_mypackage-0.0.2/setup.cfg
+-rw-r--r--   0 prashantsood   (501) staff       (20)      203 2024-05-22 05:34:30.000000 halina_mypackage-0.0.2/setup.py
```

