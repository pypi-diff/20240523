# Comparing `tmp/psi4_step-2024.3.4.tar.gz` & `tmp/psi4_step-2024.5.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psi4_step-2024.3.4.tar", last modified: Mon Mar  4 18:30:45 2024, max compression
+gzip compressed data, was "psi4_step-2024.5.23.tar", last modified: Thu May 23 14:34:11 2024, max compression
```

## Comparing `psi4_step-2024.3.4.tar` & `psi4_step-2024.5.23.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:30:45.190900 psi4_step-2024.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-03-04 18:30:45.190900 psi4_step-2024.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:30:45.178900 psi4_step-2024.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:30:45.178900 psi4_step-2024.3.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:30:45.178900 psi4_step-2024.3.4/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     9473 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:30:45.178900 psi4_step-2024.3.4/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:30:45.178900 psi4_step-2024.3.4/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:30:45.182900 psi4_step-2024.3.4/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:30:45.190900 psi4_step-2024.3.4/psi4_step/
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      428 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-04 18:30:45.190900 psi4_step-2024.3.4/psi4_step/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    52653 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/accelerated_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/accelerated_optimization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/accelerated_optimization_step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:30:45.190900 psi4_step-2024.3.4/psi4_step/data/
--rwxr-xr-x   0 runner    (1001) docker     (127)    12556 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/data/MOPAC_PM7_Hessian.flow
--rwxr-xr-x   0 runner    (1001) docker     (127)    11273 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/data/MOPAC_PM7_SPE.flow
--rwxr-xr-x   0 runner    (1001) docker     (127)    12933 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/data/MOPAC_PM7_surrogate.flow
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/data/configuration.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/data/opt_log.out
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/data/properties.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/data/psi4.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/data/seamm-psi4.yml
--rw-r--r--   0 runner    (1001) docker     (127)    17567 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/energy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/energy_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/initialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/initialization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/initialization_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/optimization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/optimization_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19732 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/psi4.py
--rw-r--r--   0 runner    (1001) docker     (127)    90749 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/psi4_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/psi4_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/psi4_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    11922 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/thermochemistry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/thermochemistry_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/thermochemistry_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/tk_accelerated_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/tk_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/tk_initialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/tk_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/tk_psi4.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/psi4_step/tk_thermochemistry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:30:45.190900 psi4_step-2024.3.4/psi4_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-03-04 18:30:45.000000 psi4_step-2024.3.4/psi4_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-04 18:30:45.000000 psi4_step-2024.3.4/psi4_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 18:30:45.000000 psi4_step-2024.3.4/psi4_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-04 18:30:45.000000 psi4_step-2024.3.4/psi4_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-04 18:30:45.000000 psi4_step-2024.3.4/psi4_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-04 18:30:45.000000 psi4_step-2024.3.4/psi4_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 18:30:32.000000 psi4_step-2024.3.4/psi4_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-04 18:30:45.190900 psi4_step-2024.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:30:45.190900 psi4_step-2024.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/tests/test_psi4_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-03-04 18:30:29.000000 psi4_step-2024.3.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:34:11.685484 psi4_step-2024.5.23/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-23 14:34:11.685484 psi4_step-2024.5.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:34:11.673484 psi4_step-2024.5.23/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:34:11.673484 psi4_step-2024.5.23/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:34:11.677484 psi4_step-2024.5.23/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9473 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:34:11.677484 psi4_step-2024.5.23/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:34:11.677484 psi4_step-2024.5.23/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:34:11.677484 psi4_step-2024.5.23/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:34:11.685484 psi4_step-2024.5.23/psi4_step/
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      428 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-23 14:34:11.685484 psi4_step-2024.5.23/psi4_step/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52653 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/accelerated_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/accelerated_optimization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/accelerated_optimization_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:34:11.685484 psi4_step-2024.5.23/psi4_step/data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12556 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/data/MOPAC_PM7_Hessian.flow
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11273 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/data/MOPAC_PM7_SPE.flow
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12933 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/data/MOPAC_PM7_surrogate.flow
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/data/configuration.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/data/opt_log.out
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/data/properties.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/data/psi4.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/data/seamm-psi4.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    17818 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/energy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/energy_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/initialization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/initialization_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8795 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/optimization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/optimization_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19732 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/psi4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91066 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/psi4_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/psi4_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/psi4_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11922 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/thermochemistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/thermochemistry_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/thermochemistry_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/tk_accelerated_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/tk_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/tk_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/tk_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/tk_psi4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/psi4_step/tk_thermochemistry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:34:11.685484 psi4_step-2024.5.23/psi4_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-23 14:34:11.000000 psi4_step-2024.5.23/psi4_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-23 14:34:11.000000 psi4_step-2024.5.23/psi4_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:34:11.000000 psi4_step-2024.5.23/psi4_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-23 14:34:11.000000 psi4_step-2024.5.23/psi4_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-23 14:34:11.000000 psi4_step-2024.5.23/psi4_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 14:34:11.000000 psi4_step-2024.5.23/psi4_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:33:55.000000 psi4_step-2024.5.23/psi4_step.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-23 14:34:11.685484 psi4_step-2024.5.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:34:11.685484 psi4_step-2024.5.23/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/tests/test_psi4_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-05-23 14:33:52.000000 psi4_step-2024.5.23/versioneer.py
```

### Comparing `psi4_step-2024.3.4/CONTRIBUTING.rst` & `psi4_step-2024.5.23/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/HISTORY.rst` & `psi4_step-2024.5.23/HISTORY.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 =======
 History
 =======
+2024.5.23 -- Added standard energy and gradients to results
+   * Added 'energy' and 'gradients' to optional results to support e.g. Energy Scan
+   * Fixed crashing bug in description of the Energy substep.
+     
+2024.3.17 -- Updated the installer
+   * Updated the installer to use the new version of the SEAMM installer.
+   * Finalizes installing either with Conda or Docker
+     
 2024.3.4 -- Allowing short names for method and DFT functionals
    * Added short names for the methods (Hamiltonians)  and DFT functionals.
    * Catch errors in Psi4 calculating properties for e.g. CISD(T) method
 
 2024.2.29 -- Completed support for containers
    * Fixed issues with running amd64 containers on arm64 systems.
```

### Comparing `psi4_step-2024.3.4/LICENSE` & `psi4_step-2024.5.23/LICENSE`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/PKG-INFO` & `psi4_step-2024.5.23/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psi4_step
-Version: 2024.3.4
+Version: 2024.5.23
 Summary: A SEAMM plug-in to setup, run and analyze quantum chemistry calculations using Psi4
 Home-page: https://github.com/molssi-seamm/psi4_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,Psi4,DFT,quantum chemistry,CCSD
 Platform: Linux
@@ -96,14 +96,22 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2024.5.23 -- Added standard energy and gradients to results
+   * Added 'energy' and 'gradients' to optional results to support e.g. Energy Scan
+   * Fixed crashing bug in description of the Energy substep.
+     
+2024.3.17 -- Updated the installer
+   * Updated the installer to use the new version of the SEAMM installer.
+   * Finalizes installing either with Conda or Docker
+     
 2024.3.4 -- Allowing short names for method and DFT functionals
    * Added short names for the methods (Hamiltonians)  and DFT functionals.
    * Catch errors in Psi4 calculating properties for e.g. CISD(T) method
 
 2024.2.29 -- Completed support for containers
    * Fixed issues with running amd64 containers on arm64 systems.
```

### Comparing `psi4_step-2024.3.4/README.rst` & `psi4_step-2024.5.23/README.rst`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/docs/Makefile` & `psi4_step-2024.5.23/docs/Makefile`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/docs/_static/SEAMM inverted.png` & `psi4_step-2024.5.23/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/docs/_static/SEAMM logo.png` & `psi4_step-2024.5.23/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/docs/_static/molssi_main_logo.png` & `psi4_step-2024.5.23/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/docs/_static/molssi_main_logo_inverted_white.png` & `psi4_step-2024.5.23/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/docs/_static/molssi_square.png` & `psi4_step-2024.5.23/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/docs/_static/nsf.png` & `psi4_step-2024.5.23/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/docs/conf.py` & `psi4_step-2024.5.23/docs/conf.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/docs/developer_guide/installation.rst` & `psi4_step-2024.5.23/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/docs/getting_started/index.rst` & `psi4_step-2024.5.23/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/docs/index.rst` & `psi4_step-2024.5.23/docs/index.rst`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/docs/make.bat` & `psi4_step-2024.5.23/docs/make.bat`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/__init__.py` & `psi4_step-2024.5.23/psi4_step/__init__.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/accelerated_optimization.py` & `psi4_step-2024.5.23/psi4_step/accelerated_optimization.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/accelerated_optimization_parameters.py` & `psi4_step-2024.5.23/psi4_step/accelerated_optimization_parameters.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/accelerated_optimization_step.py` & `psi4_step-2024.5.23/psi4_step/accelerated_optimization_step.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/data/MOPAC_PM7_Hessian.flow` & `psi4_step-2024.5.23/psi4_step/data/MOPAC_PM7_Hessian.flow`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/data/MOPAC_PM7_SPE.flow` & `psi4_step-2024.5.23/psi4_step/data/MOPAC_PM7_SPE.flow`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/data/MOPAC_PM7_surrogate.flow` & `psi4_step-2024.5.23/psi4_step/data/MOPAC_PM7_surrogate.flow`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/data/references.bib` & `psi4_step-2024.5.23/psi4_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/energy.py` & `psi4_step-2024.5.23/psi4_step/energy.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         self,
         P=None,
         calculation_type="Single-point energy",
         configuration=None,
     ):
         """Prepare information about what this node will do"""
 
-        if P is not None:
+        if P is None:
             P = self.parameters.values_to_dict()
 
         if P["level"] == "recommended":
             method = P["method"]
         else:
             method = P["advanced_method"]
 
@@ -269,14 +269,15 @@
                 and len(psi4_step.dft_functionals[functional_string]["dispersion"]) > 1
             ):
                 functional = functional + "-" + P["dispersion"]
             if restart is None:
                 lines.append(
                     f"Eelec, wfn = {calculation_type}('{functional}', return_wfn=True)"
                 )
+                lines.append(f"G = gradient('{functional}', ref_wfn=wfn)")
             else:
                 if calculation_type == "gradient":
                     lines.append(
                         f"Eelec, wfn = energy('{functional}', return_wfn=True,"
                         f" restart_file='{restart}')"
                     )
                     lines.append(f"G = gradient('{functional}', ref_wfn=wfn)")
@@ -286,14 +287,15 @@
                         f"return_wfn=True, restart_file='{restart}')"
                     )
         else:
             if restart is None:
                 lines.append(
                     f"Eelec, wfn = {calculation_type}('{method}', return_wfn=True)"
                 )
+                lines.append(f"G = gradient('{method}', ref_wfn=wfn)")
             else:
                 if calculation_type == "gradient":
                     lines.append(
                         f"Eelec, wfn = energy('{method}', return_wfn=True, "
                         f" restart_file='{restart}')"
                     )
                     lines.append(f"G = gradient('{method}', ref_wfn=wfn)")
@@ -328,14 +330,19 @@
 arrays = array_variables()
 for item in arrays:
     variables[item] = array_variable(item).np.tolist()
 arrays = wfn.array_variables()
 for item in arrays:
     variables[item] = wfn.array_variable(item).np.tolist()
 variables["Eelec"] = Eelec
+variables["energy"] = Eelec
+try:
+    variables["gradient"] = np.array(G).tolist()
+except Exception:
+    pass
 variables["_method"] = "{method}"
 variables["_method_string"] = "{method_string}"
 
 
 with open("{filename}", "w") as fd:
     json.dump(fix_multipoles(variables), fd, sort_keys=True, indent=3)
 """
```

### Comparing `psi4_step-2024.3.4/psi4_step/energy_parameters.py` & `psi4_step-2024.5.23/psi4_step/energy_parameters.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/energy_step.py` & `psi4_step-2024.5.23/psi4_step/energy_step.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/initialization.py` & `psi4_step-2024.5.23/psi4_step/initialization.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/initialization_parameters.py` & `psi4_step-2024.5.23/psi4_step/initialization_parameters.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/initialization_step.py` & `psi4_step-2024.5.23/psi4_step/initialization_step.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/optimization.py` & `psi4_step-2024.5.23/psi4_step/optimization.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/optimization_parameters.py` & `psi4_step-2024.5.23/psi4_step/optimization_parameters.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/optimization_step.py` & `psi4_step-2024.5.23/psi4_step/optimization_step.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/optimizer.py` & `psi4_step-2024.5.23/psi4_step/optimizer.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/psi4.py` & `psi4_step-2024.5.23/psi4_step/psi4.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/psi4_metadata.py` & `psi4_step-2024.5.23/psi4_step/psi4_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1620,14 +1620,27 @@
 type : str
     The type of the data: string, integer, or float.
 
 units : str
     Optional units for the result. If present, the value should be in these units.
 """
 metadata["results"] = {
+    "energy": {
+        "description": "The total energy",
+        "dimensionality": "scalar",
+        "property": "total energy#Psi4#{model}",
+        "type": "float",
+        "units": "kJ/mol",
+    },
+    "gradients": {
+        "description": "The gradients",
+        "dimensionality": "[3, n_atoms]",
+        "type": "float",
+        "units": "kJ/mol/Å",
+    },
     "(T) CORRECTION ENERGY": {
         "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd(t)"],
         "type": "float",
         "units": "",
@@ -1812,15 +1825,14 @@
         "units": "D",
     },
     "CURRENT ENERGY": {
         "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "the electronic energy from the current method",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
-        "property": "total energy#Psi4#{model}",
         "type": "float",
         "units": "E_h",
     },
     "CURRENT GRADIENT": {
         "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "the gradient of the energy for the current method",
         "dimensionality": [3, "n_atoms"],
```

### Comparing `psi4_step-2024.3.4/psi4_step/psi4_parameters.py` & `psi4_step-2024.5.23/psi4_step/psi4_parameters.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/psi4_step.py` & `psi4_step-2024.5.23/psi4_step/psi4_step.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/thermochemistry.py` & `psi4_step-2024.5.23/psi4_step/thermochemistry.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/thermochemistry_parameters.py` & `psi4_step-2024.5.23/psi4_step/thermochemistry_parameters.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/thermochemistry_step.py` & `psi4_step-2024.5.23/psi4_step/thermochemistry_step.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/tk_accelerated_optimization.py` & `psi4_step-2024.5.23/psi4_step/tk_accelerated_optimization.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/tk_energy.py` & `psi4_step-2024.5.23/psi4_step/tk_energy.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/tk_initialization.py` & `psi4_step-2024.5.23/psi4_step/tk_initialization.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/tk_optimization.py` & `psi4_step-2024.5.23/psi4_step/tk_optimization.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/tk_psi4.py` & `psi4_step-2024.5.23/psi4_step/tk_psi4.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step/tk_thermochemistry.py` & `psi4_step-2024.5.23/psi4_step/tk_thermochemistry.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step.egg-info/PKG-INFO` & `psi4_step-2024.5.23/psi4_step.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psi4_step
-Version: 2024.3.4
+Version: 2024.5.23
 Summary: A SEAMM plug-in to setup, run and analyze quantum chemistry calculations using Psi4
 Home-page: https://github.com/molssi-seamm/psi4_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,Psi4,DFT,quantum chemistry,CCSD
 Platform: Linux
@@ -96,14 +96,22 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2024.5.23 -- Added standard energy and gradients to results
+   * Added 'energy' and 'gradients' to optional results to support e.g. Energy Scan
+   * Fixed crashing bug in description of the Energy substep.
+     
+2024.3.17 -- Updated the installer
+   * Updated the installer to use the new version of the SEAMM installer.
+   * Finalizes installing either with Conda or Docker
+     
 2024.3.4 -- Allowing short names for method and DFT functionals
    * Added short names for the methods (Hamiltonians)  and DFT functionals.
    * Catch errors in Psi4 calculating properties for e.g. CISD(T) method
 
 2024.2.29 -- Completed support for containers
    * Fixed issues with running amd64 containers on arm64 systems.
```

### Comparing `psi4_step-2024.3.4/psi4_step.egg-info/SOURCES.txt` & `psi4_step-2024.5.23/psi4_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/psi4_step.egg-info/entry_points.txt` & `psi4_step-2024.5.23/psi4_step.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/setup.py` & `psi4_step-2024.5.23/setup.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/tests/test_psi4_step.py` & `psi4_step-2024.5.23/tests/test_psi4_step.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.3.4/versioneer.py` & `psi4_step-2024.5.23/versioneer.py`

 * *Files identical despite different names*

