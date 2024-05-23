# Comparing `tmp/adestis-netbox-plugin-account-management-1.7.9.tar.gz` & `tmp/adestis_netbox_plugin_account_management-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adestis-netbox-plugin-account-management-1.7.9.tar", last modified: Tue Dec  5 10:42:46 2023, max compression
+gzip compressed data, was "adestis_netbox_plugin_account_management-1.8.1.tar", last modified: Thu May 23 07:49:43 2024, max compression
```

## Comparing `adestis-netbox-plugin-account-management-1.7.9.tar` & `adestis_netbox_plugin_account_management-1.8.1.tar`

### file list

```diff
@@ -1,61 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-12-05 10:42:46.967319 adestis-netbox-plugin-account-management-1.7.9/
--rw-rw-rw-   0        0        0     1088 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/LICENSE
--rw-rw-rw-   0        0        0      175 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/MANIFEST.in
--rw-rw-rw-   0        0        0      326 2023-12-05 10:42:46.966089 adestis-netbox-plugin-account-management-1.7.9/PKG-INFO
--rw-rw-rw-   0        0        0     1446 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/README.md
-drwxrwxrwx   0        0        0        0 2023-12-05 10:42:46.839635 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/
--rw-rw-rw-   0        0        0      494 2023-12-05 10:40:12.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:42:46.888975 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/api/
--rw-rw-rw-   0        0        0        0 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/api/__init__.py
--rw-rw-rw-   0        0        0      516 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/api/nested_serializer.py
--rw-rw-rw-   0        0        0     2693 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/api/serializers.py
--rw-rw-rw-   0        0        0      301 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/api/urls.py
--rw-rw-rw-   0        0        0      682 2023-12-05 10:40:12.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/api/views.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:42:46.896011 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/filtersets/
--rw-rw-rw-   0        0        0       57 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/filtersets/__init__.py
--rw-rw-rw-   0        0        0     1944 2023-12-05 10:40:12.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/filtersets/login_credentials.py
--rw-rw-rw-   0        0        0     2560 2023-12-05 10:40:12.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/filtersets/system.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:42:46.904656 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/forms/
--rw-rw-rw-   0        0        0       57 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/forms/__init__.py
--rw-rw-rw-   0        0        0     5169 2023-12-05 10:40:12.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/forms/login_credentials.py
--rw-rw-rw-   0        0        0     8231 2023-12-05 08:50:04.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/forms/system.py
--rw-rw-rw-   0        0        0      878 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/graphql.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:42:46.930538 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/migrations/
--rw-rw-rw-   0        0        0     4725 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      444 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/migrations/0002_alter_system_system_url.py
--rw-rw-rw-   0        0        0      756 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/migrations/0003_remove_logincredentials_adestis_netbox_plugin_account_management_logincredentials_unique_login_crede.py
--rw-rw-rw-   0        0        0     4163 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/migrations/0004_alter_logincredentials_options_alter_person_options_and_more.py
--rw-rw-rw-   0        0        0      529 2023-12-05 08:40:55.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/migrations/0005_person_mitigation.py
--rw-rw-rw-   0        0        0      761 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/migrations/0006_fix_constraint_logincredentials.py
--rw-rw-rw-   0        0        0      286 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/migrations/0007_remove_logincredentials_person.py
--rw-rw-rw-   0        0        0      662 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/migrations/0008_alter_logincredentials_contact.py
--rw-rw-rw-   0        0        0      401 2023-12-05 08:40:55.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/migrations/0009_remove_logincredentials_person.py
--rw-rw-rw-   0        0        0     1114 2023-12-05 08:40:55.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/migrations/0010_remove_person_adestis_netbox_plugin_account_management_person_unique_mail_address_and_more.py
--rw-rw-rw-   0        0        0      417 2023-12-05 08:40:55.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/migrations/0011_delete_person.py
--rw-rw-rw-   0        0        0        0 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:42:46.937060 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/models/
--rw-rw-rw-   0        0        0       57 2023-12-05 08:40:55.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/models/__init__.py
--rw-rw-rw-   0        0        0     2990 2023-12-05 08:40:55.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/models/login_credentials.py
--rw-rw-rw-   0        0        0     3347 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/models/system.py
--rw-rw-rw-   0        0        0     1331 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/navigation.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:42:46.949182 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/tables/
--rw-rw-rw-   0        0        0       57 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/tables/__init__.py
--rw-rw-rw-   0        0        0      947 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/tables/login_credentials.py
--rw-rw-rw-   0        0        0     1180 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/tables/system.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:42:46.812223 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/templates/
-drwxrwxrwx   0        0        0        0 2023-12-05 10:42:46.957951 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/
--rw-rw-rw-   0        0        0      371 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/device_login_credentials_table.html
--rw-rw-rw-   0        0        0     1685 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/logincredentials.html
--rw-rw-rw-   0        0        0     2917 2023-12-05 08:40:55.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/system.html
--rw-rw-rw-   0        0        0     2110 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/urls.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:42:46.963915 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/views/
--rw-rw-rw-   0        0        0       57 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/views/__init__.py
--rw-rw-rw-   0        0        0     2544 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/views/login_credentials.py
--rw-rw-rw-   0        0        0     1734 2023-10-27 13:17:39.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/views/system.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:42:46.876708 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management.egg-info/
--rw-rw-rw-   0        0        0      326 2023-12-05 10:42:46.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3246 2023-12-05 10:42:46.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-05 10:42:46.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-12-05 10:42:46.000000 adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-05 10:42:46.967829 adestis-netbox-plugin-account-management-1.7.9/setup.cfg
--rw-rw-rw-   0        0        0      602 2023-12-05 10:40:12.000000 adestis-netbox-plugin-account-management-1.7.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:49:43.938345 adestis_netbox_plugin_account_management-1.8.1/
+-rw-rw-rw-   0        0        0     1088 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/LICENSE
+-rw-rw-rw-   0        0        0      175 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      326 2024-05-23 07:49:43.938345 adestis_netbox_plugin_account_management-1.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1446 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 07:49:43.736977 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/
+-rw-rw-rw-   0        0        0      494 2024-05-23 06:44:59.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:49:43.776859 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/api/
+-rw-rw-rw-   0        0        0        0 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/api/__init__.py
+-rw-rw-rw-   0        0        0      516 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/api/nested_serializer.py
+-rw-rw-rw-   0        0        0     2974 2024-05-22 14:31:29.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/api/serializers.py
+-rw-rw-rw-   0        0        0      301 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/api/urls.py
+-rw-rw-rw-   0        0        0      682 2024-05-22 08:01:01.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/api/views.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:49:43.790222 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/filtersets/
+-rw-rw-rw-   0        0        0       57 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/filtersets/__init__.py
+-rw-rw-rw-   0        0        0     1993 2024-05-23 07:05:26.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/filtersets/login_credentials.py
+-rw-rw-rw-   0        0        0     2558 2024-05-23 07:07:59.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/filtersets/system.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:49:43.806154 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/forms/
+-rw-rw-rw-   0        0        0       57 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/forms/__init__.py
+-rw-rw-rw-   0        0        0     5236 2024-05-23 07:20:53.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/forms/login_credentials.py
+-rw-rw-rw-   0        0        0     8268 2024-05-22 14:30:11.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/forms/system.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:49:43.817107 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/graphql/
+-rw-rw-rw-   0        0        0       57 2024-05-23 06:44:17.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/graphql/__init__.py
+-rw-rw-rw-   0        0        0      869 2024-05-23 07:04:08.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/graphql/login_credentials.py
+-rw-rw-rw-   0        0        0      845 2024-05-23 07:04:33.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/graphql/system.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:49:43.877884 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/migrations/
+-rw-rw-rw-   0        0        0     4725 2024-05-23 07:37:12.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      444 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/migrations/0002_alter_system_system_url.py
+-rw-rw-rw-   0        0        0      756 2024-05-23 07:43:07.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/migrations/0003_remove_logincredentials_adestis_netbox_plugin_account_management_logincredentials_unique_login_crede.py
+-rw-rw-rw-   0        0        0     4163 2024-05-23 07:43:07.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/migrations/0004_alter_logincredentials_options_alter_person_options_and_more.py
+-rw-rw-rw-   0        0        0      529 2023-11-06 09:36:09.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/migrations/0005_person_mitigation.py
+-rw-rw-rw-   0        0        0      761 2024-05-23 07:37:28.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/migrations/0006_fix_constraint_logincredentials.py
+-rw-rw-rw-   0        0        0      286 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/migrations/0007_remove_logincredentials_person.py
+-rw-rw-rw-   0        0        0      662 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/migrations/0008_alter_logincredentials_contact.py
+-rw-rw-rw-   0        0        0      401 2023-11-06 09:09:50.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/migrations/0009_remove_logincredentials_person.py
+-rw-rw-rw-   0        0        0     1114 2024-05-23 07:43:07.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/migrations/0010_remove_person_adestis_netbox_plugin_account_management_person_unique_mail_address_and_more.py
+-rw-rw-rw-   0        0        0      417 2024-05-23 07:43:07.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/migrations/0011_delete_person.py
+-rw-rw-rw-   0        0        0        0 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:49:43.889562 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/models/
+-rw-rw-rw-   0        0        0       57 2023-11-06 09:36:09.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/models/__init__.py
+-rw-rw-rw-   0        0        0     2990 2023-11-06 09:09:50.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/models/login_credentials.py
+-rw-rw-rw-   0        0        0     3347 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/models/system.py
+-rw-rw-rw-   0        0        0     1084 2024-05-22 11:48:39.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/navigation.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:49:43.902227 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/tables/
+-rw-rw-rw-   0        0        0       57 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/tables/__init__.py
+-rw-rw-rw-   0        0        0      947 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/tables/login_credentials.py
+-rw-rw-rw-   0        0        0     1180 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/tables/system.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:49:43.710214 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/templates/
+drwxrwxrwx   0        0        0        0 2024-05-23 07:49:43.914916 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/
+-rw-rw-rw-   0        0        0      371 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/device_login_credentials_table.html
+-rw-rw-rw-   0        0        0     1685 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/logincredentials.html
+-rw-rw-rw-   0        0        0     2917 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/system.html
+-rw-rw-rw-   0        0        0     2110 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/urls.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:49:43.928288 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/views/
+-rw-rw-rw-   0        0        0       57 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/views/__init__.py
+-rw-rw-rw-   0        0        0     2544 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/views/login_credentials.py
+-rw-rw-rw-   0        0        0     1734 2023-11-06 08:39:20.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/views/system.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:49:43.932111 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management.egg-info/
+-rw-rw-rw-   0        0        0      326 2024-05-23 07:49:43.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3384 2024-05-23 07:49:43.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 07:49:43.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-23 07:49:43.000000 adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 07:49:43.938345 adestis_netbox_plugin_account_management-1.8.1/setup.cfg
+-rw-rw-rw-   0        0        0      602 2024-05-23 06:44:59.000000 adestis_netbox_plugin_account_management-1.8.1/setup.py
```

### Comparing `adestis-netbox-plugin-account-management-1.7.9/LICENSE` & `adestis_netbox_plugin_account_management-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.7.9/README.md` & `adestis_netbox_plugin_account_management-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/api/nested_serializer.py` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/api/nested_serializer.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/api/serializers.py` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/api/serializers.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     contact = NestedContactSerializer(many=False,
                                       read_only=False,
                                       required=False)
 
     class Meta:
         model = LoginCredentials
         fields = '__all__'
+        brief_fields = '__all__'
         read_only_fields = ('contact', 'system')
 
 
 class SystemSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:adestis_netbox_plugin_account_management-api:system-detail'
     )
@@ -63,7 +64,9 @@
                                   read_only=False,
                                   required=False)
 
     class Meta:
         model = System
         fields = ('id', 'url', 'display', 'name', 'system_url', 'system_status', 'device', 'virtual_machine', 'group', 'tenant', 'cluster_group', 'cluster', 'comments', 'tags',
                   'custom_fields', 'created', 'last_updated')
+        brief_fields = ('id', 'url', 'display', 'name', 'system_url', 'system_status', 'device', 'virtual_machine', 'group', 'tenant', 'cluster_group', 'cluster', 'comments', 'tags',
+                  'custom_fields', 'created', 'last_updated')
```

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/api/views.py` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/api/views.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/filtersets/login_credentials.py` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/filtersets/login_credentials.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from utilities.forms.widgets import DatePicker
 from tenancy.models import Contact
 
 __all__ = (
     'LoginCredentialsFilterSet',
 )
 
-
 class LoginCredentialsFilterSet(NetBoxModelFilterSet):
     
     contact_id = DynamicModelMultipleChoiceField(
         queryset=Contact.objects.all(),
         required=False,
         null_option='None',
         label=_('Group')
@@ -58,9 +57,11 @@
     def search(self, queryset, name, value):
         if not value.strip():
             return queryset
         return queryset.filter(
             Q(logon_name__icontains=value) |
              Q(contact__name__icontains=value) |
             Q(login_credentials_status__icontains=value) |
-            Q(system__name__icontains=value) 
+            Q(system__name__icontains=value) |
+            Q(contact__name__icontains=value) 
+
         )
```

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/filtersets/system.py` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/filtersets/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from virtualization.models import VirtualMachine, ClusterGroup, Cluster
 from tenancy.models import TenantGroup, Tenant
 
 __all__ = (
     'SystemFilterSet',
 )
 
-
 class SystemFilterSet(NetBoxModelFilterSet):
     
     cluster_group_id = DynamicModelMultipleChoiceField(
         queryset=ClusterGroup.objects.all(),
         required=False,
         label=_('Cluster group (name)')
     )
```

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/forms/login_credentials.py` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/forms/login_credentials.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-import json
 from django import forms
 from django.core.exceptions import ValidationError
 from netbox.forms import NetBoxModelForm, NetBoxModelFilterSetForm, NetBoxModelBulkEditForm, NetBoxModelImportForm
 from utilities.forms.fields import CommentField, DynamicModelChoiceField, DynamicModelMultipleChoiceField, CSVChoiceField, CSVModelChoiceField, TagFilterField
 from utilities.forms.widgets import DatePicker
 from adestis_netbox_plugin_account_management.models.login_credentials import LoginCredentials, LoginCredentialsStatusChoices
 from adestis_netbox_plugin_account_management.models.system import System, SystemStatusChoices
 from tenancy.models import Contact
-from django.utils.translation import gettext as _
+from django.utils.translation import gettext_lazy as _
+from utilities.forms.rendering import FieldSet
+
 
 __all__ = (
     'LoginCredentialsForm',
     'LoginCredentialsFilterForm',
     'LoginCredentialsBulkEditForm',
     'LoginCredentialsCSVForm'
 )
@@ -113,25 +114,26 @@
        'valid_from', 'valid_to', 'add_tags', 'remove_tags'
     ]
 
 class LoginCredentialsFilterForm(NetBoxModelFilterSetForm):
     model = LoginCredentials
     
     fieldsets = (
-        (None, ('q', 'index', 'tag', 'contact_id', 'system', 'login_credentials_status')),
+        (None, ('q', 'index', 'tag', 'contact', 'system', 'login_credentials_status')),
     )  
 
     index = forms.IntegerField(
         required=False
     )
 
-    contact_id = DynamicModelMultipleChoiceField(
+    contact = DynamicModelMultipleChoiceField(
         queryset=Contact.objects.all(),
         required=False,
         null_option='None',
+        to_field_name='name',
         label=_('Contact')
     )
 
     system = forms.ModelMultipleChoiceField(
         queryset=System.objects.all(),
         required=False
     )
```

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/forms/system.py` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/forms/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from django import forms
 from netbox.forms import NetBoxModelForm, NetBoxModelFilterSetForm, NetBoxModelBulkEditForm, NetBoxModelImportForm
-from django.utils.translation import gettext as _
 from tenancy.models import *
 from dcim.models import *
 from utilities.forms.fields import DynamicModelChoiceField, DynamicModelMultipleChoiceField, CSVModelChoiceField, CSVChoiceField, TagFilterField
 from virtualization.models import VirtualMachine, ClusterGroup, Cluster
 from adestis_netbox_plugin_account_management.models.login_credentials import LoginCredentials, LoginCredentialsStatusChoices
 from adestis_netbox_plugin_account_management.models.system import System, SystemStatusChoices
+from django.utils.translation import gettext_lazy as _
+from utilities.forms.rendering import FieldSet
 
 __all__ = (
     'SystemForm',
     'SystemFilterForm',
     'SystemBulkEditForm',
     'SystemCSVForm'
 )
@@ -66,22 +67,20 @@
         null_option='None',
         query_params={
             'cluster_id': '$cluster',
             'device_id': '$device',
         },
         help_text=_("Pin this system to a specific virtual machine of the selected device"),
     )
-    
 
-    
     fieldsets = (
         ('System', ('name', 'system_url', 'system_status', 'tags')),
         ('Computing', ('group', 'tenant', 'cluster_group', 'cluster', 'device', 'virtual_machine')),
     )
-    
+
     class Meta:
         model = System
         fields = ('cluster_group', 'cluster', 'device', 'virtual_machine', 'name', 'system_url', 'group', 'tenant', 'system_status', 'comments', 'tags')
         
 
 class SystemBulkEditForm(NetBoxModelBulkEditForm):
```

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/migrations/0001_initial.py` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/migrations/0003_remove_logincredentials_adestis_netbox_plugin_account_management_logincredentials_unique_login_crede.py` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/migrations/0003_remove_logincredentials_adestis_netbox_plugin_account_management_logincredentials_unique_login_crede.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/migrations/0004_alter_logincredentials_options_alter_person_options_and_more.py` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/migrations/0004_alter_logincredentials_options_alter_person_options_and_more.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/migrations/0005_person_mitigation.py` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/migrations/0005_person_mitigation.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/migrations/0006_fix_constraint_logincredentials.py` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/migrations/0006_fix_constraint_logincredentials.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/migrations/0008_alter_logincredentials_contact.py` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/migrations/0008_alter_logincredentials_contact.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/migrations/0010_remove_person_adestis_netbox_plugin_account_management_person_unique_mail_address_and_more.py` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/migrations/0010_remove_person_adestis_netbox_plugin_account_management_person_unique_mail_address_and_more.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/models/login_credentials.py` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/models/login_credentials.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/models/system.py` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/models/system.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/tables/login_credentials.py` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/tables/login_credentials.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/tables/system.py` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/tables/system.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/logincredentials.html` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/logincredentials.html`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/system.html` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/system.html`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/urls.py` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/urls.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/views/login_credentials.py` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/views/login_credentials.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management/views/system.py` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management/views/system.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.7.9/adestis_netbox_plugin_account_management.egg-info/SOURCES.txt` & `adestis_netbox_plugin_account_management-1.8.1/adestis_netbox_plugin_account_management.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 adestis_netbox_plugin_account_management/__init__.py
-adestis_netbox_plugin_account_management/graphql.py
 adestis_netbox_plugin_account_management/navigation.py
 adestis_netbox_plugin_account_management/urls.py
 adestis_netbox_plugin_account_management.egg-info/PKG-INFO
 adestis_netbox_plugin_account_management.egg-info/SOURCES.txt
 adestis_netbox_plugin_account_management.egg-info/dependency_links.txt
 adestis_netbox_plugin_account_management.egg-info/top_level.txt
 adestis_netbox_plugin_account_management/api/__init__.py
@@ -17,14 +16,17 @@
 adestis_netbox_plugin_account_management/api/views.py
 adestis_netbox_plugin_account_management/filtersets/__init__.py
 adestis_netbox_plugin_account_management/filtersets/login_credentials.py
 adestis_netbox_plugin_account_management/filtersets/system.py
 adestis_netbox_plugin_account_management/forms/__init__.py
 adestis_netbox_plugin_account_management/forms/login_credentials.py
 adestis_netbox_plugin_account_management/forms/system.py
+adestis_netbox_plugin_account_management/graphql/__init__.py
+adestis_netbox_plugin_account_management/graphql/login_credentials.py
+adestis_netbox_plugin_account_management/graphql/system.py
 adestis_netbox_plugin_account_management/migrations/0001_initial.py
 adestis_netbox_plugin_account_management/migrations/0002_alter_system_system_url.py
 adestis_netbox_plugin_account_management/migrations/0003_remove_logincredentials_adestis_netbox_plugin_account_management_logincredentials_unique_login_crede.py
 adestis_netbox_plugin_account_management/migrations/0004_alter_logincredentials_options_alter_person_options_and_more.py
 adestis_netbox_plugin_account_management/migrations/0005_person_mitigation.py
 adestis_netbox_plugin_account_management/migrations/0006_fix_constraint_logincredentials.py
 adestis_netbox_plugin_account_management/migrations/0007_remove_logincredentials_person.py
```

### Comparing `adestis-netbox-plugin-account-management-1.7.9/setup.py` & `adestis_netbox_plugin_account_management-1.8.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='adestis-netbox-plugin-account-management',
-    version='1.7.9',
+    version='1.8.1',
     description='ADESTIS Account Management',
     url='https://github.com/adestis/netbox-account-management',
     author='ADESTIS GmbH',
     author_email='pypi@adestis.de',
     install_requires=[],
     packages=find_packages(),
     include_package_data=True,
```

