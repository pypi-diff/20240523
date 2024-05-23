# Comparing `tmp/lsst_daf_butler-27.2024.1900.tar.gz` & `tmp/lsst_daf_butler-27.2024.2000.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst_daf_butler-27.2024.1900.tar", last modified: Thu May  9 10:01:22 2024, max compression
+gzip compressed data, was "lsst_daf_butler-27.2024.2000.tar", last modified: Thu May 16 09:49:27 2024, max compression
```

## Comparing `lsst_daf_butler-27.2024.1900.tar` & `lsst_daf_butler-27.2024.2000.tar`

### file list

```diff
@@ -1,458 +1,458 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.261464 lsst_daf_butler-27.2024.1900/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-09 10:01:22.261464 lsst_daf_butler-27.2024.1900/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/bsd_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.189464 lsst_daf_butler-27.2024.1900/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.197465 lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/
--rw-r--r--   0 runner    (1001) docker     (127)    54247 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/concreteStorageClasses.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/configuring.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/datastores.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10776 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/dimensions.rst
--rw-r--r--   0 runner    (1001) docker     (127)    22653 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/formatters.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/organizing.rst
--rw-r--r--   0 runner    (1001) docker     (127)    23195 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/queries.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/use-in-tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/writing-subcommands.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.193464 lsst_daf_butler-27.2024.1900/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.197465 lsst_daf_butler-27.2024.1900/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.197465 lsst_daf_butler-27.2024.1900/python/lsst/daf/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.205464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    75170 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_butler_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     9619 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_butler_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_butler_instance_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_butler_repo_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_column_categorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_column_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_column_type_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    52100 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14135 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_config_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_dataset_association.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_dataset_existence.py
--rw-r--r--   0 runner    (1001) docker     (127)    32133 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_dataset_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)    30028 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_deferredDatasetHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_exceptions_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_file_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_file_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)    30151 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_labeled_butler_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15147 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_limited_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10451 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_location.py
--rw-r--r--   0 runner    (1001) docker     (127)    19541 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_named.py
--rw-r--r--   0 runner    (1001) docker     (127)    25574 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_quantum.py
--rw-r--r--   0 runner    (1001) docker     (127)    32289 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_quantum_backed.py
--rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_registry_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)    37492 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_storage_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    14504 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_storage_class_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)    23377 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_timespan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.205464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_utilities/locked_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_utilities/named_locks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_utilities/thread_safe_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    16594 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/arrow_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.205464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14768 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/butler.py
--rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/cliLog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.205464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/cmd/_remove_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/cmd/_remove_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/cmd/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.205464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/opt/
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/opt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/opt/optionGroups.py
--rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/opt/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)    44081 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/column_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.209464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/datastore.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.209464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/datastores/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/datastores/composites.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/datastores/fileDatastore.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/datastores/formatters.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/datastores/writeRecipes.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15382 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/dimensions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.209464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/old_dimensions/
--rw-r--r--   0 runner    (1001) docker     (127)    13246 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13341 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15416 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15416 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15488 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe4.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15088 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe5.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15094 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15382 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe7.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/registry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/repo_transfer_formats.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/storageClasses.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.209464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastore/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    57480 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastore/_datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    41721 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastore/cache_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastore/composites.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastore/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    34999 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastore/file_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastore/generic_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastore/record_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    13279 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastore/stored_file_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.213464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastores/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49806 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastores/chainedDatastore.py
--rw-r--r--   0 runner    (1001) docker     (127)   120549 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastores/fileDatastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastores/fileDatastoreClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.213464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastores/file_datastore/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastores/file_datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22032 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastores/file_datastore/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastores/file_datastore/retrieve_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    27060 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastores/inMemoryDatastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    23666 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/ddl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.213464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/delegates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/delegates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/delegates/arrowastropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/delegates/arrownumpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/delegates/arrownumpydict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/delegates/arrowtable.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/delegates/dataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.217465 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25254 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    55578 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)    35795 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_data_coordinate_iterable.py
--rw-r--r--   0 runner    (1001) docker     (127)    15002 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    23173 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_governor.py
--rw-r--r--   0 runner    (1001) docker     (127)    22884 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    20940 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_packer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18368 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_record_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_record_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    19925 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_records.py
--rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_skypix.py
--rw-r--r--   0 runner    (1001) docker     (127)    24448 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_universe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/construction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/record_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.217465 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/direct_butler/
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/direct_butler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    97186 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/direct_butler/_direct_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/direct_butler/_direct_butler_collections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.217465 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/direct_query_driver/
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/direct_query_driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56804 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/direct_query_driver/_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/direct_query_driver/_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/direct_query_driver/_query_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    14516 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/direct_query_driver/_query_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    10552 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/direct_query_driver/_sql_column_visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.221464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/formatters/astropyTable.py
--rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/formatters/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/formatters/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/formatters/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/formatters/matplotlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/formatters/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)    43508 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/formatters/parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/formatters/pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/formatters/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    18319 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/mapping_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/name_shrinker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/nonempty_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/persistence_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    19630 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12605 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/pydantic_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.221464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/_data_coordinate_query_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/_dataset_query_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/_dimension_record_query_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/_expression_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)    26197 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/convert_args.py
--rw-r--r--   0 runner    (1001) docker     (127)    14730 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    19227 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/expression_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    18252 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/overlaps.py
--rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/result_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.225464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/tree/
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/tree/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/tree/_column_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/tree/_column_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/tree/_column_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/tree/_column_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    22474 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/tree/_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/tree/_query_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.225464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/_caching_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/_collection_record_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    10735 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/_collection_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/_collection_summary_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/_collection_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/_dataset_type_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    60859 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/_registry_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.225464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/bridge/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/bridge/ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (127)    16738 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/bridge/monolithic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.229464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/collections/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27734 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/collections/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/collections/nameKey.py
--rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/collections/synthIntKey.py
--rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/connectionString.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.229464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/databases/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25550 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/databases/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)    18122 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/databases/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.229464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.229464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/datasets/byDimensions/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/datasets/byDimensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24042 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/datasets/byDimensions/_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    51063 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/datasets/byDimensions/_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    16706 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/datasets/byDimensions/summaries.py
--rw-r--r--   0 runner    (1001) docker     (127)    19243 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/datasets/byDimensions/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.229464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/dimensions/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/dimensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54687 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/dimensions/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.233464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/interfaces/_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    15351 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/interfaces/_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)    26746 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/interfaces/_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    79984 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/interfaces/_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    25728 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/interfaces/_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    16907 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/interfaces/_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/interfaces/_obscore.py
--rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/interfaces/_opaque.py
--rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/interfaces/_versioning.py
--rw-r--r--   0 runner    (1001) docker     (127)    21369 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/nameShrinker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.233464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/obscore/
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/obscore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/obscore/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    16298 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/obscore/_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11748 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/obscore/_records.py
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/obscore/_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/obscore/_spatial.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/obscore/default_spatial.py
--rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/obscore/pgsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/opaque.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.233464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12630 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    49430 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    33980 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/_query_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    18361 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/_query_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    39215 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    16321 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/_sql_query_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    25440 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/_sql_query_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    20955 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/butler_sql_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.237465 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22473 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/categorize.py
--rw-r--r--   0 runner    (1001) docker     (127)    22911 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/check.py
--rw-r--r--   0 runner    (1001) docker     (127)    41024 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/normalForm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.237465 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/parser/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/parser/exprTree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/parser/parserLex.py
--rw-r--r--   0 runner    (1001) docker     (127)    14359 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/parser/parserYacc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.237465 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/parser/ply/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/parser/ply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43384 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/parser/ply/lex.py
--rw-r--r--   0 runner    (1001) docker     (127)   137077 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/parser/ply/yacc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/parser/treeVisitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/find_first_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)   114903 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/sql_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.237465 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64445 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/tests/_database.py
--rw-r--r--   0 runner    (1001) docker     (127)   184946 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/tests/_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/versions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19531 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/wildcards.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.241464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/_collection_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/_http_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7944 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/_query_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/_ref_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17645 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    22666 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/_remote_butler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.241464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/registry/_query_dimension_records.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.241464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/server/_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/server/_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/server/_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.241464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/server/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/server/handlers/_external.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/server/handlers/_external_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/server/handlers/_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     8558 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/server_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/repo_relocation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.245464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/_associate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/_pruneDatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/butlerImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/certifyCalibrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/collectionChain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/configDump.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/configValidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/createRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/exportCalibs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/ingest_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/queryCollections.py
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/queryDataIds.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/queryDatasetTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/queryDatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/queryDimensionRecords.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/register_dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/removeCollections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/removeDatasetType.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/removeRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/retrieveArtifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/transferDatasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.249464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/_datasetsHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/_dummyRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12966 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/_examplePythonTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    23754 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/_testRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)    37827 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/butler_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/cliCmdTestBase.py
--rw-r--r--   0 runner    (1001) docker     (127)    17098 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/cliLogTestBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/deferredFormatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/dict_convertible_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14769 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/hybrid_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13099 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/hybrid_butler_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/server_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/testFormatters.py
--rw-r--r--   0 runner    (1001) docker     (127)    13344 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10120 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24302 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/timespan_database_representation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.249464 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/transfers/
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16952 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/transfers/_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/transfers/_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    32431 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/transfers/_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-09 10:01:21.000000 lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.261464 lsst_daf_butler-27.2024.1900/python/lsst_daf_butler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-09 10:01:22.000000 lsst_daf_butler-27.2024.1900/python/lsst_daf_butler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18665 2024-05-09 10:01:22.000000 lsst_daf_butler-27.2024.1900/python/lsst_daf_butler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:01:22.000000 lsst_daf_butler-27.2024.1900/python/lsst_daf_butler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 10:01:22.000000 lsst_daf_butler-27.2024.1900/python/lsst_daf_butler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-09 10:01:22.000000 lsst_daf_butler-27.2024.1900/python/lsst_daf_butler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 10:01:22.000000 lsst_daf_butler-27.2024.1900/python/lsst_daf_butler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:01:21.000000 lsst_daf_butler-27.2024.1900/python/lsst_daf_butler.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-09 10:01:22.261464 lsst_daf_butler-27.2024.1900/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:01:22.261464 lsst_daf_butler-27.2024.1900/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_astropyTableFormatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)   125454 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_butler_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_cliCmdAssociate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_cliCmdConfigDump.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_cliCmdConfigValidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_cliCmdCreate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_cliCmdImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_cliCmdIngestFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    21626 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_cliCmdPruneDatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_cliCmdQueryCollections.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_cliCmdQueryDataIds.py
--rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_cliCmdQueryDatasetTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    20652 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_cliCmdQueryDatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_cliCmdQueryDimensionRecords.py
--rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_cliCmdRemoveCollections.py
--rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_cliCmdRemoveRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_cliCmdRetrieveArtifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_cliLog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_cliPluginLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_cliUtilSplitCommas.py
--rw-r--r--   0 runner    (1001) docker     (127)    12494 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_cliUtilSplitKv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_cliUtilToUpper.py
--rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_cliUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_composites.py
--rw-r--r--   0 runner    (1001) docker     (127)    25806 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_connectionString.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    29972 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    84810 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_ddl.py
--rw-r--r--   0 runner    (1001) docker     (127)    17831 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_dimension_record_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    45224 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_exprParserLex.py
--rw-r--r--   0 runner    (1001) docker     (127)    24938 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_exprParserYacc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16014 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11208 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_logFormatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12245 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_matplotlibFormatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_nonempty_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_normalFormExpression.py
--rw-r--r--   0 runner    (1001) docker     (127)    27146 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_obscore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)    85156 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)    11121 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_pydantic_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_quantum.py
--rw-r--r--   0 runner    (1001) docker     (127)    18384 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_quantumBackedButler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_query_direct_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_query_direct_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    90454 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_query_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    15859 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_query_relations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_query_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)    24404 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_query_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_remote_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)    18263 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    38408 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_simpleButler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    14764 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_storageClass.py
--rw-r--r--   0 runner    (1001) docker     (127)    18219 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_testRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_thread_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_time_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13053 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_timespan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-05-09 10:01:16.000000 lsst_daf_butler-27.2024.1900/tests/test_versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.159217 lsst_daf_butler-27.2024.2000/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-16 09:49:27.159217 lsst_daf_butler-27.2024.2000/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/bsd_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.083217 lsst_daf_butler-27.2024.2000/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.091217 lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/
+-rw-r--r--   0 runner    (1001) docker     (127)    54247 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/concreteStorageClasses.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/configuring.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/datastores.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10776 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/dimensions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    22653 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/formatters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/organizing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    23195 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/queries.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/use-in-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/writing-subcommands.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.087217 lsst_daf_butler-27.2024.2000/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.091217 lsst_daf_butler-27.2024.2000/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.091217 lsst_daf_butler-27.2024.2000/python/lsst/daf/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.099217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75170 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_butler_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9619 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_butler_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_butler_instance_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_butler_repo_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_column_categorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_column_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_column_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52100 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14135 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_config_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_dataset_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_dataset_existence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32133 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_dataset_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30028 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_deferredDatasetHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_exceptions_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_file_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_file_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30151 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_labeled_butler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15147 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_limited_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10451 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19541 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_named.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25574 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32289 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_quantum_backed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_registry_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37492 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14504 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_storage_class_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23377 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_timespan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.103217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_utilities/locked_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_utilities/named_locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_utilities/thread_safe_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16594 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/arrow_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.103217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14768 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/cliLog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.103217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/cmd/_remove_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/cmd/_remove_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/cmd/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.103217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/opt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/opt/optionGroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/opt/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44081 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/column_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.103217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/datastore.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.103217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/datastores/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/datastores/composites.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/datastores/fileDatastore.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/datastores/formatters.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/datastores/writeRecipes.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15382 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/dimensions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.107217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/old_dimensions/
+-rw-r--r--   0 runner    (1001) docker     (127)    13246 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13341 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15416 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15416 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15488 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15088 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe5.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15094 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15382 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe7.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/registry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/repo_transfer_formats.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/storageClasses.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.107217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastore/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57480 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastore/_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41721 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastore/cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastore/composites.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastore/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34999 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastore/file_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastore/generic_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastore/record_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13279 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastore/stored_file_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.107217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastores/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49806 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastores/chainedDatastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120549 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastores/fileDatastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastores/fileDatastoreClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.111217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastores/file_datastore/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastores/file_datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22032 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastores/file_datastore/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastores/file_datastore/retrieve_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27060 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastores/inMemoryDatastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23666 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/ddl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.111217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/delegates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/delegates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/delegates/arrowastropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/delegates/arrownumpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/delegates/arrownumpydict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/delegates/arrowtable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/delegates/dataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.115217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25254 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55578 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35795 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_data_coordinate_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15002 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23173 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_governor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22884 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20940 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_packer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18368 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_record_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_record_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19925 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_skypix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24448 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_universe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/construction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/record_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.115217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/direct_butler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/direct_butler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100744 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/direct_butler/_direct_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/direct_butler/_direct_butler_collections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.115217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/direct_query_driver/
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/direct_query_driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56804 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/direct_query_driver/_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/direct_query_driver/_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/direct_query_driver/_query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14516 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/direct_query_driver/_query_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10552 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/direct_query_driver/_sql_column_visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.115217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/formatters/astropyTable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/formatters/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/formatters/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/formatters/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/formatters/matplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/formatters/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43508 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/formatters/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/formatters/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/formatters/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18319 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/mapping_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/name_shrinker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/nonempty_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/persistence_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19630 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12605 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/pydantic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.119217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/_data_coordinate_query_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/_dataset_query_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/_dimension_record_query_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/_expression_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26197 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/convert_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14730 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19227 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/expression_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18252 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/overlaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/result_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.119217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/tree/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/tree/_column_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/tree/_column_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/tree/_column_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/tree/_column_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22474 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/tree/_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/tree/_query_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.123217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/_caching_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/_collection_record_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10735 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/_collection_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/_collection_summary_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/_collection_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/_dataset_type_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60859 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/_registry_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.123217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/bridge/ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16738 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/bridge/monolithic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.123217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27734 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/collections/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/collections/nameKey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/collections/synthIntKey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/connectionString.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.123217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25550 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/databases/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18122 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/databases/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.127217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.127217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/datasets/byDimensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/datasets/byDimensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24042 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/datasets/byDimensions/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51063 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/datasets/byDimensions/_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16706 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/datasets/byDimensions/summaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19243 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/datasets/byDimensions/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.127217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/dimensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/dimensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54687 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/dimensions/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.127217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/interfaces/_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15351 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/interfaces/_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26746 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/interfaces/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79984 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/interfaces/_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25728 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/interfaces/_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16907 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/interfaces/_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/interfaces/_obscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/interfaces/_opaque.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/interfaces/_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21369 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/nameShrinker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.131217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/obscore/
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/obscore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/obscore/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16298 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/obscore/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11748 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/obscore/_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/obscore/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/obscore/_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/obscore/default_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/obscore/pgsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/opaque.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.131217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12630 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49430 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33980 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/_query_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18361 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/_query_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39215 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16321 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/_sql_query_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25440 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/_sql_query_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20955 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/butler_sql_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.131217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22473 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/categorize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22911 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41024 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/normalForm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.135217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/parser/exprTree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/parser/parserLex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14359 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/parser/parserYacc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.135217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/parser/ply/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/parser/ply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43384 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/parser/ply/lex.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137077 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/parser/ply/yacc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/parser/treeVisitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/find_first_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)   114903 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/sql_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.135217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64445 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/tests/_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)   184946 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/tests/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19531 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/wildcards.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.135217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/_collection_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/_http_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7944 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/_query_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/_ref_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17645 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22666 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/_remote_butler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.135217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/registry/_query_dimension_records.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.139217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/server/_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/server/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/server/_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.139217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/server/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/server/handlers/_external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/server/handlers/_external_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/server/handlers/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8558 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/server_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/repo_relocation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.143217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/_associate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/_pruneDatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/butlerImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/certifyCalibrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/collectionChain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/configDump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/configValidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/createRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/exportCalibs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/ingest_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/queryCollections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/queryDataIds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/queryDatasetTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/queryDatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/queryDimensionRecords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/register_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/removeCollections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/removeDatasetType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/removeRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/retrieveArtifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/transferDatasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.143217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/_datasetsHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/_dummyRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/_examplePythonTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23754 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/_testRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37827 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/butler_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/cliCmdTestBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17098 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/cliLogTestBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/deferredFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/dict_convertible_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14769 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/hybrid_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13099 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/hybrid_butler_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/server_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/testFormatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13344 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10120 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24302 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/timespan_database_representation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.143217 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/transfers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16952 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/transfers/_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/transfers/_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32431 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/transfers/_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 09:49:26.000000 lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.159217 lsst_daf_butler-27.2024.2000/python/lsst_daf_butler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-16 09:49:27.000000 lsst_daf_butler-27.2024.2000/python/lsst_daf_butler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18665 2024-05-16 09:49:27.000000 lsst_daf_butler-27.2024.2000/python/lsst_daf_butler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:49:27.000000 lsst_daf_butler-27.2024.2000/python/lsst_daf_butler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-16 09:49:27.000000 lsst_daf_butler-27.2024.2000/python/lsst_daf_butler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-16 09:49:27.000000 lsst_daf_butler-27.2024.2000/python/lsst_daf_butler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 09:49:27.000000 lsst_daf_butler-27.2024.2000/python/lsst_daf_butler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:49:26.000000 lsst_daf_butler-27.2024.2000/python/lsst_daf_butler.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 09:49:27.159217 lsst_daf_butler-27.2024.2000/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:49:27.159217 lsst_daf_butler-27.2024.2000/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_astropyTableFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128241 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_butler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_cliCmdAssociate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_cliCmdConfigDump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_cliCmdConfigValidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_cliCmdCreate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_cliCmdImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_cliCmdIngestFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21626 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_cliCmdPruneDatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_cliCmdQueryCollections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_cliCmdQueryDataIds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_cliCmdQueryDatasetTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20652 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_cliCmdQueryDatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_cliCmdQueryDimensionRecords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_cliCmdRemoveCollections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_cliCmdRemoveRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_cliCmdRetrieveArtifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_cliLog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_cliPluginLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_cliUtilSplitCommas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12494 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_cliUtilSplitKv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_cliUtilToUpper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_cliUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_composites.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25806 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_connectionString.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29972 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84810 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_ddl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17831 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_dimension_record_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45224 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_exprParserLex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24938 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_exprParserYacc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16014 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11208 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_logFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12245 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_matplotlibFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_nonempty_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_normalFormExpression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27146 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_obscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85156 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11121 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_pydantic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18384 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_quantumBackedButler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_query_direct_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_query_direct_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90454 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_query_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15859 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_query_relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_query_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24404 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_query_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_remote_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18263 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38408 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_simpleButler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14764 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_storageClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18219 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_testRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_thread_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13053 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_timespan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-05-16 09:49:21.000000 lsst_daf_butler-27.2024.2000/tests/test_versioning.py
```

### Comparing `lsst_daf_butler-27.2024.1900/PKG-INFO` & `lsst_daf_butler-27.2024.2000/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-daf-butler
-Version: 27.2024.1900
+Version: 27.2024.2000
 Summary: An abstraction layer for reading and writing astronomical data to datastores.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/daf_butler
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_daf_butler-27.2024.1900/README.md` & `lsst_daf_butler-27.2024.2000/README.md`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/bsd_license.txt` & `lsst_daf_butler-27.2024.2000/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/CHANGES.rst` & `lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/concreteStorageClasses.rst` & `lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/concreteStorageClasses.rst`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/configuring.rst` & `lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/configuring.rst`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/datastores.rst` & `lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/datastores.rst`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/dimensions.rst` & `lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/dimensions.rst`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/formatters.rst` & `lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/formatters.rst`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/index.rst` & `lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/index.rst`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/organizing.rst` & `lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/organizing.rst`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/queries.rst` & `lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/queries.rst`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/use-in-tests.rst` & `lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/use-in-tests.rst`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/doc/lsst.daf.butler/writing-subcommands.rst` & `lsst_daf_butler-27.2024.2000/doc/lsst.daf.butler/writing-subcommands.rst`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/gpl-v3.0.txt` & `lsst_daf_butler-27.2024.2000/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/pyproject.toml` & `lsst_daf_butler-27.2024.2000/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_butler.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_butler.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_butler_collections.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_butler_collections.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_butler_config.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_butler_config.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_butler_instance_options.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_butler_instance_options.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_butler_repo_index.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_butler_repo_index.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_column_categorization.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_column_categorization.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_column_tags.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_column_tags.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_column_type_info.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_column_type_info.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_config.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_config.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_config_support.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_config_support.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_dataset_association.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_dataset_association.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_dataset_existence.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_dataset_existence.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_dataset_ref.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_dataset_ref.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_dataset_type.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_dataset_type.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_deferredDatasetHandle.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_deferredDatasetHandle.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_exceptions.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_exceptions.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_exceptions_legacy.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_exceptions_legacy.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_file_dataset.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_file_dataset.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_file_descriptor.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_file_descriptor.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_formatter.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_formatter.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_labeled_butler_factory.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_labeled_butler_factory.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_limited_butler.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_limited_butler.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_location.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_location.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_named.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_named.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_quantum.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_quantum.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_quantum_backed.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_quantum_backed.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_registry_shim.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_registry_shim.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_storage_class.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_storage_class.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_storage_class_delegate.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_storage_class_delegate.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_timespan.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_timespan.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_topology.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_topology.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_utilities/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_utilities/locked_object.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_utilities/locked_object.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_utilities/named_locks.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_utilities/named_locks.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/_utilities/thread_safe_cache.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/_utilities/thread_safe_cache.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/arrow_utils.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/arrow_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/butler.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/butler.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/cliLog.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/cliLog.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/cmd/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/cmd/_remove_collections.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/cmd/_remove_collections.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/cmd/_remove_runs.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/cmd/_remove_runs.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/cmd/commands.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/cmd/commands.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/opt/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/opt/arguments.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/opt/arguments.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/opt/optionGroups.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/opt/optionGroups.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/opt/options.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/opt/options.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/progress.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/progress.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/cli/utils.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/cli/utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/column_spec.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/column_spec.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/datastores/composites.yaml` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/datastores/composites.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/datastores/fileDatastore.yaml` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/datastores/fileDatastore.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/datastores/formatters.yaml` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/datastores/formatters.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/datastores/writeRecipes.yaml` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/datastores/writeRecipes.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/dimensions.yaml` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/dimensions.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe0.yaml` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe0.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe1.yaml` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe1.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe2.yaml` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe2.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe3.yaml` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe3.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe4.yaml` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe4.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe5.yaml` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe5.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe6.yaml` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe6.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe7.yaml` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe7.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/registry.yaml` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/registry.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/configs/storageClasses.yaml` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/configs/storageClasses.yaml`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastore/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastore/_datastore.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastore/_datastore.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastore/cache_manager.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastore/cache_manager.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastore/composites.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastore/composites.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastore/constraints.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastore/constraints.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastore/file_templates.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastore/file_templates.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastore/generic_base.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastore/generic_base.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastore/record_data.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastore/record_data.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastore/stored_file_info.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastore/stored_file_info.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastores/chainedDatastore.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastores/chainedDatastore.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastores/fileDatastore.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastores/fileDatastore.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastores/fileDatastoreClient.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastores/fileDatastoreClient.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastores/file_datastore/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastores/file_datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastores/file_datastore/get.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastores/file_datastore/get.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastores/file_datastore/retrieve_artifacts.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastores/file_datastore/retrieve_artifacts.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/datastores/inMemoryDatastore.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/datastores/inMemoryDatastore.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/ddl.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/ddl.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/delegates/arrowastropy.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/delegates/arrowastropy.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/delegates/arrownumpy.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/delegates/arrownumpy.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/delegates/arrownumpydict.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/delegates/arrownumpydict.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/delegates/arrowtable.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/delegates/arrowtable.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/delegates/dataframe.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/delegates/dataframe.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_config.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_config.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_coordinate.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_coordinate.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_data_coordinate_iterable.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_data_coordinate_iterable.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_database.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_database.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_elements.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_elements.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_governor.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_governor.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_graph.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_graph.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_group.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_group.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_packer.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_packer.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_record_set.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_record_set.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_record_table.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_record_table.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_records.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_records.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_schema.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_schema.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_skypix.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_skypix.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/_universe.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/_universe.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/construction.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/construction.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/dimensions/record_cache.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/dimensions/record_cache.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/direct_butler/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/direct_butler/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/direct_butler/_direct_butler.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/direct_butler/_direct_butler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1865,25 +1865,75 @@
         newly_registered_dataset_types = set()
         for datasetType in source_dataset_types:
             if register_dataset_types:
                 # Let this raise immediately if inconsistent. Continuing
                 # on to find additional inconsistent dataset types
                 # might result in additional unwanted dataset types being
                 # registered.
-                if self._registry.registerDatasetType(datasetType):
-                    newly_registered_dataset_types.add(datasetType)
+                try:
+                    if self._registry.registerDatasetType(datasetType):
+                        newly_registered_dataset_types.add(datasetType)
+                except ConflictingDefinitionError as e:
+                    # Be safe and require that conversions be bidirectional
+                    # when there are storage class mismatches. This is because
+                    # get() will have to support conversion from source to
+                    # target python type (the source formatter will be
+                    # returning source python type) but there also is an
+                    # expectation that people will want to be able to get() in
+                    # the target using the source python type, which will not
+                    # require conversion for transferred datasets but might
+                    # for target-native types. Additionally, butler.get does
+                    # not know that the formatter will return the wrong
+                    # python type and so will always check that the conversion
+                    # works even though it won't need it.
+                    target_dataset_type = self.get_dataset_type(datasetType.name)
+                    target_compatible_with_source = target_dataset_type.is_compatible_with(datasetType)
+                    source_compatible_with_target = datasetType.is_compatible_with(target_dataset_type)
+                    if not (target_compatible_with_source and source_compatible_with_target):
+                        if target_compatible_with_source:
+                            e.add_note(
+                                "Target dataset type storage class is compatible with source "
+                                "but the reverse is not true."
+                            )
+                        elif source_compatible_with_target:
+                            e.add_note(
+                                "Source dataset type storage class is compatible with target "
+                                "but the reverse is not true."
+                            )
+                        else:
+                            e.add_note("If storage classes differ, please register converters.")
+                        raise
             else:
                 # If the dataset type is missing, let it fail immediately.
                 target_dataset_type = self.get_dataset_type(datasetType.name)
                 if target_dataset_type != datasetType:
-                    raise ConflictingDefinitionError(
-                        "Source butler dataset type differs from definition"
-                        f" in target butler: {datasetType} !="
-                        f" {target_dataset_type}"
-                    )
+                    target_compatible_with_source = target_dataset_type.is_compatible_with(datasetType)
+                    source_compatible_with_target = datasetType.is_compatible_with(target_dataset_type)
+                    # Both conversion directions are currently required.
+                    if not (target_compatible_with_source and source_compatible_with_target):
+                        msg = ""
+                        if target_compatible_with_source:
+                            msg = (
+                                "Target storage class is compatible with the source storage class "
+                                "but the reverse is not true."
+                            )
+                        elif source_compatible_with_target:
+                            msg = (
+                                "Source storage class is compatible with the target storage class"
+                                " but the reverse is not true."
+                            )
+                        else:
+                            msg = "If storage classes differ register converters."
+                        if msg:
+                            msg = f"({msg})"
+                        raise ConflictingDefinitionError(
+                            "Source butler dataset type differs from definition"
+                            f" in target butler: {datasetType} !="
+                            f" {target_dataset_type} {msg}"
+                        )
         if newly_registered_dataset_types:
             # We may have registered some even if there were inconsistencies
             # but should let people know (or else remove them again).
             _LOG.verbose(
                 "Registered the following dataset types in the target Butler: %s",
                 ", ".join(d.name for d in newly_registered_dataset_types),
             )
@@ -1944,15 +1994,20 @@
 
                 # Assume we are using UUIDs and the source refs will match
                 # those imported.
                 if not dry_run:
                     imported_refs = self._registry._importDatasets(refs_to_import)
                 else:
                     imported_refs = refs_to_import
-                assert set(imported_refs) == set(refs_to_import)
+
+                # Check all the UUIDs were imported, ignoring dataset type
+                # storage class differences.
+                imported_uuids = set(ref.id for ref in imported_refs)
+                uuids_to_import = set(ref.id for ref in refs_to_import)
+                assert set(imported_uuids) == set(uuids_to_import)
                 n_imported += len(imported_refs)
 
             assert len(source_refs) == n_imported
             _LOG.verbose("Imported %d datasets into destination butler", n_imported)
 
             # Ask the datastore to transfer. The datastore has to check that
             # the source datastore is compatible with the target datastore.
```

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/direct_butler/_direct_butler_collections.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/direct_butler/_direct_butler_collections.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/direct_query_driver/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/direct_query_driver/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/direct_query_driver/_driver.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/direct_query_driver/_driver.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/direct_query_driver/_postprocessing.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/direct_query_driver/_postprocessing.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/direct_query_driver/_query_builder.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/direct_query_driver/_query_builder.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/direct_query_driver/_query_plan.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/direct_query_driver/_query_plan.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/direct_query_driver/_sql_column_visitor.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/direct_query_driver/_sql_column_visitor.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/formatters/astropyTable.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/formatters/astropyTable.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/formatters/file.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/formatters/file.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/formatters/json.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/formatters/json.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/formatters/logs.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/formatters/logs.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/formatters/matplotlib.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/formatters/matplotlib.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/formatters/packages.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/formatters/packages.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/formatters/parquet.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/formatters/parquet.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/formatters/pickle.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/formatters/pickle.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/formatters/yaml.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/formatters/yaml.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/json.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/json.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/logging.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/logging.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/mapping_factory.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/mapping_factory.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/name_shrinker.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/name_shrinker.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/nonempty_mapping.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/nonempty_mapping.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/persistence_context.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/persistence_context.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/progress.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/progress.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/pydantic_utils.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/_base.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/_base.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/_data_coordinate_query_results.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/_data_coordinate_query_results.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/_dataset_query_results.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/_dataset_query_results.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/_dimension_record_query_results.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/_dimension_record_query_results.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/_expression_strings.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/_expression_strings.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/_identifiers.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/_identifiers.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/_query.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/_query.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/convert_args.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/convert_args.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/driver.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/driver.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/expression_factory.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/expression_factory.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/overlaps.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/overlaps.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/result_specs.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/result_specs.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/tree/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/tree/_base.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/tree/_base.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/tree/_column_expression.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/tree/_column_expression.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/tree/_column_literal.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/tree/_column_literal.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/tree/_column_reference.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/tree/_column_reference.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/tree/_column_set.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/tree/_column_set.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/tree/_predicate.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/tree/_predicate.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/tree/_query_tree.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/tree/_query_tree.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/queries/visitors.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/queries/visitors.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/_caching_context.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/_caching_context.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/_collection_record_cache.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/_collection_record_cache.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/_collection_summary.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/_collection_summary.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/_collection_summary_cache.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/_collection_summary_cache.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/_collection_type.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/_collection_type.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/_config.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/_config.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/_dataset_type_cache.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/_dataset_type_cache.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/_defaults.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/_defaults.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/_exceptions.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/_exceptions.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/_registry.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/_registry.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/_registry_factory.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/_registry_factory.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/attributes.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/attributes.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/bridge/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/bridge/ephemeral.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/bridge/ephemeral.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/bridge/monolithic.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/bridge/monolithic.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/collections/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/collections/_base.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/collections/_base.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/collections/nameKey.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/collections/nameKey.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/collections/synthIntKey.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/collections/synthIntKey.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/connectionString.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/connectionString.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/databases/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/databases/postgresql.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/databases/postgresql.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/databases/sqlite.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/databases/sqlite.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/datasets/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/datasets/byDimensions/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/datasets/byDimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/datasets/byDimensions/_manager.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/datasets/byDimensions/_manager.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/datasets/byDimensions/_storage.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/datasets/byDimensions/_storage.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/datasets/byDimensions/summaries.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/datasets/byDimensions/summaries.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/datasets/byDimensions/tables.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/datasets/byDimensions/tables.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/dimensions/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/dimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/dimensions/static.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/dimensions/static.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/interfaces/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/interfaces/_attributes.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/interfaces/_attributes.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/interfaces/_bridge.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/interfaces/_bridge.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/interfaces/_collections.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/interfaces/_collections.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/interfaces/_database.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/interfaces/_database.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/interfaces/_datasets.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/interfaces/_datasets.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/interfaces/_dimensions.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/interfaces/_dimensions.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/interfaces/_obscore.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/interfaces/_obscore.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/interfaces/_opaque.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/interfaces/_opaque.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/interfaces/_versioning.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/interfaces/_versioning.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/managers.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/managers.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/nameShrinker.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/nameShrinker.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/obscore/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/obscore/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/obscore/_config.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/obscore/_config.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/obscore/_manager.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/obscore/_manager.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/obscore/_records.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/obscore/_records.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/obscore/_schema.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/obscore/_schema.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/obscore/_spatial.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/obscore/_spatial.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/obscore/default_spatial.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/obscore/default_spatial.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/obscore/pgsphere.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/obscore/pgsphere.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/opaque.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/opaque.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/_builder.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/_builder.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/_query.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/_query.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/_query_backend.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/_query_backend.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/_query_context.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/_query_context.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/_readers.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/_readers.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/_results.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/_results.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/_sql_query_backend.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/_sql_query_backend.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/_sql_query_context.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/_sql_query_context.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/_structs.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/_structs.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/butler_sql_engine.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/butler_sql_engine.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/_predicate.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/_predicate.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/categorize.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/categorize.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/check.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/check.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/normalForm.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/normalForm.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/parser/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/parser/exprTree.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/parser/exprTree.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/parser/parser.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/parser/parser.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/parser/parserLex.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/parser/parserLex.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/parser/parserYacc.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/parser/parserYacc.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/parser/ply/lex.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/parser/ply/lex.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/parser/ply/yacc.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/parser/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/expressions/parser/treeVisitor.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/expressions/parser/treeVisitor.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/queries/find_first_dataset.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/queries/find_first_dataset.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/sql_registry.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/sql_registry.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/tests/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/tests/_database.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/tests/_database.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/tests/_registry.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/tests/_registry.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/versions.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/versions.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/registry/wildcards.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/registry/wildcards.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/_authentication.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/_authentication.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/_collection_args.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/_collection_args.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/_config.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/_config.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/_factory.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/_factory.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/_http_connection.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/_http_connection.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/_query_driver.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/_query_driver.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/_ref_utils.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/_ref_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/_registry.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/_registry.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/_remote_butler.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/_remote_butler.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/registry/_query_dimension_records.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/registry/_query_dimension_records.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/server/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/server/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/server/_dependencies.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/server/_dependencies.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/server/_factory.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/server/_factory.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/server/_server.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/server/_server.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/server/handlers/_external.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/server/handlers/_external.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/server/handlers/_external_query.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/server/handlers/_external_query.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/server/handlers/_internal.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/server/handlers/_internal.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/remote_butler/server_models.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/remote_butler/server_models.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/repo_relocation.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/repo_relocation.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/_associate.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/_associate.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/_pruneDatasets.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/_pruneDatasets.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/butlerImport.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/butlerImport.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/certifyCalibrations.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/certifyCalibrations.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/collectionChain.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/collectionChain.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/configDump.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/configDump.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/configValidate.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/configValidate.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/createRepo.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/createRepo.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/exportCalibs.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/exportCalibs.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/ingest_files.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/ingest_files.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/queryCollections.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/queryCollections.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/queryDataIds.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/queryDataIds.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/queryDatasetTypes.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/queryDatasetTypes.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/queryDatasets.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/queryDatasets.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/queryDimensionRecords.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/queryDimensionRecords.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/register_dataset_type.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/register_dataset_type.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/removeCollections.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/removeCollections.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/removeDatasetType.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/removeDatasetType.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/removeRuns.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/removeRuns.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/retrieveArtifacts.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/retrieveArtifacts.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/script/transferDatasets.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/script/transferDatasets.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/_datasetsHelper.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/_datasetsHelper.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/_dummyRegistry.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/_dummyRegistry.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/_examplePythonTypes.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/_examplePythonTypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,14 +270,30 @@
         """
         data = exportDict["data"] if "data" in exportDict else None
         assert isinstance(data, list | types.NoneType)
         assert isinstance(exportDict["summary"], dict | types.NoneType)
         assert isinstance(exportDict["output"], dict | types.NoneType)
         return cls(exportDict["summary"], exportDict["output"], data)
 
+    @classmethod
+    def from_model(cls, model: MetricsExampleModel) -> MetricsExample:
+        """Create metrics from Pydantic model.
+
+        Parameters
+        ----------
+        model : `MetricsExampleModel`
+            Source model.
+
+        Returns
+        -------
+        newobject : `MetricsExample`
+            New `MetricsExample` object.
+        """
+        return cls(model.summary, model.output, model.data)
+
 
 class MetricsExampleModel(BaseModel):
     """A variant of `MetricsExample` based on model."""
 
     summary: dict[str, Any] | None = None
     output: dict[str, Any] | None = None
     data: list[Any] | None = None
```

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/_testRepo.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/_testRepo.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/butler_queries.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/butler_queries.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/cliCmdTestBase.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/cliCmdTestBase.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/cliLogTestBase.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/cliLogTestBase.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/deferredFormatter.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/deferredFormatter.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/dict_convertible_model.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/dict_convertible_model.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/hybrid_butler.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/hybrid_butler.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/hybrid_butler_registry.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/hybrid_butler_registry.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/server.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/server.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/server_utils.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/server_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/testFormatters.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/testFormatters.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/tests/utils.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/tests/utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/time_utils.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/time_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/timespan_database_representation.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/timespan_database_representation.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/transfers/__init__.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/transfers/_context.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/transfers/_context.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/transfers/_interfaces.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/transfers/_interfaces.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/transfers/_yaml.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/transfers/_yaml.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst/daf/butler/utils.py` & `lsst_daf_butler-27.2024.2000/python/lsst/daf/butler/utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst_daf_butler.egg-info/PKG-INFO` & `lsst_daf_butler-27.2024.2000/python/lsst_daf_butler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-daf-butler
-Version: 27.2024.1900
+Version: 27.2024.2000
 Summary: An abstraction layer for reading and writing astronomical data to datastores.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/daf_butler
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_daf_butler-27.2024.1900/python/lsst_daf_butler.egg-info/SOURCES.txt` & `lsst_daf_butler-27.2024.2000/python/lsst_daf_butler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_astropyTableFormatter.py` & `lsst_daf_butler-27.2024.2000/tests/test_astropyTableFormatter.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_authentication.py` & `lsst_daf_butler-27.2024.2000/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_butler.py` & `lsst_daf_butler-27.2024.2000/tests/test_butler.py`

 * *Files 2% similar despite different names*

```diff
@@ -2446,14 +2446,33 @@
 
         # Configure the source butler to allow trust.
         self.source_butler._datastore._set_trust_mode(True)
 
         # Test disassembly.
         self.assertButlerTransfers(purge=True, storageClassName="StructuredComposite")
 
+    def testTransferDifferingStorageClasses(self) -> None:
+        """Test transfers when the source butler dataset type has a different
+        but compatible storage class.
+        """
+        self.create_butlers()
+
+        self.assertButlerTransfers(storageClassNameTarget="MetricsConversion")
+
+    def testTransferDifferingStorageClassesDisassembly(self) -> None:
+        """Test transfers when the source butler dataset type has a different
+        but compatible storage class and where the source butler has
+        disassembled.
+        """
+        self.create_butlers()
+
+        self.assertButlerTransfers(
+            storageClassName="StructuredComposite", storageClassNameTarget="MetricsConversion"
+        )
+
     def testAbsoluteURITransferDirect(self) -> None:
         """Test transfer using an absolute URI."""
         self._absolute_transfer("auto")
 
     def testAbsoluteURITransferCopy(self) -> None:
         """Test transfer using an absolute URI."""
         self._absolute_transfer("copy")
@@ -2485,17 +2504,27 @@
 
             uri = self.target_butler.getURI(dataset.refs[0])
             if transfer == "auto":
                 self.assertEqual(uri, temp)
             else:
                 self.assertNotEqual(uri, temp)
 
-    def assertButlerTransfers(self, purge: bool = False, storageClassName: str = "StructuredData") -> None:
+    def assertButlerTransfers(
+        self,
+        purge: bool = False,
+        storageClassName: str = "StructuredData",
+        storageClassNameTarget: str | None = None,
+    ) -> None:
         """Test that a run can be transferred to another butler."""
         storageClass = self.storageClassFactory.getStorageClass(storageClassName)
+        if storageClassNameTarget is not None:
+            storageClassTarget = self.storageClassFactory.getStorageClass(storageClassNameTarget)
+        else:
+            storageClassTarget = storageClass
+
         datasetTypeName = "random_data"
 
         # Test will create 3 collections and we will want to transfer
         # two of those three.
         runs = ["run1", "run2", "other"]
 
         # Also want to use two different dataset types to ensure that
@@ -2641,14 +2670,22 @@
             self.target_butler.transfer_from(self.source_butler, source_refs)
 
         # Transfer without creating dimensions should fail.
         with self.assertRaises(ConflictingDefinitionError) as cm:
             self.target_butler.transfer_from(self.source_butler, source_refs, register_dataset_types=True)
         self.assertIn("dimension", str(cm.exception))
 
+        # The dry run test requires dataset types to exist. If we have
+        # been given distinct storage classes for the target we have
+        # to redefine at least one of the dataset types in the target butler.
+        if storageClass != storageClassTarget:
+            self.target_butler.registry.removeDatasetType(datasetTypeNames[0])
+            datasetType = DatasetType(datasetTypeNames[0], dimensions, storageClassTarget)
+            self.target_butler.registry.registerDatasetType(datasetType)
+
         # The failed transfer above leaves registry in an inconsistent
         # state because the run is created but then rolled back without
         # the collection cache being cleared. For now force a refresh.
         # Can remove with DM-35498.
         self.target_butler.registry.refresh()
 
         # Do a dry run -- this should not have any effect on the target butler.
@@ -2701,14 +2738,35 @@
         # Now try to get the same refs from the new butler.
         for ref in source_refs:
             if ref not in deleted:
                 new_metric = self.target_butler.get(ref)
                 old_metric = self.source_butler.get(ref)
                 self.assertEqual(new_metric, old_metric)
 
+                # Try again without implicit storage class conversion
+                # triggered by using the source ref. This will do conversion
+                # since the formatter will be returning the source python type.
+                target_ref = self.target_butler.get_dataset(ref.id)
+                if target_ref.datasetType.storageClass != ref.datasetType.storageClass:
+                    new_metric = self.target_butler.get(target_ref)
+                    self.assertNotEqual(type(new_metric), type(old_metric))
+
+                    # Remove the dataset from the target and put it again
+                    # as if it was the right type all along for this butler.
+                    self.target_butler.pruneDatasets(
+                        [target_ref], unstore=True, purge=True, disassociate=True
+                    )
+                    self.target_butler.put(new_metric, target_ref)
+                    new_new_metric = self.target_butler.get(target_ref)
+                    new_old_metric = self.target_butler.get(
+                        target_ref, storageClass=ref.datasetType.storageClass
+                    )
+                    self.assertEqual(new_new_metric, new_metric)
+                    self.assertEqual(new_old_metric, old_metric)
+
         # Now prune run2 collection and create instead a CHAINED collection.
         # This should block the transfer.
         self.target_butler.removeRuns(["run2"], unstore=True)
         self.target_butler.registry.registerCollection("run2", CollectionType.CHAINED)
         with self.assertRaises(CollectionTypeError):
             # Re-importing the run1 datasets can be problematic if they
             # use integer IDs so filter those out.
```

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_butler_factory.py` & `lsst_daf_butler-27.2024.2000/tests/test_butler_factory.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_cliCmdAssociate.py` & `lsst_daf_butler-27.2024.2000/tests/test_cliCmdAssociate.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_cliCmdConfigDump.py` & `lsst_daf_butler-27.2024.2000/tests/test_cliCmdConfigDump.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_cliCmdConfigValidate.py` & `lsst_daf_butler-27.2024.2000/tests/test_cliCmdConfigValidate.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_cliCmdCreate.py` & `lsst_daf_butler-27.2024.2000/tests/test_cliCmdCreate.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_cliCmdImport.py` & `lsst_daf_butler-27.2024.2000/tests/test_cliCmdImport.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_cliCmdIngestFiles.py` & `lsst_daf_butler-27.2024.2000/tests/test_cliCmdIngestFiles.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_cliCmdPruneDatasets.py` & `lsst_daf_butler-27.2024.2000/tests/test_cliCmdPruneDatasets.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_cliCmdQueryCollections.py` & `lsst_daf_butler-27.2024.2000/tests/test_cliCmdQueryCollections.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_cliCmdQueryDataIds.py` & `lsst_daf_butler-27.2024.2000/tests/test_cliCmdQueryDataIds.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_cliCmdQueryDatasetTypes.py` & `lsst_daf_butler-27.2024.2000/tests/test_cliCmdQueryDatasetTypes.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_cliCmdQueryDatasets.py` & `lsst_daf_butler-27.2024.2000/tests/test_cliCmdQueryDatasets.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_cliCmdQueryDimensionRecords.py` & `lsst_daf_butler-27.2024.2000/tests/test_cliCmdQueryDimensionRecords.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_cliCmdRemoveCollections.py` & `lsst_daf_butler-27.2024.2000/tests/test_cliCmdRemoveCollections.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_cliCmdRemoveRuns.py` & `lsst_daf_butler-27.2024.2000/tests/test_cliCmdRemoveRuns.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_cliCmdRetrieveArtifacts.py` & `lsst_daf_butler-27.2024.2000/tests/test_cliCmdRetrieveArtifacts.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_cliLog.py` & `lsst_daf_butler-27.2024.2000/tests/test_cliLog.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_cliPluginLoader.py` & `lsst_daf_butler-27.2024.2000/tests/test_cliPluginLoader.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_cliUtilSplitCommas.py` & `lsst_daf_butler-27.2024.2000/tests/test_cliUtilSplitCommas.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_cliUtilSplitKv.py` & `lsst_daf_butler-27.2024.2000/tests/test_cliUtilSplitKv.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_cliUtilToUpper.py` & `lsst_daf_butler-27.2024.2000/tests/test_cliUtilToUpper.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_cliUtils.py` & `lsst_daf_butler-27.2024.2000/tests/test_cliUtils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_composites.py` & `lsst_daf_butler-27.2024.2000/tests/test_composites.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_config.py` & `lsst_daf_butler-27.2024.2000/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_connectionString.py` & `lsst_daf_butler-27.2024.2000/tests/test_connectionString.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_constraints.py` & `lsst_daf_butler-27.2024.2000/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_datasets.py` & `lsst_daf_butler-27.2024.2000/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_datastore.py` & `lsst_daf_butler-27.2024.2000/tests/test_datastore.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_ddl.py` & `lsst_daf_butler-27.2024.2000/tests/test_ddl.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_dimension_record_containers.py` & `lsst_daf_butler-27.2024.2000/tests/test_dimension_record_containers.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_dimensions.py` & `lsst_daf_butler-27.2024.2000/tests/test_dimensions.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_exprParserLex.py` & `lsst_daf_butler-27.2024.2000/tests/test_exprParserLex.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_exprParserYacc.py` & `lsst_daf_butler-27.2024.2000/tests/test_exprParserYacc.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_expressions.py` & `lsst_daf_butler-27.2024.2000/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_formatter.py` & `lsst_daf_butler-27.2024.2000/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_location.py` & `lsst_daf_butler-27.2024.2000/tests/test_location.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_logFormatter.py` & `lsst_daf_butler-27.2024.2000/tests/test_logFormatter.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_logging.py` & `lsst_daf_butler-27.2024.2000/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_matplotlibFormatter.py` & `lsst_daf_butler-27.2024.2000/tests/test_matplotlibFormatter.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_nonempty_mapping.py` & `lsst_daf_butler-27.2024.2000/tests/test_nonempty_mapping.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_normalFormExpression.py` & `lsst_daf_butler-27.2024.2000/tests/test_normalFormExpression.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_obscore.py` & `lsst_daf_butler-27.2024.2000/tests/test_obscore.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_packages.py` & `lsst_daf_butler-27.2024.2000/tests/test_packages.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_parquet.py` & `lsst_daf_butler-27.2024.2000/tests/test_parquet.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_postgresql.py` & `lsst_daf_butler-27.2024.2000/tests/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_progress.py` & `lsst_daf_butler-27.2024.2000/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_pydantic_utils.py` & `lsst_daf_butler-27.2024.2000/tests/test_pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_quantum.py` & `lsst_daf_butler-27.2024.2000/tests/test_quantum.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_quantumBackedButler.py` & `lsst_daf_butler-27.2024.2000/tests/test_quantumBackedButler.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_query_direct_postgresql.py` & `lsst_daf_butler-27.2024.2000/tests/test_query_direct_postgresql.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_query_direct_sqlite.py` & `lsst_daf_butler-27.2024.2000/tests/test_query_direct_sqlite.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_query_interface.py` & `lsst_daf_butler-27.2024.2000/tests/test_query_interface.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_query_relations.py` & `lsst_daf_butler-27.2024.2000/tests/test_query_relations.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_query_remote.py` & `lsst_daf_butler-27.2024.2000/tests/test_query_remote.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_query_utilities.py` & `lsst_daf_butler-27.2024.2000/tests/test_query_utilities.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_remote_butler.py` & `lsst_daf_butler-27.2024.2000/tests/test_remote_butler.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_server.py` & `lsst_daf_butler-27.2024.2000/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_simpleButler.py` & `lsst_daf_butler-27.2024.2000/tests/test_simpleButler.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_sqlite.py` & `lsst_daf_butler-27.2024.2000/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_storageClass.py` & `lsst_daf_butler-27.2024.2000/tests/test_storageClass.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_templates.py` & `lsst_daf_butler-27.2024.2000/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_testRepo.py` & `lsst_daf_butler-27.2024.2000/tests/test_testRepo.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_thread_utils.py` & `lsst_daf_butler-27.2024.2000/tests/test_thread_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_time_utils.py` & `lsst_daf_butler-27.2024.2000/tests/test_time_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_timespan.py` & `lsst_daf_butler-27.2024.2000/tests/test_timespan.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_utils.py` & `lsst_daf_butler-27.2024.2000/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_daf_butler-27.2024.1900/tests/test_versioning.py` & `lsst_daf_butler-27.2024.2000/tests/test_versioning.py`

 * *Files identical despite different names*

