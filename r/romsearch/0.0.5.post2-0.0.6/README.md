# Comparing `tmp/romsearch-0.0.5.post2.tar.gz` & `tmp/romsearch-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "romsearch-0.0.5.post2.tar", last modified: Fri May 17 23:08:08 2024, max compression
+gzip compressed data, was "romsearch-0.0.6.tar", last modified: Thu May 23 11:49:58 2024, max compression
```

## Comparing `romsearch-0.0.5.post2.tar` & `romsearch-0.0.6.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:08:08.583141 romsearch-0.0.5.post2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:08:08.567141 romsearch-0.0.5.post2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:08:08.567141 romsearch-0.0.5.post2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/.github/ISSUE_TEMPLATE/console_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/.github/ISSUE_TEMPLATE/feature_request.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:08:08.571141 romsearch-0.0.5.post2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    43912 2024-05-17 23:08:08.583141 romsearch-0.0.5.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:08:08.571141 romsearch-0.0.5.post2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/1g1r.rst
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:08:08.571141 romsearch-0.0.5.post2/docs/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/configs/clonelists.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/configs/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/configs/dats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/configs/defaults.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/configs/platforms.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/configs/regex.rst
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/configs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/configuration.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:08:08.571141 romsearch-0.0.5.post2/docs/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/gui/config_includes_excludes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/gui/config_main.rst
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/gui/config_modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/gui/config_platforms.rst
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/gui/config_regions_languages.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/gui/intro.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:08:08.575142 romsearch-0.0.5.post2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    24254 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/images/config_includes_excludes.png
--rw-r--r--   0 runner    (1001) docker     (127)    71922 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/images/config_main.png
--rw-r--r--   0 runner    (1001) docker     (127)    24790 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/images/config_modules.png
--rw-r--r--   0 runner    (1001) docker     (127)    39895 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/images/config_platforms.png
--rw-r--r--   0 runner    (1001) docker     (127)    73902 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/images/config_regions_languages.png
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/known_issues.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:08:08.575142 romsearch-0.0.5.post2/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/modules/datparser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/modules/dupeparser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/modules/gamefinder.rst
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/modules/romchooser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/modules/romdownloader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/modules/rommover.rst
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/modules/romparser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/modules/romsearch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/reference_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:08:08.575142 romsearch-0.0.5.post2/romsearch/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:08:08.575142 romsearch-0.0.5.post2/romsearch/configs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:08:08.575142 romsearch-0.0.5.post2/romsearch/configs/clonelists/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/configs/clonelists/retool.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:08:08.575142 romsearch-0.0.5.post2/romsearch/configs/dats/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/configs/dats/no-intro.yml
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/configs/dats/redump.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/configs/defaults.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:08:08.579141 romsearch-0.0.5.post2/romsearch/configs/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/configs/platforms/Nintendo - GameCube.yml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/configs/platforms/Nintendo - Nintendo Entertainment System.yml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/configs/platforms/Nintendo - Super Nintendo Entertainment System.yml
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/configs/platforms/Sony - PlayStation 2.yml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/configs/platforms/Sony - PlayStation Portable.yml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/configs/platforms/Sony - PlayStation.yml
--rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/configs/regex.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/configs/sample_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:08:08.579141 romsearch-0.0.5.post2/romsearch/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/dev/parsing_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:08:08.579141 romsearch-0.0.5.post2/romsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/gui/gui_about.py
--rw-r--r--   0 runner    (1001) docker     (127)    27172 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/gui/gui_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/gui/gui_romsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/gui/gui_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/gui/layout_about.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/gui/layout_about.ui
--rw-r--r--   0 runner    (1001) docker     (127)    96327 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/gui/layout_romsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)    89017 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/gui/layout_romsearch.ui
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:08:08.583141 romsearch-0.0.5.post2/romsearch/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/modules/datparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/modules/dupeparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/modules/gamefinder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16739 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/modules/romchooser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11552 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/modules/romdownloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/modules/rommover.py
--rw-r--r--   0 runner    (1001) docker     (127)    13987 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/modules/romparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    14022 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/modules/romsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:08:08.583141 romsearch-0.0.5.post2/romsearch/util/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/util/discord.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/util/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/util/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch/util/regex_matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:08:08.583141 romsearch-0.0.5.post2/romsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43912 2024-05-17 23:08:08.000000 romsearch-0.0.5.post2/romsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-17 23:08:08.000000 romsearch-0.0.5.post2/romsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 23:08:08.000000 romsearch-0.0.5.post2/romsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-17 23:08:08.000000 romsearch-0.0.5.post2/romsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 23:08:08.000000 romsearch-0.0.5.post2/romsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-17 23:07:59.000000 romsearch-0.0.5.post2/romsearch_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 23:08:08.583141 romsearch-0.0.5.post2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:58.156292 romsearch-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:58.136292 romsearch-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:58.140292 romsearch-0.0.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-23 11:49:54.000000 romsearch-0.0.6/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-23 11:49:54.000000 romsearch-0.0.6/.github/ISSUE_TEMPLATE/console_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-23 11:49:54.000000 romsearch-0.0.6/.github/ISSUE_TEMPLATE/feature_request.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:58.144292 romsearch-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-23 11:49:54.000000 romsearch-0.0.6/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-23 11:49:54.000000 romsearch-0.0.6/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-23 11:49:54.000000 romsearch-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-23 11:49:54.000000 romsearch-0.0.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-23 11:49:54.000000 romsearch-0.0.6/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 11:49:54.000000 romsearch-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-23 11:49:54.000000 romsearch-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    43906 2024-05-23 11:49:58.156292 romsearch-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-23 11:49:54.000000 romsearch-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:58.144292 romsearch-0.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/1g1r.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:58.144292 romsearch-0.0.6/docs/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/configs/clonelists.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/configs/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/configs/dats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/configs/defaults.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/configs/platforms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/configs/regex.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/configs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/configuration.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:58.148292 romsearch-0.0.6/docs/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/gui/config_includes_excludes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/gui/config_main.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/gui/config_modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/gui/config_platforms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/gui/config_regions_languages.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/gui/intro.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:58.148292 romsearch-0.0.6/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    24254 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/images/config_includes_excludes.png
+-rw-r--r--   0 runner    (1001) docker     (127)    71922 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/images/config_main.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27569 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/images/config_modules.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39895 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/images/config_platforms.png
+-rw-r--r--   0 runner    (1001) docker     (127)    73902 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/images/config_regions_languages.png
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/known_issues.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:58.148292 romsearch-0.0.6/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/modules/datparser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/modules/dupeparser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/modules/gamefinder.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/modules/romchooser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/modules/romdownloader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/modules/rommover.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/modules/romparser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/modules/romsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/reference_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-23 11:49:54.000000 romsearch-0.0.6/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-23 11:49:54.000000 romsearch-0.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:58.148292 romsearch-0.0.6/romsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:58.148292 romsearch-0.0.6/romsearch/configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:58.148292 romsearch-0.0.6/romsearch/configs/clonelists/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/configs/clonelists/retool.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:58.152292 romsearch-0.0.6/romsearch/configs/dats/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/configs/dats/no-intro.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/configs/dats/redump.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/configs/defaults.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:58.152292 romsearch-0.0.6/romsearch/configs/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/configs/platforms/Nintendo - GameCube.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/configs/platforms/Nintendo - Nintendo Entertainment System.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/configs/platforms/Nintendo - Super Nintendo Entertainment System.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/configs/platforms/Sony - PlayStation 2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/configs/platforms/Sony - PlayStation Portable.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/configs/platforms/Sony - PlayStation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/configs/regex.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/configs/sample_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:58.152292 romsearch-0.0.6/romsearch/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/dev/parsing_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:58.152292 romsearch-0.0.6/romsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/gui/gui_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27314 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/gui/gui_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/gui/gui_romsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/gui/gui_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/gui/layout_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/gui/layout_about.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    97636 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/gui/layout_romsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90059 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/gui/layout_romsearch.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:58.156292 romsearch-0.0.6/romsearch/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/modules/datparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/modules/dupeparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/modules/gamefinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/modules/romchooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17822 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/modules/romdownloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/modules/rommover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/modules/romparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13835 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/modules/romsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:58.156292 romsearch-0.0.6/romsearch/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/util/discord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/util/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/util/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch/util/regex_matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:58.156292 romsearch-0.0.6/romsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43906 2024-05-23 11:49:58.000000 romsearch-0.0.6/romsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-23 11:49:58.000000 romsearch-0.0.6/romsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:49:58.000000 romsearch-0.0.6/romsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-23 11:49:58.000000 romsearch-0.0.6/romsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 11:49:58.000000 romsearch-0.0.6/romsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-23 11:49:54.000000 romsearch-0.0.6/romsearch_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 11:49:58.156292 romsearch-0.0.6/setup.cfg
```

### Comparing `romsearch-0.0.5.post2/.github/ISSUE_TEMPLATE/bug_report.yml` & `romsearch-0.0.6/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/.github/ISSUE_TEMPLATE/feature_request.yml` & `romsearch-0.0.6/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/.github/workflows/build.yaml` & `romsearch-0.0.6/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/.github/workflows/publish.yaml` & `romsearch-0.0.6/.github/workflows/publish.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Build and upload
+name: Publish
 
 on: [push, pull_request]
 
 jobs:
   build_sdist_and_wheel:
     name: Build source distribution
     runs-on: ubuntu-latest
```

### Comparing `romsearch-0.0.5.post2/.gitignore` & `romsearch-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/.readthedocs.yaml` & `romsearch-0.0.6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/CHANGES.rst` & `romsearch-0.0.6/CHANGES.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,42 @@
+0.0.6 (2024-05-23)
+==================
+
+Fixes
+-----
+
+ROMChooser
+~~~~~~~~~~
+
+- Language priorities are now baked into the ROM selection. ROMs with more (and higher priority) languages
+  will now be preferred
+
+ROMDownloader
+~~~~~~~~~~~~~
+
+- Added a ``use_absolute_url`` option, which if False will strip the leading slash from the directories. This is
+  potentially useful if using an HTTP remote
+- rclone can now either sync or copy. It'll use sync if completionist mode is on, else it'll use copy which is
+  a little cleaner
+- If there are errors in the rclone command, ROMDownloader will now retry a few times
+- Improved how rclone runs, to be less verbose and hopefully more reliable
+
+ROMParser
+~~~~~~~~~
+
+- If no language is given in the ROM data, will attempt to pull this out from the region
+
+General
+~~~~~~~
+
+- Updated dev tools for the new config directory structure
+- Renamed `ftp_dir` to `dir` ion platform config files for clarity
+- Fixed error message in GUI in includes/excludes existed for an unchecked platform
+
+
 0.0.5 (2024-05-17)
 ==================
 
 Features
 --------
 
 - ROMSearch now has a GUI! This currently is just used for a more friendly way to set the config file, but will
```

### Comparing `romsearch-0.0.5.post2/LICENSE` & `romsearch-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/PKG-INFO` & `romsearch-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romsearch
-Version: 0.0.5.post2
+Version: 0.0.6
 Summary: One Stop ROM Shop
 Author: bbtufty
 Maintainer: bbtufty
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `romsearch-0.0.5.post2/README.md` & `romsearch-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/docs/1g1r.rst` & `romsearch-0.0.6/docs/1g1r.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/docs/Makefile` & `romsearch-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/docs/conf.py` & `romsearch-0.0.6/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'romsearch'
 copyright = '2024, bbtufty'
 author = 'bbtufty'
-release = '0.0.5.post2'
+release = '0.0.6'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc',
               'sphinx.ext.coverage',
               'sphinx.ext.napoleon',
```

### Comparing `romsearch-0.0.5.post2/docs/configs/config.rst` & `romsearch-0.0.6/docs/configs/config.rst`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,16 @@
       run_romchooser: true              # OPTIONAL. Whether to run ROMChooser. Defaults to true
       run_rommover: true                # OPTIONAL. Whether to run ROMMover. Defaults to true
       dry_run: false                    # OPTIONAL. Set to true to not make any changes to filesystem. Defaults to false
 
     romdownloader:                      # ROMDownloader specific options
       dry_run: false                    # OPTIONAL. Set to true to not make any changes to filesystem. Defaults to false
       remote_name: 'rclone_remote'      # Rclone remote name
+      use_absolute_url: false           # OPTIONAL. If true, will assume the path is an absolute URL for the rclone
+                                        #           remote. Set to false if using an HTTP remote!
       sync_all: false                   # OPTIONAL. If true, will download everything that rclone finds. Set to false to
                                         #           use the include_games above
 
     dupeparser:                         # DupeParser specific options
       use_dat: true                     # OPTIONAL. Whether to use .dat files or not. Defaults to true
       use_retool: true                  # OPTIONAL. Whether to use retool clonelists or not. Defaults to true
```

### Comparing `romsearch-0.0.5.post2/docs/configs/dats.rst` & `romsearch-0.0.6/docs/configs/dats.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/docs/configs/regex.rst` & `romsearch-0.0.6/docs/configs/regex.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/docs/configuration.rst` & `romsearch-0.0.6/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/docs/gui/intro.rst` & `romsearch-0.0.6/docs/gui/intro.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/docs/images/config_includes_excludes.png` & `romsearch-0.0.6/docs/images/config_includes_excludes.png`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/docs/images/config_main.png` & `romsearch-0.0.6/docs/images/config_main.png`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/docs/images/config_platforms.png` & `romsearch-0.0.6/docs/images/config_platforms.png`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/docs/images/config_regions_languages.png` & `romsearch-0.0.6/docs/images/config_regions_languages.png`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/docs/index.rst` & `romsearch-0.0.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/docs/intro.rst` & `romsearch-0.0.6/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/docs/known_issues.rst` & `romsearch-0.0.6/docs/known_issues.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/docs/make.bat` & `romsearch-0.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/docs/modules/datparser.rst` & `romsearch-0.0.6/docs/modules/datparser.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/docs/modules/dupeparser.rst` & `romsearch-0.0.6/docs/modules/dupeparser.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/docs/modules/romsearch.rst` & `romsearch-0.0.6/docs/modules/romsearch.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/pyproject.toml` & `romsearch-0.0.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "romsearch"
-version = "0.0.5.post2"
+version = "0.0.6"
 description = "One Stop ROM Shop"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 
 authors = [
     {name = "bbtufty"},
```

### Comparing `romsearch-0.0.5.post2/romsearch/__init__.py` & `romsearch-0.0.6/romsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/romsearch/configs/clonelists/retool.yml` & `romsearch-0.0.6/romsearch/configs/clonelists/retool.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/romsearch/configs/defaults.yml` & `romsearch-0.0.6/romsearch/configs/defaults.yml`

 * *Files 23% similar despite different names*

```diff
@@ -127,14 +127,69 @@
   Spanish (Mexican): "Es-MX"
   Swedish: "Sv"
   Tamil: "Ta"
   Thai: "Th"
   Turkish: "Tr"
   Ukranian: "Uk"
 
+implied_languages:
+  USA: "English"
+  World: "English"
+  Canada: "English"
+  Europe: "English"
+  UK: "English"
+  Australia: "English"
+  New Zealand: "English"
+  Singapore: "English"
+  Ireland: "English"
+  Japan: "Japanese"
+  Spain: "Spanish"
+  Mexico: "Spanish (Mexican)"
+  Argentina: "Spanish"
+  Latin America: "Spanish (Latin American)"
+  Brazil: "Portuguese (Brazilian)"
+  Portugal: "Portuguese"
+  France: "French"
+  Belgium: "French"
+  Netherlands: "Dutch"
+  Germany: "German"
+  Austria: "German"
+  Italy: "Italian"
+  Hong Kong: "Chinese (Traditional)"
+  China: "Chinese (Simplified)"
+  Taiwan: "Chinese (Traditional)"
+  Korea: "Korean"
+  Russia: "Russian"
+  Estonia: "Estonian"
+  Poland: "Polish"
+  Latvia: "Latvian"
+  Lithuania: "Lithuanian"
+  Denmark: "Danish"
+  Norway: "Norwegian"
+  Sweden: "Swedish"
+  Finland: "Finnish"
+  Iceland: "Icelandic"
+  Hungary: "Hungarian"
+  Czech: "Czech"
+  Greece: "Greek"
+  Macedonia: "Macedonian"
+  India: "English"
+  Israel: "Hebrew"
+  Slovakia: "Slovakian"
+  Turkey: "Turkish"
+  Croatia: "Croatian"
+  Slovenia: "Slovenian"
+  United Arab Emirates: "Arabic"
+  Bulgaria: "Bulgarian"
+  Romania: "Romanian"
+  Albania: "Albanian"
+  Serbia: "Serbian"
+  Indonesia: "Indonesian"
+  Unknown: "English"
+
 dat_categories:
   - "Add-Ons"
   - "Applications"
   - "Audio"
   - "Console"
   - "Bonus Discs"
   - "Coverdiscs"
```

### Comparing `romsearch-0.0.5.post2/romsearch/configs/regex.yml` & `romsearch-0.0.6/romsearch/configs/regex.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/romsearch/configs/sample_config.yml` & `romsearch-0.0.6/romsearch/configs/sample_config.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/romsearch/dev/parsing_tools.py` & `romsearch-0.0.6/romsearch/dev/parsing_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,18 +51,24 @@
     """Using a config file and platform, parse all the games from a dat
 
     This will include the dupe parsing and everything if specified in the config
     """
 
     config = load_yml(config_file)
 
-    parsed_dat_dir = config.get("parsed_dat_dir", None)
+    parsed_dat_dir = config.get("dirs", {}).get("parsed_dat_dir", None)
+
+    if parsed_dat_dir is None:
+        raise ValueError("No parsed_dat_dir found in config file")
 
     dat_filename = os.path.join(parsed_dat_dir, f"{platform} (dat parsed).json")
 
+    if not os.path.exists(dat_filename):
+        raise ValueError("No parsed dat file found")
+
     all_file_dict = check_regex_parsing(dat_filename)
 
     finder = GameFinder(config_file=config_file,
                         platform=platform,
                         )
     finder.logger.setLevel(logging.WARNING)
```

### Comparing `romsearch-0.0.5.post2/romsearch/gui/gui_config.py` & `romsearch-0.0.6/romsearch/gui/gui_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,14 +169,15 @@
             "run_romchooser": self.ui.checkBoxConfigRunRomChooser,
             "run_rommover": self.ui.checkBoxConfigRunRomMover,
             "dry_run": self.ui.checkBoxConfigDryRun,
         }
 
         self.all_romdownloader_options = {
             "sync_all": self.ui.checkBoxConfigRomDownloaderSyncAll,
+            "use_absolute_url": self.ui.checkBoxConfigRomDownloaderUseAbsoluteUrl,
             "dry_run": self.ui.checkBoxConfigRomDownloaderDryRun,
         }
 
         self.all_dupeparser_options = {
             "use_dat": self.ui.checkBoxConfigDupeParserUseDat,
             "use_retool": self.ui.checkBoxConfigDupeParserUseRetool,
         }
@@ -534,15 +535,16 @@
         for m in mappings:
             if m in self.config:
 
                 platforms = self.config[m]
                 for p in platforms:
                     includes = "\n".join(self.config[m][p])
 
-                    self.include_exclude_dict[p][mappings[m]].setPlainText(includes)
+                    if p in self.include_exclude_dict:
+                        self.include_exclude_dict[p][mappings[m]].setPlainText(includes)
 
         return True
 
     def create_file(self):
         """Get filename to save config file to"""
 
         filename, _ = QFileDialog.getSaveFileName(self,
```

### Comparing `romsearch-0.0.5.post2/romsearch/gui/gui_romsearch.py` & `romsearch-0.0.6/romsearch/gui/gui_romsearch.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/romsearch/gui/gui_utils.py` & `romsearch-0.0.6/romsearch/gui/gui_utils.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/romsearch/gui/layout_about.py` & `romsearch-0.0.6/romsearch/gui/layout_about.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/romsearch/gui/layout_about.ui` & `romsearch-0.0.6/romsearch/gui/layout_about.ui`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/romsearch/gui/layout_romsearch.py` & `romsearch-0.0.6/romsearch/gui/layout_romsearch.py`

 * *Files 1% similar despite different names*

```diff
@@ -639,14 +639,27 @@
 
         self.checkBoxConfigRomDownloaderSyncAll = QCheckBox(self.tabConfigRomDownloader)
         self.checkBoxConfigRomDownloaderSyncAll.setObjectName(u"checkBoxConfigRomDownloaderSyncAll")
         self.checkBoxConfigRomDownloaderSyncAll.setChecked(True)
 
         self.verticalLayoutConfigRomDownloaderMiddle.addWidget(self.checkBoxConfigRomDownloaderSyncAll)
 
+        self.lineConfigRomDownloaderSyncAllDividerBottom = QFrame(self.tabConfigRomDownloader)
+        self.lineConfigRomDownloaderSyncAllDividerBottom.setObjectName(u"lineConfigRomDownloaderSyncAllDividerBottom")
+        self.lineConfigRomDownloaderSyncAllDividerBottom.setFrameShadow(QFrame.Shadow.Plain)
+        self.lineConfigRomDownloaderSyncAllDividerBottom.setFrameShape(QFrame.Shape.HLine)
+
+        self.verticalLayoutConfigRomDownloaderMiddle.addWidget(self.lineConfigRomDownloaderSyncAllDividerBottom)
+
+        self.checkBoxConfigRomDownloaderUseAbsoluteUrl = QCheckBox(self.tabConfigRomDownloader)
+        self.checkBoxConfigRomDownloaderUseAbsoluteUrl.setObjectName(u"checkBoxConfigRomDownloaderUseAbsoluteUrl")
+        self.checkBoxConfigRomDownloaderUseAbsoluteUrl.setChecked(True)
+
+        self.verticalLayoutConfigRomDownloaderMiddle.addWidget(self.checkBoxConfigRomDownloaderUseAbsoluteUrl)
+
         self.lineConfigRomDownloaderDryRunTop = QFrame(self.tabConfigRomDownloader)
         self.lineConfigRomDownloaderDryRunTop.setObjectName(u"lineConfigRomDownloaderDryRunTop")
         self.lineConfigRomDownloaderDryRunTop.setFrameShadow(QFrame.Shadow.Plain)
         self.lineConfigRomDownloaderDryRunTop.setFrameShape(QFrame.Shape.HLine)
 
         self.verticalLayoutConfigRomDownloaderMiddle.addWidget(self.lineConfigRomDownloaderDryRunTop)
 
@@ -1408,14 +1421,18 @@
         self.lineEditConfigRomDownloaderRemoteName.setText("")
         self.lineEditConfigRomDownloaderRemoteName.setPlaceholderText(QCoreApplication.translate("RomSearch", u"remote", None))
 #if QT_CONFIG(statustip)
         self.checkBoxConfigRomDownloaderSyncAll.setStatusTip(QCoreApplication.translate("RomSearch", u"Whether to sync everything when running ROMDownloader or whether to filter files based on includes/excludes. Default checked", None))
 #endif // QT_CONFIG(statustip)
         self.checkBoxConfigRomDownloaderSyncAll.setText(QCoreApplication.translate("RomSearch", u"Sync All", None))
 #if QT_CONFIG(statustip)
+        self.checkBoxConfigRomDownloaderUseAbsoluteUrl.setStatusTip(QCoreApplication.translate("RomSearch", u"Whether to treat the remote URL as absolute or relative. Should be unchecked for HTTP remotes", None))
+#endif // QT_CONFIG(statustip)
+        self.checkBoxConfigRomDownloaderUseAbsoluteUrl.setText(QCoreApplication.translate("RomSearch", u"Use absolute URL", None))
+#if QT_CONFIG(statustip)
         self.checkBoxConfigRomDownloaderDryRun.setStatusTip(QCoreApplication.translate("RomSearch", u"If checked, will not make any changes to filesystem. Default unchecked", None))
 #endif // QT_CONFIG(statustip)
         self.checkBoxConfigRomDownloaderDryRun.setText(QCoreApplication.translate("RomSearch", u"Dry Run", None))
         self.tabWidgetConfig.setTabText(self.tabWidgetConfig.indexOf(self.tabConfigRomDownloader), QCoreApplication.translate("RomSearch", u"ROMDownloader", None))
 #if QT_CONFIG(statustip)
         self.checkBoxConfigDupeParserUseDat.setStatusTip(QCoreApplication.translate("RomSearch", u"Whether to use the dat file to figure out dupes. Default checked", None))
 #endif // QT_CONFIG(statustip)
```

### Comparing `romsearch-0.0.5.post2/romsearch/gui/layout_romsearch.ui` & `romsearch-0.0.6/romsearch/gui/layout_romsearch.ui`

 * *Files 1% similar despite different names*

#### Comparing `romsearch-0.0.5.post2/romsearch/gui/layout_romsearch.ui` & `romsearch-0.0.6/romsearch/gui/layout_romsearch.ui`

```diff
@@ -1064,14 +1064,37 @@
                                     </property>
                                     <property name="checked">
                                       <bool>true</bool>
                                     </property>
                                   </widget>
                                 </item>
                                 <item>
+                                  <widget class="Line" name="lineConfigRomDownloaderSyncAllDividerBottom">
+                                    <property name="frameShadow">
+                                      <enum>QFrame::Shadow::Plain</enum>
+                                    </property>
+                                    <property name="orientation">
+                                      <enum>Qt::Orientation::Horizontal</enum>
+                                    </property>
+                                  </widget>
+                                </item>
+                                <item>
+                                  <widget class="QCheckBox" name="checkBoxConfigRomDownloaderUseAbsoluteUrl">
+                                    <property name="statusTip">
+                                      <string>Whether to treat the remote URL as absolute or relative. Should be unchecked for HTTP remotes</string>
+                                    </property>
+                                    <property name="text">
+                                      <string>Use absolute URL</string>
+                                    </property>
+                                    <property name="checked">
+                                      <bool>true</bool>
+                                    </property>
+                                  </widget>
+                                </item>
+                                <item>
                                   <widget class="Line" name="lineConfigRomDownloaderDryRunTop">
                                     <property name="frameShadow">
                                       <enum>QFrame::Shadow::Plain</enum>
                                     </property>
                                     <property name="orientation">
                                       <enum>Qt::Orientation::Horizontal</enum>
                                     </property>
```

### Comparing `romsearch-0.0.5.post2/romsearch/modules/datparser.py` & `romsearch-0.0.6/romsearch/modules/datparser.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/romsearch/modules/dupeparser.py` & `romsearch-0.0.6/romsearch/modules/dupeparser.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/romsearch/modules/gamefinder.py` & `romsearch-0.0.6/romsearch/modules/gamefinder.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/romsearch/modules/romchooser.py` & `romsearch-0.0.6/romsearch/modules/romchooser.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,40 +124,14 @@
 
         for key in keys_to_pop:
             rom_dict.pop(key)
 
     return rom_dict
 
 
-def get_best_rom_per_region(rom_dict,
-                            region_preferences,
-                            ):
-    """For each individual region, get an overall best ROM"""
-    for reg_pref in region_preferences:
-
-        roms = []
-
-        for key in rom_dict:
-            if reg_pref in rom_dict[key]["regions"]:
-                roms.append(key)
-
-        if len(roms) > 1:
-            roms = get_best_roms(roms, rom_dict)
-
-            keys_to_pop = []
-            for f in rom_dict:
-                if f not in roms and reg_pref in rom_dict[f]["regions"]:
-                    keys_to_pop.append(f)
-
-            for key in keys_to_pop:
-                rom_dict.pop(key)
-
-    return rom_dict
-
-
 def remove_unwanted_roms(rom_dict, key_to_check, check_type="include"):
     """Remove unwanted ROMs from the dict
 
     If we have multiple versions lying around that may be preferred or demoted for some reason, parse them
     out here. Do this per region combo
     """
 
@@ -170,18 +144,18 @@
 
     for region in all_regions:
 
         region_game_keys = [key for key in rom_dict if region in rom_dict[key]["regions"]]
 
         # Only filter things down if we've got multiples here
         if len(region_game_keys) > 1:
-            found_demoted = [rom_dict[key][key_to_check] for key in region_game_keys]
+            found = [rom_dict[key][key_to_check] for key in region_game_keys]
 
             # Remove these, but only if we have some but not all
-            if 0 < sum(found_demoted) < len(found_demoted):
+            if 0 < sum(found) < len(found):
                 for key in region_game_keys:
                     if check_type == "include":
                         if not rom_dict[key][key_to_check]:
                             keys_to_pop.append(key)
                     elif check_type == "exclude":
                         if rom_dict[key][key_to_check]:
                             keys_to_pop.append(key)
@@ -190,53 +164,14 @@
 
     for key in keys_to_pop:
         rom_dict.pop(key)
 
     return rom_dict
 
 
-def get_best_roms(files, rom_dict):
-    """Get the best ROM(s) from a list, using a scoring system"""
-
-    # Positive scores
-    improved_version_score = 1
-    version_score = 10
-    revision_score = 100
-    budget_edition_score = 1000
-
-    # Negative scores
-    demoted_version_score = -1
-    alternate_version_score = -1
-    modern_version_score = -10
-    priority_score = -100
-
-    file_scores = np.zeros(len(files))
-
-    # Improved or demoted versions
-    file_scores += improved_version_score * np.array([int(rom_dict[f]["improved_version"]) for f in files])
-    file_scores += demoted_version_score * np.array([int(rom_dict[f]["demoted_version"]) for f in files])
-    file_scores += budget_edition_score * np.array([int(rom_dict[f]["budget_edition"]) for f in files])
-    file_scores += alternate_version_score * np.array([int(rom_dict[f]["alternate"]) for f in files])
-
-    # Version numbering, which needs to be parsed
-    file_scores += version_score * add_versioned_score(files, rom_dict, "version")
-    file_scores += revision_score * add_versioned_score(files, rom_dict, "revision")
-
-    # Downweight modern versions
-    file_scores += modern_version_score * np.array([int(rom_dict[f]["modern_version"]) for f in files])
-
-    # Priority scoring, where we subtract 1 so that the highest priority has no changed
-    file_scores += priority_score * (np.array([int(rom_dict[f]["priority"]) for f in files]) - 1)
-
-    files_idx = np.where(file_scores == np.nanmax(file_scores))[0]
-    files = np.asarray(files)[files_idx]
-
-    return files
-
-
 def add_versioned_score(files, rom_dict, key):
     """Get an order for versioned strings"""
 
     # Ensure we have a version here. If blank, set to v0
     rom_dict = copy.deepcopy(rom_dict)
     for f in rom_dict:
         if rom_dict[f][key] == "":
@@ -252,48 +187,30 @@
     for i, v in enumerate(versions_sorted):
         v_idx = np.where(versions == v)[0]
         file_scores_version[v_idx] += i
 
     return file_scores_version
 
 
-def filter_by_list(rom_dict,
-                   key,
-                   key_prefs,
-                   ):
-    """Find file with highest value in given list. If there are multiple matches, find the most updated one"""
-
-    roms = []
-
-    found_key = False
-    for key_pref in key_prefs:
-
-        if found_key:
-            continue
-
-        for val in rom_dict:
-            if key_pref in rom_dict[val][key]:
-                roms.append(val)
-                found_key = True
-
-    # If we have multiple matches here, define a best match using scoring system
-    if len(roms) > 1:
-        roms = get_best_roms(roms,
-                             rom_dict,
-                             )
+def add_language_score(files, rom_dict, language_priorities):
+    """Add language scores, include the priority of the order"""
 
-    keys_to_pop = []
-    for f in rom_dict:
-        if f not in roms:
-            keys_to_pop.append(f)
+    language_score_dict = {}
 
-    for key in keys_to_pop:
-        rom_dict.pop(key)
+    # Go backwards so the first entry is highest priority
+    for i, lang in enumerate(language_priorities[::-1]):
+        language_score_dict[lang] = i + 1
+
+    language_scores = np.zeros_like(files, dtype=int)
+    for i, f in enumerate(files):
+        for lang in rom_dict[f]["languages"]:
+            if lang in language_score_dict:
+                language_scores[i] += language_score_dict[lang]
 
-    return rom_dict
+    return language_scores
 
 
 class ROMChooser:
 
     def __init__(self,
                  platform,
                  game,
@@ -452,19 +369,143 @@
             self.logger.debug("Getting best version")
             rom_dict = get_best_version(rom_dict)
             rom_dict = remove_unwanted_roms(rom_dict, key_to_check="improved_versions", check_type="include")
             rom_dict = remove_unwanted_roms(rom_dict, key_to_check="budget_edition", check_type="include")
             rom_dict = remove_unwanted_roms(rom_dict, key_to_check="demoted_versions", check_type="exclude")
             rom_dict = remove_unwanted_roms(rom_dict, key_to_check="modern_versions", check_type="exclude")
             rom_dict = remove_unwanted_roms(rom_dict, key_to_check="alternate", check_type="exclude")
-            rom_dict = get_best_rom_per_region(rom_dict,
-                                               self.region_preferences,
-                                               )
+            rom_dict = self.get_best_rom_per_region(rom_dict,
+                                                    self.region_preferences,
+                                                    )
 
         if not self.allow_multiple_regions:
             self.logger.debug("Trimming down to a single region")
-            rom_dict = filter_by_list(rom_dict,
-                                      "regions",
-                                      self.region_preferences,
+            rom_dict = self.filter_by_list(rom_dict,
+                                           "regions",
+                                           self.region_preferences,
+                                           )
+
+        return rom_dict
+
+    def get_best_roms(self,
+                      files,
+                      rom_dict,
+                      ):
+        """Get the best ROM(s) from a list, using a scoring system"""
+
+        # Positive scores
+        improved_version_score = 1
+        version_score = 1e2
+        revision_score = 1e4
+        budget_edition_score = 1e6
+        language_score = 1e8
+
+        # Negative scores
+        demoted_version_score = -1
+        alternate_version_score = -1
+        modern_version_score = -1e2
+        priority_score = -1e4
+
+        file_scores = np.zeros(len(files))
+
+        # Just stepping through the scores in order.
+
+        # Positive scores
+
+        # Improved version
+        file_scores += improved_version_score * np.array([int(rom_dict[f]["improved_version"]) for f in files])
+
+        # Version numbering, which needs to be parsed. We edit these to only add a little each time
+        version_score_to_add = add_versioned_score(files, rom_dict, "version")
+        file_scores += version_score * (1 + (version_score_to_add - 1) / 100)
+
+        # Revision numbering, again parsed
+        revision_score_to_add = add_versioned_score(files, rom_dict, "revision")
+        file_scores += revision_score * (1 + (revision_score_to_add - 1) / 100)
+
+        # Budget edition
+        file_scores += budget_edition_score * np.array([int(rom_dict[f]["budget_edition"]) for f in files])
+
+        # Language priorities
+        language_score_to_add = add_language_score(files, rom_dict, language_priorities=self.language_preferences)
+        file_scores += language_score * (1 + (language_score_to_add - 1) / 100)
+
+        # Negative scores
+
+        # Demoted version
+        file_scores += demoted_version_score * np.array([int(rom_dict[f]["demoted_version"]) for f in files])
+
+        # Alternate version
+        file_scores += alternate_version_score * np.array([int(rom_dict[f]["alternate"]) for f in files])
+
+        # Modern version
+        file_scores += modern_version_score * np.array([int(rom_dict[f]["modern_version"]) for f in files])
+
+        # Priority scoring. We subtract 1 so that the highest priority has no changed
+        file_scores += priority_score * (np.array([int(rom_dict[f]["priority"]) for f in files]) - 1)
+
+        files_idx = np.where(file_scores == np.nanmax(file_scores))[0]
+        files = np.asarray(files)[files_idx]
+
+        return files
+
+    def get_best_rom_per_region(self,
+                                rom_dict,
+                                region_preferences,
+                                ):
+        """For each individual region, get an overall best ROM"""
+        for reg_pref in region_preferences:
+
+            roms = []
+
+            for key in rom_dict:
+                if reg_pref in rom_dict[key]["regions"]:
+                    roms.append(key)
+
+            if len(roms) > 1:
+                roms = self.get_best_roms(roms, rom_dict)
+
+                keys_to_pop = []
+                for f in rom_dict:
+                    if f not in roms and reg_pref in rom_dict[f]["regions"]:
+                        keys_to_pop.append(f)
+
+                for key in keys_to_pop:
+                    rom_dict.pop(key)
+
+        return rom_dict
+
+    def filter_by_list(self,
+                       rom_dict,
+                       key,
+                       key_prefs,
+                       ):
+        """Find file with highest value in given list. If there are multiple matches, find the most updated one"""
+
+        roms = []
+
+        found_key = False
+        for key_pref in key_prefs:
+
+            if found_key:
+                continue
+
+            for val in rom_dict:
+                if key_pref in rom_dict[val][key]:
+                    roms.append(val)
+                    found_key = True
+
+        # If we have multiple matches here, define a best match using scoring system
+        if len(roms) > 1:
+            roms = self.get_best_roms(roms,
+                                      rom_dict,
                                       )
 
+        keys_to_pop = []
+        for f in rom_dict:
+            if f not in roms:
+                keys_to_pop.append(f)
+
+        for key in keys_to_pop:
+            rom_dict.pop(key)
+
         return rom_dict
```

### Comparing `romsearch-0.0.5.post2/romsearch/modules/rommover.py` & `romsearch-0.0.6/romsearch/modules/rommover.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/romsearch/modules/romparser.py` & `romsearch-0.0.6/romsearch/modules/romparser.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,17 +89,14 @@
             game (str): Game name
             config_file (str, optional): path to config file. Defaults to None.
             config (dict, optional): configuration dictionary. Defaults to None.
             platform_config (dict, optional): platform configuration dictionary. Defaults to None.
             default_config (dict, optional): default configuration dictionary. Defaults to None.
             regex_config (dict, optional): regex configuration dictionary. Defaults to None.
             logger (logging.Logger, optional): logger instance. Defaults to None.
-
-        TODO:
-            - Default implied languages from regions
         """
 
         if platform is None:
             raise ValueError("platform must be specified")
         self.platform = platform
 
         if config_file is None and config is None:
@@ -275,28 +272,54 @@
                 file_dict[dat_cat_dict] = cat_val
 
         return file_dict
 
     def finalise_file_dict(self,
                            file_dict,
                            ):
+        """Do any last minute finalisation to the file dict"""
+
+        file_dict = self.set_game_category(file_dict)
+        file_dict = self.set_implicit_languages(file_dict)
+
+        return file_dict
+
+    def set_game_category(self,
+                          file_dict,
+                          ):
+        """If a dat category hasn't been set, set it to game"""
 
         dat_categories = self.default_config.get("dat_categories", [])
 
         for d in dat_categories:
             d_sanitized = d.lower().replace(" ", "_")
 
             if d_sanitized not in file_dict:
                 file_dict[d_sanitized] = False
 
         if all([file_dict[d.lower().replace(" ", "_")] is False for d in dat_categories]):
             file_dict["games"] = True
 
         return file_dict
 
+    def set_implicit_languages(self,
+                               file_dict,
+                               ):
+        """Set implicit language from region, if we don't already have languages"""
+
+        implied_languages = self.default_config.get("implied_languages", {})
+
+        # Only set if languages is an empty list
+        if not file_dict["languages"]:
+            for r in file_dict["regions"]:
+                if r in implied_languages:
+                    file_dict["languages"].append(implied_languages[r])
+
+        return file_dict
+
     def parse_filename(self, f, file_dict=None):
         """Parse info out of filename"""
 
         if file_dict is None:
             file_dict = {}
 
         # Split file into tags
```

### Comparing `romsearch-0.0.5.post2/romsearch/modules/romsearch.py` & `romsearch-0.0.6/romsearch/modules/romsearch.py`

 * *Files 8% similar despite different names*

```diff
@@ -270,28 +270,25 @@
                 self.logger.debug("ROMMover is not running, will not move anything")
                 continue
 
             # If we filter then download, this is where we download
             if self.romsearch_method == "filter_then_download":
                 all_files = []
                 for game in all_roms_dict:
-
-                    # Make sure we're using the regex escaped version for all the strings
-                    fs = [re.escape(f) for f in all_roms_dict[game]]
+                    fs = [f for f in all_roms_dict[game]]
 
                     all_files.extend(fs)
 
                 if self.run_romdownloader:
                     downloader = ROMDownloader(platform=platform,
                                                config=self.config,
                                                platform_config=platform_config,
                                                logger=self.logger,
-                                               override_includes=all_files,
-                                               override_excludes=[],
-                                               include_filter_wildcard=False,
+                                               rclone_method='copy',
+                                               copy_files=all_files,
                                                )
                     downloader.run()
 
                 # Replace the file time with the correct one on disk
                 for game in all_roms_dict:
 
                     for f in all_roms_dict[game]:
```

### Comparing `romsearch-0.0.5.post2/romsearch/util/__init__.py` & `romsearch-0.0.6/romsearch/util/__init__.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/romsearch/util/general.py` & `romsearch-0.0.6/romsearch/util/general.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/romsearch/util/io.py` & `romsearch-0.0.6/romsearch/util/io.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/romsearch/util/logger.py` & `romsearch-0.0.6/romsearch/util/logger.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/romsearch/util/regex_matching.py` & `romsearch-0.0.6/romsearch/util/regex_matching.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5.post2/romsearch.egg-info/PKG-INFO` & `romsearch-0.0.6/romsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romsearch
-Version: 0.0.5.post2
+Version: 0.0.6
 Summary: One Stop ROM Shop
 Author: bbtufty
 Maintainer: bbtufty
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `romsearch-0.0.5.post2/romsearch.egg-info/SOURCES.txt` & `romsearch-0.0.6/romsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

