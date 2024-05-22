# Comparing `tmp/sphinx_design-0.5.0.tar.gz` & `tmp/sphinx_design-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_design-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinx_design-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_design-0.5.0.tar` & `sphinx_design-0.6.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      600 2023-07-27 12:45:22.648600 sphinx_design-0.5.0/.github/dependabot.yml
--rw-r--r--   0        0        0     3132 2023-07-27 12:45:22.648600 sphinx_design-0.5.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2081 2023-07-27 12:45:22.648600 sphinx_design-0.5.0/.gitignore
--rw-r--r--   0        0        0     1224 2023-07-27 12:45:22.648600 sphinx_design-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      177 2023-07-27 12:45:22.648600 sphinx_design-0.5.0/.readthedocs.yml
--rw-r--r--   0        0        0     8257 2023-07-27 12:45:22.648600 sphinx_design-0.5.0/CHANGELOG.md
--rw-r--r--   0        0        0     1099 2023-07-27 12:45:22.648600 sphinx_design-0.5.0/LICENSE
--rw-r--r--   0        0        0     3114 2023-07-27 12:45:22.648600 sphinx_design-0.5.0/README.md
--rw-r--r--   0        0        0      162 2023-07-27 12:45:22.648600 sphinx_design-0.5.0/codecov.yml
--rwxr-xr-x   0        0        0      214 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/git_rebase_theme_branches.sh
--rw-r--r--   0        0        0    11363 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/package-lock.json
--rw-r--r--   0        0        0      302 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/package.json
--rw-r--r--   0        0        0     2078 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      433 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/sphinx_design/__init__.py
--rw-r--r--   0        0        0      722 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/sphinx_design/_compat.py
--rw-r--r--   0        0        0     6410 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/sphinx_design/article_info.py
--rw-r--r--   0        0        0     8252 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/sphinx_design/badges_buttons.py
--rw-r--r--   0        0        0    10377 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/sphinx_design/cards.py
--rw-r--r--   0        0        0        0 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/sphinx_design/compiled/__init__.py
--rw-r--r--   0        0        0      577 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/sphinx_design/compiled/material-icons_LICENSE
--rw-r--r--   0        0        0      106 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/sphinx_design/compiled/material-icons_VERSION.txt
--rw-r--r--   0        0        0  1613646 2023-07-27 12:45:22.668600 sphinx_design-0.5.0/sphinx_design/compiled/material_outlined.json
--rw-r--r--   0        0        0  1504323 2023-07-27 12:45:22.672600 sphinx_design-0.5.0/sphinx_design/compiled/material_regular.json
--rw-r--r--   0        0        0  2003117 2023-07-27 12:45:22.680601 sphinx_design-0.5.0/sphinx_design/compiled/material_round.json
--rw-r--r--   0        0        0  1370513 2023-07-27 12:45:22.680601 sphinx_design-0.5.0/sphinx_design/compiled/material_sharp.json
--rw-r--r--   0        0        0  1995382 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/compiled/material_twotone.json
--rw-r--r--   0        0        0     1068 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/compiled/octicon_LICENSE
--rw-r--r--   0        0        0   277166 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/compiled/octicons.json
--rw-r--r--   0        0        0      770 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/compiled/sd_tabs.js
--rw-r--r--   0        0        0    48417 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/compiled/style.min.css
--rw-r--r--   0        0        0     7822 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/dropdown.py
--rw-r--r--   0        0        0     5614 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/extension.py
--rw-r--r--   0        0        0     9839 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/grids.py
--rw-r--r--   0        0        0    10620 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/icons.py
--rw-r--r--   0        0        0       26 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/py.typed
--rw-r--r--   0        0        0     3117 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/shared.py
--rw-r--r--   0        0        0     9681 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/tabs.py
--rw-r--r--   0        0        0     2046 2023-07-27 12:45:22.688601 sphinx_design-0.5.0/tox.ini
--rw-r--r--   0        0        0     5088 1970-01-01 00:00:00.000000 sphinx_design-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      600 2024-05-22 23:12:12.811831 sphinx_design-0.6.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     3177 2024-05-22 23:12:12.811831 sphinx_design-0.6.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2081 2024-05-22 23:12:12.811831 sphinx_design-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1278 2024-05-22 23:12:12.811831 sphinx_design-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      214 2024-05-22 23:12:12.811831 sphinx_design-0.6.0/.readthedocs.yml
+-rw-r--r--   0        0        0     7834 2024-05-22 23:12:12.811831 sphinx_design-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1099 2024-05-22 23:12:12.811831 sphinx_design-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3093 2024-05-22 23:12:12.811831 sphinx_design-0.6.0/README.md
+-rw-r--r--   0        0        0      162 2024-05-22 23:12:12.815831 sphinx_design-0.6.0/codecov.yml
+-rwxr-xr-x   0        0        0      214 2024-05-22 23:12:12.815831 sphinx_design-0.6.0/git_rebase_theme_branches.sh
+-rw-r--r--   0        0        0    11363 2024-05-22 23:12:12.819831 sphinx_design-0.6.0/package-lock.json
+-rw-r--r--   0        0        0      302 2024-05-22 23:12:12.819831 sphinx_design-0.6.0/package.json
+-rw-r--r--   0        0        0     2765 2024-05-22 23:12:12.819831 sphinx_design-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      434 2024-05-22 23:12:12.819831 sphinx_design-0.6.0/sphinx_design/__init__.py
+-rw-r--r--   0        0        0      750 2024-05-22 23:12:12.819831 sphinx_design-0.6.0/sphinx_design/_compat.py
+-rw-r--r--   0        0        0     6366 2024-05-22 23:12:12.819831 sphinx_design-0.6.0/sphinx_design/article_info.py
+-rw-r--r--   0        0        0     8212 2024-05-22 23:12:12.819831 sphinx_design-0.6.0/sphinx_design/badges_buttons.py
+-rw-r--r--   0        0        0    10386 2024-05-22 23:12:12.819831 sphinx_design-0.6.0/sphinx_design/cards.py
+-rw-r--r--   0        0        0        0 2024-05-22 23:12:12.819831 sphinx_design-0.6.0/sphinx_design/compiled/__init__.py
+-rw-r--r--   0        0        0      577 2024-05-22 23:12:12.819831 sphinx_design-0.6.0/sphinx_design/compiled/material-icons_LICENSE
+-rw-r--r--   0        0        0      106 2024-05-22 23:12:12.819831 sphinx_design-0.6.0/sphinx_design/compiled/material-icons_VERSION.txt
+-rw-r--r--   0        0        0  1613646 2024-05-22 23:12:12.831831 sphinx_design-0.6.0/sphinx_design/compiled/material_outlined.json
+-rw-r--r--   0        0        0  1504323 2024-05-22 23:12:12.835831 sphinx_design-0.6.0/sphinx_design/compiled/material_regular.json
+-rw-r--r--   0        0        0  2003117 2024-05-22 23:12:12.839831 sphinx_design-0.6.0/sphinx_design/compiled/material_round.json
+-rw-r--r--   0        0        0  1370513 2024-05-22 23:12:12.843831 sphinx_design-0.6.0/sphinx_design/compiled/material_sharp.json
+-rw-r--r--   0        0        0  1995382 2024-05-22 23:12:12.843831 sphinx_design-0.6.0/sphinx_design/compiled/material_twotone.json
+-rw-r--r--   0        0        0     1068 2024-05-22 23:12:12.843831 sphinx_design-0.6.0/sphinx_design/compiled/octicon_LICENSE
+-rw-r--r--   0        0        0  1016739 2024-05-22 23:12:12.847831 sphinx_design-0.6.0/sphinx_design/compiled/octicons.json
+-rw-r--r--   0        0        0     2780 2024-05-22 23:12:12.847831 sphinx_design-0.6.0/sphinx_design/compiled/sd_tabs.js
+-rw-r--r--   0        0        0    49341 2024-05-22 23:12:12.847831 sphinx_design-0.6.0/sphinx_design/compiled/style.min.css
+-rw-r--r--   0        0        0     8007 2024-05-22 23:12:12.847831 sphinx_design-0.6.0/sphinx_design/dropdown.py
+-rw-r--r--   0        0        0     6690 2024-05-22 23:12:12.847831 sphinx_design-0.6.0/sphinx_design/extension.py
+-rw-r--r--   0        0        0     9773 2024-05-22 23:12:12.847831 sphinx_design-0.6.0/sphinx_design/grids.py
+-rw-r--r--   0        0        0    10823 2024-05-22 23:12:12.847831 sphinx_design-0.6.0/sphinx_design/icons.py
+-rw-r--r--   0        0        0       26 2024-05-22 23:12:12.847831 sphinx_design-0.6.0/sphinx_design/py.typed
+-rw-r--r--   0        0        0     7009 2024-05-22 23:12:12.847831 sphinx_design-0.6.0/sphinx_design/shared.py
+-rw-r--r--   0        0        0    10155 2024-05-22 23:12:12.847831 sphinx_design-0.6.0/sphinx_design/tabs.py
+-rw-r--r--   0        0        0     1273 2024-05-22 23:12:12.851831 sphinx_design-0.6.0/tox.ini
+-rw-r--r--   0        0        0     5204 1970-01-01 00:00:00.000000 sphinx_design-0.6.0/PKG-INFO
```

### Comparing `sphinx_design-0.5.0/.github/dependabot.yml` & `sphinx_design-0.6.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.5.0/.github/workflows/ci.yml` & `sphinx_design-0.6.0/.github/workflows/ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -10,74 +10,75 @@
 jobs:
 
   pre-commit:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
-    - name: Set up Python 3.8
+    - uses: actions/checkout@v4
+    - name: Set up Python 3.9
       uses: actions/setup-python@v4
       with:
-        python-version: 3.8
-    - uses: pre-commit/action@v3.0.0
+        python-version: 3.9
+    - uses: pre-commit/action@v3.0.1
 
   tests:
 
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest]
-        python-version: ["3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.9", "3.10", "3.11", "3.12"]
         sphinx-version: ["~=7.0"]
         include:
         - os: ubuntu-latest
-          python-version: 3.8
+          python-version: 3.9
           sphinx-version: "~=5.0"
         - os: ubuntu-latest
-          python-version: 3.8
+          python-version: 3.9
           sphinx-version: "~=6.0"
         - os: windows-latest
-          python-version: 3.8
+          python-version: 3.9
           sphinx-version: "~=7.0"
 
     runs-on: ${{ matrix.os }}
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
         cache: pip
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install --upgrade "sphinx${{ matrix.sphinx-version }}" -e .[testing]
     - name: Run pytest
       run: |
         pytest --cov=sphinx_design --cov-report=xml --cov-report=term-missing
     - name: Upload to Codecov
-      if: matrix.python-version == '3.8' && matrix.os == 'ubuntu-latest'
+      if: matrix.python-version == '3.9' && matrix.os == 'ubuntu-latest'
       uses: codecov/codecov-action@v3
       with:
+        token: ${{ secrets.CODECOV_TOKEN }}
         name: pytests
         flags: pytests
         file: ./coverage.xml
         fail_ci_if_error: true
 
   docs-build-format:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
         format: [html, latex, man]
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python 3.9
       uses: actions/setup-python@v4
       with:
         python-version: "3.9"
         cache: pip
     - name: Install dependencies
       run: |
@@ -108,19 +109,19 @@
 
     name: Publish to PyPi
     needs: [pre-commit, tests]
     if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
     runs-on: ubuntu-latest
     steps:
     - name: Checkout source
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: 3.9
     - name: install flit
       run: |
         pip install flit~=3.4
     - name: Build and publish
       run: |
         flit publish
       env:
```

### Comparing `sphinx_design-0.5.0/.gitignore` & `sphinx_design-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.5.0/.pre-commit-config.yaml` & `sphinx_design-0.6.0/.pre-commit-config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -7,39 +7,30 @@
       tests/.*xml|
       tests/.*txt|
     )$
 
 repos:
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
     - id: check-json
     - id: check-yaml
     - id: end-of-file-fixer
     - id: trailing-whitespace
 
-  - repo: https://github.com/pycqa/isort
-    rev: 5.12.0
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.4.4
     hooks:
-    - id: isort
-
-  - repo: https://github.com/psf/black
-    rev: 23.7.0
-    hooks:
-    - id: black
-
-  - repo: https://github.com/PyCQA/flake8
-    rev: 6.0.0
-    hooks:
-    - id: flake8
-      additional_dependencies: [flake8-bugbear~=22.7]
+    - id: ruff
+      args: [--fix]
+    - id: ruff-format
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.4.1
+    rev: v1.10.0
     hooks:
     - id: mypy
       additional_dependencies: []
 
   - repo: local
     hooks:
     - id: css
@@ -49,7 +40,17 @@
       language: node
       additional_dependencies: ['sass@1.35.2']
       # entry: sass
       entry: npm run css
       require_serial: true
       pass_filenames: false
       # args: [--style=compressed, --no-source-map, style/index.scss, sphinx_design/compiled/style.min.css]
+
+    - id: tsc
+      name: tsc (jsdoc)
+      entry: tsc
+      language: node
+      files: \.(js)$
+      types_or: [javascript]
+      args: [--allowJs, --noEmit, --strict]
+      additional_dependencies:
+      - typescript
```

### Comparing `sphinx_design-0.5.0/LICENSE` & `sphinx_design-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.5.0/README.md` & `sphinx_design-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,14 @@
 
 Use autoprefixer when compiling SASS (see <https://getbootstrap.com/docs/5.0/getting-started/browsers-devices/#supported-browsers>)
 
 horizontal card (grid row inside card, picture on left)
 
 subtitle for card (see <https://material.io/components/cards#anatomy>)
 
-rtd PRs not working
-
 
 [github-ci]: https://github.com/executablebooks/sphinx-design/workflows/continuous-integration/badge.svg?branch=main
 [github-link]: https://github.com/executablebooks/sphinx-design
 [codecov-badge]: https://codecov.io/gh/executablebooks/sphinx-design/branch/main/graph/badge.svg
 [codecov-link]: https://codecov.io/gh/executablebooks/sphinx-design
 [pypi-badge]: https://img.shields.io/pypi/v/sphinx-design.svg
 [pypi-link]: https://pypi.org/project/sphinx-design
```

### Comparing `sphinx_design-0.5.0/package-lock.json` & `sphinx_design-0.6.0/package-lock.json`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.5.0/sphinx_design/_compat.py` & `sphinx_design-0.6.0/sphinx_design/_compat.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Helpers for cross compatibility across dependency versions."""
+
+from collections.abc import Iterable
 from importlib import resources
-from typing import Callable, Iterable
+from typing import Callable
 
 from docutils.nodes import Element
 
 
 def findall(node: Element) -> Callable[..., Iterable[Element]]:
     """Iterate through"""
     # findall replaces traverse in docutils v0.18
```

### Comparing `sphinx_design-0.5.0/sphinx_design/article_info.py` & `sphinx_design-0.6.0/sphinx_design/article_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-from typing import List, Optional
+from typing import Optional
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from sphinx.application import Sphinx
-from sphinx.util.docutils import SphinxDirective
 
 from .icons import get_octicon
-from .shared import SEMANTIC_COLORS, create_component, make_choice
+from .shared import SEMANTIC_COLORS, SdDirective, create_component, make_choice
 
 
 def setup_article_info(app: Sphinx):
     """Setup the article information components."""
     app.add_directive("article-info", ArticleInfoDirective)
 
 
-class ArticleInfoDirective(SphinxDirective):
+class ArticleInfoDirective(SdDirective):
     """ """
 
     has_content = False
     required_arguments = 0
     optional_arguments = 0
     option_spec = {
         "avatar": directives.uri,
@@ -44,28 +43,27 @@
             # note certain nodes (like references) need to be nested in a TextElement node
             # (e.g. a pargraph)
             para = nodes.paragraph("", "", *text_nodes, classes=["sd-p-0", "sd-m-0"])
             self.set_source_info(para)
             output = [para]
         return output
 
-    def run(self) -> List[nodes.Node]:
-        """Run the directive."""
+    def run_with_defaults(self) -> list[nodes.Node]:  # noqa: PLR0915
         parse_fields = True  # parse field text
 
         top_grid = create_component(
             "grid-container",
             [
                 "sd-container-fluid",
                 "sd-sphinx-override",
                 "sd-p-0",
                 "sd-mt-2",
                 "sd-mb-4",
-            ]
-            + self.options.get("class-container", []),
+                *self.options.get("class-container", []),
+            ],
         )
         self.set_source_info(top_grid)
 
         top_row = create_component(
             "grid-row",
             ["sd-row", "sd-row-cols-2", "sd-gx-2", "sd-gy-1"],
         )
```

### Comparing `sphinx_design-0.5.0/sphinx_design/badges_buttons.py` & `sphinx_design-0.6.0/sphinx_design/badges_buttons.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import List, Optional, Tuple
+from typing import Optional
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from sphinx import addnodes
 from sphinx.application import Sphinx
-from sphinx.util.docutils import ReferenceRole, SphinxDirective, SphinxRole
+from sphinx.util.docutils import ReferenceRole, SphinxRole
 
-from sphinx_design.shared import SEMANTIC_COLORS, make_choice, text_align
+from sphinx_design.shared import SEMANTIC_COLORS, SdDirective, make_choice, text_align
 
 ROLE_NAME_BADGE_PREFIX = "bdg"
 ROLE_NAME_LINK_PREFIX = "bdg-link"
 ROLE_NAME_REF_PREFIX = "bdg-ref"
 DIRECTIVE_NAME_BUTTON_LINK = "button-link"
 DIRECTIVE_NAME_BUTTON_REF = "button-ref"
 
@@ -41,15 +41,15 @@
             XRefBadgeRole(color, outline=True),
         )
 
     app.add_directive(DIRECTIVE_NAME_BUTTON_LINK, ButtonLinkDirective)
     app.add_directive(DIRECTIVE_NAME_BUTTON_REF, ButtonRefDirective)
 
 
-def create_bdg_classes(color: Optional[str], outline: bool) -> List[str]:
+def create_bdg_classes(color: Optional[str], outline: bool) -> list[str]:
     """Create the badge classes."""
     classes = [
         "sd-sphinx-override",
         "sd-badge",
     ]
     if color is None:
         return classes
@@ -64,15 +64,15 @@
     """Role to display a badge."""
 
     def __init__(self, color: Optional[str] = None, *, outline: bool = False) -> None:
         super().__init__()
         self.color = color
         self.outline = outline
 
-    def run(self) -> Tuple[List[nodes.Node], List[nodes.system_message]]:
+    def run(self) -> tuple[list[nodes.Node], list[nodes.system_message]]:
         """Run the role."""
         node = nodes.inline(
             self.rawtext,
             self.text,
             classes=create_bdg_classes(self.color, self.outline),
         )
         self.set_source_info(node)
@@ -83,15 +83,15 @@
     """Role to display a badge with an external link."""
 
     def __init__(self, color: Optional[str] = None, *, outline: bool = False) -> None:
         super().__init__()
         self.color = color
         self.outline = outline
 
-    def run(self) -> Tuple[List[nodes.Node], List[nodes.system_message]]:
+    def run(self) -> tuple[list[nodes.Node], list[nodes.system_message]]:
         """Run the role."""
         node = nodes.reference(
             self.rawtext,
             refuri=self.target,
             classes=create_bdg_classes(self.color, self.outline),
         )
         # TODO open in new tab
@@ -106,15 +106,15 @@
     """Role to display a badge with an internal link."""
 
     def __init__(self, color: Optional[str] = None, *, outline: bool = False) -> None:
         super().__init__()
         self.color = color
         self.outline = outline
 
-    def run(self) -> Tuple[List[nodes.Node], List[nodes.system_message]]:
+    def run(self) -> tuple[list[nodes.Node], list[nodes.system_message]]:
         """Run the role."""
         options = {
             "classes": create_bdg_classes(self.color, self.outline),
             "reftarget": self.target,
             "refdoc": self.env.docname,
             "refdomain": "",
             "reftype": "any",
@@ -123,15 +123,15 @@
         }
         node = addnodes.pending_xref(self.rawtext, **options)
         self.set_source_info(node)
         node += nodes.inline(self.title, self.title, classes=["xref", "any"])
         return [node], []
 
 
-class _ButtonDirective(SphinxDirective):
+class _ButtonDirective(SdDirective):
     """A base button directive."""
 
     required_arguments = 1
     optional_arguments = 0
     final_argument_whitespace = True
     has_content = True
     option_spec = {
@@ -146,21 +146,20 @@
         "shadow": directives.flag,
         # ref button only
         "ref-type": make_choice(["any", "ref", "doc", "myst"]),
         "class": directives.class_option,
     }
 
     def create_ref_node(
-        self, rawtext: str, target: str, explicit_title: bool, classes: List[str]
+        self, rawtext: str, target: str, explicit_title: bool, classes: list[str]
     ) -> nodes.Node:
         """Create the reference node."""
         raise NotImplementedError
 
-    def run(self) -> List[nodes.Node]:
-        """Run the directive."""
+    def run_with_defaults(self) -> list[nodes.Node]:
         rawtext = self.arguments[0]
         target = directives.uri(rawtext)
         classes = ["sd-sphinx-override", "sd-btn", "sd-text-wrap"]
         if "color" in self.options:
             if "outline" in self.options:
                 classes.append(f"sd-btn-outline-{self.options['color']}")
             else:
@@ -201,29 +200,29 @@
         return [container]
 
 
 class ButtonLinkDirective(_ButtonDirective):
     """A button directive with an external link."""
 
     def create_ref_node(
-        self, rawtext: str, target: str, explicit_title: bool, classes: List[str]
+        self, rawtext: str, target: str, explicit_title: bool, classes: list[str]
     ) -> nodes.Node:
         """Create the reference node."""
         return nodes.reference(
             rawtext,
             refuri=target,
             classes=classes,
         )
 
 
 class ButtonRefDirective(_ButtonDirective):
     """A button directive with an internal link."""
 
     def create_ref_node(
-        self, rawtext: str, target: str, explicit_title: bool, classes: List[str]
+        self, rawtext: str, target: str, explicit_title: bool, classes: list[str]
     ) -> nodes.Node:
         """Create the reference node."""
         ref_type = self.options.get("ref-type", "any")
         options = {
             # TODO the presence of classes raises an error if the link cannot be found
             "classes": classes,
             "reftarget": target,
```

### Comparing `sphinx_design-0.5.0/sphinx_design/cards.py` & `sphinx_design-0.6.0/sphinx_design/cards.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import re
-from typing import List, NamedTuple, Optional, Tuple
+from typing import NamedTuple, Optional
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from docutils.statemachine import StringList
 from sphinx import addnodes
 from sphinx.application import Sphinx
 from sphinx.util.docutils import SphinxDirective
 from sphinx.util.logging import getLogger
 
 from ._compat import findall
 from .shared import (
     WARNING_TYPE,
     PassthroughTextElement,
+    SdDirective,
     create_component,
     is_component,
     make_choice,
     margin_option,
     text_align,
 )
 
@@ -36,20 +37,20 @@
 
 class CardContent(NamedTuple):
     """Split card into header (optional), body, footer (optional).
 
     (offset, content)
     """
 
-    body: Tuple[int, StringList]
-    header: Optional[Tuple[int, StringList]] = None
-    footer: Optional[Tuple[int, StringList]] = None
+    body: tuple[int, StringList]
+    header: Optional[tuple[int, StringList]] = None
+    footer: Optional[tuple[int, StringList]] = None
 
 
-class CardDirective(SphinxDirective):
+class CardDirective(SdDirective):
     """A card component."""
 
     has_content = True
     required_arguments = 0
     optional_arguments = 1  # card title
     final_argument_whitespace = True
     option_spec = {
@@ -69,19 +70,19 @@
         "class-body": directives.class_option,
         "class-title": directives.class_option,
         "class-footer": directives.class_option,
         "class-img-top": directives.class_option,
         "class-img-bottom": directives.class_option,
     }
 
-    def run(self) -> List[nodes.Node]:
+    def run_with_defaults(self) -> list[nodes.Node]:
         return [self.create_card(self, self.arguments, self.options)]
 
     @classmethod
-    def create_card(
+    def create_card(  # noqa: PLR0915
         cls, inst: SphinxDirective, arguments: Optional[list], options: dict
     ) -> nodes.Node:
         """Run the directive."""
         # TODO better degradation for latex
         card_classes = ["sd-card", "sd-sphinx-override"]
         if "width" in options:
             card_classes += [f'sd-w-{options["width"].rstrip("%")}']
@@ -114,15 +115,15 @@
             container = overlay
 
         if "img-top" in options:
             image_top = nodes.image(
                 "",
                 uri=options["img-top"],
                 alt=img_alt,
-                classes=["sd-card-img-top"] + options.get("class-img-top", []),
+                classes=["sd-card-img-top", *options.get("class-img-top", [])],
             )
             container.append(image_top)
 
         components = cls.split_content(inst.content, inst.content_offset)
 
         if components.header:
             container.append(
@@ -133,16 +134,19 @@
 
         body = cls._create_component(
             inst, "body", options, components.body[0], components.body[1]
         )
         if arguments:
             title = create_component(
                 "card-title",
-                ["sd-card-title", "sd-font-weight-bold"]
-                + options.get("class-title", []),
+                [
+                    "sd-card-title",
+                    "sd-font-weight-bold",
+                    *options.get("class-title", []),
+                ],
             )
             textnodes, _ = inst.state.inline_text(arguments[0], inst.lineno)
             title_container = PassthroughTextElement()
             title_container.extend(textnodes)
             inst.set_source_info(title_container)
             title.append(title_container)
             body.insert(0, title)
@@ -156,42 +160,39 @@
             )
 
         if "img-bottom" in options:
             image_bottom = nodes.image(
                 "",
                 uri=options["img-bottom"],
                 alt=img_alt,
-                classes=["sd-card-img-bottom"] + options.get("class-img-bottom", []),
+                classes=["sd-card-img-bottom", *options.get("class-img-bottom", [])],
             )
             container.append(image_bottom)
 
         if "link" in options:
             link_container = PassthroughTextElement()
-            _classes = ["sd-stretched-link"]
-            _rawtext = options.get("link-alt") or ""
-            if options.get("link-alt"):
-                _classes.append("sd-hide-link-text")
+            _classes = ["sd-stretched-link", "sd-hide-link-text"]
+            _rawtext = options.get("link-alt") or options["link"]
             if options.get("link-type", "url") == "url":
                 link = nodes.reference(
                     _rawtext,
                     "",
+                    nodes.inline(_rawtext, _rawtext),
                     refuri=options["link"],
                     classes=_classes,
                 )
-                if options.get("link-alt"):
-                    link.append(nodes.inline(_rawtext, _rawtext))
             else:
                 options = {
                     # TODO the presence of classes raises an error if the link cannot be found
                     "classes": _classes,
                     "reftarget": options["link"],
                     "refdoc": inst.env.docname,
                     "refdomain": "" if options["link-type"] == "any" else "std",
                     "reftype": options["link-type"],
-                    "refexplicit": True,
+                    "refexplicit": "link-alt" in options,
                     "refwarn": True,
                 }
                 link = addnodes.pending_xref(
                     _rawtext, nodes.inline(_rawtext, _rawtext), **options
                 )
             inst.set_source_info(link)
             link_container += link
@@ -221,67 +222,68 @@
             content[
                 (header_index + 1 if header_index is not None else None) : footer_index
             ],
         )
         return CardContent(body, header, footer)
 
     @classmethod
-    def _create_component(
+    def _create_component(  # noqa: PLR0913
         cls,
         inst: SphinxDirective,
         name: str,
         options: dict,
         offset: int,
         content: StringList,
     ) -> nodes.container:
         """Create the header, body, or footer."""
         component = create_component(
-            f"card-{name}", [f"sd-card-{name}"] + options.get(f"class-{name}", [])
+            f"card-{name}", [f"sd-card-{name}", *options.get(f"class-{name}", [])]
         )
         inst.set_source_info(component)  # TODO set proper lines
         inst.state.nested_parse(content, offset, component)
         cls.add_card_child_classes(component)
         return component
 
     @staticmethod
     def add_card_child_classes(node):
         """Add classes to specific child nodes."""
         for para in findall(node)(nodes.paragraph):
-            para["classes"] = ([] if "classes" not in para else para["classes"]) + [
-                "sd-card-text"
-            ]
+            para["classes"] = [*para.get("classes", []), "sd-card-text"]
         # for title in findall(node)(nodes.title):
         #     title["classes"] = ([] if "classes" not in title else title["classes"]) + [
         #         "sd-card-title"
         #     ]
 
 
-class CardCarouselDirective(SphinxDirective):
+class CardCarouselDirective(SdDirective):
     """A component, which is a container for cards in a single scrollable row."""
 
     has_content = True
     required_arguments = 1  # columns
     optional_arguments = 0
     option_spec = {
         "class": directives.class_option,
     }
 
-    def run(self) -> List[nodes.Node]:
-        """Run the directive."""
+    def run_with_defaults(self) -> list[nodes.Node]:
         self.assert_has_content()
         try:
             cols = make_choice([str(i) for i in range(1, 13)])(
                 self.arguments[0].strip()
             )
         except ValueError as exc:
-            raise self.error(f"Invalid directive argument: {exc}")
+            raise self.error(f"Invalid directive argument: {exc}") from exc
         container = create_component(
             "card-carousel",
-            ["sd-sphinx-override", "sd-cards-carousel", f"sd-card-cols-{cols}"]
-            + self.options.get("class", []),
+            [
+                "sd-sphinx-override",
+                "sd-cards-carousel",
+                f"sd-card-cols-{cols}",
+                *self.options.get("class", []),
+            ],
         )
         self.set_source_info(container)
         self.state.nested_parse(self.content, self.content_offset, container)
         for item in container.children:
             if not is_component(item, "card"):
                 LOGGER.warning(
                     "All children of a 'card-carousel' "
```

### Comparing `sphinx_design-0.5.0/sphinx_design/compiled/material-icons_LICENSE` & `sphinx_design-0.6.0/sphinx_design/compiled/material-icons_LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.5.0/sphinx_design/compiled/material_outlined.json` & `sphinx_design-0.6.0/sphinx_design/compiled/material_outlined.json`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.5.0/sphinx_design/compiled/material_regular.json` & `sphinx_design-0.6.0/sphinx_design/compiled/material_regular.json`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.5.0/sphinx_design/compiled/material_round.json` & `sphinx_design-0.6.0/sphinx_design/compiled/material_round.json`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.5.0/sphinx_design/compiled/material_sharp.json` & `sphinx_design-0.6.0/sphinx_design/compiled/material_sharp.json`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.5.0/sphinx_design/compiled/material_twotone.json` & `sphinx_design-0.6.0/sphinx_design/compiled/material_twotone.json`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.5.0/sphinx_design/compiled/octicon_LICENSE` & `sphinx_design-0.6.0/sphinx_design/compiled/octicon_LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 GitHub Inc.
+Copyright (c) 2023 GitHub Inc.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `sphinx_design-0.5.0/sphinx_design/compiled/style.min.css` & `sphinx_design-0.6.0/sphinx_design/compiled/style.min.css`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-.sd-bg-primary{background-color:var(--sd-color-primary) !important}.sd-bg-text-primary{color:var(--sd-color-primary-text) !important}button.sd-bg-primary:focus,button.sd-bg-primary:hover{background-color:var(--sd-color-primary-highlight) !important}a.sd-bg-primary:focus,a.sd-bg-primary:hover{background-color:var(--sd-color-primary-highlight) !important}.sd-bg-secondary{background-color:var(--sd-color-secondary) !important}.sd-bg-text-secondary{color:var(--sd-color-secondary-text) !important}button.sd-bg-secondary:focus,button.sd-bg-secondary:hover{background-color:var(--sd-color-secondary-highlight) !important}a.sd-bg-secondary:focus,a.sd-bg-secondary:hover{background-color:var(--sd-color-secondary-highlight) !important}.sd-bg-success{background-color:var(--sd-color-success) !important}.sd-bg-text-success{color:var(--sd-color-success-text) !important}button.sd-bg-success:focus,button.sd-bg-success:hover{background-color:var(--sd-color-success-highlight) !important}a.sd-bg-success:focus,a.sd-bg-success:hover{background-color:var(--sd-color-success-highlight) !important}.sd-bg-info{background-color:var(--sd-color-info) !important}.sd-bg-text-info{color:var(--sd-color-info-text) !important}button.sd-bg-info:focus,button.sd-bg-info:hover{background-color:var(--sd-color-info-highlight) !important}a.sd-bg-info:focus,a.sd-bg-info:hover{background-color:var(--sd-color-info-highlight) !important}.sd-bg-warning{background-color:var(--sd-color-warning) !important}.sd-bg-text-warning{color:var(--sd-color-warning-text) !important}button.sd-bg-warning:focus,button.sd-bg-warning:hover{background-color:var(--sd-color-warning-highlight) !important}a.sd-bg-warning:focus,a.sd-bg-warning:hover{background-color:var(--sd-color-warning-highlight) !important}.sd-bg-danger{background-color:var(--sd-color-danger) !important}.sd-bg-text-danger{color:var(--sd-color-danger-text) !important}button.sd-bg-danger:focus,button.sd-bg-danger:hover{background-color:var(--sd-color-danger-highlight) !important}a.sd-bg-danger:focus,a.sd-bg-danger:hover{background-color:var(--sd-color-danger-highlight) !important}.sd-bg-light{background-color:var(--sd-color-light) !important}.sd-bg-text-light{color:var(--sd-color-light-text) !important}button.sd-bg-light:focus,button.sd-bg-light:hover{background-color:var(--sd-color-light-highlight) !important}a.sd-bg-light:focus,a.sd-bg-light:hover{background-color:var(--sd-color-light-highlight) !important}.sd-bg-muted{background-color:var(--sd-color-muted) !important}.sd-bg-text-muted{color:var(--sd-color-muted-text) !important}button.sd-bg-muted:focus,button.sd-bg-muted:hover{background-color:var(--sd-color-muted-highlight) !important}a.sd-bg-muted:focus,a.sd-bg-muted:hover{background-color:var(--sd-color-muted-highlight) !important}.sd-bg-dark{background-color:var(--sd-color-dark) !important}.sd-bg-text-dark{color:var(--sd-color-dark-text) !important}button.sd-bg-dark:focus,button.sd-bg-dark:hover{background-color:var(--sd-color-dark-highlight) !important}a.sd-bg-dark:focus,a.sd-bg-dark:hover{background-color:var(--sd-color-dark-highlight) !important}.sd-bg-black{background-color:var(--sd-color-black) !important}.sd-bg-text-black{color:var(--sd-color-black-text) !important}button.sd-bg-black:focus,button.sd-bg-black:hover{background-color:var(--sd-color-black-highlight) !important}a.sd-bg-black:focus,a.sd-bg-black:hover{background-color:var(--sd-color-black-highlight) !important}.sd-bg-white{background-color:var(--sd-color-white) !important}.sd-bg-text-white{color:var(--sd-color-white-text) !important}button.sd-bg-white:focus,button.sd-bg-white:hover{background-color:var(--sd-color-white-highlight) !important}a.sd-bg-white:focus,a.sd-bg-white:hover{background-color:var(--sd-color-white-highlight) !important}.sd-text-primary,.sd-text-primary>p{color:var(--sd-color-primary) !important}a.sd-text-primary:focus,a.sd-text-primary:hover{color:var(--sd-color-primary-highlight) !important}.sd-text-secondary,.sd-text-secondary>p{color:var(--sd-color-secondary) !important}a.sd-text-secondary:focus,a.sd-text-secondary:hover{color:var(--sd-color-secondary-highlight) !important}.sd-text-success,.sd-text-success>p{color:var(--sd-color-success) !important}a.sd-text-success:focus,a.sd-text-success:hover{color:var(--sd-color-success-highlight) !important}.sd-text-info,.sd-text-info>p{color:var(--sd-color-info) !important}a.sd-text-info:focus,a.sd-text-info:hover{color:var(--sd-color-info-highlight) !important}.sd-text-warning,.sd-text-warning>p{color:var(--sd-color-warning) !important}a.sd-text-warning:focus,a.sd-text-warning:hover{color:var(--sd-color-warning-highlight) !important}.sd-text-danger,.sd-text-danger>p{color:var(--sd-color-danger) !important}a.sd-text-danger:focus,a.sd-text-danger:hover{color:var(--sd-color-danger-highlight) !important}.sd-text-light,.sd-text-light>p{color:var(--sd-color-light) !important}a.sd-text-light:focus,a.sd-text-light:hover{color:var(--sd-color-light-highlight) !important}.sd-text-muted,.sd-text-muted>p{color:var(--sd-color-muted) !important}a.sd-text-muted:focus,a.sd-text-muted:hover{color:var(--sd-color-muted-highlight) !important}.sd-text-dark,.sd-text-dark>p{color:var(--sd-color-dark) !important}a.sd-text-dark:focus,a.sd-text-dark:hover{color:var(--sd-color-dark-highlight) !important}.sd-text-black,.sd-text-black>p{color:var(--sd-color-black) !important}a.sd-text-black:focus,a.sd-text-black:hover{color:var(--sd-color-black-highlight) !important}.sd-text-white,.sd-text-white>p{color:var(--sd-color-white) !important}a.sd-text-white:focus,a.sd-text-white:hover{color:var(--sd-color-white-highlight) !important}.sd-outline-primary{border-color:var(--sd-color-primary) !important;border-style:solid !important;border-width:1px !important}a.sd-outline-primary:focus,a.sd-outline-primary:hover{border-color:var(--sd-color-primary-highlight) !important}.sd-outline-secondary{border-color:var(--sd-color-secondary) !important;border-style:solid !important;border-width:1px !important}a.sd-outline-secondary:focus,a.sd-outline-secondary:hover{border-color:var(--sd-color-secondary-highlight) !important}.sd-outline-success{border-color:var(--sd-color-success) !important;border-style:solid !important;border-width:1px !important}a.sd-outline-success:focus,a.sd-outline-success:hover{border-color:var(--sd-color-success-highlight) !important}.sd-outline-info{border-color:var(--sd-color-info) !important;border-style:solid !important;border-width:1px !important}a.sd-outline-info:focus,a.sd-outline-info:hover{border-color:var(--sd-color-info-highlight) !important}.sd-outline-warning{border-color:var(--sd-color-warning) !important;border-style:solid !important;border-width:1px !important}a.sd-outline-warning:focus,a.sd-outline-warning:hover{border-color:var(--sd-color-warning-highlight) !important}.sd-outline-danger{border-color:var(--sd-color-danger) !important;border-style:solid !important;border-width:1px !important}a.sd-outline-danger:focus,a.sd-outline-danger:hover{border-color:var(--sd-color-danger-highlight) !important}.sd-outline-light{border-color:var(--sd-color-light) !important;border-style:solid !important;border-width:1px !important}a.sd-outline-light:focus,a.sd-outline-light:hover{border-color:var(--sd-color-light-highlight) !important}.sd-outline-muted{border-color:var(--sd-color-muted) !important;border-style:solid !important;border-width:1px !important}a.sd-outline-muted:focus,a.sd-outline-muted:hover{border-color:var(--sd-color-muted-highlight) !important}.sd-outline-dark{border-color:var(--sd-color-dark) !important;border-style:solid !important;border-width:1px !important}a.sd-outline-dark:focus,a.sd-outline-dark:hover{border-color:var(--sd-color-dark-highlight) !important}.sd-outline-black{border-color:var(--sd-color-black) !important;border-style:solid !important;border-width:1px !important}a.sd-outline-black:focus,a.sd-outline-black:hover{border-color:var(--sd-color-black-highlight) !important}.sd-outline-white{border-color:var(--sd-color-white) !important;border-style:solid !important;border-width:1px !important}a.sd-outline-white:focus,a.sd-outline-white:hover{border-color:var(--sd-color-white-highlight) !important}.sd-bg-transparent{background-color:transparent !important}.sd-outline-transparent{border-color:transparent !important}.sd-text-transparent{color:transparent !important}.sd-p-0{padding:0 !important}.sd-pt-0,.sd-py-0{padding-top:0 !important}.sd-pr-0,.sd-px-0{padding-right:0 !important}.sd-pb-0,.sd-py-0{padding-bottom:0 !important}.sd-pl-0,.sd-px-0{padding-left:0 !important}.sd-p-1{padding:.25rem !important}.sd-pt-1,.sd-py-1{padding-top:.25rem !important}.sd-pr-1,.sd-px-1{padding-right:.25rem !important}.sd-pb-1,.sd-py-1{padding-bottom:.25rem !important}.sd-pl-1,.sd-px-1{padding-left:.25rem !important}.sd-p-2{padding:.5rem !important}.sd-pt-2,.sd-py-2{padding-top:.5rem !important}.sd-pr-2,.sd-px-2{padding-right:.5rem !important}.sd-pb-2,.sd-py-2{padding-bottom:.5rem !important}.sd-pl-2,.sd-px-2{padding-left:.5rem !important}.sd-p-3{padding:1rem !important}.sd-pt-3,.sd-py-3{padding-top:1rem !important}.sd-pr-3,.sd-px-3{padding-right:1rem !important}.sd-pb-3,.sd-py-3{padding-bottom:1rem !important}.sd-pl-3,.sd-px-3{padding-left:1rem !important}.sd-p-4{padding:1.5rem !important}.sd-pt-4,.sd-py-4{padding-top:1.5rem !important}.sd-pr-4,.sd-px-4{padding-right:1.5rem !important}.sd-pb-4,.sd-py-4{padding-bottom:1.5rem !important}.sd-pl-4,.sd-px-4{padding-left:1.5rem !important}.sd-p-5{padding:3rem !important}.sd-pt-5,.sd-py-5{padding-top:3rem !important}.sd-pr-5,.sd-px-5{padding-right:3rem !important}.sd-pb-5,.sd-py-5{padding-bottom:3rem !important}.sd-pl-5,.sd-px-5{padding-left:3rem !important}.sd-m-auto{margin:auto !important}.sd-mt-auto,.sd-my-auto{margin-top:auto !important}.sd-mr-auto,.sd-mx-auto{margin-right:auto !important}.sd-mb-auto,.sd-my-auto{margin-bottom:auto !important}.sd-ml-auto,.sd-mx-auto{margin-left:auto !important}.sd-m-0{margin:0 !important}.sd-mt-0,.sd-my-0{margin-top:0 !important}.sd-mr-0,.sd-mx-0{margin-right:0 !important}.sd-mb-0,.sd-my-0{margin-bottom:0 !important}.sd-ml-0,.sd-mx-0{margin-left:0 !important}.sd-m-1{margin:.25rem !important}.sd-mt-1,.sd-my-1{margin-top:.25rem !important}.sd-mr-1,.sd-mx-1{margin-right:.25rem !important}.sd-mb-1,.sd-my-1{margin-bottom:.25rem !important}.sd-ml-1,.sd-mx-1{margin-left:.25rem !important}.sd-m-2{margin:.5rem !important}.sd-mt-2,.sd-my-2{margin-top:.5rem !important}.sd-mr-2,.sd-mx-2{margin-right:.5rem !important}.sd-mb-2,.sd-my-2{margin-bottom:.5rem !important}.sd-ml-2,.sd-mx-2{margin-left:.5rem !important}.sd-m-3{margin:1rem !important}.sd-mt-3,.sd-my-3{margin-top:1rem !important}.sd-mr-3,.sd-mx-3{margin-right:1rem !important}.sd-mb-3,.sd-my-3{margin-bottom:1rem !important}.sd-ml-3,.sd-mx-3{margin-left:1rem !important}.sd-m-4{margin:1.5rem !important}.sd-mt-4,.sd-my-4{margin-top:1.5rem !important}.sd-mr-4,.sd-mx-4{margin-right:1.5rem !important}.sd-mb-4,.sd-my-4{margin-bottom:1.5rem !important}.sd-ml-4,.sd-mx-4{margin-left:1.5rem !important}.sd-m-5{margin:3rem !important}.sd-mt-5,.sd-my-5{margin-top:3rem !important}.sd-mr-5,.sd-mx-5{margin-right:3rem !important}.sd-mb-5,.sd-my-5{margin-bottom:3rem !important}.sd-ml-5,.sd-mx-5{margin-left:3rem !important}.sd-w-25{width:25% !important}.sd-w-50{width:50% !important}.sd-w-75{width:75% !important}.sd-w-100{width:100% !important}.sd-w-auto{width:auto !important}.sd-h-25{height:25% !important}.sd-h-50{height:50% !important}.sd-h-75{height:75% !important}.sd-h-100{height:100% !important}.sd-h-auto{height:auto !important}.sd-d-none{display:none !important}.sd-d-inline{display:inline !important}.sd-d-inline-block{display:inline-block !important}.sd-d-block{display:block !important}.sd-d-grid{display:grid !important}.sd-d-flex-row{display:-ms-flexbox !important;display:flex !important;flex-direction:row !important}.sd-d-flex-column{display:-ms-flexbox !important;display:flex !important;flex-direction:column !important}.sd-d-inline-flex{display:-ms-inline-flexbox !important;display:inline-flex !important}@media(min-width: 576px){.sd-d-sm-none{display:none !important}.sd-d-sm-inline{display:inline !important}.sd-d-sm-inline-block{display:inline-block !important}.sd-d-sm-block{display:block !important}.sd-d-sm-grid{display:grid !important}.sd-d-sm-flex{display:-ms-flexbox !important;display:flex !important}.sd-d-sm-inline-flex{display:-ms-inline-flexbox !important;display:inline-flex !important}}@media(min-width: 768px){.sd-d-md-none{display:none !important}.sd-d-md-inline{display:inline !important}.sd-d-md-inline-block{display:inline-block !important}.sd-d-md-block{display:block !important}.sd-d-md-grid{display:grid !important}.sd-d-md-flex{display:-ms-flexbox !important;display:flex !important}.sd-d-md-inline-flex{display:-ms-inline-flexbox !important;display:inline-flex !important}}@media(min-width: 992px){.sd-d-lg-none{display:none !important}.sd-d-lg-inline{display:inline !important}.sd-d-lg-inline-block{display:inline-block !important}.sd-d-lg-block{display:block !important}.sd-d-lg-grid{display:grid !important}.sd-d-lg-flex{display:-ms-flexbox !important;display:flex !important}.sd-d-lg-inline-flex{display:-ms-inline-flexbox !important;display:inline-flex !important}}@media(min-width: 1200px){.sd-d-xl-none{display:none !important}.sd-d-xl-inline{display:inline !important}.sd-d-xl-inline-block{display:inline-block !important}.sd-d-xl-block{display:block !important}.sd-d-xl-grid{display:grid !important}.sd-d-xl-flex{display:-ms-flexbox !important;display:flex !important}.sd-d-xl-inline-flex{display:-ms-inline-flexbox !important;display:inline-flex !important}}.sd-align-major-start{justify-content:flex-start !important}.sd-align-major-end{justify-content:flex-end !important}.sd-align-major-center{justify-content:center !important}.sd-align-major-justify{justify-content:space-between !important}.sd-align-major-spaced{justify-content:space-evenly !important}.sd-align-minor-start{align-items:flex-start !important}.sd-align-minor-end{align-items:flex-end !important}.sd-align-minor-center{align-items:center !important}.sd-align-minor-stretch{align-items:stretch !important}.sd-text-justify{text-align:justify !important}.sd-text-left{text-align:left !important}.sd-text-right{text-align:right !important}.sd-text-center{text-align:center !important}.sd-font-weight-light{font-weight:300 !important}.sd-font-weight-lighter{font-weight:lighter !important}.sd-font-weight-normal{font-weight:400 !important}.sd-font-weight-bold{font-weight:700 !important}.sd-font-weight-bolder{font-weight:bolder !important}.sd-font-italic{font-style:italic !important}.sd-text-decoration-none{text-decoration:none !important}.sd-text-lowercase{text-transform:lowercase !important}.sd-text-uppercase{text-transform:uppercase !important}.sd-text-capitalize{text-transform:capitalize !important}.sd-text-wrap{white-space:normal !important}.sd-text-nowrap{white-space:nowrap !important}.sd-text-truncate{overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.sd-fs-1,.sd-fs-1>p{font-size:calc(1.375rem + 1.5vw) !important;line-height:unset !important}.sd-fs-2,.sd-fs-2>p{font-size:calc(1.325rem + 0.9vw) !important;line-height:unset !important}.sd-fs-3,.sd-fs-3>p{font-size:calc(1.3rem + 0.6vw) !important;line-height:unset !important}.sd-fs-4,.sd-fs-4>p{font-size:calc(1.275rem + 0.3vw) !important;line-height:unset !important}.sd-fs-5,.sd-fs-5>p{font-size:1.25rem !important;line-height:unset !important}.sd-fs-6,.sd-fs-6>p{font-size:1rem !important;line-height:unset !important}.sd-border-0{border:0 solid !important}.sd-border-top-0{border-top:0 solid !important}.sd-border-bottom-0{border-bottom:0 solid !important}.sd-border-right-0{border-right:0 solid !important}.sd-border-left-0{border-left:0 solid !important}.sd-border-1{border:1px solid !important}.sd-border-top-1{border-top:1px solid !important}.sd-border-bottom-1{border-bottom:1px solid !important}.sd-border-right-1{border-right:1px solid !important}.sd-border-left-1{border-left:1px solid !important}.sd-border-2{border:2px solid !important}.sd-border-top-2{border-top:2px solid !important}.sd-border-bottom-2{border-bottom:2px solid !important}.sd-border-right-2{border-right:2px solid !important}.sd-border-left-2{border-left:2px solid !important}.sd-border-3{border:3px solid !important}.sd-border-top-3{border-top:3px solid !important}.sd-border-bottom-3{border-bottom:3px solid !important}.sd-border-right-3{border-right:3px solid !important}.sd-border-left-3{border-left:3px solid !important}.sd-border-4{border:4px solid !important}.sd-border-top-4{border-top:4px solid !important}.sd-border-bottom-4{border-bottom:4px solid !important}.sd-border-right-4{border-right:4px solid !important}.sd-border-left-4{border-left:4px solid !important}.sd-border-5{border:5px solid !important}.sd-border-top-5{border-top:5px solid !important}.sd-border-bottom-5{border-bottom:5px solid !important}.sd-border-right-5{border-right:5px solid !important}.sd-border-left-5{border-left:5px solid !important}.sd-rounded-0{border-radius:0 !important}.sd-rounded-1{border-radius:.2rem !important}.sd-rounded-2{border-radius:.3rem !important}.sd-rounded-3{border-radius:.5rem !important}.sd-rounded-pill{border-radius:50rem !important}.sd-rounded-circle{border-radius:50% !important}.shadow-none{box-shadow:none !important}.sd-shadow-sm{box-shadow:0 .125rem .25rem var(--sd-color-shadow) !important}.sd-shadow-md{box-shadow:0 .5rem 1rem var(--sd-color-shadow) !important}.sd-shadow-lg{box-shadow:0 1rem 3rem var(--sd-color-shadow) !important}@keyframes sd-slide-from-left{0%{transform:translateX(-100%)}100%{transform:translateX(0)}}@keyframes sd-slide-from-right{0%{transform:translateX(200%)}100%{transform:translateX(0)}}@keyframes sd-grow100{0%{transform:scale(0);opacity:.5}100%{transform:scale(1);opacity:1}}@keyframes sd-grow50{0%{transform:scale(0.5);opacity:.5}100%{transform:scale(1);opacity:1}}@keyframes sd-grow50-rot20{0%{transform:scale(0.5) rotateZ(-20deg);opacity:.5}75%{transform:scale(1) rotateZ(5deg);opacity:1}95%{transform:scale(1) rotateZ(-1deg);opacity:1}100%{transform:scale(1) rotateZ(0);opacity:1}}.sd-animate-slide-from-left{animation:1s ease-out 0s 1 normal none running sd-slide-from-left}.sd-animate-slide-from-right{animation:1s ease-out 0s 1 normal none running sd-slide-from-right}.sd-animate-grow100{animation:1s ease-out 0s 1 normal none running sd-grow100}.sd-animate-grow50{animation:1s ease-out 0s 1 normal none running sd-grow50}.sd-animate-grow50-rot20{animation:1s ease-out 0s 1 normal none running sd-grow50-rot20}.sd-badge{display:inline-block;padding:.35em .65em;font-size:.75em;font-weight:700;line-height:1;text-align:center;white-space:nowrap;vertical-align:baseline;border-radius:.25rem}.sd-badge:empty{display:none}a.sd-badge{text-decoration:none}.sd-btn .sd-badge{position:relative;top:-1px}.sd-btn{background-color:transparent;border:1px solid transparent;border-radius:.25rem;cursor:pointer;display:inline-block;font-weight:400;font-size:1rem;line-height:1.5;padding:.375rem .75rem;text-align:center;text-decoration:none;transition:color .15s ease-in-out,background-color .15s ease-in-out,border-color .15s ease-in-out,box-shadow .15s ease-in-out;vertical-align:middle;user-select:none;-moz-user-select:none;-ms-user-select:none;-webkit-user-select:none}.sd-btn:hover{text-decoration:none}@media(prefers-reduced-motion: reduce){.sd-btn{transition:none}}.sd-btn-primary,.sd-btn-outline-primary:hover,.sd-btn-outline-primary:focus{color:var(--sd-color-primary-text) !important;background-color:var(--sd-color-primary) !important;border-color:var(--sd-color-primary) !important;border-width:1px !important;border-style:solid !important}.sd-btn-primary:hover,.sd-btn-primary:focus{color:var(--sd-color-primary-text) !important;background-color:var(--sd-color-primary-highlight) !important;border-color:var(--sd-color-primary-highlight) !important;border-width:1px !important;border-style:solid !important}.sd-btn-outline-primary{color:var(--sd-color-primary) !important;border-color:var(--sd-color-primary) !important;border-width:1px !important;border-style:solid !important}.sd-btn-secondary,.sd-btn-outline-secondary:hover,.sd-btn-outline-secondary:focus{color:var(--sd-color-secondary-text) !important;background-color:var(--sd-color-secondary) !important;border-color:var(--sd-color-secondary) !important;border-width:1px !important;border-style:solid !important}.sd-btn-secondary:hover,.sd-btn-secondary:focus{color:var(--sd-color-secondary-text) !important;background-color:var(--sd-color-secondary-highlight) !important;border-color:var(--sd-color-secondary-highlight) !important;border-width:1px !important;border-style:solid !important}.sd-btn-outline-secondary{color:var(--sd-color-secondary) !important;border-color:var(--sd-color-secondary) !important;border-width:1px !important;border-style:solid !important}.sd-btn-success,.sd-btn-outline-success:hover,.sd-btn-outline-success:focus{color:var(--sd-color-success-text) !important;background-color:var(--sd-color-success) !important;border-color:var(--sd-color-success) !important;border-width:1px !important;border-style:solid !important}.sd-btn-success:hover,.sd-btn-success:focus{color:var(--sd-color-success-text) !important;background-color:var(--sd-color-success-highlight) !important;border-color:var(--sd-color-success-highlight) !important;border-width:1px !important;border-style:solid !important}.sd-btn-outline-success{color:var(--sd-color-success) !important;border-color:var(--sd-color-success) !important;border-width:1px !important;border-style:solid !important}.sd-btn-info,.sd-btn-outline-info:hover,.sd-btn-outline-info:focus{color:var(--sd-color-info-text) !important;background-color:var(--sd-color-info) !important;border-color:var(--sd-color-info) !important;border-width:1px !important;border-style:solid !important}.sd-btn-info:hover,.sd-btn-info:focus{color:var(--sd-color-info-text) !important;background-color:var(--sd-color-info-highlight) !important;border-color:var(--sd-color-info-highlight) !important;border-width:1px !important;border-style:solid !important}.sd-btn-outline-info{color:var(--sd-color-info) !important;border-color:var(--sd-color-info) !important;border-width:1px !important;border-style:solid !important}.sd-btn-warning,.sd-btn-outline-warning:hover,.sd-btn-outline-warning:focus{color:var(--sd-color-warning-text) !important;background-color:var(--sd-color-warning) !important;border-color:var(--sd-color-warning) !important;border-width:1px !important;border-style:solid !important}.sd-btn-warning:hover,.sd-btn-warning:focus{color:var(--sd-color-warning-text) !important;background-color:var(--sd-color-warning-highlight) !important;border-color:var(--sd-color-warning-highlight) !important;border-width:1px !important;border-style:solid !important}.sd-btn-outline-warning{color:var(--sd-color-warning) !important;border-color:var(--sd-color-warning) !important;border-width:1px !important;border-style:solid !important}.sd-btn-danger,.sd-btn-outline-danger:hover,.sd-btn-outline-danger:focus{color:var(--sd-color-danger-text) !important;background-color:var(--sd-color-danger) !important;border-color:var(--sd-color-danger) !important;border-width:1px !important;border-style:solid !important}.sd-btn-danger:hover,.sd-btn-danger:focus{color:var(--sd-color-danger-text) !important;background-color:var(--sd-color-danger-highlight) !important;border-color:var(--sd-color-danger-highlight) !important;border-width:1px !important;border-style:solid !important}.sd-btn-outline-danger{color:var(--sd-color-danger) !important;border-color:var(--sd-color-danger) !important;border-width:1px !important;border-style:solid !important}.sd-btn-light,.sd-btn-outline-light:hover,.sd-btn-outline-light:focus{color:var(--sd-color-light-text) !important;background-color:var(--sd-color-light) !important;border-color:var(--sd-color-light) !important;border-width:1px !important;border-style:solid !important}.sd-btn-light:hover,.sd-btn-light:focus{color:var(--sd-color-light-text) !important;background-color:var(--sd-color-light-highlight) !important;border-color:var(--sd-color-light-highlight) !important;border-width:1px !important;border-style:solid !important}.sd-btn-outline-light{color:var(--sd-color-light) !important;border-color:var(--sd-color-light) !important;border-width:1px !important;border-style:solid !important}.sd-btn-muted,.sd-btn-outline-muted:hover,.sd-btn-outline-muted:focus{color:var(--sd-color-muted-text) !important;background-color:var(--sd-color-muted) !important;border-color:var(--sd-color-muted) !important;border-width:1px !important;border-style:solid !important}.sd-btn-muted:hover,.sd-btn-muted:focus{color:var(--sd-color-muted-text) !important;background-color:var(--sd-color-muted-highlight) !important;border-color:var(--sd-color-muted-highlight) !important;border-width:1px !important;border-style:solid !important}.sd-btn-outline-muted{color:var(--sd-color-muted) !important;border-color:var(--sd-color-muted) !important;border-width:1px !important;border-style:solid !important}.sd-btn-dark,.sd-btn-outline-dark:hover,.sd-btn-outline-dark:focus{color:var(--sd-color-dark-text) !important;background-color:var(--sd-color-dark) !important;border-color:var(--sd-color-dark) !important;border-width:1px !important;border-style:solid !important}.sd-btn-dark:hover,.sd-btn-dark:focus{color:var(--sd-color-dark-text) !important;background-color:var(--sd-color-dark-highlight) !important;border-color:var(--sd-color-dark-highlight) !important;border-width:1px !important;border-style:solid !important}.sd-btn-outline-dark{color:var(--sd-color-dark) !important;border-color:var(--sd-color-dark) !important;border-width:1px !important;border-style:solid !important}.sd-btn-black,.sd-btn-outline-black:hover,.sd-btn-outline-black:focus{color:var(--sd-color-black-text) !important;background-color:var(--sd-color-black) !important;border-color:var(--sd-color-black) !important;border-width:1px !important;border-style:solid !important}.sd-btn-black:hover,.sd-btn-black:focus{color:var(--sd-color-black-text) !important;background-color:var(--sd-color-black-highlight) !important;border-color:var(--sd-color-black-highlight) !important;border-width:1px !important;border-style:solid !important}.sd-btn-outline-black{color:var(--sd-color-black) !important;border-color:var(--sd-color-black) !important;border-width:1px !important;border-style:solid !important}.sd-btn-white,.sd-btn-outline-white:hover,.sd-btn-outline-white:focus{color:var(--sd-color-white-text) !important;background-color:var(--sd-color-white) !important;border-color:var(--sd-color-white) !important;border-width:1px !important;border-style:solid !important}.sd-btn-white:hover,.sd-btn-white:focus{color:var(--sd-color-white-text) !important;background-color:var(--sd-color-white-highlight) !important;border-color:var(--sd-color-white-highlight) !important;border-width:1px !important;border-style:solid !important}.sd-btn-outline-white{color:var(--sd-color-white) !important;border-color:var(--sd-color-white) !important;border-width:1px !important;border-style:solid !important}.sd-stretched-link::after{position:absolute;top:0;right:0;bottom:0;left:0;z-index:1;content:""}.sd-hide-link-text{font-size:0}.sd-octicon,.sd-material-icon{display:inline-block;fill:currentColor;vertical-align:middle}.sd-avatar-xs{border-radius:50%;object-fit:cover;object-position:center;width:1rem;height:1rem}.sd-avatar-sm{border-radius:50%;object-fit:cover;object-position:center;width:3rem;height:3rem}.sd-avatar-md{border-radius:50%;object-fit:cover;object-position:center;width:5rem;height:5rem}.sd-avatar-lg{border-radius:50%;object-fit:cover;object-position:center;width:7rem;height:7rem}.sd-avatar-xl{border-radius:50%;object-fit:cover;object-position:center;width:10rem;height:10rem}.sd-avatar-inherit{border-radius:50%;object-fit:cover;object-position:center;width:inherit;height:inherit}.sd-avatar-initial{border-radius:50%;object-fit:cover;object-position:center;width:initial;height:initial}.sd-card{background-clip:border-box;background-color:var(--sd-color-card-background);border:1px solid var(--sd-color-card-border);border-radius:.25rem;color:var(--sd-color-card-text);display:-ms-flexbox;display:flex;-ms-flex-direction:column;flex-direction:column;min-width:0;position:relative;word-wrap:break-word}.sd-card>hr{margin-left:0;margin-right:0}.sd-card-hover:hover{border-color:var(--sd-color-card-border-hover);transform:scale(1.01)}.sd-card-body{-ms-flex:1 1 auto;flex:1 1 auto;padding:1rem 1rem}.sd-card-title{margin-bottom:.5rem}.sd-card-subtitle{margin-top:-0.25rem;margin-bottom:0}.sd-card-text:last-child{margin-bottom:0}.sd-card-link:hover{text-decoration:none}.sd-card-link+.card-link{margin-left:1rem}.sd-card-header{padding:.5rem 1rem;margin-bottom:0;background-color:var(--sd-color-card-header);border-bottom:1px solid var(--sd-color-card-border)}.sd-card-header:first-child{border-radius:calc(0.25rem - 1px) calc(0.25rem - 1px) 0 0}.sd-card-footer{padding:.5rem 1rem;background-color:var(--sd-color-card-footer);border-top:1px solid var(--sd-color-card-border)}.sd-card-footer:last-child{border-radius:0 0 calc(0.25rem - 1px) calc(0.25rem - 1px)}.sd-card-header-tabs{margin-right:-0.5rem;margin-bottom:-0.5rem;margin-left:-0.5rem;border-bottom:0}.sd-card-header-pills{margin-right:-0.5rem;margin-left:-0.5rem}.sd-card-img-overlay{position:absolute;top:0;right:0;bottom:0;left:0;padding:1rem;border-radius:calc(0.25rem - 1px)}.sd-card-img,.sd-card-img-bottom,.sd-card-img-top{width:100%}.sd-card-img,.sd-card-img-top{border-top-left-radius:calc(0.25rem - 1px);border-top-right-radius:calc(0.25rem - 1px)}.sd-card-img,.sd-card-img-bottom{border-bottom-left-radius:calc(0.25rem - 1px);border-bottom-right-radius:calc(0.25rem - 1px)}.sd-cards-carousel{width:100%;display:flex;flex-wrap:nowrap;-ms-flex-direction:row;flex-direction:row;overflow-x:hidden;scroll-snap-type:x mandatory}.sd-cards-carousel.sd-show-scrollbar{overflow-x:auto}.sd-cards-carousel:hover,.sd-cards-carousel:focus{overflow-x:auto}.sd-cards-carousel>.sd-card{flex-shrink:0;scroll-snap-align:start}.sd-cards-carousel>.sd-card:not(:last-child){margin-right:3px}.sd-card-cols-1>.sd-card{width:90%}.sd-card-cols-2>.sd-card{width:45%}.sd-card-cols-3>.sd-card{width:30%}.sd-card-cols-4>.sd-card{width:22.5%}.sd-card-cols-5>.sd-card{width:18%}.sd-card-cols-6>.sd-card{width:15%}.sd-card-cols-7>.sd-card{width:12.8571428571%}.sd-card-cols-8>.sd-card{width:11.25%}.sd-card-cols-9>.sd-card{width:10%}.sd-card-cols-10>.sd-card{width:9%}.sd-card-cols-11>.sd-card{width:8.1818181818%}.sd-card-cols-12>.sd-card{width:7.5%}.sd-container,.sd-container-fluid,.sd-container-lg,.sd-container-md,.sd-container-sm,.sd-container-xl{margin-left:auto;margin-right:auto;padding-left:var(--sd-gutter-x, 0.75rem);padding-right:var(--sd-gutter-x, 0.75rem);width:100%}@media(min-width: 576px){.sd-container-sm,.sd-container{max-width:540px}}@media(min-width: 768px){.sd-container-md,.sd-container-sm,.sd-container{max-width:720px}}@media(min-width: 992px){.sd-container-lg,.sd-container-md,.sd-container-sm,.sd-container{max-width:960px}}@media(min-width: 1200px){.sd-container-xl,.sd-container-lg,.sd-container-md,.sd-container-sm,.sd-container{max-width:1140px}}.sd-row{--sd-gutter-x: 1.5rem;--sd-gutter-y: 0;display:-ms-flexbox;display:flex;-ms-flex-wrap:wrap;flex-wrap:wrap;margin-top:calc(var(--sd-gutter-y) * -1);margin-right:calc(var(--sd-gutter-x) * -0.5);margin-left:calc(var(--sd-gutter-x) * -0.5)}.sd-row>*{box-sizing:border-box;flex-shrink:0;width:100%;max-width:100%;padding-right:calc(var(--sd-gutter-x) * 0.5);padding-left:calc(var(--sd-gutter-x) * 0.5);margin-top:var(--sd-gutter-y)}.sd-col{flex:1 0 0%;-ms-flex:1 0 0%}.sd-row-cols-auto>*{flex:0 0 auto;width:auto}.sd-row-cols-1>*{flex:0 0 auto;-ms-flex:0 0 auto;width:100%}.sd-row-cols-2>*{flex:0 0 auto;-ms-flex:0 0 auto;width:50%}.sd-row-cols-3>*{flex:0 0 auto;-ms-flex:0 0 auto;width:33.3333333333%}.sd-row-cols-4>*{flex:0 0 auto;-ms-flex:0 0 auto;width:25%}.sd-row-cols-5>*{flex:0 0 auto;-ms-flex:0 0 auto;width:20%}.sd-row-cols-6>*{flex:0 0 auto;-ms-flex:0 0 auto;width:16.6666666667%}.sd-row-cols-7>*{flex:0 0 auto;-ms-flex:0 0 auto;width:14.2857142857%}.sd-row-cols-8>*{flex:0 0 auto;-ms-flex:0 0 auto;width:12.5%}.sd-row-cols-9>*{flex:0 0 auto;-ms-flex:0 0 auto;width:11.1111111111%}.sd-row-cols-10>*{flex:0 0 auto;-ms-flex:0 0 auto;width:10%}.sd-row-cols-11>*{flex:0 0 auto;-ms-flex:0 0 auto;width:9.0909090909%}.sd-row-cols-12>*{flex:0 0 auto;-ms-flex:0 0 auto;width:8.3333333333%}@media(min-width: 576px){.sd-col-sm{flex:1 0 0%;-ms-flex:1 0 0%}.sd-row-cols-sm-auto{flex:1 0 auto;-ms-flex:1 0 auto;width:100%}.sd-row-cols-sm-1>*{flex:0 0 auto;-ms-flex:0 0 auto;width:100%}.sd-row-cols-sm-2>*{flex:0 0 auto;-ms-flex:0 0 auto;width:50%}.sd-row-cols-sm-3>*{flex:0 0 auto;-ms-flex:0 0 auto;width:33.3333333333%}.sd-row-cols-sm-4>*{flex:0 0 auto;-ms-flex:0 0 auto;width:25%}.sd-row-cols-sm-5>*{flex:0 0 auto;-ms-flex:0 0 auto;width:20%}.sd-row-cols-sm-6>*{flex:0 0 auto;-ms-flex:0 0 auto;width:16.6666666667%}.sd-row-cols-sm-7>*{flex:0 0 auto;-ms-flex:0 0 auto;width:14.2857142857%}.sd-row-cols-sm-8>*{flex:0 0 auto;-ms-flex:0 0 auto;width:12.5%}.sd-row-cols-sm-9>*{flex:0 0 auto;-ms-flex:0 0 auto;width:11.1111111111%}.sd-row-cols-sm-10>*{flex:0 0 auto;-ms-flex:0 0 auto;width:10%}.sd-row-cols-sm-11>*{flex:0 0 auto;-ms-flex:0 0 auto;width:9.0909090909%}.sd-row-cols-sm-12>*{flex:0 0 auto;-ms-flex:0 0 auto;width:8.3333333333%}}@media(min-width: 768px){.sd-col-md{flex:1 0 0%;-ms-flex:1 0 0%}.sd-row-cols-md-auto{flex:1 0 auto;-ms-flex:1 0 auto;width:100%}.sd-row-cols-md-1>*{flex:0 0 auto;-ms-flex:0 0 auto;width:100%}.sd-row-cols-md-2>*{flex:0 0 auto;-ms-flex:0 0 auto;width:50%}.sd-row-cols-md-3>*{flex:0 0 auto;-ms-flex:0 0 auto;width:33.3333333333%}.sd-row-cols-md-4>*{flex:0 0 auto;-ms-flex:0 0 auto;width:25%}.sd-row-cols-md-5>*{flex:0 0 auto;-ms-flex:0 0 auto;width:20%}.sd-row-cols-md-6>*{flex:0 0 auto;-ms-flex:0 0 auto;width:16.6666666667%}.sd-row-cols-md-7>*{flex:0 0 auto;-ms-flex:0 0 auto;width:14.2857142857%}.sd-row-cols-md-8>*{flex:0 0 auto;-ms-flex:0 0 auto;width:12.5%}.sd-row-cols-md-9>*{flex:0 0 auto;-ms-flex:0 0 auto;width:11.1111111111%}.sd-row-cols-md-10>*{flex:0 0 auto;-ms-flex:0 0 auto;width:10%}.sd-row-cols-md-11>*{flex:0 0 auto;-ms-flex:0 0 auto;width:9.0909090909%}.sd-row-cols-md-12>*{flex:0 0 auto;-ms-flex:0 0 auto;width:8.3333333333%}}@media(min-width: 992px){.sd-col-lg{flex:1 0 0%;-ms-flex:1 0 0%}.sd-row-cols-lg-auto{flex:1 0 auto;-ms-flex:1 0 auto;width:100%}.sd-row-cols-lg-1>*{flex:0 0 auto;-ms-flex:0 0 auto;width:100%}.sd-row-cols-lg-2>*{flex:0 0 auto;-ms-flex:0 0 auto;width:50%}.sd-row-cols-lg-3>*{flex:0 0 auto;-ms-flex:0 0 auto;width:33.3333333333%}.sd-row-cols-lg-4>*{flex:0 0 auto;-ms-flex:0 0 auto;width:25%}.sd-row-cols-lg-5>*{flex:0 0 auto;-ms-flex:0 0 auto;width:20%}.sd-row-cols-lg-6>*{flex:0 0 auto;-ms-flex:0 0 auto;width:16.6666666667%}.sd-row-cols-lg-7>*{flex:0 0 auto;-ms-flex:0 0 auto;width:14.2857142857%}.sd-row-cols-lg-8>*{flex:0 0 auto;-ms-flex:0 0 auto;width:12.5%}.sd-row-cols-lg-9>*{flex:0 0 auto;-ms-flex:0 0 auto;width:11.1111111111%}.sd-row-cols-lg-10>*{flex:0 0 auto;-ms-flex:0 0 auto;width:10%}.sd-row-cols-lg-11>*{flex:0 0 auto;-ms-flex:0 0 auto;width:9.0909090909%}.sd-row-cols-lg-12>*{flex:0 0 auto;-ms-flex:0 0 auto;width:8.3333333333%}}@media(min-width: 1200px){.sd-col-xl{flex:1 0 0%;-ms-flex:1 0 0%}.sd-row-cols-xl-auto{flex:1 0 auto;-ms-flex:1 0 auto;width:100%}.sd-row-cols-xl-1>*{flex:0 0 auto;-ms-flex:0 0 auto;width:100%}.sd-row-cols-xl-2>*{flex:0 0 auto;-ms-flex:0 0 auto;width:50%}.sd-row-cols-xl-3>*{flex:0 0 auto;-ms-flex:0 0 auto;width:33.3333333333%}.sd-row-cols-xl-4>*{flex:0 0 auto;-ms-flex:0 0 auto;width:25%}.sd-row-cols-xl-5>*{flex:0 0 auto;-ms-flex:0 0 auto;width:20%}.sd-row-cols-xl-6>*{flex:0 0 auto;-ms-flex:0 0 auto;width:16.6666666667%}.sd-row-cols-xl-7>*{flex:0 0 auto;-ms-flex:0 0 auto;width:14.2857142857%}.sd-row-cols-xl-8>*{flex:0 0 auto;-ms-flex:0 0 auto;width:12.5%}.sd-row-cols-xl-9>*{flex:0 0 auto;-ms-flex:0 0 auto;width:11.1111111111%}.sd-row-cols-xl-10>*{flex:0 0 auto;-ms-flex:0 0 auto;width:10%}.sd-row-cols-xl-11>*{flex:0 0 auto;-ms-flex:0 0 auto;width:9.0909090909%}.sd-row-cols-xl-12>*{flex:0 0 auto;-ms-flex:0 0 auto;width:8.3333333333%}}.sd-col-auto{flex:0 0 auto;-ms-flex:0 0 auto;width:auto}.sd-col-1{flex:0 0 auto;-ms-flex:0 0 auto;width:8.3333333333%}.sd-col-2{flex:0 0 auto;-ms-flex:0 0 auto;width:16.6666666667%}.sd-col-3{flex:0 0 auto;-ms-flex:0 0 auto;width:25%}.sd-col-4{flex:0 0 auto;-ms-flex:0 0 auto;width:33.3333333333%}.sd-col-5{flex:0 0 auto;-ms-flex:0 0 auto;width:41.6666666667%}.sd-col-6{flex:0 0 auto;-ms-flex:0 0 auto;width:50%}.sd-col-7{flex:0 0 auto;-ms-flex:0 0 auto;width:58.3333333333%}.sd-col-8{flex:0 0 auto;-ms-flex:0 0 auto;width:66.6666666667%}.sd-col-9{flex:0 0 auto;-ms-flex:0 0 auto;width:75%}.sd-col-10{flex:0 0 auto;-ms-flex:0 0 auto;width:83.3333333333%}.sd-col-11{flex:0 0 auto;-ms-flex:0 0 auto;width:91.6666666667%}.sd-col-12{flex:0 0 auto;-ms-flex:0 0 auto;width:100%}.sd-g-0,.sd-gy-0{--sd-gutter-y: 0}.sd-g-0,.sd-gx-0{--sd-gutter-x: 0}.sd-g-1,.sd-gy-1{--sd-gutter-y: 0.25rem}.sd-g-1,.sd-gx-1{--sd-gutter-x: 0.25rem}.sd-g-2,.sd-gy-2{--sd-gutter-y: 0.5rem}.sd-g-2,.sd-gx-2{--sd-gutter-x: 0.5rem}.sd-g-3,.sd-gy-3{--sd-gutter-y: 1rem}.sd-g-3,.sd-gx-3{--sd-gutter-x: 1rem}.sd-g-4,.sd-gy-4{--sd-gutter-y: 1.5rem}.sd-g-4,.sd-gx-4{--sd-gutter-x: 1.5rem}.sd-g-5,.sd-gy-5{--sd-gutter-y: 3rem}.sd-g-5,.sd-gx-5{--sd-gutter-x: 3rem}@media(min-width: 576px){.sd-col-sm-auto{-ms-flex:0 0 auto;flex:0 0 auto;width:auto}.sd-col-sm-1{-ms-flex:0 0 auto;flex:0 0 auto;width:8.3333333333%}.sd-col-sm-2{-ms-flex:0 0 auto;flex:0 0 auto;width:16.6666666667%}.sd-col-sm-3{-ms-flex:0 0 auto;flex:0 0 auto;width:25%}.sd-col-sm-4{-ms-flex:0 0 auto;flex:0 0 auto;width:33.3333333333%}.sd-col-sm-5{-ms-flex:0 0 auto;flex:0 0 auto;width:41.6666666667%}.sd-col-sm-6{-ms-flex:0 0 auto;flex:0 0 auto;width:50%}.sd-col-sm-7{-ms-flex:0 0 auto;flex:0 0 auto;width:58.3333333333%}.sd-col-sm-8{-ms-flex:0 0 auto;flex:0 0 auto;width:66.6666666667%}.sd-col-sm-9{-ms-flex:0 0 auto;flex:0 0 auto;width:75%}.sd-col-sm-10{-ms-flex:0 0 auto;flex:0 0 auto;width:83.3333333333%}.sd-col-sm-11{-ms-flex:0 0 auto;flex:0 0 auto;width:91.6666666667%}.sd-col-sm-12{-ms-flex:0 0 auto;flex:0 0 auto;width:100%}.sd-g-sm-0,.sd-gy-sm-0{--sd-gutter-y: 0}.sd-g-sm-0,.sd-gx-sm-0{--sd-gutter-x: 0}.sd-g-sm-1,.sd-gy-sm-1{--sd-gutter-y: 0.25rem}.sd-g-sm-1,.sd-gx-sm-1{--sd-gutter-x: 0.25rem}.sd-g-sm-2,.sd-gy-sm-2{--sd-gutter-y: 0.5rem}.sd-g-sm-2,.sd-gx-sm-2{--sd-gutter-x: 0.5rem}.sd-g-sm-3,.sd-gy-sm-3{--sd-gutter-y: 1rem}.sd-g-sm-3,.sd-gx-sm-3{--sd-gutter-x: 1rem}.sd-g-sm-4,.sd-gy-sm-4{--sd-gutter-y: 1.5rem}.sd-g-sm-4,.sd-gx-sm-4{--sd-gutter-x: 1.5rem}.sd-g-sm-5,.sd-gy-sm-5{--sd-gutter-y: 3rem}.sd-g-sm-5,.sd-gx-sm-5{--sd-gutter-x: 3rem}}@media(min-width: 768px){.sd-col-md-auto{-ms-flex:0 0 auto;flex:0 0 auto;width:auto}.sd-col-md-1{-ms-flex:0 0 auto;flex:0 0 auto;width:8.3333333333%}.sd-col-md-2{-ms-flex:0 0 auto;flex:0 0 auto;width:16.6666666667%}.sd-col-md-3{-ms-flex:0 0 auto;flex:0 0 auto;width:25%}.sd-col-md-4{-ms-flex:0 0 auto;flex:0 0 auto;width:33.3333333333%}.sd-col-md-5{-ms-flex:0 0 auto;flex:0 0 auto;width:41.6666666667%}.sd-col-md-6{-ms-flex:0 0 auto;flex:0 0 auto;width:50%}.sd-col-md-7{-ms-flex:0 0 auto;flex:0 0 auto;width:58.3333333333%}.sd-col-md-8{-ms-flex:0 0 auto;flex:0 0 auto;width:66.6666666667%}.sd-col-md-9{-ms-flex:0 0 auto;flex:0 0 auto;width:75%}.sd-col-md-10{-ms-flex:0 0 auto;flex:0 0 auto;width:83.3333333333%}.sd-col-md-11{-ms-flex:0 0 auto;flex:0 0 auto;width:91.6666666667%}.sd-col-md-12{-ms-flex:0 0 auto;flex:0 0 auto;width:100%}.sd-g-md-0,.sd-gy-md-0{--sd-gutter-y: 0}.sd-g-md-0,.sd-gx-md-0{--sd-gutter-x: 0}.sd-g-md-1,.sd-gy-md-1{--sd-gutter-y: 0.25rem}.sd-g-md-1,.sd-gx-md-1{--sd-gutter-x: 0.25rem}.sd-g-md-2,.sd-gy-md-2{--sd-gutter-y: 0.5rem}.sd-g-md-2,.sd-gx-md-2{--sd-gutter-x: 0.5rem}.sd-g-md-3,.sd-gy-md-3{--sd-gutter-y: 1rem}.sd-g-md-3,.sd-gx-md-3{--sd-gutter-x: 1rem}.sd-g-md-4,.sd-gy-md-4{--sd-gutter-y: 1.5rem}.sd-g-md-4,.sd-gx-md-4{--sd-gutter-x: 1.5rem}.sd-g-md-5,.sd-gy-md-5{--sd-gutter-y: 3rem}.sd-g-md-5,.sd-gx-md-5{--sd-gutter-x: 3rem}}@media(min-width: 992px){.sd-col-lg-auto{-ms-flex:0 0 auto;flex:0 0 auto;width:auto}.sd-col-lg-1{-ms-flex:0 0 auto;flex:0 0 auto;width:8.3333333333%}.sd-col-lg-2{-ms-flex:0 0 auto;flex:0 0 auto;width:16.6666666667%}.sd-col-lg-3{-ms-flex:0 0 auto;flex:0 0 auto;width:25%}.sd-col-lg-4{-ms-flex:0 0 auto;flex:0 0 auto;width:33.3333333333%}.sd-col-lg-5{-ms-flex:0 0 auto;flex:0 0 auto;width:41.6666666667%}.sd-col-lg-6{-ms-flex:0 0 auto;flex:0 0 auto;width:50%}.sd-col-lg-7{-ms-flex:0 0 auto;flex:0 0 auto;width:58.3333333333%}.sd-col-lg-8{-ms-flex:0 0 auto;flex:0 0 auto;width:66.6666666667%}.sd-col-lg-9{-ms-flex:0 0 auto;flex:0 0 auto;width:75%}.sd-col-lg-10{-ms-flex:0 0 auto;flex:0 0 auto;width:83.3333333333%}.sd-col-lg-11{-ms-flex:0 0 auto;flex:0 0 auto;width:91.6666666667%}.sd-col-lg-12{-ms-flex:0 0 auto;flex:0 0 auto;width:100%}.sd-g-lg-0,.sd-gy-lg-0{--sd-gutter-y: 0}.sd-g-lg-0,.sd-gx-lg-0{--sd-gutter-x: 0}.sd-g-lg-1,.sd-gy-lg-1{--sd-gutter-y: 0.25rem}.sd-g-lg-1,.sd-gx-lg-1{--sd-gutter-x: 0.25rem}.sd-g-lg-2,.sd-gy-lg-2{--sd-gutter-y: 0.5rem}.sd-g-lg-2,.sd-gx-lg-2{--sd-gutter-x: 0.5rem}.sd-g-lg-3,.sd-gy-lg-3{--sd-gutter-y: 1rem}.sd-g-lg-3,.sd-gx-lg-3{--sd-gutter-x: 1rem}.sd-g-lg-4,.sd-gy-lg-4{--sd-gutter-y: 1.5rem}.sd-g-lg-4,.sd-gx-lg-4{--sd-gutter-x: 1.5rem}.sd-g-lg-5,.sd-gy-lg-5{--sd-gutter-y: 3rem}.sd-g-lg-5,.sd-gx-lg-5{--sd-gutter-x: 3rem}}@media(min-width: 1200px){.sd-col-xl-auto{-ms-flex:0 0 auto;flex:0 0 auto;width:auto}.sd-col-xl-1{-ms-flex:0 0 auto;flex:0 0 auto;width:8.3333333333%}.sd-col-xl-2{-ms-flex:0 0 auto;flex:0 0 auto;width:16.6666666667%}.sd-col-xl-3{-ms-flex:0 0 auto;flex:0 0 auto;width:25%}.sd-col-xl-4{-ms-flex:0 0 auto;flex:0 0 auto;width:33.3333333333%}.sd-col-xl-5{-ms-flex:0 0 auto;flex:0 0 auto;width:41.6666666667%}.sd-col-xl-6{-ms-flex:0 0 auto;flex:0 0 auto;width:50%}.sd-col-xl-7{-ms-flex:0 0 auto;flex:0 0 auto;width:58.3333333333%}.sd-col-xl-8{-ms-flex:0 0 auto;flex:0 0 auto;width:66.6666666667%}.sd-col-xl-9{-ms-flex:0 0 auto;flex:0 0 auto;width:75%}.sd-col-xl-10{-ms-flex:0 0 auto;flex:0 0 auto;width:83.3333333333%}.sd-col-xl-11{-ms-flex:0 0 auto;flex:0 0 auto;width:91.6666666667%}.sd-col-xl-12{-ms-flex:0 0 auto;flex:0 0 auto;width:100%}.sd-g-xl-0,.sd-gy-xl-0{--sd-gutter-y: 0}.sd-g-xl-0,.sd-gx-xl-0{--sd-gutter-x: 0}.sd-g-xl-1,.sd-gy-xl-1{--sd-gutter-y: 0.25rem}.sd-g-xl-1,.sd-gx-xl-1{--sd-gutter-x: 0.25rem}.sd-g-xl-2,.sd-gy-xl-2{--sd-gutter-y: 0.5rem}.sd-g-xl-2,.sd-gx-xl-2{--sd-gutter-x: 0.5rem}.sd-g-xl-3,.sd-gy-xl-3{--sd-gutter-y: 1rem}.sd-g-xl-3,.sd-gx-xl-3{--sd-gutter-x: 1rem}.sd-g-xl-4,.sd-gy-xl-4{--sd-gutter-y: 1.5rem}.sd-g-xl-4,.sd-gx-xl-4{--sd-gutter-x: 1.5rem}.sd-g-xl-5,.sd-gy-xl-5{--sd-gutter-y: 3rem}.sd-g-xl-5,.sd-gx-xl-5{--sd-gutter-x: 3rem}}.sd-flex-row-reverse{flex-direction:row-reverse !important}details.sd-dropdown{position:relative}details.sd-dropdown .sd-summary-title{font-weight:700;padding-right:3em !important;-moz-user-select:none;-ms-user-select:none;-webkit-user-select:none;user-select:none}details.sd-dropdown:hover{cursor:pointer}details.sd-dropdown .sd-summary-content{cursor:default}details.sd-dropdown summary{list-style:none;padding:1em}details.sd-dropdown summary .sd-octicon.no-title{vertical-align:middle}details.sd-dropdown[open] summary .sd-octicon.no-title{visibility:hidden}details.sd-dropdown summary::-webkit-details-marker{display:none}details.sd-dropdown summary:focus{outline:none}details.sd-dropdown .sd-summary-icon{margin-right:.5em}details.sd-dropdown .sd-summary-icon svg{opacity:.8}details.sd-dropdown summary:hover .sd-summary-up svg,details.sd-dropdown summary:hover .sd-summary-down svg{opacity:1;transform:scale(1.1)}details.sd-dropdown .sd-summary-up svg,details.sd-dropdown .sd-summary-down svg{display:block;opacity:.6}details.sd-dropdown .sd-summary-up,details.sd-dropdown .sd-summary-down{pointer-events:none;position:absolute;right:1em;top:1em}details.sd-dropdown[open]>.sd-summary-title .sd-summary-down{visibility:hidden}details.sd-dropdown:not([open])>.sd-summary-title .sd-summary-up{visibility:hidden}details.sd-dropdown:not([open]).sd-card{border:none}details.sd-dropdown:not([open])>.sd-card-header{border:1px solid var(--sd-color-card-border);border-radius:.25rem}details.sd-dropdown.sd-fade-in[open] summary~*{-moz-animation:sd-fade-in .5s ease-in-out;-webkit-animation:sd-fade-in .5s ease-in-out;animation:sd-fade-in .5s ease-in-out}details.sd-dropdown.sd-fade-in-slide-down[open] summary~*{-moz-animation:sd-fade-in .5s ease-in-out,sd-slide-down .5s ease-in-out;-webkit-animation:sd-fade-in .5s ease-in-out,sd-slide-down .5s ease-in-out;animation:sd-fade-in .5s ease-in-out,sd-slide-down .5s ease-in-out}.sd-col>.sd-dropdown{width:100%}.sd-summary-content>.sd-tab-set:first-child{margin-top:0}@keyframes sd-fade-in{0%{opacity:0}100%{opacity:1}}@keyframes sd-slide-down{0%{transform:translate(0, -10px)}100%{transform:translate(0, 0)}}.sd-tab-set{border-radius:.125rem;display:flex;flex-wrap:wrap;margin:1em 0;position:relative}.sd-tab-set>input{opacity:0;position:absolute}.sd-tab-set>input:checked+label{border-color:var(--sd-color-tabs-underline-active);color:var(--sd-color-tabs-label-active)}.sd-tab-set>input:checked+label+.sd-tab-content{display:block}.sd-tab-set>input:not(:checked)+label:hover{color:var(--sd-color-tabs-label-hover);border-color:var(--sd-color-tabs-underline-hover)}.sd-tab-set>input:focus+label{outline-style:auto}.sd-tab-set>input:not(.focus-visible)+label{outline:none;-webkit-tap-highlight-color:transparent}.sd-tab-set>label{border-bottom:.125rem solid transparent;margin-bottom:0;color:var(--sd-color-tabs-label-inactive);border-color:var(--sd-color-tabs-underline-inactive);cursor:pointer;font-size:var(--sd-fontsize-tabs-label);font-weight:700;padding:1em 1.25em .5em;transition:color 250ms;width:auto;z-index:1}html .sd-tab-set>label:hover{color:var(--sd-color-tabs-label-active)}.sd-col>.sd-tab-set{width:100%}.sd-tab-content{box-shadow:0 -0.0625rem var(--sd-color-tabs-overline),0 .0625rem var(--sd-color-tabs-underline);display:none;order:99;padding-bottom:.75rem;padding-top:.75rem;width:100%}.sd-tab-content>:first-child{margin-top:0 !important}.sd-tab-content>:last-child{margin-bottom:0 !important}.sd-tab-content>.sd-tab-set{margin:0}.sd-sphinx-override,.sd-sphinx-override *{-moz-box-sizing:border-box;-webkit-box-sizing:border-box;box-sizing:border-box}.sd-sphinx-override p{margin-top:0}:root{--sd-color-primary: #0071bc;--sd-color-secondary: #6c757d;--sd-color-success: #28a745;--sd-color-info: #17a2b8;--sd-color-warning: #f0b37e;--sd-color-danger: #dc3545;--sd-color-light: #f8f9fa;--sd-color-muted: #6c757d;--sd-color-dark: #212529;--sd-color-black: black;--sd-color-white: white;--sd-color-primary-highlight: #0060a0;--sd-color-secondary-highlight: #5c636a;--sd-color-success-highlight: #228e3b;--sd-color-info-highlight: #148a9c;--sd-color-warning-highlight: #cc986b;--sd-color-danger-highlight: #bb2d3b;--sd-color-light-highlight: #d3d4d5;--sd-color-muted-highlight: #5c636a;--sd-color-dark-highlight: #1c1f23;--sd-color-black-highlight: black;--sd-color-white-highlight: #d9d9d9;--sd-color-primary-text: #fff;--sd-color-secondary-text: #fff;--sd-color-success-text: #fff;--sd-color-info-text: #fff;--sd-color-warning-text: #212529;--sd-color-danger-text: #fff;--sd-color-light-text: #212529;--sd-color-muted-text: #fff;--sd-color-dark-text: #fff;--sd-color-black-text: #fff;--sd-color-white-text: #212529;--sd-color-shadow: rgba(0, 0, 0, 0.15);--sd-color-card-border: rgba(0, 0, 0, 0.125);--sd-color-card-border-hover: hsla(231, 99%, 66%, 1);--sd-color-card-background: transparent;--sd-color-card-text: inherit;--sd-color-card-header: transparent;--sd-color-card-footer: transparent;--sd-color-tabs-label-active: hsla(231, 99%, 66%, 1);--sd-color-tabs-label-hover: hsla(231, 99%, 66%, 1);--sd-color-tabs-label-inactive: hsl(0, 0%, 66%);--sd-color-tabs-underline-active: hsla(231, 99%, 66%, 1);--sd-color-tabs-underline-hover: rgba(178, 206, 245, 0.62);--sd-color-tabs-underline-inactive: transparent;--sd-color-tabs-overline: rgb(222, 222, 222);--sd-color-tabs-underline: rgb(222, 222, 222);--sd-fontsize-tabs-label: 1rem}
+.sd-bg-primary{background-color:var(--sd-color-primary) !important}.sd-bg-text-primary{color:var(--sd-color-primary-text) !important}button.sd-bg-primary:focus,button.sd-bg-primary:hover{background-color:var(--sd-color-primary-highlight) !important}a.sd-bg-primary:focus,a.sd-bg-primary:hover{background-color:var(--sd-color-primary-highlight) !important}.sd-bg-secondary{background-color:var(--sd-color-secondary) !important}.sd-bg-text-secondary{color:var(--sd-color-secondary-text) !important}button.sd-bg-secondary:focus,button.sd-bg-secondary:hover{background-color:var(--sd-color-secondary-highlight) !important}a.sd-bg-secondary:focus,a.sd-bg-secondary:hover{background-color:var(--sd-color-secondary-highlight) !important}.sd-bg-success{background-color:var(--sd-color-success) !important}.sd-bg-text-success{color:var(--sd-color-success-text) !important}button.sd-bg-success:focus,button.sd-bg-success:hover{background-color:var(--sd-color-success-highlight) !important}a.sd-bg-success:focus,a.sd-bg-success:hover{background-color:var(--sd-color-success-highlight) !important}.sd-bg-info{background-color:var(--sd-color-info) !important}.sd-bg-text-info{color:var(--sd-color-info-text) !important}button.sd-bg-info:focus,button.sd-bg-info:hover{background-color:var(--sd-color-info-highlight) !important}a.sd-bg-info:focus,a.sd-bg-info:hover{background-color:var(--sd-color-info-highlight) !important}.sd-bg-warning{background-color:var(--sd-color-warning) !important}.sd-bg-text-warning{color:var(--sd-color-warning-text) !important}button.sd-bg-warning:focus,button.sd-bg-warning:hover{background-color:var(--sd-color-warning-highlight) !important}a.sd-bg-warning:focus,a.sd-bg-warning:hover{background-color:var(--sd-color-warning-highlight) !important}.sd-bg-danger{background-color:var(--sd-color-danger) !important}.sd-bg-text-danger{color:var(--sd-color-danger-text) !important}button.sd-bg-danger:focus,button.sd-bg-danger:hover{background-color:var(--sd-color-danger-highlight) !important}a.sd-bg-danger:focus,a.sd-bg-danger:hover{background-color:var(--sd-color-danger-highlight) !important}.sd-bg-light{background-color:var(--sd-color-light) !important}.sd-bg-text-light{color:var(--sd-color-light-text) !important}button.sd-bg-light:focus,button.sd-bg-light:hover{background-color:var(--sd-color-light-highlight) !important}a.sd-bg-light:focus,a.sd-bg-light:hover{background-color:var(--sd-color-light-highlight) !important}.sd-bg-muted{background-color:var(--sd-color-muted) !important}.sd-bg-text-muted{color:var(--sd-color-muted-text) !important}button.sd-bg-muted:focus,button.sd-bg-muted:hover{background-color:var(--sd-color-muted-highlight) !important}a.sd-bg-muted:focus,a.sd-bg-muted:hover{background-color:var(--sd-color-muted-highlight) !important}.sd-bg-dark{background-color:var(--sd-color-dark) !important}.sd-bg-text-dark{color:var(--sd-color-dark-text) !important}button.sd-bg-dark:focus,button.sd-bg-dark:hover{background-color:var(--sd-color-dark-highlight) !important}a.sd-bg-dark:focus,a.sd-bg-dark:hover{background-color:var(--sd-color-dark-highlight) !important}.sd-bg-black{background-color:var(--sd-color-black) !important}.sd-bg-text-black{color:var(--sd-color-black-text) !important}button.sd-bg-black:focus,button.sd-bg-black:hover{background-color:var(--sd-color-black-highlight) !important}a.sd-bg-black:focus,a.sd-bg-black:hover{background-color:var(--sd-color-black-highlight) !important}.sd-bg-white{background-color:var(--sd-color-white) !important}.sd-bg-text-white{color:var(--sd-color-white-text) !important}button.sd-bg-white:focus,button.sd-bg-white:hover{background-color:var(--sd-color-white-highlight) !important}a.sd-bg-white:focus,a.sd-bg-white:hover{background-color:var(--sd-color-white-highlight) !important}.sd-text-primary,.sd-text-primary>p{color:var(--sd-color-primary) !important}a.sd-text-primary:focus,a.sd-text-primary:hover{color:var(--sd-color-primary-highlight) !important}.sd-text-secondary,.sd-text-secondary>p{color:var(--sd-color-secondary) !important}a.sd-text-secondary:focus,a.sd-text-secondary:hover{color:var(--sd-color-secondary-highlight) !important}.sd-text-success,.sd-text-success>p{color:var(--sd-color-success) !important}a.sd-text-success:focus,a.sd-text-success:hover{color:var(--sd-color-success-highlight) !important}.sd-text-info,.sd-text-info>p{color:var(--sd-color-info) !important}a.sd-text-info:focus,a.sd-text-info:hover{color:var(--sd-color-info-highlight) !important}.sd-text-warning,.sd-text-warning>p{color:var(--sd-color-warning) !important}a.sd-text-warning:focus,a.sd-text-warning:hover{color:var(--sd-color-warning-highlight) !important}.sd-text-danger,.sd-text-danger>p{color:var(--sd-color-danger) !important}a.sd-text-danger:focus,a.sd-text-danger:hover{color:var(--sd-color-danger-highlight) !important}.sd-text-light,.sd-text-light>p{color:var(--sd-color-light) !important}a.sd-text-light:focus,a.sd-text-light:hover{color:var(--sd-color-light-highlight) !important}.sd-text-muted,.sd-text-muted>p{color:var(--sd-color-muted) !important}a.sd-text-muted:focus,a.sd-text-muted:hover{color:var(--sd-color-muted-highlight) !important}.sd-text-dark,.sd-text-dark>p{color:var(--sd-color-dark) !important}a.sd-text-dark:focus,a.sd-text-dark:hover{color:var(--sd-color-dark-highlight) !important}.sd-text-black,.sd-text-black>p{color:var(--sd-color-black) !important}a.sd-text-black:focus,a.sd-text-black:hover{color:var(--sd-color-black-highlight) !important}.sd-text-white,.sd-text-white>p{color:var(--sd-color-white) !important}a.sd-text-white:focus,a.sd-text-white:hover{color:var(--sd-color-white-highlight) !important}.sd-outline-primary{border-color:var(--sd-color-primary) !important;border-style:solid !important;border-width:1px !important}a.sd-outline-primary:focus,a.sd-outline-primary:hover{border-color:var(--sd-color-primary-highlight) !important}.sd-outline-secondary{border-color:var(--sd-color-secondary) !important;border-style:solid !important;border-width:1px !important}a.sd-outline-secondary:focus,a.sd-outline-secondary:hover{border-color:var(--sd-color-secondary-highlight) !important}.sd-outline-success{border-color:var(--sd-color-success) !important;border-style:solid !important;border-width:1px !important}a.sd-outline-success:focus,a.sd-outline-success:hover{border-color:var(--sd-color-success-highlight) !important}.sd-outline-info{border-color:var(--sd-color-info) !important;border-style:solid !important;border-width:1px !important}a.sd-outline-info:focus,a.sd-outline-info:hover{border-color:var(--sd-color-info-highlight) !important}.sd-outline-warning{border-color:var(--sd-color-warning) !important;border-style:solid !important;border-width:1px !important}a.sd-outline-warning:focus,a.sd-outline-warning:hover{border-color:var(--sd-color-warning-highlight) !important}.sd-outline-danger{border-color:var(--sd-color-danger) !important;border-style:solid !important;border-width:1px !important}a.sd-outline-danger:focus,a.sd-outline-danger:hover{border-color:var(--sd-color-danger-highlight) !important}.sd-outline-light{border-color:var(--sd-color-light) !important;border-style:solid !important;border-width:1px !important}a.sd-outline-light:focus,a.sd-outline-light:hover{border-color:var(--sd-color-light-highlight) !important}.sd-outline-muted{border-color:var(--sd-color-muted) !important;border-style:solid !important;border-width:1px !important}a.sd-outline-muted:focus,a.sd-outline-muted:hover{border-color:var(--sd-color-muted-highlight) !important}.sd-outline-dark{border-color:var(--sd-color-dark) !important;border-style:solid !important;border-width:1px !important}a.sd-outline-dark:focus,a.sd-outline-dark:hover{border-color:var(--sd-color-dark-highlight) !important}.sd-outline-black{border-color:var(--sd-color-black) !important;border-style:solid !important;border-width:1px !important}a.sd-outline-black:focus,a.sd-outline-black:hover{border-color:var(--sd-color-black-highlight) !important}.sd-outline-white{border-color:var(--sd-color-white) !important;border-style:solid !important;border-width:1px !important}a.sd-outline-white:focus,a.sd-outline-white:hover{border-color:var(--sd-color-white-highlight) !important}.sd-bg-transparent{background-color:transparent !important}.sd-outline-transparent{border-color:transparent !important}.sd-text-transparent{color:transparent !important}.sd-p-0{padding:0 !important}.sd-pt-0,.sd-py-0{padding-top:0 !important}.sd-pr-0,.sd-px-0{padding-right:0 !important}.sd-pb-0,.sd-py-0{padding-bottom:0 !important}.sd-pl-0,.sd-px-0{padding-left:0 !important}.sd-p-1{padding:.25rem !important}.sd-pt-1,.sd-py-1{padding-top:.25rem !important}.sd-pr-1,.sd-px-1{padding-right:.25rem !important}.sd-pb-1,.sd-py-1{padding-bottom:.25rem !important}.sd-pl-1,.sd-px-1{padding-left:.25rem !important}.sd-p-2{padding:.5rem !important}.sd-pt-2,.sd-py-2{padding-top:.5rem !important}.sd-pr-2,.sd-px-2{padding-right:.5rem !important}.sd-pb-2,.sd-py-2{padding-bottom:.5rem !important}.sd-pl-2,.sd-px-2{padding-left:.5rem !important}.sd-p-3{padding:1rem !important}.sd-pt-3,.sd-py-3{padding-top:1rem !important}.sd-pr-3,.sd-px-3{padding-right:1rem !important}.sd-pb-3,.sd-py-3{padding-bottom:1rem !important}.sd-pl-3,.sd-px-3{padding-left:1rem !important}.sd-p-4{padding:1.5rem !important}.sd-pt-4,.sd-py-4{padding-top:1.5rem !important}.sd-pr-4,.sd-px-4{padding-right:1.5rem !important}.sd-pb-4,.sd-py-4{padding-bottom:1.5rem !important}.sd-pl-4,.sd-px-4{padding-left:1.5rem !important}.sd-p-5{padding:3rem !important}.sd-pt-5,.sd-py-5{padding-top:3rem !important}.sd-pr-5,.sd-px-5{padding-right:3rem !important}.sd-pb-5,.sd-py-5{padding-bottom:3rem !important}.sd-pl-5,.sd-px-5{padding-left:3rem !important}.sd-m-auto{margin:auto !important}.sd-mt-auto,.sd-my-auto{margin-top:auto !important}.sd-mr-auto,.sd-mx-auto{margin-right:auto !important}.sd-mb-auto,.sd-my-auto{margin-bottom:auto !important}.sd-ml-auto,.sd-mx-auto{margin-left:auto !important}.sd-m-0{margin:0 !important}.sd-mt-0,.sd-my-0{margin-top:0 !important}.sd-mr-0,.sd-mx-0{margin-right:0 !important}.sd-mb-0,.sd-my-0{margin-bottom:0 !important}.sd-ml-0,.sd-mx-0{margin-left:0 !important}.sd-m-1{margin:.25rem !important}.sd-mt-1,.sd-my-1{margin-top:.25rem !important}.sd-mr-1,.sd-mx-1{margin-right:.25rem !important}.sd-mb-1,.sd-my-1{margin-bottom:.25rem !important}.sd-ml-1,.sd-mx-1{margin-left:.25rem !important}.sd-m-2{margin:.5rem !important}.sd-mt-2,.sd-my-2{margin-top:.5rem !important}.sd-mr-2,.sd-mx-2{margin-right:.5rem !important}.sd-mb-2,.sd-my-2{margin-bottom:.5rem !important}.sd-ml-2,.sd-mx-2{margin-left:.5rem !important}.sd-m-3{margin:1rem !important}.sd-mt-3,.sd-my-3{margin-top:1rem !important}.sd-mr-3,.sd-mx-3{margin-right:1rem !important}.sd-mb-3,.sd-my-3{margin-bottom:1rem !important}.sd-ml-3,.sd-mx-3{margin-left:1rem !important}.sd-m-4{margin:1.5rem !important}.sd-mt-4,.sd-my-4{margin-top:1.5rem !important}.sd-mr-4,.sd-mx-4{margin-right:1.5rem !important}.sd-mb-4,.sd-my-4{margin-bottom:1.5rem !important}.sd-ml-4,.sd-mx-4{margin-left:1.5rem !important}.sd-m-5{margin:3rem !important}.sd-mt-5,.sd-my-5{margin-top:3rem !important}.sd-mr-5,.sd-mx-5{margin-right:3rem !important}.sd-mb-5,.sd-my-5{margin-bottom:3rem !important}.sd-ml-5,.sd-mx-5{margin-left:3rem !important}.sd-w-25{width:25% !important}.sd-w-50{width:50% !important}.sd-w-75{width:75% !important}.sd-w-100{width:100% !important}.sd-w-auto{width:auto !important}.sd-h-25{height:25% !important}.sd-h-50{height:50% !important}.sd-h-75{height:75% !important}.sd-h-100{height:100% !important}.sd-h-auto{height:auto !important}.sd-d-none{display:none !important}.sd-d-inline{display:inline !important}.sd-d-inline-block{display:inline-block !important}.sd-d-block{display:block !important}.sd-d-grid{display:grid !important}.sd-d-flex-row{display:-ms-flexbox !important;display:flex !important;flex-direction:row !important}.sd-d-flex-column{display:-ms-flexbox !important;display:flex !important;flex-direction:column !important}.sd-d-inline-flex{display:-ms-inline-flexbox !important;display:inline-flex !important}@media(min-width: 576px){.sd-d-sm-none{display:none !important}.sd-d-sm-inline{display:inline !important}.sd-d-sm-inline-block{display:inline-block !important}.sd-d-sm-block{display:block !important}.sd-d-sm-grid{display:grid !important}.sd-d-sm-flex{display:-ms-flexbox !important;display:flex !important}.sd-d-sm-inline-flex{display:-ms-inline-flexbox !important;display:inline-flex !important}}@media(min-width: 768px){.sd-d-md-none{display:none !important}.sd-d-md-inline{display:inline !important}.sd-d-md-inline-block{display:inline-block !important}.sd-d-md-block{display:block !important}.sd-d-md-grid{display:grid !important}.sd-d-md-flex{display:-ms-flexbox !important;display:flex !important}.sd-d-md-inline-flex{display:-ms-inline-flexbox !important;display:inline-flex !important}}@media(min-width: 992px){.sd-d-lg-none{display:none !important}.sd-d-lg-inline{display:inline !important}.sd-d-lg-inline-block{display:inline-block !important}.sd-d-lg-block{display:block !important}.sd-d-lg-grid{display:grid !important}.sd-d-lg-flex{display:-ms-flexbox !important;display:flex !important}.sd-d-lg-inline-flex{display:-ms-inline-flexbox !important;display:inline-flex !important}}@media(min-width: 1200px){.sd-d-xl-none{display:none !important}.sd-d-xl-inline{display:inline !important}.sd-d-xl-inline-block{display:inline-block !important}.sd-d-xl-block{display:block !important}.sd-d-xl-grid{display:grid !important}.sd-d-xl-flex{display:-ms-flexbox !important;display:flex !important}.sd-d-xl-inline-flex{display:-ms-inline-flexbox !important;display:inline-flex !important}}.sd-align-major-start{justify-content:flex-start !important}.sd-align-major-end{justify-content:flex-end !important}.sd-align-major-center{justify-content:center !important}.sd-align-major-justify{justify-content:space-between !important}.sd-align-major-spaced{justify-content:space-evenly !important}.sd-align-minor-start{align-items:flex-start !important}.sd-align-minor-end{align-items:flex-end !important}.sd-align-minor-center{align-items:center !important}.sd-align-minor-stretch{align-items:stretch !important}.sd-text-justify{text-align:justify !important}.sd-text-left{text-align:left !important}.sd-text-right{text-align:right !important}.sd-text-center{text-align:center !important}.sd-font-weight-light{font-weight:300 !important}.sd-font-weight-lighter{font-weight:lighter !important}.sd-font-weight-normal{font-weight:400 !important}.sd-font-weight-bold{font-weight:700 !important}.sd-font-weight-bolder{font-weight:bolder !important}.sd-font-italic{font-style:italic !important}.sd-text-decoration-none{text-decoration:none !important}.sd-text-lowercase{text-transform:lowercase !important}.sd-text-uppercase{text-transform:uppercase !important}.sd-text-capitalize{text-transform:capitalize !important}.sd-text-wrap{white-space:normal !important}.sd-text-nowrap{white-space:nowrap !important}.sd-text-truncate{overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.sd-fs-1,.sd-fs-1>p{font-size:calc(1.375rem + 1.5vw) !important;line-height:unset !important}.sd-fs-2,.sd-fs-2>p{font-size:calc(1.325rem + 0.9vw) !important;line-height:unset !important}.sd-fs-3,.sd-fs-3>p{font-size:calc(1.3rem + 0.6vw) !important;line-height:unset !important}.sd-fs-4,.sd-fs-4>p{font-size:calc(1.275rem + 0.3vw) !important;line-height:unset !important}.sd-fs-5,.sd-fs-5>p{font-size:1.25rem !important;line-height:unset !important}.sd-fs-6,.sd-fs-6>p{font-size:1rem !important;line-height:unset !important}.sd-border-0{border:0 solid !important}.sd-border-top-0{border-top:0 solid !important}.sd-border-bottom-0{border-bottom:0 solid !important}.sd-border-right-0{border-right:0 solid !important}.sd-border-left-0{border-left:0 solid !important}.sd-border-1{border:1px solid !important}.sd-border-top-1{border-top:1px solid !important}.sd-border-bottom-1{border-bottom:1px solid !important}.sd-border-right-1{border-right:1px solid !important}.sd-border-left-1{border-left:1px solid !important}.sd-border-2{border:2px solid !important}.sd-border-top-2{border-top:2px solid !important}.sd-border-bottom-2{border-bottom:2px solid !important}.sd-border-right-2{border-right:2px solid !important}.sd-border-left-2{border-left:2px solid !important}.sd-border-3{border:3px solid !important}.sd-border-top-3{border-top:3px solid !important}.sd-border-bottom-3{border-bottom:3px solid !important}.sd-border-right-3{border-right:3px solid !important}.sd-border-left-3{border-left:3px solid !important}.sd-border-4{border:4px solid !important}.sd-border-top-4{border-top:4px solid !important}.sd-border-bottom-4{border-bottom:4px solid !important}.sd-border-right-4{border-right:4px solid !important}.sd-border-left-4{border-left:4px solid !important}.sd-border-5{border:5px solid !important}.sd-border-top-5{border-top:5px solid !important}.sd-border-bottom-5{border-bottom:5px solid !important}.sd-border-right-5{border-right:5px solid !important}.sd-border-left-5{border-left:5px solid !important}.sd-rounded-0{border-radius:0 !important}.sd-rounded-1{border-radius:.2rem !important}.sd-rounded-2{border-radius:.3rem !important}.sd-rounded-3{border-radius:.5rem !important}.sd-rounded-pill{border-radius:50rem !important}.sd-rounded-circle{border-radius:50% !important}.shadow-none{box-shadow:none !important}.sd-shadow-sm{box-shadow:0 .125rem .25rem var(--sd-color-shadow) !important}.sd-shadow-md{box-shadow:0 .5rem 1rem var(--sd-color-shadow) !important}.sd-shadow-lg{box-shadow:0 1rem 3rem var(--sd-color-shadow) !important}@keyframes sd-slide-from-left{0%{transform:translateX(-100%)}100%{transform:translateX(0)}}@keyframes sd-slide-from-right{0%{transform:translateX(200%)}100%{transform:translateX(0)}}@keyframes sd-grow100{0%{transform:scale(0);opacity:.5}100%{transform:scale(1);opacity:1}}@keyframes sd-grow50{0%{transform:scale(0.5);opacity:.5}100%{transform:scale(1);opacity:1}}@keyframes sd-grow50-rot20{0%{transform:scale(0.5) rotateZ(-20deg);opacity:.5}75%{transform:scale(1) rotateZ(5deg);opacity:1}95%{transform:scale(1) rotateZ(-1deg);opacity:1}100%{transform:scale(1) rotateZ(0);opacity:1}}.sd-animate-slide-from-left{animation:1s ease-out 0s 1 normal none running sd-slide-from-left}.sd-animate-slide-from-right{animation:1s ease-out 0s 1 normal none running sd-slide-from-right}.sd-animate-grow100{animation:1s ease-out 0s 1 normal none running sd-grow100}.sd-animate-grow50{animation:1s ease-out 0s 1 normal none running sd-grow50}.sd-animate-grow50-rot20{animation:1s ease-out 0s 1 normal none running sd-grow50-rot20}.sd-badge{display:inline-block;padding:.35em .65em;font-size:.75em;font-weight:700;line-height:1;text-align:center;white-space:nowrap;vertical-align:baseline;border-radius:.25rem}.sd-badge:empty{display:none}a.sd-badge{text-decoration:none}.sd-btn .sd-badge{position:relative;top:-1px}.sd-btn{background-color:transparent;border:1px solid transparent;border-radius:.25rem;cursor:pointer;display:inline-block;font-weight:400;font-size:1rem;line-height:1.5;padding:.375rem .75rem;text-align:center;text-decoration:none;transition:color .15s ease-in-out,background-color .15s ease-in-out,border-color .15s ease-in-out,box-shadow .15s ease-in-out;vertical-align:middle;user-select:none;-moz-user-select:none;-ms-user-select:none;-webkit-user-select:none}.sd-btn:hover{text-decoration:none}@media(prefers-reduced-motion: reduce){.sd-btn{transition:none}}.sd-btn-primary,.sd-btn-outline-primary:hover,.sd-btn-outline-primary:focus{color:var(--sd-color-primary-text) !important;background-color:var(--sd-color-primary) !important;border-color:var(--sd-color-primary) !important;border-width:1px !important;border-style:solid !important}.sd-btn-primary:hover,.sd-btn-primary:focus{color:var(--sd-color-primary-text) !important;background-color:var(--sd-color-primary-highlight) !important;border-color:var(--sd-color-primary-highlight) !important;border-width:1px !important;border-style:solid !important}.sd-btn-outline-primary{color:var(--sd-color-primary) !important;border-color:var(--sd-color-primary) !important;border-width:1px !important;border-style:solid !important}.sd-btn-secondary,.sd-btn-outline-secondary:hover,.sd-btn-outline-secondary:focus{color:var(--sd-color-secondary-text) !important;background-color:var(--sd-color-secondary) !important;border-color:var(--sd-color-secondary) !important;border-width:1px !important;border-style:solid !important}.sd-btn-secondary:hover,.sd-btn-secondary:focus{color:var(--sd-color-secondary-text) !important;background-color:var(--sd-color-secondary-highlight) !important;border-color:var(--sd-color-secondary-highlight) !important;border-width:1px !important;border-style:solid !important}.sd-btn-outline-secondary{color:var(--sd-color-secondary) !important;border-color:var(--sd-color-secondary) !important;border-width:1px !important;border-style:solid !important}.sd-btn-success,.sd-btn-outline-success:hover,.sd-btn-outline-success:focus{color:var(--sd-color-success-text) !important;background-color:var(--sd-color-success) !important;border-color:var(--sd-color-success) !important;border-width:1px !important;border-style:solid !important}.sd-btn-success:hover,.sd-btn-success:focus{color:var(--sd-color-success-text) !important;background-color:var(--sd-color-success-highlight) !important;border-color:var(--sd-color-success-highlight) !important;border-width:1px !important;border-style:solid !important}.sd-btn-outline-success{color:var(--sd-color-success) !important;border-color:var(--sd-color-success) !important;border-width:1px !important;border-style:solid !important}.sd-btn-info,.sd-btn-outline-info:hover,.sd-btn-outline-info:focus{color:var(--sd-color-info-text) !important;background-color:var(--sd-color-info) !important;border-color:var(--sd-color-info) !important;border-width:1px !important;border-style:solid !important}.sd-btn-info:hover,.sd-btn-info:focus{color:var(--sd-color-info-text) !important;background-color:var(--sd-color-info-highlight) !important;border-color:var(--sd-color-info-highlight) !important;border-width:1px !important;border-style:solid !important}.sd-btn-outline-info{color:var(--sd-color-info) !important;border-color:var(--sd-color-info) !important;border-width:1px !important;border-style:solid !important}.sd-btn-warning,.sd-btn-outline-warning:hover,.sd-btn-outline-warning:focus{color:var(--sd-color-warning-text) !important;background-color:var(--sd-color-warning) !important;border-color:var(--sd-color-warning) !important;border-width:1px !important;border-style:solid !important}.sd-btn-warning:hover,.sd-btn-warning:focus{color:var(--sd-color-warning-text) !important;background-color:var(--sd-color-warning-highlight) !important;border-color:var(--sd-color-warning-highlight) !important;border-width:1px !important;border-style:solid !important}.sd-btn-outline-warning{color:var(--sd-color-warning) !important;border-color:var(--sd-color-warning) !important;border-width:1px !important;border-style:solid !important}.sd-btn-danger,.sd-btn-outline-danger:hover,.sd-btn-outline-danger:focus{color:var(--sd-color-danger-text) !important;background-color:var(--sd-color-danger) !important;border-color:var(--sd-color-danger) !important;border-width:1px !important;border-style:solid !important}.sd-btn-danger:hover,.sd-btn-danger:focus{color:var(--sd-color-danger-text) !important;background-color:var(--sd-color-danger-highlight) !important;border-color:var(--sd-color-danger-highlight) !important;border-width:1px !important;border-style:solid !important}.sd-btn-outline-danger{color:var(--sd-color-danger) !important;border-color:var(--sd-color-danger) !important;border-width:1px !important;border-style:solid !important}.sd-btn-light,.sd-btn-outline-light:hover,.sd-btn-outline-light:focus{color:var(--sd-color-light-text) !important;background-color:var(--sd-color-light) !important;border-color:var(--sd-color-light) !important;border-width:1px !important;border-style:solid !important}.sd-btn-light:hover,.sd-btn-light:focus{color:var(--sd-color-light-text) !important;background-color:var(--sd-color-light-highlight) !important;border-color:var(--sd-color-light-highlight) !important;border-width:1px !important;border-style:solid !important}.sd-btn-outline-light{color:var(--sd-color-light) !important;border-color:var(--sd-color-light) !important;border-width:1px !important;border-style:solid !important}.sd-btn-muted,.sd-btn-outline-muted:hover,.sd-btn-outline-muted:focus{color:var(--sd-color-muted-text) !important;background-color:var(--sd-color-muted) !important;border-color:var(--sd-color-muted) !important;border-width:1px !important;border-style:solid !important}.sd-btn-muted:hover,.sd-btn-muted:focus{color:var(--sd-color-muted-text) !important;background-color:var(--sd-color-muted-highlight) !important;border-color:var(--sd-color-muted-highlight) !important;border-width:1px !important;border-style:solid !important}.sd-btn-outline-muted{color:var(--sd-color-muted) !important;border-color:var(--sd-color-muted) !important;border-width:1px !important;border-style:solid !important}.sd-btn-dark,.sd-btn-outline-dark:hover,.sd-btn-outline-dark:focus{color:var(--sd-color-dark-text) !important;background-color:var(--sd-color-dark) !important;border-color:var(--sd-color-dark) !important;border-width:1px !important;border-style:solid !important}.sd-btn-dark:hover,.sd-btn-dark:focus{color:var(--sd-color-dark-text) !important;background-color:var(--sd-color-dark-highlight) !important;border-color:var(--sd-color-dark-highlight) !important;border-width:1px !important;border-style:solid !important}.sd-btn-outline-dark{color:var(--sd-color-dark) !important;border-color:var(--sd-color-dark) !important;border-width:1px !important;border-style:solid !important}.sd-btn-black,.sd-btn-outline-black:hover,.sd-btn-outline-black:focus{color:var(--sd-color-black-text) !important;background-color:var(--sd-color-black) !important;border-color:var(--sd-color-black) !important;border-width:1px !important;border-style:solid !important}.sd-btn-black:hover,.sd-btn-black:focus{color:var(--sd-color-black-text) !important;background-color:var(--sd-color-black-highlight) !important;border-color:var(--sd-color-black-highlight) !important;border-width:1px !important;border-style:solid !important}.sd-btn-outline-black{color:var(--sd-color-black) !important;border-color:var(--sd-color-black) !important;border-width:1px !important;border-style:solid !important}.sd-btn-white,.sd-btn-outline-white:hover,.sd-btn-outline-white:focus{color:var(--sd-color-white-text) !important;background-color:var(--sd-color-white) !important;border-color:var(--sd-color-white) !important;border-width:1px !important;border-style:solid !important}.sd-btn-white:hover,.sd-btn-white:focus{color:var(--sd-color-white-text) !important;background-color:var(--sd-color-white-highlight) !important;border-color:var(--sd-color-white-highlight) !important;border-width:1px !important;border-style:solid !important}.sd-btn-outline-white{color:var(--sd-color-white) !important;border-color:var(--sd-color-white) !important;border-width:1px !important;border-style:solid !important}.sd-stretched-link::after{position:absolute;top:0;right:0;bottom:0;left:0;z-index:1;content:""}.sd-hide-link-text{font-size:0}.sd-octicon,.sd-material-icon{display:inline-block;fill:currentColor;vertical-align:middle}.sd-avatar-xs{border-radius:50%;object-fit:cover;object-position:center;width:1rem;height:1rem}.sd-avatar-sm{border-radius:50%;object-fit:cover;object-position:center;width:3rem;height:3rem}.sd-avatar-md{border-radius:50%;object-fit:cover;object-position:center;width:5rem;height:5rem}.sd-avatar-lg{border-radius:50%;object-fit:cover;object-position:center;width:7rem;height:7rem}.sd-avatar-xl{border-radius:50%;object-fit:cover;object-position:center;width:10rem;height:10rem}.sd-avatar-inherit{border-radius:50%;object-fit:cover;object-position:center;width:inherit;height:inherit}.sd-avatar-initial{border-radius:50%;object-fit:cover;object-position:center;width:initial;height:initial}.sd-card{background-clip:border-box;background-color:var(--sd-color-card-background);border:1px solid var(--sd-color-card-border);border-radius:.25rem;color:var(--sd-color-card-text);display:-ms-flexbox;display:flex;-ms-flex-direction:column;flex-direction:column;min-width:0;position:relative;word-wrap:break-word}.sd-card>hr{margin-left:0;margin-right:0}.sd-card-hover:hover{border-color:var(--sd-color-card-border-hover);transform:scale(1.01)}.sd-card-body{-ms-flex:1 1 auto;flex:1 1 auto;padding:1rem 1rem}.sd-card-title{margin-bottom:.5rem}.sd-card-subtitle{margin-top:-0.25rem;margin-bottom:0}.sd-card-text:last-child{margin-bottom:0}.sd-card-link:hover{text-decoration:none}.sd-card-link+.card-link{margin-left:1rem}.sd-card-header{padding:.5rem 1rem;margin-bottom:0;background-color:var(--sd-color-card-header);border-bottom:1px solid var(--sd-color-card-border)}.sd-card-header:first-child{border-radius:calc(0.25rem - 1px) calc(0.25rem - 1px) 0 0}.sd-card-footer{padding:.5rem 1rem;background-color:var(--sd-color-card-footer);border-top:1px solid var(--sd-color-card-border)}.sd-card-footer:last-child{border-radius:0 0 calc(0.25rem - 1px) calc(0.25rem - 1px)}.sd-card-header-tabs{margin-right:-0.5rem;margin-bottom:-0.5rem;margin-left:-0.5rem;border-bottom:0}.sd-card-header-pills{margin-right:-0.5rem;margin-left:-0.5rem}.sd-card-img-overlay{position:absolute;top:0;right:0;bottom:0;left:0;padding:1rem;border-radius:calc(0.25rem - 1px)}.sd-card-img,.sd-card-img-bottom,.sd-card-img-top{width:100%}.sd-card-img,.sd-card-img-top{border-top-left-radius:calc(0.25rem - 1px);border-top-right-radius:calc(0.25rem - 1px)}.sd-card-img,.sd-card-img-bottom{border-bottom-left-radius:calc(0.25rem - 1px);border-bottom-right-radius:calc(0.25rem - 1px)}.sd-cards-carousel{width:100%;display:flex;flex-wrap:nowrap;-ms-flex-direction:row;flex-direction:row;overflow-x:hidden;scroll-snap-type:x mandatory}.sd-cards-carousel.sd-show-scrollbar{overflow-x:auto}.sd-cards-carousel:hover,.sd-cards-carousel:focus{overflow-x:auto}.sd-cards-carousel>.sd-card{flex-shrink:0;scroll-snap-align:start}.sd-cards-carousel>.sd-card:not(:last-child){margin-right:3px}.sd-card-cols-1>.sd-card{width:90%}.sd-card-cols-2>.sd-card{width:45%}.sd-card-cols-3>.sd-card{width:30%}.sd-card-cols-4>.sd-card{width:22.5%}.sd-card-cols-5>.sd-card{width:18%}.sd-card-cols-6>.sd-card{width:15%}.sd-card-cols-7>.sd-card{width:12.8571428571%}.sd-card-cols-8>.sd-card{width:11.25%}.sd-card-cols-9>.sd-card{width:10%}.sd-card-cols-10>.sd-card{width:9%}.sd-card-cols-11>.sd-card{width:8.1818181818%}.sd-card-cols-12>.sd-card{width:7.5%}.sd-container,.sd-container-fluid,.sd-container-lg,.sd-container-md,.sd-container-sm,.sd-container-xl{margin-left:auto;margin-right:auto;padding-left:var(--sd-gutter-x, 0.75rem);padding-right:var(--sd-gutter-x, 0.75rem);width:100%}@media(min-width: 576px){.sd-container-sm,.sd-container{max-width:540px}}@media(min-width: 768px){.sd-container-md,.sd-container-sm,.sd-container{max-width:720px}}@media(min-width: 992px){.sd-container-lg,.sd-container-md,.sd-container-sm,.sd-container{max-width:960px}}@media(min-width: 1200px){.sd-container-xl,.sd-container-lg,.sd-container-md,.sd-container-sm,.sd-container{max-width:1140px}}.sd-row{--sd-gutter-x: 1.5rem;--sd-gutter-y: 0;display:-ms-flexbox;display:flex;-ms-flex-wrap:wrap;flex-wrap:wrap;margin-top:calc(var(--sd-gutter-y) * -1);margin-right:calc(var(--sd-gutter-x) * -0.5);margin-left:calc(var(--sd-gutter-x) * -0.5)}.sd-row>*{box-sizing:border-box;flex-shrink:0;width:100%;max-width:100%;padding-right:calc(var(--sd-gutter-x) * 0.5);padding-left:calc(var(--sd-gutter-x) * 0.5);margin-top:var(--sd-gutter-y)}.sd-col{flex:1 0 0%;-ms-flex:1 0 0%}.sd-row-cols-auto>*{flex:0 0 auto;width:auto}.sd-row-cols-1>*{flex:0 0 auto;-ms-flex:0 0 auto;width:100%}.sd-row-cols-2>*{flex:0 0 auto;-ms-flex:0 0 auto;width:50%}.sd-row-cols-3>*{flex:0 0 auto;-ms-flex:0 0 auto;width:33.3333333333%}.sd-row-cols-4>*{flex:0 0 auto;-ms-flex:0 0 auto;width:25%}.sd-row-cols-5>*{flex:0 0 auto;-ms-flex:0 0 auto;width:20%}.sd-row-cols-6>*{flex:0 0 auto;-ms-flex:0 0 auto;width:16.6666666667%}.sd-row-cols-7>*{flex:0 0 auto;-ms-flex:0 0 auto;width:14.2857142857%}.sd-row-cols-8>*{flex:0 0 auto;-ms-flex:0 0 auto;width:12.5%}.sd-row-cols-9>*{flex:0 0 auto;-ms-flex:0 0 auto;width:11.1111111111%}.sd-row-cols-10>*{flex:0 0 auto;-ms-flex:0 0 auto;width:10%}.sd-row-cols-11>*{flex:0 0 auto;-ms-flex:0 0 auto;width:9.0909090909%}.sd-row-cols-12>*{flex:0 0 auto;-ms-flex:0 0 auto;width:8.3333333333%}@media(min-width: 576px){.sd-col-sm{flex:1 0 0%;-ms-flex:1 0 0%}.sd-row-cols-sm-auto{flex:1 0 auto;-ms-flex:1 0 auto;width:100%}.sd-row-cols-sm-1>*{flex:0 0 auto;-ms-flex:0 0 auto;width:100%}.sd-row-cols-sm-2>*{flex:0 0 auto;-ms-flex:0 0 auto;width:50%}.sd-row-cols-sm-3>*{flex:0 0 auto;-ms-flex:0 0 auto;width:33.3333333333%}.sd-row-cols-sm-4>*{flex:0 0 auto;-ms-flex:0 0 auto;width:25%}.sd-row-cols-sm-5>*{flex:0 0 auto;-ms-flex:0 0 auto;width:20%}.sd-row-cols-sm-6>*{flex:0 0 auto;-ms-flex:0 0 auto;width:16.6666666667%}.sd-row-cols-sm-7>*{flex:0 0 auto;-ms-flex:0 0 auto;width:14.2857142857%}.sd-row-cols-sm-8>*{flex:0 0 auto;-ms-flex:0 0 auto;width:12.5%}.sd-row-cols-sm-9>*{flex:0 0 auto;-ms-flex:0 0 auto;width:11.1111111111%}.sd-row-cols-sm-10>*{flex:0 0 auto;-ms-flex:0 0 auto;width:10%}.sd-row-cols-sm-11>*{flex:0 0 auto;-ms-flex:0 0 auto;width:9.0909090909%}.sd-row-cols-sm-12>*{flex:0 0 auto;-ms-flex:0 0 auto;width:8.3333333333%}}@media(min-width: 768px){.sd-col-md{flex:1 0 0%;-ms-flex:1 0 0%}.sd-row-cols-md-auto{flex:1 0 auto;-ms-flex:1 0 auto;width:100%}.sd-row-cols-md-1>*{flex:0 0 auto;-ms-flex:0 0 auto;width:100%}.sd-row-cols-md-2>*{flex:0 0 auto;-ms-flex:0 0 auto;width:50%}.sd-row-cols-md-3>*{flex:0 0 auto;-ms-flex:0 0 auto;width:33.3333333333%}.sd-row-cols-md-4>*{flex:0 0 auto;-ms-flex:0 0 auto;width:25%}.sd-row-cols-md-5>*{flex:0 0 auto;-ms-flex:0 0 auto;width:20%}.sd-row-cols-md-6>*{flex:0 0 auto;-ms-flex:0 0 auto;width:16.6666666667%}.sd-row-cols-md-7>*{flex:0 0 auto;-ms-flex:0 0 auto;width:14.2857142857%}.sd-row-cols-md-8>*{flex:0 0 auto;-ms-flex:0 0 auto;width:12.5%}.sd-row-cols-md-9>*{flex:0 0 auto;-ms-flex:0 0 auto;width:11.1111111111%}.sd-row-cols-md-10>*{flex:0 0 auto;-ms-flex:0 0 auto;width:10%}.sd-row-cols-md-11>*{flex:0 0 auto;-ms-flex:0 0 auto;width:9.0909090909%}.sd-row-cols-md-12>*{flex:0 0 auto;-ms-flex:0 0 auto;width:8.3333333333%}}@media(min-width: 992px){.sd-col-lg{flex:1 0 0%;-ms-flex:1 0 0%}.sd-row-cols-lg-auto{flex:1 0 auto;-ms-flex:1 0 auto;width:100%}.sd-row-cols-lg-1>*{flex:0 0 auto;-ms-flex:0 0 auto;width:100%}.sd-row-cols-lg-2>*{flex:0 0 auto;-ms-flex:0 0 auto;width:50%}.sd-row-cols-lg-3>*{flex:0 0 auto;-ms-flex:0 0 auto;width:33.3333333333%}.sd-row-cols-lg-4>*{flex:0 0 auto;-ms-flex:0 0 auto;width:25%}.sd-row-cols-lg-5>*{flex:0 0 auto;-ms-flex:0 0 auto;width:20%}.sd-row-cols-lg-6>*{flex:0 0 auto;-ms-flex:0 0 auto;width:16.6666666667%}.sd-row-cols-lg-7>*{flex:0 0 auto;-ms-flex:0 0 auto;width:14.2857142857%}.sd-row-cols-lg-8>*{flex:0 0 auto;-ms-flex:0 0 auto;width:12.5%}.sd-row-cols-lg-9>*{flex:0 0 auto;-ms-flex:0 0 auto;width:11.1111111111%}.sd-row-cols-lg-10>*{flex:0 0 auto;-ms-flex:0 0 auto;width:10%}.sd-row-cols-lg-11>*{flex:0 0 auto;-ms-flex:0 0 auto;width:9.0909090909%}.sd-row-cols-lg-12>*{flex:0 0 auto;-ms-flex:0 0 auto;width:8.3333333333%}}@media(min-width: 1200px){.sd-col-xl{flex:1 0 0%;-ms-flex:1 0 0%}.sd-row-cols-xl-auto{flex:1 0 auto;-ms-flex:1 0 auto;width:100%}.sd-row-cols-xl-1>*{flex:0 0 auto;-ms-flex:0 0 auto;width:100%}.sd-row-cols-xl-2>*{flex:0 0 auto;-ms-flex:0 0 auto;width:50%}.sd-row-cols-xl-3>*{flex:0 0 auto;-ms-flex:0 0 auto;width:33.3333333333%}.sd-row-cols-xl-4>*{flex:0 0 auto;-ms-flex:0 0 auto;width:25%}.sd-row-cols-xl-5>*{flex:0 0 auto;-ms-flex:0 0 auto;width:20%}.sd-row-cols-xl-6>*{flex:0 0 auto;-ms-flex:0 0 auto;width:16.6666666667%}.sd-row-cols-xl-7>*{flex:0 0 auto;-ms-flex:0 0 auto;width:14.2857142857%}.sd-row-cols-xl-8>*{flex:0 0 auto;-ms-flex:0 0 auto;width:12.5%}.sd-row-cols-xl-9>*{flex:0 0 auto;-ms-flex:0 0 auto;width:11.1111111111%}.sd-row-cols-xl-10>*{flex:0 0 auto;-ms-flex:0 0 auto;width:10%}.sd-row-cols-xl-11>*{flex:0 0 auto;-ms-flex:0 0 auto;width:9.0909090909%}.sd-row-cols-xl-12>*{flex:0 0 auto;-ms-flex:0 0 auto;width:8.3333333333%}}.sd-col-auto{flex:0 0 auto;-ms-flex:0 0 auto;width:auto}.sd-col-1{flex:0 0 auto;-ms-flex:0 0 auto;width:8.3333333333%}.sd-col-2{flex:0 0 auto;-ms-flex:0 0 auto;width:16.6666666667%}.sd-col-3{flex:0 0 auto;-ms-flex:0 0 auto;width:25%}.sd-col-4{flex:0 0 auto;-ms-flex:0 0 auto;width:33.3333333333%}.sd-col-5{flex:0 0 auto;-ms-flex:0 0 auto;width:41.6666666667%}.sd-col-6{flex:0 0 auto;-ms-flex:0 0 auto;width:50%}.sd-col-7{flex:0 0 auto;-ms-flex:0 0 auto;width:58.3333333333%}.sd-col-8{flex:0 0 auto;-ms-flex:0 0 auto;width:66.6666666667%}.sd-col-9{flex:0 0 auto;-ms-flex:0 0 auto;width:75%}.sd-col-10{flex:0 0 auto;-ms-flex:0 0 auto;width:83.3333333333%}.sd-col-11{flex:0 0 auto;-ms-flex:0 0 auto;width:91.6666666667%}.sd-col-12{flex:0 0 auto;-ms-flex:0 0 auto;width:100%}.sd-g-0,.sd-gy-0{--sd-gutter-y: 0}.sd-g-0,.sd-gx-0{--sd-gutter-x: 0}.sd-g-1,.sd-gy-1{--sd-gutter-y: 0.25rem}.sd-g-1,.sd-gx-1{--sd-gutter-x: 0.25rem}.sd-g-2,.sd-gy-2{--sd-gutter-y: 0.5rem}.sd-g-2,.sd-gx-2{--sd-gutter-x: 0.5rem}.sd-g-3,.sd-gy-3{--sd-gutter-y: 1rem}.sd-g-3,.sd-gx-3{--sd-gutter-x: 1rem}.sd-g-4,.sd-gy-4{--sd-gutter-y: 1.5rem}.sd-g-4,.sd-gx-4{--sd-gutter-x: 1.5rem}.sd-g-5,.sd-gy-5{--sd-gutter-y: 3rem}.sd-g-5,.sd-gx-5{--sd-gutter-x: 3rem}@media(min-width: 576px){.sd-col-sm-auto{-ms-flex:0 0 auto;flex:0 0 auto;width:auto}.sd-col-sm-1{-ms-flex:0 0 auto;flex:0 0 auto;width:8.3333333333%}.sd-col-sm-2{-ms-flex:0 0 auto;flex:0 0 auto;width:16.6666666667%}.sd-col-sm-3{-ms-flex:0 0 auto;flex:0 0 auto;width:25%}.sd-col-sm-4{-ms-flex:0 0 auto;flex:0 0 auto;width:33.3333333333%}.sd-col-sm-5{-ms-flex:0 0 auto;flex:0 0 auto;width:41.6666666667%}.sd-col-sm-6{-ms-flex:0 0 auto;flex:0 0 auto;width:50%}.sd-col-sm-7{-ms-flex:0 0 auto;flex:0 0 auto;width:58.3333333333%}.sd-col-sm-8{-ms-flex:0 0 auto;flex:0 0 auto;width:66.6666666667%}.sd-col-sm-9{-ms-flex:0 0 auto;flex:0 0 auto;width:75%}.sd-col-sm-10{-ms-flex:0 0 auto;flex:0 0 auto;width:83.3333333333%}.sd-col-sm-11{-ms-flex:0 0 auto;flex:0 0 auto;width:91.6666666667%}.sd-col-sm-12{-ms-flex:0 0 auto;flex:0 0 auto;width:100%}.sd-g-sm-0,.sd-gy-sm-0{--sd-gutter-y: 0}.sd-g-sm-0,.sd-gx-sm-0{--sd-gutter-x: 0}.sd-g-sm-1,.sd-gy-sm-1{--sd-gutter-y: 0.25rem}.sd-g-sm-1,.sd-gx-sm-1{--sd-gutter-x: 0.25rem}.sd-g-sm-2,.sd-gy-sm-2{--sd-gutter-y: 0.5rem}.sd-g-sm-2,.sd-gx-sm-2{--sd-gutter-x: 0.5rem}.sd-g-sm-3,.sd-gy-sm-3{--sd-gutter-y: 1rem}.sd-g-sm-3,.sd-gx-sm-3{--sd-gutter-x: 1rem}.sd-g-sm-4,.sd-gy-sm-4{--sd-gutter-y: 1.5rem}.sd-g-sm-4,.sd-gx-sm-4{--sd-gutter-x: 1.5rem}.sd-g-sm-5,.sd-gy-sm-5{--sd-gutter-y: 3rem}.sd-g-sm-5,.sd-gx-sm-5{--sd-gutter-x: 3rem}}@media(min-width: 768px){.sd-col-md-auto{-ms-flex:0 0 auto;flex:0 0 auto;width:auto}.sd-col-md-1{-ms-flex:0 0 auto;flex:0 0 auto;width:8.3333333333%}.sd-col-md-2{-ms-flex:0 0 auto;flex:0 0 auto;width:16.6666666667%}.sd-col-md-3{-ms-flex:0 0 auto;flex:0 0 auto;width:25%}.sd-col-md-4{-ms-flex:0 0 auto;flex:0 0 auto;width:33.3333333333%}.sd-col-md-5{-ms-flex:0 0 auto;flex:0 0 auto;width:41.6666666667%}.sd-col-md-6{-ms-flex:0 0 auto;flex:0 0 auto;width:50%}.sd-col-md-7{-ms-flex:0 0 auto;flex:0 0 auto;width:58.3333333333%}.sd-col-md-8{-ms-flex:0 0 auto;flex:0 0 auto;width:66.6666666667%}.sd-col-md-9{-ms-flex:0 0 auto;flex:0 0 auto;width:75%}.sd-col-md-10{-ms-flex:0 0 auto;flex:0 0 auto;width:83.3333333333%}.sd-col-md-11{-ms-flex:0 0 auto;flex:0 0 auto;width:91.6666666667%}.sd-col-md-12{-ms-flex:0 0 auto;flex:0 0 auto;width:100%}.sd-g-md-0,.sd-gy-md-0{--sd-gutter-y: 0}.sd-g-md-0,.sd-gx-md-0{--sd-gutter-x: 0}.sd-g-md-1,.sd-gy-md-1{--sd-gutter-y: 0.25rem}.sd-g-md-1,.sd-gx-md-1{--sd-gutter-x: 0.25rem}.sd-g-md-2,.sd-gy-md-2{--sd-gutter-y: 0.5rem}.sd-g-md-2,.sd-gx-md-2{--sd-gutter-x: 0.5rem}.sd-g-md-3,.sd-gy-md-3{--sd-gutter-y: 1rem}.sd-g-md-3,.sd-gx-md-3{--sd-gutter-x: 1rem}.sd-g-md-4,.sd-gy-md-4{--sd-gutter-y: 1.5rem}.sd-g-md-4,.sd-gx-md-4{--sd-gutter-x: 1.5rem}.sd-g-md-5,.sd-gy-md-5{--sd-gutter-y: 3rem}.sd-g-md-5,.sd-gx-md-5{--sd-gutter-x: 3rem}}@media(min-width: 992px){.sd-col-lg-auto{-ms-flex:0 0 auto;flex:0 0 auto;width:auto}.sd-col-lg-1{-ms-flex:0 0 auto;flex:0 0 auto;width:8.3333333333%}.sd-col-lg-2{-ms-flex:0 0 auto;flex:0 0 auto;width:16.6666666667%}.sd-col-lg-3{-ms-flex:0 0 auto;flex:0 0 auto;width:25%}.sd-col-lg-4{-ms-flex:0 0 auto;flex:0 0 auto;width:33.3333333333%}.sd-col-lg-5{-ms-flex:0 0 auto;flex:0 0 auto;width:41.6666666667%}.sd-col-lg-6{-ms-flex:0 0 auto;flex:0 0 auto;width:50%}.sd-col-lg-7{-ms-flex:0 0 auto;flex:0 0 auto;width:58.3333333333%}.sd-col-lg-8{-ms-flex:0 0 auto;flex:0 0 auto;width:66.6666666667%}.sd-col-lg-9{-ms-flex:0 0 auto;flex:0 0 auto;width:75%}.sd-col-lg-10{-ms-flex:0 0 auto;flex:0 0 auto;width:83.3333333333%}.sd-col-lg-11{-ms-flex:0 0 auto;flex:0 0 auto;width:91.6666666667%}.sd-col-lg-12{-ms-flex:0 0 auto;flex:0 0 auto;width:100%}.sd-g-lg-0,.sd-gy-lg-0{--sd-gutter-y: 0}.sd-g-lg-0,.sd-gx-lg-0{--sd-gutter-x: 0}.sd-g-lg-1,.sd-gy-lg-1{--sd-gutter-y: 0.25rem}.sd-g-lg-1,.sd-gx-lg-1{--sd-gutter-x: 0.25rem}.sd-g-lg-2,.sd-gy-lg-2{--sd-gutter-y: 0.5rem}.sd-g-lg-2,.sd-gx-lg-2{--sd-gutter-x: 0.5rem}.sd-g-lg-3,.sd-gy-lg-3{--sd-gutter-y: 1rem}.sd-g-lg-3,.sd-gx-lg-3{--sd-gutter-x: 1rem}.sd-g-lg-4,.sd-gy-lg-4{--sd-gutter-y: 1.5rem}.sd-g-lg-4,.sd-gx-lg-4{--sd-gutter-x: 1.5rem}.sd-g-lg-5,.sd-gy-lg-5{--sd-gutter-y: 3rem}.sd-g-lg-5,.sd-gx-lg-5{--sd-gutter-x: 3rem}}@media(min-width: 1200px){.sd-col-xl-auto{-ms-flex:0 0 auto;flex:0 0 auto;width:auto}.sd-col-xl-1{-ms-flex:0 0 auto;flex:0 0 auto;width:8.3333333333%}.sd-col-xl-2{-ms-flex:0 0 auto;flex:0 0 auto;width:16.6666666667%}.sd-col-xl-3{-ms-flex:0 0 auto;flex:0 0 auto;width:25%}.sd-col-xl-4{-ms-flex:0 0 auto;flex:0 0 auto;width:33.3333333333%}.sd-col-xl-5{-ms-flex:0 0 auto;flex:0 0 auto;width:41.6666666667%}.sd-col-xl-6{-ms-flex:0 0 auto;flex:0 0 auto;width:50%}.sd-col-xl-7{-ms-flex:0 0 auto;flex:0 0 auto;width:58.3333333333%}.sd-col-xl-8{-ms-flex:0 0 auto;flex:0 0 auto;width:66.6666666667%}.sd-col-xl-9{-ms-flex:0 0 auto;flex:0 0 auto;width:75%}.sd-col-xl-10{-ms-flex:0 0 auto;flex:0 0 auto;width:83.3333333333%}.sd-col-xl-11{-ms-flex:0 0 auto;flex:0 0 auto;width:91.6666666667%}.sd-col-xl-12{-ms-flex:0 0 auto;flex:0 0 auto;width:100%}.sd-g-xl-0,.sd-gy-xl-0{--sd-gutter-y: 0}.sd-g-xl-0,.sd-gx-xl-0{--sd-gutter-x: 0}.sd-g-xl-1,.sd-gy-xl-1{--sd-gutter-y: 0.25rem}.sd-g-xl-1,.sd-gx-xl-1{--sd-gutter-x: 0.25rem}.sd-g-xl-2,.sd-gy-xl-2{--sd-gutter-y: 0.5rem}.sd-g-xl-2,.sd-gx-xl-2{--sd-gutter-x: 0.5rem}.sd-g-xl-3,.sd-gy-xl-3{--sd-gutter-y: 1rem}.sd-g-xl-3,.sd-gx-xl-3{--sd-gutter-x: 1rem}.sd-g-xl-4,.sd-gy-xl-4{--sd-gutter-y: 1.5rem}.sd-g-xl-4,.sd-gx-xl-4{--sd-gutter-x: 1.5rem}.sd-g-xl-5,.sd-gy-xl-5{--sd-gutter-y: 3rem}.sd-g-xl-5,.sd-gx-xl-5{--sd-gutter-x: 3rem}}.sd-flex-row-reverse{flex-direction:row-reverse !important}details.sd-dropdown{position:relative;font-size:var(--sd-fontsize-dropdown)}details.sd-dropdown:hover{cursor:pointer}details.sd-dropdown .sd-summary-content{cursor:default}details.sd-dropdown summary.sd-summary-title{padding:.5em 1em;font-size:var(--sd-fontsize-dropdown-title);font-weight:var(--sd-fontweight-dropdown-title);user-select:none;-moz-user-select:none;-ms-user-select:none;-webkit-user-select:none;list-style:none;display:inline-flex;justify-content:space-between}details.sd-dropdown summary.sd-summary-title::-webkit-details-marker{display:none}details.sd-dropdown summary.sd-summary-title:focus{outline:none}details.sd-dropdown summary.sd-summary-title .sd-summary-icon{margin-right:.6em;display:inline-flex;align-items:center}details.sd-dropdown summary.sd-summary-title .sd-summary-icon svg{opacity:.8}details.sd-dropdown summary.sd-summary-title .sd-summary-text{flex-grow:1;line-height:1.5;padding-right:.5rem}details.sd-dropdown summary.sd-summary-title .sd-summary-state-marker{pointer-events:none;display:inline-flex;align-items:center}details.sd-dropdown summary.sd-summary-title .sd-summary-state-marker svg{opacity:.6}details.sd-dropdown summary.sd-summary-title:hover .sd-summary-state-marker svg{opacity:1;transform:scale(1.1)}details.sd-dropdown[open] summary .sd-octicon.no-title{visibility:hidden}details.sd-dropdown .sd-summary-chevron-right{transition:.25s}details.sd-dropdown[open]>.sd-summary-title .sd-summary-chevron-right{transform:rotate(90deg)}details.sd-dropdown[open]>.sd-summary-title .sd-summary-chevron-down{transform:rotate(180deg)}details.sd-dropdown:not([open]).sd-card{border:none}details.sd-dropdown:not([open])>.sd-card-header{border:1px solid var(--sd-color-card-border);border-radius:.25rem}details.sd-dropdown.sd-fade-in[open] summary~*{-moz-animation:sd-fade-in .5s ease-in-out;-webkit-animation:sd-fade-in .5s ease-in-out;animation:sd-fade-in .5s ease-in-out}details.sd-dropdown.sd-fade-in-slide-down[open] summary~*{-moz-animation:sd-fade-in .5s ease-in-out,sd-slide-down .5s ease-in-out;-webkit-animation:sd-fade-in .5s ease-in-out,sd-slide-down .5s ease-in-out;animation:sd-fade-in .5s ease-in-out,sd-slide-down .5s ease-in-out}.sd-col>.sd-dropdown{width:100%}.sd-summary-content>.sd-tab-set:first-child{margin-top:0}@keyframes sd-fade-in{0%{opacity:0}100%{opacity:1}}@keyframes sd-slide-down{0%{transform:translate(0, -10px)}100%{transform:translate(0, 0)}}.sd-tab-set{border-radius:.125rem;display:flex;flex-wrap:wrap;margin:1em 0;position:relative}.sd-tab-set>input{opacity:0;position:absolute}.sd-tab-set>input:checked+label{border-color:var(--sd-color-tabs-underline-active);color:var(--sd-color-tabs-label-active)}.sd-tab-set>input:checked+label+.sd-tab-content{display:block}.sd-tab-set>input:not(:checked)+label:hover{color:var(--sd-color-tabs-label-hover);border-color:var(--sd-color-tabs-underline-hover)}.sd-tab-set>input:focus+label{outline-style:auto}.sd-tab-set>input:not(.focus-visible)+label{outline:none;-webkit-tap-highlight-color:transparent}.sd-tab-set>label{border-bottom:.125rem solid transparent;margin-bottom:0;color:var(--sd-color-tabs-label-inactive);border-color:var(--sd-color-tabs-underline-inactive);cursor:pointer;font-size:var(--sd-fontsize-tabs-label);font-weight:700;padding:1em 1.25em .5em;transition:color 250ms;width:auto;z-index:1}html .sd-tab-set>label:hover{color:var(--sd-color-tabs-label-active)}.sd-col>.sd-tab-set{width:100%}.sd-tab-content{box-shadow:0 -0.0625rem var(--sd-color-tabs-overline),0 .0625rem var(--sd-color-tabs-underline);display:none;order:99;padding-bottom:.75rem;padding-top:.75rem;width:100%}.sd-tab-content>:first-child{margin-top:0 !important}.sd-tab-content>:last-child{margin-bottom:0 !important}.sd-tab-content>.sd-tab-set{margin:0}.sd-sphinx-override,.sd-sphinx-override *{-moz-box-sizing:border-box;-webkit-box-sizing:border-box;box-sizing:border-box}.sd-sphinx-override p{margin-top:0}:root{--sd-color-primary: #0071bc;--sd-color-secondary: #6c757d;--sd-color-success: #28a745;--sd-color-info: #17a2b8;--sd-color-warning: #f0b37e;--sd-color-danger: #dc3545;--sd-color-light: #f8f9fa;--sd-color-muted: #6c757d;--sd-color-dark: #212529;--sd-color-black: black;--sd-color-white: white;--sd-color-primary-highlight: #0060a0;--sd-color-secondary-highlight: #5c636a;--sd-color-success-highlight: #228e3b;--sd-color-info-highlight: #148a9c;--sd-color-warning-highlight: #cc986b;--sd-color-danger-highlight: #bb2d3b;--sd-color-light-highlight: #d3d4d5;--sd-color-muted-highlight: #5c636a;--sd-color-dark-highlight: #1c1f23;--sd-color-black-highlight: black;--sd-color-white-highlight: #d9d9d9;--sd-color-primary-bg: rgba(0, 113, 188, 0.2);--sd-color-secondary-bg: rgba(108, 117, 125, 0.2);--sd-color-success-bg: rgba(40, 167, 69, 0.2);--sd-color-info-bg: rgba(23, 162, 184, 0.2);--sd-color-warning-bg: rgba(240, 179, 126, 0.2);--sd-color-danger-bg: rgba(220, 53, 69, 0.2);--sd-color-light-bg: rgba(248, 249, 250, 0.2);--sd-color-muted-bg: rgba(108, 117, 125, 0.2);--sd-color-dark-bg: rgba(33, 37, 41, 0.2);--sd-color-black-bg: rgba(0, 0, 0, 0.2);--sd-color-white-bg: rgba(255, 255, 255, 0.2);--sd-color-primary-text: #fff;--sd-color-secondary-text: #fff;--sd-color-success-text: #fff;--sd-color-info-text: #fff;--sd-color-warning-text: #212529;--sd-color-danger-text: #fff;--sd-color-light-text: #212529;--sd-color-muted-text: #fff;--sd-color-dark-text: #fff;--sd-color-black-text: #fff;--sd-color-white-text: #212529;--sd-color-shadow: rgba(0, 0, 0, 0.15);--sd-color-card-border: rgba(0, 0, 0, 0.125);--sd-color-card-border-hover: hsla(231, 99%, 66%, 1);--sd-color-card-background: transparent;--sd-color-card-text: inherit;--sd-color-card-header: transparent;--sd-color-card-footer: transparent;--sd-color-tabs-label-active: hsla(231, 99%, 66%, 1);--sd-color-tabs-label-hover: hsla(231, 99%, 66%, 1);--sd-color-tabs-label-inactive: hsl(0, 0%, 66%);--sd-color-tabs-underline-active: hsla(231, 99%, 66%, 1);--sd-color-tabs-underline-hover: rgba(178, 206, 245, 0.62);--sd-color-tabs-underline-inactive: transparent;--sd-color-tabs-overline: rgb(222, 222, 222);--sd-color-tabs-underline: rgb(222, 222, 222);--sd-fontsize-tabs-label: 1rem;--sd-fontsize-dropdown: inherit;--sd-fontsize-dropdown-title: 1rem;--sd-fontweight-dropdown-title: 700}
```

### Comparing `sphinx_design-0.5.0/sphinx_design/dropdown.py` & `sphinx_design-0.6.0/sphinx_design/dropdown.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-"""Originally Adapted from sphinxcontrib.details.directive
-"""
+"""Originally Adapted from sphinxcontrib.details.directive"""
+
 from docutils import nodes
 from docutils.parsers.rst import directives
 from sphinx.application import Sphinx
 from sphinx.transforms.post_transforms import SphinxPostTransform
-from sphinx.util.docutils import SphinxDirective
 
 from sphinx_design.shared import (
     SEMANTIC_COLORS,
+    SdDirective,
     create_component,
     is_component,
     make_choice,
     margin_option,
 )
 
 from ._compat import findall
@@ -21,19 +21,19 @@
 def setup_dropdown(app: Sphinx) -> None:
     app.add_node(dropdown_main, html=(visit_dropdown_main, depart_dropdown_main))
     app.add_node(dropdown_title, html=(visit_dropdown_title, depart_dropdown_title))
     app.add_directive("dropdown", DropdownDirective)
     app.add_post_transform(DropdownHtmlTransform)
 
 
-class dropdown_main(nodes.Element, nodes.General):
+class dropdown_main(nodes.Element, nodes.General):  # noqa: N801
     pass
 
 
-class dropdown_title(nodes.TextElement, nodes.General):
+class dropdown_title(nodes.TextElement, nodes.General):  # noqa: N801
     pass
 
 
 def visit_dropdown_main(self, node):
     if node.get("opened"):
         self.body.append(self.starttag(node, "details", open="open"))
     else:
@@ -48,15 +48,15 @@
     self.body.append(self.starttag(node, "summary"))
 
 
 def depart_dropdown_title(self, node):
     self.body.append("</summary>")
 
 
-class DropdownDirective(SphinxDirective):
+class DropdownDirective(SdDirective):
     """A directive to generate a collapsible container.
 
     Note: This directive generates a single container,
     for the title (optional) and content::
 
         <container design_component="dropdown" has_title=True>
             <rubric>
@@ -72,24 +72,26 @@
     optional_arguments = 1  # title of dropdown
     final_argument_whitespace = True
     has_content = True
     option_spec = {
         "open": directives.flag,  # make open by default
         "color": make_choice(SEMANTIC_COLORS),
         "icon": make_choice(list_octicons()),
+        "chevron": make_choice(
+            ["right-down", "down-up"]
+        ),  # chevron direction closed-open
         "animate": make_choice(("fade-in", "fade-in-slide-down")),
         "margin": margin_option,
         "name": directives.unchanged,
         "class-container": directives.class_option,
         "class-title": directives.class_option,
         "class-body": directives.class_option,
     }
 
-    def run(self):
-        """Run the directive"""
+    def run_with_defaults(self) -> list[nodes.Node]:
         # default classes
         classes = {
             "container_classes": self.options.get("margin", ["sd-mb-3"])
             + self.options.get("class-container", []),
             "title_classes": self.options.get("class-title", []),
             "body_classes": self.options.get("class-body", []),
         }
@@ -110,14 +112,15 @@
 
         container = create_component(
             "dropdown",
             opened="open" in self.options,
             type="dropdown",
             has_title=len(self.arguments) > 0,
             icon=self.options.get("icon"),
+            chevron=self.options.get("chevron"),
             **classes,
         )
         self.set_source_info(container)
         if self.arguments:
             textnodes, messages = self.state.inline_text(self.arguments[0], self.lineno)
             title_node = nodes.rubric(self.arguments[0], "", *textnodes)
             container += title_node
@@ -141,82 +144,82 @@
             ...content nodes
 
     """
 
     default_priority = 199
     formats = ("html",)
 
-    def run(self):
+    def run(self) -> None:
         """Run the transform"""
         document: nodes.document = self.document
         for node in findall(document)(lambda node: is_component(node, "dropdown")):
             # TODO option to not have card css (but requires more formatting)
             use_card = True
 
-            open_marker = create_component(
-                "dropdown-open-marker",
-                classes=["sd-summary-up"],
-                children=[
-                    nodes.raw(
-                        "",
-                        nodes.Text(get_octicon("chevron-up", height="1.5em")),
-                        format="html",
-                    )
-                ],
+            marker_type = (
+                "chevron-down" if node["chevron"] == "down-up" else "chevron-right"
             )
-            closed_marker = create_component(
-                "dropdown-closed-marker",
-                classes=["sd-summary-down"],
-                children=[
-                    nodes.raw(
-                        "",
-                        nodes.Text(get_octicon("chevron-down", height="1.5em")),
-                        format="html",
-                    )
-                ],
+            state_marker = nodes.inline(
+                "",
+                "",
+                nodes.raw(
+                    "",
+                    nodes.Text(get_octicon(marker_type, height="1.5em")),
+                    format="html",
+                ),
+                classes=["sd-summary-state-marker", f"sd-summary-{marker_type}"],
             )
 
             newnode = dropdown_main(
                 opened=node["opened"],
                 classes=["sd-sphinx-override", "sd-dropdown"]
                 + (["sd-card"] if use_card else ["sd-d-flex-column"])
                 + node["container_classes"],
             )
 
             if node["has_title"]:
-                title_children = node[0].children
+                title_text_children = node[0].children
                 if node[0].get("ids"):
                     newnode["ids"] += node[0]["ids"]
                 body_children = node[1:]
             else:
-                title_children = [
+                title_text_children = [
                     nodes.raw(
                         "...",
-                        nodes.Text(get_octicon("kebab-horizontal", height="1.5em")),
+                        nodes.Text(
+                            get_octicon(
+                                "kebab-horizontal", height="1.5em", classes=["no-title"]
+                            )
+                        ),
                         format="html",
                     )
                 ]
                 body_children = node.children
+            title_text_node = nodes.inline(
+                "",
+                "",
+                *title_text_children,
+                classes=["sd-summary-text"],
+            )
+            title_children = [title_text_node, state_marker]
             if node["icon"]:
                 title_children.insert(
                     0,
                     nodes.raw(
                         "",
-                        nodes.Text(get_octicon(node["icon"], height="1em")),
+                        get_octicon(node["icon"], height="1em"),
                         classes=["sd-summary-icon"],
                         format="html",
                     ),
                 )
 
             newnode += dropdown_title(
                 "",
                 "",
                 *title_children,
-                closed_marker,
-                open_marker,
                 classes=["sd-summary-title"]
                 + (["sd-card-header"] if use_card else [])
                 + node["title_classes"],
             )
             body_node = create_component(
                 "dropdown-body",
                 classes=["sd-summary-content"]
```

### Comparing `sphinx_design-0.5.0/sphinx_design/extension.py` & `sphinx_design-0.6.0/sphinx_design/extension.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,33 @@
+from contextlib import contextmanager
+from functools import partial
 import hashlib
 from pathlib import Path
 
 from docutils import nodes
 from docutils.parsers.rst import directives
+from sphinx import version_info as sphinx_version
 from sphinx.application import Sphinx
 from sphinx.environment import BuildEnvironment
 from sphinx.transforms import SphinxTransform
-from sphinx.util.docutils import SphinxDirective
 
 from . import compiled as static_module
 from ._compat import findall, read_text
 from .article_info import setup_article_info
 from .badges_buttons import setup_badges_and_buttons
 from .cards import setup_cards
 from .dropdown import setup_dropdown
 from .grids import setup_grids
 from .icons import setup_icons
-from .shared import PassthroughTextElement, create_component
+from .shared import (
+    PassthroughTextElement,
+    SdDirective,
+    create_component,
+    setup_custom_directives,
+)
 from .tabs import setup_tabs
 
 
 def setup_extension(app: Sphinx) -> None:
     """Set up the sphinx extension."""
     app.connect("builder-inited", update_css_js)
     app.connect("env-updated", update_css_links)
@@ -33,25 +40,44 @@
         PassthroughTextElement,
         html=(visit_depart_null, visit_depart_null),
         latex=(visit_depart_null, visit_depart_null),
         text=(visit_depart_null, visit_depart_null),
         man=(visit_depart_null, visit_depart_null),
         texinfo=(visit_depart_null, visit_depart_null),
     )
-    app.add_directive(
-        "div", Div, override=True
-    )  # override sphinx-panels implementation
-    app.add_transform(AddFirstTitleCss)
-    setup_badges_and_buttons(app)
-    setup_cards(app)
-    setup_grids(app)
-    setup_dropdown(app)
-    setup_icons(app)
-    setup_tabs(app)
-    setup_article_info(app)
+    with capture_directives(app) as directive_map:
+        app.add_directive("div", Div, override=True)
+        app.add_transform(AddFirstTitleCss)
+        setup_badges_and_buttons(app)
+        setup_cards(app)
+        setup_grids(app)
+        setup_dropdown(app)
+        setup_icons(app)
+        setup_tabs(app)
+        setup_article_info(app)
+
+    app.add_config_value("sd_custom_directives", {}, "env")
+    app.connect(
+        "config-inited", partial(setup_custom_directives, directive_map=directive_map)
+    )
+
+
+@contextmanager
+def capture_directives(app: Sphinx):
+    """Capture the directives that are registered by the extension."""
+    directive_map = {}
+    add_directive = app.add_directive
+
+    def _add_directive(name, directive, **kwargs):
+        directive_map[name] = directive
+        add_directive(name, directive, **kwargs)
+
+    app.add_directive = _add_directive
+    yield directive_map
+    app.add_directive = add_directive
 
 
 def update_css_js(app: Sphinx):
     """Copy the CSS to the build directory."""
     # reset changed identifier
     app.env.sphinx_design_css_changed = False
     # setup up new static path in output dir
@@ -63,17 +89,22 @@
     js_path = static_path / "design-tabs.js"
     app.add_js_file(js_path.name)
     if not js_path.exists():
         content = read_text(static_module, "sd_tabs.js")
         js_path.write_text(content)
     # Read the css content and hash it
     content = read_text(static_module, "style.min.css")
-    hash = hashlib.md5(content.encode("utf8")).hexdigest()
     # Write the css file
-    css_path = static_path / f"design-style.{hash}.min.css"
+    if sphinx_version < (7, 1):
+        hash = hashlib.md5(content.encode("utf8"), usedforsecurity=False).hexdigest()
+        css_path = static_path / f"sphinx-design.{hash}.min.css"
+    else:
+        # since sphinx 7.1 a checksum is added to the css file URL, so there is no need to do it here
+        # https://github.com/sphinx-doc/sphinx/pull/11415
+        css_path = static_path / "sphinx-design.min.css"
     app.add_css_file(css_path.name)
     if css_path.exists():
         return
     if static_existed:
         app.env.sphinx_design_css_changed = True
     for path in static_path.glob("*.css"):
         path.unlink()
@@ -101,36 +132,35 @@
     self.body.append("</div>\n")
 
 
 def visit_depart_null(self, node: nodes.Element) -> None:
     """visit/depart passthrough"""
 
 
-class Div(SphinxDirective):
+class Div(SdDirective):
     """Same as the ``container`` directive,
     but does not add the ``container`` class in HTML outputs,
     which can interfere with Bootstrap CSS.
     """
 
     optional_arguments = 1  # css classes
     final_argument_whitespace = True
     option_spec = {"style": directives.unchanged, "name": directives.unchanged}
     has_content = True
 
-    def run(self):
+    def run_with_defaults(self) -> list[nodes.Node]:
         try:
             if self.arguments:
                 classes = directives.class_option(self.arguments[0])
             else:
                 classes = []
-        except ValueError:
+        except ValueError as exc:
             raise self.error(
-                'Invalid class attribute value for "%s" directive: "%s".'
-                % (self.name, self.arguments[0])
-            )
+                f'Invalid class attribute value for "{self.name}" directive: "{self.arguments[0]}".'
+            ) from exc
         node = create_component("div", rawtext="\n".join(self.content), classes=classes)
         if "style" in self.options:
             node["style"] = self.options["style"]
         self.set_source_info(node)
         self.add_name(node)
         if self.content:
             self.state.nested_parse(self.content, self.content_offset, node)
```

### Comparing `sphinx_design-0.5.0/sphinx_design/grids.py` & `sphinx_design-0.6.0/sphinx_design/grids.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import List, Optional
+from typing import Optional
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from sphinx.application import Sphinx
-from sphinx.util.docutils import SphinxDirective
 from sphinx.util.logging import getLogger
 
 from .cards import CardDirective
 from .shared import (
     WARNING_TYPE,
+    SdDirective,
     create_component,
     is_component,
     make_choice,
     margin_option,
     padding_option,
     text_align,
 )
@@ -35,15 +35,15 @@
 def _media_option(
     argument: Optional[str],
     prefix: str,
     *,
     allow_auto: bool = False,
     min_num: int = 1,
     max_num: int = 12,
-) -> List[str]:
+) -> list[str]:
     """Validate the number of columns (out of 12).
 
     One or four integers (for "xs sm md lg") between 1 and 12.
     """
     validate_error_msg = (
         "argument must be 1 or 4 (xs sm md lg) values, and each value should be "
         f"{'either auto or ' if allow_auto else ''}an integer from {min_num} to {max_num}"
@@ -56,49 +56,49 @@
     if len(values) != 4:
         raise ValueError(validate_error_msg)
     for value in values:
         if allow_auto and value == "auto":
             continue
         try:
             int_value = int(value)
-        except Exception:
-            raise ValueError(validate_error_msg)
+        except Exception as exc:
+            raise ValueError(validate_error_msg) from exc
         if not (min_num <= int_value <= max_num):
             raise ValueError(validate_error_msg)
     return [f"{prefix}{values[0]}"] + [
         f"{prefix}{size}-{value}"
         for size, value in zip(["xs", "sm", "md", "lg"], values)
     ]
 
 
-def row_columns_option(argument: Optional[str]) -> List[str]:
+def row_columns_option(argument: Optional[str]) -> list[str]:
     """Validate the number of columns (out of 12) a grid row will have.
 
     One or four integers (for "xs sm md lg") between 1 and 12  (or 'auto').
     """
     return _media_option(argument, "sd-row-cols-", allow_auto=True)
 
 
-def item_columns_option(argument: Optional[str]) -> List[str]:
+def item_columns_option(argument: Optional[str]) -> list[str]:
     """Validate the number of columns (out of 12) a grid-item will take up.
 
     One or four integers (for "xs sm md lg") between 1 and 12 (or 'auto').
     """
     return _media_option(argument, "sd-col-", allow_auto=True)
 
 
-def gutter_option(argument: Optional[str]) -> List[str]:
+def gutter_option(argument: Optional[str]) -> list[str]:
     """Validate the gutter size between grid items.
 
     One or four integers (for "xs sm md lg") between 0 and 5.
     """
     return _media_option(argument, "sd-g-", min_num=0, max_num=5)
 
 
-class GridDirective(SphinxDirective):
+class GridDirective(SdDirective):
     """A grid component, which is a container for grid items (i.e. columns)."""
 
     has_content = True
     required_arguments = 0
     optional_arguments = 1  # columns
     final_argument_whitespace = True
     option_spec = {
@@ -107,22 +107,21 @@
         "padding": padding_option,
         "outline": directives.flag,
         "reverse": directives.flag,
         "class-container": directives.class_option,
         "class-row": directives.class_option,
     }
 
-    def run(self) -> List[nodes.Node]:
-        """Run the directive."""
+    def run_with_defaults(self) -> list[nodes.Node]:
         try:
             column_classes = (
                 row_columns_option(self.arguments[0]) if self.arguments else []
             )
         except ValueError as exc:
-            raise self.error(f"Invalid directive argument: {exc}")
+            raise self.error(f"Invalid directive argument: {exc}") from exc
         self.assert_has_content()
         # container-fluid is 100% width for all breakpoints,
         # rather than the fixed width of the breakpoint (like container)
         grid_classes = ["sd-container-fluid", "sd-sphinx-override"]
         container = create_component(
             "grid-container",
             grid_classes
@@ -153,15 +152,15 @@
                     type=WARNING_TYPE,
                     subtype="grid",
                 )
                 break
         return [container]
 
 
-class GridItemDirective(SphinxDirective):
+class GridItemDirective(SdDirective):
     """An item within a grid row.
 
     Can "occupy" 1 to 12 columns.
     """
 
     has_content = True
     option_spec = {
@@ -170,16 +169,15 @@
         "padding": padding_option,
         "child-direction": make_choice(["column", "row"]),
         "child-align": make_choice(["start", "end", "center", "justify", "spaced"]),
         "outline": directives.flag,
         "class": directives.class_option,
     }
 
-    def run(self) -> List[nodes.Node]:
-        """Run the directive."""
+    def run_with_defaults(self) -> list[nodes.Node]:
         if not is_component(self.state_machine.node, "grid-row"):
             LOGGER.warning(
                 f"The parent of a 'grid-item' should be a 'grid-row' [{WARNING_TYPE}.grid]",
                 location=(self.env.docname, self.lineno),
                 type=WARNING_TYPE,
                 subtype="grid",
             )
@@ -201,15 +199,15 @@
             + self.options.get("class", []),
         )
         self.set_source_info(column)
         self.state.nested_parse(self.content, self.content_offset, column)
         return [column]
 
 
-class GridItemCardDirective(SphinxDirective):
+class GridItemCardDirective(SdDirective):
     """An item within a grid row, with an internal card."""
 
     has_content = True
     required_arguments = 0
     optional_arguments = 1  # card title
     final_argument_whitespace = True
     option_spec = {
@@ -233,33 +231,32 @@
         "class-title": directives.class_option,
         "class-header": directives.class_option,
         "class-footer": directives.class_option,
         "class-img-top": directives.class_option,
         "class-img-bottom": directives.class_option,
     }
 
-    def run(self) -> List[nodes.Node]:
-        """Run the directive."""
+    def run_with_defaults(self) -> list[nodes.Node]:
         if not is_component(self.state_machine.node, "grid-row"):
             LOGGER.warning(
                 f"The parent of a 'grid-item' should be a 'grid-row' [{WARNING_TYPE}.grid]",
                 location=(self.env.docname, self.lineno),
                 type=WARNING_TYPE,
                 subtype="grid",
             )
         column = create_component(
             "grid-item",
             [
                 "sd-col",
                 "sd-d-flex-row",
-            ]
-            + self.options.get("columns", [])
-            + self.options.get("margin", [])
-            + self.options.get("padding", [])
-            + self.options.get("class-item", []),
+                *self.options.get("columns", []),
+                *self.options.get("margin", []),
+                *self.options.get("padding", []),
+                *self.options.get("class-item", []),
+            ],
         )
         card_options = {
             key: value
             for key, value in self.options.items()
             if key
             in [
                 "width",
```

### Comparing `sphinx_design-0.5.0/sphinx_design/icons.py` & `sphinx_design-0.6.0/sphinx_design/icons.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
+from collections.abc import Sequence
 from functools import lru_cache
 import json
 import re
-from typing import Any, Dict, List, Optional, Sequence, Tuple
+from typing import Any, Optional
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from sphinx.application import Sphinx
 from sphinx.util import logging
-from sphinx.util.docutils import SphinxDirective, SphinxRole
+from sphinx.util.docutils import SphinxRole
 
 from . import compiled
 from ._compat import read_text
-from .shared import WARNING_TYPE
+from .shared import WARNING_TYPE, SdDirective
 
 logger = logging.getLogger(__name__)
 
-OCTICON_VERSION = "v16.1.1"
+OCTICON_VERSION = "v19.8.0"
 
 OCTICON_CSS = """\
 .octicon {
   display: inline-block;
   vertical-align: text-top;
   fill: currentColor;
 }"""
@@ -42,21 +43,21 @@
         man=(visit_fontawesome_warning, None),
         text=(visit_fontawesome_warning, None),
         texinfo=(visit_fontawesome_warning, None),
     )
 
 
 @lru_cache(1)
-def get_octicon_data() -> Dict[str, Any]:
+def get_octicon_data() -> dict[str, Any]:
     """Load all octicon data."""
     content = read_text(compiled, "octicons.json")
     return json.loads(content)
 
 
-def list_octicons() -> List[str]:
+def list_octicons() -> list[str]:
     """List available octicon names."""
     return list(get_octicon_data().keys())
 
 
 HEIGHT_REGEX = re.compile(r"^(?P<value>\d+(\.\d+)?)(?P<unit>px|em|rem)$")
 
 
@@ -68,28 +69,28 @@
 ) -> str:
     """Return the HTML for an GitHub octicon SVG icon.
 
     :height: the height of the octicon, with suffix unit 'px', 'em' or 'rem'.
     """
     try:
         data = get_octicon_data()[name]
-    except KeyError:
-        raise KeyError(f"Unrecognised octicon: {name}")
+    except KeyError as exc:
+        raise KeyError(f"Unrecognised octicon: {name}") from exc
 
     match = HEIGHT_REGEX.match(height)
     if not match:
         raise ValueError(
             f"Invalid height: '{height}', must be format <integer><px|em|rem>"
         )
     height_value = round(float(match.group("value")), 3)
     height_unit = match.group("unit")
 
     original_height = 16
     if "16" not in data["heights"]:
-        original_height = int(list(data["heights"].keys())[0])
+        original_height = int(next(iter(data["heights"].keys())))
     elif "24" in data["heights"]:
         if height_unit == "px":
             if height_value >= 24:
                 original_height = 24
         elif height_value >= 1.5:
             original_height = 24
     original_width = data["heights"][str(original_height)]["width"]
@@ -116,15 +117,15 @@
 
 class OcticonRole(SphinxRole):
     """Role to display a GitHub octicon SVG.
 
     Additional classes can be added to the element after a semicolon.
     """
 
-    def run(self) -> Tuple[List[nodes.Node], List[nodes.system_message]]:
+    def run(self) -> tuple[list[nodes.Node], list[nodes.system_message]]:
         """Run the role."""
         values = self.text.split(";") if ";" in self.text else [self.text]
         icon = values[0]
         height = "1em" if len(values) < 2 else values[1]
         classes = "" if len(values) < 3 else values[2]
         icon = icon.strip()
         try:
@@ -137,65 +138,73 @@
             prb = self.inliner.problematic(self.rawtext, self.rawtext, msg)
             return [prb], [msg]
         node = nodes.raw("", nodes.Text(svg), format="html")
         self.set_source_info(node)
         return [node], []
 
 
-class AllOcticons(SphinxDirective):
+class AllOcticons(SdDirective):
     """Directive to generate all octicon icons.
 
     Primarily for self documentation.
     """
 
     option_spec = {
         "class": directives.class_option,
     }
 
-    def run(self) -> List[nodes.Node]:
-        """Run the directive."""
+    def run_with_defaults(self) -> list[nodes.Node]:
         classes = self.options.get("class", [])
-        list_node = nodes.bullet_list()
+        table = nodes.table()
+        group = nodes.tgroup(cols=2)
+        table += group
+        group.extend(
+            (
+                nodes.colspec(colwidth=1),
+                nodes.colspec(colwidth=1),
+            )
+        )
+        body = nodes.tbody()
+        group += body
         for icon in list_octicons():
-            item_node = nodes.list_item()
-            item_node.extend(
-                (
-                    nodes.literal(icon, icon),
-                    nodes.Text(": "),
-                    nodes.raw(
-                        "",
-                        nodes.Text(get_octicon(icon, classes=classes)),
-                        format="html",
-                    ),
-                )
+            row = nodes.row()
+            body += row
+            cell = nodes.entry()
+            row += cell
+            cell += nodes.literal(icon, icon)
+            cell = nodes.entry()
+            row += cell
+            cell += nodes.raw(
+                "",
+                get_octicon(icon, classes=classes),
+                format="html",
             )
-            list_node += item_node
-        return [list_node]
+        return [table]
 
 
-class fontawesome(nodes.Element, nodes.General):
+class fontawesome(nodes.Element, nodes.General):  # noqa: N801
     """Node for rendering fontawesome icon."""
 
 
 class FontawesomeRole(SphinxRole):
     """Role to display a Fontawesome icon.
 
     Additional classes can be added to the element after a semicolon.
     """
 
     def __init__(self, style: str) -> None:
         super().__init__()
         self.style = style
 
-    def run(self) -> Tuple[List[nodes.Node], List[nodes.system_message]]:
+    def run(self) -> tuple[list[nodes.Node], list[nodes.system_message]]:
         """Run the role."""
         icon, classes = self.text.split(";", 1) if ";" in self.text else [self.text, ""]
         icon = icon.strip()
         node = fontawesome(
-            icon=icon, classes=[self.style, f"fa-{icon}"] + classes.split()
+            icon=icon, classes=[self.style, f"fa-{icon}", *classes.split()]
         )
         self.set_source_info(node)
         return [node], []
 
 
 def visit_fontawesome_html(self, node):
     self.body.append(self.starttag(node, "span", ""))
@@ -234,15 +243,15 @@
         type=WARNING_TYPE,
         subtype="fa-build",
     )
     raise nodes.SkipNode
 
 
 @lru_cache(1)
-def get_material_icon_data(style: str) -> Dict[str, Any]:
+def get_material_icon_data(style: str) -> dict[str, Any]:
     """Load all octicon data."""
     content = read_text(compiled, f"material_{style}.json")
     return json.loads(content)
 
 
 def get_material_icon(
     style: str,
@@ -253,28 +262,28 @@
 ) -> str:
     """Return the HTML for an Google material icon SVG icon.
 
     :height: the height of the material icon, with suffix unit 'px', 'em' or 'rem'.
     """
     try:
         data = get_material_icon_data(style)[name]
-    except KeyError:
-        raise KeyError(f"Unrecognised material-{style} icon: {name}")
+    except KeyError as exc:
+        raise KeyError(f"Unrecognised material-{style} icon: {name}") from exc
 
     match = HEIGHT_REGEX.match(height)
     if not match:
         raise ValueError(
             f"Invalid height: '{height}', must be format <integer><px|em|rem>"
         )
     height_value = round(float(match.group("value")), 3)
     height_unit = match.group("unit")
 
     original_height = 20
     if "20" not in data["heights"]:
-        original_height = int(list(data["heights"].keys())[0])
+        original_height = int(next(iter(data["heights"].keys())))
     elif "24" in data["heights"]:
         if height_unit == "px":
             if height_value >= 24:
                 original_height = 24
         elif height_value >= 1.5:
             original_height = 24
     original_width = data["heights"][str(original_height)]["width"]
@@ -305,15 +314,15 @@
     Additional classes can be added to the element after a semicolon.
     """
 
     def __init__(self, style: str) -> None:
         super().__init__()
         self.style = style
 
-    def run(self) -> Tuple[List[nodes.Node], List[nodes.system_message]]:
+    def run(self) -> tuple[list[nodes.Node], list[nodes.system_message]]:
         """Run the role."""
         values = self.text.split(";") if ";" in self.text else [self.text]
         icon = values[0]
         height = "1em" if len(values) < 2 else values[1]
         classes = "" if len(values) < 3 else values[2]
         icon = icon.strip()
         try:
```

### Comparing `sphinx_design-0.5.0/sphinx_design/tabs.py` & `sphinx_design-0.6.0/sphinx_design/tabs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,60 @@
-from typing import List
-
 from docutils import nodes
 from docutils.parsers.rst import directives
 from sphinx.application import Sphinx
 from sphinx.transforms.post_transforms import SphinxPostTransform
-from sphinx.util.docutils import SphinxDirective
 from sphinx.util.logging import getLogger
 
 from ._compat import findall
-from .shared import WARNING_TYPE, create_component, is_component
+from .shared import WARNING_TYPE, SdDirective, create_component, is_component
 
 LOGGER = getLogger(__name__)
 
 
 def setup_tabs(app: Sphinx) -> None:
     app.add_directive("tab-set", TabSetDirective)
     app.add_directive("tab-item", TabItemDirective)
     app.add_directive("tab-set-code", TabSetCodeDirective)
     app.add_post_transform(TabSetHtmlTransform)
     app.add_node(sd_tab_input, html=(visit_tab_input, depart_tab_input))
     app.add_node(sd_tab_label, html=(visit_tab_label, depart_tab_label))
 
 
-class TabSetDirective(SphinxDirective):
+class TabSetDirective(SdDirective):
     """A container for a set of tab items."""
 
     has_content = True
     option_spec = {
+        "sync-group": directives.unchanged_required,
         "class": directives.class_option,
     }
 
-    def run(self) -> List[nodes.Node]:
-        """Run the directive."""
+    def run_with_defaults(self) -> list[nodes.Node]:
         self.assert_has_content()
         tab_set = create_component(
-            "tab-set", classes=["sd-tab-set"] + self.options.get("class", [])
+            "tab-set", classes=["sd-tab-set", *self.options.get("class", [])]
         )
         self.set_source_info(tab_set)
         self.state.nested_parse(self.content, self.content_offset, tab_set)
         for item in tab_set.children:
             if not is_component(item, "tab-item"):
                 LOGGER.warning(
                     f"All children of a 'tab-set' "
                     f"should be 'tab-item' [{WARNING_TYPE}.tab]",
                     location=item,
                     type=WARNING_TYPE,
                     subtype="tab",
                 )
                 break
+            if "sync_id" in item.children[0]:
+                item.children[0]["sync_group"] = self.options.get("sync-group", "tab")
         return [tab_set]
 
 
-class TabItemDirective(SphinxDirective):
+class TabItemDirective(SdDirective):
     """A single tab item in a tab set.
 
     Note: This directive generates a single container,
     for the label and content::
 
         <container design_component="tab-item" has_title=True>
             <rubric>
@@ -77,68 +76,68 @@
         "sync": directives.unchanged_required,
         "name": directives.unchanged,
         "class-container": directives.class_option,
         "class-label": directives.class_option,
         "class-content": directives.class_option,
     }
 
-    def run(self) -> List[nodes.Node]:
-        """Run the directive."""
+    def run_with_defaults(self) -> list[nodes.Node]:
         self.assert_has_content()
         if not is_component(self.state_machine.node, "tab-set"):
             LOGGER.warning(
                 f"The parent of a 'tab-item' should be a 'tab-set' [{WARNING_TYPE}.tab]",
                 location=(self.env.docname, self.lineno),
                 type=WARNING_TYPE,
                 subtype="tab",
             )
         tab_item = create_component(
             "tab-item",
-            classes=["sd-tab-item"] + self.options.get("class-container", []),
+            classes=["sd-tab-item", *self.options.get("class-container", [])],
             selected=("selected" in self.options),
         )
 
         # add tab label
         textnodes, _ = self.state.inline_text(self.arguments[0], self.lineno)
         tab_label = nodes.rubric(
             self.arguments[0],
+            "",
             *textnodes,
-            classes=["sd-tab-label"] + self.options.get("class-label", []),
+            classes=["sd-tab-label", *self.options.get("class-label", [])],
         )
         if "sync" in self.options:
             tab_label["sync_id"] = self.options["sync"]
         self.add_name(tab_label)
         tab_item += tab_label
 
         # add tab content
         tab_content = create_component(
             "tab-content",
-            classes=["sd-tab-content"] + self.options.get("class-content", []),
+            classes=["sd-tab-content", *self.options.get("class-content", [])],
         )
         self.state.nested_parse(self.content, self.content_offset, tab_content)
         tab_item += tab_content
 
         return [tab_item]
 
 
-class TabSetCodeDirective(SphinxDirective):
+class TabSetCodeDirective(SdDirective):
     """A container for a set of tab items, generated from code blocks."""
 
     has_content = True
     option_spec = {
         "no-sync": directives.flag,
+        "sync-group": directives.unchanged_required,
         "class-set": directives.class_option,
         "class-item": directives.class_option,
     }
 
-    def run(self) -> List[nodes.Node]:
-        """Run the directive."""
+    def run_with_defaults(self) -> list[nodes.Node]:
         self.assert_has_content()
         tab_set = create_component(
-            "tab-set", classes=["sd-tab-set"] + self.options.get("class-set", [])
+            "tab-set", classes=["sd-tab-set", *self.options.get("class-set", [])]
         )
         self.set_source_info(tab_set)
         self.state.nested_parse(self.content, self.content_offset, tab_set)
         new_children = []
         for item in tab_set.children:
             if not isinstance(item, nodes.literal_block):
                 LOGGER.warning(
@@ -149,56 +148,60 @@
                     subtype="tab_code",
                 )
                 continue
             language = item.get("language", "unknown")
             tab_label = nodes.rubric(
                 language.upper(),
                 nodes.Text(language.upper()),
-                classes=["sd-tab-label"] + self.options.get("class-label", []),
+                classes=["sd-tab-label", *self.options.get("class-label", [])],
             )
             if "no-sync" not in self.options:
-                tab_label["sync_id"] = f"tabcode-{language}"
+                tab_label["sync_group"] = self.options.get("sync-group", "code")
+                tab_label["sync_id"] = language
             tab_content = create_component(
                 "tab-content",
                 children=[item],
-                classes=["sd-tab-content"] + self.options.get("class-content", []),
+                classes=["sd-tab-content", *self.options.get("class-content", [])],
             )
             tab_item = create_component(
                 "tab-item",
                 children=[tab_label, tab_content],
-                classes=["sd-tab-item"] + self.options.get("class-item", []),
+                classes=["sd-tab-item", *self.options.get("class-item", [])],
             )
             new_children.append(tab_item)
         tab_set.children = new_children
         return [tab_set]
 
 
-class sd_tab_input(nodes.Element, nodes.General):
+class sd_tab_input(nodes.Element, nodes.General):  # noqa: N801
     pass
 
 
-class sd_tab_label(nodes.TextElement, nodes.General):
+class sd_tab_label(nodes.TextElement, nodes.General):  # noqa: N801
     pass
 
 
 def visit_tab_input(self, node):
     attributes = {"ids": [node["id"]], "type": node["type"], "name": node["set_id"]}
     if node["checked"]:
         attributes["checked"] = "checked"
     self.body.append(self.starttag(node, "input", **attributes))
 
 
 def depart_tab_input(self, node):
-    self.body.append("</input>")
+    # note do not add a closing tag, since this is a void element:
+    # https://developer.mozilla.org/en-US/docs/Glossary/Void_element
+    pass
 
 
 def visit_tab_label(self, node):
     attributes = {"for": node["input_id"]}
-    if "sync_id" in node:
+    if "sync_id" in node and "sync_group" in node:
         attributes["data-sync-id"] = node["sync_id"]
+        attributes["data-sync-group"] = node["sync_group"]
     self.body.append(self.starttag(node, "label", **attributes))
 
 
 def depart_tab_label(self, node):
     self.body.append("</label>")
 
 
@@ -209,23 +212,21 @@
     formats = ("html",)
 
     def run(self) -> None:
         """Run the transform."""
 
         # setup id generators
         tab_set_id_base = "sd-tab-set-"
-        tab_set_id_num = 0
         tab_item_id_base = "sd-tab-item-"
         tab_item_id_num = 0
 
-        for tab_set in findall(self.document)(
-            lambda node: is_component(node, "tab-set")
+        for tab_set_id_num, tab_set in enumerate(
+            findall(self.document)(lambda node: is_component(node, "tab-set"))
         ):
             tab_set_identity = tab_set_id_base + str(tab_set_id_num)
-            tab_set_id_num += 1
             children = []
             # get the first selected node
             selected_idx = None
             for idx, tab_item in enumerate(tab_set.children):
                 if tab_item.get("selected", False):
                     if selected_idx is None:
                         selected_idx = idx
@@ -238,15 +239,14 @@
                         )
             selected_idx = 0 if selected_idx is None else selected_idx
 
             for idx, tab_item in enumerate(tab_set.children):
                 try:
                     tab_label, tab_content = tab_item.children
                 except ValueError:
-                    print(tab_item)
                     raise
                 tab_item_identity = tab_item_id_base + str(tab_item_id_num)
                 tab_item_id_num += 1
 
                 # create: <input checked="checked" id="id" type="radio">
                 input_node = sd_tab_input(
                     "",
@@ -257,21 +257,23 @@
                 )
                 input_node.source, input_node.line = tab_item.source, tab_item.line
                 children.append(input_node)
 
                 # create: <label for="id">...</label>
                 label_node = sd_tab_label(
                     "",
+                    "",
                     *tab_label.children,
                     input_id=tab_item_identity,
                     classes=tab_label["classes"],
                 )
                 if tab_label.get("ids"):
                     label_node["ids"] += tab_label["ids"]
-                if "sync_id" in tab_label:
+                if "sync_group" in tab_label and "sync_id" in tab_label:
+                    label_node["sync_group"] = tab_label["sync_group"]
                     label_node["sync_id"] = tab_label["sync_id"]
                 label_node.source, label_node.line = tab_item.source, tab_item.line
                 children.append(label_node)
 
                 # add content
                 children.append(tab_content)
```

### Comparing `sphinx_design-0.5.0/tox.ini` & `sphinx_design-0.6.0/tox.ini`

 * *Files 25% similar despite different names*

```diff
@@ -1,72 +1,43 @@
 # To use tox, see https://tox.readthedocs.io
-# Simply pip or conda install tox
-# If you use conda, you may also want to install tox-conda
+# (you may also want to install tox-uv)
 # then run `tox` or `tox -- {pytest args}`
 # run in parallel using `tox -p`
 [tox]
-envlist = py38
+envlist = py39
 
 [testenv]
 usedevelop = true
 
-[testenv:py{38,39,310,311}]
+[testenv:py{39,310,311,312}]
 description = Run unit tests with this Python version
 extras =
     testing
 commands = pytest {posargs}
 
-[testenv:docs-{update,clean}-{alabaster,rtd,pydata,sbt,furo}]
+[testenv:docs-{alabaster,rtd,pydata,sbt,furo,im}]
 description =
-    clean: Run documentation build for this theme (removing existing builds)
-    update: Run documentation build for this theme (reusing existing builds)
+    Run documentation build for this theme
 extras =
     rtd
     rtd: theme_rtd
     pydata: theme_pydata
     sbt: theme_sbt
     furo: theme_furo
-whitelist_externals =
-    clean: rm
-    echo
+    im: theme_im
+allowlist_externals = echo
+passenv =
+    BUILDER
+    CLEAN
+    TERM
 setenv =
-    update: SKIP_APIDOC = true
     alabaster: SPHINX_THEME = alabaster
     rtd: SPHINX_THEME = sphinx_rtd_theme
     pydata: SPHINX_THEME = pydata_sphinx_theme
     sbt: SPHINX_THEME = sphinx_book_theme
     furo: SPHINX_THEME = furo
+    im: SPHINX_THEME = sphinx_immaterial
+commands_pre =
+  python -c "import shutil; shutil.rmtree('docs/_build/{env:BUILDER:html}/{env:SPHINX_THEME:}', ignore_errors=True) if '{env:CLEAN:}' else None"
 commands =
-    clean: rm -rf docs/_build/{posargs:html}
-    sphinx-build -nW --keep-going -b {posargs:html} docs/ docs/_build/{posargs:html}
-commands_post = echo "open docs/_build/{posargs:html}/index.html"
-
-[testenv:docs-live-{alabaster,rtd,pydata,sbt,furo}]
-description = Start documentation autobuild for this theme
-extras =
-    rtd
-    rtd: theme_rtd
-    pydata: theme_pydata
-    sbt: theme_sbt
-    furo: theme_furo
-deps =
-    pre-commit
-    sphinx-autobuild
-setenv =
-    alabaster: SPHINX_THEME = alabaster
-    rtd: SPHINX_THEME = sphinx_rtd_theme
-    pydata: SPHINX_THEME = pydata_sphinx_theme
-    sbt: SPHINX_THEME = sphinx_book_theme
-    furo: SPHINX_THEME = furo
-commands =
-    sphinx-autobuild \
-        --watch sphinx_design \
-        --watch style \
-        --pre-build "npm run css" \
-        --re-ignore sphinx_design/compiled/.* \
-        --re-ignore docs/_build/.* \
-        --port 0 --open-browser \
-         -n -b {posargs:html} docs/ docs/_build/{posargs:html}
-
-[flake8]
-max-line-length = 100
-extend-ignore = E203
+    sphinx-build -nW --keep-going {posargs} -b {env:BUILDER:html} docs/ docs/_build/{env:BUILDER:html}/{env:SPHINX_THEME:}
+commands_post = echo "open docs/_build//{env:BUILDER:html}/{env:SPHINX_THEME:}/index.html"
```

### Comparing `sphinx_design-0.5.0/PKG-INFO` & `sphinx_design-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 Metadata-Version: 2.1
 Name: sphinx_design
-Version: 0.5.0
+Version: 0.6.0
 Summary: A sphinx extension for designing beautiful, view size responsive web components.
 Keywords: sphinx,extension,material design,web components
 Author-email: Chris Sewell <chrisj_sewell@hotmail.com>
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Text Processing :: Markup :: reStructuredText
 Requires-Dist: sphinx>=5,<8
-Requires-Dist: pre-commit>=3,<4 ; extra == "code_style"
+Requires-Dist: pre-commit>=3,<4 ; extra == "code-style"
 Requires-Dist: myst-parser>=1,<3 ; extra == "rtd"
 Requires-Dist: myst-parser>=1,<3 ; extra == "testing"
 Requires-Dist: pytest~=7.1 ; extra == "testing"
 Requires-Dist: pytest-cov ; extra == "testing"
 Requires-Dist: pytest-regressions ; extra == "testing"
-Requires-Dist: furo~=2023.7.0 ; extra == "theme_furo"
-Requires-Dist: pydata-sphinx-theme~=0.13.0 ; extra == "theme_pydata"
-Requires-Dist: sphinx-rtd-theme~=1.0 ; extra == "theme_rtd"
-Requires-Dist: sphinx-book-theme~=1.0 ; extra == "theme_sbt"
+Requires-Dist: defusedxml ; extra == "testing"
+Requires-Dist: furo~=2024.5.4 ; extra == "theme-furo"
+Requires-Dist: sphinx-immaterial~=0.11.11 ; extra == "theme-im"
+Requires-Dist: pydata-sphinx-theme~=0.15.2 ; extra == "theme-pydata"
+Requires-Dist: sphinx-rtd-theme~=2.0 ; extra == "theme-rtd"
+Requires-Dist: sphinx-book-theme~=1.1 ; extra == "theme-sbt"
 Project-URL: Documentation, https://sphinx-design.readthedocs.io
 Project-URL: Homepage, https://github.com/executablebooks/sphinx-design
-Provides-Extra: code_style
+Provides-Extra: code-style
 Provides-Extra: rtd
 Provides-Extra: testing
-Provides-Extra: theme_furo
-Provides-Extra: theme_pydata
-Provides-Extra: theme_rtd
-Provides-Extra: theme_sbt
+Provides-Extra: theme-furo
+Provides-Extra: theme-im
+Provides-Extra: theme-pydata
+Provides-Extra: theme-rtd
+Provides-Extra: theme-sbt
 
 # sphinx-design
 
 [![Github-CI][github-ci]][github-link]
 [![Coverage Status][codecov-badge]][codecov-link]
 [![PyPI][pypi-badge]][pypi-link]
 
@@ -111,16 +114,14 @@
 
 Use autoprefixer when compiling SASS (see <https://getbootstrap.com/docs/5.0/getting-started/browsers-devices/#supported-browsers>)
 
 horizontal card (grid row inside card, picture on left)
 
 subtitle for card (see <https://material.io/components/cards#anatomy>)
 
-rtd PRs not working
-
 
 [github-ci]: https://github.com/executablebooks/sphinx-design/workflows/continuous-integration/badge.svg?branch=main
 [github-link]: https://github.com/executablebooks/sphinx-design
 [codecov-badge]: https://codecov.io/gh/executablebooks/sphinx-design/branch/main/graph/badge.svg
 [codecov-link]: https://codecov.io/gh/executablebooks/sphinx-design
 [pypi-badge]: https://img.shields.io/pypi/v/sphinx-design.svg
 [pypi-link]: https://pypi.org/project/sphinx-design
```

