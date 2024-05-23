# Comparing `tmp/AgainsTurbcnModel-0.1.tar.gz` & `tmp/AgainsTurbcnModel-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AgainsTurbcnModel-0.1.tar", last modified: Wed May 22 23:54:48 2024, max compression
+gzip compressed data, was "AgainsTurbcnModel-0.1.1.tar", last modified: Thu May 23 00:15:19 2024, max compression
```

## Comparing `AgainsTurbcnModel-0.1.tar` & `AgainsTurbcnModel-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 23:54:48.065038 AgainsTurbcnModel-0.1/
-drwxrwxrwx   0        0        0        0 2024-05-22 23:54:48.062038 AgainsTurbcnModel-0.1/AgainsTurbcnModel/
--rw-rw-rw-   0        0        0      105 2024-05-22 23:36:41.000000 AgainsTurbcnModel-0.1/AgainsTurbcnModel/__init__.py
--rw-rw-rw-   0        0        0    13075 2024-05-22 23:51:19.000000 AgainsTurbcnModel-0.1/AgainsTurbcnModel/main.py
-drwxrwxrwx   0        0        0        0 2024-05-22 23:54:48.064038 AgainsTurbcnModel-0.1/AgainsTurbcnModel.egg-info/
--rw-rw-rw-   0        0        0      120 2024-05-22 23:54:47.000000 AgainsTurbcnModel-0.1/AgainsTurbcnModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2024-05-22 23:54:48.000000 AgainsTurbcnModel-0.1/AgainsTurbcnModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 23:54:47.000000 AgainsTurbcnModel-0.1/AgainsTurbcnModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-22 23:54:47.000000 AgainsTurbcnModel-0.1/AgainsTurbcnModel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      120 2024-05-22 23:54:48.065038 AgainsTurbcnModel-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-22 23:54:48.065038 AgainsTurbcnModel-0.1/setup.cfg
--rw-rw-rw-   0        0        0      205 2024-05-22 23:54:37.000000 AgainsTurbcnModel-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 00:15:19.095463 AgainsTurbcnModel-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-05-23 00:15:19.092963 AgainsTurbcnModel-0.1.1/AgainsTurbcnModel/
+-rw-rw-rw-   0        0        0      143 2024-05-23 00:12:03.000000 AgainsTurbcnModel-0.1.1/AgainsTurbcnModel/__init__.py
+-rw-rw-rw-   0        0        0    13075 2024-05-22 23:51:19.000000 AgainsTurbcnModel-0.1.1/AgainsTurbcnModel/main.py
+drwxrwxrwx   0        0        0        0 2024-05-23 00:15:19.094962 AgainsTurbcnModel-0.1.1/AgainsTurbcnModel.egg-info/
+-rw-rw-rw-   0        0        0      122 2024-05-23 00:15:19.000000 AgainsTurbcnModel-0.1.1/AgainsTurbcnModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2024-05-23 00:15:19.000000 AgainsTurbcnModel-0.1.1/AgainsTurbcnModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 00:15:19.000000 AgainsTurbcnModel-0.1.1/AgainsTurbcnModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-23 00:15:19.000000 AgainsTurbcnModel-0.1.1/AgainsTurbcnModel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      122 2024-05-23 00:15:19.095463 AgainsTurbcnModel-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-23 00:15:19.095963 AgainsTurbcnModel-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      207 2024-05-23 00:15:12.000000 AgainsTurbcnModel-0.1.1/setup.py
```

### Comparing `AgainsTurbcnModel-0.1/AgainsTurbcnModel/main.py` & `AgainsTurbcnModel-0.1.1/AgainsTurbcnModel/main.py`

 * *Files identical despite different names*

