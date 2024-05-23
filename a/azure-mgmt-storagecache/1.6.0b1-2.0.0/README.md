# Comparing `tmp/azure-mgmt-storagecache-1.6.0b1.tar.gz` & `tmp/azure-mgmt-storagecache-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-mgmt-storagecache-1.6.0b1.tar", last modified: Thu Feb 22 05:16:57 2024, max compression
+gzip compressed data, was "azure-mgmt-storagecache-2.0.0.tar", last modified: Thu May 23 04:17:57 2024, max compression
```

## Comparing `azure-mgmt-storagecache-1.6.0b1.tar` & `azure-mgmt-storagecache-2.0.0.tar`

### file list

```diff
@@ -1,69 +1,71 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-02-22 05:16:57.868192 azure-mgmt-storagecache-1.6.0b1/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5073 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      218 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/MANIFEST.in
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     8128 2024-02-22 05:16:57.868192 azure-mgmt-storagecache-1.6.0b1/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2039 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/README.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      632 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/_meta.json
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-02-22 05:16:57.856192 azure-mgmt-storagecache-1.6.0b1/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-02-22 05:16:57.856192 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-02-22 05:16:57.856192 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      925 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3525 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1530 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    79289 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/_serialization.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6579 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/_storage_cache_management_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1344 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/_vendor.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      488 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-02-22 05:16:57.856192 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      872 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3573 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1530 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6747 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/_storage_cache_management_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1084 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/_vendor.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-02-22 05:16:57.860192 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1611 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    51677 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/_aml_filesystems_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4651 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/_asc_operations_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6073 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/_asc_usages_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   125977 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/_caches_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5749 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5847 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/_skus_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13442 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/_storage_cache_management_client_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27243 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/_storage_target_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    41238 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/_storage_targets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5867 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/_usage_models_operations.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-02-22 05:16:57.860192 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8885 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   151667 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/models/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7200 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/models/_storage_cache_management_client_enums.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-02-22 05:16:57.864192 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1611 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    63335 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/_aml_filesystems_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5926 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/_asc_operations_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7157 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/_asc_usages_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   147214 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/_caches_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6440 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6786 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/_skus_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15849 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/_storage_cache_management_client_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33214 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/_storage_target_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    50423 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/_storage_targets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6805 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/_usage_models_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-02-22 05:16:57.868192 azure-mgmt-storagecache-1.6.0b1/azure_mgmt_storagecache.egg-info/
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     8128 2024-02-22 05:16:57.000000 azure-mgmt-storagecache-1.6.0b1/azure_mgmt_storagecache.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2677 2024-02-22 05:16:57.000000 azure-mgmt-storagecache-1.6.0b1/azure_mgmt_storagecache.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-02-22 05:16:57.000000 azure-mgmt-storagecache-1.6.0b1/azure_mgmt_storagecache.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-02-22 05:16:57.000000 azure-mgmt-storagecache-1.6.0b1/azure_mgmt_storagecache.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       70 2024-02-22 05:16:57.000000 azure-mgmt-storagecache-1.6.0b1/azure_mgmt_storagecache.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-02-22 05:16:57.000000 azure-mgmt-storagecache-1.6.0b1/azure_mgmt_storagecache.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-02-22 05:16:57.868192 azure-mgmt-storagecache-1.6.0b1/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2792 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-02-22 05:16:57.868192 azure-mgmt-storagecache-1.6.0b1/tests/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2616 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/tests/conftest.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1042 2024-02-22 05:15:58.000000 azure-mgmt-storagecache-1.6.0b1/tests/test_cli_mgmt_storagecache.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:57.599052 azure-mgmt-storagecache-2.0.0/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5651 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      218 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/MANIFEST.in
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8602 2024-05-23 04:17:57.599052 azure-mgmt-storagecache-2.0.0/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2039 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/README.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      634 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/_meta.json
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:57.587052 azure-mgmt-storagecache-2.0.0/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:57.587052 azure-mgmt-storagecache-2.0.0/azure/mgmt/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:57.591052 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      925 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3442 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1530 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/_serialization.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7898 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/_storage_cache_management_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1344 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/_vendor.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:57.591052 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      872 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3490 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1530 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8094 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/_storage_cache_management_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1084 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/_vendor.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:57.595052 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1697 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    43964 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/_aml_filesystems_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4402 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/_asc_operations_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5811 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/_asc_usages_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   101899 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/_caches_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    35198 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/_import_jobs_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5549 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5622 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/_skus_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12312 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/_storage_cache_management_client_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    22883 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/_storage_target_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    34834 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/_storage_targets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5635 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/_usage_models_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:57.595052 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9606 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   167402 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/models/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9176 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/models/_storage_cache_management_client_enums.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:57.599052 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1697 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    55628 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/_aml_filesystems_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5669 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/_asc_operations_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6887 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/_asc_usages_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   123278 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/_caches_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    44093 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/_import_jobs_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6232 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6553 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/_skus_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    14742 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/_storage_cache_management_client_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    28862 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/_storage_target_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    44031 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/_storage_targets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6565 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/_usage_models_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:57.599052 azure-mgmt-storagecache-2.0.0/azure_mgmt_storagecache.egg-info/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8602 2024-05-23 04:17:57.000000 azure-mgmt-storagecache-2.0.0/azure_mgmt_storagecache.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2805 2024-05-23 04:17:57.000000 azure-mgmt-storagecache-2.0.0/azure_mgmt_storagecache.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-23 04:17:57.000000 azure-mgmt-storagecache-2.0.0/azure_mgmt_storagecache.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-23 04:17:57.000000 azure-mgmt-storagecache-2.0.0/azure_mgmt_storagecache.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       56 2024-05-23 04:17:57.000000 azure-mgmt-storagecache-2.0.0/azure_mgmt_storagecache.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-05-23 04:17:57.000000 azure-mgmt-storagecache-2.0.0/azure_mgmt_storagecache.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-05-23 04:17:57.599052 azure-mgmt-storagecache-2.0.0/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2791 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:57.599052 azure-mgmt-storagecache-2.0.0/tests/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2616 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/tests/conftest.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1042 2024-05-23 04:16:42.000000 azure-mgmt-storagecache-2.0.0/tests/test_cli_mgmt_storagecache.py
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/CHANGELOG.md` & `azure-mgmt-storagecache-2.0.0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,25 @@
 # Release History
 
+## 2.0.0 (2024-05-20)
+
+### Features Added
+
+  - Added operation group ImportJobsOperations
+  - Model AmlFilesystem has a new parameter root_squash_settings
+  - Model AmlFilesystemHsmSettings has a new parameter import_prefixes_initial
+  - Model AmlFilesystemUpdate has a new parameter root_squash_settings
+  - Model ErrorResponse has a new parameter error
+  - Model AscOperation.error changes type from ErrorResponse to AscOperationErrorResponse
+
+### Breaking Changes
+
+  - Model ErrorResponse no longer has parameter code
+  - Model ErrorResponse no longer has parameter message
+
 ## 1.6.0b1 (2024-02-22)
 
 ### Features Added
 
   - Model AmlFilesystem has a new parameter root_squash_settings
   - Model AmlFilesystemUpdate has a new parameter root_squash_settings
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/LICENSE` & `azure-mgmt-storagecache-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-mgmt-storagecache-1.6.0b1/PKG-INFO` & `azure-mgmt-storagecache-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-storagecache
-Version: 1.6.0b1
+Version: 2.0.0
 Summary: Microsoft Azure Storage Cache Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: isodate<1.0.0,>=0.6.1
-Requires-Dist: azure-common~=1.1
-Requires-Dist: azure-mgmt-core<2.0.0,>=1.3.2
 
 # Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Storage Cache Management Client Library.
 This package has been tested with Python 3.8+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
@@ -85,14 +82,30 @@
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 # Release History
 
+## 2.0.0 (2024-05-20)
+
+### Features Added
+
+  - Added operation group ImportJobsOperations
+  - Model AmlFilesystem has a new parameter root_squash_settings
+  - Model AmlFilesystemHsmSettings has a new parameter import_prefixes_initial
+  - Model AmlFilesystemUpdate has a new parameter root_squash_settings
+  - Model ErrorResponse has a new parameter error
+  - Model AscOperation.error changes type from ErrorResponse to AscOperationErrorResponse
+
+### Breaking Changes
+
+  - Model ErrorResponse no longer has parameter code
+  - Model ErrorResponse no longer has parameter message
+
 ## 1.6.0b1 (2024-02-22)
 
 ### Features Added
 
   - Model AmlFilesystem has a new parameter root_squash_settings
   - Model AmlFilesystemUpdate has a new parameter root_squash_settings
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/README.md` & `azure-mgmt-storagecache-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `azure-mgmt-storagecache-1.6.0b1/_meta.json` & `azure-mgmt-storagecache-2.0.0/_meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'autorest_command'": "'autorest specification/storagecache/resource-manager/readme.md "*

 * *                       '--generate-sample=True --include-x-ms-examples-original-file=True --python '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk '*

 * *                       '--use=@autorest/python@6.13.7 --use=@autorest/modelerfour@4.27.0 '*

 * *                       "--version=3.9.7 --version-tolerant=False'",*

 * * "'commit'": "'a013dabbe84aeb3f5d48b0e30d15fdfbb6a8d062'",*

 * * "'use'": "[' […]*

```diff
@@ -1,11 +1,11 @@
 {
     "autorest": "3.9.7",
-    "autorest_command": "autorest specification/storagecache/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.7.1 --use=@autorest/modelerfour@4.26.2 --version=3.9.7 --version-tolerant=False",
-    "commit": "aac54838d8d098a005df918d1667ff19423cc51f",
+    "autorest_command": "autorest specification/storagecache/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.13.7 --use=@autorest/modelerfour@4.27.0 --version=3.9.7 --version-tolerant=False",
+    "commit": "a013dabbe84aeb3f5d48b0e30d15fdfbb6a8d062",
     "readme": "specification/storagecache/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@6.7.1",
-        "@autorest/modelerfour@4.26.2"
+        "@autorest/python@6.13.7",
+        "@autorest/modelerfour@4.27.0"
     ]
 }
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/__init__.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/_configuration.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/_configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,63 +4,62 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any, TYPE_CHECKING
 
-from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
-from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
+from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
 
-from ._version import VERSION
+from .._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials import TokenCredential
+    from azure.core.credentials_async import AsyncTokenCredential
 
 
-class StorageCacheManagementClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+class StorageCacheManagementClientConfiguration:  # pylint: disable=too-many-instance-attributes,name-too-long
     """Configuration for StorageCacheManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials.TokenCredential
+    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2023-11-01-preview". Note that overriding
-     this default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2024-03-01". Note that overriding this
+     default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        super(StorageCacheManagementClientConfiguration, self).__init__(**kwargs)
-        api_version: str = kwargs.pop("api_version", "2023-11-01-preview")
+    def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
+        api_version: str = kwargs.pop("api_version", "2024-03-01")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
         self.subscription_id = subscription_id
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
         kwargs.setdefault("sdk_moniker", "mgmt-storagecache/{}".format(VERSION))
+        self.polling_interval = kwargs.get("polling_interval", 30)
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
-            self.authentication_policy = ARMChallengeAuthenticationPolicy(
+            self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/_patch.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/_serialization.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/_serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,16 @@
     from urllib import quote  # type: ignore
 except ImportError:
     from urllib.parse import quote
 import xml.etree.ElementTree as ET
 
 import isodate  # type: ignore
 
-from azure.core.exceptions import DeserializationError, SerializationError, raise_with_traceback
-from azure.core.serialization import NULL as AzureCoreNull
+from azure.core.exceptions import DeserializationError, SerializationError
+from azure.core.serialization import NULL as CoreNull
 
 _BOM = codecs.BOM_UTF8.decode(encoding="utf-8")
 
 ModelType = TypeVar("ModelType", bound="Model")
 JSON = MutableMapping[str, Any]
 
 
@@ -120,15 +120,15 @@
                     if isinstance(data, unicode):  # type: ignore
                         # If I'm Python 2.7 and unicode XML will scream if I try a "fromstring" on unicode string
                         data_as_str = data_as_str.encode(encoding="utf-8")  # type: ignore
                 except NameError:
                     pass
 
                 return ET.fromstring(data_as_str)  # nosec
-            except ET.ParseError:
+            except ET.ParseError as err:
                 # It might be because the server has an issue, and returned JSON with
                 # content-type XML....
                 # So let's try a JSON load, and if it's still broken
                 # let's flow the initial exception
                 def _json_attemp(data):
                     try:
                         return True, json.loads(data)
@@ -139,15 +139,15 @@
                 if success:
                     return json_result
                 # If i'm here, it's not JSON, it's not XML, let's scream
                 # and raise the last context in this block (the XML exception)
                 # The function hack is because Py2.7 messes up with exception
                 # context otherwise.
                 _LOGGER.critical("Wasn't XML not JSON, failing")
-                raise_with_traceback(DeserializationError, "XML is invalid")
+                raise DeserializationError("XML is invalid") from err
         raise DeserializationError("Cannot deserialize content-type: {}".format(content_type))
 
     @classmethod
     def deserialize_from_http_generics(cls, body_bytes: Optional[Union[AnyStr, IO]], headers: Mapping) -> Any:
         """Deserialize from HTTP response.
 
         Use bytes and headers to NOT use any requests/aiohttp or whatever
@@ -166,21 +166,14 @@
             content_type = "application/json"
 
         if body_bytes:
             return cls.deserialize_from_text(body_bytes, content_type)
         return None
 
 
-try:
-    basestring  # type: ignore
-    unicode_str = unicode  # type: ignore
-except NameError:
-    basestring = str
-    unicode_str = str
-
 _LOGGER = logging.getLogger(__name__)
 
 try:
     _long_type = long  # type: ignore
 except NameError:
     _long_type = int
 
@@ -291,15 +284,15 @@
     """
 
     _subtype_map: Dict[str, Dict[str, Any]] = {}
     _attribute_map: Dict[str, Dict[str, Any]] = {}
     _validation: Dict[str, Dict[str, Any]] = {}
 
     def __init__(self, **kwargs: Any) -> None:
-        self.additional_properties: Dict[str, Any] = {}
+        self.additional_properties: Optional[Dict[str, Any]] = {}
         for k in kwargs:
             if k not in self._attribute_map:
                 _LOGGER.warning("%s is not a known attribute of class %s and will be ignored", k, self.__class__)
             elif k in self._validation and self._validation[k].get("readonly", False):
                 _LOGGER.warning("Readonly attribute %s will be ignored in class %s", k, self.__class__)
             else:
                 setattr(self, k, kwargs[k])
@@ -336,26 +329,26 @@
             xml_map = cls._xml_map  # type: ignore
         except AttributeError:
             xml_map = {}
 
         return _create_xml_node(xml_map.get("name", cls.__name__), xml_map.get("prefix", None), xml_map.get("ns", None))
 
     def serialize(self, keep_readonly: bool = False, **kwargs: Any) -> JSON:
-        """Return the JSON that would be sent to azure from this model.
+        """Return the JSON that would be sent to server from this model.
 
         This is an alias to `as_dict(full_restapi_key_transformer, keep_readonly=False)`.
 
         If you want XML serialization, you can pass the kwargs is_xml=True.
 
         :param bool keep_readonly: If you want to serialize the readonly attributes
         :returns: A dict JSON compatible object
         :rtype: dict
         """
         serializer = Serializer(self._infer_class_models())
-        return serializer._serialize(self, keep_readonly=keep_readonly, **kwargs)
+        return serializer._serialize(self, keep_readonly=keep_readonly, **kwargs)  # type: ignore
 
     def as_dict(
         self,
         keep_readonly: bool = True,
         key_transformer: Callable[[str, Dict[str, Any], Any], Any] = attribute_transformer,
         **kwargs: Any
     ) -> JSON:
@@ -386,15 +379,15 @@
         If you want XML serialization, you can pass the kwargs is_xml=True.
 
         :param function key_transformer: A key transformer function.
         :returns: A dict JSON compatible object
         :rtype: dict
         """
         serializer = Serializer(self._infer_class_models())
-        return serializer._serialize(self, key_transformer=key_transformer, keep_readonly=keep_readonly, **kwargs)
+        return serializer._serialize(self, key_transformer=key_transformer, keep_readonly=keep_readonly, **kwargs)  # type: ignore
 
     @classmethod
     def _infer_class_models(cls):
         try:
             str_models = cls.__module__.rsplit(".", 1)[0]
             models = sys.modules[str_models]
             client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
@@ -411,15 +404,15 @@
 
         :param str data: A str using RestAPI structure. JSON by default.
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
-        return deserializer(cls.__name__, data, content_type=content_type)
+        return deserializer(cls.__name__, data, content_type=content_type)  # type: ignore
 
     @classmethod
     def from_dict(
         cls: Type[ModelType],
         data: Any,
         key_extractors: Optional[Callable[[str, Dict[str, Any], Any], Any]] = None,
         content_type: Optional[str] = None,
@@ -441,15 +434,15 @@
                 attribute_key_case_insensitive_extractor,
                 rest_key_case_insensitive_extractor,
                 last_rest_key_case_insensitive_extractor,
             ]
             if key_extractors is None
             else key_extractors
         )
-        return deserializer(cls.__name__, data, content_type=content_type)
+        return deserializer(cls.__name__, data, content_type=content_type)  # type: ignore
 
     @classmethod
     def _flatten_subtype(cls, key, objects):
         if "_subtype_map" not in cls.__dict__:
             return {}
         result = dict(cls._subtype_map[key])
         for valuetype in cls._subtype_map[key].values():
@@ -541,15 +534,15 @@
         "min_items": lambda x, y: len(x) < y,
         "max_items": lambda x, y: len(x) > y,
         "pattern": lambda x, y: not re.match(y, x, re.UNICODE),
         "unique": lambda x, y: len(x) != len(set(x)),
         "multiple": lambda x, y: x % y != 0,
     }
 
-    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
+    def __init__(self, classes: Optional[Mapping[str, type]] = None):
         self.serialize_type = {
             "iso-8601": Serializer.serialize_iso,
             "rfc-1123": Serializer.serialize_rfc,
             "unix-time": Serializer.serialize_unix,
             "duration": Serializer.serialize_duration,
             "date": Serializer.serialize_date,
             "time": Serializer.serialize_time,
@@ -557,15 +550,15 @@
             "long": Serializer.serialize_long,
             "bytearray": Serializer.serialize_bytearray,
             "base64": Serializer.serialize_base64,
             "object": self.serialize_object,
             "[]": self.serialize_iter,
             "{}": self.serialize_dict,
         }
-        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
+        self.dependencies: Dict[str, type] = dict(classes) if classes else {}
         self.key_transformer = full_restapi_key_transformer
         self.client_side_validation = True
 
     def _serialize(self, target_obj, data_type=None, **kwargs):
         """Serialize data into a string according to type.
 
         :param target_obj: The data to be serialized.
@@ -645,15 +638,15 @@
                                     new_attr.tag = "}".join([splitted_tag[0], xml_name])
                                 else:
                                     new_attr.tag = xml_name
                             serialized.append(new_attr)  # type: ignore
                         else:  # That's a basic type
                             # Integrate namespace if necessary
                             local_node = _create_xml_node(xml_name, xml_prefix, xml_ns)
-                            local_node.text = unicode_str(new_attr)
+                            local_node.text = str(new_attr)
                             serialized.append(local_node)  # type: ignore
                     else:  # JSON
                         for k in reversed(keys):  # type: ignore
                             new_attr = {k: new_attr}
 
                         _new_attr = new_attr
                         _serialized = serialized
@@ -664,15 +657,15 @@
                             _serialized = _serialized[k]
                 except ValueError as err:
                     if isinstance(err, SerializationError):
                         raise
 
         except (AttributeError, KeyError, TypeError) as err:
             msg = "Attribute {} in object {} cannot be serialized.\n{}".format(attr_name, class_name, str(target_obj))
-            raise_with_traceback(SerializationError, msg, err)
+            raise SerializationError(msg) from err
         else:
             return serialized
 
     def body(self, data, data_type, **kwargs):
         """Serialize data intended for a request body.
 
         :param data: The data to be serialized.
@@ -706,15 +699,15 @@
                     deserializer.key_extractors = [
                         rest_key_case_insensitive_extractor,
                         attribute_key_case_insensitive_extractor,
                         last_rest_key_case_insensitive_extractor,
                     ]
                 data = deserializer._deserialize(data_type, data)
             except DeserializationError as err:
-                raise_with_traceback(SerializationError, "Unable to build a model: " + str(err), err)
+                raise SerializationError("Unable to build a model: " + str(err)) from err
 
         return self._serialize(data, data_type, **kwargs)
 
     def url(self, name, data, data_type, **kwargs):
         """Serialize data intended for a URL path.
 
         :param data: The data to be serialized.
@@ -726,38 +719,39 @@
         try:
             output = self.serialize_data(data, data_type, **kwargs)
             if data_type == "bool":
                 output = json.dumps(output)
 
             if kwargs.get("skip_quote") is True:
                 output = str(output)
+                output = output.replace("{", quote("{")).replace("}", quote("}"))
             else:
                 output = quote(str(output), safe="")
         except SerializationError:
             raise TypeError("{} must be type {}.".format(name, data_type))
         else:
             return output
 
     def query(self, name, data, data_type, **kwargs):
         """Serialize data intended for a URL query.
 
         :param data: The data to be serialized.
         :param str data_type: The type to be serialized from.
         :keyword bool skip_quote: Whether to skip quote the serialized result.
         Defaults to False.
-        :rtype: str
+        :rtype: str, list
         :raises: TypeError if serialization fails.
         :raises: ValueError if data is None
         """
         try:
             # Treat the list aside, since we don't want to encode the div separator
             if data_type.startswith("["):
                 internal_data_type = data_type[1:-1]
                 do_quote = not kwargs.get("skip_quote", False)
-                return str(self.serialize_iter(data, internal_data_type, do_quote=do_quote, **kwargs))
+                return self.serialize_iter(data, internal_data_type, do_quote=do_quote, **kwargs)
 
             # Not a list, regular serialization
             output = self.serialize_data(data, data_type, **kwargs)
             if data_type == "bool":
                 output = json.dumps(output)
             if kwargs.get("skip_quote") is True:
                 output = str(output)
@@ -800,15 +794,15 @@
         :raises: ValueError if data is None
         :raises: SerializationError if serialization fails.
         """
         if data is None:
             raise ValueError("No value for given attribute")
 
         try:
-            if data is AzureCoreNull:
+            if data is CoreNull:
                 return None
             if data_type in self.basic_types.values():
                 return self.serialize_basic(data, data_type, **kwargs)
 
             elif data_type in self.serialize_type:
                 return self.serialize_type[data_type](data, **kwargs)
 
@@ -820,15 +814,15 @@
 
             iter_type = data_type[0] + data_type[-1]
             if iter_type in self.serialize_type:
                 return self.serialize_type[iter_type](data, data_type[1:-1], **kwargs)
 
         except (ValueError, TypeError) as err:
             msg = "Unable to serialize value: {!r} as type: {!r}."
-            raise_with_traceback(SerializationError, msg.format(data, data_type), err)
+            raise SerializationError(msg.format(data, data_type)) from err
         else:
             return self._serialize(data, **kwargs)
 
     @classmethod
     def _get_custom_serializers(cls, data_type, **kwargs):
         custom_serializer = kwargs.get("basic_types_serializers", {}).get(data_type)
         if custom_serializer:
@@ -989,15 +983,15 @@
         if isinstance(attr, ET.Element):
             return attr
         obj_type = type(attr)
         if obj_type in self.basic_types:
             return self.serialize_basic(attr, self.basic_types[obj_type], **kwargs)
         if obj_type is _long_type:
             return self.serialize_long(attr)
-        if obj_type is unicode_str:
+        if obj_type is str:
             return self.serialize_unicode(attr)
         if obj_type is datetime.datetime:
             return self.serialize_iso(attr)
         if obj_type is datetime.date:
             return self.serialize_date(attr)
         if obj_type is datetime.time:
             return self.serialize_time(attr)
@@ -1166,18 +1160,18 @@
                 microseconds = "." + microseconds
             date = "{:04}-{:02}-{:02}T{:02}:{:02}:{:02}".format(
                 utc.tm_year, utc.tm_mon, utc.tm_mday, utc.tm_hour, utc.tm_min, utc.tm_sec
             )
             return date + microseconds + "Z"
         except (ValueError, OverflowError) as err:
             msg = "Unable to serialize datetime object."
-            raise_with_traceback(SerializationError, msg, err)
+            raise SerializationError(msg) from err
         except AttributeError as err:
             msg = "ISO-8601 object must be valid Datetime object."
-            raise_with_traceback(TypeError, msg, err)
+            raise TypeError(msg) from err
 
     @staticmethod
     def serialize_unix(attr, **kwargs):
         """Serialize Datetime object into IntTime format.
         This is represented as seconds.
 
         :param Datetime attr: Object to be serialized.
@@ -1205,15 +1199,14 @@
             key = _decode_attribute_map_key(dict_keys[0])
             break
         working_key = _decode_attribute_map_key(dict_keys[0])
         working_data = working_data.get(working_key, data)
         if working_data is None:
             # If at any point while following flatten JSON path see None, it means
             # that all properties under are None as well
-            # https://github.com/Azure/msrest-for-python/issues/197
             return None
         key = ".".join(dict_keys[1:])
 
     return working_data.get(key)
 
 
 def rest_key_case_insensitive_extractor(attr, attr_desc, data):
@@ -1226,15 +1219,14 @@
             key = _decode_attribute_map_key(dict_keys[0])
             break
         working_key = _decode_attribute_map_key(dict_keys[0])
         working_data = attribute_key_case_insensitive_extractor(working_key, None, working_data)
         if working_data is None:
             # If at any point while following flatten JSON path see None, it means
             # that all properties under are None as well
-            # https://github.com/Azure/msrest-for-python/issues/197
             return None
         key = ".".join(dict_keys[1:])
 
     if working_data:
         return attribute_key_case_insensitive_extractor(key, None, working_data)
 
 
@@ -1367,15 +1359,15 @@
     :ivar list key_extractors: Ordered list of extractors to be used by this deserializer.
     """
 
     basic_types = {str: "str", int: "int", bool: "bool", float: "float"}
 
     valid_date = re.compile(r"\d{4}[-]\d{2}[-]\d{2}T\d{2}:\d{2}:\d{2}" r"\.?\d*Z?[-+]?[\d{2}]?:?[\d{2}]?")
 
-    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
+    def __init__(self, classes: Optional[Mapping[str, type]] = None):
         self.deserialize_type = {
             "iso-8601": Deserializer.deserialize_iso,
             "rfc-1123": Deserializer.deserialize_rfc,
             "unix-time": Deserializer.deserialize_unix,
             "duration": Deserializer.deserialize_duration,
             "date": Deserializer.deserialize_date,
             "time": Deserializer.deserialize_time,
@@ -1387,15 +1379,15 @@
             "[]": self.deserialize_iter,
             "{}": self.deserialize_dict,
         }
         self.deserialize_expected_types = {
             "duration": (isodate.Duration, datetime.timedelta),
             "iso-8601": (datetime.datetime),
         }
-        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
+        self.dependencies: Dict[str, type] = dict(classes) if classes else {}
         self.key_extractors = [rest_key_extractor, xml_key_extractor]
         # Additional properties only works if the "rest_key_extractor" is used to
         # extract the keys. Making it to work whatever the key extractor is too much
         # complicated, with no real scenario for now.
         # So adding a flag to disable additional properties detection. This flag should be
         # used if your expect the deserialization to NOT come from a JSON REST syntax.
         # Otherwise, result are unexpected
@@ -1440,15 +1432,15 @@
                     setattr(data, attr, self._deserialize(local_type, value))
                 return data
             except AttributeError:
                 return
 
         response, class_name = self._classify_target(target_obj, data)
 
-        if isinstance(response, basestring):
+        if isinstance(response, str):
             return self.deserialize_data(data, response)
         elif isinstance(response, type) and issubclass(response, Enum):
             return self.deserialize_enum(data, response)
 
         if data is None:
             return data
         try:
@@ -1477,15 +1469,15 @@
                             continue
                         raw_value = found_value
 
                 value = self.deserialize_data(raw_value, attr_desc["type"])
                 d_attrs[attr] = value
         except (AttributeError, TypeError, KeyError) as err:
             msg = "Unable to deserialize to object: " + class_name  # type: ignore
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             additional_properties = self._build_additional_properties(attributes, data)
             return self._instantiate_model(response, d_attrs, additional_properties)
 
     def _build_additional_properties(self, attribute_map, data):
         if not self.additional_properties_detection:
             return None
@@ -1511,22 +1503,22 @@
 
         :param str target: The target object type to deserialize to.
         :param str/dict data: The response data to deserialize.
         """
         if target is None:
             return None, None
 
-        if isinstance(target, basestring):
+        if isinstance(target, str):
             try:
                 target = self.dependencies[target]
             except KeyError:
                 return target, target
 
         try:
-            target = target._classify(data, self.dependencies)
+            target = target._classify(data, self.dependencies)  # type: ignore
         except AttributeError:
             pass  # Target is not a Model, no classify
         return target, target.__class__.__name__  # type: ignore
 
     def failsafe_deserialize(self, target_obj, data, content_type=None):
         """Ignores any errors encountered in deserialization,
         and falls back to not deserializing the object. Recommended
@@ -1574,15 +1566,15 @@
         if hasattr(raw_data, "body"):
             return RawDeserializer.deserialize_from_http_generics(raw_data.text(), raw_data.headers)
 
         # Assume this enough to recognize requests.Response without importing it.
         if hasattr(raw_data, "_content_consumed"):
             return RawDeserializer.deserialize_from_http_generics(raw_data.text, raw_data.headers)
 
-        if isinstance(raw_data, (basestring, bytes)) or hasattr(raw_data, "read"):
+        if isinstance(raw_data, (str, bytes)) or hasattr(raw_data, "read"):
             return RawDeserializer.deserialize_from_text(raw_data, content_type)  # type: ignore
         return raw_data
 
     def _instantiate_model(self, response, attrs, additional_properties=None):
         """Instantiate a response model passing in deserialized args.
 
         :param response: The response model class.
@@ -1648,15 +1640,15 @@
                 if isinstance(data, ET.Element):
                     data = data.text
                 return self.deserialize_enum(data, obj_type)
 
         except (ValueError, TypeError, AttributeError) as err:
             msg = "Unable to deserialize response data."
             msg += " Data: {}, {}".format(data, data_type)
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return self._deserialize(obj_type, data)
 
     def deserialize_iter(self, attr, iter_type):
         """Deserialize an iterable.
 
         :param list attr: Iterable to be deserialized.
@@ -1696,15 +1688,15 @@
         :raises: TypeError if non-builtin datatype encountered.
         """
         if attr is None:
             return None
         if isinstance(attr, ET.Element):
             # Do no recurse on XML, just return the tree as-is
             return attr
-        if isinstance(attr, basestring):
+        if isinstance(attr, str):
             return self.deserialize_basic(attr, "str")
         obj_type = type(attr)
         if obj_type in self.basic_types:
             return self.deserialize_basic(attr, self.basic_types[obj_type])
         if obj_type is _long_type:
             return self.deserialize_long(attr)
 
@@ -1753,15 +1745,15 @@
                     # None or '', node <a/> with a strong type is None.
                     # Don't try to model "empty bool" or "empty int"
                     return None
 
         if data_type == "bool":
             if attr in [True, False, 1, 0]:
                 return bool(attr)
-            elif isinstance(attr, basestring):
+            elif isinstance(attr, str):
                 if attr.lower() in ["true", "1"]:
                     return True
                 elif attr.lower() in ["false", "0"]:
                     return False
             raise TypeError("Invalid boolean value: {}".format(attr))
 
         if data_type == "str":
@@ -1804,15 +1796,14 @@
         """
         if isinstance(data, enum_obj) or data is None:
             return data
         if isinstance(data, Enum):
             data = data.value
         if isinstance(data, int):
             # Workaround. We might consider remove it in the future.
-            # https://github.com/Azure/azure-rest-api-specs/issues/141
             try:
                 return list(enum_obj.__members__.values())[data]
             except IndexError:
                 error = "{!r} is not a valid index for enum {!r}"
                 raise DeserializationError(error.format(data, enum_obj))
         try:
             return enum_obj(str(data))
@@ -1858,18 +1849,18 @@
         :param str attr: response string to be deserialized.
         :rtype: Decimal
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            return decimal.Decimal(attr)  # type: ignore
+            return decimal.Decimal(str(attr))  # type: ignore
         except decimal.DecimalException as err:
             msg = "Invalid decimal {}".format(attr)
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
 
     @staticmethod
     def deserialize_long(attr):
         """Deserialize string into long (Py2) or int (Py3).
 
         :param str attr: response string to be deserialized.
         :rtype: long or int
@@ -1889,15 +1880,15 @@
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
             duration = isodate.parse_duration(attr)
         except (ValueError, OverflowError, AttributeError) as err:
             msg = "Cannot deserialize duration object."
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return duration
 
     @staticmethod
     def deserialize_date(attr):
         """Deserialize ISO-8601 formatted string into Date object.
 
@@ -1906,15 +1897,15 @@
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         if re.search(r"[^\W\d_]", attr, re.I + re.U):  # type: ignore
             raise DeserializationError("Date must have only digits and -. Received: %s" % attr)
         # This must NOT use defaultmonth/defaultday. Using None ensure this raises an exception.
-        return isodate.parse_date(attr, defaultmonth=None, defaultday=None)
+        return isodate.parse_date(attr, defaultmonth=0, defaultday=0)
 
     @staticmethod
     def deserialize_time(attr):
         """Deserialize ISO-8601 formatted string into time object.
 
         :param str attr: response string to be deserialized.
         :rtype: datetime.time
@@ -1941,15 +1932,15 @@
             date_obj = datetime.datetime(
                 *parsed_date[:6], tzinfo=_FixedOffset(datetime.timedelta(minutes=(parsed_date[9] or 0) / 60))
             )
             if not date_obj.tzinfo:
                 date_obj = date_obj.astimezone(tz=TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to rfc datetime object."
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return date_obj
 
     @staticmethod
     def deserialize_iso(attr):
         """Deserialize ISO-8601 formatted string into Datetime object.
 
@@ -1978,15 +1969,15 @@
 
             date_obj = isodate.parse_datetime(attr)
             test_utc = date_obj.utctimetuple()
             if test_utc.tm_year > 9999 or test_utc.tm_year < 1:
                 raise OverflowError("Hit max or min date")
         except (ValueError, OverflowError, AttributeError) as err:
             msg = "Cannot deserialize datetime object."
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return date_obj
 
     @staticmethod
     def deserialize_unix(attr):
         """Serialize Datetime object into IntTime format.
         This is represented as seconds.
@@ -1994,13 +1985,14 @@
         :param int attr: Object to be serialized.
         :rtype: Datetime
         :raises: DeserializationError if format invalid
         """
         if isinstance(attr, ET.Element):
             attr = int(attr.text)  # type: ignore
         try:
+            attr = int(attr)
             date_obj = datetime.datetime.fromtimestamp(attr, TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to unix datetime object."
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return date_obj
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/_storage_cache_management_client.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/_storage_cache_management_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, TYPE_CHECKING
 
+from azure.core.pipeline import policies
 from azure.core.rest import HttpRequest, HttpResponse
 from azure.mgmt.core import ARMPipelineClient
+from azure.mgmt.core.policies import ARMAutoResourceProviderRegistrationPolicy
 
 from . import models as _models
 from ._configuration import StorageCacheManagementClientConfiguration
 from ._serialization import Deserializer, Serializer
 from .operations import (
     AmlFilesystemsOperations,
     AscOperationsOperations,
     AscUsagesOperations,
     CachesOperations,
+    ImportJobsOperations,
     Operations,
     SkusOperations,
     StorageCacheManagementClientOperationsMixin,
     StorageTargetOperations,
     StorageTargetsOperations,
     UsageModelsOperations,
 )
@@ -38,14 +41,16 @@
 ):  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
     """Azure Managed Lustre provides a fully managed Lustre® file system, integrated with Blob
     storage, for use on demand. These operations create and manage Azure Managed Lustre file
     systems.
 
     :ivar aml_filesystems: AmlFilesystemsOperations operations
     :vartype aml_filesystems: azure.mgmt.storagecache.operations.AmlFilesystemsOperations
+    :ivar import_jobs: ImportJobsOperations operations
+    :vartype import_jobs: azure.mgmt.storagecache.operations.ImportJobsOperations
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.storagecache.operations.Operations
     :ivar skus: SkusOperations operations
     :vartype skus: azure.mgmt.storagecache.operations.SkusOperations
     :ivar usage_models: UsageModelsOperations operations
     :vartype usage_models: azure.mgmt.storagecache.operations.UsageModelsOperations
     :ivar asc_operations: AscOperationsOperations operations
@@ -60,16 +65,16 @@
     :vartype storage_target: azure.mgmt.storagecache.operations.StorageTargetOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2023-11-01-preview". Note that overriding
-     this default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2024-03-01". Note that overriding this
+     default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
@@ -77,31 +82,50 @@
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = StorageCacheManagementClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        _policies = kwargs.pop("policies", None)
+        if _policies is None:
+            _policies = [
+                policies.RequestIdPolicy(**kwargs),
+                self._config.headers_policy,
+                self._config.user_agent_policy,
+                self._config.proxy_policy,
+                policies.ContentDecodePolicy(**kwargs),
+                ARMAutoResourceProviderRegistrationPolicy(),
+                self._config.redirect_policy,
+                self._config.retry_policy,
+                self._config.authentication_policy,
+                self._config.custom_hook_policy,
+                self._config.logging_policy,
+                policies.DistributedTracingPolicy(**kwargs),
+                policies.SensitiveHeaderCleanupPolicy(**kwargs) if self._config.redirect_policy else None,
+                self._config.http_logging_policy,
+            ]
+        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, policies=_policies, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.aml_filesystems = AmlFilesystemsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.import_jobs = ImportJobsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.skus = SkusOperations(self._client, self._config, self._serialize, self._deserialize)
         self.usage_models = UsageModelsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.asc_operations = AscOperationsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.asc_usages = AscUsagesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.caches = CachesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.storage_targets = StorageTargetsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.storage_target = StorageTargetOperations(self._client, self._config, self._serialize, self._deserialize)
 
-    def _send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
+    def _send_request(self, request: HttpRequest, *, stream: bool = False, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
         >>> response = client._send_request(request)
         <HttpResponse: 200 OK>
@@ -113,15 +137,15 @@
         :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
         :rtype: ~azure.core.rest.HttpResponse
         """
 
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
-        return self._client.send_request(request_copy, **kwargs)
+        return self._client.send_request(request_copy, stream=stream, **kwargs)  # type: ignore
 
     def close(self) -> None:
         self._client.close()
 
     def __enter__(self) -> "StorageCacheManagementClient":
         self._client.__enter__()
         return self
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/_vendor.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/__init__.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/_configuration.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/_configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,63 +4,62 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any, TYPE_CHECKING
 
-from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
-from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
+from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
 
-from .._version import VERSION
+from ._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials_async import AsyncTokenCredential
+    from azure.core.credentials import TokenCredential
 
 
-class StorageCacheManagementClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+class StorageCacheManagementClientConfiguration:  # pylint: disable=too-many-instance-attributes,name-too-long
     """Configuration for StorageCacheManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
+    :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2023-11-01-preview". Note that overriding
-     this default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2024-03-01". Note that overriding this
+     default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        super(StorageCacheManagementClientConfiguration, self).__init__(**kwargs)
-        api_version: str = kwargs.pop("api_version", "2023-11-01-preview")
+    def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
+        api_version: str = kwargs.pop("api_version", "2024-03-01")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
         self.subscription_id = subscription_id
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
         kwargs.setdefault("sdk_moniker", "mgmt-storagecache/{}".format(VERSION))
+        self.polling_interval = kwargs.get("polling_interval", 30)
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
-            self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(
+            self.authentication_policy = ARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/_patch.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/_storage_cache_management_client.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/_storage_cache_management_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, Awaitable, TYPE_CHECKING
 
+from azure.core.pipeline import policies
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 from azure.mgmt.core import AsyncARMPipelineClient
+from azure.mgmt.core.policies import AsyncARMAutoResourceProviderRegistrationPolicy
 
 from .. import models as _models
 from .._serialization import Deserializer, Serializer
 from ._configuration import StorageCacheManagementClientConfiguration
 from .operations import (
     AmlFilesystemsOperations,
     AscOperationsOperations,
     AscUsagesOperations,
     CachesOperations,
+    ImportJobsOperations,
     Operations,
     SkusOperations,
     StorageCacheManagementClientOperationsMixin,
     StorageTargetOperations,
     StorageTargetsOperations,
     UsageModelsOperations,
 )
@@ -38,14 +41,16 @@
 ):  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
     """Azure Managed Lustre provides a fully managed Lustre® file system, integrated with Blob
     storage, for use on demand. These operations create and manage Azure Managed Lustre file
     systems.
 
     :ivar aml_filesystems: AmlFilesystemsOperations operations
     :vartype aml_filesystems: azure.mgmt.storagecache.aio.operations.AmlFilesystemsOperations
+    :ivar import_jobs: ImportJobsOperations operations
+    :vartype import_jobs: azure.mgmt.storagecache.aio.operations.ImportJobsOperations
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.storagecache.aio.operations.Operations
     :ivar skus: SkusOperations operations
     :vartype skus: azure.mgmt.storagecache.aio.operations.SkusOperations
     :ivar usage_models: UsageModelsOperations operations
     :vartype usage_models: azure.mgmt.storagecache.aio.operations.UsageModelsOperations
     :ivar asc_operations: AscOperationsOperations operations
@@ -60,16 +65,16 @@
     :vartype storage_target: azure.mgmt.storagecache.aio.operations.StorageTargetOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2023-11-01-preview". Note that overriding
-     this default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2024-03-01". Note that overriding this
+     default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
@@ -77,31 +82,52 @@
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = StorageCacheManagementClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        _policies = kwargs.pop("policies", None)
+        if _policies is None:
+            _policies = [
+                policies.RequestIdPolicy(**kwargs),
+                self._config.headers_policy,
+                self._config.user_agent_policy,
+                self._config.proxy_policy,
+                policies.ContentDecodePolicy(**kwargs),
+                AsyncARMAutoResourceProviderRegistrationPolicy(),
+                self._config.redirect_policy,
+                self._config.retry_policy,
+                self._config.authentication_policy,
+                self._config.custom_hook_policy,
+                self._config.logging_policy,
+                policies.DistributedTracingPolicy(**kwargs),
+                policies.SensitiveHeaderCleanupPolicy(**kwargs) if self._config.redirect_policy else None,
+                self._config.http_logging_policy,
+            ]
+        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, policies=_policies, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.aml_filesystems = AmlFilesystemsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.import_jobs = ImportJobsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.skus = SkusOperations(self._client, self._config, self._serialize, self._deserialize)
         self.usage_models = UsageModelsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.asc_operations = AscOperationsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.asc_usages = AscUsagesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.caches = CachesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.storage_targets = StorageTargetsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.storage_target = StorageTargetOperations(self._client, self._config, self._serialize, self._deserialize)
 
-    def _send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
+    def _send_request(
+        self, request: HttpRequest, *, stream: bool = False, **kwargs: Any
+    ) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
         >>> response = await client._send_request(request)
         <AsyncHttpResponse: 200 OK>
@@ -113,15 +139,15 @@
         :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
         :rtype: ~azure.core.rest.AsyncHttpResponse
         """
 
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
-        return self._client.send_request(request_copy, **kwargs)
+        return self._client.send_request(request_copy, stream=stream, **kwargs)  # type: ignore
 
     async def close(self) -> None:
         await self._client.close()
 
     async def __aenter__(self) -> "StorageCacheManagementClient":
         await self._client.__aenter__()
         return self
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/_vendor.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/__init__.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._aml_filesystems_operations import AmlFilesystemsOperations
+from ._import_jobs_operations import ImportJobsOperations
 from ._storage_cache_management_client_operations import StorageCacheManagementClientOperationsMixin
 from ._operations import Operations
 from ._skus_operations import SkusOperations
 from ._usage_models_operations import UsageModelsOperations
 from ._asc_operations_operations import AscOperationsOperations
 from ._asc_usages_operations import AscUsagesOperations
 from ._caches_operations import CachesOperations
@@ -19,14 +20,15 @@
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "AmlFilesystemsOperations",
+    "ImportJobsOperations",
     "StorageCacheManagementClientOperationsMixin",
     "Operations",
     "SkusOperations",
     "UsageModelsOperations",
     "AscOperationsOperations",
     "AscUsagesOperations",
     "CachesOperations",
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/_aml_filesystems_operations.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/_storage_targets_operations.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -27,217 +27,251 @@
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._aml_filesystems_operations import (
-    build_archive_request,
-    build_cancel_archive_request,
+from ...operations._storage_targets_operations import (
     build_create_or_update_request,
     build_delete_request,
+    build_dns_refresh_request,
     build_get_request,
-    build_list_by_resource_group_request,
-    build_list_request,
-    build_update_request,
+    build_list_by_cache_request,
+    build_restore_defaults_request,
 )
 from .._vendor import StorageCacheManagementClientMixinABC
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class AmlFilesystemsOperations:
+class StorageTargetsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.storagecache.aio.StorageCacheManagementClient`'s
-        :attr:`aml_filesystems` attribute.
+        :attr:`storage_targets` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    @distributed_trace
-    def list(self, **kwargs: Any) -> AsyncIterable["_models.AmlFilesystem"]:
-        """Returns all AML file systems the user has access to under a subscription.
-
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either AmlFilesystem or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.storagecache.models.AmlFilesystem]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.AmlFilesystemsListResult] = kwargs.pop("cls", None)
-
+    async def _dns_refresh_initial(  # pylint: disable=inconsistent-return-statements
+        self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
+    ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        def prepare_request(next_link=None):
-            if not next_link:
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-                request = build_list_request(
-                    subscription_id=self._config.subscription_id,
-                    api_version=api_version,
-                    template_url=self.list.metadata["url"],
-                    headers=_headers,
-                    params=_params,
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
-            else:
-                # make call to next link with the client's api-version
-                _parsed_next_link = urllib.parse.urlparse(next_link)
-                _next_request_params = case_insensitive_dict(
-                    {
-                        key: [urllib.parse.quote(v) for v in value]
-                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
-                    }
-                )
-                _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
-                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+        _request = build_dns_refresh_request(
+            resource_group_name=resource_group_name,
+            cache_name=cache_name,
+            storage_target_name=storage_target_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            headers=_headers,
+            params=_params,
+        )
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
-        async def extract_data(pipeline_response):
-            deserialized = self._deserialize("AmlFilesystemsListResult", pipeline_response)
-            list_of_elem = deserialized.value
-            if cls:
-                list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, AsyncList(list_of_elem)
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
 
-        async def get_next(next_link=None):
-            request = prepare_request(next_link)
+        response = pipeline_response.http_response
 
-            _stream = False
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
             )
-            response = pipeline_response.http_response
 
-            if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
-                raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+        if cls:
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
-            return pipeline_response
+    @distributed_trace_async
+    async def begin_dns_refresh(
+        self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
+    ) -> AsyncLROPoller[None]:
+        """Tells a storage target to refresh its DNS information.
 
-        return AsyncItemPaged(get_next, extract_data)
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
+         from the [-0-9a-zA-Z_] char class. Required.
+        :type cache_name: str
+        :param storage_target_name: Name of Storage Target. Required.
+        :type storage_target_name: str
+        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[None]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = await self._dns_refresh_initial(  # type: ignore
+                resource_group_name=resource_group_name,
+                cache_name=cache_name,
+                storage_target_name=storage_target_name,
+                api_version=api_version,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/amlFilesystems"}
+        def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
+            if cls:
+                return cls(pipeline_response, None, {})  # type: ignore
+
+        if polling is True:
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod,
+                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
+            )
+        elif polling is False:
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return AsyncLROPoller[None].from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     @distributed_trace
-    def list_by_resource_group(self, resource_group_name: str, **kwargs: Any) -> AsyncIterable["_models.AmlFilesystem"]:
-        """Returns all AML file systems the user has access to under a resource group.
+    def list_by_cache(
+        self, resource_group_name: str, cache_name: str, **kwargs: Any
+    ) -> AsyncIterable["_models.StorageTarget"]:
+        """Returns a list of Storage Targets for the specified cache.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either AmlFilesystem or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.storagecache.models.AmlFilesystem]
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
+         from the [-0-9a-zA-Z_] char class. Required.
+        :type cache_name: str
+        :return: An iterator like instance of either StorageTarget or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.storagecache.models.StorageTarget]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.AmlFilesystemsListResult] = kwargs.pop("cls", None)
+        cls: ClsType[_models.StorageTargetsResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_resource_group_request(
+                _request = build_list_by_cache_request(
                     resource_group_name=resource_group_name,
+                    cache_name=cache_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_resource_group.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize("AmlFilesystemsListResult", pipeline_response)
+            deserialized = self._deserialize("StorageTargetsResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_resource_group.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems"
-    }
-
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, aml_filesystem_name: str, **kwargs: Any
+        self,
+        resource_group_name: str,
+        cache_name: str,
+        storage_target_name: str,
+        force: Optional[str] = None,
+        **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -245,29 +279,30 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
-            aml_filesystem_name=aml_filesystem_name,
+            cache_name=cache_name,
+            storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
+            force=force,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -276,40 +311,42 @@
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
-        self, resource_group_name: str, aml_filesystem_name: str, **kwargs: Any
+        self,
+        resource_group_name: str,
+        cache_name: str,
+        storage_target_name: str,
+        force: Optional[str] = None,
+        **kwargs: Any
     ) -> AsyncLROPoller[None]:
-        """Schedules an AML file system for deletion.
+        """Removes a Storage Target from a cache. This operation is allowed at any time, but if the cache
+        is down or unhealthy, the actual removal of the Storage Target may be delayed until the cache
+        is healthy again. Note that if the cache has data to flush to the Storage Target, the data will
+        be flushed before the Storage Target will be deleted.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
-         and hyphens. Start and end with alphanumeric. Required.
-        :type aml_filesystem_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
+         from the [-0-9a-zA-Z_] char class. Required.
+        :type cache_name: str
+        :param storage_target_name: Name of Storage Target. Required.
+        :type storage_target_name: str
+        :param force: Boolean value requesting the force delete operation for a storage target. Force
+         delete discards unwritten-data in the cache instead of flushing it to back-end storage. Default
+         value is None.
+        :type force: str
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -317,790 +354,421 @@
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
-                aml_filesystem_name=aml_filesystem_name,
+                cache_name=cache_name,
+                storage_target_name=storage_target_name,
+                force=force,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(
-                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
-            )
+            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     @distributed_trace_async
-    async def get(self, resource_group_name: str, aml_filesystem_name: str, **kwargs: Any) -> _models.AmlFilesystem:
-        """Returns an AML file system.
+    async def get(
+        self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
+    ) -> _models.StorageTarget:
+        """Returns a Storage Target from a cache.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
-         and hyphens. Start and end with alphanumeric. Required.
-        :type aml_filesystem_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: AmlFilesystem or the result of cls(response)
-        :rtype: ~azure.mgmt.storagecache.models.AmlFilesystem
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
+         from the [-0-9a-zA-Z_] char class. Required.
+        :type cache_name: str
+        :param storage_target_name: Name of Storage Target. Required.
+        :type storage_target_name: str
+        :return: StorageTarget or the result of cls(response)
+        :rtype: ~azure.mgmt.storagecache.models.StorageTarget
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.AmlFilesystem] = kwargs.pop("cls", None)
+        cls: ClsType[_models.StorageTarget] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
-            aml_filesystem_name=aml_filesystem_name,
+            cache_name=cache_name,
+            storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("AmlFilesystem", pipeline_response)
+        deserialized = self._deserialize("StorageTarget", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}"
-    }
+        return deserialized  # type: ignore
 
     async def _create_or_update_initial(
         self,
         resource_group_name: str,
-        aml_filesystem_name: str,
-        aml_filesystem: Union[_models.AmlFilesystem, IO],
+        cache_name: str,
+        storage_target_name: str,
+        storagetarget: Union[_models.StorageTarget, IO[bytes]],
         **kwargs: Any
-    ) -> _models.AmlFilesystem:
+    ) -> Optional[_models.StorageTarget]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.AmlFilesystem] = kwargs.pop("cls", None)
+        cls: ClsType[Optional[_models.StorageTarget]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(aml_filesystem, (IOBase, bytes)):
-            _content = aml_filesystem
+        if isinstance(storagetarget, (IOBase, bytes)):
+            _content = storagetarget
         else:
-            _json = self._serialize.body(aml_filesystem, "AmlFilesystem")
+            _json = self._serialize.body(storagetarget, "StorageTarget")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
-            aml_filesystem_name=aml_filesystem_name,
+            cache_name=cache_name,
+            storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 201]:
+        if response.status_code not in [200, 201, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
-        response_headers = {}
+        deserialized = None
         if response.status_code == 200:
-            deserialized = self._deserialize("AmlFilesystem", pipeline_response)
+            deserialized = self._deserialize("StorageTarget", pipeline_response)
 
         if response.status_code == 201:
-            response_headers["azure-async-operation"] = self._deserialize(
-                "str", response.headers.get("azure-async-operation")
-            )
-
-            deserialized = self._deserialize("AmlFilesystem", pipeline_response)
+            deserialized = self._deserialize("StorageTarget", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}"
-    }
-
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
-        aml_filesystem_name: str,
-        aml_filesystem: _models.AmlFilesystem,
+        cache_name: str,
+        storage_target_name: str,
+        storagetarget: _models.StorageTarget,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.AmlFilesystem]:
-        """Create or update an AML file system.
+    ) -> AsyncLROPoller[_models.StorageTarget]:
+        """Create or update a Storage Target. This operation is allowed at any time, but if the cache is
+        down or unhealthy, the actual creation/modification of the Storage Target may be delayed until
+        the cache is healthy again.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
-         and hyphens. Start and end with alphanumeric. Required.
-        :type aml_filesystem_name: str
-        :param aml_filesystem: Object containing the user-selectable properties of the AML file system.
-         If read-only properties are included, they must match the existing values of those properties.
-         Required.
-        :type aml_filesystem: ~azure.mgmt.storagecache.models.AmlFilesystem
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
+         from the [-0-9a-zA-Z_] char class. Required.
+        :type cache_name: str
+        :param storage_target_name: Name of Storage Target. Required.
+        :type storage_target_name: str
+        :param storagetarget: Object containing the definition of a Storage Target. Required.
+        :type storagetarget: ~azure.mgmt.storagecache.models.StorageTarget
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either AmlFilesystem or the result of
+        :return: An instance of AsyncLROPoller that returns either StorageTarget or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.AmlFilesystem]
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.StorageTarget]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
-        aml_filesystem_name: str,
-        aml_filesystem: IO,
+        cache_name: str,
+        storage_target_name: str,
+        storagetarget: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.AmlFilesystem]:
-        """Create or update an AML file system.
+    ) -> AsyncLROPoller[_models.StorageTarget]:
+        """Create or update a Storage Target. This operation is allowed at any time, but if the cache is
+        down or unhealthy, the actual creation/modification of the Storage Target may be delayed until
+        the cache is healthy again.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
-         and hyphens. Start and end with alphanumeric. Required.
-        :type aml_filesystem_name: str
-        :param aml_filesystem: Object containing the user-selectable properties of the AML file system.
-         If read-only properties are included, they must match the existing values of those properties.
-         Required.
-        :type aml_filesystem: IO
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
+         from the [-0-9a-zA-Z_] char class. Required.
+        :type cache_name: str
+        :param storage_target_name: Name of Storage Target. Required.
+        :type storage_target_name: str
+        :param storagetarget: Object containing the definition of a Storage Target. Required.
+        :type storagetarget: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either AmlFilesystem or the result of
+        :return: An instance of AsyncLROPoller that returns either StorageTarget or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.AmlFilesystem]
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.StorageTarget]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self,
         resource_group_name: str,
-        aml_filesystem_name: str,
-        aml_filesystem: Union[_models.AmlFilesystem, IO],
-        **kwargs: Any
-    ) -> AsyncLROPoller[_models.AmlFilesystem]:
-        """Create or update an AML file system.
+        cache_name: str,
+        storage_target_name: str,
+        storagetarget: Union[_models.StorageTarget, IO[bytes]],
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.StorageTarget]:
+        """Create or update a Storage Target. This operation is allowed at any time, but if the cache is
+        down or unhealthy, the actual creation/modification of the Storage Target may be delayed until
+        the cache is healthy again.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
-         and hyphens. Start and end with alphanumeric. Required.
-        :type aml_filesystem_name: str
-        :param aml_filesystem: Object containing the user-selectable properties of the AML file system.
-         If read-only properties are included, they must match the existing values of those properties.
-         Is either a AmlFilesystem type or a IO type. Required.
-        :type aml_filesystem: ~azure.mgmt.storagecache.models.AmlFilesystem or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either AmlFilesystem or the result of
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
+         from the [-0-9a-zA-Z_] char class. Required.
+        :type cache_name: str
+        :param storage_target_name: Name of Storage Target. Required.
+        :type storage_target_name: str
+        :param storagetarget: Object containing the definition of a Storage Target. Is either a
+         StorageTarget type or a IO[bytes] type. Required.
+        :type storagetarget: ~azure.mgmt.storagecache.models.StorageTarget or IO[bytes]
+        :return: An instance of AsyncLROPoller that returns either StorageTarget or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.AmlFilesystem]
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.StorageTarget]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.AmlFilesystem] = kwargs.pop("cls", None)
+        cls: ClsType[_models.StorageTarget] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
                 resource_group_name=resource_group_name,
-                aml_filesystem_name=aml_filesystem_name,
-                aml_filesystem=aml_filesystem,
+                cache_name=cache_name,
+                storage_target_name=storage_target_name,
+                storagetarget=storagetarget,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("AmlFilesystem", pipeline_response)
+            deserialized = self._deserialize("StorageTarget", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(
-                AsyncPollingMethod,
-                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
-            )
+            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.StorageTarget].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}"
-    }
+        return AsyncLROPoller[_models.StorageTarget](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
-    async def _update_initial(
-        self,
-        resource_group_name: str,
-        aml_filesystem_name: str,
-        aml_filesystem: Union[_models.AmlFilesystemUpdate, IO],
-        **kwargs: Any
-    ) -> Optional[_models.AmlFilesystem]:
+    async def _restore_defaults_initial(  # pylint: disable=inconsistent-return-statements
+        self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
+    ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[Optional[_models.AmlFilesystem]] = kwargs.pop("cls", None)
-
-        content_type = content_type or "application/json"
-        _json = None
-        _content = None
-        if isinstance(aml_filesystem, (IOBase, bytes)):
-            _content = aml_filesystem
-        else:
-            _json = self._serialize.body(aml_filesystem, "AmlFilesystemUpdate")
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_update_request(
+        _request = build_restore_defaults_request(
             resource_group_name=resource_group_name,
-            aml_filesystem_name=aml_filesystem_name,
+            cache_name=cache_name,
+            storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            content_type=content_type,
-            json=_json,
-            content=_content,
-            template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
-        deserialized = None
         response_headers = {}
-        if response.status_code == 200:
-            deserialized = self._deserialize("AmlFilesystem", pipeline_response)
-
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
-            response_headers["azure-async-operation"] = self._deserialize(
-                "str", response.headers.get("azure-async-operation")
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)
-
-        return deserialized
-
-    _update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}"
-    }
-
-    @overload
-    async def begin_update(
-        self,
-        resource_group_name: str,
-        aml_filesystem_name: str,
-        aml_filesystem: _models.AmlFilesystemUpdate,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> AsyncLROPoller[_models.AmlFilesystem]:
-        """Update an AML file system instance.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
-         and hyphens. Start and end with alphanumeric. Required.
-        :type aml_filesystem_name: str
-        :param aml_filesystem: Object containing the user-selectable properties of the AML file system.
-         If read-only properties are included, they must match the existing values of those properties.
-         Required.
-        :type aml_filesystem: ~azure.mgmt.storagecache.models.AmlFilesystemUpdate
-        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either AmlFilesystem or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.AmlFilesystem]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-
-    @overload
-    async def begin_update(
-        self,
-        resource_group_name: str,
-        aml_filesystem_name: str,
-        aml_filesystem: IO,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> AsyncLROPoller[_models.AmlFilesystem]:
-        """Update an AML file system instance.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
-         and hyphens. Start and end with alphanumeric. Required.
-        :type aml_filesystem_name: str
-        :param aml_filesystem: Object containing the user-selectable properties of the AML file system.
-         If read-only properties are included, they must match the existing values of those properties.
-         Required.
-        :type aml_filesystem: IO
-        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either AmlFilesystem or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.AmlFilesystem]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
-    async def begin_update(
-        self,
-        resource_group_name: str,
-        aml_filesystem_name: str,
-        aml_filesystem: Union[_models.AmlFilesystemUpdate, IO],
-        **kwargs: Any
-    ) -> AsyncLROPoller[_models.AmlFilesystem]:
-        """Update an AML file system instance.
+    async def begin_restore_defaults(
+        self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
+    ) -> AsyncLROPoller[None]:
+        """Tells a storage target to restore its settings to their default values.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
-         and hyphens. Start and end with alphanumeric. Required.
-        :type aml_filesystem_name: str
-        :param aml_filesystem: Object containing the user-selectable properties of the AML file system.
-         If read-only properties are included, they must match the existing values of those properties.
-         Is either a AmlFilesystemUpdate type or a IO type. Required.
-        :type aml_filesystem: ~azure.mgmt.storagecache.models.AmlFilesystemUpdate or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either AmlFilesystem or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.AmlFilesystem]
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
+         from the [-0-9a-zA-Z_] char class. Required.
+        :type cache_name: str
+        :param storage_target_name: Name of Storage Target. Required.
+        :type storage_target_name: str
+        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.AmlFilesystem] = kwargs.pop("cls", None)
+        cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._update_initial(
+            raw_result = await self._restore_defaults_initial(  # type: ignore
                 resource_group_name=resource_group_name,
-                aml_filesystem_name=aml_filesystem_name,
-                aml_filesystem=aml_filesystem,
+                cache_name=cache_name,
+                storage_target_name=storage_target_name,
                 api_version=api_version,
-                content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
-        def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("AmlFilesystem", pipeline_response)
+        def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, deserialized, {})
-            return deserialized
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
-                AsyncPollingMethod,
-                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
             )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}"
-    }
-
-    @overload
-    async def archive(  # pylint: disable=inconsistent-return-statements
-        self,
-        resource_group_name: str,
-        aml_filesystem_name: str,
-        archive_info: Optional[_models.AmlFilesystemArchiveInfo] = None,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> None:
-        """Archive data from the AML file system.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
-         and hyphens. Start and end with alphanumeric. Required.
-        :type aml_filesystem_name: str
-        :param archive_info: Information about the archive operation. Default value is None.
-        :type archive_info: ~azure.mgmt.storagecache.models.AmlFilesystemArchiveInfo
-        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: None or the result of cls(response)
-        :rtype: None
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-
-    @overload
-    async def archive(  # pylint: disable=inconsistent-return-statements
-        self,
-        resource_group_name: str,
-        aml_filesystem_name: str,
-        archive_info: Optional[IO] = None,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> None:
-        """Archive data from the AML file system.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
-         and hyphens. Start and end with alphanumeric. Required.
-        :type aml_filesystem_name: str
-        :param archive_info: Information about the archive operation. Default value is None.
-        :type archive_info: IO
-        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: None or the result of cls(response)
-        :rtype: None
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-
-    @distributed_trace_async
-    async def archive(  # pylint: disable=inconsistent-return-statements
-        self,
-        resource_group_name: str,
-        aml_filesystem_name: str,
-        archive_info: Optional[Union[_models.AmlFilesystemArchiveInfo, IO]] = None,
-        **kwargs: Any
-    ) -> None:
-        """Archive data from the AML file system.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
-         and hyphens. Start and end with alphanumeric. Required.
-        :type aml_filesystem_name: str
-        :param archive_info: Information about the archive operation. Is either a
-         AmlFilesystemArchiveInfo type or a IO type. Default value is None.
-        :type archive_info: ~azure.mgmt.storagecache.models.AmlFilesystemArchiveInfo or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: None or the result of cls(response)
-        :rtype: None
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[None] = kwargs.pop("cls", None)
-
-        content_type = content_type or "application/json"
-        _json = None
-        _content = None
-        if isinstance(archive_info, (IOBase, bytes)):
-            _content = archive_info
-        else:
-            if archive_info is not None:
-                _json = self._serialize.body(archive_info, "AmlFilesystemArchiveInfo")
-            else:
-                _json = None
-
-        request = build_archive_request(
-            resource_group_name=resource_group_name,
-            aml_filesystem_name=aml_filesystem_name,
-            subscription_id=self._config.subscription_id,
-            api_version=api_version,
-            content_type=content_type,
-            json=_json,
-            content=_content,
-            template_url=self.archive.metadata["url"],
-            headers=_headers,
-            params=_params,
-        )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
-
-        _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
-
-        if cls:
-            return cls(pipeline_response, None, {})
-
-    archive.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}/archive"
-    }
-
-    @distributed_trace_async
-    async def cancel_archive(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, aml_filesystem_name: str, **kwargs: Any
-    ) -> None:
-        """Cancel archiving data from the AML file system.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
-         and hyphens. Start and end with alphanumeric. Required.
-        :type aml_filesystem_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: None or the result of cls(response)
-        :rtype: None
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[None] = kwargs.pop("cls", None)
-
-        request = build_cancel_archive_request(
-            resource_group_name=resource_group_name,
-            aml_filesystem_name=aml_filesystem_name,
-            subscription_id=self._config.subscription_id,
-            api_version=api_version,
-            template_url=self.cancel_archive.metadata["url"],
-            headers=_headers,
-            params=_params,
-        )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
-
-        _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
-
-        if cls:
-            return cls(pipeline_response, None, {})
-
-    cancel_archive.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}/cancelArchive"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/_asc_operations_operations.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/_asc_operations_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -55,15 +55,14 @@
     async def get(self, location: str, operation_id: str, **kwargs: Any) -> _models.AscOperation:
         """Gets the status of an asynchronous operation for the Azure HPC Cache.
 
         :param location: The name of Azure region. Required.
         :type location: str
         :param operation_id: The ID of an ongoing async operation. Required.
         :type operation_id: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: AscOperation or the result of cls(response)
         :rtype: ~azure.mgmt.storagecache.models.AscOperation
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -74,40 +73,35 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AscOperation] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             location=location,
             operation_id=operation_id,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("AscOperation", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/locations/{location}/ascOperations/{operationId}"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/_asc_usages_operations.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/_asc_usages_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -55,15 +55,14 @@
 
     @distributed_trace
     def list(self, location: str, **kwargs: Any) -> AsyncIterable["_models.ResourceUsage"]:
         """Gets the quantity used and quota limit for resources.
 
         :param location: The name of the region to query for usage information. Required.
         :type location: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ResourceUsage or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.storagecache.models.ResourceUsage]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -77,63 +76,58 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     location=location,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ResourceUsagesListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/locations/{location}/usages"
-    }
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/_caches_operations.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/_caches_operations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -74,15 +74,14 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, **kwargs: Any) -> AsyncIterable["_models.Cache"]:
         """Returns all caches the user has access to under a subscription.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Cache or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.storagecache.models.Cache]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -96,76 +95,72 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("CachesListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/caches"}
-
     @distributed_trace
     def list_by_resource_group(self, resource_group_name: str, **kwargs: Any) -> AsyncIterable["_models.Cache"]:
         """Returns all caches the user has access to under a resource group.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Cache or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.storagecache.models.Cache]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -179,71 +174,66 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_resource_group_request(
+                _request = build_list_by_resource_group_request(
                     resource_group_name=resource_group_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_resource_group.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("CachesListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_resource_group.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches"
-    }
-
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, cache_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -253,29 +243,28 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -284,38 +273,26 @@
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(self, resource_group_name: str, cache_name: str, **kwargs: Any) -> AsyncLROPoller[None]:
         """Schedules a cache for deletion.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -334,46 +311,41 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     @distributed_trace_async
     async def get(self, resource_group_name: str, cache_name: str, **kwargs: Any) -> _models.Cache:
         """Returns a cache.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Cache or the result of cls(response)
         :rtype: ~azure.mgmt.storagecache.models.Cache
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -384,50 +356,45 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Cache] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("Cache", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}"
-    }
+        return deserialized  # type: ignore
 
     async def _create_or_update_initial(
-        self, resource_group_name: str, cache_name: str, cache: Union[_models.Cache, IO], **kwargs: Any
+        self, resource_group_name: str, cache_name: str, cache: Union[_models.Cache, IO[bytes]], **kwargs: Any
     ) -> Optional[_models.Cache]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -444,32 +411,31 @@
         _json = None
         _content = None
         if isinstance(cache, (IOBase, bytes)):
             _content = cache
         else:
             _json = self._serialize.body(cache, "Cache")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -478,21 +444,17 @@
         if response.status_code == 200:
             deserialized = self._deserialize("Cache", pipeline_response)
 
         if response.status_code == 201:
             deserialized = self._deserialize("Cache", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         cache_name: str,
         cache: _models.Cache,
@@ -510,91 +472,64 @@
         :type cache_name: str
         :param cache: Object containing the user-selectable properties of the new cache. If read-only
          properties are included, they must match the existing values of those properties. Required.
         :type cache: ~azure.mgmt.storagecache.models.Cache
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either Cache or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.Cache]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         cache_name: str,
-        cache: IO,
+        cache: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.Cache]:
         """Create or update a cache.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param cache: Object containing the user-selectable properties of the new cache. If read-only
          properties are included, they must match the existing values of those properties. Required.
-        :type cache: IO
+        :type cache: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either Cache or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.Cache]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
-        self, resource_group_name: str, cache_name: str, cache: Union[_models.Cache, IO], **kwargs: Any
+        self, resource_group_name: str, cache_name: str, cache: Union[_models.Cache, IO[bytes]], **kwargs: Any
     ) -> AsyncLROPoller[_models.Cache]:
         """Create or update a cache.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param cache: Object containing the user-selectable properties of the new cache. If read-only
          properties are included, they must match the existing values of those properties. Is either a
-         Cache type or a IO type. Required.
-        :type cache: ~azure.mgmt.storagecache.models.Cache or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         Cache type or a IO[bytes] type. Required.
+        :type cache: ~azure.mgmt.storagecache.models.Cache or IO[bytes]
         :return: An instance of AsyncLROPoller that returns either Cache or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.Cache]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -617,38 +552,40 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("Cache", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.Cache].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}"
-    }
+        return AsyncLROPoller[_models.Cache](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     async def _update_initial(
-        self, resource_group_name: str, cache_name: str, cache: Optional[Union[_models.Cache, IO]] = None, **kwargs: Any
+        self,
+        resource_group_name: str,
+        cache_name: str,
+        cache: Optional[Union[_models.Cache, IO[bytes]]] = None,
+        **kwargs: Any
     ) -> Optional[_models.Cache]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -668,32 +605,31 @@
             _content = cache
         else:
             if cache is not None:
                 _json = self._serialize.body(cache, "Cache")
             else:
                 _json = None
 
-        request = build_update_request(
+        _request = build_update_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -706,21 +642,17 @@
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
-        return deserialized
-
-    _update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     async def begin_update(
         self,
         resource_group_name: str,
         cache_name: str,
         cache: Optional[_models.Cache] = None,
@@ -739,33 +671,25 @@
         :param cache: Object containing the user-selectable properties of the cache. If read-only
          properties are included, they must match the existing values of those properties. Default value
          is None.
         :type cache: ~azure.mgmt.storagecache.models.Cache
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either Cache or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.Cache]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_update(
         self,
         resource_group_name: str,
         cache_name: str,
-        cache: Optional[IO] = None,
+        cache: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.Cache]:
         """Update a cache instance.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
@@ -773,58 +697,43 @@
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param cache: Object containing the user-selectable properties of the cache. If read-only
          properties are included, they must match the existing values of those properties. Default value
          is None.
-        :type cache: IO
+        :type cache: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either Cache or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.Cache]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_update(
-        self, resource_group_name: str, cache_name: str, cache: Optional[Union[_models.Cache, IO]] = None, **kwargs: Any
+        self,
+        resource_group_name: str,
+        cache_name: str,
+        cache: Optional[Union[_models.Cache, IO[bytes]]] = None,
+        **kwargs: Any
     ) -> AsyncLROPoller[_models.Cache]:
         """Update a cache instance.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param cache: Object containing the user-selectable properties of the cache. If read-only
          properties are included, they must match the existing values of those properties. Is either a
-         Cache type or a IO type. Default value is None.
-        :type cache: ~azure.mgmt.storagecache.models.Cache or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         Cache type or a IO[bytes] type. Default value is None.
+        :type cache: ~azure.mgmt.storagecache.models.Cache or IO[bytes]
         :return: An instance of AsyncLROPoller that returns either Cache or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.Cache]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -847,38 +756,36 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("Cache", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod,
                 AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
             )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.Cache].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}"
-    }
+        return AsyncLROPoller[_models.Cache](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     async def _debug_info_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, cache_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -889,29 +796,28 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_debug_info_request(
+        _request = build_debug_info_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._debug_info_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -920,38 +826,26 @@
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _debug_info_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/debugInfo"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_debug_info(self, resource_group_name: str, cache_name: str, **kwargs: Any) -> AsyncLROPoller[None]:
         """Tells a cache to write generate debug info for support to process.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -970,37 +864,33 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod,
                 AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
             )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_debug_info.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/debugInfo"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     async def _flush_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, cache_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -1011,29 +901,28 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_flush_request(
+        _request = build_flush_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._flush_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1042,39 +931,27 @@
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _flush_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/flush"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_flush(self, resource_group_name: str, cache_name: str, **kwargs: Any) -> AsyncLROPoller[None]:
         """Tells a cache to write all dirty data to the Storage Target(s). During the flush, clients will
         see errors returned until the flush is complete.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -1093,37 +970,33 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod,
                 AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
             )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_flush.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/flush"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     async def _start_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, cache_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -1134,29 +1007,28 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_start_request(
+        _request = build_start_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._start_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1165,38 +1037,26 @@
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _start_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/start"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_start(self, resource_group_name: str, cache_name: str, **kwargs: Any) -> AsyncLROPoller[None]:
         """Tells a Stopped state cache to transition to Active state.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -1215,37 +1075,33 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod,
                 AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
             )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_start.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/start"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     async def _stop_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, cache_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -1256,29 +1112,28 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_stop_request(
+        _request = build_stop_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._stop_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1287,38 +1142,26 @@
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _stop_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/stop"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_stop(self, resource_group_name: str, cache_name: str, **kwargs: Any) -> AsyncLROPoller[None]:
         """Tells an Active cache to transition to Stopped state.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -1337,43 +1180,39 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod,
                 AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
             )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_stop.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/stop"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     async def _start_priming_job_initial(  # pylint: disable=inconsistent-return-statements
         self,
         resource_group_name: str,
         cache_name: str,
-        primingjob: Optional[Union[_models.PrimingJob, IO]] = None,
+        primingjob: Optional[Union[_models.PrimingJob, IO[bytes]]] = None,
         **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1394,32 +1233,31 @@
             _content = primingjob
         else:
             if primingjob is not None:
                 _json = self._serialize.body(primingjob, "PrimingJob")
             else:
                 _json = None
 
-        request = build_start_priming_job_request(
+        _request = build_start_priming_job_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._start_priming_job_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1427,19 +1265,15 @@
         response_headers = {}
         response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
         response_headers["Azure-AsyncOperation"] = self._deserialize(
             "str", response.headers.get("Azure-AsyncOperation")
         )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _start_priming_job_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/startPrimingJob"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @overload
     async def begin_start_priming_job(
         self,
         resource_group_name: str,
         cache_name: str,
         primingjob: Optional[_models.PrimingJob] = None,
@@ -1456,93 +1290,66 @@
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param primingjob: Object containing the definition of a priming job. Default value is None.
         :type primingjob: ~azure.mgmt.storagecache.models.PrimingJob
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_start_priming_job(
         self,
         resource_group_name: str,
         cache_name: str,
-        primingjob: Optional[IO] = None,
+        primingjob: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Create a priming job. This operation is only allowed when the cache is healthy.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param primingjob: Object containing the definition of a priming job. Default value is None.
-        :type primingjob: IO
+        :type primingjob: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_start_priming_job(
         self,
         resource_group_name: str,
         cache_name: str,
-        primingjob: Optional[Union[_models.PrimingJob, IO]] = None,
+        primingjob: Optional[Union[_models.PrimingJob, IO[bytes]]] = None,
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Create a priming job. This operation is only allowed when the cache is healthy.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param primingjob: Object containing the definition of a priming job. Is either a PrimingJob
-         type or a IO type. Default value is None.
-        :type primingjob: ~azure.mgmt.storagecache.models.PrimingJob or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         type or a IO[bytes] type. Default value is None.
+        :type primingjob: ~azure.mgmt.storagecache.models.PrimingJob or IO[bytes]
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -1564,43 +1371,39 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod,
                 AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
             )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_start_priming_job.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/startPrimingJob"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     async def _stop_priming_job_initial(  # pylint: disable=inconsistent-return-statements
         self,
         resource_group_name: str,
         cache_name: str,
-        priming_job_id: Optional[Union[_models.PrimingJobIdParameter, IO]] = None,
+        priming_job_id: Optional[Union[_models.PrimingJobIdParameter, IO[bytes]]] = None,
         **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1621,32 +1424,31 @@
             _content = priming_job_id
         else:
             if priming_job_id is not None:
                 _json = self._serialize.body(priming_job_id, "PrimingJobIdParameter")
             else:
                 _json = None
 
-        request = build_stop_priming_job_request(
+        _request = build_stop_priming_job_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._stop_priming_job_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1655,19 +1457,15 @@
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _stop_priming_job_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/stopPrimingJob"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @overload
     async def begin_stop_priming_job(
         self,
         resource_group_name: str,
         cache_name: str,
         priming_job_id: Optional[_models.PrimingJobIdParameter] = None,
@@ -1684,93 +1482,66 @@
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param priming_job_id: Object containing the priming job ID. Default value is None.
         :type priming_job_id: ~azure.mgmt.storagecache.models.PrimingJobIdParameter
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_stop_priming_job(
         self,
         resource_group_name: str,
         cache_name: str,
-        priming_job_id: Optional[IO] = None,
+        priming_job_id: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Schedule a priming job for deletion.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param priming_job_id: Object containing the priming job ID. Default value is None.
-        :type priming_job_id: IO
+        :type priming_job_id: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_stop_priming_job(
         self,
         resource_group_name: str,
         cache_name: str,
-        priming_job_id: Optional[Union[_models.PrimingJobIdParameter, IO]] = None,
+        priming_job_id: Optional[Union[_models.PrimingJobIdParameter, IO[bytes]]] = None,
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Schedule a priming job for deletion.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param priming_job_id: Object containing the priming job ID. Is either a PrimingJobIdParameter
-         type or a IO type. Default value is None.
-        :type priming_job_id: ~azure.mgmt.storagecache.models.PrimingJobIdParameter or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         type or a IO[bytes] type. Default value is None.
+        :type priming_job_id: ~azure.mgmt.storagecache.models.PrimingJobIdParameter or IO[bytes]
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -1792,43 +1563,39 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod,
                 AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
             )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_stop_priming_job.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/stopPrimingJob"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     async def _pause_priming_job_initial(  # pylint: disable=inconsistent-return-statements
         self,
         resource_group_name: str,
         cache_name: str,
-        priming_job_id: Optional[Union[_models.PrimingJobIdParameter, IO]] = None,
+        priming_job_id: Optional[Union[_models.PrimingJobIdParameter, IO[bytes]]] = None,
         **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1849,32 +1616,31 @@
             _content = priming_job_id
         else:
             if priming_job_id is not None:
                 _json = self._serialize.body(priming_job_id, "PrimingJobIdParameter")
             else:
                 _json = None
 
-        request = build_pause_priming_job_request(
+        _request = build_pause_priming_job_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._pause_priming_job_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1883,19 +1649,15 @@
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _pause_priming_job_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/pausePrimingJob"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @overload
     async def begin_pause_priming_job(
         self,
         resource_group_name: str,
         cache_name: str,
         priming_job_id: Optional[_models.PrimingJobIdParameter] = None,
@@ -1912,93 +1674,66 @@
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param priming_job_id: Object containing the priming job ID. Default value is None.
         :type priming_job_id: ~azure.mgmt.storagecache.models.PrimingJobIdParameter
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_pause_priming_job(
         self,
         resource_group_name: str,
         cache_name: str,
-        priming_job_id: Optional[IO] = None,
+        priming_job_id: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Schedule a priming job to be paused.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param priming_job_id: Object containing the priming job ID. Default value is None.
-        :type priming_job_id: IO
+        :type priming_job_id: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_pause_priming_job(
         self,
         resource_group_name: str,
         cache_name: str,
-        priming_job_id: Optional[Union[_models.PrimingJobIdParameter, IO]] = None,
+        priming_job_id: Optional[Union[_models.PrimingJobIdParameter, IO[bytes]]] = None,
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Schedule a priming job to be paused.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param priming_job_id: Object containing the priming job ID. Is either a PrimingJobIdParameter
-         type or a IO type. Default value is None.
-        :type priming_job_id: ~azure.mgmt.storagecache.models.PrimingJobIdParameter or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         type or a IO[bytes] type. Default value is None.
+        :type priming_job_id: ~azure.mgmt.storagecache.models.PrimingJobIdParameter or IO[bytes]
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -2020,43 +1755,39 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod,
                 AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
             )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_pause_priming_job.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/pausePrimingJob"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     async def _resume_priming_job_initial(  # pylint: disable=inconsistent-return-statements
         self,
         resource_group_name: str,
         cache_name: str,
-        priming_job_id: Optional[Union[_models.PrimingJobIdParameter, IO]] = None,
+        priming_job_id: Optional[Union[_models.PrimingJobIdParameter, IO[bytes]]] = None,
         **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -2077,32 +1808,31 @@
             _content = priming_job_id
         else:
             if priming_job_id is not None:
                 _json = self._serialize.body(priming_job_id, "PrimingJobIdParameter")
             else:
                 _json = None
 
-        request = build_resume_priming_job_request(
+        _request = build_resume_priming_job_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._resume_priming_job_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -2111,19 +1841,15 @@
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _resume_priming_job_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/resumePrimingJob"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @overload
     async def begin_resume_priming_job(
         self,
         resource_group_name: str,
         cache_name: str,
         priming_job_id: Optional[_models.PrimingJobIdParameter] = None,
@@ -2140,93 +1866,66 @@
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param priming_job_id: Object containing the priming job ID. Default value is None.
         :type priming_job_id: ~azure.mgmt.storagecache.models.PrimingJobIdParameter
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_resume_priming_job(
         self,
         resource_group_name: str,
         cache_name: str,
-        priming_job_id: Optional[IO] = None,
+        priming_job_id: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Resumes a paused priming job.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param priming_job_id: Object containing the priming job ID. Default value is None.
-        :type priming_job_id: IO
+        :type priming_job_id: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_resume_priming_job(
         self,
         resource_group_name: str,
         cache_name: str,
-        priming_job_id: Optional[Union[_models.PrimingJobIdParameter, IO]] = None,
+        priming_job_id: Optional[Union[_models.PrimingJobIdParameter, IO[bytes]]] = None,
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Resumes a paused priming job.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param priming_job_id: Object containing the priming job ID. Is either a PrimingJobIdParameter
-         type or a IO type. Default value is None.
-        :type priming_job_id: ~azure.mgmt.storagecache.models.PrimingJobIdParameter or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         type or a IO[bytes] type. Default value is None.
+        :type priming_job_id: ~azure.mgmt.storagecache.models.PrimingJobIdParameter or IO[bytes]
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -2248,37 +1947,33 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod,
                 AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
             )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_resume_priming_job.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/resumePrimingJob"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     async def _upgrade_firmware_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, cache_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -2289,29 +1984,28 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_upgrade_firmware_request(
+        _request = build_upgrade_firmware_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._upgrade_firmware_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [201, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -2320,41 +2014,29 @@
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _upgrade_firmware_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/upgrade"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_upgrade_firmware(
         self, resource_group_name: str, cache_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Upgrade a cache's firmware if a new version is available. Otherwise, this operation has no
         effect.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -2373,43 +2055,39 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod,
                 AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
             )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_upgrade_firmware.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/upgrade"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     async def _space_allocation_initial(  # pylint: disable=inconsistent-return-statements
         self,
         resource_group_name: str,
         cache_name: str,
-        space_allocation: Optional[Union[List[_models.StorageTargetSpaceAllocation], IO]] = None,
+        space_allocation: Optional[Union[List[_models.StorageTargetSpaceAllocation], IO[bytes]]] = None,
         **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -2430,32 +2108,31 @@
             _content = space_allocation
         else:
             if space_allocation is not None:
                 _json = self._serialize.body(space_allocation, "[StorageTargetSpaceAllocation]")
             else:
                 _json = None
 
-        request = build_space_allocation_request(
+        _request = build_space_allocation_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._space_allocation_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -2463,19 +2140,15 @@
         response_headers = {}
         response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
         response_headers["Azure-AsyncOperation"] = self._deserialize(
             "str", response.headers.get("Azure-AsyncOperation")
         )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _space_allocation_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/spaceAllocation"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @overload
     async def begin_space_allocation(
         self,
         resource_group_name: str,
         cache_name: str,
         space_allocation: Optional[List[_models.StorageTargetSpaceAllocation]] = None,
@@ -2493,95 +2166,68 @@
         :type cache_name: str
         :param space_allocation: List containing storage target cache space percentage allocations.
          Default value is None.
         :type space_allocation: list[~azure.mgmt.storagecache.models.StorageTargetSpaceAllocation]
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_space_allocation(
         self,
         resource_group_name: str,
         cache_name: str,
-        space_allocation: Optional[IO] = None,
+        space_allocation: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Update cache space allocation.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param space_allocation: List containing storage target cache space percentage allocations.
          Default value is None.
-        :type space_allocation: IO
+        :type space_allocation: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_space_allocation(
         self,
         resource_group_name: str,
         cache_name: str,
-        space_allocation: Optional[Union[List[_models.StorageTargetSpaceAllocation], IO]] = None,
+        space_allocation: Optional[Union[List[_models.StorageTargetSpaceAllocation], IO[bytes]]] = None,
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Update cache space allocation.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param space_allocation: List containing storage target cache space percentage allocations. Is
-         either a [StorageTargetSpaceAllocation] type or a IO type. Default value is None.
+         either a [StorageTargetSpaceAllocation] type or a IO[bytes] type. Default value is None.
         :type space_allocation: list[~azure.mgmt.storagecache.models.StorageTargetSpaceAllocation] or
-         IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         IO[bytes]
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -2603,30 +2249,26 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod,
                 AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
             )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_space_allocation.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/spaceAllocation"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/_operations.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/_usage_models_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -23,111 +23,108 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._operations import build_list_request
+from ...operations._usage_models_operations import build_list_request
 from .._vendor import StorageCacheManagementClientMixinABC
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class Operations:
+class UsageModelsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.storagecache.aio.StorageCacheManagementClient`'s
-        :attr:`operations` attribute.
+        :attr:`usage_models` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, **kwargs: Any) -> AsyncIterable["_models.ApiOperation"]:
-        """Lists all of the available Resource Provider operations.
+    def list(self, **kwargs: Any) -> AsyncIterable["_models.UsageModel"]:
+        """Get the list of cache usage models available to this subscription.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either ApiOperation or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.storagecache.models.ApiOperation]
+        :return: An iterator like instance of either UsageModel or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.storagecache.models.UsageModel]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.ApiOperationListResult] = kwargs.pop("cls", None)
+        cls: ClsType[_models.UsageModelsResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
+                    subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize("ApiOperationListResult", pipeline_response)
+            deserialized = self._deserialize("UsageModelsResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {"url": "/providers/Microsoft.StorageCache/operations"}
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/_patch.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/_skus_operations.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/_skus_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -53,15 +53,14 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, **kwargs: Any) -> AsyncIterable["_models.ResourceSku"]:
         """Get the list of StorageCache.Cache SKUs available to this subscription.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ResourceSku or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.storagecache.models.ResourceSku]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -75,60 +74,57 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ResourceSkusResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/skus"}
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/_storage_cache_management_client_operations.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/_storage_cache_management_client_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -32,15 +32,17 @@
 )
 from .._vendor import StorageCacheManagementClientMixinABC
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class StorageCacheManagementClientOperationsMixin(StorageCacheManagementClientMixinABC):
+class StorageCacheManagementClientOperationsMixin(  # pylint: disable=name-too-long
+    StorageCacheManagementClientMixinABC
+):
     @overload
     async def check_aml_fs_subnets(  # pylint: disable=inconsistent-return-statements
         self,
         aml_filesystem_subnet_info: Optional[_models.AmlFilesystemSubnetInfo] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
@@ -49,51 +51,52 @@
 
         :param aml_filesystem_subnet_info: Information about the subnets to validate. Default value is
          None.
         :type aml_filesystem_subnet_info: ~azure.mgmt.storagecache.models.AmlFilesystemSubnetInfo
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def check_aml_fs_subnets(  # pylint: disable=inconsistent-return-statements
-        self, aml_filesystem_subnet_info: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
+        self,
+        aml_filesystem_subnet_info: Optional[IO[bytes]] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
     ) -> None:
         """Check that subnets will be valid for AML file system create calls.
 
         :param aml_filesystem_subnet_info: Information about the subnets to validate. Default value is
          None.
-        :type aml_filesystem_subnet_info: IO
+        :type aml_filesystem_subnet_info: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def check_aml_fs_subnets(  # pylint: disable=inconsistent-return-statements
-        self, aml_filesystem_subnet_info: Optional[Union[_models.AmlFilesystemSubnetInfo, IO]] = None, **kwargs: Any
+        self,
+        aml_filesystem_subnet_info: Optional[Union[_models.AmlFilesystemSubnetInfo, IO[bytes]]] = None,
+        **kwargs: Any
     ) -> None:
         """Check that subnets will be valid for AML file system create calls.
 
         :param aml_filesystem_subnet_info: Information about the subnets to validate. Is either a
-         AmlFilesystemSubnetInfo type or a IO type. Default value is None.
-        :type aml_filesystem_subnet_info: ~azure.mgmt.storagecache.models.AmlFilesystemSubnetInfo or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         AmlFilesystemSubnetInfo type or a IO[bytes] type. Default value is None.
+        :type aml_filesystem_subnet_info: ~azure.mgmt.storagecache.models.AmlFilesystemSubnetInfo or
+         IO[bytes]
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -121,44 +124,39 @@
             _content = aml_filesystem_subnet_info
         else:
             if aml_filesystem_subnet_info is not None:
                 _json = self._serialize.body(aml_filesystem_subnet_info, "AmlFilesystemSubnetInfo")
             else:
                 _json = None
 
-        request = build_check_aml_fs_subnets_request(
+        _request = build_check_aml_fs_subnets_request(
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.check_aml_fs_subnets.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         if cls:
-            return cls(pipeline_response, None, {})
-
-    check_aml_fs_subnets.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/checkAmlFSSubnets"
-    }
+            return cls(pipeline_response, None, {})  # type: ignore
 
     @overload
     async def get_required_aml_fs_subnets_size(
         self,
         required_aml_filesystem_subnets_size_info: Optional[_models.RequiredAmlFilesystemSubnetsSizeInfo] = None,
         *,
         content_type: str = "application/json",
@@ -169,61 +167,55 @@
         :param required_aml_filesystem_subnets_size_info: Information to determine the number of
          available IPs a subnet will need to host the AML file system. Default value is None.
         :type required_aml_filesystem_subnets_size_info:
          ~azure.mgmt.storagecache.models.RequiredAmlFilesystemSubnetsSizeInfo
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RequiredAmlFilesystemSubnetsSize or the result of cls(response)
         :rtype: ~azure.mgmt.storagecache.models.RequiredAmlFilesystemSubnetsSize
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def get_required_aml_fs_subnets_size(
         self,
-        required_aml_filesystem_subnets_size_info: Optional[IO] = None,
+        required_aml_filesystem_subnets_size_info: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.RequiredAmlFilesystemSubnetsSize:
         """Get the number of available IP addresses needed for the AML file system information provided.
 
         :param required_aml_filesystem_subnets_size_info: Information to determine the number of
          available IPs a subnet will need to host the AML file system. Default value is None.
-        :type required_aml_filesystem_subnets_size_info: IO
+        :type required_aml_filesystem_subnets_size_info: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RequiredAmlFilesystemSubnetsSize or the result of cls(response)
         :rtype: ~azure.mgmt.storagecache.models.RequiredAmlFilesystemSubnetsSize
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def get_required_aml_fs_subnets_size(
         self,
         required_aml_filesystem_subnets_size_info: Optional[
-            Union[_models.RequiredAmlFilesystemSubnetsSizeInfo, IO]
+            Union[_models.RequiredAmlFilesystemSubnetsSizeInfo, IO[bytes]]
         ] = None,
         **kwargs: Any
     ) -> _models.RequiredAmlFilesystemSubnetsSize:
         """Get the number of available IP addresses needed for the AML file system information provided.
 
         :param required_aml_filesystem_subnets_size_info: Information to determine the number of
          available IPs a subnet will need to host the AML file system. Is either a
-         RequiredAmlFilesystemSubnetsSizeInfo type or a IO type. Default value is None.
+         RequiredAmlFilesystemSubnetsSizeInfo type or a IO[bytes] type. Default value is None.
         :type required_aml_filesystem_subnets_size_info:
-         ~azure.mgmt.storagecache.models.RequiredAmlFilesystemSubnetsSizeInfo or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ~azure.mgmt.storagecache.models.RequiredAmlFilesystemSubnetsSizeInfo or IO[bytes]
         :return: RequiredAmlFilesystemSubnetsSize or the result of cls(response)
         :rtype: ~azure.mgmt.storagecache.models.RequiredAmlFilesystemSubnetsSize
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -248,41 +240,36 @@
             if required_aml_filesystem_subnets_size_info is not None:
                 _json = self._serialize.body(
                     required_aml_filesystem_subnets_size_info, "RequiredAmlFilesystemSubnetsSizeInfo"
                 )
             else:
                 _json = None
 
-        request = build_get_required_aml_fs_subnets_size_request(
+        _request = build_get_required_aml_fs_subnets_size_request(
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.get_required_aml_fs_subnets_size.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("RequiredAmlFilesystemSubnetsSize", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get_required_aml_fs_subnets_size.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/getRequiredAmlFSSubnetsSize"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/_storage_target_operations.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/_storage_target_operations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -13,56 +13,197 @@
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse
-from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
+from azure.core.pipeline.transport import HttpResponse
+from azure.core.polling import LROPoller, NoPolling, PollingMethod
 from azure.core.rest import HttpRequest
-from azure.core.tracing.decorator_async import distributed_trace_async
+from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
-from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
+from azure.mgmt.core.polling.arm_polling import ARMPolling
 
-from ... import models as _models
-from ..._vendor import _convert_request
-from ...operations._storage_target_operations import (
-    build_flush_request,
-    build_invalidate_request,
-    build_resume_request,
-    build_suspend_request,
-)
-from .._vendor import StorageCacheManagementClientMixinABC
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import StorageCacheManagementClientMixinABC, _convert_request
 
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
+
+
+def build_flush_request(
+    resource_group_name: str, cache_name: str, storage_target_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/flush",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
+        "storageTargetName": _SERIALIZER.url(
+            "storage_target_name", storage_target_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"
+        ),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_suspend_request(
+    resource_group_name: str, cache_name: str, storage_target_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/suspend",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
+        "storageTargetName": _SERIALIZER.url(
+            "storage_target_name", storage_target_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"
+        ),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_resume_request(
+    resource_group_name: str, cache_name: str, storage_target_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/resume",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
+        "storageTargetName": _SERIALIZER.url(
+            "storage_target_name", storage_target_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"
+        ),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_invalidate_request(
+    resource_group_name: str, cache_name: str, storage_target_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/invalidate",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
+        "storageTargetName": _SERIALIZER.url(
+            "storage_target_name", storage_target_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"
+        ),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 class StorageTargetOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.storagecache.aio.StorageCacheManagementClient`'s
+        :class:`~azure.mgmt.storagecache.StorageCacheManagementClient`'s
         :attr:`storage_target` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    async def _flush_initial(  # pylint: disable=inconsistent-return-statements
+    def _flush_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -71,30 +212,29 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_flush_request(
+        _request = build_flush_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._flush_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -103,96 +243,79 @@
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _flush_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/flush"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
-    @distributed_trace_async
-    async def begin_flush(
+    @distributed_trace
+    def begin_flush(
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
-    ) -> AsyncLROPoller[None]:
+    ) -> LROPoller[None]:
         """Tells the cache to write all dirty data to the Storage Target's backend storage. Client
         requests to this storage target's namespace will return errors until the flush operation
         completes.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[None]
+        :return: An instance of LROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._flush_initial(  # type: ignore
+            raw_result = self._flush_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 cache_name=cache_name,
                 storage_target_name=storage_target_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(
-                AsyncPollingMethod,
-                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
             )
         elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+            polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return LROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_flush.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/flush"
-    }
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    async def _suspend_initial(  # pylint: disable=inconsistent-return-statements
+    def _suspend_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -201,30 +324,29 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_suspend_request(
+        _request = build_suspend_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._suspend_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -233,94 +355,77 @@
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _suspend_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/suspend"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
-    @distributed_trace_async
-    async def begin_suspend(
+    @distributed_trace
+    def begin_suspend(
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
-    ) -> AsyncLROPoller[None]:
+    ) -> LROPoller[None]:
         """Suspends client access to a storage target.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[None]
+        :return: An instance of LROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._suspend_initial(  # type: ignore
+            raw_result = self._suspend_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 cache_name=cache_name,
                 storage_target_name=storage_target_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(
-                AsyncPollingMethod,
-                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
             )
         elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+            polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return LROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_suspend.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/suspend"
-    }
-
-    async def _resume_initial(  # pylint: disable=inconsistent-return-statements
+    def _resume_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -329,30 +434,29 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_resume_request(
+        _request = build_resume_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._resume_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -361,94 +465,77 @@
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
-    _resume_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/resume"
-    }
-
-    @distributed_trace_async
-    async def begin_resume(
+    @distributed_trace
+    def begin_resume(
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
-    ) -> AsyncLROPoller[None]:
+    ) -> LROPoller[None]:
         """Resumes client access to a previously suspended storage target.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[None]
+        :return: An instance of LROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._resume_initial(  # type: ignore
+            raw_result = self._resume_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 cache_name=cache_name,
                 storage_target_name=storage_target_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(
-                AsyncPollingMethod,
-                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
             )
         elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+            polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return LROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_resume.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/resume"
-    }
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    async def _invalidate_initial(  # pylint: disable=inconsistent-return-statements
+    def _invalidate_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -457,30 +544,29 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_invalidate_request(
+        _request = build_invalidate_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._invalidate_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -489,86 +575,69 @@
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _invalidate_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/invalidate"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
-    @distributed_trace_async
-    async def begin_invalidate(
+    @distributed_trace
+    def begin_invalidate(
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
-    ) -> AsyncLROPoller[None]:
+    ) -> LROPoller[None]:
         """Invalidate all cached data for a storage target. Cached files are discarded and fetched from
         the back end on the next request.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[None]
+        :return: An instance of LROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._invalidate_initial(  # type: ignore
+            raw_result = self._invalidate_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 cache_name=cache_name,
                 storage_target_name=storage_target_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(
-                AsyncPollingMethod,
-                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
             )
         elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+            polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return LROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_invalidate.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/invalidate"
-    }
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/_storage_targets_operations.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/_storage_targets_operations.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,292 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
-from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
+from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse
-from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
+from azure.core.pipeline.transport import HttpResponse
+from azure.core.polling import LROPoller, NoPolling, PollingMethod
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
-from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
-from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
+from azure.mgmt.core.polling.arm_polling import ARMPolling
 
-from ... import models as _models
-from ..._vendor import _convert_request
-from ...operations._storage_targets_operations import (
-    build_create_or_update_request,
-    build_delete_request,
-    build_dns_refresh_request,
-    build_get_request,
-    build_list_by_cache_request,
-    build_restore_defaults_request,
-)
-from .._vendor import StorageCacheManagementClientMixinABC
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import StorageCacheManagementClientMixinABC, _convert_request
 
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
+
+
+def build_dns_refresh_request(
+    resource_group_name: str, cache_name: str, storage_target_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/dnsRefresh",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
+        "storageTargetName": _SERIALIZER.url(
+            "storage_target_name", storage_target_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"
+        ),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_list_by_cache_request(
+    resource_group_name: str, cache_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_delete_request(
+    resource_group_name: str,
+    cache_name: str,
+    storage_target_name: str,
+    subscription_id: str,
+    *,
+    force: Optional[str] = None,
+    **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
+        "storageTargetName": _SERIALIZER.url(
+            "storage_target_name", storage_target_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"
+        ),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+    if force is not None:
+        _params["force"] = _SERIALIZER.query("force", force, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_get_request(
+    resource_group_name: str, cache_name: str, storage_target_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
+        "storageTargetName": _SERIALIZER.url(
+            "storage_target_name", storage_target_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"
+        ),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_create_or_update_request(
+    resource_group_name: str, cache_name: str, storage_target_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
+        "storageTargetName": _SERIALIZER.url(
+            "storage_target_name", storage_target_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"
+        ),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_restore_defaults_request(
+    resource_group_name: str, cache_name: str, storage_target_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/restoreDefaults",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
+        "storageTargetName": _SERIALIZER.url(
+            "storage_target_name", storage_target_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"
+        ),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 class StorageTargetsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.storagecache.aio.StorageCacheManagementClient`'s
+        :class:`~azure.mgmt.storagecache.StorageCacheManagementClient`'s
         :attr:`storage_targets` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    async def _dns_refresh_initial(  # pylint: disable=inconsistent-return-statements
+    def _dns_refresh_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -77,30 +295,29 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_dns_refresh_request(
+        _request = build_dns_refresh_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._dns_refresh_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -109,108 +326,90 @@
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _dns_refresh_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/dnsRefresh"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
-    @distributed_trace_async
-    async def begin_dns_refresh(
+    @distributed_trace
+    def begin_dns_refresh(
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
-    ) -> AsyncLROPoller[None]:
+    ) -> LROPoller[None]:
         """Tells a storage target to refresh its DNS information.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[None]
+        :return: An instance of LROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._dns_refresh_initial(  # type: ignore
+            raw_result = self._dns_refresh_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 cache_name=cache_name,
                 storage_target_name=storage_target_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(
-                AsyncPollingMethod,
-                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
             )
         elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+            polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return LROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_dns_refresh.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/dnsRefresh"
-    }
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     @distributed_trace
     def list_by_cache(
         self, resource_group_name: str, cache_name: str, **kwargs: Any
-    ) -> AsyncIterable["_models.StorageTarget"]:
+    ) -> Iterable["_models.StorageTarget"]:
         """Returns a list of Storage Targets for the specified cache.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either StorageTarget or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.storagecache.models.StorageTarget]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.storagecache.models.StorageTarget]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.StorageTargetsResult] = kwargs.pop("cls", None)
@@ -222,73 +421,68 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_cache_request(
+                _request = build_list_by_cache_request(
                     resource_group_name=resource_group_name,
                     cache_name=cache_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_cache.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
-        async def extract_data(pipeline_response):
+        def extract_data(pipeline_response):
             deserialized = self._deserialize("StorageTargetsResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, AsyncList(list_of_elem)
+            return deserialized.next_link or None, iter(list_of_elem)
 
-        async def get_next(next_link=None):
-            request = prepare_request(next_link)
+        def get_next(next_link=None):
+            _request = prepare_request(next_link)
 
             _stream = False
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return AsyncItemPaged(get_next, extract_data)
+        return ItemPaged(get_next, extract_data)
 
-    list_by_cache.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets"
-    }
-
-    async def _delete_initial(  # pylint: disable=inconsistent-return-statements
+    def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self,
         resource_group_name: str,
         cache_name: str,
         storage_target_name: str,
         force: Optional[str] = None,
         **kwargs: Any
     ) -> None:
@@ -302,31 +496,30 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
             force=force,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -335,29 +528,25 @@
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
-    @distributed_trace_async
-    async def begin_delete(
+    @distributed_trace
+    def begin_delete(
         self,
         resource_group_name: str,
         cache_name: str,
         storage_target_name: str,
         force: Optional[str] = None,
         **kwargs: Any
-    ) -> AsyncLROPoller[None]:
+    ) -> LROPoller[None]:
         """Removes a Storage Target from a cache. This operation is allowed at any time, but if the cache
         is down or unhealthy, the actual removal of the Storage Target may be delayed until the cache
         is healthy again. Note that if the cache has data to flush to the Storage Target, the data will
         be flushed before the Storage Target will be deleted.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
@@ -367,86 +556,73 @@
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
         :param force: Boolean value requesting the force delete operation for a storage target. Force
          delete discards unwritten-data in the cache instead of flushing it to back-end storage. Default
          value is None.
         :type force: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[None]
+        :return: An instance of LROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._delete_initial(  # type: ignore
+            raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 cache_name=cache_name,
                 storage_target_name=storage_target_name,
                 force=force,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
+            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+            polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return LROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}"
-    }
-
-    @distributed_trace_async
-    async def get(
+    @distributed_trace
+    def get(
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
     ) -> _models.StorageTarget:
         """Returns a Storage Target from a cache.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: StorageTarget or the result of cls(response)
         :rtype: ~azure.mgmt.storagecache.models.StorageTarget
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -457,55 +633,50 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.StorageTarget] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("StorageTarget", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}"
-    }
-
-    async def _create_or_update_initial(
+    def _create_or_update_initial(
         self,
         resource_group_name: str,
         cache_name: str,
         storage_target_name: str,
-        storagetarget: Union[_models.StorageTarget, IO],
+        storagetarget: Union[_models.StorageTarget, IO[bytes]],
         **kwargs: Any
     ) -> Optional[_models.StorageTarget]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -523,33 +694,32 @@
         _json = None
         _content = None
         if isinstance(storagetarget, (IOBase, bytes)):
             _content = storagetarget
         else:
             _json = self._serialize.body(storagetarget, "StorageTarget")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -558,33 +728,29 @@
         if response.status_code == 200:
             deserialized = self._deserialize("StorageTarget", pipeline_response)
 
         if response.status_code == 201:
             deserialized = self._deserialize("StorageTarget", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
-    async def begin_create_or_update(
+    def begin_create_or_update(
         self,
         resource_group_name: str,
         cache_name: str,
         storage_target_name: str,
         storagetarget: _models.StorageTarget,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.StorageTarget]:
+    ) -> LROPoller[_models.StorageTarget]:
         """Create or update a Storage Target. This operation is allowed at any time, but if the cache is
         down or unhealthy, the actual creation/modification of the Storage Target may be delayed until
         the cache is healthy again.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
@@ -594,121 +760,94 @@
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
         :param storagetarget: Object containing the definition of a Storage Target. Required.
         :type storagetarget: ~azure.mgmt.storagecache.models.StorageTarget
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either StorageTarget or the result of
+        :return: An instance of LROPoller that returns either StorageTarget or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.StorageTarget]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.storagecache.models.StorageTarget]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    async def begin_create_or_update(
+    def begin_create_or_update(
         self,
         resource_group_name: str,
         cache_name: str,
         storage_target_name: str,
-        storagetarget: IO,
+        storagetarget: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.StorageTarget]:
+    ) -> LROPoller[_models.StorageTarget]:
         """Create or update a Storage Target. This operation is allowed at any time, but if the cache is
         down or unhealthy, the actual creation/modification of the Storage Target may be delayed until
         the cache is healthy again.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
         :param storagetarget: Object containing the definition of a Storage Target. Required.
-        :type storagetarget: IO
+        :type storagetarget: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either StorageTarget or the result of
+        :return: An instance of LROPoller that returns either StorageTarget or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.StorageTarget]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.storagecache.models.StorageTarget]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
-    @distributed_trace_async
-    async def begin_create_or_update(
+    @distributed_trace
+    def begin_create_or_update(
         self,
         resource_group_name: str,
         cache_name: str,
         storage_target_name: str,
-        storagetarget: Union[_models.StorageTarget, IO],
+        storagetarget: Union[_models.StorageTarget, IO[bytes]],
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.StorageTarget]:
+    ) -> LROPoller[_models.StorageTarget]:
         """Create or update a Storage Target. This operation is allowed at any time, but if the cache is
         down or unhealthy, the actual creation/modification of the Storage Target may be delayed until
         the cache is healthy again.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
         :param storagetarget: Object containing the definition of a Storage Target. Is either a
-         StorageTarget type or a IO type. Required.
-        :type storagetarget: ~azure.mgmt.storagecache.models.StorageTarget or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either StorageTarget or the result of
+         StorageTarget type or a IO[bytes] type. Required.
+        :type storagetarget: ~azure.mgmt.storagecache.models.StorageTarget or IO[bytes]
+        :return: An instance of LROPoller that returns either StorageTarget or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.StorageTarget]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.storagecache.models.StorageTarget]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.StorageTarget] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._create_or_update_initial(
+            raw_result = self._create_or_update_initial(
                 resource_group_name=resource_group_name,
                 cache_name=cache_name,
                 storage_target_name=storage_target_name,
                 storagetarget=storagetarget,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
@@ -717,37 +856,35 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("StorageTarget", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
+            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+            polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return LROPoller[_models.StorageTarget].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}"
-    }
+        return LROPoller[_models.StorageTarget](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
-    async def _restore_defaults_initial(  # pylint: disable=inconsistent-return-statements
+    def _restore_defaults_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -756,30 +893,29 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_restore_defaults_request(
+        _request = build_restore_defaults_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._restore_defaults_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -788,84 +924,68 @@
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _restore_defaults_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/restoreDefaults"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
-    @distributed_trace_async
-    async def begin_restore_defaults(
+    @distributed_trace
+    def begin_restore_defaults(
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
-    ) -> AsyncLROPoller[None]:
+    ) -> LROPoller[None]:
         """Tells a storage target to restore its settings to their default values.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[None]
+        :return: An instance of LROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._restore_defaults_initial(  # type: ignore
+            raw_result = self._restore_defaults_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 cache_name=cache_name,
                 storage_target_name=storage_target_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(
-                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
             )
         elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+            polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return LROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_restore_defaults.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/restoreDefaults"
-    }
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/aio/operations/_usage_models_operations.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -23,112 +23,107 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._usage_models_operations import build_list_request
+from ...operations._operations import build_list_request
 from .._vendor import StorageCacheManagementClientMixinABC
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class UsageModelsOperations:
+class Operations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.storagecache.aio.StorageCacheManagementClient`'s
-        :attr:`usage_models` attribute.
+        :attr:`operations` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, **kwargs: Any) -> AsyncIterable["_models.UsageModel"]:
-        """Get the list of cache usage models available to this subscription.
+    def list(self, **kwargs: Any) -> AsyncIterable["_models.ApiOperation"]:
+        """Lists all of the available Resource Provider operations.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either UsageModel or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.storagecache.models.UsageModel]
+        :return: An iterator like instance of either ApiOperation or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.storagecache.models.ApiOperation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.UsageModelsResult] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ApiOperationListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
-                    subscription_id=self._config.subscription_id,
+                _request = build_list_request(
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize("UsageModelsResult", pipeline_response)
+            deserialized = self._deserialize("ApiOperationListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/usageModels"}
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/models/__init__.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from ._models_py3 import AmlFilesystemUpdatePropertiesMaintenanceWindow
 from ._models_py3 import AmlFilesystemsListResult
 from ._models_py3 import ApiOperation
 from ._models_py3 import ApiOperationDisplay
 from ._models_py3 import ApiOperationListResult
 from ._models_py3 import ApiOperationPropertiesServiceSpecification
 from ._models_py3 import AscOperation
+from ._models_py3 import AscOperationErrorResponse
 from ._models_py3 import BlobNfsTarget
 from ._models_py3 import Cache
 from ._models_py3 import CacheActiveDirectorySettings
 from ._models_py3 import CacheActiveDirectorySettingsCredentials
 from ._models_py3 import CacheDirectorySettings
 from ._models_py3 import CacheEncryptionSettings
 from ._models_py3 import CacheHealth
@@ -45,15 +46,20 @@
 from ._models_py3 import CacheUpgradeStatus
 from ._models_py3 import CacheUsernameDownloadSettings
 from ._models_py3 import CacheUsernameDownloadSettingsCredentials
 from ._models_py3 import CachesListResult
 from ._models_py3 import ClfsTarget
 from ._models_py3 import CloudErrorBody
 from ._models_py3 import Condition
+from ._models_py3 import ErrorAdditionalInfo
+from ._models_py3 import ErrorDetail
 from ._models_py3 import ErrorResponse
+from ._models_py3 import ImportJob
+from ._models_py3 import ImportJobUpdate
+from ._models_py3 import ImportJobsListResult
 from ._models_py3 import KeyVaultKeyReference
 from ._models_py3 import KeyVaultKeyReferenceSourceVault
 from ._models_py3 import LogSpecification
 from ._models_py3 import MetricDimension
 from ._models_py3 import MetricSpecification
 from ._models_py3 import NamespaceJunction
 from ._models_py3 import Nfs3Target
@@ -88,19 +94,22 @@
 
 from ._storage_cache_management_client_enums import AmlFilesystemHealthStateType
 from ._storage_cache_management_client_enums import AmlFilesystemIdentityType
 from ._storage_cache_management_client_enums import AmlFilesystemProvisioningStateType
 from ._storage_cache_management_client_enums import AmlFilesystemSquashMode
 from ._storage_cache_management_client_enums import ArchiveStatusType
 from ._storage_cache_management_client_enums import CacheIdentityType
+from ._storage_cache_management_client_enums import ConflictResolutionMode
 from ._storage_cache_management_client_enums import CreatedByType
 from ._storage_cache_management_client_enums import DomainJoinedType
 from ._storage_cache_management_client_enums import FilesystemSubnetStatusType
 from ._storage_cache_management_client_enums import FirmwareStatusType
 from ._storage_cache_management_client_enums import HealthStateType
+from ._storage_cache_management_client_enums import ImportJobProvisioningStateType
+from ._storage_cache_management_client_enums import ImportStatusType
 from ._storage_cache_management_client_enums import MaintenanceDayOfWeekType
 from ._storage_cache_management_client_enums import MetricAggregationType
 from ._storage_cache_management_client_enums import NfsAccessRuleAccess
 from ._storage_cache_management_client_enums import NfsAccessRuleScope
 from ._storage_cache_management_client_enums import OperationalStateType
 from ._storage_cache_management_client_enums import PrimingJobState
 from ._storage_cache_management_client_enums import ProvisioningStateType
@@ -133,14 +142,15 @@
     "AmlFilesystemUpdatePropertiesMaintenanceWindow",
     "AmlFilesystemsListResult",
     "ApiOperation",
     "ApiOperationDisplay",
     "ApiOperationListResult",
     "ApiOperationPropertiesServiceSpecification",
     "AscOperation",
+    "AscOperationErrorResponse",
     "BlobNfsTarget",
     "Cache",
     "CacheActiveDirectorySettings",
     "CacheActiveDirectorySettingsCredentials",
     "CacheDirectorySettings",
     "CacheEncryptionSettings",
     "CacheHealth",
@@ -152,15 +162,20 @@
     "CacheUpgradeStatus",
     "CacheUsernameDownloadSettings",
     "CacheUsernameDownloadSettingsCredentials",
     "CachesListResult",
     "ClfsTarget",
     "CloudErrorBody",
     "Condition",
+    "ErrorAdditionalInfo",
+    "ErrorDetail",
     "ErrorResponse",
+    "ImportJob",
+    "ImportJobUpdate",
+    "ImportJobsListResult",
     "KeyVaultKeyReference",
     "KeyVaultKeyReferenceSourceVault",
     "LogSpecification",
     "MetricDimension",
     "MetricSpecification",
     "NamespaceJunction",
     "Nfs3Target",
@@ -194,19 +209,22 @@
     "UserAssignedIdentitiesValueAutoGenerated",
     "AmlFilesystemHealthStateType",
     "AmlFilesystemIdentityType",
     "AmlFilesystemProvisioningStateType",
     "AmlFilesystemSquashMode",
     "ArchiveStatusType",
     "CacheIdentityType",
+    "ConflictResolutionMode",
     "CreatedByType",
     "DomainJoinedType",
     "FilesystemSubnetStatusType",
     "FirmwareStatusType",
     "HealthStateType",
+    "ImportJobProvisioningStateType",
+    "ImportStatusType",
     "MaintenanceDayOfWeekType",
     "MetricAggregationType",
     "NfsAccessRuleAccess",
     "NfsAccessRuleScope",
     "OperationalStateType",
     "PrimingJobState",
     "ProvisioningStateType",
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/models/_models_py3.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/models/_models_py3.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 class Resource(_serialization.Model):
     """Common fields that are returned in the response for all Azure Resource Manager resources.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -67,18 +67,18 @@
 
 class TrackedResource(Resource):
     """The resource model definition for an Azure Resource Manager tracked top level resource which
     has 'tags' and a 'location'.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -121,18 +121,18 @@
 
 class AmlFilesystem(TrackedResource):  # pylint: disable=too-many-instance-attributes
     """An AML file system instance. Follows Azure Resource Manager standards:
     https://github.com/Azure/azure-resource-manager-rpc/blob/master/v1.0/resource-api-reference.md.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -397,15 +397,15 @@
         :paramtype filesystem_subnet:
          ~azure.mgmt.storagecache.models.AmlFilesystemCheckSubnetErrorFilesystemSubnet
         """
         super().__init__(**kwargs)
         self.filesystem_subnet = filesystem_subnet
 
 
-class AmlFilesystemCheckSubnetErrorFilesystemSubnet(_serialization.Model):
+class AmlFilesystemCheckSubnetErrorFilesystemSubnet(_serialization.Model):  # pylint: disable=name-too-long
     """The error details for the AML file system's subnet.
 
     :ivar status: The status of the AML file system subnet check. Known values are: "Ok" and
      "Invalid".
     :vartype status: str or ~azure.mgmt.storagecache.models.FilesystemSubnetStatusType
     :ivar message: The details of the AML file system subnet check.
     :vartype message: str
@@ -575,60 +575,82 @@
         self.status_code = status_code
         self.status_description = status_description
 
 
 class AmlFilesystemHsmSettings(_serialization.Model):
     """AML file system HSM settings.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar container: Resource ID of storage container used for hydrating the namespace and
      archiving from the namespace. The resource provider must have permission to create SAS tokens
      on the storage account. Required.
     :vartype container: str
     :ivar logging_container: Resource ID of storage container used for logging events and errors.
      Must be a separate container in the same storage account as the hydration and archive
      container. The resource provider must have permission to create SAS tokens on the storage
      account. Required.
     :vartype logging_container: str
     :ivar import_prefix: Only blobs in the non-logging container that start with this path/prefix
-     get hydrated into the cluster namespace.
+     get imported into the cluster namespace. This is only used during initial creation of the AML
+     file system. It automatically creates an import job resource that can be deleted.
     :vartype import_prefix: str
+    :ivar import_prefixes_initial: Only blobs in the non-logging container that start with one of
+     the paths/prefixes in this array get imported into the cluster namespace. This is only used
+     during initial creation of the AML file system and has '/' as the default value. It
+     automatically creates an import job resource that can be deleted.
+    :vartype import_prefixes_initial: list[str]
     """
 
     _validation = {
         "container": {"required": True},
         "logging_container": {"required": True},
     }
 
     _attribute_map = {
         "container": {"key": "container", "type": "str"},
         "logging_container": {"key": "loggingContainer", "type": "str"},
         "import_prefix": {"key": "importPrefix", "type": "str"},
+        "import_prefixes_initial": {"key": "importPrefixesInitial", "type": "[str]"},
     }
 
-    def __init__(self, *, container: str, logging_container: str, import_prefix: str = "/", **kwargs: Any) -> None:
+    def __init__(
+        self,
+        *,
+        container: str,
+        logging_container: str,
+        import_prefix: str = "/",
+        import_prefixes_initial: Optional[List[str]] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword container: Resource ID of storage container used for hydrating the namespace and
          archiving from the namespace. The resource provider must have permission to create SAS tokens
          on the storage account. Required.
         :paramtype container: str
         :keyword logging_container: Resource ID of storage container used for logging events and
          errors.  Must be a separate container in the same storage account as the hydration and archive
          container. The resource provider must have permission to create SAS tokens on the storage
          account. Required.
         :paramtype logging_container: str
         :keyword import_prefix: Only blobs in the non-logging container that start with this
-         path/prefix get hydrated into the cluster namespace.
+         path/prefix get imported into the cluster namespace. This is only used during initial creation
+         of the AML file system. It automatically creates an import job resource that can be deleted.
         :paramtype import_prefix: str
+        :keyword import_prefixes_initial: Only blobs in the non-logging container that start with one
+         of the paths/prefixes in this array get imported into the cluster namespace. This is only used
+         during initial creation of the AML file system and has '/' as the default value. It
+         automatically creates an import job resource that can be deleted.
+        :paramtype import_prefixes_initial: list[str]
         """
         super().__init__(**kwargs)
         self.container = container
         self.logging_container = logging_container
         self.import_prefix = import_prefix
+        self.import_prefixes_initial = import_prefixes_initial
 
 
 class AmlFilesystemIdentity(_serialization.Model):
     """Managed Identity properties.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
@@ -939,15 +961,15 @@
         super().__init__(**kwargs)
         self.tags = tags
         self.encryption_settings = encryption_settings
         self.maintenance_window = maintenance_window
         self.root_squash_settings = root_squash_settings
 
 
-class AmlFilesystemUpdatePropertiesMaintenanceWindow(_serialization.Model):
+class AmlFilesystemUpdatePropertiesMaintenanceWindow(_serialization.Model):  # pylint: disable=name-too-long
     """Start time of a 30-minute weekly maintenance window.
 
     :ivar day_of_week: Day of the week on which the maintenance window will occur. Known values
      are: "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", and "Sunday".
     :vartype day_of_week: str or ~azure.mgmt.storagecache.models.MaintenanceDayOfWeekType
     :ivar time_of_day_utc: The time of day (in UTC) to start the maintenance window.
     :vartype time_of_day_utc: str
@@ -1114,15 +1136,15 @@
         :paramtype value: list[~azure.mgmt.storagecache.models.ApiOperation]
         """
         super().__init__(**kwargs)
         self.next_link = next_link
         self.value = value
 
 
-class ApiOperationPropertiesServiceSpecification(_serialization.Model):
+class ApiOperationPropertiesServiceSpecification(_serialization.Model):  # pylint: disable=name-too-long
     """Specification of the all the metrics provided for a resource type.
 
     :ivar metric_specifications: Details about operations related to metrics.
     :vartype metric_specifications: list[~azure.mgmt.storagecache.models.MetricSpecification]
     :ivar log_specifications: Details about operations related to logs.
     :vartype log_specifications: list[~azure.mgmt.storagecache.models.LogSpecification]
     """
@@ -1160,38 +1182,38 @@
     :ivar start_time: The start time of the operation.
     :vartype start_time: str
     :ivar end_time: The end time of the operation.
     :vartype end_time: str
     :ivar status: The status of the operation.
     :vartype status: str
     :ivar error: The error detail of the operation if any.
-    :vartype error: ~azure.mgmt.storagecache.models.ErrorResponse
+    :vartype error: ~azure.mgmt.storagecache.models.AscOperationErrorResponse
     :ivar output: Additional operation-specific output.
     :vartype output: dict[str, JSON]
     """
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "start_time": {"key": "startTime", "type": "str"},
         "end_time": {"key": "endTime", "type": "str"},
         "status": {"key": "status", "type": "str"},
-        "error": {"key": "error", "type": "ErrorResponse"},
+        "error": {"key": "error", "type": "AscOperationErrorResponse"},
         "output": {"key": "properties.output", "type": "{object}"},
     }
 
     def __init__(
         self,
         *,
         id: Optional[str] = None,  # pylint: disable=redefined-builtin
         name: Optional[str] = None,
         start_time: Optional[str] = None,
         end_time: Optional[str] = None,
         status: Optional[str] = None,
-        error: Optional["_models.ErrorResponse"] = None,
+        error: Optional["_models.AscOperationErrorResponse"] = None,
         output: Optional[Dict[str, JSON]] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword id: The operation Id.
         :paramtype id: str
         :keyword name: The operation name.
@@ -1199,28 +1221,54 @@
         :keyword start_time: The start time of the operation.
         :paramtype start_time: str
         :keyword end_time: The end time of the operation.
         :paramtype end_time: str
         :keyword status: The status of the operation.
         :paramtype status: str
         :keyword error: The error detail of the operation if any.
-        :paramtype error: ~azure.mgmt.storagecache.models.ErrorResponse
+        :paramtype error: ~azure.mgmt.storagecache.models.AscOperationErrorResponse
         :keyword output: Additional operation-specific output.
         :paramtype output: dict[str, JSON]
         """
         super().__init__(**kwargs)
         self.id = id
         self.name = name
         self.start_time = start_time
         self.end_time = end_time
         self.status = status
         self.error = error
         self.output = output
 
 
+class AscOperationErrorResponse(_serialization.Model):
+    """Describes the format of Error response.
+
+    :ivar code: Error code.
+    :vartype code: str
+    :ivar message: Error message indicating why the operation failed.
+    :vartype message: str
+    """
+
+    _attribute_map = {
+        "code": {"key": "code", "type": "str"},
+        "message": {"key": "message", "type": "str"},
+    }
+
+    def __init__(self, *, code: Optional[str] = None, message: Optional[str] = None, **kwargs: Any) -> None:
+        """
+        :keyword code: Error code.
+        :paramtype code: str
+        :keyword message: Error message indicating why the operation failed.
+        :paramtype message: str
+        """
+        super().__init__(**kwargs)
+        self.code = code
+        self.message = message
+
+
 class BlobNfsTarget(_serialization.Model):
     """Properties pertaining to the BlobNfsTarget.
 
     :ivar target: Resource ID of the storage container.
     :vartype target: str
     :ivar usage_model: Identifies the StorageCache usage model to be used for this storage target.
     :vartype usage_model: str
@@ -1435,15 +1483,15 @@
 
 
 class CacheActiveDirectorySettings(_serialization.Model):
     """Active Directory settings used to join a cache to a domain.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar primary_dns_ip_address: Primary DNS IP address used to resolve the Active Directory
      domain controller's fully qualified domain name. Required.
     :vartype primary_dns_ip_address: str
     :ivar secondary_dns_ip_address: Secondary DNS IP address used to resolve the Active Directory
      domain controller's fully qualified domain name.
     :vartype secondary_dns_ip_address: str
@@ -1521,15 +1569,15 @@
         self.domain_joined = None
         self.credentials = credentials
 
 
 class CacheActiveDirectorySettingsCredentials(_serialization.Model):
     """Active Directory admin credentials used to join the HPC Cache to a domain.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar username: Username of the Active Directory domain administrator. This value is stored
      encrypted and not returned on response. Required.
     :vartype username: str
     :ivar password: Plain text password of the Active Directory domain administrator. This value is
      stored encrypted and not returned on response.
     :vartype password: str
@@ -2202,44 +2250,326 @@
     def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.timestamp = None
         self.message = None
 
 
-class ErrorResponse(_serialization.Model):
-    """Describes the format of Error response.
+class ErrorAdditionalInfo(_serialization.Model):
+    """The resource management error additional info.
 
-    :ivar code: Error code.
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar type: The additional info type.
+    :vartype type: str
+    :ivar info: The additional info.
+    :vartype info: JSON
+    """
+
+    _validation = {
+        "type": {"readonly": True},
+        "info": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "type": {"key": "type", "type": "str"},
+        "info": {"key": "info", "type": "object"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.type = None
+        self.info = None
+
+
+class ErrorDetail(_serialization.Model):
+    """The error detail.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar code: The error code.
     :vartype code: str
-    :ivar message: Error message indicating why the operation failed.
+    :ivar message: The error message.
     :vartype message: str
+    :ivar target: The error target.
+    :vartype target: str
+    :ivar details: The error details.
+    :vartype details: list[~azure.mgmt.storagecache.models.ErrorDetail]
+    :ivar additional_info: The error additional info.
+    :vartype additional_info: list[~azure.mgmt.storagecache.models.ErrorAdditionalInfo]
     """
 
+    _validation = {
+        "code": {"readonly": True},
+        "message": {"readonly": True},
+        "target": {"readonly": True},
+        "details": {"readonly": True},
+        "additional_info": {"readonly": True},
+    }
+
     _attribute_map = {
         "code": {"key": "code", "type": "str"},
         "message": {"key": "message", "type": "str"},
+        "target": {"key": "target", "type": "str"},
+        "details": {"key": "details", "type": "[ErrorDetail]"},
+        "additional_info": {"key": "additionalInfo", "type": "[ErrorAdditionalInfo]"},
     }
 
-    def __init__(self, *, code: Optional[str] = None, message: Optional[str] = None, **kwargs: Any) -> None:
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.code = None
+        self.message = None
+        self.target = None
+        self.details = None
+        self.additional_info = None
+
+
+class ErrorResponse(_serialization.Model):
+    """Common error response for all Azure Resource Manager APIs to return error details for failed
+    operations. (This also follows the OData error response format.).
+
+    :ivar error: The error object.
+    :vartype error: ~azure.mgmt.storagecache.models.ErrorDetail
+    """
+
+    _attribute_map = {
+        "error": {"key": "error", "type": "ErrorDetail"},
+    }
+
+    def __init__(self, *, error: Optional["_models.ErrorDetail"] = None, **kwargs: Any) -> None:
         """
-        :keyword code: Error code.
-        :paramtype code: str
-        :keyword message: Error message indicating why the operation failed.
-        :paramtype message: str
+        :keyword error: The error object.
+        :paramtype error: ~azure.mgmt.storagecache.models.ErrorDetail
         """
         super().__init__(**kwargs)
-        self.code = code
-        self.message = message
+        self.error = error
+
+
+class ImportJob(TrackedResource):  # pylint: disable=too-many-instance-attributes
+    """An import job instance. Follows Azure Resource Manager standards:
+    https://github.com/Azure/azure-resource-manager-rpc/blob/master/v1.0/resource-api-reference.md.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar id: Fully qualified resource ID for the resource. Ex -
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.storagecache.models.SystemData
+    :ivar tags: Resource tags.
+    :vartype tags: dict[str, str]
+    :ivar location: The geo-location where the resource lives. Required.
+    :vartype location: str
+    :ivar provisioning_state: ARM provisioning state. Known values are: "Succeeded", "Failed",
+     "Creating", "Deleting", "Updating", and "Canceled".
+    :vartype provisioning_state: str or
+     ~azure.mgmt.storagecache.models.ImportJobProvisioningStateType
+    :ivar import_prefixes: An array of blob paths/prefixes that get imported into the cluster
+     namespace. It has '/' as the default value.
+    :vartype import_prefixes: list[str]
+    :ivar conflict_resolution_mode: How the import job will handle conflicts. For example, if the
+     import job is trying to bring in a directory, but a file is at that path, how it handles it.
+     Fail indicates that the import job should stop immediately and not do anything with the
+     conflict. Skip indicates that it should pass over the conflict. OverwriteIfDirty causes the
+     import job to delete and re-import the file or directory if it is a conflicting type, is dirty,
+     or was not previously imported. OverwriteAlways extends OverwriteIfDirty to include releasing
+     files that had been restored but were not dirty. Please reference
+     https://learn.microsoft.com/en-us/azure/azure-managed-lustre/ for a thorough explanation of
+     these resolution modes. Known values are: "Fail", "Skip", "OverwriteIfDirty", and
+     "OverwriteAlways".
+    :vartype conflict_resolution_mode: str or
+     ~azure.mgmt.storagecache.models.ConflictResolutionMode
+    :ivar maximum_errors: Total non-conflict oriented errors the import job will tolerate before
+     exiting with failure. -1 means infinite. 0 means exit immediately and is the default.
+    :vartype maximum_errors: int
+    :ivar state: The state of the import job. InProgress indicates the import is still running.
+     Canceled indicates it has been canceled by the user. Completed indicates import finished,
+     successfully importing all discovered blobs into the Lustre namespace. CompletedPartial
+     indicates the import finished but some blobs either were found to be conflicting and could not
+     be imported or other errors were encountered. Failed means the import was unable to complete
+     due to a fatal error. Known values are: "InProgress", "Cancelling", "Canceled", "Completed",
+     "CompletedPartial", and "Failed".
+    :vartype state: str or ~azure.mgmt.storagecache.models.ImportStatusType
+    :ivar status_message: The status message of the import job.
+    :vartype status_message: str
+    :ivar total_blobs_walked: The total blob objects walked.
+    :vartype total_blobs_walked: int
+    :ivar blobs_walked_per_second: A recent and frequently updated rate of blobs walked per second.
+    :vartype blobs_walked_per_second: int
+    :ivar total_blobs_imported: The total blobs that have been imported since import began.
+    :vartype total_blobs_imported: int
+    :ivar blobs_imported_per_second: A recent and frequently updated rate of total files,
+     directories, and symlinks imported per second.
+    :vartype blobs_imported_per_second: int
+    :ivar last_completion_time: The time of the last completed archive operation.
+    :vartype last_completion_time: ~datetime.datetime
+    :ivar last_started_time: The time the latest archive operation started.
+    :vartype last_started_time: ~datetime.datetime
+    :ivar total_errors: Number of errors in the import job.
+    :vartype total_errors: int
+    :ivar total_conflicts: Number of conflicts in the import job.
+    :vartype total_conflicts: int
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+        "location": {"required": True},
+        "provisioning_state": {"readonly": True},
+        "state": {"readonly": True},
+        "status_message": {"readonly": True},
+        "total_blobs_walked": {"readonly": True},
+        "blobs_walked_per_second": {"readonly": True},
+        "total_blobs_imported": {"readonly": True},
+        "blobs_imported_per_second": {"readonly": True},
+        "last_completion_time": {"readonly": True},
+        "last_started_time": {"readonly": True},
+        "total_errors": {"readonly": True},
+        "total_conflicts": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+        "tags": {"key": "tags", "type": "{str}"},
+        "location": {"key": "location", "type": "str"},
+        "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
+        "import_prefixes": {"key": "properties.importPrefixes", "type": "[str]"},
+        "conflict_resolution_mode": {"key": "properties.conflictResolutionMode", "type": "str"},
+        "maximum_errors": {"key": "properties.maximumErrors", "type": "int"},
+        "state": {"key": "properties.status.state", "type": "str"},
+        "status_message": {"key": "properties.status.statusMessage", "type": "str"},
+        "total_blobs_walked": {"key": "properties.status.totalBlobsWalked", "type": "int"},
+        "blobs_walked_per_second": {"key": "properties.status.blobsWalkedPerSecond", "type": "int"},
+        "total_blobs_imported": {"key": "properties.status.totalBlobsImported", "type": "int"},
+        "blobs_imported_per_second": {"key": "properties.status.blobsImportedPerSecond", "type": "int"},
+        "last_completion_time": {"key": "properties.status.lastCompletionTime", "type": "iso-8601"},
+        "last_started_time": {"key": "properties.status.lastStartedTime", "type": "iso-8601"},
+        "total_errors": {"key": "properties.status.totalErrors", "type": "int"},
+        "total_conflicts": {"key": "properties.status.totalConflicts", "type": "int"},
+    }
+
+    def __init__(
+        self,
+        *,
+        location: str,
+        tags: Optional[Dict[str, str]] = None,
+        import_prefixes: Optional[List[str]] = None,
+        conflict_resolution_mode: Union[str, "_models.ConflictResolutionMode"] = "Fail",
+        maximum_errors: int = 0,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword tags: Resource tags.
+        :paramtype tags: dict[str, str]
+        :keyword location: The geo-location where the resource lives. Required.
+        :paramtype location: str
+        :keyword import_prefixes: An array of blob paths/prefixes that get imported into the cluster
+         namespace. It has '/' as the default value.
+        :paramtype import_prefixes: list[str]
+        :keyword conflict_resolution_mode: How the import job will handle conflicts. For example, if
+         the import job is trying to bring in a directory, but a file is at that path, how it handles
+         it. Fail indicates that the import job should stop immediately and not do anything with the
+         conflict. Skip indicates that it should pass over the conflict. OverwriteIfDirty causes the
+         import job to delete and re-import the file or directory if it is a conflicting type, is dirty,
+         or was not previously imported. OverwriteAlways extends OverwriteIfDirty to include releasing
+         files that had been restored but were not dirty. Please reference
+         https://learn.microsoft.com/en-us/azure/azure-managed-lustre/ for a thorough explanation of
+         these resolution modes. Known values are: "Fail", "Skip", "OverwriteIfDirty", and
+         "OverwriteAlways".
+        :paramtype conflict_resolution_mode: str or
+         ~azure.mgmt.storagecache.models.ConflictResolutionMode
+        :keyword maximum_errors: Total non-conflict oriented errors the import job will tolerate before
+         exiting with failure. -1 means infinite. 0 means exit immediately and is the default.
+        :paramtype maximum_errors: int
+        """
+        super().__init__(tags=tags, location=location, **kwargs)
+        self.provisioning_state = None
+        self.import_prefixes = import_prefixes
+        self.conflict_resolution_mode = conflict_resolution_mode
+        self.maximum_errors = maximum_errors
+        self.state = None
+        self.status_message = None
+        self.total_blobs_walked = None
+        self.blobs_walked_per_second = None
+        self.total_blobs_imported = None
+        self.blobs_imported_per_second = None
+        self.last_completion_time = None
+        self.last_started_time = None
+        self.total_errors = None
+        self.total_conflicts = None
+
+
+class ImportJobsListResult(_serialization.Model):
+    """Result of the request to list import jobs. It contains a list of import jobs and a URL link to
+    get the next set of results.
+
+    :ivar next_link: URL to get the next set of import job list results, if there are any.
+    :vartype next_link: str
+    :ivar value: List of import jobs.
+    :vartype value: list[~azure.mgmt.storagecache.models.ImportJob]
+    """
+
+    _attribute_map = {
+        "next_link": {"key": "nextLink", "type": "str"},
+        "value": {"key": "value", "type": "[ImportJob]"},
+    }
+
+    def __init__(
+        self, *, next_link: Optional[str] = None, value: Optional[List["_models.ImportJob"]] = None, **kwargs: Any
+    ) -> None:
+        """
+        :keyword next_link: URL to get the next set of import job list results, if there are any.
+        :paramtype next_link: str
+        :keyword value: List of import jobs.
+        :paramtype value: list[~azure.mgmt.storagecache.models.ImportJob]
+        """
+        super().__init__(**kwargs)
+        self.next_link = next_link
+        self.value = value
+
+
+class ImportJobUpdate(_serialization.Model):
+    """An import job update instance.
+
+    :ivar tags: Resource tags.
+    :vartype tags: dict[str, str]
+    """
+
+    _attribute_map = {
+        "tags": {"key": "tags", "type": "{str}"},
+    }
+
+    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
+        """
+        :keyword tags: Resource tags.
+        :paramtype tags: dict[str, str]
+        """
+        super().__init__(**kwargs)
+        self.tags = tags
 
 
 class KeyVaultKeyReference(_serialization.Model):
     """Describes a reference to key vault key.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar key_url: The URL referencing a key encryption key in key vault. Required.
     :vartype key_url: str
     :ivar source_vault: Describes a resource Id to source key vault. Required.
     :vartype source_vault: ~azure.mgmt.storagecache.models.KeyVaultKeyReferenceSourceVault
     """
 
@@ -2533,15 +2863,15 @@
         self.verification_timer = verification_timer
         self.write_back_timer = write_back_timer
 
 
 class NfsAccessPolicy(_serialization.Model):
     """A set of rules describing access policies applied to NFSv3 clients of the cache.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar name: Name identifying this policy. Access Policy names are not case sensitive. Required.
     :vartype name: str
     :ivar access_rules: The set of rules describing client accesses allowed under this policy.
      Required.
     :vartype access_rules: list[~azure.mgmt.storagecache.models.NfsAccessRule]
     """
@@ -2569,15 +2899,15 @@
         self.name = name
         self.access_rules = access_rules
 
 
 class NfsAccessRule(_serialization.Model):
     """Rule to place restrictions on portions of the cache namespace being presented to clients.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar scope: Scope for this rule. The scope and filter determine which clients match the rule.
      Required. Known values are: "default", "network", and "host".
     :vartype scope: str or ~azure.mgmt.storagecache.models.NfsAccessRuleScope
     :ivar filter: Filter applied to the scope for this rule. The filter's format depends on its
      scope. 'default' scope matches all clients and has no filter value. 'network' scope takes a
      filter in CIDR format (for example, 10.99.1.0/24). 'host' takes an IP address or fully
@@ -2670,15 +3000,15 @@
 
 
 class PrimingJob(_serialization.Model):
     """A priming job instance.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar priming_job_name: The priming job name. Required.
     :vartype priming_job_name: str
     :ivar priming_manifest_url: The URL for the priming manifest file to download. This file must
      be readable from the HPC Cache. When the file is in Azure blob storage the URL should include a
      Shared Access Signature (SAS) granting read permissions on the blob. Required.
     :vartype priming_manifest_url: str
@@ -2733,15 +3063,15 @@
         self.priming_job_details = None
         self.priming_job_percent_complete = None
 
 
 class PrimingJobIdParameter(_serialization.Model):
     """Object containing the priming job ID.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar priming_job_id: The unique identifier of the priming job. Required.
     :vartype priming_job_id: str
     """
 
     _validation = {
         "priming_job_id": {"required": True, "pattern": r"^[-0-9a-zA-Z_]{1,80}$"},
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/models/_patch.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/models/_storage_cache_management_client_enums.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/models/_storage_cache_management_client_enums.py`

 * *Files 16% similar despite different names*

```diff
@@ -68,14 +68,31 @@
 
     SYSTEM_ASSIGNED = "SystemAssigned"
     USER_ASSIGNED = "UserAssigned"
     SYSTEM_ASSIGNED_USER_ASSIGNED = "SystemAssigned, UserAssigned"
     NONE = "None"
 
 
+class ConflictResolutionMode(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """How the import job will handle conflicts. For example, if the import job is trying to bring in
+    a directory, but a file is at that path, how it handles it. Fail indicates that the import job
+    should stop immediately and not do anything with the conflict. Skip indicates that it should
+    pass over the conflict. OverwriteIfDirty causes the import job to delete and re-import the file
+    or directory if it is a conflicting type, is dirty, or was not previously imported.
+    OverwriteAlways extends OverwriteIfDirty to include releasing files that had been restored but
+    were not dirty. Please reference https://learn.microsoft.com/en-us/azure/azure-managed-lustre/
+    for a thorough explanation of these resolution modes.
+    """
+
+    FAIL = "Fail"
+    SKIP = "Skip"
+    OVERWRITE_IF_DIRTY = "OverwriteIfDirty"
+    OVERWRITE_ALWAYS = "OverwriteAlways"
+
+
 class CreatedByType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The type of identity that created the resource."""
 
     USER = "User"
     APPLICATION = "Application"
     MANAGED_IDENTITY = "ManagedIdentity"
     KEY = "Key"
@@ -124,14 +141,41 @@
     UPGRADING = "Upgrading"
     FLUSHING = "Flushing"
     WAITING_FOR_KEY = "WaitingForKey"
     START_FAILED = "StartFailed"
     UPGRADE_FAILED = "UpgradeFailed"
 
 
+class ImportJobProvisioningStateType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """ARM provisioning state."""
+
+    SUCCEEDED = "Succeeded"
+    FAILED = "Failed"
+    CREATING = "Creating"
+    DELETING = "Deleting"
+    UPDATING = "Updating"
+    CANCELED = "Canceled"
+
+
+class ImportStatusType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The state of the import job. InProgress indicates the import is still running. Canceled
+    indicates it has been canceled by the user. Completed indicates import finished, successfully
+    importing all discovered blobs into the Lustre namespace. CompletedPartial indicates the import
+    finished but some blobs either were found to be conflicting and could not be imported or other
+    errors were encountered. Failed means the import was unable to complete due to a fatal error.
+    """
+
+    IN_PROGRESS = "InProgress"
+    CANCELLING = "Cancelling"
+    CANCELED = "Canceled"
+    COMPLETED = "Completed"
+    COMPLETED_PARTIAL = "CompletedPartial"
+    FAILED = "Failed"
+
+
 class MaintenanceDayOfWeekType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Day of the week on which the maintenance window will occur."""
 
     MONDAY = "Monday"
     TUESDAY = "Tuesday"
     WEDNESDAY = "Wednesday"
     THURSDAY = "Thursday"
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/__init__.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._aml_filesystems_operations import AmlFilesystemsOperations
+from ._import_jobs_operations import ImportJobsOperations
 from ._storage_cache_management_client_operations import StorageCacheManagementClientOperationsMixin
 from ._operations import Operations
 from ._skus_operations import SkusOperations
 from ._usage_models_operations import UsageModelsOperations
 from ._asc_operations_operations import AscOperationsOperations
 from ._asc_usages_operations import AscUsagesOperations
 from ._caches_operations import CachesOperations
@@ -19,14 +20,15 @@
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "AmlFilesystemsOperations",
+    "ImportJobsOperations",
     "StorageCacheManagementClientOperationsMixin",
     "Operations",
     "SkusOperations",
     "UsageModelsOperations",
     "AscOperationsOperations",
     "AscUsagesOperations",
     "CachesOperations",
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/_aml_filesystems_operations.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/_aml_filesystems_operations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -39,15 +39,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/amlFilesystems")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
@@ -63,15 +63,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems",
     )  # pylint: disable=line-too-long
@@ -95,15 +95,15 @@
 
 def build_delete_request(
     resource_group_name: str, aml_filesystem_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}",
     )  # pylint: disable=line-too-long
@@ -135,15 +135,15 @@
 
 def build_get_request(
     resource_group_name: str, aml_filesystem_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}",
     )  # pylint: disable=line-too-long
@@ -175,15 +175,15 @@
 
 def build_create_or_update_request(
     resource_group_name: str, aml_filesystem_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}",
@@ -218,15 +218,15 @@
 
 def build_update_request(
     resource_group_name: str, aml_filesystem_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}",
@@ -261,15 +261,15 @@
 
 def build_archive_request(
     resource_group_name: str, aml_filesystem_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}/archive",
@@ -304,15 +304,15 @@
 
 def build_cancel_archive_request(
     resource_group_name: str, aml_filesystem_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}/cancelArchive",
     )  # pylint: disable=line-too-long
@@ -361,15 +361,14 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, **kwargs: Any) -> Iterable["_models.AmlFilesystem"]:
         """Returns all AML file systems the user has access to under a subscription.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either AmlFilesystem or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.storagecache.models.AmlFilesystem]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -383,76 +382,72 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("AmlFilesystemsListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/amlFilesystems"}
-
     @distributed_trace
     def list_by_resource_group(self, resource_group_name: str, **kwargs: Any) -> Iterable["_models.AmlFilesystem"]:
         """Returns all AML file systems the user has access to under a resource group.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either AmlFilesystem or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.storagecache.models.AmlFilesystem]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -466,71 +461,66 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_resource_group_request(
+                _request = build_list_by_resource_group_request(
                     resource_group_name=resource_group_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_resource_group.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("AmlFilesystemsListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list_by_resource_group.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems"
-    }
-
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, aml_filesystem_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -540,29 +530,28 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             aml_filesystem_name=aml_filesystem_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -571,38 +560,26 @@
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(self, resource_group_name: str, aml_filesystem_name: str, **kwargs: Any) -> LROPoller[None]:
         """Schedules an AML file system for deletion.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
          and hyphens. Start and end with alphanumeric. Required.
         :type aml_filesystem_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -621,48 +598,43 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: PollingMethod = cast(
                 PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
             )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}"
-    }
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     @distributed_trace
     def get(self, resource_group_name: str, aml_filesystem_name: str, **kwargs: Any) -> _models.AmlFilesystem:
         """Returns an AML file system.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
          and hyphens. Start and end with alphanumeric. Required.
         :type aml_filesystem_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: AmlFilesystem or the result of cls(response)
         :rtype: ~azure.mgmt.storagecache.models.AmlFilesystem
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -673,53 +645,48 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AmlFilesystem] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             aml_filesystem_name=aml_filesystem_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("AmlFilesystem", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}"
-    }
+        return deserialized  # type: ignore
 
     def _create_or_update_initial(
         self,
         resource_group_name: str,
         aml_filesystem_name: str,
-        aml_filesystem: Union[_models.AmlFilesystem, IO],
+        aml_filesystem: Union[_models.AmlFilesystem, IO[bytes]],
         **kwargs: Any
     ) -> _models.AmlFilesystem:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -737,32 +704,31 @@
         _json = None
         _content = None
         if isinstance(aml_filesystem, (IOBase, bytes)):
             _content = aml_filesystem
         else:
             _json = self._serialize.body(aml_filesystem, "AmlFilesystem")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             aml_filesystem_name=aml_filesystem_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -779,18 +745,14 @@
             deserialized = self._deserialize("AmlFilesystem", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}"
-    }
-
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         aml_filesystem_name: str,
         aml_filesystem: _models.AmlFilesystem,
         *,
@@ -808,34 +770,26 @@
         :param aml_filesystem: Object containing the user-selectable properties of the AML file system.
          If read-only properties are included, they must match the existing values of those properties.
          Required.
         :type aml_filesystem: ~azure.mgmt.storagecache.models.AmlFilesystem
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either AmlFilesystem or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.storagecache.models.AmlFilesystem]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         aml_filesystem_name: str,
-        aml_filesystem: IO,
+        aml_filesystem: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.AmlFilesystem]:
         """Create or update an AML file system.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
@@ -843,63 +797,44 @@
         :type resource_group_name: str
         :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
          and hyphens. Start and end with alphanumeric. Required.
         :type aml_filesystem_name: str
         :param aml_filesystem: Object containing the user-selectable properties of the AML file system.
          If read-only properties are included, they must match the existing values of those properties.
          Required.
-        :type aml_filesystem: IO
+        :type aml_filesystem: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either AmlFilesystem or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.storagecache.models.AmlFilesystem]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create_or_update(
         self,
         resource_group_name: str,
         aml_filesystem_name: str,
-        aml_filesystem: Union[_models.AmlFilesystem, IO],
+        aml_filesystem: Union[_models.AmlFilesystem, IO[bytes]],
         **kwargs: Any
     ) -> LROPoller[_models.AmlFilesystem]:
         """Create or update an AML file system.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
          and hyphens. Start and end with alphanumeric. Required.
         :type aml_filesystem_name: str
         :param aml_filesystem: Object containing the user-selectable properties of the AML file system.
          If read-only properties are included, they must match the existing values of those properties.
-         Is either a AmlFilesystem type or a IO type. Required.
-        :type aml_filesystem: ~azure.mgmt.storagecache.models.AmlFilesystem or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         Is either a AmlFilesystem type or a IO[bytes] type. Required.
+        :type aml_filesystem: ~azure.mgmt.storagecache.models.AmlFilesystem or IO[bytes]
         :return: An instance of LROPoller that returns either AmlFilesystem or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.storagecache.models.AmlFilesystem]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -923,43 +858,41 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("AmlFilesystem", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: PollingMethod = cast(
                 PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
             )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[_models.AmlFilesystem].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}"
-    }
+        return LROPoller[_models.AmlFilesystem](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     def _update_initial(
         self,
         resource_group_name: str,
         aml_filesystem_name: str,
-        aml_filesystem: Union[_models.AmlFilesystemUpdate, IO],
+        aml_filesystem: Union[_models.AmlFilesystemUpdate, IO[bytes]],
         **kwargs: Any
     ) -> Optional[_models.AmlFilesystem]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -977,32 +910,31 @@
         _json = None
         _content = None
         if isinstance(aml_filesystem, (IOBase, bytes)):
             _content = aml_filesystem
         else:
             _json = self._serialize.body(aml_filesystem, "AmlFilesystemUpdate")
 
-        request = build_update_request(
+        _request = build_update_request(
             resource_group_name=resource_group_name,
             aml_filesystem_name=aml_filesystem_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1015,21 +947,17 @@
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["azure-async-operation"] = self._deserialize(
                 "str", response.headers.get("azure-async-operation")
             )
 
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)
-
-        return deserialized
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
-    _update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     def begin_update(
         self,
         resource_group_name: str,
         aml_filesystem_name: str,
         aml_filesystem: _models.AmlFilesystemUpdate,
@@ -1048,34 +976,26 @@
         :param aml_filesystem: Object containing the user-selectable properties of the AML file system.
          If read-only properties are included, they must match the existing values of those properties.
          Required.
         :type aml_filesystem: ~azure.mgmt.storagecache.models.AmlFilesystemUpdate
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either AmlFilesystem or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.storagecache.models.AmlFilesystem]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_update(
         self,
         resource_group_name: str,
         aml_filesystem_name: str,
-        aml_filesystem: IO,
+        aml_filesystem: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.AmlFilesystem]:
         """Update an AML file system instance.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
@@ -1083,63 +1003,44 @@
         :type resource_group_name: str
         :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
          and hyphens. Start and end with alphanumeric. Required.
         :type aml_filesystem_name: str
         :param aml_filesystem: Object containing the user-selectable properties of the AML file system.
          If read-only properties are included, they must match the existing values of those properties.
          Required.
-        :type aml_filesystem: IO
+        :type aml_filesystem: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either AmlFilesystem or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.storagecache.models.AmlFilesystem]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_update(
         self,
         resource_group_name: str,
         aml_filesystem_name: str,
-        aml_filesystem: Union[_models.AmlFilesystemUpdate, IO],
+        aml_filesystem: Union[_models.AmlFilesystemUpdate, IO[bytes]],
         **kwargs: Any
     ) -> LROPoller[_models.AmlFilesystem]:
         """Update an AML file system instance.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
          and hyphens. Start and end with alphanumeric. Required.
         :type aml_filesystem_name: str
         :param aml_filesystem: Object containing the user-selectable properties of the AML file system.
          If read-only properties are included, they must match the existing values of those properties.
-         Is either a AmlFilesystemUpdate type or a IO type. Required.
-        :type aml_filesystem: ~azure.mgmt.storagecache.models.AmlFilesystemUpdate or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         Is either a AmlFilesystemUpdate type or a IO[bytes] type. Required.
+        :type aml_filesystem: ~azure.mgmt.storagecache.models.AmlFilesystemUpdate or IO[bytes]
         :return: An instance of LROPoller that returns either AmlFilesystem or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.storagecache.models.AmlFilesystem]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -1163,37 +1064,35 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("AmlFilesystem", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: PollingMethod = cast(
                 PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
             )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[_models.AmlFilesystem].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}"
-    }
+        return LROPoller[_models.AmlFilesystem](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     @overload
     def archive(  # pylint: disable=inconsistent-return-statements
         self,
         resource_group_name: str,
         aml_filesystem_name: str,
         archive_info: Optional[_models.AmlFilesystemArchiveInfo] = None,
@@ -1210,72 +1109,66 @@
          and hyphens. Start and end with alphanumeric. Required.
         :type aml_filesystem_name: str
         :param archive_info: Information about the archive operation. Default value is None.
         :type archive_info: ~azure.mgmt.storagecache.models.AmlFilesystemArchiveInfo
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def archive(  # pylint: disable=inconsistent-return-statements
         self,
         resource_group_name: str,
         aml_filesystem_name: str,
-        archive_info: Optional[IO] = None,
+        archive_info: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> None:
         """Archive data from the AML file system.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
          and hyphens. Start and end with alphanumeric. Required.
         :type aml_filesystem_name: str
         :param archive_info: Information about the archive operation. Default value is None.
-        :type archive_info: IO
+        :type archive_info: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def archive(  # pylint: disable=inconsistent-return-statements
         self,
         resource_group_name: str,
         aml_filesystem_name: str,
-        archive_info: Optional[Union[_models.AmlFilesystemArchiveInfo, IO]] = None,
+        archive_info: Optional[Union[_models.AmlFilesystemArchiveInfo, IO[bytes]]] = None,
         **kwargs: Any
     ) -> None:
         """Archive data from the AML file system.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
          and hyphens. Start and end with alphanumeric. Required.
         :type aml_filesystem_name: str
         :param archive_info: Information about the archive operation. Is either a
-         AmlFilesystemArchiveInfo type or a IO type. Default value is None.
-        :type archive_info: ~azure.mgmt.storagecache.models.AmlFilesystemArchiveInfo or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         AmlFilesystemArchiveInfo type or a IO[bytes] type. Default value is None.
+        :type archive_info: ~azure.mgmt.storagecache.models.AmlFilesystemArchiveInfo or IO[bytes]
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -1298,60 +1191,54 @@
             _content = archive_info
         else:
             if archive_info is not None:
                 _json = self._serialize.body(archive_info, "AmlFilesystemArchiveInfo")
             else:
                 _json = None
 
-        request = build_archive_request(
+        _request = build_archive_request(
             resource_group_name=resource_group_name,
             aml_filesystem_name=aml_filesystem_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.archive.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         if cls:
-            return cls(pipeline_response, None, {})
-
-    archive.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}/archive"
-    }
+            return cls(pipeline_response, None, {})  # type: ignore
 
     @distributed_trace
     def cancel_archive(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, aml_filesystem_name: str, **kwargs: Any
     ) -> None:
         """Cancel archiving data from the AML file system.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
          and hyphens. Start and end with alphanumeric. Required.
         :type aml_filesystem_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -1362,36 +1249,31 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_cancel_archive_request(
+        _request = build_cancel_archive_request(
             resource_group_name=resource_group_name,
             aml_filesystem_name=aml_filesystem_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.cancel_archive.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         if cls:
-            return cls(pipeline_response, None, {})
-
-    cancel_archive.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/amlFilesystems/{amlFilesystemName}/cancelArchive"
-    }
+            return cls(pipeline_response, None, {})  # type: ignore
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/_asc_operations_operations.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/_asc_operations_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -34,15 +34,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_get_request(location: str, operation_id: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/locations/{location}/ascOperations/{operationId}",
     )  # pylint: disable=line-too-long
@@ -86,15 +86,14 @@
     def get(self, location: str, operation_id: str, **kwargs: Any) -> _models.AscOperation:
         """Gets the status of an asynchronous operation for the Azure HPC Cache.
 
         :param location: The name of Azure region. Required.
         :type location: str
         :param operation_id: The ID of an ongoing async operation. Required.
         :type operation_id: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: AscOperation or the result of cls(response)
         :rtype: ~azure.mgmt.storagecache.models.AscOperation
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -105,40 +104,35 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AscOperation] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             location=location,
             operation_id=operation_id,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("AscOperation", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/locations/{location}/ascOperations/{operationId}"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/_asc_usages_operations.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/_asc_usages_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -36,15 +36,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(location: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/locations/{location}/usages"
     )  # pylint: disable=line-too-long
     path_format_arguments = {
@@ -84,15 +84,14 @@
 
     @distributed_trace
     def list(self, location: str, **kwargs: Any) -> Iterable["_models.ResourceUsage"]:
         """Gets the quantity used and quota limit for resources.
 
         :param location: The name of the region to query for usage information. Required.
         :type location: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ResourceUsage or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.storagecache.models.ResourceUsage]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -106,63 +105,58 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     location=location,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ResourceUsagesListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
-
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/locations/{location}/usages"
-    }
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/_operations.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -36,15 +36,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.StorageCache/operations")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -74,15 +74,14 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, **kwargs: Any) -> Iterable["_models.ApiOperation"]:
         """Lists all of the available Resource Provider operations.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ApiOperation or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.storagecache.models.ApiOperation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -96,59 +95,56 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ApiOperationListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
-
-    list.metadata = {"url": "/providers/Microsoft.StorageCache/operations"}
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/_patch.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/_skus_operations.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/_usage_models_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -36,19 +36,19 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
-    _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/skus")
+    _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/usageModels")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -56,105 +56,101 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class SkusOperations:
+class UsageModelsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.storagecache.StorageCacheManagementClient`'s
-        :attr:`skus` attribute.
+        :attr:`usage_models` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, **kwargs: Any) -> Iterable["_models.ResourceSku"]:
-        """Get the list of StorageCache.Cache SKUs available to this subscription.
+    def list(self, **kwargs: Any) -> Iterable["_models.UsageModel"]:
+        """Get the list of cache usage models available to this subscription.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either ResourceSku or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.storagecache.models.ResourceSku]
+        :return: An iterator like instance of either UsageModel or the result of cls(response)
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.storagecache.models.UsageModel]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.ResourceSkusResult] = kwargs.pop("cls", None)
+        cls: ClsType[_models.UsageModelsResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
-            deserialized = self._deserialize("ResourceSkusResult", pipeline_response)
+            deserialized = self._deserialize("UsageModelsResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
-
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/skus"}
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/_storage_cache_management_client_operations.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/_storage_cache_management_client_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -35,15 +35,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_check_aml_fs_subnets_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/checkAmlFSSubnets"
     )
@@ -60,19 +60,21 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_get_required_aml_fs_subnets_size_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
+def build_get_required_aml_fs_subnets_size_request(  # pylint: disable=name-too-long
+    subscription_id: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/getRequiredAmlFSSubnetsSize"
     )  # pylint: disable=line-too-long
@@ -89,15 +91,17 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class StorageCacheManagementClientOperationsMixin(StorageCacheManagementClientMixinABC):
+class StorageCacheManagementClientOperationsMixin(  # pylint: disable=name-too-long
+    StorageCacheManagementClientMixinABC
+):
     @overload
     def check_aml_fs_subnets(  # pylint: disable=inconsistent-return-statements
         self,
         aml_filesystem_subnet_info: Optional[_models.AmlFilesystemSubnetInfo] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
@@ -106,51 +110,52 @@
 
         :param aml_filesystem_subnet_info: Information about the subnets to validate. Default value is
          None.
         :type aml_filesystem_subnet_info: ~azure.mgmt.storagecache.models.AmlFilesystemSubnetInfo
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def check_aml_fs_subnets(  # pylint: disable=inconsistent-return-statements
-        self, aml_filesystem_subnet_info: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
+        self,
+        aml_filesystem_subnet_info: Optional[IO[bytes]] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
     ) -> None:
         """Check that subnets will be valid for AML file system create calls.
 
         :param aml_filesystem_subnet_info: Information about the subnets to validate. Default value is
          None.
-        :type aml_filesystem_subnet_info: IO
+        :type aml_filesystem_subnet_info: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def check_aml_fs_subnets(  # pylint: disable=inconsistent-return-statements
-        self, aml_filesystem_subnet_info: Optional[Union[_models.AmlFilesystemSubnetInfo, IO]] = None, **kwargs: Any
+        self,
+        aml_filesystem_subnet_info: Optional[Union[_models.AmlFilesystemSubnetInfo, IO[bytes]]] = None,
+        **kwargs: Any
     ) -> None:
         """Check that subnets will be valid for AML file system create calls.
 
         :param aml_filesystem_subnet_info: Information about the subnets to validate. Is either a
-         AmlFilesystemSubnetInfo type or a IO type. Default value is None.
-        :type aml_filesystem_subnet_info: ~azure.mgmt.storagecache.models.AmlFilesystemSubnetInfo or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         AmlFilesystemSubnetInfo type or a IO[bytes] type. Default value is None.
+        :type aml_filesystem_subnet_info: ~azure.mgmt.storagecache.models.AmlFilesystemSubnetInfo or
+         IO[bytes]
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -178,44 +183,39 @@
             _content = aml_filesystem_subnet_info
         else:
             if aml_filesystem_subnet_info is not None:
                 _json = self._serialize.body(aml_filesystem_subnet_info, "AmlFilesystemSubnetInfo")
             else:
                 _json = None
 
-        request = build_check_aml_fs_subnets_request(
+        _request = build_check_aml_fs_subnets_request(
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.check_aml_fs_subnets.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         if cls:
-            return cls(pipeline_response, None, {})
-
-    check_aml_fs_subnets.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/checkAmlFSSubnets"
-    }
+            return cls(pipeline_response, None, {})  # type: ignore
 
     @overload
     def get_required_aml_fs_subnets_size(
         self,
         required_aml_filesystem_subnets_size_info: Optional[_models.RequiredAmlFilesystemSubnetsSizeInfo] = None,
         *,
         content_type: str = "application/json",
@@ -226,61 +226,55 @@
         :param required_aml_filesystem_subnets_size_info: Information to determine the number of
          available IPs a subnet will need to host the AML file system. Default value is None.
         :type required_aml_filesystem_subnets_size_info:
          ~azure.mgmt.storagecache.models.RequiredAmlFilesystemSubnetsSizeInfo
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RequiredAmlFilesystemSubnetsSize or the result of cls(response)
         :rtype: ~azure.mgmt.storagecache.models.RequiredAmlFilesystemSubnetsSize
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def get_required_aml_fs_subnets_size(
         self,
-        required_aml_filesystem_subnets_size_info: Optional[IO] = None,
+        required_aml_filesystem_subnets_size_info: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.RequiredAmlFilesystemSubnetsSize:
         """Get the number of available IP addresses needed for the AML file system information provided.
 
         :param required_aml_filesystem_subnets_size_info: Information to determine the number of
          available IPs a subnet will need to host the AML file system. Default value is None.
-        :type required_aml_filesystem_subnets_size_info: IO
+        :type required_aml_filesystem_subnets_size_info: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RequiredAmlFilesystemSubnetsSize or the result of cls(response)
         :rtype: ~azure.mgmt.storagecache.models.RequiredAmlFilesystemSubnetsSize
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def get_required_aml_fs_subnets_size(
         self,
         required_aml_filesystem_subnets_size_info: Optional[
-            Union[_models.RequiredAmlFilesystemSubnetsSizeInfo, IO]
+            Union[_models.RequiredAmlFilesystemSubnetsSizeInfo, IO[bytes]]
         ] = None,
         **kwargs: Any
     ) -> _models.RequiredAmlFilesystemSubnetsSize:
         """Get the number of available IP addresses needed for the AML file system information provided.
 
         :param required_aml_filesystem_subnets_size_info: Information to determine the number of
          available IPs a subnet will need to host the AML file system. Is either a
-         RequiredAmlFilesystemSubnetsSizeInfo type or a IO type. Default value is None.
+         RequiredAmlFilesystemSubnetsSizeInfo type or a IO[bytes] type. Default value is None.
         :type required_aml_filesystem_subnets_size_info:
-         ~azure.mgmt.storagecache.models.RequiredAmlFilesystemSubnetsSizeInfo or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ~azure.mgmt.storagecache.models.RequiredAmlFilesystemSubnetsSizeInfo or IO[bytes]
         :return: RequiredAmlFilesystemSubnetsSize or the result of cls(response)
         :rtype: ~azure.mgmt.storagecache.models.RequiredAmlFilesystemSubnetsSize
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -305,41 +299,36 @@
             if required_aml_filesystem_subnets_size_info is not None:
                 _json = self._serialize.body(
                     required_aml_filesystem_subnets_size_info, "RequiredAmlFilesystemSubnetsSizeInfo"
                 )
             else:
                 _json = None
 
-        request = build_get_required_aml_fs_subnets_size_request(
+        _request = build_get_required_aml_fs_subnets_size_request(
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.get_required_aml_fs_subnets_size.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("RequiredAmlFilesystemSubnetsSize", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get_required_aml_fs_subnets_size.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/getRequiredAmlFSSubnetsSize"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/_storage_target_operations.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/aio/operations/_import_jobs_operations.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,210 +1,74 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, Callable, Dict, Optional, TypeVar, Union, cast
+from io import IOBase
+from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+import urllib.parse
 
+from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import HttpResponse
-from azure.core.polling import LROPoller, NoPolling, PollingMethod
+from azure.core.pipeline.transport import AsyncHttpResponse
+from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
+from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
-from azure.mgmt.core.polling.arm_polling import ARMPolling
+from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
-from .. import models as _models
-from .._serialization import Serializer
-from .._vendor import StorageCacheManagementClientMixinABC, _convert_request
+from ... import models as _models
+from ..._vendor import _convert_request
+from ...operations._import_jobs_operations import (
+    build_create_or_update_request,
+    build_delete_request,
+    build_get_request,
+    build_list_by_aml_filesystem_request,
+    build_update_request,
+)
+from .._vendor import StorageCacheManagementClientMixinABC
 
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
-
-_SERIALIZER = Serializer()
-_SERIALIZER.client_side_validation = False
-
-
-def build_flush_request(
-    resource_group_name: str, cache_name: str, storage_target_name: str, subscription_id: str, **kwargs: Any
-) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = kwargs.pop(
-        "template_url",
-        "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/flush",
-    )  # pylint: disable=line-too-long
-    path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-        "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
-        "storageTargetName": _SERIALIZER.url(
-            "storage_target_name", storage_target_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"
-        ),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_suspend_request(
-    resource_group_name: str, cache_name: str, storage_target_name: str, subscription_id: str, **kwargs: Any
-) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = kwargs.pop(
-        "template_url",
-        "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/suspend",
-    )  # pylint: disable=line-too-long
-    path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-        "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
-        "storageTargetName": _SERIALIZER.url(
-            "storage_target_name", storage_target_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"
-        ),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_resume_request(
-    resource_group_name: str, cache_name: str, storage_target_name: str, subscription_id: str, **kwargs: Any
-) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = kwargs.pop(
-        "template_url",
-        "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/resume",
-    )  # pylint: disable=line-too-long
-    path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-        "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
-        "storageTargetName": _SERIALIZER.url(
-            "storage_target_name", storage_target_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"
-        ),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_invalidate_request(
-    resource_group_name: str, cache_name: str, storage_target_name: str, subscription_id: str, **kwargs: Any
-) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = kwargs.pop(
-        "template_url",
-        "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/invalidate",
-    )  # pylint: disable=line-too-long
-    path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-        "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
-        "storageTargetName": _SERIALIZER.url(
-            "storage_target_name", storage_target_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"
-        ),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
-    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
-
-class StorageTargetOperations:
+class ImportJobsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.storagecache.StorageCacheManagementClient`'s
-        :attr:`storage_target` attribute.
+        :class:`~azure.mgmt.storagecache.aio.StorageCacheManagementClient`'s
+        :attr:`import_jobs` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    def _flush_initial(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
+    async def _delete_initial(  # pylint: disable=inconsistent-return-statements
+        self, resource_group_name: str, aml_filesystem_name: str, import_job_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -212,500 +76,700 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_flush_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
-            cache_name=cache_name,
-            storage_target_name=storage_target_name,
+            aml_filesystem_name=aml_filesystem_name,
+            import_job_name=import_job_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._flush_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 202, 204]:
+        if response.status_code not in [202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _flush_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/flush"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
-    @distributed_trace
-    def begin_flush(
-        self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
-    ) -> LROPoller[None]:
-        """Tells the cache to write all dirty data to the Storage Target's backend storage. Client
-        requests to this storage target's namespace will return errors until the flush operation
-        completes.
+    @distributed_trace_async
+    async def begin_delete(
+        self, resource_group_name: str, aml_filesystem_name: str, import_job_name: str, **kwargs: Any
+    ) -> AsyncLROPoller[None]:
+        """Schedules an import job for deletion.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
-         from the [-0-9a-zA-Z_] char class. Required.
-        :type cache_name: str
-        :param storage_target_name: Name of Storage Target. Required.
-        :type storage_target_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either None or the result of cls(response)
-        :rtype: ~azure.core.polling.LROPoller[None]
+        :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
+         and hyphens. Start and end with alphanumeric. Required.
+        :type aml_filesystem_name: str
+        :param import_job_name: Name for the import job. Allows alphanumerics, underscores, and
+         hyphens. Start and end with alphanumeric. Required.
+        :type import_job_name: str
+        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
-        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = self._flush_initial(  # type: ignore
+            raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
-                cache_name=cache_name,
-                storage_target_name=storage_target_name,
+                aml_filesystem_name=aml_filesystem_name,
+                import_job_name=import_job_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
-            polling_method: PollingMethod = cast(
-                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
             )
         elif polling is False:
-            polling_method = cast(PollingMethod, NoPolling())
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_flush.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/flush"
-    }
+    @distributed_trace_async
+    async def get(
+        self, resource_group_name: str, aml_filesystem_name: str, import_job_name: str, **kwargs: Any
+    ) -> _models.ImportJob:
+        """Returns an import job.
 
-    def _suspend_initial(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
-    ) -> None:
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
+         and hyphens. Start and end with alphanumeric. Required.
+        :type aml_filesystem_name: str
+        :param import_job_name: Name for the import job. Allows alphanumerics, underscores, and
+         hyphens. Start and end with alphanumeric. Required.
+        :type import_job_name: str
+        :return: ImportJob or the result of cls(response)
+        :rtype: ~azure.mgmt.storagecache.models.ImportJob
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[None] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ImportJob] = kwargs.pop("cls", None)
 
-        request = build_suspend_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
-            cache_name=cache_name,
-            storage_target_name=storage_target_name,
+            aml_filesystem_name=aml_filesystem_name,
+            import_job_name=import_job_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._suspend_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 202, 204]:
+        if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        response_headers = {}
-        if response.status_code == 202:
-            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
-            response_headers["Azure-AsyncOperation"] = self._deserialize(
-                "str", response.headers.get("Azure-AsyncOperation")
-            )
+        deserialized = self._deserialize("ImportJob", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _suspend_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/suspend"
-    }
-
-    @distributed_trace
-    def begin_suspend(
-        self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
-    ) -> LROPoller[None]:
-        """Suspends client access to a storage target.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
-         from the [-0-9a-zA-Z_] char class. Required.
-        :type cache_name: str
-        :param storage_target_name: Name of Storage Target. Required.
-        :type storage_target_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either None or the result of cls(response)
-        :rtype: ~azure.core.polling.LROPoller[None]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[None] = kwargs.pop("cls", None)
-        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
-        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
-        if cont_token is None:
-            raw_result = self._suspend_initial(  # type: ignore
-                resource_group_name=resource_group_name,
-                cache_name=cache_name,
-                storage_target_name=storage_target_name,
-                api_version=api_version,
-                cls=lambda x, y, z: x,
-                headers=_headers,
-                params=_params,
-                **kwargs
-            )
-        kwargs.pop("error_map", None)
-
-        def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
-            if cls:
-                return cls(pipeline_response, None, {})
-
-        if polling is True:
-            polling_method: PollingMethod = cast(
-                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
-            )
-        elif polling is False:
-            polling_method = cast(PollingMethod, NoPolling())
-        else:
-            polling_method = polling
-        if cont_token:
-            return LROPoller.from_continuation_token(
-                polling_method=polling_method,
-                continuation_token=cont_token,
-                client=self._client,
-                deserialization_callback=get_long_running_output,
-            )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    begin_suspend.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/suspend"
-    }
+        return deserialized  # type: ignore
 
-    def _resume_initial(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
-    ) -> None:
+    async def _create_or_update_initial(
+        self,
+        resource_group_name: str,
+        aml_filesystem_name: str,
+        import_job_name: str,
+        import_job: Union[_models.ImportJob, IO[bytes]],
+        **kwargs: Any
+    ) -> _models.ImportJob:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        _headers = kwargs.pop("headers", {}) or {}
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[None] = kwargs.pop("cls", None)
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ImportJob] = kwargs.pop("cls", None)
 
-        request = build_resume_request(
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(import_job, (IOBase, bytes)):
+            _content = import_job
+        else:
+            _json = self._serialize.body(import_job, "ImportJob")
+
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
-            cache_name=cache_name,
-            storage_target_name=storage_target_name,
+            aml_filesystem_name=aml_filesystem_name,
+            import_job_name=import_job_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._resume_initial.metadata["url"],
+            content_type=content_type,
+            json=_json,
+            content=_content,
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 202, 204]:
+        if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
-        if response.status_code == 202:
-            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
-            response_headers["Azure-AsyncOperation"] = self._deserialize(
-                "str", response.headers.get("Azure-AsyncOperation")
+        if response.status_code == 200:
+            deserialized = self._deserialize("ImportJob", pipeline_response)
+
+        if response.status_code == 201:
+            response_headers["azure-async-operation"] = self._deserialize(
+                "str", response.headers.get("azure-async-operation")
             )
 
+            deserialized = self._deserialize("ImportJob", pipeline_response)
+
         if cls:
-            return cls(pipeline_response, None, response_headers)
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
-    _resume_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/resume"
-    }
+        return deserialized  # type: ignore
 
-    @distributed_trace
-    def begin_resume(
-        self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
-    ) -> LROPoller[None]:
-        """Resumes client access to a previously suspended storage target.
+    @overload
+    async def begin_create_or_update(
+        self,
+        resource_group_name: str,
+        aml_filesystem_name: str,
+        import_job_name: str,
+        import_job: _models.ImportJob,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.ImportJob]:
+        """Create or update an import job. Import jobs are automatically deleted 72 hours after
+        completion.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
-         from the [-0-9a-zA-Z_] char class. Required.
-        :type cache_name: str
-        :param storage_target_name: Name of Storage Target. Required.
-        :type storage_target_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either None or the result of cls(response)
-        :rtype: ~azure.core.polling.LROPoller[None]
+        :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
+         and hyphens. Start and end with alphanumeric. Required.
+        :type aml_filesystem_name: str
+        :param import_job_name: Name for the import job. Allows alphanumerics, underscores, and
+         hyphens. Start and end with alphanumeric. Required.
+        :type import_job_name: str
+        :param import_job: Object containing the user-selectable properties of the import job. If
+         read-only properties are included, they must match the existing values of those properties.
+         Required.
+        :type import_job: ~azure.mgmt.storagecache.models.ImportJob
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: An instance of AsyncLROPoller that returns either ImportJob or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.ImportJob]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        _headers = kwargs.pop("headers", {}) or {}
+
+    @overload
+    async def begin_create_or_update(
+        self,
+        resource_group_name: str,
+        aml_filesystem_name: str,
+        import_job_name: str,
+        import_job: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.ImportJob]:
+        """Create or update an import job. Import jobs are automatically deleted 72 hours after
+        completion.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
+         and hyphens. Start and end with alphanumeric. Required.
+        :type aml_filesystem_name: str
+        :param import_job_name: Name for the import job. Allows alphanumerics, underscores, and
+         hyphens. Start and end with alphanumeric. Required.
+        :type import_job_name: str
+        :param import_job: Object containing the user-selectable properties of the import job. If
+         read-only properties are included, they must match the existing values of those properties.
+         Required.
+        :type import_job: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: An instance of AsyncLROPoller that returns either ImportJob or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.ImportJob]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def begin_create_or_update(
+        self,
+        resource_group_name: str,
+        aml_filesystem_name: str,
+        import_job_name: str,
+        import_job: Union[_models.ImportJob, IO[bytes]],
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.ImportJob]:
+        """Create or update an import job. Import jobs are automatically deleted 72 hours after
+        completion.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
+         and hyphens. Start and end with alphanumeric. Required.
+        :type aml_filesystem_name: str
+        :param import_job_name: Name for the import job. Allows alphanumerics, underscores, and
+         hyphens. Start and end with alphanumeric. Required.
+        :type import_job_name: str
+        :param import_job: Object containing the user-selectable properties of the import job. If
+         read-only properties are included, they must match the existing values of those properties. Is
+         either a ImportJob type or a IO[bytes] type. Required.
+        :type import_job: ~azure.mgmt.storagecache.models.ImportJob or IO[bytes]
+        :return: An instance of AsyncLROPoller that returns either ImportJob or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.ImportJob]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[None] = kwargs.pop("cls", None)
-        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ImportJob] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = self._resume_initial(  # type: ignore
+            raw_result = await self._create_or_update_initial(
                 resource_group_name=resource_group_name,
-                cache_name=cache_name,
-                storage_target_name=storage_target_name,
+                aml_filesystem_name=aml_filesystem_name,
+                import_job_name=import_job_name,
+                import_job=import_job,
                 api_version=api_version,
+                content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
-        def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("ImportJob", pipeline_response)
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
+            return deserialized
 
         if polling is True:
-            polling_method: PollingMethod = cast(
-                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod,
+                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
             )
         elif polling is False:
-            polling_method = cast(PollingMethod, NoPolling())
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.ImportJob].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_resume.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/resume"
-    }
+        return AsyncLROPoller[_models.ImportJob](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
-    def _invalidate_initial(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
-    ) -> None:
+    async def _update_initial(
+        self,
+        resource_group_name: str,
+        aml_filesystem_name: str,
+        import_job_name: str,
+        import_job: Union[_models.ImportJobUpdate, IO[bytes]],
+        **kwargs: Any
+    ) -> Optional[_models.ImportJob]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        _headers = kwargs.pop("headers", {}) or {}
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[None] = kwargs.pop("cls", None)
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.ImportJob]] = kwargs.pop("cls", None)
 
-        request = build_invalidate_request(
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(import_job, (IOBase, bytes)):
+            _content = import_job
+        else:
+            _json = self._serialize.body(import_job, "ImportJobUpdate")
+
+        _request = build_update_request(
             resource_group_name=resource_group_name,
-            cache_name=cache_name,
-            storage_target_name=storage_target_name,
+            aml_filesystem_name=aml_filesystem_name,
+            import_job_name=import_job_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._invalidate_initial.metadata["url"],
+            content_type=content_type,
+            json=_json,
+            content=_content,
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 202, 204]:
+        if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
+        deserialized = None
         response_headers = {}
+        if response.status_code == 200:
+            deserialized = self._deserialize("ImportJob", pipeline_response)
+
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
-            response_headers["Azure-AsyncOperation"] = self._deserialize(
-                "str", response.headers.get("Azure-AsyncOperation")
+            response_headers["azure-async-operation"] = self._deserialize(
+                "str", response.headers.get("azure-async-operation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
-    _invalidate_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/invalidate"
-    }
+        return deserialized  # type: ignore
 
-    @distributed_trace
-    def begin_invalidate(
-        self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
-    ) -> LROPoller[None]:
-        """Invalidate all cached data for a storage target. Cached files are discarded and fetched from
-        the back end on the next request.
+    @overload
+    async def begin_update(
+        self,
+        resource_group_name: str,
+        aml_filesystem_name: str,
+        import_job_name: str,
+        import_job: _models.ImportJobUpdate,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.ImportJob]:
+        """Update an import job instance.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
-         from the [-0-9a-zA-Z_] char class. Required.
-        :type cache_name: str
-        :param storage_target_name: Name of Storage Target. Required.
-        :type storage_target_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either None or the result of cls(response)
-        :rtype: ~azure.core.polling.LROPoller[None]
+        :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
+         and hyphens. Start and end with alphanumeric. Required.
+        :type aml_filesystem_name: str
+        :param import_job_name: Name for the import job. Allows alphanumerics, underscores, and
+         hyphens. Start and end with alphanumeric. Required.
+        :type import_job_name: str
+        :param import_job: Object containing the user-selectable properties of the import job. If
+         read-only properties are included, they must match the existing values of those properties.
+         Required.
+        :type import_job: ~azure.mgmt.storagecache.models.ImportJobUpdate
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: An instance of AsyncLROPoller that returns either ImportJob or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.ImportJob]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        _headers = kwargs.pop("headers", {}) or {}
+
+    @overload
+    async def begin_update(
+        self,
+        resource_group_name: str,
+        aml_filesystem_name: str,
+        import_job_name: str,
+        import_job: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.ImportJob]:
+        """Update an import job instance.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
+         and hyphens. Start and end with alphanumeric. Required.
+        :type aml_filesystem_name: str
+        :param import_job_name: Name for the import job. Allows alphanumerics, underscores, and
+         hyphens. Start and end with alphanumeric. Required.
+        :type import_job_name: str
+        :param import_job: Object containing the user-selectable properties of the import job. If
+         read-only properties are included, they must match the existing values of those properties.
+         Required.
+        :type import_job: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: An instance of AsyncLROPoller that returns either ImportJob or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.ImportJob]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def begin_update(
+        self,
+        resource_group_name: str,
+        aml_filesystem_name: str,
+        import_job_name: str,
+        import_job: Union[_models.ImportJobUpdate, IO[bytes]],
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.ImportJob]:
+        """Update an import job instance.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
+         and hyphens. Start and end with alphanumeric. Required.
+        :type aml_filesystem_name: str
+        :param import_job_name: Name for the import job. Allows alphanumerics, underscores, and
+         hyphens. Start and end with alphanumeric. Required.
+        :type import_job_name: str
+        :param import_job: Object containing the user-selectable properties of the import job. If
+         read-only properties are included, they must match the existing values of those properties. Is
+         either a ImportJobUpdate type or a IO[bytes] type. Required.
+        :type import_job: ~azure.mgmt.storagecache.models.ImportJobUpdate or IO[bytes]
+        :return: An instance of AsyncLROPoller that returns either ImportJob or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.ImportJob]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[None] = kwargs.pop("cls", None)
-        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ImportJob] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = self._invalidate_initial(  # type: ignore
+            raw_result = await self._update_initial(
                 resource_group_name=resource_group_name,
-                cache_name=cache_name,
-                storage_target_name=storage_target_name,
+                aml_filesystem_name=aml_filesystem_name,
+                import_job_name=import_job_name,
+                import_job=import_job,
                 api_version=api_version,
+                content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
-        def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("ImportJob", pipeline_response)
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
+            return deserialized
 
         if polling is True:
-            polling_method: PollingMethod = cast(
-                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod,
+                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
             )
         elif polling is False:
-            polling_method = cast(PollingMethod, NoPolling())
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.ImportJob].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+        return AsyncLROPoller[_models.ImportJob](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
+
+    @distributed_trace
+    def list_by_aml_filesystem(
+        self, resource_group_name: str, aml_filesystem_name: str, **kwargs: Any
+    ) -> AsyncIterable["_models.ImportJob"]:
+        """Returns all import jobs the user has access to under an AML File System.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param aml_filesystem_name: Name for the AML file system. Allows alphanumerics, underscores,
+         and hyphens. Start and end with alphanumeric. Required.
+        :type aml_filesystem_name: str
+        :return: An iterator like instance of either ImportJob or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.storagecache.models.ImportJob]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.ImportJobsListResult] = kwargs.pop("cls", None)
+
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        def prepare_request(next_link=None):
+            if not next_link:
+
+                _request = build_list_by_aml_filesystem_request(
+                    resource_group_name=resource_group_name,
+                    aml_filesystem_name=aml_filesystem_name,
+                    subscription_id=self._config.subscription_id,
+                    api_version=api_version,
+                    headers=_headers,
+                    params=_params,
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+
+            else:
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                _request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
+
+        async def extract_data(pipeline_response):
+            deserialized = self._deserialize("ImportJobsListResult", pipeline_response)
+            list_of_elem = deserialized.value
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return deserialized.next_link or None, AsyncList(list_of_elem)
+
+        async def get_next(next_link=None):
+            _request = prepare_request(next_link)
+
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+            response = pipeline_response.http_response
+
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+
+            return pipeline_response
 
-    begin_invalidate.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/invalidate"
-    }
+        return AsyncItemPaged(get_next, extract_data)
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure/mgmt/storagecache/operations/_usage_models_operations.py` & `azure-mgmt-storagecache-2.0.0/azure/mgmt/storagecache/operations/_skus_operations.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -36,19 +36,19 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
-    _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/usageModels")
+    _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/skus")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -56,105 +56,101 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class UsageModelsOperations:
+class SkusOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.storagecache.StorageCacheManagementClient`'s
-        :attr:`usage_models` attribute.
+        :attr:`skus` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, **kwargs: Any) -> Iterable["_models.UsageModel"]:
-        """Get the list of cache usage models available to this subscription.
+    def list(self, **kwargs: Any) -> Iterable["_models.ResourceSku"]:
+        """Get the list of StorageCache.Cache SKUs available to this subscription.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either UsageModel or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.storagecache.models.UsageModel]
+        :return: An iterator like instance of either ResourceSku or the result of cls(response)
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.storagecache.models.ResourceSku]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.UsageModelsResult] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ResourceSkusResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
-            deserialized = self._deserialize("UsageModelsResult", pipeline_response)
+            deserialized = self._deserialize("ResourceSkusResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
-
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/usageModels"}
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure_mgmt_storagecache.egg-info/PKG-INFO` & `azure-mgmt-storagecache-2.0.0/azure_mgmt_storagecache.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-storagecache
-Version: 1.6.0b1
+Version: 2.0.0
 Summary: Microsoft Azure Storage Cache Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: isodate<1.0.0,>=0.6.1
-Requires-Dist: azure-common~=1.1
-Requires-Dist: azure-mgmt-core<2.0.0,>=1.3.2
 
 # Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Storage Cache Management Client Library.
 This package has been tested with Python 3.8+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
@@ -85,14 +82,30 @@
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 # Release History
 
+## 2.0.0 (2024-05-20)
+
+### Features Added
+
+  - Added operation group ImportJobsOperations
+  - Model AmlFilesystem has a new parameter root_squash_settings
+  - Model AmlFilesystemHsmSettings has a new parameter import_prefixes_initial
+  - Model AmlFilesystemUpdate has a new parameter root_squash_settings
+  - Model ErrorResponse has a new parameter error
+  - Model AscOperation.error changes type from ErrorResponse to AscOperationErrorResponse
+
+### Breaking Changes
+
+  - Model ErrorResponse no longer has parameter code
+  - Model ErrorResponse no longer has parameter message
+
 ## 1.6.0b1 (2024-02-22)
 
 ### Features Added
 
   - Model AmlFilesystem has a new parameter root_squash_settings
   - Model AmlFilesystemUpdate has a new parameter root_squash_settings
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/azure_mgmt_storagecache.egg-info/SOURCES.txt` & `azure-mgmt-storagecache-2.0.0/azure_mgmt_storagecache.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 azure/mgmt/storagecache/aio/_storage_cache_management_client.py
 azure/mgmt/storagecache/aio/_vendor.py
 azure/mgmt/storagecache/aio/operations/__init__.py
 azure/mgmt/storagecache/aio/operations/_aml_filesystems_operations.py
 azure/mgmt/storagecache/aio/operations/_asc_operations_operations.py
 azure/mgmt/storagecache/aio/operations/_asc_usages_operations.py
 azure/mgmt/storagecache/aio/operations/_caches_operations.py
+azure/mgmt/storagecache/aio/operations/_import_jobs_operations.py
 azure/mgmt/storagecache/aio/operations/_operations.py
 azure/mgmt/storagecache/aio/operations/_patch.py
 azure/mgmt/storagecache/aio/operations/_skus_operations.py
 azure/mgmt/storagecache/aio/operations/_storage_cache_management_client_operations.py
 azure/mgmt/storagecache/aio/operations/_storage_target_operations.py
 azure/mgmt/storagecache/aio/operations/_storage_targets_operations.py
 azure/mgmt/storagecache/aio/operations/_usage_models_operations.py
@@ -36,14 +37,15 @@
 azure/mgmt/storagecache/models/_patch.py
 azure/mgmt/storagecache/models/_storage_cache_management_client_enums.py
 azure/mgmt/storagecache/operations/__init__.py
 azure/mgmt/storagecache/operations/_aml_filesystems_operations.py
 azure/mgmt/storagecache/operations/_asc_operations_operations.py
 azure/mgmt/storagecache/operations/_asc_usages_operations.py
 azure/mgmt/storagecache/operations/_caches_operations.py
+azure/mgmt/storagecache/operations/_import_jobs_operations.py
 azure/mgmt/storagecache/operations/_operations.py
 azure/mgmt/storagecache/operations/_patch.py
 azure/mgmt/storagecache/operations/_skus_operations.py
 azure/mgmt/storagecache/operations/_storage_cache_management_client_operations.py
 azure/mgmt/storagecache/operations/_storage_target_operations.py
 azure/mgmt/storagecache/operations/_storage_targets_operations.py
 azure/mgmt/storagecache/operations/_usage_models_operations.py
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/setup.py` & `azure-mgmt-storagecache-2.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     long_description_content_type="text/markdown",
     license="MIT License",
     author="Microsoft Corporation",
     author_email="azpysdkhelp@microsoft.com",
     url="https://github.com/Azure/azure-sdk-for-python",
     keywords="azure, azure sdk",  # update with search keywords relevant to the azure service / product
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
@@ -70,13 +70,13 @@
         ]
     ),
     include_package_data=True,
     package_data={
         "pytyped": ["py.typed"],
     },
     install_requires=[
-        "isodate<1.0.0,>=0.6.1",
-        "azure-common~=1.1",
-        "azure-mgmt-core>=1.3.2,<2.0.0",
+        "isodate>=0.6.1",
+        "azure-common>=1.1",
+        "azure-mgmt-core>=1.3.2",
     ],
     python_requires=">=3.8",
 )
```

### Comparing `azure-mgmt-storagecache-1.6.0b1/tests/conftest.py` & `azure-mgmt-storagecache-2.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-storagecache-1.6.0b1/tests/test_cli_mgmt_storagecache.py` & `azure-mgmt-storagecache-2.0.0/tests/test_cli_mgmt_storagecache.py`

 * *Files identical despite different names*

