# Comparing `tmp/pyerualjetwork-1.1.4.tar.gz` & `tmp/pyerualjetwork-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.1.4.tar", last modified: Thu May 23 00:23:27 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.1.5.tar", last modified: Thu May 23 00:30:56 2024, max compression
```

## Comparing `pyerualjetwork-1.1.4.tar` & `pyerualjetwork-1.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 00:23:27.811836 pyerualjetwork-1.1.4/
-drwxrwxrwx   0        0        0        0 2024-05-23 00:23:27.796210 pyerualjetwork-1.1.4/DPNN/
--rw-rw-rw-   0        0        0    40243 2024-05-22 22:36:00.000000 pyerualjetwork-1.1.4/DPNN/DPNN.py
--rw-rw-rw-   0        0        0      691 2024-05-23 00:22:55.000000 pyerualjetwork-1.1.4/DPNN/__init__.py
--rw-rw-rw-   0        0        0      276 2024-05-23 00:23:27.796210 pyerualjetwork-1.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-23 00:23:27.796210 pyerualjetwork-1.1.4/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      276 2024-05-23 00:23:27.000000 pyerualjetwork-1.1.4/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-23 00:23:27.000000 pyerualjetwork-1.1.4/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 00:23:27.000000 pyerualjetwork-1.1.4/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-23 00:23:27.000000 pyerualjetwork-1.1.4/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 00:23:27.811836 pyerualjetwork-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      452 2024-05-23 00:23:13.000000 pyerualjetwork-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 00:30:56.736061 pyerualjetwork-1.1.5/
+-rw-rw-rw-   0        0        0      276 2024-05-23 00:30:56.736061 pyerualjetwork-1.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 00:30:56.725529 pyerualjetwork-1.1.5/plan/
+-rw-rw-rw-   0        0        0      315 2024-05-23 00:30:11.000000 pyerualjetwork-1.1.5/plan/__init__.py
+-rw-rw-rw-   0        0        0    40243 2024-05-22 22:36:00.000000 pyerualjetwork-1.1.5/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-23 00:30:56.736061 pyerualjetwork-1.1.5/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      276 2024-05-23 00:30:56.000000 pyerualjetwork-1.1.5/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-23 00:30:56.000000 pyerualjetwork-1.1.5/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 00:30:56.000000 pyerualjetwork-1.1.5/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-23 00:30:56.000000 pyerualjetwork-1.1.5/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 00:30:56.736061 pyerualjetwork-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      452 2024-05-23 00:30:49.000000 pyerualjetwork-1.1.5/setup.py
```

### Comparing `pyerualjetwork-1.1.4/DPNN/DPNN.py` & `pyerualjetwork-1.1.5/plan/plan.py`

 * *Files identical despite different names*

