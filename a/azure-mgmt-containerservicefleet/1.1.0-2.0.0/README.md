# Comparing `tmp/azure-mgmt-containerservicefleet-1.1.0.tar.gz` & `tmp/azure-mgmt-containerservicefleet-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-mgmt-containerservicefleet-1.1.0.tar", last modified: Wed Apr  3 06:49:50 2024, max compression
+gzip compressed data, was "azure-mgmt-containerservicefleet-2.0.0.tar", last modified: Thu May 23 04:17:05 2024, max compression
```

## Comparing `azure-mgmt-containerservicefleet-1.1.0.tar` & `azure-mgmt-containerservicefleet-2.0.0.tar`

### file list

```diff
@@ -1,284 +1,309 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.573011 azure-mgmt-containerservicefleet-1.1.0/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1238 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      227 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/MANIFEST.in
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     4347 2024-04-03 06:49:50.573011 azure-mgmt-containerservicefleet-1.1.0/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2079 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/README.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1795 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/_meta.json
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.525011 azure-mgmt-containerservicefleet-1.1.0/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.525011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.529011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      751 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3129 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18103 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/_container_service_fleet_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78953 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/_serialization.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      345 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.529011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      596 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3193 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18481 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/aio/_container_service_fleet_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      360 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/models.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.529011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      935 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3473 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5886 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/_container_service_fleet_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/_vendor.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.529011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      882 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3521 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6059 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/_container_service_fleet_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.529011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      926 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25384 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/_fleet_members_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    36135 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/_fleets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5767 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.533011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2308 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2447 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/models/_container_service_fleet_mgmt_client_enums.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    29307 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/models/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.533011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      926 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    32443 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/_fleet_members_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    46254 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/_fleets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6484 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.533011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      935 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3473 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5572 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/_container_service_fleet_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/_vendor.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.533011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      882 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3521 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5736 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/_container_service_fleet_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.537011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      872 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    26339 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/operations/_fleet_members_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    37155 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/operations/_fleets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/operations/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.537011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1970 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1370 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/models/_container_service_fleet_mgmt_client_enums.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    23900 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/models/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.537011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      872 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33415 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/operations/_fleet_members_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    47291 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/operations/_fleets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.537011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      935 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3473 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5572 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/_container_service_fleet_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/_vendor.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.541011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      882 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3521 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5736 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/_container_service_fleet_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.541011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      872 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    26339 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/operations/_fleet_members_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    37155 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/operations/_fleets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/operations/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.541011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1970 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1370 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/models/_container_service_fleet_mgmt_client_enums.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    23900 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/models/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.541011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      872 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33415 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/operations/_fleet_members_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    47291 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/operations/_fleets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.545011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      935 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3473 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6235 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/_container_service_fleet_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/_vendor.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.545011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      882 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3521 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6412 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/_container_service_fleet_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.545011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1012 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    32035 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/_fleet_members_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    36135 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/_fleets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5767 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    36913 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/_update_runs_operations.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.545011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3539 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4200 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/models/_container_service_fleet_mgmt_client_enums.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    50427 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/models/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.549011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1012 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    41205 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/_fleet_members_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    46254 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/_fleets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6484 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    47548 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/_update_runs_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.549011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      935 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3473 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6235 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/_container_service_fleet_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/_vendor.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.549011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      882 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3521 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6412 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/_container_service_fleet_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.553011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1012 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    35499 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/_fleet_members_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    39450 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/_fleets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5767 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    36913 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/_update_runs_operations.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.553011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4271 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5924 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/models/_container_service_fleet_mgmt_client_enums.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    63450 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/models/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.553011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1012 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    44555 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/_fleet_members_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    49455 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/_fleets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6484 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    47548 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/_update_runs_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.553011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      935 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3473 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6689 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/_container_service_fleet_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/_vendor.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.557011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      882 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3521 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6870 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/_container_service_fleet_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.557011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1132 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    35499 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_fleet_members_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25933 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_fleet_update_strategies_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    39450 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_fleets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5767 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    36913 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_update_runs_operations.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.557011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4572 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6273 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/models/_container_service_fleet_mgmt_client_enums.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    70347 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/models/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.561011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1132 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    44555 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_fleet_members_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33046 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_fleet_update_strategies_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    49455 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_fleets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6484 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    47548 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_update_runs_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.561011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      935 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3457 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6552 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/_container_service_fleet_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/_vendor.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.561011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      882 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3505 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6728 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/_container_service_fleet_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.565011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1132 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    35137 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_fleet_members_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25680 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_fleet_update_strategies_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    39021 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_fleets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5721 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    36524 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_update_runs_operations.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.565011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4372 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6273 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/models/_container_service_fleet_mgmt_client_enums.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    63371 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/models/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.565011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1132 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    44153 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_fleet_members_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    32761 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_fleet_update_strategies_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    48970 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_fleets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6430 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    47111 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_update_runs_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.569011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      935 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3473 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6689 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/_container_service_fleet_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/_vendor.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.569011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      882 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3521 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6870 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/_container_service_fleet_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.569011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1132 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    35499 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_fleet_members_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25933 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_fleet_update_strategies_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    39450 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_fleets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5767 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    46981 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_update_runs_operations.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.569011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4773 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6976 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/models/_container_service_fleet_mgmt_client_enums.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    72753 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/models/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.573011 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1132 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    44555 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_fleet_members_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33046 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_fleet_update_strategies_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    49455 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_fleets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6484 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    59600 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_update_runs_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-03 06:49:50.573011 azure-mgmt-containerservicefleet-1.1.0/azure_mgmt_containerservicefleet.egg-info/
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     4347 2024-04-03 06:49:50.000000 azure-mgmt-containerservicefleet-1.1.0/azure_mgmt_containerservicefleet.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    17572 2024-04-03 06:49:50.000000 azure-mgmt-containerservicefleet-1.1.0/azure_mgmt_containerservicefleet.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-03 06:49:50.000000 azure-mgmt-containerservicefleet-1.1.0/azure_mgmt_containerservicefleet.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-03 06:49:50.000000 azure-mgmt-containerservicefleet-1.1.0/azure_mgmt_containerservicefleet.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       56 2024-04-03 06:49:50.000000 azure-mgmt-containerservicefleet-1.1.0/azure_mgmt_containerservicefleet.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-04-03 06:49:50.000000 azure-mgmt-containerservicefleet-1.1.0/azure_mgmt_containerservicefleet.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-04-03 06:49:50.573011 azure-mgmt-containerservicefleet-1.1.0/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2808 2024-04-03 06:48:16.000000 azure-mgmt-containerservicefleet-1.1.0/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.957346 azure-mgmt-containerservicefleet-2.0.0/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1432 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      227 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/MANIFEST.in
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4440 2024-05-23 04:17:05.957346 azure-mgmt-containerservicefleet-2.0.0/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2079 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/README.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1916 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/_meta.json
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.905339 azure-mgmt-containerservicefleet-2.0.0/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.905339 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.909339 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      751 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3129 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19626 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/_container_service_fleet_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78953 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/_serialization.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      345 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.909339 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      596 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3193 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    20050 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/aio/_container_service_fleet_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      360 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/models.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.909339 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      935 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3473 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5886 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/_container_service_fleet_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/_vendor.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.909339 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      882 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3521 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6059 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/_container_service_fleet_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.909339 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      926 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25384 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/_fleet_members_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    36135 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/_fleets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5767 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.913340 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2308 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2447 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/models/_container_service_fleet_mgmt_client_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    29311 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/models/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.913340 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      926 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    32443 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/_fleet_members_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    46254 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/_fleets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6484 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.913340 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      935 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3473 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5572 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/_container_service_fleet_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/_vendor.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.913340 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      882 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3521 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5736 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/_container_service_fleet_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.917340 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      872 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    26339 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/operations/_fleet_members_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    37155 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/operations/_fleets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/operations/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.917340 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1970 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1370 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/models/_container_service_fleet_mgmt_client_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    23900 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/models/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.917340 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      872 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33415 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/operations/_fleet_members_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    47291 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/operations/_fleets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/operations/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.917340 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      935 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3473 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5572 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/_container_service_fleet_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/_vendor.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.917340 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      882 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3521 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5736 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/_container_service_fleet_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.921341 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      872 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    26339 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/operations/_fleet_members_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    37155 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/operations/_fleets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/operations/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.921341 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1970 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1370 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/models/_container_service_fleet_mgmt_client_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    23900 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/models/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.921341 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      872 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33415 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/operations/_fleet_members_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    47291 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/operations/_fleets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/operations/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.921341 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      935 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3473 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6235 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/_container_service_fleet_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/_vendor.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.925341 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      882 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3521 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6412 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/_container_service_fleet_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.925341 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1012 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    32035 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/_fleet_members_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    36135 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/_fleets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5767 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    36913 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/_update_runs_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.925341 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3539 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4200 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/models/_container_service_fleet_mgmt_client_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    50433 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/models/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.925341 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1012 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    41205 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/_fleet_members_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    46254 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/_fleets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6484 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    47548 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/_update_runs_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.929342 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      935 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3473 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6235 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/_container_service_fleet_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/_vendor.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.929342 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      882 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3521 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6412 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/_container_service_fleet_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.929342 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1012 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    35499 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/_fleet_members_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    39450 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/_fleets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5767 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    36913 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/_update_runs_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.929342 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4271 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5924 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/models/_container_service_fleet_mgmt_client_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    63456 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/models/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.933342 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1012 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    44555 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/_fleet_members_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    49455 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/_fleets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6484 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    47548 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/_update_runs_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.933342 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      935 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3473 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6689 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/_container_service_fleet_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/_vendor.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.933342 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      882 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3521 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6870 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/_container_service_fleet_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.937343 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1132 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    35499 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_fleet_members_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25933 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_fleet_update_strategies_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    39450 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_fleets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5767 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    36913 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_update_runs_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.937343 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4572 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6273 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/models/_container_service_fleet_mgmt_client_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    70369 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/models/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.937343 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1132 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    44555 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_fleet_members_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33046 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_fleet_update_strategies_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    49455 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_fleets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6484 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    47548 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_update_runs_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.937343 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      935 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3457 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6552 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/_container_service_fleet_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/_vendor.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.941343 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      882 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3505 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6728 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/_container_service_fleet_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.941343 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1132 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    35137 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_fleet_members_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25680 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_fleet_update_strategies_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    39021 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_fleets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5721 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    36524 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_update_runs_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.941343 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4372 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6273 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/models/_container_service_fleet_mgmt_client_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    63393 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/models/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.941343 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1132 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    44153 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_fleet_members_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    32761 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_fleet_update_strategies_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    48970 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_fleets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6430 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    47111 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_update_runs_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.945344 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      935 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3473 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6689 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/_container_service_fleet_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/_vendor.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.945344 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      882 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3521 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6870 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/_container_service_fleet_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.949344 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1132 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    35499 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_fleet_members_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25933 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_fleet_update_strategies_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    39450 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_fleets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5767 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    46981 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_update_runs_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.949344 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4773 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6976 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/models/_container_service_fleet_mgmt_client_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    72775 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/models/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.949344 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1132 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    44555 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_fleet_members_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33046 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_fleet_update_strategies_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    49455 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_fleets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6484 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    59600 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_update_runs_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.949344 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      935 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3457 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6552 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/_container_service_fleet_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/_vendor.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.953345 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      882 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3505 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6728 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/aio/_container_service_fleet_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/aio/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.953345 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1132 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    35137 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/aio/operations/_fleet_members_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25680 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/aio/operations/_fleet_update_strategies_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    39021 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/aio/operations/_fleets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5721 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/aio/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/aio/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    46483 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/aio/operations/_update_runs_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.953345 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4773 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6976 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/models/_container_service_fleet_mgmt_client_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    70901 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/models/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.957346 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1132 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    44153 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/operations/_fleet_members_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    32761 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/operations/_fleet_update_strategies_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    48970 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/operations/_fleets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6430 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    59046 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_04_01/operations/_update_runs_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-23 04:17:05.957346 azure-mgmt-containerservicefleet-2.0.0/azure_mgmt_containerservicefleet.egg-info/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4440 2024-05-23 04:17:05.000000 azure-mgmt-containerservicefleet-2.0.0/azure_mgmt_containerservicefleet.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19144 2024-05-23 04:17:05.000000 azure-mgmt-containerservicefleet-2.0.0/azure_mgmt_containerservicefleet.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-23 04:17:05.000000 azure-mgmt-containerservicefleet-2.0.0/azure_mgmt_containerservicefleet.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-23 04:17:05.000000 azure-mgmt-containerservicefleet-2.0.0/azure_mgmt_containerservicefleet.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       56 2024-05-23 04:17:05.000000 azure-mgmt-containerservicefleet-2.0.0/azure_mgmt_containerservicefleet.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-05-23 04:17:05.000000 azure-mgmt-containerservicefleet-2.0.0/azure_mgmt_containerservicefleet.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-05-23 04:17:05.957346 azure-mgmt-containerservicefleet-2.0.0/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2808 2024-05-23 04:15:45.000000 azure-mgmt-containerservicefleet-2.0.0/setup.py
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/CHANGELOG.md` & `azure-mgmt-containerservicefleet-2.0.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Release History
 
+## 2.0.0 (2024-05-20)
+
+### Breaking Changes
+
+  - Model APIServerAccessProfile no longer has parameter enable_vnet_integration
+  - Model APIServerAccessProfile no longer has parameter subnet_id
+
 ## 1.1.0 (2024-04-03)
 
 ### Features Added
 
   - Added operation UpdateRunsOperations.begin_skip
   - Model Fleet has a new parameter hub_profile
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/LICENSE` & `azure-mgmt-containerservicefleet-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/PKG-INFO` & `azure-mgmt-containerservicefleet-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-containerservicefleet
-Version: 1.1.0
+Version: 2.0.0
 Summary: Microsoft Azure Containerservicefleet Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,17 +16,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: isodate>=0.6.1
-Requires-Dist: azure-common>=1.1
-Requires-Dist: azure-mgmt-core>=1.3.2
 
 # Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Containerservicefleet Management Client Library.
 This package has been tested with Python 3.8+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
@@ -85,14 +82,21 @@
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 # Release History
 
+## 2.0.0 (2024-05-20)
+
+### Breaking Changes
+
+  - Model APIServerAccessProfile no longer has parameter enable_vnet_integration
+  - Model APIServerAccessProfile no longer has parameter subnet_id
+
 ## 1.1.0 (2024-04-03)
 
 ### Features Added
 
   - Added operation UpdateRunsOperations.begin_skip
   - Model Fleet has a new parameter hub_profile
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/README.md` & `azure-mgmt-containerservicefleet-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/_configuration.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/_container_service_fleet_mgmt_client.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/_container_service_fleet_mgmt_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     :param base_url: Service URL
     :type base_url: str
     :param profile: A profile definition, from KnownProfiles to dict.
     :type profile: azure.profiles.KnownProfiles
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
     """
 
-    DEFAULT_API_VERSION = '2023-10-15'
+    DEFAULT_API_VERSION = '2024-04-01'
     _PROFILE_TAG = "azure.mgmt.containerservicefleet.ContainerServiceFleetMgmtClient"
     LATEST_PROFILE = ProfileDefinition({
         _PROFILE_TAG: {
             None: DEFAULT_API_VERSION,
         }},
         _PROFILE_TAG + " latest"
     )
@@ -112,14 +112,15 @@
            * 2022-07-02-preview: :mod:`v2022_07_02_preview.models<azure.mgmt.containerservicefleet.v2022_07_02_preview.models>`
            * 2022-06-02-preview: :mod:`v2022_09_02_preview.models<azure.mgmt.containerservicefleet.v2022_09_02_preview.models>`
            * 2023-03-15-preview: :mod:`v2023_03_15_preview.models<azure.mgmt.containerservicefleet.v2023_03_15_preview.models>`
            * 2023-06-15-preview: :mod:`v2023_06_15_preview.models<azure.mgmt.containerservicefleet.v2023_06_15_preview.models>`
            * 2023-08-15-preview: :mod:`v2023_08_15_preview.models<azure.mgmt.containerservicefleet.v2023_08_15_preview.models>`
            * 2023-10-15: :mod:`v2023_10_15.models<azure.mgmt.containerservicefleet.v2023_10_15.models>`
            * 2024-02-02-preview: :mod:`v2024_02_02_preview.models<azure.mgmt.containerservicefleet.v2024_02_02_preview.models>`
+           * 2024-04-01: :mod:`v2024_04_01.models<azure.mgmt.containerservicefleet.v2024_04_01.models>`
         """
         if api_version == '2022-09-02-preview':
             from .v2022_06_02_preview import models
             return models
         elif api_version == '2022-07-02-preview':
             from .v2022_07_02_preview import models
             return models
@@ -137,28 +138,32 @@
             return models
         elif api_version == '2023-10-15':
             from .v2023_10_15 import models
             return models
         elif api_version == '2024-02-02-preview':
             from .v2024_02_02_preview import models
             return models
+        elif api_version == '2024-04-01':
+            from .v2024_04_01 import models
+            return models
         raise ValueError("API version {} is not available".format(api_version))
 
     @property
     def fleet_members(self):
         """Instance depends on the API version:
 
            * 2022-09-02-preview: :class:`FleetMembersOperations<azure.mgmt.containerservicefleet.v2022_06_02_preview.operations.FleetMembersOperations>`
            * 2022-07-02-preview: :class:`FleetMembersOperations<azure.mgmt.containerservicefleet.v2022_07_02_preview.operations.FleetMembersOperations>`
            * 2022-06-02-preview: :class:`FleetMembersOperations<azure.mgmt.containerservicefleet.v2022_09_02_preview.operations.FleetMembersOperations>`
            * 2023-03-15-preview: :class:`FleetMembersOperations<azure.mgmt.containerservicefleet.v2023_03_15_preview.operations.FleetMembersOperations>`
            * 2023-06-15-preview: :class:`FleetMembersOperations<azure.mgmt.containerservicefleet.v2023_06_15_preview.operations.FleetMembersOperations>`
            * 2023-08-15-preview: :class:`FleetMembersOperations<azure.mgmt.containerservicefleet.v2023_08_15_preview.operations.FleetMembersOperations>`
            * 2023-10-15: :class:`FleetMembersOperations<azure.mgmt.containerservicefleet.v2023_10_15.operations.FleetMembersOperations>`
            * 2024-02-02-preview: :class:`FleetMembersOperations<azure.mgmt.containerservicefleet.v2024_02_02_preview.operations.FleetMembersOperations>`
+           * 2024-04-01: :class:`FleetMembersOperations<azure.mgmt.containerservicefleet.v2024_04_01.operations.FleetMembersOperations>`
         """
         api_version = self._get_api_version('fleet_members')
         if api_version == '2022-09-02-preview':
             from .v2022_06_02_preview.operations import FleetMembersOperations as OperationClass
         elif api_version == '2022-07-02-preview':
             from .v2022_07_02_preview.operations import FleetMembersOperations as OperationClass
         elif api_version == '2022-06-02-preview':
@@ -169,34 +174,39 @@
             from .v2023_06_15_preview.operations import FleetMembersOperations as OperationClass
         elif api_version == '2023-08-15-preview':
             from .v2023_08_15_preview.operations import FleetMembersOperations as OperationClass
         elif api_version == '2023-10-15':
             from .v2023_10_15.operations import FleetMembersOperations as OperationClass
         elif api_version == '2024-02-02-preview':
             from .v2024_02_02_preview.operations import FleetMembersOperations as OperationClass
+        elif api_version == '2024-04-01':
+            from .v2024_04_01.operations import FleetMembersOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'fleet_members'".format(api_version))
         self._config.api_version = api_version
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)), api_version)
 
     @property
     def fleet_update_strategies(self):
         """Instance depends on the API version:
 
            * 2023-08-15-preview: :class:`FleetUpdateStrategiesOperations<azure.mgmt.containerservicefleet.v2023_08_15_preview.operations.FleetUpdateStrategiesOperations>`
            * 2023-10-15: :class:`FleetUpdateStrategiesOperations<azure.mgmt.containerservicefleet.v2023_10_15.operations.FleetUpdateStrategiesOperations>`
            * 2024-02-02-preview: :class:`FleetUpdateStrategiesOperations<azure.mgmt.containerservicefleet.v2024_02_02_preview.operations.FleetUpdateStrategiesOperations>`
+           * 2024-04-01: :class:`FleetUpdateStrategiesOperations<azure.mgmt.containerservicefleet.v2024_04_01.operations.FleetUpdateStrategiesOperations>`
         """
         api_version = self._get_api_version('fleet_update_strategies')
         if api_version == '2023-08-15-preview':
             from .v2023_08_15_preview.operations import FleetUpdateStrategiesOperations as OperationClass
         elif api_version == '2023-10-15':
             from .v2023_10_15.operations import FleetUpdateStrategiesOperations as OperationClass
         elif api_version == '2024-02-02-preview':
             from .v2024_02_02_preview.operations import FleetUpdateStrategiesOperations as OperationClass
+        elif api_version == '2024-04-01':
+            from .v2024_04_01.operations import FleetUpdateStrategiesOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'fleet_update_strategies'".format(api_version))
         self._config.api_version = api_version
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)), api_version)
 
     @property
     def fleets(self):
@@ -206,14 +216,15 @@
            * 2022-07-02-preview: :class:`FleetsOperations<azure.mgmt.containerservicefleet.v2022_07_02_preview.operations.FleetsOperations>`
            * 2022-06-02-preview: :class:`FleetsOperations<azure.mgmt.containerservicefleet.v2022_09_02_preview.operations.FleetsOperations>`
            * 2023-03-15-preview: :class:`FleetsOperations<azure.mgmt.containerservicefleet.v2023_03_15_preview.operations.FleetsOperations>`
            * 2023-06-15-preview: :class:`FleetsOperations<azure.mgmt.containerservicefleet.v2023_06_15_preview.operations.FleetsOperations>`
            * 2023-08-15-preview: :class:`FleetsOperations<azure.mgmt.containerservicefleet.v2023_08_15_preview.operations.FleetsOperations>`
            * 2023-10-15: :class:`FleetsOperations<azure.mgmt.containerservicefleet.v2023_10_15.operations.FleetsOperations>`
            * 2024-02-02-preview: :class:`FleetsOperations<azure.mgmt.containerservicefleet.v2024_02_02_preview.operations.FleetsOperations>`
+           * 2024-04-01: :class:`FleetsOperations<azure.mgmt.containerservicefleet.v2024_04_01.operations.FleetsOperations>`
         """
         api_version = self._get_api_version('fleets')
         if api_version == '2022-09-02-preview':
             from .v2022_06_02_preview.operations import FleetsOperations as OperationClass
         elif api_version == '2022-07-02-preview':
             from .v2022_07_02_preview.operations import FleetsOperations as OperationClass
         elif api_version == '2022-06-02-preview':
@@ -224,14 +235,16 @@
             from .v2023_06_15_preview.operations import FleetsOperations as OperationClass
         elif api_version == '2023-08-15-preview':
             from .v2023_08_15_preview.operations import FleetsOperations as OperationClass
         elif api_version == '2023-10-15':
             from .v2023_10_15.operations import FleetsOperations as OperationClass
         elif api_version == '2024-02-02-preview':
             from .v2024_02_02_preview.operations import FleetsOperations as OperationClass
+        elif api_version == '2024-04-01':
+            from .v2024_04_01.operations import FleetsOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'fleets'".format(api_version))
         self._config.api_version = api_version
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)), api_version)
 
     @property
     def operations(self):
@@ -239,54 +252,60 @@
 
            * 2022-09-02-preview: :class:`Operations<azure.mgmt.containerservicefleet.v2022_06_02_preview.operations.Operations>`
            * 2023-03-15-preview: :class:`Operations<azure.mgmt.containerservicefleet.v2023_03_15_preview.operations.Operations>`
            * 2023-06-15-preview: :class:`Operations<azure.mgmt.containerservicefleet.v2023_06_15_preview.operations.Operations>`
            * 2023-08-15-preview: :class:`Operations<azure.mgmt.containerservicefleet.v2023_08_15_preview.operations.Operations>`
            * 2023-10-15: :class:`Operations<azure.mgmt.containerservicefleet.v2023_10_15.operations.Operations>`
            * 2024-02-02-preview: :class:`Operations<azure.mgmt.containerservicefleet.v2024_02_02_preview.operations.Operations>`
+           * 2024-04-01: :class:`Operations<azure.mgmt.containerservicefleet.v2024_04_01.operations.Operations>`
         """
         api_version = self._get_api_version('operations')
         if api_version == '2022-09-02-preview':
             from .v2022_06_02_preview.operations import Operations as OperationClass
         elif api_version == '2023-03-15-preview':
             from .v2023_03_15_preview.operations import Operations as OperationClass
         elif api_version == '2023-06-15-preview':
             from .v2023_06_15_preview.operations import Operations as OperationClass
         elif api_version == '2023-08-15-preview':
             from .v2023_08_15_preview.operations import Operations as OperationClass
         elif api_version == '2023-10-15':
             from .v2023_10_15.operations import Operations as OperationClass
         elif api_version == '2024-02-02-preview':
             from .v2024_02_02_preview.operations import Operations as OperationClass
+        elif api_version == '2024-04-01':
+            from .v2024_04_01.operations import Operations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'operations'".format(api_version))
         self._config.api_version = api_version
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)), api_version)
 
     @property
     def update_runs(self):
         """Instance depends on the API version:
 
            * 2023-03-15-preview: :class:`UpdateRunsOperations<azure.mgmt.containerservicefleet.v2023_03_15_preview.operations.UpdateRunsOperations>`
            * 2023-06-15-preview: :class:`UpdateRunsOperations<azure.mgmt.containerservicefleet.v2023_06_15_preview.operations.UpdateRunsOperations>`
            * 2023-08-15-preview: :class:`UpdateRunsOperations<azure.mgmt.containerservicefleet.v2023_08_15_preview.operations.UpdateRunsOperations>`
            * 2023-10-15: :class:`UpdateRunsOperations<azure.mgmt.containerservicefleet.v2023_10_15.operations.UpdateRunsOperations>`
            * 2024-02-02-preview: :class:`UpdateRunsOperations<azure.mgmt.containerservicefleet.v2024_02_02_preview.operations.UpdateRunsOperations>`
+           * 2024-04-01: :class:`UpdateRunsOperations<azure.mgmt.containerservicefleet.v2024_04_01.operations.UpdateRunsOperations>`
         """
         api_version = self._get_api_version('update_runs')
         if api_version == '2023-03-15-preview':
             from .v2023_03_15_preview.operations import UpdateRunsOperations as OperationClass
         elif api_version == '2023-06-15-preview':
             from .v2023_06_15_preview.operations import UpdateRunsOperations as OperationClass
         elif api_version == '2023-08-15-preview':
             from .v2023_08_15_preview.operations import UpdateRunsOperations as OperationClass
         elif api_version == '2023-10-15':
             from .v2023_10_15.operations import UpdateRunsOperations as OperationClass
         elif api_version == '2024-02-02-preview':
             from .v2024_02_02_preview.operations import UpdateRunsOperations as OperationClass
+        elif api_version == '2024-04-01':
+            from .v2024_04_01.operations import UpdateRunsOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'update_runs'".format(api_version))
         self._config.api_version = api_version
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)), api_version)
 
     def close(self):
         self._client.close()
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/_serialization.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/_serialization.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/aio/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/aio/_configuration.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/aio/_container_service_fleet_mgmt_client.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/aio/_container_service_fleet_mgmt_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     :param base_url: Service URL
     :type base_url: str
     :param profile: A profile definition, from KnownProfiles to dict.
     :type profile: azure.profiles.KnownProfiles
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
     """
 
-    DEFAULT_API_VERSION = '2023-10-15'
+    DEFAULT_API_VERSION = '2024-04-01'
     _PROFILE_TAG = "azure.mgmt.containerservicefleet.ContainerServiceFleetMgmtClient"
     LATEST_PROFILE = ProfileDefinition({
         _PROFILE_TAG: {
             None: DEFAULT_API_VERSION,
         }},
         _PROFILE_TAG + " latest"
     )
@@ -112,14 +112,15 @@
            * 2022-07-02-preview: :mod:`v2022_07_02_preview.models<azure.mgmt.containerservicefleet.v2022_07_02_preview.models>`
            * 2022-06-02-preview: :mod:`v2022_09_02_preview.models<azure.mgmt.containerservicefleet.v2022_09_02_preview.models>`
            * 2023-03-15-preview: :mod:`v2023_03_15_preview.models<azure.mgmt.containerservicefleet.v2023_03_15_preview.models>`
            * 2023-06-15-preview: :mod:`v2023_06_15_preview.models<azure.mgmt.containerservicefleet.v2023_06_15_preview.models>`
            * 2023-08-15-preview: :mod:`v2023_08_15_preview.models<azure.mgmt.containerservicefleet.v2023_08_15_preview.models>`
            * 2023-10-15: :mod:`v2023_10_15.models<azure.mgmt.containerservicefleet.v2023_10_15.models>`
            * 2024-02-02-preview: :mod:`v2024_02_02_preview.models<azure.mgmt.containerservicefleet.v2024_02_02_preview.models>`
+           * 2024-04-01: :mod:`v2024_04_01.models<azure.mgmt.containerservicefleet.v2024_04_01.models>`
         """
         if api_version == '2022-09-02-preview':
             from ..v2022_06_02_preview import models
             return models
         elif api_version == '2022-07-02-preview':
             from ..v2022_07_02_preview import models
             return models
@@ -137,28 +138,32 @@
             return models
         elif api_version == '2023-10-15':
             from ..v2023_10_15 import models
             return models
         elif api_version == '2024-02-02-preview':
             from ..v2024_02_02_preview import models
             return models
+        elif api_version == '2024-04-01':
+            from ..v2024_04_01 import models
+            return models
         raise ValueError("API version {} is not available".format(api_version))
 
     @property
     def fleet_members(self):
         """Instance depends on the API version:
 
            * 2022-09-02-preview: :class:`FleetMembersOperations<azure.mgmt.containerservicefleet.v2022_06_02_preview.aio.operations.FleetMembersOperations>`
            * 2022-07-02-preview: :class:`FleetMembersOperations<azure.mgmt.containerservicefleet.v2022_07_02_preview.aio.operations.FleetMembersOperations>`
            * 2022-06-02-preview: :class:`FleetMembersOperations<azure.mgmt.containerservicefleet.v2022_09_02_preview.aio.operations.FleetMembersOperations>`
            * 2023-03-15-preview: :class:`FleetMembersOperations<azure.mgmt.containerservicefleet.v2023_03_15_preview.aio.operations.FleetMembersOperations>`
            * 2023-06-15-preview: :class:`FleetMembersOperations<azure.mgmt.containerservicefleet.v2023_06_15_preview.aio.operations.FleetMembersOperations>`
            * 2023-08-15-preview: :class:`FleetMembersOperations<azure.mgmt.containerservicefleet.v2023_08_15_preview.aio.operations.FleetMembersOperations>`
            * 2023-10-15: :class:`FleetMembersOperations<azure.mgmt.containerservicefleet.v2023_10_15.aio.operations.FleetMembersOperations>`
            * 2024-02-02-preview: :class:`FleetMembersOperations<azure.mgmt.containerservicefleet.v2024_02_02_preview.aio.operations.FleetMembersOperations>`
+           * 2024-04-01: :class:`FleetMembersOperations<azure.mgmt.containerservicefleet.v2024_04_01.aio.operations.FleetMembersOperations>`
         """
         api_version = self._get_api_version('fleet_members')
         if api_version == '2022-09-02-preview':
             from ..v2022_06_02_preview.aio.operations import FleetMembersOperations as OperationClass
         elif api_version == '2022-07-02-preview':
             from ..v2022_07_02_preview.aio.operations import FleetMembersOperations as OperationClass
         elif api_version == '2022-06-02-preview':
@@ -169,34 +174,39 @@
             from ..v2023_06_15_preview.aio.operations import FleetMembersOperations as OperationClass
         elif api_version == '2023-08-15-preview':
             from ..v2023_08_15_preview.aio.operations import FleetMembersOperations as OperationClass
         elif api_version == '2023-10-15':
             from ..v2023_10_15.aio.operations import FleetMembersOperations as OperationClass
         elif api_version == '2024-02-02-preview':
             from ..v2024_02_02_preview.aio.operations import FleetMembersOperations as OperationClass
+        elif api_version == '2024-04-01':
+            from ..v2024_04_01.aio.operations import FleetMembersOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'fleet_members'".format(api_version))
         self._config.api_version = api_version
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)), api_version)
 
     @property
     def fleet_update_strategies(self):
         """Instance depends on the API version:
 
            * 2023-08-15-preview: :class:`FleetUpdateStrategiesOperations<azure.mgmt.containerservicefleet.v2023_08_15_preview.aio.operations.FleetUpdateStrategiesOperations>`
            * 2023-10-15: :class:`FleetUpdateStrategiesOperations<azure.mgmt.containerservicefleet.v2023_10_15.aio.operations.FleetUpdateStrategiesOperations>`
            * 2024-02-02-preview: :class:`FleetUpdateStrategiesOperations<azure.mgmt.containerservicefleet.v2024_02_02_preview.aio.operations.FleetUpdateStrategiesOperations>`
+           * 2024-04-01: :class:`FleetUpdateStrategiesOperations<azure.mgmt.containerservicefleet.v2024_04_01.aio.operations.FleetUpdateStrategiesOperations>`
         """
         api_version = self._get_api_version('fleet_update_strategies')
         if api_version == '2023-08-15-preview':
             from ..v2023_08_15_preview.aio.operations import FleetUpdateStrategiesOperations as OperationClass
         elif api_version == '2023-10-15':
             from ..v2023_10_15.aio.operations import FleetUpdateStrategiesOperations as OperationClass
         elif api_version == '2024-02-02-preview':
             from ..v2024_02_02_preview.aio.operations import FleetUpdateStrategiesOperations as OperationClass
+        elif api_version == '2024-04-01':
+            from ..v2024_04_01.aio.operations import FleetUpdateStrategiesOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'fleet_update_strategies'".format(api_version))
         self._config.api_version = api_version
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)), api_version)
 
     @property
     def fleets(self):
@@ -206,14 +216,15 @@
            * 2022-07-02-preview: :class:`FleetsOperations<azure.mgmt.containerservicefleet.v2022_07_02_preview.aio.operations.FleetsOperations>`
            * 2022-06-02-preview: :class:`FleetsOperations<azure.mgmt.containerservicefleet.v2022_09_02_preview.aio.operations.FleetsOperations>`
            * 2023-03-15-preview: :class:`FleetsOperations<azure.mgmt.containerservicefleet.v2023_03_15_preview.aio.operations.FleetsOperations>`
            * 2023-06-15-preview: :class:`FleetsOperations<azure.mgmt.containerservicefleet.v2023_06_15_preview.aio.operations.FleetsOperations>`
            * 2023-08-15-preview: :class:`FleetsOperations<azure.mgmt.containerservicefleet.v2023_08_15_preview.aio.operations.FleetsOperations>`
            * 2023-10-15: :class:`FleetsOperations<azure.mgmt.containerservicefleet.v2023_10_15.aio.operations.FleetsOperations>`
            * 2024-02-02-preview: :class:`FleetsOperations<azure.mgmt.containerservicefleet.v2024_02_02_preview.aio.operations.FleetsOperations>`
+           * 2024-04-01: :class:`FleetsOperations<azure.mgmt.containerservicefleet.v2024_04_01.aio.operations.FleetsOperations>`
         """
         api_version = self._get_api_version('fleets')
         if api_version == '2022-09-02-preview':
             from ..v2022_06_02_preview.aio.operations import FleetsOperations as OperationClass
         elif api_version == '2022-07-02-preview':
             from ..v2022_07_02_preview.aio.operations import FleetsOperations as OperationClass
         elif api_version == '2022-06-02-preview':
@@ -224,14 +235,16 @@
             from ..v2023_06_15_preview.aio.operations import FleetsOperations as OperationClass
         elif api_version == '2023-08-15-preview':
             from ..v2023_08_15_preview.aio.operations import FleetsOperations as OperationClass
         elif api_version == '2023-10-15':
             from ..v2023_10_15.aio.operations import FleetsOperations as OperationClass
         elif api_version == '2024-02-02-preview':
             from ..v2024_02_02_preview.aio.operations import FleetsOperations as OperationClass
+        elif api_version == '2024-04-01':
+            from ..v2024_04_01.aio.operations import FleetsOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'fleets'".format(api_version))
         self._config.api_version = api_version
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)), api_version)
 
     @property
     def operations(self):
@@ -239,54 +252,60 @@
 
            * 2022-09-02-preview: :class:`Operations<azure.mgmt.containerservicefleet.v2022_06_02_preview.aio.operations.Operations>`
            * 2023-03-15-preview: :class:`Operations<azure.mgmt.containerservicefleet.v2023_03_15_preview.aio.operations.Operations>`
            * 2023-06-15-preview: :class:`Operations<azure.mgmt.containerservicefleet.v2023_06_15_preview.aio.operations.Operations>`
            * 2023-08-15-preview: :class:`Operations<azure.mgmt.containerservicefleet.v2023_08_15_preview.aio.operations.Operations>`
            * 2023-10-15: :class:`Operations<azure.mgmt.containerservicefleet.v2023_10_15.aio.operations.Operations>`
            * 2024-02-02-preview: :class:`Operations<azure.mgmt.containerservicefleet.v2024_02_02_preview.aio.operations.Operations>`
+           * 2024-04-01: :class:`Operations<azure.mgmt.containerservicefleet.v2024_04_01.aio.operations.Operations>`
         """
         api_version = self._get_api_version('operations')
         if api_version == '2022-09-02-preview':
             from ..v2022_06_02_preview.aio.operations import Operations as OperationClass
         elif api_version == '2023-03-15-preview':
             from ..v2023_03_15_preview.aio.operations import Operations as OperationClass
         elif api_version == '2023-06-15-preview':
             from ..v2023_06_15_preview.aio.operations import Operations as OperationClass
         elif api_version == '2023-08-15-preview':
             from ..v2023_08_15_preview.aio.operations import Operations as OperationClass
         elif api_version == '2023-10-15':
             from ..v2023_10_15.aio.operations import Operations as OperationClass
         elif api_version == '2024-02-02-preview':
             from ..v2024_02_02_preview.aio.operations import Operations as OperationClass
+        elif api_version == '2024-04-01':
+            from ..v2024_04_01.aio.operations import Operations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'operations'".format(api_version))
         self._config.api_version = api_version
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)), api_version)
 
     @property
     def update_runs(self):
         """Instance depends on the API version:
 
            * 2023-03-15-preview: :class:`UpdateRunsOperations<azure.mgmt.containerservicefleet.v2023_03_15_preview.aio.operations.UpdateRunsOperations>`
            * 2023-06-15-preview: :class:`UpdateRunsOperations<azure.mgmt.containerservicefleet.v2023_06_15_preview.aio.operations.UpdateRunsOperations>`
            * 2023-08-15-preview: :class:`UpdateRunsOperations<azure.mgmt.containerservicefleet.v2023_08_15_preview.aio.operations.UpdateRunsOperations>`
            * 2023-10-15: :class:`UpdateRunsOperations<azure.mgmt.containerservicefleet.v2023_10_15.aio.operations.UpdateRunsOperations>`
            * 2024-02-02-preview: :class:`UpdateRunsOperations<azure.mgmt.containerservicefleet.v2024_02_02_preview.aio.operations.UpdateRunsOperations>`
+           * 2024-04-01: :class:`UpdateRunsOperations<azure.mgmt.containerservicefleet.v2024_04_01.aio.operations.UpdateRunsOperations>`
         """
         api_version = self._get_api_version('update_runs')
         if api_version == '2023-03-15-preview':
             from ..v2023_03_15_preview.aio.operations import UpdateRunsOperations as OperationClass
         elif api_version == '2023-06-15-preview':
             from ..v2023_06_15_preview.aio.operations import UpdateRunsOperations as OperationClass
         elif api_version == '2023-08-15-preview':
             from ..v2023_08_15_preview.aio.operations import UpdateRunsOperations as OperationClass
         elif api_version == '2023-10-15':
             from ..v2023_10_15.aio.operations import UpdateRunsOperations as OperationClass
         elif api_version == '2024-02-02-preview':
             from ..v2024_02_02_preview.aio.operations import UpdateRunsOperations as OperationClass
+        elif api_version == '2024-04-01':
+            from ..v2024_04_01.aio.operations import UpdateRunsOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'update_runs'".format(api_version))
         self._config.api_version = api_version
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)), api_version)
 
     async def close(self):
         await self._client.close()
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/_configuration.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/_container_service_fleet_mgmt_client.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/_container_service_fleet_mgmt_client.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/_vendor.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/_configuration.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/_container_service_fleet_mgmt_client.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/_container_service_fleet_mgmt_client.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/_fleet_members_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/_fleet_members_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -510,16 +510,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self,
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/_fleets_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/_fleets_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -709,16 +709,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self, resource_group_name: str, fleet_name: str, if_match: Optional[str] = None, **kwargs: Any
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/models/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/models/_container_service_fleet_mgmt_client_enums.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/models/_container_service_fleet_mgmt_client_enums.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/models/_models_py3.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/models/_models_py3.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,42 +378,41 @@
         self.fqdn = None
         self.kubernetes_version = None
 
 
 class FleetListResult(_serialization.Model):
     """The response of a Fleet list operation.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     All required parameters must be populated in order to send to server.
 
     :ivar value: The Fleet items on this page. Required.
     :vartype value: list[~azure.mgmt.containerservicefleet.v2022_06_02_preview.models.Fleet]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
-        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[Fleet]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.Fleet"], **kwargs: Any) -> None:
+    def __init__(self, *, value: List["_models.Fleet"], next_link: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword value: The Fleet items on this page. Required.
         :paramtype value: list[~azure.mgmt.containerservicefleet.v2022_06_02_preview.models.Fleet]
+        :keyword next_link: The link to the next page of items.
+        :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
-        self.next_link = None
+        self.next_link = next_link
 
 
 class ProxyResource(Resource):
     """The resource model definition for a Azure Resource Manager proxy resource. It will not have
     tags and a location.
 
     Variables are only populated by the server, and will be ignored when sending a request.
@@ -494,43 +493,42 @@
         self.cluster_resource_id = cluster_resource_id
         self.provisioning_state = None
 
 
 class FleetMemberListResult(_serialization.Model):
     """The response of a FleetMember list operation.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     All required parameters must be populated in order to send to server.
 
     :ivar value: The FleetMember items on this page. Required.
     :vartype value: list[~azure.mgmt.containerservicefleet.v2022_06_02_preview.models.FleetMember]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
-        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[FleetMember]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.FleetMember"], **kwargs: Any) -> None:
+    def __init__(self, *, value: List["_models.FleetMember"], next_link: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword value: The FleetMember items on this page. Required.
         :paramtype value:
          list[~azure.mgmt.containerservicefleet.v2022_06_02_preview.models.FleetMember]
+        :keyword next_link: The link to the next page of items.
+        :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
-        self.next_link = None
+        self.next_link = next_link
 
 
 class FleetPatch(_serialization.Model):
     """Properties of a Fleet that can be patched.
 
     :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/models/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/_fleet_members_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/_fleet_members_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -692,16 +692,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self,
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/_fleets_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/_fleets_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -949,16 +949,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self, resource_group_name: str, fleet_name: str, if_match: Optional[str] = None, **kwargs: Any
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/_configuration.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/_container_service_fleet_mgmt_client.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/_container_service_fleet_mgmt_client.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/_vendor.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/_configuration.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/_container_service_fleet_mgmt_client.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/_container_service_fleet_mgmt_client.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/operations/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/operations/_fleet_members_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/operations/_fleet_members_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/operations/_fleets_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/operations/_fleets_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/operations/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/models/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/models/_container_service_fleet_mgmt_client_enums.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/models/_container_service_fleet_mgmt_client_enums.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/models/_models_py3.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/models/_models_py3.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/models/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/operations/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/operations/_fleet_members_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/operations/_fleet_members_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/operations/_fleets_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/operations/_fleets_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/operations/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_07_02_preview/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/_configuration.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/_container_service_fleet_mgmt_client.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/_container_service_fleet_mgmt_client.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/_vendor.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/_configuration.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/_container_service_fleet_mgmt_client.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/_container_service_fleet_mgmt_client.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/operations/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/operations/_fleet_members_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/operations/_fleet_members_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/operations/_fleets_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/operations/_fleets_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/operations/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/models/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/models/_container_service_fleet_mgmt_client_enums.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/models/_container_service_fleet_mgmt_client_enums.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/models/_models_py3.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/models/_models_py3.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/models/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/operations/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/operations/_fleet_members_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/operations/_fleet_members_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/operations/_fleets_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/operations/_fleets_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/operations/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2022_09_02_preview/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/_configuration.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/_container_service_fleet_mgmt_client.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/_container_service_fleet_mgmt_client.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/_vendor.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/_configuration.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/_container_service_fleet_mgmt_client.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/_container_service_fleet_mgmt_client.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/_fleet_members_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/_fleet_members_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -670,16 +670,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self,
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/_fleets_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/_fleets_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -709,16 +709,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self, resource_group_name: str, fleet_name: str, if_match: Optional[str] = None, **kwargs: Any
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/_update_runs_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/_update_runs_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -512,16 +512,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self,
@@ -643,16 +643,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("UpdateRun", pipeline_response)
 
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace_async
@@ -782,16 +782,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("UpdateRun", pipeline_response)
 
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace_async
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/models/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/models/_container_service_fleet_mgmt_client_enums.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/models/_container_service_fleet_mgmt_client_enums.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/models/_models_py3.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/models/_models_py3.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,42 +378,41 @@
         self.fqdn = None
         self.kubernetes_version = None
 
 
 class FleetListResult(_serialization.Model):
     """The response of a Fleet list operation.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     All required parameters must be populated in order to send to server.
 
     :ivar value: The Fleet items on this page. Required.
     :vartype value: list[~azure.mgmt.containerservicefleet.v2023_03_15_preview.models.Fleet]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
-        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[Fleet]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.Fleet"], **kwargs: Any) -> None:
+    def __init__(self, *, value: List["_models.Fleet"], next_link: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword value: The Fleet items on this page. Required.
         :paramtype value: list[~azure.mgmt.containerservicefleet.v2023_03_15_preview.models.Fleet]
+        :keyword next_link: The link to the next page of items.
+        :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
-        self.next_link = None
+        self.next_link = next_link
 
 
 class ProxyResource(Resource):
     """The resource model definition for a Azure Resource Manager proxy resource. It will not have
     tags and a location.
 
     Variables are only populated by the server, and will be ignored when sending a request.
@@ -503,43 +502,42 @@
         self.group = group
         self.provisioning_state = None
 
 
 class FleetMemberListResult(_serialization.Model):
     """The response of a FleetMember list operation.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     All required parameters must be populated in order to send to server.
 
     :ivar value: The FleetMember items on this page. Required.
     :vartype value: list[~azure.mgmt.containerservicefleet.v2023_03_15_preview.models.FleetMember]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
-        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[FleetMember]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.FleetMember"], **kwargs: Any) -> None:
+    def __init__(self, *, value: List["_models.FleetMember"], next_link: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword value: The FleetMember items on this page. Required.
         :paramtype value:
          list[~azure.mgmt.containerservicefleet.v2023_03_15_preview.models.FleetMember]
+        :keyword next_link: The link to the next page of items.
+        :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
-        self.next_link = None
+        self.next_link = next_link
 
 
 class FleetMemberUpdate(_serialization.Model):
     """The type used for update operations of the FleetMember.
 
     :ivar group: The group this member belongs to for multi-cluster update management.
     :vartype group: str
@@ -1030,42 +1028,41 @@
         self.managed_cluster_update = managed_cluster_update
         self.status = None
 
 
 class UpdateRunListResult(_serialization.Model):
     """The response of a UpdateRun list operation.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     All required parameters must be populated in order to send to server.
 
     :ivar value: The UpdateRun items on this page. Required.
     :vartype value: list[~azure.mgmt.containerservicefleet.v2023_03_15_preview.models.UpdateRun]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
-        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[UpdateRun]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.UpdateRun"], **kwargs: Any) -> None:
+    def __init__(self, *, value: List["_models.UpdateRun"], next_link: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword value: The UpdateRun items on this page. Required.
         :paramtype value: list[~azure.mgmt.containerservicefleet.v2023_03_15_preview.models.UpdateRun]
+        :keyword next_link: The link to the next page of items.
+        :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
-        self.next_link = None
+        self.next_link = next_link
 
 
 class UpdateRunStatus(_serialization.Model):
     """The status of a UpdateRun.
 
     Variables are only populated by the server, and will be ignored when sending a request.
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/models/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/_fleet_members_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/_fleet_members_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -905,16 +905,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self,
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/_fleets_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/_fleets_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -949,16 +949,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self, resource_group_name: str, fleet_name: str, if_match: Optional[str] = None, **kwargs: Any
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/_update_runs_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/_update_runs_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -787,16 +787,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self,
@@ -918,16 +918,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("UpdateRun", pipeline_response)
 
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace
@@ -1056,16 +1056,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("UpdateRun", pipeline_response)
 
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/_configuration.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/_container_service_fleet_mgmt_client.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/_container_service_fleet_mgmt_client.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/_vendor.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/_configuration.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/_container_service_fleet_mgmt_client.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/_container_service_fleet_mgmt_client.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/_fleet_members_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/_fleet_members_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -528,16 +528,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("FleetMember", pipeline_response)
 
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @overload
@@ -745,16 +745,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self,
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/_fleets_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/_fleets_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -582,16 +582,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("Fleet", pipeline_response)
 
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @overload
@@ -779,16 +779,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self, resource_group_name: str, fleet_name: str, if_match: Optional[str] = None, **kwargs: Any
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/_update_runs_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/_update_runs_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -512,16 +512,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self,
@@ -643,16 +643,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("UpdateRun", pipeline_response)
 
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace_async
@@ -782,16 +782,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("UpdateRun", pipeline_response)
 
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace_async
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/models/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/models/_container_service_fleet_mgmt_client_enums.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/models/_container_service_fleet_mgmt_client_enums.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/models/_models_py3.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/models/_models_py3.py`

 * *Files 2% similar despite different names*

```diff
@@ -475,42 +475,41 @@
         self.fqdn = None
         self.kubernetes_version = None
 
 
 class FleetListResult(_serialization.Model):
     """The response of a Fleet list operation.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     All required parameters must be populated in order to send to server.
 
     :ivar value: The Fleet items on this page. Required.
     :vartype value: list[~azure.mgmt.containerservicefleet.v2023_06_15_preview.models.Fleet]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
-        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[Fleet]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.Fleet"], **kwargs: Any) -> None:
+    def __init__(self, *, value: List["_models.Fleet"], next_link: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword value: The Fleet items on this page. Required.
         :paramtype value: list[~azure.mgmt.containerservicefleet.v2023_06_15_preview.models.Fleet]
+        :keyword next_link: The link to the next page of items.
+        :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
-        self.next_link = None
+        self.next_link = next_link
 
 
 class ProxyResource(Resource):
     """The resource model definition for a Azure Resource Manager proxy resource. It will not have
     tags and a location.
 
     Variables are only populated by the server, and will be ignored when sending a request.
@@ -600,43 +599,42 @@
         self.group = group
         self.provisioning_state = None
 
 
 class FleetMemberListResult(_serialization.Model):
     """The response of a FleetMember list operation.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     All required parameters must be populated in order to send to server.
 
     :ivar value: The FleetMember items on this page. Required.
     :vartype value: list[~azure.mgmt.containerservicefleet.v2023_06_15_preview.models.FleetMember]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
-        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[FleetMember]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.FleetMember"], **kwargs: Any) -> None:
+    def __init__(self, *, value: List["_models.FleetMember"], next_link: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword value: The FleetMember items on this page. Required.
         :paramtype value:
          list[~azure.mgmt.containerservicefleet.v2023_06_15_preview.models.FleetMember]
+        :keyword next_link: The link to the next page of items.
+        :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
-        self.next_link = None
+        self.next_link = next_link
 
 
 class FleetMemberUpdate(_serialization.Model):
     """The type used for update operations of the FleetMember.
 
     :ivar group: The group this member belongs to for multi-cluster update management.
     :vartype group: str
@@ -1305,42 +1303,41 @@
         self.managed_cluster_update = managed_cluster_update
         self.status = None
 
 
 class UpdateRunListResult(_serialization.Model):
     """The response of a UpdateRun list operation.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     All required parameters must be populated in order to send to server.
 
     :ivar value: The UpdateRun items on this page. Required.
     :vartype value: list[~azure.mgmt.containerservicefleet.v2023_06_15_preview.models.UpdateRun]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
-        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[UpdateRun]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.UpdateRun"], **kwargs: Any) -> None:
+    def __init__(self, *, value: List["_models.UpdateRun"], next_link: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword value: The UpdateRun items on this page. Required.
         :paramtype value: list[~azure.mgmt.containerservicefleet.v2023_06_15_preview.models.UpdateRun]
+        :keyword next_link: The link to the next page of items.
+        :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
-        self.next_link = None
+        self.next_link = next_link
 
 
 class UpdateRunStatus(_serialization.Model):
     """The status of a UpdateRun.
 
     Variables are only populated by the server, and will be ignored when sending a request.
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/models/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/_fleet_members_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/_fleet_members_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -763,16 +763,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("FleetMember", pipeline_response)
 
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @overload
@@ -979,16 +979,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self,
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/_fleets_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/_fleets_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -822,16 +822,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("Fleet", pipeline_response)
 
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @overload
@@ -1018,16 +1018,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self, resource_group_name: str, fleet_name: str, if_match: Optional[str] = None, **kwargs: Any
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/_update_runs_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/_update_runs_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -787,16 +787,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self,
@@ -918,16 +918,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("UpdateRun", pipeline_response)
 
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace
@@ -1056,16 +1056,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("UpdateRun", pipeline_response)
 
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/_configuration.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/_container_service_fleet_mgmt_client.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/_container_service_fleet_mgmt_client.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/_vendor.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/_configuration.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/_container_service_fleet_mgmt_client.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/_container_service_fleet_mgmt_client.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_fleet_members_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_fleet_members_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -528,16 +528,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("FleetMember", pipeline_response)
 
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @overload
@@ -745,16 +745,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self,
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_fleet_update_strategies_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_fleet_update_strategies_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -511,16 +511,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self,
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_fleets_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_fleets_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -582,16 +582,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("Fleet", pipeline_response)
 
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @overload
@@ -779,16 +779,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self, resource_group_name: str, fleet_name: str, if_match: Optional[str] = None, **kwargs: Any
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_update_runs_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_update_runs_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -512,16 +512,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self,
@@ -643,16 +643,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("UpdateRun", pipeline_response)
 
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace_async
@@ -782,16 +782,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("UpdateRun", pipeline_response)
 
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace_async
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/models/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/models/_container_service_fleet_mgmt_client_enums.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/models/_container_service_fleet_mgmt_client_enums.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/models/_models_py3.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/models/_models_py3.py`

 * *Files 2% similar despite different names*

```diff
@@ -486,42 +486,41 @@
         self.kubernetes_version = None
         self.portal_fqdn = None
 
 
 class FleetListResult(_serialization.Model):
     """The response of a Fleet list operation.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     All required parameters must be populated in order to send to server.
 
     :ivar value: The Fleet items on this page. Required.
     :vartype value: list[~azure.mgmt.containerservicefleet.v2023_08_15_preview.models.Fleet]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
-        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[Fleet]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.Fleet"], **kwargs: Any) -> None:
+    def __init__(self, *, value: List["_models.Fleet"], next_link: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword value: The Fleet items on this page. Required.
         :paramtype value: list[~azure.mgmt.containerservicefleet.v2023_08_15_preview.models.Fleet]
+        :keyword next_link: The link to the next page of items.
+        :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
-        self.next_link = None
+        self.next_link = next_link
 
 
 class ProxyResource(Resource):
     """The resource model definition for a Azure Resource Manager proxy resource. It will not have
     tags and a location.
 
     Variables are only populated by the server, and will be ignored when sending a request.
@@ -611,43 +610,42 @@
         self.group = group
         self.provisioning_state = None
 
 
 class FleetMemberListResult(_serialization.Model):
     """The response of a FleetMember list operation.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     All required parameters must be populated in order to send to server.
 
     :ivar value: The FleetMember items on this page. Required.
     :vartype value: list[~azure.mgmt.containerservicefleet.v2023_08_15_preview.models.FleetMember]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
-        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[FleetMember]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.FleetMember"], **kwargs: Any) -> None:
+    def __init__(self, *, value: List["_models.FleetMember"], next_link: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword value: The FleetMember items on this page. Required.
         :paramtype value:
          list[~azure.mgmt.containerservicefleet.v2023_08_15_preview.models.FleetMember]
+        :keyword next_link: The link to the next page of items.
+        :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
-        self.next_link = None
+        self.next_link = next_link
 
 
 class FleetMemberUpdate(_serialization.Model):
     """The type used for update operations of the FleetMember.
 
     :ivar group: The group this member belongs to for multi-cluster update management.
     :vartype group: str
@@ -764,44 +762,45 @@
         self.provisioning_state = None
         self.strategy = strategy
 
 
 class FleetUpdateStrategyListResult(_serialization.Model):
     """The response of a FleetUpdateStrategy list operation.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     All required parameters must be populated in order to send to server.
 
     :ivar value: The FleetUpdateStrategy items on this page. Required.
     :vartype value:
      list[~azure.mgmt.containerservicefleet.v2023_08_15_preview.models.FleetUpdateStrategy]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
-        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[FleetUpdateStrategy]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.FleetUpdateStrategy"], **kwargs: Any) -> None:
+    def __init__(
+        self, *, value: List["_models.FleetUpdateStrategy"], next_link: Optional[str] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword value: The FleetUpdateStrategy items on this page. Required.
         :paramtype value:
          list[~azure.mgmt.containerservicefleet.v2023_08_15_preview.models.FleetUpdateStrategy]
+        :keyword next_link: The link to the next page of items.
+        :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
-        self.next_link = None
+        self.next_link = next_link
 
 
 class ManagedClusterUpdate(_serialization.Model):
     """The update to be applied to the ManagedClusters.
 
     All required parameters must be populated in order to send to server.
 
@@ -1451,42 +1450,41 @@
         self.managed_cluster_update = managed_cluster_update
         self.status = None
 
 
 class UpdateRunListResult(_serialization.Model):
     """The response of a UpdateRun list operation.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     All required parameters must be populated in order to send to server.
 
     :ivar value: The UpdateRun items on this page. Required.
     :vartype value: list[~azure.mgmt.containerservicefleet.v2023_08_15_preview.models.UpdateRun]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
-        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[UpdateRun]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.UpdateRun"], **kwargs: Any) -> None:
+    def __init__(self, *, value: List["_models.UpdateRun"], next_link: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword value: The UpdateRun items on this page. Required.
         :paramtype value: list[~azure.mgmt.containerservicefleet.v2023_08_15_preview.models.UpdateRun]
+        :keyword next_link: The link to the next page of items.
+        :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
-        self.next_link = None
+        self.next_link = next_link
 
 
 class UpdateRunStatus(_serialization.Model):
     """The status of a UpdateRun.
 
     Variables are only populated by the server, and will be ignored when sending a request.
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/models/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_fleet_members_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_fleet_members_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -763,16 +763,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("FleetMember", pipeline_response)
 
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @overload
@@ -979,16 +979,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self,
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_fleet_update_strategies_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_fleet_update_strategies_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -693,16 +693,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self,
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_fleets_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_fleets_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -822,16 +822,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("Fleet", pipeline_response)
 
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @overload
@@ -1018,16 +1018,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self, resource_group_name: str, fleet_name: str, if_match: Optional[str] = None, **kwargs: Any
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_update_runs_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_update_runs_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -787,16 +787,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self,
@@ -918,16 +918,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("UpdateRun", pipeline_response)
 
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace
@@ -1056,16 +1056,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("UpdateRun", pipeline_response)
 
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/_configuration.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/_container_service_fleet_mgmt_client.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/_container_service_fleet_mgmt_client.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/_vendor.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/_configuration.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/_container_service_fleet_mgmt_client.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/_container_service_fleet_mgmt_client.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_fleet_members_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_fleet_members_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -517,16 +517,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("FleetMember", pipeline_response)
 
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @overload
@@ -729,16 +729,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self,
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_fleet_update_strategies_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_fleet_update_strategies_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -500,16 +500,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self,
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_fleets_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_fleets_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -570,16 +570,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("Fleet", pipeline_response)
 
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @overload
@@ -762,16 +762,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self, resource_group_name: str, fleet_name: str, if_match: Optional[str] = None, **kwargs: Any
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_update_runs_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_update_runs_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,16 +501,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self,
@@ -628,16 +628,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("UpdateRun", pipeline_response)
 
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace_async
@@ -763,16 +763,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("UpdateRun", pipeline_response)
 
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace_async
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/models/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/models/_container_service_fleet_mgmt_client_enums.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/models/_container_service_fleet_mgmt_client_enums.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/models/_models_py3.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/models/_models_py3.py`

 * *Files 2% similar despite different names*

```diff
@@ -336,42 +336,41 @@
         super().__init__(**kwargs)
         self.kubeconfigs = None
 
 
 class FleetListResult(_serialization.Model):
     """The response of a Fleet list operation.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     All required parameters must be populated in order to send to server.
 
     :ivar value: The Fleet items on this page. Required.
     :vartype value: list[~azure.mgmt.containerservicefleet.v2023_10_15.models.Fleet]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
-        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[Fleet]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.Fleet"], **kwargs: Any) -> None:
+    def __init__(self, *, value: List["_models.Fleet"], next_link: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword value: The Fleet items on this page. Required.
         :paramtype value: list[~azure.mgmt.containerservicefleet.v2023_10_15.models.Fleet]
+        :keyword next_link: The link to the next page of items.
+        :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
-        self.next_link = None
+        self.next_link = next_link
 
 
 class ProxyResource(Resource):
     """The resource model definition for a Azure Resource Manager proxy resource. It will not have
     tags and a location.
 
     Variables are only populated by the server, and will be ignored when sending a request.
@@ -461,42 +460,41 @@
         self.group = group
         self.provisioning_state = None
 
 
 class FleetMemberListResult(_serialization.Model):
     """The response of a FleetMember list operation.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     All required parameters must be populated in order to send to server.
 
     :ivar value: The FleetMember items on this page. Required.
     :vartype value: list[~azure.mgmt.containerservicefleet.v2023_10_15.models.FleetMember]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
-        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[FleetMember]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.FleetMember"], **kwargs: Any) -> None:
+    def __init__(self, *, value: List["_models.FleetMember"], next_link: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword value: The FleetMember items on this page. Required.
         :paramtype value: list[~azure.mgmt.containerservicefleet.v2023_10_15.models.FleetMember]
+        :keyword next_link: The link to the next page of items.
+        :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
-        self.next_link = None
+        self.next_link = next_link
 
 
 class FleetMemberUpdate(_serialization.Model):
     """The type used for update operations of the FleetMember.
 
     :ivar group: The group this member belongs to for multi-cluster update management.
     :vartype group: str
@@ -610,43 +608,44 @@
         self.provisioning_state = None
         self.strategy = strategy
 
 
 class FleetUpdateStrategyListResult(_serialization.Model):
     """The response of a FleetUpdateStrategy list operation.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     All required parameters must be populated in order to send to server.
 
     :ivar value: The FleetUpdateStrategy items on this page. Required.
     :vartype value: list[~azure.mgmt.containerservicefleet.v2023_10_15.models.FleetUpdateStrategy]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
-        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[FleetUpdateStrategy]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.FleetUpdateStrategy"], **kwargs: Any) -> None:
+    def __init__(
+        self, *, value: List["_models.FleetUpdateStrategy"], next_link: Optional[str] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword value: The FleetUpdateStrategy items on this page. Required.
         :paramtype value:
          list[~azure.mgmt.containerservicefleet.v2023_10_15.models.FleetUpdateStrategy]
+        :keyword next_link: The link to the next page of items.
+        :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
-        self.next_link = None
+        self.next_link = next_link
 
 
 class ManagedClusterUpdate(_serialization.Model):
     """The update to be applied to the ManagedClusters.
 
     All required parameters must be populated in order to send to server.
 
@@ -1291,42 +1290,41 @@
         self.managed_cluster_update = managed_cluster_update
         self.status = None
 
 
 class UpdateRunListResult(_serialization.Model):
     """The response of a UpdateRun list operation.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     All required parameters must be populated in order to send to server.
 
     :ivar value: The UpdateRun items on this page. Required.
     :vartype value: list[~azure.mgmt.containerservicefleet.v2023_10_15.models.UpdateRun]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
-        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[UpdateRun]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.UpdateRun"], **kwargs: Any) -> None:
+    def __init__(self, *, value: List["_models.UpdateRun"], next_link: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword value: The UpdateRun items on this page. Required.
         :paramtype value: list[~azure.mgmt.containerservicefleet.v2023_10_15.models.UpdateRun]
+        :keyword next_link: The link to the next page of items.
+        :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
-        self.next_link = None
+        self.next_link = next_link
 
 
 class UpdateRunStatus(_serialization.Model):
     """The status of a UpdateRun.
 
     Variables are only populated by the server, and will be ignored when sending a request.
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/models/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_fleet_members_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_fleet_members_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -752,16 +752,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("FleetMember", pipeline_response)
 
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @overload
@@ -963,16 +963,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self,
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_fleet_update_strategies_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_fleet_update_strategies_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -682,16 +682,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self,
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_fleets_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_fleets_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -810,16 +810,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("Fleet", pipeline_response)
 
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @overload
@@ -1001,16 +1001,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self, resource_group_name: str, fleet_name: str, if_match: Optional[str] = None, **kwargs: Any
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_update_runs_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2023_10_15/operations/_update_runs_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -776,16 +776,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self,
@@ -903,16 +903,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("UpdateRun", pipeline_response)
 
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace
@@ -1037,16 +1037,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("UpdateRun", pipeline_response)
 
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/_configuration.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/_container_service_fleet_mgmt_client.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/_container_service_fleet_mgmt_client.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/_vendor.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/_configuration.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/_container_service_fleet_mgmt_client.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/_container_service_fleet_mgmt_client.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_fleet_members_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_fleet_members_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -528,16 +528,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("FleetMember", pipeline_response)
 
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @overload
@@ -745,16 +745,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self,
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_fleet_update_strategies_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_fleet_update_strategies_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -511,16 +511,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self,
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_fleets_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_fleets_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -582,16 +582,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("Fleet", pipeline_response)
 
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @overload
@@ -779,16 +779,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self, resource_group_name: str, fleet_name: str, if_match: Optional[str] = None, **kwargs: Any
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_update_runs_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_update_runs_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -513,16 +513,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self,
@@ -657,16 +657,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("UpdateRun", pipeline_response)
 
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @overload
@@ -876,16 +876,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("UpdateRun", pipeline_response)
 
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace_async
@@ -1015,16 +1015,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("UpdateRun", pipeline_response)
 
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace_async
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/models/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/models/_container_service_fleet_mgmt_client_enums.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/models/_container_service_fleet_mgmt_client_enums.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/models/_models_py3.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/models/_models_py3.py`

 * *Files 2% similar despite different names*

```diff
@@ -486,42 +486,41 @@
         self.kubernetes_version = None
         self.portal_fqdn = None
 
 
 class FleetListResult(_serialization.Model):
     """The response of a Fleet list operation.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     All required parameters must be populated in order to send to server.
 
     :ivar value: The Fleet items on this page. Required.
     :vartype value: list[~azure.mgmt.containerservicefleet.v2024_02_02_preview.models.Fleet]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
-        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[Fleet]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.Fleet"], **kwargs: Any) -> None:
+    def __init__(self, *, value: List["_models.Fleet"], next_link: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword value: The Fleet items on this page. Required.
         :paramtype value: list[~azure.mgmt.containerservicefleet.v2024_02_02_preview.models.Fleet]
+        :keyword next_link: The link to the next page of items.
+        :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
-        self.next_link = None
+        self.next_link = next_link
 
 
 class ProxyResource(Resource):
     """The resource model definition for a Azure Resource Manager proxy resource. It will not have
     tags and a location.
 
     Variables are only populated by the server, and will be ignored when sending a request.
@@ -611,43 +610,42 @@
         self.group = group
         self.provisioning_state = None
 
 
 class FleetMemberListResult(_serialization.Model):
     """The response of a FleetMember list operation.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     All required parameters must be populated in order to send to server.
 
     :ivar value: The FleetMember items on this page. Required.
     :vartype value: list[~azure.mgmt.containerservicefleet.v2024_02_02_preview.models.FleetMember]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
-        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[FleetMember]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.FleetMember"], **kwargs: Any) -> None:
+    def __init__(self, *, value: List["_models.FleetMember"], next_link: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword value: The FleetMember items on this page. Required.
         :paramtype value:
          list[~azure.mgmt.containerservicefleet.v2024_02_02_preview.models.FleetMember]
+        :keyword next_link: The link to the next page of items.
+        :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
-        self.next_link = None
+        self.next_link = next_link
 
 
 class FleetMemberUpdate(_serialization.Model):
     """The type used for update operations of the FleetMember.
 
     :ivar group: The group this member belongs to for multi-cluster update management.
     :vartype group: str
@@ -764,44 +762,45 @@
         self.provisioning_state = None
         self.strategy = strategy
 
 
 class FleetUpdateStrategyListResult(_serialization.Model):
     """The response of a FleetUpdateStrategy list operation.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     All required parameters must be populated in order to send to server.
 
     :ivar value: The FleetUpdateStrategy items on this page. Required.
     :vartype value:
      list[~azure.mgmt.containerservicefleet.v2024_02_02_preview.models.FleetUpdateStrategy]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
-        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[FleetUpdateStrategy]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.FleetUpdateStrategy"], **kwargs: Any) -> None:
+    def __init__(
+        self, *, value: List["_models.FleetUpdateStrategy"], next_link: Optional[str] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword value: The FleetUpdateStrategy items on this page. Required.
         :paramtype value:
          list[~azure.mgmt.containerservicefleet.v2024_02_02_preview.models.FleetUpdateStrategy]
+        :keyword next_link: The link to the next page of items.
+        :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
-        self.next_link = None
+        self.next_link = next_link
 
 
 class ManagedClusterUpdate(_serialization.Model):
     """The update to be applied to the ManagedClusters.
 
     All required parameters must be populated in order to send to server.
 
@@ -1517,42 +1516,41 @@
         self.managed_cluster_update = managed_cluster_update
         self.status = None
 
 
 class UpdateRunListResult(_serialization.Model):
     """The response of a UpdateRun list operation.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     All required parameters must be populated in order to send to server.
 
     :ivar value: The UpdateRun items on this page. Required.
     :vartype value: list[~azure.mgmt.containerservicefleet.v2024_02_02_preview.models.UpdateRun]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
-        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[UpdateRun]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.UpdateRun"], **kwargs: Any) -> None:
+    def __init__(self, *, value: List["_models.UpdateRun"], next_link: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword value: The UpdateRun items on this page. Required.
         :paramtype value: list[~azure.mgmt.containerservicefleet.v2024_02_02_preview.models.UpdateRun]
+        :keyword next_link: The link to the next page of items.
+        :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
-        self.next_link = None
+        self.next_link = next_link
 
 
 class UpdateRunStatus(_serialization.Model):
     """The status of a UpdateRun.
 
     Variables are only populated by the server, and will be ignored when sending a request.
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/models/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/__init__.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_fleet_members_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_fleet_members_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -763,16 +763,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("FleetMember", pipeline_response)
 
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @overload
@@ -979,16 +979,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self,
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_fleet_update_strategies_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_fleet_update_strategies_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -693,16 +693,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self,
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_fleets_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_fleets_operations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -822,16 +822,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("Fleet", pipeline_response)
 
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @overload
@@ -1018,16 +1018,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self, resource_group_name: str, fleet_name: str, if_match: Optional[str] = None, **kwargs: Any
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_patch.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_update_runs_operations.py` & `azure-mgmt-containerservicefleet-2.0.0/azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_update_runs_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -841,16 +841,16 @@
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self,
@@ -985,16 +985,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("UpdateRun", pipeline_response)
 
         if response.status_code == 202:
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @overload
@@ -1201,16 +1201,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("UpdateRun", pipeline_response)
 
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace
@@ -1339,16 +1339,16 @@
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("UpdateRun", pipeline_response)
 
         if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure_mgmt_containerservicefleet.egg-info/PKG-INFO` & `azure-mgmt-containerservicefleet-2.0.0/azure_mgmt_containerservicefleet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-containerservicefleet
-Version: 1.1.0
+Version: 2.0.0
 Summary: Microsoft Azure Containerservicefleet Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,17 +16,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: isodate>=0.6.1
-Requires-Dist: azure-common>=1.1
-Requires-Dist: azure-mgmt-core>=1.3.2
 
 # Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Containerservicefleet Management Client Library.
 This package has been tested with Python 3.8+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
@@ -85,14 +82,21 @@
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 # Release History
 
+## 2.0.0 (2024-05-20)
+
+### Breaking Changes
+
+  - Model APIServerAccessProfile no longer has parameter enable_vnet_integration
+  - Model APIServerAccessProfile no longer has parameter subnet_id
+
 ## 1.1.0 (2024-04-03)
 
 ### Features Added
 
   - Added operation UpdateRunsOperations.begin_skip
   - Model Fleet has a new parameter hub_profile
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/azure_mgmt_containerservicefleet.egg-info/SOURCES.txt` & `azure-mgmt-containerservicefleet-2.0.0/azure_mgmt_containerservicefleet.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 azure/mgmt/containerservicefleet/aio/_container_service_fleet_mgmt_client.py
 azure/mgmt/containerservicefleet/v2022_06_02_preview/__init__.py
 azure/mgmt/containerservicefleet/v2022_06_02_preview/_configuration.py
 azure/mgmt/containerservicefleet/v2022_06_02_preview/_container_service_fleet_mgmt_client.py
 azure/mgmt/containerservicefleet/v2022_06_02_preview/_patch.py
 azure/mgmt/containerservicefleet/v2022_06_02_preview/_vendor.py
 azure/mgmt/containerservicefleet/v2022_06_02_preview/_version.py
-azure/mgmt/containerservicefleet/v2022_06_02_preview/py.typed
 azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/__init__.py
 azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/_configuration.py
 azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/_container_service_fleet_mgmt_client.py
 azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/_patch.py
 azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/__init__.py
 azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/_fleet_members_operations.py
 azure/mgmt/containerservicefleet/v2022_06_02_preview/aio/operations/_fleets_operations.py
@@ -43,15 +42,14 @@
 azure/mgmt/containerservicefleet/v2022_06_02_preview/operations/_patch.py
 azure/mgmt/containerservicefleet/v2022_07_02_preview/__init__.py
 azure/mgmt/containerservicefleet/v2022_07_02_preview/_configuration.py
 azure/mgmt/containerservicefleet/v2022_07_02_preview/_container_service_fleet_mgmt_client.py
 azure/mgmt/containerservicefleet/v2022_07_02_preview/_patch.py
 azure/mgmt/containerservicefleet/v2022_07_02_preview/_vendor.py
 azure/mgmt/containerservicefleet/v2022_07_02_preview/_version.py
-azure/mgmt/containerservicefleet/v2022_07_02_preview/py.typed
 azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/__init__.py
 azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/_configuration.py
 azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/_container_service_fleet_mgmt_client.py
 azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/_patch.py
 azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/operations/__init__.py
 azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/operations/_fleet_members_operations.py
 azure/mgmt/containerservicefleet/v2022_07_02_preview/aio/operations/_fleets_operations.py
@@ -66,15 +64,14 @@
 azure/mgmt/containerservicefleet/v2022_07_02_preview/operations/_patch.py
 azure/mgmt/containerservicefleet/v2022_09_02_preview/__init__.py
 azure/mgmt/containerservicefleet/v2022_09_02_preview/_configuration.py
 azure/mgmt/containerservicefleet/v2022_09_02_preview/_container_service_fleet_mgmt_client.py
 azure/mgmt/containerservicefleet/v2022_09_02_preview/_patch.py
 azure/mgmt/containerservicefleet/v2022_09_02_preview/_vendor.py
 azure/mgmt/containerservicefleet/v2022_09_02_preview/_version.py
-azure/mgmt/containerservicefleet/v2022_09_02_preview/py.typed
 azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/__init__.py
 azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/_configuration.py
 azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/_container_service_fleet_mgmt_client.py
 azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/_patch.py
 azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/operations/__init__.py
 azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/operations/_fleet_members_operations.py
 azure/mgmt/containerservicefleet/v2022_09_02_preview/aio/operations/_fleets_operations.py
@@ -89,15 +86,14 @@
 azure/mgmt/containerservicefleet/v2022_09_02_preview/operations/_patch.py
 azure/mgmt/containerservicefleet/v2023_03_15_preview/__init__.py
 azure/mgmt/containerservicefleet/v2023_03_15_preview/_configuration.py
 azure/mgmt/containerservicefleet/v2023_03_15_preview/_container_service_fleet_mgmt_client.py
 azure/mgmt/containerservicefleet/v2023_03_15_preview/_patch.py
 azure/mgmt/containerservicefleet/v2023_03_15_preview/_vendor.py
 azure/mgmt/containerservicefleet/v2023_03_15_preview/_version.py
-azure/mgmt/containerservicefleet/v2023_03_15_preview/py.typed
 azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/__init__.py
 azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/_configuration.py
 azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/_container_service_fleet_mgmt_client.py
 azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/_patch.py
 azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/__init__.py
 azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/_fleet_members_operations.py
 azure/mgmt/containerservicefleet/v2023_03_15_preview/aio/operations/_fleets_operations.py
@@ -116,15 +112,14 @@
 azure/mgmt/containerservicefleet/v2023_03_15_preview/operations/_update_runs_operations.py
 azure/mgmt/containerservicefleet/v2023_06_15_preview/__init__.py
 azure/mgmt/containerservicefleet/v2023_06_15_preview/_configuration.py
 azure/mgmt/containerservicefleet/v2023_06_15_preview/_container_service_fleet_mgmt_client.py
 azure/mgmt/containerservicefleet/v2023_06_15_preview/_patch.py
 azure/mgmt/containerservicefleet/v2023_06_15_preview/_vendor.py
 azure/mgmt/containerservicefleet/v2023_06_15_preview/_version.py
-azure/mgmt/containerservicefleet/v2023_06_15_preview/py.typed
 azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/__init__.py
 azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/_configuration.py
 azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/_container_service_fleet_mgmt_client.py
 azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/_patch.py
 azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/__init__.py
 azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/_fleet_members_operations.py
 azure/mgmt/containerservicefleet/v2023_06_15_preview/aio/operations/_fleets_operations.py
@@ -143,15 +138,14 @@
 azure/mgmt/containerservicefleet/v2023_06_15_preview/operations/_update_runs_operations.py
 azure/mgmt/containerservicefleet/v2023_08_15_preview/__init__.py
 azure/mgmt/containerservicefleet/v2023_08_15_preview/_configuration.py
 azure/mgmt/containerservicefleet/v2023_08_15_preview/_container_service_fleet_mgmt_client.py
 azure/mgmt/containerservicefleet/v2023_08_15_preview/_patch.py
 azure/mgmt/containerservicefleet/v2023_08_15_preview/_vendor.py
 azure/mgmt/containerservicefleet/v2023_08_15_preview/_version.py
-azure/mgmt/containerservicefleet/v2023_08_15_preview/py.typed
 azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/__init__.py
 azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/_configuration.py
 azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/_container_service_fleet_mgmt_client.py
 azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/_patch.py
 azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/__init__.py
 azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_fleet_members_operations.py
 azure/mgmt/containerservicefleet/v2023_08_15_preview/aio/operations/_fleet_update_strategies_operations.py
@@ -172,15 +166,14 @@
 azure/mgmt/containerservicefleet/v2023_08_15_preview/operations/_update_runs_operations.py
 azure/mgmt/containerservicefleet/v2023_10_15/__init__.py
 azure/mgmt/containerservicefleet/v2023_10_15/_configuration.py
 azure/mgmt/containerservicefleet/v2023_10_15/_container_service_fleet_mgmt_client.py
 azure/mgmt/containerservicefleet/v2023_10_15/_patch.py
 azure/mgmt/containerservicefleet/v2023_10_15/_vendor.py
 azure/mgmt/containerservicefleet/v2023_10_15/_version.py
-azure/mgmt/containerservicefleet/v2023_10_15/py.typed
 azure/mgmt/containerservicefleet/v2023_10_15/aio/__init__.py
 azure/mgmt/containerservicefleet/v2023_10_15/aio/_configuration.py
 azure/mgmt/containerservicefleet/v2023_10_15/aio/_container_service_fleet_mgmt_client.py
 azure/mgmt/containerservicefleet/v2023_10_15/aio/_patch.py
 azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/__init__.py
 azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_fleet_members_operations.py
 azure/mgmt/containerservicefleet/v2023_10_15/aio/operations/_fleet_update_strategies_operations.py
@@ -201,15 +194,14 @@
 azure/mgmt/containerservicefleet/v2023_10_15/operations/_update_runs_operations.py
 azure/mgmt/containerservicefleet/v2024_02_02_preview/__init__.py
 azure/mgmt/containerservicefleet/v2024_02_02_preview/_configuration.py
 azure/mgmt/containerservicefleet/v2024_02_02_preview/_container_service_fleet_mgmt_client.py
 azure/mgmt/containerservicefleet/v2024_02_02_preview/_patch.py
 azure/mgmt/containerservicefleet/v2024_02_02_preview/_vendor.py
 azure/mgmt/containerservicefleet/v2024_02_02_preview/_version.py
-azure/mgmt/containerservicefleet/v2024_02_02_preview/py.typed
 azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/__init__.py
 azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/_configuration.py
 azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/_container_service_fleet_mgmt_client.py
 azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/_patch.py
 azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/__init__.py
 azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_fleet_members_operations.py
 azure/mgmt/containerservicefleet/v2024_02_02_preview/aio/operations/_fleet_update_strategies_operations.py
@@ -224,13 +216,41 @@
 azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/__init__.py
 azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_fleet_members_operations.py
 azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_fleet_update_strategies_operations.py
 azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_fleets_operations.py
 azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_operations.py
 azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_patch.py
 azure/mgmt/containerservicefleet/v2024_02_02_preview/operations/_update_runs_operations.py
+azure/mgmt/containerservicefleet/v2024_04_01/__init__.py
+azure/mgmt/containerservicefleet/v2024_04_01/_configuration.py
+azure/mgmt/containerservicefleet/v2024_04_01/_container_service_fleet_mgmt_client.py
+azure/mgmt/containerservicefleet/v2024_04_01/_patch.py
+azure/mgmt/containerservicefleet/v2024_04_01/_vendor.py
+azure/mgmt/containerservicefleet/v2024_04_01/_version.py
+azure/mgmt/containerservicefleet/v2024_04_01/aio/__init__.py
+azure/mgmt/containerservicefleet/v2024_04_01/aio/_configuration.py
+azure/mgmt/containerservicefleet/v2024_04_01/aio/_container_service_fleet_mgmt_client.py
+azure/mgmt/containerservicefleet/v2024_04_01/aio/_patch.py
+azure/mgmt/containerservicefleet/v2024_04_01/aio/operations/__init__.py
+azure/mgmt/containerservicefleet/v2024_04_01/aio/operations/_fleet_members_operations.py
+azure/mgmt/containerservicefleet/v2024_04_01/aio/operations/_fleet_update_strategies_operations.py
+azure/mgmt/containerservicefleet/v2024_04_01/aio/operations/_fleets_operations.py
+azure/mgmt/containerservicefleet/v2024_04_01/aio/operations/_operations.py
+azure/mgmt/containerservicefleet/v2024_04_01/aio/operations/_patch.py
+azure/mgmt/containerservicefleet/v2024_04_01/aio/operations/_update_runs_operations.py
+azure/mgmt/containerservicefleet/v2024_04_01/models/__init__.py
+azure/mgmt/containerservicefleet/v2024_04_01/models/_container_service_fleet_mgmt_client_enums.py
+azure/mgmt/containerservicefleet/v2024_04_01/models/_models_py3.py
+azure/mgmt/containerservicefleet/v2024_04_01/models/_patch.py
+azure/mgmt/containerservicefleet/v2024_04_01/operations/__init__.py
+azure/mgmt/containerservicefleet/v2024_04_01/operations/_fleet_members_operations.py
+azure/mgmt/containerservicefleet/v2024_04_01/operations/_fleet_update_strategies_operations.py
+azure/mgmt/containerservicefleet/v2024_04_01/operations/_fleets_operations.py
+azure/mgmt/containerservicefleet/v2024_04_01/operations/_operations.py
+azure/mgmt/containerservicefleet/v2024_04_01/operations/_patch.py
+azure/mgmt/containerservicefleet/v2024_04_01/operations/_update_runs_operations.py
 azure_mgmt_containerservicefleet.egg-info/PKG-INFO
 azure_mgmt_containerservicefleet.egg-info/SOURCES.txt
 azure_mgmt_containerservicefleet.egg-info/dependency_links.txt
 azure_mgmt_containerservicefleet.egg-info/not-zip-safe
 azure_mgmt_containerservicefleet.egg-info/requires.txt
 azure_mgmt_containerservicefleet.egg-info/top_level.txt
```

### Comparing `azure-mgmt-containerservicefleet-1.1.0/setup.py` & `azure-mgmt-containerservicefleet-2.0.0/setup.py`

 * *Files identical despite different names*

