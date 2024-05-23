# Comparing `tmp/swh.loader.svn-2.1.0.tar.gz` & `tmp/swh_loader_svn-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh.loader.svn-2.1.0.tar", last modified: Thu Mar 14 15:40:32 2024, max compression
+gzip compressed data, was "swh_loader_svn-2.2.0.tar", last modified: Thu May 23 09:03:10 2024, max compression
```

## Comparing `swh.loader.svn-2.1.0.tar` & `swh_loader_svn-2.2.0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-14 15:40:32.037064 swh.loader.svn-2.1.0/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      158 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      361 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)      943 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)       14 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3278 2024-03-14 15:40:32.037064 swh.loader.svn-2.1.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1254 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-14 15:40:32.017064 swh.loader.svn-2.1.0/bin/
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      552 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/bin/init-svn-repository.sh
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      761 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/bin/swh-svn
--rw-r--r--   0 jenkins    (115) jenkins    (120)      567 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-14 15:40:32.017064 swh.loader.svn-2.1.0/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-14 15:40:32.021064 swh.loader.svn-2.1.0/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-14 15:40:32.021064 swh.loader.svn-2.1.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      265 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6651 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/docs/swh-loader-svn.txt
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-14 15:40:32.021064 swh.loader.svn-2.1.0/install/
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      644 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/install/install-pysvn.sh
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      109 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/install/install-subvertpy.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)      465 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1804 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      281 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)       91 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      103 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      292 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/requirements.txt
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-14 15:40:32.021064 swh.loader.svn-2.1.0/resources/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      860 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/resources/svn.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-03-14 15:40:32.041064 swh.loader.svn-2.1.0/setup.cfg
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3483 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/setup.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5873 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/svn-lib-client-analysis.org
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-14 15:40:32.013064 swh.loader.svn-2.1.0/swh/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-14 15:40:32.013064 swh.loader.svn-2.1.0/swh/loader/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-14 15:40:32.025064 swh.loader.svn-2.1.0/swh/loader/svn/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      672 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2427 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/converters.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4070 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/directory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      667 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/exception.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9055 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/fast_crawler.cpp
--rw-r--r--   0 jenkins    (115) jenkins    (120)      515 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/fast_crawler.pyi
--rw-r--r--   0 jenkins    (115) jenkins    (120)    33376 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/loader.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/py.typed
--rw-r--r--   0 jenkins    (115) jenkins    (120)    31251 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/replay.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    25023 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/svn_repo.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1521 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/svn_retry.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1148 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tasks.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-14 15:40:32.029064 swh.loader.svn-2.1.0/swh/loader/svn/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2690 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-14 15:40:32.033064 swh.loader.svn-2.1.0/swh/loader/svn/tests/data/
--rw-r--r--   0 jenkins    (115) jenkins    (120)   360057 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/data/httthttt.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)   389343 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/data/mediawiki-repo-r407-eol-native-crlf.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)      201 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/data/penguinsdbtools2018.dump.gz
--rw-r--r--   0 jenkins    (115) jenkins    (120)   419840 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/data/pkg-doc-linux-r10.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)   430080 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/data/pkg-doc-linux-r11.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)   911360 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/data/pkg-doc-linux-r12.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)    28495 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/data/pkg-gourmet-add-remove-dir.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)   133120 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/data/pkg-gourmet-tampered-rev6-log.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)   163840 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/data/pkg-gourmet-with-edge-case-links-and-files.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35440 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/data/pkg-gourmet-with-external-id.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)    30908 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/data/pkg-gourmet-with-updates.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)   163840 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/data/pkg-gourmet-with-wrong-link-cases.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)    28193 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/data/pkg-gourmet.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)   406052 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/data/pyang-repo-r343-eol-native-mixed-lf-crlf.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3985 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/test_converters.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7312 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/test_directory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    68855 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/test_externals.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2370 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/test_fast_crawler.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    17874 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/test_loader.org
--rw-r--r--   0 jenkins    (115) jenkins    (120)    79831 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/test_loader.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4415 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/test_svn_repo.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12995 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/test_svn_retry.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1114 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/test_task.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1469 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/test_task_directory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      459 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/test_tasks.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    21409 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3734 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/tests/utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    16766 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/swh/loader/svn/utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-14 15:40:32.037064 swh.loader.svn-2.1.0/swh.loader.svn.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3278 2024-03-14 15:40:31.000000 swh.loader.svn-2.1.0/swh.loader.svn.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2476 2024-03-14 15:40:32.000000 swh.loader.svn-2.1.0/swh.loader.svn.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-03-14 15:40:31.000000 swh.loader.svn-2.1.0/swh.loader.svn.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      102 2024-03-14 15:40:31.000000 swh.loader.svn-2.1.0/swh.loader.svn.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      402 2024-03-14 15:40:31.000000 swh.loader.svn-2.1.0/swh.loader.svn.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-03-14 15:40:31.000000 swh.loader.svn-2.1.0/swh.loader.svn.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1390 2024-03-14 15:40:25.000000 swh.loader.svn-2.1.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 09:03:10.543994 swh_loader_svn-2.2.0/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      158 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      361 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1385 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       14 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3348 2024-05-23 09:03:10.543994 swh_loader_svn-2.2.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1254 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 09:03:10.511995 swh_loader_svn-2.2.0/bin/
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      552 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/bin/init-svn-repository.sh
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      761 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/bin/swh-svn
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      567 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 09:03:10.511995 swh_loader_svn-2.2.0/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 09:03:10.511995 swh_loader_svn-2.2.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 09:03:10.511995 swh_loader_svn-2.2.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      265 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6651 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/docs/swh-loader-svn.txt
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 09:03:10.515995 swh_loader_svn-2.2.0/install/
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      644 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/install/install-pysvn.sh
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      109 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/install/install-subvertpy.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      465 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1861 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      282 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       92 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      138 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      292 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/requirements.txt
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 09:03:10.515995 swh_loader_svn-2.2.0/resources/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      860 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/resources/svn.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-05-23 09:03:10.543994 swh_loader_svn-2.2.0/setup.cfg
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3483 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/setup.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5873 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/svn-lib-client-analysis.org
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 09:03:10.503995 swh_loader_svn-2.2.0/swh/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 09:03:10.503995 swh_loader_svn-2.2.0/swh/loader/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 09:03:10.523995 swh_loader_svn-2.2.0/swh/loader/svn/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      860 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2427 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/converters.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4094 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/directory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      667 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/exception.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9055 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/fast_crawler.cpp
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      515 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/fast_crawler.pyi
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    33352 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/loader.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/py.typed
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    31295 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/replay.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    25023 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/svn_repo.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1521 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/svn_retry.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1148 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tasks.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 09:03:10.527994 swh_loader_svn-2.2.0/swh/loader/svn/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3657 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 09:03:10.535994 swh_loader_svn-2.2.0/swh/loader/svn/tests/data/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)   360057 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/data/httthttt.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)   389343 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/data/mediawiki-repo-r407-eol-native-crlf.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      201 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/data/penguinsdbtools2018.dump.gz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)   419840 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/data/pkg-doc-linux-r10.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)   430080 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/data/pkg-doc-linux-r11.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)   911360 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/data/pkg-doc-linux-r12.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    28495 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/data/pkg-gourmet-add-remove-dir.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)   133120 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/data/pkg-gourmet-tampered-rev6-log.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)   163840 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/data/pkg-gourmet-with-edge-case-links-and-files.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35440 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/data/pkg-gourmet-with-external-id.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    30908 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/data/pkg-gourmet-with-updates.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)   163840 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/data/pkg-gourmet-with-wrong-link-cases.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    28193 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/data/pkg-gourmet.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)   406052 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/data/pyang-repo-r343-eol-native-mixed-lf-crlf.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3985 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/test_converters.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7312 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/test_directory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    71588 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/test_externals.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2370 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/test_fast_crawler.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    17874 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/test_loader.org
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    79879 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/test_loader.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4415 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/test_svn_repo.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12995 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/test_svn_retry.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1114 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/test_task.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1469 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/test_task_directory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      459 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/test_tasks.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    21409 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3734 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/tests/utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    16766 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/swh/loader/svn/utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 09:03:10.539994 swh_loader_svn-2.2.0/swh.loader.svn.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3348 2024-05-23 09:03:10.000000 swh_loader_svn-2.2.0/swh.loader.svn.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2476 2024-05-23 09:03:10.000000 swh_loader_svn-2.2.0/swh.loader.svn.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-05-23 09:03:10.000000 swh_loader_svn-2.2.0/swh.loader.svn.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      155 2024-05-23 09:03:10.000000 swh_loader_svn-2.2.0/swh.loader.svn.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      437 2024-05-23 09:03:10.000000 swh_loader_svn-2.2.0/swh.loader.svn.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-05-23 09:03:10.000000 swh_loader_svn-2.2.0/swh.loader.svn.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1120 2024-05-23 09:03:04.000000 swh_loader_svn-2.2.0/tox.ini
```

### Comparing `swh.loader.svn-2.1.0/CODE_OF_CONDUCT.md` & `swh_loader_svn-2.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/LICENSE` & `swh_loader_svn-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/PKG-INFO` & `swh_loader_svn-2.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.svn
-Version: 2.1.0
+Version: 2.2.0
 Summary: Software Heritage Loader SVN
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-loader-svn
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-loader-svn/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-loader-svn/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-loader-svn.git
@@ -19,31 +19,32 @@
 License-File: AUTHORS
 Requires-Dist: click
 Requires-Dist: iso8601
 Requires-Dist: subvertpy>=0.9.4
 Requires-Dist: tenacity>=6.2
 Requires-Dist: typing-extensions
 Requires-Dist: swh.storage>=0.11.3
-Requires-Dist: swh.model>=6.6.0
+Requires-Dist: swh.model>=6.13.0
 Requires-Dist: swh.scheduler>=0.0.39
 Requires-Dist: swh.loader.core>=5.14.2
 Provides-Extra: testing
 Requires-Dist: click; extra == "testing"
 Requires-Dist: iso8601; extra == "testing"
 Requires-Dist: subvertpy>=0.9.4; extra == "testing"
 Requires-Dist: tenacity>=6.2; extra == "testing"
 Requires-Dist: typing-extensions; extra == "testing"
 Requires-Dist: swh.storage>=0.11.3; extra == "testing"
-Requires-Dist: swh.model>=6.6.0; extra == "testing"
+Requires-Dist: swh.model>=6.13.0; extra == "testing"
 Requires-Dist: swh.scheduler>=0.0.39; extra == "testing"
 Requires-Dist: swh.loader.core>=5.14.2; extra == "testing"
 Requires-Dist: pytest>=8.1; extra == "testing"
 Requires-Dist: pytest-mock; extra == "testing"
 Requires-Dist: pytest-postgresql; extra == "testing"
 Requires-Dist: swh.core[http]>=0.0.61; extra == "testing"
+Requires-Dist: swh.loader.core[testing]>=5.18.0; extra == "testing"
 Requires-Dist: types-click; extra == "testing"
 Requires-Dist: types-python-dateutil; extra == "testing"
 
 Software Heritage - Subversion loader |build status|
 ====================================================
 
 .. |build status| image:: https://jenkins.softwareheritage.org/job/DLDSVN/job/master/badge/icon
```

### Comparing `swh.loader.svn-2.1.0/README.rst` & `swh_loader_svn-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/bin/init-svn-repository.sh` & `swh_loader_svn-2.2.0/bin/init-svn-repository.sh`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/bin/swh-svn` & `swh_loader_svn-2.2.0/bin/swh-svn`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/conftest.py` & `swh_loader_svn-2.2.0/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/docs/swh-loader-svn.txt` & `swh_loader_svn-2.2.0/docs/swh-loader-svn.txt`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/install/install-pysvn.sh` & `swh_loader_svn-2.2.0/install/install-pysvn.sh`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/pyproject.toml` & `swh_loader_svn-2.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 [tool.setuptools.dynamic.optional-dependencies]
 testing = {file = ["requirements.txt", "requirements-swh.txt", "requirements-test.txt"]}
 
 [project.entry-points."swh.workers"]
 "loader.svn" = "swh.loader.svn:register"
 "loader.svn-export" = "swh.loader.svn:register_export"
+"loader.svn-no-dump" = "swh.loader.svn:register_no_dump"
 
 [project.urls]
 "Homepage" = "https://gitlab.softwareheritage.org/swh/devel/swh-loader-svn"
 "Bug Reports" = "https://gitlab.softwareheritage.org/swh/devel/swh-loader-svn/-/issues"
 "Funding" = "https://www.softwareheritage.org/donate"
 "Documentation" = "https://docs.softwareheritage.org/devel/swh-loader-svn/"
 "Source" = "https://gitlab.softwareheritage.org/swh/devel/swh-loader-svn.git"
```

### Comparing `swh.loader.svn-2.1.0/resources/svn.ini` & `swh_loader_svn-2.2.0/resources/svn.ini`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/setup.py` & `swh_loader_svn-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/svn-lib-client-analysis.org` & `swh_loader_svn-2.2.0/svn-lib-client-analysis.org`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/__init__.py` & `swh_loader_svn-2.2.0/swh/loader/svn/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,7 +18,16 @@
 def register_export() -> Dict[str, Any]:
     from swh.loader.svn.directory import SvnExportLoader
 
     return {
         "task_modules": [],
         "loader": SvnExportLoader,
     }
+
+
+def register_no_dump() -> Dict[str, Any]:
+    from swh.loader.svn.loader import SvnLoader
+
+    return {
+        "task_modules": [f"{__name__}.tasks"],
+        "loader": SvnLoader,
+    }
```

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/converters.py` & `swh_loader_svn-2.2.0/swh/loader/svn/converters.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/directory.py` & `swh_loader_svn-2.2.0/swh/loader/svn/directory.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import os
 from pathlib import Path
 import tempfile
 from typing import Iterator, List, Optional
 
 from swh.loader.core.loader import BaseDirectoryLoader
 from swh.loader.svn.svn_repo import SvnRepo, get_svn_repo
-from swh.model.model import Snapshot, SnapshotBranch, TargetType
+from swh.model.model import Snapshot, SnapshotBranch, SnapshotTargetType
 
 
 class SvnExportLoader(BaseDirectoryLoader):
     """Load a svn tree at a specific svn revision into the swh archive.
 
     It is also possible to load a subset of the source tree by explicitly
     specifying the sub-paths to export in the ``svn_paths`` optional parameter.
@@ -103,16 +103,16 @@
     def build_snapshot(self) -> Snapshot:
         """Build snapshot without losing the svn revision context."""
         assert self.directory is not None
         branch_name = f"rev_{self.svn_revision}".encode()
         return Snapshot(
             branches={
                 b"HEAD": SnapshotBranch(
-                    target_type=TargetType.ALIAS,
+                    target_type=SnapshotTargetType.ALIAS,
                     target=branch_name,
                 ),
                 branch_name: SnapshotBranch(
-                    target_type=TargetType.DIRECTORY,
+                    target_type=SnapshotTargetType.DIRECTORY,
                     target=self.directory.hash,
                 ),
             }
         )
```

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/exception.py` & `swh_loader_svn-2.2.0/swh/loader/svn/exception.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/fast_crawler.cpp` & `swh_loader_svn-2.2.0/swh/loader/svn/fast_crawler.cpp`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/fast_crawler.pyi` & `swh_loader_svn-2.2.0/swh/loader/svn/fast_crawler.pyi`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/loader.py` & `swh_loader_svn-2.2.0/swh/loader/svn/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from swh.model.model import (
     Content,
     Directory,
     Revision,
     SkippedContent,
     Snapshot,
     SnapshotBranch,
-    TargetType,
+    SnapshotTargetType,
 )
 from swh.storage.algos.snapshot import snapshot_get_latest
 from swh.storage.interface import StorageInterface
 
 from . import converters
 from .exception import SvnLoaderHistoryAltered, SvnLoaderUneventful
 from .utils import (
@@ -179,15 +179,15 @@
             return None
         branches = latest_snapshot.branches
         if not branches:
             return None
         branch = branches.get(DEFAULT_BRANCH)
         if not branch:
             return None
-        if branch.target_type != TargetType.REVISION:
+        if branch.target_type != SnapshotTargetType.REVISION:
             return None
         swh_id = branch.target
 
         revision = storage.revision_get([swh_id])[0]
         if not revision:
             return None
         return latest_snapshot, revision
@@ -320,24 +320,24 @@
                     path = obj.data["path"].replace(checked_dir.data["path"], b"")
                     if not path:
                         # ignore root directory
                         continue
                     if path not in dir:
                         self.log.debug(
                             "%s with path %s is missing in reconstructed repository filesystem",
-                            obj.object_type,  # type: ignore
+                            obj.object_type,
                             path,
                         )
                     elif dir[path].hash != checked_dir[path].hash:
                         self.log.debug(
                             "%s with path %s has different hash in reconstructed repository filesystem",  # noqa
-                            obj.object_type,  # type: ignore
+                            obj.object_type,
                             path,
                         )
-                        if obj.object_type == "content":  # type: ignore
+                        if obj.object_type == "content":
                             self.log.debug(
                                 "expected sha1: %s, actual sha1: %s",
                                 hashutil.hash_to_hex(checked_dir[path].data["sha1"]),
                                 hashutil.hash_to_hex(dir[path].data["sha1"]),
                             )
                             # compute and display diff between contents
                             file_path = (
@@ -558,15 +558,15 @@
             Optional[Snapshot] The newly created snapshot
 
         """
         if revision:  # Priority to the revision
             snap = Snapshot(
                 branches={
                     DEFAULT_BRANCH: SnapshotBranch(
-                        target=revision.id, target_type=TargetType.REVISION
+                        target=revision.id, target_type=SnapshotTargetType.REVISION
                     )
                 }
             )
         elif snapshot:  # Fallback to prior snapshot
             snap = snapshot
         else:
             raise ValueError(
```

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/replay.py` & `swh_loader_svn-2.2.0/swh/loader/svn/replay.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     cast,
 )
 
 from subvertpy import SubversionException, properties
 from subvertpy.ra import RemoteAccess
 
 from swh.model import from_disk
-from swh.model.from_disk import DiskBackedContent
 from swh.model.model import Content, Directory, SkippedContent
 
 if TYPE_CHECKING:
     from swh.loader.svn.svn_repo import SvnRepo
 
 from swh.loader.svn.utils import (
     ExternalDefinition,
@@ -408,26 +407,28 @@
                 self.remove_external_path(
                     external_path,
                     root_path=path_bytes,
                     remove_subpaths=False,
                     force=True,
                 )
 
-        if path_bytes not in self.editor.external_paths:
-            self.remove_child(path_bytes)
-        elif os.path.isdir(fullpath):
+        if os.path.isdir(fullpath):
             # versioned and external paths can overlap so we need to iterate on
-            # all subpaths to check which ones to remove
-            for root, dirs, files in os.walk(fullpath):
+            # all subpaths to check which ones to remove, paths are iterated in
+            # a bottom-up manner to ensure all related dir states are removed
+            for root, dirs, files in os.walk(fullpath, topdown=False):
                 for p in chain(dirs, files):
                     full_repo_path = os.path.join(root, p)
                     repo_path = full_repo_path.replace(self.rootpath + b"/", b"")
                     if repo_path not in self.editor.external_paths:
                         self.remove_child(repo_path)
 
+        if path_bytes not in self.editor.external_paths:
+            self.remove_child(path_bytes)
+
     def close(self):
         """Function called when we finish processing a repository.
 
         SVN external definitions are processed by it.
         """
         if self.editor.debug:
             logger.debug("Closing directory %s", self.path)
@@ -659,17 +660,17 @@
                             for p in chain(dirs, files)
                         ]
                     )
 
                 self.dir_states[self.path].externals_paths.update(external_paths)
 
                 for external_path in external_paths:
-                    self.editor.external_paths[
+                    self.editor.external_paths.add(
                         os.path.join(self.path, external_path)
-                    ] += 1
+                    )
 
             # ensure hash update for the directory with externals set
             self.directory[self.path].update_hash(force=True)
 
     def remove_external_path(
         self,
         external_path: bytes,
@@ -682,35 +683,37 @@
         """
         path = root_path if root_path else self.path
         fullpath = os.path.join(path, external_path)
 
         if self.editor.debug:
             logger.debug("Removing external path %s", fullpath)
 
-        # decrement number of references for external path when we really remove it
-        # (when remove_subpaths is False, we just cleanup the external path before
-        # copying exported paths in it)
-        if force or (fullpath in self.editor.external_paths and remove_subpaths):
-            self.editor.external_paths[fullpath] -= 1
+        can_remove_external = True
+        subpath_split = fullpath.split(b"/")[:-1]
+        # check there is no overlapping external set in ancestor directories
+        # and mark current external not to be removed if it is the case
+        for i in reversed(range(1, len(subpath_split))):
+            subpath = b"/".join(subpath_split[0:i])
+            subdir_state = self.editor.dir_states.get(subpath)
+            if subdir_state and fullpath in {
+                os.path.join(subpath, ext_path)
+                for ext_path in subdir_state.externals_paths
+            }:
+                can_remove_external = False
+                break
 
-        if (
-            fullpath in self.editor.external_paths
-            and self.editor.external_paths[fullpath] == 0
-        ):
+        if force or can_remove_external:
             self.remove_child(fullpath)
-            self.editor.external_paths.pop(fullpath, None)
+            self.editor.external_paths.discard(fullpath)
             self.editor.valid_externals.pop(fullpath, None)
             for path in list(self.editor.external_paths):
                 if path.startswith(fullpath + b"/"):
-                    self.editor.external_paths[path] -= 1
-                    if self.editor.external_paths[path] == 0:
-                        self.editor.external_paths.pop(path)
+                    self.editor.external_paths.remove(path)
 
         if remove_subpaths:
-            subpath_split = fullpath.split(b"/")[:-1]
             for i in reversed(range(1, len(subpath_split) + 1)):
                 # delete external sub-directory only if it is not versioned
                 subpath = b"/".join(subpath_split[0:i])
                 try:
                     self.svnrepo.info(
                         svn_urljoin(self.svnrepo.repos_root_url, os.fsdecode(subpath)),
                         peg_revision=self.editor.revnum,
@@ -757,15 +760,15 @@
         svnrepo: SvnRepo,
         temp_dir: str,
         debug: bool = False,
     ):
         self.rootpath = rootpath
         self.directory = directory
         self.dir_states: Dict[bytes, DirState] = defaultdict(DirState)
-        self.external_paths: Dict[bytes, int] = defaultdict(int)
+        self.external_paths: Set[bytes] = set()
         self.valid_externals: Dict[bytes, Tuple[str, bool]] = {}
         self.dead_externals: Set[Tuple[str, Optional[int], Optional[int], bool]] = set()
         self.externals_cache_dir = tempfile.mkdtemp(dir=temp_dir)
         self.externals_cache: Dict[ExternalDefinition, bytes] = {}
         self.svnrepo = svnrepo
         self.revnum = -1
         self.debug = debug
@@ -848,15 +851,15 @@
         contents: List[Content] = []
         skipped_contents: List[SkippedContent] = []
         directories: List[Directory] = []
 
         for obj_node in self.directory.collect():
             obj = obj_node.to_model()  # type: ignore
             obj_type = obj.object_type
-            if obj_type in (Content.object_type, DiskBackedContent.object_type):
+            if obj_type == Content.object_type:
                 contents.append(obj.with_data())
             elif obj_type == SkippedContent.object_type:
                 skipped_contents.append(obj)
             elif obj_type == Directory.object_type:
                 directories.append(obj)
             else:
                 assert False, obj_type
```

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/svn_repo.py` & `swh_loader_svn-2.2.0/swh/loader/svn/svn_repo.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/svn_retry.py` & `swh_loader_svn-2.2.0/swh/loader/svn/svn_retry.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tasks.py` & `swh_loader_svn-2.2.0/swh/loader/svn/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/data/httthttt.tgz` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/data/httthttt.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/data/mediawiki-repo-r407-eol-native-crlf.tgz` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/data/mediawiki-repo-r407-eol-native-crlf.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/data/pkg-doc-linux-r10.tgz` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/data/pkg-doc-linux-r10.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/data/pkg-doc-linux-r11.tgz` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/data/pkg-doc-linux-r11.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/data/pkg-doc-linux-r12.tgz` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/data/pkg-doc-linux-r12.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/data/pkg-gourmet-add-remove-dir.tgz` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/data/pkg-gourmet-add-remove-dir.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/data/pkg-gourmet-tampered-rev6-log.tgz` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/data/pkg-gourmet-tampered-rev6-log.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/data/pkg-gourmet-with-edge-case-links-and-files.tgz` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/data/pkg-gourmet-with-edge-case-links-and-files.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/data/pkg-gourmet-with-external-id.tgz` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/data/pkg-gourmet-with-external-id.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/data/pkg-gourmet-with-updates.tgz` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/data/pkg-gourmet-with-updates.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/data/pkg-gourmet-with-wrong-link-cases.tgz` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/data/pkg-gourmet-with-wrong-link-cases.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/data/pkg-gourmet.tgz` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/data/pkg-gourmet.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/data/pyang-repo-r343-eol-native-mixed-lf-crlf.tgz` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/data/pyang-repo-r343-eol-native-mixed-lf-crlf.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/test_converters.py` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/test_directory.py` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/test_externals.py` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/test_externals.py`

 * *Files 1% similar despite different names*

```diff
@@ -2480,7 +2480,103 @@
     assert_last_visit_matches(
         loader.storage,
         repo_url,
         status="full",
         type="svn",
     )
     check_snapshot(loader.snapshot, loader.storage)
+
+
+def test_loader_svn_externals_replace(
+    svn_loader_cls, swh_storage, repo_url, external_repo_url, tmp_path
+):
+    # first commit on external
+    add_commit(
+        external_repo_url,
+        "Create some directories and files in an external repository",
+        [
+            CommitChange(
+                change_type=CommitChangeType.AddOrUpdate,
+                path="code/hello/hello-world",
+                properties={"svn:executable": "*"},
+                data=b"#!/bin/bash\necho Hello World !",
+            ),
+            CommitChange(
+                change_type=CommitChangeType.AddOrUpdate,
+                path="code/foo/foo.sh",
+                properties={"svn:executable": "*"},
+                data=b"#!/bin/bash\necho foo",
+            ),
+        ],
+    )
+
+    add_commit(
+        repo_url,
+        (
+            "Set trunk/externals/bin external targeting code/hello directory "
+            "in external repository"
+        ),
+        [
+            CommitChange(
+                change_type=CommitChangeType.AddOrUpdate,
+                path="trunk/externals/",
+                properties={
+                    "svn:externals": (
+                        f"{svn_urljoin(external_repo_url, 'code/hello')} bin\n"
+                    )
+                },
+            ),
+        ],
+    )
+
+    add_commit(
+        repo_url,
+        (
+            "Replace trunk/externals/bin external to target code/foo directory "
+            "in external repository"
+        ),
+        [
+            CommitChange(
+                change_type=CommitChangeType.AddOrUpdate,
+                path="trunk/externals/",
+                properties={
+                    "svn:externals": (
+                        f"{svn_urljoin(external_repo_url, 'code/foo')} bin\n"
+                    )
+                },
+            ),
+        ],
+    )
+
+    add_commit(
+        repo_url,
+        (
+            "Replace trunk/externals/bin external to target code/hello directory again "
+            "in external repository"
+        ),
+        [
+            CommitChange(
+                change_type=CommitChangeType.AddOrUpdate,
+                path="trunk/externals/",
+                properties={
+                    "svn:externals": (
+                        f"{svn_urljoin(external_repo_url, 'code/hello')} bin\n"
+                    )
+                },
+            ),
+        ],
+    )
+
+    loader = svn_loader_cls(
+        swh_storage,
+        repo_url,
+        temp_directory=tmp_path,
+        check_revision=1,
+    )
+    assert loader.load() == {"status": "eventful"}
+    assert_last_visit_matches(
+        loader.storage,
+        repo_url,
+        status="full",
+        type="svn",
+    )
+    check_snapshot(loader.snapshot, loader.storage)
```

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/test_fast_crawler.py` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/test_fast_crawler.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/test_loader.org` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/test_loader.org`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/test_loader.py` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/test_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2016-2023  The Software Heritage developers
+# Copyright (C) 2016-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import itertools
 import logging
 import os
@@ -25,34 +25,34 @@
     assert_last_visit_matches,
     check_snapshot,
     get_stats,
     prepare_repository_from_archive,
 )
 from swh.model.from_disk import DentryPerms, Directory
 from swh.model.hashutil import hash_to_bytes
-from swh.model.model import Snapshot, SnapshotBranch, TargetType
+from swh.model.model import Snapshot, SnapshotBranch, SnapshotTargetType
 
 from .utils import CommitChange, CommitChangeType, add_commit
 
 GOURMET_SNAPSHOT = Snapshot(
     id=hash_to_bytes("889cacc2731e3312abfb2b1a0c18ade82a949e07"),
     branches={
         b"HEAD": SnapshotBranch(
             target=hash_to_bytes("4876cb10aec6f708f7466dddf547567b65f6c39c"),
-            target_type=TargetType.REVISION,
+            target_type=SnapshotTargetType.REVISION,
         )
     },
 )
 
 GOURMET_UPDATES_SNAPSHOT = Snapshot(
     id=hash_to_bytes("11086d15317014e43d2438b7ffc712c44f1b8afe"),
     branches={
         b"HEAD": SnapshotBranch(
             target=hash_to_bytes("171dc35522bfd17dda4e90a542a0377fb2fc707a"),
-            target_type=TargetType.REVISION,
+            target_type=SnapshotTargetType.REVISION,
         )
     },
 )
 
 
 def test_loader_svn_not_found_no_mock(svn_loader_cls, swh_storage, tmp_path):
     """Given an unknown repository, the loader visit ends up in status not_found"""
@@ -521,15 +521,15 @@
 
     assert loader.load() == {"status": "eventful"}
     mediawiki_snapshot = Snapshot(
         id=hash_to_bytes("d6d6e9703f157c5702d9a4a5dec878926ed4ab76"),
         branches={
             b"HEAD": SnapshotBranch(
                 target=hash_to_bytes("7da4975c363101b819756d33459f30a866d01b1b"),
-                target_type=TargetType.REVISION,
+                target_type=SnapshotTargetType.REVISION,
             )
         },
     )
     check_snapshot(mediawiki_snapshot, loader.storage)
 
     assert_last_visit_matches(
         loader.storage,
@@ -563,15 +563,15 @@
 
     assert loader.load() == {"status": "eventful"}
     pyang_snapshot = Snapshot(
         id=hash_to_bytes("6d9590de11b00a5801de0ff3297c5b44bbbf7d24"),
         branches={
             b"HEAD": SnapshotBranch(
                 target=hash_to_bytes("9c6962eeb9164a636c374be700672355e34a98a7"),
-                target_type=TargetType.REVISION,
+                target_type=SnapshotTargetType.REVISION,
             )
         },
     )
     check_snapshot(pyang_snapshot, loader.storage)
 
     assert_last_visit_matches(
         loader.storage,
@@ -606,15 +606,15 @@
 
     assert loader.load() == {"status": "eventful"}
     gourmet_edge_cases_snapshot = Snapshot(
         id=hash_to_bytes("18e60982fe521a2546ab8c3c73a535d80462d9d0"),
         branches={
             b"HEAD": SnapshotBranch(
                 target=hash_to_bytes("3f43af2578fccf18b0d4198e48563da7929dc608"),
-                target_type=TargetType.REVISION,
+                target_type=SnapshotTargetType.REVISION,
             )
         },
     )
     check_snapshot(gourmet_edge_cases_snapshot, loader.storage)
 
     assert_last_visit_matches(
         loader.storage,
@@ -647,15 +647,15 @@
 
     assert loader.load() == {"status": "eventful"}
     gourmet_wrong_links_snapshot = Snapshot(
         id=hash_to_bytes("b17f38acabb90f066dedd30c29f01a02af88a5c4"),
         branches={
             b"HEAD": SnapshotBranch(
                 target=hash_to_bytes("cf30d3bb9d5967d0a2bbeacc405f10a5dd9b138a"),
-                target_type=TargetType.REVISION,
+                target_type=SnapshotTargetType.REVISION,
             )
         },
     )
     check_snapshot(gourmet_wrong_links_snapshot, loader.storage)
 
     assert_last_visit_matches(
         loader.storage,
@@ -906,15 +906,15 @@
 
     assert loader.load() == {"status": "eventful"}
     expected_snapshot = Snapshot(
         id=hash_to_bytes("70487267f682c07e52a2371061369b6cf5bffa47"),
         branches={
             b"HEAD": SnapshotBranch(
                 target=hash_to_bytes("604a17dbb15e8d7ecb3e9f3768d09bf493667a93"),
-                target_type=TargetType.REVISION,
+                target_type=SnapshotTargetType.REVISION,
             )
         },
     )
     check_snapshot(expected_snapshot, loader.storage)
 
     assert_last_visit_matches(
         loader.storage,
@@ -2186,17 +2186,14 @@
     )
 
     # compute repo URLs that will be made available by svnserve
     repo_path = repo_url.replace("file://", "")
     repo_root = os.path.dirname(repo_path)
     repo_name = os.path.basename(repo_path)
     username, password = credentials
-    port = 12000
-    repo_url_no_auth = f"svn://localhost:{port}/{repo_name}"
-    repo_url = f"svn://{username}:{password}@localhost:{port}/{repo_name}"
 
     # disable anonymous access and require authentication on test repo
     with open(os.path.join(repo_path, "conf", "svnserve.conf"), "w") as svnserve_conf:
         svnserve_conf.write(
             textwrap.dedent(
                 """
                 [general]
@@ -2215,15 +2212,17 @@
         )
 
     # add a user with read/write access on test repo
     with open(os.path.join(repo_path, "conf", "passwd"), "w") as passwd:
         passwd.write(f"[users]\n{username} = {password}")
 
     # execute svnserve
-    svnserve(repo_root, port)
+    port = svnserve(repo_root)
+    repo_url_no_auth = f"svn://localhost:{port}/{repo_name}"
+    repo_url = f"svn://{username}:{password}@localhost:{port}/{repo_name}"
 
     # check loading failed with no authentication in URL apart for anonymous credentials
     loader = svn_loader_cls(swh_storage, repo_url_no_auth, temp_directory=tmp_path)
     assert (
         loader.load() == {"status": "uneventful"}
         if username != "anonymous"
         else {"status": "eventful"}
```

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/test_svn_repo.py` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/test_svn_repo.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/test_svn_retry.py` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/test_svn_retry.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/test_task.py` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/test_task_directory.py` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/test_task_directory.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/test_utils.py` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/tests/utils.py` & `swh_loader_svn-2.2.0/swh/loader/svn/tests/utils.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh/loader/svn/utils.py` & `swh_loader_svn-2.2.0/swh/loader/svn/utils.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/swh.loader.svn.egg-info/PKG-INFO` & `swh_loader_svn-2.2.0/swh.loader.svn.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.svn
-Version: 2.1.0
+Version: 2.2.0
 Summary: Software Heritage Loader SVN
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-loader-svn
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-loader-svn/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-loader-svn/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-loader-svn.git
@@ -19,31 +19,32 @@
 License-File: AUTHORS
 Requires-Dist: click
 Requires-Dist: iso8601
 Requires-Dist: subvertpy>=0.9.4
 Requires-Dist: tenacity>=6.2
 Requires-Dist: typing-extensions
 Requires-Dist: swh.storage>=0.11.3
-Requires-Dist: swh.model>=6.6.0
+Requires-Dist: swh.model>=6.13.0
 Requires-Dist: swh.scheduler>=0.0.39
 Requires-Dist: swh.loader.core>=5.14.2
 Provides-Extra: testing
 Requires-Dist: click; extra == "testing"
 Requires-Dist: iso8601; extra == "testing"
 Requires-Dist: subvertpy>=0.9.4; extra == "testing"
 Requires-Dist: tenacity>=6.2; extra == "testing"
 Requires-Dist: typing-extensions; extra == "testing"
 Requires-Dist: swh.storage>=0.11.3; extra == "testing"
-Requires-Dist: swh.model>=6.6.0; extra == "testing"
+Requires-Dist: swh.model>=6.13.0; extra == "testing"
 Requires-Dist: swh.scheduler>=0.0.39; extra == "testing"
 Requires-Dist: swh.loader.core>=5.14.2; extra == "testing"
 Requires-Dist: pytest>=8.1; extra == "testing"
 Requires-Dist: pytest-mock; extra == "testing"
 Requires-Dist: pytest-postgresql; extra == "testing"
 Requires-Dist: swh.core[http]>=0.0.61; extra == "testing"
+Requires-Dist: swh.loader.core[testing]>=5.18.0; extra == "testing"
 Requires-Dist: types-click; extra == "testing"
 Requires-Dist: types-python-dateutil; extra == "testing"
 
 Software Heritage - Subversion loader |build status|
 ====================================================
 
 .. |build status| image:: https://jenkins.softwareheritage.org/job/DLDSVN/job/master/badge/icon
```

### Comparing `swh.loader.svn-2.1.0/swh.loader.svn.egg-info/SOURCES.txt` & `swh_loader_svn-2.2.0/swh.loader.svn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-2.1.0/tox.ini` & `swh_loader_svn-2.2.0/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -3,30 +3,27 @@
 envlist =
   black
   flake8
   mypy
   py3
 
 [testenv]
+usedevelop = true
 extras =
   testing
 deps =
   pytest-cov
   swh.scheduler[testing] >= 0.5.0
   dev: pdbpp
 commands =
   pytest --doctest-modules \
-         --rootdir {envsitepackagesdir} \
-         --cov={envsitepackagesdir}/swh/loader/svn \
+         --cov=swh/loader/svn \
          --cov-branch \
-         {envsitepackagesdir}/swh/loader/svn \
+         swh/loader/svn \
          {posargs}
-# --rootdir (with --import-mode from pytest.ini) are required to make tests
-# that depends on the test file to be a proper submodule of the swh namespace
-# after migration to PEP420 (implicit namespace).
 
 [testenv:black]
 skip_install = true
 deps =
   black==23.1.0
 commands =
   {envpython} -m black --check swh
```

