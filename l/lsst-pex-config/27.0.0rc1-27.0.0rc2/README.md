# Comparing `tmp/lsst_pex_config-27.0.0rc1.tar.gz` & `tmp/lsst_pex_config-27.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst_pex_config-27.0.0rc1.tar", last modified: Wed May  1 21:15:37 2024, max compression
+gzip compressed data, was "lsst_pex_config-27.0.0rc2.tar", last modified: Thu May 23 01:51:18 2024, max compression
```

## Comparing `lsst_pex_config-27.0.0rc1.tar` & `lsst_pex_config-27.0.0rc2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:15:37.079249 lsst_pex_config-27.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-01 21:15:37.079249 lsst_pex_config-27.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/bsd_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:15:37.067249 lsst_pex_config-27.0.0rc1/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:15:37.071249 lsst_pex_config-27.0.0rc1/doc/lsst.pex.config/
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/doc/lsst.pex.config/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/doc/lsst.pex.config/design-notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/doc/lsst.pex.config/field-types.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/doc/lsst.pex.config/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/doc/lsst.pex.config/inspecting-configs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/doc/lsst.pex.config/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/doc/lsst.pex.config/registry-intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/doc/lsst.pex.config/wrapping-cpp-control-objects.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:15:37.067249 lsst_pex_config-27.0.0rc1/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:15:37.071249 lsst_pex_config-27.0.0rc1/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:15:37.071249 lsst_pex_config-27.0.0rc1/python/lsst/pex/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:15:37.075249 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/_doNotImportMe.py
--rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/callStack.py
--rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/choiceField.py
--rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)    61518 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    23842 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/configChoiceField.py
--rw-r--r--   0 runner    (1001) docker     (127)    11391 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/configDictField.py
--rw-r--r--   0 runner    (1001) docker     (127)    11533 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/configField.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:15:37.075249 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/configurableActions/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/configurableActions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/configurableActions/_configurableAction.py
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/configurableActions/_configurableActionField.py
--rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/configurableActions/_configurableActionStructField.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/configurableActions/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    18239 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/configurableField.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/dictField.py
--rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/history.py
--rw-r--r--   0 runner    (1001) docker     (127)    18381 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/listField.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/rangeField.py
--rw-r--r--   0 runner    (1001) docker     (127)    15871 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 21:15:36.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/python/lsst/pex/config/wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:15:37.079249 lsst_pex_config-27.0.0rc1/python/lsst_pex_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-01 21:15:37.000000 lsst_pex_config-27.0.0rc1/python/lsst_pex_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-01 21:15:37.000000 lsst_pex_config-27.0.0rc1/python/lsst_pex_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:15:37.000000 lsst_pex_config-27.0.0rc1/python/lsst_pex_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-01 21:15:37.000000 lsst_pex_config-27.0.0rc1/python/lsst_pex_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 21:15:37.000000 lsst_pex_config-27.0.0rc1/python/lsst_pex_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:15:36.000000 lsst_pex_config-27.0.0rc1/python/lsst_pex_config.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-01 21:15:37.079249 lsst_pex_config-27.0.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:15:37.079249 lsst_pex_config-27.0.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/tests/testLib.py
--rw-r--r--   0 runner    (1001) docker     (127)    22205 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/tests/test__file__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/tests/test_configChoiceField.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/tests/test_configDictField.py
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/tests/test_configurableActions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/tests/test_configurableField.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/tests/test_dictField.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/tests/test_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/tests/test_listField.py
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/tests/test_ticket1911.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/tests/test_ticket1914.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/tests/test_ticket1915.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/tests/test_ticket1929.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/tests/test_ticket1995.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/tests/test_ticket2818.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/tests/test_ticketDM-7337.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/tests/test_unloaded_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-01 21:15:28.000000 lsst_pex_config-27.0.0rc1/tests/test_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:18.605458 lsst_pex_config-27.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-23 01:51:18.605458 lsst_pex_config-27.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/bsd_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:18.593458 lsst_pex_config-27.0.0rc2/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:18.597458 lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/design-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/field-types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/inspecting-configs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/registry-intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/wrapping-cpp-control-objects.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:18.593458 lsst_pex_config-27.0.0rc2/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:18.597458 lsst_pex_config-27.0.0rc2/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:18.597458 lsst_pex_config-27.0.0rc2/python/lsst/pex/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:18.597458 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/_doNotImportMe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/callStack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/choiceField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61518 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23842 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configChoiceField.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11391 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configDictField.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11533 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configField.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:18.601457 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableActions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableActions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableActions/_configurableAction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableActions/_configurableActionField.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableActions/_configurableActionStructField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableActions/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18239 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/dictField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18381 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/listField.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/rangeField.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15871 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 01:51:18.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:18.605458 lsst_pex_config-27.0.0rc2/python/lsst_pex_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-23 01:51:18.000000 lsst_pex_config-27.0.0rc2/python/lsst_pex_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-23 01:51:18.000000 lsst_pex_config-27.0.0rc2/python/lsst_pex_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:51:18.000000 lsst_pex_config-27.0.0rc2/python/lsst_pex_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-23 01:51:18.000000 lsst_pex_config-27.0.0rc2/python/lsst_pex_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 01:51:18.000000 lsst_pex_config-27.0.0rc2/python/lsst_pex_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:51:17.000000 lsst_pex_config-27.0.0rc2/python/lsst_pex_config.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-23 01:51:18.605458 lsst_pex_config-27.0.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:18.605458 lsst_pex_config-27.0.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/testLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22205 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test__file__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_configChoiceField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_configDictField.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_configurableActions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_configurableField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_dictField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_listField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_ticket1911.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_ticket1914.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_ticket1915.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_ticket1929.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_ticket1995.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_ticket2818.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_ticketDM-7337.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_unloaded_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_wrap.py
```

### Comparing `lsst_pex_config-27.0.0rc1/PKG-INFO` & `lsst_pex_config-27.0.0rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-pex-config
-Version: 27.0.0rc1
+Version: 27.0.0rc2
 Summary: A flexible configuration system using Python files.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License, GPLv3+
 Project-URL: Homepage, https://github.com/lsst/pex_config
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_pex_config-27.0.0rc1/README.rst` & `lsst_pex_config-27.0.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/bsd_license.txt` & `lsst_pex_config-27.0.0rc2/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/doc/lsst.pex.config/CHANGES.rst` & `lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/doc/lsst.pex.config/design-notes.rst` & `lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/design-notes.rst`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/doc/lsst.pex.config/field-types.rst` & `lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/field-types.rst`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/doc/lsst.pex.config/index.rst` & `lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/index.rst`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/doc/lsst.pex.config/inspecting-configs.rst` & `lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/inspecting-configs.rst`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/doc/lsst.pex.config/overview.rst` & `lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/overview.rst`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/doc/lsst.pex.config/registry-intro.rst` & `lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/registry-intro.rst`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/doc/lsst.pex.config/wrapping-cpp-control-objects.rst` & `lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/wrapping-cpp-control-objects.rst`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/gpl-v3.0.txt` & `lsst_pex_config-27.0.0rc2/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/pyproject.toml` & `lsst_pex_config-27.0.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst/pex/config/__init__.py` & `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst/pex/config/callStack.py` & `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/callStack.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst/pex/config/choiceField.py` & `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/choiceField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst/pex/config/comparison.py` & `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/comparison.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst/pex/config/config.py` & `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/config.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst/pex/config/configChoiceField.py` & `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configChoiceField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst/pex/config/configDictField.py` & `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configDictField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst/pex/config/configField.py` & `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst/pex/config/configurableActions/__init__.py` & `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableActions/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst/pex/config/configurableActions/_configurableAction.py` & `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableActions/_configurableAction.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst/pex/config/configurableActions/_configurableActionField.py` & `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableActions/_configurableActionField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst/pex/config/configurableActions/_configurableActionStructField.py` & `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableActions/_configurableActionStructField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst/pex/config/configurableActions/tests.py` & `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableActions/tests.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst/pex/config/configurableField.py` & `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst/pex/config/convert.py` & `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/convert.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst/pex/config/dictField.py` & `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/dictField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst/pex/config/history.py` & `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/history.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst/pex/config/listField.py` & `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/listField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst/pex/config/rangeField.py` & `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/rangeField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst/pex/config/registry.py` & `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/registry.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst/pex/config/wrap.py` & `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/wrap.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst_pex_config.egg-info/PKG-INFO` & `lsst_pex_config-27.0.0rc2/python/lsst_pex_config.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-pex-config
-Version: 27.0.0rc1
+Version: 27.0.0rc2
 Summary: A flexible configuration system using Python files.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License, GPLv3+
 Project-URL: Homepage, https://github.com/lsst/pex_config
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_pex_config-27.0.0rc1/python/lsst_pex_config.egg-info/SOURCES.txt` & `lsst_pex_config-27.0.0rc2/python/lsst_pex_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/tests/testLib.py` & `lsst_pex_config-27.0.0rc2/tests/testLib.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/tests/test_Config.py` & `lsst_pex_config-27.0.0rc2/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/tests/test__file__.py` & `lsst_pex_config-27.0.0rc2/tests/test__file__.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/tests/test_configChoiceField.py` & `lsst_pex_config-27.0.0rc2/tests/test_configChoiceField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/tests/test_configDictField.py` & `lsst_pex_config-27.0.0rc2/tests/test_configDictField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/tests/test_configurableActions.py` & `lsst_pex_config-27.0.0rc2/tests/test_configurableActions.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/tests/test_configurableField.py` & `lsst_pex_config-27.0.0rc2/tests/test_configurableField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/tests/test_dictField.py` & `lsst_pex_config-27.0.0rc2/tests/test_dictField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/tests/test_history.py` & `lsst_pex_config-27.0.0rc2/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/tests/test_listField.py` & `lsst_pex_config-27.0.0rc2/tests/test_listField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/tests/test_registry.py` & `lsst_pex_config-27.0.0rc2/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/tests/test_ticket1911.py` & `lsst_pex_config-27.0.0rc2/tests/test_ticket1911.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/tests/test_ticket1914.py` & `lsst_pex_config-27.0.0rc2/tests/test_ticket1914.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/tests/test_ticket1915.py` & `lsst_pex_config-27.0.0rc2/tests/test_ticket1915.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/tests/test_ticket1929.py` & `lsst_pex_config-27.0.0rc2/tests/test_ticket1929.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/tests/test_ticket1995.py` & `lsst_pex_config-27.0.0rc2/tests/test_ticket1995.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/tests/test_ticket2818.py` & `lsst_pex_config-27.0.0rc2/tests/test_ticket2818.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/tests/test_ticketDM-7337.py` & `lsst_pex_config-27.0.0rc2/tests/test_ticketDM-7337.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/tests/test_unloaded_yaml.py` & `lsst_pex_config-27.0.0rc2/tests/test_unloaded_yaml.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc1/tests/test_wrap.py` & `lsst_pex_config-27.0.0rc2/tests/test_wrap.py`

 * *Files identical despite different names*

