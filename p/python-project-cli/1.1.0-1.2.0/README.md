# Comparing `tmp/python_project_cli-1.1.0.tar.gz` & `tmp/python_project_cli-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_project_cli-1.1.0.tar", max compression
+gzip compressed data, was "python_project_cli-1.2.0.tar", max compression
```

## Comparing `python_project_cli-1.1.0.tar` & `python_project_cli-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2024-05-17 17:21:46.831250 python_project_cli-1.1.0/LICENSE
--rw-r--r--   0        0        0     1557 2024-05-17 17:21:46.831250 python_project_cli-1.1.0/README.md
--rw-r--r--   0        0        0     2387 2024-05-17 17:21:47.899263 python_project_cli-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-17 17:21:46.831250 python_project_cli-1.1.0/src/python_project_cli/__init__.py
--rw-r--r--   0        0        0     1858 2024-05-17 17:21:47.899263 python_project_cli-1.1.0/src/python_project_cli/main.py
--rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 python_project_cli-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-23 12:59:08.754524 python_project_cli-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1572 2024-05-23 12:59:08.754524 python_project_cli-1.2.0/README.md
+-rw-r--r--   0        0        0     2387 2024-05-23 12:59:09.710522 python_project_cli-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-23 12:59:08.758524 python_project_cli-1.2.0/src/python_project_cli/__init__.py
+-rw-r--r--   0        0        0     1895 2024-05-23 12:59:09.710522 python_project_cli-1.2.0/src/python_project_cli/main.py
+-rw-r--r--   0        0        0     2376 1970-01-01 00:00:00.000000 python_project_cli-1.2.0/PKG-INFO
```

### Comparing `python_project_cli-1.1.0/LICENSE` & `python_project_cli-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_project_cli-1.1.0/README.md` & `python_project_cli-1.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # MentorMate Python CLI
 A CLI tool for generating Django and FastAPI projects.
 
 ![Tests](https://github.com/MentorMate/python-project-cli/actions/workflows/tests.yaml/badge.svg)
 
-![Deploy](https://github.com/MentorMate/python-project-cli/actions/workflows/main_release.yaml/badge.svg)
+![Deploy](https://github.com/MentorMate/python-project-cli/actions/workflows/release.yaml/badge.svg)
 
 ## Overview
 This is a python-cli tool for interactive project setup, following best practices for **Django** and **FastAPI**.
 In order to assure easier distribution, the project is deployed as **pypi** package.
 For optimal maintenance the project utilizes the **tox** framework.
 
 # Installation
@@ -33,12 +33,12 @@
     ```
 
 ### Frameworks
 - Django
 - FastAPI
 
 ### Project Maintenance (Internal)
-[Confluence link](https://mentormate.atlassian.net/wiki/spaces/MMSDLC/pages/4325900953/Python+CLI+documentation)
+[Confluence link](https://mentormate.atlassian.net/wiki/spaces/MMSDLC/pages/4325900953/Python+CLI+documentation#Package-Maintenance)
 
 ## License
 PYTHON-PROJECT-CLI is unlicensed, as found in the
 [LICENSE](https://github.com/MentorMate/python-project-cli/blob/development/LICENSE) file.
```

### Comparing `python_project_cli-1.1.0/pyproject.toml` & `python_project_cli-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "python_project_cli"
-version = "1.1.0"
+version = "1.2.0"
 authors = ["alexandermentormate"]
 description = "CLI for building base djang and fastapi based projects"
 readme = "README.md"
 homepage = "https://github.com/MentorMate/python-project-cli/"
 repository = "https://github.com/MentorMate/python-project-cli/"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `python_project_cli-1.1.0/src/python_project_cli/main.py` & `python_project_cli-1.2.0/src/python_project_cli/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from subprocess import run
 from rich.console import Console
 from rich.table import Table
 from rich import print
 import typer
 from typing_extensions import Annotated
 
-__version__ = '1.1.0'
+__version__ = '1.2.0'
 
-app = typer.Typer(add_completion=False)
+app = typer.Typer(add_completion=False, no_args_is_help=True)
 console = Console()
 
 
 class Frameworks(StrEnum):
     django = 'Django'
     fast_api = 'FastAPI'
 
@@ -57,15 +57,15 @@
         f'[bold]{Frameworks.django}[bold]',
         f'[blue]{REPO_URLS[Frameworks.django]}[blue]',
         ':white_check_mark:',
     )
     table.add_row(
         f'[bold]{Frameworks.fast_api}[bold]',
         f'[blue]{REPO_URLS[Frameworks.fast_api]}[blue]',
-        ':x:',
+        ':white_check_mark:',
     )
     console.print(table)
 
 
 @app.command(help='CLI version.')
 def version() -> None:
     print(f'[bold]CLI Version:[bold] {__version__}')
```

### Comparing `python_project_cli-1.1.0/PKG-INFO` & `python_project_cli-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_project_cli
-Version: 1.1.0
+Version: 1.2.0
 Summary: CLI for building base djang and fastapi based projects
 Home-page: https://github.com/MentorMate/python-project-cli/
 Author: alexandermentormate
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 
 # MentorMate Python CLI
 A CLI tool for generating Django and FastAPI projects.
 
 ![Tests](https://github.com/MentorMate/python-project-cli/actions/workflows/tests.yaml/badge.svg)
 
-![Deploy](https://github.com/MentorMate/python-project-cli/actions/workflows/main_release.yaml/badge.svg)
+![Deploy](https://github.com/MentorMate/python-project-cli/actions/workflows/release.yaml/badge.svg)
 
 ## Overview
 This is a python-cli tool for interactive project setup, following best practices for **Django** and **FastAPI**.
 In order to assure easier distribution, the project is deployed as **pypi** package.
 For optimal maintenance the project utilizes the **tox** framework.
 
 # Installation
@@ -51,13 +51,13 @@
     ```
 
 ### Frameworks
 - Django
 - FastAPI
 
 ### Project Maintenance (Internal)
-[Confluence link](https://mentormate.atlassian.net/wiki/spaces/MMSDLC/pages/4325900953/Python+CLI+documentation)
+[Confluence link](https://mentormate.atlassian.net/wiki/spaces/MMSDLC/pages/4325900953/Python+CLI+documentation#Package-Maintenance)
 
 ## License
 PYTHON-PROJECT-CLI is unlicensed, as found in the
 [LICENSE](https://github.com/MentorMate/python-project-cli/blob/development/LICENSE) file.
```

