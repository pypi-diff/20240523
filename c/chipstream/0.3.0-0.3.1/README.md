# Comparing `tmp/chipstream-0.3.0.tar.gz` & `tmp/chipstream-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chipstream-0.3.0.tar", last modified: Mon May 20 22:33:27 2024, max compression
+gzip compressed data, was "chipstream-0.3.1.tar", last modified: Wed May 22 22:05:52 2024, max compression
```

## Comparing `chipstream-0.3.0.tar` & `chipstream-0.3.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.321227 chipstream-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.313227 chipstream-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.313227 chipstream-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-20 22:33:21.000000 chipstream-0.3.0/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-20 22:33:21.000000 chipstream-0.3.0/.github/workflows/deploy_github.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-20 22:33:21.000000 chipstream-0.3.0/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-20 22:33:21.000000 chipstream-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-20 22:33:21.000000 chipstream-0.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-20 22:33:21.000000 chipstream-0.3.0/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 22:33:21.000000 chipstream-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-20 22:33:27.321227 chipstream-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-20 22:33:21.000000 chipstream-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.317227 chipstream-0.3.0/build-recipes/
--rw-r--r--   0 runner    (1001) docker     (127)    75281 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/ChipStream.icns
--rw-r--r--   0 runner    (1001) docker     (127)   353118 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/ChipStream.ico
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/ChipStreamLauncher.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/ChipStreamLauncherCLI.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/hook-chipstream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/macos_ChipStream.spec
--rwxr-xr-x   0 runner    (1001) docker     (127)     1981 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/macos_build_app.sh
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/macos_build_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/win_ChipStream.spec
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/win_build_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/win_chipstream.iss_dummy
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/win_make_iss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.317227 chipstream-0.3.0/chipstream/
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 22:33:27.000000 chipstream-0.3.0/chipstream/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.317227 chipstream-0.3.0/chipstream/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/cli/cli_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/cli/cli_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/cli/cli_proc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/cli/cli_valid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.321227 chipstream-0.3.0/chipstream/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.321227 chipstream-0.3.0/chipstream/gui/img/
--rw-r--r--   0 runner    (1001) docker     (127)    14396 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/gui/img/chipstream_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    13478 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/gui/main_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/gui/main_window.ui
--rw-r--r--   0 runner    (1001) docker     (127)     9702 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/gui/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/gui/splash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/gui/table_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/path_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.321227 chipstream-0.3.0/chipstream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-20 22:33:27.000000 chipstream-0.3.0/chipstream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-20 22:33:27.000000 chipstream-0.3.0/chipstream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:33:27.000000 chipstream-0.3.0/chipstream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-20 22:33:27.000000 chipstream-0.3.0/chipstream.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-20 22:33:27.000000 chipstream-0.3.0/chipstream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 22:33:27.000000 chipstream-0.3.0/chipstream.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.321227 chipstream-0.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.321227 chipstream-0.3.0/docs/artwork/
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-20 22:33:21.000000 chipstream-0.3.0/docs/artwork/chipstream_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-05-20 22:33:21.000000 chipstream-0.3.0/docs/artwork/chipstream_splash.png
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-20 22:33:21.000000 chipstream-0.3.0/docs/artwork/chipstream_splash.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-20 22:33:21.000000 chipstream-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-20 22:33:21.000000 chipstream-0.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-20 22:33:21.000000 chipstream-0.3.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-20 22:33:21.000000 chipstream-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 22:33:27.321227 chipstream-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.321227 chipstream-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-20 22:33:21.000000 chipstream-0.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.321227 chipstream-0.3.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)   154010 2024-05-20 22:33:21.000000 chipstream-0.3.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-20 22:33:21.000000 chipstream-0.3.0/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 22:33:21.000000 chipstream-0.3.0/tests/requirements-full.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 22:33:21.000000 chipstream-0.3.0/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-20 22:33:21.000000 chipstream-0.3.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-20 22:33:21.000000 chipstream-0.3.0/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-20 22:33:21.000000 chipstream-0.3.0/tests/test_gui_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-20 22:33:21.000000 chipstream-0.3.0/tests/test_path_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.347383 chipstream-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.335383 chipstream-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.335383 chipstream-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-22 22:05:49.000000 chipstream-0.3.1/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-22 22:05:49.000000 chipstream-0.3.1/.github/workflows/deploy_github.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-22 22:05:49.000000 chipstream-0.3.1/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-22 22:05:49.000000 chipstream-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-22 22:05:49.000000 chipstream-0.3.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-22 22:05:49.000000 chipstream-0.3.1/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 22:05:49.000000 chipstream-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-22 22:05:52.347383 chipstream-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-22 22:05:49.000000 chipstream-0.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.339383 chipstream-0.3.1/build-recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)    75281 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/ChipStream.icns
+-rw-r--r--   0 runner    (1001) docker     (127)   353118 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/ChipStream.ico
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/ChipStreamLauncher.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/ChipStreamLauncherCLI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/hook-chipstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/macos_ChipStream.spec
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1981 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/macos_build_app.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/macos_build_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/win_ChipStream.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/win_build_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/win_chipstream.iss_dummy
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/win_make_iss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.339383 chipstream-0.3.1/chipstream/
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 22:05:52.000000 chipstream-0.3.1/chipstream/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.343383 chipstream-0.3.1/chipstream/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/cli/cli_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/cli/cli_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/cli/cli_proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/cli/cli_valid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.343383 chipstream-0.3.1/chipstream/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.343383 chipstream-0.3.1/chipstream/gui/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    14396 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/gui/img/chipstream_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/gui/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15448 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/gui/main_window.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     9702 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/gui/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/gui/splash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/gui/table_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/path_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.347383 chipstream-0.3.1/chipstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-22 22:05:52.000000 chipstream-0.3.1/chipstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-22 22:05:52.000000 chipstream-0.3.1/chipstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:05:52.000000 chipstream-0.3.1/chipstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-22 22:05:52.000000 chipstream-0.3.1/chipstream.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-22 22:05:52.000000 chipstream-0.3.1/chipstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 22:05:52.000000 chipstream-0.3.1/chipstream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.343383 chipstream-0.3.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.343383 chipstream-0.3.1/docs/artwork/
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-22 22:05:49.000000 chipstream-0.3.1/docs/artwork/chipstream_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-05-22 22:05:49.000000 chipstream-0.3.1/docs/artwork/chipstream_splash.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-22 22:05:49.000000 chipstream-0.3.1/docs/artwork/chipstream_splash.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-22 22:05:49.000000 chipstream-0.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-22 22:05:49.000000 chipstream-0.3.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 22:05:49.000000 chipstream-0.3.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-22 22:05:49.000000 chipstream-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 22:05:52.347383 chipstream-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.343383 chipstream-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-22 22:05:49.000000 chipstream-0.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.343383 chipstream-0.3.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   154010 2024-05-22 22:05:49.000000 chipstream-0.3.1/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-22 22:05:49.000000 chipstream-0.3.1/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 22:05:49.000000 chipstream-0.3.1/tests/requirements-full.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 22:05:49.000000 chipstream-0.3.1/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-22 22:05:49.000000 chipstream-0.3.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-22 22:05:49.000000 chipstream-0.3.1/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-22 22:05:49.000000 chipstream-0.3.1/tests/test_gui_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-22 22:05:49.000000 chipstream-0.3.1/tests/test_path_cache.py
```

### Comparing `chipstream-0.3.0/.github/workflows/check.yml` & `chipstream-0.3.1/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/.github/workflows/deploy_github.yml` & `chipstream-0.3.1/.github/workflows/deploy_github.yml`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/.github/workflows/deploy_pypi.yml` & `chipstream-0.3.1/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/.gitignore` & `chipstream-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/CHANGELOG` & `chipstream-0.3.1/CHANGELOG`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+0.3.1
+ - ref: migrate from QTableView to QTableWidget (issues with Windows 11)
 0.3.0
  - BREAKING CHANGE: major changes in dcnum postprocessing
  - feat: allow to select whether volume should be computed
  - feat: allow to select whether flickering correction should be done
  - feat: allow to specify number of events to analyze in CLI
  - enh: expose background computation parameters in CLI
  - ref: move `manager` module to `gui` module
```

### Comparing `chipstream-0.3.0/LICENSE` & `chipstream-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/PKG-INFO` & `chipstream-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chipstream
-Version: 0.3.0
+Version: 0.3.1
 Summary: GUI for DC data postprocessing
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: GPL version 3.0 or later
 Project-URL: source, https://github.com/DC-Analysis/ChipStream
 Project-URL: tracker, https://github.com/DC-Analysis/ChipStream/issues
 Project-URL: documentation, https://chipstream.readthedocs.io/en/stable/
```

### Comparing `chipstream-0.3.0/README.rst` & `chipstream-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/build-recipes/ChipStream.icns` & `chipstream-0.3.1/build-recipes/ChipStream.icns`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/build-recipes/ChipStream.ico` & `chipstream-0.3.1/build-recipes/ChipStream.ico`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/build-recipes/Readme.md` & `chipstream-0.3.1/build-recipes/Readme.md`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/build-recipes/hook-chipstream.py` & `chipstream-0.3.1/build-recipes/hook-chipstream.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/build-recipes/macos_ChipStream.spec` & `chipstream-0.3.1/build-recipes/macos_ChipStream.spec`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/build-recipes/macos_build_app.sh` & `chipstream-0.3.1/build-recipes/macos_build_app.sh`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/build-recipes/win_ChipStream.spec` & `chipstream-0.3.1/build-recipes/win_ChipStream.spec`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/build-recipes/win_chipstream.iss_dummy` & `chipstream-0.3.1/build-recipes/win_chipstream.iss_dummy`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/build-recipes/win_make_iss.py` & `chipstream-0.3.1/build-recipes/win_make_iss.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/chipstream/__init__.py` & `chipstream-0.3.1/chipstream/__init__.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/chipstream/cli/cli_common.py` & `chipstream-0.3.1/chipstream/cli/cli_common.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/chipstream/cli/cli_main.py` & `chipstream-0.3.1/chipstream/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/chipstream/cli/cli_proc.py` & `chipstream-0.3.1/chipstream/cli/cli_proc.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/chipstream/cli/cli_valid.py` & `chipstream-0.3.1/chipstream/cli/cli_valid.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/chipstream/gui/__init__.py` & `chipstream-0.3.1/chipstream/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/chipstream/gui/img/chipstream_icon.png` & `chipstream-0.3.1/chipstream/gui/img/chipstream_icon.png`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/chipstream/gui/main_window.py` & `chipstream-0.3.1/chipstream/gui/main_window.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,34 +12,37 @@
 from dcnum.feat import feat_background
 from PyQt6 import uic, QtCore, QtWidgets
 from PyQt6.QtCore import QStandardPaths
 
 from ..path_cache import PathCache
 from .._version import version
 
+from .manager import ChipStreamJobManager
 from . import splash
 
 
 class ChipStream(QtWidgets.QMainWindow):
     run_completed = QtCore.pyqtSignal()
 
     def __init__(self, *arguments):
         """Initialize ChipStream GUI
 
         If you pass the "--version" command line argument, the
         application will print the version after initialization
         and exit.
         """
+        self.job_manager = ChipStreamJobManager()
         QtWidgets.QMainWindow.__init__(self)
         ref_ui = resources.files("chipstream.gui") / "main_window.ui"
         with resources.as_file(ref_ui) as path_ui:
             uic.loadUi(path_ui, self)
 
+        self.tableWidget_input.set_job_manager(self.job_manager)
+
         self.logger = logging.getLogger(__name__)
-        self.manager = self.tableView_input.model.manager
 
         # Populate segmenter combobox
         self.comboBox_segmenter.blockSignals(True)
         self.comboBox_segmenter.clear()
         self.comboBox_segmenter.addItem("Disabled (from input file)", "copy")
         self.comboBox_segmenter.addItem("Threshold-based", "thresh")
         self.comboBox_segmenter.blockSignals(False)
@@ -88,40 +91,41 @@
         for ii, path in enumerate(self.path_cache):
             self.comboBox_output.addItem(str(path), ii)
         self.comboBox_output.addItem("Select output directory", "new")
         self.comboBox_output.currentIndexChanged.connect(self.on_path_out)
 
         # Signals
         self.run_completed.connect(self.on_run_completed)
-        self.tableView_input.row_selected.connect(self.on_select_job)
+        self.tableWidget_input.row_selected.connect(self.on_select_job)
 
         # if "--version" was specified, print the version and exit
         if "--version" in arguments:
             print(version)
             QtWidgets.QApplication.processEvents(
                 QtCore.QEventLoop.ProcessEventsFlag.AllEvents, 300)
             sys.exit(0)
 
         # Create a timer that continuously updates self.textBrowser
         self.timer = QtCore.QTimer()
-        self.timer.timeout.connect(self.tableView_input.on_selection_changed)
+        self.timer.timeout.connect(self.tableWidget_input.on_selection_changed)
         self.timer.start(1000)
 
         splash.splash_close()
 
         # finalize
         self.show()
         self.activateWindow()
         self.setWindowState(QtCore.Qt.WindowState.WindowActive)
 
     def append_paths(self, path_list):
         """Add input paths to the table"""
-        if not self.manager.is_busy():
+        if not self.job_manager.is_busy():
             for pp in path_list:
-                self.tableView_input.add_input_path(pp)
+                self.job_manager.add_path(pp)
+            self.tableWidget_input.update_from_job_manager()
 
     @QtCore.pyqtSlot(QtCore.QEvent)
     def dragEnterEvent(self, e):
         """Whether files are accepted"""
         if e.mimeData().hasUrls():
             e.accept()
         else:
@@ -183,15 +187,15 @@
         if segmenter == "copy":
             job_kwargs["no_basins_in_output"] = \
                 not self.checkBox_basin_based.isChecked()
 
         return job_kwargs
 
     def is_running(self):
-        return self.manager.is_alive()
+        return self.job_manager.is_busy()
 
     @QtCore.pyqtSlot()
     def on_action_about(self) -> None:
         """Show imprint."""
         gh = "DC-analysis/ChipStream"
         rtd = "chipstream.readthedocs.io"
         about_text = (f"GUI for DC data postprocessing (background "
@@ -216,15 +220,16 @@
         if pathlist:
             # add to list
             self.append_paths(pathlist)
 
     @QtCore.pyqtSlot()
     def on_action_clear(self):
         """Clear the current table view"""
-        self.manager.clear()
+        self.job_manager.clear()
+        self.tableWidget_input.update_from_job_manager()
 
     @QtCore.pyqtSlot()
     def on_action_docs(self):
         webbrowser.open("https://chipstream.readthedocs.io")
 
     @QtCore.pyqtSlot()
     def on_action_software(self) -> None:
@@ -254,15 +259,15 @@
         QtCore.QCoreApplication.quit()
 
     @QtCore.pyqtSlot()
     def on_path_out(self):
         data = self.comboBox_output.currentData()
         if data == "input":
             # Store output data alongside input data
-            self.manager.set_output_path(None)
+            self.job_manager.set_output_path(None)
         elif data == "new":
             # New output path
             default = "." if len(self.path_cache) == 0 else self.path_cache[-1]
             # Open a directory selection dialog
             path = QtWidgets.QFileDialog.getExistingDirectory(
                 self,
                 "Choose data output directory",
@@ -273,47 +278,46 @@
                 self.comboBox_output.insertItem(
                     len(self.path_cache) + 1,  # index in combobox
                     path,
                     len(self.path_cache),  # user data == index in path_cache
                     )
                 self.comboBox_output.setCurrentIndex(len(self.path_cache) + 1)
                 self.path_cache.add_path(pathlib.Path(path))
-                self.manager.set_output_path(path)
+                self.job_manager.set_output_path(path)
             else:
                 # User pressed cancel
                 self.comboBox_output.setCurrentIndex(0)
-                self.manager.set_output_path(None)
+                self.job_manager.set_output_path(None)
             self.comboBox_output.blockSignals(False)
         else:
             # Data is an integer index for `self.path_cache`
-            self.manager.set_output_path(self.path_cache[data])
-        print(self.manager._path_out)
+            self.job_manager.set_output_path(self.path_cache[data])
 
     @QtCore.pyqtSlot()
     def on_run(self):
         """Run the analysis"""
         # When we start running, we disable all the controls until we are
         # finished. The user can still add items to the list but not
         # change the pipeline.
         self.widget_options.setEnabled(False)
-        self.manager.run_all_in_thread(
+        self.job_manager.run_all_in_thread(
             job_kwargs=self.get_job_kwargs(),
             callback_when_done=self.run_completed.emit)
 
     @QtCore.pyqtSlot()
     def on_run_completed(self):
         self.widget_options.setEnabled(True)
 
     @QtCore.pyqtSlot(int)
     def on_select_job(self, row):
         if row < 0:
             info = "No job selected."
         else:
             # Display some information in the lower text box.
-            info = self.manager.get_info(row)
+            info = self.job_manager.get_info(row)
         # Compare the text to the current text.
         old_text = self.textBrowser.toPlainText()
         if info != old_text:
             sb = self.textBrowser.verticalScrollBar()
             is_at_end = sb.maximum() - sb.value() <= 10
             self.textBrowser.setText(info)
             if info.strip().startswith(old_text.strip()) and is_at_end:
```

### Comparing `chipstream-0.3.0/chipstream/gui/main_window.ui` & `chipstream-0.3.1/chipstream/gui/main_window.ui`

 * *Files 4% similar despite different names*

#### Comparing `chipstream-0.3.0/chipstream/gui/main_window.ui` & `chipstream-0.3.1/chipstream/gui/main_window.ui`

```diff
@@ -37,48 +37,75 @@
               </widget>
             </item>
             <item>
               <widget class="QSplitter" name="splitter">
                 <property name="orientation">
                   <enum>Qt::Vertical</enum>
                 </property>
-                <widget class="ProgressTable" name="tableView_input">
+                <widget class="ProgressTable" name="tableWidget_input">
                   <property name="sizePolicy">
                     <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
                       <horstretch>1</horstretch>
                       <verstretch>3</verstretch>
                     </sizepolicy>
                   </property>
+                  <property name="editTriggers">
+                    <set>QAbstractItemView::NoEditTriggers</set>
+                  </property>
                   <property name="dragDropMode">
-                    <enum>QAbstractItemView::InternalMove</enum>
+                    <enum>QAbstractItemView::NoDragDrop</enum>
                   </property>
                   <property name="alternatingRowColors">
                     <bool>true</bool>
                   </property>
                   <property name="selectionMode">
                     <enum>QAbstractItemView::SingleSelection</enum>
                   </property>
                   <property name="selectionBehavior">
                     <enum>QAbstractItemView::SelectRows</enum>
                   </property>
+                  <property name="textElideMode">
+                    <enum>Qt::ElideMiddle</enum>
+                  </property>
+                  <property name="horizontalScrollMode">
+                    <enum>QAbstractItemView::ScrollPerPixel</enum>
+                  </property>
                   <property name="sortingEnabled">
                     <bool>true</bool>
                   </property>
                   <property name="cornerButtonEnabled">
                     <bool>false</bool>
                   </property>
                   <attribute name="horizontalHeaderMinimumSectionSize">
-                    <number>50</number>
+                    <number>100</number>
                   </attribute>
-                  <attribute name="horizontalHeaderStretchLastSection">
-                    <bool>true</bool>
+                  <attribute name="horizontalHeaderDefaultSectionSize">
+                    <number>100</number>
                   </attribute>
-                  <attribute name="verticalHeaderVisible">
+                  <attribute name="horizontalHeaderShowSortIndicator" stdset="0">
                     <bool>false</bool>
                   </attribute>
+                  <attribute name="horizontalHeaderStretchLastSection">
+                    <bool>true</bool>
+                  </attribute>
+                  <column>
+                    <property name="text">
+                      <string>Path</string>
+                    </property>
+                  </column>
+                  <column>
+                    <property name="text">
+                      <string>State</string>
+                    </property>
+                  </column>
+                  <column>
+                    <property name="text">
+                      <string>Progress</string>
+                    </property>
+                  </column>
                 </widget>
                 <widget class="QTextBrowser" name="textBrowser">
                   <property name="sizePolicy">
                     <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
                       <horstretch>1</horstretch>
                       <verstretch>1</verstretch>
                     </sizepolicy>
@@ -424,15 +451,15 @@
         <string>Clear list</string>
       </property>
     </action>
   </widget>
   <customwidgets>
     <customwidget>
       <class>ProgressTable</class>
-      <extends>QTableView</extends>
+      <extends>QTableWidget</extends>
       <header>chipstream.gui.table_progress</header>
     </customwidget>
   </customwidgets>
   <resources/>
   <connections>
     <connection>
       <sender>comboBox_segmenter</sender>
```

### Comparing `chipstream-0.3.0/chipstream/gui/manager.py` & `chipstream-0.3.1/chipstream/gui/manager.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/chipstream/path_cache.py` & `chipstream-0.3.1/chipstream/path_cache.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/chipstream.egg-info/PKG-INFO` & `chipstream-0.3.1/chipstream.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chipstream
-Version: 0.3.0
+Version: 0.3.1
 Summary: GUI for DC data postprocessing
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: GPL version 3.0 or later
 Project-URL: source, https://github.com/DC-Analysis/ChipStream
 Project-URL: tracker, https://github.com/DC-Analysis/ChipStream/issues
 Project-URL: documentation, https://chipstream.readthedocs.io/en/stable/
```

### Comparing `chipstream-0.3.0/chipstream.egg-info/SOURCES.txt` & `chipstream-0.3.1/chipstream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/docs/artwork/chipstream_icon.svg` & `chipstream-0.3.1/docs/artwork/chipstream_icon.svg`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/docs/artwork/chipstream_splash.png` & `chipstream-0.3.1/docs/artwork/chipstream_splash.png`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/docs/artwork/chipstream_splash.svg` & `chipstream-0.3.1/docs/artwork/chipstream_splash.svg`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/docs/conf.py` & `chipstream-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/pyproject.toml` & `chipstream-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/tests/conftest.py` & `chipstream-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip` & `chipstream-0.3.1/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/tests/helper_methods.py` & `chipstream-0.3.1/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/tests/test_cli.py` & `chipstream-0.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/tests/test_gui.py` & `chipstream-0.3.1/tests/test_gui.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,27 +33,27 @@
         QtCore.QEventLoop.ProcessEventsFlag.AllEvents, 300)
 
 
 def test_gui_basic(mw):
     # Just check some known properties in the UI.
     assert mw.spinBox_thresh.value() == -6
     assert mw.checkBox_feat_bright.isChecked()
-    assert len(mw.manager) == 0
+    assert len(mw.job_manager) == 0
 
 
 @pytest.mark.parametrize("correct_offset", [True, False])
 def test_gui_correct_offset(mw, correct_offset):
     path = retrieve_data(
         "fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip")
     mw.append_paths([path])
     mw.checkBox_pixel_size.setChecked(True)
     mw.checkBox_bg_flickering.setChecked(correct_offset)
     mw.doubleSpinBox_pixel_size.setValue(0.666)
     mw.on_run()
-    while mw.manager.is_busy():
+    while mw.job_manager.is_busy():
         time.sleep(.1)
     out_path = path.with_name(path.stem + "_dcn.rtdc")
     assert out_path.exists()
 
     with h5py.File(out_path) as h5:
         assert np.allclose(h5.attrs["imaging:pixel size"],
                            0.666,
@@ -64,15 +64,15 @@
 def test_gui_set_pixel_size(mw):
     path = retrieve_data(
         "fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip")
     mw.append_paths([path])
     mw.checkBox_pixel_size.setChecked(True)
     mw.doubleSpinBox_pixel_size.setValue(0.666)
     mw.on_run()
-    while mw.manager.is_busy():
+    while mw.job_manager.is_busy():
         time.sleep(.1)
     out_path = path.with_name(path.stem + "_dcn.rtdc")
     assert out_path.exists()
 
     with h5py.File(out_path) as h5:
         assert np.allclose(h5.attrs["imaging:pixel size"],
                            0.666,
@@ -84,15 +84,15 @@
     path = retrieve_data(
         "fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip")
     mw.append_paths([path])
     mw.checkBox_pixel_size.setChecked(True)
     mw.checkBox_feat_volume.setChecked(use_volume)
     mw.doubleSpinBox_pixel_size.setValue(0.666)
     mw.on_run()
-    while mw.manager.is_busy():
+    while mw.job_manager.is_busy():
         time.sleep(.1)
     out_path = path.with_name(path.stem + "_dcn.rtdc")
     assert out_path.exists()
 
     with h5py.File(out_path) as h5:
         assert np.allclose(h5.attrs["imaging:pixel size"],
                            0.666,
```

### Comparing `chipstream-0.3.0/tests/test_gui_manager.py` & `chipstream-0.3.1/tests/test_gui_manager.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.0/tests/test_path_cache.py` & `chipstream-0.3.1/tests/test_path_cache.py`

 * *Files identical despite different names*

