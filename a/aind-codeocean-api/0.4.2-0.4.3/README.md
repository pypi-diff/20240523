# Comparing `tmp/aind_codeocean_api-0.4.2.tar.gz` & `tmp/aind_codeocean_api-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_codeocean_api-0.4.2.tar", last modified: Tue Feb  6 01:34:34 2024, max compression
+gzip compressed data, was "aind_codeocean_api-0.4.3.tar", last modified: Wed May 22 22:19:55 2024, max compression
```

## Comparing `aind_codeocean_api-0.4.2.tar` & `aind_codeocean_api-0.4.3.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:34:34.591850 aind_codeocean_api-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:34:34.579850 aind_codeocean_api-0.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:34:34.583850 aind_codeocean_api-0.4.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:34:34.583850 aind_codeocean_api-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/.github/workflows/lint_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-02-06 01:34:34.591850 aind_codeocean_api-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:34:34.583850 aind_codeocean_api-0.4.2/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:34:34.583850 aind_codeocean_api-0.4.2/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:34:34.587850 aind_codeocean_api-0.4.2/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/doc_template/source/aind_codeocean_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/doc_template/source/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:34:34.587850 aind_codeocean_api-0.4.2/integration/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/integration/.env.template
--rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/integration/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 01:34:34.591850 aind_codeocean_api-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:34:34.583850 aind_codeocean_api-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:34:34.587850 aind_codeocean_api-0.4.2/src/aind_codeocean_api/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-06 01:34:17.000000 aind_codeocean_api-0.4.2/src/aind_codeocean_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/src/aind_codeocean_api/codeocean.py
--rw-r--r--   0 runner    (1001) docker     (127)    10319 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/src/aind_codeocean_api/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:34:34.587850 aind_codeocean_api-0.4.2/src/aind_codeocean_api/models/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/src/aind_codeocean_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/src/aind_codeocean_api/models/basic_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/src/aind_codeocean_api/models/computations_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/src/aind_codeocean_api/models/data_assets_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:34:34.587850 aind_codeocean_api-0.4.2/src/aind_codeocean_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-02-06 01:34:34.000000 aind_codeocean_api-0.4.2/src/aind_codeocean_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-02-06 01:34:34.000000 aind_codeocean_api-0.4.2/src/aind_codeocean_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 01:34:34.000000 aind_codeocean_api-0.4.2/src/aind_codeocean_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-06 01:34:34.000000 aind_codeocean_api-0.4.2/src/aind_codeocean_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-06 01:34:34.000000 aind_codeocean_api-0.4.2/src/aind_codeocean_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:34:34.587850 aind_codeocean_api-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:34:34.587850 aind_codeocean_api-0.4.2/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/tests/resources/fake_credentials.json
--rw-r--r--   0 runner    (1001) docker     (127)    36949 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/tests/test_codeocean_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-02-06 01:34:16.000000 aind_codeocean_api-0.4.2/tests/test_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.793037 aind_codeocean_api-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.785036 aind_codeocean_api-0.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.785036 aind_codeocean_api-0.4.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.785036 aind_codeocean_api-0.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/.github/workflows/lint_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-22 22:19:55.793037 aind_codeocean_api-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.789037 aind_codeocean_api-0.4.3/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.789037 aind_codeocean_api-0.4.3/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.789037 aind_codeocean_api-0.4.3/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/doc_template/source/aind_codeocean_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/doc_template/source/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.789037 aind_codeocean_api-0.4.3/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/integration/.env.template
+-rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/integration/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 22:19:55.793037 aind_codeocean_api-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.785036 aind_codeocean_api-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.789037 aind_codeocean_api-0.4.3/src/aind_codeocean_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api/codeocean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10319 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.793037 aind_codeocean_api-0.4.3/src/aind_codeocean_api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api/models/basic_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api/models/computations_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api/models/data_assets_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.793037 aind_codeocean_api-0.4.3/src/aind_codeocean_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-22 22:19:55.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-22 22:19:55.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:19:55.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-22 22:19:55.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 22:19:55.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.793037 aind_codeocean_api-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.793037 aind_codeocean_api-0.4.3/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/tests/resources/fake_credentials.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36949 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/tests/test_codeocean_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/tests/test_credentials.py
```

### Comparing `aind_codeocean_api-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_codeocean_api-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_codeocean_api-0.4.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/.github/ISSUE_TEMPLATE/user-story.md` & `aind_codeocean_api-0.4.3/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/.github/workflows/lint_and_test.yml` & `aind_codeocean_api-0.4.3/.github/workflows/lint_and_test.yml`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/.github/workflows/tag_and_publish.yml` & `aind_codeocean_api-0.4.3/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/.gitignore` & `aind_codeocean_api-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/LICENSE` & `aind_codeocean_api-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/PKG-INFO` & `aind_codeocean_api-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_codeocean_api
-Version: 0.4.2
+Version: 0.4.3
 Summary: CodeOcean API manager in Python
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_codeocean_api-0.4.2/README.md` & `aind_codeocean_api-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/doc_template/Makefile` & `aind_codeocean_api-0.4.3/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/doc_template/make.bat` & `aind_codeocean_api-0.4.3/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/doc_template/source/_static/dark-logo.svg` & `aind_codeocean_api-0.4.3/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/doc_template/source/_static/favicon.ico` & `aind_codeocean_api-0.4.3/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/doc_template/source/_static/light-logo.svg` & `aind_codeocean_api-0.4.3/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/doc_template/source/aind_codeocean_api.rst` & `aind_codeocean_api-0.4.3/doc_template/source/aind_codeocean_api.rst`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/doc_template/source/conf.py` & `aind_codeocean_api-0.4.3/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/integration/run_tests.py` & `aind_codeocean_api-0.4.3/integration/run_tests.py`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/pyproject.toml` & `aind_codeocean_api-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/src/aind_codeocean_api/codeocean.py` & `aind_codeocean_api-0.4.3/src/aind_codeocean_api/codeocean.py`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/src/aind_codeocean_api/credentials.py` & `aind_codeocean_api-0.4.3/src/aind_codeocean_api/credentials.py`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/src/aind_codeocean_api/models/basic_request.py` & `aind_codeocean_api-0.4.3/src/aind_codeocean_api/models/basic_request.py`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/src/aind_codeocean_api/models/computations_requests.py` & `aind_codeocean_api-0.4.3/src/aind_codeocean_api/models/computations_requests.py`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/src/aind_codeocean_api/models/data_assets_requests.py` & `aind_codeocean_api-0.4.3/src/aind_codeocean_api/models/data_assets_requests.py`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/src/aind_codeocean_api.egg-info/PKG-INFO` & `aind_codeocean_api-0.4.3/src/aind_codeocean_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_codeocean_api
-Version: 0.4.2
+Version: 0.4.3
 Summary: CodeOcean API manager in Python
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_codeocean_api-0.4.2/src/aind_codeocean_api.egg-info/SOURCES.txt` & `aind_codeocean_api-0.4.3/src/aind_codeocean_api.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 doc_template/source/_static/favicon.ico
 doc_template/source/_static/light-logo.svg
 integration/.env.template
 integration/run_tests.py
 src/aind_codeocean_api/__init__.py
 src/aind_codeocean_api/codeocean.py
 src/aind_codeocean_api/credentials.py
+src/aind_codeocean_api/py.typed
 src/aind_codeocean_api.egg-info/PKG-INFO
 src/aind_codeocean_api.egg-info/SOURCES.txt
 src/aind_codeocean_api.egg-info/dependency_links.txt
 src/aind_codeocean_api.egg-info/requires.txt
 src/aind_codeocean_api.egg-info/top_level.txt
 src/aind_codeocean_api/models/__init__.py
 src/aind_codeocean_api/models/basic_request.py
```

### Comparing `aind_codeocean_api-0.4.2/tests/test_codeocean_requests.py` & `aind_codeocean_api-0.4.3/tests/test_codeocean_requests.py`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.2/tests/test_credentials.py` & `aind_codeocean_api-0.4.3/tests/test_credentials.py`

 * *Files identical despite different names*

