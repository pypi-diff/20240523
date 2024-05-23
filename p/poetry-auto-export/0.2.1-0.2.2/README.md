# Comparing `tmp/poetry_auto_export-0.2.1.tar.gz` & `tmp/poetry_auto_export-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_auto_export-0.2.1.tar", max compression
+gzip compressed data, was "poetry_auto_export-0.2.2.tar", max compression
```

## Comparing `poetry_auto_export-0.2.1.tar` & `poetry_auto_export-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2024-03-10 23:44:03.963632 poetry_auto_export-0.2.1/LICENSE
--rw-r--r--   0        0        0     2566 2024-03-10 23:44:03.963632 poetry_auto_export-0.2.1/README.md
--rw-r--r--   0        0        0       87 2024-03-10 23:44:03.963632 poetry_auto_export-0.2.1/poetry_auto_export/__init__.py
--rw-r--r--   0        0        0     5248 2024-03-10 23:44:03.963632 poetry_auto_export-0.2.1/poetry_auto_export/plugin.py
--rw-r--r--   0        0        0      726 2024-03-10 23:44:03.963632 poetry_auto_export-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3310 1970-01-01 00:00:00.000000 poetry_auto_export-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-23 20:18:32.608220 poetry_auto_export-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2566 2024-05-23 20:18:32.608220 poetry_auto_export-0.2.2/README.md
+-rw-r--r--   0        0        0       87 2024-05-23 20:18:32.608220 poetry_auto_export-0.2.2/poetry_auto_export/__init__.py
+-rw-r--r--   0        0        0     5340 2024-05-23 20:18:32.608220 poetry_auto_export-0.2.2/poetry_auto_export/plugin.py
+-rw-r--r--   0        0        0      726 2024-05-23 20:18:32.608220 poetry_auto_export-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3310 1970-01-01 00:00:00.000000 poetry_auto_export-0.2.2/PKG-INFO
```

### Comparing `poetry_auto_export-0.2.1/LICENSE` & `poetry_auto_export-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_auto_export-0.2.1/README.md` & `poetry_auto_export-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `poetry_auto_export-0.2.1/poetry_auto_export/plugin.py` & `poetry_auto_export-0.2.2/poetry_auto_export/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 Export = dict
 
 
 class PoetryAutoExport(ApplicationPlugin):
     def activate(self, application: Application):
         if not application.event_dispatcher:
             return
+        try:
+            application.poetry
+        except RuntimeError:
+            return
         self.configs = self._parse_pyproject(application.poetry.pyproject.data)
         application.event_dispatcher.add_listener(TERMINATE, self.run_exports)
         return super().activate(application)
 
     def _parse_pyproject(self, pyproject: Container) -> list[Export]:
         """Parse the pyproject.toml file for export configuration(s)."""
         configs: list[Export] = []
```

### Comparing `poetry_auto_export-0.2.1/pyproject.toml` & `poetry_auto_export-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-auto-export"
-version = "0.2.1"
+version = "0.2.2"
 description = "Automatically create requirements.txt on every poetry lock"
 authors = ["Hubert Bereś <h.beres@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Ddedalus/poetry-auto-export"
 packages = [{ include = "poetry_auto_export" }]
 [tool.poetry.dependencies]
```

### Comparing `poetry_auto_export-0.2.1/PKG-INFO` & `poetry_auto_export-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-auto-export
-Version: 0.2.1
+Version: 0.2.2
 Summary: Automatically create requirements.txt on every poetry lock
 Home-page: https://github.com/Ddedalus/poetry-auto-export
 License: MIT
 Author: Hubert Bereś
 Author-email: h.beres@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

