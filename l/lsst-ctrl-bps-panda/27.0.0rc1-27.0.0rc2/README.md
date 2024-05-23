# Comparing `tmp/lsst_ctrl_bps_panda-27.0.0rc1.tar.gz` & `tmp/lsst_ctrl_bps_panda-27.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst_ctrl_bps_panda-27.0.0rc1.tar", last modified: Wed May  1 21:16:39 2024, max compression
+gzip compressed data, was "lsst_ctrl_bps_panda-27.0.0rc2.tar", last modified: Thu May 23 01:52:11 2024, max compression
```

## Comparing `lsst_ctrl_bps_panda-27.0.0rc1.tar` & `lsst_ctrl_bps_panda-27.0.0rc2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.604740 lsst_ctrl_bps_panda-27.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-01 21:16:39.604740 lsst_ctrl_bps_panda-27.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/bsd_license.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.596740 lsst_ctrl_bps_panda-27.0.0rc1/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.596740 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.596740 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.596740 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.600740 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.600740 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.600740 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/cli/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/cli/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/cli/cmd/panda_auth_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/cli/panda_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/cmd_line_embedder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.600740 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/conf_example/
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/conf_example/example_panda_SLAC.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/conf_example/pipelines_check_idf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/conf_example/test_idf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/conf_example/test_sdf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/conf_example/test_usdf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.600740 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/edgenode/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/edgenode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/edgenode/build_cmd_line_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/edgenode/cmd_line_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/panda_auth_drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/panda_auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16267 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/panda_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    28165 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 21:16:39.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.604740 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst_ctrl_bps_panda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-01 21:16:39.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst_ctrl_bps_panda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-01 21:16:39.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst_ctrl_bps_panda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:16:39.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst_ctrl_bps_panda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-01 21:16:39.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst_ctrl_bps_panda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 21:16:39.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst_ctrl_bps_panda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:16:39.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst_ctrl_bps_panda.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-01 21:16:39.604740 lsst_ctrl_bps_panda-27.0.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.604740 lsst_ctrl_bps_panda-27.0.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/tests/test_cmd_line_embedder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/tests/test_panda_auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:11.594782 lsst_ctrl_bps_panda-27.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-23 01:52:11.594782 lsst_ctrl_bps_panda-27.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/bsd_license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:11.586782 lsst_ctrl_bps_panda-27.0.0rc2/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:11.586782 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:11.586782 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:11.586782 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:11.590782 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:11.590782 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:11.590782 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/cli/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/cli/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/cli/cmd/panda_auth_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/cli/panda_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/cmd_line_embedder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:11.590782 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/conf_example/
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/conf_example/example_panda_SLAC.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/conf_example/pipelines_check_idf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/conf_example/test_idf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/conf_example/test_sdf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/conf_example/test_usdf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:11.590782 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/edgenode/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/edgenode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/edgenode/build_cmd_line_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/edgenode/cmd_line_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/panda_auth_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/panda_auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16267 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/panda_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28165 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 01:52:11.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:11.594782 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst_ctrl_bps_panda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-23 01:52:11.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst_ctrl_bps_panda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-23 01:52:11.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst_ctrl_bps_panda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:52:11.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst_ctrl_bps_panda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-23 01:52:11.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst_ctrl_bps_panda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 01:52:11.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst_ctrl_bps_panda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:52:11.000000 lsst_ctrl_bps_panda-27.0.0rc2/python/lsst_ctrl_bps_panda.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-23 01:52:11.594782 lsst_ctrl_bps_panda-27.0.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:11.594782 lsst_ctrl_bps_panda-27.0.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/tests/test_cmd_line_embedder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/tests/test_panda_auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-23 01:52:03.000000 lsst_ctrl_bps_panda-27.0.0rc2/tests/test_utils.py
```

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/PKG-INFO` & `lsst_ctrl_bps_panda-27.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-bps-panda
-Version: 27.0.0rc1
+Version: 27.0.0rc2
 Summary: PanDA plugin for lsst-ctrl-bps.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_bps_panda
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/README.rst` & `lsst_ctrl_bps_panda-27.0.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/bsd_license.txt` & `lsst_ctrl_bps_panda-27.0.0rc2/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/gpl-v3.0.txt` & `lsst_ctrl_bps_panda-27.0.0rc2/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/pyproject.toml` & `lsst_ctrl_bps_panda-27.0.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/__init__.py` & `lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/cli/cmd/__init__.py` & `lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/cli/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/cli/cmd/panda_auth_commands.py` & `lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/cli/cmd/panda_auth_commands.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/cli/panda_auth.py` & `lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/cli/panda_auth.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/cmd_line_embedder.py` & `lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/cmd_line_embedder.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/conf_example/example_panda_SLAC.yaml` & `lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/conf_example/example_panda_SLAC.yaml`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/conf_example/pipelines_check_idf.yaml` & `lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/conf_example/pipelines_check_idf.yaml`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/constants.py` & `lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/constants.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/edgenode/build_cmd_line_decoder.py` & `lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/edgenode/build_cmd_line_decoder.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/edgenode/cmd_line_decoder.py` & `lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/edgenode/cmd_line_decoder.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/panda_auth_drivers.py` & `lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/panda_auth_drivers.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/panda_auth_utils.py` & `lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/panda_auth_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/panda_service.py` & `lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/panda_service.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/utils.py` & `lsst_ctrl_bps_panda-27.0.0rc2/python/lsst/ctrl/bps/panda/utils.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst_ctrl_bps_panda.egg-info/PKG-INFO` & `lsst_ctrl_bps_panda-27.0.0rc2/python/lsst_ctrl_bps_panda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-bps-panda
-Version: 27.0.0rc1
+Version: 27.0.0rc2
 Summary: PanDA plugin for lsst-ctrl-bps.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_bps_panda
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst_ctrl_bps_panda.egg-info/SOURCES.txt` & `lsst_ctrl_bps_panda-27.0.0rc2/python/lsst_ctrl_bps_panda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/tests/test_cmd_line_embedder.py` & `lsst_ctrl_bps_panda-27.0.0rc2/tests/test_cmd_line_embedder.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/tests/test_panda_auth_utils.py` & `lsst_ctrl_bps_panda-27.0.0rc2/tests/test_panda_auth_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_panda-27.0.0rc1/tests/test_utils.py` & `lsst_ctrl_bps_panda-27.0.0rc2/tests/test_utils.py`

 * *Files identical despite different names*

