# Comparing `tmp/nextline_alert-0.1.5.tar.gz` & `tmp/nextline_alert-0.1.6.tar.gz`

## Comparing `nextline_alert-0.1.5.tar` & `nextline_alert-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,29 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/setup.cfg
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/.github/dependabot.yml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/.github/release.yml
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/.github/workflows/release.yml
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/.github/workflows/type-check.yml
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/.github/workflows/unit-test.yml
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/src/nextline_alert/__about__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/src/nextline_alert/__init__.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/src/nextline_alert/default.toml
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/src/nextline_alert/emitter.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/src/nextline_alert/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/src/nextline_alert/py.typed
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/src/nextline_alert/schema/__init__.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/src/nextline_alert/schema/query.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/tests/test_emitter.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/tests/test_version.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/LICENSE.txt
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/README.md
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/setup.cfg
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/.github/CODEOWNERS
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/.github/dependabot.yml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/.github/release.yml
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/.github/workflows/release.yml
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/.github/workflows/type-check.yml
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/.github/workflows/unit-test-latest.yml
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/.github/workflows/unit-test-min.yml
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/.github/workflows/unit-test.yml
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/.vscode/settings.json
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/ci/latest/requirements.txt
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/ci/minimum/requirements.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/src/nextline_alert/__about__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/src/nextline_alert/__init__.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/src/nextline_alert/default.toml
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/src/nextline_alert/emitter.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/src/nextline_alert/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/src/nextline_alert/py.typed
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/src/nextline_alert/schema/__init__.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/src/nextline_alert/schema/query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/tests/test_emitter.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/tests/test_version.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/LICENSE.txt
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/README.md
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 nextline_alert-0.1.6/PKG-INFO
```

### Comparing `nextline_alert-0.1.5/.github/workflows/pypi.yml` & `nextline_alert-0.1.6/.github/workflows/pypi.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 jobs:
   deploy:
     runs-on: ubuntu-latest
     environment: pypi
     permissions:
       id-token: write
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: '3.10'
 
       - name: Install packages
         run: |
           pip install --upgrade pip
           pip install --upgrade hatch
```

### Comparing `nextline_alert-0.1.5/.github/workflows/release.yml` & `nextline_alert-0.1.6/.github/workflows/release.yml`

 * *Files 22% similar despite different names*

```diff
@@ -9,17 +9,17 @@
   deploy:
     runs-on: ubuntu-latest
     permissions:
       contents: write
 
     steps:
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
       - name: Install gh CLI
-        uses: actions/setup-node@v3
+        uses: actions/setup-node@v4
         with:
           node-version: "18"
       - name: Create Release
         env:
           GH_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         run: |
           gh release create ${GITHUB_REF#refs/tags/} \
```

### Comparing `nextline_alert-0.1.5/.github/workflows/type-check.yml` & `nextline_alert-0.1.6/.github/workflows/type-check.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 name: Check static types
 
 on:
   push:
     branches:
-      - "**"
+      - main
   pull_request:
     branches:
-      - "**"
+      - main
 
 jobs:
   run:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.10"
 
       - name: Install packages
         run: |
           pip install --upgrade pip
           pip install -e '.[tests]'
```

### Comparing `nextline_alert-0.1.5/.github/workflows/unit-test.yml` & `nextline_alert-0.1.6/.github/workflows/unit-test.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 name: Run unit tests
 
 on:
   push:
     branches:
-      - "**"
+      - main
   pull_request:
     branches:
-      - "**"
+      - main
 
 concurrency:
   group: unit-test-${{ github.head_ref }}
   cancel-in-progress: true
 
 env:
   PYTHONUNBUFFERED: "1"
@@ -22,29 +22,39 @@
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.10", "3.11", "3.12"]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install packages
         run: |
           pip install --upgrade pip
           pip install -e '.[tests]'
           pip list
 
       - name: Run tests
         run: pytest -vv --cov --cov-report=xml
 
+      - name: Check Codecov token  # e.g., Dependabot doesn't have the CODECOV_TOKEN
+        id: check_codecov_token
+        run: |
+          if [ -n "${{ secrets.CODECOV_TOKEN }}" ]; then
+            echo "exists=true" >> $GITHUB_OUTPUT
+          else
+            echo "exists=false" >> $GITHUB_OUTPUT
+          fi
+
       - name: Upload coverage to Codecov
+        if: steps.check_codecov_token.outputs.exists == 'true'
         uses: codecov/codecov-action@v4
         with:
           fail_ci_if_error: true
           token: ${{ secrets.CODECOV_TOKEN }}
           verbose: true
```

### Comparing `nextline_alert-0.1.5/src/nextline_alert/emitter.py` & `nextline_alert-0.1.6/src/nextline_alert/emitter.py`

 * *Files identical despite different names*

### Comparing `nextline_alert-0.1.5/src/nextline_alert/plugin.py` & `nextline_alert-0.1.6/src/nextline_alert/plugin.py`

 * *Files identical despite different names*

### Comparing `nextline_alert-0.1.5/tests/test_emitter.py` & `nextline_alert-0.1.6/tests/test_emitter.py`

 * *Files identical despite different names*

### Comparing `nextline_alert-0.1.5/.gitignore` & `nextline_alert-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `nextline_alert-0.1.5/LICENSE.txt` & `nextline_alert-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nextline_alert-0.1.5/README.md` & `nextline_alert-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-# Nextline Alert
+# nextline-alert
 
 [![PyPI - Version](https://img.shields.io/pypi/v/nextline-alert.svg)](https://pypi.org/project/nextline-alert)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nextline-alert.svg)](https://pypi.org/project/nextline-alert)
 
 [![Test Status](https://github.com/simonsobs/nextline-alert/actions/workflows/unit-test.yml/badge.svg)](https://github.com/simonsobs/nextline-alert/actions/workflows/unit-test.yml)
 [![Test Status](https://github.com/simonsobs/nextline-alert/actions/workflows/type-check.yml/badge.svg)](https://github.com/simonsobs/nextline-alert/actions/workflows/type-check.yml)
 [![codecov](https://codecov.io/gh/simonsobs/nextline-alert/branch/main/graph/badge.svg)](https://codecov.io/gh/simonsobs/nextline-alert)
 
 A plugin for [nextline-graphql](https://github.com/simonsobs/nextline-graphql).
 Emit alerts to [Campana](https://github.com/simonsobs/campana)
 
-
 ## Installation
 
 ```console
 pip install nextline-alert
 ```
 
 ## Configuration
```

### Comparing `nextline_alert-0.1.5/pyproject.toml` & `nextline_alert-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 [project.optional-dependencies]
 tests = [
   "pytest-asyncio>=0.23",
   "pytest-cov>=4.1",
   "pytest-timeout>=2.2",
   "pytest>=7.4",
-  "respx>=0.20",
+  "respx>=0.20.1",
 ]
 
 [project.urls]
 Documentation = "https://github.com/simonsobs/nextline-alert#readme"
 Issues = "https://github.com/simonsobs/nextline-alert/issues"
 Source = "https://github.com/simonsobs/nextline-alert"
```

### Comparing `nextline_alert-0.1.5/PKG-INFO` & `nextline_alert-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nextline-alert
-Version: 0.1.5
+Version: 0.1.6
 Summary: A plugin of nextline-graphql. Emit alerts to Campana
 Project-URL: Documentation, https://github.com/simonsobs/nextline-alert#readme
 Project-URL: Issues, https://github.com/simonsobs/nextline-alert/issues
 Project-URL: Source, https://github.com/simonsobs/nextline-alert
 Author-email: Simons Observatory <so_software@simonsobservatory.org>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -19,30 +19,29 @@
 Requires-Dist: httpx>=0.26
 Requires-Dist: nextline-graphql>=0.7.8
 Provides-Extra: tests
 Requires-Dist: pytest-asyncio>=0.23; extra == 'tests'
 Requires-Dist: pytest-cov>=4.1; extra == 'tests'
 Requires-Dist: pytest-timeout>=2.2; extra == 'tests'
 Requires-Dist: pytest>=7.4; extra == 'tests'
-Requires-Dist: respx>=0.20; extra == 'tests'
+Requires-Dist: respx>=0.20.1; extra == 'tests'
 Description-Content-Type: text/markdown
 
-# Nextline Alert
+# nextline-alert
 
 [![PyPI - Version](https://img.shields.io/pypi/v/nextline-alert.svg)](https://pypi.org/project/nextline-alert)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nextline-alert.svg)](https://pypi.org/project/nextline-alert)
 
 [![Test Status](https://github.com/simonsobs/nextline-alert/actions/workflows/unit-test.yml/badge.svg)](https://github.com/simonsobs/nextline-alert/actions/workflows/unit-test.yml)
 [![Test Status](https://github.com/simonsobs/nextline-alert/actions/workflows/type-check.yml/badge.svg)](https://github.com/simonsobs/nextline-alert/actions/workflows/type-check.yml)
 [![codecov](https://codecov.io/gh/simonsobs/nextline-alert/branch/main/graph/badge.svg)](https://codecov.io/gh/simonsobs/nextline-alert)
 
 A plugin for [nextline-graphql](https://github.com/simonsobs/nextline-graphql).
 Emit alerts to [Campana](https://github.com/simonsobs/campana)
 
-
 ## Installation
 
 ```console
 pip install nextline-alert
 ```
 
 ## Configuration
```

