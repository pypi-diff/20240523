# Comparing `tmp/ElasticEmail-4.0.24.tar.gz` & `tmp/elasticemail-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ElasticEmail-4.0.24.tar", last modified: Mon Nov 27 14:16:50 2023, max compression
+gzip compressed data, was "elasticemail-4.1.0.tar", last modified: Thu May 23 09:32:05 2024, max compression
```

## Comparing `ElasticEmail-4.0.24.tar` & `elasticemail-4.1.0.tar`

### file list

```diff
@@ -1,1014 +1,912 @@
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.616716 ElasticEmail-4.0.24/
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:49.980722 ElasticEmail-4.0.24/ElasticEmail/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1504 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/__init__.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:49.996721 ElasticEmail-4.0.24/ElasticEmail/api/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      218 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/api/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    27527 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/api/campaigns_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    50021 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/api/contacts_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    22555 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/api/emails_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    45287 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/api/events_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    27123 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/api/files_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    31896 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/api/inbound_route_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    38240 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/api/lists_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    54298 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/api/security_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    27291 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/api/segments_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    27679 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/api/statistics_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    33839 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/api/sub_accounts_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    63553 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/api/suppressions_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    28255 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/api/templates_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    53083 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/api/verifications_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    59261 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/api_client.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.000721 ElasticEmail-4.0.24/ElasticEmail/apis/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      214 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/apis/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11938 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/apis/path_to_api.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.044721 ElasticEmail-4.0.24/ElasticEmail/apis/paths/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      239 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      174 2023-11-27 14:16:08.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/campaigns.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      269 2023-11-27 14:16:08.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/campaigns_name.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      171 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/contacts.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      115 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/contacts_delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      269 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/contacts_email.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      115 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/contacts_export.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      130 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/contacts_export_id_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      115 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/contacts_import.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)       98 2023-11-27 14:16:14.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/emails.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      117 2023-11-27 14:16:14.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/emails_mergefile.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      115 2023-11-27 14:16:14.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/emails_msgid_view.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      125 2023-11-27 14:16:14.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/emails_transactional.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)       95 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/events.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      143 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/events_channels_export_id_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      121 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/events_channels_name.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      137 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/events_channels_name_export.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      111 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/events_export.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      126 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/events_export_id_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      122 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/events_transactionid.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      162 2023-11-27 14:16:19.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/files.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      182 2023-11-27 14:16:19.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/files_name.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      111 2023-11-27 14:16:19.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/files_name_info.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      183 2023-11-27 14:16:21.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/inboundroute.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      273 2023-11-27 14:16:21.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/inboundroute_id.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      118 2023-11-27 14:16:21.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/inboundroute_order.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      162 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/lists.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      253 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/lists_name.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      122 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/lists_name_contacts.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      135 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/lists_name_contacts_remove.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      194 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/security_apikeys.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      296 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/security_apikeys_name.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      185 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/security_smtp.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      284 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/security_smtp_name.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      171 2023-11-27 14:16:28.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/segments.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      265 2023-11-27 14:16:28.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/segments_name.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      103 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/statistics.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      122 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/statistics_campaigns.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      131 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/statistics_campaigns_name.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      120 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/statistics_channels.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      129 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/statistics_channels_name.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      180 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/subaccounts.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      203 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/subaccounts_email.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      137 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/subaccounts_email_credits.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      144 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/subaccounts_email_settings_email.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      107 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/suppressions.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      206 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/suppressions_bounces.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      138 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/suppressions_bounces_import.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      215 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/suppressions_complaints.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      144 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/suppressions_complaints_import.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      206 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/suppressions_email.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      221 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/suppressions_unsubscribes.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      148 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/suppressions_unsubscribes_import.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      174 2023-11-27 14:16:37.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/templates.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      269 2023-11-27 14:16:37.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/templates_name.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      109 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/verifications.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      292 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/verifications_email.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      123 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/verifications_files.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      134 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/verifications_files_id.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      138 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/verifications_files_id_result.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      155 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/verifications_files_id_result_download.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      153 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/verifications_files_id_verification.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      133 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/apis/paths/verifications_files_result.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2234 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/apis/tag_to_api.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.052721 ElasticEmail-4.0.24/ElasticEmail/apis/tags/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      671 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/apis/tags/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1623 2023-11-27 14:16:08.000000 ElasticEmail-4.0.24/ElasticEmail/apis/tags/campaigns_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2023 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/ElasticEmail/apis/tags/contacts_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1555 2023-11-27 14:16:14.000000 ElasticEmail-4.0.24/ElasticEmail/apis/tags/emails_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1941 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/ElasticEmail/apis/tags/events_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1572 2023-11-27 14:16:19.000000 ElasticEmail-4.0.24/ElasticEmail/apis/tags/files_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1754 2023-11-27 14:16:21.000000 ElasticEmail-4.0.24/ElasticEmail/apis/tags/inbound_route_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1796 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/ElasticEmail/apis/tags/lists_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2210 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/ElasticEmail/apis/tags/security_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1607 2023-11-27 14:16:28.000000 ElasticEmail-4.0.24/ElasticEmail/apis/tags/segments_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1716 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/ElasticEmail/apis/tags/statistics_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1835 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/ElasticEmail/apis/tags/sub_accounts_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2597 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/ElasticEmail/apis/tags/suppressions_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1623 2023-11-27 14:16:37.000000 ElasticEmail-4.0.24/ElasticEmail/apis/tags/templates_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2410 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/apis/tags/verifications_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    17320 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/configuration.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5282 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/exceptions.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.172720 ElasticEmail-4.0.24/ElasticEmail/model/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      346 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8966 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/access_level.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6500 2023-11-27 14:15:41.000000 ElasticEmail-4.0.24/ElasticEmail/model/access_level.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2134 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/account_status_enum.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1912 2023-11-27 14:15:42.000000 ElasticEmail-4.0.24/ElasticEmail/model/account_status_enum.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9345 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/api_key.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9345 2023-11-27 14:15:44.000000 ElasticEmail-4.0.24/ElasticEmail/model/api_key.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8113 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/api_key_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8113 2023-11-27 14:15:45.000000 ElasticEmail-4.0.24/ElasticEmail/model/api_key_payload.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2075 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/body_content_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1893 2023-11-27 14:15:46.000000 ElasticEmail-4.0.24/ElasticEmail/model/body_content_type.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4482 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/body_part.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4482 2023-11-27 14:15:46.000000 ElasticEmail-4.0.24/ElasticEmail/model/body_part.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6598 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/campaign.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6598 2023-11-27 14:15:47.000000 ElasticEmail-4.0.24/ElasticEmail/model/campaign.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8097 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/campaign_options.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8097 2023-11-27 14:15:48.000000 ElasticEmail-4.0.24/ElasticEmail/model/campaign_options.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5486 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/campaign_recipient.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5486 2023-11-27 14:15:48.000000 ElasticEmail-4.0.24/ElasticEmail/model/campaign_recipient.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2569 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/campaign_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2228 2023-11-27 14:15:48.000000 ElasticEmail-4.0.24/ElasticEmail/model/campaign_status.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     7120 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/campaign_template.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     7120 2023-11-27 14:15:49.000000 ElasticEmail-4.0.24/ElasticEmail/model/campaign_template.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10652 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/channel_log_status_summary.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10652 2023-11-27 14:15:49.000000 ElasticEmail-4.0.24/ElasticEmail/model/channel_log_status_summary.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1861 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/compression_format.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1744 2023-11-27 14:15:50.000000 ElasticEmail-4.0.24/ElasticEmail/model/compression_format.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5265 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/consent_data.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5265 2023-11-27 14:15:50.000000 ElasticEmail-4.0.24/ElasticEmail/model/consent_data.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1948 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/consent_tracking.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1793 2023-11-27 14:15:50.000000 ElasticEmail-4.0.24/ElasticEmail/model/consent_tracking.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11779 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/contact.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11779 2023-11-27 14:15:51.000000 ElasticEmail-4.0.24/ElasticEmail/model/contact.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12786 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/contact_activity.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12786 2023-11-27 14:15:51.000000 ElasticEmail-4.0.24/ElasticEmail/model/contact_activity.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     7251 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/contact_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     7251 2023-11-27 14:15:52.000000 ElasticEmail-4.0.24/ElasticEmail/model/contact_payload.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2590 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/contact_source.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2213 2023-11-27 14:15:52.000000 ElasticEmail-4.0.24/ElasticEmail/model/contact_source.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2724 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/contact_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2330 2023-11-27 14:15:52.000000 ElasticEmail-4.0.24/ElasticEmail/model/contact_status.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5502 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/contact_update_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5502 2023-11-27 14:15:52.000000 ElasticEmail-4.0.24/ElasticEmail/model/contact_update_payload.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5737 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/contacts_list.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5737 2023-11-27 14:15:53.000000 ElasticEmail-4.0.24/ElasticEmail/model/contacts_list.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2013 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/delivery_optimization_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1830 2023-11-27 14:15:53.000000 ElasticEmail-4.0.24/ElasticEmail/model/delivery_optimization_type.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13950 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/email_content.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13950 2023-11-27 14:15:53.000000 ElasticEmail-4.0.24/ElasticEmail/model/email_content.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5351 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/email_data.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5351 2023-11-27 14:15:54.000000 ElasticEmail-4.0.24/ElasticEmail/model/email_data.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5462 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/email_message_data.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5462 2023-11-27 14:15:54.000000 ElasticEmail-4.0.24/ElasticEmail/model/email_message_data.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2207 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/email_predicted_validation_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1980 2023-11-27 14:15:54.000000 ElasticEmail-4.0.24/ElasticEmail/model/email_predicted_validation_status.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4883 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/email_recipient.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4883 2023-11-27 14:15:54.000000 ElasticEmail-4.0.24/ElasticEmail/model/email_recipient.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3801 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/email_send.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3801 2023-11-27 14:15:54.000000 ElasticEmail-4.0.24/ElasticEmail/model/email_send.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10809 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/email_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10809 2023-11-27 14:15:55.000000 ElasticEmail-4.0.24/ElasticEmail/model/email_status.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4674 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/email_transactional_message_data.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4674 2023-11-27 14:15:55.000000 ElasticEmail-4.0.24/ElasticEmail/model/email_transactional_message_data.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9093 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/email_validation_result.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9093 2023-11-27 14:15:55.000000 ElasticEmail-4.0.24/ElasticEmail/model/email_validation_result.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2182 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/email_validation_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1963 2023-11-27 14:15:55.000000 ElasticEmail-4.0.24/ElasticEmail/model/email_validation_status.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4065 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/email_view.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4065 2023-11-27 14:15:55.000000 ElasticEmail-4.0.24/ElasticEmail/model/email_view.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4514 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/emails_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4514 2023-11-27 14:15:56.000000 ElasticEmail-4.0.24/ElasticEmail/model/emails_payload.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2502 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/encoding_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2189 2023-11-27 14:15:56.000000 ElasticEmail-4.0.24/ElasticEmail/model/encoding_type.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2597 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/event_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2249 2023-11-27 14:15:56.000000 ElasticEmail-4.0.24/ElasticEmail/model/event_type.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1904 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/events_order_by.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1745 2023-11-27 14:15:56.000000 ElasticEmail-4.0.24/ElasticEmail/model/events_order_by.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1960 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/export_file_formats.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1817 2023-11-27 14:15:56.000000 ElasticEmail-4.0.24/ElasticEmail/model/export_file_formats.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3751 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/export_link.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3751 2023-11-27 14:15:56.000000 ElasticEmail-4.0.24/ElasticEmail/model/export_link.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2102 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/export_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1911 2023-11-27 14:15:56.000000 ElasticEmail-4.0.24/ElasticEmail/model/export_status.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6962 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/file_info.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6962 2023-11-27 14:15:57.000000 ElasticEmail-4.0.24/ElasticEmail/model/file_info.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4370 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/file_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4370 2023-11-27 14:15:57.000000 ElasticEmail-4.0.24/ElasticEmail/model/file_payload.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3983 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/file_upload_result.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3983 2023-11-27 14:15:57.000000 ElasticEmail-4.0.24/ElasticEmail/model/file_upload_result.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6277 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/inbound_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6277 2023-11-27 14:15:57.000000 ElasticEmail-4.0.24/ElasticEmail/model/inbound_payload.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6814 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/inbound_route.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6814 2023-11-27 14:15:57.000000 ElasticEmail-4.0.24/ElasticEmail/model/inbound_route.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2023 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/inbound_route_action_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1834 2023-11-27 14:15:58.000000 ElasticEmail-4.0.24/ElasticEmail/model/inbound_route_action_type.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1879 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/inbound_route_filter_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1737 2023-11-27 14:15:58.000000 ElasticEmail-4.0.24/ElasticEmail/model/inbound_route_filter_type.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5188 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/list_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5188 2023-11-27 14:15:58.000000 ElasticEmail-4.0.24/ElasticEmail/model/list_payload.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3884 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/list_update_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3884 2023-11-27 14:15:58.000000 ElasticEmail-4.0.24/ElasticEmail/model/list_update_payload.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2841 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/log_job_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2413 2023-11-27 14:15:58.000000 ElasticEmail-4.0.24/ElasticEmail/model/log_job_status.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10060 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/log_status_summary.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10060 2023-11-27 14:15:58.000000 ElasticEmail-4.0.24/ElasticEmail/model/log_status_summary.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4582 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/merge_email_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4582 2023-11-27 14:15:59.000000 ElasticEmail-4.0.24/ElasticEmail/model/merge_email_payload.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4877 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/message_attachment.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4877 2023-11-27 14:15:59.000000 ElasticEmail-4.0.24/ElasticEmail/model/message_attachment.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3918 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/message_category.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3128 2023-11-27 14:15:59.000000 ElasticEmail-4.0.24/ElasticEmail/model/message_category.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9865 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/new_api_key.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9865 2023-11-27 14:15:59.000000 ElasticEmail-4.0.24/ElasticEmail/model/new_api_key.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9041 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/new_smtp_credentials.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9041 2023-11-27 14:16:00.000000 ElasticEmail-4.0.24/ElasticEmail/model/new_smtp_credentials.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6877 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/options.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6877 2023-11-27 14:16:00.000000 ElasticEmail-4.0.24/ElasticEmail/model/options.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10694 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/recipient_event.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10694 2023-11-27 14:16:00.000000 ElasticEmail-4.0.24/ElasticEmail/model/recipient_event.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3678 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/segment.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3678 2023-11-27 14:16:00.000000 ElasticEmail-4.0.24/ElasticEmail/model/segment.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3659 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/segment_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3659 2023-11-27 14:16:01.000000 ElasticEmail-4.0.24/ElasticEmail/model/segment_payload.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8521 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/smtp_credentials.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8521 2023-11-27 14:16:01.000000 ElasticEmail-4.0.24/ElasticEmail/model/smtp_credentials.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6614 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/smtp_credentials_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6614 2023-11-27 14:16:01.000000 ElasticEmail-4.0.24/ElasticEmail/model/smtp_credentials_payload.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4009 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/sort_order_item.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4009 2023-11-27 14:16:01.000000 ElasticEmail-4.0.24/ElasticEmail/model/sort_order_item.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1844 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/split_optimization_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1719 2023-11-27 14:16:02.000000 ElasticEmail-4.0.24/ElasticEmail/model/split_optimization_type.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4153 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/split_options.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4153 2023-11-27 14:16:02.000000 ElasticEmail-4.0.24/ElasticEmail/model/split_options.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8220 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/sub_account_info.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8220 2023-11-27 14:16:02.000000 ElasticEmail-4.0.24/ElasticEmail/model/sub_account_info.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3845 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/subaccount_email_credits_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3845 2023-11-27 14:16:02.000000 ElasticEmail-4.0.24/ElasticEmail/model/subaccount_email_credits_payload.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8645 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/subaccount_email_settings.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8645 2023-11-27 14:16:02.000000 ElasticEmail-4.0.24/ElasticEmail/model/subaccount_email_settings.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     7953 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/subaccount_email_settings_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     7953 2023-11-27 14:16:03.000000 ElasticEmail-4.0.24/ElasticEmail/model/subaccount_email_settings_payload.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5137 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/subaccount_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5137 2023-11-27 14:16:03.000000 ElasticEmail-4.0.24/ElasticEmail/model/subaccount_payload.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3392 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/subaccount_settings_info.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3392 2023-11-27 14:16:03.000000 ElasticEmail-4.0.24/ElasticEmail/model/subaccount_settings_info.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3456 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/subaccount_settings_info_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3456 2023-11-27 14:16:03.000000 ElasticEmail-4.0.24/ElasticEmail/model/subaccount_settings_info_payload.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6541 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/suppression.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6541 2023-11-27 14:16:03.000000 ElasticEmail-4.0.24/ElasticEmail/model/suppression.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6981 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/template.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6981 2023-11-27 14:16:03.000000 ElasticEmail-4.0.24/ElasticEmail/model/template.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5804 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/template_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5804 2023-11-27 14:16:04.000000 ElasticEmail-4.0.24/ElasticEmail/model/template_payload.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1878 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/template_scope.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1747 2023-11-27 14:16:04.000000 ElasticEmail-4.0.24/ElasticEmail/model/template_scope.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2191 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/template_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1938 2023-11-27 14:16:04.000000 ElasticEmail-4.0.24/ElasticEmail/model/template_type.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6528 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/transactional_recipient.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6528 2023-11-27 14:16:04.000000 ElasticEmail-4.0.24/ElasticEmail/model/transactional_recipient.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4777 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/utm.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4777 2023-11-27 14:16:05.000000 ElasticEmail-4.0.24/ElasticEmail/model/utm.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6447 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/verification_file_result.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6447 2023-11-27 14:16:05.000000 ElasticEmail-4.0.24/ElasticEmail/model/verification_file_result.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8138 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/verification_file_result_details.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8138 2023-11-27 14:16:05.000000 ElasticEmail-4.0.24/ElasticEmail/model/verification_file_result_details.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2207 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/model/verification_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1974 2023-11-27 14:16:05.000000 ElasticEmail-4.0.24/ElasticEmail/model/verification_status.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    83360 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/ElasticEmail/model_utils.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.172720 ElasticEmail-4.0.24/ElasticEmail/models/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5783 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/models/__init__.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.172720 ElasticEmail-4.0.24/ElasticEmail/paths/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3296 2023-11-27 14:16:39.000000 ElasticEmail-4.0.24/ElasticEmail/paths/__init__.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.176720 ElasticEmail-4.0.24/ElasticEmail/paths/campaigns/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      301 2023-11-27 14:16:08.000000 ElasticEmail-4.0.24/ElasticEmail/paths/campaigns/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10998 2023-11-27 14:16:08.000000 ElasticEmail-4.0.24/ElasticEmail/paths/campaigns/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10891 2023-11-27 14:16:08.000000 ElasticEmail-4.0.24/ElasticEmail/paths/campaigns/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11416 2023-11-27 14:16:08.000000 ElasticEmail-4.0.24/ElasticEmail/paths/campaigns/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11309 2023-11-27 14:16:08.000000 ElasticEmail-4.0.24/ElasticEmail/paths/campaigns/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.180720 ElasticEmail-4.0.24/ElasticEmail/paths/campaigns_name/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      311 2023-11-27 14:16:08.000000 ElasticEmail-4.0.24/ElasticEmail/paths/campaigns_name/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8138 2023-11-27 14:16:07.000000 ElasticEmail-4.0.24/ElasticEmail/paths/campaigns_name/delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8031 2023-11-27 14:16:07.000000 ElasticEmail-4.0.24/ElasticEmail/paths/campaigns_name/delete.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9716 2023-11-27 14:16:07.000000 ElasticEmail-4.0.24/ElasticEmail/paths/campaigns_name/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9609 2023-11-27 14:16:07.000000 ElasticEmail-4.0.24/ElasticEmail/paths/campaigns_name/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13663 2023-11-27 14:16:07.000000 ElasticEmail-4.0.24/ElasticEmail/paths/campaigns_name/put.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13556 2023-11-27 14:16:07.000000 ElasticEmail-4.0.24/ElasticEmail/paths/campaigns_name/put.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.184720 ElasticEmail-4.0.24/ElasticEmail/paths/contacts/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      299 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10703 2023-11-27 14:16:11.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10596 2023-11-27 14:16:11.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    15809 2023-11-27 14:16:11.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    15702 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.188720 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_delete/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      313 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_delete/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9832 2023-11-27 14:16:10.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_delete/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9725 2023-11-27 14:16:10.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_delete/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.192720 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_email/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      311 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_email/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8144 2023-11-27 14:16:09.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_email/delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8037 2023-11-27 14:16:09.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_email/delete.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9719 2023-11-27 14:16:09.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_email/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9612 2023-11-27 14:16:09.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_email/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13781 2023-11-27 14:16:09.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_email/put.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13674 2023-11-27 14:16:10.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_email/put.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.196720 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_export/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      313 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_export/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11800 2023-11-27 14:16:10.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_export/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11693 2023-11-27 14:16:10.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_export/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.196720 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_export_id_status/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      333 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_export_id_status/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9840 2023-11-27 14:16:10.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_export_id_status/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9733 2023-11-27 14:16:10.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_export_id_status/get.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.196720 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_import/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      313 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_import/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    15223 2023-11-27 14:16:11.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_import/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    15116 2023-11-27 14:16:11.000000 ElasticEmail-4.0.24/ElasticEmail/paths/contacts_import/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.200720 ElasticEmail-4.0.24/ElasticEmail/paths/emails/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      295 2023-11-27 14:16:14.000000 ElasticEmail-4.0.24/ElasticEmail/paths/emails/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11480 2023-11-27 14:16:13.000000 ElasticEmail-4.0.24/ElasticEmail/paths/emails/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11373 2023-11-27 14:16:13.000000 ElasticEmail-4.0.24/ElasticEmail/paths/emails/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.200720 ElasticEmail-4.0.24/ElasticEmail/paths/emails_mergefile/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      315 2023-11-27 14:16:14.000000 ElasticEmail-4.0.24/ElasticEmail/paths/emails_mergefile/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11618 2023-11-27 14:16:13.000000 ElasticEmail-4.0.24/ElasticEmail/paths/emails_mergefile/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11511 2023-11-27 14:16:13.000000 ElasticEmail-4.0.24/ElasticEmail/paths/emails_mergefile/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.204720 ElasticEmail-4.0.24/ElasticEmail/paths/emails_msgid_view/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      317 2023-11-27 14:16:14.000000 ElasticEmail-4.0.24/ElasticEmail/paths/emails_msgid_view/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9756 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/ElasticEmail/paths/emails_msgid_view/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9649 2023-11-27 14:16:13.000000 ElasticEmail-4.0.24/ElasticEmail/paths/emails_msgid_view/get.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.204720 ElasticEmail-4.0.24/ElasticEmail/paths/emails_transactional/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      323 2023-11-27 14:16:14.000000 ElasticEmail-4.0.24/ElasticEmail/paths/emails_transactional/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11737 2023-11-27 14:16:13.000000 ElasticEmail-4.0.24/ElasticEmail/paths/emails_transactional/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11630 2023-11-27 14:16:14.000000 ElasticEmail-4.0.24/ElasticEmail/paths/emails_transactional/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.208720 ElasticEmail-4.0.24/ElasticEmail/paths/events/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      295 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/ElasticEmail/paths/events/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13477 2023-11-27 14:16:16.000000 ElasticEmail-4.0.24/ElasticEmail/paths/events/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13370 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/ElasticEmail/paths/events/get.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.208720 ElasticEmail-4.0.24/ElasticEmail/paths/events_channels_export_id_status/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      347 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/ElasticEmail/paths/events_channels_export_id_status/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9924 2023-11-27 14:16:15.000000 ElasticEmail-4.0.24/ElasticEmail/paths/events_channels_export_id_status/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9817 2023-11-27 14:16:15.000000 ElasticEmail-4.0.24/ElasticEmail/paths/events_channels_export_id_status/get.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.212720 ElasticEmail-4.0.24/ElasticEmail/paths/events_channels_name/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      323 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/ElasticEmail/paths/events_channels_name/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    15633 2023-11-27 14:16:15.000000 ElasticEmail-4.0.24/ElasticEmail/paths/events_channels_name/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    15526 2023-11-27 14:16:15.000000 ElasticEmail-4.0.24/ElasticEmail/paths/events_channels_name/get.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.216719 ElasticEmail-4.0.24/ElasticEmail/paths/events_channels_name_export/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      337 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/ElasticEmail/paths/events_channels_name_export/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    15258 2023-11-27 14:16:14.000000 ElasticEmail-4.0.24/ElasticEmail/paths/events_channels_name_export/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    15151 2023-11-27 14:16:14.000000 ElasticEmail-4.0.24/ElasticEmail/paths/events_channels_name_export/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.216719 ElasticEmail-4.0.24/ElasticEmail/paths/events_export/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      309 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/ElasticEmail/paths/events_export/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13102 2023-11-27 14:16:16.000000 ElasticEmail-4.0.24/ElasticEmail/paths/events_export/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12995 2023-11-27 14:16:16.000000 ElasticEmail-4.0.24/ElasticEmail/paths/events_export/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.220719 ElasticEmail-4.0.24/ElasticEmail/paths/events_export_id_status/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      329 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/ElasticEmail/paths/events_export_id_status/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9818 2023-11-27 14:16:15.000000 ElasticEmail-4.0.24/ElasticEmail/paths/events_export_id_status/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9711 2023-11-27 14:16:15.000000 ElasticEmail-4.0.24/ElasticEmail/paths/events_export_id_status/get.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.220719 ElasticEmail-4.0.24/ElasticEmail/paths/events_transactionid/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      323 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/ElasticEmail/paths/events_transactionid/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    14762 2023-11-27 14:16:14.000000 ElasticEmail-4.0.24/ElasticEmail/paths/events_transactionid/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    14655 2023-11-27 14:16:14.000000 ElasticEmail-4.0.24/ElasticEmail/paths/events_transactionid/get.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.224719 ElasticEmail-4.0.24/ElasticEmail/paths/files/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      293 2023-11-27 14:16:19.000000 ElasticEmail-4.0.24/ElasticEmail/paths/files/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10675 2023-11-27 14:16:18.000000 ElasticEmail-4.0.24/ElasticEmail/paths/files/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10568 2023-11-27 14:16:19.000000 ElasticEmail-4.0.24/ElasticEmail/paths/files/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    14360 2023-11-27 14:16:19.000000 ElasticEmail-4.0.24/ElasticEmail/paths/files/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    14253 2023-11-27 14:16:19.000000 ElasticEmail-4.0.24/ElasticEmail/paths/files/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.228719 ElasticEmail-4.0.24/ElasticEmail/paths/files_name/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      303 2023-11-27 14:16:19.000000 ElasticEmail-4.0.24/ElasticEmail/paths/files_name/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8090 2023-11-27 14:16:18.000000 ElasticEmail-4.0.24/ElasticEmail/paths/files_name/delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     7983 2023-11-27 14:16:18.000000 ElasticEmail-4.0.24/ElasticEmail/paths/files_name/delete.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9616 2023-11-27 14:16:18.000000 ElasticEmail-4.0.24/ElasticEmail/paths/files_name/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9509 2023-11-27 14:16:18.000000 ElasticEmail-4.0.24/ElasticEmail/paths/files_name/get.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.228719 ElasticEmail-4.0.24/ElasticEmail/paths/files_name_info/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      313 2023-11-27 14:16:19.000000 ElasticEmail-4.0.24/ElasticEmail/paths/files_name_info/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9731 2023-11-27 14:16:18.000000 ElasticEmail-4.0.24/ElasticEmail/paths/files_name_info/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9624 2023-11-27 14:16:18.000000 ElasticEmail-4.0.24/ElasticEmail/paths/files_name_info/get.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.232719 ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      307 2023-11-27 14:16:21.000000 ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8319 2023-11-27 14:16:20.000000 ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8212 2023-11-27 14:16:20.000000 ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11550 2023-11-27 14:16:21.000000 ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11443 2023-11-27 14:16:21.000000 ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.236719 ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute_id/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      313 2023-11-27 14:16:21.000000 ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute_id/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8132 2023-11-27 14:16:19.000000 ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute_id/delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8025 2023-11-27 14:16:19.000000 ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute_id/delete.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9722 2023-11-27 14:16:19.000000 ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute_id/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9615 2023-11-27 14:16:20.000000 ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute_id/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13754 2023-11-27 14:16:20.000000 ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute_id/put.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13647 2023-11-27 14:16:20.000000 ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute_id/put.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.236719 ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute_order/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      319 2023-11-27 14:16:21.000000 ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute_order/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13022 2023-11-27 14:16:20.000000 ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute_order/put.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12915 2023-11-27 14:16:21.000000 ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute_order/put.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.240719 ElasticEmail-4.0.24/ElasticEmail/paths/lists/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      293 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/ElasticEmail/paths/lists/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10703 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/ElasticEmail/paths/lists/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10596 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/ElasticEmail/paths/lists/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11440 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/ElasticEmail/paths/lists/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11333 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/ElasticEmail/paths/lists/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.244719 ElasticEmail-4.0.24/ElasticEmail/paths/lists_name/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      303 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/ElasticEmail/paths/lists_name/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8090 2023-11-27 14:16:22.000000 ElasticEmail-4.0.24/ElasticEmail/paths/lists_name/delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     7983 2023-11-27 14:16:22.000000 ElasticEmail-4.0.24/ElasticEmail/paths/lists_name/delete.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9681 2023-11-27 14:16:22.000000 ElasticEmail-4.0.24/ElasticEmail/paths/lists_name/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9574 2023-11-27 14:16:22.000000 ElasticEmail-4.0.24/ElasticEmail/paths/lists_name/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13720 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/ElasticEmail/paths/lists_name/put.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13613 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/ElasticEmail/paths/lists_name/put.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.248719 ElasticEmail-4.0.24/ElasticEmail/paths/lists_name_contacts/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      321 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/ElasticEmail/paths/lists_name_contacts/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13842 2023-11-27 14:16:21.000000 ElasticEmail-4.0.24/ElasticEmail/paths/lists_name_contacts/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13735 2023-11-27 14:16:21.000000 ElasticEmail-4.0.24/ElasticEmail/paths/lists_name_contacts/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.248719 ElasticEmail-4.0.24/ElasticEmail/paths/lists_name_contacts_remove/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      335 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/ElasticEmail/paths/lists_name_contacts_remove/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12178 2023-11-27 14:16:22.000000 ElasticEmail-4.0.24/ElasticEmail/paths/lists_name_contacts_remove/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12071 2023-11-27 14:16:22.000000 ElasticEmail-4.0.24/ElasticEmail/paths/lists_name_contacts_remove/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.252719 ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      315 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10504 2023-11-27 14:16:25.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10397 2023-11-27 14:16:25.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11589 2023-11-27 14:16:25.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11482 2023-11-27 14:16:25.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.260719 ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys_name/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      325 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys_name/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10394 2023-11-27 14:16:24.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys_name/delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10287 2023-11-27 14:16:24.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys_name/delete.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11967 2023-11-27 14:16:24.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys_name/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11860 2023-11-27 14:16:24.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys_name/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13826 2023-11-27 14:16:24.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys_name/put.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13719 2023-11-27 14:16:24.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys_name/put.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.264719 ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      309 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10543 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10436 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11631 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11524 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.268719 ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp_name/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      319 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp_name/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10370 2023-11-27 14:16:25.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp_name/delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10263 2023-11-27 14:16:25.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp_name/delete.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11970 2023-11-27 14:16:25.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp_name/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11863 2023-11-27 14:16:25.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp_name/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13868 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp_name/put.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13761 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp_name/put.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.272719 ElasticEmail-4.0.24/ElasticEmail/paths/segments/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      299 2023-11-27 14:16:28.000000 ElasticEmail-4.0.24/ElasticEmail/paths/segments/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10703 2023-11-27 14:16:27.000000 ElasticEmail-4.0.24/ElasticEmail/paths/segments/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10596 2023-11-27 14:16:28.000000 ElasticEmail-4.0.24/ElasticEmail/paths/segments/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11481 2023-11-27 14:16:28.000000 ElasticEmail-4.0.24/ElasticEmail/paths/segments/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11374 2023-11-27 14:16:28.000000 ElasticEmail-4.0.24/ElasticEmail/paths/segments/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.280719 ElasticEmail-4.0.24/ElasticEmail/paths/segments_name/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      309 2023-11-27 14:16:28.000000 ElasticEmail-4.0.24/ElasticEmail/paths/segments_name/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8126 2023-11-27 14:16:27.000000 ElasticEmail-4.0.24/ElasticEmail/paths/segments_name/delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8019 2023-11-27 14:16:27.000000 ElasticEmail-4.0.24/ElasticEmail/paths/segments_name/delete.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9701 2023-11-27 14:16:27.000000 ElasticEmail-4.0.24/ElasticEmail/paths/segments_name/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9594 2023-11-27 14:16:27.000000 ElasticEmail-4.0.24/ElasticEmail/paths/segments_name/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13728 2023-11-27 14:16:27.000000 ElasticEmail-4.0.24/ElasticEmail/paths/segments_name/put.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13621 2023-11-27 14:16:27.000000 ElasticEmail-4.0.24/ElasticEmail/paths/segments_name/put.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.280719 ElasticEmail-4.0.24/ElasticEmail/paths/statistics/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      303 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/ElasticEmail/paths/statistics/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10616 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/ElasticEmail/paths/statistics/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10509 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/ElasticEmail/paths/statistics/get.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.280719 ElasticEmail-4.0.24/ElasticEmail/paths/statistics_campaigns/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      323 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/ElasticEmail/paths/statistics_campaigns/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10956 2023-11-27 14:16:28.000000 ElasticEmail-4.0.24/ElasticEmail/paths/statistics_campaigns/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10849 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/ElasticEmail/paths/statistics_campaigns/get.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.284719 ElasticEmail-4.0.24/ElasticEmail/paths/statistics_campaigns_name/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      333 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/ElasticEmail/paths/statistics_campaigns_name/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9890 2023-11-27 14:16:28.000000 ElasticEmail-4.0.24/ElasticEmail/paths/statistics_campaigns_name/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9783 2023-11-27 14:16:28.000000 ElasticEmail-4.0.24/ElasticEmail/paths/statistics_campaigns_name/get.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.284719 ElasticEmail-4.0.24/ElasticEmail/paths/statistics_channels/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      321 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/ElasticEmail/paths/statistics_channels/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10944 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/ElasticEmail/paths/statistics_channels/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10837 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/ElasticEmail/paths/statistics_channels/get.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.288719 ElasticEmail-4.0.24/ElasticEmail/paths/statistics_channels_name/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      331 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/ElasticEmail/paths/statistics_channels_name/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9878 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/ElasticEmail/paths/statistics_channels_name/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9771 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/ElasticEmail/paths/statistics_channels_name/get.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.292719 ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      305 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10790 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10683 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11561 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11454 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.292719 ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts_email/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      317 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts_email/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8180 2023-11-27 14:16:30.000000 ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts_email/delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8073 2023-11-27 14:16:30.000000 ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts_email/delete.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9778 2023-11-27 14:16:30.000000 ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts_email/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9671 2023-11-27 14:16:30.000000 ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts_email/get.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.296719 ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts_email_credits/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      333 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts_email_credits/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12281 2023-11-27 14:16:30.000000 ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts_email_credits/patch.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12174 2023-11-27 14:16:30.000000 ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts_email_credits/patch.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.296719 ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts_email_settings_email/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      347 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts_email_settings_email/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    14015 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts_email_settings_email/put.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13908 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts_email_settings_email/put.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.300719 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      307 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10778 2023-11-27 14:16:34.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10671 2023-11-27 14:16:34.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions/get.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.304719 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_bounces/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      323 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_bounces/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11140 2023-11-27 14:16:32.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_bounces/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11033 2023-11-27 14:16:32.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_bounces/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12946 2023-11-27 14:16:32.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_bounces/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12839 2023-11-27 14:16:32.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_bounces/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.304719 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_bounces_import/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      337 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_bounces_import/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12401 2023-11-27 14:16:32.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_bounces_import/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12294 2023-11-27 14:16:32.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_bounces_import/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.308719 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_complaints/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      329 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_complaints/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11177 2023-11-27 14:16:33.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_complaints/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11070 2023-11-27 14:16:33.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_complaints/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12988 2023-11-27 14:16:33.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_complaints/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12881 2023-11-27 14:16:34.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_complaints/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.312719 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_complaints_import/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      343 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_complaints_import/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12443 2023-11-27 14:16:33.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_complaints_import/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12336 2023-11-27 14:16:33.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_complaints_import/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.312719 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_email/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      319 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_email/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8192 2023-11-27 14:16:32.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_email/delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8085 2023-11-27 14:16:33.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_email/delete.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9778 2023-11-27 14:16:33.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_email/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9671 2023-11-27 14:16:33.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_email/get.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.316719 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_unsubscribes/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      333 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_unsubscribes/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11201 2023-11-27 14:16:34.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_unsubscribes/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11094 2023-11-27 14:16:34.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_unsubscribes/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13016 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_unsubscribes/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12909 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_unsubscribes/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.320719 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_unsubscribes_import/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      347 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_unsubscribes_import/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12471 2023-11-27 14:16:34.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_unsubscribes_import/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12364 2023-11-27 14:16:34.000000 ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_unsubscribes_import/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.324719 ElasticEmail-4.0.24/ElasticEmail/paths/templates/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      301 2023-11-27 14:16:37.000000 ElasticEmail-4.0.24/ElasticEmail/paths/templates/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12672 2023-11-27 14:16:36.000000 ElasticEmail-4.0.24/ElasticEmail/paths/templates/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12565 2023-11-27 14:16:37.000000 ElasticEmail-4.0.24/ElasticEmail/paths/templates/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11503 2023-11-27 14:16:37.000000 ElasticEmail-4.0.24/ElasticEmail/paths/templates/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11396 2023-11-27 14:16:37.000000 ElasticEmail-4.0.24/ElasticEmail/paths/templates/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.328719 ElasticEmail-4.0.24/ElasticEmail/paths/templates_name/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      311 2023-11-27 14:16:37.000000 ElasticEmail-4.0.24/ElasticEmail/paths/templates_name/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8138 2023-11-27 14:16:36.000000 ElasticEmail-4.0.24/ElasticEmail/paths/templates_name/delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8031 2023-11-27 14:16:36.000000 ElasticEmail-4.0.24/ElasticEmail/paths/templates_name/delete.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9716 2023-11-27 14:16:36.000000 ElasticEmail-4.0.24/ElasticEmail/paths/templates_name/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9609 2023-11-27 14:16:36.000000 ElasticEmail-4.0.24/ElasticEmail/paths/templates_name/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13750 2023-11-27 14:16:36.000000 ElasticEmail-4.0.24/ElasticEmail/paths/templates_name/put.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13643 2023-11-27 14:16:36.000000 ElasticEmail-4.0.24/ElasticEmail/paths/templates_name/put.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.328719 ElasticEmail-4.0.24/ElasticEmail/paths/verifications/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      309 2023-11-27 14:16:39.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10876 2023-11-27 14:16:39.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10769 2023-11-27 14:16:39.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications/get.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.332718 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_email/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      321 2023-11-27 14:16:39.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_email/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8217 2023-11-27 14:16:37.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_email/delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8110 2023-11-27 14:16:37.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_email/delete.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9835 2023-11-27 14:16:38.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_email/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9728 2023-11-27 14:16:38.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_email/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9835 2023-11-27 14:16:38.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_email/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9728 2023-11-27 14:16:38.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_email/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.336718 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      321 2023-11-27 14:16:39.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    14095 2023-11-27 14:16:39.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13988 2023-11-27 14:16:39.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.340718 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      327 2023-11-27 14:16:39.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8227 2023-11-27 14:16:38.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id/delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8120 2023-11-27 14:16:38.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id/delete.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.344718 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id_result/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      341 2023-11-27 14:16:39.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id_result/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12416 2023-11-27 14:16:38.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id_result/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12309 2023-11-27 14:16:39.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id_result/get.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.344718 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id_result_download/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      359 2023-11-27 14:16:39.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id_result_download/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9927 2023-11-27 14:16:38.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id_result_download/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9820 2023-11-27 14:16:38.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id_result_download/get.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.348718 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id_verification/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      353 2023-11-27 14:16:39.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id_verification/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8322 2023-11-27 14:16:39.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id_verification/post.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8215 2023-11-27 14:16:39.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id_verification/post.pyi
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.348718 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_result/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      335 2023-11-27 14:16:39.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_result/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8562 2023-11-27 14:16:39.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_result/get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8455 2023-11-27 14:16:39.000000 ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_result/get.pyi
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11308 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/rest.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    98414 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/ElasticEmail/schemas.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.616716 ElasticEmail-4.0.24/ElasticEmail.egg-info/
--rw-r--r--   0 radzaw    (1000) radzaw    (1000)    31833 2023-11-27 14:16:49.000000 ElasticEmail-4.0.24/ElasticEmail.egg-info/PKG-INFO
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    37803 2023-11-27 14:16:49.000000 ElasticEmail-4.0.24/ElasticEmail.egg-info/SOURCES.txt
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        1 2023-11-27 14:16:49.000000 ElasticEmail-4.0.24/ElasticEmail.egg-info/dependency_links.txt
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)       32 2023-11-27 14:16:49.000000 ElasticEmail-4.0.24/ElasticEmail.egg-info/requires.txt
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)       18 2023-11-27 14:16:49.000000 ElasticEmail-4.0.24/ElasticEmail.egg-info/top_level.txt
--rw-r--r--   0 radzaw    (1000) radzaw    (1000)    31833 2023-11-27 14:16:50.616716 ElasticEmail-4.0.24/PKG-INFO
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    31481 2023-11-27 14:16:42.000000 ElasticEmail-4.0.24/README.md
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)       69 2023-11-27 14:16:50.620716 ElasticEmail-4.0.24/setup.cfg
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2189 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/setup.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.424718 ElasticEmail-4.0.24/test/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1365 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_access_level.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1408 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_account_status_enum.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1425 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_api_key.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1475 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_api_key_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1394 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_body_content_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1344 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_body_part.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1458 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_campaign.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1393 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_campaign_options.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1407 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_campaign_recipient.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1386 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_campaign_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1400 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_campaign_template.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1943 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_campaigns_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1451 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_channel_log_status_summary.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1407 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_compression_format.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1365 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_consent_data.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1393 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_consent_tracking.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1431 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_contact.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1393 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_contact_activity.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1430 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_contact_hist_event_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1386 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_contact_history.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1481 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_contact_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1379 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_contact_source.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1379 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_contact_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1429 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_contact_update_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2737 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_contacts_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1372 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_contacts_list.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1457 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_delivery_optimization_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1574 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_email_content.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1434 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_email_data.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1508 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_email_message_data.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1386 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_email_recipient.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1351 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_email_send.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1365 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_email_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1493 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_email_transactional_message_data.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1572 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_email_validation_result.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1436 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_email_validation_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1351 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_email_view.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1808 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_emails_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1379 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_emails_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1372 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_encoding_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1351 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_event_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2366 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_events_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1380 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_events_order_by.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1408 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_export_file_formats.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1358 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_export_link.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1372 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_export_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1344 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_file_info.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1365 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_file_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1401 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_file_upload_result.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1886 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_files_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1386 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_inbound_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1372 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_inbound_route.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1444 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_inbound_route_action_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2118 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_inbound_route_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1444 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_inbound_route_filter_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1365 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_list_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1408 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_list_update_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2224 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_lists_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1373 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_log_job_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1401 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_log_status_summary.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1408 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_merge_email_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1407 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_message_attachment.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1393 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_message_category.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.496717 ElasticEmail-4.0.24/test/test_models/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/test/test_models/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1312 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_access_level.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1337 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_account_status_enum.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1292 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_api_key.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1321 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_api_key_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1329 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_body_content_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1300 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_body_part.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1299 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_campaign.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1328 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_campaign_options.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1336 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_campaign_recipient.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1324 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_campaign_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1332 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_campaign_template.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1362 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_channel_log_status_summary.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1336 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_compression_format.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1312 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_consent_data.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1328 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_consent_tracking.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1295 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_contact.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1328 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_contact_activity.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1324 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_contact_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1320 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_contact_source.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1320 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_contact_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1349 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_contact_update_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1316 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_contacts_list.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1365 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_delivery_optimization_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1316 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_email_content.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1304 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_email_data.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1333 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_email_message_data.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1390 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_email_predicted_validation_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1324 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_email_recipient.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1304 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_email_send.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1312 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_email_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1386 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_email_transactional_message_data.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1353 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_email_validation_result.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1353 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_email_validation_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1304 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_email_view.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1320 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_emails_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1316 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_encoding_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1304 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_event_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1321 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_events_order_by.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1337 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_export_file_formats.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1308 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_export_link.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1316 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_export_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1300 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_file_info.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1312 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_file_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1333 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_file_upload_result.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1324 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_inbound_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1316 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_inbound_route.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1358 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_inbound_route_action_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1358 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_inbound_route_filter_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1312 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_list_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1337 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_list_update_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1317 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_log_job_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1333 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_log_status_summary.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1337 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_merge_email_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1336 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_message_attachment.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1328 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_message_category.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1305 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_new_api_key.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1341 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_new_smtp_credentials.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1295 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_options.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1324 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_recipient_event.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1295 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_segment.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1324 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_segment_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1328 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_smtp_credentials.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1357 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_smtp_credentials_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1321 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_sort_order_item.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1353 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_split_optimization_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1316 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_split_options.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1325 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_sub_account_info.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1386 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_subaccount_email_credits_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1361 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_subaccount_email_settings.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1390 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_subaccount_email_settings_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1336 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_subaccount_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1357 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_subaccount_settings_info.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1386 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_subaccount_settings_info_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1311 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_suppression.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1299 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_template.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1328 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_template_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1320 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_template_scope.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1316 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_template_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1356 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_transactional_recipient.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1279 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_utm.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1357 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_verification_file_result.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1386 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_verification_file_result_details.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1340 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_models/test_verification_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1447 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_new_api_key.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1415 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_new_smtp_credentials.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1336 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_options.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.496717 ElasticEmail-4.0.24/test/test_paths/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1995 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/test/test_paths/__init__.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.500717 ElasticEmail-4.0.24/test/test_paths/test_campaigns/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:08.000000 ElasticEmail-4.0.24/test/test_paths/test_campaigns/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      795 2023-11-27 14:16:08.000000 ElasticEmail-4.0.24/test/test_paths/test_campaigns/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      798 2023-11-27 14:16:08.000000 ElasticEmail-4.0.24/test/test_paths/test_campaigns/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.504717 ElasticEmail-4.0.24/test/test_paths/test_campaigns_name/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:08.000000 ElasticEmail-4.0.24/test/test_paths/test_campaigns_name/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      839 2023-11-27 14:16:08.000000 ElasticEmail-4.0.24/test/test_paths/test_campaigns_name/test_delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      807 2023-11-27 14:16:08.000000 ElasticEmail-4.0.24/test/test_paths/test_campaigns_name/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      811 2023-11-27 14:16:08.000000 ElasticEmail-4.0.24/test/test_paths/test_campaigns_name/test_put.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.504717 ElasticEmail-4.0.24/test/test_paths/test_contacts/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/test/test_paths/test_contacts/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      791 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/test/test_paths/test_contacts/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      794 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/test/test_paths/test_contacts/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.508717 ElasticEmail-4.0.24/test/test_paths/test_contacts_delete/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/test/test_paths/test_contacts_delete/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      843 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/test/test_paths/test_contacts_delete/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.508717 ElasticEmail-4.0.24/test/test_paths/test_contacts_email/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/test/test_paths/test_contacts_email/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      838 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/test/test_paths/test_contacts_email/test_delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      806 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/test/test_paths/test_contacts_email/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      810 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/test/test_paths/test_contacts_email/test_put.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.512717 ElasticEmail-4.0.24/test/test_paths/test_contacts_export/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/test/test_paths/test_contacts_export/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      815 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/test/test_paths/test_contacts_export/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.512717 ElasticEmail-4.0.24/test/test_paths/test_contacts_export_id_status/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/test/test_paths/test_contacts_export_id_status/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      842 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/test/test_paths/test_contacts_export_id_status/test_get.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.512717 ElasticEmail-4.0.24/test/test_paths/test_contacts_import/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/test/test_paths/test_contacts_import/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      836 2023-11-27 14:16:12.000000 ElasticEmail-4.0.24/test/test_paths/test_contacts_import/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.516717 ElasticEmail-4.0.24/test/test_paths/test_emails/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:14.000000 ElasticEmail-4.0.24/test/test_paths/test_emails/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      793 2023-11-27 14:16:14.000000 ElasticEmail-4.0.24/test/test_paths/test_emails/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.516717 ElasticEmail-4.0.24/test/test_paths/test_emails_mergefile/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:14.000000 ElasticEmail-4.0.24/test/test_paths/test_emails_mergefile/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      825 2023-11-27 14:16:14.000000 ElasticEmail-4.0.24/test/test_paths/test_emails_mergefile/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.520717 ElasticEmail-4.0.24/test/test_paths/test_emails_msgid_view/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:14.000000 ElasticEmail-4.0.24/test/test_paths/test_emails_msgid_view/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      811 2023-11-27 14:16:14.000000 ElasticEmail-4.0.24/test/test_paths/test_emails_msgid_view/test_get.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.520717 ElasticEmail-4.0.24/test/test_paths/test_emails_transactional/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:14.000000 ElasticEmail-4.0.24/test/test_paths/test_emails_transactional/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      841 2023-11-27 14:16:14.000000 ElasticEmail-4.0.24/test/test_paths/test_emails_transactional/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.520717 ElasticEmail-4.0.24/test/test_paths/test_events/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/test/test_paths/test_events/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      783 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/test/test_paths/test_events/test_get.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.524717 ElasticEmail-4.0.24/test/test_paths/test_events_channels_export_id_status/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/test/test_paths/test_events_channels_export_id_status/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      869 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/test/test_paths/test_events_channels_export_id_status/test_get.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.524717 ElasticEmail-4.0.24/test/test_paths/test_events_channels_name/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/test/test_paths/test_events_channels_name/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      829 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/test/test_paths/test_events_channels_name/test_get.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.528717 ElasticEmail-4.0.24/test/test_paths/test_events_channels_name_export/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/test/test_paths/test_events_channels_name_export/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      853 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/test/test_paths/test_events_channels_name_export/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.528717 ElasticEmail-4.0.24/test/test_paths/test_events_export/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/test/test_paths/test_events_export/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      807 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/test/test_paths/test_events_export/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.528717 ElasticEmail-4.0.24/test/test_paths/test_events_export_id_status/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/test/test_paths/test_events_export_id_status/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      836 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/test/test_paths/test_events_export_id_status/test_get.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.528717 ElasticEmail-4.0.24/test/test_paths/test_events_transactionid/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/test/test_paths/test_events_transactionid/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      829 2023-11-27 14:16:17.000000 ElasticEmail-4.0.24/test/test_paths/test_events_transactionid/test_get.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.532717 ElasticEmail-4.0.24/test/test_paths/test_files/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:19.000000 ElasticEmail-4.0.24/test/test_paths/test_files/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      779 2023-11-27 14:16:19.000000 ElasticEmail-4.0.24/test/test_paths/test_files/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      785 2023-11-27 14:16:19.000000 ElasticEmail-4.0.24/test/test_paths/test_files/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.532717 ElasticEmail-4.0.24/test/test_paths/test_files_name/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:19.000000 ElasticEmail-4.0.24/test/test_paths/test_files_name/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      823 2023-11-27 14:16:19.000000 ElasticEmail-4.0.24/test/test_paths/test_files_name/test_delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      795 2023-11-27 14:16:19.000000 ElasticEmail-4.0.24/test/test_paths/test_files_name/test_get.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.536717 ElasticEmail-4.0.24/test/test_paths/test_files_name_info/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:19.000000 ElasticEmail-4.0.24/test/test_paths/test_files_name_info/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      812 2023-11-27 14:16:19.000000 ElasticEmail-4.0.24/test/test_paths/test_files_name_info/test_get.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.536717 ElasticEmail-4.0.24/test/test_paths/test_inboundroute/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:21.000000 ElasticEmail-4.0.24/test/test_paths/test_inboundroute/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      800 2023-11-27 14:16:21.000000 ElasticEmail-4.0.24/test/test_paths/test_inboundroute/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      807 2023-11-27 14:16:21.000000 ElasticEmail-4.0.24/test/test_paths/test_inboundroute/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.540717 ElasticEmail-4.0.24/test/test_paths/test_inboundroute_id/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:21.000000 ElasticEmail-4.0.24/test/test_paths/test_inboundroute_id/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      839 2023-11-27 14:16:21.000000 ElasticEmail-4.0.24/test/test_paths/test_inboundroute_id/test_delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      806 2023-11-27 14:16:21.000000 ElasticEmail-4.0.24/test/test_paths/test_inboundroute_id/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      811 2023-11-27 14:16:21.000000 ElasticEmail-4.0.24/test/test_paths/test_inboundroute_id/test_put.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.540717 ElasticEmail-4.0.24/test/test_paths/test_inboundroute_order/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:21.000000 ElasticEmail-4.0.24/test/test_paths/test_inboundroute_order/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      822 2023-11-27 14:16:21.000000 ElasticEmail-4.0.24/test/test_paths/test_inboundroute_order/test_put.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.544717 ElasticEmail-4.0.24/test/test_paths/test_lists/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/test/test_paths/test_lists/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      779 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/test/test_paths/test_lists/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      782 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/test/test_paths/test_lists/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.544717 ElasticEmail-4.0.24/test/test_paths/test_lists_name/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/test/test_paths/test_lists_name/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      823 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/test/test_paths/test_lists_name/test_delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      791 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/test/test_paths/test_lists_name/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      795 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/test/test_paths/test_lists_name/test_put.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.548717 ElasticEmail-4.0.24/test/test_paths/test_lists_name_contacts/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/test/test_paths/test_lists_name_contacts/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      832 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/test/test_paths/test_lists_name_contacts/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.548717 ElasticEmail-4.0.24/test/test_paths/test_lists_name_contacts_remove/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/test/test_paths/test_lists_name_contacts_remove/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      877 2023-11-27 14:16:23.000000 ElasticEmail-4.0.24/test/test_paths/test_lists_name_contacts_remove/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.552717 ElasticEmail-4.0.24/test/test_paths/test_security_apikeys/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/test/test_paths/test_security_apikeys/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      812 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/test/test_paths/test_security_apikeys/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      815 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/test/test_paths/test_security_apikeys/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.552717 ElasticEmail-4.0.24/test/test_paths/test_security_apikeys_name/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/test/test_paths/test_security_apikeys_name/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      856 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/test/test_paths/test_security_apikeys_name/test_delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      824 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/test/test_paths/test_security_apikeys_name/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      828 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/test/test_paths/test_security_apikeys_name/test_put.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.556717 ElasticEmail-4.0.24/test/test_paths/test_security_smtp/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/test/test_paths/test_security_smtp/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      812 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/test/test_paths/test_security_smtp/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      815 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/test/test_paths/test_security_smtp/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.560716 ElasticEmail-4.0.24/test/test_paths/test_security_smtp_name/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/test/test_paths/test_security_smtp_name/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      856 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/test/test_paths/test_security_smtp_name/test_delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      824 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/test/test_paths/test_security_smtp_name/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      828 2023-11-27 14:16:26.000000 ElasticEmail-4.0.24/test/test_paths/test_security_smtp_name/test_put.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.560716 ElasticEmail-4.0.24/test/test_paths/test_segments/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:28.000000 ElasticEmail-4.0.24/test/test_paths/test_segments/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      791 2023-11-27 14:16:28.000000 ElasticEmail-4.0.24/test/test_paths/test_segments/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      794 2023-11-27 14:16:28.000000 ElasticEmail-4.0.24/test/test_paths/test_segments/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.564716 ElasticEmail-4.0.24/test/test_paths/test_segments_name/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:28.000000 ElasticEmail-4.0.24/test/test_paths/test_segments_name/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      835 2023-11-27 14:16:28.000000 ElasticEmail-4.0.24/test/test_paths/test_segments_name/test_delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      803 2023-11-27 14:16:28.000000 ElasticEmail-4.0.24/test/test_paths/test_segments_name/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      807 2023-11-27 14:16:28.000000 ElasticEmail-4.0.24/test/test_paths/test_segments_name/test_put.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.564716 ElasticEmail-4.0.24/test/test_paths/test_statistics/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/test/test_paths/test_statistics/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      799 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/test/test_paths/test_statistics/test_get.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.564716 ElasticEmail-4.0.24/test/test_paths/test_statistics_campaigns/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/test/test_paths/test_statistics_campaigns/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      832 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/test/test_paths/test_statistics_campaigns/test_get.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.564716 ElasticEmail-4.0.24/test/test_paths/test_statistics_campaigns_name/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/test/test_paths/test_statistics_campaigns_name/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      844 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/test/test_paths/test_statistics_campaigns_name/test_get.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.568716 ElasticEmail-4.0.24/test/test_paths/test_statistics_channels/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/test/test_paths/test_statistics_channels/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      828 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/test/test_paths/test_statistics_channels/test_get.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.568716 ElasticEmail-4.0.24/test/test_paths/test_statistics_channels_name/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/test/test_paths/test_statistics_channels_name/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      840 2023-11-27 14:16:29.000000 ElasticEmail-4.0.24/test/test_paths/test_statistics_channels_name/test_get.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.572716 ElasticEmail-4.0.24/test/test_paths/test_subaccounts/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/test/test_paths/test_subaccounts/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      803 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/test/test_paths/test_subaccounts/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      806 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/test/test_paths/test_subaccounts/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.576716 ElasticEmail-4.0.24/test/test_paths/test_subaccounts_email/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/test/test_paths/test_subaccounts_email/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      850 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/test/test_paths/test_subaccounts_email/test_delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      818 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/test/test_paths/test_subaccounts_email/test_get.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.576716 ElasticEmail-4.0.24/test/test_paths/test_subaccounts_email_credits/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/test/test_paths/test_subaccounts_email_credits/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      881 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/test/test_paths/test_subaccounts_email_credits/test_patch.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.576716 ElasticEmail-4.0.24/test/test_paths/test_subaccounts_email_settings_email/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/test/test_paths/test_subaccounts_email_settings_email/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      878 2023-11-27 14:16:31.000000 ElasticEmail-4.0.24/test/test_paths/test_subaccounts_email_settings_email/test_put.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.580716 ElasticEmail-4.0.24/test/test_paths/test_suppressions/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/test/test_paths/test_suppressions/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      806 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/test/test_paths/test_suppressions/test_get.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.580716 ElasticEmail-4.0.24/test/test_paths/test_suppressions_bounces/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/test/test_paths/test_suppressions_bounces/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      827 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/test/test_paths/test_suppressions_bounces/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      828 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/test/test_paths/test_suppressions_bounces/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.584716 ElasticEmail-4.0.24/test/test_paths/test_suppressions_bounces_import/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/test/test_paths/test_suppressions_bounces_import/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      872 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/test/test_paths/test_suppressions_bounces_import/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.588716 ElasticEmail-4.0.24/test/test_paths/test_suppressions_complaints/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/test/test_paths/test_suppressions_complaints/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      840 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/test/test_paths/test_suppressions_complaints/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      840 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/test/test_paths/test_suppressions_complaints/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.588716 ElasticEmail-4.0.24/test/test_paths/test_suppressions_complaints_import/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/test/test_paths/test_suppressions_complaints_import/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      884 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/test/test_paths/test_suppressions_complaints_import/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.592716 ElasticEmail-4.0.24/test/test_paths/test_suppressions_email/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/test/test_paths/test_suppressions_email/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      854 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/test/test_paths/test_suppressions_email/test_delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      821 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/test/test_paths/test_suppressions_email/test_get.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.592716 ElasticEmail-4.0.24/test/test_paths/test_suppressions_unsubscribes/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/test/test_paths/test_suppressions_unsubscribes/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      848 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/test/test_paths/test_suppressions_unsubscribes/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      848 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/test/test_paths/test_suppressions_unsubscribes/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.596716 ElasticEmail-4.0.24/test/test_paths/test_suppressions_unsubscribes_import/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/test/test_paths/test_suppressions_unsubscribes_import/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      892 2023-11-27 14:16:35.000000 ElasticEmail-4.0.24/test/test_paths/test_suppressions_unsubscribes_import/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.596716 ElasticEmail-4.0.24/test/test_paths/test_templates/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:37.000000 ElasticEmail-4.0.24/test/test_paths/test_templates/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      795 2023-11-27 14:16:37.000000 ElasticEmail-4.0.24/test/test_paths/test_templates/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      798 2023-11-27 14:16:37.000000 ElasticEmail-4.0.24/test/test_paths/test_templates/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.600716 ElasticEmail-4.0.24/test/test_paths/test_templates_name/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:37.000000 ElasticEmail-4.0.24/test/test_paths/test_templates_name/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      839 2023-11-27 14:16:37.000000 ElasticEmail-4.0.24/test/test_paths/test_templates_name/test_delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      807 2023-11-27 14:16:37.000000 ElasticEmail-4.0.24/test/test_paths/test_templates_name/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      811 2023-11-27 14:16:37.000000 ElasticEmail-4.0.24/test/test_paths/test_templates_name/test_put.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.604716 ElasticEmail-4.0.24/test/test_paths/test_verifications/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/test/test_paths/test_verifications/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      824 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/test/test_paths/test_verifications/test_get.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.604716 ElasticEmail-4.0.24/test/test_paths/test_verifications_email/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/test/test_paths/test_verifications_email/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      871 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/test/test_paths/test_verifications_email/test_delete.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      838 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/test/test_paths/test_verifications_email/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      824 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/test/test_paths/test_verifications_email/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.608716 ElasticEmail-4.0.24/test/test_paths/test_verifications_files/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/test/test_paths/test_verifications_files/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      835 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/test/test_paths/test_verifications_files/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.608716 ElasticEmail-4.0.24/test/test_paths/test_verifications_files_id/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/test/test_paths/test_verifications_files_id/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      877 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/test/test_paths/test_verifications_files_id/test_delete.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.608716 ElasticEmail-4.0.24/test/test_paths/test_verifications_files_id_result/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/test/test_paths/test_verifications_files_id_result/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      872 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/test/test_paths/test_verifications_files_id_result/test_get.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.612716 ElasticEmail-4.0.24/test/test_paths/test_verifications_files_id_result_download/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/test/test_paths/test_verifications_files_id_result_download/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      893 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/test/test_paths/test_verifications_files_id_result_download/test_get.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.612716 ElasticEmail-4.0.24/test/test_paths/test_verifications_files_id_verification/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/test/test_paths/test_verifications_files_id_verification/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      895 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/test/test_paths/test_verifications_files_id_verification/test_post.py
-drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:50.616716 ElasticEmail-4.0.24/test/test_paths/test_verifications_files_result/
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/test/test_paths/test_verifications_files_result/__init__.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      858 2023-11-27 14:16:40.000000 ElasticEmail-4.0.24/test/test_paths/test_verifications_files_result/test_get.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1386 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_recipient_event.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2813 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_security_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1336 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_segment.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1386 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_segment_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1923 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_segments_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1393 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_smtp_credentials.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1443 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_smtp_credentials_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1380 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_sort_order_item.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1436 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_split_optimization_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1372 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_split_options.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2032 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_statistics_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1387 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_sub_account_info.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2227 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_sub_accounts_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1493 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_subaccount_email_credits_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1450 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_subaccount_email_settings.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1500 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_subaccount_email_settings_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1407 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_subaccount_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1443 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_subaccount_settings_info.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1493 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_subaccount_settings_info_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1364 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_suppression.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3258 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_suppressions_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1426 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_template.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1476 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_template_payload.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1602 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_template_scope.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1408 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_template_scope_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1372 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_template_type.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1943 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_templates_api.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1442 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_transactional_recipient.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1308 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_utm.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1443 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_verification_file_result.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1629 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_verification_file_result_details.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1414 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_verification_status.py
--rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2886 2023-11-27 14:15:36.000000 ElasticEmail-4.0.24/test/test_verifications_api.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.323182 elasticemail-4.1.0/
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:04.823186 elasticemail-4.1.0/ElasticEmail/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1503 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    59260 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/api_client.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:04.827186 elasticemail-4.1.0/ElasticEmail/apis/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      214 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/apis/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12178 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/apis/path_to_api.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:04.871185 elasticemail-4.1.0/ElasticEmail/apis/paths/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      239 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      174 2024-05-23 09:31:19.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/campaigns.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      269 2024-05-23 09:31:19.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/campaigns_name.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      171 2024-05-23 09:31:23.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/contacts.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      115 2024-05-23 09:31:23.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/contacts_delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      269 2024-05-23 09:31:23.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/contacts_email.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      115 2024-05-23 09:31:23.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/contacts_export.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      130 2024-05-23 09:31:23.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/contacts_export_id_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      115 2024-05-23 09:31:23.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/contacts_import.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)       98 2024-05-23 09:31:26.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/emails.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      117 2024-05-23 09:31:26.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/emails_mergefile.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      115 2024-05-23 09:31:26.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/emails_msgid_view.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      125 2024-05-23 09:31:26.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/emails_transactional.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      135 2024-05-23 09:31:26.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/emails_transactionid_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)       95 2024-05-23 09:31:29.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/events.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      143 2024-05-23 09:31:29.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/events_channels_export_id_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      121 2024-05-23 09:31:29.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/events_channels_name.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      137 2024-05-23 09:31:29.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/events_channels_name_export.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      111 2024-05-23 09:31:29.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/events_export.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      126 2024-05-23 09:31:29.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/events_export_id_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      122 2024-05-23 09:31:29.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/events_transactionid.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      162 2024-05-23 09:31:31.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/files.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      182 2024-05-23 09:31:31.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/files_name.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      111 2024-05-23 09:31:31.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/files_name_info.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      183 2024-05-23 09:31:34.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/inboundroute.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      273 2024-05-23 09:31:34.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/inboundroute_id.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      118 2024-05-23 09:31:34.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/inboundroute_order.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      162 2024-05-23 09:31:36.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/lists.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      253 2024-05-23 09:31:36.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/lists_name.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      122 2024-05-23 09:31:36.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/lists_name_contacts.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      135 2024-05-23 09:31:36.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/lists_name_contacts_remove.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      194 2024-05-23 09:31:39.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/security_apikeys.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      296 2024-05-23 09:31:39.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/security_apikeys_name.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      185 2024-05-23 09:31:39.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/security_smtp.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      284 2024-05-23 09:31:39.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/security_smtp_name.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      171 2024-05-23 09:31:41.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/segments.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      265 2024-05-23 09:31:41.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/segments_name.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      103 2024-05-23 09:31:42.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/statistics.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      122 2024-05-23 09:31:42.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/statistics_campaigns.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      131 2024-05-23 09:31:42.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/statistics_campaigns_name.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      120 2024-05-23 09:31:42.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/statistics_channels.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      129 2024-05-23 09:31:42.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/statistics_channels_name.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      180 2024-05-23 09:31:44.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/subaccounts.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      203 2024-05-23 09:31:44.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/subaccounts_email.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      137 2024-05-23 09:31:44.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/subaccounts_email_credits.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      144 2024-05-23 09:31:44.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/subaccounts_email_settings_email.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      107 2024-05-23 09:31:48.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/suppressions.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      206 2024-05-23 09:31:48.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/suppressions_bounces.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      138 2024-05-23 09:31:48.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/suppressions_bounces_import.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      215 2024-05-23 09:31:48.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/suppressions_complaints.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      144 2024-05-23 09:31:48.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/suppressions_complaints_import.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      206 2024-05-23 09:31:48.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/suppressions_email.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      221 2024-05-23 09:31:48.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/suppressions_unsubscribes.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      148 2024-05-23 09:31:48.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/suppressions_unsubscribes_import.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      174 2024-05-23 09:31:50.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/templates.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      269 2024-05-23 09:31:50.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/templates_name.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      109 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/verifications.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      292 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/verifications_email.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      123 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/verifications_files.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      134 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/verifications_files_id.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      138 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/verifications_files_id_result.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      155 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/verifications_files_id_result_download.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      153 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/verifications_files_id_verification.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      133 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/apis/paths/verifications_files_result.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2234 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/apis/tag_to_api.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:04.879185 elasticemail-4.1.0/ElasticEmail/apis/tags/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      671 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/apis/tags/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1623 2024-05-23 09:31:20.000000 elasticemail-4.1.0/ElasticEmail/apis/tags/campaigns_api.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2023 2024-05-23 09:31:24.000000 elasticemail-4.1.0/ElasticEmail/apis/tags/contacts_api.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1685 2024-05-23 09:31:26.000000 elasticemail-4.1.0/ElasticEmail/apis/tags/emails_api.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1941 2024-05-23 09:31:29.000000 elasticemail-4.1.0/ElasticEmail/apis/tags/events_api.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1572 2024-05-23 09:31:31.000000 elasticemail-4.1.0/ElasticEmail/apis/tags/files_api.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1754 2024-05-23 09:31:34.000000 elasticemail-4.1.0/ElasticEmail/apis/tags/inbound_route_api.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1796 2024-05-23 09:31:36.000000 elasticemail-4.1.0/ElasticEmail/apis/tags/lists_api.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2210 2024-05-23 09:31:39.000000 elasticemail-4.1.0/ElasticEmail/apis/tags/security_api.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1607 2024-05-23 09:31:41.000000 elasticemail-4.1.0/ElasticEmail/apis/tags/segments_api.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1716 2024-05-23 09:31:42.000000 elasticemail-4.1.0/ElasticEmail/apis/tags/statistics_api.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1835 2024-05-23 09:31:44.000000 elasticemail-4.1.0/ElasticEmail/apis/tags/sub_accounts_api.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2597 2024-05-23 09:31:48.000000 elasticemail-4.1.0/ElasticEmail/apis/tags/suppressions_api.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1623 2024-05-23 09:31:50.000000 elasticemail-4.1.0/ElasticEmail/apis/tags/templates_api.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2410 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/apis/tags/verifications_api.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    17319 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/configuration.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5282 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/exceptions.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:04.987184 elasticemail-4.1.0/ElasticEmail/model/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      346 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8928 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/access_level.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6481 2024-05-23 09:30:52.000000 elasticemail-4.1.0/ElasticEmail/model/access_level.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2134 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/account_status_enum.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1912 2024-05-23 09:30:53.000000 elasticemail-4.1.0/ElasticEmail/model/account_status_enum.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9345 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/api_key.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9345 2024-05-23 09:30:54.000000 elasticemail-4.1.0/ElasticEmail/model/api_key.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8113 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/api_key_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8113 2024-05-23 09:30:56.000000 elasticemail-4.1.0/ElasticEmail/model/api_key_payload.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2075 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/body_content_type.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1893 2024-05-23 09:30:57.000000 elasticemail-4.1.0/ElasticEmail/model/body_content_type.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4482 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/body_part.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4482 2024-05-23 09:30:57.000000 elasticemail-4.1.0/ElasticEmail/model/body_part.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6598 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/campaign.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6598 2024-05-23 09:30:58.000000 elasticemail-4.1.0/ElasticEmail/model/campaign.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9362 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/campaign_options.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9362 2024-05-23 09:30:58.000000 elasticemail-4.1.0/ElasticEmail/model/campaign_options.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5486 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/campaign_recipient.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5486 2024-05-23 09:30:59.000000 elasticemail-4.1.0/ElasticEmail/model/campaign_recipient.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2569 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/campaign_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2228 2024-05-23 09:30:59.000000 elasticemail-4.1.0/ElasticEmail/model/campaign_status.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     7147 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/campaign_template.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     7147 2024-05-23 09:30:59.000000 elasticemail-4.1.0/ElasticEmail/model/campaign_template.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10652 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/channel_log_status_summary.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10652 2024-05-23 09:31:00.000000 elasticemail-4.1.0/ElasticEmail/model/channel_log_status_summary.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1861 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/compression_format.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1744 2024-05-23 09:31:00.000000 elasticemail-4.1.0/ElasticEmail/model/compression_format.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5265 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/consent_data.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5265 2024-05-23 09:31:01.000000 elasticemail-4.1.0/ElasticEmail/model/consent_data.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1948 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/consent_tracking.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1793 2024-05-23 09:31:01.000000 elasticemail-4.1.0/ElasticEmail/model/consent_tracking.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11779 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/contact.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11779 2024-05-23 09:31:01.000000 elasticemail-4.1.0/ElasticEmail/model/contact.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12786 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/contact_activity.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12786 2024-05-23 09:31:02.000000 elasticemail-4.1.0/ElasticEmail/model/contact_activity.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     7251 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/contact_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     7251 2024-05-23 09:31:02.000000 elasticemail-4.1.0/ElasticEmail/model/contact_payload.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2590 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/contact_source.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2213 2024-05-23 09:31:03.000000 elasticemail-4.1.0/ElasticEmail/model/contact_source.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2724 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/contact_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2330 2024-05-23 09:31:03.000000 elasticemail-4.1.0/ElasticEmail/model/contact_status.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5502 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/contact_update_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5502 2024-05-23 09:31:03.000000 elasticemail-4.1.0/ElasticEmail/model/contact_update_payload.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5737 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/contacts_list.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5737 2024-05-23 09:31:03.000000 elasticemail-4.1.0/ElasticEmail/model/contacts_list.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2013 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/delivery_optimization_type.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1830 2024-05-23 09:31:03.000000 elasticemail-4.1.0/ElasticEmail/model/delivery_optimization_type.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13977 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/email_content.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13977 2024-05-23 09:31:04.000000 elasticemail-4.1.0/ElasticEmail/model/email_content.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5351 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/email_data.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5351 2024-05-23 09:31:04.000000 elasticemail-4.1.0/ElasticEmail/model/email_data.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4787 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/email_job_failed_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4787 2024-05-23 09:31:05.000000 elasticemail-4.1.0/ElasticEmail/model/email_job_failed_status.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    21425 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/email_job_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    21425 2024-05-23 09:31:05.000000 elasticemail-4.1.0/ElasticEmail/model/email_job_status.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5439 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/email_message_data.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5439 2024-05-23 09:31:06.000000 elasticemail-4.1.0/ElasticEmail/model/email_message_data.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2207 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/email_predicted_validation_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1980 2024-05-23 09:31:06.000000 elasticemail-4.1.0/ElasticEmail/model/email_predicted_validation_status.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4883 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/email_recipient.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4883 2024-05-23 09:31:06.000000 elasticemail-4.1.0/ElasticEmail/model/email_recipient.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3801 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/email_send.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3801 2024-05-23 09:31:07.000000 elasticemail-4.1.0/ElasticEmail/model/email_send.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10809 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/email_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10809 2024-05-23 09:31:07.000000 elasticemail-4.1.0/ElasticEmail/model/email_status.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4651 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/email_transactional_message_data.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4651 2024-05-23 09:31:07.000000 elasticemail-4.1.0/ElasticEmail/model/email_transactional_message_data.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9093 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/email_validation_result.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9093 2024-05-23 09:31:07.000000 elasticemail-4.1.0/ElasticEmail/model/email_validation_result.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2182 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/email_validation_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1963 2024-05-23 09:31:08.000000 elasticemail-4.1.0/ElasticEmail/model/email_validation_status.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4065 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/email_view.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4065 2024-05-23 09:31:08.000000 elasticemail-4.1.0/ElasticEmail/model/email_view.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4514 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/emails_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4514 2024-05-23 09:31:08.000000 elasticemail-4.1.0/ElasticEmail/model/emails_payload.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2502 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/encoding_type.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2189 2024-05-23 09:31:08.000000 elasticemail-4.1.0/ElasticEmail/model/encoding_type.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2597 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/event_type.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2249 2024-05-23 09:31:08.000000 elasticemail-4.1.0/ElasticEmail/model/event_type.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1904 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/events_order_by.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1745 2024-05-23 09:31:08.000000 elasticemail-4.1.0/ElasticEmail/model/events_order_by.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1960 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/export_file_formats.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1817 2024-05-23 09:31:08.000000 elasticemail-4.1.0/ElasticEmail/model/export_file_formats.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3751 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/export_link.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3751 2024-05-23 09:31:08.000000 elasticemail-4.1.0/ElasticEmail/model/export_link.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2102 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/export_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1911 2024-05-23 09:31:09.000000 elasticemail-4.1.0/ElasticEmail/model/export_status.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6962 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/file_info.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6962 2024-05-23 09:31:09.000000 elasticemail-4.1.0/ElasticEmail/model/file_info.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4370 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/file_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4370 2024-05-23 09:31:09.000000 elasticemail-4.1.0/ElasticEmail/model/file_payload.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3983 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/file_upload_result.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3983 2024-05-23 09:31:09.000000 elasticemail-4.1.0/ElasticEmail/model/file_upload_result.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6277 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/inbound_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6277 2024-05-23 09:31:09.000000 elasticemail-4.1.0/ElasticEmail/model/inbound_payload.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6814 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/inbound_route.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6814 2024-05-23 09:31:09.000000 elasticemail-4.1.0/ElasticEmail/model/inbound_route.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2023 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/inbound_route_action_type.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1834 2024-05-23 09:31:10.000000 elasticemail-4.1.0/ElasticEmail/model/inbound_route_action_type.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1879 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/inbound_route_filter_type.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1737 2024-05-23 09:31:10.000000 elasticemail-4.1.0/ElasticEmail/model/inbound_route_filter_type.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5188 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/list_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5188 2024-05-23 09:31:10.000000 elasticemail-4.1.0/ElasticEmail/model/list_payload.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3884 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/list_update_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3884 2024-05-23 09:31:10.000000 elasticemail-4.1.0/ElasticEmail/model/list_update_payload.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2841 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/log_job_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2413 2024-05-23 09:31:10.000000 elasticemail-4.1.0/ElasticEmail/model/log_job_status.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10060 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/log_status_summary.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10060 2024-05-23 09:31:10.000000 elasticemail-4.1.0/ElasticEmail/model/log_status_summary.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4559 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/merge_email_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4559 2024-05-23 09:31:11.000000 elasticemail-4.1.0/ElasticEmail/model/merge_email_payload.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4877 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/message_attachment.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4877 2024-05-23 09:31:11.000000 elasticemail-4.1.0/ElasticEmail/model/message_attachment.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3918 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/message_category.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3128 2024-05-23 09:31:11.000000 elasticemail-4.1.0/ElasticEmail/model/message_category.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9865 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/new_api_key.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9865 2024-05-23 09:31:11.000000 elasticemail-4.1.0/ElasticEmail/model/new_api_key.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9041 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/new_smtp_credentials.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9041 2024-05-23 09:31:12.000000 elasticemail-4.1.0/ElasticEmail/model/new_smtp_credentials.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8286 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/options.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8286 2024-05-23 09:31:12.000000 elasticemail-4.1.0/ElasticEmail/model/options.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10694 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/recipient_event.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10694 2024-05-23 09:31:12.000000 elasticemail-4.1.0/ElasticEmail/model/recipient_event.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3678 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/segment.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3678 2024-05-23 09:31:13.000000 elasticemail-4.1.0/ElasticEmail/model/segment.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3659 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/segment_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3659 2024-05-23 09:31:13.000000 elasticemail-4.1.0/ElasticEmail/model/segment_payload.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8521 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/smtp_credentials.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8521 2024-05-23 09:31:13.000000 elasticemail-4.1.0/ElasticEmail/model/smtp_credentials.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6614 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/smtp_credentials_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6614 2024-05-23 09:31:13.000000 elasticemail-4.1.0/ElasticEmail/model/smtp_credentials_payload.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4009 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/sort_order_item.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4009 2024-05-23 09:31:13.000000 elasticemail-4.1.0/ElasticEmail/model/sort_order_item.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1844 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/split_optimization_type.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1719 2024-05-23 09:31:13.000000 elasticemail-4.1.0/ElasticEmail/model/split_optimization_type.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4153 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/split_options.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4153 2024-05-23 09:31:14.000000 elasticemail-4.1.0/ElasticEmail/model/split_options.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8220 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/sub_account_info.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8220 2024-05-23 09:31:14.000000 elasticemail-4.1.0/ElasticEmail/model/sub_account_info.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3845 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/subaccount_email_credits_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3845 2024-05-23 09:31:14.000000 elasticemail-4.1.0/ElasticEmail/model/subaccount_email_credits_payload.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8645 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/subaccount_email_settings.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8645 2024-05-23 09:31:14.000000 elasticemail-4.1.0/ElasticEmail/model/subaccount_email_settings.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     7953 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/subaccount_email_settings_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     7953 2024-05-23 09:31:15.000000 elasticemail-4.1.0/ElasticEmail/model/subaccount_email_settings_payload.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5137 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/subaccount_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5137 2024-05-23 09:31:15.000000 elasticemail-4.1.0/ElasticEmail/model/subaccount_payload.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3392 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/subaccount_settings_info.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3392 2024-05-23 09:31:15.000000 elasticemail-4.1.0/ElasticEmail/model/subaccount_settings_info.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3456 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/subaccount_settings_info_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3456 2024-05-23 09:31:15.000000 elasticemail-4.1.0/ElasticEmail/model/subaccount_settings_info_payload.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6541 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/suppression.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6541 2024-05-23 09:31:15.000000 elasticemail-4.1.0/ElasticEmail/model/suppression.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6981 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/template.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6981 2024-05-23 09:31:15.000000 elasticemail-4.1.0/ElasticEmail/model/template.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5804 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/template_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5804 2024-05-23 09:31:15.000000 elasticemail-4.1.0/ElasticEmail/model/template_payload.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1878 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/template_scope.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1747 2024-05-23 09:31:16.000000 elasticemail-4.1.0/ElasticEmail/model/template_scope.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2191 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/template_type.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1938 2024-05-23 09:31:16.000000 elasticemail-4.1.0/ElasticEmail/model/template_type.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6528 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/transactional_recipient.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6528 2024-05-23 09:31:16.000000 elasticemail-4.1.0/ElasticEmail/model/transactional_recipient.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4777 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/utm.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     4777 2024-05-23 09:31:16.000000 elasticemail-4.1.0/ElasticEmail/model/utm.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6447 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/verification_file_result.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     6447 2024-05-23 09:31:16.000000 elasticemail-4.1.0/ElasticEmail/model/verification_file_result.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8138 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/verification_file_result_details.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8138 2024-05-23 09:31:17.000000 elasticemail-4.1.0/ElasticEmail/model/verification_file_result_details.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2207 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/model/verification_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1974 2024-05-23 09:31:17.000000 elasticemail-4.1.0/ElasticEmail/model/verification_status.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:04.991184 elasticemail-4.1.0/ElasticEmail/models/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     5922 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/models/__init__.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:04.991184 elasticemail-4.1.0/ElasticEmail/paths/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     3363 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/paths/__init__.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:04.995184 elasticemail-4.1.0/ElasticEmail/paths/campaigns/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      301 2024-05-23 09:31:19.000000 elasticemail-4.1.0/ElasticEmail/paths/campaigns/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10998 2024-05-23 09:31:19.000000 elasticemail-4.1.0/ElasticEmail/paths/campaigns/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10891 2024-05-23 09:31:19.000000 elasticemail-4.1.0/ElasticEmail/paths/campaigns/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11416 2024-05-23 09:31:19.000000 elasticemail-4.1.0/ElasticEmail/paths/campaigns/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11309 2024-05-23 09:31:19.000000 elasticemail-4.1.0/ElasticEmail/paths/campaigns/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:04.999184 elasticemail-4.1.0/ElasticEmail/paths/campaigns_name/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      311 2024-05-23 09:31:19.000000 elasticemail-4.1.0/ElasticEmail/paths/campaigns_name/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8138 2024-05-23 09:31:18.000000 elasticemail-4.1.0/ElasticEmail/paths/campaigns_name/delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8031 2024-05-23 09:31:18.000000 elasticemail-4.1.0/ElasticEmail/paths/campaigns_name/delete.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9716 2024-05-23 09:31:18.000000 elasticemail-4.1.0/ElasticEmail/paths/campaigns_name/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9609 2024-05-23 09:31:18.000000 elasticemail-4.1.0/ElasticEmail/paths/campaigns_name/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13663 2024-05-23 09:31:19.000000 elasticemail-4.1.0/ElasticEmail/paths/campaigns_name/put.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13556 2024-05-23 09:31:19.000000 elasticemail-4.1.0/ElasticEmail/paths/campaigns_name/put.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.003184 elasticemail-4.1.0/ElasticEmail/paths/contacts/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      299 2024-05-23 09:31:23.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10703 2024-05-23 09:31:22.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10596 2024-05-23 09:31:22.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    15809 2024-05-23 09:31:23.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    15702 2024-05-23 09:31:23.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.007184 elasticemail-4.1.0/ElasticEmail/paths/contacts_delete/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      313 2024-05-23 09:31:23.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts_delete/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9832 2024-05-23 09:31:21.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts_delete/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9725 2024-05-23 09:31:22.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts_delete/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.011184 elasticemail-4.1.0/ElasticEmail/paths/contacts_email/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      311 2024-05-23 09:31:23.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts_email/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8144 2024-05-23 09:31:20.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts_email/delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8037 2024-05-23 09:31:20.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts_email/delete.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9719 2024-05-23 09:31:20.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts_email/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9612 2024-05-23 09:31:21.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts_email/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13781 2024-05-23 09:31:21.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts_email/put.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13674 2024-05-23 09:31:21.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts_email/put.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.011184 elasticemail-4.1.0/ElasticEmail/paths/contacts_export/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      313 2024-05-23 09:31:23.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts_export/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11800 2024-05-23 09:31:22.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts_export/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11693 2024-05-23 09:31:22.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts_export/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.015184 elasticemail-4.1.0/ElasticEmail/paths/contacts_export_id_status/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      333 2024-05-23 09:31:23.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts_export_id_status/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9840 2024-05-23 09:31:22.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts_export_id_status/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9733 2024-05-23 09:31:22.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts_export_id_status/get.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.015184 elasticemail-4.1.0/ElasticEmail/paths/contacts_import/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      313 2024-05-23 09:31:23.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts_import/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    15223 2024-05-23 09:31:23.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts_import/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    15116 2024-05-23 09:31:23.000000 elasticemail-4.1.0/ElasticEmail/paths/contacts_import/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.015184 elasticemail-4.1.0/ElasticEmail/paths/emails/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      295 2024-05-23 09:31:26.000000 elasticemail-4.1.0/ElasticEmail/paths/emails/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11480 2024-05-23 09:31:25.000000 elasticemail-4.1.0/ElasticEmail/paths/emails/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11373 2024-05-23 09:31:26.000000 elasticemail-4.1.0/ElasticEmail/paths/emails/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.019184 elasticemail-4.1.0/ElasticEmail/paths/emails_mergefile/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      315 2024-05-23 09:31:26.000000 elasticemail-4.1.0/ElasticEmail/paths/emails_mergefile/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11618 2024-05-23 09:31:25.000000 elasticemail-4.1.0/ElasticEmail/paths/emails_mergefile/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11511 2024-05-23 09:31:25.000000 elasticemail-4.1.0/ElasticEmail/paths/emails_mergefile/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.019184 elasticemail-4.1.0/ElasticEmail/paths/emails_msgid_view/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      317 2024-05-23 09:31:26.000000 elasticemail-4.1.0/ElasticEmail/paths/emails_msgid_view/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9756 2024-05-23 09:31:24.000000 elasticemail-4.1.0/ElasticEmail/paths/emails_msgid_view/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9649 2024-05-23 09:31:24.000000 elasticemail-4.1.0/ElasticEmail/paths/emails_msgid_view/get.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.023184 elasticemail-4.1.0/ElasticEmail/paths/emails_transactional/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      323 2024-05-23 09:31:26.000000 elasticemail-4.1.0/ElasticEmail/paths/emails_transactional/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11737 2024-05-23 09:31:26.000000 elasticemail-4.1.0/ElasticEmail/paths/emails_transactional/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11630 2024-05-23 09:31:26.000000 elasticemail-4.1.0/ElasticEmail/paths/emails_transactional/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.023184 elasticemail-4.1.0/ElasticEmail/paths/emails_transactionid_status/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      337 2024-05-23 09:31:26.000000 elasticemail-4.1.0/ElasticEmail/paths/emails_transactionid_status/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    14982 2024-05-23 09:31:24.000000 elasticemail-4.1.0/ElasticEmail/paths/emails_transactionid_status/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    14875 2024-05-23 09:31:25.000000 elasticemail-4.1.0/ElasticEmail/paths/emails_transactionid_status/get.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.027184 elasticemail-4.1.0/ElasticEmail/paths/events/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      295 2024-05-23 09:31:29.000000 elasticemail-4.1.0/ElasticEmail/paths/events/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13477 2024-05-23 09:31:29.000000 elasticemail-4.1.0/ElasticEmail/paths/events/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13370 2024-05-23 09:31:29.000000 elasticemail-4.1.0/ElasticEmail/paths/events/get.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.027184 elasticemail-4.1.0/ElasticEmail/paths/events_channels_export_id_status/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      347 2024-05-23 09:31:29.000000 elasticemail-4.1.0/ElasticEmail/paths/events_channels_export_id_status/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9924 2024-05-23 09:31:28.000000 elasticemail-4.1.0/ElasticEmail/paths/events_channels_export_id_status/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9817 2024-05-23 09:31:28.000000 elasticemail-4.1.0/ElasticEmail/paths/events_channels_export_id_status/get.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.027184 elasticemail-4.1.0/ElasticEmail/paths/events_channels_name/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      323 2024-05-23 09:31:29.000000 elasticemail-4.1.0/ElasticEmail/paths/events_channels_name/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    15633 2024-05-23 09:31:28.000000 elasticemail-4.1.0/ElasticEmail/paths/events_channels_name/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    15526 2024-05-23 09:31:28.000000 elasticemail-4.1.0/ElasticEmail/paths/events_channels_name/get.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.031184 elasticemail-4.1.0/ElasticEmail/paths/events_channels_name_export/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      337 2024-05-23 09:31:29.000000 elasticemail-4.1.0/ElasticEmail/paths/events_channels_name_export/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    15258 2024-05-23 09:31:27.000000 elasticemail-4.1.0/ElasticEmail/paths/events_channels_name_export/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    15151 2024-05-23 09:31:28.000000 elasticemail-4.1.0/ElasticEmail/paths/events_channels_name_export/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.031184 elasticemail-4.1.0/ElasticEmail/paths/events_export/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      309 2024-05-23 09:31:29.000000 elasticemail-4.1.0/ElasticEmail/paths/events_export/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13102 2024-05-23 09:31:29.000000 elasticemail-4.1.0/ElasticEmail/paths/events_export/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12995 2024-05-23 09:31:29.000000 elasticemail-4.1.0/ElasticEmail/paths/events_export/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.035184 elasticemail-4.1.0/ElasticEmail/paths/events_export_id_status/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      329 2024-05-23 09:31:29.000000 elasticemail-4.1.0/ElasticEmail/paths/events_export_id_status/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9818 2024-05-23 09:31:28.000000 elasticemail-4.1.0/ElasticEmail/paths/events_export_id_status/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9711 2024-05-23 09:31:28.000000 elasticemail-4.1.0/ElasticEmail/paths/events_export_id_status/get.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.035184 elasticemail-4.1.0/ElasticEmail/paths/events_transactionid/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      323 2024-05-23 09:31:29.000000 elasticemail-4.1.0/ElasticEmail/paths/events_transactionid/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    14762 2024-05-23 09:31:27.000000 elasticemail-4.1.0/ElasticEmail/paths/events_transactionid/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    14655 2024-05-23 09:31:27.000000 elasticemail-4.1.0/ElasticEmail/paths/events_transactionid/get.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.039184 elasticemail-4.1.0/ElasticEmail/paths/files/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      293 2024-05-23 09:31:31.000000 elasticemail-4.1.0/ElasticEmail/paths/files/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10675 2024-05-23 09:31:31.000000 elasticemail-4.1.0/ElasticEmail/paths/files/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10568 2024-05-23 09:31:31.000000 elasticemail-4.1.0/ElasticEmail/paths/files/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    14360 2024-05-23 09:31:31.000000 elasticemail-4.1.0/ElasticEmail/paths/files/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    14253 2024-05-23 09:31:31.000000 elasticemail-4.1.0/ElasticEmail/paths/files/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.043184 elasticemail-4.1.0/ElasticEmail/paths/files_name/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      303 2024-05-23 09:31:31.000000 elasticemail-4.1.0/ElasticEmail/paths/files_name/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8090 2024-05-23 09:31:30.000000 elasticemail-4.1.0/ElasticEmail/paths/files_name/delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     7983 2024-05-23 09:31:30.000000 elasticemail-4.1.0/ElasticEmail/paths/files_name/delete.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9616 2024-05-23 09:31:30.000000 elasticemail-4.1.0/ElasticEmail/paths/files_name/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9509 2024-05-23 09:31:30.000000 elasticemail-4.1.0/ElasticEmail/paths/files_name/get.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.043184 elasticemail-4.1.0/ElasticEmail/paths/files_name_info/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      313 2024-05-23 09:31:31.000000 elasticemail-4.1.0/ElasticEmail/paths/files_name_info/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9731 2024-05-23 09:31:31.000000 elasticemail-4.1.0/ElasticEmail/paths/files_name_info/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9624 2024-05-23 09:31:31.000000 elasticemail-4.1.0/ElasticEmail/paths/files_name_info/get.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.047184 elasticemail-4.1.0/ElasticEmail/paths/inboundroute/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      307 2024-05-23 09:31:34.000000 elasticemail-4.1.0/ElasticEmail/paths/inboundroute/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8319 2024-05-23 09:31:32.000000 elasticemail-4.1.0/ElasticEmail/paths/inboundroute/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8212 2024-05-23 09:31:33.000000 elasticemail-4.1.0/ElasticEmail/paths/inboundroute/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11550 2024-05-23 09:31:33.000000 elasticemail-4.1.0/ElasticEmail/paths/inboundroute/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11443 2024-05-23 09:31:33.000000 elasticemail-4.1.0/ElasticEmail/paths/inboundroute/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.051184 elasticemail-4.1.0/ElasticEmail/paths/inboundroute_id/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      313 2024-05-23 09:31:34.000000 elasticemail-4.1.0/ElasticEmail/paths/inboundroute_id/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8132 2024-05-23 09:31:32.000000 elasticemail-4.1.0/ElasticEmail/paths/inboundroute_id/delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8025 2024-05-23 09:31:32.000000 elasticemail-4.1.0/ElasticEmail/paths/inboundroute_id/delete.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9722 2024-05-23 09:31:32.000000 elasticemail-4.1.0/ElasticEmail/paths/inboundroute_id/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9615 2024-05-23 09:31:32.000000 elasticemail-4.1.0/ElasticEmail/paths/inboundroute_id/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13754 2024-05-23 09:31:32.000000 elasticemail-4.1.0/ElasticEmail/paths/inboundroute_id/put.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13647 2024-05-23 09:31:32.000000 elasticemail-4.1.0/ElasticEmail/paths/inboundroute_id/put.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.051184 elasticemail-4.1.0/ElasticEmail/paths/inboundroute_order/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      319 2024-05-23 09:31:34.000000 elasticemail-4.1.0/ElasticEmail/paths/inboundroute_order/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13022 2024-05-23 09:31:33.000000 elasticemail-4.1.0/ElasticEmail/paths/inboundroute_order/put.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12915 2024-05-23 09:31:33.000000 elasticemail-4.1.0/ElasticEmail/paths/inboundroute_order/put.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.055184 elasticemail-4.1.0/ElasticEmail/paths/lists/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      293 2024-05-23 09:31:36.000000 elasticemail-4.1.0/ElasticEmail/paths/lists/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10703 2024-05-23 09:31:36.000000 elasticemail-4.1.0/ElasticEmail/paths/lists/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10596 2024-05-23 09:31:36.000000 elasticemail-4.1.0/ElasticEmail/paths/lists/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11440 2024-05-23 09:31:36.000000 elasticemail-4.1.0/ElasticEmail/paths/lists/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11333 2024-05-23 09:31:36.000000 elasticemail-4.1.0/ElasticEmail/paths/lists/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.059184 elasticemail-4.1.0/ElasticEmail/paths/lists_name/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      303 2024-05-23 09:31:36.000000 elasticemail-4.1.0/ElasticEmail/paths/lists_name/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8090 2024-05-23 09:31:35.000000 elasticemail-4.1.0/ElasticEmail/paths/lists_name/delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     7983 2024-05-23 09:31:35.000000 elasticemail-4.1.0/ElasticEmail/paths/lists_name/delete.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9681 2024-05-23 09:31:35.000000 elasticemail-4.1.0/ElasticEmail/paths/lists_name/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9574 2024-05-23 09:31:35.000000 elasticemail-4.1.0/ElasticEmail/paths/lists_name/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13720 2024-05-23 09:31:35.000000 elasticemail-4.1.0/ElasticEmail/paths/lists_name/put.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13613 2024-05-23 09:31:35.000000 elasticemail-4.1.0/ElasticEmail/paths/lists_name/put.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.063184 elasticemail-4.1.0/ElasticEmail/paths/lists_name_contacts/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      321 2024-05-23 09:31:36.000000 elasticemail-4.1.0/ElasticEmail/paths/lists_name_contacts/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13842 2024-05-23 09:31:34.000000 elasticemail-4.1.0/ElasticEmail/paths/lists_name_contacts/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13735 2024-05-23 09:31:34.000000 elasticemail-4.1.0/ElasticEmail/paths/lists_name_contacts/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.063184 elasticemail-4.1.0/ElasticEmail/paths/lists_name_contacts_remove/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      335 2024-05-23 09:31:36.000000 elasticemail-4.1.0/ElasticEmail/paths/lists_name_contacts_remove/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12178 2024-05-23 09:31:34.000000 elasticemail-4.1.0/ElasticEmail/paths/lists_name_contacts_remove/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12071 2024-05-23 09:31:34.000000 elasticemail-4.1.0/ElasticEmail/paths/lists_name_contacts_remove/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.067184 elasticemail-4.1.0/ElasticEmail/paths/security_apikeys/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      315 2024-05-23 09:31:39.000000 elasticemail-4.1.0/ElasticEmail/paths/security_apikeys/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10504 2024-05-23 09:31:37.000000 elasticemail-4.1.0/ElasticEmail/paths/security_apikeys/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10397 2024-05-23 09:31:37.000000 elasticemail-4.1.0/ElasticEmail/paths/security_apikeys/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11589 2024-05-23 09:31:38.000000 elasticemail-4.1.0/ElasticEmail/paths/security_apikeys/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11482 2024-05-23 09:31:38.000000 elasticemail-4.1.0/ElasticEmail/paths/security_apikeys/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.071184 elasticemail-4.1.0/ElasticEmail/paths/security_apikeys_name/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      325 2024-05-23 09:31:39.000000 elasticemail-4.1.0/ElasticEmail/paths/security_apikeys_name/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10394 2024-05-23 09:31:36.000000 elasticemail-4.1.0/ElasticEmail/paths/security_apikeys_name/delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10287 2024-05-23 09:31:37.000000 elasticemail-4.1.0/ElasticEmail/paths/security_apikeys_name/delete.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11967 2024-05-23 09:31:37.000000 elasticemail-4.1.0/ElasticEmail/paths/security_apikeys_name/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11860 2024-05-23 09:31:37.000000 elasticemail-4.1.0/ElasticEmail/paths/security_apikeys_name/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13826 2024-05-23 09:31:37.000000 elasticemail-4.1.0/ElasticEmail/paths/security_apikeys_name/put.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13719 2024-05-23 09:31:37.000000 elasticemail-4.1.0/ElasticEmail/paths/security_apikeys_name/put.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.075184 elasticemail-4.1.0/ElasticEmail/paths/security_smtp/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      309 2024-05-23 09:31:39.000000 elasticemail-4.1.0/ElasticEmail/paths/security_smtp/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10543 2024-05-23 09:31:39.000000 elasticemail-4.1.0/ElasticEmail/paths/security_smtp/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10436 2024-05-23 09:31:39.000000 elasticemail-4.1.0/ElasticEmail/paths/security_smtp/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11631 2024-05-23 09:31:39.000000 elasticemail-4.1.0/ElasticEmail/paths/security_smtp/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11524 2024-05-23 09:31:39.000000 elasticemail-4.1.0/ElasticEmail/paths/security_smtp/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.079184 elasticemail-4.1.0/ElasticEmail/paths/security_smtp_name/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      319 2024-05-23 09:31:39.000000 elasticemail-4.1.0/ElasticEmail/paths/security_smtp_name/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10370 2024-05-23 09:31:38.000000 elasticemail-4.1.0/ElasticEmail/paths/security_smtp_name/delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10263 2024-05-23 09:31:38.000000 elasticemail-4.1.0/ElasticEmail/paths/security_smtp_name/delete.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11970 2024-05-23 09:31:38.000000 elasticemail-4.1.0/ElasticEmail/paths/security_smtp_name/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11863 2024-05-23 09:31:38.000000 elasticemail-4.1.0/ElasticEmail/paths/security_smtp_name/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13868 2024-05-23 09:31:38.000000 elasticemail-4.1.0/ElasticEmail/paths/security_smtp_name/put.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13761 2024-05-23 09:31:38.000000 elasticemail-4.1.0/ElasticEmail/paths/security_smtp_name/put.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.083184 elasticemail-4.1.0/ElasticEmail/paths/segments/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      299 2024-05-23 09:31:41.000000 elasticemail-4.1.0/ElasticEmail/paths/segments/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10703 2024-05-23 09:31:40.000000 elasticemail-4.1.0/ElasticEmail/paths/segments/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10596 2024-05-23 09:31:40.000000 elasticemail-4.1.0/ElasticEmail/paths/segments/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11481 2024-05-23 09:31:41.000000 elasticemail-4.1.0/ElasticEmail/paths/segments/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11374 2024-05-23 09:31:41.000000 elasticemail-4.1.0/ElasticEmail/paths/segments/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.087184 elasticemail-4.1.0/ElasticEmail/paths/segments_name/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      309 2024-05-23 09:31:41.000000 elasticemail-4.1.0/ElasticEmail/paths/segments_name/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8126 2024-05-23 09:31:40.000000 elasticemail-4.1.0/ElasticEmail/paths/segments_name/delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8019 2024-05-23 09:31:40.000000 elasticemail-4.1.0/ElasticEmail/paths/segments_name/delete.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9701 2024-05-23 09:31:40.000000 elasticemail-4.1.0/ElasticEmail/paths/segments_name/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9594 2024-05-23 09:31:40.000000 elasticemail-4.1.0/ElasticEmail/paths/segments_name/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13728 2024-05-23 09:31:40.000000 elasticemail-4.1.0/ElasticEmail/paths/segments_name/put.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13621 2024-05-23 09:31:40.000000 elasticemail-4.1.0/ElasticEmail/paths/segments_name/put.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.087184 elasticemail-4.1.0/ElasticEmail/paths/statistics/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      303 2024-05-23 09:31:42.000000 elasticemail-4.1.0/ElasticEmail/paths/statistics/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10616 2024-05-23 09:31:42.000000 elasticemail-4.1.0/ElasticEmail/paths/statistics/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10509 2024-05-23 09:31:42.000000 elasticemail-4.1.0/ElasticEmail/paths/statistics/get.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.091184 elasticemail-4.1.0/ElasticEmail/paths/statistics_campaigns/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      323 2024-05-23 09:31:42.000000 elasticemail-4.1.0/ElasticEmail/paths/statistics_campaigns/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10956 2024-05-23 09:31:41.000000 elasticemail-4.1.0/ElasticEmail/paths/statistics_campaigns/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10849 2024-05-23 09:31:41.000000 elasticemail-4.1.0/ElasticEmail/paths/statistics_campaigns/get.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.091184 elasticemail-4.1.0/ElasticEmail/paths/statistics_campaigns_name/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      333 2024-05-23 09:31:42.000000 elasticemail-4.1.0/ElasticEmail/paths/statistics_campaigns_name/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9890 2024-05-23 09:31:41.000000 elasticemail-4.1.0/ElasticEmail/paths/statistics_campaigns_name/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9783 2024-05-23 09:31:41.000000 elasticemail-4.1.0/ElasticEmail/paths/statistics_campaigns_name/get.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.095183 elasticemail-4.1.0/ElasticEmail/paths/statistics_channels/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      321 2024-05-23 09:31:42.000000 elasticemail-4.1.0/ElasticEmail/paths/statistics_channels/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10944 2024-05-23 09:31:42.000000 elasticemail-4.1.0/ElasticEmail/paths/statistics_channels/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10837 2024-05-23 09:31:42.000000 elasticemail-4.1.0/ElasticEmail/paths/statistics_channels/get.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.095183 elasticemail-4.1.0/ElasticEmail/paths/statistics_channels_name/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      331 2024-05-23 09:31:42.000000 elasticemail-4.1.0/ElasticEmail/paths/statistics_channels_name/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9878 2024-05-23 09:31:42.000000 elasticemail-4.1.0/ElasticEmail/paths/statistics_channels_name/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9771 2024-05-23 09:31:42.000000 elasticemail-4.1.0/ElasticEmail/paths/statistics_channels_name/get.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.099184 elasticemail-4.1.0/ElasticEmail/paths/subaccounts/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      305 2024-05-23 09:31:44.000000 elasticemail-4.1.0/ElasticEmail/paths/subaccounts/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10790 2024-05-23 09:31:44.000000 elasticemail-4.1.0/ElasticEmail/paths/subaccounts/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10683 2024-05-23 09:31:44.000000 elasticemail-4.1.0/ElasticEmail/paths/subaccounts/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11561 2024-05-23 09:31:44.000000 elasticemail-4.1.0/ElasticEmail/paths/subaccounts/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11454 2024-05-23 09:31:44.000000 elasticemail-4.1.0/ElasticEmail/paths/subaccounts/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.103184 elasticemail-4.1.0/ElasticEmail/paths/subaccounts_email/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      317 2024-05-23 09:31:44.000000 elasticemail-4.1.0/ElasticEmail/paths/subaccounts_email/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8180 2024-05-23 09:31:43.000000 elasticemail-4.1.0/ElasticEmail/paths/subaccounts_email/delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8073 2024-05-23 09:31:43.000000 elasticemail-4.1.0/ElasticEmail/paths/subaccounts_email/delete.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9778 2024-05-23 09:31:43.000000 elasticemail-4.1.0/ElasticEmail/paths/subaccounts_email/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9671 2024-05-23 09:31:43.000000 elasticemail-4.1.0/ElasticEmail/paths/subaccounts_email/get.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.103184 elasticemail-4.1.0/ElasticEmail/paths/subaccounts_email_credits/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      333 2024-05-23 09:31:44.000000 elasticemail-4.1.0/ElasticEmail/paths/subaccounts_email_credits/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12281 2024-05-23 09:31:43.000000 elasticemail-4.1.0/ElasticEmail/paths/subaccounts_email_credits/patch.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12174 2024-05-23 09:31:43.000000 elasticemail-4.1.0/ElasticEmail/paths/subaccounts_email_credits/patch.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.107184 elasticemail-4.1.0/ElasticEmail/paths/subaccounts_email_settings_email/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      347 2024-05-23 09:31:44.000000 elasticemail-4.1.0/ElasticEmail/paths/subaccounts_email_settings_email/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    14015 2024-05-23 09:31:43.000000 elasticemail-4.1.0/ElasticEmail/paths/subaccounts_email_settings_email/put.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13908 2024-05-23 09:31:44.000000 elasticemail-4.1.0/ElasticEmail/paths/subaccounts_email_settings_email/put.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.107184 elasticemail-4.1.0/ElasticEmail/paths/suppressions/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      307 2024-05-23 09:31:48.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10778 2024-05-23 09:31:47.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10671 2024-05-23 09:31:47.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions/get.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.111184 elasticemail-4.1.0/ElasticEmail/paths/suppressions_bounces/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      323 2024-05-23 09:31:48.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_bounces/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11140 2024-05-23 09:31:45.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_bounces/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11033 2024-05-23 09:31:45.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_bounces/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12946 2024-05-23 09:31:45.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_bounces/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12839 2024-05-23 09:31:45.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_bounces/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.111184 elasticemail-4.1.0/ElasticEmail/paths/suppressions_bounces_import/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      337 2024-05-23 09:31:48.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_bounces_import/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12401 2024-05-23 09:31:45.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_bounces_import/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12294 2024-05-23 09:31:45.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_bounces_import/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.115183 elasticemail-4.1.0/ElasticEmail/paths/suppressions_complaints/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      329 2024-05-23 09:31:48.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_complaints/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11177 2024-05-23 09:31:46.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_complaints/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11070 2024-05-23 09:31:46.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_complaints/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12988 2024-05-23 09:31:47.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_complaints/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12881 2024-05-23 09:31:47.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_complaints/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.119183 elasticemail-4.1.0/ElasticEmail/paths/suppressions_complaints_import/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      343 2024-05-23 09:31:48.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_complaints_import/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12443 2024-05-23 09:31:46.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_complaints_import/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12336 2024-05-23 09:31:46.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_complaints_import/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.123183 elasticemail-4.1.0/ElasticEmail/paths/suppressions_email/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      319 2024-05-23 09:31:48.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_email/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8192 2024-05-23 09:31:45.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_email/delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8085 2024-05-23 09:31:46.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_email/delete.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9778 2024-05-23 09:31:46.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_email/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9671 2024-05-23 09:31:46.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_email/get.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.123183 elasticemail-4.1.0/ElasticEmail/paths/suppressions_unsubscribes/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      333 2024-05-23 09:31:48.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_unsubscribes/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11201 2024-05-23 09:31:47.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_unsubscribes/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11094 2024-05-23 09:31:47.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_unsubscribes/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13016 2024-05-23 09:31:48.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_unsubscribes/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12909 2024-05-23 09:31:48.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_unsubscribes/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.127183 elasticemail-4.1.0/ElasticEmail/paths/suppressions_unsubscribes_import/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      347 2024-05-23 09:31:48.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_unsubscribes_import/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12471 2024-05-23 09:31:47.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_unsubscribes_import/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12364 2024-05-23 09:31:47.000000 elasticemail-4.1.0/ElasticEmail/paths/suppressions_unsubscribes_import/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.131183 elasticemail-4.1.0/ElasticEmail/paths/templates/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      301 2024-05-23 09:31:50.000000 elasticemail-4.1.0/ElasticEmail/paths/templates/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12672 2024-05-23 09:31:50.000000 elasticemail-4.1.0/ElasticEmail/paths/templates/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12565 2024-05-23 09:31:50.000000 elasticemail-4.1.0/ElasticEmail/paths/templates/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11503 2024-05-23 09:31:50.000000 elasticemail-4.1.0/ElasticEmail/paths/templates/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11396 2024-05-23 09:31:50.000000 elasticemail-4.1.0/ElasticEmail/paths/templates/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.135183 elasticemail-4.1.0/ElasticEmail/paths/templates_name/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      311 2024-05-23 09:31:50.000000 elasticemail-4.1.0/ElasticEmail/paths/templates_name/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8138 2024-05-23 09:31:49.000000 elasticemail-4.1.0/ElasticEmail/paths/templates_name/delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8031 2024-05-23 09:31:49.000000 elasticemail-4.1.0/ElasticEmail/paths/templates_name/delete.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9716 2024-05-23 09:31:49.000000 elasticemail-4.1.0/ElasticEmail/paths/templates_name/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9609 2024-05-23 09:31:49.000000 elasticemail-4.1.0/ElasticEmail/paths/templates_name/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13750 2024-05-23 09:31:49.000000 elasticemail-4.1.0/ElasticEmail/paths/templates_name/put.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13643 2024-05-23 09:31:49.000000 elasticemail-4.1.0/ElasticEmail/paths/templates_name/put.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.135183 elasticemail-4.1.0/ElasticEmail/paths/verifications/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      309 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10876 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    10769 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications/get.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.139183 elasticemail-4.1.0/ElasticEmail/paths/verifications_email/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      321 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_email/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8217 2024-05-23 09:31:51.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_email/delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8110 2024-05-23 09:31:51.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_email/delete.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9835 2024-05-23 09:31:51.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_email/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9728 2024-05-23 09:31:51.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_email/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9835 2024-05-23 09:31:51.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_email/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9728 2024-05-23 09:31:51.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_email/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.143183 elasticemail-4.1.0/ElasticEmail/paths/verifications_files/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      321 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_files/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    14095 2024-05-23 09:31:52.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_files/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    13988 2024-05-23 09:31:52.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_files/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.147183 elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      327 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8227 2024-05-23 09:31:51.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id/delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8120 2024-05-23 09:31:51.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id/delete.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.147183 elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id_result/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      341 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id_result/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12416 2024-05-23 09:31:52.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id_result/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    12309 2024-05-23 09:31:52.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id_result/get.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.151183 elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id_result_download/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      359 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id_result_download/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9927 2024-05-23 09:31:52.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id_result_download/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     9820 2024-05-23 09:31:52.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id_result_download/get.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.151183 elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id_verification/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      353 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id_verification/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8322 2024-05-23 09:31:52.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id_verification/post.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8215 2024-05-23 09:31:52.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id_verification/post.pyi
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.155183 elasticemail-4.1.0/ElasticEmail/paths/verifications_files_result/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      335 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_files_result/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8562 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_files_result/get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     8455 2024-05-23 09:31:53.000000 elasticemail-4.1.0/ElasticEmail/paths/verifications_files_result/get.pyi
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    11308 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/rest.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    98414 2024-05-23 09:31:54.000000 elasticemail-4.1.0/ElasticEmail/schemas.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.323182 elasticemail-4.1.0/ElasticEmail.egg-info/
+-rw-r--r--   0 radzaw    (1000) radzaw    (1000)    32110 2024-05-23 09:32:04.000000 elasticemail-4.1.0/ElasticEmail.egg-info/PKG-INFO
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    34902 2024-05-23 09:32:04.000000 elasticemail-4.1.0/ElasticEmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        1 2024-05-23 09:32:04.000000 elasticemail-4.1.0/ElasticEmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)       32 2024-05-23 09:32:04.000000 elasticemail-4.1.0/ElasticEmail.egg-info/requires.txt
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)       18 2024-05-23 09:32:04.000000 elasticemail-4.1.0/ElasticEmail.egg-info/top_level.txt
+-rw-r--r--   0 radzaw    (1000) radzaw    (1000)    32110 2024-05-23 09:32:05.323182 elasticemail-4.1.0/PKG-INFO
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)    31759 2024-05-23 09:31:56.000000 elasticemail-4.1.0/README.md
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)       69 2024-05-23 09:32:05.323182 elasticemail-4.1.0/setup.cfg
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     2188 2024-05-23 09:31:54.000000 elasticemail-4.1.0/setup.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:04.783186 elasticemail-4.1.0/test/
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.219183 elasticemail-4.1.0/test/test_models/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:53.000000 elasticemail-4.1.0/test/test_models/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1312 2024-05-23 09:30:52.000000 elasticemail-4.1.0/test/test_models/test_access_level.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1337 2024-05-23 09:30:53.000000 elasticemail-4.1.0/test/test_models/test_account_status_enum.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1292 2024-05-23 09:30:54.000000 elasticemail-4.1.0/test/test_models/test_api_key.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1321 2024-05-23 09:30:56.000000 elasticemail-4.1.0/test/test_models/test_api_key_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1329 2024-05-23 09:30:57.000000 elasticemail-4.1.0/test/test_models/test_body_content_type.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1300 2024-05-23 09:30:57.000000 elasticemail-4.1.0/test/test_models/test_body_part.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1299 2024-05-23 09:30:58.000000 elasticemail-4.1.0/test/test_models/test_campaign.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1328 2024-05-23 09:30:58.000000 elasticemail-4.1.0/test/test_models/test_campaign_options.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1336 2024-05-23 09:30:59.000000 elasticemail-4.1.0/test/test_models/test_campaign_recipient.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1324 2024-05-23 09:30:59.000000 elasticemail-4.1.0/test/test_models/test_campaign_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1332 2024-05-23 09:30:59.000000 elasticemail-4.1.0/test/test_models/test_campaign_template.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1362 2024-05-23 09:31:00.000000 elasticemail-4.1.0/test/test_models/test_channel_log_status_summary.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1336 2024-05-23 09:31:00.000000 elasticemail-4.1.0/test/test_models/test_compression_format.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1312 2024-05-23 09:31:01.000000 elasticemail-4.1.0/test/test_models/test_consent_data.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1328 2024-05-23 09:31:01.000000 elasticemail-4.1.0/test/test_models/test_consent_tracking.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1295 2024-05-23 09:31:01.000000 elasticemail-4.1.0/test/test_models/test_contact.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1328 2024-05-23 09:31:02.000000 elasticemail-4.1.0/test/test_models/test_contact_activity.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1324 2024-05-23 09:31:02.000000 elasticemail-4.1.0/test/test_models/test_contact_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1320 2024-05-23 09:31:03.000000 elasticemail-4.1.0/test/test_models/test_contact_source.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1320 2024-05-23 09:31:03.000000 elasticemail-4.1.0/test/test_models/test_contact_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1349 2024-05-23 09:31:03.000000 elasticemail-4.1.0/test/test_models/test_contact_update_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1316 2024-05-23 09:31:03.000000 elasticemail-4.1.0/test/test_models/test_contacts_list.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1365 2024-05-23 09:31:03.000000 elasticemail-4.1.0/test/test_models/test_delivery_optimization_type.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1316 2024-05-23 09:31:04.000000 elasticemail-4.1.0/test/test_models/test_email_content.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1304 2024-05-23 09:31:04.000000 elasticemail-4.1.0/test/test_models/test_email_data.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1350 2024-05-23 09:31:05.000000 elasticemail-4.1.0/test/test_models/test_email_job_failed_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1325 2024-05-23 09:31:05.000000 elasticemail-4.1.0/test/test_models/test_email_job_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1333 2024-05-23 09:31:06.000000 elasticemail-4.1.0/test/test_models/test_email_message_data.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1390 2024-05-23 09:31:06.000000 elasticemail-4.1.0/test/test_models/test_email_predicted_validation_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1324 2024-05-23 09:31:06.000000 elasticemail-4.1.0/test/test_models/test_email_recipient.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1304 2024-05-23 09:31:07.000000 elasticemail-4.1.0/test/test_models/test_email_send.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1312 2024-05-23 09:31:07.000000 elasticemail-4.1.0/test/test_models/test_email_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1386 2024-05-23 09:31:07.000000 elasticemail-4.1.0/test/test_models/test_email_transactional_message_data.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1353 2024-05-23 09:31:07.000000 elasticemail-4.1.0/test/test_models/test_email_validation_result.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1353 2024-05-23 09:31:08.000000 elasticemail-4.1.0/test/test_models/test_email_validation_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1304 2024-05-23 09:31:08.000000 elasticemail-4.1.0/test/test_models/test_email_view.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1320 2024-05-23 09:31:08.000000 elasticemail-4.1.0/test/test_models/test_emails_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1316 2024-05-23 09:31:08.000000 elasticemail-4.1.0/test/test_models/test_encoding_type.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1304 2024-05-23 09:31:08.000000 elasticemail-4.1.0/test/test_models/test_event_type.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1321 2024-05-23 09:31:08.000000 elasticemail-4.1.0/test/test_models/test_events_order_by.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1337 2024-05-23 09:31:08.000000 elasticemail-4.1.0/test/test_models/test_export_file_formats.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1308 2024-05-23 09:31:08.000000 elasticemail-4.1.0/test/test_models/test_export_link.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1316 2024-05-23 09:31:09.000000 elasticemail-4.1.0/test/test_models/test_export_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1300 2024-05-23 09:31:09.000000 elasticemail-4.1.0/test/test_models/test_file_info.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1312 2024-05-23 09:31:09.000000 elasticemail-4.1.0/test/test_models/test_file_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1333 2024-05-23 09:31:09.000000 elasticemail-4.1.0/test/test_models/test_file_upload_result.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1324 2024-05-23 09:31:09.000000 elasticemail-4.1.0/test/test_models/test_inbound_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1316 2024-05-23 09:31:10.000000 elasticemail-4.1.0/test/test_models/test_inbound_route.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1358 2024-05-23 09:31:10.000000 elasticemail-4.1.0/test/test_models/test_inbound_route_action_type.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1358 2024-05-23 09:31:10.000000 elasticemail-4.1.0/test/test_models/test_inbound_route_filter_type.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1312 2024-05-23 09:31:10.000000 elasticemail-4.1.0/test/test_models/test_list_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1337 2024-05-23 09:31:10.000000 elasticemail-4.1.0/test/test_models/test_list_update_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1317 2024-05-23 09:31:10.000000 elasticemail-4.1.0/test/test_models/test_log_job_status.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1333 2024-05-23 09:31:10.000000 elasticemail-4.1.0/test/test_models/test_log_status_summary.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1337 2024-05-23 09:31:11.000000 elasticemail-4.1.0/test/test_models/test_merge_email_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1336 2024-05-23 09:31:11.000000 elasticemail-4.1.0/test/test_models/test_message_attachment.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1328 2024-05-23 09:31:11.000000 elasticemail-4.1.0/test/test_models/test_message_category.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1305 2024-05-23 09:31:11.000000 elasticemail-4.1.0/test/test_models/test_new_api_key.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1341 2024-05-23 09:31:12.000000 elasticemail-4.1.0/test/test_models/test_new_smtp_credentials.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1295 2024-05-23 09:31:12.000000 elasticemail-4.1.0/test/test_models/test_options.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1324 2024-05-23 09:31:12.000000 elasticemail-4.1.0/test/test_models/test_recipient_event.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1295 2024-05-23 09:31:13.000000 elasticemail-4.1.0/test/test_models/test_segment.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1324 2024-05-23 09:31:13.000000 elasticemail-4.1.0/test/test_models/test_segment_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1328 2024-05-23 09:31:13.000000 elasticemail-4.1.0/test/test_models/test_smtp_credentials.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1357 2024-05-23 09:31:13.000000 elasticemail-4.1.0/test/test_models/test_smtp_credentials_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1321 2024-05-23 09:31:13.000000 elasticemail-4.1.0/test/test_models/test_sort_order_item.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1353 2024-05-23 09:31:13.000000 elasticemail-4.1.0/test/test_models/test_split_optimization_type.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1316 2024-05-23 09:31:14.000000 elasticemail-4.1.0/test/test_models/test_split_options.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1325 2024-05-23 09:31:14.000000 elasticemail-4.1.0/test/test_models/test_sub_account_info.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1386 2024-05-23 09:31:14.000000 elasticemail-4.1.0/test/test_models/test_subaccount_email_credits_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1361 2024-05-23 09:31:14.000000 elasticemail-4.1.0/test/test_models/test_subaccount_email_settings.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1390 2024-05-23 09:31:15.000000 elasticemail-4.1.0/test/test_models/test_subaccount_email_settings_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1336 2024-05-23 09:31:15.000000 elasticemail-4.1.0/test/test_models/test_subaccount_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1357 2024-05-23 09:31:15.000000 elasticemail-4.1.0/test/test_models/test_subaccount_settings_info.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1386 2024-05-23 09:31:15.000000 elasticemail-4.1.0/test/test_models/test_subaccount_settings_info_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1311 2024-05-23 09:31:15.000000 elasticemail-4.1.0/test/test_models/test_suppression.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1299 2024-05-23 09:31:15.000000 elasticemail-4.1.0/test/test_models/test_template.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1328 2024-05-23 09:31:15.000000 elasticemail-4.1.0/test/test_models/test_template_payload.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1320 2024-05-23 09:31:16.000000 elasticemail-4.1.0/test/test_models/test_template_scope.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1316 2024-05-23 09:31:16.000000 elasticemail-4.1.0/test/test_models/test_template_type.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1356 2024-05-23 09:31:16.000000 elasticemail-4.1.0/test/test_models/test_transactional_recipient.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1279 2024-05-23 09:31:16.000000 elasticemail-4.1.0/test/test_models/test_utm.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1357 2024-05-23 09:31:16.000000 elasticemail-4.1.0/test/test_models/test_verification_file_result.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1386 2024-05-23 09:31:17.000000 elasticemail-4.1.0/test/test_models/test_verification_file_result_details.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1340 2024-05-23 09:31:17.000000 elasticemail-4.1.0/test/test_models/test_verification_status.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.219183 elasticemail-4.1.0/test/test_paths/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)     1995 2024-05-23 09:31:53.000000 elasticemail-4.1.0/test/test_paths/__init__.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.219183 elasticemail-4.1.0/test/test_paths/test_campaigns/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:20.000000 elasticemail-4.1.0/test/test_paths/test_campaigns/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      795 2024-05-23 09:31:20.000000 elasticemail-4.1.0/test/test_paths/test_campaigns/test_get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      798 2024-05-23 09:31:20.000000 elasticemail-4.1.0/test/test_paths/test_campaigns/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.223183 elasticemail-4.1.0/test/test_paths/test_campaigns_name/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:20.000000 elasticemail-4.1.0/test/test_paths/test_campaigns_name/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      839 2024-05-23 09:31:19.000000 elasticemail-4.1.0/test/test_paths/test_campaigns_name/test_delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      807 2024-05-23 09:31:20.000000 elasticemail-4.1.0/test/test_paths/test_campaigns_name/test_get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      811 2024-05-23 09:31:20.000000 elasticemail-4.1.0/test/test_paths/test_campaigns_name/test_put.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.223183 elasticemail-4.1.0/test/test_paths/test_contacts/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:24.000000 elasticemail-4.1.0/test/test_paths/test_contacts/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      791 2024-05-23 09:31:24.000000 elasticemail-4.1.0/test/test_paths/test_contacts/test_get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      794 2024-05-23 09:31:24.000000 elasticemail-4.1.0/test/test_paths/test_contacts/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.227182 elasticemail-4.1.0/test/test_paths/test_contacts_delete/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:23.000000 elasticemail-4.1.0/test/test_paths/test_contacts_delete/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      843 2024-05-23 09:31:23.000000 elasticemail-4.1.0/test/test_paths/test_contacts_delete/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.227182 elasticemail-4.1.0/test/test_paths/test_contacts_email/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:23.000000 elasticemail-4.1.0/test/test_paths/test_contacts_email/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      838 2024-05-23 09:31:23.000000 elasticemail-4.1.0/test/test_paths/test_contacts_email/test_delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      806 2024-05-23 09:31:23.000000 elasticemail-4.1.0/test/test_paths/test_contacts_email/test_get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      810 2024-05-23 09:31:23.000000 elasticemail-4.1.0/test/test_paths/test_contacts_email/test_put.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.231182 elasticemail-4.1.0/test/test_paths/test_contacts_export/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:23.000000 elasticemail-4.1.0/test/test_paths/test_contacts_export/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      815 2024-05-23 09:31:23.000000 elasticemail-4.1.0/test/test_paths/test_contacts_export/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.231182 elasticemail-4.1.0/test/test_paths/test_contacts_export_id_status/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:23.000000 elasticemail-4.1.0/test/test_paths/test_contacts_export_id_status/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      842 2024-05-23 09:31:23.000000 elasticemail-4.1.0/test/test_paths/test_contacts_export_id_status/test_get.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.231182 elasticemail-4.1.0/test/test_paths/test_contacts_import/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:24.000000 elasticemail-4.1.0/test/test_paths/test_contacts_import/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      836 2024-05-23 09:31:24.000000 elasticemail-4.1.0/test/test_paths/test_contacts_import/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.231182 elasticemail-4.1.0/test/test_paths/test_emails/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:26.000000 elasticemail-4.1.0/test/test_paths/test_emails/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      793 2024-05-23 09:31:26.000000 elasticemail-4.1.0/test/test_paths/test_emails/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.235182 elasticemail-4.1.0/test/test_paths/test_emails_mergefile/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:26.000000 elasticemail-4.1.0/test/test_paths/test_emails_mergefile/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      825 2024-05-23 09:31:26.000000 elasticemail-4.1.0/test/test_paths/test_emails_mergefile/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.235182 elasticemail-4.1.0/test/test_paths/test_emails_msgid_view/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:26.000000 elasticemail-4.1.0/test/test_paths/test_emails_msgid_view/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      811 2024-05-23 09:31:26.000000 elasticemail-4.1.0/test/test_paths/test_emails_msgid_view/test_get.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.235182 elasticemail-4.1.0/test/test_paths/test_emails_transactional/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:26.000000 elasticemail-4.1.0/test/test_paths/test_emails_transactional/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      841 2024-05-23 09:31:26.000000 elasticemail-4.1.0/test/test_paths/test_emails_transactional/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.239182 elasticemail-4.1.0/test/test_paths/test_emails_transactionid_status/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:26.000000 elasticemail-4.1.0/test/test_paths/test_emails_transactionid_status/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      841 2024-05-23 09:31:26.000000 elasticemail-4.1.0/test/test_paths/test_emails_transactionid_status/test_get.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.239182 elasticemail-4.1.0/test/test_paths/test_events/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:29.000000 elasticemail-4.1.0/test/test_paths/test_events/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      783 2024-05-23 09:31:29.000000 elasticemail-4.1.0/test/test_paths/test_events/test_get.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.239182 elasticemail-4.1.0/test/test_paths/test_events_channels_export_id_status/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:29.000000 elasticemail-4.1.0/test/test_paths/test_events_channels_export_id_status/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      869 2024-05-23 09:31:29.000000 elasticemail-4.1.0/test/test_paths/test_events_channels_export_id_status/test_get.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.239182 elasticemail-4.1.0/test/test_paths/test_events_channels_name/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:29.000000 elasticemail-4.1.0/test/test_paths/test_events_channels_name/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      829 2024-05-23 09:31:29.000000 elasticemail-4.1.0/test/test_paths/test_events_channels_name/test_get.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.243182 elasticemail-4.1.0/test/test_paths/test_events_channels_name_export/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:29.000000 elasticemail-4.1.0/test/test_paths/test_events_channels_name_export/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      853 2024-05-23 09:31:29.000000 elasticemail-4.1.0/test/test_paths/test_events_channels_name_export/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.243182 elasticemail-4.1.0/test/test_paths/test_events_export/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:29.000000 elasticemail-4.1.0/test/test_paths/test_events_export/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      807 2024-05-23 09:31:29.000000 elasticemail-4.1.0/test/test_paths/test_events_export/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.243182 elasticemail-4.1.0/test/test_paths/test_events_export_id_status/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:29.000000 elasticemail-4.1.0/test/test_paths/test_events_export_id_status/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      836 2024-05-23 09:31:29.000000 elasticemail-4.1.0/test/test_paths/test_events_export_id_status/test_get.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.247182 elasticemail-4.1.0/test/test_paths/test_events_transactionid/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:29.000000 elasticemail-4.1.0/test/test_paths/test_events_transactionid/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      829 2024-05-23 09:31:29.000000 elasticemail-4.1.0/test/test_paths/test_events_transactionid/test_get.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.247182 elasticemail-4.1.0/test/test_paths/test_files/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:31.000000 elasticemail-4.1.0/test/test_paths/test_files/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      779 2024-05-23 09:31:31.000000 elasticemail-4.1.0/test/test_paths/test_files/test_get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      785 2024-05-23 09:31:31.000000 elasticemail-4.1.0/test/test_paths/test_files/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.247182 elasticemail-4.1.0/test/test_paths/test_files_name/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:31.000000 elasticemail-4.1.0/test/test_paths/test_files_name/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      823 2024-05-23 09:31:31.000000 elasticemail-4.1.0/test/test_paths/test_files_name/test_delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      795 2024-05-23 09:31:31.000000 elasticemail-4.1.0/test/test_paths/test_files_name/test_get.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.251182 elasticemail-4.1.0/test/test_paths/test_files_name_info/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:31.000000 elasticemail-4.1.0/test/test_paths/test_files_name_info/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      812 2024-05-23 09:31:31.000000 elasticemail-4.1.0/test/test_paths/test_files_name_info/test_get.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.251182 elasticemail-4.1.0/test/test_paths/test_inboundroute/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:34.000000 elasticemail-4.1.0/test/test_paths/test_inboundroute/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      800 2024-05-23 09:31:34.000000 elasticemail-4.1.0/test/test_paths/test_inboundroute/test_get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      807 2024-05-23 09:31:34.000000 elasticemail-4.1.0/test/test_paths/test_inboundroute/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.255182 elasticemail-4.1.0/test/test_paths/test_inboundroute_id/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:34.000000 elasticemail-4.1.0/test/test_paths/test_inboundroute_id/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      839 2024-05-23 09:31:34.000000 elasticemail-4.1.0/test/test_paths/test_inboundroute_id/test_delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      806 2024-05-23 09:31:34.000000 elasticemail-4.1.0/test/test_paths/test_inboundroute_id/test_get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      811 2024-05-23 09:31:34.000000 elasticemail-4.1.0/test/test_paths/test_inboundroute_id/test_put.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.255182 elasticemail-4.1.0/test/test_paths/test_inboundroute_order/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:34.000000 elasticemail-4.1.0/test/test_paths/test_inboundroute_order/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      822 2024-05-23 09:31:34.000000 elasticemail-4.1.0/test/test_paths/test_inboundroute_order/test_put.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.259182 elasticemail-4.1.0/test/test_paths/test_lists/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:36.000000 elasticemail-4.1.0/test/test_paths/test_lists/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      779 2024-05-23 09:31:36.000000 elasticemail-4.1.0/test/test_paths/test_lists/test_get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      782 2024-05-23 09:31:36.000000 elasticemail-4.1.0/test/test_paths/test_lists/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.259182 elasticemail-4.1.0/test/test_paths/test_lists_name/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:36.000000 elasticemail-4.1.0/test/test_paths/test_lists_name/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      823 2024-05-23 09:31:36.000000 elasticemail-4.1.0/test/test_paths/test_lists_name/test_delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      791 2024-05-23 09:31:36.000000 elasticemail-4.1.0/test/test_paths/test_lists_name/test_get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      795 2024-05-23 09:31:36.000000 elasticemail-4.1.0/test/test_paths/test_lists_name/test_put.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.259182 elasticemail-4.1.0/test/test_paths/test_lists_name_contacts/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:36.000000 elasticemail-4.1.0/test/test_paths/test_lists_name_contacts/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      832 2024-05-23 09:31:36.000000 elasticemail-4.1.0/test/test_paths/test_lists_name_contacts/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.263182 elasticemail-4.1.0/test/test_paths/test_lists_name_contacts_remove/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:36.000000 elasticemail-4.1.0/test/test_paths/test_lists_name_contacts_remove/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      877 2024-05-23 09:31:36.000000 elasticemail-4.1.0/test/test_paths/test_lists_name_contacts_remove/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.263182 elasticemail-4.1.0/test/test_paths/test_security_apikeys/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:39.000000 elasticemail-4.1.0/test/test_paths/test_security_apikeys/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      812 2024-05-23 09:31:39.000000 elasticemail-4.1.0/test/test_paths/test_security_apikeys/test_get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      815 2024-05-23 09:31:39.000000 elasticemail-4.1.0/test/test_paths/test_security_apikeys/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.267182 elasticemail-4.1.0/test/test_paths/test_security_apikeys_name/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:39.000000 elasticemail-4.1.0/test/test_paths/test_security_apikeys_name/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      856 2024-05-23 09:31:39.000000 elasticemail-4.1.0/test/test_paths/test_security_apikeys_name/test_delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      824 2024-05-23 09:31:39.000000 elasticemail-4.1.0/test/test_paths/test_security_apikeys_name/test_get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      828 2024-05-23 09:31:39.000000 elasticemail-4.1.0/test/test_paths/test_security_apikeys_name/test_put.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.267182 elasticemail-4.1.0/test/test_paths/test_security_smtp/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:39.000000 elasticemail-4.1.0/test/test_paths/test_security_smtp/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      812 2024-05-23 09:31:39.000000 elasticemail-4.1.0/test/test_paths/test_security_smtp/test_get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      815 2024-05-23 09:31:39.000000 elasticemail-4.1.0/test/test_paths/test_security_smtp/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.271182 elasticemail-4.1.0/test/test_paths/test_security_smtp_name/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:39.000000 elasticemail-4.1.0/test/test_paths/test_security_smtp_name/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      856 2024-05-23 09:31:39.000000 elasticemail-4.1.0/test/test_paths/test_security_smtp_name/test_delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      824 2024-05-23 09:31:39.000000 elasticemail-4.1.0/test/test_paths/test_security_smtp_name/test_get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      828 2024-05-23 09:31:39.000000 elasticemail-4.1.0/test/test_paths/test_security_smtp_name/test_put.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.271182 elasticemail-4.1.0/test/test_paths/test_segments/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:41.000000 elasticemail-4.1.0/test/test_paths/test_segments/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      791 2024-05-23 09:31:41.000000 elasticemail-4.1.0/test/test_paths/test_segments/test_get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      794 2024-05-23 09:31:41.000000 elasticemail-4.1.0/test/test_paths/test_segments/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.275182 elasticemail-4.1.0/test/test_paths/test_segments_name/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:41.000000 elasticemail-4.1.0/test/test_paths/test_segments_name/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      835 2024-05-23 09:31:41.000000 elasticemail-4.1.0/test/test_paths/test_segments_name/test_delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      803 2024-05-23 09:31:41.000000 elasticemail-4.1.0/test/test_paths/test_segments_name/test_get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      807 2024-05-23 09:31:41.000000 elasticemail-4.1.0/test/test_paths/test_segments_name/test_put.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.275182 elasticemail-4.1.0/test/test_paths/test_statistics/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:42.000000 elasticemail-4.1.0/test/test_paths/test_statistics/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      799 2024-05-23 09:31:42.000000 elasticemail-4.1.0/test/test_paths/test_statistics/test_get.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.279182 elasticemail-4.1.0/test/test_paths/test_statistics_campaigns/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:42.000000 elasticemail-4.1.0/test/test_paths/test_statistics_campaigns/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      832 2024-05-23 09:31:42.000000 elasticemail-4.1.0/test/test_paths/test_statistics_campaigns/test_get.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.279182 elasticemail-4.1.0/test/test_paths/test_statistics_campaigns_name/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:42.000000 elasticemail-4.1.0/test/test_paths/test_statistics_campaigns_name/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      844 2024-05-23 09:31:42.000000 elasticemail-4.1.0/test/test_paths/test_statistics_campaigns_name/test_get.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.279182 elasticemail-4.1.0/test/test_paths/test_statistics_channels/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:42.000000 elasticemail-4.1.0/test/test_paths/test_statistics_channels/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      828 2024-05-23 09:31:42.000000 elasticemail-4.1.0/test/test_paths/test_statistics_channels/test_get.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.283182 elasticemail-4.1.0/test/test_paths/test_statistics_channels_name/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:42.000000 elasticemail-4.1.0/test/test_paths/test_statistics_channels_name/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      840 2024-05-23 09:31:42.000000 elasticemail-4.1.0/test/test_paths/test_statistics_channels_name/test_get.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.283182 elasticemail-4.1.0/test/test_paths/test_subaccounts/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:44.000000 elasticemail-4.1.0/test/test_paths/test_subaccounts/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      803 2024-05-23 09:31:44.000000 elasticemail-4.1.0/test/test_paths/test_subaccounts/test_get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      806 2024-05-23 09:31:44.000000 elasticemail-4.1.0/test/test_paths/test_subaccounts/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.287182 elasticemail-4.1.0/test/test_paths/test_subaccounts_email/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:44.000000 elasticemail-4.1.0/test/test_paths/test_subaccounts_email/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      850 2024-05-23 09:31:44.000000 elasticemail-4.1.0/test/test_paths/test_subaccounts_email/test_delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      818 2024-05-23 09:31:44.000000 elasticemail-4.1.0/test/test_paths/test_subaccounts_email/test_get.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.287182 elasticemail-4.1.0/test/test_paths/test_subaccounts_email_credits/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:44.000000 elasticemail-4.1.0/test/test_paths/test_subaccounts_email_credits/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      881 2024-05-23 09:31:44.000000 elasticemail-4.1.0/test/test_paths/test_subaccounts_email_credits/test_patch.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.291182 elasticemail-4.1.0/test/test_paths/test_subaccounts_email_settings_email/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:44.000000 elasticemail-4.1.0/test/test_paths/test_subaccounts_email_settings_email/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      878 2024-05-23 09:31:44.000000 elasticemail-4.1.0/test/test_paths/test_subaccounts_email_settings_email/test_put.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.291182 elasticemail-4.1.0/test/test_paths/test_suppressions/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:48.000000 elasticemail-4.1.0/test/test_paths/test_suppressions/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      806 2024-05-23 09:31:48.000000 elasticemail-4.1.0/test/test_paths/test_suppressions/test_get.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.291182 elasticemail-4.1.0/test/test_paths/test_suppressions_bounces/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:48.000000 elasticemail-4.1.0/test/test_paths/test_suppressions_bounces/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      827 2024-05-23 09:31:48.000000 elasticemail-4.1.0/test/test_paths/test_suppressions_bounces/test_get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      828 2024-05-23 09:31:48.000000 elasticemail-4.1.0/test/test_paths/test_suppressions_bounces/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.295182 elasticemail-4.1.0/test/test_paths/test_suppressions_bounces_import/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:48.000000 elasticemail-4.1.0/test/test_paths/test_suppressions_bounces_import/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      872 2024-05-23 09:31:48.000000 elasticemail-4.1.0/test/test_paths/test_suppressions_bounces_import/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.295182 elasticemail-4.1.0/test/test_paths/test_suppressions_complaints/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:48.000000 elasticemail-4.1.0/test/test_paths/test_suppressions_complaints/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      840 2024-05-23 09:31:48.000000 elasticemail-4.1.0/test/test_paths/test_suppressions_complaints/test_get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      840 2024-05-23 09:31:48.000000 elasticemail-4.1.0/test/test_paths/test_suppressions_complaints/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.299182 elasticemail-4.1.0/test/test_paths/test_suppressions_complaints_import/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:48.000000 elasticemail-4.1.0/test/test_paths/test_suppressions_complaints_import/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      884 2024-05-23 09:31:48.000000 elasticemail-4.1.0/test/test_paths/test_suppressions_complaints_import/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.299182 elasticemail-4.1.0/test/test_paths/test_suppressions_email/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:48.000000 elasticemail-4.1.0/test/test_paths/test_suppressions_email/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      854 2024-05-23 09:31:48.000000 elasticemail-4.1.0/test/test_paths/test_suppressions_email/test_delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      821 2024-05-23 09:31:48.000000 elasticemail-4.1.0/test/test_paths/test_suppressions_email/test_get.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.303182 elasticemail-4.1.0/test/test_paths/test_suppressions_unsubscribes/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:48.000000 elasticemail-4.1.0/test/test_paths/test_suppressions_unsubscribes/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      848 2024-05-23 09:31:48.000000 elasticemail-4.1.0/test/test_paths/test_suppressions_unsubscribes/test_get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      848 2024-05-23 09:31:48.000000 elasticemail-4.1.0/test/test_paths/test_suppressions_unsubscribes/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.303182 elasticemail-4.1.0/test/test_paths/test_suppressions_unsubscribes_import/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:48.000000 elasticemail-4.1.0/test/test_paths/test_suppressions_unsubscribes_import/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      892 2024-05-23 09:31:48.000000 elasticemail-4.1.0/test/test_paths/test_suppressions_unsubscribes_import/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.307182 elasticemail-4.1.0/test/test_paths/test_templates/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:50.000000 elasticemail-4.1.0/test/test_paths/test_templates/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      795 2024-05-23 09:31:50.000000 elasticemail-4.1.0/test/test_paths/test_templates/test_get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      798 2024-05-23 09:31:50.000000 elasticemail-4.1.0/test/test_paths/test_templates/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.307182 elasticemail-4.1.0/test/test_paths/test_templates_name/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:50.000000 elasticemail-4.1.0/test/test_paths/test_templates_name/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      839 2024-05-23 09:31:50.000000 elasticemail-4.1.0/test/test_paths/test_templates_name/test_delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      807 2024-05-23 09:31:50.000000 elasticemail-4.1.0/test/test_paths/test_templates_name/test_get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      811 2024-05-23 09:31:50.000000 elasticemail-4.1.0/test/test_paths/test_templates_name/test_put.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.311182 elasticemail-4.1.0/test/test_paths/test_verifications/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:53.000000 elasticemail-4.1.0/test/test_paths/test_verifications/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      824 2024-05-23 09:31:53.000000 elasticemail-4.1.0/test/test_paths/test_verifications/test_get.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.311182 elasticemail-4.1.0/test/test_paths/test_verifications_email/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:53.000000 elasticemail-4.1.0/test/test_paths/test_verifications_email/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      871 2024-05-23 09:31:53.000000 elasticemail-4.1.0/test/test_paths/test_verifications_email/test_delete.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      838 2024-05-23 09:31:53.000000 elasticemail-4.1.0/test/test_paths/test_verifications_email/test_get.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      824 2024-05-23 09:31:53.000000 elasticemail-4.1.0/test/test_paths/test_verifications_email/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.315182 elasticemail-4.1.0/test/test_paths/test_verifications_files/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:53.000000 elasticemail-4.1.0/test/test_paths/test_verifications_files/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      835 2024-05-23 09:31:53.000000 elasticemail-4.1.0/test/test_paths/test_verifications_files/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.315182 elasticemail-4.1.0/test/test_paths/test_verifications_files_id/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:53.000000 elasticemail-4.1.0/test/test_paths/test_verifications_files_id/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      877 2024-05-23 09:31:53.000000 elasticemail-4.1.0/test/test_paths/test_verifications_files_id/test_delete.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.319182 elasticemail-4.1.0/test/test_paths/test_verifications_files_id_result/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:53.000000 elasticemail-4.1.0/test/test_paths/test_verifications_files_id_result/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      872 2024-05-23 09:31:53.000000 elasticemail-4.1.0/test/test_paths/test_verifications_files_id_result/test_get.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.319182 elasticemail-4.1.0/test/test_paths/test_verifications_files_id_result_download/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:53.000000 elasticemail-4.1.0/test/test_paths/test_verifications_files_id_result_download/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      893 2024-05-23 09:31:53.000000 elasticemail-4.1.0/test/test_paths/test_verifications_files_id_result_download/test_get.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.319182 elasticemail-4.1.0/test/test_paths/test_verifications_files_id_verification/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:53.000000 elasticemail-4.1.0/test/test_paths/test_verifications_files_id_verification/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      895 2024-05-23 09:31:53.000000 elasticemail-4.1.0/test/test_paths/test_verifications_files_id_verification/test_post.py
+drwxrwxr-x   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:32:05.323182 elasticemail-4.1.0/test/test_paths/test_verifications_files_result/
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)        0 2024-05-23 09:31:53.000000 elasticemail-4.1.0/test/test_paths/test_verifications_files_result/__init__.py
+-rw-rw-r--   0 radzaw    (1000) radzaw    (1000)      858 2024-05-23 09:31:53.000000 elasticemail-4.1.0/test/test_paths/test_verifications_files_result/test_get.py
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/__init__.py` & `elasticemail-4.1.0/ElasticEmail/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-__version__ = "4.0.24"
+__version__ = "4.1.0"
 
 # import ApiClient
 from ElasticEmail.api_client import ApiClient
 
 # import Configuration
 from ElasticEmail.configuration import Configuration
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/api_client.py` & `elasticemail-4.1.0/ElasticEmail/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1000,15 +1000,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = HTTPHeaderDict()
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/4.0.24/python'
+        self.user_agent = 'OpenAPI-Generator/4.1.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/apis/path_to_api.py` & `elasticemail-4.1.0/ElasticEmail/apis/path_to_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from ElasticEmail.apis.paths.contacts_email import ContactsEmail
 from ElasticEmail.apis.paths.contacts_delete import ContactsDelete
 from ElasticEmail.apis.paths.contacts_export import ContactsExport
 from ElasticEmail.apis.paths.contacts_export_id_status import ContactsExportIdStatus
 from ElasticEmail.apis.paths.contacts_import import ContactsImport
 from ElasticEmail.apis.paths.emails import Emails
 from ElasticEmail.apis.paths.emails_msgid_view import EmailsMsgidView
+from ElasticEmail.apis.paths.emails_transactionid_status import EmailsTransactionidStatus
 from ElasticEmail.apis.paths.emails_mergefile import EmailsMergefile
 from ElasticEmail.apis.paths.emails_transactional import EmailsTransactional
 from ElasticEmail.apis.paths.events import Events
 from ElasticEmail.apis.paths.events_transactionid import EventsTransactionid
 from ElasticEmail.apis.paths.events_channels_name import EventsChannelsName
 from ElasticEmail.apis.paths.events_channels_name_export import EventsChannelsNameExport
 from ElasticEmail.apis.paths.events_channels_export_id_status import EventsChannelsExportIdStatus
@@ -73,14 +74,15 @@
         PathValues.CONTACTS_EMAIL: ContactsEmail,
         PathValues.CONTACTS_DELETE: ContactsDelete,
         PathValues.CONTACTS_EXPORT: ContactsExport,
         PathValues.CONTACTS_EXPORT_ID_STATUS: ContactsExportIdStatus,
         PathValues.CONTACTS_IMPORT: ContactsImport,
         PathValues.EMAILS: Emails,
         PathValues.EMAILS_MSGID_VIEW: EmailsMsgidView,
+        PathValues.EMAILS_TRANSACTIONID_STATUS: EmailsTransactionidStatus,
         PathValues.EMAILS_MERGEFILE: EmailsMergefile,
         PathValues.EMAILS_TRANSACTIONAL: EmailsTransactional,
         PathValues.EVENTS: Events,
         PathValues.EVENTS_TRANSACTIONID: EventsTransactionid,
         PathValues.EVENTS_CHANNELS_NAME: EventsChannelsName,
         PathValues.EVENTS_CHANNELS_NAME_EXPORT: EventsChannelsNameExport,
         PathValues.EVENTS_CHANNELS_EXPORT_ID_STATUS: EventsChannelsExportIdStatus,
@@ -140,14 +142,15 @@
         PathValues.CONTACTS_EMAIL: ContactsEmail,
         PathValues.CONTACTS_DELETE: ContactsDelete,
         PathValues.CONTACTS_EXPORT: ContactsExport,
         PathValues.CONTACTS_EXPORT_ID_STATUS: ContactsExportIdStatus,
         PathValues.CONTACTS_IMPORT: ContactsImport,
         PathValues.EMAILS: Emails,
         PathValues.EMAILS_MSGID_VIEW: EmailsMsgidView,
+        PathValues.EMAILS_TRANSACTIONID_STATUS: EmailsTransactionidStatus,
         PathValues.EMAILS_MERGEFILE: EmailsMergefile,
         PathValues.EMAILS_TRANSACTIONAL: EmailsTransactional,
         PathValues.EVENTS: Events,
         PathValues.EVENTS_TRANSACTIONID: EventsTransactionid,
         PathValues.EVENTS_CHANNELS_NAME: EventsChannelsName,
         PathValues.EVENTS_CHANNELS_NAME_EXPORT: EventsChannelsNameExport,
         PathValues.EVENTS_CHANNELS_EXPORT_ID_STATUS: EventsChannelsExportIdStatus,
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/apis/tag_to_api.py` & `elasticemail-4.1.0/ElasticEmail/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/apis/tags/__init__.py` & `elasticemail-4.1.0/ElasticEmail/apis/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/apis/tags/campaigns_api.py` & `elasticemail-4.1.0/ElasticEmail/apis/tags/campaigns_api.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/apis/tags/contacts_api.py` & `elasticemail-4.1.0/ElasticEmail/apis/tags/contacts_api.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/apis/tags/emails_api.py` & `elasticemail-4.1.0/ElasticEmail/apis/tags/emails_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 from ElasticEmail.paths.emails_msgid_view.get import EmailsByMsgidViewGet
+from ElasticEmail.paths.emails_transactionid_status.get import EmailsByTransactionidStatusGet
 from ElasticEmail.paths.emails_mergefile.post import EmailsMergefilePost
 from ElasticEmail.paths.emails.post import EmailsPost
 from ElasticEmail.paths.emails_transactional.post import EmailsTransactionalPost
 
 
 class EmailsApi(
     EmailsByMsgidViewGet,
+    EmailsByTransactionidStatusGet,
     EmailsMergefilePost,
     EmailsPost,
     EmailsTransactionalPost,
 ):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/apis/tags/events_api.py` & `elasticemail-4.1.0/ElasticEmail/apis/tags/events_api.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/apis/tags/files_api.py` & `elasticemail-4.1.0/ElasticEmail/apis/tags/files_api.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/apis/tags/inbound_route_api.py` & `elasticemail-4.1.0/ElasticEmail/apis/tags/inbound_route_api.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/apis/tags/lists_api.py` & `elasticemail-4.1.0/ElasticEmail/apis/tags/lists_api.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/apis/tags/security_api.py` & `elasticemail-4.1.0/ElasticEmail/apis/tags/security_api.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/apis/tags/segments_api.py` & `elasticemail-4.1.0/ElasticEmail/apis/tags/segments_api.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/apis/tags/statistics_api.py` & `elasticemail-4.1.0/ElasticEmail/apis/tags/statistics_api.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/apis/tags/sub_accounts_api.py` & `elasticemail-4.1.0/ElasticEmail/apis/tags/sub_accounts_api.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/apis/tags/suppressions_api.py` & `elasticemail-4.1.0/ElasticEmail/apis/tags/suppressions_api.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/apis/tags/templates_api.py` & `elasticemail-4.1.0/ElasticEmail/apis/tags/templates_api.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/apis/tags/verifications_api.py` & `elasticemail-4.1.0/ElasticEmail/apis/tags/verifications_api.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/configuration.py` & `elasticemail-4.1.0/ElasticEmail/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,15 +397,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 4.0.0\n"\
-               "SDK Package Version: 4.0.24".\
+               "SDK Package Version: 4.1.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/exceptions.py` & `elasticemail-4.1.0/ElasticEmail/exceptions.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/access_level.py` & `elasticemail-4.1.0/ElasticEmail/model/access_level.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,21 +77,21 @@
             "ModifySupport": "MODIFY_SUPPORT",
             "ViewCustomFields": "VIEW_CUSTOM_FIELDS",
             "ModifyCustomFields": "MODIFY_CUSTOM_FIELDS",
             "ModifyWebNotifications": "MODIFY_WEB_NOTIFICATIONS",
             "ExtendedLogs": "EXTENDED_LOGS",
             "VerifyEmails": "VERIFY_EMAILS",
             "Modify2FASms": "MODIFY2FASMS",
-            "DisableContactsStore": "DISABLE_CONTACTS_STORE",
             "ModifyLandingPages": "MODIFY_LANDING_PAGES",
             "ViewLandingPages": "VIEW_LANDING_PAGES",
             "ModifySuppressions": "MODIFY_SUPPRESSIONS",
             "ViewSuppressions": "VIEW_SUPPRESSIONS",
             "ViewDragDropEditor": "VIEW_DRAG_DROP_EDITOR",
             "ViewTemplateEditor": "VIEW_TEMPLATE_EDITOR",
+            "ViewAITools": "VIEW_AITOOLS",
         }
     
     @schemas.classproperty
     def NONE(cls):
         return cls("None")
     
     @schemas.classproperty
@@ -263,18 +263,14 @@
         return cls("VerifyEmails")
     
     @schemas.classproperty
     def MODIFY2FASMS(cls):
         return cls("Modify2FASms")
     
     @schemas.classproperty
-    def DISABLE_CONTACTS_STORE(cls):
-        return cls("DisableContactsStore")
-    
-    @schemas.classproperty
     def MODIFY_LANDING_PAGES(cls):
         return cls("ModifyLandingPages")
     
     @schemas.classproperty
     def VIEW_LANDING_PAGES(cls):
         return cls("ViewLandingPages")
     
@@ -289,7 +285,11 @@
     @schemas.classproperty
     def VIEW_DRAG_DROP_EDITOR(cls):
         return cls("ViewDragDropEditor")
     
     @schemas.classproperty
     def VIEW_TEMPLATE_EDITOR(cls):
         return cls("ViewTemplateEditor")
+    
+    @schemas.classproperty
+    def VIEW_AITOOLS(cls):
+        return cls("ViewAITools")
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/access_level.pyi` & `elasticemail-4.1.0/ElasticEmail/model/access_level.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -207,18 +207,14 @@
         return cls("VerifyEmails")
     
     @schemas.classproperty
     def MODIFY2FASMS(cls):
         return cls("Modify2FASms")
     
     @schemas.classproperty
-    def DISABLE_CONTACTS_STORE(cls):
-        return cls("DisableContactsStore")
-    
-    @schemas.classproperty
     def MODIFY_LANDING_PAGES(cls):
         return cls("ModifyLandingPages")
     
     @schemas.classproperty
     def VIEW_LANDING_PAGES(cls):
         return cls("ViewLandingPages")
     
@@ -233,7 +229,11 @@
     @schemas.classproperty
     def VIEW_DRAG_DROP_EDITOR(cls):
         return cls("ViewDragDropEditor")
     
     @schemas.classproperty
     def VIEW_TEMPLATE_EDITOR(cls):
         return cls("ViewTemplateEditor")
+    
+    @schemas.classproperty
+    def VIEW_AITOOLS(cls):
+        return cls("ViewAITools")
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/account_status_enum.py` & `elasticemail-4.1.0/ElasticEmail/model/account_status_enum.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/account_status_enum.pyi` & `elasticemail-4.1.0/ElasticEmail/model/account_status_enum.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/api_key.py` & `elasticemail-4.1.0/ElasticEmail/model/api_key.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/api_key.pyi` & `elasticemail-4.1.0/ElasticEmail/model/api_key.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/api_key_payload.py` & `elasticemail-4.1.0/ElasticEmail/model/api_key_payload.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/api_key_payload.pyi` & `elasticemail-4.1.0/ElasticEmail/model/api_key_payload.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/body_content_type.py` & `elasticemail-4.1.0/ElasticEmail/model/body_content_type.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/body_content_type.pyi` & `elasticemail-4.1.0/ElasticEmail/model/body_content_type.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/body_part.py` & `elasticemail-4.1.0/ElasticEmail/model/body_part.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/body_part.pyi` & `elasticemail-4.1.0/ElasticEmail/model/body_part.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/campaign.py` & `elasticemail-4.1.0/ElasticEmail/model/campaign.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/campaign.pyi` & `elasticemail-4.1.0/ElasticEmail/model/campaign.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/campaign_options.py` & `elasticemail-4.1.0/ElasticEmail/model/campaign_options.py`

 * *Files 18% similar despite different names*

```diff
@@ -112,23 +112,27 @@
                     _configuration: typing.Optional[schemas.Configuration] = None,
                 ) -> 'ScheduleFor':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                     )
+            TriggerFrequency = schemas.Float64Schema
+            TriggerCount = schemas.Int32Schema
         
             @staticmethod
             def SplitOptions() -> typing.Type['SplitOptions']:
                 return SplitOptions
             __annotations__ = {
                 "DeliveryOptimization": DeliveryOptimization,
                 "TrackOpens": TrackOpens,
                 "TrackClicks": TrackClicks,
                 "ScheduleFor": ScheduleFor,
+                "TriggerFrequency": TriggerFrequency,
+                "TriggerCount": TriggerCount,
                 "SplitOptions": SplitOptions,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["DeliveryOptimization"]) -> 'DeliveryOptimizationType': ...
     
     @typing.overload
@@ -137,20 +141,26 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["TrackClicks"]) -> MetaOapg.properties.TrackClicks: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["ScheduleFor"]) -> MetaOapg.properties.ScheduleFor: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["TriggerFrequency"]) -> MetaOapg.properties.TriggerFrequency: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["TriggerCount"]) -> MetaOapg.properties.TriggerCount: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["SplitOptions"]) -> 'SplitOptions': ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["DeliveryOptimization", "TrackOpens", "TrackClicks", "ScheduleFor", "SplitOptions", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["DeliveryOptimization", "TrackOpens", "TrackClicks", "ScheduleFor", "TriggerFrequency", "TriggerCount", "SplitOptions", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["DeliveryOptimization"]) -> typing.Union['DeliveryOptimizationType', schemas.Unset]: ...
     
@@ -160,41 +170,51 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["TrackClicks"]) -> typing.Union[MetaOapg.properties.TrackClicks, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["ScheduleFor"]) -> typing.Union[MetaOapg.properties.ScheduleFor, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["TriggerFrequency"]) -> typing.Union[MetaOapg.properties.TriggerFrequency, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["TriggerCount"]) -> typing.Union[MetaOapg.properties.TriggerCount, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["SplitOptions"]) -> typing.Union['SplitOptions', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["DeliveryOptimization", "TrackOpens", "TrackClicks", "ScheduleFor", "SplitOptions", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["DeliveryOptimization", "TrackOpens", "TrackClicks", "ScheduleFor", "TriggerFrequency", "TriggerCount", "SplitOptions", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         DeliveryOptimization: typing.Union['DeliveryOptimizationType', schemas.Unset] = schemas.unset,
         TrackOpens: typing.Union[MetaOapg.properties.TrackOpens, None, bool, schemas.Unset] = schemas.unset,
         TrackClicks: typing.Union[MetaOapg.properties.TrackClicks, None, bool, schemas.Unset] = schemas.unset,
         ScheduleFor: typing.Union[MetaOapg.properties.ScheduleFor, None, str, datetime, schemas.Unset] = schemas.unset,
+        TriggerFrequency: typing.Union[MetaOapg.properties.TriggerFrequency, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        TriggerCount: typing.Union[MetaOapg.properties.TriggerCount, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         SplitOptions: typing.Union['SplitOptions', schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'CampaignOptions':
         return super().__new__(
             cls,
             *_args,
             DeliveryOptimization=DeliveryOptimization,
             TrackOpens=TrackOpens,
             TrackClicks=TrackClicks,
             ScheduleFor=ScheduleFor,
+            TriggerFrequency=TriggerFrequency,
+            TriggerCount=TriggerCount,
             SplitOptions=SplitOptions,
             _configuration=_configuration,
             **kwargs,
         )
 
 from ElasticEmail.model.delivery_optimization_type import DeliveryOptimizationType
 from ElasticEmail.model.split_options import SplitOptions
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/campaign_options.pyi` & `elasticemail-4.1.0/ElasticEmail/model/campaign_options.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -112,23 +112,27 @@
                     _configuration: typing.Optional[schemas.Configuration] = None,
                 ) -> 'ScheduleFor':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                     )
+            TriggerFrequency = schemas.Float64Schema
+            TriggerCount = schemas.Int32Schema
         
             @staticmethod
             def SplitOptions() -> typing.Type['SplitOptions']:
                 return SplitOptions
             __annotations__ = {
                 "DeliveryOptimization": DeliveryOptimization,
                 "TrackOpens": TrackOpens,
                 "TrackClicks": TrackClicks,
                 "ScheduleFor": ScheduleFor,
+                "TriggerFrequency": TriggerFrequency,
+                "TriggerCount": TriggerCount,
                 "SplitOptions": SplitOptions,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["DeliveryOptimization"]) -> 'DeliveryOptimizationType': ...
     
     @typing.overload
@@ -137,20 +141,26 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["TrackClicks"]) -> MetaOapg.properties.TrackClicks: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["ScheduleFor"]) -> MetaOapg.properties.ScheduleFor: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["TriggerFrequency"]) -> MetaOapg.properties.TriggerFrequency: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["TriggerCount"]) -> MetaOapg.properties.TriggerCount: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["SplitOptions"]) -> 'SplitOptions': ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["DeliveryOptimization", "TrackOpens", "TrackClicks", "ScheduleFor", "SplitOptions", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["DeliveryOptimization", "TrackOpens", "TrackClicks", "ScheduleFor", "TriggerFrequency", "TriggerCount", "SplitOptions", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["DeliveryOptimization"]) -> typing.Union['DeliveryOptimizationType', schemas.Unset]: ...
     
@@ -160,41 +170,51 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["TrackClicks"]) -> typing.Union[MetaOapg.properties.TrackClicks, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["ScheduleFor"]) -> typing.Union[MetaOapg.properties.ScheduleFor, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["TriggerFrequency"]) -> typing.Union[MetaOapg.properties.TriggerFrequency, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["TriggerCount"]) -> typing.Union[MetaOapg.properties.TriggerCount, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["SplitOptions"]) -> typing.Union['SplitOptions', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["DeliveryOptimization", "TrackOpens", "TrackClicks", "ScheduleFor", "SplitOptions", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["DeliveryOptimization", "TrackOpens", "TrackClicks", "ScheduleFor", "TriggerFrequency", "TriggerCount", "SplitOptions", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         DeliveryOptimization: typing.Union['DeliveryOptimizationType', schemas.Unset] = schemas.unset,
         TrackOpens: typing.Union[MetaOapg.properties.TrackOpens, None, bool, schemas.Unset] = schemas.unset,
         TrackClicks: typing.Union[MetaOapg.properties.TrackClicks, None, bool, schemas.Unset] = schemas.unset,
         ScheduleFor: typing.Union[MetaOapg.properties.ScheduleFor, None, str, datetime, schemas.Unset] = schemas.unset,
+        TriggerFrequency: typing.Union[MetaOapg.properties.TriggerFrequency, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        TriggerCount: typing.Union[MetaOapg.properties.TriggerCount, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         SplitOptions: typing.Union['SplitOptions', schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'CampaignOptions':
         return super().__new__(
             cls,
             *_args,
             DeliveryOptimization=DeliveryOptimization,
             TrackOpens=TrackOpens,
             TrackClicks=TrackClicks,
             ScheduleFor=ScheduleFor,
+            TriggerFrequency=TriggerFrequency,
+            TriggerCount=TriggerCount,
             SplitOptions=SplitOptions,
             _configuration=_configuration,
             **kwargs,
         )
 
 from ElasticEmail.model.delivery_optimization_type import DeliveryOptimizationType
 from ElasticEmail.model.split_options import SplitOptions
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/campaign_recipient.py` & `elasticemail-4.1.0/ElasticEmail/model/campaign_recipient.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/campaign_recipient.pyi` & `elasticemail-4.1.0/ElasticEmail/model/campaign_recipient.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/campaign_status.py` & `elasticemail-4.1.0/ElasticEmail/model/campaign_status.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/campaign_status.pyi` & `elasticemail-4.1.0/ElasticEmail/model/campaign_status.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/campaign_template.py` & `elasticemail-4.1.0/ElasticEmail/model/campaign_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,21 @@
     Do not edit the class manually.
 
     Content of a Campaign
     """
 
 
     class MetaOapg:
+        required = {
+            "From",
+        }
         
         class properties:
-            Poolname = schemas.StrSchema
             _from = schemas.StrSchema
+            Poolname = schemas.StrSchema
             ReplyTo = schemas.StrSchema
             Subject = schemas.StrSchema
             TemplateName = schemas.StrSchema
             
             
             class AttachFiles(
                 schemas.ListSchema
@@ -68,30 +71,31 @@
                 def __getitem__(self, i: int) -> MetaOapg.items:
                     return super().__getitem__(i)
         
             @staticmethod
             def Utm() -> typing.Type['Utm']:
                 return Utm
             __annotations__ = {
-                "Poolname": Poolname,
                 "From": _from,
+                "Poolname": Poolname,
                 "ReplyTo": ReplyTo,
                 "Subject": Subject,
                 "TemplateName": TemplateName,
                 "AttachFiles": AttachFiles,
                 "Utm": Utm,
             }
     
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Poolname"]) -> MetaOapg.properties.Poolname: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["From"]) -> MetaOapg.properties._from: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["Poolname"]) -> MetaOapg.properties.Poolname: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["ReplyTo"]) -> MetaOapg.properties.ReplyTo: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Subject"]) -> MetaOapg.properties.Subject: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["TemplateName"]) -> MetaOapg.properties.TemplateName: ...
@@ -101,24 +105,24 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Utm"]) -> 'Utm': ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["Poolname", "From", "ReplyTo", "Subject", "TemplateName", "AttachFiles", "Utm", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["From", "Poolname", "ReplyTo", "Subject", "TemplateName", "AttachFiles", "Utm", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Poolname"]) -> typing.Union[MetaOapg.properties.Poolname, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["From"]) -> MetaOapg.properties._from: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["From"]) -> typing.Union[MetaOapg.properties._from, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["Poolname"]) -> typing.Union[MetaOapg.properties.Poolname, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["ReplyTo"]) -> typing.Union[MetaOapg.properties.ReplyTo, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Subject"]) -> typing.Union[MetaOapg.properties.Subject, schemas.Unset]: ...
     
@@ -130,15 +134,15 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Utm"]) -> typing.Union['Utm', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["Poolname", "From", "ReplyTo", "Subject", "TemplateName", "AttachFiles", "Utm", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["From", "Poolname", "ReplyTo", "Subject", "TemplateName", "AttachFiles", "Utm", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         Poolname: typing.Union[MetaOapg.properties.Poolname, str, schemas.Unset] = schemas.unset,
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/campaign_template.pyi` & `elasticemail-4.1.0/ElasticEmail/model/campaign_template.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,21 @@
     Do not edit the class manually.
 
     Content of a Campaign
     """
 
 
     class MetaOapg:
+        required = {
+            "From",
+        }
         
         class properties:
-            Poolname = schemas.StrSchema
             _from = schemas.StrSchema
+            Poolname = schemas.StrSchema
             ReplyTo = schemas.StrSchema
             Subject = schemas.StrSchema
             TemplateName = schemas.StrSchema
             
             
             class AttachFiles(
                 schemas.ListSchema
@@ -68,30 +71,31 @@
                 def __getitem__(self, i: int) -> MetaOapg.items:
                     return super().__getitem__(i)
         
             @staticmethod
             def Utm() -> typing.Type['Utm']:
                 return Utm
             __annotations__ = {
-                "Poolname": Poolname,
                 "From": _from,
+                "Poolname": Poolname,
                 "ReplyTo": ReplyTo,
                 "Subject": Subject,
                 "TemplateName": TemplateName,
                 "AttachFiles": AttachFiles,
                 "Utm": Utm,
             }
     
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Poolname"]) -> MetaOapg.properties.Poolname: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["From"]) -> MetaOapg.properties._from: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["Poolname"]) -> MetaOapg.properties.Poolname: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["ReplyTo"]) -> MetaOapg.properties.ReplyTo: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Subject"]) -> MetaOapg.properties.Subject: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["TemplateName"]) -> MetaOapg.properties.TemplateName: ...
@@ -101,24 +105,24 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Utm"]) -> 'Utm': ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["Poolname", "From", "ReplyTo", "Subject", "TemplateName", "AttachFiles", "Utm", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["From", "Poolname", "ReplyTo", "Subject", "TemplateName", "AttachFiles", "Utm", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Poolname"]) -> typing.Union[MetaOapg.properties.Poolname, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["From"]) -> MetaOapg.properties._from: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["From"]) -> typing.Union[MetaOapg.properties._from, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["Poolname"]) -> typing.Union[MetaOapg.properties.Poolname, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["ReplyTo"]) -> typing.Union[MetaOapg.properties.ReplyTo, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Subject"]) -> typing.Union[MetaOapg.properties.Subject, schemas.Unset]: ...
     
@@ -130,15 +134,15 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Utm"]) -> typing.Union['Utm', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["Poolname", "From", "ReplyTo", "Subject", "TemplateName", "AttachFiles", "Utm", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["From", "Poolname", "ReplyTo", "Subject", "TemplateName", "AttachFiles", "Utm", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         Poolname: typing.Union[MetaOapg.properties.Poolname, str, schemas.Unset] = schemas.unset,
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/channel_log_status_summary.py` & `elasticemail-4.1.0/ElasticEmail/model/channel_log_status_summary.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/channel_log_status_summary.pyi` & `elasticemail-4.1.0/ElasticEmail/model/channel_log_status_summary.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/compression_format.py` & `elasticemail-4.1.0/ElasticEmail/model/compression_format.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/compression_format.pyi` & `elasticemail-4.1.0/ElasticEmail/model/compression_format.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/consent_data.py` & `elasticemail-4.1.0/ElasticEmail/model/consent_data.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/consent_data.pyi` & `elasticemail-4.1.0/ElasticEmail/model/consent_data.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/consent_tracking.py` & `elasticemail-4.1.0/ElasticEmail/model/consent_tracking.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/consent_tracking.pyi` & `elasticemail-4.1.0/ElasticEmail/model/consent_tracking.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/contact.py` & `elasticemail-4.1.0/ElasticEmail/model/contact.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/contact.pyi` & `elasticemail-4.1.0/ElasticEmail/model/contact.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/contact_activity.py` & `elasticemail-4.1.0/ElasticEmail/model/contact_activity.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/contact_activity.pyi` & `elasticemail-4.1.0/ElasticEmail/model/contact_activity.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/contact_payload.py` & `elasticemail-4.1.0/ElasticEmail/model/contact_payload.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/contact_payload.pyi` & `elasticemail-4.1.0/ElasticEmail/model/contact_payload.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/contact_source.py` & `elasticemail-4.1.0/ElasticEmail/model/contact_source.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/contact_source.pyi` & `elasticemail-4.1.0/ElasticEmail/model/contact_source.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/contact_status.py` & `elasticemail-4.1.0/ElasticEmail/model/contact_status.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/contact_status.pyi` & `elasticemail-4.1.0/ElasticEmail/model/contact_status.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/contact_update_payload.py` & `elasticemail-4.1.0/ElasticEmail/model/contact_update_payload.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/contact_update_payload.pyi` & `elasticemail-4.1.0/ElasticEmail/model/contact_update_payload.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/contacts_list.py` & `elasticemail-4.1.0/ElasticEmail/model/contacts_list.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/contacts_list.pyi` & `elasticemail-4.1.0/ElasticEmail/model/contacts_list.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/delivery_optimization_type.py` & `elasticemail-4.1.0/ElasticEmail/model/delivery_optimization_type.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/delivery_optimization_type.pyi` & `elasticemail-4.1.0/ElasticEmail/model/delivery_optimization_type.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/email_content.py` & `elasticemail-4.1.0/ElasticEmail/model/email_content.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,16 +33,20 @@
     Do not edit the class manually.
 
     Proper e-mail content
     """
 
 
     class MetaOapg:
+        required = {
+            "From",
+        }
         
         class properties:
+            _from = schemas.StrSchema
             
             
             class Body(
                 schemas.ListSchema
             ):
             
             
@@ -147,15 +151,14 @@
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             Postback = schemas.StrSchema
             EnvelopeFrom = schemas.StrSchema
-            _from = schemas.StrSchema
             ReplyTo = schemas.StrSchema
             Subject = schemas.StrSchema
             TemplateName = schemas.StrSchema
             
             
             class AttachFiles(
                 schemas.ListSchema
@@ -179,28 +182,32 @@
                 def __getitem__(self, i: int) -> MetaOapg.items:
                     return super().__getitem__(i)
         
             @staticmethod
             def Utm() -> typing.Type['Utm']:
                 return Utm
             __annotations__ = {
+                "From": _from,
                 "Body": Body,
                 "Merge": Merge,
                 "Attachments": Attachments,
                 "Headers": Headers,
                 "Postback": Postback,
                 "EnvelopeFrom": EnvelopeFrom,
-                "From": _from,
                 "ReplyTo": ReplyTo,
                 "Subject": Subject,
                 "TemplateName": TemplateName,
                 "AttachFiles": AttachFiles,
                 "Utm": Utm,
             }
     
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["From"]) -> MetaOapg.properties._from: ...
+    
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Body"]) -> MetaOapg.properties.Body: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Merge"]) -> MetaOapg.properties.Merge: ...
     
     @typing.overload
@@ -212,17 +219,14 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Postback"]) -> MetaOapg.properties.Postback: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["EnvelopeFrom"]) -> MetaOapg.properties.EnvelopeFrom: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["From"]) -> MetaOapg.properties._from: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["ReplyTo"]) -> MetaOapg.properties.ReplyTo: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Subject"]) -> MetaOapg.properties.Subject: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["TemplateName"]) -> MetaOapg.properties.TemplateName: ...
@@ -232,20 +236,23 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Utm"]) -> 'Utm': ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["Body", "Merge", "Attachments", "Headers", "Postback", "EnvelopeFrom", "From", "ReplyTo", "Subject", "TemplateName", "AttachFiles", "Utm", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["From", "Body", "Merge", "Attachments", "Headers", "Postback", "EnvelopeFrom", "ReplyTo", "Subject", "TemplateName", "AttachFiles", "Utm", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["From"]) -> MetaOapg.properties._from: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Body"]) -> typing.Union[MetaOapg.properties.Body, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Merge"]) -> typing.Union[MetaOapg.properties.Merge, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Attachments"]) -> typing.Union[MetaOapg.properties.Attachments, schemas.Unset]: ...
@@ -256,17 +263,14 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Postback"]) -> typing.Union[MetaOapg.properties.Postback, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["EnvelopeFrom"]) -> typing.Union[MetaOapg.properties.EnvelopeFrom, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["From"]) -> typing.Union[MetaOapg.properties._from, schemas.Unset]: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["ReplyTo"]) -> typing.Union[MetaOapg.properties.ReplyTo, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Subject"]) -> typing.Union[MetaOapg.properties.Subject, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["TemplateName"]) -> typing.Union[MetaOapg.properties.TemplateName, schemas.Unset]: ...
@@ -276,15 +280,15 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Utm"]) -> typing.Union['Utm', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["Body", "Merge", "Attachments", "Headers", "Postback", "EnvelopeFrom", "From", "ReplyTo", "Subject", "TemplateName", "AttachFiles", "Utm", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["From", "Body", "Merge", "Attachments", "Headers", "Postback", "EnvelopeFrom", "ReplyTo", "Subject", "TemplateName", "AttachFiles", "Utm", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         Body: typing.Union[MetaOapg.properties.Body, list, tuple, schemas.Unset] = schemas.unset,
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/email_content.pyi` & `elasticemail-4.1.0/ElasticEmail/model/email_content.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -33,16 +33,20 @@
     Do not edit the class manually.
 
     Proper e-mail content
     """
 
 
     class MetaOapg:
+        required = {
+            "From",
+        }
         
         class properties:
+            _from = schemas.StrSchema
             
             
             class Body(
                 schemas.ListSchema
             ):
             
             
@@ -147,15 +151,14 @@
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             Postback = schemas.StrSchema
             EnvelopeFrom = schemas.StrSchema
-            _from = schemas.StrSchema
             ReplyTo = schemas.StrSchema
             Subject = schemas.StrSchema
             TemplateName = schemas.StrSchema
             
             
             class AttachFiles(
                 schemas.ListSchema
@@ -179,28 +182,32 @@
                 def __getitem__(self, i: int) -> MetaOapg.items:
                     return super().__getitem__(i)
         
             @staticmethod
             def Utm() -> typing.Type['Utm']:
                 return Utm
             __annotations__ = {
+                "From": _from,
                 "Body": Body,
                 "Merge": Merge,
                 "Attachments": Attachments,
                 "Headers": Headers,
                 "Postback": Postback,
                 "EnvelopeFrom": EnvelopeFrom,
-                "From": _from,
                 "ReplyTo": ReplyTo,
                 "Subject": Subject,
                 "TemplateName": TemplateName,
                 "AttachFiles": AttachFiles,
                 "Utm": Utm,
             }
     
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["From"]) -> MetaOapg.properties._from: ...
+    
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Body"]) -> MetaOapg.properties.Body: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Merge"]) -> MetaOapg.properties.Merge: ...
     
     @typing.overload
@@ -212,17 +219,14 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Postback"]) -> MetaOapg.properties.Postback: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["EnvelopeFrom"]) -> MetaOapg.properties.EnvelopeFrom: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["From"]) -> MetaOapg.properties._from: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["ReplyTo"]) -> MetaOapg.properties.ReplyTo: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Subject"]) -> MetaOapg.properties.Subject: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["TemplateName"]) -> MetaOapg.properties.TemplateName: ...
@@ -232,20 +236,23 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Utm"]) -> 'Utm': ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["Body", "Merge", "Attachments", "Headers", "Postback", "EnvelopeFrom", "From", "ReplyTo", "Subject", "TemplateName", "AttachFiles", "Utm", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["From", "Body", "Merge", "Attachments", "Headers", "Postback", "EnvelopeFrom", "ReplyTo", "Subject", "TemplateName", "AttachFiles", "Utm", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["From"]) -> MetaOapg.properties._from: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Body"]) -> typing.Union[MetaOapg.properties.Body, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Merge"]) -> typing.Union[MetaOapg.properties.Merge, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Attachments"]) -> typing.Union[MetaOapg.properties.Attachments, schemas.Unset]: ...
@@ -256,17 +263,14 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Postback"]) -> typing.Union[MetaOapg.properties.Postback, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["EnvelopeFrom"]) -> typing.Union[MetaOapg.properties.EnvelopeFrom, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["From"]) -> typing.Union[MetaOapg.properties._from, schemas.Unset]: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["ReplyTo"]) -> typing.Union[MetaOapg.properties.ReplyTo, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Subject"]) -> typing.Union[MetaOapg.properties.Subject, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["TemplateName"]) -> typing.Union[MetaOapg.properties.TemplateName, schemas.Unset]: ...
@@ -276,15 +280,15 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Utm"]) -> typing.Union['Utm', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["Body", "Merge", "Attachments", "Headers", "Postback", "EnvelopeFrom", "From", "ReplyTo", "Subject", "TemplateName", "AttachFiles", "Utm", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["From", "Body", "Merge", "Attachments", "Headers", "Postback", "EnvelopeFrom", "ReplyTo", "Subject", "TemplateName", "AttachFiles", "Utm", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         Body: typing.Union[MetaOapg.properties.Body, list, tuple, schemas.Unset] = schemas.unset,
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/email_data.py` & `elasticemail-4.1.0/ElasticEmail/model/email_data.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/email_data.pyi` & `elasticemail-4.1.0/ElasticEmail/model/email_data.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/email_message_data.py` & `elasticemail-4.1.0/ElasticEmail/model/email_message_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     Email data
     """
 
 
     class MetaOapg:
         required = {
             "Recipients",
+            "Content",
         }
         
         class properties:
             
             
             class Recipients(
                 schemas.ListSchema
@@ -79,14 +80,15 @@
             __annotations__ = {
                 "Recipients": Recipients,
                 "Content": Content,
                 "Options": Options,
             }
     
     Recipients: MetaOapg.properties.Recipients
+    Content: 'EmailContent'
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Recipients"]) -> MetaOapg.properties.Recipients: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Content"]) -> 'EmailContent': ...
     
@@ -101,15 +103,15 @@
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Recipients"]) -> MetaOapg.properties.Recipients: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Content"]) -> typing.Union['EmailContent', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["Content"]) -> 'EmailContent': ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Options"]) -> typing.Union['Options', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
@@ -117,15 +119,15 @@
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         Recipients: typing.Union[MetaOapg.properties.Recipients, list, tuple, ],
-        Content: typing.Union['EmailContent', schemas.Unset] = schemas.unset,
+        Content: 'EmailContent',
         Options: typing.Union['Options', schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'EmailMessageData':
         return super().__new__(
             cls,
             *_args,
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/email_message_data.pyi` & `elasticemail-4.1.0/ElasticEmail/model/email_message_data.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     Email data
     """
 
 
     class MetaOapg:
         required = {
             "Recipients",
+            "Content",
         }
         
         class properties:
             
             
             class Recipients(
                 schemas.ListSchema
@@ -79,14 +80,15 @@
             __annotations__ = {
                 "Recipients": Recipients,
                 "Content": Content,
                 "Options": Options,
             }
     
     Recipients: MetaOapg.properties.Recipients
+    Content: 'EmailContent'
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Recipients"]) -> MetaOapg.properties.Recipients: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Content"]) -> 'EmailContent': ...
     
@@ -101,15 +103,15 @@
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Recipients"]) -> MetaOapg.properties.Recipients: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Content"]) -> typing.Union['EmailContent', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["Content"]) -> 'EmailContent': ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Options"]) -> typing.Union['Options', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
@@ -117,15 +119,15 @@
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         Recipients: typing.Union[MetaOapg.properties.Recipients, list, tuple, ],
-        Content: typing.Union['EmailContent', schemas.Unset] = schemas.unset,
+        Content: 'EmailContent',
         Options: typing.Union['Options', schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'EmailMessageData':
         return super().__new__(
             cls,
             *_args,
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/email_predicted_validation_status.py` & `elasticemail-4.1.0/ElasticEmail/model/email_predicted_validation_status.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/email_predicted_validation_status.pyi` & `elasticemail-4.1.0/ElasticEmail/model/email_predicted_validation_status.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/email_recipient.py` & `elasticemail-4.1.0/ElasticEmail/model/email_recipient.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/email_recipient.pyi` & `elasticemail-4.1.0/ElasticEmail/model/email_recipient.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/email_send.py` & `elasticemail-4.1.0/ElasticEmail/model/email_send.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/email_send.pyi` & `elasticemail-4.1.0/ElasticEmail/model/email_send.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/email_status.py` & `elasticemail-4.1.0/ElasticEmail/model/email_status.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/email_status.pyi` & `elasticemail-4.1.0/ElasticEmail/model/email_status.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/email_transactional_message_data.py` & `elasticemail-4.1.0/ElasticEmail/model/email_transactional_message_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     Email data
     """
 
 
     class MetaOapg:
         required = {
             "Recipients",
+            "Content",
         }
         
         class properties:
         
             @staticmethod
             def Recipients() -> typing.Type['TransactionalRecipient']:
                 return TransactionalRecipient
@@ -57,14 +58,15 @@
             __annotations__ = {
                 "Recipients": Recipients,
                 "Content": Content,
                 "Options": Options,
             }
     
     Recipients: 'TransactionalRecipient'
+    Content: 'EmailContent'
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Recipients"]) -> 'TransactionalRecipient': ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Content"]) -> 'EmailContent': ...
     
@@ -79,15 +81,15 @@
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Recipients"]) -> 'TransactionalRecipient': ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Content"]) -> typing.Union['EmailContent', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["Content"]) -> 'EmailContent': ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Options"]) -> typing.Union['Options', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
@@ -95,15 +97,15 @@
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         Recipients: 'TransactionalRecipient',
-        Content: typing.Union['EmailContent', schemas.Unset] = schemas.unset,
+        Content: 'EmailContent',
         Options: typing.Union['Options', schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'EmailTransactionalMessageData':
         return super().__new__(
             cls,
             *_args,
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/email_transactional_message_data.pyi` & `elasticemail-4.1.0/ElasticEmail/model/email_transactional_message_data.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     Email data
     """
 
 
     class MetaOapg:
         required = {
             "Recipients",
+            "Content",
         }
         
         class properties:
         
             @staticmethod
             def Recipients() -> typing.Type['TransactionalRecipient']:
                 return TransactionalRecipient
@@ -57,14 +58,15 @@
             __annotations__ = {
                 "Recipients": Recipients,
                 "Content": Content,
                 "Options": Options,
             }
     
     Recipients: 'TransactionalRecipient'
+    Content: 'EmailContent'
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Recipients"]) -> 'TransactionalRecipient': ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Content"]) -> 'EmailContent': ...
     
@@ -79,15 +81,15 @@
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Recipients"]) -> 'TransactionalRecipient': ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Content"]) -> typing.Union['EmailContent', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["Content"]) -> 'EmailContent': ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Options"]) -> typing.Union['Options', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
@@ -95,15 +97,15 @@
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         Recipients: 'TransactionalRecipient',
-        Content: typing.Union['EmailContent', schemas.Unset] = schemas.unset,
+        Content: 'EmailContent',
         Options: typing.Union['Options', schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'EmailTransactionalMessageData':
         return super().__new__(
             cls,
             *_args,
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/email_validation_result.py` & `elasticemail-4.1.0/ElasticEmail/model/email_validation_result.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/email_validation_result.pyi` & `elasticemail-4.1.0/ElasticEmail/model/email_validation_result.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/email_validation_status.py` & `elasticemail-4.1.0/ElasticEmail/model/email_validation_status.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/email_validation_status.pyi` & `elasticemail-4.1.0/ElasticEmail/model/email_validation_status.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/email_view.py` & `elasticemail-4.1.0/ElasticEmail/model/email_view.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/email_view.pyi` & `elasticemail-4.1.0/ElasticEmail/model/email_view.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/emails_payload.py` & `elasticemail-4.1.0/ElasticEmail/model/emails_payload.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/emails_payload.pyi` & `elasticemail-4.1.0/ElasticEmail/model/emails_payload.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/encoding_type.py` & `elasticemail-4.1.0/ElasticEmail/model/encoding_type.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/encoding_type.pyi` & `elasticemail-4.1.0/ElasticEmail/model/encoding_type.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/event_type.py` & `elasticemail-4.1.0/ElasticEmail/model/event_type.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/event_type.pyi` & `elasticemail-4.1.0/ElasticEmail/model/event_type.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/events_order_by.py` & `elasticemail-4.1.0/ElasticEmail/model/events_order_by.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/events_order_by.pyi` & `elasticemail-4.1.0/ElasticEmail/model/events_order_by.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/export_file_formats.py` & `elasticemail-4.1.0/ElasticEmail/model/export_file_formats.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/export_file_formats.pyi` & `elasticemail-4.1.0/ElasticEmail/model/export_file_formats.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/export_link.py` & `elasticemail-4.1.0/ElasticEmail/model/export_link.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/export_link.pyi` & `elasticemail-4.1.0/ElasticEmail/model/export_link.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/export_status.py` & `elasticemail-4.1.0/ElasticEmail/model/export_status.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/export_status.pyi` & `elasticemail-4.1.0/ElasticEmail/model/export_status.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/file_info.py` & `elasticemail-4.1.0/ElasticEmail/model/file_info.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/file_info.pyi` & `elasticemail-4.1.0/ElasticEmail/model/file_info.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/file_payload.py` & `elasticemail-4.1.0/ElasticEmail/model/file_payload.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/file_payload.pyi` & `elasticemail-4.1.0/ElasticEmail/model/file_payload.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/file_upload_result.py` & `elasticemail-4.1.0/ElasticEmail/model/file_upload_result.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/file_upload_result.pyi` & `elasticemail-4.1.0/ElasticEmail/model/file_upload_result.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/inbound_payload.py` & `elasticemail-4.1.0/ElasticEmail/model/inbound_payload.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/inbound_payload.pyi` & `elasticemail-4.1.0/ElasticEmail/model/inbound_payload.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/inbound_route.py` & `elasticemail-4.1.0/ElasticEmail/model/inbound_route.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/inbound_route.pyi` & `elasticemail-4.1.0/ElasticEmail/model/inbound_route.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/inbound_route_action_type.py` & `elasticemail-4.1.0/ElasticEmail/model/inbound_route_action_type.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/inbound_route_action_type.pyi` & `elasticemail-4.1.0/ElasticEmail/model/inbound_route_action_type.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/inbound_route_filter_type.py` & `elasticemail-4.1.0/ElasticEmail/model/inbound_route_filter_type.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/inbound_route_filter_type.pyi` & `elasticemail-4.1.0/ElasticEmail/model/inbound_route_filter_type.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/list_payload.py` & `elasticemail-4.1.0/ElasticEmail/model/list_payload.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/list_payload.pyi` & `elasticemail-4.1.0/ElasticEmail/model/list_payload.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/list_update_payload.py` & `elasticemail-4.1.0/ElasticEmail/model/list_update_payload.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/list_update_payload.pyi` & `elasticemail-4.1.0/ElasticEmail/model/list_update_payload.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/log_job_status.py` & `elasticemail-4.1.0/ElasticEmail/model/log_job_status.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/log_job_status.pyi` & `elasticemail-4.1.0/ElasticEmail/model/log_job_status.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/log_status_summary.py` & `elasticemail-4.1.0/ElasticEmail/model/log_status_summary.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/log_status_summary.pyi` & `elasticemail-4.1.0/ElasticEmail/model/log_status_summary.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/merge_email_payload.py` & `elasticemail-4.1.0/ElasticEmail/model/merge_email_payload.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     Do not edit the class manually.
     """
 
 
     class MetaOapg:
         required = {
             "MergeFile",
+            "Content",
         }
         
         class properties:
         
             @staticmethod
             def MergeFile() -> typing.Type['MessageAttachment']:
                 return MessageAttachment
@@ -55,14 +56,15 @@
             __annotations__ = {
                 "MergeFile": MergeFile,
                 "Content": Content,
                 "Options": Options,
             }
     
     MergeFile: 'MessageAttachment'
+    Content: 'EmailContent'
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["MergeFile"]) -> 'MessageAttachment': ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Content"]) -> 'EmailContent': ...
     
@@ -77,15 +79,15 @@
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["MergeFile"]) -> 'MessageAttachment': ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Content"]) -> typing.Union['EmailContent', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["Content"]) -> 'EmailContent': ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Options"]) -> typing.Union['Options', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
@@ -93,15 +95,15 @@
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         MergeFile: 'MessageAttachment',
-        Content: typing.Union['EmailContent', schemas.Unset] = schemas.unset,
+        Content: 'EmailContent',
         Options: typing.Union['Options', schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'MergeEmailPayload':
         return super().__new__(
             cls,
             *_args,
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/merge_email_payload.pyi` & `elasticemail-4.1.0/ElasticEmail/model/merge_email_payload.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     Do not edit the class manually.
     """
 
 
     class MetaOapg:
         required = {
             "MergeFile",
+            "Content",
         }
         
         class properties:
         
             @staticmethod
             def MergeFile() -> typing.Type['MessageAttachment']:
                 return MessageAttachment
@@ -55,14 +56,15 @@
             __annotations__ = {
                 "MergeFile": MergeFile,
                 "Content": Content,
                 "Options": Options,
             }
     
     MergeFile: 'MessageAttachment'
+    Content: 'EmailContent'
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["MergeFile"]) -> 'MessageAttachment': ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Content"]) -> 'EmailContent': ...
     
@@ -77,15 +79,15 @@
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["MergeFile"]) -> 'MessageAttachment': ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Content"]) -> typing.Union['EmailContent', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["Content"]) -> 'EmailContent': ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Options"]) -> typing.Union['Options', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
@@ -93,15 +95,15 @@
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         MergeFile: 'MessageAttachment',
-        Content: typing.Union['EmailContent', schemas.Unset] = schemas.unset,
+        Content: 'EmailContent',
         Options: typing.Union['Options', schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'MergeEmailPayload':
         return super().__new__(
             cls,
             *_args,
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/message_attachment.py` & `elasticemail-4.1.0/ElasticEmail/model/message_attachment.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/message_attachment.pyi` & `elasticemail-4.1.0/ElasticEmail/model/message_attachment.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/message_category.py` & `elasticemail-4.1.0/ElasticEmail/model/message_category.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/message_category.pyi` & `elasticemail-4.1.0/ElasticEmail/model/message_category.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/new_api_key.py` & `elasticemail-4.1.0/ElasticEmail/model/new_api_key.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/new_api_key.pyi` & `elasticemail-4.1.0/ElasticEmail/model/new_api_key.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/new_smtp_credentials.py` & `elasticemail-4.1.0/ElasticEmail/model/new_smtp_credentials.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/new_smtp_credentials.pyi` & `elasticemail-4.1.0/ElasticEmail/model/new_smtp_credentials.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/options.py` & `elasticemail-4.1.0/ElasticEmail/model/options.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,16 +66,62 @@
                     )
             PoolName = schemas.StrSchema
             ChannelName = schemas.StrSchema
         
             @staticmethod
             def Encoding() -> typing.Type['EncodingType']:
                 return EncodingType
-            TrackOpens = schemas.BoolSchema
-            TrackClicks = schemas.BoolSchema
+            
+            
+            class TrackOpens(
+                schemas.BoolBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneBoolMixin
+            ):
+            
+            
+                class MetaOapg:
+                    format = 'boolean'
+            
+            
+                def __new__(
+                    cls,
+                    *_args: typing.Union[None, bool, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> 'TrackOpens':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                    )
+            
+            
+            class TrackClicks(
+                schemas.BoolBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneBoolMixin
+            ):
+            
+            
+                class MetaOapg:
+                    format = 'boolean'
+            
+            
+                def __new__(
+                    cls,
+                    *_args: typing.Union[None, bool, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> 'TrackClicks':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                    )
             __annotations__ = {
                 "TimeOffset": TimeOffset,
                 "PoolName": PoolName,
                 "ChannelName": ChannelName,
                 "Encoding": Encoding,
                 "TrackOpens": TrackOpens,
                 "TrackClicks": TrackClicks,
@@ -135,16 +181,16 @@
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         TimeOffset: typing.Union[MetaOapg.properties.TimeOffset, None, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         PoolName: typing.Union[MetaOapg.properties.PoolName, str, schemas.Unset] = schemas.unset,
         ChannelName: typing.Union[MetaOapg.properties.ChannelName, str, schemas.Unset] = schemas.unset,
         Encoding: typing.Union['EncodingType', schemas.Unset] = schemas.unset,
-        TrackOpens: typing.Union[MetaOapg.properties.TrackOpens, bool, schemas.Unset] = schemas.unset,
-        TrackClicks: typing.Union[MetaOapg.properties.TrackClicks, bool, schemas.Unset] = schemas.unset,
+        TrackOpens: typing.Union[MetaOapg.properties.TrackOpens, None, bool, schemas.Unset] = schemas.unset,
+        TrackClicks: typing.Union[MetaOapg.properties.TrackClicks, None, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'Options':
         return super().__new__(
             cls,
             *_args,
             TimeOffset=TimeOffset,
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/options.pyi` & `elasticemail-4.1.0/ElasticEmail/model/options.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -66,16 +66,62 @@
                     )
             PoolName = schemas.StrSchema
             ChannelName = schemas.StrSchema
         
             @staticmethod
             def Encoding() -> typing.Type['EncodingType']:
                 return EncodingType
-            TrackOpens = schemas.BoolSchema
-            TrackClicks = schemas.BoolSchema
+            
+            
+            class TrackOpens(
+                schemas.BoolBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneBoolMixin
+            ):
+            
+            
+                class MetaOapg:
+                    format = 'boolean'
+            
+            
+                def __new__(
+                    cls,
+                    *_args: typing.Union[None, bool, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> 'TrackOpens':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                    )
+            
+            
+            class TrackClicks(
+                schemas.BoolBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneBoolMixin
+            ):
+            
+            
+                class MetaOapg:
+                    format = 'boolean'
+            
+            
+                def __new__(
+                    cls,
+                    *_args: typing.Union[None, bool, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> 'TrackClicks':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                    )
             __annotations__ = {
                 "TimeOffset": TimeOffset,
                 "PoolName": PoolName,
                 "ChannelName": ChannelName,
                 "Encoding": Encoding,
                 "TrackOpens": TrackOpens,
                 "TrackClicks": TrackClicks,
@@ -135,16 +181,16 @@
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         TimeOffset: typing.Union[MetaOapg.properties.TimeOffset, None, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         PoolName: typing.Union[MetaOapg.properties.PoolName, str, schemas.Unset] = schemas.unset,
         ChannelName: typing.Union[MetaOapg.properties.ChannelName, str, schemas.Unset] = schemas.unset,
         Encoding: typing.Union['EncodingType', schemas.Unset] = schemas.unset,
-        TrackOpens: typing.Union[MetaOapg.properties.TrackOpens, bool, schemas.Unset] = schemas.unset,
-        TrackClicks: typing.Union[MetaOapg.properties.TrackClicks, bool, schemas.Unset] = schemas.unset,
+        TrackOpens: typing.Union[MetaOapg.properties.TrackOpens, None, bool, schemas.Unset] = schemas.unset,
+        TrackClicks: typing.Union[MetaOapg.properties.TrackClicks, None, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'Options':
         return super().__new__(
             cls,
             *_args,
             TimeOffset=TimeOffset,
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/recipient_event.py` & `elasticemail-4.1.0/ElasticEmail/model/recipient_event.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/recipient_event.pyi` & `elasticemail-4.1.0/ElasticEmail/model/recipient_event.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/segment.py` & `elasticemail-4.1.0/ElasticEmail/model/segment.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/segment.pyi` & `elasticemail-4.1.0/ElasticEmail/model/segment.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/segment_payload.py` & `elasticemail-4.1.0/ElasticEmail/model/segment_payload.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/segment_payload.pyi` & `elasticemail-4.1.0/ElasticEmail/model/segment_payload.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/smtp_credentials.py` & `elasticemail-4.1.0/ElasticEmail/model/smtp_credentials.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/smtp_credentials.pyi` & `elasticemail-4.1.0/ElasticEmail/model/smtp_credentials.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/smtp_credentials_payload.py` & `elasticemail-4.1.0/ElasticEmail/model/smtp_credentials_payload.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/smtp_credentials_payload.pyi` & `elasticemail-4.1.0/ElasticEmail/model/smtp_credentials_payload.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/sort_order_item.py` & `elasticemail-4.1.0/ElasticEmail/model/sort_order_item.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/sort_order_item.pyi` & `elasticemail-4.1.0/ElasticEmail/model/sort_order_item.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/split_optimization_type.py` & `elasticemail-4.1.0/ElasticEmail/model/split_optimization_type.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/split_optimization_type.pyi` & `elasticemail-4.1.0/ElasticEmail/model/split_optimization_type.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/split_options.py` & `elasticemail-4.1.0/ElasticEmail/model/split_options.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/split_options.pyi` & `elasticemail-4.1.0/ElasticEmail/model/split_options.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/sub_account_info.py` & `elasticemail-4.1.0/ElasticEmail/model/sub_account_info.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/sub_account_info.pyi` & `elasticemail-4.1.0/ElasticEmail/model/sub_account_info.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/subaccount_email_credits_payload.py` & `elasticemail-4.1.0/ElasticEmail/model/subaccount_email_credits_payload.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/subaccount_email_credits_payload.pyi` & `elasticemail-4.1.0/ElasticEmail/model/subaccount_email_credits_payload.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/subaccount_email_settings.py` & `elasticemail-4.1.0/ElasticEmail/model/subaccount_email_settings.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/subaccount_email_settings.pyi` & `elasticemail-4.1.0/ElasticEmail/model/subaccount_email_settings.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/subaccount_email_settings_payload.py` & `elasticemail-4.1.0/ElasticEmail/model/subaccount_email_settings_payload.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/subaccount_email_settings_payload.pyi` & `elasticemail-4.1.0/ElasticEmail/model/subaccount_email_settings_payload.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/subaccount_payload.py` & `elasticemail-4.1.0/ElasticEmail/model/subaccount_payload.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/subaccount_payload.pyi` & `elasticemail-4.1.0/ElasticEmail/model/subaccount_payload.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/subaccount_settings_info.py` & `elasticemail-4.1.0/ElasticEmail/model/subaccount_settings_info.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/subaccount_settings_info.pyi` & `elasticemail-4.1.0/ElasticEmail/model/subaccount_settings_info.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/subaccount_settings_info_payload.py` & `elasticemail-4.1.0/ElasticEmail/model/subaccount_settings_info_payload.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/subaccount_settings_info_payload.pyi` & `elasticemail-4.1.0/ElasticEmail/model/subaccount_settings_info_payload.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/suppression.py` & `elasticemail-4.1.0/ElasticEmail/model/suppression.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/suppression.pyi` & `elasticemail-4.1.0/ElasticEmail/model/suppression.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/template.py` & `elasticemail-4.1.0/ElasticEmail/model/template.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/template.pyi` & `elasticemail-4.1.0/ElasticEmail/model/template.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/template_payload.py` & `elasticemail-4.1.0/ElasticEmail/model/template_payload.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/template_payload.pyi` & `elasticemail-4.1.0/ElasticEmail/model/template_payload.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/template_scope.py` & `elasticemail-4.1.0/ElasticEmail/model/template_scope.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/template_scope.pyi` & `elasticemail-4.1.0/ElasticEmail/model/template_scope.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/template_type.py` & `elasticemail-4.1.0/ElasticEmail/model/template_type.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/template_type.pyi` & `elasticemail-4.1.0/ElasticEmail/model/template_type.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/transactional_recipient.py` & `elasticemail-4.1.0/ElasticEmail/model/transactional_recipient.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/transactional_recipient.pyi` & `elasticemail-4.1.0/ElasticEmail/model/transactional_recipient.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/utm.py` & `elasticemail-4.1.0/ElasticEmail/model/utm.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/utm.pyi` & `elasticemail-4.1.0/ElasticEmail/model/utm.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/verification_file_result.py` & `elasticemail-4.1.0/ElasticEmail/model/verification_file_result.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/verification_file_result.pyi` & `elasticemail-4.1.0/ElasticEmail/model/verification_file_result.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/verification_file_result_details.py` & `elasticemail-4.1.0/ElasticEmail/model/verification_file_result_details.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/verification_file_result_details.pyi` & `elasticemail-4.1.0/ElasticEmail/model/verification_file_result_details.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/verification_status.py` & `elasticemail-4.1.0/ElasticEmail/model/verification_status.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/model/verification_status.pyi` & `elasticemail-4.1.0/ElasticEmail/model/verification_status.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/models/__init__.py` & `elasticemail-4.1.0/ElasticEmail/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 from ElasticEmail.model.contact_source import ContactSource
 from ElasticEmail.model.contact_status import ContactStatus
 from ElasticEmail.model.contact_update_payload import ContactUpdatePayload
 from ElasticEmail.model.contacts_list import ContactsList
 from ElasticEmail.model.delivery_optimization_type import DeliveryOptimizationType
 from ElasticEmail.model.email_content import EmailContent
 from ElasticEmail.model.email_data import EmailData
+from ElasticEmail.model.email_job_failed_status import EmailJobFailedStatus
+from ElasticEmail.model.email_job_status import EmailJobStatus
 from ElasticEmail.model.email_message_data import EmailMessageData
 from ElasticEmail.model.email_predicted_validation_status import EmailPredictedValidationStatus
 from ElasticEmail.model.email_recipient import EmailRecipient
 from ElasticEmail.model.email_send import EmailSend
 from ElasticEmail.model.email_status import EmailStatus
 from ElasticEmail.model.email_transactional_message_data import EmailTransactionalMessageData
 from ElasticEmail.model.email_validation_result import EmailValidationResult
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/__init__.py` & `elasticemail-4.1.0/ElasticEmail/paths/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     CONTACTS_EMAIL = "/contacts/{email}"
     CONTACTS_DELETE = "/contacts/delete"
     CONTACTS_EXPORT = "/contacts/export"
     CONTACTS_EXPORT_ID_STATUS = "/contacts/export/{id}/status"
     CONTACTS_IMPORT = "/contacts/import"
     EMAILS = "/emails"
     EMAILS_MSGID_VIEW = "/emails/{msgid}/view"
+    EMAILS_TRANSACTIONID_STATUS = "/emails/{transactionid}/status"
     EMAILS_MERGEFILE = "/emails/mergefile"
     EMAILS_TRANSACTIONAL = "/emails/transactional"
     EVENTS = "/events"
     EVENTS_TRANSACTIONID = "/events/{transactionid}"
     EVENTS_CHANNELS_NAME = "/events/channels/{name}"
     EVENTS_CHANNELS_NAME_EXPORT = "/events/channels/{name}/export"
     EVENTS_CHANNELS_EXPORT_ID_STATUS = "/events/channels/export/{id}/status"
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/campaigns/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/campaigns/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/campaigns/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/campaigns/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/campaigns/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/campaigns/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/campaigns/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/campaigns/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/campaigns_name/delete.py` & `elasticemail-4.1.0/ElasticEmail/paths/campaigns_name/delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/campaigns_name/delete.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/campaigns_name/delete.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/campaigns_name/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/campaigns_name/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/campaigns_name/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/campaigns_name/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/campaigns_name/put.py` & `elasticemail-4.1.0/ElasticEmail/paths/campaigns_name/put.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/campaigns_name/put.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/campaigns_name/put.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/contacts/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/contacts/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/contacts/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/contacts/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/contacts/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/contacts/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/contacts/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/contacts/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/contacts_delete/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/contacts_delete/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/contacts_delete/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/contacts_delete/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/contacts_email/delete.py` & `elasticemail-4.1.0/ElasticEmail/paths/contacts_email/delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/contacts_email/delete.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/contacts_email/delete.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/contacts_email/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/contacts_email/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/contacts_email/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/contacts_email/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/contacts_email/put.py` & `elasticemail-4.1.0/ElasticEmail/paths/contacts_email/put.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/contacts_email/put.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/contacts_email/put.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/contacts_export/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/contacts_export/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/contacts_export/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/contacts_export/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/contacts_export_id_status/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/contacts_export_id_status/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/contacts_export_id_status/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/contacts_export_id_status/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/contacts_import/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/contacts_import/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/contacts_import/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/contacts_import/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/emails/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/emails/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/emails/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/emails/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/emails_mergefile/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/emails_mergefile/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/emails_mergefile/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/emails_mergefile/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/emails_msgid_view/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/emails_msgid_view/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/emails_msgid_view/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/emails_msgid_view/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/emails_transactional/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/emails_transactional/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/emails_transactional/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/emails_transactional/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/events/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/events/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/events/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/events/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/events_channels_export_id_status/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/events_channels_export_id_status/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/events_channels_export_id_status/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/events_channels_export_id_status/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/events_channels_name/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/events_channels_name/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/events_channels_name/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/events_channels_name/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/events_channels_name_export/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/events_channels_name_export/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/events_channels_name_export/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/events_channels_name_export/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/events_export/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/events_export/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/events_export/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/events_export/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/events_export_id_status/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/events_export_id_status/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/events_export_id_status/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/events_export_id_status/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/events_transactionid/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/events_transactionid/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/events_transactionid/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/events_transactionid/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/files/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/files/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/files/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/files/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/files/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/files/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/files/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/files/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/files_name/delete.py` & `elasticemail-4.1.0/ElasticEmail/paths/files_name/delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/files_name/delete.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/files_name/delete.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/files_name/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/files_name/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/files_name/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/files_name/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/files_name_info/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/files_name_info/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/files_name_info/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/files_name_info/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/inboundroute/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/inboundroute/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/inboundroute/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/inboundroute/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute_id/delete.py` & `elasticemail-4.1.0/ElasticEmail/paths/inboundroute_id/delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute_id/delete.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/inboundroute_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute_id/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/inboundroute_id/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute_id/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/inboundroute_id/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute_id/put.py` & `elasticemail-4.1.0/ElasticEmail/paths/inboundroute_id/put.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute_id/put.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/inboundroute_id/put.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute_order/put.py` & `elasticemail-4.1.0/ElasticEmail/paths/inboundroute_order/put.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/inboundroute_order/put.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/inboundroute_order/put.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/lists/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/lists/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/lists/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/lists/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/lists/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/lists/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/lists/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/lists/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/lists_name/delete.py` & `elasticemail-4.1.0/ElasticEmail/paths/lists_name/delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/lists_name/delete.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/lists_name/delete.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/lists_name/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/lists_name/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/lists_name/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/lists_name/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/lists_name/put.py` & `elasticemail-4.1.0/ElasticEmail/paths/lists_name/put.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/lists_name/put.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/lists_name/put.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/lists_name_contacts/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/lists_name_contacts/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/lists_name_contacts/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/lists_name_contacts/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/lists_name_contacts_remove/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/lists_name_contacts_remove/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/lists_name_contacts_remove/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/lists_name_contacts_remove/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/security_apikeys/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/security_apikeys/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/security_apikeys/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/security_apikeys/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys_name/delete.py` & `elasticemail-4.1.0/ElasticEmail/paths/security_apikeys_name/delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys_name/delete.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/security_apikeys_name/delete.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys_name/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/security_apikeys_name/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys_name/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/security_apikeys_name/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys_name/put.py` & `elasticemail-4.1.0/ElasticEmail/paths/security_apikeys_name/put.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/security_apikeys_name/put.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/security_apikeys_name/put.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/security_smtp/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/security_smtp/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/security_smtp/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/security_smtp/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp_name/delete.py` & `elasticemail-4.1.0/ElasticEmail/paths/security_smtp_name/delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp_name/delete.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/security_smtp_name/delete.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp_name/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/security_smtp_name/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp_name/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/security_smtp_name/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp_name/put.py` & `elasticemail-4.1.0/ElasticEmail/paths/security_smtp_name/put.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/security_smtp_name/put.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/security_smtp_name/put.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/segments/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/segments/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/segments/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/segments/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/segments/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/segments/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/segments/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/segments/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/segments_name/delete.py` & `elasticemail-4.1.0/ElasticEmail/paths/segments_name/delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/segments_name/delete.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/segments_name/delete.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/segments_name/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/segments_name/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/segments_name/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/segments_name/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/segments_name/put.py` & `elasticemail-4.1.0/ElasticEmail/paths/segments_name/put.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/segments_name/put.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/segments_name/put.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/statistics/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/statistics/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/statistics/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/statistics/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/statistics_campaigns/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/statistics_campaigns/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/statistics_campaigns/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/statistics_campaigns/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/statistics_campaigns_name/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/statistics_campaigns_name/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/statistics_campaigns_name/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/statistics_campaigns_name/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/statistics_channels/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/statistics_channels/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/statistics_channels/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/statistics_channels/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/statistics_channels_name/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/statistics_channels_name/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/statistics_channels_name/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/statistics_channels_name/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/subaccounts/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/subaccounts/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/subaccounts/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/subaccounts/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts_email/delete.py` & `elasticemail-4.1.0/ElasticEmail/paths/subaccounts_email/delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts_email/delete.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/subaccounts_email/delete.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts_email/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/subaccounts_email/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts_email/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/subaccounts_email/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts_email_credits/patch.py` & `elasticemail-4.1.0/ElasticEmail/paths/subaccounts_email_credits/patch.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts_email_credits/patch.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/subaccounts_email_credits/patch.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts_email_settings_email/put.py` & `elasticemail-4.1.0/ElasticEmail/paths/subaccounts_email_settings_email/put.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/subaccounts_email_settings_email/put.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/subaccounts_email_settings_email/put.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_bounces/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions_bounces/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_bounces/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions_bounces/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_bounces/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions_bounces/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_bounces/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions_bounces/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_bounces_import/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions_bounces_import/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_bounces_import/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions_bounces_import/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_complaints/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions_complaints/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_complaints/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions_complaints/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_complaints/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions_complaints/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_complaints/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions_complaints/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_complaints_import/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions_complaints_import/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_complaints_import/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions_complaints_import/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_email/delete.py` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions_email/delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_email/delete.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions_email/delete.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_email/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions_email/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_email/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions_email/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_unsubscribes/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions_unsubscribes/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_unsubscribes/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions_unsubscribes/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_unsubscribes/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions_unsubscribes/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_unsubscribes/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions_unsubscribes/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_unsubscribes_import/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions_unsubscribes_import/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/suppressions_unsubscribes_import/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/suppressions_unsubscribes_import/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/templates/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/templates/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/templates/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/templates/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/templates/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/templates/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/templates/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/templates/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/templates_name/delete.py` & `elasticemail-4.1.0/ElasticEmail/paths/templates_name/delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/templates_name/delete.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/templates_name/delete.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/templates_name/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/templates_name/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/templates_name/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/templates_name/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/templates_name/put.py` & `elasticemail-4.1.0/ElasticEmail/paths/templates_name/put.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/templates_name/put.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/templates_name/put.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/verifications/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/verifications/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/verifications/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/verifications/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/verifications_email/delete.py` & `elasticemail-4.1.0/ElasticEmail/paths/verifications_email/delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/verifications_email/delete.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/verifications_email/delete.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/verifications_email/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/verifications_email/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/verifications_email/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/verifications_email/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/verifications_email/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/verifications_email/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/verifications_email/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/verifications_email/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/verifications_files/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/verifications_files/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id/delete.py` & `elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id/delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id/delete.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id_result/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id_result/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id_result/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id_result/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id_result_download/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id_result_download/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id_result_download/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id_result_download/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id_verification/post.py` & `elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id_verification/post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_id_verification/post.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/verifications_files_id_verification/post.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_result/get.py` & `elasticemail-4.1.0/ElasticEmail/paths/verifications_files_result/get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/paths/verifications_files_result/get.pyi` & `elasticemail-4.1.0/ElasticEmail/paths/verifications_files_result/get.pyi`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/rest.py` & `elasticemail-4.1.0/ElasticEmail/rest.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail/schemas.py` & `elasticemail-4.1.0/ElasticEmail/schemas.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/ElasticEmail.egg-info/PKG-INFO` & `elasticemail-4.1.0/ElasticEmail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ElasticEmail
-Version: 4.0.24
+Version: 4.1.0
 Summary: Elastic Email REST API
 Home-page: 
 Author: Elastic Email
 Author-email: support@elasticemail.com
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,Elastic Email REST API
 Requires-Python: >=3.6
@@ -22,15 +22,15 @@
 To start using this API, you will need your Access Token (available [here](https://app.elasticemail.com/marketing/settings/new/manage-api)). Remember to keep it safe. Required access levels are listed in the given request’s description.
 
 Downloadable library clients can be found in our Github repository [here](https://github.com/ElasticEmail/elasticemail-python)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 4.0.0
-- Package version: 4.0.24
+- Package version: 4.1.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python &gt;&#x3D;3.7
 
 ## Migration from other generators like python and python-legacy
@@ -126,17 +126,17 @@
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
-pip install git+https://github.com/elasticemail/elasticemail-python.git
+pip install git+https://github.com/radzawee/elasticemail-python.git
 ```
-(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/elasticemail/elasticemail-python.git`)
+(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/radzawee/elasticemail-python.git`)
 
 Then import the package:
 ```python
 import ElasticEmail
 ```
 
 ### Setuptools
@@ -236,14 +236,15 @@
 *ContactsApi* | [**contacts_delete_post**](docs/apis/tags/ContactsApi.md#contacts_delete_post) | **post** /contacts/delete | Delete Contacts Bulk
 *ContactsApi* | [**contacts_export_by_id_status_get**](docs/apis/tags/ContactsApi.md#contacts_export_by_id_status_get) | **get** /contacts/export/{id}/status | Check Export Status
 *ContactsApi* | [**contacts_export_post**](docs/apis/tags/ContactsApi.md#contacts_export_post) | **post** /contacts/export | Export Contacts
 *ContactsApi* | [**contacts_get**](docs/apis/tags/ContactsApi.md#contacts_get) | **get** /contacts | Load Contacts
 *ContactsApi* | [**contacts_import_post**](docs/apis/tags/ContactsApi.md#contacts_import_post) | **post** /contacts/import | Upload Contacts
 *ContactsApi* | [**contacts_post**](docs/apis/tags/ContactsApi.md#contacts_post) | **post** /contacts | Add Contact
 *EmailsApi* | [**emails_by_msgid_view_get**](docs/apis/tags/EmailsApi.md#emails_by_msgid_view_get) | **get** /emails/{msgid}/view | View Email
+*EmailsApi* | [**emails_by_transactionid_status_get**](docs/apis/tags/EmailsApi.md#emails_by_transactionid_status_get) | **get** /emails/{transactionid}/status | Get Status
 *EmailsApi* | [**emails_mergefile_post**](docs/apis/tags/EmailsApi.md#emails_mergefile_post) | **post** /emails/mergefile | Send Bulk Emails CSV
 *EmailsApi* | [**emails_post**](docs/apis/tags/EmailsApi.md#emails_post) | **post** /emails | Send Bulk Emails
 *EmailsApi* | [**emails_transactional_post**](docs/apis/tags/EmailsApi.md#emails_transactional_post) | **post** /emails/transactional | Send Transactional Email
 *EventsApi* | [**events_by_transactionid_get**](docs/apis/tags/EventsApi.md#events_by_transactionid_get) | **get** /events/{transactionid} | Load Email Events
 *EventsApi* | [**events_channels_by_name_export_post**](docs/apis/tags/EventsApi.md#events_channels_by_name_export_post) | **post** /events/channels/{name}/export | Export Channel Events
 *EventsApi* | [**events_channels_by_name_get**](docs/apis/tags/EventsApi.md#events_channels_by_name_get) | **get** /events/channels/{name} | Load Channel Events
 *EventsApi* | [**events_channels_export_by_id_status_get**](docs/apis/tags/EventsApi.md#events_channels_export_by_id_status_get) | **get** /events/channels/export/{id}/status | Check Channel Export Status
@@ -345,14 +346,16 @@
  - [ContactSource](docs/models/ContactSource.md)
  - [ContactStatus](docs/models/ContactStatus.md)
  - [ContactUpdatePayload](docs/models/ContactUpdatePayload.md)
  - [ContactsList](docs/models/ContactsList.md)
  - [DeliveryOptimizationType](docs/models/DeliveryOptimizationType.md)
  - [EmailContent](docs/models/EmailContent.md)
  - [EmailData](docs/models/EmailData.md)
+ - [EmailJobFailedStatus](docs/models/EmailJobFailedStatus.md)
+ - [EmailJobStatus](docs/models/EmailJobStatus.md)
  - [EmailMessageData](docs/models/EmailMessageData.md)
  - [EmailPredictedValidationStatus](docs/models/EmailPredictedValidationStatus.md)
  - [EmailRecipient](docs/models/EmailRecipient.md)
  - [EmailSend](docs/models/EmailSend.md)
  - [EmailStatus](docs/models/EmailStatus.md)
  - [EmailTransactionalMessageData](docs/models/EmailTransactionalMessageData.md)
  - [EmailValidationResult](docs/models/EmailValidationResult.md)
```

### Comparing `ElasticEmail-4.0.24/ElasticEmail.egg-info/SOURCES.txt` & `elasticemail-4.1.0/ElasticEmail.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,21 @@
 README.md
 setup.cfg
 setup.py
 ElasticEmail/__init__.py
 ElasticEmail/api_client.py
 ElasticEmail/configuration.py
 ElasticEmail/exceptions.py
-ElasticEmail/model_utils.py
 ElasticEmail/rest.py
 ElasticEmail/schemas.py
 ElasticEmail.egg-info/PKG-INFO
 ElasticEmail.egg-info/SOURCES.txt
 ElasticEmail.egg-info/dependency_links.txt
 ElasticEmail.egg-info/requires.txt
 ElasticEmail.egg-info/top_level.txt
-ElasticEmail/api/__init__.py
-ElasticEmail/api/campaigns_api.py
-ElasticEmail/api/contacts_api.py
-ElasticEmail/api/emails_api.py
-ElasticEmail/api/events_api.py
-ElasticEmail/api/files_api.py
-ElasticEmail/api/inbound_route_api.py
-ElasticEmail/api/lists_api.py
-ElasticEmail/api/security_api.py
-ElasticEmail/api/segments_api.py
-ElasticEmail/api/statistics_api.py
-ElasticEmail/api/sub_accounts_api.py
-ElasticEmail/api/suppressions_api.py
-ElasticEmail/api/templates_api.py
-ElasticEmail/api/verifications_api.py
 ElasticEmail/apis/__init__.py
 ElasticEmail/apis/path_to_api.py
 ElasticEmail/apis/tag_to_api.py
 ElasticEmail/apis/paths/__init__.py
 ElasticEmail/apis/paths/campaigns.py
 ElasticEmail/apis/paths/campaigns_name.py
 ElasticEmail/apis/paths/contacts.py
@@ -40,14 +24,15 @@
 ElasticEmail/apis/paths/contacts_export.py
 ElasticEmail/apis/paths/contacts_export_id_status.py
 ElasticEmail/apis/paths/contacts_import.py
 ElasticEmail/apis/paths/emails.py
 ElasticEmail/apis/paths/emails_mergefile.py
 ElasticEmail/apis/paths/emails_msgid_view.py
 ElasticEmail/apis/paths/emails_transactional.py
+ElasticEmail/apis/paths/emails_transactionid_status.py
 ElasticEmail/apis/paths/events.py
 ElasticEmail/apis/paths/events_channels_export_id_status.py
 ElasticEmail/apis/paths/events_channels_name.py
 ElasticEmail/apis/paths/events_channels_name_export.py
 ElasticEmail/apis/paths/events_export.py
 ElasticEmail/apis/paths/events_export_id_status.py
 ElasticEmail/apis/paths/events_transactionid.py
@@ -156,14 +141,18 @@
 ElasticEmail/model/contacts_list.pyi
 ElasticEmail/model/delivery_optimization_type.py
 ElasticEmail/model/delivery_optimization_type.pyi
 ElasticEmail/model/email_content.py
 ElasticEmail/model/email_content.pyi
 ElasticEmail/model/email_data.py
 ElasticEmail/model/email_data.pyi
+ElasticEmail/model/email_job_failed_status.py
+ElasticEmail/model/email_job_failed_status.pyi
+ElasticEmail/model/email_job_status.py
+ElasticEmail/model/email_job_status.pyi
 ElasticEmail/model/email_message_data.py
 ElasticEmail/model/email_message_data.pyi
 ElasticEmail/model/email_predicted_validation_status.py
 ElasticEmail/model/email_predicted_validation_status.pyi
 ElasticEmail/model/email_recipient.py
 ElasticEmail/model/email_recipient.pyi
 ElasticEmail/model/email_send.py
@@ -322,14 +311,17 @@
 ElasticEmail/paths/emails_mergefile/post.pyi
 ElasticEmail/paths/emails_msgid_view/__init__.py
 ElasticEmail/paths/emails_msgid_view/get.py
 ElasticEmail/paths/emails_msgid_view/get.pyi
 ElasticEmail/paths/emails_transactional/__init__.py
 ElasticEmail/paths/emails_transactional/post.py
 ElasticEmail/paths/emails_transactional/post.pyi
+ElasticEmail/paths/emails_transactionid_status/__init__.py
+ElasticEmail/paths/emails_transactionid_status/get.py
+ElasticEmail/paths/emails_transactionid_status/get.pyi
 ElasticEmail/paths/events/__init__.py
 ElasticEmail/paths/events/get.py
 ElasticEmail/paths/events/get.pyi
 ElasticEmail/paths/events_channels_export_id_status/__init__.py
 ElasticEmail/paths/events_channels_export_id_status/get.py
 ElasticEmail/paths/events_channels_export_id_status/get.pyi
 ElasticEmail/paths/events_channels_name/__init__.py
@@ -528,113 +520,14 @@
 ElasticEmail/paths/verifications_files_id_result_download/get.pyi
 ElasticEmail/paths/verifications_files_id_verification/__init__.py
 ElasticEmail/paths/verifications_files_id_verification/post.py
 ElasticEmail/paths/verifications_files_id_verification/post.pyi
 ElasticEmail/paths/verifications_files_result/__init__.py
 ElasticEmail/paths/verifications_files_result/get.py
 ElasticEmail/paths/verifications_files_result/get.pyi
-test/test_access_level.py
-test/test_account_status_enum.py
-test/test_api_key.py
-test/test_api_key_payload.py
-test/test_body_content_type.py
-test/test_body_part.py
-test/test_campaign.py
-test/test_campaign_options.py
-test/test_campaign_recipient.py
-test/test_campaign_status.py
-test/test_campaign_template.py
-test/test_campaigns_api.py
-test/test_channel_log_status_summary.py
-test/test_compression_format.py
-test/test_consent_data.py
-test/test_consent_tracking.py
-test/test_contact.py
-test/test_contact_activity.py
-test/test_contact_hist_event_type.py
-test/test_contact_history.py
-test/test_contact_payload.py
-test/test_contact_source.py
-test/test_contact_status.py
-test/test_contact_update_payload.py
-test/test_contacts_api.py
-test/test_contacts_list.py
-test/test_delivery_optimization_type.py
-test/test_email_content.py
-test/test_email_data.py
-test/test_email_message_data.py
-test/test_email_recipient.py
-test/test_email_send.py
-test/test_email_status.py
-test/test_email_transactional_message_data.py
-test/test_email_validation_result.py
-test/test_email_validation_status.py
-test/test_email_view.py
-test/test_emails_api.py
-test/test_emails_payload.py
-test/test_encoding_type.py
-test/test_event_type.py
-test/test_events_api.py
-test/test_events_order_by.py
-test/test_export_file_formats.py
-test/test_export_link.py
-test/test_export_status.py
-test/test_file_info.py
-test/test_file_payload.py
-test/test_file_upload_result.py
-test/test_files_api.py
-test/test_inbound_payload.py
-test/test_inbound_route.py
-test/test_inbound_route_action_type.py
-test/test_inbound_route_api.py
-test/test_inbound_route_filter_type.py
-test/test_list_payload.py
-test/test_list_update_payload.py
-test/test_lists_api.py
-test/test_log_job_status.py
-test/test_log_status_summary.py
-test/test_merge_email_payload.py
-test/test_message_attachment.py
-test/test_message_category.py
-test/test_new_api_key.py
-test/test_new_smtp_credentials.py
-test/test_options.py
-test/test_recipient_event.py
-test/test_security_api.py
-test/test_segment.py
-test/test_segment_payload.py
-test/test_segments_api.py
-test/test_smtp_credentials.py
-test/test_smtp_credentials_payload.py
-test/test_sort_order_item.py
-test/test_split_optimization_type.py
-test/test_split_options.py
-test/test_statistics_api.py
-test/test_sub_account_info.py
-test/test_sub_accounts_api.py
-test/test_subaccount_email_credits_payload.py
-test/test_subaccount_email_settings.py
-test/test_subaccount_email_settings_payload.py
-test/test_subaccount_payload.py
-test/test_subaccount_settings_info.py
-test/test_subaccount_settings_info_payload.py
-test/test_suppression.py
-test/test_suppressions_api.py
-test/test_template.py
-test/test_template_payload.py
-test/test_template_scope.py
-test/test_template_scope_type.py
-test/test_template_type.py
-test/test_templates_api.py
-test/test_transactional_recipient.py
-test/test_utm.py
-test/test_verification_file_result.py
-test/test_verification_file_result_details.py
-test/test_verification_status.py
-test/test_verifications_api.py
 test/test_models/__init__.py
 test/test_models/test_access_level.py
 test/test_models/test_account_status_enum.py
 test/test_models/test_api_key.py
 test/test_models/test_api_key_payload.py
 test/test_models/test_body_content_type.py
 test/test_models/test_body_part.py
@@ -653,14 +546,16 @@
 test/test_models/test_contact_source.py
 test/test_models/test_contact_status.py
 test/test_models/test_contact_update_payload.py
 test/test_models/test_contacts_list.py
 test/test_models/test_delivery_optimization_type.py
 test/test_models/test_email_content.py
 test/test_models/test_email_data.py
+test/test_models/test_email_job_failed_status.py
+test/test_models/test_email_job_status.py
 test/test_models/test_email_message_data.py
 test/test_models/test_email_predicted_validation_status.py
 test/test_models/test_email_recipient.py
 test/test_models/test_email_send.py
 test/test_models/test_email_status.py
 test/test_models/test_email_transactional_message_data.py
 test/test_models/test_email_validation_result.py
@@ -742,14 +637,16 @@
 test/test_paths/test_emails/test_post.py
 test/test_paths/test_emails_mergefile/__init__.py
 test/test_paths/test_emails_mergefile/test_post.py
 test/test_paths/test_emails_msgid_view/__init__.py
 test/test_paths/test_emails_msgid_view/test_get.py
 test/test_paths/test_emails_transactional/__init__.py
 test/test_paths/test_emails_transactional/test_post.py
+test/test_paths/test_emails_transactionid_status/__init__.py
+test/test_paths/test_emails_transactionid_status/test_get.py
 test/test_paths/test_events/__init__.py
 test/test_paths/test_events/test_get.py
 test/test_paths/test_events_channels_export_id_status/__init__.py
 test/test_paths/test_events_channels_export_id_status/test_get.py
 test/test_paths/test_events_channels_name/__init__.py
 test/test_paths/test_events_channels_name/test_get.py
 test/test_paths/test_events_channels_name_export/__init__.py
```

### Comparing `ElasticEmail-4.0.24/PKG-INFO` & `elasticemail-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ElasticEmail
-Version: 4.0.24
+Version: 4.1.0
 Summary: Elastic Email REST API
 Home-page: 
 Author: Elastic Email
 Author-email: support@elasticemail.com
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,Elastic Email REST API
 Requires-Python: >=3.6
@@ -22,15 +22,15 @@
 To start using this API, you will need your Access Token (available [here](https://app.elasticemail.com/marketing/settings/new/manage-api)). Remember to keep it safe. Required access levels are listed in the given request’s description.
 
 Downloadable library clients can be found in our Github repository [here](https://github.com/ElasticEmail/elasticemail-python)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 4.0.0
-- Package version: 4.0.24
+- Package version: 4.1.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python &gt;&#x3D;3.7
 
 ## Migration from other generators like python and python-legacy
@@ -126,17 +126,17 @@
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
-pip install git+https://github.com/elasticemail/elasticemail-python.git
+pip install git+https://github.com/radzawee/elasticemail-python.git
 ```
-(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/elasticemail/elasticemail-python.git`)
+(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/radzawee/elasticemail-python.git`)
 
 Then import the package:
 ```python
 import ElasticEmail
 ```
 
 ### Setuptools
@@ -236,14 +236,15 @@
 *ContactsApi* | [**contacts_delete_post**](docs/apis/tags/ContactsApi.md#contacts_delete_post) | **post** /contacts/delete | Delete Contacts Bulk
 *ContactsApi* | [**contacts_export_by_id_status_get**](docs/apis/tags/ContactsApi.md#contacts_export_by_id_status_get) | **get** /contacts/export/{id}/status | Check Export Status
 *ContactsApi* | [**contacts_export_post**](docs/apis/tags/ContactsApi.md#contacts_export_post) | **post** /contacts/export | Export Contacts
 *ContactsApi* | [**contacts_get**](docs/apis/tags/ContactsApi.md#contacts_get) | **get** /contacts | Load Contacts
 *ContactsApi* | [**contacts_import_post**](docs/apis/tags/ContactsApi.md#contacts_import_post) | **post** /contacts/import | Upload Contacts
 *ContactsApi* | [**contacts_post**](docs/apis/tags/ContactsApi.md#contacts_post) | **post** /contacts | Add Contact
 *EmailsApi* | [**emails_by_msgid_view_get**](docs/apis/tags/EmailsApi.md#emails_by_msgid_view_get) | **get** /emails/{msgid}/view | View Email
+*EmailsApi* | [**emails_by_transactionid_status_get**](docs/apis/tags/EmailsApi.md#emails_by_transactionid_status_get) | **get** /emails/{transactionid}/status | Get Status
 *EmailsApi* | [**emails_mergefile_post**](docs/apis/tags/EmailsApi.md#emails_mergefile_post) | **post** /emails/mergefile | Send Bulk Emails CSV
 *EmailsApi* | [**emails_post**](docs/apis/tags/EmailsApi.md#emails_post) | **post** /emails | Send Bulk Emails
 *EmailsApi* | [**emails_transactional_post**](docs/apis/tags/EmailsApi.md#emails_transactional_post) | **post** /emails/transactional | Send Transactional Email
 *EventsApi* | [**events_by_transactionid_get**](docs/apis/tags/EventsApi.md#events_by_transactionid_get) | **get** /events/{transactionid} | Load Email Events
 *EventsApi* | [**events_channels_by_name_export_post**](docs/apis/tags/EventsApi.md#events_channels_by_name_export_post) | **post** /events/channels/{name}/export | Export Channel Events
 *EventsApi* | [**events_channels_by_name_get**](docs/apis/tags/EventsApi.md#events_channels_by_name_get) | **get** /events/channels/{name} | Load Channel Events
 *EventsApi* | [**events_channels_export_by_id_status_get**](docs/apis/tags/EventsApi.md#events_channels_export_by_id_status_get) | **get** /events/channels/export/{id}/status | Check Channel Export Status
@@ -345,14 +346,16 @@
  - [ContactSource](docs/models/ContactSource.md)
  - [ContactStatus](docs/models/ContactStatus.md)
  - [ContactUpdatePayload](docs/models/ContactUpdatePayload.md)
  - [ContactsList](docs/models/ContactsList.md)
  - [DeliveryOptimizationType](docs/models/DeliveryOptimizationType.md)
  - [EmailContent](docs/models/EmailContent.md)
  - [EmailData](docs/models/EmailData.md)
+ - [EmailJobFailedStatus](docs/models/EmailJobFailedStatus.md)
+ - [EmailJobStatus](docs/models/EmailJobStatus.md)
  - [EmailMessageData](docs/models/EmailMessageData.md)
  - [EmailPredictedValidationStatus](docs/models/EmailPredictedValidationStatus.md)
  - [EmailRecipient](docs/models/EmailRecipient.md)
  - [EmailSend](docs/models/EmailSend.md)
  - [EmailStatus](docs/models/EmailStatus.md)
  - [EmailTransactionalMessageData](docs/models/EmailTransactionalMessageData.md)
  - [EmailValidationResult](docs/models/EmailValidationResult.md)
```

### Comparing `ElasticEmail-4.0.24/README.md` & `elasticemail-4.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 To start using this API, you will need your Access Token (available [here](https://app.elasticemail.com/marketing/settings/new/manage-api)). Remember to keep it safe. Required access levels are listed in the given request’s description.
 
 Downloadable library clients can be found in our Github repository [here](https://github.com/ElasticEmail/elasticemail-python)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 4.0.0
-- Package version: 4.0.24
+- Package version: 4.1.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python &gt;&#x3D;3.7
 
 ## Migration from other generators like python and python-legacy
@@ -112,17 +112,17 @@
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
-pip install git+https://github.com/elasticemail/elasticemail-python.git
+pip install git+https://github.com/radzawee/elasticemail-python.git
 ```
-(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/elasticemail/elasticemail-python.git`)
+(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/radzawee/elasticemail-python.git`)
 
 Then import the package:
 ```python
 import ElasticEmail
 ```
 
 ### Setuptools
@@ -222,14 +222,15 @@
 *ContactsApi* | [**contacts_delete_post**](docs/apis/tags/ContactsApi.md#contacts_delete_post) | **post** /contacts/delete | Delete Contacts Bulk
 *ContactsApi* | [**contacts_export_by_id_status_get**](docs/apis/tags/ContactsApi.md#contacts_export_by_id_status_get) | **get** /contacts/export/{id}/status | Check Export Status
 *ContactsApi* | [**contacts_export_post**](docs/apis/tags/ContactsApi.md#contacts_export_post) | **post** /contacts/export | Export Contacts
 *ContactsApi* | [**contacts_get**](docs/apis/tags/ContactsApi.md#contacts_get) | **get** /contacts | Load Contacts
 *ContactsApi* | [**contacts_import_post**](docs/apis/tags/ContactsApi.md#contacts_import_post) | **post** /contacts/import | Upload Contacts
 *ContactsApi* | [**contacts_post**](docs/apis/tags/ContactsApi.md#contacts_post) | **post** /contacts | Add Contact
 *EmailsApi* | [**emails_by_msgid_view_get**](docs/apis/tags/EmailsApi.md#emails_by_msgid_view_get) | **get** /emails/{msgid}/view | View Email
+*EmailsApi* | [**emails_by_transactionid_status_get**](docs/apis/tags/EmailsApi.md#emails_by_transactionid_status_get) | **get** /emails/{transactionid}/status | Get Status
 *EmailsApi* | [**emails_mergefile_post**](docs/apis/tags/EmailsApi.md#emails_mergefile_post) | **post** /emails/mergefile | Send Bulk Emails CSV
 *EmailsApi* | [**emails_post**](docs/apis/tags/EmailsApi.md#emails_post) | **post** /emails | Send Bulk Emails
 *EmailsApi* | [**emails_transactional_post**](docs/apis/tags/EmailsApi.md#emails_transactional_post) | **post** /emails/transactional | Send Transactional Email
 *EventsApi* | [**events_by_transactionid_get**](docs/apis/tags/EventsApi.md#events_by_transactionid_get) | **get** /events/{transactionid} | Load Email Events
 *EventsApi* | [**events_channels_by_name_export_post**](docs/apis/tags/EventsApi.md#events_channels_by_name_export_post) | **post** /events/channels/{name}/export | Export Channel Events
 *EventsApi* | [**events_channels_by_name_get**](docs/apis/tags/EventsApi.md#events_channels_by_name_get) | **get** /events/channels/{name} | Load Channel Events
 *EventsApi* | [**events_channels_export_by_id_status_get**](docs/apis/tags/EventsApi.md#events_channels_export_by_id_status_get) | **get** /events/channels/export/{id}/status | Check Channel Export Status
@@ -331,14 +332,16 @@
  - [ContactSource](docs/models/ContactSource.md)
  - [ContactStatus](docs/models/ContactStatus.md)
  - [ContactUpdatePayload](docs/models/ContactUpdatePayload.md)
  - [ContactsList](docs/models/ContactsList.md)
  - [DeliveryOptimizationType](docs/models/DeliveryOptimizationType.md)
  - [EmailContent](docs/models/EmailContent.md)
  - [EmailData](docs/models/EmailData.md)
+ - [EmailJobFailedStatus](docs/models/EmailJobFailedStatus.md)
+ - [EmailJobStatus](docs/models/EmailJobStatus.md)
  - [EmailMessageData](docs/models/EmailMessageData.md)
  - [EmailPredictedValidationStatus](docs/models/EmailPredictedValidationStatus.md)
  - [EmailRecipient](docs/models/EmailRecipient.md)
  - [EmailSend](docs/models/EmailSend.md)
  - [EmailStatus](docs/models/EmailStatus.md)
  - [EmailTransactionalMessageData](docs/models/EmailTransactionalMessageData.md)
  - [EmailValidationResult](docs/models/EmailValidationResult.md)
```

### Comparing `ElasticEmail-4.0.24/setup.py` & `elasticemail-4.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 from os import path
 
 NAME = "ElasticEmail"
-VERSION = "4.0.24"
+VERSION = "4.1.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `ElasticEmail-4.0.24/test/test_access_level.py` & `elasticemail-4.1.0/test/test_models/test_contact_update_payload.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.access_level import AccessLevel
-
-
-class TestAccessLevel(unittest.TestCase):
-    """AccessLevel unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.contact_update_payload import ContactUpdatePayload
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testAccessLevel(self):
-        """Test AccessLevel"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = AccessLevel()  # noqa: E501
-        pass
+class TestContactUpdatePayload(unittest.TestCase):
+    """ContactUpdatePayload unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_account_status_enum.py` & `elasticemail-4.1.0/test/test_models/test_export_status.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.account_status_enum import AccountStatusEnum
-
-
-class TestAccountStatusEnum(unittest.TestCase):
-    """AccountStatusEnum unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.export_status import ExportStatus
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testAccountStatusEnum(self):
-        """Test AccountStatusEnum"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = AccountStatusEnum()  # noqa: E501
-        pass
+class TestExportStatus(unittest.TestCase):
+    """ExportStatus unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_api_key.py` & `elasticemail-4.1.0/test/test_models/test_inbound_payload.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.access_level import AccessLevel
-globals()['AccessLevel'] = AccessLevel
-from ElasticEmail.model.api_key import ApiKey
-
-
-class TestApiKey(unittest.TestCase):
-    """ApiKey unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.inbound_payload import InboundPayload
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testApiKey(self):
-        """Test ApiKey"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ApiKey()  # noqa: E501
-        pass
+class TestInboundPayload(unittest.TestCase):
+    """InboundPayload unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_api_key_payload.py` & `elasticemail-4.1.0/test/test_models/test_segment_payload.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.access_level import AccessLevel
-globals()['AccessLevel'] = AccessLevel
-from ElasticEmail.model.api_key_payload import ApiKeyPayload
-
-
-class TestApiKeyPayload(unittest.TestCase):
-    """ApiKeyPayload unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.segment_payload import SegmentPayload
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testApiKeyPayload(self):
-        """Test ApiKeyPayload"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ApiKeyPayload()  # noqa: E501
-        pass
+class TestSegmentPayload(unittest.TestCase):
+    """SegmentPayload unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_body_content_type.py` & `elasticemail-4.1.0/test/test_models/test_options.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.body_content_type import BodyContentType
-
-
-class TestBodyContentType(unittest.TestCase):
-    """BodyContentType unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.options import Options
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testBodyContentType(self):
-        """Test BodyContentType"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = BodyContentType()  # noqa: E501
-        pass
+class TestOptions(unittest.TestCase):
+    """Options unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_body_part.py` & `elasticemail-4.1.0/test/test_models/test_verification_status.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.body_part import BodyPart
-
-
-class TestBodyPart(unittest.TestCase):
-    """BodyPart unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.verification_status import VerificationStatus
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testBodyPart(self):
-        """Test BodyPart"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = BodyPart()  # noqa: E501
-        pass
+class TestVerificationStatus(unittest.TestCase):
+    """VerificationStatus unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_campaign.py` & `elasticemail-4.1.0/test/test_models/test_campaign.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.campaign_template import CampaignTemplate
-globals()['CampaignTemplate'] = CampaignTemplate
 from ElasticEmail.model.campaign import Campaign
+from ElasticEmail import configuration
 
 
 class TestCampaign(unittest.TestCase):
     """Campaign unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testCampaign(self):
-        """Test Campaign"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = Campaign()  # noqa: E501
-        pass
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_campaign_options.py` & `elasticemail-4.1.0/test/test_models/test_campaign_options.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
 from ElasticEmail.model.campaign_options import CampaignOptions
+from ElasticEmail import configuration
 
 
 class TestCampaignOptions(unittest.TestCase):
     """CampaignOptions unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testCampaignOptions(self):
-        """Test CampaignOptions"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = CampaignOptions()  # noqa: E501
-        pass
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_campaign_recipient.py` & `elasticemail-4.1.0/test/test_models/test_email_validation_status.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.campaign_recipient import CampaignRecipient
-
-
-class TestCampaignRecipient(unittest.TestCase):
-    """CampaignRecipient unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.email_validation_status import EmailValidationStatus
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testCampaignRecipient(self):
-        """Test CampaignRecipient"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = CampaignRecipient()  # noqa: E501
-        pass
+class TestEmailValidationStatus(unittest.TestCase):
+    """EmailValidationStatus unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_campaign_status.py` & `elasticemail-4.1.0/test/test_models/test_email_predicted_validation_status.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.campaign_status import CampaignStatus
-
-
-class TestCampaignStatus(unittest.TestCase):
-    """CampaignStatus unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.email_predicted_validation_status import EmailPredictedValidationStatus
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testCampaignStatus(self):
-        """Test CampaignStatus"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = CampaignStatus()  # noqa: E501
-        pass
+class TestEmailPredictedValidationStatus(unittest.TestCase):
+    """EmailPredictedValidationStatus unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_campaign_template.py` & `elasticemail-4.1.0/test/test_models/test_campaign_status.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.campaign_template import CampaignTemplate
-
-
-class TestCampaignTemplate(unittest.TestCase):
-    """CampaignTemplate unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.campaign_status import CampaignStatus
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testCampaignTemplate(self):
-        """Test CampaignTemplate"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = CampaignTemplate()  # noqa: E501
-        pass
+class TestCampaignStatus(unittest.TestCase):
+    """CampaignStatus unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_channel_log_status_summary.py` & `elasticemail-4.1.0/test/test_models/test_email_job_status.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.channel_log_status_summary import ChannelLogStatusSummary
-
-
-class TestChannelLogStatusSummary(unittest.TestCase):
-    """ChannelLogStatusSummary unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.email_job_status import EmailJobStatus
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testChannelLogStatusSummary(self):
-        """Test ChannelLogStatusSummary"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ChannelLogStatusSummary()  # noqa: E501
-        pass
+class TestEmailJobStatus(unittest.TestCase):
+    """EmailJobStatus unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_compression_format.py` & `elasticemail-4.1.0/test/test_models/test_verification_file_result_details.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.compression_format import CompressionFormat
-
-
-class TestCompressionFormat(unittest.TestCase):
-    """CompressionFormat unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.verification_file_result_details import VerificationFileResultDetails
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testCompressionFormat(self):
-        """Test CompressionFormat"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = CompressionFormat()  # noqa: E501
-        pass
+class TestVerificationFileResultDetails(unittest.TestCase):
+    """VerificationFileResultDetails unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_consent_data.py` & `elasticemail-4.1.0/test/test_models/test_consent_tracking.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.consent_data import ConsentData
-
-
-class TestConsentData(unittest.TestCase):
-    """ConsentData unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.consent_tracking import ConsentTracking
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testConsentData(self):
-        """Test ConsentData"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ConsentData()  # noqa: E501
-        pass
+class TestConsentTracking(unittest.TestCase):
+    """ConsentTracking unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_consent_tracking.py` & `elasticemail-4.1.0/test/test_models/test_email_send.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.consent_tracking import ConsentTracking
-
-
-class TestConsentTracking(unittest.TestCase):
-    """ConsentTracking unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.email_send import EmailSend
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testConsentTracking(self):
-        """Test ConsentTracking"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ConsentTracking()  # noqa: E501
-        pass
+class TestEmailSend(unittest.TestCase):
+    """EmailSend unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_contact.py` & `elasticemail-4.1.0/test/test_models/test_consent_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
 from ElasticEmail.model.consent_data import ConsentData
-globals()['ConsentData'] = ConsentData
-from ElasticEmail.model.contact import Contact
-
-
-class TestContact(unittest.TestCase):
-    """Contact unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testContact(self):
-        """Test Contact"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = Contact()  # noqa: E501
-        pass
+class TestConsentData(unittest.TestCase):
+    """ConsentData unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_contact_activity.py` & `elasticemail-4.1.0/test/test_models/test_compression_format.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.contact_activity import ContactActivity
-
-
-class TestContactActivity(unittest.TestCase):
-    """ContactActivity unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.compression_format import CompressionFormat
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testContactActivity(self):
-        """Test ContactActivity"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ContactActivity()  # noqa: E501
-        pass
+class TestCompressionFormat(unittest.TestCase):
+    """CompressionFormat unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_contact_hist_event_type.py` & `elasticemail-4.1.0/test/test_models/test_file_payload.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.contact_hist_event_type import ContactHistEventType
-
-
-class TestContactHistEventType(unittest.TestCase):
-    """ContactHistEventType unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.file_payload import FilePayload
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testContactHistEventType(self):
-        """Test ContactHistEventType"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ContactHistEventType()  # noqa: E501
-        pass
+class TestFilePayload(unittest.TestCase):
+    """FilePayload unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_contact_history.py` & `elasticemail-4.1.0/test/test_models/test_subaccount_email_settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.contact_history import ContactHistory
-
-
-class TestContactHistory(unittest.TestCase):
-    """ContactHistory unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.subaccount_email_settings import SubaccountEmailSettings
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testContactHistory(self):
-        """Test ContactHistory"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ContactHistory()  # noqa: E501
-        pass
+class TestSubaccountEmailSettings(unittest.TestCase):
+    """SubaccountEmailSettings unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_contact_payload.py` & `elasticemail-4.1.0/test/test_models/test_list_update_payload.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.consent_data import ConsentData
-globals()['ConsentData'] = ConsentData
-from ElasticEmail.model.contact_payload import ContactPayload
-
-
-class TestContactPayload(unittest.TestCase):
-    """ContactPayload unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.list_update_payload import ListUpdatePayload
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testContactPayload(self):
-        """Test ContactPayload"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ContactPayload()  # noqa: E501
-        pass
+class TestListUpdatePayload(unittest.TestCase):
+    """ListUpdatePayload unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_contact_source.py` & `elasticemail-4.1.0/test/test_models/test_transactional_recipient.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.contact_source import ContactSource
-
-
-class TestContactSource(unittest.TestCase):
-    """ContactSource unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.transactional_recipient import TransactionalRecipient
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testContactSource(self):
-        """Test ContactSource"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ContactSource()  # noqa: E501
-        pass
+class TestTransactionalRecipient(unittest.TestCase):
+    """TransactionalRecipient unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_contact_status.py` & `elasticemail-4.1.0/test/test_models/test_email_status.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.contact_status import ContactStatus
-
-
-class TestContactStatus(unittest.TestCase):
-    """ContactStatus unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.email_status import EmailStatus
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testContactStatus(self):
-        """Test ContactStatus"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ContactStatus()  # noqa: E501
-        pass
+class TestEmailStatus(unittest.TestCase):
+    """EmailStatus unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_contact_update_payload.py` & `elasticemail-4.1.0/test/test_models/test_subaccount_email_settings_payload.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.contact_update_payload import ContactUpdatePayload
-
-
-class TestContactUpdatePayload(unittest.TestCase):
-    """ContactUpdatePayload unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.subaccount_email_settings_payload import SubaccountEmailSettingsPayload
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testContactUpdatePayload(self):
-        """Test ContactUpdatePayload"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ContactUpdatePayload()  # noqa: E501
-        pass
+class TestSubaccountEmailSettingsPayload(unittest.TestCase):
+    """SubaccountEmailSettingsPayload unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_contacts_list.py` & `elasticemail-4.1.0/test/test_models/test_events_order_by.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.contacts_list import ContactsList
-
-
-class TestContactsList(unittest.TestCase):
-    """ContactsList unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.events_order_by import EventsOrderBy
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testContactsList(self):
-        """Test ContactsList"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ContactsList()  # noqa: E501
-        pass
+class TestEventsOrderBy(unittest.TestCase):
+    """EventsOrderBy unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_delivery_optimization_type.py` & `elasticemail-4.1.0/test/test_models/test_delivery_optimization_type.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
 from ElasticEmail.model.delivery_optimization_type import DeliveryOptimizationType
+from ElasticEmail import configuration
 
 
 class TestDeliveryOptimizationType(unittest.TestCase):
     """DeliveryOptimizationType unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testDeliveryOptimizationType(self):
-        """Test DeliveryOptimizationType"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = DeliveryOptimizationType()  # noqa: E501
-        pass
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_email_content.py` & `elasticemail-4.1.0/test/test_models/test_body_content_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.body_part import BodyPart
-from ElasticEmail.model.message_attachment import MessageAttachment
-globals()['BodyPart'] = BodyPart
-globals()['MessageAttachment'] = MessageAttachment
-from ElasticEmail.model.email_content import EmailContent
-
-
-class TestEmailContent(unittest.TestCase):
-    """EmailContent unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testEmailContent(self):
-        """Test EmailContent"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = EmailContent()  # noqa: E501
-        pass
+from ElasticEmail.model.body_content_type import BodyContentType
+from ElasticEmail import configuration
+
+
+class TestBodyContentType(unittest.TestCase):
+    """BodyContentType unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_email_data.py` & `elasticemail-4.1.0/test/test_models/test_template_payload.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.file_info import FileInfo
-globals()['FileInfo'] = FileInfo
-from ElasticEmail.model.email_data import EmailData
-
-
-class TestEmailData(unittest.TestCase):
-    """EmailData unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.template_payload import TemplatePayload
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testEmailData(self):
-        """Test EmailData"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = EmailData()  # noqa: E501
-        pass
+class TestTemplatePayload(unittest.TestCase):
+    """TemplatePayload unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_email_message_data.py` & `elasticemail-4.1.0/test/test_models/test_api_key_payload.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.email_recipient import EmailRecipient
-globals()['EmailRecipient'] = EmailRecipient
-from ElasticEmail.model.email_message_data import EmailMessageData
-
-
-class TestEmailMessageData(unittest.TestCase):
-    """EmailMessageData unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.api_key_payload import ApiKeyPayload
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testEmailMessageData(self):
-        """Test EmailMessageData"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = EmailMessageData()  # noqa: E501
-        pass
+class TestApiKeyPayload(unittest.TestCase):
+    """ApiKeyPayload unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_email_recipient.py` & `elasticemail-4.1.0/test/test_models/test_campaign_recipient.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.email_recipient import EmailRecipient
-
-
-class TestEmailRecipient(unittest.TestCase):
-    """EmailRecipient unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.campaign_recipient import CampaignRecipient
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testEmailRecipient(self):
-        """Test EmailRecipient"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = EmailRecipient()  # noqa: E501
-        pass
+class TestCampaignRecipient(unittest.TestCase):
+    """CampaignRecipient unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_email_send.py` & `elasticemail-4.1.0/test/test_models/test_email_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.email_send import EmailSend
-
-
-class TestEmailSend(unittest.TestCase):
-    """EmailSend unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.email_data import EmailData
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testEmailSend(self):
-        """Test EmailSend"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = EmailSend()  # noqa: E501
-        pass
+class TestEmailData(unittest.TestCase):
+    """EmailData unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_email_status.py` & `elasticemail-4.1.0/test/test_models/test_inbound_route_action_type.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.email_status import EmailStatus
-
-
-class TestEmailStatus(unittest.TestCase):
-    """EmailStatus unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.inbound_route_action_type import InboundRouteActionType
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testEmailStatus(self):
-        """Test EmailStatus"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = EmailStatus()  # noqa: E501
-        pass
+class TestInboundRouteActionType(unittest.TestCase):
+    """InboundRouteActionType unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_email_validation_result.py` & `elasticemail-4.1.0/test/test_models/test_log_job_status.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.email_validation_status import EmailValidationStatus
-globals()['EmailValidationStatus'] = EmailValidationStatus
-from ElasticEmail.model.email_validation_result import EmailValidationResult
-
-
-class TestEmailValidationResult(unittest.TestCase):
-    """EmailValidationResult unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.log_job_status import LogJobStatus
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testEmailValidationResult(self):
-        """Test EmailValidationResult"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = EmailValidationResult()  # noqa: E501
-        pass
+class TestLogJobStatus(unittest.TestCase):
+    """LogJobStatus unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_email_validation_status.py` & `elasticemail-4.1.0/test/test_models/test_email_validation_result.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.email_validation_status import EmailValidationStatus
-
-
-class TestEmailValidationStatus(unittest.TestCase):
-    """EmailValidationStatus unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.email_validation_result import EmailValidationResult
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testEmailValidationStatus(self):
-        """Test EmailValidationStatus"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = EmailValidationStatus()  # noqa: E501
-        pass
+class TestEmailValidationResult(unittest.TestCase):
+    """EmailValidationResult unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_email_view.py` & `elasticemail-4.1.0/test/test_models/test_list_payload.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.email_view import EmailView
-
-
-class TestEmailView(unittest.TestCase):
-    """EmailView unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.list_payload import ListPayload
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testEmailView(self):
-        """Test EmailView"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = EmailView()  # noqa: E501
-        pass
+class TestListPayload(unittest.TestCase):
+    """ListPayload unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_emails_payload.py` & `elasticemail-4.1.0/test/test_models/test_contact_payload.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.emails_payload import EmailsPayload
-
-
-class TestEmailsPayload(unittest.TestCase):
-    """EmailsPayload unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.contact_payload import ContactPayload
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testEmailsPayload(self):
-        """Test EmailsPayload"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = EmailsPayload()  # noqa: E501
-        pass
+class TestContactPayload(unittest.TestCase):
+    """ContactPayload unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_encoding_type.py` & `elasticemail-4.1.0/test/test_models/test_event_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.encoding_type import EncodingType
-
-
-class TestEncodingType(unittest.TestCase):
-    """EncodingType unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.event_type import EventType
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testEncodingType(self):
-        """Test EncodingType"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = EncodingType()  # noqa: E501
-        pass
+class TestEventType(unittest.TestCase):
+    """EventType unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_event_type.py` & `elasticemail-4.1.0/test/test_models/test_verification_file_result.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.event_type import EventType
-
-
-class TestEventType(unittest.TestCase):
-    """EventType unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.verification_file_result import VerificationFileResult
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testEventType(self):
-        """Test EventType"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = EventType()  # noqa: E501
-        pass
+class TestVerificationFileResult(unittest.TestCase):
+    """VerificationFileResult unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_events_order_by.py` & `elasticemail-4.1.0/test/test_models/test_new_smtp_credentials.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.events_order_by import EventsOrderBy
-
-
-class TestEventsOrderBy(unittest.TestCase):
-    """EventsOrderBy unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.new_smtp_credentials import NewSmtpCredentials
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testEventsOrderBy(self):
-        """Test EventsOrderBy"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = EventsOrderBy()  # noqa: E501
-        pass
+class TestNewSmtpCredentials(unittest.TestCase):
+    """NewSmtpCredentials unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_export_file_formats.py` & `elasticemail-4.1.0/test/test_models/test_export_file_formats.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
 from ElasticEmail.model.export_file_formats import ExportFileFormats
+from ElasticEmail import configuration
 
 
 class TestExportFileFormats(unittest.TestCase):
     """ExportFileFormats unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testExportFileFormats(self):
-        """Test ExportFileFormats"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ExportFileFormats()  # noqa: E501
-        pass
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_export_link.py` & `elasticemail-4.1.0/test/test_models/test_email_view.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.export_link import ExportLink
-
-
-class TestExportLink(unittest.TestCase):
-    """ExportLink unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.email_view import EmailView
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testExportLink(self):
-        """Test ExportLink"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ExportLink()  # noqa: E501
-        pass
+class TestEmailView(unittest.TestCase):
+    """EmailView unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_export_status.py` & `elasticemail-4.1.0/test/test_models/test_message_attachment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.export_status import ExportStatus
-
-
-class TestExportStatus(unittest.TestCase):
-    """ExportStatus unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.message_attachment import MessageAttachment
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testExportStatus(self):
-        """Test ExportStatus"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ExportStatus()  # noqa: E501
-        pass
+class TestMessageAttachment(unittest.TestCase):
+    """MessageAttachment unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_file_info.py` & `elasticemail-4.1.0/test/test_models/test_channel_log_status_summary.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.file_info import FileInfo
-
-
-class TestFileInfo(unittest.TestCase):
-    """FileInfo unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.channel_log_status_summary import ChannelLogStatusSummary
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testFileInfo(self):
-        """Test FileInfo"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = FileInfo()  # noqa: E501
-        pass
+class TestChannelLogStatusSummary(unittest.TestCase):
+    """ChannelLogStatusSummary unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_inbound_route.py` & `elasticemail-4.1.0/test/test_models/test_inbound_route.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
 from ElasticEmail.model.inbound_route import InboundRoute
+from ElasticEmail import configuration
 
 
 class TestInboundRoute(unittest.TestCase):
     """InboundRoute unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testInboundRoute(self):
-        """Test InboundRoute"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = InboundRoute()  # noqa: E501
-        pass
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_inbound_route_action_type.py` & `elasticemail-4.1.0/test/test_models/test_contact_status.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.inbound_route_action_type import InboundRouteActionType
-
-
-class TestInboundRouteActionType(unittest.TestCase):
-    """InboundRouteActionType unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.contact_status import ContactStatus
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testInboundRouteActionType(self):
-        """Test InboundRouteActionType"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = InboundRouteActionType()  # noqa: E501
-        pass
+class TestContactStatus(unittest.TestCase):
+    """ContactStatus unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_inbound_route_filter_type.py` & `elasticemail-4.1.0/test/test_models/test_recipient_event.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.inbound_route_filter_type import InboundRouteFilterType
-
-
-class TestInboundRouteFilterType(unittest.TestCase):
-    """InboundRouteFilterType unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.recipient_event import RecipientEvent
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testInboundRouteFilterType(self):
-        """Test InboundRouteFilterType"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = InboundRouteFilterType()  # noqa: E501
-        pass
+class TestRecipientEvent(unittest.TestCase):
+    """RecipientEvent unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_list_payload.py` & `elasticemail-4.1.0/test/test_models/test_merge_email_payload.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.list_payload import ListPayload
-
-
-class TestListPayload(unittest.TestCase):
-    """ListPayload unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.merge_email_payload import MergeEmailPayload
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testListPayload(self):
-        """Test ListPayload"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ListPayload()  # noqa: E501
-        pass
+class TestMergeEmailPayload(unittest.TestCase):
+    """MergeEmailPayload unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_list_update_payload.py` & `elasticemail-4.1.0/test/test_models/test_emails_payload.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.list_update_payload import ListUpdatePayload
-
-
-class TestListUpdatePayload(unittest.TestCase):
-    """ListUpdatePayload unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.emails_payload import EmailsPayload
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testListUpdatePayload(self):
-        """Test ListUpdatePayload"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ListUpdatePayload()  # noqa: E501
-        pass
+class TestEmailsPayload(unittest.TestCase):
+    """EmailsPayload unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_log_job_status.py` & `elasticemail-4.1.0/test/test_models/test_account_status_enum.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.log_job_status import LogJobStatus
-
-
-class TestLogJobStatus(unittest.TestCase):
-    """LogJobStatus unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.account_status_enum import AccountStatusEnum
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testLogJobStatus(self):
-        """Test LogJobStatus"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = LogJobStatus()  # noqa: E501
-        pass
+class TestAccountStatusEnum(unittest.TestCase):
+    """AccountStatusEnum unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_log_status_summary.py` & `elasticemail-4.1.0/test/test_models/test_log_status_summary.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
 from ElasticEmail.model.log_status_summary import LogStatusSummary
+from ElasticEmail import configuration
 
 
 class TestLogStatusSummary(unittest.TestCase):
     """LogStatusSummary unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testLogStatusSummary(self):
-        """Test LogStatusSummary"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = LogStatusSummary()  # noqa: E501
-        pass
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_merge_email_payload.py` & `elasticemail-4.1.0/test/test_models/test_smtp_credentials_payload.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.merge_email_payload import MergeEmailPayload
-
-
-class TestMergeEmailPayload(unittest.TestCase):
-    """MergeEmailPayload unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.smtp_credentials_payload import SmtpCredentialsPayload
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testMergeEmailPayload(self):
-        """Test MergeEmailPayload"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = MergeEmailPayload()  # noqa: E501
-        pass
+class TestSmtpCredentialsPayload(unittest.TestCase):
+    """SmtpCredentialsPayload unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_message_attachment.py` & `elasticemail-4.1.0/test/test_models/test_email_recipient.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.message_attachment import MessageAttachment
-
-
-class TestMessageAttachment(unittest.TestCase):
-    """MessageAttachment unit test stubs"""
-
-    def setUp(self):
-        pass
+from ElasticEmail.model.email_recipient import EmailRecipient
+from ElasticEmail import configuration
 
-    def tearDown(self):
-        pass
 
-    def testMessageAttachment(self):
-        """Test MessageAttachment"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = MessageAttachment()  # noqa: E501
-        pass
+class TestEmailRecipient(unittest.TestCase):
+    """EmailRecipient unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_message_category.py` & `elasticemail-4.1.0/test/test_models/test_message_category.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,26 @@
+# coding: utf-8
+
 """
     Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    To start using this API, you will need your Access Token (available <a href=\"https://elasticemail.com/account#/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    This is the documentation for REST API. If you’d like to read our legacy documentation regarding Web API v2 click <a href=\"https://api.elasticemail.com/public/help\">here</a>.  # noqa: E501
+    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
     The version of the OpenAPI document: 4.0.0
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
 import ElasticEmail
 from ElasticEmail.model.message_category import MessageCategory
+from ElasticEmail import configuration
 
 
 class TestMessageCategory(unittest.TestCase):
     """MessageCategory unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testMessageCategory(self):
-        """Test MessageCategory"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = MessageCategory()  # noqa: E501
-        pass
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_access_level.py` & `elasticemail-4.1.0/test/test_models/test_access_level.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_models/test_account_status_enum.py` & `elasticemail-4.1.0/test/test_models/test_subaccount_settings_info_payload.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.account_status_enum import AccountStatusEnum
+from ElasticEmail.model.subaccount_settings_info_payload import SubaccountSettingsInfoPayload
 from ElasticEmail import configuration
 
 
-class TestAccountStatusEnum(unittest.TestCase):
-    """AccountStatusEnum unit test stubs"""
+class TestSubaccountSettingsInfoPayload(unittest.TestCase):
+    """SubaccountSettingsInfoPayload unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_api_key.py` & `elasticemail-4.1.0/test/test_models/test_api_key.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_models/test_api_key_payload.py` & `elasticemail-4.1.0/test/test_models/test_email_content.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.api_key_payload import ApiKeyPayload
+from ElasticEmail.model.email_content import EmailContent
 from ElasticEmail import configuration
 
 
-class TestApiKeyPayload(unittest.TestCase):
-    """ApiKeyPayload unit test stubs"""
+class TestEmailContent(unittest.TestCase):
+    """EmailContent unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_body_content_type.py` & `elasticemail-4.1.0/test/test_models/test_utm.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.body_content_type import BodyContentType
+from ElasticEmail.model.utm import Utm
 from ElasticEmail import configuration
 
 
-class TestBodyContentType(unittest.TestCase):
-    """BodyContentType unit test stubs"""
+class TestUtm(unittest.TestCase):
+    """Utm unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_body_part.py` & `elasticemail-4.1.0/test/test_models/test_body_part.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_models/test_campaign.py` & `elasticemail-4.1.0/test/test_models/test_contacts_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.campaign import Campaign
+from ElasticEmail.model.contacts_list import ContactsList
 from ElasticEmail import configuration
 
 
-class TestCampaign(unittest.TestCase):
-    """Campaign unit test stubs"""
+class TestContactsList(unittest.TestCase):
+    """ContactsList unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_campaign_options.py` & `elasticemail-4.1.0/test/test_models/test_sort_order_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.campaign_options import CampaignOptions
+from ElasticEmail.model.sort_order_item import SortOrderItem
 from ElasticEmail import configuration
 
 
-class TestCampaignOptions(unittest.TestCase):
-    """CampaignOptions unit test stubs"""
+class TestSortOrderItem(unittest.TestCase):
+    """SortOrderItem unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_campaign_recipient.py` & `elasticemail-4.1.0/test/test_models/test_new_api_key.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.campaign_recipient import CampaignRecipient
+from ElasticEmail.model.new_api_key import NewApiKey
 from ElasticEmail import configuration
 
 
-class TestCampaignRecipient(unittest.TestCase):
-    """CampaignRecipient unit test stubs"""
+class TestNewApiKey(unittest.TestCase):
+    """NewApiKey unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_campaign_status.py` & `elasticemail-4.1.0/test/test_models/test_file_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.campaign_status import CampaignStatus
+from ElasticEmail.model.file_info import FileInfo
 from ElasticEmail import configuration
 
 
-class TestCampaignStatus(unittest.TestCase):
-    """CampaignStatus unit test stubs"""
+class TestFileInfo(unittest.TestCase):
+    """FileInfo unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_campaign_template.py` & `elasticemail-4.1.0/test/test_models/test_campaign_template.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_models/test_channel_log_status_summary.py` & `elasticemail-4.1.0/test/test_models/test_suppression.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.channel_log_status_summary import ChannelLogStatusSummary
+from ElasticEmail.model.suppression import Suppression
 from ElasticEmail import configuration
 
 
-class TestChannelLogStatusSummary(unittest.TestCase):
-    """ChannelLogStatusSummary unit test stubs"""
+class TestSuppression(unittest.TestCase):
+    """Suppression unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_compression_format.py` & `elasticemail-4.1.0/test/test_models/test_template_scope.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.compression_format import CompressionFormat
+from ElasticEmail.model.template_scope import TemplateScope
 from ElasticEmail import configuration
 
 
-class TestCompressionFormat(unittest.TestCase):
-    """CompressionFormat unit test stubs"""
+class TestTemplateScope(unittest.TestCase):
+    """TemplateScope unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_consent_data.py` & `elasticemail-4.1.0/test/test_models/test_contact.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.consent_data import ConsentData
+from ElasticEmail.model.contact import Contact
 from ElasticEmail import configuration
 
 
-class TestConsentData(unittest.TestCase):
-    """ConsentData unit test stubs"""
+class TestContact(unittest.TestCase):
+    """Contact unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_consent_tracking.py` & `elasticemail-4.1.0/test/test_models/test_file_upload_result.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.consent_tracking import ConsentTracking
+from ElasticEmail.model.file_upload_result import FileUploadResult
 from ElasticEmail import configuration
 
 
-class TestConsentTracking(unittest.TestCase):
-    """ConsentTracking unit test stubs"""
+class TestFileUploadResult(unittest.TestCase):
+    """FileUploadResult unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_contact.py` & `elasticemail-4.1.0/test/test_models/test_segment.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.contact import Contact
+from ElasticEmail.model.segment import Segment
 from ElasticEmail import configuration
 
 
-class TestContact(unittest.TestCase):
-    """Contact unit test stubs"""
+class TestSegment(unittest.TestCase):
+    """Segment unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_contact_activity.py` & `elasticemail-4.1.0/test/test_models/test_contact_activity.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_models/test_contact_payload.py` & `elasticemail-4.1.0/test/test_models/test_smtp_credentials.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.contact_payload import ContactPayload
+from ElasticEmail.model.smtp_credentials import SmtpCredentials
 from ElasticEmail import configuration
 
 
-class TestContactPayload(unittest.TestCase):
-    """ContactPayload unit test stubs"""
+class TestSmtpCredentials(unittest.TestCase):
+    """SmtpCredentials unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_contact_source.py` & `elasticemail-4.1.0/test/test_models/test_contact_source.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_models/test_contact_status.py` & `elasticemail-4.1.0/test/test_models/test_email_message_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.contact_status import ContactStatus
+from ElasticEmail.model.email_message_data import EmailMessageData
 from ElasticEmail import configuration
 
 
-class TestContactStatus(unittest.TestCase):
-    """ContactStatus unit test stubs"""
+class TestEmailMessageData(unittest.TestCase):
+    """EmailMessageData unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_contact_update_payload.py` & `elasticemail-4.1.0/test/test_models/test_template_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.contact_update_payload import ContactUpdatePayload
+from ElasticEmail.model.template_type import TemplateType
 from ElasticEmail import configuration
 
 
-class TestContactUpdatePayload(unittest.TestCase):
-    """ContactUpdatePayload unit test stubs"""
+class TestTemplateType(unittest.TestCase):
+    """TemplateType unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_contacts_list.py` & `elasticemail-4.1.0/test/test_models/test_email_job_failed_status.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.contacts_list import ContactsList
+from ElasticEmail.model.email_job_failed_status import EmailJobFailedStatus
 from ElasticEmail import configuration
 
 
-class TestContactsList(unittest.TestCase):
-    """ContactsList unit test stubs"""
+class TestEmailJobFailedStatus(unittest.TestCase):
+    """EmailJobFailedStatus unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_delivery_optimization_type.py` & `elasticemail-4.1.0/test/test_models/test_split_optimization_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.delivery_optimization_type import DeliveryOptimizationType
+from ElasticEmail.model.split_optimization_type import SplitOptimizationType
 from ElasticEmail import configuration
 
 
-class TestDeliveryOptimizationType(unittest.TestCase):
-    """DeliveryOptimizationType unit test stubs"""
+class TestSplitOptimizationType(unittest.TestCase):
+    """SplitOptimizationType unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_email_content.py` & `elasticemail-4.1.0/test/test_models/test_split_options.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.email_content import EmailContent
+from ElasticEmail.model.split_options import SplitOptions
 from ElasticEmail import configuration
 
 
-class TestEmailContent(unittest.TestCase):
-    """EmailContent unit test stubs"""
+class TestSplitOptions(unittest.TestCase):
+    """SplitOptions unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_email_data.py` & `elasticemail-4.1.0/test/test_models/test_template.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.email_data import EmailData
+from ElasticEmail.model.template import Template
 from ElasticEmail import configuration
 
 
-class TestEmailData(unittest.TestCase):
-    """EmailData unit test stubs"""
+class TestTemplate(unittest.TestCase):
+    """Template unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_email_message_data.py` & `elasticemail-4.1.0/test/test_models/test_export_link.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.email_message_data import EmailMessageData
+from ElasticEmail.model.export_link import ExportLink
 from ElasticEmail import configuration
 
 
-class TestEmailMessageData(unittest.TestCase):
-    """EmailMessageData unit test stubs"""
+class TestExportLink(unittest.TestCase):
+    """ExportLink unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_email_predicted_validation_status.py` & `elasticemail-4.1.0/test/test_models/test_encoding_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.email_predicted_validation_status import EmailPredictedValidationStatus
+from ElasticEmail.model.encoding_type import EncodingType
 from ElasticEmail import configuration
 
 
-class TestEmailPredictedValidationStatus(unittest.TestCase):
-    """EmailPredictedValidationStatus unit test stubs"""
+class TestEncodingType(unittest.TestCase):
+    """EncodingType unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_email_recipient.py` & `elasticemail-4.1.0/test/test_models/test_subaccount_settings_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.email_recipient import EmailRecipient
+from ElasticEmail.model.subaccount_settings_info import SubaccountSettingsInfo
 from ElasticEmail import configuration
 
 
-class TestEmailRecipient(unittest.TestCase):
-    """EmailRecipient unit test stubs"""
+class TestSubaccountSettingsInfo(unittest.TestCase):
+    """SubaccountSettingsInfo unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_email_send.py` & `elasticemail-4.1.0/test/test_models/test_email_transactional_message_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.email_send import EmailSend
+from ElasticEmail.model.email_transactional_message_data import EmailTransactionalMessageData
 from ElasticEmail import configuration
 
 
-class TestEmailSend(unittest.TestCase):
-    """EmailSend unit test stubs"""
+class TestEmailTransactionalMessageData(unittest.TestCase):
+    """EmailTransactionalMessageData unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_email_status.py` & `elasticemail-4.1.0/test/test_models/test_sub_account_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.email_status import EmailStatus
+from ElasticEmail.model.sub_account_info import SubAccountInfo
 from ElasticEmail import configuration
 
 
-class TestEmailStatus(unittest.TestCase):
-    """EmailStatus unit test stubs"""
+class TestSubAccountInfo(unittest.TestCase):
+    """SubAccountInfo unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_email_transactional_message_data.py` & `elasticemail-4.1.0/test/test_models/test_inbound_route_filter_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.email_transactional_message_data import EmailTransactionalMessageData
+from ElasticEmail.model.inbound_route_filter_type import InboundRouteFilterType
 from ElasticEmail import configuration
 
 
-class TestEmailTransactionalMessageData(unittest.TestCase):
-    """EmailTransactionalMessageData unit test stubs"""
+class TestInboundRouteFilterType(unittest.TestCase):
+    """InboundRouteFilterType unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_email_validation_result.py` & `elasticemail-4.1.0/test/test_models/test_subaccount_payload.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.email_validation_result import EmailValidationResult
+from ElasticEmail.model.subaccount_payload import SubaccountPayload
 from ElasticEmail import configuration
 
 
-class TestEmailValidationResult(unittest.TestCase):
-    """EmailValidationResult unit test stubs"""
+class TestSubaccountPayload(unittest.TestCase):
+    """SubaccountPayload unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_email_validation_status.py` & `elasticemail-4.1.0/test/test_paths/test_subaccounts_email_settings_email/test_put.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,43 @@
 # coding: utf-8
 
 """
-    Elastic Email REST API
 
-    This API is based on the REST API architecture, allowing the user to easily manage their data with this resource-based approach.    Every API call is established on which specific request type (GET, POST, PUT, DELETE) will be used.    The API has a limit of 20 concurrent connections and a hard timeout of 600 seconds per request.    To start using this API, you will need your Access Token (available <a target=\"_blank\" href=\"https://app.elasticemail.com/marketing/settings/new/manage-api\">here</a>). Remember to keep it safe. Required access levels are listed in the given request’s description.    Downloadable library clients can be found in our Github repository <a target=\"_blank\" href=\"https://github.com/ElasticEmail?tab=repositories&q=%22rest+api%22+in%3Areadme\">here</a>  # noqa: E501
 
-    The version of the OpenAPI document: 4.0.0
-    Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
+from unittest.mock import patch
+
+import urllib3
 
 import ElasticEmail
-from ElasticEmail.model.email_validation_status import EmailValidationStatus
-from ElasticEmail import configuration
+from ElasticEmail.paths.subaccounts_email_settings_email import put  # noqa: E501
+from ElasticEmail import configuration, schemas, api_client
+
+from .. import ApiTestMixin
 
 
-class TestEmailValidationStatus(unittest.TestCase):
-    """EmailValidationStatus unit test stubs"""
+class TestSubaccountsEmailSettingsEmail(ApiTestMixin, unittest.TestCase):
+    """
+    SubaccountsEmailSettingsEmail unit test stubs
+        Update SubAccount Email Settings  # noqa: E501
+    """
     _configuration = configuration.Configuration()
 
+    def setUp(self):
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+
+    def tearDown(self):
+        pass
+
+    response_status = 201
+
+
+
+
+
 
 if __name__ == '__main__':
     unittest.main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ElasticEmail-4.0.24/test/test_models/test_email_view.py` & `elasticemail-4.1.0/test/test_models/test_subaccount_email_credits_payload.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: support@elasticemail.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import ElasticEmail
-from ElasticEmail.model.email_view import EmailView
+from ElasticEmail.model.subaccount_email_credits_payload import SubaccountEmailCreditsPayload
 from ElasticEmail import configuration
 
 
-class TestEmailView(unittest.TestCase):
-    """EmailView unit test stubs"""
+class TestSubaccountEmailCreditsPayload(unittest.TestCase):
+    """SubaccountEmailCreditsPayload unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_paths/__init__.py` & `elasticemail-4.1.0/test/test_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_campaigns/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_campaigns/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_campaigns/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_campaigns/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_campaigns_name/test_delete.py` & `elasticemail-4.1.0/test/test_paths/test_campaigns_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_campaigns_name/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_campaigns_name/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_campaigns_name/test_put.py` & `elasticemail-4.1.0/test/test_paths/test_campaigns_name/test_put.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_contacts/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_contacts/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_contacts/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_contacts/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_contacts_delete/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_contacts_delete/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_contacts_email/test_delete.py` & `elasticemail-4.1.0/test/test_paths/test_contacts_email/test_delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_contacts_email/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_contacts_email/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_contacts_email/test_put.py` & `elasticemail-4.1.0/test/test_paths/test_contacts_email/test_put.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_contacts_export/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_contacts_export/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_contacts_export_id_status/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_contacts_export_id_status/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_contacts_import/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_contacts_import/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_emails/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_emails/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_emails_mergefile/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_emails_mergefile/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_emails_msgid_view/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_emails_msgid_view/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_emails_transactional/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_emails_transactional/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_events/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_events/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_events_channels_export_id_status/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_events_channels_export_id_status/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_events_channels_name/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_events_channels_name/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_events_channels_name_export/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_events_channels_name_export/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_events_export/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_events_export/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_events_export_id_status/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_events_export_id_status/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_events_transactionid/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_events_transactionid/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_files/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_files/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_files/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_files/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_files_name/test_delete.py` & `elasticemail-4.1.0/test/test_paths/test_files_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_files_name/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_files_name/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_files_name_info/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_files_name_info/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_inboundroute/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_inboundroute/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_inboundroute/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_inboundroute/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_inboundroute_id/test_delete.py` & `elasticemail-4.1.0/test/test_paths/test_inboundroute_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_inboundroute_id/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_inboundroute_id/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_inboundroute_id/test_put.py` & `elasticemail-4.1.0/test/test_paths/test_inboundroute_id/test_put.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_inboundroute_order/test_put.py` & `elasticemail-4.1.0/test/test_paths/test_inboundroute_order/test_put.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_lists/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_lists/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_lists/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_lists/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_lists_name/test_delete.py` & `elasticemail-4.1.0/test/test_paths/test_lists_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_lists_name/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_lists_name/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_lists_name/test_put.py` & `elasticemail-4.1.0/test/test_paths/test_lists_name/test_put.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_lists_name_contacts/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_lists_name_contacts/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_lists_name_contacts_remove/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_lists_name_contacts_remove/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_security_apikeys/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_security_apikeys/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_security_apikeys/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_security_apikeys/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_security_apikeys_name/test_delete.py` & `elasticemail-4.1.0/test/test_paths/test_security_apikeys_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_security_apikeys_name/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_security_apikeys_name/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_security_apikeys_name/test_put.py` & `elasticemail-4.1.0/test/test_paths/test_security_apikeys_name/test_put.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_security_smtp/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_security_smtp/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_security_smtp/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_security_smtp/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_security_smtp_name/test_delete.py` & `elasticemail-4.1.0/test/test_paths/test_security_smtp_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_security_smtp_name/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_security_smtp_name/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_security_smtp_name/test_put.py` & `elasticemail-4.1.0/test/test_paths/test_security_smtp_name/test_put.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_segments/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_segments/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_segments/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_segments/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_segments_name/test_delete.py` & `elasticemail-4.1.0/test/test_paths/test_segments_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_segments_name/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_segments_name/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_segments_name/test_put.py` & `elasticemail-4.1.0/test/test_paths/test_segments_name/test_put.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_statistics/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_statistics/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_statistics_campaigns/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_statistics_campaigns/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_statistics_campaigns_name/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_statistics_campaigns_name/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_statistics_channels/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_statistics_channels/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_statistics_channels_name/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_statistics_channels_name/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_subaccounts/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_subaccounts/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_subaccounts/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_subaccounts/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_subaccounts_email/test_delete.py` & `elasticemail-4.1.0/test/test_paths/test_subaccounts_email/test_delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_subaccounts_email/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_subaccounts_email/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_subaccounts_email_credits/test_patch.py` & `elasticemail-4.1.0/test/test_paths/test_subaccounts_email_credits/test_patch.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_subaccounts_email_settings_email/test_put.py` & `elasticemail-4.1.0/test/test_paths/test_suppressions_unsubscribes_import/test_post.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,36 +8,33 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import ElasticEmail
-from ElasticEmail.paths.subaccounts_email_settings_email import put  # noqa: E501
+from ElasticEmail.paths.suppressions_unsubscribes_import import post  # noqa: E501
 from ElasticEmail import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestSubaccountsEmailSettingsEmail(ApiTestMixin, unittest.TestCase):
+class TestSuppressionsUnsubscribesImport(ApiTestMixin, unittest.TestCase):
     """
-    SubaccountsEmailSettingsEmail unit test stubs
-        Update SubAccount Email Settings  # noqa: E501
+    SuppressionsUnsubscribesImport unit test stubs
+        Add Unsubscribes Async  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 201
-
-
-
-
+    response_status = 202
+    response_body = ''
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_suppressions/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_suppressions/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_suppressions_bounces/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_suppressions_bounces/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_suppressions_bounces/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_suppressions_bounces/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_suppressions_bounces_import/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_suppressions_bounces_import/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_suppressions_complaints/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_suppressions_complaints/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_suppressions_complaints/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_suppressions_complaints/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_suppressions_complaints_import/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_suppressions_complaints_import/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_suppressions_email/test_delete.py` & `elasticemail-4.1.0/test/test_paths/test_suppressions_email/test_delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_suppressions_email/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_suppressions_email/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_suppressions_unsubscribes/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_suppressions_unsubscribes/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_suppressions_unsubscribes/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_suppressions_unsubscribes/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_suppressions_unsubscribes_import/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_templates/test_post.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,33 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import ElasticEmail
-from ElasticEmail.paths.suppressions_unsubscribes_import import post  # noqa: E501
+from ElasticEmail.paths.templates import post  # noqa: E501
 from ElasticEmail import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestSuppressionsUnsubscribesImport(ApiTestMixin, unittest.TestCase):
+class TestTemplates(ApiTestMixin, unittest.TestCase):
     """
-    SuppressionsUnsubscribesImport unit test stubs
-        Add Unsubscribes Async  # noqa: E501
+    Templates unit test stubs
+        Add Template  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 202
-    response_body = ''
+    response_status = 201
+
+
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_templates/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_templates/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_templates/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_templates_name/test_delete.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,36 +8,33 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import ElasticEmail
-from ElasticEmail.paths.templates import post  # noqa: E501
+from ElasticEmail.paths.templates_name import delete  # noqa: E501
 from ElasticEmail import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestTemplates(ApiTestMixin, unittest.TestCase):
+class TestTemplatesName(ApiTestMixin, unittest.TestCase):
     """
-    Templates unit test stubs
-        Add Template  # noqa: E501
+    TemplatesName unit test stubs
+        Delete Template  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 201
-
-
-
-
+    response_status = 200
+    response_body = ''
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_templates_name/test_delete.py` & `elasticemail-4.1.0/test/test_paths/test_templates_name/test_get.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,33 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import ElasticEmail
-from ElasticEmail.paths.templates_name import delete  # noqa: E501
+from ElasticEmail.paths.templates_name import get  # noqa: E501
 from ElasticEmail import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestTemplatesName(ApiTestMixin, unittest.TestCase):
     """
     TemplatesName unit test stubs
-        Delete Template  # noqa: E501
+        Load Template  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
     response_status = 200
-    response_body = ''
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_templates_name/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_templates_name/test_put.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import ElasticEmail
-from ElasticEmail.paths.templates_name import get  # noqa: E501
+from ElasticEmail.paths.templates_name import put  # noqa: E501
 from ElasticEmail import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestTemplatesName(ApiTestMixin, unittest.TestCase):
     """
     TemplatesName unit test stubs
-        Load Template  # noqa: E501
+        Update Template  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
     response_status = 200
 
 
 
 
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_templates_name/test_put.py` & `elasticemail-4.1.0/test/test_paths/test_verifications_files/test_post.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import ElasticEmail
-from ElasticEmail.paths.templates_name import put  # noqa: E501
+from ElasticEmail.paths.verifications_files import post  # noqa: E501
 from ElasticEmail import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestTemplatesName(ApiTestMixin, unittest.TestCase):
+class TestVerificationsFiles(ApiTestMixin, unittest.TestCase):
     """
-    TemplatesName unit test stubs
-        Update Template  # noqa: E501
+    VerificationsFiles unit test stubs
+        Upload File with Emails  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
     response_status = 200
 
 
 
 
-
-
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_verifications/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_verifications/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_verifications_email/test_delete.py` & `elasticemail-4.1.0/test/test_paths/test_verifications_email/test_delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_verifications_email/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_verifications_email/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_verifications_email/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_verifications_email/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_verifications_files/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_verifications_files_result/test_get.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import ElasticEmail
-from ElasticEmail.paths.verifications_files import post  # noqa: E501
+from ElasticEmail.paths.verifications_files_result import get  # noqa: E501
 from ElasticEmail import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestVerificationsFiles(ApiTestMixin, unittest.TestCase):
+class TestVerificationsFilesResult(ApiTestMixin, unittest.TestCase):
     """
-    VerificationsFiles unit test stubs
-        Upload File with Emails  # noqa: E501
+    VerificationsFilesResult unit test stubs
+        Get Files Verification Results  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
     response_status = 200
```

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_verifications_files_id/test_delete.py` & `elasticemail-4.1.0/test/test_paths/test_verifications_files_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_verifications_files_id_result/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_verifications_files_id_result/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_verifications_files_id_result_download/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_verifications_files_id_result_download/test_get.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_verifications_files_id_verification/test_post.py` & `elasticemail-4.1.0/test/test_paths/test_verifications_files_id_verification/test_post.py`

 * *Files identical despite different names*

### Comparing `ElasticEmail-4.0.24/test/test_paths/test_verifications_files_result/test_get.py` & `elasticemail-4.1.0/test/test_paths/test_emails_transactionid_status/test_get.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import ElasticEmail
-from ElasticEmail.paths.verifications_files_result import get  # noqa: E501
+from ElasticEmail.paths.emails_transactionid_status import get  # noqa: E501
 from ElasticEmail import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestVerificationsFilesResult(ApiTestMixin, unittest.TestCase):
+class TestEmailsTransactionidStatus(ApiTestMixin, unittest.TestCase):
     """
-    VerificationsFilesResult unit test stubs
-        Get Files Verification Results  # noqa: E501
+    EmailsTransactionidStatus unit test stubs
+        Get Status  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
```

