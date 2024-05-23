# Comparing `tmp/chanjo-report-4.9.2.tar.gz` & `tmp/chanjo-report-4.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chanjo-report-4.9.2.tar", last modified: Mon Feb  7 14:01:26 2022, max compression
+gzip compressed data, was "dist/chanjo-report-4.9.3.tar", last modified: Tue Apr 26 12:37:59 2022, max compression
```

## Comparing `chanjo-report-4.9.2.tar` & `chanjo-report-4.9.3.tar`

### file list

```diff
@@ -1,66 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-07 14:01:26.000000 chanjo-report-4.9.2/
--rw-r--r--   0 runner    (1001) docker     (116)      341 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (116)     5071 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (116)     5067 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (116)     1057 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      306 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2865 2022-02-07 14:01:26.000000 chanjo-report-4.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1870 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-07 14:01:26.000000 chanjo-report-4.9.2/chanjo_report/
--rw-r--r--   0 runner    (1001) docker     (116)     1025 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/chanjo_report/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-07 14:01:26.000000 chanjo-report-4.9.2/chanjo_report/cli/
--rw-r--r--   0 runner    (1001) docker     (116)       49 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/chanjo_report/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      783 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/chanjo_report/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (116)      589 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/chanjo_report/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-07 14:01:26.000000 chanjo-report-4.9.2/chanjo_report/interfaces/
--rw-r--r--   0 runner    (1001) docker     (116)       82 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/chanjo_report/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      863 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/chanjo_report/interfaces/html.py
--rw-r--r--   0 runner    (1001) docker     (116)      950 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/chanjo_report/interfaces/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-07 14:01:26.000000 chanjo-report-4.9.2/chanjo_report/server/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/chanjo_report/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2305 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/chanjo_report/server/app.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-07 14:01:26.000000 chanjo-report-4.9.2/chanjo_report/server/blueprints/
--rw-r--r--   0 runner    (1001) docker     (116)       82 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/chanjo_report/server/blueprints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-07 14:01:26.000000 chanjo-report-4.9.2/chanjo_report/server/blueprints/index/
--rw-r--r--   0 runner    (1001) docker     (116)       52 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/chanjo_report/server/blueprints/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      647 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/chanjo_report/server/blueprints/index/views.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-07 14:01:26.000000 chanjo-report-4.9.2/chanjo_report/server/blueprints/report/
--rw-r--r--   0 runner    (1001) docker     (116)       53 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/chanjo_report/server/blueprints/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2102 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/chanjo_report/server/blueprints/report/controllers.py
--rw-r--r--   0 runner    (1001) docker     (116)     7214 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/chanjo_report/server/blueprints/report/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     5250 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/chanjo_report/server/blueprints/report/views.py
--rw-r--r--   0 runner    (1001) docker     (116)      664 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/chanjo_report/server/config.py
--rw-r--r--   0 runner    (1001) docker     (116)      234 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/chanjo_report/server/constants.py
--rw-r--r--   0 runner    (1001) docker     (116)      209 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/chanjo_report/server/extensions.py
--rw-r--r--   0 runner    (1001) docker     (116)     1118 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/chanjo_report/server/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-07 14:01:26.000000 chanjo-report-4.9.2/chanjo_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2865 2022-02-07 14:01:26.000000 chanjo-report-4.9.2/chanjo_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1433 2022-02-07 14:01:26.000000 chanjo-report-4.9.2/chanjo_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-02-07 14:01:26.000000 chanjo-report-4.9.2/chanjo_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       58 2022-02-07 14:01:26.000000 chanjo-report-4.9.2/chanjo_report.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-02-07 14:01:26.000000 chanjo-report-4.9.2/chanjo_report.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      147 2022-02-07 14:01:26.000000 chanjo-report-4.9.2/chanjo_report.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2022-02-07 14:01:26.000000 chanjo-report-4.9.2/chanjo_report.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-07 14:01:26.000000 chanjo-report-4.9.2/docs/
--rw-r--r--   0 runner    (1001) docker     (116)       27 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (116)     8461 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)       32 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (116)       27 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (116)      509 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)      208 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (116)     6466 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (116)       26 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (116)       83 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-07 14:01:26.000000 chanjo-report-4.9.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (116)       57 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/requirements/conda.txt
--rw-r--r--   0 runner    (1001) docker     (116)      133 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (116)      167 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      102 2022-02-07 14:01:26.000000 chanjo-report-4.9.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (116)     3305 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)     1418 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-07 14:01:26.000000 chanjo-report-4.9.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-07 14:01:26.000000 chanjo-report-4.9.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/tests/fixtures/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (116)     1574 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/tests/fixtures/CCDS.mini.coverage.bed
--rw-r--r--   0 runner    (1001) docker     (116)     4716 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/tests/fixtures/test.sambamba.bed
--rwxr-xr-x   0 runner    (1001) docker     (116)      320 2022-02-07 14:01:19.000000 chanjo-report-4.9.2/tests/test_chanjo-report.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-26 12:37:59.000000 chanjo-report-4.9.3/
+-rw-r--r--   0 runner    (1001) docker     (116)      341 2022-04-26 12:37:43.000000 chanjo-report-4.9.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (116)     5271 2022-04-26 12:37:43.000000 chanjo-report-4.9.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (116)     5067 2022-04-26 12:37:43.000000 chanjo-report-4.9.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1057 2022-04-26 12:37:43.000000 chanjo-report-4.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      306 2022-04-26 12:37:43.000000 chanjo-report-4.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     2865 2022-04-26 12:37:59.000000 chanjo-report-4.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1870 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-26 12:37:59.000000 chanjo-report-4.9.3/chanjo_report/
+-rw-r--r--   0 runner    (1001) docker     (116)     1025 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/chanjo_report/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-26 12:37:59.000000 chanjo-report-4.9.3/chanjo_report/cli/
+-rw-r--r--   0 runner    (1001) docker     (116)       49 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/chanjo_report/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      783 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/chanjo_report/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (116)      589 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/chanjo_report/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-26 12:37:59.000000 chanjo-report-4.9.3/chanjo_report/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (116)       82 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/chanjo_report/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      863 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/chanjo_report/interfaces/html.py
+-rw-r--r--   0 runner    (1001) docker     (116)      950 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/chanjo_report/interfaces/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-26 12:37:59.000000 chanjo-report-4.9.3/chanjo_report/server/
+-rw-r--r--   0 runner    (1001) docker     (116)       24 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/chanjo_report/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2305 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/chanjo_report/server/app.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-26 12:37:59.000000 chanjo-report-4.9.3/chanjo_report/server/blueprints/
+-rw-r--r--   0 runner    (1001) docker     (116)       82 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/chanjo_report/server/blueprints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-26 12:37:59.000000 chanjo-report-4.9.3/chanjo_report/server/blueprints/index/
+-rw-r--r--   0 runner    (1001) docker     (116)       52 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/chanjo_report/server/blueprints/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      647 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/chanjo_report/server/blueprints/index/views.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-26 12:37:59.000000 chanjo-report-4.9.3/chanjo_report/server/blueprints/report/
+-rw-r--r--   0 runner    (1001) docker     (116)       53 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/chanjo_report/server/blueprints/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2102 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/chanjo_report/server/blueprints/report/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7214 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/chanjo_report/server/blueprints/report/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5250 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/chanjo_report/server/blueprints/report/views.py
+-rw-r--r--   0 runner    (1001) docker     (116)      664 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/chanjo_report/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (116)      234 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/chanjo_report/server/constants.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1167 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/chanjo_report/server/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1118 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/chanjo_report/server/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-26 12:37:59.000000 chanjo-report-4.9.3/chanjo_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     2865 2022-04-26 12:37:59.000000 chanjo-report-4.9.3/chanjo_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1389 2022-04-26 12:37:59.000000 chanjo-report-4.9.3/chanjo_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-26 12:37:59.000000 chanjo-report-4.9.3/chanjo_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       58 2022-04-26 12:37:59.000000 chanjo-report-4.9.3/chanjo_report.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-26 12:37:59.000000 chanjo-report-4.9.3/chanjo_report.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)      187 2022-04-26 12:37:59.000000 chanjo-report-4.9.3/chanjo_report.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       14 2022-04-26 12:37:59.000000 chanjo-report-4.9.3/chanjo_report.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-26 12:37:59.000000 chanjo-report-4.9.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (116)       27 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (116)     8461 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (116)       32 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       27 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      509 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      208 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     6466 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (116)       26 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       83 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      187 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      102 2022-04-26 12:37:59.000000 chanjo-report-4.9.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (116)     3558 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1418 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-26 12:37:59.000000 chanjo-report-4.9.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-26 12:37:59.000000 chanjo-report-4.9.3/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/tests/fixtures/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (116)     1574 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/tests/fixtures/CCDS.mini.coverage.bed
+-rw-r--r--   0 runner    (1001) docker     (116)     4716 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/tests/fixtures/test.sambamba.bed
+-rwxr-xr-x   0 runner    (1001) docker     (116)      320 2022-04-26 12:37:44.000000 chanjo-report-4.9.3/tests/test_chanjo-report.py
```

### Comparing `chanjo-report-4.9.2/CHANGELOG.md` & `chanjo-report-4.9.3/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Change log
 
+## 4.9.3 (2022-04-26)
+### Changed
+- Install requirements from requirements file parsed in setup.py
+### Fixed
+- Error launching the app due to `LocalStack.__ident_func__` missing in werkzeug >= 2.1.x
+
 ## 4.9.2 (2022-02-07)
 ### Fixed
 - App crashing when unsupported gene IDs are provided in the report endpoint
 
 ## 4.9.1 (2022-01-20)
 ### Fixed
 - Typo in Makefile preventing loading of demodata
```

### Comparing `chanjo-report-4.9.2/CONTRIBUTING.md` & `chanjo-report-4.9.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `chanjo-report-4.9.2/LICENSE` & `chanjo-report-4.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chanjo-report-4.9.2/PKG-INFO` & `chanjo-report-4.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: chanjo-report
-Version: 4.9.2
+Version: 4.9.3
 Summary: Automatically render coverage reports from Chanjo ouput
 Home-page: https://github.com/robinandeer/chanjo-report
 Author: Robin Andeer
 Author-email: robin.andeer@scilifelab.se
 License: MIT
 Description: ![Example report (eng)](artwork/screenshot.png)
```

### Comparing `chanjo-report-4.9.2/README.md` & `chanjo-report-4.9.3/README.md`

 * *Files identical despite different names*

### Comparing `chanjo-report-4.9.2/chanjo_report/__init__.py` & `chanjo-report-4.9.3/chanjo_report/__init__.py`

 * *Files identical despite different names*

### Comparing `chanjo-report-4.9.2/chanjo_report/cli/core.py` & `chanjo-report-4.9.3/chanjo_report/cli/core.py`

 * *Files identical despite different names*

### Comparing `chanjo-report-4.9.2/chanjo_report/cli/utils.py` & `chanjo-report-4.9.3/chanjo_report/cli/utils.py`

 * *Files identical despite different names*

### Comparing `chanjo-report-4.9.2/chanjo_report/interfaces/html.py` & `chanjo-report-4.9.3/chanjo_report/interfaces/html.py`

 * *Files identical despite different names*

### Comparing `chanjo-report-4.9.2/chanjo_report/interfaces/pdf.py` & `chanjo-report-4.9.3/chanjo_report/interfaces/pdf.py`

 * *Files identical despite different names*

### Comparing `chanjo-report-4.9.2/chanjo_report/server/app.py` & `chanjo-report-4.9.3/chanjo_report/server/app.py`

 * *Files identical despite different names*

### Comparing `chanjo-report-4.9.2/chanjo_report/server/blueprints/index/views.py` & `chanjo-report-4.9.3/chanjo_report/server/blueprints/index/views.py`

 * *Files identical despite different names*

### Comparing `chanjo-report-4.9.2/chanjo_report/server/blueprints/report/controllers.py` & `chanjo-report-4.9.3/chanjo_report/server/blueprints/report/controllers.py`

 * *Files identical despite different names*

### Comparing `chanjo-report-4.9.2/chanjo_report/server/blueprints/report/utils.py` & `chanjo-report-4.9.3/chanjo_report/server/blueprints/report/utils.py`

 * *Files identical despite different names*

### Comparing `chanjo-report-4.9.2/chanjo_report/server/blueprints/report/views.py` & `chanjo-report-4.9.3/chanjo_report/server/blueprints/report/views.py`

 * *Files identical despite different names*

### Comparing `chanjo-report-4.9.2/chanjo_report/server/config.py` & `chanjo-report-4.9.3/chanjo_report/server/config.py`

 * *Files identical despite different names*

### Comparing `chanjo-report-4.9.2/chanjo_report/server/utils.py` & `chanjo-report-4.9.3/chanjo_report/server/utils.py`

 * *Files identical despite different names*

### Comparing `chanjo-report-4.9.2/chanjo_report.egg-info/PKG-INFO` & `chanjo-report-4.9.3/chanjo_report.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: chanjo-report
-Version: 4.9.2
+Version: 4.9.3
 Summary: Automatically render coverage reports from Chanjo ouput
 Home-page: https://github.com/robinandeer/chanjo-report
 Author: Robin Andeer
 Author-email: robin.andeer@scilifelab.se
 License: MIT
 Description: ![Example report (eng)](artwork/screenshot.png)
```

### Comparing `chanjo-report-4.9.2/chanjo_report.egg-info/SOURCES.txt` & `chanjo-report-4.9.3/chanjo_report.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -40,13 +40,11 @@
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
-requirements/conda.txt
-requirements/dev.txt
 tests/test_chanjo-report.py
 tests/fixtures/.gitkeep
 tests/fixtures/CCDS.mini.coverage.bed
 tests/fixtures/test.sambamba.bed
```

### Comparing `chanjo-report-4.9.2/docs/conf.py` & `chanjo-report-4.9.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chanjo-report-4.9.2/docs/make.bat` & `chanjo-report-4.9.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chanjo-report-4.9.2/setup.py` & `chanjo-report-4.9.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,38 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """Based on https://github.com/pypa/sampleproject/blob/master/setup.py."""
 import codecs
+import io
 import os
 import sys
 
 from setuptools import find_packages, setup
 from setuptools.command.test import test as TestCommand
 
+HERE = os.path.abspath(os.path.dirname(__file__))
+
+
+def parse_reqs(req_path="./requirements.txt"):
+    """Parse lib requirements from requirement.txt file"""
+    install_requires = []
+    with io.open(os.path.join(HERE, "requirements.txt"), encoding="utf-8") as handle:
+        # remove comments and empty lines
+        lines = (line.strip() for line in handle if line.strip() and not line.startswith("#"))
+
+        for line in lines:
+            # add the line as a new requirement
+            install_requires.append(line)
+
+    return install_requires
+
+
+REQUIRED = parse_reqs()
+
+
 # shortcut for building/publishing to Pypi
 if sys.argv[-1] == "publish":
     os.system("python setup.py sdist bdist_wheel upload")
     sys.exit()
 
 
 # this is a plug-in for setuptools that will invoke py.test
@@ -36,23 +57,22 @@
         # import here, because outside the required eggs aren't loaded yet
         import pytest
 
         sys.exit(pytest.main(self.test_args))
 
 
 # get the long description from the relevant file
-HERE = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 
 setup(
     name="chanjo-report",
     # versions should comply with PEP440
-    version="4.9.2",
+    version="4.9.3",
     description="Automatically render coverage reports from Chanjo ouput",
     long_description=LONG_DESCRIPTION,
     # what does your project relate to?
     keywords="chanjo-report development",
     author="Robin Andeer",
     author_email="robin.andeer@scilifelab.se",
     license="MIT",
@@ -68,29 +88,15 @@
             "server/blueprints/report/templates/report/*.html",
             "server/blueprints/report/templates/report/layouts/*.html",
             "server/blueprints/report/templates/report/components/*.html",
             "server/translations/sv/LC_MESSAGES/*",
         ]
     },
     zip_safe=False,
-    install_requires=[
-        "setuptools",
-        "chanjo>=4.1.0",
-        "Flask-WeasyPrint",
-        "cairocffi",
-        "lxml>=3.0",
-        "cffi",
-        "Flask",
-        "SQLAlchemy",
-        "Flask-Babel",
-        "tabulate",
-        "Flask-Alchy",
-        "Flask-SQLAlchemy==2.1",
-        "pymysql",
-    ],
+    install_requires=REQUIRED,
     tests_require=["pytest"],
     cmdclass={"test": PyTest},
     # to provide executable scripts, use entry points
     entry_points={
         "chanjo.subcommands.4": ["report = chanjo_report.cli:report"],
     },
     # see: http://pypi.python.org/pypi?%3Aaction=list_classifiers
```

### Comparing `chanjo-report-4.9.2/tasks.py` & `chanjo-report-4.9.3/tasks.py`

 * *Files identical despite different names*

### Comparing `chanjo-report-4.9.2/tests/fixtures/CCDS.mini.coverage.bed` & `chanjo-report-4.9.3/tests/fixtures/CCDS.mini.coverage.bed`

 * *Files identical despite different names*

### Comparing `chanjo-report-4.9.2/tests/fixtures/test.sambamba.bed` & `chanjo-report-4.9.3/tests/fixtures/test.sambamba.bed`

 * *Files identical despite different names*

