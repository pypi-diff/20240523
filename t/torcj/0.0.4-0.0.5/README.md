# Comparing `tmp/torcj-0.0.4.tar.gz` & `tmp/torcj-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torcj-0.0.4.tar", last modified: Thu May 23 11:01:28 2024, max compression
+gzip compressed data, was "torcj-0.0.5.tar", last modified: Thu May 23 11:03:46 2024, max compression
```

## Comparing `torcj-0.0.4.tar` & `torcj-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:01:28.526224 torcj-0.0.4/
--rw-r--r--   0 castle    (1000) castle    (1000)       93 2024-05-23 11:01:28.525224 torcj-0.0.4/PKG-INFO
--rw-r--r--   0 castle    (1000) castle    (1000)       59 2024-05-23 10:33:25.000000 torcj-0.0.4/README.md
--rw-r--r--   0 castle    (1000) castle    (1000)       38 2024-05-23 11:01:28.526224 torcj-0.0.4/setup.cfg
--rw-r--r--   0 castle    (1000) castle    (1000)      163 2024-05-23 11:01:03.000000 torcj-0.0.4/setup.py
-drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:01:28.524224 torcj-0.0.4/torcj/
--rw-r--r--   0 castle    (1000) castle    (1000)       29 2024-05-23 10:53:35.000000 torcj-0.0.4/torcj/__init__.py
--rw-r--r--   0 castle    (1000) castle    (1000)     1506 2024-05-23 11:00:45.000000 torcj-0.0.4/torcj/main.py
-drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:01:28.525224 torcj-0.0.4/torcj.egg-info/
--rw-r--r--   0 castle    (1000) castle    (1000)       93 2024-05-23 11:01:28.000000 torcj-0.0.4/torcj.egg-info/PKG-INFO
--rw-r--r--   0 castle    (1000) castle    (1000)      166 2024-05-23 11:01:28.000000 torcj-0.0.4/torcj.egg-info/SOURCES.txt
--rw-r--r--   0 castle    (1000) castle    (1000)        1 2024-05-23 11:01:28.000000 torcj-0.0.4/torcj.egg-info/dependency_links.txt
--rw-r--r--   0 castle    (1000) castle    (1000)        6 2024-05-23 11:01:28.000000 torcj-0.0.4/torcj.egg-info/top_level.txt
+drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:03:46.137983 torcj-0.0.5/
+-rw-r--r--   0 castle    (1000) castle    (1000)       93 2024-05-23 11:03:46.137983 torcj-0.0.5/PKG-INFO
+-rw-r--r--   0 castle    (1000) castle    (1000)       59 2024-05-23 10:33:25.000000 torcj-0.0.5/README.md
+-rw-r--r--   0 castle    (1000) castle    (1000)       38 2024-05-23 11:03:46.137983 torcj-0.0.5/setup.cfg
+-rw-r--r--   0 castle    (1000) castle    (1000)      163 2024-05-23 11:03:43.000000 torcj-0.0.5/setup.py
+drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:03:46.136983 torcj-0.0.5/torcj/
+-rw-r--r--   0 castle    (1000) castle    (1000)       29 2024-05-23 10:53:35.000000 torcj-0.0.5/torcj/__init__.py
+-rw-r--r--   0 castle    (1000) castle    (1000)     1494 2024-05-23 11:03:27.000000 torcj-0.0.5/torcj/main.py
+drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:03:46.137983 torcj-0.0.5/torcj.egg-info/
+-rw-r--r--   0 castle    (1000) castle    (1000)       93 2024-05-23 11:03:46.000000 torcj-0.0.5/torcj.egg-info/PKG-INFO
+-rw-r--r--   0 castle    (1000) castle    (1000)      166 2024-05-23 11:03:46.000000 torcj-0.0.5/torcj.egg-info/SOURCES.txt
+-rw-r--r--   0 castle    (1000) castle    (1000)        1 2024-05-23 11:03:46.000000 torcj-0.0.5/torcj.egg-info/dependency_links.txt
+-rw-r--r--   0 castle    (1000) castle    (1000)        6 2024-05-23 11:03:46.000000 torcj-0.0.5/torcj.egg-info/top_level.txt
```

### Comparing `torcj-0.0.4/torcj/main.py` & `torcj-0.0.5/torcj/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import os
 import json
 
+base_dir = os.path.dirname(__file__)
+directory_path = os.path.join(base_dir, "programs")
+json_output_file = os.path.join(base_dir, "storage.json")
+
 
 class TextWriter:
     def __init__(self) -> None:
         with open(os.path.join(base_dir, "storage.json"), "r") as file:
             self.data = json.load(file)
 
     def print_names(self) -> None:
@@ -38,14 +42,10 @@
 
     def save_to_json(data, output_file):
         with open(output_file, "w") as json_file:
             json.dump(data, json_file, indent=4)
 
 
 if __name__ == "__main__":
-    base_dir = os.path.dirname(__file__)
-    directory_path = os.path.join(base_dir, "programs")
-    json_output_file = os.path.join(base_dir, "storage.json")
-
     files_data = TextStore.read_python_files(directory_path)
     TextStore.save_to_json(files_data, json_output_file)
     print("Data successfully stored in", json_output_file)
```

