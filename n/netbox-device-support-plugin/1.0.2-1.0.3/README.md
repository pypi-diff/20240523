# Comparing `tmp/netbox_device_support_plugin-1.0.2.tar.gz` & `tmp/netbox_device_support_plugin-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_device_support_plugin-1.0.2.tar", last modified: Fri May 17 19:44:05 2024, max compression
+gzip compressed data, was "netbox_device_support_plugin-1.0.3.tar", last modified: Wed May 22 12:09:36 2024, max compression
```

## Comparing `netbox_device_support_plugin-1.0.2.tar` & `netbox_device_support_plugin-1.0.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.606308 netbox_device_support_plugin-1.0.2/
--rw-r--r--   0 vsts      (1001) docker     (127)     1068 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)       58 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    13514 2024-05-17 19:44:05.606308 netbox_device_support_plugin-1.0.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)    12867 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.602308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2917 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/admin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.602308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/api/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4667 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/api/serializers.py
--rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/api/urls.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1657 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/api/views.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6089 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/filtersets.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13398 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/forms.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.602308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/management/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/management/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.602308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/management/commands/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/management/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    40821 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/management/commands/sync_cisco_support_data.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8273 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/management/commands/sync_fortinet_support_data.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8319 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/management/commands/sync_purestorage_support_data.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.602308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/migrations/
--rw-r--r--   0 vsts      (1001) docker     (127)     7956 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/migrations/0001_initial.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/migrations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    32812 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/models.py
--rw-r--r--   0 vsts      (1001) docker     (127)      739 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/navigation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5749 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/tables.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6535 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/template_content.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.598308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.602308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/
--rw-r--r--   0 vsts      (1001) docker     (127)     6284 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/cisco_device_support.html
--rw-r--r--   0 vsts      (1001) docker     (127)     4237 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/cisco_device_type_support.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.602308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/
--rw-r--r--   0 vsts      (1001) docker     (127)      832 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_contract_coverage_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      896 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_partner_contract_coverage_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)     1078 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eorfa_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eos_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)     1038 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eoscr_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)     1030 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eosm_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      966 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvca_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)     1046 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvs_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_last_day_support_bar.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.602308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/fortinet/
--rw-r--r--   0 vsts      (1001) docker     (127)     4308 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/fortinet/fortinet_device_support.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.606308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/fortinet/inc/
--rw-r--r--   0 vsts      (1001) docker     (127)      896 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/fortinet/inc/device_eor_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      896 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/fortinet/inc/device_eos_bar.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.606308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/purestorage/
--rw-r--r--   0 vsts      (1001) docker     (127)     1845 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/purestorage/purestorage_device_support.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.606308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templatetags/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templatetags/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2960 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templatetags/filters.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2107 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/urls.py
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3402 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/views.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.606308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    13514 2024-05-17 19:44:05.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2649 2024-05-17 19:44:05.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-17 19:44:05.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-17 19:44:05.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)       29 2024-05-17 19:44:05.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-17 19:44:05.606308 netbox_device_support_plugin-1.0.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1570 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.822099 netbox_device_support_plugin-1.0.3/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1068 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)       58 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    14554 2024-05-22 12:09:36.822099 netbox_device_support_plugin-1.0.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    13907 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.810099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1271 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2917 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/admin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.814099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/api/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4667 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/api/serializers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1272 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/api/urls.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1657 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/api/views.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6089 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/filtersets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13692 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/forms.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.814099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/management/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/management/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.814099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/management/commands/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/management/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40821 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/management/commands/sync_cisco_support_data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8273 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/management/commands/sync_fortinet_support_data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8319 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/management/commands/sync_purestorage_support_data.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.814099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/migrations/
+-rw-r--r--   0 vsts      (1001) docker     (127)     7956 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/migrations/0001_initial.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/migrations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    32739 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/models.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2362 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/navigation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5749 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/tables.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4639 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/template_content.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.810099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.818099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6033 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/cisco_device_support.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     4140 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/cisco_device_type_support.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.818099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/
+-rw-r--r--   0 vsts      (1001) docker     (127)      840 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_contract_coverage_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      904 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_partner_contract_coverage_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     1086 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eorfa_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      896 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eos_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     1046 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eoscr_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     1038 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eosm_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      974 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvca_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     1054 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvs_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_last_day_support_bar.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.818099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/fortinet/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3989 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/fortinet/fortinet_device_support.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.818099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/fortinet/inc/
+-rw-r--r--   0 vsts      (1001) docker     (127)      892 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/fortinet/inc/device_eor_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      892 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/fortinet/inc/device_eos_bar.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.818099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/purestorage/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1551 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/purestorage/purestorage_device_support.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.818099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templatetags/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templatetags/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2960 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templatetags/filters.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2107 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/urls.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3336 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/views.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.818099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    14554 2024-05-22 12:09:36.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2649 2024-05-22 12:09:36.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-22 12:09:36.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-22 12:09:36.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)       29 2024-05-22 12:09:36.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-22 12:09:36.822099 netbox_device_support_plugin-1.0.3/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1570 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/setup.py
```

### Comparing `netbox_device_support_plugin-1.0.2/LICENSE` & `netbox_device_support_plugin-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.2/PKG-INFO` & `netbox_device_support_plugin-1.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-device-support-plugin
-Version: 1.0.2
+Version: 1.0.3
 Summary: Cisco device support, device type support, and software release information with the Cisco support APIs
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
@@ -23,29 +23,41 @@
 # NetBox Cisco Support Plugin
 ----
 </br>
 
 This `README.md` documentation contains the following sections:
 
 * [Plugin Overview](#plugin-overview)
+    * [Cisco](#cisco)
+    * [Fortinet](#fortinet)
+    * [Pure Storage](#pure-storage)
 * [Compatibility](#compatibility)
 * [Installation](#installation)
 * [Enable the Plugin](#enable-the-plugin)
 * [Configure the Plugin](#configure-the-plugin)
+    * [Mandatory Settings](#mandatory-settings)
+    * [Optional Settings](#optional-settings)
 * [Rebuild and Restart NetBox-Docker](#rebuild-and-restart-netbox-docker)
 * [Run Database Migrations](#run-database-migrations)
-* [Sync the Cisco Support Data](#sync-the-device-support-data)
+* [Sync the Device Support Data](#sync-the-device-support-data)
+    * [Cisco](#cisco-1)
+    * [Fortinet](#fortinet-1)
+    * [Pure Storage](#pure-storage-1)
 * [How it works](#how-it-works)
 * [Plugin Screenshots](#plugin-screenshots)
 * [Languages and Tools](#languages-and-tools)
 
 # Plugin Overview
 ----
 </br>
 
+## Cisco
+----
+</br>
+
 This [NetBox](https://github.com/netbox-community/netbox) tracks with the data from the Cisco support APIs
 the device support status, the device type EoX status as well as the recommended software release. Each
 Cisco device and Cisco device type have a detail view with all data. There is also a list view with filter
 options for all devices or device types. All data can also be received and updated over the NetBox REST API.
 
 There is a Python script calles `sync_cisco_support_data` which can be used as below to update all fields
 which contains data from the Cisco support APIs. This script can be executed for example inside a Azure
@@ -126,25 +138,43 @@
 > **No Edit Views**
 >
 > Manual edit of fields only in the NetBox Django admin portal
 > At the moment there are no edit views to edit field of any data model of this plugin. The because the
 > idea of this plugin is not to change fields manually (only automated by Python or REST API). If you want
 > to change field manually, at the moment this can only be done in the NetBox Django admin portal.
 
+## Fortinet
+----
+</br>
+
+> **In Development**
+>
+> The device support coverage of Fortinet is in development
+
+## Pure Storage
+----
+</br>
+
+> **In Development**
+>
+> The device support coverage of Pure Storage is in development
+
 # Compatibility
 ----
 </br>
 
-> :warning: **NetBox 3.5**: This plugin is for NetBox 3.5
+> :warning: **NetBox 4.0**: The latest release of this plugin is for NetBox 4.0
 
 This plugin is compatible with [NetBox](https://netbox.readthedocs.org/) 3.5.0 and later.
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |      3.5       |      0.0.1     |
+|      4.0       |      1.0.3     |
+
 
 # Installation
 ----
 </br>
 
 The installation and configuration steps are for the [NetBox-Docker](https://github.com/netbox-community/netbox-docker)
 installation. To install this plugin make sure you followed the prerequisites for using NetBox plugins with
@@ -169,23 +199,31 @@
 
 Enable the `netbox-device-support-plugin` plugin in `/netbox-docker/configuration/plugins.py` and add the
 plugin configuration also in the same file.
 
 ```python
 # Enable installed plugins. Add the name of each plugin to the list.
 PLUGINS = [
-    "netbox_napalm_plugin",
     "netbox_device_support_plugin",
 ]
 ```
 
 # Configure the Plugin
 ----
 </br>
 
+> **Fortinet and Pure Storage in Development**
+>
+> The section plugin configuration describes only the vendor Cisco as Fortinet and Pure Storage are still
+> in development
+
+## Mandatory Settings
+----
+</br>
+
 In order to get valid API response data, several requirements must be fulfilled:
 
 1. A [Cisco API ID and secret](https://apiconsole.cisco.com/) (with access to the APIs "EoX V5 API",
 "Serial Number to Information API Version 2" and "Software Suggestion") must have been created and
 configured inside `plugins.py`
 
     The following plugin configuration options are mandatory for the Cisco support API.
@@ -203,27 +241,31 @@
         "netbox_device_support_plugin": {
             "CISCO_SUPPORT_API_CLIENT_ID": environ.get("CISCO_SUPPORT_API_CLIENT_ID", ""),
             "CISCO_SUPPORT_API_CLIENT_SECRET": environ.get("CISCO_SUPPORT_API_CLIENT_SECRET", ""),
         },
     }
     ```
 
-2. A manufacturer called `Cisco` must have been configured inside NetBox. If your manufacturer is named
+## Optional Settings
+----
+</br>
+
+1. A manufacturer called `Cisco`, must have been configured inside NetBox. If your manufacturer is named
 differently, change it inside the plugin configuration in `plugins.py`:
 
     ```python
     PLUGINS_CONFIG = {
         "netbox_device_support_plugin": {
             ...,
             "MANUFACTURER": "Cisco Systems" # Optional setting for definiing the manufacturer
         }
     }
     ```
 
-3. Optional the `TEMPLATE_EXTENSION_PLACEMENT` can be changed inside the plugin configuration in `plugins.py`:
+2. Optional the `TEMPLATE_EXTENSION_PLACEMENT` can be changed inside the plugin configuration in `plugins.py`:
 
     ```python
     PLUGINS_CONFIG = {
         "netbox_device_support_plugin": {
             ...,
             "TEMPLATE_EXTENSION_PLACEMENT": "left" # Optional setting render the content on the left or right side
         }
@@ -253,15 +295,19 @@
 
 Restore the database and run the Django database migration to your existing NetBox database.
 
 ```bash
 python3 manage.py migrate
 ```
 
-# Sync the Cisco Support Data
+# Sync the Device Support Data
+----
+</br>
+
+## Cisco
 ----
 </br>
 
 In order that `sync_cisco_support_data` works correctly, several requirements must be fulfilled:
 
 1. All devices types for manufacturer Cisco must have filled the optional `Part number` field inside NetBox
 with the correct Base PID for that Cisco product.
@@ -278,15 +324,15 @@
 ```bash
 python3 manage.py sync_cisco_support_data.py
 ```
 
 Execute a Azure DevOps Build Pipeline which runs `sync_cisco_support_data.py` to periodically refresh the
 data or create a cronjob which to the same a bit more old school.
 
-# How it works
+### How it works
 ----
 </br>
 
 1. Calling the `sync_cisco_support_data` method will catch all device types for the configured manufacturer.
 
 2. Each device types `Part number` will be send to Cisco EoX API. API answer will be saved inside a
 `CiscoDeviceTypeSupport` model. One `CiscoDeviceTypeSupport` per device type.
@@ -306,16 +352,33 @@
 7. Field Coloring: Expired timestamps or no data will be colored red, timestamps which will expire in the next
 calendar year will be colored yellow for planning or forecast reasons.
 
 8. Progress Bar: The progress bars will visualize the timestamps duration to the expiration date. The
 progress bar color will be green until the timestamp will expire in the next calendar year. Then the color
 will change to yellow. The color will finally change to red when the timestamp expire within 60 days.
 
+## Fortinet
+----
+</br>
+
+> **In Development**
+>
+> The device support coverage of Fortinet is in development
+
+## Pure Storage
+----
+</br>
+
+> **In Development**
+>
+> The device support coverage of Fortinet is in development
+
 # Plugin Screenshots
 ----
+</br>
 
 ## Device Detail View
 ![Device Detail View](images/device_detail_view.png)
 
 ## Device Type Detail View
 ![Device Type Detail View](images/device_type_detail_view.png)
```

### Comparing `netbox_device_support_plugin-1.0.2/README.md` & `netbox_device_support_plugin-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,41 @@
 # NetBox Cisco Support Plugin
 ----
 </br>
 
 This `README.md` documentation contains the following sections:
 
 * [Plugin Overview](#plugin-overview)
+    * [Cisco](#cisco)
+    * [Fortinet](#fortinet)
+    * [Pure Storage](#pure-storage)
 * [Compatibility](#compatibility)
 * [Installation](#installation)
 * [Enable the Plugin](#enable-the-plugin)
 * [Configure the Plugin](#configure-the-plugin)
+    * [Mandatory Settings](#mandatory-settings)
+    * [Optional Settings](#optional-settings)
 * [Rebuild and Restart NetBox-Docker](#rebuild-and-restart-netbox-docker)
 * [Run Database Migrations](#run-database-migrations)
-* [Sync the Cisco Support Data](#sync-the-device-support-data)
+* [Sync the Device Support Data](#sync-the-device-support-data)
+    * [Cisco](#cisco-1)
+    * [Fortinet](#fortinet-1)
+    * [Pure Storage](#pure-storage-1)
 * [How it works](#how-it-works)
 * [Plugin Screenshots](#plugin-screenshots)
 * [Languages and Tools](#languages-and-tools)
 
 # Plugin Overview
 ----
 </br>
 
+## Cisco
+----
+</br>
+
 This [NetBox](https://github.com/netbox-community/netbox) tracks with the data from the Cisco support APIs
 the device support status, the device type EoX status as well as the recommended software release. Each
 Cisco device and Cisco device type have a detail view with all data. There is also a list view with filter
 options for all devices or device types. All data can also be received and updated over the NetBox REST API.
 
 There is a Python script calles `sync_cisco_support_data` which can be used as below to update all fields
 which contains data from the Cisco support APIs. This script can be executed for example inside a Azure
@@ -109,25 +121,43 @@
 > **No Edit Views**
 >
 > Manual edit of fields only in the NetBox Django admin portal
 > At the moment there are no edit views to edit field of any data model of this plugin. The because the
 > idea of this plugin is not to change fields manually (only automated by Python or REST API). If you want
 > to change field manually, at the moment this can only be done in the NetBox Django admin portal.
 
+## Fortinet
+----
+</br>
+
+> **In Development**
+>
+> The device support coverage of Fortinet is in development
+
+## Pure Storage
+----
+</br>
+
+> **In Development**
+>
+> The device support coverage of Pure Storage is in development
+
 # Compatibility
 ----
 </br>
 
-> :warning: **NetBox 3.5**: This plugin is for NetBox 3.5
+> :warning: **NetBox 4.0**: The latest release of this plugin is for NetBox 4.0
 
 This plugin is compatible with [NetBox](https://netbox.readthedocs.org/) 3.5.0 and later.
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |      3.5       |      0.0.1     |
+|      4.0       |      1.0.3     |
+
 
 # Installation
 ----
 </br>
 
 The installation and configuration steps are for the [NetBox-Docker](https://github.com/netbox-community/netbox-docker)
 installation. To install this plugin make sure you followed the prerequisites for using NetBox plugins with
@@ -152,23 +182,31 @@
 
 Enable the `netbox-device-support-plugin` plugin in `/netbox-docker/configuration/plugins.py` and add the
 plugin configuration also in the same file.
 
 ```python
 # Enable installed plugins. Add the name of each plugin to the list.
 PLUGINS = [
-    "netbox_napalm_plugin",
     "netbox_device_support_plugin",
 ]
 ```
 
 # Configure the Plugin
 ----
 </br>
 
+> **Fortinet and Pure Storage in Development**
+>
+> The section plugin configuration describes only the vendor Cisco as Fortinet and Pure Storage are still
+> in development
+
+## Mandatory Settings
+----
+</br>
+
 In order to get valid API response data, several requirements must be fulfilled:
 
 1. A [Cisco API ID and secret](https://apiconsole.cisco.com/) (with access to the APIs "EoX V5 API",
 "Serial Number to Information API Version 2" and "Software Suggestion") must have been created and
 configured inside `plugins.py`
 
     The following plugin configuration options are mandatory for the Cisco support API.
@@ -186,27 +224,31 @@
         "netbox_device_support_plugin": {
             "CISCO_SUPPORT_API_CLIENT_ID": environ.get("CISCO_SUPPORT_API_CLIENT_ID", ""),
             "CISCO_SUPPORT_API_CLIENT_SECRET": environ.get("CISCO_SUPPORT_API_CLIENT_SECRET", ""),
         },
     }
     ```
 
-2. A manufacturer called `Cisco` must have been configured inside NetBox. If your manufacturer is named
+## Optional Settings
+----
+</br>
+
+1. A manufacturer called `Cisco`, must have been configured inside NetBox. If your manufacturer is named
 differently, change it inside the plugin configuration in `plugins.py`:
 
     ```python
     PLUGINS_CONFIG = {
         "netbox_device_support_plugin": {
             ...,
             "MANUFACTURER": "Cisco Systems" # Optional setting for definiing the manufacturer
         }
     }
     ```
 
-3. Optional the `TEMPLATE_EXTENSION_PLACEMENT` can be changed inside the plugin configuration in `plugins.py`:
+2. Optional the `TEMPLATE_EXTENSION_PLACEMENT` can be changed inside the plugin configuration in `plugins.py`:
 
     ```python
     PLUGINS_CONFIG = {
         "netbox_device_support_plugin": {
             ...,
             "TEMPLATE_EXTENSION_PLACEMENT": "left" # Optional setting render the content on the left or right side
         }
@@ -236,15 +278,19 @@
 
 Restore the database and run the Django database migration to your existing NetBox database.
 
 ```bash
 python3 manage.py migrate
 ```
 
-# Sync the Cisco Support Data
+# Sync the Device Support Data
+----
+</br>
+
+## Cisco
 ----
 </br>
 
 In order that `sync_cisco_support_data` works correctly, several requirements must be fulfilled:
 
 1. All devices types for manufacturer Cisco must have filled the optional `Part number` field inside NetBox
 with the correct Base PID for that Cisco product.
@@ -261,15 +307,15 @@
 ```bash
 python3 manage.py sync_cisco_support_data.py
 ```
 
 Execute a Azure DevOps Build Pipeline which runs `sync_cisco_support_data.py` to periodically refresh the
 data or create a cronjob which to the same a bit more old school.
 
-# How it works
+### How it works
 ----
 </br>
 
 1. Calling the `sync_cisco_support_data` method will catch all device types for the configured manufacturer.
 
 2. Each device types `Part number` will be send to Cisco EoX API. API answer will be saved inside a
 `CiscoDeviceTypeSupport` model. One `CiscoDeviceTypeSupport` per device type.
@@ -289,16 +335,33 @@
 7. Field Coloring: Expired timestamps or no data will be colored red, timestamps which will expire in the next
 calendar year will be colored yellow for planning or forecast reasons.
 
 8. Progress Bar: The progress bars will visualize the timestamps duration to the expiration date. The
 progress bar color will be green until the timestamp will expire in the next calendar year. Then the color
 will change to yellow. The color will finally change to red when the timestamp expire within 60 days.
 
+## Fortinet
+----
+</br>
+
+> **In Development**
+>
+> The device support coverage of Fortinet is in development
+
+## Pure Storage
+----
+</br>
+
+> **In Development**
+>
+> The device support coverage of Fortinet is in development
+
 # Plugin Screenshots
 ----
+</br>
 
 ## Device Detail View
 ![Device Detail View](images/device_detail_view.png)
 
 ## Device Type Detail View
 ![Device Type Detail View](images/device_type_detail_view.png)
```

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/__init__.py` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,21 +9,26 @@
     version = __version__
     author = "Willi Kubny"
     author_email = "willi.kubny@gmail.com"
     base_url = "device-support"
     min_version = "3.5.0"
     required_settings = []
     default_settings = {
+        # General Settings
         "TEMPLATE_EXTENSION_PLACEMENT": "right",  # "right" or "left"
+        "DEVICE_VENDORS": ["Cisco"],  # List of vendors names to be used in the plugin
+        # Cisco Settings
         "CISCO_MANUFACTURER": "Cisco",
         "CISCO_SUPPORT_API_CLIENT_ID": "",
         "CISCO_SUPPORT_API_CLIENT_SECRET": "",
+        # Fortinet Settings
         "FORTINET_MANUFACTURER": "Fortinet",
         "FORTINET_SUPPORT_API_CLIENT_ID": "",
         "FORTINET_SUPPORT_API_CLIENT_SECRET": "",
+        # PureStorage Settings
         "PURESTORAGE_MANUFACTURER": "Pure Storage",
         "PURESTORAGE_SUPPORT_API_CLIENT_ID": "",
         "PURESTORAGE_SUPPORT_API_CLIENT_SECRET": "",
     }
 
 
 config = DeviceSupportConfig
```

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/admin.py` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/admin.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/api/serializers.py` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/api/views.py` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/filtersets.py` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/forms.py` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 #### Cisco Support ##########################################################################################
 
 
 class CiscoDeviceSupportFilterForm(SavedFiltersMixin, FilterForm):
     model = CiscoDeviceSupport
 
     fieldsets = (
-        FieldSet("name", "pid", name=("General")),
+        FieldSet(
+            "name",
+            "pid",
+            name=("General"),
+        ),
         FieldSet(
             "recommended_release",
             "desired_release_status",
             "desired_release",
             "current_release_status",
             "current_release",
             name=("Software Release"),
@@ -225,15 +229,19 @@
     )
 
 
 class CiscoDeviceTypeSupportFilterForm(SavedFiltersMixin, FilterForm):
     model = CiscoDeviceTypeSupport
 
     fieldsets = (
-        FieldSet("name", "pid", name=("General")),
+        FieldSet(
+            "name",
+            "pid",
+            name=("General"),
+        ),
         FieldSet(
             "eox_has_error",
             "eox_error",
             "eox_announcement_date",
             "end_of_sale_date",
             "end_of_sw_maintenance_releases",
             "end_of_security_vul_support_date",
@@ -322,24 +330,33 @@
 #### Fortinet Support #######################################################################################
 
 
 class FortinetDeviceSupportFilterForm(SavedFiltersMixin, FilterForm):
     model = FortinetDeviceSupport
 
     fieldsets = (
-        FieldSet("name", "pid", name=("General")),
+        FieldSet(
+            "name",
+            "pid",
+            name=("General"),
+        ),
         FieldSet(
             "recommended_release",
             "desired_release_status",
             "desired_release",
             "current_release_status",
             "current_release",
             name=("Software Release"),
         ),
-        FieldSet("partner", "end_of_renewal_date", "end_of_support_date", name=("Device Support")),
+        FieldSet(
+            "partner",
+            "end_of_renewal_date",
+            "end_of_support_date",
+            name=("Device Support"),
+        ),
     )
 
     name = forms.CharField(
         required=False,
         label="Device Name",
         help_text="Case-insensitive exact match",
     )
@@ -404,16 +421,24 @@
 #### PureStorage Support ####################################################################################
 
 
 class PureStorageDeviceSupportFilterForm(SavedFiltersMixin, FilterForm):
     model = PureStorageDeviceSupport
 
     fieldsets = (
-        FieldSet("name", "pid", name=("General")),
-        FieldSet("desired_release", "current_release", name=("Software Release")),
+        FieldSet(
+            "name",
+            "pid",
+            name=("General"),
+        ),
+        FieldSet(
+            "desired_release",
+            "current_release",
+            name=("Software Release"),
+        ),
     )
 
     name = forms.CharField(
         required=False,
         label="Device Name",
         help_text="Case-insensitive exact match",
     )
```

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/management/commands/sync_cisco_support_data.py` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/management/commands/sync_cisco_support_data.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/management/commands/sync_fortinet_support_data.py` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/management/commands/sync_fortinet_support_data.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/management/commands/sync_purestorage_support_data.py` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/management/commands/sync_purestorage_support_data.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/migrations/0001_initial.py` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/models.py` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,17 +371,15 @@
         # Set the last_date_of_support from the CiscoDeviceTypeSupport last_date_of_support
         self.last_date_of_support = cisco_device_type_support_obj.last_date_of_support
 
         # Set the api_status
         if self.sr_no_owner:
             self.api_status = "API user associated with contract and device"
         else:
-            self.api_status = (
-                "API user not associated with contract and device (Not authorized to most API information)"
-            )
+            self.api_status = "API user not associated with contract and device"
 
         # Set the contract_supplier
         if (
             self.contract_supplier is None
             or self.contract_supplier == "None"
             or self.contract_supplier == "Cisco SNTC"
             or self.contract_supplier == "Not covered"
```

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/tables.py` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/cisco_device_support.html` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/cisco_device_support.html`

 * *Files 12% similar despite different names*

```diff
@@ -21,18 +21,17 @@
                         <td>Current Release</td>
                         <td style="width: 40px"><i {{ cisco_device_support.current_release_status|coverage_class_boolian }}></i></td>
                         <td>{{ cisco_device_support.current_release|placeholder }}</td>
                     </tr>
                 {% endif %}
             </tbody>
         </table>
-        <div class="text-muted">Last updated: {{ cisco_device_support.last_updated }}</div>
     </div>
     <div class="card">
-        <h5 class="card-header" style="padding:0px 0px 16px 0px">Cisco Device Support</h5>
+        <h5 class="card-header">Cisco Device Support</h5>
         <table class="table table-hover panel-body attr-table">
             <tbody>
                 <tr {{ cisco_device_support.sr_no_owner|coverage_class }}>
                     <td style="width: 40%">Is associated with a Cisco ID</td>
                     <td style="width: 40px"><i {{ cisco_device_support.sr_no_owner|coverage_class_boolian }}></i></td>
                     <td>{{ cisco_device_support.api_status|placeholder }}</td>
                 </tr>
@@ -69,15 +68,15 @@
                     <td colspan="2">{{ cisco_device_support.warranty_type|placeholder }}</td>
                 </tr>
             </tbody>
         </table>
         {% if not cisco_device_support.contract_supplier or "Cisco SNTC" in cisco_device_support.contract_supplier or "Not covered" in cisco_device_support.contract_supplier %}
             {# Comment: Omit the partner support contract table #}
         {% else %}
-            <h5 class="card-header" style="padding:16px 0px 16px 0px">{{ cisco_device_support.contract_supplier }} Device Support</h5>
+            <h5 class="card-header">{{ cisco_device_support.contract_supplier }} Device Support</h5>
             <table class="table table-hover panel-body attr-table">
                 <tbody>
                     <tr {{ cisco_device_support.partner_status|coverage_class }}>
                         <td style="width: 40%">Contract Status</td>
                         <td>{{ cisco_device_support.partner_status|placeholder }}</td>
                     </tr>
                     <tr {{ cisco_device_support.partner_coverage_end_date|expiration_class }}>
@@ -94,12 +93,11 @@
                     <tr {{ cisco_device_support.partner_customer_number|coverage_class }}>
                         <td>Customer Number</td>
                         <td>{{ cisco_device_support.partner_customer_number|placeholder }}</td>
                     </tr>
                 </tbody>
             </table>
         {% endif %}
-        <div class="text-muted">Last updated: {{ cisco_device_support.last_updated }}</div>
     </div>
 {% endif %}
 
 {% include "cisco/cisco_device_type_support.html" %}
```

#### html2text {}

```diff
@@ -1,12 +1,10 @@
 {% load filters %} {% if cisco_device_support %}
 **** CCiissccoo SSooffttwwaarree RReelleeaassee ****
-Last updated: {{ cisco_device_support.last_updated }}
 **** CCiissccoo DDeevviiccee SSuuppppoorrtt ****
 {% if not cisco_device_support.contract_supplier or "Cisco SNTC" in
 cisco_device_support.contract_supplier or "Not covered" in
 cisco_device_support.contract_supplier %} {# Comment: Omit the partner support
 contract table #} {% else %}
 **** {{{{ cciissccoo__ddeevviiccee__ssuuppppoorrtt..ccoonnttrraacctt__ssuupppplliieerr }}}} DDeevviiccee SSuuppppoorrtt ****
 {% endif %}
-Last updated: {{ cisco_device_support.last_updated }}
 {% endif %} {% include "cisco/cisco_device_type_support.html" %}
```

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/cisco_device_type_support.html` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/cisco_device_type_support.html`

 * *Files 3% similar despite different names*

```diff
@@ -64,10 +64,9 @@
                         <td style="width: 40%">EoX Status</td>
                         <td style="width: 40px"><i {{ cisco_device_type_support.eox_has_error|eox_class_boolian }}></i></td>
                         <td>{{ cisco_device_type_support.eox_error }}</td>
                     </tr>
                 {% endif %}
             </tbody>
         </table>
-        <div class="text-muted">Last updated: {{ cisco_device_type_support.last_updated }}</div>
     </div>
 {% endif %}
```

#### html2text {}

```diff
@@ -1,4 +1,3 @@
 {% load filters %} {% if cisco_device_type_support %}
 **** CCiissccoo DDeevviiccee TTyyppee SSuuppppoorrtt ****
-Last updated: {{ cisco_device_type_support.last_updated }}
 {% endif %}
```

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_contract_coverage_bar.html` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_contract_coverage_bar.html`

 * *Files 9% similar despite different names*

```diff
@@ -9,11 +9,11 @@
             style="width: {{ cisco_device_support.coverage_progress }}%;"
         >
         {% if cisco_device_support.coverage_progress >= 45 %}
             {{ cisco_device_support.coverage_end_date|timeuntil }} remaining
         {% endif %}
         </div>
         {% if cisco_device_support.coverage_progress < 45 %}
-            <span class="ps-1">{{ cisco_device_support.coverage_end_date|timeuntil }} remaining</span>
+            <span style="margin:auto;">{{ cisco_device_support.coverage_end_date|timeuntil }} remaining</span>
         {% endif %}
     </div>
 {% endif %}
```

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_partner_contract_coverage_bar.html` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_partner_contract_coverage_bar.html`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,11 @@
             style="width: {{ cisco_device_support.partner_coverage_progress }}%;"
         >
         {% if cisco_device_support.partner_coverage_progress >= 45 %}
             {{ cisco_device_support.partner_coverage_end_date|timeuntil }} remaining
         {% endif %}
         </div>
         {% if cisco_device_support.partner_coverage_progress < 45 %}
-            <span class="ps-1">{{ cisco_device_support.partner_coverage_end_date|timeuntil }} remaining</span>
+            <span style="margin:auto;">{{ cisco_device_support.partner_coverage_end_date|timeuntil }} remaining</span>
         {% endif %}
     </div>
 {% endif %}
```

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eorfa_bar.html` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eorfa_bar.html`

 * *Files 3% similar despite different names*

```diff
@@ -9,11 +9,11 @@
             style="width: {{ cisco_device_type_support.end_of_routine_failure_analysis_date_progress }}%;"
         >
         {% if cisco_device_type_support.end_of_routine_failure_analysis_date_progress >= 45 %}
             {{ cisco_device_type_support.end_of_routine_failure_analysis_date|timeuntil }} remaining
         {% endif %}
         </div>
         {% if cisco_device_type_support.end_of_routine_failure_analysis_date_progress < 45 %}
-            <span class="ps-1">{{ cisco_device_type_support.end_of_routine_failure_analysis_date|timeuntil }} remaining</span>
+            <span style="margin:auto;">{{ cisco_device_type_support.end_of_routine_failure_analysis_date|timeuntil }} remaining</span>
         {% endif %}
     </div>
 {% endif %}
```

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eos_bar.html` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eos_bar.html`

 * *Files 7% similar despite different names*

```diff
@@ -9,11 +9,11 @@
             style="width: {{ cisco_device_type_support.end_of_sale_progress }}%;"
         >
         {% if cisco_device_type_support.end_of_sale_progress >= 45 %}
             {{ cisco_device_type_support.end_of_sale_date|timeuntil }} remaining
         {% endif %}
         </div>
         {% if cisco_device_type_support.end_of_sale_progress < 45 %}
-            <span class="ps-1">{{ cisco_device_type_support.end_of_sale_date|timeuntil }} remaining</span>
+            <span style="margin:auto;">{{ cisco_device_type_support.end_of_sale_date|timeuntil }} remaining</span>
         {% endif %}
     </div>
 {% endif %}
```

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eoscr_bar.html` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eoscr_bar.html`

 * *Files 3% similar despite different names*

```diff
@@ -9,11 +9,11 @@
             style="width: {{ cisco_device_type_support.end_of_service_contract_renewal_progress }}%;"
         >
         {% if cisco_device_type_support.end_of_service_contract_renewal_progress >= 45 %}
             {{ cisco_device_type_support.end_of_service_contract_renewal|timeuntil }} remaining
         {% endif %}
         </div>
         {% if cisco_device_type_support.end_of_service_contract_renewal_progress < 45 %}
-            <span class="ps-1">{{ cisco_device_type_support.end_of_service_contract_renewal|timeuntil }} remaining</span>
+            <span style="margin:auto;">{{ cisco_device_type_support.end_of_service_contract_renewal|timeuntil }} remaining</span>
         {% endif %}
     </div>
 {% endif %}
```

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eosm_bar.html` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eosm_bar.html`

 * *Files 9% similar despite different names*

```diff
@@ -9,11 +9,11 @@
             style="width: {{ cisco_device_type_support.end_of_sw_maintenance_releases_progress }}%;"
         >
         {% if cisco_device_type_support.end_of_sw_maintenance_releases_progress >= 45 %}
             {{ cisco_device_type_support.end_of_sw_maintenance_releases|timeuntil }} remaining
         {% endif %}
         </div>
         {% if cisco_device_type_support.end_of_sw_maintenance_releases_progress < 45 %}
-            <span class="ps-1">{{ cisco_device_type_support.end_of_sw_maintenance_releases|timeuntil }} remaining</span>
+            <span style="margin:auto;">{{ cisco_device_type_support.end_of_sw_maintenance_releases|timeuntil }} remaining</span>
         {% endif %}
     </div>
 {% endif %}
```

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvca_bar.html` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvca_bar.html`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,11 @@
             style="width: {{ cisco_device_type_support.end_of_svc_attach_date_progress }}%;"
         >
         {% if cisco_device_type_support.end_of_svc_attach_date_progress >= 45 %}
             {{ cisco_device_type_support.end_of_svc_attach_date|timeuntil }} remaining
         {% endif %}
         </div>
         {% if cisco_device_type_support.end_of_svc_attach_date_progress < 45 %}
-            <span class="ps-1">{{ cisco_device_type_support.end_of_svc_attach_date|timeuntil }} remaining</span>
+            <span style="margin:auto;">{{ cisco_device_type_support.end_of_svc_attach_date|timeuntil }} remaining</span>
         {% endif %}
     </div>
 {% endif %}
```

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvs_bar.html` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_last_day_support_bar.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-{% if cisco_device_type_support.end_of_security_vul_support_date_progress %}
+{% if cisco_device_type_support.last_date_of_support_progress %}
     <div style="height: 4px;"></div>
     <div class="progress">
         <div role="progressbar"
             aria-valuemin="0"
             aria-valuemax="100"
-            aria-valuenow="{{ cisco_device_type_support.end_of_security_vul_support_date_progress }}"
-            class="progress-bar {{ cisco_device_type_support.end_of_security_vul_support_date_progress_bar_class }}"
-            style="width: {{ cisco_device_type_support.end_of_security_vul_support_date_progress }}%;"
+            aria-valuenow="{{ cisco_device_type_support.last_date_of_support_progress }}"
+            class="progress-bar {{ cisco_device_type_support.last_date_of_support_progress_bar_class }}"
+            style="width: {{ cisco_device_type_support.last_date_of_support_progress }}%;"
         >
-        {% if cisco_device_type_support.end_of_security_vul_support_date_progress >= 45 %}
-            {{ cisco_device_type_support.end_of_security_vul_support_date|timeuntil }} remaining
+        {% if cisco_device_type_support.last_date_of_support_progress >= 45 %}
+            {{ cisco_device_type_support.last_date_of_support|timeuntil }} remaining
         {% endif %}
         </div>
-        {% if cisco_device_type_support.end_of_security_vul_support_date_progress < 45 %}
-            <span class="ps-1">{{ cisco_device_type_support.end_of_security_vul_support_date|timeuntil }} remaining</span>
-        {% endif %}
+    {% if cisco_device_type_support.last_date_of_support_progress < 45 %}
+        <span style="margin:auto;">{{ cisco_device_type_support.last_date_of_support|timeuntil }} remaining</span>
+    {% endif %}
     </div>
 {% endif %}
```

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/fortinet/fortinet_device_support.html` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/fortinet/fortinet_device_support.html`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
                 <tr {{ fortinet_device_support.current_release_status|current_release_status_class }}>
                     <td>Current Release</td>
                     <td style="width: 40px"><i {{ fortinet_device_support.current_release_status|coverage_class_boolian }}></i></td>
                     <td>{{ fortinet_device_support.current_release|placeholder }}</td>
                 </tr>
             </tbody>
         </table>
-        <div class="text-muted">Last updated: {{ fortinet_device_support.last_updated }}</div>
     </div>
     <div class="card">
         <h5 class="card-header">Fortinet License Coverage</h5>
         <table class="table table-hover panel-body attr-table">
             <tbody>
                 <tr>
                     <td colspan="2" class="text-center text-muted">— Not implemented yet —</td>
@@ -38,15 +37,14 @@
                     <td class="text-muted">
                         'Expiration Date'<br>
                         'Expiration Bar'
                     </td>
                 </tr>
             </tbody>
         </table>
-        <div class="text-muted">Last updated: {{ fortinet_device_support.last_updated }}</div>
     </div>
     <div class="card">
         <h5 class="card-header">Fortinet Device Support</h5>
         <table class="table table-hover panel-body attr-table">
             <tbody>
                 <tr {{ fortinet_device_support.partner|coverage_class }}>
                     <td style="width: 40%">Partner</td>
@@ -64,15 +62,15 @@
                     <td>
                         {{ fortinet_device_support.end_of_support_date|placeholder }}<br>
                         {% include "fortinet/inc/device_eos_bar.html" %}
                     </td>
                 </tr>
             </tbody>
         </table>
-        <h6 class="card-header" style="padding:16px 0px 16px 0px">Entitlements</h6>
+        <h6 class="card-header">Entitlements</h6>
         <table class="table table-hover panel-body attr-table">
             <tbody>
                 <tr>
                     <td colspan="2" class="text-center text-muted">— Not implemented yet —</td>
                 </tr>
                 <tr>
                     <td style="width: 40%" class="text-muted">
@@ -82,10 +80,9 @@
                     <td class="text-muted">
                         'Expiration Date'<br>
                         'Expiration Bar'
                     </td>
                 </tr>
             </tbody>
         </table>
-        <div class="text-muted">Last updated: {{ fortinet_device_support.last_updated }}</div>
     </div>
 {% endif %}
```

#### html2text {}

```diff
@@ -1,15 +1,12 @@
 {% load filters %} {% if fortinet_device_support %}
 **** FFoorrttiinneett SSooffttwwaarree RReelleeaassee ****
-Last updated: {{ fortinet_device_support.last_updated }}
 **** FFoorrttiinneett LLiicceennssee CCoovveerraaggee ****
 â Not implemented yet â
 'License Description' 'Expiration Date'
 '(License Type)'      'Expiration Bar'
-Last updated: {{ fortinet_device_support.last_updated }}
 **** FFoorrttiinneett DDeevviiccee SSuuppppoorrtt ****
 ** EEnnttiittlleemmeennttss **
 â Not implemented yet â
 'Support Description' 'Expiration Date'
 '(Support Level)'     'Expiration Bar'
-Last updated: {{ fortinet_device_support.last_updated }}
 {% endif %}
```

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/fortinet/inc/device_eor_bar.html` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/fortinet/inc/device_eor_bar.html`

 * *Files 16% similar despite different names*

```diff
@@ -8,12 +8,12 @@
             class="progress-bar {{ fortinet_device_support.end_of_renewal_progress_bar_class }}"
             style="width: {{ fortinet_device_support.end_of_renewal_progress }}%;"
         >
         {% if fortinet_device_support.end_of_renewal_progress >= 45 %}
             {{ fortinet_device_support.end_of_renewal_date|timeuntil }} remaining
         {% endif %}
         </div>
-        {% if fortinet_device_support.end_of_renewal_progress < 45 %}
-            <span class="ps-1">{{ fortinet_device_support.end_of_renewal_date|timeuntil }} remaining</span>
-        {% endif %}
+    {% if fortinet_device_support.end_of_renewal_progress < 45 %}
+        <span style="margin:auto;">{{ fortinet_device_support.end_of_renewal_date|timeuntil }} remaining</span>
+    {% endif %}
     </div>
 {% endif %}
```

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/fortinet/inc/device_eos_bar.html` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/fortinet/inc/device_eos_bar.html`

 * *Files 2% similar despite different names*

```diff
@@ -8,12 +8,12 @@
             class="progress-bar {{ fortinet_device_support.end_of_support_progress_bar_class }}"
             style="width: {{ fortinet_device_support.end_of_support_progress }}%;"
         >
         {% if fortinet_device_support.end_of_support_progress >= 45 %}
             {{ fortinet_device_support.end_of_support_date|timeuntil }} remaining
         {% endif %}
         </div>
-        {% if fortinet_device_support.end_of_support_progress < 45 %}
-            <span class="ps-1">{{ fortinet_device_support.end_of_support_date|timeuntil }} remaining</span>
-        {% endif %}
+    {% if fortinet_device_support.end_of_support_progress < 45 %}
+        <span style="margin:auto;">{{ fortinet_device_support.end_of_support_date|timeuntil }} remaining</span>
+    {% endif %}
     </div>
 {% endif %}
```

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/purestorage/purestorage_device_support.html` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/purestorage/purestorage_device_support.html`

 * *Files 18% similar despite different names*

```diff
@@ -11,32 +11,29 @@
                 </tr>
                 <tr {{ purestorage_device_support.current_release|coverage_class }} >
                     <td>Current Release</td>
                     <td colspan="2">{{ purestorage_device_support.current_release|placeholder }}</td>
                 </tr>
             </tbody>
         </table>
-        <div class="text-muted">Last updated: {{ purestorage_device_support.last_updated }}</div>
     </div>
     <div class="card">
         <h5 class="card-header">Pure Storage License Coverage</h5>
         <table class="table table-hover panel-body attr-table">
             <tbody>
                 <tr>
                     <td class="text-center text-muted">— Not implemented yet —</td>
                 </tr>
             </tbody>
         </table>
-        <div class="text-muted">Last updated: {{ purestorage_device_support.last_updated }}</div>
     </div>
     <div class="card">
         <h5 class="card-header">Pure Storage Device Support</h5>
         <table class="table table-hover panel-body attr-table">
             <tbody>
                 <tr>
                     <td class="text-center text-muted">— Not implemented yet —</td>
                 </tr>
             </tbody>
         </table>
-        <div class="text-muted">Last updated: {{ purestorage_device_support.last_updated }}</div>
     </div>
 {% endif %}
```

#### html2text {}

```diff
@@ -1,10 +1,7 @@
 {% load filters %} {% if purestorage_device_support %}
 **** PPuurree SSttoorraaggee SSooffttwwaarree RReelleeaassee ****
-Last updated: {{ purestorage_device_support.last_updated }}
 **** PPuurree SSttoorraaggee LLiicceennssee CCoovveerraaggee ****
 â Not implemented yet â
-Last updated: {{ purestorage_device_support.last_updated }}
 **** PPuurree SSttoorraaggee DDeevviiccee SSuuppppoorrtt ****
 â Not implemented yet â
-Last updated: {{ purestorage_device_support.last_updated }}
 {% endif %}
```

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templatetags/filters.py` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templatetags/filters.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/urls.py` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/views.py` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from collections import defaultdict
-from django.utils.translation import gettext_lazy
 from netbox.views import generic
 from . import filtersets, models, tables, forms
 
 
 #### Cisco Device Support ###################################################################################
 
 
@@ -18,15 +16,15 @@
 class CiscoDeviceSupportDeleteView(generic.ObjectDeleteView):
     queryset = models.CiscoDeviceSupport.objects.all()
 
 
 class CiscoDeviceSupportBulkDeleteView(generic.BulkDeleteView):
     queryset = models.CiscoDeviceSupport.objects.all()
     filterset = filtersets.CiscoDeviceSupportFilterSet
-    table = tables.CiscoDeviceSupport
+    table = tables.CiscoDeviceSupportTable
 
 
 #### Cisco Device Type Support ##############################################################################
 
 
 class CiscoDeviceTypeSupportListView(generic.ObjectListView):
     queryset = models.CiscoDeviceTypeSupport.objects.all()
@@ -39,15 +37,15 @@
 class CiscoDeviceTypeSupportDeleteView(generic.ObjectDeleteView):
     queryset = models.CiscoDeviceTypeSupport.objects.all()
 
 
 class CiscoDeviceTypeSupportBulkDeleteView(generic.BulkDeleteView):
     queryset = models.CiscoDeviceTypeSupport.objects.all()
     filterset = filtersets.CiscoDeviceTypeSupportFilterSet
-    table = tables.CiscoDeviceTypeSupport
+    table = tables.CiscoDeviceTypeSupportTable
 
 
 #### Fortinet Support #######################################################################################
 
 
 class FortinetDeviceSupportListView(generic.ObjectListView):
     queryset = models.FortinetDeviceSupport.objects.all()
@@ -60,15 +58,15 @@
 class FortinetDeviceSupportDeleteView(generic.ObjectDeleteView):
     queryset = models.FortinetDeviceSupport.objects.all()
 
 
 class FortinetDeviceSupportBulkDeleteView(generic.BulkDeleteView):
     queryset = models.FortinetDeviceSupport.objects.all()
     filterset = filtersets.FortinetDeviceSupportFilterSet
-    table = tables.FortinetDeviceSupport
+    table = tables.FortinetDeviceSupportTable
 
 
 #### PureStorage Support ####################################################################################
 
 
 class PureStorageDeviceSupportListView(generic.ObjectListView):
     queryset = models.PureStorageDeviceSupport.objects.all()
@@ -81,8 +79,8 @@
 class PureStorageDeviceSupportDeleteView(generic.ObjectDeleteView):
     queryset = models.PureStorageDeviceSupport.objects.all()
 
 
 class PureStorageDeviceSupportBulkDeleteView(generic.BulkDeleteView):
     queryset = models.PureStorageDeviceSupport.objects.all()
     filterset = filtersets.PureStorageDeviceSupportFilterSet
-    table = tables.PureStorageDeviceSupport
+    table = tables.PureStorageDeviceSupportTable
```

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin.egg-info/PKG-INFO` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-device-support-plugin
-Version: 1.0.2
+Version: 1.0.3
 Summary: Cisco device support, device type support, and software release information with the Cisco support APIs
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
@@ -23,29 +23,41 @@
 # NetBox Cisco Support Plugin
 ----
 </br>
 
 This `README.md` documentation contains the following sections:
 
 * [Plugin Overview](#plugin-overview)
+    * [Cisco](#cisco)
+    * [Fortinet](#fortinet)
+    * [Pure Storage](#pure-storage)
 * [Compatibility](#compatibility)
 * [Installation](#installation)
 * [Enable the Plugin](#enable-the-plugin)
 * [Configure the Plugin](#configure-the-plugin)
+    * [Mandatory Settings](#mandatory-settings)
+    * [Optional Settings](#optional-settings)
 * [Rebuild and Restart NetBox-Docker](#rebuild-and-restart-netbox-docker)
 * [Run Database Migrations](#run-database-migrations)
-* [Sync the Cisco Support Data](#sync-the-device-support-data)
+* [Sync the Device Support Data](#sync-the-device-support-data)
+    * [Cisco](#cisco-1)
+    * [Fortinet](#fortinet-1)
+    * [Pure Storage](#pure-storage-1)
 * [How it works](#how-it-works)
 * [Plugin Screenshots](#plugin-screenshots)
 * [Languages and Tools](#languages-and-tools)
 
 # Plugin Overview
 ----
 </br>
 
+## Cisco
+----
+</br>
+
 This [NetBox](https://github.com/netbox-community/netbox) tracks with the data from the Cisco support APIs
 the device support status, the device type EoX status as well as the recommended software release. Each
 Cisco device and Cisco device type have a detail view with all data. There is also a list view with filter
 options for all devices or device types. All data can also be received and updated over the NetBox REST API.
 
 There is a Python script calles `sync_cisco_support_data` which can be used as below to update all fields
 which contains data from the Cisco support APIs. This script can be executed for example inside a Azure
@@ -126,25 +138,43 @@
 > **No Edit Views**
 >
 > Manual edit of fields only in the NetBox Django admin portal
 > At the moment there are no edit views to edit field of any data model of this plugin. The because the
 > idea of this plugin is not to change fields manually (only automated by Python or REST API). If you want
 > to change field manually, at the moment this can only be done in the NetBox Django admin portal.
 
+## Fortinet
+----
+</br>
+
+> **In Development**
+>
+> The device support coverage of Fortinet is in development
+
+## Pure Storage
+----
+</br>
+
+> **In Development**
+>
+> The device support coverage of Pure Storage is in development
+
 # Compatibility
 ----
 </br>
 
-> :warning: **NetBox 3.5**: This plugin is for NetBox 3.5
+> :warning: **NetBox 4.0**: The latest release of this plugin is for NetBox 4.0
 
 This plugin is compatible with [NetBox](https://netbox.readthedocs.org/) 3.5.0 and later.
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |      3.5       |      0.0.1     |
+|      4.0       |      1.0.3     |
+
 
 # Installation
 ----
 </br>
 
 The installation and configuration steps are for the [NetBox-Docker](https://github.com/netbox-community/netbox-docker)
 installation. To install this plugin make sure you followed the prerequisites for using NetBox plugins with
@@ -169,23 +199,31 @@
 
 Enable the `netbox-device-support-plugin` plugin in `/netbox-docker/configuration/plugins.py` and add the
 plugin configuration also in the same file.
 
 ```python
 # Enable installed plugins. Add the name of each plugin to the list.
 PLUGINS = [
-    "netbox_napalm_plugin",
     "netbox_device_support_plugin",
 ]
 ```
 
 # Configure the Plugin
 ----
 </br>
 
+> **Fortinet and Pure Storage in Development**
+>
+> The section plugin configuration describes only the vendor Cisco as Fortinet and Pure Storage are still
+> in development
+
+## Mandatory Settings
+----
+</br>
+
 In order to get valid API response data, several requirements must be fulfilled:
 
 1. A [Cisco API ID and secret](https://apiconsole.cisco.com/) (with access to the APIs "EoX V5 API",
 "Serial Number to Information API Version 2" and "Software Suggestion") must have been created and
 configured inside `plugins.py`
 
     The following plugin configuration options are mandatory for the Cisco support API.
@@ -203,27 +241,31 @@
         "netbox_device_support_plugin": {
             "CISCO_SUPPORT_API_CLIENT_ID": environ.get("CISCO_SUPPORT_API_CLIENT_ID", ""),
             "CISCO_SUPPORT_API_CLIENT_SECRET": environ.get("CISCO_SUPPORT_API_CLIENT_SECRET", ""),
         },
     }
     ```
 
-2. A manufacturer called `Cisco` must have been configured inside NetBox. If your manufacturer is named
+## Optional Settings
+----
+</br>
+
+1. A manufacturer called `Cisco`, must have been configured inside NetBox. If your manufacturer is named
 differently, change it inside the plugin configuration in `plugins.py`:
 
     ```python
     PLUGINS_CONFIG = {
         "netbox_device_support_plugin": {
             ...,
             "MANUFACTURER": "Cisco Systems" # Optional setting for definiing the manufacturer
         }
     }
     ```
 
-3. Optional the `TEMPLATE_EXTENSION_PLACEMENT` can be changed inside the plugin configuration in `plugins.py`:
+2. Optional the `TEMPLATE_EXTENSION_PLACEMENT` can be changed inside the plugin configuration in `plugins.py`:
 
     ```python
     PLUGINS_CONFIG = {
         "netbox_device_support_plugin": {
             ...,
             "TEMPLATE_EXTENSION_PLACEMENT": "left" # Optional setting render the content on the left or right side
         }
@@ -253,15 +295,19 @@
 
 Restore the database and run the Django database migration to your existing NetBox database.
 
 ```bash
 python3 manage.py migrate
 ```
 
-# Sync the Cisco Support Data
+# Sync the Device Support Data
+----
+</br>
+
+## Cisco
 ----
 </br>
 
 In order that `sync_cisco_support_data` works correctly, several requirements must be fulfilled:
 
 1. All devices types for manufacturer Cisco must have filled the optional `Part number` field inside NetBox
 with the correct Base PID for that Cisco product.
@@ -278,15 +324,15 @@
 ```bash
 python3 manage.py sync_cisco_support_data.py
 ```
 
 Execute a Azure DevOps Build Pipeline which runs `sync_cisco_support_data.py` to periodically refresh the
 data or create a cronjob which to the same a bit more old school.
 
-# How it works
+### How it works
 ----
 </br>
 
 1. Calling the `sync_cisco_support_data` method will catch all device types for the configured manufacturer.
 
 2. Each device types `Part number` will be send to Cisco EoX API. API answer will be saved inside a
 `CiscoDeviceTypeSupport` model. One `CiscoDeviceTypeSupport` per device type.
@@ -306,16 +352,33 @@
 7. Field Coloring: Expired timestamps or no data will be colored red, timestamps which will expire in the next
 calendar year will be colored yellow for planning or forecast reasons.
 
 8. Progress Bar: The progress bars will visualize the timestamps duration to the expiration date. The
 progress bar color will be green until the timestamp will expire in the next calendar year. Then the color
 will change to yellow. The color will finally change to red when the timestamp expire within 60 days.
 
+## Fortinet
+----
+</br>
+
+> **In Development**
+>
+> The device support coverage of Fortinet is in development
+
+## Pure Storage
+----
+</br>
+
+> **In Development**
+>
+> The device support coverage of Fortinet is in development
+
 # Plugin Screenshots
 ----
+</br>
 
 ## Device Detail View
 ![Device Detail View](images/device_detail_view.png)
 
 ## Device Type Detail View
 ![Device Type Detail View](images/device_type_detail_view.png)
```

### Comparing `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin.egg-info/SOURCES.txt` & `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.2/setup.py` & `netbox_device_support_plugin-1.0.3/setup.py`

 * *Files identical despite different names*

