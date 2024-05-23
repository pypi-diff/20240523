# Comparing `tmp/space_exploration_common_lib-0.0.7.tar.gz` & `tmp/space_exploration_common_lib-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space_exploration_common_lib-0.0.7.tar", last modified: Mon May 20 19:21:24 2024, max compression
+gzip compressed data, was "space_exploration_common_lib-0.0.8.tar", last modified: Thu May 23 16:53:57 2024, max compression
```

## Comparing `space_exploration_common_lib-0.0.7.tar` & `space_exploration_common_lib-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:24.958196 space_exploration_common_lib-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-20 19:21:24.958196 space_exploration_common_lib-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-20 19:21:12.000000 space_exploration_common_lib-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:21:24.958196 space_exploration_common_lib-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-20 19:21:12.000000 space_exploration_common_lib-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:24.958196 space_exploration_common_lib-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:24.958196 space_exploration_common_lib-0.0.7/src/space_exploration_common_lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:12.000000 space_exploration_common_lib-0.0.7/src/space_exploration_common_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:24.958196 space_exploration_common_lib-0.0.7/src/space_exploration_common_lib/model/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-20 19:21:12.000000 space_exploration_common_lib-0.0.7/src/space_exploration_common_lib/model/Duration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:12.000000 space_exploration_common_lib-0.0.7/src/space_exploration_common_lib/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:24.958196 space_exploration_common_lib-0.0.7/src/space_exploration_common_lib/model/mission/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-20 19:21:12.000000 space_exploration_common_lib-0.0.7/src/space_exploration_common_lib/model/mission/ProjectMercury.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:12.000000 space_exploration_common_lib-0.0.7/src/space_exploration_common_lib/model/mission/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:24.958196 space_exploration_common_lib-0.0.7/src/space_exploration_common_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-20 19:21:24.000000 space_exploration_common_lib-0.0.7/src/space_exploration_common_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-20 19:21:24.000000 space_exploration_common_lib-0.0.7/src/space_exploration_common_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:21:24.000000 space_exploration_common_lib-0.0.7/src/space_exploration_common_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 19:21:24.000000 space_exploration_common_lib-0.0.7/src/space_exploration_common_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-20 19:21:24.000000 space_exploration_common_lib-0.0.7/src/space_exploration_common_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:53:57.356332 space_exploration_common_lib-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-23 16:53:57.356332 space_exploration_common_lib-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-23 16:53:44.000000 space_exploration_common_lib-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 16:53:57.356332 space_exploration_common_lib-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-23 16:53:44.000000 space_exploration_common_lib-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:53:57.352332 space_exploration_common_lib-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:53:57.352332 space_exploration_common_lib-0.0.8/src/space_exploration_common_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:53:44.000000 space_exploration_common_lib-0.0.8/src/space_exploration_common_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:53:57.356332 space_exploration_common_lib-0.0.8/src/space_exploration_common_lib/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-23 16:53:44.000000 space_exploration_common_lib-0.0.8/src/space_exploration_common_lib/model/Astronaut.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-23 16:53:44.000000 space_exploration_common_lib-0.0.8/src/space_exploration_common_lib/model/Duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:53:44.000000 space_exploration_common_lib-0.0.8/src/space_exploration_common_lib/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:53:57.356332 space_exploration_common_lib-0.0.8/src/space_exploration_common_lib/model/mission/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-23 16:53:44.000000 space_exploration_common_lib-0.0.8/src/space_exploration_common_lib/model/mission/ProjectMercury.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:53:44.000000 space_exploration_common_lib-0.0.8/src/space_exploration_common_lib/model/mission/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:53:57.356332 space_exploration_common_lib-0.0.8/src/space_exploration_common_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-23 16:53:57.000000 space_exploration_common_lib-0.0.8/src/space_exploration_common_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-23 16:53:57.000000 space_exploration_common_lib-0.0.8/src/space_exploration_common_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 16:53:57.000000 space_exploration_common_lib-0.0.8/src/space_exploration_common_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 16:53:57.000000 space_exploration_common_lib-0.0.8/src/space_exploration_common_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-23 16:53:57.000000 space_exploration_common_lib-0.0.8/src/space_exploration_common_lib.egg-info/top_level.txt
```

### Comparing `space_exploration_common_lib-0.0.7/setup.py` & `space_exploration_common_lib-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `space_exploration_common_lib-0.0.7/src/space_exploration_common_lib/model/mission/ProjectMercury.py` & `space_exploration_common_lib-0.0.8/src/space_exploration_common_lib/model/mission/ProjectMercury.py`

 * *Files identical despite different names*

### Comparing `space_exploration_common_lib-0.0.7/src/space_exploration_common_lib.egg-info/SOURCES.txt` & `space_exploration_common_lib-0.0.8/src/space_exploration_common_lib.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,11 +2,12 @@
 setup.py
 src/space_exploration_common_lib/__init__.py
 src/space_exploration_common_lib.egg-info/PKG-INFO
 src/space_exploration_common_lib.egg-info/SOURCES.txt
 src/space_exploration_common_lib.egg-info/dependency_links.txt
 src/space_exploration_common_lib.egg-info/requires.txt
 src/space_exploration_common_lib.egg-info/top_level.txt
+src/space_exploration_common_lib/model/Astronaut.py
 src/space_exploration_common_lib/model/Duration.py
 src/space_exploration_common_lib/model/__init__.py
 src/space_exploration_common_lib/model/mission/ProjectMercury.py
 src/space_exploration_common_lib/model/mission/__init__.py
```

