# Comparing `tmp/printlinter-0.1.0.tar.gz` & `tmp/printlinter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "printlinter-0.1.0.tar", max compression
+gzip compressed data, was "printlinter-0.2.0.tar", max compression
```

## Comparing `printlinter-0.1.0.tar` & `printlinter-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    13863 2024-03-28 14:12:51.695198 printlinter-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     9145 2024-03-28 15:12:49.350804 printlinter-0.1.0/README.md
--rw-r--r--   0        0        0       91 2024-03-28 14:12:51.695198 printlinter-0.1.0/cli_app/__init__.py
--rw-r--r--   0        0        0      102 2024-03-28 15:12:49.350804 printlinter-0.1.0/cli_app/__main__.py
--rw-r--r--   0        0        0     4909 2024-03-28 15:12:49.350804 printlinter-0.1.0/cli_app/cli.py
--rw-r--r--   0        0        0      365 2024-03-28 15:12:49.350804 printlinter-0.1.0/cli_app/main.py
--rw-r--r--   0        0        0      497 2024-03-28 15:12:49.350804 printlinter-0.1.0/printlinter/__init__.py
--rw-r--r--   0        0        0     2074 2024-03-28 15:12:49.350804 printlinter-0.1.0/printlinter/classes.py
--rw-r--r--   0        0        0     5672 2024-03-28 15:12:49.350804 printlinter-0.1.0/printlinter/config.py
--rw-r--r--   0        0        0     2216 2024-03-28 15:12:49.350804 printlinter-0.1.0/printlinter/ignored_processing.py
--rw-r--r--   0        0        0     3587 2024-03-28 15:12:49.350804 printlinter-0.1.0/printlinter/parser.py
--rw-r--r--   0        0        0     6106 2024-03-28 15:12:49.354804 printlinter-0.1.0/printlinter/visitor.py
--rw-r--r--   0        0        0     4324 2024-03-28 15:12:49.354804 printlinter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10280 1970-01-01 00:00:00.000000 printlinter-0.1.0/setup.py
--rw-r--r--   0        0        0     9751 1970-01-01 00:00:00.000000 printlinter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    13863 2024-05-07 10:56:33.689472 printlinter-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0    12066 2024-05-23 14:19:24.451794 printlinter-0.2.0/README.md
+-rw-r--r--   0        0        0       91 2024-05-07 10:56:33.689472 printlinter-0.2.0/cli_app/__init__.py
+-rw-r--r--   0        0        0      102 2024-05-07 10:56:33.689472 printlinter-0.2.0/cli_app/__main__.py
+-rw-r--r--   0        0        0     5958 2024-05-23 14:19:24.451794 printlinter-0.2.0/cli_app/cli.py
+-rw-r--r--   0        0        0      365 2024-05-07 10:56:33.689472 printlinter-0.2.0/cli_app/main.py
+-rw-r--r--   0        0        0      586 2024-05-23 14:19:24.455793 printlinter-0.2.0/printlinter/__init__.py
+-rw-r--r--   0        0        0     3178 2024-05-23 14:19:24.455793 printlinter-0.2.0/printlinter/classes.py
+-rw-r--r--   0        0        0     7048 2024-05-23 14:19:24.455793 printlinter-0.2.0/printlinter/config.py
+-rw-r--r--   0        0        0     2989 2024-05-23 14:19:24.455793 printlinter-0.2.0/printlinter/ignored_processing.py
+-rw-r--r--   0        0        0     6293 2024-05-23 14:19:24.455793 printlinter-0.2.0/printlinter/parser.py
+-rw-r--r--   0        0        0     6107 2024-05-23 14:19:24.455793 printlinter-0.2.0/printlinter/visitor.py
+-rw-r--r--   0        0        0     4105 2024-05-23 14:19:24.455793 printlinter-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    13344 1970-01-01 00:00:00.000000 printlinter-0.2.0/setup.py
+-rw-r--r--   0        0        0    12672 1970-01-01 00:00:00.000000 printlinter-0.2.0/PKG-INFO
```

### Comparing `printlinter-0.1.0/LICENSE.md` & `printlinter-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `printlinter-0.1.0/README.md` & `printlinter-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!-- markdownlint-disable-file MD041 -->
 
-<!-- TODO: Add badge
-TODO: logo -->
+<!-- TODO: Add badge -->
+![logo](logo.png)
 
 [English readme](README.md) **·** [Français readme](doc/readme/README.fr.md)
 
 PrintLinter is a python linter to detect and signals display functions in python code.
 
 ## Summary
 
@@ -15,23 +15,30 @@
     - [Lint](#lint)
       - [Example](#example)
 - [Error codes](#error-codes)
   - [Standard library](#standard-library)
 - [Ignore errors](#ignore-errors)
   - [Ignore error inline](#ignore-error-inline)
     - [Examples](#examples)
-  - [Ignore a whole file](#ignore-a-whole-file)
+  - [Ignore error on the next line](#ignore-error-on-the-next-line)
     - [Examples](#examples-1)
+  - [Ignore a whole file](#ignore-a-whole-file)
+    - [Examples](#examples-2)
       - [Simple error](#simple-error)
       - [library errors](#library-errors)
       - [All errors](#all-errors)
+  - [Ignore a block of code](#ignore-a-block-of-code)
+    - [Examples](#examples-3)
+      - [Simple error](#simple-error-1)
+      - [All errors](#all-errors-1)
 - [Configuration](#configuration)
   - [Target version](#target-version)
   - [Ignored files](#ignored-files)
   - [Disabled rules](#disabled-rules)
+  - [Color](#color)
   - [Examples of configuration files](#examples-of-configuration-files)
     - [Yaml/Yml configuration file](#yamlyml-configuration-file)
     - [Json configuration file](#json-configuration-file)
     - [Toml configuration file](#toml-configuration-file)
     - [Pyproject configuration file](#pyproject-configuration-file)
 - [But then](#but-then)
 
@@ -67,14 +74,51 @@
 printlinter lint <file|folder>
 ```
 
 The product output look like this.
 
 `file_path:line:column error_code display_function_detected error_name`
 
+By default we disable the linter in some folders.
+
+- `node_modules`
+- `.vscode/`
+- `__pycache__/`
+- `build/`
+- `develop-eggs/`
+- `dist/`
+- `downloads/`
+- `eggs/`
+- `.eggs/`
+- `lib/`
+- `lib64/`
+- `parts/`
+- `sdist/`
+- `var/`
+- `wheels/`
+- `pip-wheel-metadata/`
+- `share/python-wheels/`
+- `htmlcov/`
+- `.tox/`
+- `.nox/`
+- `.hypothesis/`
+- `.pytest_cache/`
+- `docs/_build/`
+- `__pypackages__/`
+- `.mypy_cache/`
+- `.ruff_cache`
+- `.pyre/`
+- `env/`
+- `venv/`
+- `ENV/`
+- `env.bak/`
+- `venv.bak/`
+- `.venv/`
+- `.env/`
+
 #### Example
 
 <!-- markdownlint-disable MD013 -->
 ```sh
 tests/testing_files/mixed/mixed0.py:5:0: PPL001 `print("toto")` print-detected
 tests/testing_files/mixed/mixed0.py:6:0: PPL002 `pprint("titi")` prettyprint-detected
 tests/testing_files/mixed/mixed1/mixed2.py:5:0: PPL001 `print("toto")` print-detected
@@ -143,65 +187,153 @@
 
 ```python
 toto = 1
 titi = 2
 print (toto + titi) # noqa: PPL001
 ```
 
+## Ignore error on the next line
+
+To ignore a rule on the next line, add a comment at the line before code to ignore.
+`<printlinter disable-next (error_code)>`.
+
+<!-- markdownlint-disable-next-line MD024 -->
+### Examples
+
+```python
+toto = 1
+titi = 2
+# <printlinter disable-next PPL001>
+print (toto + titi) # ignored error
+```
+
 ## Ignore a whole file
 
 To ignore a rule, library rules or all rules, add a comment at the beging of the file.
-`# <py-printlinter disable-file <error_code>`.
+`# <printlinter disable-file (error_code)>`.
 
 <!-- markdownlint-disable-next-line MD036 -->
 **The comment must be before any code in a file.**
 
 <!-- markdownlint-disable-next-line MD024 -->
 ### Examples
 
 #### Simple error
 
 ```python
-# <py-printlinter disable-file PPL002>
+# <printlinter disable-file PPL002>
 from pprint import pprint
 toto = 1
 titi = 2
 pprint(titi + toto)  # ignored error
 ...
 ```
 
 #### library errors
 
 ```python
-# <py-printlinter disable-file PPL000>
+# <printlinter disable-file PPL000>
 import sys
 toto = 1
 titi = 2
 print(titi + toto)  # ignored error
 sys.stdout.write(titi + toto)  # ignored error
 ...
 ```
 
 #### All errors
 
 ```python
-# <py-printlinter disable-file ALL>
+# <printlinter disable-file ALL>
 from sys import stdout, stderr
 from pprint import pprint
 toto = 1
 titi = 2
 print(titi + toto)  # ignored error
 pprint(titi + toto)  # ignored error
 stdout.write(titi + toto)  # ignored error
 stderr.write(titi + toto)  # ignored error
 stdout.writelines(titi + toto)  # ignored error
 stderr.writelines(titi + toto)  # ignored error
 ...
 ```
 
+## Ignore a block of code
+
+To ignore a block of code (disable the linter) on a rules or all rules (disable library
+rules come later), add a comment before the block you want ignore:
+`<printlinter disable (error_code)`. To re enable the linter add an other comment after
+the block of code: `<printlinter enable (error_code)>`. You are don't have to re enable
+the linter after disabled it.
+
+<!-- markdownlint-disable-next-line MD024 -->
+### Examples
+
+<!-- markdownlint-disable-next-line MD024 -->
+#### Simple error
+
+```python
+from pprint import pprint
+# <printlinter disable PPL001>
+print("toto") # ignored error
+pprint("titit")
+# <printlinter enable PPL001>
+...
+```
+
+You can nested ignored block.
+
+```python
+from pprint import pprint
+
+# <printlinter disable PPL002>
+
+pprint("titi") # ignored error
+
+# <printlinter disable PPL001>
+print("toto") # ignored error
+# <printlinter enable PPL001>
+
+print("tutu") # NOT IGNORED ERROR
+pprint("tata") # ignored error
+
+# <printlinter enable PPL002>
+...
+```
+
+without re enable the linter.
+
+```python
+from pprint import pprint
+# <printlinter disable PPL001>
+print("toto") # ignored error
+pprint("titit")
+...
+print('toto') # ignored error
+```
+
+<!-- markdownlint-disable-next-line MD024 -->
+#### All errors
+
+```python
+from sys import stdout, stderr
+from pprint import pprint
+toto = 1
+titi = 2
+# <printlinter disable ALL>
+print(titi + toto)  # ignored error
+pprint(titi + toto)  # ignored error
+stdout.write(titi + toto)  # ignored error
+stderr.write(titi + toto)  # ignored error
+stdout.writelines(titi + toto)  # ignored error
+stderr.writelines(titi + toto)  # ignored error
+# <printlinter enable ALL>
+...
+```
+
 # Configuration
 
 You can configurate the linter with a configuration file (configuration by command line,
 will arrive in a future version).
 
 PrintLinter supports 3 differents file type.
 
@@ -243,59 +375,67 @@
 
 ## Disabled rules
 
 The config file allows to disable rules, in all files and folders.
 
 You can see examples of this config [here](#examples-of-configuration-files).
 
+## Color
+
+The config file allows to enable or disable colorized output. By default the `color` option
+is on `True`.
+
+You can see examples of this config [here](#examples-of-configuration-files).
+
 ## Examples of configuration files
 
 ### Yaml/Yml configuration file
 
 ```yaml
 printlinter:
   target_version: "3.10"
   ignored_files: [toto.py]
   disabled_rules: [PPL001]
+  color: true
 ```
 
 ### Json configuration file
 
 ```json
 {
   "printlinter": {
     "target_version": "3.10",
     "ignored_files": ["toto.py"],
-    "disabled_rules": ["PPL001"]
+    "disabled_rules": ["PPL001"],
+    "color": false
   }
 }
 
 ```
 
 ### Toml configuration file
 
 ```toml
 [printlinter]
 target_version = "3.10"
 ignored_files = ["toto.py"]
 disabled_rules = ["PPL001"]
+color = true
 ```
 
 ### Pyproject configuration file
 
 ```toml
 [tool.printlinter]
 target_version = "3.10"
 ignored_files = ["toto.py"]
 disabled_rules = ["PPL001"]
+color = false
 ```
 
 # But then
 
 Too see the next features to be developed see [TODO](TODO.md). Here's a small,
 non-exhaustive list of what's comming in the future versions.
 
-- Ignore a code block in a file.
-- Ignore the next line.
 - Lint display functions from other libraries.
 - Add other configuration options.
-- Add translation in other languages
```

### Comparing `printlinter-0.1.0/cli_app/cli.py` & `printlinter-0.2.0/cli_app/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,172 +2,206 @@
 
 # Standard imports
 from pathlib import Path
 
 # Third party imports
 import typer
 from rich.console import Console
+from rich.progress import track
 
 # First party imports
 from printlinter import Config
 from printlinter import __app_name__ as ppl_app_name
 from printlinter import __version__ as ppl_version
-from printlinter import contains_print, enumerate_file, get_not_ignore_issue, parse_file
+from printlinter import (
+    contains_print,
+    enumerate_file,
+    get_not_ignored_issue,
+    parse_file,
+)
 
 APP = typer.Typer(help="Print linter", rich_markup_mode="rich")
 
-CONSOLE = Console()
 
-
-def version_callback(value: bool) -> None:
-    """
-    Get the version, display the version if `--version` was used.
-
-    Args:
-        value: Boolean to known if we display the version or not.
-    """
-    if value:
-        CONSOLE.print(f"{ppl_app_name} v.{ppl_version}")
-        raise typer.Exit()
-
-
-def path_callback(path: Path) -> Path:
+def _path_callback(path: Path) -> Path:
     """
     Check if the path exist and if it's a directory.
 
     Args:
         path: Path to check.
 
     Raises:
         FileNotFoundError: If the path does not exist.
         NotADirectoryError: If the given path is not a directory.
 
     Examples:
-        >>> path_callback(Path("printlinter"))
+        >>> _path_callback(Path("printlinter"))
         PosixPath('printlinter')
 
         >>> try:
-        ...     path_callback(Path("azert.qwerty"))
+        ...     _path_callback(Path("azert.qwerty"))
         ... except(FileNotFoundError):
         ...     False
         False
 
         >>> try:
-        ...     path_callback(Path("README.md"))
+        ...     _path_callback(Path("README.md"))
         ... except(TypeError):
         ...     False
         False
     """
     if not path.exists():
         raise FileNotFoundError(f"The path: {path} does not exist")
     if not path.is_dir() and path.suffix != ".py":
         raise TypeError(f"The given file {path} must be a python file (.py)")
     return path
 
 
-def is_a_file(file_name: Path) -> Path | None:
+def _is_a_file(file_name: Path) -> Path | None:
     """
     Check if given path is a file.
 
     If the path is the default path (`Path(".")`) return None.
 
     Args:
         file_name: Path to check.
 
     Returns:
         The given path or None if given path is the default path (`Path(".")`).
 
     Examples:
-        >>> is_a_file(Path("."))
+        >>> _is_a_file(Path("."))
         None
 
-        >>> is_a_file(Path("README.md"))
+        >>> _is_a_file(Path("README.md"))
         PosixPath('README.md')
 
         >>> try:
-        ...     is_a_file(Path("printlinter"))
+        ...     _is_a_file(Path("printlinter"))
         ... except FileNotFoundError:
         ...     False
         False
     """
     if file_name == Path("."):
         return None
     if file_name.is_dir() or not file_name.is_file():
         raise FileNotFoundError(f"The path: {file_name} is not a file")
     return file_name
 
 
+def _is_ignored_rep(ignored_rep: list[Path], path: Path) -> bool:
+    """
+    Check if given path is in an ignored repository.
+
+    Args:
+        ignored_rep: All ignored repositories
+        path: Path to check.
+
+    Returns:
+        True if path is in an ignored repository, False otherwise.
+    """
+    for rep in ignored_rep:
+        if all(part in path.parts for part in rep.parts):
+            return True
+
+    return False
+
+
+def version_callback(value: bool) -> None:
+    """
+    Get the version, display the version if `--version` was used.
+
+    Args:
+        value: Boolean to known if we display the version or not.
+    """
+    config = Config()
+    console = Console(color_system="auto" if config.color else None)
+    if value:
+        console.print(f"{ppl_app_name} v.{ppl_version}")
+        raise typer.Exit()
+
+
 @APP.command(name="lint", help="lint the code to find print")
 def lint(
     path: Path = typer.Argument(
         Path("."),
         help="Path to lint",
         show_default=False,
-        callback=path_callback,
+        callback=_path_callback,
     ),
     config_file: Path = typer.Option(
         Path("."),
         help="Configuration file",
         show_default=False,
-        callback=is_a_file,
+        callback=_is_a_file,
     ),
 ) -> None:
     """
     Lint the given path or default path: `.`.
 
     Args:
         path: Path to lint.
         config_file: Optional config file.
     """
     warning = False
     config = Config(config_file)
+    console = Console(color_system="auto" if config.color else None)
 
     if path.is_dir():
         files_path = enumerate_file(path)
     else:
         files_path = [path]
 
     all_ignored_lines = []
     all_ignored_files = []
+    all_ignored_blocks = []
     issues = []
-    for file_path in files_path:
-        if file_path.absolute() in [
-            Path(path).absolute() for path in config.ignored_files
-        ]:
+    for file_path in track(files_path, description="Processing..."):
+        if (
+            file_path.absolute()
+            in [Path(path).absolute() for path in config.ignored_files]
+        ) or _is_ignored_rep(config.ignored_rep, file_path):
             continue
 
-        tree, ignored_lines, ignored_files = parse_file(
+        tree, ignored_lines, ignored_files, ignored_blocks = parse_file(
             file_path.as_posix(), config.target_version
         )
         issues = contains_print(file_path, tree)
         all_ignored_lines.extend(ignored_lines)
 
         if ignored_files is None:
             warning = True
-            CONSOLE.print(
+            console.print(
                 f"[bold][orange3]Warning ⚠️ [/orange3] {file_path}[/bold]: The ignore "
                 "file comment must be before code and docstring, we skip this ignore "
                 "comment. The file will be lint as if the file were not ignored."
             )
         else:
             all_ignored_files.extend(ignored_files)
 
-    not_ignored_issues = get_not_ignore_issue(
+        all_ignored_blocks.extend(ignored_blocks)
+
+    not_ignored_issues = get_not_ignored_issue(
         issues,
         all_ignored_lines,
         all_ignored_files,
+        all_ignored_blocks,
         config.disabled_rules,
     )
 
+    # TODO: pass ignored value of issue at true when it is ignored. it's usful to get a
+    # list of ignred issues.
+    # console.print(f"[bold]ISSUES:\n{issues}\n[/bold]") # noqa: ERA001
+
     if warning:
         print()
     for issue in not_ignored_issues:
-        CONSOLE.print(str(issue))
+        console.print(str(issue))
 
-    CONSOLE.print(f"Found [bold red]{len(not_ignored_issues)}[/bold red] errors")
+    console.print(f"Found [bold red]{len(not_ignored_issues)}[/bold red] errors")
 
 
 @APP.callback()
 def main(
     _version: bool = typer.Option(
         False,
         "--version",
```

### Comparing `printlinter-0.1.0/printlinter/classes.py` & `printlinter-0.2.0/printlinter/classes.py`

 * *Files 27% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 
     line_as_str: str | None
     "String representation of the line."
 
     from_file: Path | None
     "File who contain the line with the issue."
 
-    ignore: bool
-    "If this issue is ignore or not."
+    ignored: bool
+    "If this issue is ignored or not."
 
     def __str__(self) -> str:
         """
         Get issue as string.
 
         Returns:
             The string representation of the issue.
@@ -57,29 +57,76 @@
             f"[bold]{self.from_file}[/bold]:{self.num_line}:{self.num_col}: "
             f"[bold red]{self.issue.err_code}[/bold red] [bold]`[/bold]"
             f"{self.line_as_str}[bold]`[/bold] {self.issue.name}"
         )
 
 
 @dataclass
-class IgnoreLine:
-    """Ignore line class."""
+class IgnoredLine:
+    """Ignored line class."""
 
     line_num: int
     "Line number of the ignored line."
 
     error_code: str
-    "Code of the ignore issue."
+    "Code of the ignored issue."
 
     from_file: Path | None
     "File who contains the ignored line."
 
 
 @dataclass
-class IgnoreFile:
-    """Ignore file class."""
+class IgnoredFile:
+    """Ignored file class."""
 
     error_code: str
-    "Code of the ignore issue."
+    "Code of the ignored issue."
 
     from_file: Path | None
     "File who contains the ignored line."
+
+
+@dataclass
+class IgnoredBlock:
+    """Ignored block of code class."""
+
+    error_code: str
+    "Code of the ignored issue."
+
+    line_from: int
+    "Begin of ignored block."
+
+    line_to: int
+    "End of ignored block."
+
+    from_file: Path | None
+    "File who contains the ignored line."
+
+    def __init__(
+        self,
+        error_code: str,
+        line_from: int,
+        line_to: int,
+        from_file: Path | None,
+    ) -> None:
+        """
+        Initialize an IngoredBlock class.
+
+        Args:
+            error_code: Given error code.
+            line_from: Given line from.
+            line_to: Given line to.
+            from_file: Given from file.
+
+        Raise:
+            ValueError: If `g_line_from` <= `g_line_to`.
+        """
+        if line_to <= line_from:
+            raise ValueError(
+                f"Given line to ({line_to}) must be strictly greater then given line "
+                f"from ({line_from})"
+            )
+
+        self.error_code = error_code
+        self.line_from = line_from
+        self.line_to = line_to
+        self.from_file = from_file
```

### Comparing `printlinter-0.1.0/printlinter/ignored_processing.py` & `printlinter-0.2.0/printlinter/ignored_processing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Processing ingoed lines functions."""
 
 # Local imports
-from .classes import IgnoreFile, IgnoreLine, IssueInfo
+from .classes import IgnoredBlock, IgnoredFile, IgnoredLine, IssueInfo
 
 FAMILIRY_ERR_CODE = [
     "PPL000",
     "PPL100",
     "PPL200",
     "PPL300",
     "PPL400",
@@ -13,72 +13,92 @@
     "PPL600",
     "PPL700",
     "PPL800",
     "PPL900",
 ]
 
 
-def get_not_ignore_issue(
+def get_not_ignored_issue(
     issues: list[IssueInfo],
-    ignore_lines: list[IgnoreLine],
-    ignore_files: list[IgnoreFile],
+    ignored_lines: list[IgnoredLine],
+    ignored_files: list[IgnoredFile],
+    ignored_blocks: list[IgnoredBlock],
     disabled_rules: list[str],
 ) -> list[IssueInfo]:
     """
     Get all not ignored issues.
 
     Args:
         issues: All issue found.
-        ignore_lines: All ignored lines.
-        ignore_files: All ignored files.
+        ignored_lines: All ignored lines.
+        ignored_files: All ignored files.
+        ignored_blocks: All ignored blocks of code.
         disabled_rules: All disabled rules.
 
     Returns:
         All lines are not ignored.
     """
     result = []
 
     for issue in issues:
         if issue.issue.err_code in disabled_rules:
             continue
 
-        ignore_all_file_equivalence = IgnoreFile(
+        ignored_all_file_equivalence = IgnoredFile(
             error_code="ALL",
             from_file=issue.from_file,
         )
-        if ignore_all_file_equivalence in ignore_files:
+        if ignored_all_file_equivalence in ignored_files:
             continue
 
         # Ignore a file with a family of code (like PPL000, PPL100, ...)
         for index in range(len(FAMILIRY_ERR_CODE) - 1):
             err_code_min = FAMILIRY_ERR_CODE[index]
             err_code_max = FAMILIRY_ERR_CODE[index + 1]
             if err_code_min < issue.issue.err_code < err_code_max:
                 ignored_err_code = err_code_min
 
-        ignore_family_file_equivalence = IgnoreFile(
+        ignored_family_file_equivalence = IgnoredFile(
             error_code=ignored_err_code,
             from_file=issue.from_file,
         )
-        if ignore_family_file_equivalence in ignore_files:
+        if ignored_family_file_equivalence in ignored_files:
             continue
 
         # Files with specific code (like PPL001, PPL005, ...)
-        ignore_file_equivalence = IgnoreFile(
+        ignored_file_equivalence = IgnoredFile(
             error_code=issue.issue.err_code,
             from_file=issue.from_file,
         )
-        if ignore_file_equivalence in ignore_files:
+        if ignored_file_equivalence in ignored_files:
             continue
 
         # Ignored lines
-        ignore_line_equivalence = IgnoreLine(
+        ignored_line_equivalence = IgnoredLine(
             issue.num_line,
             error_code=issue.issue.err_code,
             from_file=issue.from_file,
         )
-        if ignore_line_equivalence in ignore_lines:
+        if ignored_line_equivalence in ignored_lines:
+            continue
+
+        # Ignored blocks
+        # TODO: ignore a librairy rules for a block of code
+        issue_in_ignored_block = False
+        for ignored_block in ignored_blocks:
+            if (
+                ignored_block.from_file == issue.from_file
+                and ignored_block.line_from <= issue.num_line <= ignored_block.line_to
+                and (
+                    ignored_block.error_code == "ALL"
+                    or ignored_block.error_code == issue.issue.err_code
+                )
+            ):
+                issue_in_ignored_block = True
+                continue
+
+        if issue_in_ignored_block:
             continue
 
         result.append(issue)
 
     return result
```

### Comparing `printlinter-0.1.0/printlinter/visitor.py` & `printlinter-0.2.0/printlinter/visitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 
         found_print = IssueInfo(
             issue_type,
             node.lineno,
             node.col_offset,
             line_as_str=None,
             from_file=None,
-            ignore=False,
+            ignored=False,
         )
         self.found_prints.append(cast(IssueInfo, found_print))
 
         return None
 
 
 def _add_file_info(node_visitor: PrintNodeVisitor, file_path: Path) -> None:
```

### Comparing `printlinter-0.1.0/pyproject.toml` & `printlinter-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "printlinter"
-version = "0.1.0"
+version = "0.2.0"
 description = "print linter to know where is the test print"
 authors = ["ulysse <ulysse.chosson@obspm.fr>"]
 license = "EUPL v1.2"
 readme = "README.md"
 packages = [{ include = "cli_app" }, { include = "printlinter" }]
 
 [tool.poetry.scripts]
@@ -28,14 +28,15 @@
 ruff = "^0.0.262"
 pytest-cov = "^4.1.0"
 assertpy = "^1.1"
 mypy = "^1.8.0"
 pytest-icdiff = "^0.9"
 types-toml = "^0.10.8.20240310"
 types-pyyaml = "^6.0.12.20240311"
+black = "^24.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = "--xdoctest"
@@ -70,20 +71,14 @@
 warn_return_any = true
 warn_unused_configs = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 check_untyped_defs = true
 disallow_untyped_decorators = true
 
-# mypy per-module options:
-
-# [[tool.mypy.overrides]]
-# module = []
-# ignore_missing_imports = true
-
 [tool.ruff]
 line-length = 88
 
 select = [
     "F",      # Pyflakes: generic
     "E",      # pycodestyle: generic
     "I",      # isort and flake8-tidy-imports: import order and correctness
@@ -122,18 +117,16 @@
     "D408",
     "D409",
     "D413",
     "S101",    # assert in code --> needed for pytest
     "E999",    # syntax error -> does not support pattern matching yet https://github.com/charliermarsh/ruff/issues/282
     "ANN101",  # Conflict with mypy
     "PLR2004", # Magic value not really magic value
-    # TODO: Passer a des pipes quand l'issue sera resolue.
-    "UP007", # Typer need Optional: https://github.com/tiangolo/typer/issues/533
-    "C901",  # Not really ussefull in this project
-    "B008",  # Not really ussefull in this project
+    "C901",    # Not really ussefull in this project
+    "B008",    # Not really ussefull in this project
 ]
 
 
 # Exclude a variety of commonly ignored directories.
 exclude = [
     "tests",
     ".bzr",
```

### Comparing `printlinter-0.1.0/setup.py` & `printlinter-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,460 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: printlinter
+Version: 0.2.0
+Summary: print linter to know where is the test print
+License: EUPL v1.2
+Author: ulysse
+Author-email: ulysse.chosson@obspm.fr
+Requires-Python: >=3.10,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: rich (>=12.5.1,<13.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: typer (>=0.7.0,<0.8.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['cli_app', 'printlinter']
+<!-- markdownlint-disable-file MD041 -->
 
-package_data = \
-{'': ['*']}
+<!-- TODO: Add badge -->
+![logo](logo.png)
 
-install_requires = \
-['pyyaml>=6.0.1,<7.0.0',
- 'rich>=12.5.1,<13.0.0',
- 'toml>=0.10.2,<0.11.0',
- 'typer>=0.7.0,<0.8.0']
-
-entry_points = \
-{'console_scripts': ['printlinter = cli_app.main:main']}
-
-setup_kwargs = {
-    'name': 'printlinter',
-    'version': '0.1.0',
-    'description': 'print linter to know where is the test print',
-    'long_description': '<!-- markdownlint-disable-file MD041 -->\n\n<!-- TODO: Add badge\nTODO: logo -->\n\n[English readme](README.md) **·** [Français readme](doc/readme/README.fr.md)\n\nPrintLinter is a python linter to detect and signals display functions in python code.\n\n## Summary\n\n- [Installing](#installing)\n- [Usage](#usage)\n  - [Verbs](#verbs)\n    - [Lint](#lint)\n      - [Example](#example)\n- [Error codes](#error-codes)\n  - [Standard library](#standard-library)\n- [Ignore errors](#ignore-errors)\n  - [Ignore error inline](#ignore-error-inline)\n    - [Examples](#examples)\n  - [Ignore a whole file](#ignore-a-whole-file)\n    - [Examples](#examples-1)\n      - [Simple error](#simple-error)\n      - [library errors](#library-errors)\n      - [All errors](#all-errors)\n- [Configuration](#configuration)\n  - [Target version](#target-version)\n  - [Ignored files](#ignored-files)\n  - [Disabled rules](#disabled-rules)\n  - [Examples of configuration files](#examples-of-configuration-files)\n    - [Yaml/Yml configuration file](#yamlyml-configuration-file)\n    - [Json configuration file](#json-configuration-file)\n    - [Toml configuration file](#toml-configuration-file)\n    - [Pyproject configuration file](#pyproject-configuration-file)\n- [But then](#but-then)\n\n# Installing\n\nInstall with `pip` or your favorite PyPI package manageer.\n\n```sh\npip install printlinter\n```\n\nRun the following command to test PrintLinter.\n\n```sh\nprintlinter --version\n```\n\n# Usage\n\n## Verbs\n\nFor help on using a verb.\n\n```sh\nprintlinter <verb> --help\n```\n\n### Lint\n\nTo lint a file or a folder.\n\n```sh\nprintlinter lint <file|folder>\n```\n\nThe product output look like this.\n\n`file_path:line:column error_code display_function_detected error_name`\n\n#### Example\n\n<!-- markdownlint-disable MD013 -->\n```sh\ntests/testing_files/mixed/mixed0.py:5:0: PPL001 `print("toto")` print-detected\ntests/testing_files/mixed/mixed0.py:6:0: PPL002 `pprint("titi")` prettyprint-detected\ntests/testing_files/mixed/mixed1/mixed2.py:5:0: PPL001 `print("toto")` print-detected\ntests/testing_files/mixed/mixed1/mixed2.py:6:0: PPL002 `pprint("titi")` prettyprint-detected\ntests/testing_files/pprint/pprint1.py:6:0: PPL002 `pprint("Hello, world")` prettyprint-detected\ntests/testing_files/pprint/pprint2/pprint3.py:11:4: PPL002 `pprint("tata")` prettyprint-detected\ntests/testing_files/ignored_files/ignore_ppl005.py:7:0: PPL001 `print("toto")` print-detected\ntests/testing_files/ignored_files/ignore_nothing.py:6:0: PPL001 `print("toto")` print-detected\ntests/testing_files/ignored_files/ignore_nothing.py:8:0: PPL002 `pprint("toto")` prettyprint-detected\ntests/testing_files/ignored_files/ignore_ppl006.py:7:0: PPL001 `print("toto")` print-detected\ntests/testing_files/ignored_files/ignore_ppl002.py:7:0: PPL001 `print("toto")` print-detected\ntests/testing_files/ignored_files/ignore_ppl001.py:9:0: PPL002 `pprint("toto")` prettyprint-detected\ntests/testing_files/ignored_files/ignore_ppl004.py:7:0: PPL001 `print("toto")` print-detected\ntests/testing_files/ignored_files/ignore_ppl003.py:7:0: PPL001 `print("toto")` print-detected\ntests/testing_files/ignored_files/disable_in_wrong_place.py:8:0: PPL001 `print("toto")` print-detected\ntests/testing_files/sys/stderr/write/stderr1.py:7:0: PPL004 `sys.stderr.write("Hello, world")` sys.stderr.write-detected\ntests/testing_files/sys/stderr/write/stderr1.py:8:0: PPL004 `stderr.write("Hello, world")` sys.stderr.write-detected\ntests/testing_files/sys/stderr/write/stderr2/stderr3.py:13:4: PPL004 `sys.stderr.write("tata")` sys.stderr.write-detected\ntests/testing_files/sys/stderr/write/stderr2/stderr3.py:14:4: PPL004 `stderr.write("tata")` sys.stderr.write-detected\ntests/testing_files/sys/stderr/writelines/stderr1.py:7:0: PPL006 `sys.stderr.writelines(["Hello", "world"])` sys.stderr.writelines-detected\ntests/testing_files/sys/stderr/writelines/stderr1.py:8:0: PPL006 `stderr.writelines(["Hello", "world"])` sys.stderr.writelines-detected\ntests/testing_files/sys/stderr/writelines/stderr2/stderr3.py:13:4: PPL006 `sys.stderr.writelines(["tata", "tutu"])`\nsys.stderr.writelines-detected\ntests/testing_files/sys/stderr/writelines/stderr2/stderr3.py:14:4: PPL006 `stderr.writelines(["tata", "tutu"])`\nsys.stderr.writelines-detected\ntests/testing_files/sys/stdout/write/stdout1.py:7:0: PPL003 `sys.stdout.write("Hello, world")` sys.stdout.write-detected\ntests/testing_files/sys/stdout/write/stdout2/stdout3.py:13:4: PPL003 `sys.stdout.write("tata")` sys.stdout.write-detected\ntests/testing_files/sys/stdout/writelines/stdout1.py:7:0: PPL005 `sys.stdout.writelines(["Hello", "world"])` sys.stdout.writelines-detected\ntests/testing_files/sys/stdout/writelines/stdout2/stdout3.py:14:4: PPL005 `stdout.writelines(["tata", "tutu"])`\nsys.stdout.writelines-detected\ntests/testing_files/print/toto_1.py:3:0: PPL001 `print("Hello, world")` print-detected\ntests/testing_files/print/toto2/toto3.py:7:4: PPL001 `print("tata")` print-detected\nFound 27 errors\n```\n<!-- markdownlint-enable MD013 -->\n\n# Error codes\n\nAll errors have an individual code based on `PPLXXX`.\nEach library have its own error "domain".\n\n| Library  | Error domain |\n|:---------|:-------------|\n| Standard | PPL0XX       |\n\n## Standard library\n\n| Function                | Error code |\n|:------------------------|:-----------|\n| `print`                 | PPL001     |\n| `pprint`                | PPL002     |\n| `sys.stdout.write`      | PPL003     |\n| `sys.stderr.write`      | PPL004     |\n| `sys.stdout.writelines` | PPL005     |\n| `sys.stderr.writelines` | PPL006     |\n\n# Ignore errors\n\nYou can ignore errors with the linter.\n\n## Ignore error inline\n\nTo ignore a rule inline, add a comment at the end of the line. `# noqa: <error_code>`.\n\n### Examples\n\n```python\ntoto = 1\ntiti = 2\nprint (toto + titi) # noqa: PPL001\n```\n\n## Ignore a whole file\n\nTo ignore a rule, library rules or all rules, add a comment at the beging of the file.\n`# <py-printlinter disable-file <error_code>`.\n\n<!-- markdownlint-disable-next-line MD036 -->\n**The comment must be before any code in a file.**\n\n<!-- markdownlint-disable-next-line MD024 -->\n### Examples\n\n#### Simple error\n\n```python\n# <py-printlinter disable-file PPL002>\nfrom pprint import pprint\ntoto = 1\ntiti = 2\npprint(titi + toto)  # ignored error\n...\n```\n\n#### library errors\n\n```python\n# <py-printlinter disable-file PPL000>\nimport sys\ntoto = 1\ntiti = 2\nprint(titi + toto)  # ignored error\nsys.stdout.write(titi + toto)  # ignored error\n...\n```\n\n#### All errors\n\n```python\n# <py-printlinter disable-file ALL>\nfrom sys import stdout, stderr\nfrom pprint import pprint\ntoto = 1\ntiti = 2\nprint(titi + toto)  # ignored error\npprint(titi + toto)  # ignored error\nstdout.write(titi + toto)  # ignored error\nstderr.write(titi + toto)  # ignored error\nstdout.writelines(titi + toto)  # ignored error\nstderr.writelines(titi + toto)  # ignored error\n...\n```\n\n# Configuration\n\nYou can configurate the linter with a configuration file (configuration by command line,\nwill arrive in a future version).\n\nPrintLinter supports 3 differents file type.\n\n- `.yaml/.yml`\n- `.json`\n- `.toml`\n\nBy default the linter use one of thoses files load in this order.\n\n- `printlinter.yaml`\n- `printlinter.yml`\n- `printlinter.json`\n- `printlinter.toml`\n- `pyproject.toml`\n\nAlternatively, you can use another file and fill it in by running linter from the command\nline.\n\n```sh\nprintlinter lint <file|folder> --config-file </path/of/config/file>\n```\n\n## Target version\n\nThe config file allows to specify the python target version for the parser. Use a\nstring like this `3.10` or `3.7` to specify the version.\n\n<!-- markdownlint-disable-next-line MD036 -->\n**The python target version MUST be contains between 3.7 and 3.10**\n\nYou can see examples of this config [here](#examples-of-configuration-files).\n\n## Ignored files\n\nThe config file allows to ignore files, unlike the comment that allows errors to be\nignored in a whole file this configuration option prevents the linter from reading the file.\n\nYou can see examples of this config [here](#examples-of-configuration-files).\n\n## Disabled rules\n\nThe config file allows to disable rules, in all files and folders.\n\nYou can see examples of this config [here](#examples-of-configuration-files).\n\n## Examples of configuration files\n\n### Yaml/Yml configuration file\n\n```yaml\nprintlinter:\n  target_version: "3.10"\n  ignored_files: [toto.py]\n  disabled_rules: [PPL001]\n```\n\n### Json configuration file\n\n```json\n{\n  "printlinter": {\n    "target_version": "3.10",\n    "ignored_files": ["toto.py"],\n    "disabled_rules": ["PPL001"]\n  }\n}\n\n```\n\n### Toml configuration file\n\n```toml\n[printlinter]\ntarget_version = "3.10"\nignored_files = ["toto.py"]\ndisabled_rules = ["PPL001"]\n```\n\n### Pyproject configuration file\n\n```toml\n[tool.printlinter]\ntarget_version = "3.10"\nignored_files = ["toto.py"]\ndisabled_rules = ["PPL001"]\n```\n\n# But then\n\nToo see the next features to be developed see [TODO](TODO.md). Here\'s a small,\nnon-exhaustive list of what\'s comming in the future versions.\n\n- Ignore a code block in a file.\n- Ignore the next line.\n- Lint display functions from other libraries.\n- Add other configuration options.\n- Add translation in other languages\n',
-    'author': 'ulysse',
-    'author_email': 'ulysse.chosson@obspm.fr',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
+[English readme](README.md) **·** [Français readme](doc/readme/README.fr.md)
+
+PrintLinter is a python linter to detect and signals display functions in python code.
+
+## Summary
+
+- [Installing](#installing)
+- [Usage](#usage)
+  - [Verbs](#verbs)
+    - [Lint](#lint)
+      - [Example](#example)
+- [Error codes](#error-codes)
+  - [Standard library](#standard-library)
+- [Ignore errors](#ignore-errors)
+  - [Ignore error inline](#ignore-error-inline)
+    - [Examples](#examples)
+  - [Ignore error on the next line](#ignore-error-on-the-next-line)
+    - [Examples](#examples-1)
+  - [Ignore a whole file](#ignore-a-whole-file)
+    - [Examples](#examples-2)
+      - [Simple error](#simple-error)
+      - [library errors](#library-errors)
+      - [All errors](#all-errors)
+  - [Ignore a block of code](#ignore-a-block-of-code)
+    - [Examples](#examples-3)
+      - [Simple error](#simple-error-1)
+      - [All errors](#all-errors-1)
+- [Configuration](#configuration)
+  - [Target version](#target-version)
+  - [Ignored files](#ignored-files)
+  - [Disabled rules](#disabled-rules)
+  - [Color](#color)
+  - [Examples of configuration files](#examples-of-configuration-files)
+    - [Yaml/Yml configuration file](#yamlyml-configuration-file)
+    - [Json configuration file](#json-configuration-file)
+    - [Toml configuration file](#toml-configuration-file)
+    - [Pyproject configuration file](#pyproject-configuration-file)
+- [But then](#but-then)
+
+# Installing
+
+Install with `pip` or your favorite PyPI package manageer.
+
+```sh
+pip install printlinter
+```
+
+Run the following command to test PrintLinter.
+
+```sh
+printlinter --version
+```
+
+# Usage
+
+## Verbs
+
+For help on using a verb.
+
+```sh
+printlinter <verb> --help
+```
+
+### Lint
+
+To lint a file or a folder.
+
+```sh
+printlinter lint <file|folder>
+```
+
+The product output look like this.
+
+`file_path:line:column error_code display_function_detected error_name`
+
+By default we disable the linter in some folders.
+
+- `node_modules`
+- `.vscode/`
+- `__pycache__/`
+- `build/`
+- `develop-eggs/`
+- `dist/`
+- `downloads/`
+- `eggs/`
+- `.eggs/`
+- `lib/`
+- `lib64/`
+- `parts/`
+- `sdist/`
+- `var/`
+- `wheels/`
+- `pip-wheel-metadata/`
+- `share/python-wheels/`
+- `htmlcov/`
+- `.tox/`
+- `.nox/`
+- `.hypothesis/`
+- `.pytest_cache/`
+- `docs/_build/`
+- `__pypackages__/`
+- `.mypy_cache/`
+- `.ruff_cache`
+- `.pyre/`
+- `env/`
+- `venv/`
+- `ENV/`
+- `env.bak/`
+- `venv.bak/`
+- `.venv/`
+- `.env/`
+
+#### Example
+
+<!-- markdownlint-disable MD013 -->
+```sh
+tests/testing_files/mixed/mixed0.py:5:0: PPL001 `print("toto")` print-detected
+tests/testing_files/mixed/mixed0.py:6:0: PPL002 `pprint("titi")` prettyprint-detected
+tests/testing_files/mixed/mixed1/mixed2.py:5:0: PPL001 `print("toto")` print-detected
+tests/testing_files/mixed/mixed1/mixed2.py:6:0: PPL002 `pprint("titi")` prettyprint-detected
+tests/testing_files/pprint/pprint1.py:6:0: PPL002 `pprint("Hello, world")` prettyprint-detected
+tests/testing_files/pprint/pprint2/pprint3.py:11:4: PPL002 `pprint("tata")` prettyprint-detected
+tests/testing_files/ignored_files/ignore_ppl005.py:7:0: PPL001 `print("toto")` print-detected
+tests/testing_files/ignored_files/ignore_nothing.py:6:0: PPL001 `print("toto")` print-detected
+tests/testing_files/ignored_files/ignore_nothing.py:8:0: PPL002 `pprint("toto")` prettyprint-detected
+tests/testing_files/ignored_files/ignore_ppl006.py:7:0: PPL001 `print("toto")` print-detected
+tests/testing_files/ignored_files/ignore_ppl002.py:7:0: PPL001 `print("toto")` print-detected
+tests/testing_files/ignored_files/ignore_ppl001.py:9:0: PPL002 `pprint("toto")` prettyprint-detected
+tests/testing_files/ignored_files/ignore_ppl004.py:7:0: PPL001 `print("toto")` print-detected
+tests/testing_files/ignored_files/ignore_ppl003.py:7:0: PPL001 `print("toto")` print-detected
+tests/testing_files/ignored_files/disable_in_wrong_place.py:8:0: PPL001 `print("toto")` print-detected
+tests/testing_files/sys/stderr/write/stderr1.py:7:0: PPL004 `sys.stderr.write("Hello, world")` sys.stderr.write-detected
+tests/testing_files/sys/stderr/write/stderr1.py:8:0: PPL004 `stderr.write("Hello, world")` sys.stderr.write-detected
+tests/testing_files/sys/stderr/write/stderr2/stderr3.py:13:4: PPL004 `sys.stderr.write("tata")` sys.stderr.write-detected
+tests/testing_files/sys/stderr/write/stderr2/stderr3.py:14:4: PPL004 `stderr.write("tata")` sys.stderr.write-detected
+tests/testing_files/sys/stderr/writelines/stderr1.py:7:0: PPL006 `sys.stderr.writelines(["Hello", "world"])` sys.stderr.writelines-detected
+tests/testing_files/sys/stderr/writelines/stderr1.py:8:0: PPL006 `stderr.writelines(["Hello", "world"])` sys.stderr.writelines-detected
+tests/testing_files/sys/stderr/writelines/stderr2/stderr3.py:13:4: PPL006 `sys.stderr.writelines(["tata", "tutu"])`
+sys.stderr.writelines-detected
+tests/testing_files/sys/stderr/writelines/stderr2/stderr3.py:14:4: PPL006 `stderr.writelines(["tata", "tutu"])`
+sys.stderr.writelines-detected
+tests/testing_files/sys/stdout/write/stdout1.py:7:0: PPL003 `sys.stdout.write("Hello, world")` sys.stdout.write-detected
+tests/testing_files/sys/stdout/write/stdout2/stdout3.py:13:4: PPL003 `sys.stdout.write("tata")` sys.stdout.write-detected
+tests/testing_files/sys/stdout/writelines/stdout1.py:7:0: PPL005 `sys.stdout.writelines(["Hello", "world"])` sys.stdout.writelines-detected
+tests/testing_files/sys/stdout/writelines/stdout2/stdout3.py:14:4: PPL005 `stdout.writelines(["tata", "tutu"])`
+sys.stdout.writelines-detected
+tests/testing_files/print/toto_1.py:3:0: PPL001 `print("Hello, world")` print-detected
+tests/testing_files/print/toto2/toto3.py:7:4: PPL001 `print("tata")` print-detected
+Found 27 errors
+```
+<!-- markdownlint-enable MD013 -->
+
+# Error codes
+
+All errors have an individual code based on `PPLXXX`.
+Each library have its own error "domain".
+
+| Library  | Error domain |
+|:---------|:-------------|
+| Standard | PPL0XX       |
+
+## Standard library
+
+| Function                | Error code |
+|:------------------------|:-----------|
+| `print`                 | PPL001     |
+| `pprint`                | PPL002     |
+| `sys.stdout.write`      | PPL003     |
+| `sys.stderr.write`      | PPL004     |
+| `sys.stdout.writelines` | PPL005     |
+| `sys.stderr.writelines` | PPL006     |
+
+# Ignore errors
+
+You can ignore errors with the linter.
+
+## Ignore error inline
+
+To ignore a rule inline, add a comment at the end of the line. `# noqa: <error_code>`.
+
+### Examples
+
+```python
+toto = 1
+titi = 2
+print (toto + titi) # noqa: PPL001
+```
+
+## Ignore error on the next line
+
+To ignore a rule on the next line, add a comment at the line before code to ignore.
+`<printlinter disable-next (error_code)>`.
+
+<!-- markdownlint-disable-next-line MD024 -->
+### Examples
+
+```python
+toto = 1
+titi = 2
+# <printlinter disable-next PPL001>
+print (toto + titi) # ignored error
+```
+
+## Ignore a whole file
+
+To ignore a rule, library rules or all rules, add a comment at the beging of the file.
+`# <printlinter disable-file (error_code)>`.
+
+<!-- markdownlint-disable-next-line MD036 -->
+**The comment must be before any code in a file.**
+
+<!-- markdownlint-disable-next-line MD024 -->
+### Examples
+
+#### Simple error
+
+```python
+# <printlinter disable-file PPL002>
+from pprint import pprint
+toto = 1
+titi = 2
+pprint(titi + toto)  # ignored error
+...
+```
+
+#### library errors
+
+```python
+# <printlinter disable-file PPL000>
+import sys
+toto = 1
+titi = 2
+print(titi + toto)  # ignored error
+sys.stdout.write(titi + toto)  # ignored error
+...
+```
+
+#### All errors
+
+```python
+# <printlinter disable-file ALL>
+from sys import stdout, stderr
+from pprint import pprint
+toto = 1
+titi = 2
+print(titi + toto)  # ignored error
+pprint(titi + toto)  # ignored error
+stdout.write(titi + toto)  # ignored error
+stderr.write(titi + toto)  # ignored error
+stdout.writelines(titi + toto)  # ignored error
+stderr.writelines(titi + toto)  # ignored error
+...
+```
+
+## Ignore a block of code
+
+To ignore a block of code (disable the linter) on a rules or all rules (disable library
+rules come later), add a comment before the block you want ignore:
+`<printlinter disable (error_code)`. To re enable the linter add an other comment after
+the block of code: `<printlinter enable (error_code)>`. You are don't have to re enable
+the linter after disabled it.
+
+<!-- markdownlint-disable-next-line MD024 -->
+### Examples
+
+<!-- markdownlint-disable-next-line MD024 -->
+#### Simple error
+
+```python
+from pprint import pprint
+# <printlinter disable PPL001>
+print("toto") # ignored error
+pprint("titit")
+# <printlinter enable PPL001>
+...
+```
+
+You can nested ignored block.
+
+```python
+from pprint import pprint
+
+# <printlinter disable PPL002>
+
+pprint("titi") # ignored error
+
+# <printlinter disable PPL001>
+print("toto") # ignored error
+# <printlinter enable PPL001>
+
+print("tutu") # NOT IGNORED ERROR
+pprint("tata") # ignored error
+
+# <printlinter enable PPL002>
+...
+```
+
+without re enable the linter.
+
+```python
+from pprint import pprint
+# <printlinter disable PPL001>
+print("toto") # ignored error
+pprint("titit")
+...
+print('toto') # ignored error
+```
+
+<!-- markdownlint-disable-next-line MD024 -->
+#### All errors
+
+```python
+from sys import stdout, stderr
+from pprint import pprint
+toto = 1
+titi = 2
+# <printlinter disable ALL>
+print(titi + toto)  # ignored error
+pprint(titi + toto)  # ignored error
+stdout.write(titi + toto)  # ignored error
+stderr.write(titi + toto)  # ignored error
+stdout.writelines(titi + toto)  # ignored error
+stderr.writelines(titi + toto)  # ignored error
+# <printlinter enable ALL>
+...
+```
+
+# Configuration
+
+You can configurate the linter with a configuration file (configuration by command line,
+will arrive in a future version).
+
+PrintLinter supports 3 differents file type.
+
+- `.yaml/.yml`
+- `.json`
+- `.toml`
+
+By default the linter use one of thoses files load in this order.
+
+- `printlinter.yaml`
+- `printlinter.yml`
+- `printlinter.json`
+- `printlinter.toml`
+- `pyproject.toml`
+
+Alternatively, you can use another file and fill it in by running linter from the command
+line.
+
+```sh
+printlinter lint <file|folder> --config-file </path/of/config/file>
+```
+
+## Target version
+
+The config file allows to specify the python target version for the parser. Use a
+string like this `3.10` or `3.7` to specify the version.
+
+<!-- markdownlint-disable-next-line MD036 -->
+**The python target version MUST be contains between 3.7 and 3.10**
+
+You can see examples of this config [here](#examples-of-configuration-files).
+
+## Ignored files
+
+The config file allows to ignore files, unlike the comment that allows errors to be
+ignored in a whole file this configuration option prevents the linter from reading the file.
+
+You can see examples of this config [here](#examples-of-configuration-files).
+
+## Disabled rules
+
+The config file allows to disable rules, in all files and folders.
+
+You can see examples of this config [here](#examples-of-configuration-files).
+
+## Color
+
+The config file allows to enable or disable colorized output. By default the `color` option
+is on `True`.
+
+You can see examples of this config [here](#examples-of-configuration-files).
+
+## Examples of configuration files
+
+### Yaml/Yml configuration file
+
+```yaml
+printlinter:
+  target_version: "3.10"
+  ignored_files: [toto.py]
+  disabled_rules: [PPL001]
+  color: true
+```
+
+### Json configuration file
+
+```json
+{
+  "printlinter": {
+    "target_version": "3.10",
+    "ignored_files": ["toto.py"],
+    "disabled_rules": ["PPL001"],
+    "color": false
+  }
 }
 
+```
+
+### Toml configuration file
+
+```toml
+[printlinter]
+target_version = "3.10"
+ignored_files = ["toto.py"]
+disabled_rules = ["PPL001"]
+color = true
+```
+
+### Pyproject configuration file
+
+```toml
+[tool.printlinter]
+target_version = "3.10"
+ignored_files = ["toto.py"]
+disabled_rules = ["PPL001"]
+color = false
+```
+
+# But then
+
+Too see the next features to be developed see [TODO](TODO.md). Here's a small,
+non-exhaustive list of what's comming in the future versions.
+
+- Lint display functions from other libraries.
+- Add other configuration options.
 
-setup(**setup_kwargs)
```

