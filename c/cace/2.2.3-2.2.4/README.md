# Comparing `tmp/cace-2.2.3.tar.gz` & `tmp/cace-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cace-2.2.3.tar", last modified: Fri Apr 26 06:58:56 2024, max compression
+gzip compressed data, was "cace-2.2.4.tar", last modified: Thu May 23 10:10:14 2024, max compression
```

## Comparing `cace-2.2.3.tar` & `cace-2.2.4.tar`

### file list

```diff
@@ -1,91 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.038775 cace-2.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.022775 cace-2.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.026775 cace-2.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-26 06:58:35.000000 cace-2.2.3/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-26 06:58:35.000000 cace-2.2.3/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-26 06:58:35.000000 cace-2.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-26 06:58:35.000000 cace-2.2.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-26 06:58:35.000000 cace-2.2.3/Changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-26 06:58:35.000000 cace-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-26 06:58:35.000000 cace-2.2.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-26 06:58:56.038775 cace-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-04-26 06:58:35.000000 cace-2.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.026775 cace-2.2.3/cace/
--rwxr-xr-x   0 runner    (1001) docker     (127)      623 2024-04-26 06:58:35.000000 cace-2.2.3/cace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-26 06:58:35.000000 cace-2.2.3/cace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-26 06:58:35.000000 cace-2.2.3/cace/__version__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5906 2024-04-26 06:58:35.000000 cace-2.2.3/cace/cace_cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    44151 2024-04-26 06:58:35.000000 cace-2.2.3/cace/cace_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.034775 cace-2.2.3/cace/common/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19058 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_calculate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23616 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_collate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12819 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26024 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_evaluate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    70978 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_gensim.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14672 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_launch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20756 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_makeplot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12523 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_measure.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10797 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_read.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    46512 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_regenerate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8733 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_simulate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_unused.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    55674 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/cace_write.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7321 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/electrical_parameter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13039 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/layout_estimate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12310 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/netlist_precheck.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2540 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/physical_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/safe_eval.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14709 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/simulation_job.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22242 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/simulation_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8949 2024-04-26 06:58:35.000000 cace-2.2.3/cace/common/spiceunits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.034775 cace-2.2.3/cace/gui/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1922 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/consoletext.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29517 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/editparam.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26903 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/failreport.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3780 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/helpwindow.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24388 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/rowwidget.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7191 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16180 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/simhints.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4221 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/textreport.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2450 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/tksimpledialog.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-04-26 06:58:35.000000 cace-2.2.3/cace/gui/tooltip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.038775 cace-2.2.3/cace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-26 06:58:55.000000 cace-2.2.3/cace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-26 06:58:56.000000 cace-2.2.3/cace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 06:58:55.000000 cace-2.2.3/cace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-26 06:58:55.000000 cace-2.2.3/cace.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 06:58:55.000000 cace-2.2.3/cace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 06:58:55.000000 cace-2.2.3/cace.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.034775 cace-2.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-26 06:58:35.000000 cace-2.2.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-26 06:58:35.000000 cace-2.2.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.034775 cace-2.2.3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.034775 cace-2.2.3/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   183493 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/_static/cace_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/characterization.md
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.038775 cace-2.2.3/docs/source/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/dev/codebase.md
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/dev/coding_style.md
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/dev/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.038775 cace-2.2.3/docs/source/formats/
--rw-r--r--   0 runner    (1001) docker     (127)    22593 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/formats/format_description.md
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/formats/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/formats/schematic_description.md
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.038775 cace-2.2.3/docs/source/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/usage/cace_cli.md
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/usage/cace_gui.md
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/usage/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-26 06:58:35.000000 cace-2.2.3/docs/source/usage/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-26 06:58:35.000000 cace-2.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 06:58:35.000000 cace-2.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-26 06:58:35.000000 cace-2.2.3/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-26 06:58:35.000000 cace-2.2.3/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 06:58:56.038775 cace-2.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:58:56.038775 cace-2.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-26 06:58:35.000000 cace-2.2.3/tests/context.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 06:58:35.000000 cace-2.2.3/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.526706 cace-2.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.506706 cace-2.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.506706 cace-2.2.4/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.510706 cace-2.2.4/.github/actions/build_nix/
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-23 10:09:51.000000 cace-2.2.4/.github/actions/build_nix/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.510706 cace-2.2.4/.github/actions/check_space/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-23 10:09:51.000000 cace-2.2.4/.github/actions/check_space/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.514706 cace-2.2.4/.github/actions/setup_env/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-23 10:09:51.000000 cace-2.2.4/.github/actions/setup_env/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.514706 cace-2.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-23 10:09:51.000000 cace-2.2.4/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10011 2024-05-23 10:09:51.000000 cace-2.2.4/.github/workflows/ci_nix.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-23 10:09:51.000000 cace-2.2.4/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-23 10:09:51.000000 cace-2.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-23 10:09:51.000000 cace-2.2.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-23 10:09:51.000000 cace-2.2.4/Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-23 10:09:51.000000 cace-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-23 10:09:51.000000 cace-2.2.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-23 10:10:14.526706 cace-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-23 10:09:51.000000 cace-2.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.514706 cace-2.2.4/cace/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      623 2024-05-23 10:09:51.000000 cace-2.2.4/cace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-23 10:09:51.000000 cace-2.2.4/cace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-23 10:09:51.000000 cace-2.2.4/cace/__version__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6297 2024-05-23 10:09:51.000000 cace-2.2.4/cace/cace_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44151 2024-05-23 10:09:51.000000 cace-2.2.4/cace/cace_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.518706 cace-2.2.4/cace/common/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19058 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_calculate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23616 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_collate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12819 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26024 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_evaluate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    70978 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_gensim.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14672 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_launch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20756 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_makeplot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12523 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_measure.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10797 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_read.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46512 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_regenerate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8733 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_simulate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_unused.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    65589 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_write.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7321 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/electrical_parameter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13039 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/layout_estimate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12310 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/netlist_precheck.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2540 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/physical_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/safe_eval.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14709 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/simulation_job.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22283 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/simulation_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8949 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/spiceunits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.522706 cace-2.2.4/cace/gui/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1922 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/consoletext.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29517 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/editparam.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26903 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/failreport.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3780 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/helpwindow.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24388 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/rowwidget.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7191 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16180 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/simhints.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4221 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/textreport.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2450 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/tksimpledialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-23 10:09:51.000000 cace-2.2.4/cace/open_pdks_rev
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.526706 cace-2.2.4/cace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-23 10:10:14.000000 cace-2.2.4/cace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-23 10:10:14.000000 cace-2.2.4/cace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:10:14.000000 cace-2.2.4/cace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-23 10:10:14.000000 cace-2.2.4/cace.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-23 10:10:14.000000 cace-2.2.4/cace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 10:10:14.000000 cace-2.2.4/cace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-23 10:09:51.000000 cace-2.2.4/default.nix
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.522706 cace-2.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-23 10:09:51.000000 cace-2.2.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-23 10:09:51.000000 cace-2.2.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.522706 cace-2.2.4/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.522706 cace-2.2.4/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   183493 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/_static/cace_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/characterization.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.522706 cace-2.2.4/docs/source/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/dev/codebase.md
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/dev/coding_style.md
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/dev/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.526706 cace-2.2.4/docs/source/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)    22593 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/formats/format_description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/formats/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/formats/schematic_description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.526706 cace-2.2.4/docs/source/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/usage/cace_cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/usage/cace_gui.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/usage/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/usage/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-23 10:09:51.000000 cace-2.2.4/flake.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-23 10:09:51.000000 cace-2.2.4/flake.nix
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.526706 cace-2.2.4/nix/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 10:09:51.000000 cace-2.2.4/nix/colab-env.nix
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-23 10:09:51.000000 cace-2.2.4/nix/create-shell.nix
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-23 10:09:51.000000 cace-2.2.4/nix/docker.nix
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-23 10:09:51.000000 cace-2.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-23 10:09:51.000000 cace-2.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-23 10:09:51.000000 cace-2.2.4/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-23 10:09:51.000000 cace-2.2.4/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 10:10:14.526706 cace-2.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-23 10:09:51.000000 cace-2.2.4/shell.nix
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.526706 cace-2.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-23 10:09:51.000000 cace-2.2.4/tests/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-23 10:09:51.000000 cace-2.2.4/tests/test1.py
```

### Comparing `cace-2.2.3/.github/workflows/ci.yaml` & `cace-2.2.4/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/.github/workflows/pypi.yaml` & `cace-2.2.4/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/.readthedocs.yaml` & `cace-2.2.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/Changelog.md` & `cace-2.2.4/Changelog.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+# 2.2.4
+
+## Common
+
+- Add `markdown_summary`
+
+## CLI
+
+- Call `markdown_summary` at the end and print to stdout
+- Change `--summary` argument to print to file
+
 # 2.2.3
 
 ## Common
 
 - Improve scheduling of parameters
   - Simpler and more reliable
 - Queued parameters can now be canceled
```

### Comparing `cace-2.2.3/LICENSE` & `cace-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/Makefile` & `cace-2.2.4/Makefile`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/PKG-INFO` & `cace-2.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: cace
-Version: 2.2.3
+Version: 2.2.4
 Summary: Circuit Automatic Characterization Engine
 Author-email: Tim Edwards <tim@efabless.com>, Leo Moser <leo.moser@efabless.com>
 Project-URL: Homepage, https://github.com/efabless/cace
 Project-URL: Issues, https://github.com/efabless/cace/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.6.0
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: pillow>=10.1.0
+Requires-Dist: volare>=0.16.0
 
 <h1 align="center">CACE</h1>
 <h2 align="center">Circuit Automatic Characterization Engine</h2>
 <p align="center">
     <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg" alt="License: Apache 2.0"/></a>
     <img src="https://github.com/efabless/cace/actions/workflows/ci.yaml/badge.svg?branch=main" alt="GitHub Actions Status Badge" />
     <a href="https://cace.readthedocs.io/"><img src="https://readthedocs.org/projects/cace/badge/?version=latest" alt="Documentation Build Status Badge"/></a>
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: cace Version: 2.2.3 Summary: Circuit Automatic
+Metadata-Version: 2.1 Name: cace Version: 2.2.4 Summary: Circuit Automatic
 Characterization Engine Author-email: Tim Edwards
 efabless.com>, Leo Moser
 efabless.com> Project-URL: Homepage, https://github.com/efabless/cace Project-
 URL: Issues, https://github.com/efabless/cace/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 matplotlib>=3.6.0 Requires-Dist: numpy>=1.20.0 Requires-Dist: pillow>=10.1.0
+Requires-Dist: volare>=0.16.0
                               ************ CCAACCEE ************
              ********** CCiirrccuuiitt AAuuttoommaattiicc CChhaarraacctteerriizzaattiioonn EEnnggiinnee **********
  _[_L_i_c_e_n_s_e_:_ _A_p_a_c_h_e_ _2_._0_][GitHub Actions Status Badge]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _B_u_i_l_d_ _S_t_a_t_u_s
                 _B_a_d_g_e_]_[_P_y_t_h_o_n_ _3_._8_ _o_r_ _h_i_g_h_e_r_]_[_C_o_d_e_ _S_t_y_l_e_:_ _b_l_u_e_]
                    _[_I_n_v_i_t_e_ _t_o_ _t_h_e_ _O_p_e_n_ _S_o_u_r_c_e_ _S_i_l_i_c_o_n_ _S_l_a_c_k_]
 CACE is a set of python scripts that take an input file in the CACE 4.0 format
 and uses the information found there in combination with CACE-compatible
```

### Comparing `cace-2.2.3/README.md` & `cace-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/__init__.py` & `cace-2.2.4/cace/__init__.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/__main__.py` & `cace-2.2.4/cace/__main__.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/__version__.py` & `cace-2.2.4/cace/__version__.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = '2.2.3'
+__version__ = '2.2.4'
 
 if __name__ == '__main__':
     print(__version__, end='')
```

### Comparing `cace-2.2.3/cace/cace_cli.py` & `cace-2.2.4/cace/cace_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -106,16 +106,15 @@
         '--no-simulation',
         action='store_true',
         help="""does not re-run simulations if the output file exists.
     (Warning: Does not check if simulations are out of date)""",
     )
     parser.add_argument(
         '--summary',
-        action='store_true',
-        help='prints a summary of results at the end',
+        help='output path for the summary e.g. final/summary.md',
     )
 
     # Parse arguments
     args = parser.parse_args()
 
     # Create the SimulationManager
     simulation_manager = SimulationManager()
@@ -148,15 +147,15 @@
 
     # Queue specified parameters
     if args.parameter:
         if args.debug:
             print(f'Running simulation for: {args.parameter}')
 
         for pname in args.parameter:
-            simulation_manager.queue_simulation(pname)
+            simulation_manager.queue_parameter(pname)
     # Queue all parameters
     else:
         pnames = simulation_manager.get_all_pnames()
 
         if args.debug:
             print(f'Running simulation for: {pnames}')
 
@@ -171,16 +170,27 @@
 
     if args.debug:
         print('Done with CACE simulations and evaluations.')
 
     if args.outfile:
         simulation_manager.save_datasheet(args.outfile)
 
+    # Print the summary to stdout
+    simulation_manager.summarize_datasheet()
+
+    # Print the summary to a file
     if args.summary:
-        print('')
-        print('CACE Summary of results:')
-        print('------------------------')
-        simulation_manager.summarize_datasheet(args.parameter)
+        dirname = os.path.dirname(args.summary) or os.getcwd()
+        filename = os.path.basename(args.summary)
+
+        # Check whether path to file exists
+        if os.path.isdir(dirname):
+            with open(os.path.join(dirname, filename), 'w') as ofile:
+                simulation_manager.summarize_datasheet(ofile)
+        else:
+            print(
+                f"Couldn't write summary, invalid path: {os.path.dirname(args.summary)}"
+            )
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `cace-2.2.3/cace/cace_gui.py` & `cace-2.2.4/cace/cace_gui.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/common/cace_calculate.py` & `cace-2.2.4/cace/common/cace_calculate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/common/cace_collate.py` & `cace-2.2.4/cace/common/cace_collate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/common/cace_compat.py` & `cace-2.2.4/cace/common/cace_compat.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/common/cace_evaluate.py` & `cace-2.2.4/cace/common/cace_evaluate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/common/cace_gensim.py` & `cace-2.2.4/cace/common/cace_gensim.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/common/cace_launch.py` & `cace-2.2.4/cace/common/cace_launch.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/common/cace_makeplot.py` & `cace-2.2.4/cace/common/cace_makeplot.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/common/cace_measure.py` & `cace-2.2.4/cace/common/cace_measure.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/common/cace_read.py` & `cace-2.2.4/cace/common/cace_read.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/common/cace_regenerate.py` & `cace-2.2.4/cace/common/cace_regenerate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/common/cace_simulate.py` & `cace-2.2.4/cace/common/cace_simulate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/common/cace_unused.txt` & `cace-2.2.4/cace/common/cace_unused.txt`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/common/cace_write.py` & `cace-2.2.4/cace/common/cace_write.py`

 * *Files 10% similar despite different names*

```diff
@@ -876,14 +876,311 @@
             outline += resultlist[0] + ' (' + resultlist[1] + ')\n'
 
             sys.stdout.buffer.write(outline.encode('latin1'))
 
     print('')
 
 
+def markdown_summary(datasheet, file=None):
+    """
+    Print a brief summary to either stdout or any file that is passed.
+    The summary is formatted in Markdown and can be viewed with any
+    Markdown viewer
+    """
+
+    # Table spacings
+    sp = [20, 20, 10, 12, 10, 12, 10, 12, 8]
+
+    skip_msg = 'Skip 🟧'
+    fail_msg = 'Fail ❌'
+    pass_msg = 'Pass ✅'
+
+    print('\n# CACE Summary\n', file=file)
+
+    print(
+        f'**general**\n\n'
+        f'- name: {datasheet["name"]}\n'
+        f'- description: {datasheet["description"]}\n'
+        f'- commit: {datasheet["commit"]}\n'
+        f'- PDK: {datasheet["PDK"]}\n'
+        f'- cace_format: {datasheet["cace_format"]}\n',
+        file=file,
+    )
+
+    print(
+        f'**authorship**\n\n'
+        f'- designer: {datasheet["authorship"]["designer"]}\n'
+        f'- company: {datasheet["authorship"]["company"]}\n'
+        f'- creation_date: {datasheet["authorship"]["creation_date"]}\n'
+        f'- license: {datasheet["authorship"]["license"]}\n',
+        file=file,
+    )
+
+    print(
+        f'**netlist source**: {datasheet["runtime_options"]["netlist_source"]}\n',
+        file=file,
+    )
+
+    print('## Electrical Parameters\n', file=file)
+
+    # Print the table headings
+    print(
+        f'| {"Parameter": ^{sp[0]}} '
+        f'| {"Testbench": ^{sp[1]}} '
+        f'| {"Min Limit": ^{sp[2]}} '
+        f'| {"Min Value": ^{sp[3]}} '
+        f'| {"Typ Target": ^{sp[4]}} '
+        f'| {"Typ Value": ^{sp[5]}} '
+        f'| {"Max Limit": ^{sp[6]}} '
+        f'| {"Max Value": ^{sp[7]}} '
+        f'| {"Status": ^{sp[8]}} |',
+        file=file,
+    )
+    # Print the separators
+    print(
+        f'| :{"-"*(sp[0]-1)} '
+        f'| :{"-"*(sp[1]-1)} '
+        f'| {"-"*(sp[2]-1)}: '
+        f'| {"-"*(sp[3]-1)}: '
+        f'| {"-"*(sp[4]-1)}: '
+        f'| {"-"*(sp[5]-1)}: '
+        f'| {"-"*(sp[6]-1)}: '
+        f'| {"-"*(sp[7]-1)}: '
+        f'| :{"-"*(sp[8]-2)}: |',
+        file=file,
+    )
+
+    if 'electrical_parameters' in datasheet:
+        for eparam in datasheet['electrical_parameters']:
+
+            # Get the unit
+            unit = eparam['unit'] if 'unit' in eparam else None
+
+            limits = {'minimum': '', 'typical': '', 'maximum': ''}
+
+            # Get the limits from the spec
+            if 'spec' in eparam:
+                for spec_type in ['minimum', 'typical', 'maximum']:
+                    if spec_type in eparam['spec']:
+                        limits[spec_type] = eparam['spec'][spec_type]
+
+                        if isinstance(limits[spec_type], list):
+                            limits[spec_type] = limits[spec_type][0]
+
+            values = {'minimum': '', 'typical': '', 'maximum': ''}
+
+            # Get the results
+            passing = None
+            if 'results' in eparam:
+                passing = True
+
+                for result_type in ['minimum', 'typical', 'maximum']:
+                    if result_type in eparam['results']:
+                        values[result_type] = eparam['results'][result_type][0]
+
+                        # Any fail fails the whole parameter
+                        if eparam['results'][result_type][1] != 'pass':
+                            passing = False
+
+            # Get the status message
+            status = pass_msg if passing else fail_msg
+
+            if passing == None:
+                status = skip_msg
+
+            if 'status' in eparam and eparam['status'] == 'skip':
+                status = skip_msg
+
+            # Get the testbench
+            testbench = ''
+            if 'simulate' in eparam:
+                testbench = eparam['simulate']['template']
+
+            # Don't print any unit if empty or any
+            no_unit = ['', 'any']
+
+            # Print the row for the parameter
+            parameter_str = eparam['name']
+            testbench_str = testbench
+            min_limit_str = (
+                f'{limits["minimum"]} {unit}'
+                if unit and not limits['minimum'] in no_unit
+                else limits['minimum']
+            )
+            min_value_str = (
+                f'{values["minimum"]} {unit}'
+                if unit and not values['minimum'] in no_unit
+                else values['minimum']
+            )
+            typ_limit_str = (
+                f'{limits["typical"]} {unit}'
+                if unit and not limits['typical'] in no_unit
+                else limits['typical']
+            )
+            typ_value_str = (
+                f'{values["typical"]} {unit}'
+                if unit and not values['typical'] in no_unit
+                else values['typical']
+            )
+            max_limit_str = (
+                f'{limits["maximum"]} {unit}'
+                if unit and not limits['maximum'] in no_unit
+                else limits['maximum']
+            )
+            max_value_str = (
+                f'{values["maximum"]} {unit}'
+                if unit and not values['maximum'] in no_unit
+                else values['maximum']
+            )
+            status_str = status
+
+            print(
+                f'| {parameter_str: <{sp[0]}} '
+                f'| {testbench_str: <{sp[1]}} '
+                f'| {min_limit_str: >{sp[2]}} '
+                f'| {min_value_str: >{sp[3]}} '
+                f'| {typ_limit_str: >{sp[4]}} '
+                f'| {typ_value_str: >{sp[5]}} '
+                f'| {max_limit_str: >{sp[6]}} '
+                f'| {max_value_str: >{sp[7]}} '
+                f'| {status_str: ^{sp[8]-1}} |',
+                file=file,
+            )
+
+    print('\n## Physical Parameters\n', file=file)
+
+    # Print the table headings
+    print(
+        f'| {"Parameter": ^{sp[0]}} '
+        f'| {"Tool": ^{sp[1]}} '
+        f'| {"Min Limit": ^{sp[2]}} '
+        f'| {"Min Value": ^{sp[3]}} '
+        f'| {"Typ Target": ^{sp[4]}} '
+        f'| {"Typ Value": ^{sp[5]}} '
+        f'| {"Max Limit": ^{sp[6]}} '
+        f'| {"Max Value": ^{sp[7]}} '
+        f'| {"Status": ^{sp[8]}} |',
+        file=file,
+    )
+    # Print the separators
+    print(
+        f'| :{"-"*(sp[0]-1)} '
+        f'| :{"-"*(sp[1]-1)} '
+        f'| {"-"*(sp[2]-1)}: '
+        f'| {"-"*(sp[3]-1)}: '
+        f'| {"-"*(sp[4]-1)}: '
+        f'| {"-"*(sp[5]-1)}: '
+        f'| {"-"*(sp[6]-1)}: '
+        f'| {"-"*(sp[7]-1)}: '
+        f'| :{"-"*(sp[8]-2)}: |',
+        file=file,
+    )
+
+    if 'physical_parameters' in datasheet:
+        for pparam in datasheet['physical_parameters']:
+
+            # Get the unit
+            unit = pparam['unit'] if 'unit' in pparam else None
+
+            limits = {'minimum': '', 'typical': '', 'maximum': ''}
+
+            # Get the limits from the spec
+            if 'spec' in pparam:
+                for spec_type in ['minimum', 'typical', 'maximum']:
+                    if spec_type in pparam['spec']:
+                        limits[spec_type] = pparam['spec'][spec_type]
+
+                        if isinstance(limits[spec_type], list):
+                            limits[spec_type] = limits[spec_type][0]
+
+            values = {'minimum': '', 'typical': '', 'maximum': ''}
+
+            # Get the results
+            passing = None
+            if 'results' in pparam:
+                passing = True
+
+                for result_type in ['minimum', 'typical', 'maximum']:
+                    if result_type in pparam['results']:
+                        values[result_type] = pparam['results'][result_type][0]
+
+                        # Any fail fails the whole parameter
+                        if pparam['results'][result_type][1] != 'pass':
+                            passing = False
+
+            # Get the status message
+            status = pass_msg if passing else fail_msg
+
+            if passing == None:
+                status = skip_msg
+
+            if 'status' in pparam and pparam['status'] == 'skip':
+                status = skip_msg
+
+            # Get the tool
+            tool = ''
+            if 'evaluate' in pparam:
+                tool = pparam['evaluate']['tool']
+                if isinstance(tool, list):
+                    tool = tool[0]
+
+            # Don't print any unit if empty or any
+            no_unit = ['', 'any']
+
+            # Print the row for the parameter
+            parameter_str = pparam['name']
+            tool_str = tool
+            min_limit_str = (
+                f'{limits["minimum"]} {unit}'
+                if unit and not limits['minimum'] in no_unit
+                else limits['minimum']
+            )
+            min_value_str = (
+                f'{values["minimum"]} {unit}'
+                if unit and not values['minimum'] in no_unit
+                else values['minimum']
+            )
+            typ_limit_str = (
+                f'{limits["typical"]} {unit}'
+                if unit and not limits['typical'] in no_unit
+                else limits['typical']
+            )
+            typ_value_str = (
+                f'{values["typical"]} {unit}'
+                if unit and not values['typical'] in no_unit
+                else values['typical']
+            )
+            max_limit_str = (
+                f'{limits["maximum"]} {unit}'
+                if unit and not limits['maximum'] in no_unit
+                else limits['maximum']
+            )
+            max_value_str = (
+                f'{values["maximum"]} {unit}'
+                if unit and not values['maximum'] in no_unit
+                else values['maximum']
+            )
+            status_str = status
+
+            print(
+                f'| {parameter_str: <{sp[0]}} '
+                f'| {tool_str: <{sp[1]}} '
+                f'| {min_limit_str: >{sp[2]}} '
+                f'| {min_value_str: >{sp[3]}} '
+                f'| {typ_limit_str: >{sp[4]}} '
+                f'| {typ_value_str: >{sp[5]}} '
+                f'| {max_limit_str: >{sp[6]}} '
+                f'| {max_value_str: >{sp[7]}} '
+                f'| {status_str: ^{sp[8]-1}} |',
+                file=file,
+            )
+
+    print('', file=file)
+
+
 # ---------------------------------------------------------------
 # cace_summary
 #
 # Print a summary report of results from a datasheet
 #
 # "datasheet" is a CACE characterization dataset
 # "paramname" is a list of parameters to summarize,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cace-2.2.3/cace/common/electrical_parameter.py` & `cace-2.2.4/cace/common/electrical_parameter.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/common/layout_estimate.py` & `cace-2.2.4/cace/common/layout_estimate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/common/netlist_precheck.py` & `cace-2.2.4/cace/common/netlist_precheck.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/common/physical_parameter.py` & `cace-2.2.4/cace/common/physical_parameter.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/common/safe_eval.py` & `cace-2.2.4/cace/common/safe_eval.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/common/simulation_job.py` & `cace-2.2.4/cace/common/simulation_job.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/common/simulation_manager.py` & `cace-2.2.4/cace/common/simulation_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,20 @@
 import time
 import shutil
 import signal
 import threading
 
 from .cace_read import cace_read
 from .cace_compat import cace_compat
-from .cace_write import cace_write, cace_summary, cace_generate_html
+from .cace_write import (
+    cace_write,
+    cace_summary,
+    markdown_summary,
+    cace_generate_html,
+)
 from .physical_parameter import PhysicalParameter
 from .electrical_parameter import ElectricalParameter
 
 
 class SimulationManager:
     """
     The SimulationManager manages the simulation queue
@@ -204,16 +209,16 @@
         """Set a new datasheet"""
         self.datasheet = datasheet
 
     def get_datasheet(self):
         """Return the datasheet"""
         return self.datasheet
 
-    def summarize_datasheet(self, pnames=[]):
-        cace_summary(self.datasheet, pnames)
+    def summarize_datasheet(self, file=None):
+        markdown_summary(self.datasheet, file)
 
     def generate_html(self):
         debug = self.get_runtime_options('debug')
         cace_generate_html(self.datasheet, None, debug)
 
     def duplicate_parameter(self, pname):
         param = self.find_parameter(pname)
```

### Comparing `cace-2.2.3/cace/common/spiceunits.py` & `cace-2.2.4/cace/common/spiceunits.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/gui/consoletext.py` & `cace-2.2.4/cace/gui/consoletext.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/gui/editparam.py` & `cace-2.2.4/cace/gui/editparam.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/gui/failreport.py` & `cace-2.2.4/cace/gui/failreport.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/gui/helpwindow.py` & `cace-2.2.4/cace/gui/helpwindow.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/gui/rowwidget.py` & `cace-2.2.4/cace/gui/rowwidget.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/gui/settings.py` & `cace-2.2.4/cace/gui/settings.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/gui/simhints.py` & `cace-2.2.4/cace/gui/simhints.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/gui/style.py` & `cace-2.2.4/cace/gui/style.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/gui/textreport.py` & `cace-2.2.4/cace/gui/textreport.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/gui/tksimpledialog.py` & `cace-2.2.4/cace/gui/tksimpledialog.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace/gui/tooltip.py` & `cace-2.2.4/cace/gui/tooltip.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/cace.egg-info/PKG-INFO` & `cace-2.2.4/cace.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: cace
-Version: 2.2.3
+Version: 2.2.4
 Summary: Circuit Automatic Characterization Engine
 Author-email: Tim Edwards <tim@efabless.com>, Leo Moser <leo.moser@efabless.com>
 Project-URL: Homepage, https://github.com/efabless/cace
 Project-URL: Issues, https://github.com/efabless/cace/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.6.0
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: pillow>=10.1.0
+Requires-Dist: volare>=0.16.0
 
 <h1 align="center">CACE</h1>
 <h2 align="center">Circuit Automatic Characterization Engine</h2>
 <p align="center">
     <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg" alt="License: Apache 2.0"/></a>
     <img src="https://github.com/efabless/cace/actions/workflows/ci.yaml/badge.svg?branch=main" alt="GitHub Actions Status Badge" />
     <a href="https://cace.readthedocs.io/"><img src="https://readthedocs.org/projects/cace/badge/?version=latest" alt="Documentation Build Status Badge"/></a>
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: cace Version: 2.2.3 Summary: Circuit Automatic
+Metadata-Version: 2.1 Name: cace Version: 2.2.4 Summary: Circuit Automatic
 Characterization Engine Author-email: Tim Edwards
 efabless.com>, Leo Moser
 efabless.com> Project-URL: Homepage, https://github.com/efabless/cace Project-
 URL: Issues, https://github.com/efabless/cace/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 matplotlib>=3.6.0 Requires-Dist: numpy>=1.20.0 Requires-Dist: pillow>=10.1.0
+Requires-Dist: volare>=0.16.0
                               ************ CCAACCEE ************
              ********** CCiirrccuuiitt AAuuttoommaattiicc CChhaarraacctteerriizzaattiioonn EEnnggiinnee **********
  _[_L_i_c_e_n_s_e_:_ _A_p_a_c_h_e_ _2_._0_][GitHub Actions Status Badge]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _B_u_i_l_d_ _S_t_a_t_u_s
                 _B_a_d_g_e_]_[_P_y_t_h_o_n_ _3_._8_ _o_r_ _h_i_g_h_e_r_]_[_C_o_d_e_ _S_t_y_l_e_:_ _b_l_u_e_]
                    _[_I_n_v_i_t_e_ _t_o_ _t_h_e_ _O_p_e_n_ _S_o_u_r_c_e_ _S_i_l_i_c_o_n_ _S_l_a_c_k_]
 CACE is a set of python scripts that take an input file in the CACE 4.0 format
 and uses the information found there in combination with CACE-compatible
```

### Comparing `cace-2.2.3/cace.egg-info/SOURCES.txt` & `cace-2.2.4/cace.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 .gitignore
 .readthedocs.yaml
 Changelog.md
 LICENSE
 Makefile
 README.md
+default.nix
+flake.lock
+flake.nix
 pyproject.toml
 requirements.txt
 requirements_dev.txt
 requirements_docs.txt
+shell.nix
+.github/actions/build_nix/action.yml
+.github/actions/check_space/action.yml
+.github/actions/setup_env/action.yml
 .github/workflows/ci.yaml
+.github/workflows/ci_nix.yml
 .github/workflows/pypi.yaml
 cace/__init__.py
 cace/__main__.py
 cace/__version__.py
 cace/cace_cli.py
 cace/cace_gui.py
+cace/open_pdks_rev
 cace.egg-info/PKG-INFO
 cace.egg-info/SOURCES.txt
 cace.egg-info/dependency_links.txt
 cace.egg-info/entry_points.txt
 cace.egg-info/requires.txt
 cace.egg-info/top_level.txt
 cace/common/__init__.py
@@ -67,9 +76,12 @@
 docs/source/formats/format_description.md
 docs/source/formats/index.md
 docs/source/formats/schematic_description.md
 docs/source/usage/cace_cli.md
 docs/source/usage/cace_gui.md
 docs/source/usage/getting_started.md
 docs/source/usage/index.md
+nix/colab-env.nix
+nix/create-shell.nix
+nix/docker.nix
 tests/context.py
 tests/test1.py
```

### Comparing `cace-2.2.3/docs/Makefile` & `cace-2.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/docs/make.bat` & `cace-2.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/docs/source/_static/cace_screenshot.png` & `cace-2.2.4/docs/source/_static/cace_screenshot.png`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/docs/source/characterization.md` & `cace-2.2.4/docs/source/characterization.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/docs/source/conf.py` & `cace-2.2.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/docs/source/formats/format_description.md` & `cace-2.2.4/docs/source/formats/format_description.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/docs/source/formats/schematic_description.md` & `cace-2.2.4/docs/source/formats/schematic_description.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/docs/source/index.md` & `cace-2.2.4/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/docs/source/usage/cace_cli.md` & `cace-2.2.4/docs/source/usage/cace_cli.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/docs/source/usage/cace_gui.md` & `cace-2.2.4/docs/source/usage/cace_gui.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/docs/source/usage/getting_started.md` & `cace-2.2.4/docs/source/usage/getting_started.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.3/pyproject.toml` & `cace-2.2.4/pyproject.toml`

 * *Files identical despite different names*

