# Comparing `tmp/pyerualjetwork-1.0.8.tar.gz` & `tmp/pyerualjetwork-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.0.8.tar", last modified: Wed May 22 23:01:59 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.0.9.tar", last modified: Wed May 22 23:28:06 2024, max compression
```

## Comparing `pyerualjetwork-1.0.8.tar` & `pyerualjetwork-1.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 23:01:59.295580 pyerualjetwork-1.0.8/
--rw-rw-rw-   0        0        0      276 2024-05-22 23:01:59.295580 pyerualjetwork-1.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-22 23:01:59.270975 pyerualjetwork-1.0.8/pyerualjetwork/
--rw-rw-rw-   0        0        0       21 2024-05-22 23:01:30.000000 pyerualjetwork-1.0.8/pyerualjetwork/__init__.py
--rw-rw-rw-   0        0        0    40243 2024-05-22 22:36:00.000000 pyerualjetwork-1.0.8/pyerualjetwork/pyerualjetwork.py
-drwxrwxrwx   0        0        0        0 2024-05-22 23:01:59.295580 pyerualjetwork-1.0.8/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      276 2024-05-22 23:01:58.000000 pyerualjetwork-1.0.8/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-05-22 23:01:59.000000 pyerualjetwork-1.0.8/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 23:01:58.000000 pyerualjetwork-1.0.8/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-22 23:01:58.000000 pyerualjetwork-1.0.8/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 23:01:59.295580 pyerualjetwork-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      452 2024-05-22 23:01:49.000000 pyerualjetwork-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 23:28:06.798565 pyerualjetwork-1.0.9/
+-rw-rw-rw-   0        0        0      276 2024-05-22 23:28:06.798565 pyerualjetwork-1.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 23:28:06.782920 pyerualjetwork-1.0.9/pyerualjetwork/
+-rw-rw-rw-   0        0        0      632 2024-05-22 23:27:13.000000 pyerualjetwork-1.0.9/pyerualjetwork/__init__.py
+-rw-rw-rw-   0        0        0    40243 2024-05-22 22:36:00.000000 pyerualjetwork-1.0.9/pyerualjetwork/pyerualjetwork.py
+drwxrwxrwx   0        0        0        0 2024-05-22 23:28:06.798565 pyerualjetwork-1.0.9/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      276 2024-05-22 23:28:06.000000 pyerualjetwork-1.0.9/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-05-22 23:28:06.000000 pyerualjetwork-1.0.9/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 23:28:06.000000 pyerualjetwork-1.0.9/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-22 23:28:06.000000 pyerualjetwork-1.0.9/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 23:28:06.798565 pyerualjetwork-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      452 2024-05-22 23:27:47.000000 pyerualjetwork-1.0.9/setup.py
```

### Comparing `pyerualjetwork-1.0.8/pyerualjetwork/pyerualjetwork.py` & `pyerualjetwork-1.0.9/pyerualjetwork/pyerualjetwork.py`

 * *Files identical despite different names*
