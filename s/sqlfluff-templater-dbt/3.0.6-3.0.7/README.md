# Comparing `tmp/sqlfluff_templater_dbt-3.0.6.tar.gz` & `tmp/sqlfluff_templater_dbt-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlfluff_templater_dbt-3.0.6.tar", last modified: Mon May  6 19:38:39 2024, max compression
+gzip compressed data, was "sqlfluff_templater_dbt-3.0.7.tar", last modified: Thu May 23 09:39:46 2024, max compression
```

## Comparing `sqlfluff_templater_dbt-3.0.6.tar` & `sqlfluff_templater_dbt-3.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:39.926756 sqlfluff_templater_dbt-3.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-06 19:38:31.000000 sqlfluff_templater_dbt-3.0.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-06 19:38:39.926756 sqlfluff_templater_dbt-3.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-06 19:38:31.000000 sqlfluff_templater_dbt-3.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-06 19:38:39.926756 sqlfluff_templater_dbt-3.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-06 19:38:31.000000 sqlfluff_templater_dbt-3.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:39.922756 sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-06 19:38:31.000000 sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33073 2024-05-06 19:38:31.000000 sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt/templater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:39.926756 sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-06 19:38:39.000000 sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-06 19:38:39.000000 sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:38:39.000000 sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-06 19:38:39.000000 sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-06 19:38:39.000000 sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-06 19:38:39.000000 sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:46.360223 sqlfluff_templater_dbt-3.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-23 09:39:39.000000 sqlfluff_templater_dbt-3.0.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-23 09:39:46.360223 sqlfluff_templater_dbt-3.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-23 09:39:39.000000 sqlfluff_templater_dbt-3.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-23 09:39:46.360223 sqlfluff_templater_dbt-3.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-23 09:39:39.000000 sqlfluff_templater_dbt-3.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:46.356223 sqlfluff_templater_dbt-3.0.7/sqlfluff_templater_dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-23 09:39:39.000000 sqlfluff_templater_dbt-3.0.7/sqlfluff_templater_dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34598 2024-05-23 09:39:39.000000 sqlfluff_templater_dbt-3.0.7/sqlfluff_templater_dbt/templater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:46.356223 sqlfluff_templater_dbt-3.0.7/sqlfluff_templater_dbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-23 09:39:46.000000 sqlfluff_templater_dbt-3.0.7/sqlfluff_templater_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-23 09:39:46.000000 sqlfluff_templater_dbt-3.0.7/sqlfluff_templater_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:39:46.000000 sqlfluff_templater_dbt-3.0.7/sqlfluff_templater_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 09:39:46.000000 sqlfluff_templater_dbt-3.0.7/sqlfluff_templater_dbt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-23 09:39:46.000000 sqlfluff_templater_dbt-3.0.7/sqlfluff_templater_dbt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-23 09:39:46.000000 sqlfluff_templater_dbt-3.0.7/sqlfluff_templater_dbt.egg-info/top_level.txt
```

### Comparing `sqlfluff_templater_dbt-3.0.6/LICENSE.md` & `sqlfluff_templater_dbt-3.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqlfluff_templater_dbt-3.0.6/PKG-INFO` & `sqlfluff_templater_dbt-3.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff-templater-dbt
-Version: 3.0.6
+Version: 3.0.7
 Summary: Lint your dbt project SQL
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
@@ -30,15 +30,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: sqlfluff==3.0.6
+Requires-Dist: sqlfluff==3.0.7
 Requires-Dist: dbt-core>=1.0.0
 Requires-Dist: jinja2-simple-tags>=0.3.1
 Requires-Dist: markupsafe
 Requires-Dist: pydantic
 Requires-Dist: rich
 Requires-Dist: ruamel.yaml
```

### Comparing `sqlfluff_templater_dbt-3.0.6/setup.cfg` & `sqlfluff_templater_dbt-3.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlfluff-templater-dbt
-version = 3.0.6
+version = 3.0.7
 description = Lint your dbt project SQL
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sqlfluff/sqlfluff
 author = Alan Cruickshank
 author_email = alan@designingoverload.com
 license = MIT License
@@ -60,15 +60,15 @@
 	tsql
 	dbt
 
 [options]
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	sqlfluff==3.0.6
+	sqlfluff==3.0.7
 	dbt-core>=1.0.0
 	jinja2-simple-tags>=0.3.1
 	markupsafe
 	pydantic
 	rich
 	ruamel.yaml
```

### Comparing `sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt/templater.py` & `sqlfluff_templater_dbt-3.0.7/sqlfluff_templater_dbt/templater.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,16 @@
     # an empty string pre 1.5.x
     vars: Optional[Union[Dict, str]] = None
     # NOTE: The `which` argument here isn't covered in tests, but many
     # dbt packages assume that it will have been set.
     # https://github.com/sqlfluff/sqlfluff/issues/4861
     # https://github.com/sqlfluff/sqlfluff/issues/4965
     which: Optional[str] = "compile"
+    # NOTE: As of dbt 1.8, the following is required to exist.
+    REQUIRE_RESOURCE_NAMES_WITHOUT_SPACES: Optional[bool] = None
 
 
 class DbtTemplater(JinjaTemplater):
     """A templater using dbt."""
 
     name = "dbt"
     sequential_fail_limit = 3
@@ -143,14 +145,20 @@
     @cached_property
     def dbt_config(self):
         """Loads the dbt config."""
         from dbt import flags
         from dbt.adapters.factory import register_adapter
         from dbt.config.runtime import RuntimeConfig as DbtRuntimeConfig
 
+        if self.dbt_version_tuple >= (1, 8):
+            from dbt_common.clients.system import get_env
+            from dbt_common.context import set_invocation_context
+
+            set_invocation_context(get_env())
+
         # Attempt to silence internal logging at this point.
         # https://github.com/sqlfluff/sqlfluff/issues/5054
         self.try_silence_dbt_logs()
 
         if self.dbt_version_tuple >= (1, 5):
             user_config = None
             # 1.5.x+ this is a dict.
@@ -174,34 +182,40 @@
                 profiles_dir=self.profiles_dir,
                 profile=self._get_profile(),
                 vars=cli_vars,
                 threads=1,
             ),
             user_config,
         )
-        self.dbt_config = DbtRuntimeConfig.from_args(
+        _dbt_config = DbtRuntimeConfig.from_args(
             DbtConfigArgs(
                 project_dir=self.project_dir,
                 profiles_dir=self.profiles_dir,
                 profile=self._get_profile(),
                 target=self._get_target(),
                 vars=cli_vars,
                 threads=1,
             )
         )
-        register_adapter(self.dbt_config)
-        return self.dbt_config
+
+        if self.dbt_version_tuple >= (1, 8):
+            from dbt.mp_context import get_mp_context
+
+            register_adapter(_dbt_config, get_mp_context())
+        else:
+            register_adapter(_dbt_config)
+
+        return _dbt_config
 
     @cached_property
     def dbt_compiler(self):
         """Loads the dbt compiler."""
         from dbt.compilation import Compiler as DbtCompiler
 
-        self.dbt_compiler = DbtCompiler(self.dbt_config)
-        return self.dbt_compiler
+        return DbtCompiler(self.dbt_config)
 
     @cached_property
     def dbt_manifest(self):
         """Loads the dbt manifest."""
         from dbt.exceptions import DbtProjectError
 
         # NOTE: The uninstalled packages error only exists from around
@@ -229,22 +243,22 @@
             # Changing cwd temporarily as dbt is not using project_dir to
             # read/write `target/partial_parse.msgpack`. This can be undone when
             # https://github.com/dbt-labs/dbt-core/issues/6055 is solved.
             # For dbt 1.4+ this isn't necessary, but it is required for 1.3
             # and before.
             if self.dbt_version_tuple < (1, 4):
                 os.chdir(self.project_dir)
-            self.dbt_manifest = ManifestLoader.get_full_manifest(self.dbt_config)
+            _dbt_manifest = ManifestLoader.get_full_manifest(self.dbt_config)
         except summary_errors as err:  # pragma: no cover
             raise SQLFluffUserError(f"{err.__class__.__name__}: {err}")
         finally:
             if self.dbt_version_tuple < (1, 4):
                 os.chdir(old_cwd)
 
-        return self.dbt_manifest
+        return _dbt_manifest
 
     @cached_property
     def dbt_selector_method(self):
         """Loads the dbt selector method."""
         if self.formatter:  # pragma: no cover TODO?
             self.formatter.dispatch_compilation_header(
                 "dbt templater", "Compiling dbt project..."
@@ -256,24 +270,24 @@
         from dbt.graph.selector_methods import (
             MethodName as DbtMethodName,
         )
 
         selector_methods_manager = DbtSelectorMethodManager(
             self.dbt_manifest, previous_state=None
         )
-        self.dbt_selector_method = selector_methods_manager.get_method(
+        _dbt_selector_method = selector_methods_manager.get_method(
             DbtMethodName.Path, method_arguments=[]
         )
 
         if self.formatter:  # pragma: no cover TODO?
             self.formatter.dispatch_compilation_header(
                 "dbt templater", "Project Compiled."
             )
 
-        return self.dbt_selector_method
+        return _dbt_selector_method
 
     def _get_profiles_dir(self):
         """Get the dbt profiles directory from the configuration.
 
         The default is `~/.dbt` but we use the
         default_profiles_dir from the dbt library to
         support a change of default in the future, as well
@@ -455,15 +469,20 @@
         self.project_dir = self._get_project_dir()
         self.profiles_dir = self._get_profiles_dir()
         fname_absolute_path = os.path.abspath(fname) if fname != "stdin" else fname
 
         try:
             # These are the names in dbt-core 1.4.1+
             # https://github.com/dbt-labs/dbt-core/pull/6539
-            from dbt.exceptions import CompilationError, FailedToConnectError
+            from dbt.exceptions import CompilationError
+
+            if self.dbt_version_tuple >= (1, 8):
+                from dbt.adapters.exceptions import FailedToConnectError
+            else:
+                from dbt.exceptions import FailedToConnectError
         except ImportError:
             # These are the historic names for older dbt-core versions
             from dbt.exceptions import CompilationException as CompilationError
             from dbt.exceptions import (
                 FailedToConnectException as FailedToConnectError,
             )
 
@@ -588,14 +607,17 @@
                         env = args[0]
                         globals = args[2] if len(args) >= 3 else kwargs["globals"]
 
                         # Overwrite the outer render_func
                         def render_func(in_str):
                             env.add_extension(SnapshotExtension)
                             template = env.from_string(in_str, globals=globals)
+                            if self.dbt_version_tuple >= (1, 8):
+                                # dbt 1.8 requires a context for rendering the template.
+                                return template.render(globals)
                             return template.render()
 
             return old_from_string(*args, **kwargs)
 
         # NOTE: We need to inject the project root here in reaction to the
         # breaking change upstream with dbt. Coverage works in 1.5.2, but
         # appears to no longer be covered in 1.5.3.
@@ -624,15 +646,18 @@
             if v.config.materialized == "ephemeral"
             and not getattr(v, "compiled", False)
         )
 
         try:
             # These are the names in dbt-core 1.4.1+
             # https://github.com/dbt-labs/dbt-core/pull/6539
-            from dbt.exceptions import UndefinedMacroError
+            if self.dbt_version_tuple >= (1, 8):
+                from dbt_common.exceptions import UndefinedMacroError
+            else:
+                from dbt.exceptions import UndefinedMacroError
         except ImportError:
             # These are the historic names for older dbt-core versions
             from dbt.exceptions import UndefinedMacroException as UndefinedMacroError
 
         with self.connection():
             # Apply the monkeypatch.
             Environment.from_string = from_string
@@ -787,15 +812,24 @@
         # In previous versions, we relied on the functionality removed in
         # https://github.com/dbt-labs/dbt-core/pull/4062.
         adapter = self.adapters.get(self.project_dir)
         if adapter is None:
             adapter = get_adapter(self.dbt_config)
             self.adapters[self.project_dir] = adapter
             adapter.acquire_connection("master")
-            adapter.set_relations_cache(self.dbt_manifest)
+            if self.dbt_version_tuple >= (1, 8):
+                # See notes from https://github.com/dbt-labs/dbt-adapters/discussions/87
+                # about the decoupling of the adapters from core.
+                from dbt.context.providers import generate_runtime_macro_context
+
+                adapter.set_macro_resolver(self.dbt_manifest)
+                adapter.set_macro_context_generator(generate_runtime_macro_context)
+                adapter.set_relations_cache(self.dbt_manifest.nodes.values())
+            else:
+                adapter.set_relations_cache(self.dbt_manifest)
 
         yield
         # :TRICKY: Once connected, we never disconnect. Making multiple
         # connections during linting has proven to cause major performance
         # issues.
```

### Comparing `sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt.egg-info/PKG-INFO` & `sqlfluff_templater_dbt-3.0.7/sqlfluff_templater_dbt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff-templater-dbt
-Version: 3.0.6
+Version: 3.0.7
 Summary: Lint your dbt project SQL
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
@@ -30,15 +30,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: sqlfluff==3.0.6
+Requires-Dist: sqlfluff==3.0.7
 Requires-Dist: dbt-core>=1.0.0
 Requires-Dist: jinja2-simple-tags>=0.3.1
 Requires-Dist: markupsafe
 Requires-Dist: pydantic
 Requires-Dist: rich
 Requires-Dist: ruamel.yaml
```

