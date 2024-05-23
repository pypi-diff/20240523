# Comparing `tmp/torcj-0.0.7.tar.gz` & `tmp/torcj-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torcj-0.0.7.tar", last modified: Thu May 23 11:16:00 2024, max compression
+gzip compressed data, was "torcj-0.0.8.tar", last modified: Thu May 23 11:21:32 2024, max compression
```

## Comparing `torcj-0.0.7.tar` & `torcj-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:16:00.656245 torcj-0.0.7/
--rw-r--r--   0 castle    (1000) castle    (1000)       93 2024-05-23 11:16:00.656245 torcj-0.0.7/PKG-INFO
--rw-r--r--   0 castle    (1000) castle    (1000)       59 2024-05-23 10:33:25.000000 torcj-0.0.7/README.md
--rw-r--r--   0 castle    (1000) castle    (1000)       38 2024-05-23 11:16:00.656245 torcj-0.0.7/setup.cfg
--rw-r--r--   0 castle    (1000) castle    (1000)      209 2024-05-23 11:15:58.000000 torcj-0.0.7/setup.py
-drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:16:00.654245 torcj-0.0.7/torcj/
--rw-r--r--   0 castle    (1000) castle    (1000)       29 2024-05-23 10:53:35.000000 torcj-0.0.7/torcj/__init__.py
--rw-r--r--   0 castle    (1000) castle    (1000)     1494 2024-05-23 11:03:27.000000 torcj-0.0.7/torcj/main.py
--rw-r--r--   0 castle    (1000) castle    (1000)   106896 2024-05-23 10:29:40.000000 torcj-0.0.7/torcj/storage.json
-drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:16:00.656245 torcj-0.0.7/torcj.egg-info/
--rw-r--r--   0 castle    (1000) castle    (1000)       93 2024-05-23 11:16:00.000000 torcj-0.0.7/torcj.egg-info/PKG-INFO
--rw-r--r--   0 castle    (1000) castle    (1000)      185 2024-05-23 11:16:00.000000 torcj-0.0.7/torcj.egg-info/SOURCES.txt
--rw-r--r--   0 castle    (1000) castle    (1000)        1 2024-05-23 11:16:00.000000 torcj-0.0.7/torcj.egg-info/dependency_links.txt
--rw-r--r--   0 castle    (1000) castle    (1000)        6 2024-05-23 11:16:00.000000 torcj-0.0.7/torcj.egg-info/top_level.txt
+drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:21:32.836288 torcj-0.0.8/
+-rw-r--r--   0 castle    (1000) castle    (1000)       93 2024-05-23 11:21:32.836288 torcj-0.0.8/PKG-INFO
+-rw-r--r--   0 castle    (1000) castle    (1000)       59 2024-05-23 10:33:25.000000 torcj-0.0.8/README.md
+-rw-r--r--   0 castle    (1000) castle    (1000)       38 2024-05-23 11:21:32.836288 torcj-0.0.8/setup.cfg
+-rw-r--r--   0 castle    (1000) castle    (1000)      209 2024-05-23 11:20:46.000000 torcj-0.0.8/setup.py
+drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:21:32.834288 torcj-0.0.8/torcj/
+-rw-r--r--   0 castle    (1000) castle    (1000)       29 2024-05-23 10:53:35.000000 torcj-0.0.8/torcj/__init__.py
+-rw-r--r--   0 castle    (1000) castle    (1000)     1497 2024-05-23 11:20:48.000000 torcj-0.0.8/torcj/main.py
+-rw-r--r--   0 castle    (1000) castle    (1000)   106896 2024-05-23 10:29:40.000000 torcj-0.0.8/torcj/storage.json
+drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:21:32.836288 torcj-0.0.8/torcj.egg-info/
+-rw-r--r--   0 castle    (1000) castle    (1000)       93 2024-05-23 11:21:32.000000 torcj-0.0.8/torcj.egg-info/PKG-INFO
+-rw-r--r--   0 castle    (1000) castle    (1000)      185 2024-05-23 11:21:32.000000 torcj-0.0.8/torcj.egg-info/SOURCES.txt
+-rw-r--r--   0 castle    (1000) castle    (1000)        1 2024-05-23 11:21:32.000000 torcj-0.0.8/torcj.egg-info/dependency_links.txt
+-rw-r--r--   0 castle    (1000) castle    (1000)        6 2024-05-23 11:21:32.000000 torcj-0.0.8/torcj.egg-info/top_level.txt
```

### Comparing `torcj-0.0.7/torcj/main.py` & `torcj-0.0.8/torcj/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         print([i for i in self.data])
 
     def print_file(self, name) -> str:
         print(self.data[name])
         return self.data[name]
 
     def write_file(self, name: str) -> None:
-        with open("main.py", "w") as f:
+        with open("main.ipynb", "w") as f:
             f.write(self.data[name])
 
 
 class TextStore:
     def read_python_files(directory: str) -> None:
         python_files = [
             file
```

### Comparing `torcj-0.0.7/torcj/storage.json` & `torcj-0.0.8/torcj/storage.json`

 * *Files identical despite different names*

