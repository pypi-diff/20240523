# Comparing `tmp/netbox_device_support_plugin-1.0.3.tar.gz` & `tmp/netbox_device_support_plugin-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_device_support_plugin-1.0.3.tar", last modified: Wed May 22 12:09:36 2024, max compression
+gzip compressed data, was "netbox_device_support_plugin-1.0.4.tar", last modified: Thu May 23 14:25:13 2024, max compression
```

## Comparing `netbox_device_support_plugin-1.0.3.tar` & `netbox_device_support_plugin-1.0.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.822099 netbox_device_support_plugin-1.0.3/
--rw-r--r--   0 vsts      (1001) docker     (127)     1068 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)       58 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    14554 2024-05-22 12:09:36.822099 netbox_device_support_plugin-1.0.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)    13907 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.810099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/
--rw-r--r--   0 vsts      (1001) docker     (127)     1271 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2917 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/admin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.814099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/api/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4667 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/api/serializers.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1272 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/api/urls.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1657 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/api/views.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6089 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/filtersets.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13692 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/forms.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.814099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/management/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/management/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.814099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/management/commands/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/management/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    40821 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/management/commands/sync_cisco_support_data.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8273 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/management/commands/sync_fortinet_support_data.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8319 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/management/commands/sync_purestorage_support_data.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.814099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/migrations/
--rw-r--r--   0 vsts      (1001) docker     (127)     7956 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/migrations/0001_initial.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/migrations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    32739 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/models.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2362 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/navigation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5749 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/tables.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4639 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/template_content.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.810099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.818099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/
--rw-r--r--   0 vsts      (1001) docker     (127)     6033 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/cisco_device_support.html
--rw-r--r--   0 vsts      (1001) docker     (127)     4140 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/cisco_device_type_support.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.818099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/
--rw-r--r--   0 vsts      (1001) docker     (127)      840 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_contract_coverage_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      904 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_partner_contract_coverage_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)     1086 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eorfa_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      896 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eos_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)     1046 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eoscr_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)     1038 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eosm_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      974 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvca_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)     1054 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvs_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_last_day_support_bar.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.818099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/fortinet/
--rw-r--r--   0 vsts      (1001) docker     (127)     3989 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/fortinet/fortinet_device_support.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.818099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/fortinet/inc/
--rw-r--r--   0 vsts      (1001) docker     (127)      892 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/fortinet/inc/device_eor_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      892 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/fortinet/inc/device_eos_bar.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.818099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/purestorage/
--rw-r--r--   0 vsts      (1001) docker     (127)     1551 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/purestorage/purestorage_device_support.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.818099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templatetags/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templatetags/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2960 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templatetags/filters.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2107 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/urls.py
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3336 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/views.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 12:09:36.818099 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    14554 2024-05-22 12:09:36.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2649 2024-05-22 12:09:36.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-22 12:09:36.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-22 12:09:36.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)       29 2024-05-22 12:09:36.000000 netbox_device_support_plugin-1.0.3/netbox_device_support_plugin.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-22 12:09:36.822099 netbox_device_support_plugin-1.0.3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1570 2024-05-22 12:09:16.000000 netbox_device_support_plugin-1.0.3/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 14:25:13.194813 netbox_device_support_plugin-1.0.4/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1068 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)       58 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    14554 2024-05-23 14:25:13.194813 netbox_device_support_plugin-1.0.4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    13907 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 14:25:13.186813 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1271 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2917 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/admin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 14:25:13.190813 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/api/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4667 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/api/serializers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1272 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/api/urls.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1657 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/api/views.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6089 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/filtersets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13692 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/forms.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 14:25:13.190813 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/management/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/management/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 14:25:13.190813 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/management/commands/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/management/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43791 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/management/commands/sync_cisco_support_data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8273 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/management/commands/sync_fortinet_support_data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8319 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/management/commands/sync_purestorage_support_data.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 14:25:13.194813 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/migrations/
+-rw-r--r--   0 vsts      (1001) docker     (127)     7956 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/migrations/0001_initial.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/migrations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    32739 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/models.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2362 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/navigation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5757 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/tables.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4335 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/template_content.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 14:25:13.182813 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 14:25:13.194813 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6033 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/cisco_device_support.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     4140 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/cisco_device_type_support.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 14:25:13.194813 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/inc/
+-rw-r--r--   0 vsts      (1001) docker     (127)      840 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/inc/device_contract_coverage_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      904 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/inc/device_partner_contract_coverage_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     1086 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/inc/device_type_eorfa_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      896 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/inc/device_type_eos_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     1046 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/inc/device_type_eoscr_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     1038 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/inc/device_type_eosm_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      974 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvca_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     1054 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvs_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/inc/device_type_last_day_support_bar.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 14:25:13.194813 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/fortinet/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3989 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/fortinet/fortinet_device_support.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 14:25:13.194813 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/fortinet/inc/
+-rw-r--r--   0 vsts      (1001) docker     (127)      892 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/fortinet/inc/device_eor_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      892 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/fortinet/inc/device_eos_bar.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 14:25:13.194813 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/purestorage/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1551 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/purestorage/purestorage_device_support.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 14:25:13.194813 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templatetags/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templatetags/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2960 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templatetags/filters.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2108 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/urls.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3336 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/views.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 14:25:13.194813 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    14554 2024-05-23 14:25:13.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2649 2024-05-23 14:25:13.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-23 14:25:13.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-23 14:25:12.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)       29 2024-05-23 14:25:13.000000 netbox_device_support_plugin-1.0.4/netbox_device_support_plugin.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-23 14:25:13.194813 netbox_device_support_plugin-1.0.4/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1570 2024-05-23 14:24:57.000000 netbox_device_support_plugin-1.0.4/setup.py
```

### Comparing `netbox_device_support_plugin-1.0.3/LICENSE` & `netbox_device_support_plugin-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/PKG-INFO` & `netbox_device_support_plugin-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-device-support-plugin
-Version: 1.0.3
+Version: 1.0.4
 Summary: Cisco device support, device type support, and software release information with the Cisco support APIs
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox_device_support_plugin-1.0.3/README.md` & `netbox_device_support_plugin-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/__init__.py` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/admin.py` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/admin.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/api/serializers.py` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/api/urls.py` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/api/views.py` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/filtersets.py` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/forms.py` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/forms.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/management/commands/sync_cisco_support_data.py` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/management/commands/sync_cisco_support_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -147,22 +147,24 @@
         try:
             ds = CiscoDeviceSupport.objects.get(device=d)
         except CiscoDeviceSupport.DoesNotExist:
             ds = CiscoDeviceSupport(device=d)
 
         #### Get recommended_release ########################################################################
         if isinstance(data, str):
-            # Save model object for device
-            ds.recommended_release = data
-            ds.desired_release_status = True
-            ds.current_release_status = True
             print(self.task_info(text=text, changed=False))
             print(f"{serial_number} - {data}")
-            # Save model object for device
-            ds.save()
+            # Update recommended_release if the value has changed
+            if ds.recommended_release != data:
+                ds.recommended_release = data
+                ds.desired_release_status = True
+                ds.current_release_status = True
+                # Save model object for device
+                ds.save()
+
             return True
 
         # Empty string to fill with the recommended releases and the error description
         recommended_release = ""
         error_description = ""
         # As there can be multiple suggestions with the same ID and release, but only with different mdfId,
         # the no_duplicates list will be created to eliminate duplicate IDs and release information.
@@ -190,40 +192,48 @@
             # Remove the last two characters from the string to remove the trailing slash
             if error_description_stdout.endswith(" / "):
                 error_description_stdout = error_description_stdout[:-2]
             # Error 'No records Found' is not a real error, but a valid response from the API
             if "No records Found" in error_description:
                 print(self.task_info(text=text, changed=False))
                 print(f"{serial_number} - recommended_release: No records Found")
-                ds.recommended_release = "No records Found"
-                rtn = True
-            else:
-                print(self.task_error(text=text, changed=False))
-                print(f"{serial_number} - recommended_release: {error_description_stdout}")
+                # Update recommended_release if the value has changed
+                if ds.recommended_release != "No records Found":
+                    ds.recommended_release = "No records Found"
+                    # Save model object for device
+                    ds.save()
+
+                return True
+            # Else it's a real error. Print the error description and return False
+            print(self.task_error(text=text, changed=False))
+            print(f"{serial_number} - recommended_release: {error_description_stdout}")
+            # Update recommended_release if the value has changed
+            if ds.recommended_release != "":
                 ds.recommended_release = ""
-                rtn = False
-            # Save model object for device
-            ds.save()
-            return rtn
+                # Save model object for device
+                ds.save()
+
+            return False
 
         recommended_release_stdout = recommended_release.replace("\n", " / ")
         # Remove the last two characters from the string to remove the trailing slash
         if recommended_release_stdout.endswith(" / "):
             recommended_release_stdout = recommended_release_stdout[:-2]
 
         print(self.task_info(text=text, changed=False))
         print(f"{serial_number} - recommended_release: {recommended_release_stdout}")
+        # Update recommended_release if the value has changed
+        if ds.recommended_release != recommended_release:
+            ds.recommended_release = recommended_release
+            # Save model object for device
+            ds.save()
 
-        ds.recommended_release = recommended_release
         # Desired release and current release can't be gathered by the Cisco Support API.
         # They should be added/updated over the RestAPI
 
-        #### Save model object for device ###################################################################
-        ds.save()
-
         return True
 
     # Updates a single device with current SNI coverage status data
     def update_device_sni_status_data(self, device):
         #### Get model object for device type ###############################################################
         text = f"Get data for serial number {device['sr_no']}"
         # Get the device object from NetBox
@@ -244,24 +254,26 @@
         #### Get sr_no_owner and api_status #################################################################
         # A "YES" string is not quite boolean :-)
         covered = True if device["sr_no_owner"] == "YES" else False
 
         print(self.task_info(text=text, changed=False))
         print(f"{device['sr_no']} - sr_no_owner: {covered}")
 
-        # Update sr_no_owner
-        ds.sr_no_owner = covered
-
-        #### Save model object for device ###################################################################
-        ds.save()
+        # Update sr_no_owner and save model object for device
+        if ds.is_covered != covered:
+            ds.sr_no_owner = covered
+            ds.save()
 
         return True
 
     # Updates a single device with current SNI coverage summary data
     def update_device_sni_summary_data(self, device):
+        # Control variable to only save the object if something has changed
+        value_changed = False
+
         #### Get model object for device ####################################################################
         text = f"Get data for serial number {device['sr_no']}"
         # Get the device object from NetBox
         try:
             d = Device.objects.get(serial=device["sr_no"])
         except MultipleObjectsReturned:
             # Error if netbox has multiple SN's and skip updating
@@ -289,98 +301,114 @@
 
         #### Get is_covered and contract_supplier ###########################################################
         # A "YES" string is not quite boolean :-)
         covered = True if device["is_covered"] == "YES" else False
 
         print(f"{device['sr_no']} - covered: {covered}")
 
-        # Update is_covered
-        ds.is_covered = covered
+        # Update is_covered if the value has changed
+        if ds.is_covered != covered:
+            ds.is_covered = covered
+            value_changed = True
 
         # The field contract_supplier and all fields regarding a Cisco partner contract like IBM TLS can't be
         # updated by the script and should be updated over the REST API.
 
         #### Get service_contract_number ####################################################################
         try:
             if not device["service_contract_number"]:
                 print(f"{device['sr_no']} - service_contract_number: None")
             else:
                 service_contract_number = device["service_contract_number"]
                 print(f"{device['sr_no']} - service_contract_number: {service_contract_number}")
 
-                # Update service_contract_number
-                ds.service_contract_number = service_contract_number
+                # Update service_contract_number if the value has changed
+                if ds.service_contract_number != service_contract_number:
+                    ds.service_contract_number = service_contract_number
+                    value_changed = True
 
         except KeyError:
             print(f"{device['sr_no']} - service_contract_number: None")
 
         #### Get service_line_descr #########################################################################
         try:
             if not device["service_line_descr"]:
                 print(f"{device['sr_no']} - service_line_descr: None")
             else:
                 service_line_descr = device["service_line_descr"]
                 print(f"{device['sr_no']} - service_line_descr: {service_line_descr}")
 
-                # Update service_line_descr
-                ds.service_line_descr = service_line_descr
+                # Update service_line_descr if the value has changed
+                if ds.service_line_descr != service_line_descr:
+                    ds.service_line_descr = service_line_descr
+                    value_changed = True
 
         except KeyError:
             print(f"{device['sr_no']} - service_line_descr: None")
 
         #### Get warranty_type ##############################################################################
         try:
             if not device["warranty_type"]:
                 print(f"{device['sr_no']} - warranty_type: None")
             else:
                 warranty_type = device["warranty_type"]
                 print(f"{device['sr_no']} - warranty_type: {warranty_type}")
 
-                # Update warranty_type
-                ds.warranty_type = warranty_type
+                # Update warranty_type if the value has changed
+                if ds.warranty_type != warranty_type:
+                    ds.warranty_type = warranty_type
+                    value_changed = True
 
         except KeyError:
             print(f"{device['sr_no']} - warranty_type: None")
 
         #### Get warranty_end_date ##########################################################################
         try:
             if not device["warranty_end_date"]:
                 print(f"{device['sr_no']} - warranty_end_date: None")
             else:
                 warranty_end_date_string = device["warranty_end_date"]
                 warranty_end_date = datetime.strptime(warranty_end_date_string, "%Y-%m-%d").date()
                 print(f"{device['sr_no']} - warranty_end_date: {warranty_end_date}")
 
-                # Update warranty_end_date
-                ds.warranty_end_date = warranty_end_date
+                # Update warranty_end_date if the value has changed
+                if ds.warranty_end_date != warranty_end_date:
+                    ds.warranty_end_date = warranty_end_date
+                    value_changed = True
 
         except KeyError:
             print(f"{device['sr_no']} - warranty_end_date: : None")
 
         #### Get covered_product_line_end_date ##############################################################
         try:
             if not device["covered_product_line_end_date"]:
                 print(f"{device['sr_no']} - covered_product_line_end_date: None")
             else:
                 coverage_end_date_string = device["covered_product_line_end_date"]
                 coverage_end_date = datetime.strptime(coverage_end_date_string, "%Y-%m-%d").date()
                 print(f"{device['sr_no']} - coverage_end_date: {coverage_end_date}")
 
-                # Update coverage_end_date
-                ds.coverage_end_date = coverage_end_date
+                # Update coverage_end_date if the value has changed
+                if ds.coverage_end_date != coverage_end_date:
+                    ds.coverage_end_date = coverage_end_date
+                    value_changed = True
 
         except KeyError:
             print(f"{device['sr_no']} - coverage_end_date: None")
 
         #### Save model object for device ###################################################################
-        ds.save()
+        if value_changed:
+            ds.save()
 
         return True
 
     def update_device_type_eox_data(self, pid, data):
+        # Control variable to only save the object if something has changed
+        value_changed = False
+
         #### Get model object for device type ###############################################################
         try:
             # Get the device type object for the supplied PID
             dt = DeviceType.objects.get(part_number=pid)
 
         except MultipleObjectsReturned:
             # Error if netbox has multiple PN's
@@ -420,31 +448,37 @@
         # Print the output for eox_has_error and eox_error
         if eox_has_error:
             print(self.task_error(text=f"Get data for PID {pid}", changed=False))
         else:
             print(self.task_info(text=f"Get data for PID {pid}", changed=False))
         print(output)
 
-        # Update eox_error
-        dts.eox_has_error = eox_has_error
-        dts.eox_error = eox_error
+        # Update eox_has_error and eox_error if the value has changed
+        if dts.eox_has_error != eox_has_error:
+            dts.eox_has_error = eox_has_error
+            value_changed = True
+        if dts.eox_error != eox_error:
+            dts.eox_error = eox_error
+            value_changed = True
 
         #### Get eox_announcement_date ######################################################################
         try:
             # Check if JSON contains EOXExternalAnnouncementDate with value field
             if not data["EOXRecord"][0]["EOXExternalAnnouncementDate"]["value"]:
                 print(f"{pid} - eox_announcement_date: None")
             else:
                 eox_announcement_date_string = data["EOXRecord"][0]["EOXExternalAnnouncementDate"]["value"]
                 # Cast this value to datetime.date object
                 eox_announcement_date = datetime.strptime(eox_announcement_date_string, "%Y-%m-%d").date()
                 print(f"{pid} - eox_announcement_date: {eox_announcement_date}")
 
-                # Update eox_announcement_date
-                dts.eox_announcement_date = eox_announcement_date
+                # Update eox_announcement_date if the value has changed
+                if dts.eox_announcement_date != eox_announcement_date:
+                    dts.eox_announcement_date = eox_announcement_date
+                    value_changed = True
 
         # Do nothing when JSON field does not exist
         except KeyError:
             print(f"{pid} - eox_announcement_date: None")
 
         #### Get end_of_sale_date ###########################################################################
         try:
@@ -453,16 +487,18 @@
                 print(f"{pid} - end_of_sale_date: None")
             else:
                 end_of_sale_date_string = data["EOXRecord"][0]["EndOfSaleDate"]["value"]
                 # Cast this value to datetime.date object
                 end_of_sale_date = datetime.strptime(end_of_sale_date_string, "%Y-%m-%d").date()
                 print(f"{pid} - end_of_sale_date: {end_of_sale_date}")
 
-                # Update end_of_sale_date
-                dts.end_of_sale_date = end_of_sale_date
+                # Update end_of_sale_date if the value has changed
+                if dts.end_of_sale_date != end_of_sale_date:
+                    dts.end_of_sale_date = end_of_sale_date
+                    value_changed = True
 
         # Do nothing when JSON field does not exist
         except KeyError:
             print(f"{pid} - end_of_sale_date: None")
 
         #### Get end_of_sw_maintenance_releases #############################################################
         try:
@@ -473,16 +509,18 @@
                     "value"
                 ]
                 end_of_sw_maintenance_releases = datetime.strptime(
                     end_of_sw_maintenance_releases_string, "%Y-%m-%d"
                 ).date()
                 print(f"{pid} - end_of_sw_maintenance_releases: {end_of_sw_maintenance_releases}")
 
-                # Update end_of_sw_maintenance_releases
-                dts.end_of_sw_maintenance_releases = end_of_sw_maintenance_releases
+                # Update end_of_sw_maintenance_releases if the value has changed
+                if dts.end_of_sw_maintenance_releases != end_of_sw_maintenance_releases:
+                    dts.end_of_sw_maintenance_releases = end_of_sw_maintenance_releases
+                    value_changed = True
 
         # Do nothing when JSON field does not exist
         except KeyError:
             print(f"{pid} - end_of_sw_maintenance_releases: None")
 
         #### Get end_of_security_vul_support_date ###########################################################
         try:
@@ -493,16 +531,18 @@
                     "value"
                 ]
                 end_of_security_vul_support_date = datetime.strptime(
                     end_of_security_vul_support_date_string, "%Y-%m-%d"
                 ).date()
                 print(f"{pid} - end_of_security_vul_support_date: {end_of_security_vul_support_date}")
 
-                # Update
-                dts.end_of_security_vul_support_date = end_of_security_vul_support_date
+                # Update end_of_security_vul_support_date if the value has changed
+                if dts.end_of_security_vul_support_date != end_of_security_vul_support_date:
+                    dts.end_of_security_vul_support_date = end_of_security_vul_support_date
+                    value_changed = True
 
         # Do nothing when JSON field does not exist
         except KeyError:
             print(f"{pid} - end_of_security_vul_support_date: None")
 
         #### Get end_of_routine_failure_analysis_date #######################################################
         try:
@@ -513,16 +553,18 @@
                     "EndOfRoutineFailureAnalysisDate"
                 ]["value"]
                 end_of_routine_failure_analysis_date = datetime.strptime(
                     end_of_routine_failure_analysis_date_string, "%Y-%m-%d"
                 ).date()
                 print(f"{pid} - end_of_routine_failure_analysis_date: {end_of_routine_failure_analysis_date}")
 
-                # Update end_of_routine_failure_analysis_date
-                dts.end_of_routine_failure_analysis_date = end_of_routine_failure_analysis_date
+                # Update end_of_routine_failure_analysis_date if the value has changed
+                if dts.end_of_routine_failure_analysis_date != end_of_routine_failure_analysis_date:
+                    dts.end_of_routine_failure_analysis_date = end_of_routine_failure_analysis_date
+                    value_changed = True
 
         # Do nothing when JSON field does not exist
         except KeyError:
             print(f"{pid} - end_of_routine_failure_analysis_date: None")
 
         #### Get end_of_service_contract_renewal ############################################################
         try:
@@ -533,55 +575,62 @@
                     "value"
                 ]
                 end_of_service_contract_renewal = datetime.strptime(
                     end_of_service_contract_renewal_string, "%Y-%m-%d"
                 ).date()
                 print(f"{pid} - end_of_service_contract_renewal: {end_of_service_contract_renewal}")
 
-                # Update end_of_service_contract_renewal
-                dts.end_of_service_contract_renewal = end_of_service_contract_renewal
+                # Update end_of_service_contract_renewal if the value has changed
+                if dts.end_of_service_contract_renewal != end_of_service_contract_renewal:
+                    dts.end_of_service_contract_renewal = end_of_service_contract_renewal
+                    value_changed = True
 
         # Do nothing when JSON field does not exist
         except KeyError:
             print(f"{pid} - end_of_service_contract_renewal: None")
 
         #### Get last_date_of_support #######################################################################
         try:
             if not data["EOXRecord"][0]["LastDateOfSupport"]["value"]:
                 print(f"{pid} - last_date_of_support: None")
             else:
                 last_date_of_support_string = data["EOXRecord"][0]["LastDateOfSupport"]["value"]
                 last_date_of_support = datetime.strptime(last_date_of_support_string, "%Y-%m-%d").date()
                 print(f"{pid} - last_date_of_support: {last_date_of_support}")
 
-                # Update last_date_of_support
-                dts.last_date_of_support = last_date_of_support
+                # Update last_date_of_support if the value has changed
+                if dts.last_date_of_support != last_date_of_support:
+                    dts.last_date_of_support = last_date_of_support
+                    value_changed = True
 
         # Do nothing when JSON field does not exist
         except KeyError:
             print(f"{pid} - last_date_of_support: None")
 
         #### Get end_of_svc_attach_date #####################################################################
         try:
             if not data["EOXRecord"][0]["EndOfSvcAttachDate"]["value"]:
                 print(f"{pid} - end_of_svc_attach_date: None")
             else:
                 end_of_svc_attach_date_string = data["EOXRecord"][0]["EndOfSvcAttachDate"]["value"]
                 end_of_svc_attach_date = datetime.strptime(end_of_svc_attach_date_string, "%Y-%m-%d").date()
                 print(f"{pid} - end_of_svc_attach_date: {end_of_svc_attach_date}")
 
-                # Update end_of_svc_attach_date
-                dts.end_of_svc_attach_date = end_of_svc_attach_date
+                # Update end_of_svc_attach_date if value has changed
+                if dts.end_of_svc_attach_date != end_of_svc_attach_date:
+                    dts.end_of_svc_attach_date = end_of_svc_attach_date
+                    value_changed = True
 
         # Do nothing when JSON field does not exist
         except KeyError:
             print(f"{pid} - end_of_svc_attach_date: None")
 
         #### Save model object for device type ##############################################################
-        dts.save()
+        if value_changed:
+            dts.save()
 
         return False if eox_has_error else True
 
     def get_device_types(self, manufacturer):
         task = "Get Manufacturer"
         print(self.task_name(text=task))
```

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/management/commands/sync_fortinet_support_data.py` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/management/commands/sync_fortinet_support_data.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/management/commands/sync_purestorage_support_data.py` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/management/commands/sync_purestorage_support_data.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/migrations/0001_initial.py` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/models.py` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/models.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/navigation.py` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/tables.py` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/tables.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,28 +32,29 @@
     end_of_sw_maintenance_releases = columns.DateColumn()
     end_of_security_vul_support_date = columns.DateColumn()
     end_of_routine_failure_analysis_date = columns.DateColumn()
     end_of_service_contract_renewal = columns.DateColumn()
     end_of_svc_attach_date = columns.DateColumn()
     last_date_of_support = columns.DateColumn()
 
-    actions = columns.ActionsColumn(actions=("delete",))
+    actions = columns.ActionsColumn(actions=("delete"))
 
     class Meta(NetBoxTable.Meta):
         model = CiscoDeviceSupport
         # fmt: off
         fields = (
-            "pk", "id", "device", "pid", "serial", "recommended_release", "desired_release", "current_release",
-            "desired_release_status", "current_release_status", "api_status", "sr_no_owner", "is_covered",
-            "contract_supplier", "coverage_end_date", "service_line_descr", "service_contract_number",
-            "warranty_end_date", "warranty_type", "partner_status", "partner_service_level",
-            "partner_customer_number", "partner_coverage_end_date", "eox_has_error", "eox_error",
-            "eox_announcement_date", "end_of_sale_date", "end_of_sw_maintenance_releases",
-            "end_of_security_vul_support_date", "end_of_routine_failure_analysis_date",
-            "end_of_service_contract_renewal", "last_date_of_support", "end_of_svc_attach_date",
+            "pk", "id", "device", "pid", "serial", "recommended_release", "desired_release",
+            "current_release", "desired_release_status", "current_release_status", "api_status",
+            "sr_no_owner", "is_covered", "contract_supplier", "coverage_end_date", "service_line_descr",
+            "service_contract_number", "warranty_end_date", "warranty_type", "partner_status",
+            "partner_service_level", "partner_customer_number", "partner_coverage_end_date",
+            "eox_has_error", "eox_error", "eox_announcement_date", "end_of_sale_date",
+            "end_of_sw_maintenance_releases", "end_of_security_vul_support_date",
+            "end_of_routine_failure_analysis_date", "end_of_service_contract_renewal",
+            "last_date_of_support", "end_of_svc_attach_date",
         )
         default_columns = (
             "device", "desired_release_status", "desired_release", "current_release_status",
             "current_release", "sr_no_owner", "is_covered", "contract_supplier", "coverage_end_date",
             "service_line_descr", "eox_announcement_date",
         )
         # fmt: on
@@ -71,15 +72,15 @@
     end_of_sw_maintenance_releases = columns.DateColumn()
     end_of_security_vul_support_date = columns.DateColumn()
     end_of_routine_failure_analysis_date = columns.DateColumn()
     end_of_service_contract_renewal = columns.DateColumn()
     end_of_svc_attach_date = columns.DateColumn()
     last_date_of_support = columns.DateColumn()
 
-    actions = columns.ActionsColumn(actions=("delete",))
+    actions = columns.ActionsColumn(actions=("delete"))
 
     class Meta(NetBoxTable.Meta):
         model = CiscoDeviceTypeSupport
         # fmt: off
         fields = (
             "pk", "id", "device_type", "pid", "eox_has_error", "eox_error", "eox_announcement_date",
             "end_of_sale_date", "end_of_sw_maintenance_releases", "end_of_security_vul_support_date",
@@ -102,23 +103,23 @@
     id = tables.Column(linkify=False)
 
     device = tables.Column(linkify=True)
 
     desired_release_status = columns.BooleanColumn()
     current_release_status = columns.BooleanColumn()
 
-    actions = columns.ActionsColumn(actions=("delete",))
+    actions = columns.ActionsColumn(actions=("delete"))
 
     class Meta(NetBoxTable.Meta):
         model = FortinetDeviceSupport
         # fmt: off
         fields = (
-            "pk", "id", "device", "pid", "serial", "recommended_release", "desired_release", "current_release",
-            "desired_release_status", "current_release_status", "partner", "end_of_renewal_date",
-            "end_of_support_date",
+            "pk", "id", "device", "pid", "serial", "recommended_release", "desired_release",
+            "current_release", "desired_release_status", "current_release_status", "partner",
+            "end_of_renewal_date", "end_of_support_date",
         )
         default_columns = (
             "device", "desired_release_status", "desired_release", "current_release_status",
             "current_release", "end_of_renewal_date", "end_of_support_date",
         )
         # fmt: on
 
@@ -127,15 +128,15 @@
 
 
 class PureStorageDeviceSupportTable(NetBoxTable):
     id = tables.Column(linkify=False)
 
     device = tables.Column(linkify=True)
 
-    actions = columns.ActionsColumn(actions=("delete",))
+    actions = columns.ActionsColumn(actions=("delete"))
 
     class Meta(NetBoxTable.Meta):
         model = PureStorageDeviceSupport
         # fmt: off
         fields = (
             "pk", "id", "device", "pid", "serial", "desired_release", "current_release",
         )
```

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/template_content.py` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/template_content.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 class CiscoDeviceTypeSupportInformation(PluginTemplateExtension):
     model = "dcim.devicetype"
 
     def _template_content(self):
         try:
             cisco_device_type_support = CiscoDeviceTypeSupport.objects.get(device_type=self.context["object"])
         except CiscoDeviceTypeSupport.DoesNotExist:
-            print("No Cisco Device Type Support Entry found")
             cisco_device_type_support = None
 
         return self.render(
             "cisco/cisco_device_type_support.html",
             {"cisco_device_type_support": cisco_device_type_support},
         )
 
@@ -45,23 +44,21 @@
 class CiscoDeviceSupportInformation(PluginTemplateExtension):
     model = "dcim.device"
 
     def _template_content(self):
         try:
             cisco_device_support = CiscoDeviceSupport.objects.get(device=self.context["object"])
         except CiscoDeviceSupport.DoesNotExist:
-            print("No Cisco Device Support Entry found")
             cisco_device_support = None
 
         try:
             cisco_device_type_support = CiscoDeviceTypeSupport.objects.get(
                 device_type=self.context["object"].device_type
             )
         except CiscoDeviceTypeSupport.DoesNotExist:
-            print("No Cisco Device Type Support Entry found")
             cisco_device_type_support = None
 
         return self.render(
             "cisco/cisco_device_support.html",
             {
                 "cisco_device_support": cisco_device_support,
                 "cisco_device_type_support": cisco_device_type_support,
@@ -85,15 +82,14 @@
 class FortinetDeviceSupportInformation(PluginTemplateExtension):
     model = "dcim.device"
 
     def _template_content(self):
         try:
             fortinet_device_support = FortinetDeviceSupport.objects.get(device=self.context["object"])
         except FortinetDeviceSupport.DoesNotExist:
-            print("No Fortinet Device Support Entry found")
             fortinet_device_support = None
 
         return self.render(
             "fortinet/fortinet_device_support.html",
             {"fortinet_device_support": fortinet_device_support},
         )
 
@@ -114,15 +110,14 @@
 class PureStorageDeviceSupportInformation(PluginTemplateExtension):
     model = "dcim.device"
 
     def _template_content(self):
         try:
             purestorage_device_support = PureStorageDeviceSupport.objects.get(device=self.context["object"])
         except PureStorageDeviceSupport.DoesNotExist:
-            print("No PureStorage Device Support Entry found")
             purestorage_device_support = None
 
         return self.render(
             "purestorage/purestorage_device_support.html",
             {"purestorage_device_support": purestorage_device_support},
         )
```

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/cisco_device_support.html` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/cisco_device_support.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/cisco_device_type_support.html` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/cisco_device_type_support.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_contract_coverage_bar.html` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/inc/device_contract_coverage_bar.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_partner_contract_coverage_bar.html` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/inc/device_partner_contract_coverage_bar.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eorfa_bar.html` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/inc/device_type_eorfa_bar.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eos_bar.html` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/inc/device_type_eos_bar.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eoscr_bar.html` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/inc/device_type_eoscr_bar.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eosm_bar.html` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/inc/device_type_eosm_bar.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvca_bar.html` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvca_bar.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvs_bar.html` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvs_bar.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/cisco/inc/device_type_last_day_support_bar.html` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/cisco/inc/device_type_last_day_support_bar.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/fortinet/fortinet_device_support.html` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/fortinet/fortinet_device_support.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/fortinet/inc/device_eor_bar.html` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/fortinet/inc/device_eor_bar.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/fortinet/inc/device_eos_bar.html` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/fortinet/inc/device_eos_bar.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templates/purestorage/purestorage_device_support.html` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templates/purestorage/purestorage_device_support.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/templatetags/filters.py` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/templatetags/filters.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/urls.py` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django.urls import path
 from . import views
 
 
 app_name = "netbox_device_support_plugin"
 
+
 urlpatterns = (
     # Cisco Device Support
     path(
         "cisco-device/",
         views.CiscoDeviceSupportListView.as_view(),
         name="ciscodevicesupport_list",
     ),
```

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin/views.py` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin/views.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin.egg-info/PKG-INFO` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-device-support-plugin
-Version: 1.0.3
+Version: 1.0.4
 Summary: Cisco device support, device type support, and software release information with the Cisco support APIs
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox_device_support_plugin-1.0.3/netbox_device_support_plugin.egg-info/SOURCES.txt` & `netbox_device_support_plugin-1.0.4/netbox_device_support_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.3/setup.py` & `netbox_device_support_plugin-1.0.4/setup.py`

 * *Files identical despite different names*

