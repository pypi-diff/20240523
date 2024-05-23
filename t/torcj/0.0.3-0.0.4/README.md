# Comparing `tmp/torcj-0.0.3.tar.gz` & `tmp/torcj-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torcj-0.0.3.tar", last modified: Thu May 23 10:58:48 2024, max compression
+gzip compressed data, was "torcj-0.0.4.tar", last modified: Thu May 23 11:01:28 2024, max compression
```

## Comparing `torcj-0.0.3.tar` & `torcj-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 10:58:48.490236 torcj-0.0.3/
--rw-r--r--   0 castle    (1000) castle    (1000)       93 2024-05-23 10:58:48.489235 torcj-0.0.3/PKG-INFO
--rw-r--r--   0 castle    (1000) castle    (1000)       59 2024-05-23 10:33:25.000000 torcj-0.0.3/README.md
--rw-r--r--   0 castle    (1000) castle    (1000)       38 2024-05-23 10:58:48.490236 torcj-0.0.3/setup.cfg
--rw-r--r--   0 castle    (1000) castle    (1000)      163 2024-05-23 10:58:43.000000 torcj-0.0.3/setup.py
-drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 10:58:48.488234 torcj-0.0.3/torcj/
--rw-r--r--   0 castle    (1000) castle    (1000)       29 2024-05-23 10:53:35.000000 torcj-0.0.3/torcj/__init__.py
--rw-r--r--   0 castle    (1000) castle    (1000)     1493 2024-05-23 10:53:32.000000 torcj-0.0.3/torcj/main.py
-drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 10:58:48.489235 torcj-0.0.3/torcj.egg-info/
--rw-r--r--   0 castle    (1000) castle    (1000)       93 2024-05-23 10:58:48.000000 torcj-0.0.3/torcj.egg-info/PKG-INFO
--rw-r--r--   0 castle    (1000) castle    (1000)      166 2024-05-23 10:58:48.000000 torcj-0.0.3/torcj.egg-info/SOURCES.txt
--rw-r--r--   0 castle    (1000) castle    (1000)        1 2024-05-23 10:58:48.000000 torcj-0.0.3/torcj.egg-info/dependency_links.txt
--rw-r--r--   0 castle    (1000) castle    (1000)        6 2024-05-23 10:58:48.000000 torcj-0.0.3/torcj.egg-info/top_level.txt
+drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:01:28.526224 torcj-0.0.4/
+-rw-r--r--   0 castle    (1000) castle    (1000)       93 2024-05-23 11:01:28.525224 torcj-0.0.4/PKG-INFO
+-rw-r--r--   0 castle    (1000) castle    (1000)       59 2024-05-23 10:33:25.000000 torcj-0.0.4/README.md
+-rw-r--r--   0 castle    (1000) castle    (1000)       38 2024-05-23 11:01:28.526224 torcj-0.0.4/setup.cfg
+-rw-r--r--   0 castle    (1000) castle    (1000)      163 2024-05-23 11:01:03.000000 torcj-0.0.4/setup.py
+drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:01:28.524224 torcj-0.0.4/torcj/
+-rw-r--r--   0 castle    (1000) castle    (1000)       29 2024-05-23 10:53:35.000000 torcj-0.0.4/torcj/__init__.py
+-rw-r--r--   0 castle    (1000) castle    (1000)     1506 2024-05-23 11:00:45.000000 torcj-0.0.4/torcj/main.py
+drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:01:28.525224 torcj-0.0.4/torcj.egg-info/
+-rw-r--r--   0 castle    (1000) castle    (1000)       93 2024-05-23 11:01:28.000000 torcj-0.0.4/torcj.egg-info/PKG-INFO
+-rw-r--r--   0 castle    (1000) castle    (1000)      166 2024-05-23 11:01:28.000000 torcj-0.0.4/torcj.egg-info/SOURCES.txt
+-rw-r--r--   0 castle    (1000) castle    (1000)        1 2024-05-23 11:01:28.000000 torcj-0.0.4/torcj.egg-info/dependency_links.txt
+-rw-r--r--   0 castle    (1000) castle    (1000)        6 2024-05-23 11:01:28.000000 torcj-0.0.4/torcj.egg-info/top_level.txt
```

### Comparing `torcj-0.0.3/torcj/main.py` & `torcj-0.0.4/torcj/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import json
 
 
 class TextWriter:
-    def __init__(self, json_file: str) -> None:
-        with open(json_file, "r") as file:
+    def __init__(self) -> None:
+        with open(os.path.join(base_dir, "storage.json"), "r") as file:
             self.data = json.load(file)
 
     def print_names(self) -> None:
         print([i for i in self.data])
 
     def print_file(self, name) -> str:
         print(self.data[name])
```

