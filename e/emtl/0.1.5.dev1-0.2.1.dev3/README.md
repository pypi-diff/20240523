# Comparing `tmp/emtl-0.1.5.dev1.tar.gz` & `tmp/emtl-0.2.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emtl-0.1.5.dev1.tar", last modified: Wed Apr 24 03:16:21 2024, max compression
+gzip compressed data, was "emtl-0.2.1.dev3.tar", last modified: Thu May 23 01:00:46 2024, max compression
```

## Comparing `emtl-0.1.5.dev1.tar` & `emtl-0.2.1.dev3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.076150 emtl-0.1.5.dev1/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      757 2024-04-19 03:14:30.000000 emtl-0.1.5.dev1/.bumpversion.cfg
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1906 2024-04-19 03:14:30.000000 emtl-0.1.5.dev1/.cookiecutterrc
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      149 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/.coveragerc
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      353 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/.editorconfig
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.056150 emtl-0.1.5.dev1/.github/
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.056150 emtl-0.1.5.dev1/.github/workflows/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      907 2024-04-19 01:18:25.000000 emtl-0.1.5.dev1/.github/workflows/document.yml
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     3925 2024-04-19 01:32:21.000000 emtl-0.1.5.dev1/.github/workflows/github-actions.yml
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      734 2024-04-16 01:37:37.000000 emtl-0.1.5.dev1/.gitignore
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      686 2024-04-16 01:27:59.000000 emtl-0.1.5.dev1/.pre-commit-config.yaml
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      285 2024-04-17 09:47:16.000000 emtl-0.1.5.dev1/.readthedocs.yml
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       65 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/AUTHORS.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      296 2024-04-19 03:09:42.000000 emtl-0.1.5.dev1/CHANGELOG.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2274 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/CONTRIBUTING.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1117 2024-04-16 01:42:17.000000 emtl-0.1.5.dev1/LICENSE
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2115 2024-04-24 03:16:21.076150 emtl-0.1.5.dev1/PKG-INFO
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2251 2024-04-19 03:14:30.000000 emtl-0.1.5.dev1/README.rst
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.066150 emtl-0.1.5.dev1/ci/
--rwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)     2867 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/ci/bootstrap.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       72 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/ci/requirements.txt
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.056150 emtl-0.1.5.dev1/ci/templates/
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.056150 emtl-0.1.5.dev1/ci/templates/.github/
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.066150 emtl-0.1.5.dev1/ci/templates/.github/workflows/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2179 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.066150 emtl-0.1.5.dev1/docs/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       28 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/docs/authors.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       30 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/docs/changelog.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1150 2024-04-19 03:14:30.000000 emtl-0.1.5.dev1/docs/conf.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       33 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/docs/contributing.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      244 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/docs/index.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       84 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/docs/installation.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       27 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/docs/readme.rst
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.066150 emtl-0.1.5.dev1/docs/reference/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      146 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/docs/reference/emtl.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       56 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/docs/reference/index.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       14 2024-04-19 02:32:39.000000 emtl-0.1.5.dev1/docs/requirements.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      109 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/docs/spelling_wordlist.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      157 2024-04-19 02:08:08.000000 emtl-0.1.5.dev1/docs/usage.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1381 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/pyproject.toml
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1303 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/pytest.ini
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       38 2024-04-24 03:16:21.076150 emtl-0.1.5.dev1/setup.cfg
--rwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)     3066 2024-04-19 03:14:30.000000 emtl-0.1.5.dev1/setup.py
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.056150 emtl-0.1.5.dev1/src/
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.066150 emtl-0.1.5.dev1/src/emtl/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      183 2024-04-19 03:14:30.000000 emtl-0.1.5.dev1/src/emtl/__init__.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      354 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/src/emtl/__main__.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      424 2024-04-24 03:16:20.000000 emtl-0.1.5.dev1/src/emtl/_version.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1003 2024-04-17 00:52:46.000000 emtl-0.1.5.dev1/src/emtl/cli.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1083 2024-04-17 03:52:39.000000 emtl-0.1.5.dev1/src/emtl/const.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     4376 2024-04-23 11:01:13.000000 emtl-0.1.5.dev1/src/emtl/core.py
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.066150 emtl-0.1.5.dev1/src/emtl/tests/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/src/emtl/tests/__init__.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      133 2024-04-17 01:52:16.000000 emtl-0.1.5.dev1/src/emtl/tests/test_cli.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      624 2024-04-19 01:18:25.000000 emtl-0.1.5.dev1/src/emtl/tests/test_core.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1585 2024-04-18 02:05:24.000000 emtl-0.1.5.dev1/src/emtl/utils.py
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.066150 emtl-0.1.5.dev1/src/emtl.egg-info/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2115 2024-04-24 03:16:20.000000 emtl-0.1.5.dev1/src/emtl.egg-info/PKG-INFO
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1045 2024-04-24 03:16:21.000000 emtl-0.1.5.dev1/src/emtl.egg-info/SOURCES.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        1 2024-04-24 03:16:20.000000 emtl-0.1.5.dev1/src/emtl.egg-info/dependency_links.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       38 2024-04-24 03:16:20.000000 emtl-0.1.5.dev1/src/emtl.egg-info/entry_points.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        1 2024-04-16 09:34:21.000000 emtl-0.1.5.dev1/src/emtl.egg-info/not-zip-safe
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       63 2024-04-24 03:16:20.000000 emtl-0.1.5.dev1/src/emtl.egg-info/requires.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        5 2024-04-24 03:16:20.000000 emtl-0.1.5.dev1/src/emtl.egg-info/top_level.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1593 2024-04-17 08:38:27.000000 emtl-0.1.5.dev1/tox.ini
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.966884 emtl-0.2.1.dev3/
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      761 2024-05-21 10:21:56.000000 emtl-0.2.1.dev3/.bumpversion.cfg
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     1906 2024-05-21 10:21:56.000000 emtl-0.2.1.dev3/.cookiecutterrc
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      149 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/.coveragerc
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      353 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/.editorconfig
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.956884 emtl-0.2.1.dev3/.github/
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.966884 emtl-0.2.1.dev3/.github/workflows/
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      907 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/.github/workflows/document.yml
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     2721 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/.github/workflows/github-actions.yml
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      734 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/.gitignore
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      686 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/.pre-commit-config.yaml
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      285 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/.readthedocs.yml
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       65 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/AUTHORS.rst
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      550 2024-05-21 10:15:07.000000 emtl-0.2.1.dev3/CHANGELOG.rst
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     2274 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/CONTRIBUTING.rst
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     1117 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/LICENSE
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     2530 2024-05-23 01:00:46.966884 emtl-0.2.1.dev3/PKG-INFO
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     2423 2024-05-22 10:56:16.000000 emtl-0.2.1.dev3/README.rst
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.966884 emtl-0.2.1.dev3/ci/
+-rwxr-xr-x   0 riiy      (1000) riiy      (1000)     2867 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/ci/bootstrap.py
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       72 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/ci/requirements.txt
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.956884 emtl-0.2.1.dev3/ci/templates/
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.956884 emtl-0.2.1.dev3/ci/templates/.github/
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.966884 emtl-0.2.1.dev3/ci/templates/.github/workflows/
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     2179 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.966884 emtl-0.2.1.dev3/docs/
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       28 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/docs/authors.rst
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       30 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/docs/changelog.rst
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     1150 2024-05-21 10:21:56.000000 emtl-0.2.1.dev3/docs/conf.py
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       33 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/docs/contributing.rst
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      244 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/docs/index.rst
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       84 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/docs/installation.rst
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       27 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/docs/readme.rst
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.966884 emtl-0.2.1.dev3/docs/reference/
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      146 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/docs/reference/emtl.rst
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       56 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/docs/reference/index.rst
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       14 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/docs/requirements.txt
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      109 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/docs/spelling_wordlist.txt
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      183 2024-05-22 10:57:54.000000 emtl-0.2.1.dev3/docs/usage.rst
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     1381 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/pyproject.toml
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     1303 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/pytest.ini
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       38 2024-05-23 01:00:46.966884 emtl-0.2.1.dev3/setup.cfg
+-rwxr-xr-x   0 riiy      (1000) riiy      (1000)     3055 2024-05-21 10:21:56.000000 emtl-0.2.1.dev3/setup.py
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.956884 emtl-0.2.1.dev3/src/
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.966884 emtl-0.2.1.dev3/src/emtl/
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      547 2024-05-21 10:21:56.000000 emtl-0.2.1.dev3/src/emtl/__init__.py
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      354 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/src/emtl/__main__.py
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      424 2024-05-23 01:00:46.000000 emtl-0.2.1.dev3/src/emtl/_version.py
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      988 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/src/emtl/cli.py
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     1083 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/src/emtl/const.py
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     7105 2024-05-22 02:20:03.000000 emtl-0.2.1.dev3/src/emtl/core.py
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.966884 emtl-0.2.1.dev3/src/emtl/tests/
+-rw-r--r--   0 riiy      (1000) riiy      (1000)        0 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/src/emtl/tests/__init__.py
+-rw-r--r--   0 riiy      (1000) riiy      (1000)      126 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/src/emtl/tests/test_cli.py
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     2215 2024-05-22 02:26:03.000000 emtl-0.2.1.dev3/src/emtl/tests/test_core.py
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     1371 2024-05-20 02:16:50.000000 emtl-0.2.1.dev3/src/emtl/utils.py
+drwxr-xr-x   0 riiy      (1000) riiy      (1000)        0 2024-05-23 01:00:46.966884 emtl-0.2.1.dev3/src/emtl.egg-info/
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     2530 2024-05-23 01:00:46.000000 emtl-0.2.1.dev3/src/emtl.egg-info/PKG-INFO
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     1045 2024-05-23 01:00:46.000000 emtl-0.2.1.dev3/src/emtl.egg-info/SOURCES.txt
+-rw-r--r--   0 riiy      (1000) riiy      (1000)        1 2024-05-23 01:00:46.000000 emtl-0.2.1.dev3/src/emtl.egg-info/dependency_links.txt
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       38 2024-05-23 01:00:46.000000 emtl-0.2.1.dev3/src/emtl.egg-info/entry_points.txt
+-rw-r--r--   0 riiy      (1000) riiy      (1000)        1 2024-05-23 01:00:46.000000 emtl-0.2.1.dev3/src/emtl.egg-info/not-zip-safe
+-rw-r--r--   0 riiy      (1000) riiy      (1000)       63 2024-05-23 01:00:46.000000 emtl-0.2.1.dev3/src/emtl.egg-info/requires.txt
+-rw-r--r--   0 riiy      (1000) riiy      (1000)        5 2024-05-23 01:00:46.000000 emtl-0.2.1.dev3/src/emtl.egg-info/top_level.txt
+-rw-r--r--   0 riiy      (1000) riiy      (1000)     1525 2024-05-20 01:46:20.000000 emtl-0.2.1.dev3/tox.ini
```

### Comparing `emtl-0.1.5.dev1/.bumpversion.cfg` & `emtl-0.2.1.dev3/.bumpversion.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.4
+current_version = 0.2.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = "fallback_version": "{current_version}"
 replace = "fallback_version": "{new_version}"
 
@@ -20,9 +20,9 @@
 replace = version = release = "{new_version}"
 
 [bumpversion:file:src/emtl/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
 [bumpversion:file:.cookiecutterrc]
-search = version: {current_version}
-replace = version: {new_version}
+search = version: "{current_version}"
+replace = version: "{new_version}"
```

### Comparing `emtl-0.1.5.dev1/.cookiecutterrc` & `emtl-0.2.1.dev3/.cookiecutterrc`

 * *Files 1% similar despite different names*

```diff
@@ -50,12 +50,12 @@
     setup_py_uses_setuptools_scm: "yes"
     sphinx_docs: "yes"
     sphinx_docs_hosting: "https://emtl.readthedocs.io/"
     sphinx_doctest: "no"
     sphinx_theme: "alabaster"
     test_matrix_separate_coverage: "yes"
     tests_inside_package: "yes"
-    version: "0.1.3"
+    version: "0.2.0"
     version_manager: "bump2version"
     website: "riiy.gihub.io/emtl"
     year_from: "2024"
     year_to: "2025"
```

### Comparing `emtl-0.1.5.dev1/.github/workflows/document.yml` & `emtl-0.2.1.dev3/.github/workflows/document.yml`

 * *Files identical despite different names*

### Comparing `emtl-0.1.5.dev1/.gitignore` & `emtl-0.2.1.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `emtl-0.1.5.dev1/.pre-commit-config.yaml` & `emtl-0.2.1.dev3/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   pre-commit install --install-hooks
 # To update the versions:
 #   pre-commit autoupdate
 exclude: '^(\.tox|ci/templates|\.bumpversion\.cfg)(/|$)'
 # Note the order is intentional to avoid multiple passes of the hooks
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.7
+    rev: v0.4.1
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix, --show-fixes]
   - repo: https://github.com/psf/black
     rev: 24.4.0
     hooks:
       - id: black
```

### Comparing `emtl-0.1.5.dev1/CONTRIBUTING.rst` & `emtl-0.2.1.dev3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `emtl-0.1.5.dev1/LICENSE` & `emtl-0.2.1.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `emtl-0.1.5.dev1/PKG-INFO` & `emtl-0.2.1.dev3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: emtl
-Version: 0.1.5.dev1
-Summary: 东方财富自动交易系统
+Version: 0.2.1.dev3
+Summary: 东方财富自动交易接口
 Home-page: https://github.com/riiy/emtl
-Author: Eastmoney Trade Library
+Author: Riiy
 Author-email: riiyzhou@gmail.com
 License: MIT
 Project-URL: Documentation, https://emtl.readthedocs.io/
 Project-URL: Changelog, https://emtl.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/riiy/emtl/issues
 Keywords: autotrade,trade,东方财富,股票,交易,交易机器人
 Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -29,15 +29,15 @@
 
 ========
 Overview
 ========
 
 
 
-东方财富自动交易系统
+东方财富自动交易接口
 
 * Free software: MIT license
 
 Installation
 ============
 
 ::
@@ -77,14 +77,21 @@
 
     - - Other
       - ::
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
+Getting help
+============
+
+
+Join `Telegram group <https://t.me/em_trade_lib>`_. Asking a question here is often the quickest way to get a pointer in the right direction.
+
+
 Changelog
 =========
 
 
 0.1.0 (2024-04-14)
 ------------------
 
@@ -101,8 +108,30 @@
 * add login && add asset position
 
 0.1.3 (2024-04-19)
 ------------------
 
 * update docs theme
 
+0.1.5 (2024-04-24)
+------------------
+
+* update login refrence
+
+0.1.7 (2024-04-27)
+------------------
+
+* add insert order api
+
+
+0.1.8 (2024-04-30)
+------------------
+
+* delete macos actions
+
+
+0.2.0 (2024-05-21)
+------------------
+
+* complete all method
+
```

### Comparing `emtl-0.1.5.dev1/README.rst` & `emtl-0.2.1.dev3/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -37,23 +37,23 @@
     :alt: Supported versions
     :target: https://pypi.org/project/emtl
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/emtl.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/emtl
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/riiy/emtl/v0.1.4.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/riiy/emtl/v0.2.0.svg
     :alt: Commits since latest release
-    :target: https://github.com/riiy/emtl/compare/v0.1.4...master
+    :target: https://github.com/riiy/emtl/compare/v0.2.0...master
 
 
 
 .. end-badges
 
-东方财富自动交易系统
+东方财富自动交易接口
 
 * Free software: MIT license
 
 Installation
 ============
 
 ::
@@ -91,7 +91,14 @@
             set PYTEST_ADDOPTS=--cov-append
             tox
 
     - - Other
       - ::
 
             PYTEST_ADDOPTS=--cov-append tox
+
+
+Getting help
+============
+
+
+Join `Telegram group <https://t.me/em_trade_lib>`_. Asking a question here is often the quickest way to get a pointer in the right direction.
```

### Comparing `emtl-0.1.5.dev1/ci/bootstrap.py` & `emtl-0.2.1.dev3/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `emtl-0.1.5.dev1/ci/templates/.github/workflows/github-actions.yml` & `emtl-0.2.1.dev3/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `emtl-0.1.5.dev1/docs/conf.py` & `emtl-0.2.1.dev3/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     from pkg_resources import get_distribution
 
     version = release = get_distribution("emtl").version
 except Exception:
     import traceback
 
     traceback.print_exc()
-    version = release = "0.1.4"
+    version = release = "0.2.0"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/riiy/emtl/issues/%s", "#%s"),
     "pr": ("https://github.com/riiy/emtl/pull/%s", "PR #%s"),
 }
```

### Comparing `emtl-0.1.5.dev1/pyproject.toml` & `emtl-0.2.1.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emtl-0.1.5.dev1/pytest.ini` & `emtl-0.2.1.dev3/pytest.ini`

 * *Files identical despite different names*

### Comparing `emtl-0.1.5.dev1/setup.py` & `emtl-0.2.1.dev3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,33 +12,33 @@
 
 
 setup(
     name="emtl",
     use_scm_version={
         "local_scheme": "dirty-tag",
         "write_to": "src/emtl/_version.py",
-        "fallback_version": "0.1.4",
+        "fallback_version": "0.2.0",
     },
     license="MIT",
-    description="东方财富自动交易系统",
+    description="东方财富自动交易接口",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
-    author="Eastmoney Trade Library",
+    author="Riiy",
     author_email="riiyzhou@gmail.com",
     url="https://github.com/riiy/emtl",
     packages=find_packages("src"),
     package_dir={"": "src"},
     py_modules=[path.stem for path in Path("src").glob("*.py")],
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         # complete classifier list: http://pypi.python.org/pypi?%3Aaction=list_classifiers
-        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: Unix",
         "Operating System :: POSIX",
         # "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

### Comparing `emtl-0.1.5.dev1/src/emtl/const.py` & `emtl-0.2.1.dev3/src/emtl/const.py`

 * *Files identical despite different names*

### Comparing `emtl-0.1.5.dev1/src/emtl/utils.py` & `emtl-0.2.1.dev3/src/emtl/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import base64
 import logging
-from dataclasses import dataclass
-from typing import Any
-from typing import Optional
+import math
 
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import padding
 from cryptography.hazmat.primitives.asymmetric import rsa
 
 rsa_public_key = """
 -----BEGIN PUBLIC KEY-----
@@ -14,38 +12,35 @@
 c0AT4qIJ/xtbBcHkFPK77upnsfDTJiVEuQDH+MiMeb+XhCLNKZGp0yaUU6GlxZdp
 +nLW8b7Kmijr3iepaDhcbVTsYBWchaWUXauj9Lrhz58/6AE/NF0aMolxIGpsi+ST
 2hSHPu3GSXMdhPCkWQIDAQAB
 -----END PUBLIC KEY-----
 """
 
 
-@dataclass
-class Response:
-    message: str
-    status: int
-    error_code: str
-    data: Any
-
-    def is_ok(self) -> bool:
-        return not self.message and self.status == 0
-
-
 def get_logger(name):
     """Logger."""
     formater = "%(asctime)s %(name)-20s %(funcName)s %(lineno)d: %(levelname)-8s: %(message)s"
     logging.basicConfig(format=formater, force=True, level=logging.INFO)
     logger = logging.getLogger(name)
     return logger
 
 
-def response_deserialize(data: dict) -> Optional[Response]:
-    if data is None:
-        return None
-    return Response(
-        data["Message"] if "Message" in data else "", data["Status"], data["Errcode"] if "Errcode" in data else "", data["Data"]
-    )
-
-
 def emt_trade_encrypt(content: str) -> str:
     _pub_key: rsa.RSAPublicKey = serialization.load_pem_public_key(rsa_public_key.encode("utf-8"))  # type:ignore
     encrypt_text = _pub_key.encrypt(content.encode(), padding.PKCS1v15())
     return base64.b64encode(encrypt_text).decode("utf-8")
+
+
+def double_equal(a, b) -> bool:
+    return math.fabs(a - b) < 1e-6
+
+
+def get_float(data: dict, key: str) -> float:
+    if v := data[key].strip():
+        return float(v)
+    return 0.0
+
+
+def get_int(data: dict, key: str) -> int:
+    if v := data[key].strip():
+        return int(v)
+    return 0
```

### Comparing `emtl-0.1.5.dev1/src/emtl.egg-info/PKG-INFO` & `emtl-0.2.1.dev3/src/emtl.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: emtl
-Version: 0.1.5.dev1
-Summary: 东方财富自动交易系统
+Version: 0.2.1.dev3
+Summary: 东方财富自动交易接口
 Home-page: https://github.com/riiy/emtl
-Author: Eastmoney Trade Library
+Author: Riiy
 Author-email: riiyzhou@gmail.com
 License: MIT
 Project-URL: Documentation, https://emtl.readthedocs.io/
 Project-URL: Changelog, https://emtl.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/riiy/emtl/issues
 Keywords: autotrade,trade,东方财富,股票,交易,交易机器人
 Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -29,15 +29,15 @@
 
 ========
 Overview
 ========
 
 
 
-东方财富自动交易系统
+东方财富自动交易接口
 
 * Free software: MIT license
 
 Installation
 ============
 
 ::
@@ -77,14 +77,21 @@
 
     - - Other
       - ::
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
+Getting help
+============
+
+
+Join `Telegram group <https://t.me/em_trade_lib>`_. Asking a question here is often the quickest way to get a pointer in the right direction.
+
+
 Changelog
 =========
 
 
 0.1.0 (2024-04-14)
 ------------------
 
@@ -101,8 +108,30 @@
 * add login && add asset position
 
 0.1.3 (2024-04-19)
 ------------------
 
 * update docs theme
 
+0.1.5 (2024-04-24)
+------------------
+
+* update login refrence
+
+0.1.7 (2024-04-27)
+------------------
+
+* add insert order api
+
+
+0.1.8 (2024-04-30)
+------------------
+
+* delete macos actions
+
+
+0.2.0 (2024-05-21)
+------------------
+
+* complete all method
+
```

### Comparing `emtl-0.1.5.dev1/src/emtl.egg-info/SOURCES.txt` & `emtl-0.2.1.dev3/src/emtl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emtl-0.1.5.dev1/tox.ini` & `emtl-0.2.1.dev3/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ; a generative tox configuration, see: https://tox.wiki/en/latest/user_guide.html#generative-environments
 [tox]
 envlist =
     clean,
     check,
     docs,
-    {py310,py311}-{cover,nocov},
+    {py310,py311}-{cover},
     report
 ignore_basepython_conflict = true
 
 [testenv]
 basepython =
     py310: {env:TOXPYTHON:python3.10}
     py311: {env:TOXPYTHON:python3.11}
@@ -26,20 +26,18 @@
 setenv =
     PYTHONPATH={toxinidir}/tests
     PYTHONUNBUFFERED=yes
 passenv =
     *
 usedevelop =
     cover: true
-    nocov: false
 deps =
     pytest
     cover: pytest-cov
 commands =
-    nocov: {posargs:pytest -vv --ignore=src}
     cover: {posargs:pytest --cov --cov-report=term-missing --cov-report=xml -vv}
 
 [testenv:check]
 deps =
     docutils
     pre-commit
     readme-renderer
```

