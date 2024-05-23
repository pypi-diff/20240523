# Comparing `tmp/Complex_Bidintha-0.1.tar.gz` & `tmp/Complex_Bidintha-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Complex_Bidintha-0.1.tar", last modified: Thu May 23 09:11:00 2024, max compression
+gzip compressed data, was "Complex_Bidintha-0.2.tar", last modified: Thu May 23 09:24:56 2024, max compression
```

## Comparing `Complex_Bidintha-0.1.tar` & `Complex_Bidintha-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 09:11:00.771456 Complex_Bidintha-0.1/
-drwxrwxrwx   0        0        0        0 2024-05-23 09:11:00.747050 Complex_Bidintha-0.1/Complex/
--rw-rw-rw-   0        0        0     1727 2024-05-23 08:41:16.000000 Complex_Bidintha-0.1/Complex/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 09:11:00.760432 Complex_Bidintha-0.1/Complex_Bidintha.egg-info/
--rw-rw-rw-   0        0        0      179 2024-05-23 09:11:00.000000 Complex_Bidintha-0.1/Complex_Bidintha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-05-23 09:11:00.000000 Complex_Bidintha-0.1/Complex_Bidintha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 09:11:00.000000 Complex_Bidintha-0.1/Complex_Bidintha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-23 09:11:00.000000 Complex_Bidintha-0.1/Complex_Bidintha.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-05-23 08:08:20.000000 Complex_Bidintha-0.1/License.txt
--rw-rw-rw-   0        0        0      179 2024-05-23 09:11:00.771456 Complex_Bidintha-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-23 08:08:09.000000 Complex_Bidintha-0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 09:11:00.771456 Complex_Bidintha-0.1/setup.cfg
--rw-rw-rw-   0        0        0      250 2024-05-23 09:10:23.000000 Complex_Bidintha-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:24:56.102589 Complex_Bidintha-0.2/
+drwxrwxrwx   0        0        0        0 2024-05-23 09:24:56.093032 Complex_Bidintha-0.2/Complex/
+-rw-rw-rw-   0        0        0     1727 2024-05-23 08:41:16.000000 Complex_Bidintha-0.2/Complex/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:24:56.102589 Complex_Bidintha-0.2/Complex_Bidintha.egg-info/
+-rw-rw-rw-   0        0        0      880 2024-05-23 09:24:55.000000 Complex_Bidintha-0.2/Complex_Bidintha.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-05-23 09:24:56.000000 Complex_Bidintha-0.2/Complex_Bidintha.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 09:24:55.000000 Complex_Bidintha-0.2/Complex_Bidintha.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-23 09:24:55.000000 Complex_Bidintha-0.2/Complex_Bidintha.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-05-23 08:08:20.000000 Complex_Bidintha-0.2/License.txt
+-rw-rw-rw-   0        0        0      880 2024-05-23 09:24:56.102589 Complex_Bidintha-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-23 08:08:09.000000 Complex_Bidintha-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 09:24:56.102589 Complex_Bidintha-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      977 2024-05-23 09:20:44.000000 Complex_Bidintha-0.2/setup.py
```

### Comparing `Complex_Bidintha-0.1/Complex/__init__.py` & `Complex_Bidintha-0.2/Complex/__init__.py`

 * *Files identical despite different names*

