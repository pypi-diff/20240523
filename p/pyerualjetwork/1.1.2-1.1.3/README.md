# Comparing `tmp/pyerualjetwork-1.1.2.tar.gz` & `tmp/pyerualjetwork-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.1.2.tar", last modified: Thu May 23 00:10:22 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.1.3.tar", last modified: Thu May 23 00:11:47 2024, max compression
```

## Comparing `pyerualjetwork-1.1.2.tar` & `pyerualjetwork-1.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 00:10:22.286200 pyerualjetwork-1.1.2/
-drwxrwxrwx   0        0        0        0 2024-05-23 00:10:22.270193 pyerualjetwork-1.1.2/DPNN/
--rw-rw-rw-   0        0        0    40243 2024-05-22 22:36:00.000000 pyerualjetwork-1.1.2/DPNN/DPNN.py
--rw-rw-rw-   0        0        0      234 2024-05-23 00:06:25.000000 pyerualjetwork-1.1.2/DPNN/__init__.py
--rw-rw-rw-   0        0        0      276 2024-05-23 00:10:22.286200 pyerualjetwork-1.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-23 00:10:22.286200 pyerualjetwork-1.1.2/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      276 2024-05-23 00:10:21.000000 pyerualjetwork-1.1.2/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-23 00:10:22.000000 pyerualjetwork-1.1.2/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 00:10:21.000000 pyerualjetwork-1.1.2/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-23 00:10:21.000000 pyerualjetwork-1.1.2/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 00:10:22.286200 pyerualjetwork-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      452 2024-05-23 00:10:15.000000 pyerualjetwork-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 00:11:47.416992 pyerualjetwork-1.1.3/
+drwxrwxrwx   0        0        0        0 2024-05-23 00:11:47.401359 pyerualjetwork-1.1.3/DPNN/
+-rw-rw-rw-   0        0        0    40243 2024-05-22 22:36:00.000000 pyerualjetwork-1.1.3/DPNN/DPNN.py
+-rw-rw-rw-   0        0        0      203 2024-05-23 00:11:33.000000 pyerualjetwork-1.1.3/DPNN/__init__.py
+-rw-rw-rw-   0        0        0      276 2024-05-23 00:11:47.416992 pyerualjetwork-1.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 00:11:47.416992 pyerualjetwork-1.1.3/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      276 2024-05-23 00:11:47.000000 pyerualjetwork-1.1.3/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-23 00:11:47.000000 pyerualjetwork-1.1.3/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 00:11:47.000000 pyerualjetwork-1.1.3/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-23 00:11:47.000000 pyerualjetwork-1.1.3/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 00:11:47.416992 pyerualjetwork-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      452 2024-05-23 00:11:40.000000 pyerualjetwork-1.1.3/setup.py
```

### Comparing `pyerualjetwork-1.1.2/DPNN/DPNN.py` & `pyerualjetwork-1.1.3/DPNN/DPNN.py`

 * *Files identical despite different names*

