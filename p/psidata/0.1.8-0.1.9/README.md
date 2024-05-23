# Comparing `tmp/psidata-0.1.8.tar.gz` & `tmp/psidata-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psidata-0.1.8.tar", last modified: Fri Aug 25 16:28:41 2023, max compression
+gzip compressed data, was "psidata-0.1.9.tar", last modified: Wed Oct 11 21:25:49 2023, max compression
```

## Comparing `psidata-0.1.8.tar` & `psidata-0.1.9.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.378991 psidata-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.370990 psidata-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.374991 psidata-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-08-25 16:28:31.000000 psidata-0.1.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-25 16:28:31.000000 psidata-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-25 16:28:31.000000 psidata-0.1.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-25 16:28:31.000000 psidata-0.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-25 16:28:41.378991 psidata-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-25 16:28:31.000000 psidata-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.374991 psidata-0.1.8/psidata/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-25 16:28:31.000000 psidata-0.1.8/psidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-25 16:28:31.000000 psidata-0.1.8/psidata/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-08-25 16:28:31.000000 psidata-0.1.8/psidata/bcolz_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-08-25 16:28:31.000000 psidata-0.1.8/psidata/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-08-25 16:28:31.000000 psidata-0.1.8/psidata/legacy_bcolz_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-08-25 16:28:31.000000 psidata-0.1.8/psidata/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-08-25 16:28:31.000000 psidata-0.1.8/psidata/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-25 16:28:41.000000 psidata-0.1.8/psidata/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-08-25 16:28:31.000000 psidata-0.1.8/psidata/zarr_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.374991 psidata-0.1.8/psidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-25 16:28:41.000000 psidata-0.1.8/psidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-08-25 16:28:41.000000 psidata-0.1.8/psidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-25 16:28:41.000000 psidata-0.1.8/psidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-25 16:28:41.000000 psidata-0.1.8/psidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-25 16:28:41.000000 psidata-0.1.8/psidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-25 16:28:31.000000 psidata-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-25 16:28:41.378991 psidata-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.374991 psidata-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.370990 psidata-0.1.8/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.374991 psidata-0.1.8/tests/data/bcolz/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/epoch_md.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.374991 psidata-0.1.8/tests/data/bcolz/recording/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.374991 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/__attrs__
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/__rootdirs__
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.374991 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/duration/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/duration/__attrs__
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.374991 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/duration/data/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/duration/data/__0.blp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.374991 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/duration/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/duration/meta/sizes
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/duration/meta/storage
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.374991 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/exclude/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/exclude/__attrs__
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.378991 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/exclude/data/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/exclude/data/__0.blp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.378991 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/exclude/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/exclude/meta/sizes
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/exclude/meta/storage
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.378991 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/t0/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/t0/__attrs__
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.378991 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/t0/data/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/t0/data/__0.blp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.378991 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/t0/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/t0/meta/sizes
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/t0/meta/storage
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.378991 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/trial_number/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/trial_number/__attrs__
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.378991 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/trial_number/data/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/trial_number/data/__0.blp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.378991 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/trial_number/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/trial_number/meta/sizes
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/trial_number/meta/storage
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.378991 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/trial_type/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/trial_type/__attrs__
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.378991 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/trial_type/data/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/trial_type/data/__0.blp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.378991 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/trial_type/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/trial_type/meta/sizes
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md/trial_type/meta/storage
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/epoch_md.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.378991 psidata-0.1.8/tests/data/bcolz/recording/signal/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/signal/__attrs__
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.378991 psidata-0.1.8/tests/data/bcolz/recording/signal/data/
--rw-r--r--   0 runner    (1001) docker     (123)    70118 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/signal/data/__0.blp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 16:28:41.378991 psidata-0.1.8/tests/data/bcolz/recording/signal/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/signal/meta/sizes
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/recording/signal/meta/storage
--rw-r--r--   0 runner    (1001) docker     (123)    80128 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/data/bcolz/signal.npy
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/generate_test_bcolz_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-25 16:28:31.000000 psidata-0.1.8/tests/test_legacy_bcolz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.345785 psidata-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.333785 psidata-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.337785 psidata-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2023-10-11 21:25:36.000000 psidata-0.1.9/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2023-10-11 21:25:36.000000 psidata-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2023-10-11 21:25:36.000000 psidata-0.1.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2023-10-11 21:25:36.000000 psidata-0.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2023-10-11 21:25:49.345785 psidata-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-10-11 21:25:36.000000 psidata-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.337785 psidata-0.1.9/psidata/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2023-10-11 21:25:36.000000 psidata-0.1.9/psidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2023-10-11 21:25:36.000000 psidata-0.1.9/psidata/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2023-10-11 21:25:36.000000 psidata-0.1.9/psidata/bcolz_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2023-10-11 21:25:36.000000 psidata-0.1.9/psidata/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2023-10-11 21:25:36.000000 psidata-0.1.9/psidata/legacy_bcolz_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2023-10-11 21:25:36.000000 psidata-0.1.9/psidata/recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2023-10-11 21:25:36.000000 psidata-0.1.9/psidata/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-11 21:25:49.000000 psidata-0.1.9/psidata/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2023-10-11 21:25:36.000000 psidata-0.1.9/psidata/zarr_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.341785 psidata-0.1.9/psidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2023-10-11 21:25:49.000000 psidata-0.1.9/psidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2023-10-11 21:25:49.000000 psidata-0.1.9/psidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-11 21:25:49.000000 psidata-0.1.9/psidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2023-10-11 21:25:49.000000 psidata-0.1.9/psidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-11 21:25:49.000000 psidata-0.1.9/psidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-10-11 21:25:36.000000 psidata-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-11 21:25:49.345785 psidata-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.341785 psidata-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.333785 psidata-0.1.9/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.341785 psidata-0.1.9/tests/data/bcolz/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/epoch_md.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.341785 psidata-0.1.9/tests/data/bcolz/recording/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.341785 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/__attrs__
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/__rootdirs__
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.341785 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/duration/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/duration/__attrs__
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.341785 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/duration/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/duration/data/__0.blp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.341785 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/duration/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/duration/meta/sizes
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/duration/meta/storage
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.341785 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/exclude/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/exclude/__attrs__
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.341785 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/exclude/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/exclude/data/__0.blp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.341785 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/exclude/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/exclude/meta/sizes
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/exclude/meta/storage
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.341785 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/t0/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/t0/__attrs__
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.341785 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/t0/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/t0/data/__0.blp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.341785 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/t0/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/t0/meta/sizes
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/t0/meta/storage
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.341785 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/trial_number/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/trial_number/__attrs__
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.341785 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/trial_number/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/trial_number/data/__0.blp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.341785 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/trial_number/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/trial_number/meta/sizes
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/trial_number/meta/storage
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.341785 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/trial_type/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/trial_type/__attrs__
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.341785 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/trial_type/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/trial_type/data/__0.blp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.341785 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/trial_type/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/trial_type/meta/sizes
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md/trial_type/meta/storage
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/epoch_md.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.345785 psidata-0.1.9/tests/data/bcolz/recording/signal/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/signal/__attrs__
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.345785 psidata-0.1.9/tests/data/bcolz/recording/signal/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    70118 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/signal/data/__0.blp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 21:25:49.345785 psidata-0.1.9/tests/data/bcolz/recording/signal/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/signal/meta/sizes
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/recording/signal/meta/storage
+-rw-r--r--   0 runner    (1001) docker     (127)    80128 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/data/bcolz/signal.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/generate_test_bcolz_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2023-10-11 21:25:36.000000 psidata-0.1.9/tests/test_legacy_bcolz.py
```

### Comparing `psidata-0.1.8/.github/workflows/publish-to-pypi.yml` & `psidata-0.1.9/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `psidata-0.1.8/.gitignore` & `psidata-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `psidata-0.1.8/LICENSE.txt` & `psidata-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `psidata-0.1.8/PKG-INFO` & `psidata-0.1.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psidata
-Version: 0.1.8
+Version: 0.1.9
 Summary: Lightweight wrapper for managing psiexperiment data
 Author-email: Brad Buran <bburan@alum.mit.edu>, Brad Buran <buran@ohsu.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 Maintainer-email: Brad Buran <bburan@alum.mit.edu>, Brad Buran <buran@ohsu.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 License: MIT License
         
         Copyright (c) 2017-2022 psiepxeriment development team
         
@@ -24,18 +24,28 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: yaml
 Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-console-scripts; extra == "test"
 Provides-Extra: bcolz-backend
+Requires-Dist: bcolz; extra == "bcolz-backend"
 Provides-Extra: legacy-bcolz-backend
+Requires-Dist: blosc; extra == "legacy-bcolz-backend"
 Provides-Extra: zarr-backend
-License-File: LICENSE.txt
+Requires-Dist: zarr; extra == "zarr-backend"
 
 # psidata: tools for processing data collected using psiexperiment
 
 **psidata** is a Python package that provides a simple interface for
 reprocessing data collected using psiexperiment.
```

### Comparing `psidata-0.1.8/psidata/bcolz_tools.py` & `psidata-0.1.9/psidata/bcolz_tools.py`

 * *Files identical despite different names*

### Comparing `psidata-0.1.8/psidata/calibration.py` & `psidata-0.1.9/psidata/calibration.py`

 * *Files identical despite different names*

### Comparing `psidata-0.1.8/psidata/legacy_bcolz_tools.py` & `psidata-0.1.9/psidata/legacy_bcolz_tools.py`

 * *Files identical despite different names*

### Comparing `psidata-0.1.8/psidata/recording.py` & `psidata-0.1.9/psidata/recording.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             If the setting is not identical across all trials.
         KeyError
             If the setting does not exist.
         '''
         table = getattr(self, self._setting_table)
         values = np.unique(table[setting_name])
         if len(values) != 1:
-            raise ValueError('{name} is not unique across all epochs.')
+            raise ValueError(f'{setting_name} is not unique across all epochs.')
         return values[0]
 
     def get_setting_default(self, setting_name, default):
         '''
         Return value for setting
 
         Parameters
```

### Comparing `psidata-0.1.8/psidata/signal.py` & `psidata-0.1.9/psidata/signal.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,16 @@
             Timestamps (in seconds) of segments to load
         offset : float
             Offset (in seconds) relative to timestamp. If a pre-timestamp
             (i.e., prestimulus) baseline is needed, specify a negative number.
         duration : float
             Duration of segment to extract, relative to timestamp + offset.
         ...
+        downsample : {None, int}
+            Decimation factor of signal.
         preload : bool
             If True, load entire array into memory before extracting segments.
             This is usually much faster.
         '''
         if cb is None:
             cb = lambda *a, **kw: None
```

### Comparing `psidata-0.1.8/psidata/zarr_tools.py` & `psidata-0.1.9/psidata/zarr_tools.py`

 * *Files identical despite different names*

### Comparing `psidata-0.1.8/psidata.egg-info/PKG-INFO` & `psidata-0.1.9/psidata.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psidata
-Version: 0.1.8
+Version: 0.1.9
 Summary: Lightweight wrapper for managing psiexperiment data
 Author-email: Brad Buran <bburan@alum.mit.edu>, Brad Buran <buran@ohsu.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 Maintainer-email: Brad Buran <bburan@alum.mit.edu>, Brad Buran <buran@ohsu.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 License: MIT License
         
         Copyright (c) 2017-2022 psiepxeriment development team
         
@@ -24,18 +24,28 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: yaml
 Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-console-scripts; extra == "test"
 Provides-Extra: bcolz-backend
+Requires-Dist: bcolz; extra == "bcolz-backend"
 Provides-Extra: legacy-bcolz-backend
+Requires-Dist: blosc; extra == "legacy-bcolz-backend"
 Provides-Extra: zarr-backend
-License-File: LICENSE.txt
+Requires-Dist: zarr; extra == "zarr-backend"
 
 # psidata: tools for processing data collected using psiexperiment
 
 **psidata** is a Python package that provides a simple interface for
 reprocessing data collected using psiexperiment.
```

### Comparing `psidata-0.1.8/psidata.egg-info/SOURCES.txt` & `psidata-0.1.9/psidata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psidata-0.1.8/pyproject.toml` & `psidata-0.1.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     {name = "Brad Buran", email="bburan@alum.mit.edu"},
     {name = "Brad Buran", email="buran@ohsu.edu"},
     {name = "Buran Consulting, LLC", email="info@bradburan.com"}
 ]
 dependencies = [
     "numpy",
 	"pandas",
+	"yaml",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 docs = ["sphinx", "sphinx_rtd_theme"]
 test = ["pytest", "pytest-console-scripts"]
 bcolz-backend = ["bcolz"]
```

### Comparing `psidata-0.1.8/tests/data/bcolz/recording/signal/data/__0.blp` & `psidata-0.1.9/tests/data/bcolz/recording/signal/data/__0.blp`

 * *Files identical despite different names*

### Comparing `psidata-0.1.8/tests/data/bcolz/signal.npy` & `psidata-0.1.9/tests/data/bcolz/signal.npy`

 * *Files identical despite different names*

### Comparing `psidata-0.1.8/tests/generate_test_bcolz_data.py` & `psidata-0.1.9/tests/generate_test_bcolz_data.py`

 * *Files identical despite different names*

### Comparing `psidata-0.1.8/tests/test_legacy_bcolz.py` & `psidata-0.1.9/tests/test_legacy_bcolz.py`

 * *Files identical despite different names*

