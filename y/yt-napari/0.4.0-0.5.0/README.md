# Comparing `tmp/yt-napari-0.4.0.tar.gz` & `tmp/yt_napari-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt-napari-0.4.0.tar", last modified: Mon Feb 12 19:25:30 2024, max compression
+gzip compressed data, was "yt_napari-0.5.0.tar", last modified: Thu May 23 19:19:53 2024, max compression
```

## Comparing `yt-napari-0.4.0.tar` & `yt_napari-0.5.0.tar`

### file list

```diff
@@ -1,76 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:25:30.109280 yt-napari-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:25:30.093280 yt-napari-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:25:30.097280 yt-napari-0.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-02-12 19:25:18.000000 yt-napari-0.4.0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-02-12 19:25:18.000000 yt-napari-0.4.0/.github/ISSUE_TEMPLATE/feedback-and-discussion.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:25:30.097280 yt-napari-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-02-12 19:25:18.000000 yt-napari-0.4.0/.github/workflows/check_build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-02-12 19:25:18.000000 yt-napari-0.4.0/.github/workflows/check_manifest.yml
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-02-12 19:25:18.000000 yt-napari-0.4.0/.github/workflows/create_gh_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-02-12 19:25:18.000000 yt-napari-0.4.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-02-12 19:25:18.000000 yt-napari-0.4.0/.github/workflows/weekly_build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-02-12 19:25:18.000000 yt-napari-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-02-12 19:25:18.000000 yt-napari-0.4.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-02-12 19:25:18.000000 yt-napari-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-12 19:25:18.000000 yt-napari-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15288 2024-02-12 19:25:30.109280 yt-napari-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13621 2024-02-12 19:25:18.000000 yt-napari-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-02-12 19:25:19.000000 yt-napari-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-02-12 19:25:30.109280 yt-napari-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-12 19:25:19.000000 yt-napari-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:25:30.093280 yt-napari-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:25:30.101280 yt-napari-0.4.0/src/yt_napari/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_ds_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    13007 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_gui_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    28384 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_model_ingestor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_schema_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_special_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:25:30.105280 yt-napari-0.4.0/src/yt_napari/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_tests/_test_json.json
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_tests/_test_json_slice.json
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_tests/_test_json_timeseries.json
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_tests/_test_json_timeseries_stack.json
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_tests/test_ds_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_tests/test_gui_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_tests/test_metadata_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    17315 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_tests/test_model_ingestor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_tests/test_regions_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_tests/test_schema_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_tests/test_schema_version_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_tests/test_slices_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     7430 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_tests/test_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_tests/test_timeseries_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_tests/test_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_tests/test_widget_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-12 19:25:29.000000 yt-napari-0.4.0/src/yt_napari/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_widget_matadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/_widget_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:25:30.105280 yt-napari-0.4.0/src/yt_napari/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7199 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/schemas/_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/schemas/_version_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/schemas/yt-napari_0.0.1.json
--rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/schemas/yt-napari_0.1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    10072 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/schemas/yt-napari_0.2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    10072 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/schemas/yt-napari_0.2.1.json
--rw-r--r--   0 runner    (1001) docker     (127)    10436 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/schemas/yt-napari_0.3.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/schemas/yt-napari_0.4.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    15556 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)    17568 2024-02-12 19:25:19.000000 yt-napari-0.4.0/src/yt_napari/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:25:30.105280 yt-napari-0.4.0/src/yt_napari.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15288 2024-02-12 19:25:29.000000 yt-napari-0.4.0/src/yt_napari.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-02-12 19:25:30.000000 yt-napari-0.4.0/src/yt_napari.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 19:25:29.000000 yt-napari-0.4.0/src/yt_napari.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-12 19:25:29.000000 yt-napari-0.4.0/src/yt_napari.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-12 19:25:29.000000 yt-napari-0.4.0/src/yt_napari.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-12 19:25:29.000000 yt-napari-0.4.0/src/yt_napari.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:19:53.431334 yt_napari-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:19:53.419334 yt_napari-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:19:53.419334 yt_napari-0.5.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-23 19:19:43.000000 yt_napari-0.5.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-23 19:19:43.000000 yt_napari-0.5.0/.github/ISSUE_TEMPLATE/feedback-and-discussion.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:19:53.423334 yt_napari-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-23 19:19:43.000000 yt_napari-0.5.0/.github/workflows/check_build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-23 19:19:43.000000 yt_napari-0.5.0/.github/workflows/check_manifest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-23 19:19:43.000000 yt_napari-0.5.0/.github/workflows/create_gh_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-23 19:19:43.000000 yt_napari-0.5.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-23 19:19:43.000000 yt_napari-0.5.0/.github/workflows/weekly_build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-23 19:19:43.000000 yt_napari-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-23 19:19:43.000000 yt_napari-0.5.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-23 19:19:43.000000 yt_napari-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-23 19:19:43.000000 yt_napari-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15288 2024-05-23 19:19:53.431334 yt_napari-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13621 2024-05-23 19:19:43.000000 yt_napari-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-23 19:19:43.000000 yt_napari-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-23 19:19:53.435334 yt_napari-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-23 19:19:43.000000 yt_napari-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:19:53.419334 yt_napari-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:19:53.423334 yt_napari-0.5.0/src/yt_napari/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_ds_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14033 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_gui_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29426 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_model_ingestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_schema_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_special_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:19:53.431334 yt_napari-0.5.0/src/yt_napari/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_tests/_test_json.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_tests/_test_json_slice.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_tests/_test_json_timeseries.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_tests/_test_json_timeseries_stack.json
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_tests/test_covering_grid_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_tests/test_ds_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_tests/test_gui_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_tests/test_metadata_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17413 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_tests/test_model_ingestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_tests/test_regions_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_tests/test_schema_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_tests/test_schema_version_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_tests/test_slices_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_tests/test_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_tests/test_timeseries_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_tests/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_tests/test_widget_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 19:19:53.000000 yt_napari-0.5.0/src/yt_napari/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_widget_matadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12656 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/_widget_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:19:53.431334 yt_napari-0.5.0/src/yt_napari/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7199 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/schemas/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/schemas/_version_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/schemas/yt-napari_0.0.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/schemas/yt-napari_0.1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10072 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/schemas/yt-napari_0.2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10072 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/schemas/yt-napari_0.2.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10436 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/schemas/yt-napari_0.3.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/schemas/yt-napari_0.4.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/schemas/yt-napari_0.5.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16866 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20375 2024-05-23 19:19:43.000000 yt_napari-0.5.0/src/yt_napari/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:19:53.431334 yt_napari-0.5.0/src/yt_napari.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15288 2024-05-23 19:19:53.000000 yt_napari-0.5.0/src/yt_napari.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-23 19:19:53.000000 yt_napari-0.5.0/src/yt_napari.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:19:53.000000 yt_napari-0.5.0/src/yt_napari.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 19:19:53.000000 yt_napari-0.5.0/src/yt_napari.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-23 19:19:53.000000 yt_napari-0.5.0/src/yt_napari.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 19:19:53.000000 yt_napari-0.5.0/src/yt_napari.egg-info/top_level.txt
```

### Comparing `yt-napari-0.4.0/.github/ISSUE_TEMPLATE/bug-report.md` & `yt_napari-0.5.0/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/.github/workflows/check_build.yml` & `yt_napari-0.5.0/.github/workflows/check_build.yml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 jobs:
   twinecheck:
     name: twinecheck
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: '3.10'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -U setuptools setuptools_scm wheel twine
     - name: Build and check
```

### Comparing `yt-napari-0.4.0/.github/workflows/check_manifest.yml` & `yt_napari-0.5.0/.github/workflows/check_manifest.yml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 jobs:
   check-manifest:
     runs-on: ubuntu-latest
     steps:
     - name: Checkout Source
       uses: actions/checkout@v4
     - name: Setup Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: '3.10'
     - name: installalation
       run: |
         python -m pip install --upgrade pip
         python -m pip install check-manifest
         python -m pip install .
```

### Comparing `yt-napari-0.4.0/.github/workflows/test_and_deploy.yml` & `yt_napari-0.5.0/.github/workflows/test_and_deploy.yml`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         platform: [ubuntu-latest, windows-latest, macos-latest]
         python-version: ['3.9', '3.10', '3.11']
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       # install libraries that enable testing on Qt on linux
       - name: Install QT libraries for Linux
         uses:  tlambert03/setup-qt-libs@v1
 
@@ -54,36 +54,36 @@
 
       - name: Install dependencies
         run: |
           python -m pip install setuptools tox tox-gh-actions
 
       # this runs the platform-specific tests declared in tox.ini
       - name: Test with tox
-        uses: GabrielBB/xvfb-action@v1
+        uses: aganders3/headless-gui@v2
         with:
           # run tox using the version of Python in `PATH`
           run: |
             tox
         env:
           PLATFORM: ${{ matrix.platform }}
 
       - name: Coverage
-        uses: codecov/codecov-action@v2
+        uses: codecov/codecov-action@v4
 
   deploy:
     # this will run when you have tagged a commit, starting with "v*"
     # and requires that you have put your twine API key in your
     # github secrets (see readme for details)
     needs: [test]
     runs-on: ubuntu-latest
     if: contains(github.ref, 'tags')
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v5
         with:
           python-version: "3.x"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -U setuptools setuptools_scm wheel twine
       - name: Build and publish
```

### Comparing `yt-napari-0.4.0/.github/workflows/weekly_build.yml` & `yt_napari-0.5.0/.github/workflows/weekly_build.yml`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         platform: [ubuntu-latest, windows-latest, macos-latest]
         python-version: ['3.10']
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       # install libraries that enable testing on Qt on linux
       - name: Install QT libraries for Linux
         uses:  tlambert03/setup-qt-libs@v1
 
@@ -36,17 +36,14 @@
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install setuptools tox tox-gh-actions
 
       # this runs the platform-specific tests declared in tox.ini
       - name: Test with tox
-        uses: GabrielBB/xvfb-action@v1
+        uses: aganders3/headless-gui@v2
         with:
           # run tox using the version of Python in `PATH`
           run: |
             tox
         env:
           PLATFORM: ${{ matrix.platform }}
-
-      - name: Coverage
-        uses: codecov/codecov-action@v2
```

### Comparing `yt-napari-0.4.0/.gitignore` & `yt_napari-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/HISTORY.md` & `yt_napari-0.5.0/HISTORY.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+## v0.5.0
+
+### New Features
+* covering grid support ([#120](https://github.com/data-exp-lab/yt-napari/pull/120))
+
+### Maintenance
+* replace np.random.random with new Generator api ([#130](https://github.com/data-exp-lab/yt-napari/pull/130))
+
+
 ## v0.4.0
 This release upgrades required dependencies:
 * napari >= 0.4.19
 * pydantic>2.0
 
 ## v0.3.0
```

### Comparing `yt-napari-0.4.0/LICENSE` & `yt_napari-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/PKG-INFO` & `yt_napari-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-napari
-Version: 0.4.0
+Version: 0.5.0
 Summary: A napari plugin for loading data from yt
 Home-page: https://github.com/data-exp-lab/yt-napari
 Author: Chris Havlin
 Author-email: chris.havlin@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/data-exp-lab/yt-napari/issues
 Project-URL: Documentation, https://github.com/data-exp-lab/yt-napari#README.md
```

### Comparing `yt-napari-0.4.0/README.md` & `yt_napari-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/setup.cfg` & `yt_napari-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/_data_model.py` & `yt_napari-0.5.0/src/yt_napari/_data_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,14 +62,34 @@
     resolution: Tuple[int, int, int] = Field(
         (400, 400, 400),
         description="the resolution at which to sample between the edges.",
     )
     rescale: bool = Field(False, description="rescale the final image between 0,1")
 
 
+class CoveringGrid(_ytBaseModel):
+    fields: List[ytField] = Field(
+        None, description="list of fields to load for this selection"
+    )
+    left_edge: Left_Edge = Field(
+        None,
+        description="the left edge (min x, min y, min z)",
+    )
+    right_edge: Right_Edge = Field(
+        None,
+        description="the right edge (max x, max y, max z)",
+    )
+    level: int = Field(0, description="Grid level to sample at")
+    num_ghost_zones: int = Field(
+        0,
+        description="Number of ghost zones to include",
+    )
+    rescale: bool = Field(False, description="rescale the final image between 0,1")
+
+
 class Slice(_ytBaseModel):
     fields: List[ytField] = Field(
         None, description="list of fields to load for this selection"
     )
     normal: str = Field(None, description="the normal axis of the slice")
     center: Length_Tuple = Field(
         None, description="The center point of the slice, default domain center"
@@ -89,14 +109,17 @@
     )
     rescale: bool = Field(False, description="rescale the final image between 0,1")
 
 
 class SelectionObject(_ytBaseModel):
     regions: List[Region] = Field(None, description="a list of regions to load")
     slices: List[Slice] = Field(None, description="a list of slices to load")
+    covering_grids: List[CoveringGrid] = Field(
+        None, description="a list of covering grids to load"
+    )
 
 
 class DataContainer(_ytBaseModel):
     filename: str = Field(None, description="the filename for the dataset")
     selections: SelectionObject = Field(
         None, description="selections to load in this dataset"
     )
```

### Comparing `yt-napari-0.4.0/src/yt_napari/_ds_cache.py` & `yt_napari-0.5.0/src/yt_napari/_ds_cache.py`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/_gui_utilities.py` & `yt_napari-0.5.0/src/yt_napari/_gui_utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,20 +97,24 @@
 
     def get_widget_instance(self, pydantic_model, field: str):
         # return a widget instance for a given pydantic model and field
         if self.is_registered(pydantic_model, field, required=True):
             func, args, kwargs = self.registry[pydantic_model][field]["magicgui"]
             return func(*args, **kwargs)
 
-    def get_pydantic_attr(self, pydantic_model, field: str, widget_instance):
+    def get_pydantic_attr(
+        self, pydantic_model, field: str, widget_instance, required: bool = True
+    ):
         # given a widget instance, return an object that can be used to set a
         # pydantic field
-        if self.is_registered(pydantic_model, field, required=True):
+        if self.is_registered(pydantic_model, field, required=required):
             func, args, kwargs = self.registry[pydantic_model][field]["pydantic"]
             return func(widget_instance, *args, **kwargs)
+        else:
+            raise RuntimeError("Could not retrieve pydantic attribute.")
 
     def add_pydantic_to_container(
         self,
         py_model: pydantic.BaseModel,
         container: widgets.Container,
         ignore_attrs: Optional[Union[str, List[str]]] = None,
     ):
@@ -210,14 +214,23 @@
     return widgets.FileEdit(*args, **kwargs)
 
 
 def get_filename(file_widget: widgets.FileEdit):
     return str(file_widget.value)
 
 
+def get_int_box_widget(*args, **kwargs):
+    # could remove the need for this if the model uses pathlib.Path for typing
+    return widgets.IntText(*args, **kwargs)
+
+
+def get_int_val(int_box: widgets.IntText):
+    return int(int_box.value)
+
+
 def get_magicguidefault(field_name: str, field_def: pydantic.fields.Field):
     # returns an instance of the default widget selected by magicgui
     # returns an instance of the default widget selected by magicgui
     ftype = field_def.annotation
     opts_dict = dict(name=field_name, annotation=ftype)
     if (
         not type(field_def.default) is PydanticUndefinedType
@@ -225,14 +238,18 @@
     ):
         opts_dict["value"] = field_def.default
     new_widget_cls, ops = type_map.get_widget_class(
         annotation=ftype,
         options=opts_dict,
         raise_on_unknown=False,
     )
+
+    if new_widget_cls == widgets.TupleEdit:
+        ops["options"] = {"min": -1e12, "max": 1e12}
+
     return new_widget_cls(**ops)
 
 
 def embed_in_list(widget_instance) -> list:
     # for when the widget value should be embedded in a list
     returnval = [widget_instance.value]
     return returnval
@@ -251,16 +268,18 @@
     return py_model.model_fields[field]
 
 
 # the following model-field tuples will be embedded in containers
 _models_to_embed_in_list = (
     (_data_model.Slice, "fields"),
     (_data_model.Region, "fields"),
+    (_data_model.CoveringGrid, "fields"),
     (_data_model.DataContainer, "selections"),
     (_data_model.SelectionObject, "regions"),
+    (_data_model.SelectionObject, "covering_grids"),
     (_data_model.SelectionObject, "slices"),
 )
 
 
 def _register_yt_data_model(translator: MagicPydanticRegistry):
     # registers some special cases for pydantic fields.
     translator.register(
@@ -293,14 +312,29 @@
         magicgui_args=(
             "file_list",
             _data_model.TimeSeriesFileSelection.model_fields["file_list"],
         ),
         pydantic_attr_factory=handle_str_list_edit,
     )
 
+    translator.register(
+        _data_model.CoveringGrid,
+        "level",
+        magicgui_factory=get_int_box_widget,
+        magicgui_kwargs={"name": "level"},
+        pydantic_attr_factory=get_int_val,
+    )
+    translator.register(
+        _data_model.CoveringGrid,
+        "num_ghost_zones",
+        magicgui_factory=get_int_box_widget,
+        magicgui_kwargs={"name": "num_ghost_zones"},
+        pydantic_attr_factory=get_int_val,
+    )
+
 
 translator = MagicPydanticRegistry()
 _register_yt_data_model(translator)
 
 
 def get_yt_data_container(
     ignore_attrs: Optional[Union[str, List[str]]] = None,
@@ -314,15 +348,15 @@
         pydantic_model_class,
         data_container,
         ignore_attrs=ignore_attrs,
     )
     return data_container
 
 
-_valid_selections = ("Region", "Slice")
+_valid_selections = ("Region", "Slice", "CoveringGrid")
 
 
 def get_yt_selection_container(selection_type: str, return_native: bool = False):
     # return a container for a single selection
     if selection_type not in _valid_selections:
         raise ValueError(
             f"selection_type must be one of {_valid_selections}, "
```

### Comparing `yt-napari-0.4.0/src/yt_napari/_model_ingestor.py` & `yt_napari-0.5.0/src/yt_napari/_model_ingestor.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import numpy as np
 import yt
 from unyt import unit_object, unit_registry, unyt_array, unyt_quantity
 
 from yt_napari import _special_loaders
 from yt_napari._data_model import (
+    CoveringGrid,
     DataContainer,
     InputModel,
     MetadataModel,
     Region,
     SelectionObject,
     Slice,
     Timeseries,
@@ -25,14 +26,38 @@
 ) -> Tuple[unyt_array, unyt_array]:
     # return the center and width from a left and right edge
     center = (right_edge + left_edge) / 2.0
     width = right_edge - left_edge
     return center, width
 
 
+def _get_covering_grid(
+    ds, left_edge, right_edge, level, num_ghost_zones, test_dims=None
+):
+    # returns a covering grid instance and the resolution of the covering grid
+    if test_dims is None:
+        test_dims = (4, 4, 4)
+    nghostzones = num_ghost_zones
+    temp_cg = ds.covering_grid(level, left_edge, test_dims, num_ghost_zones=nghostzones)
+    effective_dds = temp_cg.dds
+    dims = (right_edge - left_edge) / effective_dds
+    # get the actual covering grid
+    frb = ds.covering_grid(level, left_edge, dims, num_ghost_zones=nghostzones)
+    return frb, dims
+
+
+def _get_region_frb(ds, LE, RE, res):
+    frb = ds.r[
+        LE[0] : RE[0] : complex(0, res[0]),  # noqa: E203
+        LE[1] : RE[1] : complex(0, res[1]),  # noqa: E203
+        LE[2] : RE[2] : complex(0, res[2]),  # noqa: E203
+    ]
+    return frb
+
+
 class LayerDomain:
     # container for domain info for a single layer
     # left_edge, right_edge, resolution, n_d are all self explanatory.
     # other parameters:
     #
     # new_dim_value: optional unyt_quantity.
     #   If n_d == 2, and upgrade_to_3D is subsequently called, then this value
@@ -430,36 +455,41 @@
 
 def _load_3D_regions(
     ds,
     selections: SelectionObject,
     layer_list: list,
     timeseries_container: Optional[TimeseriesContainer] = None,
 ) -> list:
-    for sel in selections.regions:
+
+    sels = []
+    for seltype in ("regions", "covering_grids"):
+        if getattr(selections, seltype) is not None:
+            sels += [sel for sel in getattr(selections, seltype)]
+
+    for sel in sels:
         # get the left, right edge as a unitful array, initialize the layer
         # domain tracking for this layer and update the global domain extent
         if sel.left_edge is None:
             LE = ds.domain_left_edge
         else:
             LE = ds.arr(sel.left_edge.value, sel.left_edge.unit)
 
         if sel.right_edge is None:
             RE = ds.domain_right_edge
         else:
             RE = ds.arr(sel.right_edge.value, sel.right_edge.unit)
-        res = sel.resolution
-        layer_domain = LayerDomain(left_edge=LE, right_edge=RE, resolution=res)
 
-        # create the fixed resolution buffer
-        frb = ds.r[
-            LE[0] : RE[0] : complex(0, res[0]),  # noqa: E203
-            LE[1] : RE[1] : complex(0, res[1]),  # noqa: E203
-            LE[2] : RE[2] : complex(0, res[2]),  # noqa: E203
-        ]
+        if isinstance(sel, Region):
+            res = sel.resolution
+            frb = _get_region_frb(ds, LE, RE, res)
+        elif isinstance(sel, CoveringGrid):
+            frb, dims = _get_covering_grid(ds, LE, RE, sel.level, sel.num_ghost_zones)
+            res = dims
 
+        layer_domain = LayerDomain(left_edge=LE, right_edge=RE, resolution=res)
         for field_container in sel.fields:
             field = (field_container.field_type, field_container.field_name)
 
             data = frb[field]  # extract the field (the slow part)
             if field_container.take_log:
                 data = np.log10(data)
 
@@ -596,15 +626,15 @@
 
 def _load_selections_from_ds(
     ds,
     selections: SelectionObject,
     layer_list: List[SpatialLayer],
     timeseries_container: Optional[TimeseriesContainer] = None,
 ) -> List[SpatialLayer]:
-    if selections.regions is not None:
+    if selections.regions is not None or selections.covering_grids is not None:
         layer_list = _load_3D_regions(
             ds, selections, layer_list, timeseries_container=timeseries_container
         )
     if selections.slices is not None:
         layer_list = _load_2D_slices(
             ds, selections, layer_list, timeseries_container=timeseries_container
         )
```

### Comparing `yt-napari-0.4.0/src/yt_napari/_reader.py` & `yt_napari-0.5.0/src/yt_napari/_reader.py`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/_special_loaders.py` & `yt_napari-0.5.0/src/yt_napari/_special_loaders.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from pathlib import Path
 
 import numpy as np
 import yt
 
 
 def _ytnapari_load_grid():
-    arr = np.random.random(size=(64, 64, 64))
+    rng = np.random.default_rng()
+    arr = rng.random(size=(64, 64, 64))
     d = dict(density=(arr, "g/cm**3"), temperature=(arr, "K"))
     bbox = np.array([[-1.5, 1.5], [-1.5, 1.5], [-1.5, 1.5]])
     shp = arr.shape
     return yt.load_uniform_grid(d, shp, length_unit="Mpc", bbox=bbox, nprocs=64)
 
 
 def _construct_ugrid_timeseries(top_dir: Path, nfiles: int):
```

### Comparing `yt-napari-0.4.0/src/yt_napari/_tests/_test_json.json` & `yt_napari-0.5.0/src/yt_napari/_tests/_test_json.json`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/_tests/_test_json_slice.json` & `yt_napari-0.5.0/src/yt_napari/_tests/_test_json_slice.json`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/_tests/_test_json_timeseries.json` & `yt_napari-0.5.0/src/yt_napari/_tests/_test_json_timeseries.json`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/_tests/_test_json_timeseries_stack.json` & `yt_napari-0.5.0/src/yt_napari/_tests/_test_json_timeseries_stack.json`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/_tests/conftest.py` & `yt_napari-0.5.0/src/yt_napari/_tests/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import yt
 
 
 @pytest.fixture(scope="session")
 def yt_ugrid_ds_fn(tmpdir_factory):
     # this fixture generates a random yt dataset saved to disk that can be
     # re-loaded and sampled.
-    arr = np.random.random(size=(64, 64, 64))
+    rng = np.random.default_rng()
+    arr = rng.random(size=(64, 64, 64))
     d = dict(density=(arr, "g/cm**3"), temperature=(arr, "K"))
     bbox = np.array([[-1.5, 1.5], [-1.5, 1.5], [-1.5, 1.5]])
     shp = arr.shape
     ds = yt.load_uniform_grid(d, shp, length_unit="Mpc", bbox=bbox, nprocs=64)
     ad = ds.all_data()
     fn = str(tmpdir_factory.mktemp("data").join("uniform_grid_data.h5"))
     ad.save_as_dataset(
```

### Comparing `yt-napari-0.4.0/src/yt_napari/_tests/test_config.py` & `yt_napari-0.5.0/src/yt_napari/_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/_tests/test_ds_cache.py` & `yt_napari-0.5.0/src/yt_napari/_tests/test_ds_cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,24 +22,22 @@
     ds_from_store = dataset_cache.get_ds(ds_name)
     assert ds_from_store == ds
     ds_from_store = dataset_cache.most_recent
     assert ds_from_store == ds
 
     dataset_cache.rm_ds(ds_name)
     assert dataset_cache.exists(ds_name) is False
-    assert len(dataset_cache.available) == 0
 
     ds_none = dataset_cache.get_ds("doesnotexist")
     assert ds_none is None
     assert "doesnotexist not found in cache" in caplog.text
 
     dataset_cache.add_ds(ds, ds_name)
     assert dataset_cache.exists(ds_name)
     dataset_cache.rm_all()
-    assert len(dataset_cache.available) == 0
     assert dataset_cache.most_recent is None
 
 
 def test_ds_destruction():
     ds = get_new_ds()
     dataset_cache.add_ds(ds, "hellotest")
     dataset_cache.rm_ds("hellotest")
```

### Comparing `yt-napari-0.4.0/src/yt_napari/_tests/test_gui_utilities.py` & `yt_napari-0.5.0/src/yt_napari/_tests/test_gui_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,18 @@
 
     with pytest.raises(KeyError):
         reg.is_registered(Model, "missing_field", required=True)
 
     pyvalue = reg.get_pydantic_attr(Model, "field_1", widget_instance)
     assert pyvalue == "2_testxyz"
 
+    with pytest.raises(RuntimeError, match="Could not retrieve pydantic attribute."):
+        reg.get_pydantic_attr(
+            Model, "field_does_not_exist", widget_instance, required=False
+        )
     widget_instance.close()
 
 
 def test_yt_widget(backend):
     app = use_app(backend)  # noqa: F841
 
     file_editor = gu.get_file_widget(value="test")
```

### Comparing `yt-napari-0.4.0/src/yt_napari/_tests/test_metadata_widget.py` & `yt_napari-0.5.0/src/yt_napari/_tests/test_metadata_widget.py`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/_tests/test_model_ingestor.py` & `yt_napari-0.5.0/src/yt_napari/_tests/test_model_ingestor.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,17 +207,18 @@
 
 
 def test_reference_layer(domains_to_test):
     # assemble some fake layer tuples
     im_type = "image"
 
     spatial_layer_list = []
+    rng = np.random.default_rng()
     for d in domains_to_test.domain_sets:
         layer_domain = _mi.LayerDomain(d.left_edge, d.right_edge, d.resolution)
-        im = np.random.random(d.resolution)
+        im = rng.random(d.resolution)
         spatial_layer_list.append((im, {}, im_type, layer_domain))
 
     layer_for_ref = spatial_layer_list[0][3]
     ref_layer = _mi.ReferenceLayer(layer_for_ref)
 
     # check that transformations relative to the same layer are null
     scale = ref_layer.calculate_scale(layer_for_ref)
@@ -266,25 +267,26 @@
 
 
 def test_ref_layer_selection(domains_to_test):
     # assemble some fake layer tuples
     im_type = "image"
 
     spatial_layer_list = []
+    rng = np.random.default_rng()
     for d in domains_to_test.domain_sets:
         layer_domain = _mi.LayerDomain(d.left_edge, d.right_edge, d.resolution)
-        im = np.random.random(d.resolution)
+        im = rng.random(d.resolution)
         spatial_layer_list.append((im, {}, im_type, layer_domain))
 
     # add another small volume layer
     le = unyt.unyt_array([0.1, 0.1, 0.1], "m")
     re = unyt.unyt_array([0.2, 0.2, 0.2], "m")
     res = (3, 4, 5)
     small_vol_domain = _mi.LayerDomain(le, re, resolution=res)
-    im = np.random.random(res)
+    im = rng.random(res)
     spatial_layer_list.append((im, {}, im_type, small_vol_domain))
 
     first_ref = _mi._choose_ref_layer(spatial_layer_list, method="first_in_list")
     expected_ref = spatial_layer_list[0][3]
     assert np.all(first_ref.left_edge == expected_ref.left_edge)
     assert np.all(first_ref.right_edge == expected_ref.right_edge)
 
@@ -305,16 +307,16 @@
 
     le = unyt.unyt_array([1, 1], "km")
     re = unyt.unyt_array([2000.0, 2000.0], "m")
     res = (10, 20)
     layer_2d = _mi.LayerDomain(
         le, re, res, n_d=2, new_dim_value=unyt.unyt_quantity(1, "km")
     )
-
-    sp_layer = (np.random.random(res), {}, "testname", layer_2d)
+    rng = np.random.default_rng()
+    sp_layer = (rng.random(res), {}, "testname", layer_2d)
     new_layer_2d = ref.align_sanitize_layer(sp_layer)
     assert "scale" not in new_layer_2d[1]  # no scale when it is all 1
 
 
 @pytest.fixture
 def selection_objs():
     slc_1 = _dm.Slice(
@@ -388,31 +390,31 @@
 
     im_kwargs = {}
     shp = (10, 10, 10)
     # note: domain here is a placeholder, not actually used in tc
     domain = _mi.LayerDomain(
         unyt.unyt_array([0, 0, 0], "m"), unyt.unyt_array([1.0, 1.0, 1.0], "m"), shp
     )
-    im = np.random.random(shp)
+    rng = np.random.default_rng()
+    im = rng.random(shp)
 
-    print("what what")
     for _ in range(3):
         tc.add(reg_1, ("enzo", "temperature"), (im, im_kwargs, "image", domain))
 
     assert len(tc.layers_in_selections[0]) == 3
 
     shp = (10, 10)
     # note: domain here is a placeholder, not actually used in tc
     domain = _mi.LayerDomain(
         unyt.unyt_array([0, 0], "m"),
         unyt.unyt_array([1.0, 1.0], "m"),
         shp,
         n_d=2,
     )
-    im = np.random.random(shp)
+    im = rng.random(shp)
 
     for _ in range(2):
         tc.add(slc_1, ("enzo", "temperature"), (im, im_kwargs, "image", domain))
     for _ in range(2):
         tc.add(slc_3, ("enzo", "temperature"), (im, im_kwargs, "image", domain))
 
     assert len(tc.layers_in_selections[1]) == 4
@@ -490,28 +492,29 @@
 
     files = _mi._generate_file_list("test_fi_blah_???")
     assert len(files) == nfiles
     ytcfg.set("yt", "test_data_dir", init_dir)
 
 
 def test_linear_rescale():
-    data = 10 * np.random.random((5, 5))
+    rng = np.random.default_rng()
+    data = 10 * rng.random((5, 5))
     rsc = _mi._linear_rescale(data)
     assert rsc.min() == 0.0
     assert rsc.max() == 1.0
 
     data[0, 0] = np.nan
     rsc = _mi._linear_rescale(data)
     assert np.nanmin(rsc) == 0.0
     assert np.nanmax(rsc) == 1.0
 
     data[1, 1] = np.inf
     rsc = _mi._linear_rescale(data)
     assert np.nanmin(rsc) == 0.0
     assert np.nanmax(rsc) == 1.0
 
-    data = 10 * np.random.random((5, 5))
+    data = 10 * rng.random((5, 5))
     data[1, 1] = np.inf
     with pytest.warns(RuntimeWarning, match="invalid value"):
         rsc = _mi._linear_rescale(data, fill_inf=False)
         assert np.nanmin(rsc) == 0.0
         assert np.nanmax(rsc) == 0.0
```

### Comparing `yt-napari-0.4.0/src/yt_napari/_tests/test_reader.py` & `yt_napari-0.5.0/src/yt_napari/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/_tests/test_regions_json.py` & `yt_napari-0.5.0/src/yt_napari/_tests/test_regions_json.py`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/_tests/test_schema_manager.py` & `yt_napari-0.5.0/src/yt_napari/_tests/test_schema_manager.py`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/_tests/test_schema_version_comparisons.py` & `yt_napari-0.5.0/src/yt_napari/_tests/test_schema_version_comparisons.py`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/_tests/test_slices_json.py` & `yt_napari-0.5.0/src/yt_napari/_tests/test_slices_json.py`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/_tests/test_timeseries.py` & `yt_napari-0.5.0/src/yt_napari/_tests/test_timeseries.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from yt_napari._special_loaders import _construct_ugrid_timeseries
 
 
 @pytest.fixture(scope="module")
 def yt_ds_0():
     # this fixture generates a random yt dataset saved to disk that can be
     # re-loaded and sampled.
-    arr = np.random.random(size=(16, 16, 16))
+    rng = np.random.default_rng()
+    arr = rng.random(size=(16, 16, 16))
     d = dict(density=(arr, "g/cm**3"), temperature=(arr, "K"))
     bbox = np.array([[-1.5, 1.5], [-1.5, 1.5], [-1.5, 1.5]])
     shp = arr.shape
     ds = yt.load_uniform_grid(d, shp, length_unit="Mpc", bbox=bbox, nprocs=64)
     return ds
 
 
@@ -86,14 +87,21 @@
     assert np.all(reg3._scale == 1.0)
 
     reg4 = ts.Region(_field, resolution=sample_res, take_log=False)
     data4 = reg4.sample_ds(yt_ds_0)
     assert np.all(np.log10(data4) == data)
 
 
+def test_covering_grid(yt_ds_0):
+    cg = ts.CoveringGrid(_field)
+    data = cg.sample_ds(yt_ds_0)
+    # sampled at level 0 for full domain, so should get out the base dimensions
+    assert data.shape == tuple(yt_ds_0.domain_dimensions)
+
+
 def test_slice(yt_ds_0):
     sample_res = (20, 20)
     slc = ts.Slice(_field, "x", resolution=sample_res)
 
     data = slc.sample_ds(yt_ds_0)
     assert data.shape == sample_res
 
@@ -175,15 +183,16 @@
     kwargdict = {}
     ts._validate_scale(selection, kwargdict, True, 10.0)
     assert len(kwargdict["scale"]) == selection.nd + 1
     assert np.any(kwargdict["scale"] != 1.0)
     assert kwargdict["scale"][0] == 10.0
 
     # check that existing scale is not over-ridden
-    sc_scale = np.random.random((selection.nd,))
+    rng = np.random.default_rng()
+    sc_scale = rng.random((selection.nd,))
     kwargdict = {"scale": sc_scale}
     ts._validate_scale(selection, kwargdict, False, 1.0)
     assert np.all(kwargdict["scale"] == sc_scale)
 
     kwargdict = {"scale": sc_scale}
     ts._validate_scale(selection, kwargdict, True, 1.0)
     assert np.all(kwargdict["scale"][1:] == sc_scale)
```

### Comparing `yt-napari-0.4.0/src/yt_napari/_tests/test_timeseries_json.py` & `yt_napari-0.5.0/src/yt_napari/_tests/test_timeseries_json.py`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/_tests/test_viewer.py` & `yt_napari-0.5.0/src/yt_napari/_tests/test_viewer.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,21 @@
     expected_layers += 2  # the above will add layers!
     assert len(viewer.layers) == expected_layers
 
     sc.add_region(viewer, yt_ds, ("gas", "density"), resolution=res)
     expected_layers += 1
     assert len(viewer.layers) == expected_layers
 
+    LE = yt_ds.domain_left_edge
+    dds = yt_ds.domain_width / yt_ds.domain_dimensions
+    RE = yt_ds.arr(LE + dds * 10)
+    sc.add_covering_grid(viewer, yt_ds, ("gas", "density"), left_edge=LE, right_edge=RE)
+    expected_layers += 1
+    assert len(viewer.layers) == expected_layers
+
     # build a new scene so it builds from prior
     sc = Scene()
     sc.add_region(viewer, yt_ds, ("gas", "density"))
     expected_layers += 1
     assert len(viewer.layers) == expected_layers
```

### Comparing `yt-napari-0.4.0/src/yt_napari/_tests/test_widget_reader.py` & `yt_napari-0.5.0/src/yt_napari/_tests/test_widget_reader.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,17 +40,18 @@
     r.deleteLater()
 
 
 def _rebuild_data(final_shape, data):
     # the yt file thats being loaded from the pytest fixture is a saved
     # dataset created from an in-memory uniform grid, and the re-loaded
     # dataset will not have the full functionality of a ds. so here, we
-    # inject a correctly shaped random array here. If we start using full
+    # inject a correctly shaped random array. If we start using full
     # test datasets from yt in testing, this should be changed.
-    return np.random.random(final_shape) * data.mean()
+    rng = np.random.default_rng()
+    return rng.random(final_shape) * data.mean()
 
 
 def test_save_widget_reader(make_napari_viewer, yt_ugrid_ds_fn, tmp_path):
     viewer = make_napari_viewer()
     r = _wr.ReaderWidget(napari_viewer=viewer)
     r.ds_container.filename.value = yt_ugrid_ds_fn
     r.ds_container.store_in_cache.value = False
@@ -232,7 +233,32 @@
         10,
     ]
 
     # ensure that the saved json is a valid model
     _ = InputModel.model_validate(saved_data)
 
     tsr.deleteLater()
+
+
+def test_covering_grid_selection(make_napari_viewer, yt_ugrid_ds_fn):
+    viewer = make_napari_viewer()
+    r = _wr.ReaderWidget(napari_viewer=viewer)
+    r.ds_container.filename.value = yt_ugrid_ds_fn
+    r.ds_container.store_in_cache.value = False
+    r.new_selection_type.setCurrentIndex(2)
+    r.add_new_button.click()
+    assert len(r.active_selections) == 1
+    sel = list(r.active_selections.values())[0]
+    assert isinstance(sel, _wr.SelectionEntry)
+    assert sel.selection_type == "CoveringGrid"
+
+    mgui_region = sel.selection_container_raw
+    mgui_region.fields.field_type.value = "gas"
+    mgui_region.fields.field_name.value = "density"
+    mgui_region.level.value = 0
+
+    mgui_region.left_edge.value.value = (-1.5,) * 3
+    mgui_region.right_edge.value.value = (1.5,) * 3
+    rebuild = partial(_rebuild_data, (64, 64, 64))
+    r._post_load_function = rebuild
+    r.load_data()
+    r.deleteLater()
```

### Comparing `yt-napari-0.4.0/src/yt_napari/_widget_matadata.py` & `yt_napari-0.5.0/src/yt_napari/_widget_matadata.py`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/_widget_reader.py` & `yt_napari-0.5.0/src/yt_napari/_widget_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,14 @@
         self.layout().addLayout(load_group)
 
         ss = widgets.PushButton(text="Save Selection")
         ss.clicked.connect(self.save_selection)
         load_group.addWidget(ss.native)
 
     def save_selection(self):
-        py_kwargs = {}
         py_kwargs = self._validate_data_model()
 
         file_dialog = QFileDialog()
         file_dialog.setFileMode(QFileDialog.AnyFile)
         file_dialog.setAcceptMode(QFileDialog.AcceptSave)
         file_dialog.setNameFilter("JSON Files (*.json);;All Files (*)")
 
@@ -146,15 +145,14 @@
         # same data ingestion function as the json loader.
 
         py_kwargs = self._validate_data_model()
         model = _data_model.InputModel.model_validate(py_kwargs)
 
         # process each layer
         layer_list, _ = _model_ingestor._process_validated_model(model)
-
         # align all layers after checking for or setting the reference layer
         ref_layer = _check_for_reference_layer(self.viewer.layers)
         if ref_layer is None:
             ref_layer = _model_ingestor._choose_ref_layer(layer_list)
         layer_list = ref_layer.align_sanitize_layers(layer_list)
 
         for new_layer in layer_list:
@@ -162,19 +160,21 @@
             if self._post_load_function is not None:
                 im_arr = self._post_load_function(im_arr)
 
             # add the new layer
             self.viewer.add_image(im_arr, **im_kwargs)
 
     def _validate_data_model(self):
-        # this function save json data
+
         selections_by_type = defaultdict(list)
         for selection in self.active_selections.values():
             py_kwargs = selection.get_current_pydantic_kwargs()
             sel_key = selection.selection_type.lower() + "s"
+            if "covering" in sel_key:
+                sel_key = "covering_grids"
             selections_by_type[sel_key].append(py_kwargs)
 
         # next, process remaining arguments (skipping selections):
         py_kwargs = {}
         _gui_utilities.translator.get_pydantic_kwargs(
             self.ds_container,
             self._pydantic_model,
```

### Comparing `yt-napari-0.4.0/src/yt_napari/config.py` & `yt_napari-0.5.0/src/yt_napari/config.py`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/napari.yaml` & `yt_napari-0.5.0/src/yt_napari/napari.yaml`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/schemas/_manager.py` & `yt_napari-0.5.0/src/yt_napari/schemas/_manager.py`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/schemas/_version_comparison.py` & `yt_napari-0.5.0/src/yt_napari/schemas/_version_comparison.py`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/schemas/yt-napari_0.0.1.json` & `yt_napari-0.5.0/src/yt_napari/schemas/yt-napari_0.0.1.json`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/schemas/yt-napari_0.1.0.json` & `yt_napari-0.5.0/src/yt_napari/schemas/yt-napari_0.1.0.json`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/schemas/yt-napari_0.2.0.json` & `yt_napari-0.5.0/src/yt_napari/schemas/yt-napari_0.2.0.json`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/schemas/yt-napari_0.2.1.json` & `yt_napari-0.5.0/src/yt_napari/schemas/yt-napari_0.2.1.json`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/schemas/yt-napari_0.3.0.json` & `yt_napari-0.5.0/src/yt_napari/schemas/yt-napari_0.3.0.json`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/schemas/yt-napari_0.4.0.json` & `yt_napari-0.5.0/src/yt_napari/schemas/yt-napari_0.4.0.json`

 * *Files identical despite different names*

### Comparing `yt-napari-0.4.0/src/yt_napari/timeseries.py` & `yt_napari-0.5.0/src/yt_napari/timeseries.py`

 * *Files 26% similar despite different names*

```diff
@@ -43,50 +43,31 @@
     @staticmethod
     def _validate_unit_tuple(val):
         if isinstance(val, tuple):
             return val[0], val[1]
         return None, None
 
 
-class Region(_Selection):
+class _RegionBase(_Selection, abc.ABC):
     """
-    A 3D rectangular selection through a domain.
-
-    Parameters
-    ----------
-    field: (str, str)
-        a yt field present in all timeseries to load.
-    left_edge: unyt_array or (ndarray, str)
-        (optional) a 3-element unyt_array defining the left edge of the region,
-        defaults to the domain left_edge of each active timestep.
-    right_edge: unyt_array or (ndarray, str)
-        (optional) a 3-element unyt_array defining the right edge of the region,
-        defaults to the domain right_edge of each active timestep.
-    resolution: (int, int, int)
-        (optional) 3-element tuple defining the resolution to sample at. Default
-        is (400, 400, 400).
-    take_log: bool
-        (optional) If True, take the log10 of the sampled field. Defaults to the
-        default behavior for the field in the dataset.
+    Base class for 3D box-like regions
     """
 
     nd = 3
 
     def __init__(
         self,
         field: Tuple[str, str],
         left_edge: Optional[Union[unyt_array, Tuple[np.ndarray, str]]] = None,
         right_edge: Optional[Union[unyt_array, Tuple[np.ndarray, str]]] = None,
-        resolution: Optional[Tuple[int, int, int]] = (400, 400, 400),
         take_log: Optional[bool] = None,
     ):
         super().__init__(field, take_log=take_log)
         self.left_edge = left_edge
         self.right_edge = right_edge
-        self.resolution = resolution
         self._le, self._le_units = self._validate_unit_tuple(left_edge)
         self._re, self._re_units = self._validate_unit_tuple(right_edge)
 
         if self.left_edge is not None and self.right_edge is not None:
             if self._le is not None:
                 LE = self._le
             else:
@@ -98,14 +79,68 @@
                 RE = self.right_edge
             self._calc_aspect_ratio(LE, RE)
 
     def _calc_aspect_ratio(self, LE, RE):
         wid = RE - LE
         self._aspect_ratio = wid / wid[0]
 
+    def _get_edges(self, ds):
+        if self.left_edge is None:
+            LE = ds.domain_left_edge
+        elif self._le is not None:
+            LE = ds.arr(self._le, self._le_units)
+        else:
+            LE = self.left_edge
+
+        if self.right_edge is None:
+            RE = ds.domain_right_edge
+        elif self._re is not None:
+            RE = ds.arr(self._re, self._re_units)
+        else:
+            RE = self.right_edge
+        return LE, RE
+
+
+class Region(_RegionBase):
+    """
+    A 3D rectangular selection through a domain.
+
+    Parameters
+    ----------
+    field: (str, str)
+        a yt field present in all timeseries to load.
+    left_edge: unyt_array or (ndarray, str)
+        (optional) a 3-element unyt_array defining the left edge of the region,
+        defaults to the domain left_edge of each active timestep.
+    right_edge: unyt_array or (ndarray, str)
+        (optional) a 3-element unyt_array defining the right edge of the region,
+        defaults to the domain right_edge of each active timestep.
+    resolution: (int, int, int)
+        (optional) 3-element tuple defining the resolution to sample at. Default
+        is (400, 400, 400).
+    take_log: bool
+        (optional) If True, take the log10 of the sampled field. Defaults to the
+        default behavior for the field in the dataset.
+    """
+
+    nd = 3
+
+    def __init__(
+        self,
+        field: Tuple[str, str],
+        left_edge: Optional[Union[unyt_array, Tuple[np.ndarray, str]]] = None,
+        right_edge: Optional[Union[unyt_array, Tuple[np.ndarray, str]]] = None,
+        resolution: Optional[Tuple[int, int, int]] = (400, 400, 400),
+        take_log: Optional[bool] = None,
+    ):
+        super().__init__(
+            field, left_edge=left_edge, right_edge=right_edge, take_log=take_log
+        )
+        self.resolution = resolution
+
     def sample_ds(self, ds):
         """
         return a fixed resolution sample of a field in a yt dataset.
 
         Parameters
         ----------
         ds : yt dataset
@@ -124,39 +159,54 @@
         >>> reg_data = reg.sample_ds(ds)
 
         Notes
         -----
         This is equivalent to `ds.r[...,...,..][field]`, but is a useful
         abstraction for applying the same selection to a series of datasets.
         """
-        if self.left_edge is None:
-            LE = ds.domain_left_edge
-        elif self._le is not None:
-            LE = ds.arr(self._le, self._le_units)
-        else:
-            LE = self.left_edge
 
-        if self.right_edge is None:
-            RE = ds.domain_right_edge
-        elif self._re is not None:
-            RE = ds.arr(self._re, self._re_units)
-        else:
-            RE = self.right_edge
+        LE, RE = self._get_edges(ds)
 
         res = self.resolution
         if self._aspect_ratio is None:
             self._calc_aspect_ratio(LE, RE)
 
-        # create the fixed resolution buffer
-        frb = ds.r[
-            LE[0] : RE[0] : complex(0, res[0]),  # noqa: E203
-            LE[1] : RE[1] : complex(0, res[1]),  # noqa: E203
-            LE[2] : RE[2] : complex(0, res[2]),  # noqa: E203
-        ]
+        frb = _mi._get_region_frb(ds, LE, RE, res)
+
+        data = frb[self.field]
+        return self._finalize_array(ds, data)
+
+
+class CoveringGrid(_RegionBase):
+
+    def __init__(
+        self,
+        field: Tuple[str, str],
+        left_edge: Optional[Union[unyt_array, Tuple[np.ndarray, str]]] = None,
+        right_edge: Optional[Union[unyt_array, Tuple[np.ndarray, str]]] = None,
+        level: Optional[int] = 0,
+        num_ghost_zones: Optional[int] = 0,
+        take_log: Optional[bool] = None,
+    ):
+
+        super().__init__(
+            field, left_edge=left_edge, right_edge=right_edge, take_log=take_log
+        )
+        self.level = level
+        self.num_ghost_zones = num_ghost_zones
+
+    def sample_ds(self, ds):
+        LE, RE = self._get_edges(ds)
+
+        if self._aspect_ratio is None:
+            self._calc_aspect_ratio(LE, RE)
 
+        frb, _ = _mi._get_covering_grid(
+            ds, LE, RE, self.level, self.num_ghost_zones, test_dims=None
+        )
         data = frb[self.field]
         return self._finalize_array(ds, data)
 
 
 class Slice(_Selection):
     """
     A 2D axis-normal slice through a domain.
```

### Comparing `yt-napari-0.4.0/src/yt_napari/viewer.py` & `yt_napari-0.5.0/src/yt_napari/viewer.py`

 * *Files 6% similar despite different names*

```diff
@@ -196,14 +196,104 @@
             take_log,
             colormap=colormap,
             link_to=link_to,
             rescale=rescale,
             **kwargs,
         )
 
+    def add_covering_grid(
+        self,
+        viewer: Viewer,
+        ds,
+        field: Tuple[str, str],
+        left_edge: Optional[unyt_array] = None,
+        right_edge: Optional[unyt_array] = None,
+        level: Optional[int] = 0,
+        num_ghost_zones: Optional[int] = 0,
+        take_log: Optional[bool] = None,
+        colormap: Optional[str] = None,
+        link_to: Optional[Union[str, Layer]] = None,
+        rescale: Optional[bool] = False,
+        **kwargs,
+    ):
+        """
+        uniformly sample a region from a yt dataset using a covering grid
+        and add it to a viewer
+
+        Parameters
+        ----------
+        viewer: napari.Viewer
+            the active napari viewer
+        ds
+            the yt dataset to sample
+        field: Tuple[str, str]
+            the field tuple to sample  e.g., ('enzo', 'Density')
+        left_edge: unyt_array
+            the left edge of the bounding box
+        right_edge: unyt_array
+            the right edge of the bounding box
+        level: int
+            the level to sample at (default 0)
+        num_ghost_zones: int
+            number of ghost zones to inclue (default 0)
+        take_log : Optional[bool]
+            if True, will take the log of the extracted data. Defaults to the
+            default behavior for the field set by ds.
+        colormap : Optional[str]
+            the color map to use, default is "viridis"
+        link_to : Optional[Union[str, Layer]]
+            specify a layer to which the new layer should link
+        **kwargs :
+            any keyword argument accepted by Viewer.add_image()
+
+        Examples
+        --------
+
+        >>> import napari
+        >>> import yt
+        >>> from yt_napari.viewer import Scene
+        >>> viewer = napari.Viewer()
+        >>> ds = yt.load_sample("IsolatedGalaxy")
+        >>> yt_scene = Scene()
+        >>> yt_scene.add_region(viewer, ds, ("enzo", "Temperature"))
+
+        """
+
+        # set defaults
+        if left_edge is None:
+            left_edge = ds.domain_left_edge
+        if right_edge is None:
+            right_edge = ds.domain_right_edge
+
+        if take_log is None:
+            take_log = ds._get_field_info(field).take_log
+
+        # create the fixed resolution buffer
+        frb, dims = _mi._get_covering_grid(
+            ds, left_edge, right_edge, level, num_ghost_zones
+        )
+        data = frb[field]
+        if take_log:
+            data = np.log10(data)
+
+        # add the bounds of this new layer
+        layer_domain = _mi.LayerDomain(left_edge, right_edge, dims)
+
+        self._add_to_scene(
+            viewer,
+            data,
+            layer_domain,
+            field,
+            take_log,
+            colormap=colormap,
+            link_to=link_to,
+            rescale=rescale,
+            **kwargs,
+        )
+
     def add_to_viewer(
         self,
         viewer: Viewer,
         ds,
         field: Tuple[str, str],
         resolution: Optional[Tuple[int, int, int]] = None,
         left_edge: Optional[unyt_array] = None,
```

### Comparing `yt-napari-0.4.0/src/yt_napari.egg-info/PKG-INFO` & `yt_napari-0.5.0/src/yt_napari.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-napari
-Version: 0.4.0
+Version: 0.5.0
 Summary: A napari plugin for loading data from yt
 Home-page: https://github.com/data-exp-lab/yt-napari
 Author: Chris Havlin
 Author-email: chris.havlin@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/data-exp-lab/yt-napari/issues
 Project-URL: Documentation, https://github.com/data-exp-lab/yt-napari#README.md
```

### Comparing `yt-napari-0.4.0/src/yt_napari.egg-info/SOURCES.txt` & `yt_napari-0.5.0/src/yt_napari.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 src/yt_napari/_tests/__init__.py
 src/yt_napari/_tests/_test_json.json
 src/yt_napari/_tests/_test_json_slice.json
 src/yt_napari/_tests/_test_json_timeseries.json
 src/yt_napari/_tests/_test_json_timeseries_stack.json
 src/yt_napari/_tests/conftest.py
 src/yt_napari/_tests/test_config.py
+src/yt_napari/_tests/test_covering_grid_json.py
 src/yt_napari/_tests/test_ds_cache.py
 src/yt_napari/_tests/test_gui_utilities.py
 src/yt_napari/_tests/test_metadata_widget.py
 src/yt_napari/_tests/test_model_ingestor.py
 src/yt_napari/_tests/test_reader.py
 src/yt_napari/_tests/test_regions_json.py
 src/yt_napari/_tests/test_schema_manager.py
@@ -59,8 +60,9 @@
 src/yt_napari/schemas/_manager.py
 src/yt_napari/schemas/_version_comparison.py
 src/yt_napari/schemas/yt-napari_0.0.1.json
 src/yt_napari/schemas/yt-napari_0.1.0.json
 src/yt_napari/schemas/yt-napari_0.2.0.json
 src/yt_napari/schemas/yt-napari_0.2.1.json
 src/yt_napari/schemas/yt-napari_0.3.0.json
-src/yt_napari/schemas/yt-napari_0.4.0.json
+src/yt_napari/schemas/yt-napari_0.4.0.json
+src/yt_napari/schemas/yt-napari_0.5.0.json
```

