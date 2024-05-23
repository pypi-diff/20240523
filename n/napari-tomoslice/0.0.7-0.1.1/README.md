# Comparing `tmp/napari-tomoslice-0.0.7.tar.gz` & `tmp/napari_tomoslice-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-tomoslice-0.0.7.tar", last modified: Tue Feb  1 22:21:40 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `napari-tomoslice-0.0.7.tar` & `napari_tomoslice-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 22:21:40.490012 napari-tomoslice-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 22:21:40.486012 napari-tomoslice-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 22:21:40.486012 napari-tomoslice-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1870 2022-02-01 22:21:28.000000 napari-tomoslice-0.0.7/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)      947 2022-02-01 22:21:28.000000 napari-tomoslice-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-02-01 22:21:28.000000 napari-tomoslice-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-02-01 22:21:28.000000 napari-tomoslice-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4097 2022-02-01 22:21:40.490012 napari-tomoslice-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2885 2022-02-01 22:21:28.000000 napari-tomoslice-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 22:21:40.486012 napari-tomoslice-0.0.7/napari_tomoslice/
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-02-01 22:21:28.000000 napari-tomoslice-0.0.7/napari_tomoslice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 22:21:40.490012 napari-tomoslice-0.0.7/napari_tomoslice/_qt/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 22:21:28.000000 napari-tomoslice-0.0.7/napari_tomoslice/_qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-02-01 22:21:28.000000 napari-tomoslice-0.0.7/napari_tomoslice/_qt/named_labeled_slider.py
--rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-02-01 22:21:28.000000 napari-tomoslice-0.0.7/napari_tomoslice/_qt/open_close_buttons.py
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-02-01 22:21:28.000000 napari-tomoslice-0.0.7/napari_tomoslice/_qt/selectable_button_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     3884 2022-02-01 22:21:28.000000 napari-tomoslice-0.0.7/napari_tomoslice/_qt/tomoslice.py
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-02-01 22:21:28.000000 napari-tomoslice-0.0.7/napari_tomoslice/_qt/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-02-01 22:21:28.000000 napari-tomoslice-0.0.7/napari_tomoslice/_qt/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-02-01 22:21:40.000000 napari-tomoslice-0.0.7/napari_tomoslice/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-02-01 22:21:28.000000 napari-tomoslice-0.0.7/napari_tomoslice/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2830 2022-02-01 22:21:28.000000 napari-tomoslice-0.0.7/napari_tomoslice/interactivity_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3954 2022-02-01 22:21:28.000000 napari-tomoslice-0.0.7/napari_tomoslice/plane_controls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-02-01 22:21:28.000000 napari-tomoslice-0.0.7/napari_tomoslice/points_controls.py
--rw-r--r--   0 runner    (1001) docker     (121)     9387 2022-02-01 22:21:28.000000 napari-tomoslice-0.0.7/napari_tomoslice/tomoslice.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 22:21:40.490012 napari-tomoslice-0.0.7/napari_tomoslice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4097 2022-02-01 22:21:40.000000 napari-tomoslice-0.0.7/napari_tomoslice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      850 2022-02-01 22:21:40.000000 napari-tomoslice-0.0.7/napari_tomoslice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-01 22:21:40.000000 napari-tomoslice-0.0.7/napari_tomoslice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-02-01 22:21:40.000000 napari-tomoslice-0.0.7/napari_tomoslice.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-02-01 22:21:40.000000 napari-tomoslice-0.0.7/napari_tomoslice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-02-01 22:21:40.000000 napari-tomoslice-0.0.7/napari_tomoslice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-02-01 22:21:28.000000 napari-tomoslice-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1384 2022-02-01 22:21:40.490012 napari-tomoslice-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-02-01 22:21:28.000000 napari-tomoslice-0.0.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-02-01 22:21:28.000000 napari-tomoslice-0.0.7/tox.ini
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/.cruft.json
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/.github_changelog_generator
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/requirements.txt
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0  1765500 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/assets/spheres.gif
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/src/napari_tomoslice/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/src/napari_tomoslice/_constants.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/src/napari_tomoslice/console.py
+-rw-r--r--   0        0        0     8965 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/src/napari_tomoslice/tomoslice_app.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/src/napari_tomoslice/tomoslice_cli.py
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/src/napari_tomoslice/utils.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/src/napari_tomoslice/io/__init__.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/src/napari_tomoslice/io/paths.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/src/napari_tomoslice/io/points.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/src/napari_tomoslice/io/spheres.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/src/napari_tomoslice/io/volume.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/src/napari_tomoslice/widgets/__init__.py
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/src/napari_tomoslice/widgets/tomoslice_widget.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/tests/test_io.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/README.md
+-rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 napari_tomoslice-0.1.1/PKG-INFO
```

### Comparing `napari-tomoslice-0.0.7/.gitignore` & `napari_tomoslice-0.1.1/.gitignore`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
 var/
+wheels/
 *.egg-info/
 .installed.cfg
 *.egg
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
@@ -38,42 +39,67 @@
 htmlcov/
 .tox/
 .coverage
 .coverage.*
 .cache
 nosetests.xml
 coverage.xml
-*,cover
+*.cover
 .hypothesis/
-.napari_cache
+.pytest_cache/
 
 # Translations
 *.mo
 *.pot
 
 # Django stuff:
 *.log
 local_settings.py
 
-# Flask instance folder
+# Flask stuff:
 instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
 
 # Sphinx documentation
 docs/_build/
 
-# MkDocs documentation
-/site/
-
 # PyBuilder
 target/
 
-# IPython Notebook
+# Jupyter Notebook
 .ipynb_checkpoints
 
 # pyenv
 .python-version
 
-# OS
-.DS_Store
+# celery beat schedule file
+celerybeat-schedule
+
+# SageMath parsed files
+*.sage.py
+
+# dotenv
+.env
+
+# virtualenv
+.venv
+venv/
+ENV/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
 
-# written by setuptools_scm
-*/_version.py
+# IDE settings
+.vscode/
```

### Comparing `napari-tomoslice-0.0.7/LICENSE` & `napari_tomoslice-0.1.1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-
-Copyright (c) 2021, Alister Burt
-All rights reserved.
+Copyright (c) 2023, Alister Burt
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
 
-* Neither the name of napari-tomoslice nor the names of its
-  contributors may be used to endorse or promote products derived from
-  this software without specific prior written permission.
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
 AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
 IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
```

