# Comparing `tmp/torcj-0.0.8.tar.gz` & `tmp/torcj-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torcj-0.0.8.tar", last modified: Thu May 23 11:21:32 2024, max compression
+gzip compressed data, was "torcj-0.0.9.tar", last modified: Thu May 23 12:38:14 2024, max compression
```

## Comparing `torcj-0.0.8.tar` & `torcj-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:21:32.836288 torcj-0.0.8/
--rw-r--r--   0 castle    (1000) castle    (1000)       93 2024-05-23 11:21:32.836288 torcj-0.0.8/PKG-INFO
--rw-r--r--   0 castle    (1000) castle    (1000)       59 2024-05-23 10:33:25.000000 torcj-0.0.8/README.md
--rw-r--r--   0 castle    (1000) castle    (1000)       38 2024-05-23 11:21:32.836288 torcj-0.0.8/setup.cfg
--rw-r--r--   0 castle    (1000) castle    (1000)      209 2024-05-23 11:20:46.000000 torcj-0.0.8/setup.py
-drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:21:32.834288 torcj-0.0.8/torcj/
--rw-r--r--   0 castle    (1000) castle    (1000)       29 2024-05-23 10:53:35.000000 torcj-0.0.8/torcj/__init__.py
--rw-r--r--   0 castle    (1000) castle    (1000)     1497 2024-05-23 11:20:48.000000 torcj-0.0.8/torcj/main.py
--rw-r--r--   0 castle    (1000) castle    (1000)   106896 2024-05-23 10:29:40.000000 torcj-0.0.8/torcj/storage.json
-drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:21:32.836288 torcj-0.0.8/torcj.egg-info/
--rw-r--r--   0 castle    (1000) castle    (1000)       93 2024-05-23 11:21:32.000000 torcj-0.0.8/torcj.egg-info/PKG-INFO
--rw-r--r--   0 castle    (1000) castle    (1000)      185 2024-05-23 11:21:32.000000 torcj-0.0.8/torcj.egg-info/SOURCES.txt
--rw-r--r--   0 castle    (1000) castle    (1000)        1 2024-05-23 11:21:32.000000 torcj-0.0.8/torcj.egg-info/dependency_links.txt
--rw-r--r--   0 castle    (1000) castle    (1000)        6 2024-05-23 11:21:32.000000 torcj-0.0.8/torcj.egg-info/top_level.txt
+drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 12:38:14.851007 torcj-0.0.9/
+-rw-r--r--   0 castle    (1000) castle    (1000)       93 2024-05-23 12:38:14.850007 torcj-0.0.9/PKG-INFO
+-rw-r--r--   0 castle    (1000) castle    (1000)       59 2024-05-23 10:33:25.000000 torcj-0.0.9/README.md
+-rw-r--r--   0 castle    (1000) castle    (1000)       38 2024-05-23 12:38:14.851007 torcj-0.0.9/setup.cfg
+-rw-r--r--   0 castle    (1000) castle    (1000)      209 2024-05-23 11:46:03.000000 torcj-0.0.9/setup.py
+drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 12:38:14.849007 torcj-0.0.9/torcj/
+-rw-r--r--   0 castle    (1000) castle    (1000)       29 2024-05-23 10:53:35.000000 torcj-0.0.9/torcj/__init__.py
+-rw-r--r--   0 castle    (1000) castle    (1000)     1558 2024-05-23 12:36:23.000000 torcj-0.0.9/torcj/main.py
+-rw-r--r--   0 castle    (1000) castle    (1000)   106896 2024-05-23 12:37:59.000000 torcj-0.0.9/torcj/storage.json
+drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 12:38:14.850007 torcj-0.0.9/torcj.egg-info/
+-rw-r--r--   0 castle    (1000) castle    (1000)       93 2024-05-23 12:38:14.000000 torcj-0.0.9/torcj.egg-info/PKG-INFO
+-rw-r--r--   0 castle    (1000) castle    (1000)      185 2024-05-23 12:38:14.000000 torcj-0.0.9/torcj.egg-info/SOURCES.txt
+-rw-r--r--   0 castle    (1000) castle    (1000)        1 2024-05-23 12:38:14.000000 torcj-0.0.9/torcj.egg-info/dependency_links.txt
+-rw-r--r--   0 castle    (1000) castle    (1000)        6 2024-05-23 12:38:14.000000 torcj-0.0.9/torcj.egg-info/top_level.txt
```

### Comparing `torcj-0.0.8/torcj/main.py` & `torcj-0.0.9/torcj/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,33 +2,37 @@
 import json
 
 base_dir = os.path.dirname(__file__)
 directory_path = os.path.join(base_dir, "programs")
 json_output_file = os.path.join(base_dir, "storage.json")
 
 
-class TextWriter:
+class Writer:
     def __init__(self) -> None:
         with open(os.path.join(base_dir, "storage.json"), "r") as file:
             self.data = json.load(file)
 
-    def print_names(self) -> None:
+    def names(self) -> None:
         print([i for i in self.data])
 
-    def print_file(self, name) -> str:
-        print(self.data[name])
-        return self.data[name]
+    def get(self, name: str):
+        cells = json.loads(self.data[name])["cells"]
+        text = ""
+        sources = [cell["source"] for cell in cells]
+        for i in sources:
+            text += "".join(i)
+        return text
 
-    def write_file(self, name: str) -> None:
+    def write(self, name: str) -> None:
         with open("main.ipynb", "w") as f:
             f.write(self.data[name])
 
 
-class TextStore:
-    def read_python_files(directory: str) -> None:
+class Store:
+    def read(directory: str) -> None:
         python_files = [
             file
             for file in os.listdir(directory)
             if file.endswith(".py") or file.endswith(".ipynb")
         ]
         files_data = {}
 
@@ -36,16 +40,16 @@
             file_path = os.path.join(directory, file_name)
             with open(file_path, "r") as file:
                 content = file.read()
                 files_data[file_name] = content
 
         return files_data
 
-    def save_to_json(data, output_file):
+    def save(data, output_file):
         with open(output_file, "w") as json_file:
             json.dump(data, json_file, indent=4)
 
 
 if __name__ == "__main__":
-    files_data = TextStore.read_python_files(directory_path)
-    TextStore.save_to_json(files_data, json_output_file)
+    files_data = Store.read(directory_path)
+    Store.save(files_data, json_output_file)
     print("Data successfully stored in", json_output_file)
```

### Comparing `torcj-0.0.8/torcj/storage.json` & `torcj-0.0.9/torcj/storage.json`

 * *Files identical despite different names*

