# Comparing `tmp/pyerualjetwork-1.0.4.tar.gz` & `tmp/pyerualjetwork-1.0.5.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.0.4.tar", last modified: Wed May 22 20:05:40 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.0.5.post0.tar", last modified: Wed May 22 22:21:32 2024, max compression
```

## Comparing `pyerualjetwork-1.0.4.tar` & `pyerualjetwork-1.0.5.post0.tar`

### file list

```diff
@@ -1,12 +1,9 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 20:05:40.029028 pyerualjetwork-1.0.4/
-drwxrwxrwx   0        0        0        0 2024-05-22 20:05:40.008742 pyerualjetwork-1.0.4/DPNN/
--rw-rw-rw-   0        0        0    40242 2024-05-22 19:58:55.000000 pyerualjetwork-1.0.4/DPNN/DPNN.py
--rw-rw-rw-   0        0        0      765 2024-05-22 19:21:22.000000 pyerualjetwork-1.0.4/DPNN/__init__.py
--rw-rw-rw-   0        0        0      276 2024-05-22 20:05:40.025004 pyerualjetwork-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-22 20:05:40.025004 pyerualjetwork-1.0.4/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      276 2024-05-22 20:05:39.000000 pyerualjetwork-1.0.4/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-22 20:05:39.000000 pyerualjetwork-1.0.4/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 20:05:39.000000 pyerualjetwork-1.0.4/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-22 20:05:39.000000 pyerualjetwork-1.0.4/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 20:05:40.084936 pyerualjetwork-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      452 2024-05-22 20:05:22.000000 pyerualjetwork-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:21:31.991065 pyerualjetwork-1.0.5.post0/
+-rw-rw-rw-   0        0        0      282 2024-05-22 22:21:31.991065 pyerualjetwork-1.0.5.post0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 22:21:31.991065 pyerualjetwork-1.0.5.post0/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      282 2024-05-22 22:21:31.000000 pyerualjetwork-1.0.5.post0/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      160 2024-05-22 22:21:31.000000 pyerualjetwork-1.0.5.post0/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 22:21:31.000000 pyerualjetwork-1.0.5.post0/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 22:21:31.000000 pyerualjetwork-1.0.5.post0/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 22:21:31.991065 pyerualjetwork-1.0.5.post0/setup.cfg
+-rw-rw-rw-   0        0        0      453 2024-05-22 22:21:16.000000 pyerualjetwork-1.0.5.post0/setup.py
```

