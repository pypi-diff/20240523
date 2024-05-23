# Comparing `tmp/auroris-0.1.2.tar.gz` & `tmp/auroris-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auroris-0.1.2.tar", last modified: Wed May  8 00:57:25 2024, max compression
+gzip compressed data, was "auroris-0.1.3.tar", last modified: Thu May 23 20:50:54 2024, max compression
```

## Comparing `auroris-0.1.2.tar` & `auroris-0.1.3.tar`

### file list

```diff
@@ -1,94 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.059462 auroris-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.047462 auroris-0.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.047462 auroris-0.1.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/ISSUE_TEMPLATE/default-template.md
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/changelog_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.051462 auroris-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-08 00:53:38.000000 auroris-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 00:53:38.000000 auroris-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-08 00:57:25.059462 auroris-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-08 00:53:38.000000 auroris-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.051462 auroris-0.1.2/auroris/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.051462 auroris-0.1.2/auroris/curation/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/curation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/curation/_curator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.051462 auroris-0.1.2/auroris/curation/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/curation/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/curation/actions/_ac_stereoisomer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/curation/actions/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/curation/actions/_deduplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/curation/actions/_discretize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/curation/actions/_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)    10842 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/curation/actions/_mol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/curation/actions/_outlier.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/curation/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.051462 auroris-0.1.2/auroris/report/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/report/_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.055462 auroris-0.1.2/auroris/report/broadcaster/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/report/broadcaster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/report/broadcaster/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/report/broadcaster/_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/report/broadcaster/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.055462 auroris-0.1.2/auroris/report/broadcaster/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/report/broadcaster/templates/report.html.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.055462 auroris-0.1.2/auroris/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/visualization/_chemspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/visualization/_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/visualization/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.059462 auroris-0.1.2/auroris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-08 00:57:24.000000 auroris-0.1.2/auroris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-08 00:57:25.000000 auroris-0.1.2/auroris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:57:24.000000 auroris-0.1.2/auroris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 00:57:24.000000 auroris-0.1.2/auroris.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-08 00:57:24.000000 auroris-0.1.2/auroris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 00:57:24.000000 auroris-0.1.2/auroris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.055462 auroris-0.1.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.055462 auroris-0.1.2/docs/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.055462 auroris-0.1.2/docs/api/actions/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/api/actions/deduplication.md
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/api/actions/discretization.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/api/actions/mol.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/api/actions/outlier_detection.md
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/api/actions/stereo_ac.md
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/api/curator.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/api/functional.md
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/api/types.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/api/visualization.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.047462 auroris-0.1.2/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.055462 auroris-0.1.2/docs/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/assets/css/custom-alchemy.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.055462 auroris-0.1.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/images/logo-black.svg
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/images/logo-white.svg
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.055462 auroris-0.1.2/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)   168635 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/tutorials/getting_started.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-08 00:53:38.000000 auroris-0.1.2/env.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-08 00:53:38.000000 auroris-0.1.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-08 00:53:38.000000 auroris-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 00:57:25.059462 auroris-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.059462 auroris-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-08 00:53:38.000000 auroris-0.1.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-08 00:53:38.000000 auroris-0.1.2/tests/test_curator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-08 00:53:38.000000 auroris-0.1.2/tests/test_deduplication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-08 00:53:38.000000 auroris-0.1.2/tests/test_discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-08 00:53:38.000000 auroris-0.1.2/tests/test_mol_curation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-08 00:53:38.000000 auroris-0.1.2/tests/test_outlier_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-08 00:53:38.000000 auroris-0.1.2/tests/test_stereoisomer_ac.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:50:54.779556 auroris-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:50:54.771556 auroris-0.1.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 20:49:14.000000 auroris-0.1.3/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-23 20:49:14.000000 auroris-0.1.3/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:50:54.771556 auroris-0.1.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-23 20:49:14.000000 auroris-0.1.3/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-23 20:49:14.000000 auroris-0.1.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-23 20:49:14.000000 auroris-0.1.3/.github/ISSUE_TEMPLATE/default-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-23 20:49:14.000000 auroris-0.1.3/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-23 20:49:14.000000 auroris-0.1.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-23 20:49:14.000000 auroris-0.1.3/.github/changelog_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:50:54.771556 auroris-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-23 20:49:14.000000 auroris-0.1.3/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-23 20:49:14.000000 auroris-0.1.3/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-23 20:49:14.000000 auroris-0.1.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-23 20:49:14.000000 auroris-0.1.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-23 20:49:14.000000 auroris-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 20:49:14.000000 auroris-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-23 20:49:14.000000 auroris-0.1.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-05-23 20:50:54.779556 auroris-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-23 20:49:14.000000 auroris-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:50:54.771556 auroris-0.1.3/auroris/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:50:54.771556 auroris-0.1.3/auroris/curation/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/curation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/curation/_curator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:50:54.775556 auroris-0.1.3/auroris/curation/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/curation/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/curation/actions/_ac_stereoisomer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/curation/actions/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/curation/actions/_deduplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/curation/actions/_discretize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/curation/actions/_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12311 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/curation/actions/_mol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/curation/actions/_outlier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/curation/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:50:54.775556 auroris-0.1.3/auroris/report/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/report/_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:50:54.775556 auroris-0.1.3/auroris/report/broadcaster/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/report/broadcaster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/report/broadcaster/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/report/broadcaster/_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/report/broadcaster/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:50:54.775556 auroris-0.1.3/auroris/report/broadcaster/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/report/broadcaster/templates/report.html.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:50:54.775556 auroris-0.1.3/auroris/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/visualization/_chemspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/visualization/_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-23 20:49:14.000000 auroris-0.1.3/auroris/visualization/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:50:54.779556 auroris-0.1.3/auroris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-05-23 20:50:54.000000 auroris-0.1.3/auroris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-23 20:50:54.000000 auroris-0.1.3/auroris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:50:54.000000 auroris-0.1.3/auroris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-23 20:50:54.000000 auroris-0.1.3/auroris.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-23 20:50:54.000000 auroris-0.1.3/auroris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 20:50:54.000000 auroris-0.1.3/auroris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:50:54.775556 auroris-0.1.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:50:54.775556 auroris-0.1.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-23 20:49:14.000000 auroris-0.1.3/docs/api/actions.md
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 20:49:14.000000 auroris-0.1.3/docs/api/curator.md
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-23 20:49:14.000000 auroris-0.1.3/docs/api/functional.md
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-23 20:49:14.000000 auroris-0.1.3/docs/api/types.md
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-23 20:49:14.000000 auroris-0.1.3/docs/api/utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-23 20:49:14.000000 auroris-0.1.3/docs/api/visualization.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:50:54.767556 auroris-0.1.3/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:50:54.775556 auroris-0.1.3/docs/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-23 20:49:14.000000 auroris-0.1.3/docs/assets/css/custom-auroris.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:50:54.779556 auroris-0.1.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-23 20:49:14.000000 auroris-0.1.3/docs/images/logo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-23 20:49:14.000000 auroris-0.1.3/docs/images/logo-white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-23 20:49:14.000000 auroris-0.1.3/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:50:54.779556 auroris-0.1.3/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    84671 2024-05-23 20:49:14.000000 auroris-0.1.3/docs/tutorials/getting_started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-23 20:49:14.000000 auroris-0.1.3/env.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-23 20:49:14.000000 auroris-0.1.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-23 20:49:14.000000 auroris-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 20:50:54.779556 auroris-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:50:54.779556 auroris-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-23 20:49:14.000000 auroris-0.1.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-23 20:49:14.000000 auroris-0.1.3/tests/test_curator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-23 20:49:14.000000 auroris-0.1.3/tests/test_deduplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-23 20:49:14.000000 auroris-0.1.3/tests/test_discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-23 20:49:14.000000 auroris-0.1.3/tests/test_mol_curation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-23 20:49:14.000000 auroris-0.1.3/tests/test_outlier_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-23 20:49:14.000000 auroris-0.1.3/tests/test_stereoisomer_ac.py
```

### Comparing `auroris-0.1.2/.github/CODE_OF_CONDUCT.md` & `auroris-0.1.3/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `auroris-0.1.2/.github/ISSUE_TEMPLATE/bug-report.yml` & `auroris-0.1.3/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `auroris-0.1.2/.github/ISSUE_TEMPLATE/default-template.md` & `auroris-0.1.3/.github/ISSUE_TEMPLATE/default-template.md`

 * *Files identical despite different names*

### Comparing `auroris-0.1.2/.github/ISSUE_TEMPLATE/feature-request.md` & `auroris-0.1.3/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `auroris-0.1.2/.github/PULL_REQUEST_TEMPLATE.md` & `auroris-0.1.3/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `auroris-0.1.2/.github/workflows/code-check.yml` & `auroris-0.1.3/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `auroris-0.1.2/.github/workflows/doc.yml` & `auroris-0.1.3/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `auroris-0.1.2/.github/workflows/release.yml` & `auroris-0.1.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `auroris-0.1.2/.github/workflows/test.yml` & `auroris-0.1.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `auroris-0.1.2/.gitignore` & `auroris-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `auroris-0.1.2/LICENSE` & `auroris-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `auroris-0.1.2/auroris/cli.py` & `auroris-0.1.3/auroris/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,38 @@
+from typing import Optional
+
 import datamol as dm
-import pandas as pd
 import typer
 
 from auroris.curation import Curator
 from auroris.report.broadcaster import HTMLBroadcaster
 
 app = typer.Typer()
 
 
 @app.command()
-def curate(config_path: str, dataset_path: str, destination: str, overwrite: bool = False):
-    # Load data
-    dataset = pd.read_csv(dataset_path)
+def curate(config_path: str, destination: str, dataset_path: Optional[str] = None, overwrite: bool = False):
+    # Create the curator
     curator = Curator.from_json(config_path)
 
+    # Overwrite the source dataset if it is set
+    if dataset_path is not None:
+        curator.src_dataset_path = dataset_path
+
     # Run curation
-    dataset, report = curator(dataset)
+    dataset, report = curator.transform()
 
     # Save dataset
     dm.fs.mkdir(destination, exist_ok=overwrite)
-    path = dm.fs.join(destination, "curated.csv")
-    dataset.to_csv(path, index=False)
+    path = dm.fs.join(destination, "curated.parquet")
+    dataset.to_parquet(path, index=False)
+
+    # Save a copy of the curation config
+    config_destination = dm.fs.join(destination, "config.json")
+    curator.to_json(config_destination)
 
     # Save report as HTML
     report_destination = dm.fs.join(destination, "report")
     broadcaster = HTMLBroadcaster(report, report_destination)
     broadcaster.broadcast()
```

### Comparing `auroris-0.1.2/auroris/curation/actions/_ac_stereoisomer.py` & `auroris-0.1.3/auroris/curation/actions/_ac_stereoisomer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,38 @@
-from typing import Dict, List, Optional
+from typing import Dict, List, Literal, Optional
 
 import datamol as dm
 import numpy as np
 import pandas as pd
+from pydantic import Field
 
 from auroris.curation.actions._base import BaseAction
 from auroris.curation.actions._outlier import modified_zscore
 from auroris.report import CurationReport
 from auroris.types import VerbosityLevel
 from auroris.utils import is_regression
 
 
 def detect_streoisomer_activity_cliff(
     dataset: pd.DataFrame,
     stereoisomer_id_col: str,
     y_cols: List[str],
-    threshold: float = 1.0,
+    threshold: float = 2.0,
     prefix: str = "AC_",
-):
+) -> pd.DataFrame:
+    """
+    Detect activity cliff among stereoisomers based on classification label or pre-defined threshold for continuous values.
+
+    Args:
+        dataset: Dataframe
+        stereoisomer_id_col: Column which identifies the stereoisomers
+        y_cols: List of columns for bioactivities
+        threshold: Threshold to identify the activity cliff. Currently, the difference of zscores between isomers are used for identification.
+        prefix: Prefix for the adding columns
+    """
     dataset_ori = dataset.copy(deep=True)
     ac_cols = {y_col: [] for y_col in y_cols}
     group_index_list = np.array(
         [group.index.values for _, group in dataset.groupby(stereoisomer_id_col, sort=False)]
     )
     for y_col in y_cols:
         is_reg = is_regression(dataset[y_col].dropna().values)
@@ -47,22 +58,31 @@
         dataset_ori.loc[rows, f"{prefix}{y_col}"] = np.array(ac_cols[y_col]).astype(bool)
 
     return dataset_ori
 
 
 class StereoIsomerACDetection(BaseAction):
     """
-    Automatic detection of outliers.
+    Automatic detection of activity shift between stereoisomers.
+
+    See [`auroris.curation.functional.detect_streoisomer_activity_cliff`][] for the docs of the
+    `stereoisomer_id_col`, `y_cols` and `threshold` attributes
+
+    Attributes:
+        mol_col: Column with the SMILES or RDKit Molecule objects.
+            If specified, will be used to render an image for the activity cliffs.
     """
 
-    stereoisomer_id_col: str
-    y_cols: List[str]
-    threshold: float = 2.0
+    name: Literal["ac_stereoisomer"] = "ac_stereoisomer"
     prefix: str = "AC_"
-    mol_col: str = "MOL_smiles"
+
+    stereoisomer_id_col: str = "MOL_molhash_id_no_stereo"
+    y_cols: List[str] = Field(default_factory=list)
+    threshold: float = 2.0
+    mol_col: Optional[str] = "MOL_smiles"
 
     def transform(
         self,
         dataset: pd.DataFrame,
         report: Optional[CurationReport] = None,
         verbosity: VerbosityLevel = VerbosityLevel.NORMAL,
         parallelized_kwargs: Optional[Dict] = None,
@@ -71,31 +91,39 @@
             dataset=dataset,
             stereoisomer_id_col=self.stereoisomer_id_col,
             y_cols=self.y_cols,
             threshold=self.threshold,
             prefix=self.prefix,
         )
 
+        # Log the following information to the report:
+        # - Newly added columns
+        # - Number of activity cliffs found
+        # - Image of the activity cliffs
+
         if report is not None:
             for col in self.y_cols:
                 col_with_prefix = self.get_column_name(col)
                 report.log_new_column(col_with_prefix)
 
-                has_cliff = dataset[col_with_prefix].notna()
+                has_cliff = dataset[col_with_prefix]
                 num_cliff = has_cliff.sum()
 
                 if num_cliff > 0:
                     report.log(
                         f"Found {num_cliff} activity cliffs among stereoisomers "
                         f"with respect to the {col} column."
                     )
-                    to_plot = dataset.loc[has_cliff, self.mol_col]
-                    legends = (col + dataset.loc[has_cliff, col].astype(str)).tolist()
 
-                    image = dm.to_image([dm.to_mol(s) for s in to_plot], legends=legends, use_svg=False)
-                    report.log_image(image)
+                    if self.mol_col is not None:
+                        to_plot = dataset.loc[has_cliff, self.mol_col]
+                        legends = (col + dataset.loc[has_cliff, col].astype(str)).tolist()
+                        image = dm.to_image([dm.to_mol(s) for s in to_plot], legends=legends, use_svg=False)
+                        report.log_image(
+                            image_or_figure=image, title="Detection of activity shifts among stereoisomers"
+                        )
 
                 else:
                     report.log(
-                        "Found no activity cliffs among stereoisomers with respect to the {col} column."
+                        f"Found no activity cliffs among stereoisomers with respect to the {col} column."
                     )
         return dataset
```

### Comparing `auroris-0.1.2/auroris/curation/actions/_base.py` & `auroris-0.1.3/auroris/curation/actions/_base.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,34 +6,32 @@
 
 from auroris.types import VerbosityLevel
 
 if TYPE_CHECKING:
     from auroris.report import CurationReport
 
 
-ACTION_REGISTRY = []
-
-
 class BaseAction(BaseModel, abc.ABC):
     """
     An action in the curation process.
 
-    Args:
-        prefix: If the action adds columns, use this prefix.
-        completed: If the action has completed.
-        dep_action: Name of dependent action.
+    Info: The importance of reproducibility
+        One of the main goals in designing `auroris` is to make it easy to reproduce the curation process.
+        Reproducibility is key to scientific research. This is why a BaseAction needs to be serializable and
+        uniquely identified by a `name`.
+
+    Attributes:
+        name: The name that uniquely identifies the action. This is used to serialize and deserialize the action.
+        prefix: This prefix is used when an action adds columns to a dataset.
+            If not set, it defaults to the name in uppercase.
     """
 
+    name: str
     prefix: str = None
 
-    @property
-    def name(self) -> str:
-        """The name of the action. Needs to be unique."""
-        return self.__class__.__name__
-
     @model_validator(mode="after")
     @classmethod
     def _validate_model(cls, m: "BaseAction"):
         if m.prefix is None:
             m.prefix = m.name.upper() + "_"
         return m
 
@@ -48,11 +46,7 @@
         verbosity: VerbosityLevel = VerbosityLevel.NORMAL,
         parallelized_kwargs: Optional[Dict] = None,
     ):
         raise NotImplementedError
 
     def __call__(self, dataset: pd.DataFrame):
         return self.transform(dataset)
-
-    def __init_subclass__(cls, **kwargs):
-        super().__init_subclass__(**kwargs)
-        ACTION_REGISTRY.append(cls)
```

### Comparing `auroris-0.1.2/auroris/curation/actions/_deduplicate.py` & `auroris-0.1.3/auroris/curation/actions/_deduplicate.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,28 +49,37 @@
     merged_df = merged_df.drop_duplicates(subset=deduplicate_on, keep=keep).reset_index(drop=True)
     return merged_df
 
 
 class Deduplication(BaseAction):
     """
     Automatic detection of outliers.
+
+    See [`auroris.curation.functional.deduplicate`][] for the docs of the
+    `deduplicate_on`, `y_cols`, `keep` and `method` attributes
     """
 
+    name: Literal["deduplicate"] = "deduplicate"
+
     deduplicate_on: Optional[Union[str, List[str]]] = None
     y_cols: Optional[Union[str, List[str]]] = None
     keep: Literal["first", "last"] = "first"
     method: Literal["mean", "median"] = "median"
 
     def transform(
         self,
         dataset: pd.DataFrame,
         report: Optional[CurationReport] = None,
         verbosity: VerbosityLevel = VerbosityLevel.NORMAL,
         parallelized_kwargs: Optional[Dict] = None,
     ):
-        return deduplicate(
+        dataset_dedup = deduplicate(
             dataset,
             deduplicate_on=self.deduplicate_on,
             y_cols=self.y_cols,
             keep=self.keep,
             method=self.method,
         )
+        if report is not None:
+            num_duplicates = len(dataset) - len(dataset_dedup)
+            report.log(f"Deduplication merged and removed {num_duplicates} duplicated molecules from dataset")
+        return dataset_dedup
```

### Comparing `auroris-0.1.2/auroris/curation/actions/_discretize.py` & `auroris-0.1.3/auroris/curation/actions/_discretize.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 def discretize(
     X: np.ndarray,
     thresholds: Union[np.ndarray, list],
     inplace: bool = False,
     allow_nan: bool = True,
     label_order: Literal["ascending", "descending"] = "ascending",
 ) -> np.ndarray:
-    """Thresholding of array-like or scipy.sparse matrix into binary or multiclass labels.
+    """
+    Thresholding of array-like or scipy.sparse matrix into binary or multiclass labels.
 
     Args:
         X : The data to discretize, element by element.
             scipy.sparse matrices should be in CSR or CSC format to avoid an
             un-necessary copy.
 
         thresholds: Interval boundaries that include the right bin edge.
@@ -72,21 +73,35 @@
         X[nan_idx] = np.nan
     if binarize and label_order == "descending":
         X = 1 - X
     return X
 
 
 class Discretization(BaseAction):
-    input_column: str
+    """
+    Thresholding bioactivity columns to binary or multiclass labels.
+
+    See [`auroris.curation.functional.discretize`][] for the docs of the
+    `thresholds`, `inplace`, `allow_nan` and `label_order` attributes
+
+    Attributes:
+        input_column: The column to discretize.
+        log_scale: Whether a visual depiction of the discretization should be on a log scale.
+    """
+
+    name: Literal["discretize"] = "discretize"
     prefix: str = "CLS_"
+
+    input_column: str
     thresholds: List[float]
+
     inplace: bool = False
     allow_nan: bool = True
     label_order: Literal["ascending", "descending"] = "ascending"
-    log_scale: bool = True
+    log_scale: bool = False
 
     def transform(
         self,
         dataset: pd.DataFrame,
         report: Optional[CurationReport] = None,
         verbosity: VerbosityLevel = VerbosityLevel.NORMAL,
         parallelized_kwargs: Optional[Dict] = None,
```

### Comparing `auroris-0.1.2/auroris/curation/actions/_mol.py` & `auroris-0.1.3/auroris/curation/actions/_mol.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,47 @@
 from functools import partial
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Dict, List, Literal, Optional, Tuple, Union
 
 import datamol as dm
 import numpy as np
 import pandas as pd
 from rdkit.Chem import FindMolChiralCenters
 
 from auroris.curation.actions._base import BaseAction
 from auroris.report import CurationReport
 from auroris.types import VerbosityLevel
 from auroris.visualization import visualize_chemspace
+from auroris.visualization.utils import create_figure
 
 
 def curate_molecules(
     mols: List[Union[str, dm.Mol]],
     progress: bool = True,
     remove_salt_solvent: bool = True,
     remove_stereo: bool = False,
     count_stereoisomers: bool = True,
     count_stereocenters: bool = True,
     **parallelized_kwargs,
-):
+) -> Tuple:
+    """
+    Curate a list of molecules.
+
+    Args:
+        mols: List of molecules.
+        progress: Whether show curation progress.
+        remove_salt_solvent: Whether remove salt and solvent from molecule.
+        remove_stereo: Whether remove stereo chemistry information from molecule.
+        count_stereoisomers: Whether count the number of stereoisomers of molecule.
+        count_stereocenters: Whether count the number of stereocenters of molecule.
+
+    Returns:
+        mol_dict: Dictionary of molecule and additional metadata
+        num_invalid: Number of invßßalid molecules
+
+    """
     fn = partial(
         _curate_molecule,
         remove_salt_solvent=remove_salt_solvent,
         remove_stereo=remove_stereo,
         count_stereoisomers=count_stereoisomers,
         count_stereocenters=count_stereocenters,
     )
@@ -182,18 +199,19 @@
         "num_stereo_center": num_stereo_center,
         "undefined_E_D": undefined_E_D,
         "undefined_E/Z": undefined_E_Z,
     }
 
 
 def _num_stereo_centers(mol: dm.Mol) -> Tuple[int]:
-    """Get the number of defined and undefined stereo centers of a given molecule
-        by accessing the all and only defined stereo centers.
-        It's to facilitate the analysis of the stereo isomers.
-        None will be return if there is no stereo centers in the molecule.
+    """
+    Get the number of defined and undefined stereo centers of a given molecule
+    by accessing the all and only defined stereo centers.
+    It's to facilitate the analysis of the stereo isomers.
+    None will be return if there is no stereo centers in the molecule.
 
      Args:
          mol: Molecule
 
     Returns:
         nun_defined_centers: Number of defined stereo centers.
         nun_undefined_centers: Number of undefined stereo centers.
@@ -209,39 +227,46 @@
     num_defined_centers = len(FindMolChiralCenters(mol, force=True, includeUnassigned=False))
     nun_undefined_centers = num_all_centers - num_defined_centers
     return num_all_centers, num_defined_centers, nun_undefined_centers
 
 
 class MoleculeCuration(BaseAction):
     """
+    Automated molecule curation and chemistry space distribution.
+
+    See [`auroris.curation.functional.curate_molecules`][] for the docs of the
+    `remove_salt_solvent`, `remove_stereo`, `count_stereoisomers`, and `count_stereocenters` attributes
+
     Attributes:
         input_column: The name of the column that has the molecules (either `dm.Mol` objects or SMILES).
-        remove_salt_solvent: When set to 'True', all disconnected salts and solvents
-            will be removed from molecule. In most of the cases, it is recommended to remove the salts/solvents.
-        remove_stereo: Whether remove stereochemistry information from molecule.
-            If it's known that the stereochemistry do not contribute to the bioactivity of interest,
-            the stereochemistry information can be removed.
+        X_col: Column with custom features for each of the molecules. If None, will use ECFP.
+        y_cols: Column names for bioactivities, which will be used to colorcode the chemical space visualization.
     """
 
-    input_column: str
+    name: Literal["mol_curation"] = "mol_curation"
     prefix: str = "MOL_"
+
+    input_column: str
     remove_salt_solvent: bool = True
     remove_stereo: bool = False
     count_stereoisomers: bool = True
     count_stereocenters: bool = True
 
+    X_col: Optional[str] = None
+    y_cols: Optional[Union[str, List[str]]] = None
+
     def transform(
         self,
         dataset: pd.DataFrame,
         report: Optional[CurationReport] = None,
         verbosity: VerbosityLevel = VerbosityLevel.NORMAL,
         parallelized_kwargs: Optional[Dict] = None,
     ) -> pd.DataFrame:
+        # Run the curation
         mols = dataset[self.input_column].values
-
         parallelized_kwargs = parallelized_kwargs or {}
         mol_dict, num_invalid = curate_molecules(
             mols,
             progress=verbosity > 1,
             remove_salt_solvent=self.remove_salt_solvent,
             remove_stereo=self.remove_stereo,
             count_stereoisomers=self.count_stereoisomers,
@@ -253,48 +278,63 @@
 
         if num_invalid > 0:
             if report is not None:
                 report.log(f"Couldn't preprocess {num_invalid} / {len(dataset)} molecules.")
 
         dataset = pd.concat([dataset, df], axis=1)
 
+        # Log information to the report
+        # - New columns with the curated molecule information
+
         if report is not None:
             for col in df.columns:
                 report.log_new_column(col)
 
             smiles_col = self.get_column_name("smiles")
             smiles = dataset[smiles_col].dropna().values
 
-            with dm.without_rdkit_log():
-                # Temporary disable logs because of deprecation warning
-                X = np.array([dm.to_fp(smi) for smi in smiles])
+            if self.X_col is None:
+                featurizer = "ECFP"
+                with dm.without_rdkit_log():
+                    X = np.array([dm.to_fp(smi) for smi in smiles])
+                report.log("Default `ecfp` fingerprint is used to visualize the chemical space.")
+
+            else:
+                featurizer = self.X_col
+                X = dataset[self.X_col].values
+
+            # list of data per column
+            y = dataset[self.y_cols].T.values.tolist() if self.y_cols else None
 
-            fig = visualize_chemspace(X=X)
-            report.log_image(fig, "Distribution in Chemical Space")
+            fig = visualize_chemspace(X=X, y=y, labels=self.y_cols)
+            report.log_image(fig, title=f"Distribution in Chemical Space - {featurizer}")
 
             if self.count_stereocenters:
                 # Plot all compounds with undefined stereocenters for visual inspection
-
                 undefined_col = self.get_column_name("num_undefined_stereo_center")
                 defined_col = self.get_column_name("num_defined_stereo_center")
 
                 to_plot = dataset.query(f"{undefined_col} > 0 ")
                 num_mol_undefined = to_plot.shape[0]
                 report.log(f"Molecules with undefined stereocenter detected: {num_mol_undefined}.")
 
                 if num_mol_undefined > 0:
                     legends = []
                     for _, row in to_plot.iterrows():
                         undefined = row[undefined_col]
                         defined = row[defined_col]
                         legends.append(f"Undefined:{undefined}\n Definded:{defined}")
 
-                    image = dm.to_image(to_plot[smiles_col].tolist(), legends=legends, use_svg=False)
+                    with create_figure(n_plots=1, n_cols=1) as (image, _):
+                        dm.to_image(
+                            to_plot[smiles_col].tolist(), legends=legends, use_svg=False, returnPNG=True
+                        )
+
                     report.log_image(
                         image,
                         title="Molecules with undefined stereocenters",
-                        description=f"There are {num_mol_undefined} molecules with undefined stereocenter(s)."
-                        f"It's recommanded to use <auroris.curaion.action.StereoIsomerACDetection> and"
-                        f"check the stereoisomers and activity cliffs in the dataset.",
+                        description=f"There are {num_mol_undefined} molecules with undefined stereocenter(s). "
+                        "It's recommended to use <auroris.curation.action.StereoIsomerACDetection> and "
+                        "check the stereoisomers and activity cliffs in the dataset.",
                     )
 
         return dataset
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `auroris-0.1.2/auroris/curation/actions/_outlier.py` & `auroris-0.1.3/auroris/curation/actions/_outlier.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,60 +14,14 @@
 from auroris.report import CurationReport
 from auroris.types import VerbosityLevel
 from auroris.visualization import visualize_distribution_with_outliers
 
 OutlierDetectionMethod: TypeAlias = Literal["iso", "lof", "svm", "ee", "zscore"]
 
 
-def detect_outliers(X: np.ndarray, method: OutlierDetectionMethod = "zscore", **kwargs: Any):
-    """Functional interface for detecting outliers
-
-    Args:
-        X: The observations that we want to classify as inliers or outliers.
-        method: The method to use for outlier detection.
-        **kwargs: Keyword arguments for the outlier detection method.
-    """
-
-    if X.ndim != 1:
-        raise ValueError("X must be a 1D array for outlier detection.")
-
-    detector_cls = _OUTLIER_METHODS[method]
-    detector = detector_cls(**kwargs)
-    indices = np.flatnonzero(~np.isnan(X))
-
-    in_ = X[indices].reshape(-1, 1)
-    out_ = detector.fit_predict(in_)
-
-    is_inlier = np.full_like(X, np.nan)
-    is_inlier[indices] = out_.flatten()
-
-    is_outlier = is_inlier == -1
-    return is_outlier
-
-
-def modified_zscore(data: np.ndarray, consistency_correction: float = 1.4826):
-    """
-    The modified z score is calculated from the median absolute deviation (MAD).
-    These values must be multiplied by a constant to approximate the standard deviation.
-
-    The modified z score might be more robust than the standard z score because it relies
-    on the median (MED) for calculating the z score.
-
-    modified Z score = (X-MED) / (consistency_correction*MAD)
-
-    """
-    median = np.nanmedian(data)
-
-    deviation_from_med = np.array(data) - median
-
-    mad = np.nanmedian(np.abs(deviation_from_med))
-    mod_zscore = deviation_from_med / (consistency_correction * mad)
-    return mod_zscore
-
-
 class ZscoreOutlier(OutlierMixin):
     """
     Detect outliers by the absolute value of the Z-score.
 
     Uses a scikit-learn compatible interface.
 
     Args:
@@ -118,22 +72,85 @@
         Args:
             X: The observations that we want to classify as inliers or outliers.
         """
         self.fit(X)
         return self.predict(X)
 
 
+_OUTLIER_METHODS: Dict[OutlierDetectionMethod, OutlierMixin] = {
+    "iso": IsolationForest,
+    "lof": LocalOutlierFactor,
+    "svm": OneClassSVM,
+    "ee": EllipticEnvelope,
+    "zscore": ZscoreOutlier,
+}
+
+
+def detect_outliers(X: np.ndarray, method: OutlierDetectionMethod = "zscore", **kwargs: Any):
+    """Functional interface for detecting outliers
+
+    Args:
+        X: The observations that we want to classify as inliers or outliers.
+        method: The method to use for outlier detection.
+        **kwargs: Keyword arguments for the outlier detection method.
+    """
+
+    if X.ndim != 1:
+        raise ValueError("X must be a 1D array for outlier detection.")
+
+    detector_cls = _OUTLIER_METHODS[method]
+    detector = detector_cls(**kwargs)
+    indices = np.flatnonzero(~np.isnan(X))
+
+    in_ = X[indices].reshape(-1, 1)
+    out_ = detector.fit_predict(in_)
+
+    is_inlier = np.full_like(X, np.nan)
+    is_inlier[indices] = out_.flatten()
+
+    is_outlier = is_inlier == -1
+    return is_outlier
+
+
+def modified_zscore(data: np.ndarray, consistency_correction: float = 1.4826):
+    """
+    The modified z score is calculated from the median absolute deviation (MAD).
+    These values must be multiplied by a constant to approximate the standard deviation.
+
+    The modified z score might be more robust than the standard z score because it relies
+    on the median (MED) for calculating the z score.
+
+    modified Z score = (X-MED) / (consistency_correction*MAD)
+
+    """
+    median = np.nanmedian(data)
+
+    deviation_from_med = np.array(data) - median
+
+    mad = np.nanmedian(np.abs(deviation_from_med))
+    mod_zscore = deviation_from_med / (consistency_correction * mad)
+    return mod_zscore
+
+
 class OutlierDetection(BaseAction):
     """
     Automatic detection of outliers.
+
+    See [`auroris.curation.functional.detect_outliers`][] for the docs of the
+    `method` and `kwargs` attributes
+
+    Attributes:
+        columns: The columns for which to detect outliers.
     """
 
-    method: OutlierDetectionMethod
-    columns: List[str]
-    prefix: str = "OUTLIER_"
+    name: Literal["outlier_detection"] = "outlier_detection"
+    prefix: str = Field(default="OUTLIER_", description="Prefix for added column names.")
+
+    method: OutlierDetectionMethod = Field(..., description="Method name for outlier detection.")
+    columns: List[str] = Field(..., description="Column names to detect outliers.")
     kwargs: Dict = Field(default_factory=dict)
 
     def transform(
         self,
         dataset: pd.DataFrame,
         report: Optional[CurationReport] = None,
         verbosity: VerbosityLevel = VerbosityLevel.NORMAL,
@@ -141,24 +158,21 @@
     ):
         for column in self.columns:
             values = dataset[column].values
             is_outlier = detect_outliers(values, self.method, **self.kwargs)
 
             is_outlier_col_label = self.get_column_name(column)
             dataset[is_outlier_col_label] = is_outlier
+            num_outliers = sum(is_outlier)
 
             if report is not None:
                 report.log_new_column(is_outlier_col_label)
-
-                fig = visualize_distribution_with_outliers(values=values, is_outlier=is_outlier)
-                report.log_image(fig)
+                report.log(
+                    f"Found {num_outliers} potential outliers "
+                    f"with respect to the {column} column for review."
+                )
+                fig = visualize_distribution_with_outliers(
+                    values=values, is_outlier=is_outlier, title=f"Probability Plot - {column}"
+                )
+                report.log_image(fig, title=f"Outlier detection - {column}")
 
         return dataset
-
-
-_OUTLIER_METHODS: Dict[OutlierDetectionMethod, OutlierMixin] = {
-    "iso": IsolationForest,
-    "lof": LocalOutlierFactor,
-    "svm": OneClassSVM,
-    "ee": EllipticEnvelope,
-    "zscore": ZscoreOutlier,
-}
```

### Comparing `auroris-0.1.2/auroris/report/_report.py` & `auroris-0.1.3/auroris/report/_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from matplotlib import pyplot as plt
 from matplotlib.figure import Figure
 from PIL.Image import Image as ImageType
 from pydantic import BaseModel, ConfigDict, Field, PrivateAttr
 
 from auroris import __version__
-from auroris.utils import fig2img
+from auroris.utils import bytes2img, fig2img
 
 
 class AnnotatedImage(BaseModel):
     """
     Image data, potentially with a title and / or description.
     """
 
@@ -76,14 +76,16 @@
         description: Optional[str] = None,
     ):
         """Logs an image. Also accepts Matplotlib figures, which will be converted to images."""
         self._check_active_section()
         if isinstance(image_or_figure, Figure):
             image = fig2img(image_or_figure)
             plt.close(image_or_figure)
+        elif isinstance(image_or_figure, ByteString):
+            image = bytes2img(image_or_figure)
         else:
             image = image_or_figure
 
         image = AnnotatedImage(image=image, title=title, description=description)
         self._active_section.images.append(image)
 
     def _check_active_section(self):
```

### Comparing `auroris-0.1.2/auroris/report/broadcaster/_logger.py` & `auroris-0.1.3/auroris/report/broadcaster/_logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 
 class LoggerBroadcaster(ReportBroadcaster):
     """Simple broadcaster for debugging that will simply write to the terminal"""
 
     def __init__(self, report: CurationReport):
         super().__init__(report)
-        self.logger = logging.getLogger()
+        self.logger = logging.getLogger(self.__class__.__name__)
         self.logger.setLevel(logging.DEBUG)
 
         handler = logging.StreamHandler(sys.stdout)
         handler.setFormatter(ColoredFormatter())
 
         for handler in self.logger.handlers:
             self.logger.removeHandler(handler)
@@ -47,14 +47,15 @@
         self.on_report_start(self._report)
         for section in self._report.sections:
             self.on_section_start(section)
             for log in section.logs:
                 self.render_log(log)
             for image in section.images:
                 self.render_image(image)
+        self.on_report_end(self._report)
 
     def render_log(self, message: str):
         self.logger.debug(f"[LOG]: {message}")
 
     def render_image(self, image: AnnotatedImage):
         width, height = image.image.size
         self.logger.debug(f"[IMG]: Dimensions {width} x {height}")
@@ -62,7 +63,10 @@
     def on_section_start(self, section: Section):
         self.logger.info(f"===== {section.title} =====")
 
     def on_report_start(self, report: CurationReport):
         self.logger.critical("===== Curation Report =====")
         self.logger.debug(f"Time: {report.time_stamp.strftime('%Y-%m-%d %H:%M:%S')}")
         self.logger.debug(f"Version: {report.auroris_version}")
+
+    def on_report_end(self, report: CurationReport):
+        self.logger.critical("===== Curation Report END =====")
```

### Comparing `auroris-0.1.2/auroris/report/broadcaster/templates/report.html.jinja` & `auroris-0.1.3/auroris/report/broadcaster/templates/report.html.jinja`

 * *Files identical despite different names*

### Comparing `auroris-0.1.2/auroris/visualization/_chemspace.py` & `auroris-0.1.3/auroris/visualization/_chemspace.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,67 +8,68 @@
 try:
     import umap  # type: ignore
 except ImportError:
     umap = None
 
 
 def visualize_chemspace(
-    X: Union[List[np.ndarray], np.ndarray],
+    X: np.ndarray,
     y: Optional[Union[List[np.ndarray], np.ndarray]] = None,
     labels: Optional[List[str]] = None,
-    n_cols: int = 3,
+    n_cols: int = 2,
     fig_base_size: float = 8,
     w_h_ratio: float = 0.5,
     dpi: int = 150,
     seaborn_theme: Optional[str] = "whitegrid",
     **umap_kwargs: Any,
 ):
-    """Plot the chemical space. Also, color based on the target values.
+    """Plot the coverage in chemical space. Also, color based on the target values.
 
     Args:
-        X: A list of arrays with the features.
+        X: Array the molecular features.
         y: A list of arrays with the target values.
         labels: Optional list of labels for each set of features.
         n_cols: Number of columns in the subplots.
         fig_base_size: Base size of the plots.
         w_h_ratio: Width/height ratio.
         dpi: DPI value of the figure.
         seaborn_theme: Seaborn theme.
         **umap_kwargs: Keyword arguments for the UMAP algorithm.
     """
 
     if umap is None:
         raise ImportError("Please run `pip install umap-learn` to use UMAP visualizations for the chemspace.")
 
-    if isinstance(X, np.ndarray):
-        X = [X]
     if isinstance(y, np.ndarray):
         y = [y]
+
     if y is None:
-        y = [None for _ in range(len(X))]
-    if len(X) != len(y):
-        raise ValueError("X and y must have the same length.")
+        y = [None]
 
     if labels is None:
-        labels = ["" for i in range(len(X))]
+        labels = ["" for _ in range(len(y))]
+
+    if len(y) != len(labels):
+        raise ValueError("`labels` and `y` must have the same length.")
+
+    embedding = umap.UMAP(**umap_kwargs).fit_transform(X)
+    umap_0, umap_1 = embedding[:, 0], embedding[:, 1]
 
     with create_figure(
-        n_plots=len(X),
+        n_plots=len(y),
         n_cols=n_cols,
         fig_base_size=fig_base_size,
         w_h_ratio=w_h_ratio,
         dpi=dpi,
         seaborn_theme=seaborn_theme,
     ) as (fig, axes):
-        for idx, (X_i, y_i, label) in enumerate(zip(X, y, labels)):
-            embedding = umap.UMAP(**umap_kwargs).fit_transform(X_i)
-            umap_0, umap_1 = embedding[:, 0], embedding[:, 1]
-
+        for idx, (y_i, label) in enumerate(zip(y, labels)):
             ax = sns.scatterplot(
                 x=umap_0,
                 y=umap_1,
                 hue=y_i,
                 ax=axes[idx],
             )
+            ax.set_xlabel("Component 0")
+            ax.set_xlabel("Component 1")
             ax.set_title(label)
-
     return fig
```

### Comparing `auroris-0.1.2/auroris/visualization/_distribution.py` & `auroris-0.1.3/auroris/visualization/_distribution.py`

 * *Files 21% similar despite different names*

```diff
@@ -38,19 +38,19 @@
     ylim = ax.get_ylim()
 
     # Color the area under the KDE curve in accordance with the bins
     # Also added a vertical dashed line for each bin boundary
     for threshold in bins:
         if log_scale and lower != -np.inf:
             lower = np.log(lower)
+
         if log_scale and threshold != np.inf:
             threshold = np.log(threshold)
 
         mask = (xs > lower) & (xs <= threshold)
-        lower = threshold
 
         # Update xs to make sure they cover the range even if the
         # coordinates don't fully cover it
         masked_xs = xs[mask]
 
         if len(masked_xs) == 0:
             continue
@@ -71,40 +71,57 @@
 
         label = f"{_format(lower)}, {_format(threshold)}"
         label = f"({label})" if threshold == np.inf else f"({label}]"
         label += f" - {pct:.2%}"
 
         ax.fill_between(masked_xs, ys[mask], alpha=0.5, label=label)
         ax.plot([threshold, threshold], [ylim[0], ys[mask][-1]], "k--")
+        lower = threshold
 
     ax.legend()
     return fig
 
 
 def visualize_distribution_with_outliers(
-    values: np.ndarray,
-    is_outlier: Optional[List[bool]] = None,
+    values: np.ndarray, is_outlier: Optional[List[bool]] = None, title: str = "Probability Plot"
 ):
-    """Visualize the distribution of the data and highlight the potential outliers."""
+    """
+    Visualize the distribution of the data and highlight the potential outliers.
+
+    Args:
+        values: Values for visulization.
+        is_outlier: List of outlier flag.
+        title: Title of plot
+
+    """
 
     if is_outlier is None:
         # Import here to prevent ciruclar imports
         from auroris.curation.functional import detect_outliers
 
         is_outlier = detect_outliers(values)
 
     # sort both value and outlier indicator
     sorted_ind = np.argsort(values)
     values = values[sorted_ind]
     is_outlier = is_outlier[sorted_ind]
 
-    with create_figure(n_plots=2) as (fig, axes):
-        sns.scatterplot(
-            x=np.arange(len(values)),
-            y=values,
-            hue=is_outlier,
-            palette={1.0: "red", 0.0: "navy", 0.5: "grey"},
-            ax=axes[0],
-        )
-        stats.probplot(values, dist="norm", plot=axes[1])
+    with create_figure(n_plots=1) as (fig, axes):
+        res = stats.probplot(values, dist="norm", fit=True, plot=axes[0])
+        x = res[0][0]
+        y = res[0][1]
+
+        # Specify the indices of data points to highlight
+        highlight_indices = np.argwhere(is_outlier.__eq__(True)).flatten()
+        highlight_color = "red"
+
+        # Overlay specific points with different colors
+        for idx in highlight_indices:
+            axes[0].plot(
+                x[idx], y[idx], marker="o", markersize=8, color=highlight_color
+            )  # Red circles for highlighted points
+
+        axes[0].set_xlabel("Theoretical quantiles")
+        axes[0].set_ylabel("Ordered Values")
+        axes[0].set_title(title)
 
     return fig
```

### Comparing `auroris-0.1.2/auroris/visualization/utils.py` & `auroris-0.1.3/auroris/visualization/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     n_plots: int,
     n_cols: Optional[int] = None,
     fig_base_size: float = 8,
     w_h_ratio: float = 0.5,
     dpi: int = 150,
     seaborn_theme: Optional[str] = "whitegrid",
 ):
-    """Creates a figure with the desired size"""
+    """Creates a figure with the desired size and layout"""
 
     if seaborn_theme is not None:
         sns.set_theme(style=seaborn_theme)
 
     if n_cols is None or n_cols > n_plots:
         n_cols = n_plots
```

### Comparing `auroris-0.1.2/auroris.egg-info/SOURCES.txt` & `auroris-0.1.3/auroris.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .gitignore
 LICENSE
+NOTICE
 README.md
 env.yml
 mkdocs.yml
 pyproject.toml
 .github/CODEOWNERS
 .github/CODE_OF_CONDUCT.md
 .github/PULL_REQUEST_TEMPLATE.md
@@ -46,24 +47,21 @@
 auroris/report/broadcaster/_logger.py
 auroris/report/broadcaster/templates/report.html.jinja
 auroris/visualization/__init__.py
 auroris/visualization/_chemspace.py
 auroris/visualization/_distribution.py
 auroris/visualization/utils.py
 docs/index.md
+docs/api/actions.md
 docs/api/curator.md
 docs/api/functional.md
 docs/api/types.md
+docs/api/utils.md
 docs/api/visualization.md
-docs/api/actions/deduplication.md
-docs/api/actions/discretization.md
-docs/api/actions/mol.md
-docs/api/actions/outlier_detection.md
-docs/api/actions/stereo_ac.md
-docs/assets/css/custom-alchemy.css
+docs/assets/css/custom-auroris.css
 docs/images/logo-black.svg
 docs/images/logo-white.svg
 docs/tutorials/getting_started.ipynb
 tests/conftest.py
 tests/test_curator.py
 tests/test_deduplication.py
 tests/test_discretization.py
```

### Comparing `auroris-0.1.2/docs/assets/css/custom-alchemy.css` & `auroris-0.1.3/docs/assets/css/custom-auroris.css`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 :root {
 
   /*
   For a list of all available variables, see
   https://github.com/squidfunk/mkdocs-material/blob/master/src/assets/stylesheets/main/_colors.scss
   */
-  --polaris-primary:    hsla(236, 100%, 19%, 1.0);
-  --polaris-secondary: hsla(290, 61%, 43%, 1.0);
-  --polaris-ternary: hsla(236, 100%, 9%, 1.0);
+  --auroris-primary:    rgb(36, 82, 97);
+  --auroris-secondary: rgb(70, 201, 190);
+  --auroris-ternary: rgb(0, 61, 94);
 }
 
 /* Change the header background to use a gradient */
 .md-header {
-  background-image: linear-gradient(to right, var(--polaris-secondary), var(--polaris-primary));
+  background-image: linear-gradient(to right, var(--auroris-secondary), var(--auroris-primary));
 }
 
 /* Change the footer background to use a gradient */
 .md-footer {
-  background-image: linear-gradient(to right, var(--polaris-primary), var(--polaris-ternary));
+  background-image: linear-gradient(to right, var(--auroris-primary), var(--auroris-ternary));
 }
 
 /* Change the tabs background to use a gradient */
 .md-tabs {
-  background-image: linear-gradient(to right, #F4F6F9, #dfc3e2);
-  color: var(--polaris-ternary);
+  background-image: linear-gradient(to right, #F4F6F9, #d7f2c3);
+  color: var(--auroris-ternary);
 }
 
 /* Remove the `In` and `Out` block in rendered Jupyter notebooks */
 .md-container .jp-Cell-outputWrapper .jp-OutputPrompt.jp-OutputArea-prompt,
 .md-container .jp-Cell-inputWrapper .jp-InputPrompt.jp-InputArea-prompt {
   display: none !important;
 }
```

### Comparing `auroris-0.1.2/env.yml` & `auroris-0.1.3/env.yml`

 * *Files 21% similar despite different names*

```diff
@@ -6,14 +6,15 @@
   - pip
   - tqdm
   - loguru
   - typer
   - pydantic >=2
   - fsspec
   - pillow
+  - pyarrow
 
   # Scientific
   - numpy
   - pandas < 2.2.0
   - scipy
   - scikit-learn
   - seaborn
@@ -40,8 +41,8 @@
   - mkdocs-material >=9.4.7
   - mkdocstrings
   - mkdocstrings-python
   - mkdocs-jupyter
   - markdown-include
   - mdx_truly_sane_lists
   - nbconvert
-  - mike >=1.0.0
+  - mike >=1.0.0
```

### Comparing `auroris-0.1.2/mkdocs.yml` & `auroris-0.1.3/mkdocs.yml`

 * *Files 7% similar despite different names*

```diff
@@ -14,24 +14,23 @@
 
 nav:
   - Getting started:
       - Auroris: index.md
   - Tutorials:
       - Getting Started: tutorials/getting_started.ipynb
   - API Reference:
-      - Curator: api/curator.md
-      - Actions: 
-          - Deduplication: api/actions/deduplication.md
-          - Discretization: api/actions/discretization.md
-          - Molecule Curation: api/actions/mol.md
-          - Outlier Detection: api/actions/outlier_detection.md
-          - Stereoisomer AC: api/actions/stereo_ac.md
-      - Functional: api/functional.md
-      - Visualization: api/visualization.md
-      - Types: api/types.md
+      - Core: 
+        - Curator: api/curator.md
+        - Actions: api/actions.md
+      - Functional API:
+        - Curation: api/functional.md
+        - Visualization: api/visualization.md
+      - Misc: 
+        - Types: api/types.md
+        - Utils: api/utils.md
   - Community: https://discord.gg/vBFd8p6H7u
   - Polaris Hub: https://polarishub.io/
 
 theme:
   name: material
   palette:
     primary: deep purple
```

### Comparing `auroris-0.1.2/pyproject.toml` & `auroris-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     "pandas < 2.2.0",
     "scipy",
     "scikit-learn",
     "seaborn",
     "datamol >=0.12.1",
     "pillow",
     "fsspec",
+    "pyarrow",
 ]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "pytest-xdist",
     "pytest-cov",
```

### Comparing `auroris-0.1.2/tests/test_curator.py` & `auroris-0.1.3/tests/test_curator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import os
 
+from pandas.core.api import DataFrame as DataFrame
+
 from auroris.curation import Curator
 from auroris.curation.actions import Discretization, MoleculeCuration, OutlierDetection
 from auroris.report.broadcaster import HTMLBroadcaster, LoggerBroadcaster
 
 try:
     import jinja2
 except ImportError:
     jinja2 = None
 
 
 def test_curator_save_load(tmpdir):
     curator = Curator(
         steps=[
-            OutlierDetection(method="zscore", columns=["outlier_column"]),
             MoleculeCuration(input_column="smiles"),
+            OutlierDetection(method="zscore", columns=["outlier_column"]),
         ],
     )
     path = os.path.join(tmpdir, "curator.json")
     curator.to_json(path)
-    curator.from_json(path)
+    curator_reload = curator.from_json(path)
+
+    assert len(curator.steps) == len(curator_reload.steps)
+    for step1, step2 in zip(curator.steps, curator_reload.steps):
+        assert step1 == step2
 
-    assert len(curator.steps) == 2
-    assert curator.steps[0].method == "zscore"
-    assert curator.steps[0].columns == ["outlier_column"]
+    assert curator.steps[1].method == "zscore"
+    assert curator.steps[1].columns == ["outlier_column"]
 
 
 def test_curator_integration(dataset, tmpdir):
     curator = Curator(
         steps=[
             OutlierDetection(method="zscore", columns=["outlier_column"]),
             MoleculeCuration(input_column="smiles"),
```

### Comparing `auroris-0.1.2/tests/test_deduplication.py` & `auroris-0.1.3/tests/test_deduplication.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.2/tests/test_discretization.py` & `auroris-0.1.3/tests/test_discretization.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.2/tests/test_mol_curation.py` & `auroris-0.1.3/tests/test_mol_curation.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.2/tests/test_outlier_detection.py` & `auroris-0.1.3/tests/test_outlier_detection.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.2/tests/test_stereoisomer_ac.py` & `auroris-0.1.3/tests/test_stereoisomer_ac.py`

 * *Files identical despite different names*

