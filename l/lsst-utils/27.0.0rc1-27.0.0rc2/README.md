# Comparing `tmp/lsst_utils-27.0.0rc1.tar.gz` & `tmp/lsst_utils-27.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst_utils-27.0.0rc1.tar", last modified: Wed May  1 21:16:16 2024, max compression
+gzip compressed data, was "lsst_utils-27.0.0rc2.tar", last modified: Thu May 23 01:53:34 2024, max compression
```

## Comparing `lsst_utils-27.0.0rc1.tar` & `lsst_utils-27.0.0rc2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:16.293961 lsst_utils-27.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-01 21:16:16.293961 lsst_utils-27.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:16.277961 lsst_utils-27.0.0rc1/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:16.281961 lsst_utils-27.0.0rc1/doc/lsst.utils/
--rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/doc/lsst.utils/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/doc/lsst.utils/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:16.281961 lsst_utils-27.0.0rc1/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:16.281961 lsst_utils-27.0.0rc1/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:16.285961 lsst_utils-27.0.0rc1/python/lsst/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/_packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11378 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/db_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/doImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/inheritDoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14836 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    24665 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/packages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:16.285961 lsst_utils-27.0.0rc1/python/lsst/utils/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/plotting/limits.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    39013 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/threads.py
--rw-r--r--   0 runner    (1001) docker     (127)    16806 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/usage.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 21:16:16.000000 lsst_utils-27.0.0rc1/python/lsst/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    19205 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:16.293961 lsst_utils-27.0.0rc1/python/lsst_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-01 21:16:16.000000 lsst_utils-27.0.0rc1/python/lsst_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-01 21:16:16.000000 lsst_utils-27.0.0rc1/python/lsst_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:16:16.000000 lsst_utils-27.0.0rc1/python/lsst_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-01 21:16:16.000000 lsst_utils-27.0.0rc1/python/lsst_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 21:16:16.000000 lsst_utils-27.0.0rc1/python/lsst_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:16:15.000000 lsst_utils-27.0.0rc1/python/lsst_utils.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-01 21:16:16.293961 lsst_utils-27.0.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:16.293961 lsst_utils-27.0.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18133 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_db_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_doImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_getPackageDir.py
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_getTempFilePath.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_inheritDoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)     8375 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_plotting_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_threads.py
--rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17166 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:53:34.054531 lsst_utils-27.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-23 01:53:34.054531 lsst_utils-27.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:53:34.038531 lsst_utils-27.0.0rc2/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:53:34.042531 lsst_utils-27.0.0rc2/doc/lsst.utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/doc/lsst.utils/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/doc/lsst.utils/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:53:34.042531 lsst_utils-27.0.0rc2/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:53:34.042531 lsst_utils-27.0.0rc2/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:53:34.046531 lsst_utils-27.0.0rc2/python/lsst/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11378 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/db_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/doImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/inheritDoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14836 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24665 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/packages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:53:34.046531 lsst_utils-27.0.0rc2/python/lsst/utils/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/plotting/limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    39013 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16806 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 01:53:33.000000 lsst_utils-27.0.0rc2/python/lsst/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19205 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:53:34.054531 lsst_utils-27.0.0rc2/python/lsst_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-23 01:53:34.000000 lsst_utils-27.0.0rc2/python/lsst_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-23 01:53:34.000000 lsst_utils-27.0.0rc2/python/lsst_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:53:34.000000 lsst_utils-27.0.0rc2/python/lsst_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-23 01:53:34.000000 lsst_utils-27.0.0rc2/python/lsst_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 01:53:34.000000 lsst_utils-27.0.0rc2/python/lsst_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:53:33.000000 lsst_utils-27.0.0rc2/python/lsst_utils.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-23 01:53:34.054531 lsst_utils-27.0.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:53:34.054531 lsst_utils-27.0.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18133 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_db_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_doImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_getPackageDir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_getTempFilePath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_inheritDoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8375 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_plotting_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17166 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_wrappers.py
```

### Comparing `lsst_utils-27.0.0rc1/LICENSE` & `lsst_utils-27.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/PKG-INFO` & `lsst_utils-27.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-utils
-Version: 27.0.0rc1
+Version: 27.0.0rc2
 Summary: Utility functions from Rubin Observatory Data Management for the Legacy Survey of Space and Time (LSST).
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/utils
 Keywords: lsst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_utils-27.0.0rc1/README.rst` & `lsst_utils-27.0.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/doc/lsst.utils/CHANGES.rst` & `lsst_utils-27.0.0rc2/doc/lsst.utils/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/doc/lsst.utils/index.rst` & `lsst_utils-27.0.0rc2/doc/lsst.utils/index.rst`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/pyproject.toml` & `lsst_utils-27.0.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/python/lsst/utils/__init__.py` & `lsst_utils-27.0.0rc2/python/lsst/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/python/lsst/utils/_packaging.py` & `lsst_utils-27.0.0rc2/python/lsst/utils/_packaging.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/python/lsst/utils/classes.py` & `lsst_utils-27.0.0rc2/python/lsst/utils/classes.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/python/lsst/utils/db_auth.py` & `lsst_utils-27.0.0rc2/python/lsst/utils/db_auth.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/python/lsst/utils/deprecated.py` & `lsst_utils-27.0.0rc2/python/lsst/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/python/lsst/utils/doImport.py` & `lsst_utils-27.0.0rc2/python/lsst/utils/doImport.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/python/lsst/utils/ellipsis.py` & `lsst_utils-27.0.0rc2/python/lsst/utils/ellipsis.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/python/lsst/utils/inheritDoc.py` & `lsst_utils-27.0.0rc2/python/lsst/utils/inheritDoc.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/python/lsst/utils/introspection.py` & `lsst_utils-27.0.0rc2/python/lsst/utils/introspection.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/python/lsst/utils/iteration.py` & `lsst_utils-27.0.0rc2/python/lsst/utils/iteration.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/python/lsst/utils/logging.py` & `lsst_utils-27.0.0rc2/python/lsst/utils/logging.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/python/lsst/utils/packages.py` & `lsst_utils-27.0.0rc2/python/lsst/utils/packages.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/python/lsst/utils/plotting/limits.py` & `lsst_utils-27.0.0rc2/python/lsst/utils/plotting/limits.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/python/lsst/utils/tests.py` & `lsst_utils-27.0.0rc2/python/lsst/utils/tests.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/python/lsst/utils/threads.py` & `lsst_utils-27.0.0rc2/python/lsst/utils/threads.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/python/lsst/utils/timer.py` & `lsst_utils-27.0.0rc2/python/lsst/utils/timer.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/python/lsst/utils/usage.py` & `lsst_utils-27.0.0rc2/python/lsst/utils/usage.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/python/lsst/utils/wrappers.py` & `lsst_utils-27.0.0rc2/python/lsst/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/python/lsst_utils.egg-info/PKG-INFO` & `lsst_utils-27.0.0rc2/python/lsst_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-utils
-Version: 27.0.0rc1
+Version: 27.0.0rc2
 Summary: Utility functions from Rubin Observatory Data Management for the Legacy Survey of Space and Time (LSST).
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/utils
 Keywords: lsst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_utils-27.0.0rc1/python/lsst_utils.egg-info/SOURCES.txt` & `lsst_utils-27.0.0rc2/python/lsst_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/tests/test_classes.py` & `lsst_utils-27.0.0rc2/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/tests/test_db_auth.py` & `lsst_utils-27.0.0rc2/tests/test_db_auth.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/tests/test_decorators.py` & `lsst_utils-27.0.0rc2/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/tests/test_deprecated.py` & `lsst_utils-27.0.0rc2/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/tests/test_doImport.py` & `lsst_utils-27.0.0rc2/tests/test_doImport.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/tests/test_ellipsis.py` & `lsst_utils-27.0.0rc2/tests/test_ellipsis.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/tests/test_executables.py` & `lsst_utils-27.0.0rc2/tests/test_executables.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/tests/test_getPackageDir.py` & `lsst_utils-27.0.0rc2/tests/test_getPackageDir.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/tests/test_getTempFilePath.py` & `lsst_utils-27.0.0rc2/tests/test_getTempFilePath.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/tests/test_import.py` & `lsst_utils-27.0.0rc2/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/tests/test_inheritDoc.py` & `lsst_utils-27.0.0rc2/tests/test_inheritDoc.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/tests/test_introspection.py` & `lsst_utils-27.0.0rc2/tests/test_introspection.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/tests/test_iteration.py` & `lsst_utils-27.0.0rc2/tests/test_iteration.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/tests/test_logging.py` & `lsst_utils-27.0.0rc2/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/tests/test_ordering.py` & `lsst_utils-27.0.0rc2/tests/test_ordering.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/tests/test_packages.py` & `lsst_utils-27.0.0rc2/tests/test_packages.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/tests/test_plotting_limits.py` & `lsst_utils-27.0.0rc2/tests/test_plotting_limits.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/tests/test_threads.py` & `lsst_utils-27.0.0rc2/tests/test_threads.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/tests/test_timer.py` & `lsst_utils-27.0.0rc2/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/tests/test_usage.py` & `lsst_utils-27.0.0rc2/tests/test_usage.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/tests/test_utils.py` & `lsst_utils-27.0.0rc2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc1/tests/test_wrappers.py` & `lsst_utils-27.0.0rc2/tests/test_wrappers.py`

 * *Files identical despite different names*

