# Comparing `tmp/sema4ai_actions-0.7.0.tar.gz` & `tmp/sema4ai_actions-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sema4ai_actions-0.7.0.tar", max compression
+gzip compressed data, was "sema4ai_actions-0.8.0.tar", max compression
```

## Comparing `sema4ai_actions-0.7.0.tar` & `sema4ai_actions-0.8.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     2971 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/README.md
--rw-r--r--   0        0        0      971 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     5508 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/__init__.py
--rw-r--r--   0        0        0       80 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/__main__.py
--rw-r--r--   0        0        0    16339 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_action.py
--rw-r--r--   0        0        0     7567 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_action_context.py
--rw-r--r--   0        0        0    11652 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_args_dispatcher.py
--rw-r--r--   0        0        0     1494 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_callback.py
--rw-r--r--   0        0        0     8339 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_collect_actions.py
--rw-r--r--   0        0        0    33643 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_commands.py
--rw-r--r--   0        0        0     2276 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_config.py
--rw-r--r--   0        0        0      336 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_constants.py
--rw-r--r--   0        0        0        0 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_customization/__init__.py
--rw-r--r--   0        0        0     2722 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_customization/_extension_points.py
--rw-r--r--   0        0        0     9922 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_customization/_plugin_manager.py
--rw-r--r--   0        0        0      220 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_exceptions.py
--rw-r--r--   0        0        0     5638 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_fixtures.py
--rw-r--r--   0        0        0     2500 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_hooks.py
--rw-r--r--   0        0        0     7491 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_interrupts.py
--rw-r--r--   0        0        0     1367 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_lifecycle.py
--rw-r--r--   0        0        0    13368 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_lint_action.py
--rw-r--r--   0        0        0     1082 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_log_auto_setup.py
--rw-r--r--   0        0        0     3074 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_log_output_setup.py
--rw-r--r--   0        0        0     6342 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_managed_parameters.py
--rw-r--r--   0        0        0     6023 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_protocols.py
--rw-r--r--   0        0        0    13813 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_remove_refs.py
--rw-r--r--   0        0        0     2906 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_request.py
--rw-r--r--   0        0        0     1023 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_request_impl.py
--rw-r--r--   0        0        0     6615 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_secret/__init__.py
--rw-r--r--   0        0        0     5153 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_secret/_oauth2_secret.py
--rw-r--r--   0        0        0     2678 2024-05-22 11:54:50.423717 sema4ai_actions-0.7.0/src/sema4ai/actions/_secret/_secret.py
--rw-r--r--   0        0        0     3134 2024-05-22 11:54:50.423717 sema4ai_actions-0.7.0/src/sema4ai/actions/api.py
--rw-r--r--   0        0        0     2277 2024-05-22 11:54:50.423717 sema4ai_actions-0.7.0/src/sema4ai/actions/cli.py
--rw-r--r--   0        0        0        0 2024-05-22 11:54:50.423717 sema4ai_actions-0.7.0/src/sema4ai/actions/py.typed
--rw-r--r--   0        0        0     3788 1970-01-01 00:00:00.000000 sema4ai_actions-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     2971 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/README.md
+-rw-r--r--   0        0        0      877 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     5588 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/__init__.py
+-rw-r--r--   0        0        0       80 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/__main__.py
+-rw-r--r--   0        0        0    16310 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_action.py
+-rw-r--r--   0        0        0     7567 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_action_context.py
+-rw-r--r--   0        0        0    11652 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_args_dispatcher.py
+-rw-r--r--   0        0        0     1494 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_callback.py
+-rw-r--r--   0        0        0     8339 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_collect_actions.py
+-rw-r--r--   0        0        0    35568 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_commands.py
+-rw-r--r--   0        0        0     2276 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_config.py
+-rw-r--r--   0        0        0      331 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_constants.py
+-rw-r--r--   0        0        0        0 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_customization/__init__.py
+-rw-r--r--   0        0        0     2722 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_customization/_extension_points.py
+-rw-r--r--   0        0        0     9922 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_customization/_plugin_manager.py
+-rw-r--r--   0        0        0      220 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_exceptions.py
+-rw-r--r--   0        0        0     5638 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_fixtures.py
+-rw-r--r--   0        0        0     2500 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_hooks.py
+-rw-r--r--   0        0        0     7491 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_interrupts.py
+-rw-r--r--   0        0        0     1367 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_lifecycle.py
+-rw-r--r--   0        0        0    13368 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_lint_action.py
+-rw-r--r--   0        0        0     1082 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_log_auto_setup.py
+-rw-r--r--   0        0        0     3074 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_log_output_setup.py
+-rw-r--r--   0        0        0     6342 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_managed_parameters.py
+-rw-r--r--   0        0        0     6023 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_protocols.py
+-rw-r--r--   0        0        0    13813 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_remove_refs.py
+-rw-r--r--   0        0        0     2906 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_request.py
+-rw-r--r--   0        0        0     1023 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_request_impl.py
+-rw-r--r--   0        0        0     1116 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_response.py
+-rw-r--r--   0        0        0     6615 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_secret/__init__.py
+-rw-r--r--   0        0        0     5153 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_secret/_oauth2_secret.py
+-rw-r--r--   0        0        0     2678 2024-05-23 13:51:24.506319 sema4ai_actions-0.8.0/src/sema4ai/actions/_secret/_secret.py
+-rw-r--r--   0        0        0     3134 2024-05-23 13:51:24.510320 sema4ai_actions-0.8.0/src/sema4ai/actions/api.py
+-rw-r--r--   0        0        0     2277 2024-05-23 13:51:24.510320 sema4ai_actions-0.8.0/src/sema4ai/actions/cli.py
+-rw-r--r--   0        0        0        0 2024-05-23 13:51:24.510320 sema4ai_actions-0.8.0/src/sema4ai/actions/py.typed
+-rw-r--r--   0        0        0     3825 1970-01-01 00:00:00.000000 sema4ai_actions-0.8.0/PKG-INFO
```

### Comparing `sema4ai_actions-0.7.0/README.md` & `sema4ai_actions-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/pyproject.toml` & `sema4ai_actions-0.8.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sema4ai-actions"
-version = "0.7.0"
+version = "0.8.0"
 description = "Sema4AI Actions"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/Sema4AI/actions/"
 license = "Apache-2.0"
@@ -13,22 +13,20 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 cryptography = "^42.0.5"
 robocorp-log = ">=2.4,<3"
 robocorp-truststore= ">=0.8.0"
 psutil = "^5.0"
 docstring_parser_fork = "^0.0.5"
+pydantic = "^2.0" # Required for the `Response[T]`
 
 [tool.poetry.group.dev.dependencies]
 sema4ai-devutils = { path = "../devutils/", develop = true }
 types-psutil = "^5.9"
 
-# We just need it for tests. In runtime duck-typing is used to
-# check for `cls.parse_obj(dict)` and `cls.model_json_schema()`
-pydantic = "^2.6"
 
 
 [tool.mypy]
 mypy_path = "src:tests"
 
 [tool.black]
 skip-string-normalization = false
```

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/__init__.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,17 +34,18 @@
 
 from pathlib import Path
 from typing import Callable, Optional, overload
 
 from ._fixtures import setup, teardown
 from ._protocols import IAction, Status
 from ._request import Request
+from ._response import ActionError, Response
 from ._secret import OAuth2Secret, Secret
 
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 @overload
 def action(func: Callable) -> Callable:
     ...
 
@@ -186,18 +187,20 @@
     """
     from sema4ai.actions import _action
 
     return _action.get_current_action()
 
 
 __all__ = [
+    "ActionError",
     "IAction",
+    "OAuth2Secret",
     "Request",
+    "Response",
     "Secret",
-    "OAuth2Secret",
     "Status",
     "action",
     "action_cache",
     "get_current_action",
     "get_output_dir",
     "session_cache",
     "setup",
```

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_action.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -436,19 +436,20 @@
                     "".join(traceback.format_exception(*action.exc_info)),
                     kind=self.KIND_TRACEBACK,
                 )
 
         if self._print_result and action.status == Status.PASS:
             show("result:", kind=self.KIND_IMPORTANT)
             try:
-                if hasattr(result, "model_dump_json"):
+                dump = result
+                if hasattr(result, "model_dump"):
                     # Support for pydantic
-                    result_as_json_str = result.model_dump_json(indent=4)
-                else:
-                    result_as_json_str = json.dumps(result, indent=4)
+                    dump = result.model_dump()
+
+                result_as_json_str = json.dumps(dump, indent=4)
             except Exception:
                 raise RuntimeError(
                     "The resulting value: {result} cannot be converted to JSON."
                 )
 
             show(
                 result_as_json_str,
```

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_action_context.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_action_context.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_args_dispatcher.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_args_dispatcher.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_callback.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_callback.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_collect_actions.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_collect_actions.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_commands.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,24 @@
 
 class _OsExit(enum.Enum):
     NO = 0
     BEFORE_TEARDOWN = 1
     AFTER_TEARDOWN = 2
 
 
+def _has_response_schema(action: IAction) -> bool:
+    output_schema = action.output_schema
+    if isinstance(output_schema, dict):
+        properties = output_schema.get("properties")
+        if properties and isinstance(properties, dict):
+            if set(properties.keys()) == {"result", "error"}:
+                return True
+    return False
+
+
 def run(
     *,
     output_dir: str,
     path: str,
     action_name: Union[Sequence[str], str, None],
     max_log_files: int = 5,
     max_log_file_size: str = "1MB",
@@ -226,14 +236,16 @@
             in the console (note that even if false it should be also added to the
             `log.html`).
 
     Returns:
         0 if everything went well.
         1 if there was some error running the action.
     """
+    from sema4ai.actions._response import ActionError, Response
+
     # If it's set it'll only consider files under the ROBOT_ROOT to contain user code
     # we leave it unset so that it considers all files under lib or site-packages as
     # lib code and everything else is user code.
     os.environ.pop("ROBOT_ROOT", None)
     import copy
 
     from robocorp.log import ConsoleMessageKind, console, redirect
@@ -438,14 +450,18 @@
                         collect_actions(pm, p, action_names, glob)
                     )
 
                     if not actions:
                         raise ActionsCollectError(
                             f"Did not find any actions in: {path}"
                         )
+                    if len(actions) > 1:
+                        raise ActionsCollectError(
+                            f"Expected a single action to be run. Found: {', '.join(x.name for x in actions)}."
+                        )
                 except Exception as e:
                     run_status = "ERROR"
                     setup_message = str(e)
 
                     log.exception()
                     if not isinstance(e, ActionsCollectError):
                         traceback.print_exc()
@@ -483,21 +499,48 @@
 
                             else:
                                 kwargs = _normalize_arguments(
                                     pm, action, additional_arguments or []
                                 )
 
                             result = action.run(**kwargs)
+
                             action.result = result
                             action.status = Status.PASS
+
+                            if _has_response_schema(action):
+                                if getattr(result, "error", None):
+                                    action.status = Status.FAIL
+                                    action.message = str(result.error)
+
                         except Exception as e:
                             action.status = Status.FAIL
-                            # Make sure we put some message even if str(e) is empty.
-                            action.message = str(e) or f"{e.__class__}"
                             action.exc_info = sys.exc_info()
+
+                            if isinstance(e, ActionError):
+                                # Custom support: if an action raised an
+                                # expected error, provide a custom response
+                                error_msg = (
+                                    str(e)
+                                    or (
+                                        f"Error ({e.__class__.__name__})"  # Maybe it's a subclass?
+                                    )
+                                )
+                                action.message = error_msg
+                            else:
+                                # In this case, as it's unexpected, just show the class
+                                # (we don't show the message because it could contain
+                                # private information and that goes out to the LLM).
+                                action.message = (
+                                    f"Unexpected error ({e.__class__.__name__})"
+                                )
+
+                            if _has_response_schema(action):
+                                action.result = Response(error=action.message)
+
                         finally:
                             with interrupt_on_timeout(
                                 teardown_dump_threads_timeout,
                                 teardown_interrupt_timeout,
                                 "Teardown",
                                 "--teardown-dump-threads-timeout",
                                 "RC_TEARDOWN_DUMP_THREADS_TIMEOUT",
```

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_config.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_config.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_customization/_extension_points.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_customization/_extension_points.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_customization/_plugin_manager.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_customization/_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_fixtures.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_fixtures.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_hooks.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_hooks.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_interrupts.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_interrupts.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_lifecycle.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_lint_action.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_lint_action.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_log_auto_setup.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_log_auto_setup.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_log_output_setup.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_log_output_setup.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_managed_parameters.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_managed_parameters.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_protocols.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_protocols.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_remove_refs.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_remove_refs.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_request.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_request.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_request_impl.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_request_impl.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_secret/__init__.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_secret/_oauth2_secret.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_secret/_oauth2_secret.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/_secret/_secret.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/_secret/_secret.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/api.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/api.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/src/sema4ai/actions/cli.py` & `sema4ai_actions-0.8.0/src/sema4ai/actions/cli.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.7.0/PKG-INFO` & `sema4ai_actions-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: sema4ai-actions
-Version: 0.7.0
+Version: 0.8.0
 Summary: Sema4AI Actions
 Home-page: https://github.com/Sema4AI/actions/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cryptography (>=42.0.5,<43.0.0)
 Requires-Dist: docstring_parser_fork (>=0.0.5,<0.0.6)
 Requires-Dist: psutil (>=5.0,<6.0)
+Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: robocorp-log (>=2.4,<3)
 Requires-Dist: robocorp-truststore (>=0.8.0)
 Project-URL: Repository, https://github.com/Sema4AI/actions/
 Description-Content-Type: text/markdown
 
 # ⚡️ sema4ai-actions
```

