# Comparing `tmp/AAIT25-0.0.8.tar.gz` & `tmp/AAIT25-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AAIT25-0.0.8.tar", last modified: Thu May 23 18:13:32 2024, max compression
+gzip compressed data, was "AAIT25-0.0.9.tar", last modified: Thu May 23 18:27:20 2024, max compression
```

## Comparing `AAIT25-0.0.8.tar` & `AAIT25-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 18:13:32.512547 AAIT25-0.0.8/
-drwxrwxrwx   0        0        0        0 2024-05-23 18:13:32.510547 AAIT25-0.0.8/AAIT25.egg-info/
--rw-rw-rw-   0        0        0      347 2024-05-23 18:13:32.000000 AAIT25-0.0.8/AAIT25.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-05-23 18:13:32.000000 AAIT25-0.0.8/AAIT25.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 18:13:32.000000 AAIT25-0.0.8/AAIT25.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-23 18:13:32.000000 AAIT25-0.0.8/AAIT25.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 18:13:32.000000 AAIT25-0.0.8/AAIT25.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0       29 2024-05-23 18:13:32.000000 AAIT25-0.0.8/AAIT25.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 18:13:32.000000 AAIT25-0.0.8/AAIT25.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.8/License.txt
--rw-rw-rw-   0        0        0      347 2024-05-23 18:13:32.511547 AAIT25-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 18:13:32.511547 AAIT25-0.0.8/orangecontrib/
--rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT25-0.0.8/orangecontrib/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-23 18:13:32.512547 AAIT25-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1782 2024-05-23 18:13:25.000000 AAIT25-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:27:20.171788 AAIT25-0.0.9/
+drwxrwxrwx   0        0        0        0 2024-05-23 18:27:20.169783 AAIT25-0.0.9/AAIT25.egg-info/
+-rw-rw-rw-   0        0        0      347 2024-05-23 18:27:20.000000 AAIT25-0.0.9/AAIT25.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-05-23 18:27:20.000000 AAIT25-0.0.9/AAIT25.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 18:27:20.000000 AAIT25-0.0.9/AAIT25.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-23 18:27:20.000000 AAIT25-0.0.9/AAIT25.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 18:27:20.000000 AAIT25-0.0.9/AAIT25.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0       29 2024-05-23 18:27:20.000000 AAIT25-0.0.9/AAIT25.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 18:27:20.000000 AAIT25-0.0.9/AAIT25.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.9/License.txt
+-rw-rw-rw-   0        0        0      347 2024-05-23 18:27:20.170786 AAIT25-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 18:27:20.169783 AAIT25-0.0.9/orangecontrib/
+-rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT25-0.0.9/orangecontrib/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 18:27:20.171788 AAIT25-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1782 2024-05-23 18:27:11.000000 AAIT25-0.0.9/setup.py
```

### Comparing `AAIT25-0.0.8/setup.py` & `AAIT25-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Nom du package PyPI
 NAME = "AAIT25"
 
 # Version du package PyPI
-VERSION = "0.0.8"  # la version doit être supérieure à la précédente sinon la publication sera refusée
+VERSION = "0.0.9"  # la version doit être supérieure à la précédente sinon la publication sera refusée
 
 # Facultatif / Adaptable à souhait
 AUTHOR = "Orange community"
 AUTHOR_EMAIL = ""
 URL = ""
 DESCRIPTION = ("Advanced Artificial Intelligence Tools is a package meant to develop "
                "and enable advanced AI functionalities in Orange Data Mining.")
```

