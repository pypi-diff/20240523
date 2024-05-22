# Comparing `tmp/pyerualjetwork-1.0.6.tar.gz` & `tmp/pyerualjetwork-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.0.6.tar", last modified: Wed May 22 22:46:27 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.0.7.tar", last modified: Wed May 22 22:57:05 2024, max compression
```

## Comparing `pyerualjetwork-1.0.6.tar` & `pyerualjetwork-1.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 22:46:27.960766 pyerualjetwork-1.0.6/
--rw-rw-rw-   0        0        0      276 2024-05-22 22:46:27.951760 pyerualjetwork-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-22 22:46:27.936138 pyerualjetwork-1.0.6/pyerualjetwork/
--rw-rw-rw-   0        0        0      659 2024-05-22 22:41:43.000000 pyerualjetwork-1.0.6/pyerualjetwork/__init__.py
--rw-rw-rw-   0        0        0    40243 2024-05-22 22:36:00.000000 pyerualjetwork-1.0.6/pyerualjetwork/pyerualjetwork.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:46:27.951760 pyerualjetwork-1.0.6/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      276 2024-05-22 22:46:27.000000 pyerualjetwork-1.0.6/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-05-22 22:46:27.000000 pyerualjetwork-1.0.6/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 22:46:27.000000 pyerualjetwork-1.0.6/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-22 22:46:27.000000 pyerualjetwork-1.0.6/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 22:46:27.960766 pyerualjetwork-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      452 2024-05-22 22:44:15.000000 pyerualjetwork-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:57:05.945253 pyerualjetwork-1.0.7/
+-rw-rw-rw-   0        0        0      276 2024-05-22 22:57:05.945253 pyerualjetwork-1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 22:57:05.930750 pyerualjetwork-1.0.7/pyerualjetwork/
+-rw-rw-rw-   0        0        0      636 2024-05-22 22:56:06.000000 pyerualjetwork-1.0.7/pyerualjetwork/__init__.py
+-rw-rw-rw-   0        0        0    40243 2024-05-22 22:36:00.000000 pyerualjetwork-1.0.7/pyerualjetwork/pyerualjetwork.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:57:05.945253 pyerualjetwork-1.0.7/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      276 2024-05-22 22:57:05.000000 pyerualjetwork-1.0.7/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-05-22 22:57:05.000000 pyerualjetwork-1.0.7/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 22:57:05.000000 pyerualjetwork-1.0.7/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-22 22:57:05.000000 pyerualjetwork-1.0.7/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 22:57:05.945253 pyerualjetwork-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      452 2024-05-22 22:56:52.000000 pyerualjetwork-1.0.7/setup.py
```

### Comparing `pyerualjetwork-1.0.6/pyerualjetwork/__init__.py` & `pyerualjetwork-1.0.7/pyerualjetwork/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import pyerualjetwork
 from pyerualjetwork import TrainDPNN
 from pyerualjetwork import WeightIdentification
 from pyerualjetwork import SynapticPruning
 from pyerualjetwork import SynapticDividing
 from pyerualjetwork import Fex
 from pyerualjetwork import Cat
 from pyerualjetwork import Normalization
```

### Comparing `pyerualjetwork-1.0.6/pyerualjetwork/pyerualjetwork.py` & `pyerualjetwork-1.0.7/pyerualjetwork/pyerualjetwork.py`

 * *Files identical despite different names*

