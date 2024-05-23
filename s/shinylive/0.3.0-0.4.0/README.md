# Comparing `tmp/shinylive-0.3.0.tar.gz` & `tmp/shinylive-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinylive-0.3.0.tar", last modified: Tue Apr 16 17:10:10 2024, max compression
+gzip compressed data, was "shinylive-0.4.0.tar", last modified: Thu May 23 20:35:15 2024, max compression
```

## Comparing `shinylive-0.3.0.tar` & `shinylive-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:10:10.550255 shinylive-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-16 17:09:52.000000 shinylive-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-16 17:10:10.550255 shinylive-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-16 17:09:52.000000 shinylive-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-16 17:10:10.550255 shinylive-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 17:09:52.000000 shinylive-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:10:10.550255 shinylive-0.3.0/shinylive/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-16 17:09:52.000000 shinylive-0.3.0/shinylive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-16 17:09:52.000000 shinylive-0.3.0/shinylive/_app_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-04-16 17:09:52.000000 shinylive-0.3.0/shinylive/_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)    19194 2024-04-16 17:09:52.000000 shinylive-0.3.0/shinylive/_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-04-16 17:09:52.000000 shinylive-0.3.0/shinylive/_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    17783 2024-04-16 17:09:52.000000 shinylive-0.3.0/shinylive/_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    25113 2024-04-16 17:09:52.000000 shinylive-0.3.0/shinylive/_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-16 17:09:52.000000 shinylive-0.3.0/shinylive/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:10:10.550255 shinylive-0.3.0/shinylive/_version/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-16 17:09:52.000000 shinylive-0.3.0/shinylive/_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:09:52.000000 shinylive-0.3.0/shinylive/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:10:10.550255 shinylive-0.3.0/shinylive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-16 17:10:10.000000 shinylive-0.3.0/shinylive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-16 17:10:10.000000 shinylive-0.3.0/shinylive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:10:10.000000 shinylive-0.3.0/shinylive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 17:10:10.000000 shinylive-0.3.0/shinylive.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:10:10.000000 shinylive-0.3.0/shinylive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-16 17:10:10.000000 shinylive-0.3.0/shinylive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 17:10:10.000000 shinylive-0.3.0/shinylive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:35:15.849802 shinylive-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-23 20:34:59.000000 shinylive-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-23 20:35:15.849802 shinylive-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-23 20:34:59.000000 shinylive-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-23 20:35:15.849802 shinylive-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 20:34:59.000000 shinylive-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:35:15.849802 shinylive-0.4.0/shinylive/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-23 20:34:59.000000 shinylive-0.4.0/shinylive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-23 20:34:59.000000 shinylive-0.4.0/shinylive/_app_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-05-23 20:34:59.000000 shinylive-0.4.0/shinylive/_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19230 2024-05-23 20:34:59.000000 shinylive-0.4.0/shinylive/_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-05-23 20:34:59.000000 shinylive-0.4.0/shinylive/_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17783 2024-05-23 20:34:59.000000 shinylive-0.4.0/shinylive/_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25131 2024-05-23 20:34:59.000000 shinylive-0.4.0/shinylive/_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-23 20:34:59.000000 shinylive-0.4.0/shinylive/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:35:15.849802 shinylive-0.4.0/shinylive/_version/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-23 20:34:59.000000 shinylive-0.4.0/shinylive/_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:34:59.000000 shinylive-0.4.0/shinylive/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:35:15.849802 shinylive-0.4.0/shinylive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-23 20:35:15.000000 shinylive-0.4.0/shinylive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-23 20:35:15.000000 shinylive-0.4.0/shinylive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:35:15.000000 shinylive-0.4.0/shinylive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-23 20:35:15.000000 shinylive-0.4.0/shinylive.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:35:15.000000 shinylive-0.4.0/shinylive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-23 20:35:15.000000 shinylive-0.4.0/shinylive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 20:35:15.000000 shinylive-0.4.0/shinylive.egg-info/top_level.txt
```

### Comparing `shinylive-0.3.0/LICENSE` & `shinylive-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shinylive-0.3.0/PKG-INFO` & `shinylive-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shinylive
-Version: 0.3.0
+Version: 0.4.0
 Summary: Run Shiny applications running Python in the browser.
 Home-page: https://github.com/posit-dev/py-shinylive
 Author: Winston Chang
 Author-email: winston@posit.co
 License: MIT
 Project-URL: Bug Tracker, https://github.com/posit-dev/py-shinylive/issues
 Project-URL: Documentation, https://github.com/posit-dev/py-shinylive
```

### Comparing `shinylive-0.3.0/README.md` & `shinylive-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `shinylive-0.3.0/setup.cfg` & `shinylive-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `shinylive-0.3.0/shinylive/_app_json.py` & `shinylive-0.4.0/shinylive/_app_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             if filename == "shinylive.js":
                 print(
                     f"Warning: Found shinylive.js in source directory '{appdir}/{rel_dir}'. Are you including a shinylive distribution in your app?"
                 )
 
             type: Literal["text", "binary"] = "text"
             try:
-                with open(root / filename, "r") as f:
+                with open(root / filename, "r", encoding="utf-8") as f:
                     file_content = f.read()
                     type = "text"
             except UnicodeDecodeError:
                 # If text failed, try binary.
                 with open(root / filename, "rb") as f:
                     file_content_bin = f.read()
                     file_content = base64.b64encode(file_content_bin).decode("utf-8")
```

### Comparing `shinylive-0.3.0/shinylive/_assets.py` & `shinylive-0.4.0/shinylive/_assets.py`

 * *Files identical despite different names*

### Comparing `shinylive-0.3.0/shinylive/_deps.py` & `shinylive-0.4.0/shinylive/_deps.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,15 +326,15 @@
     ):
         raise RuntimeError("Must provide either `json_file` or `json_content`.")
 
     file_contents: list[FileContentJson] = []
 
     if json_file is not None:
         json_file = Path(json_file)
-        with open(json_file) as f:
+        with open(json_file, encoding="utf-8") as f:
             file_contents = json.load(f)
 
     if json_content is not None:
         file_contents = json.loads(json_content)
 
     pkg_infos = find_package_deps(file_contents)
     deps = _pyodide_pkg_infos_to_quarto_html_dep_items(pkg_infos)
@@ -510,15 +510,15 @@
 @functools.lru_cache
 def _pyodide_lock_data() -> PyodideLockFile:
     """
     Read in the Pyodide pyodide-lock.json file and return the contents. The result is
     cached, so if the file changes, it won't register until the Python session is
     restarted.
     """
-    with open(pyodide_lock_json_file(), "r") as f:
+    with open(pyodide_lock_json_file(), "r", encoding="utf-8") as f:
         return json.load(f)
 
 
 # From pyodide._base.find_imports
 def _find_imports(source: str) -> list[str]:
     """
     Finds the imports in a Python source code string
```

### Comparing `shinylive-0.3.0/shinylive/_export.py` & `shinylive-0.4.0/shinylive/_export.py`

 * *Files identical despite different names*

### Comparing `shinylive-0.3.0/shinylive/_main.py` & `shinylive-0.4.0/shinylive/_main.py`

 * *Files identical despite different names*

### Comparing `shinylive-0.3.0/shinylive/_url.py` & `shinylive-0.4.0/shinylive/_url.py`

 * *Files 0% similar despite different names*

```diff
@@ -725,15 +725,15 @@
 # Copied from https://github.com/posit-dev/py-shiny/blob/main/docs/_renderer.py#L231
 def read_file(file: str | Path, root_dir: str | Path | None = None) -> FileContentJson:
     file = Path(file)
 
     type: Literal["text", "binary"] = "text"
 
     try:
-        with open(file, "r") as f:
+        with open(file, "r", encoding="utf-8") as f:
             file_content = f.read()
             type = "text"
     except UnicodeDecodeError:
         # If text failed, try binary.
         with open(file, "rb") as f:
             file_content_bin = f.read()
             file_content = base64.b64encode(file_content_bin).decode("utf-8")
```

### Comparing `shinylive-0.3.0/shinylive/_utils.py` & `shinylive-0.4.0/shinylive/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 FromTo = Tuple[str, str]
 
 
 def copy_file_and_substitute(
     src: str | Path, dest: str | Path, *, replacements: Sequence[FromTo]
 ) -> None:
-    with open(src, "r") as fin:
+    with open(src, "r", encoding="utf-8") as fin:
         in_content = fin.read()
         for from_str, to_str in replacements:
             in_content = in_content.replace(from_str, to_str)
         with open(dest, "w") as fout:
             fout.write(in_content)
```

### Comparing `shinylive-0.3.0/shinylive.egg-info/PKG-INFO` & `shinylive-0.4.0/shinylive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shinylive
-Version: 0.3.0
+Version: 0.4.0
 Summary: Run Shiny applications running Python in the browser.
 Home-page: https://github.com/posit-dev/py-shinylive
 Author: Winston Chang
 Author-email: winston@posit.co
 License: MIT
 Project-URL: Bug Tracker, https://github.com/posit-dev/py-shinylive/issues
 Project-URL: Documentation, https://github.com/posit-dev/py-shinylive
```

