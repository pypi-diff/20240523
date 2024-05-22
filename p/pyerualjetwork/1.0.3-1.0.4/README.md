# Comparing `tmp/pyerualjetwork-1.0.3.tar.gz` & `tmp/pyerualjetwork-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.0.3.tar", last modified: Wed May 22 19:33:27 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.0.4.tar", last modified: Wed May 22 20:05:40 2024, max compression
```

## Comparing `pyerualjetwork-1.0.3.tar` & `pyerualjetwork-1.0.4.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 19:33:27.305801 pyerualjetwork-1.0.3/
--rw-rw-rw-   0        0        0      276 2024-05-22 19:33:27.305801 pyerualjetwork-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-22 19:33:27.290177 pyerualjetwork-1.0.3/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      276 2024-05-22 19:33:26.000000 pyerualjetwork-1.0.3/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2024-05-22 19:33:27.000000 pyerualjetwork-1.0.3/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 19:33:26.000000 pyerualjetwork-1.0.3/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 19:33:26.000000 pyerualjetwork-1.0.3/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 19:33:27.305801 pyerualjetwork-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      452 2024-05-22 19:22:44.000000 pyerualjetwork-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:05:40.029028 pyerualjetwork-1.0.4/
+drwxrwxrwx   0        0        0        0 2024-05-22 20:05:40.008742 pyerualjetwork-1.0.4/DPNN/
+-rw-rw-rw-   0        0        0    40242 2024-05-22 19:58:55.000000 pyerualjetwork-1.0.4/DPNN/DPNN.py
+-rw-rw-rw-   0        0        0      765 2024-05-22 19:21:22.000000 pyerualjetwork-1.0.4/DPNN/__init__.py
+-rw-rw-rw-   0        0        0      276 2024-05-22 20:05:40.025004 pyerualjetwork-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 20:05:40.025004 pyerualjetwork-1.0.4/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      276 2024-05-22 20:05:39.000000 pyerualjetwork-1.0.4/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-22 20:05:39.000000 pyerualjetwork-1.0.4/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 20:05:39.000000 pyerualjetwork-1.0.4/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-22 20:05:39.000000 pyerualjetwork-1.0.4/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 20:05:40.084936 pyerualjetwork-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      452 2024-05-22 20:05:22.000000 pyerualjetwork-1.0.4/setup.py
```

