# Comparing `tmp/python_re3data-0.1.0.tar.gz` & `tmp/python_re3data-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, last modified: Thu May 23 16:47:19 2024, max compression
```

## Comparing `python_re3data-0.1.0.tar` & `python_re3data-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 python_re3data-0.1.0/src/re3data/__about__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 python_re3data-0.1.0/src/re3data/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 python_re3data-0.1.0/src/re3data/__main__.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 python_re3data-0.1.0/src/re3data/_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_re3data-0.1.0/src/re3data/py.typed
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 python_re3data-0.1.0/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 python_re3data-0.1.0/LICENSE
--rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 python_re3data-0.1.0/README.md
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 python_re3data-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 python_re3data-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      113 2024-05-23 16:47:19.000000 python_re3data-0.2.0/src/re3data/__about__.py
+-rw-r--r--   0        0        0      295 2024-05-23 16:47:19.000000 python_re3data-0.2.0/src/re3data/__init__.py
+-rw-r--r--   0        0        0      185 2024-05-23 16:47:19.000000 python_re3data-0.2.0/src/re3data/__main__.py
+-rw-r--r--   0        0        0     1084 2024-05-23 16:47:19.000000 python_re3data-0.2.0/src/re3data/_cli.py
+-rw-r--r--   0        0        0     4992 2024-05-23 16:47:19.000000 python_re3data-0.2.0/src/re3data/_client.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:47:19.000000 python_re3data-0.2.0/src/re3data/py.typed
+-rw-r--r--   0        0        0     1160 2024-05-23 16:47:19.000000 python_re3data-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1082 2024-05-23 16:47:19.000000 python_re3data-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7529 2024-05-23 16:47:19.000000 python_re3data-0.2.0/README.md
+-rw-r--r--   0        0        0     7008 2024-05-23 16:47:19.000000 python_re3data-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9555 2024-05-23 16:47:19.000000 python_re3data-0.2.0/PKG-INFO
```

### Comparing `python_re3data-0.1.0/src/re3data/_cli.py` & `python_re3data-0.2.0/src/re3data/_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-"""re3data command line interface."""
+# SPDX-FileCopyrightText: 2024 Heinz-Alexander Fütterer
+#
+# SPDX-License-Identifier: MIT
+
+"""python-re3data command line interface."""
 
 import logging
 import sys
 import typing
 
 logger = logging.getLogger(__name__)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python_re3data-0.1.0/.gitignore` & `python_re3data-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `python_re3data-0.1.0/LICENSE` & `python_re3data-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_re3data-0.1.0/pyproject.toml` & `python_re3data-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -82,14 +82,19 @@
 packages = [
   "src/re3data",
 ]
 
 [tool.hatch.version]
 path = "src/re3data/__about__.py"
 
+[tool.hatch.env]
+requires = [
+  "hatch-pip-compile",
+]
+
 [tool.hatch.envs.default]
 installer = "uv"
 features = [
   "dev",
   "test",
 ]
 post-install-commands = [
@@ -112,25 +117,27 @@
 
 [tool.hatch.envs.docs]
 features = [
   "cli",
   "docs",
 ]
 template = "docs"
+type = "pip-compile"
+pip-compile-hashes = true
+pip-compile-installer = "uv"
+pip-compile-resolver = "uv"
+lock-filename = "requirements/{env_name}.txt"
+
 [tool.hatch.envs.docs.scripts]
 cli = "typer src/re3data/_cli.py utils docs --name=re3data --title='CLI Reference' --output docs/src/cli.md"
 build = "mkdocs build --config-file=docs/mkdocs.yml"
 serve = "mkdocs serve --verbose --config-file=docs/mkdocs.yml"
 deploy = "mike deploy --push --update-aliases $(hatch version) latest --config-file=docs/mkdocs.yml"
 
-# ruff
-# Ref: https://docs.astral.sh/ruff/configuration/
-# ------------------------------------------------------------------------------
-
-[tool.ruff]
+[tool.ruff] # Ref: https://docs.astral.sh/ruff/configuration/
 line-length = 120
 src = [
   "src",
   "tests",
 ]
 # Ref: https://docs.astral.sh/ruff/settings/#format
 format.docstring-code-format = true
@@ -153,14 +160,18 @@
   "SIM",  # flake8-simplify
   "T20",  # flake8-print
   "TCH",  # flake8-type-checking
   "UP",   # pyupgrade
   "W",    # pycodestyle
   "YTT",  # flake8-2020
 ]
+lint.ignore = [
+  "D105", # undocumented-magic-method
+  "D107", # undocumented-public-init
+]
 lint.per-file-ignores."src/re3data/__about__.py" = [
   "D100", # undocumented-public-module
 ]
 lint.per-file-ignores."tests/*" = [
   "D100",    # undocumented-public-module
   "D103",    # undocumented-public-function
   "PLR2004", # magic-value-comparison
@@ -168,106 +179,79 @@
 lint.unfixable = [
   "F401", # unused-import
 ]
 lint.isort.known-first-party = [
   "re3data",
 ]
 lint.pydocstyle.convention = "google"
-lint.ignore = [
-  "D105", # undocumented-magic-method
-  "D107", # undocumented-public-init
-]
-
-# sp-repo-review
-# Ref: https://github.com/scientific-python/cookie/tree/main#list-of-checks
-# ------------------------------------------------------------------------------
 
-[tool.repo-review]
+[tool.repo-review] # Ref: https://github.com/scientific-python/cookie/tree/main#list-of-checks
 ignore = [
   # PC is Pre-commit
   "PC111", # blacken-docs
   "PC160", # codespell
   "PC170", # pygrep hooks
   "PC180", # prettier
   "RTD",   # read the docs
 ]
 
-# pytest
-# Ref: https://docs.pytest.org/en/stable/customize.html
-# ------------------------------------------------------------------------------
-
-[tool.pytest.ini_options]
+[tool.pytest.ini_options] # Ref: https://docs.pytest.org/en/stable/customize.html
 minversion = "8.0"
 addopts = [
   "-ra",
   "--showlocals",
   "--strict-markers",
   "--strict-config",
 ]
 filterwarnings = [
   "error",
 ]
 log_cli_level = "INFO"
 xfail_strict = true
 testpaths = "tests"
 
-# coverage.py
-# Ref: https://coverage.readthedocs.io/en/latest/config.html
-# ------------------------------------------------------------------------------
-
-[tool.coverage.run]
+[tool.coverage.run] # Ref: https://coverage.readthedocs.io/en/latest/config.html
 branch = true
 parallel = true
 source = [
   "re3data",
 ]
 omit = [
   "__about__.py",
   "__main__.py",
 ]
 
 [tool.coverage.report]
 exclude_also = [
   "if TYPE_CHECKING:",
+  "@abstractmethod",
 ]
 fail_under = 90
 show_missing = true
 skip_covered = true
 skip_empty = true
 
-# mypy
-# Ref: https://mypy.readthedocs.io/en/stable/config_file.html#using-a-pyproject-toml-file
-# ------------------------------------------------------------------------------
-
-[tool.mypy]
+[tool.mypy] # Ref: https://mypy.readthedocs.io/en/stable/config_file.html#using-a-pyproject-toml-file
 python_version = "3.10"
 strict = true
 pretty = true
 show_column_numbers = true
 show_error_context = true
 enable_error_code = [
   "ignore-without-code",
   "redundant-expr",
   "truthy-bool",
 ]
 warn_unreachable = true
 
-# licensecheck
-# Ref: https://github.com/FHPythonUtils/LicenseCheck/#example-1-pyprojecttoml
-# ------------------------------------------------------------------------------
-
-[tool.licensecheck]
+[tool.licensecheck] # Ref: https://github.com/FHPythonUtils/LicenseCheck/#example-1-pyprojecttoml
 using = "PEP631"
 format = "ansi"
 
-# python-semantic-release
-# Ref: https://python-semantic-release.readthedocs.io/en/latest/configuration.html#settings
-# ------------------------------------------------------------------------------
-
-[tool.semantic_release]
+[tool.semantic_release] # Ref: https://python-semantic-release.readthedocs.io/en/latest/configuration.html#settings
 commit_author = "github-actions[bot] <41898282+github-actions[bot]@users.noreply.github.com>"
 commit_message = "chore: release {version}\n\nAutomatically generated by python-semantic-release [skip ci]"
 major_on_zero = false
 tag_format = "{version}"
 version_variables = [
   "src/re3data/__about__.py:__version__",
 ]
@@ -277,16 +261,12 @@
 git add CITATION.cff
 python -m pip install "build[uv]"
 python -m build --installer=uv
 """
 changelog.template_dir = ".github/templates"
 changelog.environment.keep_trailing_newline = true
 
-# typos
-# Ref: https://github.com/crate-ci/typos/blob/master/docs/reference.md
-# ------------------------------------------------------------------------------
-
-[tool.typos]
+[tool.typos] # Ref: https://github.com/crate-ci/typos/blob/master/docs/reference.md
 # add "spellchecker:disable-line" to ignore specific lines
 default.extend-ignore-re = [
   "(?Rm)^.*# spellchecker:disable-line$",
 ]
```

### Comparing `python_re3data-0.1.0/PKG-INFO` & `python_re3data-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,60 @@
-Metadata-Version: 2.3
-Name: python-re3data
-Version: 0.1.0
-Summary: The Pythonic client for the re3data API.
-Project-URL: Changelog, https://github.com/afuetterer/python-re3data/blob/main/CHANGELOG.md
-Project-URL: Documentation, https://afuetterer.github.io/python-re3data
-Project-URL: Issues, https://github.com/afuetterer/python-re3data/issues
-Project-URL: Repository, https://github.com/afuetterer/python-re3data.git
-Author: Heinz-Alexander Fütterer
-License: MIT
-License-File: LICENSE
-Keywords: api,api-client,metadata,re3data,repositories,research data
-Classifier: Development Status :: 1 - Planning
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Text Processing :: Markup :: XML
-Classifier: Typing :: Typed
-Requires-Python: >=3.10
-Requires-Dist: httpx>=0.27
-Provides-Extra: cli
-Requires-Dist: typer>=0.12; extra == 'cli'
-Provides-Extra: dev
-Requires-Dist: pre-commit~=3.7; extra == 'dev'
-Requires-Dist: typer>=0.12; extra == 'dev'
-Provides-Extra: docs
-Requires-Dist: mike~=2.1; extra == 'docs'
-Requires-Dist: mkdocs-include-markdown-plugin~=6.0; extra == 'docs'
-Requires-Dist: mkdocs-material~=9.5; extra == 'docs'
-Requires-Dist: mkdocstrings[python]~=0.25; extra == 'docs'
-Requires-Dist: mkdocs~=1.6; extra == 'docs'
-Provides-Extra: test
-Requires-Dist: pytest-cov~=5.0; extra == 'test'
-Requires-Dist: pytest-mock~=3.14; extra == 'test'
-Requires-Dist: pytest-randomly~=3.15; extra == 'test'
-Requires-Dist: pytest-recording~=0.13; extra == 'test'
-Requires-Dist: pytest-xdist~=3.6; extra == 'test'
-Requires-Dist: pytest~=8.2; extra == 'test'
-Requires-Dist: respx~=0.21; extra == 'test'
-Description-Content-Type: text/markdown
-
 # python-re3data: The Pythonic client for the re3data API.
 
 > ⚠️ Please note that this project is currently under active development. As such, it is considered a work in progress,
 > and breaking changes may be introduced at any time. We encourage users to frequently check back for updates and to
 > exercise caution when using this project in production environments. Contributions and feedback are welcome to help
 > move the project towards a more stable release (v1.0.0).
 
-| __CI__   | [![pre-commit.ci status][pre-commit-ci-badge]][pre-commit-ci-status] [![ci][ci-badge]][ci-workflow] [![coverage][coverage-badge]][ci-workflow] [![codeql][codeql-badge]][codeql-workflow] |
-| :------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| __Docs__ | [![docs][docs-badge]][docs-workflow]                                                                                                                                                      |
-| __Meta__ | [![OpenSSF Scorecard][scorecard-badge]][scorecard-url] [![hatch][hatch-badge]][hatch] [![ruff][ruff-badge]][ruff] [![mypy][mypy-badge]][mypy] [![License][license-badge]][license-url]    |
+| __CI__      | [![pre-commit.ci status][pre-commit-ci-badge]][pre-commit-ci-status] [![ci][ci-badge]][ci-workflow] [![coverage][coverage-badge]][ci-workflow] [![codeql][codeql-badge]][codeql-workflow]                                                                                      |
+| :---------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| __Docs__    | [![docs][docs-badge]][docs-workflow]                                                                                                                                                                                                                                           |
+| __Package__ | [![pypi-status][status-badge]][pypi-url] [![pypi-version][pypi-version-badge]][pypi-url] [![pypi-python-versions][pypi-python-versions-badge]][pypi-url] [![all-downloads][all-downloads-badge]][pepy-tech-url] [![monthly-downloads][monthly-downloads-badge]][pepy-tech-url] |
+| __Meta__    | [![OpenSSF Scorecard][scorecard-badge]][scorecard-url] [![hatch][hatch-badge]][hatch] [![ruff][ruff-badge]][ruff] [![mypy][mypy-badge]][mypy] [![License][license-badge]][license-url]                                                                                         |
 
 `python-re3data` is a Python library that simplifies interacting with the [re3data](https://www.re3data.org) (Registry
 of Research Data Repositories) [REST API](https://www.re3data.org/api/doc), allowing you to easily retrieve and process
 metadata about research data repositories in a convenient and Pythonic way.
 
-**Table of Contents**
+```pycon
+>>> import re3data
+>>> response = re3data.repositories.list()
+>>> print(response)
+<?xml version="1.0" encoding="UTF-8"?>
+<list>
+  <repository>
+    <id>r3d100010468</id>
+    <doi>https://doi.org/10.17616/R3QP53</doi>
+    <name>Zenodo</name>
+    <link href="https://www.re3data.org/api/beta/repository/r3d100010468" rel="self" />
+  </repository>
+... (remaining repositories truncated)
+```
+
+```pycon
+>>> response = re3data.repositories.get("r3d100010468")
+>>> print(response)
+<?xml version="1.0" encoding="utf-8"?>
+<!--re3data.org Schema for the Description of Research Data Repositories. Version 2.2, December 2014. doi:10.2312/re3.006-->
+<r3d:re3data xmlns:r3d="http://www.re3data.org/schema/2-2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://www.re3data.org/schema/2-2 http://schema.re3data.org/2-2/re3dataV2-2.xsd">
+  <r3d:repository>
+    <r3d:re3data.orgIdentifier>r3d100010468</r3d:re3data.orgIdentifier>
+    <r3d:repositoryName language="eng">Zenodo</r3d:repositoryName>
+    <r3d:repositoryURL>https://zenodo.org/</r3d:repositoryURL>
+... (remaining fields truncated)
+```
+
+## Features
 
-- [Installation](#installation)
-- [License](#license)
+- Pythonic API interactions: Interact with the re3data API in a Pythonic way, without having to worry about low-level
+    HTTP requests or XML parsing.
+- Repository metadata retrieval: Easily fetch and process metadata about research data repositories using
+    `re3data.repositories.list()`.
+- Repository details retrieval: Get detailed information about a specific repository using
+    `re3data.repositories.get(repository_id)`.
 
 ## Requirements
 
 [Python](https://www.python.org/downloads/) >= 3.10
 
 `python-re3data` is built with:
 
@@ -96,30 +83,36 @@
 | ---------------------------------------------- | ------------------------------------------------------------------------------------ | -------------------------------------------------------------------------- |
 | [py3data](https://github.com/J535D165/py3data) | `py3data` is a lightweight and thin Python interface to the beta version of the API. | ![last-commit](https://img.shields.io/github/last-commit/J535D165/py3data) |
 
 ## License
 
 `python-re3data` is distributed under the terms of the [MIT License][license-url].
 
-<!-- Markdown links -->
+<!-- Refs -->
 
+[all-downloads-badge]: https://static.pepy.tech/badge/python-re3data
 [ci-badge]: https://github.com/afuetterer/python-re3data/actions/workflows/main.yml/badge.svg
 [ci-workflow]: https://github.com/afuetterer/python-re3data/actions/workflows/main.yml
 [codeql-badge]: https://github.com/afuetterer/python-re3data/actions/workflows/codeql.yml/badge.svg
 [codeql-workflow]: https://github.com/afuetterer/python-re3data/actions/workflows/codeql.yml
 [coverage-badge]: https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/afuetterer/adc66df152c473c1aa136557ee8181ca/raw/coverage-badge.json
 [docs-badge]: https://github.com/afuetterer/python-re3data/actions/workflows/docs.yml/badge.svg
 [docs-url]: https://afuetterer.github.io/python-re3data
 [docs-workflow]: https://github.com/afuetterer/python-re3data/actions/workflows/docs.yml
 [hatch]: https://github.com/pypa/hatch
 [hatch-badge]: https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg
 [license-badge]: https://img.shields.io/badge/license-MIT-blue.svg
 [license-url]: https://spdx.org/licenses/MIT.html
+[monthly-downloads-badge]: https://static.pepy.tech/badge/python-re3data/month
 [mypy]: https://mypy-lang.org
 [mypy-badge]: https://img.shields.io/badge/types-mypy-blue.svg
+[pepy-tech-url]: https://pepy.tech/project/python-re3data
 [pre-commit-ci-badge]: https://results.pre-commit.ci/badge/github/afuetterer/python-re3data/main.svg
 [pre-commit-ci-status]: https://results.pre-commit.ci/latest/github/afuetterer/python-re3data/main
+[pypi-python-versions-badge]: https://img.shields.io/pypi/pyversions/python-re3data.svg?logo=python&label=Python
 [pypi-url]: https://pypi.org/project/python-re3data/
+[pypi-version-badge]: https://img.shields.io/pypi/v/python-re3data.svg?logo=pypi&label=PyPI
 [ruff]: https://github.com/astral-sh/ruff
 [ruff-badge]: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
 [scorecard-badge]: https://api.securityscorecards.dev/projects/github.com/afuetterer/python-re3data/badge
 [scorecard-url]: https://securityscorecards.dev/viewer/?uri=github.com/afuetterer/python-re3data
+[status-badge]: https://img.shields.io/pypi/status/python-re3data?logo=pypi
```

