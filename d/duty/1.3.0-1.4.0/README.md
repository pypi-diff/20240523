# Comparing `tmp/duty-1.3.0.tar.gz` & `tmp/duty-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duty-1.3.0.tar", last modified: Sun Apr 28 11:33:30 2024, max compression
+gzip compressed data, was "duty-1.4.0.tar", last modified: Thu May 23 15:38:02 2024, max compression
```

## Comparing `duty-1.3.0.tar` & `duty-1.4.0.tar`

### file list

```diff
@@ -1,29 +1,52 @@
--rw-r--r--   0        0        0      754 2024-04-28 09:16:59.233481 duty-1.3.0/LICENSE
--rw-r--r--   0        0        0     1313 2024-04-28 09:17:01.843375 duty-1.3.0/README.md
--rw-r--r--   0        0        0     1815 2024-04-28 11:33:30.514749 duty-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      144 2024-04-28 09:17:01.843375 duty-1.3.0/src/duty/__init__.py
--rw-r--r--   0        0        0      333 2024-04-28 09:16:59.326811 duty-1.3.0/src/duty/__main__.py
--rw-r--r--   0        0        0     1661 2023-04-10 14:47:07.887091 duty-1.3.0/src/duty/callables/__init__.py
--rw-r--r--   0        0        0      367 2023-04-13 14:11:08.482199 duty-1.3.0/src/duty/callables/_io.py
--rw-r--r--   0        0        0     4699 2023-04-13 14:16:42.639974 duty-1.3.0/src/duty/callables/autoflake.py
--rw-r--r--   0        0        0     7153 2023-04-10 14:49:36.264138 duty-1.3.0/src/duty/callables/black.py
--rw-r--r--   0        0        0     3221 2023-04-10 14:49:09.981212 duty-1.3.0/src/duty/callables/blacken_docs.py
--rw-r--r--   0        0        0    23843 2023-06-26 13:00:14.421342 duty-1.3.0/src/duty/callables/coverage.py
--rw-r--r--   0        0        0     8476 2023-06-26 13:00:14.418009 duty-1.3.0/src/duty/callables/flake8.py
--rw-r--r--   0        0        0     5060 2023-06-26 13:00:14.418009 duty-1.3.0/src/duty/callables/interrogate.py
--rw-r--r--   0        0        0    26437 2023-06-26 13:00:14.424676 duty-1.3.0/src/duty/callables/isort.py
--rw-r--r--   0        0        0     7902 2023-04-10 14:48:43.645095 duty-1.3.0/src/duty/callables/mkdocs.py
--rw-r--r--   0        0        0    19797 2023-07-29 12:54:54.885248 duty-1.3.0/src/duty/callables/mypy.py
--rw-r--r--   0        0        0    18345 2023-07-29 12:54:54.885248 duty-1.3.0/src/duty/callables/pytest.py
--rw-r--r--   0        0        0    13312 2023-10-25 15:48:08.558711 duty-1.3.0/src/duty/callables/ruff.py
--rw-r--r--   0        0        0     2389 2024-01-31 17:21:26.267901 duty-1.3.0/src/duty/callables/safety.py
--rw-r--r--   0        0        0      842 2023-07-29 12:54:54.885248 duty-1.3.0/src/duty/callables/ssort.py
--rw-r--r--   0        0        0     8436 2024-04-28 09:17:01.843375 duty-1.3.0/src/duty/cli.py
--rw-r--r--   0        0        0     6590 2024-01-31 17:20:51.348290 duty-1.3.0/src/duty/collection.py
--rw-r--r--   0        0        0     2985 2024-01-31 17:20:51.331623 duty-1.3.0/src/duty/context.py
--rw-r--r--   0        0        0     2813 2024-04-28 09:16:59.320144 duty-1.3.0/src/duty/debug.py
--rw-r--r--   0        0        0     2986 2024-01-31 17:22:07.087443 duty-1.3.0/src/duty/decorator.py
--rw-r--r--   0        0        0      358 2023-02-17 18:11:31.715248 duty-1.3.0/src/duty/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-28 09:16:59.323478 duty-1.3.0/src/duty/py.typed
--rw-r--r--   0        0        0     8052 2024-04-28 11:21:33.351666 duty-1.3.0/src/duty/validation.py
--rw-r--r--   0        0        0     2837 1970-01-01 00:00:00.000000 duty-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      754 2024-04-28 09:16:59.233481 duty-1.4.0/LICENSE
+-rw-r--r--   0        0        0     1313 2024-04-28 09:17:01.843375 duty-1.4.0/README.md
+-rw-r--r--   0        0        0     1870 2024-05-23 15:38:02.473969 duty-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      144 2024-04-28 09:17:01.843375 duty-1.4.0/src/duty/__init__.py
+-rw-r--r--   0        0        0      333 2024-04-28 09:16:59.326811 duty-1.4.0/src/duty/__main__.py
+-rw-r--r--   0        0        0     1042 2024-05-18 13:44:43.024245 duty-1.4.0/src/duty/callables/__init__.py
+-rw-r--r--   0        0        0      367 2024-05-18 13:27:52.548708 duty-1.4.0/src/duty/callables/_io.py
+-rw-r--r--   0        0        0     4699 2024-05-18 13:27:52.548708 duty-1.4.0/src/duty/callables/autoflake.py
+-rw-r--r--   0        0        0     7153 2024-05-18 13:27:52.565374 duty-1.4.0/src/duty/callables/black.py
+-rw-r--r--   0        0        0     3221 2024-05-18 13:27:52.565374 duty-1.4.0/src/duty/callables/blacken_docs.py
+-rw-r--r--   0        0        0     2150 2024-05-18 13:27:52.582040 duty-1.4.0/src/duty/callables/build.py
+-rw-r--r--   0        0        0    23843 2024-05-18 13:27:52.582040 duty-1.4.0/src/duty/callables/coverage.py
+-rw-r--r--   0        0        0     8476 2024-05-18 13:27:52.608707 duty-1.4.0/src/duty/callables/flake8.py
+-rw-r--r--   0        0        0     7455 2024-05-18 13:27:52.612040 duty-1.4.0/src/duty/callables/git_changelog.py
+-rw-r--r--   0        0        0     7391 2024-05-18 13:27:52.612040 duty-1.4.0/src/duty/callables/griffe.py
+-rw-r--r--   0        0        0     5060 2024-05-18 13:27:52.612040 duty-1.4.0/src/duty/callables/interrogate.py
+-rw-r--r--   0        0        0    26437 2024-05-18 13:27:52.612040 duty-1.4.0/src/duty/callables/isort.py
+-rw-r--r--   0        0        0     7902 2024-05-18 13:27:52.612040 duty-1.4.0/src/duty/callables/mkdocs.py
+-rw-r--r--   0        0        0    19797 2024-05-18 13:27:52.625373 duty-1.4.0/src/duty/callables/mypy.py
+-rw-r--r--   0        0        0    18345 2024-05-18 13:27:52.625373 duty-1.4.0/src/duty/callables/pytest.py
+-rw-r--r--   0        0        0    13312 2024-05-18 13:27:52.638706 duty-1.4.0/src/duty/callables/ruff.py
+-rw-r--r--   0        0        0     2389 2024-05-18 13:27:52.655373 duty-1.4.0/src/duty/callables/safety.py
+-rw-r--r--   0        0        0      842 2024-05-18 13:27:52.655373 duty-1.4.0/src/duty/callables/ssort.py
+-rw-r--r--   0        0        0     9511 2024-05-18 13:27:52.655373 duty-1.4.0/src/duty/callables/twine.py
+-rw-r--r--   0        0        0     8521 2024-05-18 14:49:27.599329 duty-1.4.0/src/duty/cli.py
+-rw-r--r--   0        0        0     6590 2024-01-31 17:20:51.348290 duty-1.4.0/src/duty/collection.py
+-rw-r--r--   0        0        0     3191 2024-05-18 13:04:50.817135 duty-1.4.0/src/duty/context.py
+-rw-r--r--   0        0        0     2813 2024-04-28 09:16:59.320144 duty-1.4.0/src/duty/debug.py
+-rw-r--r--   0        0        0     2986 2024-01-31 17:22:07.087443 duty-1.4.0/src/duty/decorator.py
+-rw-r--r--   0        0        0      358 2023-02-17 18:11:31.715248 duty-1.4.0/src/duty/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-28 09:16:59.323478 duty-1.4.0/src/duty/py.typed
+-rw-r--r--   0        0        0     1179 2024-05-18 13:55:14.593456 duty-1.4.0/src/duty/tools/__init__.py
+-rw-r--r--   0        0        0     5285 2024-05-18 13:48:25.208664 duty-1.4.0/src/duty/tools/_autoflake.py
+-rw-r--r--   0        0        0     1474 2024-05-19 10:05:51.166617 duty-1.4.0/src/duty/tools/_base.py
+-rw-r--r--   0        0        0     7907 2024-05-18 13:48:31.915175 duty-1.4.0/src/duty/tools/_black.py
+-rw-r--r--   0        0        0     4632 2024-05-18 13:48:36.901727 duty-1.4.0/src/duty/tools/_blacken_docs.py
+-rw-r--r--   0        0        0     2567 2024-05-18 13:48:42.304936 duty-1.4.0/src/duty/tools/_build.py
+-rw-r--r--   0        0        0    26341 2024-05-18 13:48:47.154824 duty-1.4.0/src/duty/tools/_coverage.py
+-rw-r--r--   0        0        0     9371 2024-05-18 13:49:00.247859 duty-1.4.0/src/duty/tools/_flake8.py
+-rw-r--r--   0        0        0     8247 2024-05-18 13:49:03.521118 duty-1.4.0/src/duty/tools/_git_changelog.py
+-rw-r--r--   0        0        0     7944 2024-05-18 13:49:03.521118 duty-1.4.0/src/duty/tools/_griffe.py
+-rw-r--r--   0        0        0     5730 2024-05-18 13:49:03.764446 duty-1.4.0/src/duty/tools/_interrogate.py
+-rw-r--r--   0        0        0    28352 2024-05-18 13:49:03.764446 duty-1.4.0/src/duty/tools/_isort.py
+-rw-r--r--   0        0        0     9027 2024-05-19 10:58:47.425006 duty-1.4.0/src/duty/tools/_mkdocs.py
+-rw-r--r--   0        0        0    21555 2024-05-18 13:49:03.764446 duty-1.4.0/src/duty/tools/_mypy.py
+-rw-r--r--   0        0        0    20064 2024-05-18 13:49:03.764446 duty-1.4.0/src/duty/tools/_pytest.py
+-rw-r--r--   0        0        0    15226 2024-05-18 13:49:03.521118 duty-1.4.0/src/duty/tools/_ruff.py
+-rw-r--r--   0        0        0     3141 2024-05-18 13:49:03.764446 duty-1.4.0/src/duty/tools/_safety.py
+-rw-r--r--   0        0        0     1097 2024-05-18 13:49:03.521118 duty-1.4.0/src/duty/tools/_ssort.py
+-rw-r--r--   0        0        0    10347 2024-05-18 13:49:03.764446 duty-1.4.0/src/duty/tools/_twine.py
+-rw-r--r--   0        0        0     8052 2024-04-28 11:21:33.351666 duty-1.4.0/src/duty/validation.py
+-rw-r--r--   0        0        0     2900 1970-01-01 00:00:00.000000 duty-1.4.0/PKG-INFO
```

### Comparing `duty-1.3.0/LICENSE` & `duty-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `duty-1.3.0/README.md` & `duty-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `duty-1.3.0/pyproject.toml` & `duty-1.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -35,16 +35,17 @@
     "Topic :: Software Development",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = [
     "eval-type-backport; python_version < '3.10'",
     "failprint>=0.11,!=1.0.0",
+    "typing-extensions>=4.0; python_version < '3.11'",
 ]
-version = "1.3.0"
+version = "1.4.0"
 
 [project.license]
 text = "ISC"
 
 [project.urls]
 Homepage = "https://pawamoy.github.io/duty"
 Documentation = "https://pawamoy.github.io/duty"
```

### Comparing `duty-1.3.0/src/duty/callables/autoflake.py` & `duty-1.4.0/src/duty/callables/autoflake.py`

 * *Files identical despite different names*

### Comparing `duty-1.3.0/src/duty/callables/black.py` & `duty-1.4.0/src/duty/callables/black.py`

 * *Files identical despite different names*

### Comparing `duty-1.3.0/src/duty/callables/blacken_docs.py` & `duty-1.4.0/src/duty/callables/blacken_docs.py`

 * *Files identical despite different names*

### Comparing `duty-1.3.0/src/duty/callables/coverage.py` & `duty-1.4.0/src/duty/callables/coverage.py`

 * *Files identical despite different names*

### Comparing `duty-1.3.0/src/duty/callables/flake8.py` & `duty-1.4.0/src/duty/callables/flake8.py`

 * *Files identical despite different names*

### Comparing `duty-1.3.0/src/duty/callables/interrogate.py` & `duty-1.4.0/src/duty/callables/interrogate.py`

 * *Files identical despite different names*

### Comparing `duty-1.3.0/src/duty/callables/isort.py` & `duty-1.4.0/src/duty/callables/isort.py`

 * *Files identical despite different names*

### Comparing `duty-1.3.0/src/duty/callables/mkdocs.py` & `duty-1.4.0/src/duty/callables/mkdocs.py`

 * *Files identical despite different names*

### Comparing `duty-1.3.0/src/duty/callables/mypy.py` & `duty-1.4.0/src/duty/callables/mypy.py`

 * *Files identical despite different names*

### Comparing `duty-1.3.0/src/duty/callables/pytest.py` & `duty-1.4.0/src/duty/callables/pytest.py`

 * *Files identical despite different names*

### Comparing `duty-1.3.0/src/duty/callables/ruff.py` & `duty-1.4.0/src/duty/callables/ruff.py`

 * *Files identical despite different names*

### Comparing `duty-1.3.0/src/duty/callables/safety.py` & `duty-1.4.0/src/duty/callables/safety.py`

 * *Files identical despite different names*

### Comparing `duty-1.3.0/src/duty/callables/ssort.py` & `duty-1.4.0/src/duty/callables/ssort.py`

 * *Files identical despite different names*

### Comparing `duty-1.3.0/src/duty/cli.py` & `duty-1.4.0/src/duty/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,16 @@
             - its positional arguments
             - its keyword arguments
     """
     commands = []
     for arg_list in arg_lists:
         duty = collection.get(arg_list[0])
         opts, remainder = parse_options(duty, arg_list[1:])
+        if remainder and remainder[0] == "--":
+            remainder = remainder[1:]
         duty.options_override = {**global_opts, **opts}
         commands.append((duty, *parse_args(duty, remainder)))
     return commands
 
 
 def print_help(parser: ArgParser, opts: argparse.Namespace, collection: Collection) -> None:
     """Print general help or duties help.
```

### Comparing `duty-1.3.0/src/duty/collection.py` & `duty-1.4.0/src/duty/collection.py`

 * *Files identical despite different names*

### Comparing `duty-1.3.0/src/duty/context.py` & `duty-1.4.0/src/duty/context.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Module containing the context definition."""
 
 from __future__ import annotations
 
 import os
-from contextlib import contextmanager
+from contextlib import contextmanager, suppress
 from typing import Any, Callable, Iterator, List, Union
 
 from failprint.runners import run as failprint_run
 
 from duty.exceptions import DutyFailure
+from duty.tools import Tool
 
 CmdType = Union[str, List[str], Callable]
 
 
 class Context:
     """A simple context class.
 
@@ -63,14 +64,18 @@
 
         Returns:
             The output of the command.
         """
         final_options = dict(self._options)
         final_options.update(options)
 
+        if "command" not in final_options and isinstance(cmd, Tool):
+            with suppress(ValueError):
+                final_options["command"] = cmd.cli_command
+
         allow_overrides = final_options.pop("allow_overrides", True)
         workdir = final_options.pop("workdir", None)
 
         if allow_overrides:
             final_options.update(self._options_override)
 
         with self.cd(workdir):
```

### Comparing `duty-1.3.0/src/duty/debug.py` & `duty-1.4.0/src/duty/debug.py`

 * *Files identical despite different names*

### Comparing `duty-1.3.0/src/duty/decorator.py` & `duty-1.4.0/src/duty/decorator.py`

 * *Files identical despite different names*

### Comparing `duty-1.3.0/src/duty/validation.py` & `duty-1.4.0/src/duty/validation.py`

 * *Files identical despite different names*

### Comparing `duty-1.3.0/PKG-INFO` & `duty-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duty
-Version: 1.3.0
+Version: 1.4.0
 Summary: A simple task runner.
 Keywords: task-runner,task,runner,cross-platform
 Author-Email: =?utf-8?q?Timoth=C3=A9e_Mazzucotelli?= <dev@pawamoy.fr>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -27,14 +27,15 @@
 Project-URL: Issues, https://github.com/pawamoy/duty/issues
 Project-URL: Discussions, https://github.com/pawamoy/duty/discussions
 Project-URL: Gitter, https://gitter.im/duty/community
 Project-URL: Funding, https://github.com/sponsors/pawamoy
 Requires-Python: >=3.8
 Requires-Dist: eval-type-backport; python_version < "3.10"
 Requires-Dist: failprint!=1.0.0,>=0.11
+Requires-Dist: typing-extensions>=4.0; python_version < "3.11"
 Description-Content-Type: text/markdown
 
 # duty
 
 [![ci](https://github.com/pawamoy/duty/workflows/ci/badge.svg)](https://github.com/pawamoy/duty/actions?query=workflow%3Aci)
 [![documentation](https://img.shields.io/badge/docs-mkdocs-708FCC.svg?style=flat)](https://pawamoy.github.io/duty/)
 [![pypi version](https://img.shields.io/pypi/v/duty.svg)](https://pypi.org/project/duty/)
```

