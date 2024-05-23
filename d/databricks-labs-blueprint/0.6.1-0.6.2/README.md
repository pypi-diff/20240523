# Comparing `tmp/databricks_labs_blueprint-0.6.1.tar.gz` & `tmp/databricks_labs_blueprint-0.6.2.tar.gz`

## Comparing `databricks_labs_blueprint-0.6.1.tar` & `databricks_labs_blueprint-0.6.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/__init__.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/__main__.py
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/cli.py
--rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/commands.py
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/entrypoint.py
--rw-r--r--   0        0        0    42934 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/installation.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/installer.py
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/limiter.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/logger.py
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/parallel.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/py.typed
--rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/tui.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/upgrades.py
--rw-r--r--   0        0        0    14116 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/wheels.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/.gitignore
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/LICENSE
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/NOTICE
--rw-r--r--   0        0        0    45992 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/README.md
--rw-r--r--   0        0        0    26290 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    46795 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/__init__.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/__main__.py
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/cli.py
+-rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/commands.py
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/entrypoint.py
+-rw-r--r--   0        0        0    42934 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/installation.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/installer.py
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/limiter.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/logger.py
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/parallel.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/py.typed
+-rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/tui.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/upgrades.py
+-rw-r--r--   0        0        0    14116 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/wheels.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/.gitignore
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/LICENSE
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/NOTICE
+-rw-r--r--   0        0        0    45992 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/README.md
+-rw-r--r--   0        0        0    26290 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0    46795 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/PKG-INFO
```

### Comparing `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/__main__.py` & `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/__main__.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/cli.py` & `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -32,14 +32,20 @@
     def prompts_argument_name(self) -> str | None:
         sig = inspect.signature(self.fn)
         for param in sig.parameters.values():
             if param.annotation is Prompts:
                 return param.name
         return None
 
+    def get_argument_type(self, argument_name: str) -> str | None:
+        sig = inspect.signature(self.fn)
+        if argument_name not in sig.parameters:
+            return None
+        return sig.parameters[argument_name].annotation.__name__
+
 
 class App:
     def __init__(self, __file: str):
         self._mapping: dict[str, Command] = {}
         self._logger = get_logger(__file)
         self._product_info = ProductInfo(__file)
 
@@ -73,17 +79,26 @@
             raise KeyError(msg)
         flags = payload["flags"]
         log_level = flags.pop("log_level")
         if log_level == "disabled":
             log_level = "info"
         databricks_logger = logging.getLogger("databricks")
         databricks_logger.setLevel(log_level.upper())
-        kwargs = {k.replace("-", "_"): v for k, v in flags.items()}
+        kwargs = {k.replace("-", "_"): v for k, v in flags.items() if v != ""}
+        cmd = self._mapping[command]
+        # modify kwargs to match the type of the argument
+        for kwarg in list(kwargs.keys()):
+            match cmd.get_argument_type(kwarg):
+                case "int":
+                    kwargs[kwarg] = int(kwargs[kwarg])
+                case "bool":
+                    kwargs[kwarg] = kwargs[kwarg].lower() == "true"
+                case "float":
+                    kwargs[kwarg] = float(kwargs[kwarg])
         try:
-            cmd = self._mapping[command]
             if cmd.needs_workspace_client():
                 kwargs["w"] = self._workspace_client()
             elif cmd.is_account:
                 kwargs["a"] = self._account_client()
             prompts_argument = cmd.prompts_argument_name()
             if prompts_argument:
                 kwargs[prompts_argument] = Prompts()
```

### Comparing `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/commands.py` & `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/commands.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/entrypoint.py` & `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/entrypoint.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/installation.py` & `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/installation.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/installer.py` & `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/installer.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/limiter.py` & `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/limiter.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/logger.py` & `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/logger.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/parallel.py` & `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/parallel.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/tui.py` & `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/tui.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/upgrades.py` & `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/upgrades.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/wheels.py` & `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/wheels.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.1/.gitignore` & `databricks_labs_blueprint-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.1/LICENSE` & `databricks_labs_blueprint-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.1/README.md` & `databricks_labs_blueprint-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.1/pyproject.toml` & `databricks_labs_blueprint-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.1/PKG-INFO` & `databricks_labs_blueprint-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: databricks-labs-blueprint
-Version: 0.6.1
+Version: 0.6.2
 Summary: Common libraries for Databricks Labs
 Project-URL: Issues, https://github.com/databrickslabs/blueprint/issues
 Project-URL: Source, https://github.com/databrickslabs/blueprint
 License-File: LICENSE
 License-File: NOTICE
 Keywords: Databricks
 Classifier: Development Status :: 3 - Alpha
```

