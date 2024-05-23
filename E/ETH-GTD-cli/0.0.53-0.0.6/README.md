# Comparing `tmp/eth_gtd_cli-0.0.53.tar.gz` & `tmp/eth_gtd_cli-0.0.6.tar.gz`

## Comparing `eth_gtd_cli-0.0.53.tar` & `eth_gtd_cli-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,16 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.53/deploy.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.53/src/ETH_GTD_cli/__init__.py
--rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.53/src/ETH_GTD_cli/auth.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.53/src/ETH_GTD_cli/consts.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.53/src/ETH_GTD_cli/helper.py
--rw-r--r--   0        0        0     8641 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.53/src/ETH_GTD_cli/main.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.53/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.53/LICENSE
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.53/README.md
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.53/pyproject.toml
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.53/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/.idea/.gitignore
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/.idea/CLI.iml
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/.idea/misc.xml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/.idea/modules.xml
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/.idea/vcs.xml
+-rw-r--r--   0        0        0     8397 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/.idea/workspace.xml
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/src/ETH_GTD_cli/__init__.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/src/ETH_GTD_cli/consts.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/src/ETH_GTD_cli/helper.py
+-rw-r--r--   0        0        0     6247 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/src/ETH_GTD_cli/main.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/LICENSE
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/PKG-INFO
```

### Comparing `eth_gtd_cli-0.0.53/src/ETH_GTD_cli/helper.py` & `eth_gtd_cli-0.0.6/src/ETH_GTD_cli/helper.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,97 @@
 import fnmatch
-import math
 import os
 import threading
-import glob
 
 import httpx
 import tqdm
 from rich import print
 import queue
 
 from .consts import API_URL
-from typing import Dict
 
-def expand_and_match(path_pattern):
-    expanded_path = os.path.expanduser(path_pattern)
-    expanded_path = os.path.expandvars(expanded_path)
 
-    normalized_path = os.path.normpath(expanded_path)
+def list_files_recursive(path, recursive: bool, pattern: str, depth: int = 0):
+    files = []
+    res = {}
+    try:
+        entries = os.listdir(path)
+    except PermissionError:
+        return False
+
+    for entry in entries:
+        full_path = os.path.join(path, entry)
+        if os.path.isdir(full_path):
+            if recursive:
+                sub_res = list_files_recursive(full_path, recursive, pattern, depth + 1)
+                if sub_res:
+                    res[full_path.split('/')[-1]] = sub_res
+        elif fnmatch.fnmatch(entry, pattern):
+            files.append(entry)
+
+    if len(files) > 0:
+        res[''] = files
+    if len(res.keys()) > 0:
+        return res
+    return None
+
+def printFiles(files, depth: int = 0):
+    for key in files.keys():
+        if key == "":
+            for file in files[key]:
+                print("  " * depth + "- " + file)
+        else:
+            print("  " * depth + "- " + key)
+            printFiles(files[key], depth + 1)
+
+def convertFilesStructure(files, currentDir: str = ""):
+    res = []
+    for key in files.keys():
+        if key == "":
+            for file in files[key]:
+                res.append(currentDir + file)
+        else:
+            res.extend(convertFilesStructure(files[key], currentDir + key + "/"))
+    return res
 
-    if '**' in normalized_path:
-        file_list = glob.glob(normalized_path, recursive=True)
-    else:
-        file_list = glob.glob(normalized_path)
-
-    return file_list
-
-def uploadFiles(files: Dict[str, str], paths: Dict[str,str], nrThreads: int):
+def uploadFiles(files: dict[str, str], paths: dict[str,str], nrThreads: int):
     _queue = queue.Queue()
     for file in files.items():
         _queue.put(file)
     threads = []
-    pbar = tqdm.tqdm(total=len(files.items())*100)
+    pbar = tqdm.tqdm(total=len(files.items()))
     for i in range(nrThreads):
         thread = threading.Thread(target=uploadFile, args=(_queue, paths, pbar))
         thread.start()
         threads.append(thread)
     for thread in threads:
         thread.join()
 
-def uploadFile(_queue: queue.Queue, paths: Dict[str, str], pbar: tqdm):
+def uploadFile(_queue: queue.Queue, paths: dict[str, str], pbar: tqdm):
     while True:
         try:
             filename, url = _queue.get(timeout=3)
             filepath = paths[filename]
-            headers = {
-                'Content-Type': 'application/octet-stream'
-            }
-            chunk_size = 4096 * 512
             with open(filepath, "rb") as f:
-                nr_chunks = math.ceil(os.path.getsize(filepath) / chunk_size)
-                update_size = math.floor(1000000 / nr_chunks) / 10000
-
-                print(f"Uploading: {filename}")
-                while chunk := f.read(chunk_size):  # Read in chunks of 4KB
-                    resp = httpx.put(url, content=chunk, headers=headers, timeout=60.0)
-                    resp.raise_for_status()
-                    pbar.update(update_size)
+                file_data = f.read()
+                headers = {
+                    'Content-Type': 'application/octet-stream'
+                }
 
+                resp = httpx.put(url, content=file_data, headers=headers)
+                resp.raise_for_status()
                 httpx.post(API_URL + "/queue/confirmUpload", json={"filename": filename})
+                pbar.update(1)
 
         except queue.Empty:
             break
 
 
 if __name__ == '__main__':
-    res = expand_and_match("~/Downloads/dodo_mission_2024_02_08-20240408T074313Z-003/**.bag")
-    print(res)
+    path = '~/Downloads/dodo_mission_2024_02_08-20240408T074313Z-004/dodo_mission_2024_02_08'
+    path = os.path.expanduser(path)
+    files = list_files_recursive(
+        path,
+        True,
+        pattern='*.bag')
+    printFiles(files)
+    print(convertFilesStructure(files))
```

### Comparing `eth_gtd_cli-0.0.53/LICENSE` & `eth_gtd_cli-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.53/pyproject.toml` & `eth_gtd_cli-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ETH_GTD_cli"
-version = "0.0.53"
+version = "0.0.6"
 authors = [
   { name="Johann Schwabe", email="jschwab@ethz.ch" },
 ]
 description = "A CLI for the ETH project Grand Tour"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 dependencies = [
   "typer",
   "httpx",
   "tqdm"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

