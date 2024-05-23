# Comparing `tmp/wagtail_cblocks-0.4.1.tar.gz` & `tmp/wagtail_cblocks-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_cblocks-0.4.1.tar", last modified: Thu May  4 14:02:30 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `wagtail_cblocks-0.4.1.tar` & `wagtail_cblocks-0.4.2.tar`

### file list

```diff
@@ -1,64 +1,38 @@
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.253506 wagtail_cblocks-0.4.1/
--rw-r--r--   0 jerome    (1000) jerome    (1000)      319 2021-03-04 09:52:17.000000 wagtail_cblocks-0.4.1/.editorconfig
--rw-r--r--   0 jerome    (1000) jerome    (1000)      263 2022-03-09 15:21:21.000000 wagtail_cblocks-0.4.1/.gitignore
--rw-r--r--   0 jerome    (1000) jerome    (1000)      784 2023-05-04 13:28:04.000000 wagtail_cblocks-0.4.1/.gitlab-ci.yml
--rw-r--r--   0 jerome    (1000) jerome    (1000)      607 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 jerome    (1000) jerome    (1000)     2328 2023-05-04 14:01:36.000000 wagtail_cblocks-0.4.1/CHANGELOG.md
--rw-r--r--   0 jerome    (1000) jerome    (1000)    35149 2021-03-04 09:51:01.000000 wagtail_cblocks-0.4.1/LICENSE
--rw-r--r--   0 jerome    (1000) jerome    (1000)      108 2021-03-04 09:56:09.000000 wagtail_cblocks-0.4.1/MANIFEST.in
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1103 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/Makefile
--rw-r--r--   0 jerome    (1000) jerome    (1000)     4864 2023-05-04 14:02:30.253506 wagtail_cblocks-0.4.1/PKG-INFO
--rw-r--r--   0 jerome    (1000) jerome    (1000)     3807 2023-05-04 13:29:40.000000 wagtail_cblocks-0.4.1/README.md
--rw-r--r--   0 jerome    (1000) jerome    (1000)     2076 2023-05-04 13:26:21.000000 wagtail_cblocks-0.4.1/noxfile.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)      793 2022-03-09 14:08:45.000000 wagtail_cblocks-0.4.1/pyproject.toml
--rw-r--r--   0 jerome    (1000) jerome    (1000)       53 2022-03-09 14:08:45.000000 wagtail_cblocks-0.4.1/requirements-dev.txt
--rw-r--r--   0 jerome    (1000) jerome    (1000)       32 2022-03-09 14:08:45.000000 wagtail_cblocks-0.4.1/requirements-test.txt
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1180 2023-05-04 14:02:30.253506 wagtail_cblocks-0.4.1/setup.cfg
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.245506 wagtail_cblocks-0.4.1/tests/
--rw-r--r--   0 jerome    (1000) jerome    (1000)        0 2021-03-04 15:56:35.000000 wagtail_cblocks-0.4.1/tests/__init__.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)      160 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/tests/conftest.py
--rwxr-xr-x   0 jerome    (1000) jerome    (1000)      378 2022-03-31 09:47:32.000000 wagtail_cblocks-0.4.1/tests/manage.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.245506 wagtail_cblocks-0.4.1/tests/migrations/
--rw-r--r--   0 jerome    (1000) jerome    (1000)    96025 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/tests/migrations/0001_initial.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)        0 2021-03-04 16:37:56.000000 wagtail_cblocks-0.4.1/tests/migrations/__init__.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1977 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/tests/models.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     2417 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/tests/settings.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.237506 wagtail_cblocks-0.4.1/tests/templates/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.249506 wagtail_cblocks-0.4.1/tests/templates/tests/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.249506 wagtail_cblocks-0.4.1/tests/templates/tests/blocks/
--rw-r--r--   0 jerome    (1000) jerome    (1000)      195 2021-08-17 12:43:58.000000 wagtail_cblocks-0.4.1/tests/templates/tests/blocks/hero_block.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)      406 2021-08-16 16:09:20.000000 wagtail_cblocks-0.4.1/tests/templates/tests/blocks/row_columns_block.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)      849 2021-08-16 16:09:20.000000 wagtail_cblocks-0.4.1/tests/templates/tests/standard_page.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1971 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/tests/test_admin.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)    10682 2022-03-09 13:45:36.000000 wagtail_cblocks-0.4.1/tests/test_blocks.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)      445 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/tests/test_factories.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)      524 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/tests/urls.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.249506 wagtail_cblocks-0.4.1/wagtail_cblocks/
--rw-r--r--   0 jerome    (1000) jerome    (1000)        0 2021-03-02 16:06:36.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/__init__.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     8851 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/blocks.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)      681 2021-03-08 21:24:51.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/factories.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.237506 wagtail_cblocks-0.4.1/wagtail_cblocks/locale/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.237506 wagtail_cblocks-0.4.1/wagtail_cblocks/locale/fr/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.249506 wagtail_cblocks-0.4.1/wagtail_cblocks/locale/fr/LC_MESSAGES/
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1253 2022-03-24 10:55:23.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1646 2022-03-31 09:50:25.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.237506 wagtail_cblocks-0.4.1/wagtail_cblocks/static/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.237506 wagtail_cblocks-0.4.1/wagtail_cblocks/static/wagtail_cblocks/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.249506 wagtail_cblocks-0.4.1/wagtail_cblocks/static/wagtail_cblocks/css/
--rw-r--r--   0 jerome    (1000) jerome    (1000)      149 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/static/wagtail_cblocks/css/editor.css
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.237506 wagtail_cblocks-0.4.1/wagtail_cblocks/templates/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.253506 wagtail_cblocks-0.4.1/wagtail_cblocks/templates/wagtail_cblocks/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.253506 wagtail_cblocks-0.4.1/wagtail_cblocks/templates/wagtail_cblocks/block_forms/
--rw-r--r--   0 jerome    (1000) jerome    (1000)      750 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/templates/wagtail_cblocks/block_forms/link_block.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)      115 2021-08-16 16:09:20.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/templates/wagtail_cblocks/button_block.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)      336 2021-03-10 15:54:52.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/templates/wagtail_cblocks/columns_block.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)       77 2021-03-03 09:07:28.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/templates/wagtail_cblocks/heading_block.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)      402 2021-03-10 09:29:05.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/templates/wagtail_cblocks/image_block.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)       12 2021-03-03 09:07:35.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/templates/wagtail_cblocks/paragraph_block.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)      297 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/wagtail_hooks.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.249506 wagtail_cblocks-0.4.1/wagtail_cblocks.egg-info/
--rw-r--r--   0 jerome    (1000) jerome    (1000)     4864 2023-05-04 14:02:30.000000 wagtail_cblocks-0.4.1/wagtail_cblocks.egg-info/PKG-INFO
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1393 2023-05-04 14:02:30.000000 wagtail_cblocks-0.4.1/wagtail_cblocks.egg-info/SOURCES.txt
--rw-r--r--   0 jerome    (1000) jerome    (1000)        1 2023-05-04 14:02:30.000000 wagtail_cblocks-0.4.1/wagtail_cblocks.egg-info/dependency_links.txt
--rw-r--r--   0 jerome    (1000) jerome    (1000)       52 2023-05-04 14:02:30.000000 wagtail_cblocks-0.4.1/wagtail_cblocks.egg-info/requires.txt
--rw-r--r--   0 jerome    (1000) jerome    (1000)       16 2023-05-04 14:02:30.000000 wagtail_cblocks-0.4.1/wagtail_cblocks.egg-info/top_level.txt
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/.editorconfig
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/CHANGELOG.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/MANIFEST.in
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/Makefile
+-rwxr-xr-x   0        0        0      248 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/manage.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/tox.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/tests/conftest.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/tests/models.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/tests/settings.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/tests/test_admin.py
+-rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/tests/test_blocks.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/tests/test_factories.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/tests/urls.py
+-rw-r--r--   0        0        0    96025 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/tests/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/tests/migrations/__init__.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/tests/templates/tests/standard_page.html
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/tests/templates/tests/blocks/hero_block.html
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/tests/templates/tests/blocks/row_columns_block.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/wagtail_cblocks/__init__.py
+-rw-r--r--   0        0        0     8865 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/wagtail_cblocks/blocks.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/wagtail_cblocks/factories.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/wagtail_cblocks/wagtail_hooks.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/wagtail_cblocks/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/wagtail_cblocks/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/wagtail_cblocks/static/wagtail_cblocks/css/editor.css
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/wagtail_cblocks/templates/wagtail_cblocks/button_block.html
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/wagtail_cblocks/templates/wagtail_cblocks/columns_block.html
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/wagtail_cblocks/templates/wagtail_cblocks/heading_block.html
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/wagtail_cblocks/templates/wagtail_cblocks/image_block.html
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/wagtail_cblocks/templates/wagtail_cblocks/paragraph_block.html
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/wagtail_cblocks/templates/wagtail_cblocks/block_forms/link_block.html
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/README.md
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 wagtail_cblocks-0.4.2/PKG-INFO
```

### Comparing `wagtail_cblocks-0.4.1/CHANGELOG.md` & `wagtail_cblocks-0.4.2/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
+## 0.4.2 - 2024-05-23
+### Changed
+- Require Django >=4.2 and Wagtail >=5.2
+
 ## 0.4.1 - 2023-05-04
 
 This release only removes the Wagtail's maximum supported version to prevent
 conflicting dependencies.
 
 ## 0.4.0 - 2023-04-02
 ### Changed
```

### Comparing `wagtail_cblocks-0.4.1/LICENSE` & `wagtail_cblocks-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_cblocks-0.4.1/Makefile` & `wagtail_cblocks-0.4.2/Makefile`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,49 @@
-.PHONY: clean format help
 .DEFAULT_GOAL := help
 
 PYTHON := venv/bin/python
 
+.PHONY: help
 help:
 	@echo "Please use 'make <target>' where <target> is one of"
 	@echo ""
 	@grep '^[^.#]\+:\s\+.*#' Makefile | \
 	  sed "s/\(.\+\):\s*\(.*\) #\s*\(.*\)/`printf "\033[93m"`  \1`printf "\033[0m"`	\3 [\2]/" | \
 	  expand -35
 	@echo ""
 	@echo "Check the Makefile to know exactly what each target is doing."
 
+.PHONY: clean
 clean: # Remove all builds and Python artifacts
 	find wagtail_cblocks tests \
 	  \( -name '*.py[co]' -o -name '__pycache__' \) -exec rm -rf {} +
 	rm -rf build dist .eggs *.egg-info
 
+.PHONY: test
 test: # Run tests quickly with the current Python
 	$(PYTHON) -m pytest --cov --cov-report=term:skip-covered
 
+.PHONY: test-wip
 test-wip: # Run tests marked as wip with the current Python
 	$(PYTHON) -m pytest -vv -m 'wip' --pdb
 
+.PHONY: test-all
 test-all: # Run tests on all Django and Wagtail versions
-	nox
+	tox
 
-format: # Fix all the Python code syntax and imports order
-	pre-commit run --all-files --hook-stage=manual
+.PHONY: lint
+lint: # Check the Python code syntax and style
+	@$(PYTHON) -m ruff check
+	@$(PYTHON) -m ruff format --check --quiet
+
+.PHONY: format
+format: # Format and fix the Python code syntax
+	$(PYTHON) -m ruff check --fix
+	$(PYTHON) -m ruff format
 
+.PHONY: release
 release: dist # Package and upload a release
 	$(PYTHON) -m twine upload dist/*
 
+.PHONY: dist
 dist: clean # Build source and wheel package
 	$(PYTHON) -m build
-	ls -l dist
```

### Comparing `wagtail_cblocks-0.4.1/PKG-INFO` & `wagtail_cblocks-0.4.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,55 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: wagtail_cblocks
-Version: 0.4.1
+Version: 0.4.2
 Summary: Collection of StreamField blocks for Wagtail
-Author: Cliss XXI
-Author-email: contact@cliss21.com
-License: AGPLv3+
-Project-URL: Bug Tracker, https://framagit.org/cliss21/wagtail-cblocks/-/issues
-Project-URL: Source Code, https://framagit.org/cliss21/wagtail-cblocks
-Keywords: wagtail,blocks,streamfield
+Project-URL: Repository, https://framagit.org/cliss21/wagtail-cblocks
+Project-URL: Issues, https://framagit.org/cliss21/wagtail-cblocks/-/issues
+Author-email: Cliss XXI <contact@cliss21.com>
+License-Expression: AGPL-3.0-or-later
+License-File: LICENSE
+Keywords: blocks,streamfield,wagtail
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Wagtail
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Framework :: Django
-Classifier: Framework :: Wagtail
-Requires-Python: <4,>=3.7
-Description-Content-Type: text/markdown
+Requires-Python: >=3.8
+Requires-Dist: django>=4.2
+Requires-Dist: wagtail>=5.2
+Provides-Extra: dev
+Requires-Dist: pytest-cov~=5.0; extra == 'dev'
+Requires-Dist: pytest-django~=4.8; extra == 'dev'
+Requires-Dist: pytest~=8.2; extra == 'dev'
+Requires-Dist: ruff~=0.4.4; extra == 'dev'
+Requires-Dist: wagtail-factories>=4.0.0; extra == 'dev'
 Provides-Extra: factories
-License-File: LICENSE
+Requires-Dist: wagtail-factories>=4.0.0; extra == 'factories'
+Description-Content-Type: text/markdown
 
 # wagtail-cblocks
 
 A collection of StreamField blocks to use in Wagtail CMS.
 
 **Warning!** This project is still early on in its development lifecycle. It is
 possible for breaking changes to occur between versions until reaching a stable
 1.0. Feedback and pull requests are welcome.
 
 ## Requirements
 
 wagtail-cblocks requires the following:
-- **Wagtail** (4.1 LTS, 4.2, 5.0)
-- **Django** (3.2 LTS, 4.1, 4.2 LTS)
-- **Python 3** (3.7, 3.8, 3.9, 3.10, 3.11)
+- **Python 3** (3.8, 3.9, 3.10, 3.11, 3.12)
+- **Django** (4.2 LTS, 5.0)
+- **Wagtail** (5.2 LTS, 6.0, 6.1)
 
 ## Installation
 
 1. Install using ``pip``:
    ```shell
    $ pip install wagtail-cblocks
    ```
@@ -116,48 +123,38 @@
 2. Create a virtual environment and activate it:
    ```shell
    $ python3 -m venv venv
    $ source venv/bin/activate
    ```
 3. Install this package and its requirements:
    ```shell
-   (venv)$ pip install -r requirements-dev.txt
+   (venv)$ pip install --editable ".[dev]" "tox>=4.11"
    ```
 
-Finally, if you want to run the test application to preview the blocks, you will
-have to create the database before running a development server:
-```shell
-(venv)$ ./tests/manage.py migrate
-(venv)$ ./tests/manage.py runserver
-```
+To run the test app interactively, use ``tox -e interactive``, visit
+[http://127.0.0.1:8020/admin](http://127.0.0.1:8000/admin/) and log in
+with `admin` / `changeme`.
 
 ### Contributing
 
 The tests are written with [pytest] and code coverage is measured with [coverage].
 You can use the following commands while developing:
 - ``make test``: run the tests and output a quick report of code coverage
 - ``make test-wip``: only run the tests marked as 'wip'
 - ``make test-all``: run the tests on all supported versions of Django and
   Wagtail with [nox]
 
-The Python code is formatted and linted thanks to [flake8], [isort] and [black].
-All of these tools are configured in [pre-commit] and you should consider to
-install its git hook scripts by running:
-```shell
-(venv)$ pre-commit install
-```
+The Python code is formatted and linted thanks to [ruff]. You can check the code
+with ``make lint`` and try to fix the reported issues with ``make format``.
 
 When submitting a pull-request, please ensure that the code is well formatted
 and covered, and that all the tests pass.
 
 [pytest]: https://docs.pytest.org/
 [coverage]: https://coverage.readthedocs.io/
 [nox]: https://nox.thea.codes/
-[flake8]: https://flake8.pycqa.org/
-[isort]: https://pycqa.github.io/isort/
-[black]: https://black.readthedocs.io/
-[pre-commit]: https://pre-commit.com/
+[ruff]: https://docs.astral.sh/ruff/
 
 ## License
 
 This extension is mainly developed by [Cliss XXI](https://www.cliss21.com) and
 licensed under the [AGPLv3+](LICENSE). Any contribution is welcome!
```

### Comparing `wagtail_cblocks-0.4.1/README.md` & `wagtail_cblocks-0.4.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 **Warning!** This project is still early on in its development lifecycle. It is
 possible for breaking changes to occur between versions until reaching a stable
 1.0. Feedback and pull requests are welcome.
 
 ## Requirements
 
 wagtail-cblocks requires the following:
-- **Wagtail** (4.1 LTS, 4.2, 5.0)
-- **Django** (3.2 LTS, 4.1, 4.2 LTS)
-- **Python 3** (3.7, 3.8, 3.9, 3.10, 3.11)
+- **Python 3** (3.8, 3.9, 3.10, 3.11, 3.12)
+- **Django** (4.2 LTS, 5.0)
+- **Wagtail** (5.2 LTS, 6.0, 6.1)
 
 ## Installation
 
 1. Install using ``pip``:
    ```shell
    $ pip install wagtail-cblocks
    ```
@@ -89,48 +89,38 @@
 2. Create a virtual environment and activate it:
    ```shell
    $ python3 -m venv venv
    $ source venv/bin/activate
    ```
 3. Install this package and its requirements:
    ```shell
-   (venv)$ pip install -r requirements-dev.txt
+   (venv)$ pip install --editable ".[dev]" "tox>=4.11"
    ```
 
-Finally, if you want to run the test application to preview the blocks, you will
-have to create the database before running a development server:
-```shell
-(venv)$ ./tests/manage.py migrate
-(venv)$ ./tests/manage.py runserver
-```
+To run the test app interactively, use ``tox -e interactive``, visit
+[http://127.0.0.1:8020/admin](http://127.0.0.1:8000/admin/) and log in
+with `admin` / `changeme`.
 
 ### Contributing
 
 The tests are written with [pytest] and code coverage is measured with [coverage].
 You can use the following commands while developing:
 - ``make test``: run the tests and output a quick report of code coverage
 - ``make test-wip``: only run the tests marked as 'wip'
 - ``make test-all``: run the tests on all supported versions of Django and
   Wagtail with [nox]
 
-The Python code is formatted and linted thanks to [flake8], [isort] and [black].
-All of these tools are configured in [pre-commit] and you should consider to
-install its git hook scripts by running:
-```shell
-(venv)$ pre-commit install
-```
+The Python code is formatted and linted thanks to [ruff]. You can check the code
+with ``make lint`` and try to fix the reported issues with ``make format``.
 
 When submitting a pull-request, please ensure that the code is well formatted
 and covered, and that all the tests pass.
 
 [pytest]: https://docs.pytest.org/
 [coverage]: https://coverage.readthedocs.io/
 [nox]: https://nox.thea.codes/
-[flake8]: https://flake8.pycqa.org/
-[isort]: https://pycqa.github.io/isort/
-[black]: https://black.readthedocs.io/
-[pre-commit]: https://pre-commit.com/
+[ruff]: https://docs.astral.sh/ruff/
 
 ## License
 
 This extension is mainly developed by [Cliss XXI](https://www.cliss21.com) and
 licensed under the [AGPLv3+](LICENSE). Any contribution is welcome!
```

### Comparing `wagtail_cblocks-0.4.1/tests/migrations/0001_initial.py` & `wagtail_cblocks-0.4.2/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_cblocks-0.4.1/tests/models.py` & `wagtail_cblocks-0.4.2/tests/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,68 +10,68 @@
     ImageBlock,
     ParagraphBlock,
     Style,
     StylizedStructBlock,
 )
 
 BUTTON_STYLES = [
-    Style('primary', "Primary", 'btn-primary'),
-    Style('secondary', "Secondary", 'btn-secondary'),
-    Style('primary-lg', "Large primary", 'btn-primary btn-lg'),
+    Style("primary", "Primary", "btn-primary"),
+    Style("secondary", "Secondary", "btn-secondary"),
+    Style("primary-lg", "Large primary", "btn-primary btn-lg"),
 ]
-BUTTON_DEFAULT_STYLE = 'primary-lg'
+BUTTON_DEFAULT_STYLE = "primary-lg"
 
 
 class BaseBlock(StreamBlock):
     title_block = HeadingBlock()
     paragraph_block = ParagraphBlock()
     button_block = ButtonBlock(
         styles=BUTTON_STYLES, default_style=BUTTON_DEFAULT_STYLE
     )
     image_block = ImageBlock()
 
 
 class RowColumnsBlock(ColumnsBlock):
     LAYOUT_CHOICES = [
-        ('2', "2-columns"),
-        ('3', "3-columns"),
-        ('4', "4-columns"),
-        ('auto', "natural width"),
+        ("2", "2-columns"),
+        ("3", "3-columns"),
+        ("4", "4-columns"),
+        ("auto", "natural width"),
     ]
 
-    layout = ChoiceBlock(choices=LAYOUT_CHOICES, default='auto')
+    layout = ChoiceBlock(choices=LAYOUT_CHOICES, default="auto")
 
     class Meta:
         label = "Row columns"
-        template = 'tests/blocks/row_columns_block.html'
+        template = "tests/blocks/row_columns_block.html"
         column_block = BaseBlock()
 
 
 class HeroBlock(StylizedStructBlock):
     blocks = BaseBlock(
-        local_blocks=[('columns_block', ColumnsBlock(BaseBlock()))],
+        local_blocks=[("columns_block", ColumnsBlock(BaseBlock()))],
         label="Content",
     )
 
     styles = [
-        Style('centered', "Centered", 'my-5 text-center hero-centered'),
-        Style('responsive', "Responsive", 'container col-xxl-8'),
-        Style('dark', "Dark", 'bg-dark text-white text-center'),
+        Style("centered", "Centered", "my-5 text-center hero-centered"),
+        Style("responsive", "Responsive", "container col-xxl-8"),
+        Style("dark", "Dark", "bg-dark text-white text-center"),
     ]
 
     class Meta:
         label = "Hero"
-        template = 'tests/blocks/hero_block.html'
+        template = "tests/blocks/hero_block.html"
 
 
 class BodyBlock(BaseBlock):
     hero_block = HeroBlock()
     columns_block = ColumnsBlock(BaseBlock())
     row_columns_block = RowColumnsBlock()
 
 
 class StandardPage(Page):
     body = StreamField(BodyBlock(), use_json_field=True)
 
     content_panels = Page.content_panels + [
-        FieldPanel('body'),
+        FieldPanel("body"),
     ]
```

### Comparing `wagtail_cblocks-0.4.1/tests/settings.py` & `wagtail_cblocks-0.4.2/tests/settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,106 +1,126 @@
 import os
 from pathlib import Path
 
 BASE_DIR = Path(__file__).parent
+VAR_DIR = Path(__file__).parent / "var"
 
-VAR_DIR = Path(__file__).parent / 'var'
+# GENERAL
 
-DEBUG = True if os.environ.get('DEBUG', '0') == '1' else False
+DEBUG = True if os.environ.get("INTERACTIVE", "0") == "1" else False
+
+SECRET_KEY = "not-a-secure-key"  # noqa: S105
+
+ALLOWED_HOSTS = ["localhost", "testserver"]
+
+# INTERNATIONALIZATION
+
+LANGUAGE_CODE = "en-us"
+
+TIME_ZONE = "UTC"
+
+USE_TZ = True
+
+# DATABASE
 
 DATABASES = {
-    'default': {
-        'ENGINE': 'django.db.backends.sqlite3',
-        'NAME': str(BASE_DIR / 'sqlite.db'),
+    "default": {
+        "ENGINE": "django.db.backends.sqlite3",
+        "NAME": str(BASE_DIR / "sqlite.db"),
     }
 }
 
-SECRET_KEY = 'not needed'
+DEFAULT_AUTO_FIELD = "django.db.models.AutoField"
+
+# URLS
 
-ALLOWED_HOSTS = ['localhost', 'testserver']
+ROOT_URLCONF = "tests.urls"
 
-ROOT_URLCONF = 'tests.urls'
+# APP CONFIGURATION
 
-STATIC_URL = '/static/'
+INSTALLED_APPS = [
+    "wagtail_cblocks",
+    "tests",
+    # wagtail
+    "wagtail.sites",
+    "wagtail.users",
+    "wagtail.documents",
+    "wagtail.images",
+    "wagtail.search",
+    "wagtail.admin",
+    "wagtail",
+    "modelcluster",
+    "taggit",
+    # django
+    "django.contrib.auth",
+    "django.contrib.contenttypes",
+    "django.contrib.sessions",
+    "django.contrib.messages",
+    "django.contrib.staticfiles",
+]
+
+# PASSWORDS
+
+PASSWORD_HASHERS = ["django.contrib.auth.hashers.MD5PasswordHasher"]
+
+# MIDDLEWARE
+
+MIDDLEWARE = [
+    "django.middleware.security.SecurityMiddleware",
+    "django.contrib.sessions.middleware.SessionMiddleware",
+    "django.middleware.common.CommonMiddleware",
+    "django.middleware.csrf.CsrfViewMiddleware",
+    "django.contrib.auth.middleware.AuthenticationMiddleware",
+    "django.contrib.messages.middleware.MessageMiddleware",
+    "django.middleware.clickjacking.XFrameOptionsMiddleware",
+    "wagtail.contrib.redirects.middleware.RedirectMiddleware",
+]
+
+# STATIC
+
+STATIC_ROOT = VAR_DIR / "static"
+
+STATIC_URL = "/static/"
 
 STATICFILES_FINDERS = [
-    'django.contrib.staticfiles.finders.AppDirectoriesFinder',
+    "django.contrib.staticfiles.finders.FileSystemFinder",
+    "django.contrib.staticfiles.finders.AppDirectoriesFinder",
 ]
 
-STATIC_ROOT = VAR_DIR / 'static'
+# MEDIA
 
-MEDIA_URL = '/media/'
+MEDIA_ROOT = VAR_DIR / "media"
 
-MEDIA_ROOT = VAR_DIR / 'media'
+MEDIA_URL = "/media/"
 
-USE_TZ = True
+# TEMPLATES
 
 TEMPLATES = [
     {
-        'BACKEND': 'django.template.backends.django.DjangoTemplates',
-        'DIRS': [],
-        'APP_DIRS': True,
-        'OPTIONS': {
-            'debug': DEBUG,
-            'context_processors': [
-                'django.template.context_processors.debug',
-                'django.template.context_processors.request',
-                'django.contrib.auth.context_processors.auth',
-                'django.contrib.messages.context_processors.messages',
+        "BACKEND": "django.template.backends.django.DjangoTemplates",
+        "DIRS": [],
+        "APP_DIRS": True,
+        "OPTIONS": {
+            "context_processors": [
+                "django.template.context_processors.debug",
+                "django.template.context_processors.request",
+                "django.contrib.auth.context_processors.auth",
+                "django.contrib.messages.context_processors.messages",
             ],
         },
     },
 ]
 
-MIDDLEWARE = [
-    'django.contrib.sessions.middleware.SessionMiddleware',
-    'django.middleware.common.CommonMiddleware',
-    'django.middleware.csrf.CsrfViewMiddleware',
-    'django.contrib.auth.middleware.AuthenticationMiddleware',
-    'django.contrib.messages.middleware.MessageMiddleware',
-    'django.middleware.clickjacking.XFrameOptionsMiddleware',
-]
-
-INSTALLED_APPS = [
-    # django
-    'django.contrib.auth',
-    'django.contrib.contenttypes',
-    'django.contrib.sessions',
-    'django.contrib.messages',
-    'django.contrib.staticfiles',
-    # wagtail
-    'wagtail.sites',
-    'wagtail.users',
-    'wagtail.documents',
-    'wagtail.images',
-    'wagtail.search',
-    'wagtail.admin',
-    'wagtail',
-    'modelcluster',
-    'taggit',
-    # wagtail_cblocks
-    'wagtail_cblocks',
-    'tests',
-]
-
-PASSWORD_HASHERS = ['django.contrib.auth.hashers.MD5PasswordHasher']
-
-DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'
+# CACHES
 
 CACHES = {
-    'default': {
-        'BACKEND': 'django.core.cache.backends.db.DatabaseCache',
-        'LOCATION': 'cache',
+    "default": {
+        "BACKEND": "django.core.cache.backends.locmem.LocMemCache",
+        "LOCATION": "",
     }
 }
 
-# Wagtail settings
-
-WAGTAILADMIN_BASE_URL = 'http://testserver'
+# WAGTAIL
 
-WAGTAIL_SITE_NAME = 'wagtail-cblocks test'
+WAGTAILADMIN_BASE_URL = "http://testserver"
 
-WAGTAILSEARCH_BACKENDS = {
-    'default': {
-        'BACKEND': 'wagtail.search.backends.database',
-    }
-}
+WAGTAIL_SITE_NAME = "wagtail-cblocks test"
```

### Comparing `wagtail_cblocks-0.4.1/tests/templates/tests/standard_page.html` & `wagtail_cblocks-0.4.2/tests/templates/tests/standard_page.html`

 * *Files identical despite different names*

### Comparing `wagtail_cblocks-0.4.1/tests/test_admin.py` & `wagtail_cblocks-0.4.2/tests/test_admin.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,53 +10,53 @@
 from pytest_django.asserts import assertContains
 
 from .models import StandardPage
 
 
 @pytest.mark.django_db
 def test_insert_editor_css(admin_client, root_page):
-    response = admin_client.get('/admin/pages/%d/edit/' % root_page.id)
-    assertContains(response, 'wagtail_cblocks/css/editor.css')
+    response = admin_client.get("/admin/pages/%d/edit/" % root_page.id)
+    assertContains(response, "wagtail_cblocks/css/editor.css")
 
 
 @pytest.mark.django_db
 class TestStylizedStructBlock:
     def test_page_preview(self, admin_client, root_page):
         add_url = reverse(
-            'wagtailadmin_pages:add',
-            args=('tests', 'standardpage', root_page.id),
+            "wagtailadmin_pages:add",
+            args=("tests", "standardpage", root_page.id),
         )
 
         form_data = nested_form_data(
             {
-                'title': "A page",
-                'body': streamfield(
+                "title": "A page",
+                "body": streamfield(
                     [
                         (
-                            'hero_block',
+                            "hero_block",
                             {
-                                'style': 'centered',
-                                'blocks': streamfield(
+                                "style": "centered",
+                                "blocks": streamfield(
                                     [
                                         (
-                                            'paragraph_block',
-                                            rich_text('<p>Lorem ipsum</p>'),
+                                            "paragraph_block",
+                                            rich_text("<p>Lorem ipsum</p>"),
                                         ),
                                     ]
                                 ),
                             },
                         ),
                     ]
                 ),
             }
         )
-        form_data['slug'] = 'a-page'
+        form_data["slug"] = "a-page"
         response = admin_client.post(add_url, data=form_data)
         assert response.status_code == 302
 
-        page = StandardPage.objects.get(slug='a-page')
-        preview_url = reverse('wagtailadmin_pages:view_draft', args=(page.id,))
+        page = StandardPage.objects.get(slug="a-page")
+        preview_url = reverse("wagtailadmin_pages:view_draft", args=(page.id,))
 
         response = admin_client.get(preview_url)
         assert response.status_code == 200
-        assertContains(response, 'hero-centered')
-        assertContains(response, 'Lorem ipsum')
+        assertContains(response, "hero-centered")
+        assertContains(response, "Lorem ipsum")
```

### Comparing `wagtail_cblocks-0.4.1/tests/test_blocks.py` & `wagtail_cblocks-0.4.2/tests/test_blocks.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,314 +14,312 @@
 class BlockTest:
     def render(self, data, block=None):
         if block is None:
             block = self.block
         return block.render(block.to_python(data))
 
     def render_html(self, *args, **kwargs):
-        return BeautifulSoup(self.render(*args, **kwargs), 'html.parser')
+        return BeautifulSoup(self.render(*args, **kwargs), "html.parser")
 
 
 class TestCSSClassMixin:
     class Block(CSSClassMixin, blocks.ParagraphBlock):
         pass
 
     def test_in_meta(self):
         class Block(self.Block):
             class Meta:
-                css_class = 'lead'
+                css_class = "lead"
 
         block = Block()
-        context = block.get_context(block.to_python('<p>Paragraph</p>'))
-        assert context['css_class'] == 'lead'
+        context = block.get_context(block.to_python("<p>Paragraph</p>"))
+        assert context["css_class"] == "lead"
 
-    @pytest.mark.parametrize('value', ('lead', {'lead'}, ['lead']))
+    @pytest.mark.parametrize("value", ("lead", {"lead"}, ["lead"]))
     def test_at_init(self, value):
         block = self.Block(css_class=value)
-        context = block.get_context(block.to_python('<p>Paragraph</p>'))
-        assert context['css_class'] == 'lead'
+        context = block.get_context(block.to_python("<p>Paragraph</p>"))
+        assert context["css_class"] == "lead"
 
     def test_empty(self):
         block = self.Block()
-        context = block.get_context(block.to_python('<p>Paragraph</p>'))
-        assert context['css_class'] == ''
+        context = block.get_context(block.to_python("<p>Paragraph</p>"))
+        assert context["css_class"] == ""
 
 
 class TestStylizedStructBlock:
     STYLES = [
-        Style('foo', "Foo", 'is-foo'),
-        Style('bar', "Bar", 'is-bar'),
+        Style("foo", "Foo", "is-foo"),
+        Style("bar", "Bar", "is-bar"),
     ]
 
     def test_empty_styles(self):
         block = StylizedStructBlock()
-        assert 'style' not in block.child_blocks
+        assert "style" not in block.child_blocks
         context = block.get_context(block.to_python({}))
-        assert context['css_class'] == ''
+        assert context["css_class"] == ""
 
     def test_styles_from_property(self):
         class Block(StylizedStructBlock):
             styles = self.STYLES
 
-        value = Block().to_python({'style': 'foo'})
-        assert value.get('style').name == 'foo'
+        value = Block().to_python({"style": "foo"})
+        assert value.get("style").name == "foo"
 
     def test_style(self):
         block = StylizedStructBlock(styles=self.STYLES)
-        value = block.to_python({'style': 'foo'})
-        assert block.get_prep_value(value) == {'style': 'foo'}
-        assert isinstance(value['style'], Style)
-        assert value['style'].name == 'foo'
+        value = block.to_python({"style": "foo"})
+        assert block.get_prep_value(value) == {"style": "foo"}
+        assert isinstance(value["style"], Style)
+        assert value["style"].name == "foo"
         context = block.get_context(value)
-        assert context['css_class'] == 'is-foo'
+        assert context["css_class"] == "is-foo"
 
     def test_style_with_css_class(self):
-        block = StylizedStructBlock(styles=self.STYLES, css_class='block')
-        context = block.get_context(block.to_python({'style': 'foo'}))
-        assert context['css_class'] == 'block is-foo'
+        block = StylizedStructBlock(styles=self.STYLES, css_class="block")
+        context = block.get_context(block.to_python({"style": "foo"}))
+        assert context["css_class"] == "block is-foo"
 
     def test_default_style(self):
-        block = StylizedStructBlock(styles=self.STYLES, default_style='bar')
+        block = StylizedStructBlock(styles=self.STYLES, default_style="bar")
         value = block.to_python({})
-        assert isinstance(value.get('style'), Style)
-        assert value.get('style').name == 'bar'
+        assert isinstance(value.get("style"), Style)
+        assert value.get("style").name == "bar"
         context = block.get_context(value)
-        assert context['css_class'] == 'is-bar'
+        assert context["css_class"] == "is-bar"
 
     def test_default_style_object(self):
         block = StylizedStructBlock(
             styles=self.STYLES, default_style=self.STYLES[1]
         )
         value = block.to_python({})
-        assert isinstance(value.get('style'), Style)
-        assert value.get('style').name == 'bar'
+        assert isinstance(value.get("style"), Style)
+        assert value.get("style").name == "bar"
 
     def test_unknown_style(self):
-        block = StylizedStructBlock(styles=self.STYLES, default_style='bar')
-        value = block.to_python({'style': 'baz'})
-        assert value.get('style') is None
+        block = StylizedStructBlock(styles=self.STYLES, default_style="bar")
+        value = block.to_python({"style": "baz"})
+        assert value.get("style") is None
         context = block.get_context(value)
-        assert context['css_class'] == ''
+        assert context["css_class"] == ""
 
 
 class TestHeadingBlock(BlockTest):
     block = blocks.HeadingBlock()
 
     def test_render(self):
         assertHTMLEqual(
-            self.render({'text': "Un titre !", 'level': 2}),
+            self.render({"text": "Un titre !", "level": 2}),
             '<h2 id="un-titre">Un titre !</h2>',
         )
 
 
 class TestParagraphBlock(BlockTest):
     block = blocks.ParagraphBlock()
 
     def test_features(self):
         assert self.block.features == blocks.ParagraphBlock.features
 
-        block = blocks.ParagraphBlock(features=['bold', 'italic'])
-        assert block.features == ['bold', 'italic']
+        block = blocks.ParagraphBlock(features=["bold", "italic"])
+        assert block.features == ["bold", "italic"]
 
     def test_render(self):
-        data = '<p><i>Un</i> paragraphe !</p>'
+        data = "<p><i>Un</i> paragraphe !</p>"
         assertHTMLEqual(self.render(data), data)
 
 
 @pytest.mark.django_db
 class TestLinkBlock:
     block = blocks.LinkBlock()
 
     def get_value(self, target):
-        return self.block.to_python({'target': target})
+        return self.block.to_python({"target": target})
 
     def test_local_blocks(self):
-        block = blocks.LinkBlock([('text', blocks.ParagraphBlock())])
-        assert list(block.child_blocks.keys()) == ['text', 'target']
+        block = blocks.LinkBlock([("text", blocks.ParagraphBlock())])
+        assert list(block.child_blocks.keys()) == ["text", "target"]
 
     def test_required(self):
         block = blocks.LinkBlock(required=False)
         assert block.required is False
-        assert block.child_blocks['target'].required is False
+        assert block.child_blocks["target"].required is False
 
         assert self.block.required is True
-        assert self.block.child_blocks['target'].required is True
+        assert self.block.child_blocks["target"].required is True
 
     def test_href_value_page(self, root_page):
-        page = PageFactory(parent=root_page, title="About", slug='about')
-        value = self.get_value([{'type': 'page', 'value': page.id}])
-        assert value.href == '/about/'
+        page = PageFactory(parent=root_page, title="About", slug="about")
+        value = self.get_value([{"type": "page", "value": page.id}])
+        assert value.href == "/about/"
 
     def test_href_value_page_invalid(self):
-        value = self.get_value([{'type': 'page', 'value': 1000}])
+        value = self.get_value([{"type": "page", "value": 1000}])
         assert value.href is None
 
     def test_href_value_document(self):
         document = DocumentFactory()
-        value = self.get_value([{'type': 'document', 'value': document.id}])
+        value = self.get_value([{"type": "document", "value": document.id}])
         assert value.href == document.file.url
 
     def test_href_value_document_invalid(self):
-        value = self.get_value([{'type': 'document', 'value': 1000}])
+        value = self.get_value([{"type": "document", "value": 1000}])
         assert value.href is None
 
     def test_href_value_image(self):
         image = ImageFactory()
-        value = self.get_value([{'type': 'image', 'value': image.id}])
+        value = self.get_value([{"type": "image", "value": image.id}])
         assert value.href == image.file.url
 
     def test_href_value_image_invalid(self):
-        value = self.get_value([{'type': 'image', 'value': 1000}])
+        value = self.get_value([{"type": "image", "value": 1000}])
         assert value.href is None
 
     def test_href_value_external_url(self):
-        url = 'http://example.org/truc/'
-        value = self.get_value([{'type': 'url', 'value': url}])
+        url = "http://example.org/truc/"
+        value = self.get_value([{"type": "url", "value": url}])
         assert value.href == url
 
     def test_href_value_anchor(self):
-        anchor = '#truc'
-        value = self.get_value([{'type': 'anchor', 'value': anchor}])
+        anchor = "#truc"
+        value = self.get_value([{"type": "anchor", "value": anchor}])
         assert value.href == anchor
 
     def test_href_value_empty(self):
         value = self.get_value([])
         assert value.href is None
 
     def test_href_value_no_target(self):
-        block = blocks.LinkBlock([('text', blocks.ParagraphBlock())])
-        value = block.to_python({'text': "some text"})
+        block = blocks.LinkBlock([("text", blocks.ParagraphBlock())])
+        value = block.to_python({"text": "some text"})
         assert value.href is None
 
 
 class TestButtonBlock(BlockTest):
     block = blocks.ButtonBlock()
 
     def test_render_link(self):
-        url = 'http://example.org/truc/'
+        url = "http://example.org/truc/"
         assertHTMLEqual(
             self.render(
                 {
-                    'text': "Lien",
-                    'link': {'target': [{'type': 'url', 'value': url}]},
+                    "text": "Lien",
+                    "link": {"target": [{"type": "url", "value": url}]},
                 }
             ),
-            '<a class="btn mb-3" href="{}">Lien</a>'.format(url),
+            f'<a class="btn mb-3" href="{url}">Lien</a>',
         )
 
 
 @pytest.mark.django_db
 class TestImageBlock(BlockTest):
     block = blocks.ImageBlock()
 
     def test_render(self):
         html = self.render_html(
             {
-                'image': ImageFactory().id,
-                'caption': '',
-                'link': {'target': []},
+                "image": ImageFactory().id,
+                "caption": "",
+                "link": {"target": []},
             }
         )
-        assert len(html.select('img.figure-img.img-fluid.mb-0')) == 1
-        assert not html.select('figcaption')
-        assert not html.select('a')
+        assert len(html.select("img.figure-img.img-fluid.mb-0")) == 1
+        assert not html.select("figcaption")
+        assert not html.select("a")
 
     def test_render_with_caption(self):
         html = self.render_html(
             {
-                'image': ImageFactory().id,
-                'caption': "Une légende en dessous.",
-                'link': {'target': []},
+                "image": ImageFactory().id,
+                "caption": "Une légende en dessous.",
+                "link": {"target": []},
             }
         )
-        assert html.select_one('figcaption').text == "Une légende en dessous."
-        assert not html.select('a')
+        assert html.select_one("figcaption").text == "Une légende en dessous."
+        assert not html.select("a")
 
     def test_render_with_link(self):
-        url = 'http://example.org/truc/'
+        url = "http://example.org/truc/"
         html = self.render_html(
             {
-                'image': ImageFactory().id,
-                'caption': '',
-                'link': {'target': [{'type': 'url', 'value': url}]},
+                "image": ImageFactory().id,
+                "caption": "",
+                "link": {"target": [{"type": "url", "value": url}]},
             }
         )
-        assert html.select_one('a').attrs['href'] == url
-        assert not html.select('figcaption')
+        assert html.select_one("a").attrs["href"] == url
+        assert not html.select("figcaption")
 
 
 class TestColumnsBlock(BlockTest):
     block = blocks.ColumnsBlock(BaseBlock())
 
     def test_columns_block_order(self):
-        assert list(self.block.child_blocks.keys())[0] == 'columns'
+        assert list(self.block.child_blocks.keys())[0] == "columns"
 
     def test_render(self):
-        url = 'http://example.org/truc/'
+        url = "http://example.org/truc/"
         data = {
-            'columns': [
+            "columns": [
                 [
                     {
-                        'type': 'button_block',
-                        'value': {
-                            'text': "Lien",
-                            'link': {
-                                'target': [{'type': 'url', 'value': url}],
+                        "type": "button_block",
+                        "value": {
+                            "text": "Lien",
+                            "link": {
+                                "target": [{"type": "url", "value": url}],
                             },
-                            'style': 'primary',
+                            "style": "primary",
                         },
                     },
                     {
-                        'type': 'paragraph_block',
-                        'value': "<p>A first paragraph.</p>",
+                        "type": "paragraph_block",
+                        "value": "<p>A first paragraph.</p>",
                     },
                 ],
                 [
                     {
-                        'type': 'paragraph_block',
-                        'value': "<p>Another paragraph.</p>",
+                        "type": "paragraph_block",
+                        "value": "<p>Another paragraph.</p>",
                     },
                 ],
             ],
-            'horizontal_align': 'center',
+            "horizontal_align": "center",
         }
         assertHTMLEqual(
             self.render(data),
             (
                 '<div class="row text-center">'
                 '<div class="col-sm">{}{}</div>'
                 '<div class="col-sm">{}</div>'
-                '</div>'
+                "</div>"
             ).format(
-                '<a class="btn btn-primary mb-3" href="{}">Lien</a>'.format(
-                    url
-                ),
-                '<p>A first paragraph.</p>',
-                '<p>Another paragraph.</p>',
+                f'<a class="btn btn-primary mb-3" href="{url}">Lien</a>',
+                "<p>A first paragraph.</p>",
+                "<p>Another paragraph.</p>",
             ),
         )
 
     def test_sublcass_render(self):
         data = {
-            'columns': [
+            "columns": [
                 [
                     {
-                        'type': 'paragraph_block',
-                        'value': "<p>A first paragraph.</p>",
+                        "type": "paragraph_block",
+                        "value": "<p>A first paragraph.</p>",
                     },
                 ],
             ],
-            'layout': 'auto',
+            "layout": "auto",
         }
         assertHTMLEqual(
             self.render(data, RowColumnsBlock()),
             (
                 '<div class="row row-cols-auto">'
                 '<div class="col"><p>A first paragraph.</p></div>'
-                '</div>'
+                "</div>"
             ),
         )
 
     def test_required_column_block(self):
         with pytest.raises(ImproperlyConfigured):
 
             class DummyColumnsBlock(ColumnsBlock):
```

### Comparing `wagtail_cblocks-0.4.1/tests/urls.py` & `wagtail_cblocks-0.4.2/tests/urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from django.urls import include, path
 
 from wagtail import urls as wagtail_urls
 from wagtail.admin import urls as wagtailadmin_urls
 from wagtail.documents import urls as wagtaildocs_urls
 
 urlpatterns = [
-    path('admin/', include(wagtailadmin_urls)),
-    path('documents/', include(wagtaildocs_urls)),
-    path('', include(wagtail_urls)),
+    path("admin/", include(wagtailadmin_urls)),
+    path("documents/", include(wagtaildocs_urls)),
+    path("", include(wagtail_urls)),
 ]
 
 if settings.DEBUG:
     from django.conf.urls.static import static
 
     urlpatterns += static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)
```

### Comparing `wagtail_cblocks-0.4.1/wagtail_cblocks/blocks.py` & `wagtail_cblocks-0.4.2/wagtail_cblocks/blocks.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,34 +9,34 @@
 from wagtail import blocks as wagtail_blocks
 from wagtail.documents.blocks import DocumentChooserBlock
 from wagtail.images.blocks import ImageChooserBlock
 
 # MIXINS AND BASE CLASSES
 # ------------------------------------------------------------------------------
 
-Style = namedtuple('Style', ['name', 'label', 'css_class'])
+Style = namedtuple("Style", ["name", "label", "css_class"])
 
 
 class CSSClassMixin:
     """
     Add the CSS class defined for a block to its rendering context.
     """
 
     def get_css_classes(self, value):
-        if hasattr(self.meta, 'css_class'):
+        if hasattr(self.meta, "css_class"):
             if isinstance(self.meta.css_class, str):
                 return [self.meta.css_class]
             if not isinstance(self.meta.css_class, list):
                 return list(self.meta.css_class)
             return self.meta.css_class
         return []
 
     def get_context(self, value, **kwargs):
         context = super().get_context(value, **kwargs)
-        context['css_class'] = ' '.join(self.get_css_classes(value))
+        context["css_class"] = " ".join(self.get_css_classes(value))
         return context
 
 
 class StyleChoiceBlock(wagtail_blocks.ChoiceBlock):
     class Meta:
         label = _("Style")
 
@@ -85,154 +85,154 @@
         super().__init__(*args, **kwargs)
 
         if styles is None:
             styles = self.styles
 
         if styles:
             style = StyleChoiceBlock(styles, default=self.meta.default_style)
-            style.set_name('style')
+            style.set_name("style")
 
-            self.child_blocks['style'] = style
+            self.child_blocks["style"] = style
 
     def get_css_classes(self, value):
         css_classes = super().get_css_classes(value)
-        style = value.get('style', None)
+        style = value.get("style", None)
         if style and style.css_class:
             css_classes.append(style.css_class)
         return css_classes
 
 
 # TYPOGRAPHY
 # ------------------------------------------------------------------------------
 
 HEADING_LEVELS = [
-    (i, _("Level %(level)d heading") % {'level': i}) for i in range(2, 6)
+    (i, _("Level %(level)d heading") % {"level": i}) for i in range(2, 6)
 ]
 
 
 class HeadingValue(wagtail_blocks.StructValue):
     @cached_property
     def tag(self):
         """Return the HTML tag to use for the level."""
-        return 'h{}'.format(self.get('level'))
+        return "h{}".format(self.get("level"))
 
     @cached_property
     def anchor(self):
         """Generate a slug from the title to be used as an anchor."""
-        return slugify(self.get('text'))
+        return slugify(self.get("text"))
 
 
 class HeadingBlock(wagtail_blocks.StructBlock):
     """
     A section heading with a choosable level.
     """
 
-    text = wagtail_blocks.CharBlock(label=_("Title"), classname='title')
+    text = wagtail_blocks.CharBlock(label=_("Title"), classname="title")
     level = wagtail_blocks.ChoiceBlock(
         choices=HEADING_LEVELS,
         default=2,
         label=_("Level"),
     )
 
     class Meta:
-        icon = 'title'
+        icon = "title"
         label = _("Title")
-        template = 'wagtail_cblocks/heading_block.html'
+        template = "wagtail_cblocks/heading_block.html"
         value_class = HeadingValue
 
 
 class ParagraphBlock(wagtail_blocks.RichTextBlock):
     """
     A paragraph with simple or customized features.
     """
 
-    features = ('bold', 'italic', 'ol', 'ul', 'hr', 'link', 'document-link')
+    features = ("bold", "italic", "ol", "ul", "hr", "link", "document-link")
 
     def __init__(self, features=None, **kwargs):
         if features is None:
             features = self.features
         return super().__init__(features=features, **kwargs)
 
     class Meta:
-        icon = 'pilcrow'
+        icon = "pilcrow"
         label = _("Paragraph")
-        template = 'wagtail_cblocks/paragraph_block.html'
+        template = "wagtail_cblocks/paragraph_block.html"
 
 
 # LINK AND BUTTONS
 # ------------------------------------------------------------------------------
 
 
 class LinkTargetBlock(wagtail_blocks.StreamBlock):
     """
     The target of a link, used by `LinkBlock`.
     """
 
     page = wagtail_blocks.PageChooserBlock(
-        label=_("Page"), icon='doc-empty-inverse'
+        label=_("Page"), icon="doc-empty-inverse"
     )
-    document = DocumentChooserBlock(label=_("Document"), icon='doc-full')
+    document = DocumentChooserBlock(label=_("Document"), icon="doc-full")
     image = ImageChooserBlock(label=_("Image"))
     url = wagtail_blocks.URLBlock(label=_("External link"))
     anchor = wagtail_blocks.CharBlock(
         label=_("Anchor link"),
-        help_text=mark_safe(
+        help_text=mark_safe(  # noqa: S308
             _(
                 "An anchor in the current page, for example: "
                 "<code>#target-id</code>."
             )
         ),
     )
 
     def set_name(self, name):
         # Do not generate a label from the name as Block.set_name does
         self.name = name
 
     class Meta:
-        icon = 'link'
+        icon = "link"
         max_num = 1
-        form_classname = 'link-target-block'
+        form_classname = "link-target-block"
 
 
 class LinkValue(wagtail_blocks.StructValue):
     @cached_property
     def href(self):
         """Return the URL of the chosen target or `None` if it is undefined."""
         try:
-            child_value = self['target'][0].value
+            child_value = self["target"][0].value
         except (IndexError, KeyError):
             return None
-        if hasattr(child_value, 'file') and hasattr(child_value.file, 'url'):
+        if hasattr(child_value, "file") and hasattr(child_value.file, "url"):
             href = child_value.file.url
-        elif hasattr(child_value, 'url'):
+        elif hasattr(child_value, "url"):
             href = child_value.url
         else:
             href = child_value
         return href
 
 
 class LinkBlock(wagtail_blocks.StructBlock):
     """
     A link with a target chosen from a range of types - i.e. a page, an URL.
     """
 
     class Meta:
-        icon = 'link'
+        icon = "link"
         label = _("Link")
         value_class = LinkValue
-        form_classname = 'link-block'
-        form_template = 'wagtail_cblocks/block_forms/link_block.html'
+        form_classname = "link-block"
+        form_template = "wagtail_cblocks/block_forms/link_block.html"
 
     def __init__(self, *args, required=True, **kwargs):
         super().__init__(*args, required=required, **kwargs)
 
         target = LinkTargetBlock(required=required)
-        target.set_name('target')
+        target.set_name("target")
 
-        self.child_blocks['target'] = target
+        self.child_blocks["target"] = target
 
     @property
     def required(self):
         return self.meta.required
 
 
 class ButtonBlock(StylizedStructBlock):
@@ -240,17 +240,17 @@
     A button which acts like a link.
     """
 
     text = wagtail_blocks.CharBlock(label=_("Text"))
     link = LinkBlock()
 
     class Meta:
-        icon = 'link'
+        icon = "link"
         label = _("Button")
-        template = 'wagtail_cblocks/button_block.html'
+        template = "wagtail_cblocks/button_block.html"
 
 
 # IMAGES
 # ------------------------------------------------------------------------------
 
 
 class ImageBlock(wagtail_blocks.StructBlock):
@@ -259,26 +259,26 @@
     """
 
     image = ImageChooserBlock(label=_("Image"))
     caption = wagtail_blocks.CharBlock(required=False, label=_("Caption"))
     link = LinkBlock(required=False)
 
     class Meta:
-        icon = 'image'
+        icon = "image"
         label = _("Image")
-        template = 'wagtail_cblocks/image_block.html'
+        template = "wagtail_cblocks/image_block.html"
 
 
 # LAYOUT
 # ------------------------------------------------------------------------------
 
 HORIZONTAL_ALIGNMENTS = [
-    ('start', _("Left")),
-    ('center', _("Center")),
-    ('end', _("Right")),
+    ("start", _("Left")),
+    ("center", _("Center")),
+    ("end", _("Right")),
 ]
 HORIZONTAL_ALIGNMENT_DEFAULT = None
 
 
 class ColumnsBlock(wagtail_blocks.StructBlock):
     """
     A list of columns which can be horizontally aligned.
@@ -288,31 +288,31 @@
         choices=HORIZONTAL_ALIGNMENTS,
         default=HORIZONTAL_ALIGNMENT_DEFAULT,
         required=False,
         label=_("Horizontal alignment"),
     )
 
     class Meta:
-        icon = 'table'
+        icon = "table"
         label = _("Columns")
-        template = 'wagtail_cblocks/columns_block.html'
+        template = "wagtail_cblocks/columns_block.html"
 
     def __init__(self, column_block=None, **kwargs):
         super().__init__(**kwargs)
 
         if column_block is None:
-            if not hasattr(self.meta, 'column_block'):
+            if not hasattr(self.meta, "column_block"):
                 raise ImproperlyConfigured(
                     "ColumnsBlock was not passed a 'column_block' object"
                 )
             column_block = self.meta.column_block
 
         columns = wagtail_blocks.ListBlock(
             column_block,
             collapsed=True,
-            form_classname='columns-block-list',
+            form_classname="columns-block-list",
             label=_("Columns"),
         )
-        columns.set_name('columns')
+        columns.set_name("columns")
 
-        self.child_blocks['columns'] = columns
-        self.child_blocks.move_to_end('columns', last=False)
+        self.child_blocks["columns"] = columns
+        self.child_blocks.move_to_end("columns", last=False)
```

### Comparing `wagtail_cblocks-0.4.1/wagtail_cblocks/factories.py` & `wagtail_cblocks-0.4.2/wagtail_cblocks/factories.py`

 * *Files identical despite different names*

### Comparing `wagtail_cblocks-0.4.1/wagtail_cblocks/locale/fr/LC_MESSAGES/django.mo` & `wagtail_cblocks-0.4.2/wagtail_cblocks/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_cblocks-0.4.1/wagtail_cblocks/locale/fr/LC_MESSAGES/django.po` & `wagtail_cblocks-0.4.2/wagtail_cblocks/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_cblocks-0.4.1/wagtail_cblocks/templates/wagtail_cblocks/block_forms/link_block.html` & `wagtail_cblocks-0.4.2/wagtail_cblocks/templates/wagtail_cblocks/block_forms/link_block.html`

 * *Files identical despite different names*

