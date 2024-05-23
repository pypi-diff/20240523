# Comparing `tmp/typeshed_stats-24.5.21.tar.gz` & `tmp/typeshed_stats-24.5.22.tar.gz`

## Comparing `typeshed_stats-24.5.21.tar` & `typeshed_stats-24.5.22.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.editorconfig
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.gitattributes
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.markdownlint.yaml
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/mkdocs.yml
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/website_macros.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.github/renovate.json5
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.github/workflows/check-requirements.yml
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.github/workflows/regen-examples-and-docs.yml
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.github/workflows/test-website.yml
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.github/workflows/test.yml
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.github/workflows/typecheck.yml
--rw-r--r--   0        0        0    31439 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/examples/example.csv
--rw-r--r--   0        0        0   170878 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/examples/example.json
--rw-r--r--   0        0        0   286068 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/examples/example.md
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/scripts/regenerate.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/scripts/runtests.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/src/typeshed_stats/__init__.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/src/typeshed_stats/__main__.py
--rw-r--r--   0        0        0    10933 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/src/typeshed_stats/_cli.py
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/src/typeshed_stats/_markdown_template.md.jinja
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/src/typeshed_stats/_version.py
--rw-r--r--   0        0        0    50756 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/src/typeshed_stats/gather.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/src/typeshed_stats/py.typed
--rw-r--r--   0        0        0     7855 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/src/typeshed_stats/serialize.py
--rw-r--r--   0        0        0   791271 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/big_logo.png
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/cli.md
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/gather.md
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/index.md
--rw-r--r--   0        0        0   111209 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/logo.png
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/serialize.md
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/stats-csv.md
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/stats.md
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/.snippets/links.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/.snippets/refs.md
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/javascripts/filtertable.js
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/javascripts/tablesort.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/tests/__init__.py
--rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/tests/conftest.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/tests/test___all__.py
--rw-r--r--   0        0        0    22122 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/tests/test__cli.py
--rw-r--r--   0        0        0    42127 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/tests/test_gather.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/tests/test_running_from_command_line.py
--rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/tests/test_serialize.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/LICENSE
--rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/README.md
--rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/pyproject.toml
--rw-r--r--   0        0        0     8708 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/PKG-INFO
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/.editorconfig
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/.gitattributes
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/.markdownlint.yaml
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/mkdocs.yml
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/website_macros.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/.github/renovate.json5
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/.github/workflows/check-requirements.yml
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/.github/workflows/regen-examples-and-docs.yml
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/.github/workflows/test-website.yml
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/.github/workflows/test.yml
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/.github/workflows/typecheck.yml
+-rw-r--r--   0        0        0    31439 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/examples/example.csv
+-rw-r--r--   0        0        0   170878 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/examples/example.json
+-rw-r--r--   0        0        0   286068 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/examples/example.md
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/scripts/regenerate.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/scripts/runtests.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/src/typeshed_stats/__init__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/src/typeshed_stats/__main__.py
+-rw-r--r--   0        0        0    10933 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/src/typeshed_stats/_cli.py
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/src/typeshed_stats/_markdown_template.md.jinja
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/src/typeshed_stats/_version.py
+-rw-r--r--   0        0        0    50756 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/src/typeshed_stats/gather.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/src/typeshed_stats/py.typed
+-rw-r--r--   0        0        0     7855 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/src/typeshed_stats/serialize.py
+-rw-r--r--   0        0        0   791271 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/stats_website/big_logo.png
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/stats_website/cli.md
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/stats_website/gather.md
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/stats_website/index.md
+-rw-r--r--   0        0        0   111209 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/stats_website/logo.png
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/stats_website/serialize.md
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/stats_website/stats-csv.md
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/stats_website/stats.md
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/stats_website/.snippets/links.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/stats_website/.snippets/refs.md
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/stats_website/javascripts/filtertable.js
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/stats_website/javascripts/tablesort.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/tests/__init__.py
+-rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/tests/conftest.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/tests/test___all__.py
+-rw-r--r--   0        0        0    22122 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/tests/test__cli.py
+-rw-r--r--   0        0        0    42127 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/tests/test_gather.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/tests/test_running_from_command_line.py
+-rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/tests/test_serialize.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/LICENSE
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/README.md
+-rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/pyproject.toml
+-rw-r--r--   0        0        0     8708 2020-02-02 00:00:00.000000 typeshed_stats-24.5.22/PKG-INFO
```

### Comparing `typeshed_stats-24.5.21/.pre-commit-config.yaml` & `typeshed_stats-24.5.22/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/mkdocs.yml` & `typeshed_stats-24.5.22/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/website_macros.py` & `typeshed_stats-24.5.22/website_macros.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/.github/renovate.json5` & `typeshed_stats-24.5.22/.github/renovate.json5`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/.github/workflows/check-requirements.yml` & `typeshed_stats-24.5.22/.github/workflows/check-requirements.yml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/.github/workflows/publish.yml` & `typeshed_stats-24.5.22/.github/workflows/publish.yml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 name: Publish Python distributions to PyPI
 
 on:
   push:
   workflow_dispatch:
   schedule:
-    - cron: "0 0 * * 0"
+    - cron: "0 0 * * *"
 
 permissions:
   contents: read
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.head_ref || github.run_id }}
   cancel-in-progress: true
```

### Comparing `typeshed_stats-24.5.21/.github/workflows/regen-examples-and-docs.yml` & `typeshed_stats-24.5.22/.github/workflows/regen-examples-and-docs.yml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/.github/workflows/test-website.yml` & `typeshed_stats-24.5.22/.github/workflows/test-website.yml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/.github/workflows/test.yml` & `typeshed_stats-24.5.22/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/.github/workflows/typecheck.yml` & `typeshed_stats-24.5.22/.github/workflows/typecheck.yml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/examples/example.csv` & `typeshed_stats-24.5.22/examples/example.csv`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/examples/example.json` & `typeshed_stats-24.5.22/examples/example.json`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/examples/example.md` & `typeshed_stats-24.5.22/examples/example.md`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/scripts/regenerate.py` & `typeshed_stats-24.5.22/scripts/regenerate.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/scripts/runtests.py` & `typeshed_stats-24.5.22/scripts/runtests.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/src/typeshed_stats/_cli.py` & `typeshed_stats-24.5.22/src/typeshed_stats/_cli.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/src/typeshed_stats/_markdown_template.md.jinja` & `typeshed_stats-24.5.22/src/typeshed_stats/_markdown_template.md.jinja`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/src/typeshed_stats/gather.py` & `typeshed_stats-24.5.22/src/typeshed_stats/gather.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/src/typeshed_stats/serialize.py` & `typeshed_stats-24.5.22/src/typeshed_stats/serialize.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/stats_website/big_logo.png` & `typeshed_stats-24.5.22/stats_website/big_logo.png`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/stats_website/gather.md` & `typeshed_stats-24.5.22/stats_website/gather.md`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/stats_website/logo.png` & `typeshed_stats-24.5.22/stats_website/logo.png`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/stats_website/stats-csv.md` & `typeshed_stats-24.5.22/stats_website/stats-csv.md`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/stats_website/.snippets/links.md` & `typeshed_stats-24.5.22/stats_website/.snippets/links.md`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/stats_website/javascripts/filtertable.js` & `typeshed_stats-24.5.22/stats_website/javascripts/filtertable.js`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/tests/conftest.py` & `typeshed_stats-24.5.22/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/tests/test___all__.py` & `typeshed_stats-24.5.22/tests/test___all__.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/tests/test__cli.py` & `typeshed_stats-24.5.22/tests/test__cli.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/tests/test_gather.py` & `typeshed_stats-24.5.22/tests/test_gather.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/tests/test_running_from_command_line.py` & `typeshed_stats-24.5.22/tests/test_running_from_command_line.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/tests/test_serialize.py` & `typeshed_stats-24.5.22/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/.gitignore` & `typeshed_stats-24.5.22/.gitignore`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/LICENSE` & `typeshed_stats-24.5.22/LICENSE`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/README.md` & `typeshed_stats-24.5.22/README.md`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/pyproject.toml` & `typeshed_stats-24.5.22/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.21/PKG-INFO` & `typeshed_stats-24.5.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: typeshed_stats
-Version: 24.5.21
+Version: 24.5.22
 Summary: Library and command-line tool to gather stats on typeshed packages
 Project-URL: Homepage, https://github.com/AlexWaygood/typeshed-stats
 Project-URL: Bug Tracker, https://github.com/AlexWaygood/typeshed-stats/issues
 Author-email: Alex Waygood <alex.waygood@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: stubs,typeshed,typing
```

