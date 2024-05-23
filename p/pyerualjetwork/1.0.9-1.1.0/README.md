# Comparing `tmp/pyerualjetwork-1.0.9.tar.gz` & `tmp/pyerualjetwork-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.0.9.tar", last modified: Wed May 22 23:28:06 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.1.0.tar", last modified: Wed May 22 23:52:46 2024, max compression
```

## Comparing `pyerualjetwork-1.0.9.tar` & `pyerualjetwork-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 23:28:06.798565 pyerualjetwork-1.0.9/
--rw-rw-rw-   0        0        0      276 2024-05-22 23:28:06.798565 pyerualjetwork-1.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-22 23:28:06.782920 pyerualjetwork-1.0.9/pyerualjetwork/
--rw-rw-rw-   0        0        0      632 2024-05-22 23:27:13.000000 pyerualjetwork-1.0.9/pyerualjetwork/__init__.py
--rw-rw-rw-   0        0        0    40243 2024-05-22 22:36:00.000000 pyerualjetwork-1.0.9/pyerualjetwork/pyerualjetwork.py
-drwxrwxrwx   0        0        0        0 2024-05-22 23:28:06.798565 pyerualjetwork-1.0.9/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      276 2024-05-22 23:28:06.000000 pyerualjetwork-1.0.9/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-05-22 23:28:06.000000 pyerualjetwork-1.0.9/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 23:28:06.000000 pyerualjetwork-1.0.9/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-22 23:28:06.000000 pyerualjetwork-1.0.9/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 23:28:06.798565 pyerualjetwork-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      452 2024-05-22 23:27:47.000000 pyerualjetwork-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 23:52:46.890574 pyerualjetwork-1.1.0/
+-rw-rw-rw-   0        0        0      276 2024-05-22 23:52:46.890574 pyerualjetwork-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 23:52:46.859335 pyerualjetwork-1.1.0/pyerualjetwork/
+-rw-rw-rw-   0        0        0      213 2024-05-22 23:52:08.000000 pyerualjetwork-1.1.0/pyerualjetwork/__init__.py
+-rw-rw-rw-   0        0        0    40243 2024-05-22 22:36:00.000000 pyerualjetwork-1.1.0/pyerualjetwork/pyerualjetwork.py
+drwxrwxrwx   0        0        0        0 2024-05-22 23:52:46.874953 pyerualjetwork-1.1.0/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      276 2024-05-22 23:52:46.000000 pyerualjetwork-1.1.0/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-05-22 23:52:46.000000 pyerualjetwork-1.1.0/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 23:52:46.000000 pyerualjetwork-1.1.0/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-22 23:52:46.000000 pyerualjetwork-1.1.0/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 23:52:46.890574 pyerualjetwork-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      452 2024-05-22 23:52:38.000000 pyerualjetwork-1.1.0/setup.py
```

### Comparing `pyerualjetwork-1.0.9/pyerualjetwork/pyerualjetwork.py` & `pyerualjetwork-1.1.0/pyerualjetwork/pyerualjetwork.py`

 * *Files identical despite different names*

