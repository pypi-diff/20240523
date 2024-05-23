# Comparing `tmp/AAIT25-0.0.1.tar.gz` & `tmp/AAIT25-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AAIT25-0.0.1.tar", last modified: Thu May 23 17:45:35 2024, max compression
+gzip compressed data, was "AAIT25-0.0.2.tar", last modified: Thu May 23 17:49:04 2024, max compression
```

## Comparing `AAIT25-0.0.1.tar` & `AAIT25-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 17:45:35.595590 AAIT25-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-23 17:45:35.594598 AAIT25-0.0.1/AAIT25.egg-info/
--rw-rw-rw-   0        0        0      347 2024-05-23 17:45:35.000000 AAIT25-0.0.1/AAIT25.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-05-23 17:45:35.000000 AAIT25-0.0.1/AAIT25.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 17:45:35.000000 AAIT25-0.0.1/AAIT25.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-23 17:45:35.000000 AAIT25-0.0.1/AAIT25.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 17:45:35.000000 AAIT25-0.0.1/AAIT25.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0       29 2024-05-23 17:45:35.000000 AAIT25-0.0.1/AAIT25.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 17:45:35.000000 AAIT25-0.0.1/AAIT25.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.1/License.txt
--rw-rw-rw-   0        0        0      347 2024-05-23 17:45:35.595590 AAIT25-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 17:45:35.594598 AAIT25-0.0.1/orangecontrib/
--rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT25-0.0.1/orangecontrib/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-23 17:45:35.595590 AAIT25-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1980 2024-05-23 17:45:17.000000 AAIT25-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:49:04.244297 AAIT25-0.0.2/
+drwxrwxrwx   0        0        0        0 2024-05-23 17:49:04.242298 AAIT25-0.0.2/AAIT25.egg-info/
+-rw-rw-rw-   0        0        0      347 2024-05-23 17:49:04.000000 AAIT25-0.0.2/AAIT25.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-05-23 17:49:04.000000 AAIT25-0.0.2/AAIT25.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 17:49:04.000000 AAIT25-0.0.2/AAIT25.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-23 17:49:04.000000 AAIT25-0.0.2/AAIT25.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 17:49:04.000000 AAIT25-0.0.2/AAIT25.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0       29 2024-05-23 17:49:04.000000 AAIT25-0.0.2/AAIT25.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 17:49:04.000000 AAIT25-0.0.2/AAIT25.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.2/License.txt
+-rw-rw-rw-   0        0        0      347 2024-05-23 17:49:04.243298 AAIT25-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 17:49:04.243298 AAIT25-0.0.2/orangecontrib/
+-rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT25-0.0.2/orangecontrib/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 17:49:04.244297 AAIT25-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1980 2024-05-23 17:48:56.000000 AAIT25-0.0.2/setup.py
```

### Comparing `AAIT25-0.0.1/setup.py` & `AAIT25-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 # Nom du package PyPI
 NAME = "AAIT25"
 
 # Version du package PyPI
-VERSION = "0.0.1"  # la version doit être supérieure à la précédente sinon la publication sera refusée
+VERSION = "0.0.2"  # la version doit être supérieure à la précédente sinon la publication sera refusée
 
 # Facultatif / Adaptable à souhait
 AUTHOR = "Orange community"
 AUTHOR_EMAIL = ""
 URL = ""
 DESCRIPTION = ("Advanced Artificial Intelligence Tools is a package meant to develop "
                "and enable advanced AI functionalities in Orange Data Mining.")
```

