# Comparing `tmp/click_extra-4.7.5.tar.gz` & `tmp/click_extra-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click_extra-4.7.5.tar", max compression
+gzip compressed data, was "click_extra-4.8.0.tar", max compression
```

## Comparing `click_extra-4.7.5.tar` & `click_extra-4.8.0.tar`

### file list

```diff
@@ -1,34 +1,21 @@
--rw-r--r--   0        0        0     7446 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/__init__.py
--rw-r--r--   0        0        0    31127 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/colorize.py
--rw-r--r--   0        0        0    15756 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/commands.py
--rw-r--r--   0        0        0    16508 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/config.py
--rw-r--r--   0        0        0     4069 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/decorators.py
--rw-r--r--   0        0        0     6205 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/docs_update.py
--rw-r--r--   0        0        0    11866 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/logging.py
--rw-r--r--   0        0        0    27132 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/parameters.py
--rw-r--r--   0        0        0    17269 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/platforms.py
--rw-r--r--   0        0        0        0 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/py.typed
--rw-r--r--   0        0        0     7843 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/pygments.py
--rw-r--r--   0        0        0     5057 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/sphinx.py
--rw-r--r--   0        0        0     6340 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/tabulate.py
--rw-r--r--   0        0        0     2716 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/telemetry.py
--rw-r--r--   0        0        0    23592 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/testing.py
--rw-r--r--   0        0        0      770 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/__init__.py
--rw-r--r--   0        0        0    13021 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/conftest.py
--rw-r--r--   0        0        0    26216 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_colorize.py
--rw-r--r--   0        0        0    14677 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_commands.py
--rw-r--r--   0        0        0    17030 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_config.py
--rw-r--r--   0        0        0     7216 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_logging.py
--rw-r--r--   0        0        0    21037 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_parameters.py
--rw-r--r--   0        0        0    10884 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_platforms.py
--rw-r--r--   0        0        0     8404 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_pygments.py
--rw-r--r--   0        0        0    14482 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_tabulate.py
--rw-r--r--   0        0        0     3165 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_telemetry.py
--rw-r--r--   0        0        0     8259 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_testing.py
--rw-r--r--   0        0        0     3551 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_timer.py
--rw-r--r--   0        0        0     8925 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_version.py
--rw-r--r--   0        0        0     2637 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/timer.py
--rw-r--r--   0        0        0    17760 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/version.py
--rw-r--r--   0        0        0     8981 2024-04-05 10:52:24.659415 click_extra-4.7.5/pyproject.toml
--rw-r--r--   0        0        0     6735 2024-04-05 10:52:24.659415 click_extra-4.7.5/readme.md
--rw-r--r--   0        0        0     9827 1970-01-01 00:00:00.000000 click_extra-4.7.5/PKG-INFO
+-rw-r--r--   0        0        0     7446 2024-05-23 05:59:21.196422 click_extra-4.8.0/click_extra/__init__.py
+-rw-r--r--   0        0        0    31127 2024-05-23 05:59:21.196422 click_extra-4.8.0/click_extra/colorize.py
+-rw-r--r--   0        0        0    15819 2024-05-23 05:59:21.196422 click_extra-4.8.0/click_extra/commands.py
+-rw-r--r--   0        0        0    16508 2024-05-23 05:59:21.196422 click_extra-4.8.0/click_extra/config.py
+-rw-r--r--   0        0        0     4069 2024-05-23 05:59:21.196422 click_extra-4.8.0/click_extra/decorators.py
+-rw-r--r--   0        0        0     6205 2024-05-23 05:59:21.196422 click_extra-4.8.0/click_extra/docs_update.py
+-rw-r--r--   0        0        0    11866 2024-05-23 05:59:21.196422 click_extra-4.8.0/click_extra/logging.py
+-rw-r--r--   0        0        0    27132 2024-05-23 05:59:21.200422 click_extra-4.8.0/click_extra/parameters.py
+-rw-r--r--   0        0        0    17269 2024-05-23 05:59:21.200422 click_extra-4.8.0/click_extra/platforms.py
+-rw-r--r--   0        0        0        0 2024-05-23 05:59:21.200422 click_extra-4.8.0/click_extra/py.typed
+-rw-r--r--   0        0        0     8034 2024-05-23 05:59:21.200422 click_extra-4.8.0/click_extra/pygments.py
+-rw-r--r--   0        0        0    13209 2024-05-23 05:59:21.200422 click_extra-4.8.0/click_extra/pytest.py
+-rw-r--r--   0        0        0     5237 2024-05-23 05:59:21.200422 click_extra-4.8.0/click_extra/sphinx.py
+-rw-r--r--   0        0        0     6340 2024-05-23 05:59:21.200422 click_extra-4.8.0/click_extra/tabulate.py
+-rw-r--r--   0        0        0     2716 2024-05-23 05:59:21.200422 click_extra-4.8.0/click_extra/telemetry.py
+-rw-r--r--   0        0        0    23592 2024-05-23 05:59:21.200422 click_extra-4.8.0/click_extra/testing.py
+-rw-r--r--   0        0        0     2637 2024-05-23 05:59:21.200422 click_extra-4.8.0/click_extra/timer.py
+-rw-r--r--   0        0        0    17760 2024-05-23 05:59:21.200422 click_extra-4.8.0/click_extra/version.py
+-rw-r--r--   0        0        0    10160 2024-05-23 05:59:21.204422 click_extra-4.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6735 2024-05-23 05:59:21.204422 click_extra-4.8.0/readme.md
+-rw-r--r--   0        0        0    10072 1970-01-01 00:00:00.000000 click_extra-4.8.0/PKG-INFO
```

### Comparing `click_extra-4.7.5/click_extra/__init__.py` & `click_extra-4.8.0/click_extra/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 """Expose package-wide elements."""
 
 import sys
 
-__version__ = "4.7.5"
+__version__ = "4.8.0"
 """Examples of valid version strings according :pep:`440#version-scheme`:
 
 .. code-block:: python
 
     __version__ = "1.2.3.dev1"  # Development release 1
     __version__ = "1.2.3a1"  # Alpha Release 1
     __version__ = "1.2.3b1"  # Beta Release 1
```

### Comparing `click_extra-4.7.5/click_extra/colorize.py` & `click_extra-4.8.0/click_extra/colorize.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.5/click_extra/commands.py` & `click_extra-4.8.0/click_extra/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,16 @@
     #. ``-h``, ``--help``
 
     .. todo::
         For bullet-proof handling of edge-cases, we should probably add an indirection
         layer to have the processing order of options (the one below) different from
         the presentation order of options in the help screen.
 
-        This is probably something that has been requested in {issue}`544`.
+        This is probably something that has been `requested in issue #544
+        <https://github.com/kdeldycke/click-extra/issues/544>`_.
 
     .. important::
         Sensitivity to order still remains to be proven. With the code of Click Extra
         and its dependencies moving fast, there is a non-zero chance that all the
         options are now sound enough to be re-ordered in a more natural way.
     """
     return [
```

### Comparing `click_extra-4.7.5/click_extra/config.py` & `click_extra-4.8.0/click_extra/config.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.5/click_extra/decorators.py` & `click_extra-4.8.0/click_extra/decorators.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.5/click_extra/docs_update.py` & `click_extra-4.8.0/click_extra/docs_update.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.5/click_extra/logging.py` & `click_extra-4.8.0/click_extra/logging.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.5/click_extra/parameters.py` & `click_extra-4.8.0/click_extra/parameters.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.5/click_extra/platforms.py` & `click_extra-4.8.0/click_extra/platforms.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.5/click_extra/pygments.py` & `click_extra-4.8.0/click_extra/pygments.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,22 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 """Helpers and utilities to allow Pygments to parse and render ANSI codes."""
 
 from __future__ import annotations
 
+try:
+    import pygments  # noqa: F401
+except ImportError:
+    raise ImportError(
+        "You need to install click_extra[pygments] extra dependencies to use this "
+        "module."
+    )
+
 from typing import Iterable, Iterator
 
 from pygments import lexers
 from pygments.filter import Filter
 from pygments.filters import TokenMergeFilter
 from pygments.formatter import _lookup_style  # type: ignore[attr-defined]
 from pygments.formatters import HtmlFormatter
```

### Comparing `click_extra-4.7.5/click_extra/sphinx.py` & `click_extra-4.8.0/click_extra/sphinx.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,21 +53,29 @@
     Fix the need to have both ``.. click:example::`` and ``.. click:run::`` directives
     in the same ``{eval-rst}`` block in MyST. This is required to have both directives
     shares states and context.
 """
 
 from __future__ import annotations
 
+try:
+    import sphinx  # noqa: F401
+except ImportError:
+    raise ImportError(
+        "You need to install click_extra[sphinx] extra dependencies to use this "
+        "module."
+    )
+
 from typing import Any
 
 from docutils.statemachine import ViewList
 from sphinx.highlighting import PygmentsBridge
 
 from .pygments import AnsiHtmlFormatter
-from .tests.conftest import ExtraCliRunner
+from .testing import ExtraCliRunner
 
 
 class PatchedViewList(ViewList):
     """Force the rendering of ANSI shell session.
 
     Replaces the ``.. sourcecode:: shell-session`` code block produced by
     ``.. click:run::`` directive with an ANSI Shell Session:
```

### Comparing `click_extra-4.7.5/click_extra/tabulate.py` & `click_extra-4.8.0/click_extra/tabulate.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.5/click_extra/telemetry.py` & `click_extra-4.8.0/click_extra/telemetry.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.5/click_extra/testing.py` & `click_extra-4.8.0/click_extra/testing.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.5/click_extra/tests/conftest.py` & `click_extra-4.8.0/click_extra/pytest.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,18 +9,26 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
-"""Fixtures, configuration and helpers for tests."""
+"""Pytest fixtures and marks to help testing Click CLIs."""
 
 from __future__ import annotations
 
+try:
+    import pytest  # noqa: F401
+except ImportError:
+    raise ImportError(
+        "You need to install click_extra[pytest] extra dependencies to use this "
+        "module."
+    )
+
 from typing import TYPE_CHECKING, Any
 
 import click
 import click.testing
 import cloup
 import pytest
 
@@ -59,23 +67,23 @@
 
 See:
 - https://github.com/pallets/click/issues/2111
 - https://github.com/pallets/click/issues/2110
 """
 
 
-@pytest.fixture()
+@pytest.fixture
 def extra_runner():
     """Runner fixture for ``click.testing.ExtraCliRunner``."""
     runner = ExtraCliRunner()
     with runner.isolated_filesystem():
         yield runner
 
 
-@pytest.fixture()
+@pytest.fixture
 def invoke(extra_runner):
     """Invoke fixture shorthand for ``click.testing.ExtraCliRunner.invoke``."""
     return extra_runner.invoke
 
 
 # XXX Support for decorator without parenthesis in Cloup has been reported upstream:
 # https://github.com/janluke/cloup/issues/127
@@ -184,15 +192,15 @@
         if with_types:
             args.append(deco_type)
         decorator_params.append(pytest.param(*args, id=label, marks=marks))
 
     return tuple(decorator_params)
 
 
-@pytest.fixture()
+@pytest.fixture
 def create_config(tmp_path):
     """A generic fixture to produce a temporary configuration file."""
 
     def _create_config(filename: str | Path, content: str) -> Path:
         """Create a fake configuration file."""
         config_path: Path
         if isinstance(filename, str):
```

### Comparing `click_extra-4.7.5/click_extra/timer.py` & `click_extra-4.8.0/click_extra/timer.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.5/click_extra/version.py` & `click_extra-4.8.0/click_extra/version.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.5/pyproject.toml` & `click_extra-4.8.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 # Docs: https://python-poetry.org/docs/pyproject/
 name = "click-extra"
-version = "4.7.5"
+version = "4.8.0"
 description = "🌈 Extra colorization and configuration loading for Click."
 license = 'GPL-2.0-or-later'
 authors = ["Kevin Deldycke <kevin@deldycke.com>"]
 readme = "readme.md"
 homepage = 'https://github.com/kdeldycke/click-extra'
 repository = 'https://github.com/kdeldycke/click-extra'
 documentation = 'https://kdeldycke.github.io/click-extra'
@@ -75,59 +75,82 @@
 # https://github.com/pallets/click/issues/2416
 # https://github.com/pallets/click/pull/2417
 click = "^8.1.4"
 # Cloup 3.0.5 fix incompatibility with autodoc: https://github.com/janluke/cloup/issues/177
 cloup = "^3.0.5"
 commentjson = "^0.9.0"
 mergedeep = "^1.3.4"
-# Pallets-Sphinx-Themes 2.1.1 is the first version removing old and conflicting Python 2 code.
-Pallets-Sphinx-Themes = "^2.1.1"
-# Pygments 2.14.0 is the first version with ``lexers.algebra.GAPConsoleLexer`` that is referenced in our code.
-pygments = "^2.14"
-# pygments-ansi-color 0.3.0 is the first version to set the default theme of ANSI colors.
-pygments-ansi-color = "^0.3.0"
 pyyaml = "^6.0.0"
 # regex is required for case-insensitive matches in Unicode.
 # v2023.3.22 is the first to drop Python 3.7.
-regex = "^2023.3.22"
+regex = "^2024.4.16"
 # requests 2.28.2 is the first version to support charset_normalizer 3.x.
 requests = "^2.28.2"
-# Sphinx 6 is the first version to drop Python 3.7.
-sphinx = ">=6"
 # tabulate 0.9 is the first to add `*grid` and `*outline` formats.
 tabulate = { extras = ["widechars"], version = "^0.9" }
 tomli = { version = "^2.0.1", python = "< 3.11" }
 wcmatch = "^8.5"
 xmltodict = "^0.13.0"
 
-[tool.poetry.group.dev.dependencies]
+### pygments extra group - optional dependencies
+# Pygments 2.14.0 is the first version with ``lexers.algebra.GAPConsoleLexer`` that is referenced in our code.
+pygments = { version = "^2.14", optional = true }
+# pygments-ansi-color 0.3.0 is the first version to set the default theme of ANSI colors.
+pygments-ansi-color = { version = "^0.3.0", optional = true }
+
+### sphinx extra group - optional dependencies
+# Pallets-Sphinx-Themes 2.1.1 is the first version removing old and conflicting Python 2 code.
+Pallets-Sphinx-Themes = { version = "^2.1.1", optional = true }
+# Sphinx 6 is the first version to drop Python 3.7.
+sphinx = { version = ">=6", optional = true }
+
+### pytest extra group - optional dependencies
+pytest = { version = ">=8", optional = true }
+
+[tool.poetry.extras]
+pygments = ["pygments", "pygments-ansi-color"]
+sphinx = ["pygments", "pygments-ansi-color", "Pallets-Sphinx-Themes", "sphinx"]
+pytest = ["pytest"]
+
+[tool.poetry.group.test]
+optional = true
+
+[tool.poetry.group.test.dependencies]
 coverage = { extras = ["toml"], version = "^7.2.3" }
-furo = "^2024.1.29"
-mypy = "^1.2.0"
-myst-parser = "^2.0.0"
-pytest = "^8.0.0"
 # More pytest plugins at: https://docs.pytest.org/en/latest/reference/plugin_list.html
 pytest-cases = "^3.8.3"
 pytest-cov = "^5.0.0"
 pytest-github-actions-annotate-failures = "^0.2.0"
 pytest-httpserver = "^1.0.6"
 pytest-randomly = "^3.12.0"
+
+[tool.poetry.group.typing]
+optional = true
+
+[tool.poetry.group.typing.dependencies]
+types-Pygments = "^2.15.0.0"
+types-PyYAML = "^6.0.12.9"
+types-regex = "^2024.4.16.20240423"
+types-requests = "^2.28.11.17"
+types-tabulate = "^0.9.0.2"
+types-xmltodict = "^0.13.0.2"
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+furo = "^2024.1.29"
+myst-parser = "^3.0.0"
 sphinx-autodoc-typehints = "^2.0.0"
 sphinx-copybutton = "^0.5.2"
 # sphinx-design 0.5.0 is the first to allow Sphinx 7.
 sphinx-design = "^0.5.0"
 sphinx-issues = "^4.0.0"
 sphinxext-opengraph = "^0.9.0"
 sphinxcontrib-mermaid = "^0.9"
-types-Pygments = "^2.15.0.0"
-types-PyYAML = "^6.0.12.9"
-types-regex = "^2023.3.23.1"
-types-requests = "^2.28.11.17"
-types-tabulate = "^0.9.0.2"
-types-xmltodict = "^0.13.0.2"
 
 [tool.poetry.plugins."pygments.formatters"]
 ansi-html-formatter = "click_extra.pygments:AnsiHtmlFormatter"
 
 [tool.poetry.plugins."pygments.filters"]
 ansi-filter = "click_extra.pygments:AnsiFilter"
 
@@ -148,14 +171,19 @@
 ansi-psysh-console = "click_extra.pygments:AnsiPsyshConsoleLexer"
 ansi-python-console = "click_extra.pygments:AnsiPythonConsoleLexer"
 ansi-r-console = "click_extra.pygments:AnsiRConsoleLexer"
 ansi-ruby-console = "click_extra.pygments:AnsiRubyConsoleLexer"
 ansi-sqlite-console = "click_extra.pygments:AnsiSqliteConsoleLexer"
 ansi-tcsh-session = "click_extra.pygments:AnsiTcshSessionLexer"
 
+[project.entry-points.pytest11]
+# Make additional fixtures available to pytest.
+# See: https://docs.pytest.org/en/latest/how-to/writing_plugins.html#making-your-plugin-installable-by-others
+click-extra = "click_extra.pytest"
+
 [tool.mypy]
 warn_unused_configs = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_return_any = true
 warn_unreachable = true
 pretty = true
@@ -168,29 +196,38 @@
     "furo",
     "mergedeep.*",
     "pallets_sphinx_themes.*",
 ]
 
 [tool.pytest.ini_options]
 # https://docs.pytest.org/en/latest/customize.html#pyproject-toml
-# --cov-config=pyproject.toml : is specified at CLI level instead of letting coverage find it because of this bug:
-#   https://github.com/nedbat/coveragepy/issues/512#issuecomment-399707938
-#   https://github.com/pytest-dev/pytest-cov/issues/168#issuecomment-327533847
-#   https://github.com/pytest-dev/pytest-cov/issues/243
-addopts = "--durations=10 --cov-report=term --cov-report=xml --cov-config=pyproject.toml --cov=click_extra"
+addopts = [
+    "--durations=10",
+    "--cov-report=term",
+    "--cov-report=xml",
+    # --cov-config=pyproject.toml : is specified at CLI level instead of letting coverage find it because of this bug:
+    #   https://github.com/nedbat/coveragepy/issues/512#issuecomment-399707938
+    #   https://github.com/pytest-dev/pytest-cov/issues/168#issuecomment-327533847
+    #   https://github.com/pytest-dev/pytest-cov/issues/243
+    "--cov-config=pyproject.toml",
+    "--cov=click_extra",
+    # See: https://docs.pytest.org/en/latest/explanation/goodpractices.html#tests-outside-application-code
+    "--import-mode=importlib",
+]
+# Make sure tests that are expected to fail do not resurect and start working all of a sudden.
 xfail_strict = true
 
 # https://coverage.readthedocs.io/en/latest/config.html
 [tool.coverage.run]
 branch = true
 [tool.coverage.report]
 precision = 2
 
 [tool.bumpversion]
-current_version = "4.7.5"
+current_version = "4.8.0"
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 # Update Python package version in any __init__.py file.
 glob = "./**/__init__.py"
 ignore_missing_version = true
```

### Comparing `click_extra-4.7.5/readme.md` & `click_extra-4.8.0/readme.md`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.5/PKG-INFO` & `click_extra-4.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-extra
-Version: 4.7.5
+Version: 4.8.0
 Summary: 🌈 Extra colorization and configuration loading for Click.
 Home-page: https://github.com/kdeldycke/click-extra
 License: GPL-2.0-or-later
 Keywords: ansi-colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-tabulate,sphinx,terminal,toml,xml,yaml
 Author: Kevin Deldycke
 Author-email: kevin@deldycke.com
 Requires-Python: >=3.8,<4.0
@@ -36,26 +36,30 @@
 Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: Topic :: Text Processing :: Markup :: reStructuredText
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Dist: Pallets-Sphinx-Themes (>=2.1.1,<3.0.0)
+Provides-Extra: pygments
+Provides-Extra: pytest
+Provides-Extra: sphinx
+Requires-Dist: Pallets-Sphinx-Themes (>=2.1.1,<3.0.0) ; extra == "sphinx"
 Requires-Dist: boltons (>=24.0.0,<25.0.0)
 Requires-Dist: click (>=8.1.4,<9.0.0)
 Requires-Dist: cloup (>=3.0.5,<4.0.0)
 Requires-Dist: commentjson (>=0.9.0,<0.10.0)
 Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
-Requires-Dist: pygments (>=2.14,<3.0)
-Requires-Dist: pygments-ansi-color (>=0.3.0,<0.4.0)
+Requires-Dist: pygments (>=2.14,<3.0) ; extra == "pygments" or extra == "sphinx"
+Requires-Dist: pygments-ansi-color (>=0.3.0,<0.4.0) ; extra == "pygments" or extra == "sphinx"
+Requires-Dist: pytest (>=8) ; extra == "pytest"
 Requires-Dist: pyyaml (>=6.0.0,<7.0.0)
-Requires-Dist: regex (>=2023.3.22,<2024.0.0)
+Requires-Dist: regex (>=2024.4.16,<2025.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: sphinx (>=6)
+Requires-Dist: sphinx (>=6) ; extra == "sphinx"
 Requires-Dist: tabulate[widechars] (>=0.9,<0.10)
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
 Requires-Dist: wcmatch (>=8.5,<9.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Project-URL: Changelog, https://kdeldycke.github.io/click-extra/changelog.html
 Project-URL: Documentation, https://kdeldycke.github.io/click-extra
 Project-URL: Funding, https://github.com/sponsors/kdeldycke
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: click-extra Version: 4.7.5 Summary: ð Extra
+Metadata-Version: 2.1 Name: click-extra Version: 4.8.0 Summary: ð Extra
 colorization and configuration loading for Click. Home-page: https://
 github.com/kdeldycke/click-extra License: GPL-2.0-or-later Keywords: ansi-
 colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-
 tabulate,sphinx,terminal,toml,xml,yaml Author: Kevin Deldycke Author-email:
 kevin@deldycke.com Requires-Python: >=3.8,<4.0 Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Environment :: Plugins Classifier: Framework :: Pytest Classifier: Framework ::
@@ -20,24 +20,27 @@
 Libraries :: Python Modules Classifier: Topic :: Software Development :: User
 Interfaces Classifier: Topic :: System :: Logging Classifier: Topic :: System
 :: Shells Classifier: Topic :: Terminals Classifier: Topic :: Text Processing
 :: Filters Classifier: Topic :: Text Processing :: Markup :: HTML Classifier:
 Topic :: Text Processing :: Markup :: Markdown Classifier: Topic :: Text
 Processing :: Markup :: XML Classifier: Topic :: Text Processing :: Markup ::
 reStructuredText Classifier: Topic :: Utilities Classifier: Typing :: Typed
-Requires-Dist: Pallets-Sphinx-Themes (>=2.1.1,<3.0.0) Requires-Dist: boltons
-(>=24.0.0,<25.0.0) Requires-Dist: click (>=8.1.4,<9.0.0) Requires-Dist: cloup
-(>=3.0.5,<4.0.0) Requires-Dist: commentjson (>=0.9.0,<0.10.0) Requires-Dist:
-mergedeep (>=1.3.4,<2.0.0) Requires-Dist: pygments (>=2.14,<3.0) Requires-Dist:
-pygments-ansi-color (>=0.3.0,<0.4.0) Requires-Dist: pyyaml (>=6.0.0,<7.0.0)
-Requires-Dist: regex (>=2023.3.22,<2024.0.0) Requires-Dist: requests
-(>=2.28.2,<3.0.0) Requires-Dist: sphinx (>=6) Requires-Dist: tabulate
-[widechars] (>=0.9,<0.10) Requires-Dist: tomli (>=2.0.1,<3.0.0) ;
-python_version < "3.11" Requires-Dist: wcmatch (>=8.5,<9.0) Requires-Dist:
-xmltodict (>=0.13.0,<0.14.0) Project-URL: Changelog, https://
+Provides-Extra: pygments Provides-Extra: pytest Provides-Extra: sphinx
+Requires-Dist: Pallets-Sphinx-Themes (>=2.1.1,<3.0.0) ; extra == "sphinx"
+Requires-Dist: boltons (>=24.0.0,<25.0.0) Requires-Dist: click (>=8.1.4,<9.0.0)
+Requires-Dist: cloup (>=3.0.5,<4.0.0) Requires-Dist: commentjson
+(>=0.9.0,<0.10.0) Requires-Dist: mergedeep (>=1.3.4,<2.0.0) Requires-Dist:
+pygments (>=2.14,<3.0) ; extra == "pygments" or extra == "sphinx" Requires-
+Dist: pygments-ansi-color (>=0.3.0,<0.4.0) ; extra == "pygments" or extra ==
+"sphinx" Requires-Dist: pytest (>=8) ; extra == "pytest" Requires-Dist: pyyaml
+(>=6.0.0,<7.0.0) Requires-Dist: regex (>=2024.4.16,<2025.0.0) Requires-Dist:
+requests (>=2.28.2,<3.0.0) Requires-Dist: sphinx (>=6) ; extra == "sphinx"
+Requires-Dist: tabulate[widechars] (>=0.9,<0.10) Requires-Dist: tomli
+(>=2.0.1,<3.0.0) ; python_version < "3.11" Requires-Dist: wcmatch (>=8.5,<9.0)
+Requires-Dist: xmltodict (>=0.13.0,<0.14.0) Project-URL: Changelog, https://
 kdeldycke.github.io/click-extra/changelog.html Project-URL: Documentation,
 https://kdeldycke.github.io/click-extra Project-URL: Funding, https://
 github.com/sponsors/kdeldycke Project-URL: Issues, https://github.com/
 kdeldycke/click-extra/issues Project-URL: Repository, https://github.com/
 kdeldycke/click-extra Description-Content-Type: text/markdown
                                  _[_C_l_i_c_k_ _E_x_t_r_a_]
 [![Last release](https://img.shields.io/pypi/v/click-extra.svg)](https://
```

