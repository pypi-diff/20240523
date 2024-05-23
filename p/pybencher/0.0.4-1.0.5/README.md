# Comparing `tmp/pybencher-0.0.4.tar.gz` & `tmp/pybencher-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybencher-0.0.4.tar", last modified: Thu Jan 25 10:11:43 2024, max compression
+gzip compressed data, was "pybencher-1.0.5.tar", last modified: Thu May 23 17:40:22 2024, max compression
```

## Comparing `pybencher-0.0.4.tar` & `pybencher-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-01-25 10:11:43.730491 pybencher-0.0.4/
--rw-rw-rw-   0        0        0     1089 2024-01-25 09:33:50.000000 pybencher-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3673 2024-01-25 10:11:43.727490 pybencher-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2992 2024-01-25 09:33:50.000000 pybencher-0.0.4/README.md
--rw-rw-rw-   0        0        0      736 2024-01-25 10:11:03.000000 pybencher-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-25 10:11:43.730491 pybencher-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-25 10:11:43.693482 pybencher-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-01-25 10:11:43.726490 pybencher-0.0.4/src/pybencher.egg-info/
--rw-rw-rw-   0        0        0     3673 2024-01-25 10:11:43.000000 pybencher-0.0.4/src/pybencher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-01-25 10:11:43.000000 pybencher-0.0.4/src/pybencher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-25 10:11:43.000000 pybencher-0.0.4/src/pybencher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-01-25 10:11:43.000000 pybencher-0.0.4/src/pybencher.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5998 2024-01-25 09:59:34.000000 pybencher-0.0.4/src/pybencher.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:40:22.264593 pybencher-1.0.5/
+-rw-rw-rw-   0        0        0     1089 2024-01-25 09:33:50.000000 pybencher-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     6629 2024-05-23 17:40:22.260592 pybencher-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5946 2024-05-23 17:40:00.000000 pybencher-1.0.5/README.md
+-rw-rw-rw-   0        0        0      736 2024-05-23 17:36:16.000000 pybencher-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 17:40:22.265595 pybencher-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 17:40:22.228585 pybencher-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 17:40:22.258592 pybencher-1.0.5/src/pybencher.egg-info/
+-rw-rw-rw-   0        0        0     6629 2024-05-23 17:40:22.000000 pybencher-1.0.5/src/pybencher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-05-23 17:40:22.000000 pybencher-1.0.5/src/pybencher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 17:40:22.000000 pybencher-1.0.5/src/pybencher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 17:40:22.000000 pybencher-1.0.5/src/pybencher.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8649 2024-05-23 14:23:25.000000 pybencher-1.0.5/src/pybencher.py
```

### Comparing `pybencher-0.0.4/LICENSE` & `pybencher-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pybencher-0.0.4/pyproject.toml` & `pybencher-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pybencher"
-version = "0.0.4"
+version = "1.0.5"
 authors = [
   { name="Barnaby Gill", email="barnabasgill@gmail.com" },
 ]
 description = "PyBencher is a Python benchmarking module for benchmarking several python functions at once. PyBencher supports tuneable benchmarking parameters as well as args and kwargs for function calls."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

