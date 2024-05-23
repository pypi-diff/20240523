# Comparing `tmp/alchemlyb-2.2.0.tar.gz` & `tmp/alchemlyb-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchemlyb-2.2.0.tar", last modified: Sat Apr  6 19:25:26 2024, max compression
+gzip compressed data, was "alchemlyb-2.3.0.tar", last modified: Thu May 23 20:03:43 2024, max compression
```

## Comparing `alchemlyb-2.2.0.tar` & `alchemlyb-2.3.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.697085 alchemlyb-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-06 19:25:26.697085 alchemlyb-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-06 19:25:26.697085 alchemlyb-2.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1796 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.685085 alchemlyb-2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.685085 alchemlyb-2.2.0/src/alchemlyb/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-06 19:25:26.697085 alchemlyb-2.2.0/src/alchemlyb/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.689085 alchemlyb-2.2.0/src/alchemlyb/convergence/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/convergence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12546 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/convergence/convergence.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/convergence/pade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.689085 alchemlyb-2.2.0/src/alchemlyb/estimators/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/estimators/bar_.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/estimators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/estimators/mbar_.py
--rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/estimators/ti_.py
--rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/estimators/ti_gaussian_quadrature_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.689085 alchemlyb-2.2.0/src/alchemlyb/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15731 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/parsing/amber.py
--rw-r--r--   0 runner    (1001) docker     (127)    18526 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/parsing/gmx.py
--rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/parsing/gomc.py
--rw-r--r--   0 runner    (1001) docker     (127)    17739 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/parsing/namd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/parsing/parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/parsing/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.689085 alchemlyb-2.2.0/src/alchemlyb/postprocessors/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/postprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/postprocessors/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.693085 alchemlyb-2.2.0/src/alchemlyb/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20197 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/preprocessing/subsampling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.693085 alchemlyb-2.2.0/src/alchemlyb/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.693085 alchemlyb-2.2.0/src/alchemlyb/tests/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_amber.py
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_gmx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_gomc.py
--rw-r--r--   0 runner    (1001) docker     (127)    14652 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_namd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/test_convergence.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/test_fep_estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)    19462 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/test_ti_estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/test_ti_gaussian_quadrature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/test_visualisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    17565 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/test_workflow_ABFE.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.697085 alchemlyb-2.2.0/src/alchemlyb/visualisation/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/visualisation/convergence.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/visualisation/dF_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/visualisation/mbar_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/visualisation/ti_dhdl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.697085 alchemlyb-2.2.0/src/alchemlyb/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33431 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/workflows/abfe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/workflows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.697085 alchemlyb-2.2.0/src/alchemlyb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-06 19:25:26.000000 alchemlyb-2.2.0/src/alchemlyb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-06 19:25:26.000000 alchemlyb-2.2.0/src/alchemlyb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 19:25:26.000000 alchemlyb-2.2.0/src/alchemlyb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-06 19:25:26.000000 alchemlyb-2.2.0/src/alchemlyb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 19:25:26.000000 alchemlyb-2.2.0/src/alchemlyb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:03:43.351217 alchemlyb-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-23 20:03:43.351217 alchemlyb-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-23 20:03:43.351217 alchemlyb-2.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1796 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:03:43.339217 alchemlyb-2.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:03:43.343217 alchemlyb-2.3.0/src/alchemlyb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-23 20:03:43.351217 alchemlyb-2.3.0/src/alchemlyb/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:03:43.343217 alchemlyb-2.3.0/src/alchemlyb/convergence/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/convergence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13790 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/convergence/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/convergence/pade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:03:43.343217 alchemlyb-2.3.0/src/alchemlyb/estimators/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/estimators/bar_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/estimators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/estimators/mbar_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/estimators/ti_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/estimators/ti_gaussian_quadrature_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:03:43.343217 alchemlyb-2.3.0/src/alchemlyb/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15731 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/parsing/amber.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18526 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/parsing/gmx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/parsing/gomc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17739 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/parsing/namd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/parsing/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/parsing/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:03:43.347217 alchemlyb-2.3.0/src/alchemlyb/postprocessors/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/postprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/postprocessors/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:03:43.347217 alchemlyb-2.3.0/src/alchemlyb/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20197 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/preprocessing/subsampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:03:43.347217 alchemlyb-2.3.0/src/alchemlyb/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:03:43.347217 alchemlyb-2.3.0/src/alchemlyb/tests/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/tests/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/tests/parsing/test_amber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/tests/parsing/test_gmx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/tests/parsing/test_gomc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14652 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/tests/parsing/test_namd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/tests/parsing/test_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/tests/parsing/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/tests/test_convergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/tests/test_fep_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19462 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/tests/test_ti_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/tests/test_ti_gaussian_quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/tests/test_visualisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/tests/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17565 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/tests/test_workflow_ABFE.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:03:43.351217 alchemlyb-2.3.0/src/alchemlyb/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/visualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/visualisation/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/visualisation/dF_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/visualisation/mbar_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/visualisation/ti_dhdl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:03:43.351217 alchemlyb-2.3.0/src/alchemlyb/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33431 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/workflows/abfe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/src/alchemlyb/workflows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:03:43.351217 alchemlyb-2.3.0/src/alchemlyb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-23 20:03:43.000000 alchemlyb-2.3.0/src/alchemlyb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-23 20:03:43.000000 alchemlyb-2.3.0/src/alchemlyb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:03:43.000000 alchemlyb-2.3.0/src/alchemlyb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-23 20:03:43.000000 alchemlyb-2.3.0/src/alchemlyb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 20:03:43.000000 alchemlyb-2.3.0/src/alchemlyb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-05-23 20:03:29.000000 alchemlyb-2.3.0/versioneer.py
```

### Comparing `alchemlyb-2.2.0/AUTHORS` & `alchemlyb-2.3.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/LICENSE` & `alchemlyb-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/PKG-INFO` & `alchemlyb-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemlyb
-Version: 2.2.0
+Version: 2.3.0
 Summary: the simple alchemistry library
 Author: David Dotson
 Author-email: dotsdl@gmail.com
 Maintainer: Oliver Beckstein
 Maintainer-email: orbeckst@gmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `alchemlyb-2.2.0/README.rst` & `alchemlyb-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/setup.py` & `alchemlyb-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/__init__.py` & `alchemlyb-2.3.0/src/alchemlyb/__init__.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/convergence/convergence.py` & `alchemlyb-2.3.0/src/alchemlyb/convergence/convergence.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 """Functions for assessing convergence of free energy estimates and raw data."""
 
+from typing import Any, List, Tuple
 from warnings import warn
 
 import numpy as np
 import pandas as pd
 from loguru import logger
+from sklearn.base import BaseEstimator
 
 from .. import concat
 from ..estimators import BAR, TI, MBAR, FEP_ESTIMATORS, TI_ESTIMATORS
 from ..postprocessors.units import to_kT
 
 estimators_dispatch = {"BAR": BAR, "TI": TI, "MBAR": MBAR}
 
 
-def forward_backward_convergence(df_list, estimator="MBAR", num=10, **kwargs):
+def forward_backward_convergence(
+    df_list, estimator="MBAR", num=10, error_tol: float = 3, **kwargs
+):
     """Forward and backward convergence of the free energy estimate.
 
     Generate the free energy estimate as a function of time in both directions,
     with the specified number of equally spaced points in the time
     [Klimovich2015]_. For example, setting `num` to 10 would give the forward
     convergence which is the free energy estimate from the first 10%, 20%, 30%,
     ... of the data. The Backward would give the estimate from the last 10%,
@@ -31,14 +35,20 @@
         Name of the estimators.
         See the important note below on the use of "MBAR".
 
         .. deprecated:: 1.0.0
            Lower case input is also accepted until release 2.0.0.
     num : int
         The number of time points.
+    error_tol : float
+        The maximum error tolerated for analytic error. If the analytic error is
+        bigger than the error tolerance, the bootstrap error will be used.
+
+        .. versionadded:: 2.3.0
+
     kwargs : dict
         Keyword arguments to be passed to the estimator.
 
     Returns
     -------
     :class:`pandas.DataFrame`
         The DataFrame with convergence data. ::
@@ -78,67 +88,47 @@
 
     if estimator not in (FEP_ESTIMATORS + TI_ESTIMATORS):
         msg = f"Estimator {estimator} is not available in {FEP_ESTIMATORS + TI_ESTIMATORS}."
         logger.error(msg)
         raise ValueError(msg)
     else:
         # select estimator class by name
-        estimator_fit = estimators_dispatch[estimator](**kwargs).fit
+        my_estimator = estimators_dispatch[estimator](**kwargs)
         logger.info(f"Use {estimator} estimator for convergence analysis.")
 
     logger.info("Begin forward analysis")
     forward_list = []
     forward_error_list = []
     for i in range(1, num + 1):
         logger.info("Forward analysis: {:.2f}%".format(100 * i / num))
         sample = []
         for data in df_list:
             sample.append(data[: len(data) // num * i])
-        sample = concat(sample)
-        result = estimator_fit(sample)
-        forward_list.append(result.delta_f_.iloc[0, -1])
-        if estimator.lower() == "bar":
-            error = np.sqrt(
-                sum(
-                    [
-                        result.d_delta_f_.iloc[i, i + 1] ** 2
-                        for i in range(len(result.d_delta_f_) - 1)
-                    ]
-                )
-            )
-            forward_error_list.append(error)
-        else:
-            forward_error_list.append(result.d_delta_f_.iloc[0, -1])
+        mean, error = _forward_backward_convergence_estimate(
+            sample, estimator, my_estimator, error_tol, **kwargs
+        )
+        forward_list.append(mean)
+        forward_error_list.append(error)
         logger.info(
             "{:.2f} +/- {:.2f} kT".format(forward_list[-1], forward_error_list[-1])
         )
 
     logger.info("Begin backward analysis")
     backward_list = []
     backward_error_list = []
     for i in range(1, num + 1):
         logger.info("Backward analysis: {:.2f}%".format(100 * i / num))
         sample = []
         for data in df_list:
             sample.append(data[-len(data) // num * i :])
-        sample = concat(sample)
-        result = estimator_fit(sample)
-        backward_list.append(result.delta_f_.iloc[0, -1])
-        if estimator.lower() == "bar":
-            error = np.sqrt(
-                sum(
-                    [
-                        result.d_delta_f_.iloc[i, i + 1] ** 2
-                        for i in range(len(result.d_delta_f_) - 1)
-                    ]
-                )
-            )
-            backward_error_list.append(error)
-        else:
-            backward_error_list.append(result.d_delta_f_.iloc[0, -1])
+        mean, error = _forward_backward_convergence_estimate(
+            sample, estimator, my_estimator, error_tol, **kwargs
+        )
+        backward_list.append(mean)
+        backward_error_list.append(error)
         logger.info(
             "{:.2f} +/- {:.2f} kT".format(backward_list[-1], backward_error_list[-1])
         )
 
     convergence = pd.DataFrame(
         {
             "Forward": forward_list,
@@ -148,14 +138,65 @@
             "data_fraction": [i / num for i in range(1, num + 1)],
         }
     )
     convergence.attrs = df_list[0].attrs
     return convergence
 
 
+def _forward_backward_convergence_estimate(
+    sample_list: List[pd.DataFrame],
+    estimator: str,
+    my_estimator: BaseEstimator,
+    error_tol: float,
+    **kwargs: Any,
+) -> Tuple[float, float]:
+    """Use estimator to run the estimation and return the mean and error.
+
+    Parameters
+    ----------
+    sample_list: A list of samples as pandas Dataframe.
+    estimator: The string of the estimator
+    my_estimator: The estimator object.
+    error_tol: The error tolerance.
+    kwargs
+
+    Returns
+    -------
+        mean: The delta_f between 0 and 1
+        error: The d_delta_f between 0 and 1
+    """
+    sample = concat(sample_list)
+    result = my_estimator.fit(sample)
+    if estimator == "MBAR":
+        my_estimator.initial_f_k = result.delta_f_.iloc[0, :]
+    mean = result.delta_f_.iloc[0, -1]
+    if estimator.lower() == "bar":
+        error = np.sqrt(
+            sum(
+                [
+                    result.d_delta_f_.iloc[i, i + 1] ** 2
+                    for i in range(len(result.d_delta_f_) - 1)
+                ]
+            )
+        )
+    else:
+        error = result.d_delta_f_.iloc[0, -1]
+    if estimator.lower() == "mbar" and error > error_tol:
+        logger.warning(
+            f"Statistical Error ({error}) bigger than error tolerance ({error_tol}), use bootstrap error instead."
+        )
+        bootstraps_estimator = estimators_dispatch[estimator](
+            n_bootstraps=50, initial_f_k=result.delta_f_.iloc[0, :], **kwargs
+        )
+        bootstraps_estimator.fit(sample)
+        error = bootstraps_estimator.d_delta_f_.iloc[0, -1]
+
+    return mean, error
+
+
 def _cummean(vals, out_length):
     """The cumulative mean of an array.
 
     This function computes the cumulative mean and shapes the result to the
     desired length.
 
     Parameters
```

### Comparing `alchemlyb-2.2.0/src/alchemlyb/estimators/bar_.py` & `alchemlyb-2.3.0/src/alchemlyb/estimators/bar_.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/estimators/mbar_.py` & `alchemlyb-2.3.0/src/alchemlyb/estimators/mbar_.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,16 @@
+from __future__ import annotations
+from typing import Literal
+
+import numpy as np
 import pandas as pd
 import pymbar
 from sklearn.base import BaseEstimator
 
+from . import BAR
 from .base import _EstimatorMixOut
 
 
 class MBAR(BaseEstimator, _EstimatorMixOut):
     r"""Multi-state Bennett acceptance ratio (MBAR).
 
     Parameters
@@ -13,17 +18,26 @@
 
     maximum_iterations : int, optional
         Set to limit the maximum number of iterations performed.
 
     relative_tolerance : float, optional
         Set to determine the relative tolerance convergence criteria.
 
-    initial_f_k : np.ndarray, float, shape=(K), optional
-        Set to the initial dimensionless free energies to use as a
-        guess (default None, which sets all :math:`f_k = 0`).
+    initial_f_k : np.ndarray, float, shape=(K), optional or String `BAR`
+        When `isinstance(initial_f_k, np.ndarray)`, `initial_f_k` will be used as
+        initial guess for MBAR estimator. initial_f_k should be dimensionless
+        free energies.
+        When `initial_f_k` is ``None``, ``initial_f_k`` will be set to 0.
+        When `initial_f_k` is set to "BAR", a BAR calculation will be done and
+        the result is used as the initial guess (default).
+
+        .. versionchanged:: 2.3.0
+           The new default is now "BAR" as it provides a substantial speedup
+           over the previous default `None`.
+           
 
     method : str, optional, default="robust"
         The optimization routine to use.  This can be any of the methods
         available via :func:`scipy.optimize.minimize` or
         :func:`scipy.optimize.root`.
 
     n_bootstraps : int, optional
@@ -67,22 +81,27 @@
         `n_bootstraps` option added.
     """
 
     def __init__(
         self,
         maximum_iterations=10000,
         relative_tolerance=1.0e-7,
-        initial_f_k=None,
+        initial_f_k: np.ndarray | Literal["BAR"] | None = "BAR",
         method="robust",
         n_bootstraps=0,
         verbose=False,
     ):
         self.maximum_iterations = maximum_iterations
         self.relative_tolerance = relative_tolerance
-        self.initial_f_k = initial_f_k
+        if isinstance(initial_f_k, str) and initial_f_k != "BAR":
+            raise ValueError(
+                f"Only `BAR` is supported as string input to `initial_f_k`. Got ({initial_f_k})."
+            )
+        else:
+            self.initial_f_k = initial_f_k
         self.method = method
         self.verbose = verbose
         self.n_bootstraps = n_bootstraps
 
         # handle for pymbar.MBAR object
         self._mbar = None
 
@@ -104,21 +123,32 @@
         groups = u_nk.groupby(level=u_nk.index.names[1:])
         N_k = [
             (len(groups.get_group(i)) if i in groups.groups else 0)
             for i in u_nk.columns
         ]
         self._states_ = u_nk.columns.values.tolist()
 
+        if isinstance(self.initial_f_k, str) and self.initial_f_k == "BAR":
+            bar = BAR(
+                maximum_iterations=self.maximum_iterations,
+                relative_tolerance=self.relative_tolerance,
+                verbose=self.verbose,
+            )
+            bar.fit(u_nk)
+            initial_f_k = bar.delta_f_.iloc[0, :]
+        else:
+            initial_f_k = self.initial_f_k
+
         self._mbar = pymbar.MBAR(
             u_nk.T,
             N_k,
             maximum_iterations=self.maximum_iterations,
             relative_tolerance=self.relative_tolerance,
             verbose=self.verbose,
-            initial_f_k=self.initial_f_k,
+            initial_f_k=initial_f_k,
             solver_protocol=self.method,
             n_bootstraps=self.n_bootstraps,
         )
         if self.n_bootstraps == 0:
             uncertainty_method = None
         else:
             uncertainty_method = "bootstrap"
```

### Comparing `alchemlyb-2.2.0/src/alchemlyb/estimators/ti_.py` & `alchemlyb-2.3.0/src/alchemlyb/estimators/ti_.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/estimators/ti_gaussian_quadrature_.py` & `alchemlyb-2.3.0/src/alchemlyb/estimators/ti_gaussian_quadrature_.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/parsing/__init__.py` & `alchemlyb-2.3.0/src/alchemlyb/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/parsing/amber.py` & `alchemlyb-2.3.0/src/alchemlyb/parsing/amber.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/parsing/gmx.py` & `alchemlyb-2.3.0/src/alchemlyb/parsing/gmx.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/parsing/gomc.py` & `alchemlyb-2.3.0/src/alchemlyb/parsing/gomc.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/parsing/namd.py` & `alchemlyb-2.3.0/src/alchemlyb/parsing/namd.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/parsing/parquet.py` & `alchemlyb-2.3.0/src/alchemlyb/parsing/parquet.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/parsing/util.py` & `alchemlyb-2.3.0/src/alchemlyb/parsing/util.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/postprocessors/units.py` & `alchemlyb-2.3.0/src/alchemlyb/postprocessors/units.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/preprocessing/__init__.py` & `alchemlyb-2.3.0/src/alchemlyb/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/preprocessing/subsampling.py` & `alchemlyb-2.3.0/src/alchemlyb/preprocessing/subsampling.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/tests/conftest.py` & `alchemlyb-2.3.0/src/alchemlyb/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_amber.py` & `alchemlyb-2.3.0/src/alchemlyb/tests/parsing/test_amber.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_gmx.py` & `alchemlyb-2.3.0/src/alchemlyb/tests/parsing/test_gmx.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_gomc.py` & `alchemlyb-2.3.0/src/alchemlyb/tests/parsing/test_gomc.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_namd.py` & `alchemlyb-2.3.0/src/alchemlyb/tests/parsing/test_namd.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_parquet.py` & `alchemlyb-2.3.0/src/alchemlyb/tests/parsing/test_parquet.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_util.py` & `alchemlyb-2.3.0/src/alchemlyb/tests/parsing/test_util.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/tests/test_convergence.py` & `alchemlyb-2.3.0/src/alchemlyb/tests/test_convergence.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,14 +32,23 @@
 
 
 def test_convergence_wrong_cases(gmx_benzene_Coulomb_u_nk):
     with pytest.warns(DeprecationWarning, match="Using lower-case strings for"):
         forward_backward_convergence(gmx_benzene_Coulomb_u_nk, "mbar")
 
 
+def test_convergence_bootstrap(gmx_benzene_Coulomb_u_nk, caplog):
+    normal_c = forward_backward_convergence(gmx_benzene_Coulomb_u_nk, "mbar", num=2)
+    bootstrap_c = forward_backward_convergence(
+        gmx_benzene_Coulomb_u_nk, "mbar", error_tol=0.01, num=2
+    )
+    assert "use bootstrap error instead." in caplog.text
+    assert (bootstrap_c["Forward_Error"] != normal_c["Forward_Error"]).all()
+
+
 def test_convergence_method(gmx_benzene_Coulomb_u_nk):
     convergence = forward_backward_convergence(
         gmx_benzene_Coulomb_u_nk, "MBAR", num=2, method="adaptive"
     )
     assert len(convergence) == 2
```

### Comparing `alchemlyb-2.2.0/src/alchemlyb/tests/test_fep_estimators.py` & `alchemlyb-2.3.0/src/alchemlyb/tests/test_fep_estimators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Tests for all FEP-based estimators in ``alchemlyb``.
 
 """
 
+import numpy as np
 import pytest
 
 import alchemlyb
 from alchemlyb.estimators import MBAR, BAR
 
 
 class FEPestimatorMixin:
@@ -147,7 +148,22 @@
     mbar = MBAR()
     mbar.fit(u_nk)
     mbar_mean = mbar.delta_f_.loc[0.00, 1.00]
     mbar_err = mbar.d_delta_f_.loc[0.00, 1.00]
 
     assert mbar_bootstrap_mean == mbar_mean
     assert mbar_bootstrap_err != mbar_err
+
+
+def test_wrong_initial_f_k():
+    with pytest.raises(
+        ValueError, match="Only `BAR` is supported as string input to `initial_f_k`"
+    ):
+        MBAR(initial_f_k="aaa")
+
+
+@pytest.mark.parametrize("initial_f_k", ["BAR", None])
+def test_initial_f_k(gmx_benzene_Coulomb_u_nk, initial_f_k):
+    u_nk = alchemlyb.concat(gmx_benzene_Coulomb_u_nk)
+    mbar = MBAR(initial_f_k=initial_f_k)
+    mbar.fit(u_nk)
+    assert np.isclose(mbar.delta_f_.loc[0.00, 1.00], 3.0411556983908046)
```

### Comparing `alchemlyb-2.2.0/src/alchemlyb/tests/test_preprocessing.py` & `alchemlyb-2.3.0/src/alchemlyb/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/tests/test_ti_estimators.py` & `alchemlyb-2.3.0/src/alchemlyb/tests/test_ti_estimators.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/tests/test_ti_gaussian_quadrature.py` & `alchemlyb-2.3.0/src/alchemlyb/tests/test_ti_gaussian_quadrature.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/tests/test_units.py` & `alchemlyb-2.3.0/src/alchemlyb/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/tests/test_visualisation.py` & `alchemlyb-2.3.0/src/alchemlyb/tests/test_visualisation.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/tests/test_workflow.py` & `alchemlyb-2.3.0/src/alchemlyb/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/tests/test_workflow_ABFE.py` & `alchemlyb-2.3.0/src/alchemlyb/tests/test_workflow_ABFE.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/visualisation/convergence.py` & `alchemlyb-2.3.0/src/alchemlyb/visualisation/convergence.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/visualisation/dF_state.py` & `alchemlyb-2.3.0/src/alchemlyb/visualisation/dF_state.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/visualisation/mbar_matrix.py` & `alchemlyb-2.3.0/src/alchemlyb/visualisation/mbar_matrix.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/visualisation/ti_dhdl.py` & `alchemlyb-2.3.0/src/alchemlyb/visualisation/ti_dhdl.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/workflows/abfe.py` & `alchemlyb-2.3.0/src/alchemlyb/workflows/abfe.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb/workflows/base.py` & `alchemlyb-2.3.0/src/alchemlyb/workflows/base.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/src/alchemlyb.egg-info/PKG-INFO` & `alchemlyb-2.3.0/src/alchemlyb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemlyb
-Version: 2.2.0
+Version: 2.3.0
 Summary: the simple alchemistry library
 Author: David Dotson
 Author-email: dotsdl@gmail.com
 Maintainer: Oliver Beckstein
 Maintainer-email: orbeckst@gmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `alchemlyb-2.2.0/src/alchemlyb.egg-info/SOURCES.txt` & `alchemlyb-2.3.0/src/alchemlyb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.2.0/versioneer.py` & `alchemlyb-2.3.0/versioneer.py`

 * *Files identical despite different names*

