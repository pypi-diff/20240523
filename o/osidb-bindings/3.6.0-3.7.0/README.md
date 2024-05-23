# Comparing `tmp/osidb-bindings-3.6.0.tar.gz` & `tmp/osidb_bindings-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osidb-bindings-3.6.0.tar", last modified: Mon Jan 29 16:02:54 2024, max compression
+gzip compressed data, was "osidb_bindings-3.7.0.tar", last modified: Thu May 23 12:12:36 2024, max compression
```

## Comparing `osidb-bindings-3.6.0.tar` & `osidb_bindings-3.7.0.tar`

### file list

```diff
@@ -1,337 +1,362 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:02:54.704393 osidb-bindings-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-01-29 16:02:54.704393 osidb-bindings-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:02:54.652393 osidb-bindings-3.6.0/osidb_bindings/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:02:54.652393 osidb-bindings-3.6.0/osidb_bindings/bindings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:02:54.652393 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:02:54.652393 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:02:54.652393 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/auth/auth_token_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/auth/auth_token_refresh_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/auth/auth_token_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/auth/auth_token_verify_create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:02:54.652393 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/collectors/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/collectors/collectors_api_v1_status_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/collectors/collectors_healthy_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/collectors/collectors_retrieve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:02:54.656393 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/exploits/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/exploits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_collect_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_cve_map_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_epss_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_flaw_data_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_data_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_date_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_explanations_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_pending_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_status_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_supported_products_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:02:54.664393 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_cvss_scores_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_cvss_scores_destroy.py
--rw-r--r--   0 runner    (1001) docker     (127)    20792 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_cvss_scores_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_cvss_scores_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_cvss_scores_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_destroy.py
--rw-r--r--   0 runner    (1001) docker     (127)   108374 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_acknowledgments_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_acknowledgments_destroy.py
--rw-r--r--   0 runner    (1001) docker     (127)    20435 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_acknowledgments_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_acknowledgments_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_acknowledgments_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_cvss_scores_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_cvss_scores_destroy.py
--rw-r--r--   0 runner    (1001) docker     (127)    20720 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_cvss_scores_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_cvss_scores_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_cvss_scores_update.py
--rw-r--r--   0 runner    (1001) docker     (127)   175984 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_package_versions_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_package_versions_destroy.py
--rw-r--r--   0 runner    (1001) docker     (127)    19235 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_package_versions_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_package_versions_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_package_versions_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_promote_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_destroy.py
--rw-r--r--   0 runner    (1001) docker     (127)    20673 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_reject_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_manifest_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_schema_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_status_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    97360 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_healthy_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_whoami_retrieve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:02:54.664393 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osim/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_adjust_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osim/osim_healthy_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osim/osim_retrieve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:02:54.664393 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/trackers/trackers_api_v1_file_create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:02:54.668393 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/workflows/workflows_api_v1_adjust_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/workflows/workflows_api_v1_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/workflows/workflows_api_v1_retrieve_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/workflows/workflows_healthy_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/workflows/workflows_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:02:54.704393 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)    17316 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21110 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/affect.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/affect_cvss.py
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/affect_cvss_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/affect_cvss_put.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/affect_meta_attr.py
--rw-r--r--   0 runner    (1001) docker     (127)    20355 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/affect_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/affect_post_meta_attr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/affect_report_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/affect_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/affectedness_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/auth_token_create_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/auth_token_refresh_create_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/auth_token_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/auth_token_verify_create_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/blank_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/collectors_healthy_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/collectors_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/comment_meta_attr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/epss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/erratum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploit_only_report_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploit_only_report_data_source_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_collect_update_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200_cves.py
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_epss_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_flaw_data_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_data_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_action_required_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_no_action_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_not_relevant_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200_explanations_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200_pending_actions_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_status_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_supported_products_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)    47737 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_acknowledgment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_acknowledgment_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_acknowledgment_put.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_classification_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_comment_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_comment_post_meta_attr.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_comment_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_cvss.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_cvss_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_cvss_put.py
--rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_meta_attr.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_meta_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_package_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_package_version_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_package_version_put.py
--rw-r--r--   0 runner    (1001) docker     (127)    47007 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_post_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_post_classification_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     9749 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_post_meta_attr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_reference_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_reference_put.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_reference_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_report_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_uuid_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/impact_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/issuer_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/major_incident_state_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/maturity_preliminary_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/meta_meta_attr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/module_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/nist_cvss_validation_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    15815 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_create_response_201.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_create_response_201.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_destroy_response_204.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_list_issuer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_update_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_destroy_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_affectedness.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_cvss_scores_issuer.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_flaw_impact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_flaw_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_flaw_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_impact.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_order_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_trackers_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    15825 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)    15815 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_update_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_acknowledgments_create_response_201.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_acknowledgments_destroy_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_acknowledgments_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_acknowledgments_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_acknowledgments_update_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_create_response_201.py
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)    33142 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_create_response_201.py
--rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_cvss_scores_create_response_201.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_cvss_scores_destroy_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_cvss_scores_list_issuer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_cvss_scores_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_cvss_scores_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_cvss_scores_update_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_affectedness.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_impact.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_trackers_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_cvss_scores_issuer.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_impact.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_major_incident_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_nist_cvss_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_order_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_references_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_requires_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_package_versions_create_response_201.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_package_versions_destroy_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_package_versions_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_package_versions_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_package_versions_update_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_promote_create_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_create_response_201.py
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_destroy_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_list_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_update_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_reject_create_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)    33152 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)    33142 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_update_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_manifest_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_lang.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8097 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_create_response_201.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_affectedness.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_flaw_impact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_flaw_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_flaw_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_impact.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_order_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     8107 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     8097 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_update_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_healthy_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_adjust_create_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_2_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osim_healthy_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osim_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/package.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/package_ver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_affect_cvss_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_affect_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_epss_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_exploit_only_report_data_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_flaw_acknowledgment_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_flaw_comment_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_flaw_cvss_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_flaw_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_flaw_package_version_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_flaw_reference_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_flaw_report_data_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_supported_products_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_tracker_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/ps_stream_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/reject.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/requires_summary_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/resolution_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/source_8d8_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/supported_products.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/token_obtain_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/token_refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/token_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/tracker_meta_attr.py
--rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/tracker_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/tracker_post_meta_attr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/tracker_report_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/tracker_suggestion.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/tracker_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/workflows_api_v1_adjust_create_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/workflows_api_v1_retrieve_2_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/workflows_api_v1_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/workflows_healthy_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/workflows_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)    16880 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/osidb_bindings/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:02:54.704393 osidb-bindings-3.6.0/osidb_bindings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-01-29 16:02:54.000000 osidb-bindings-3.6.0/osidb_bindings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    25200 2024-01-29 16:02:54.000000 osidb-bindings-3.6.0/osidb_bindings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 16:02:54.000000 osidb-bindings-3.6.0/osidb_bindings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-29 16:02:54.000000 osidb-bindings-3.6.0/osidb_bindings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-29 16:02:54.000000 osidb-bindings-3.6.0/osidb_bindings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 16:02:54.704393 osidb-bindings-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:02:54.704393 osidb-bindings-3.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-01-29 16:02:42.000000 osidb-bindings-3.6.0/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:36.052259 osidb_bindings-3.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-23 12:12:36.052259 osidb_bindings-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:35.996258 osidb_bindings-3.7.0/osidb_bindings/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:35.996258 osidb_bindings-3.7.0/osidb_bindings/bindings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:35.996258 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:35.996258 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:35.996258 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/auth/auth_token_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/auth/auth_token_refresh_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/auth/auth_token_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/auth/auth_token_verify_create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:35.996258 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/collectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/collectors/collectors_api_v1_status_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/collectors/collectors_healthy_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/collectors/collectors_retrieve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:36.000258 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/exploits/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/exploits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_collect_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_cve_map_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_epss_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_flaw_data_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_data_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_date_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_explanations_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_pending_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_status_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_supported_products_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:36.008258 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_cvss_scores_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_cvss_scores_destroy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20792 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_cvss_scores_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_cvss_scores_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_cvss_scores_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_destroy.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109468 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_acknowledgments_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_acknowledgments_destroy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20435 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_acknowledgments_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_acknowledgments_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_acknowledgments_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_cvss_scores_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_cvss_scores_destroy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20720 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_cvss_scores_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_cvss_scores_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_cvss_scores_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)   179218 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_package_versions_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_package_versions_destroy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19235 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_package_versions_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_package_versions_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_package_versions_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_promote_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_destroy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20673 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_reject_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_manifest_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_schema_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_status_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98680 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_healthy_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_whoami_retrieve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:36.008258 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osim/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_adjust_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osim/osim_healthy_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osim/osim_retrieve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:36.008258 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/trackers/trackers_api_v1_file_create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:36.012258 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/workflows/workflows_api_v1_adjust_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/workflows/workflows_api_v1_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/workflows/workflows_api_v1_retrieve_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/workflows/workflows_healthy_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/workflows/workflows_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:36.048259 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    18666 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22464 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/affect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/affect_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/affect_cvss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/affect_cvss_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/affect_cvss_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/affect_cvss_post_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/affect_cvss_put.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/affect_cvss_put_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/affect_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21734 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/affect_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/affect_post_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/affect_post_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/affect_report_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/affect_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/affectedness_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/auth_token_create_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/auth_token_refresh_create_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/auth_token_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/auth_token_verify_create_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/blank_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/collectors_healthy_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/collectors_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/comment_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/comment_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/cvss_version_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/epss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/erratum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploit_only_report_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploit_only_report_data_source_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_collect_update_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200_cves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_epss_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_flaw_data_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_data_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_action_required_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_no_action_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_not_relevant_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200_explanations_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200_pending_actions_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_status_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_supported_products_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49322 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_acknowledgment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_acknowledgment_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_acknowledgment_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_acknowledgment_post_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_acknowledgment_put.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_acknowledgment_put_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_classification_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_comment_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_comment_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_comment_post_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_comment_post_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_comment_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_cvss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_cvss_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_cvss_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_cvss_post_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_cvss_put.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_cvss_put_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_meta_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_package_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_package_version_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_package_version_put.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48617 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_post_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_post_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_post_classification_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9749 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_post_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_reference_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_reference_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_reference_post_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_reference_put.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_reference_put_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_reference_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_report_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_uuid_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/impact_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/issuer_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/major_incident_state_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/maturity_preliminary_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/meta_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/meta_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/module_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/nist_cvss_validation_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16637 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_create_response_201.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_create_response_201.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_destroy_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_list_issuer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7051 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_update_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_destroy_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_affectedness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_cvss_scores_issuer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_flaw_impact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_flaw_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_flaw_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_impact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_order_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_trackers_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16647 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16637 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_update_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_acknowledgments_create_response_201.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_acknowledgments_destroy_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_acknowledgments_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5973 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_acknowledgments_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_acknowledgments_update_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_create_response_201.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34111 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_create_response_201.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_cvss_scores_create_response_201.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_cvss_scores_destroy_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_cvss_scores_list_issuer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_cvss_scores_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_cvss_scores_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_cvss_scores_update_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_affectedness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_impact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_trackers_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_cvss_scores_issuer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_impact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_major_incident_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_nist_cvss_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_order_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_references_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_requires_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_workflow_state_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_package_versions_create_response_201.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_package_versions_destroy_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_package_versions_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_package_versions_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_package_versions_update_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_promote_create_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_create_response_201.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_destroy_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_list_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_update_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_reject_create_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34121 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34111 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_update_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_manifest_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_create_response_201.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_affectedness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_flaw_impact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_flaw_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_flaw_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_impact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_order_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8667 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_update_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_healthy_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_adjust_create_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_2_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osim_healthy_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osim_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/package_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/package_ver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_affect_cvss_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_affect_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_epss_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_exploit_only_report_data_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_flaw_acknowledgment_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_flaw_comment_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_flaw_cvss_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_flaw_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_flaw_package_version_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_flaw_reference_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_flaw_report_data_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_supported_products_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_tracker_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/ps_stream_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/reject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/requires_summary_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/resolution_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/source_8d8_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/supported_products.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/token_obtain_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/token_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/token_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11289 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/tracker_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/tracker_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/tracker_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/tracker_post_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/tracker_post_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/tracker_report_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/tracker_suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/tracker_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/workflows_api_v1_adjust_create_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/workflows_api_v1_retrieve_2_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/workflows_api_v1_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/workflows_healthy_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/workflows_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16998 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/osidb_bindings/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:36.052259 osidb_bindings-3.7.0/osidb_bindings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-23 12:12:35.000000 osidb_bindings-3.7.0/osidb_bindings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26937 2024-05-23 12:12:35.000000 osidb_bindings-3.7.0/osidb_bindings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 12:12:35.000000 osidb_bindings-3.7.0/osidb_bindings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-23 12:12:35.000000 osidb_bindings-3.7.0/osidb_bindings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 12:12:35.000000 osidb_bindings-3.7.0/osidb_bindings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 12:12:36.052259 osidb_bindings-3.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:36.052259 osidb_bindings-3.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-23 12:12:22.000000 osidb_bindings-3.7.0/tests/test_core.py
```

### Comparing `osidb-bindings-3.6.0/LICENSE` & `osidb_bindings-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/PKG-INFO` & `osidb_bindings-3.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osidb-bindings
-Version: 3.6.0
+Version: 3.7.0
 Summary: Python bindings for accessing OSIDB API
 Home-page: https://github.com/RedHatProductSecurity/osidb-bindings
 Author: Jakub Frejlach, Red Hat Product Security
 Author-email: jfrejlac@redhat.com
 Project-URL: Changelog, https://github.com/RedHatProductSecurity/osidb-bindings/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/RedHatProductSecurity/osidb-bindings/blob/master/TUTORIAL.md
 Project-URL: Source, https://github.com/RedHatProductSecurity/osidb-bindings
```

### Comparing `osidb-bindings-3.6.0/README.md` & `osidb_bindings-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/auth/auth_token_create.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/auth/auth_token_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/auth/auth_token_refresh_create.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/auth/auth_token_refresh_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/auth/auth_token_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/auth/auth_token_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/auth/auth_token_verify_create.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/auth/auth_token_verify_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/collectors/collectors_api_v1_status_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/collectors/collectors_api_v1_status_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/collectors/collectors_healthy_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/collectors/collectors_healthy_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/collectors/collectors_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/collectors/collectors_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_collect_update.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_collect_update.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_cve_map_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_cve_map_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_epss_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_epss_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_flaw_data_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_flaw_data_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_data_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_data_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_date_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_date_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_explanations_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_explanations_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_pending_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_pending_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_status_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_status_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_supported_products_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_supported_products_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/__init__.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/__init__.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_create.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_update.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 from typing import Any, Dict, Optional
 
 import requests
 
 from ...client import AuthenticatedClient
-from ...models.affect_post import AffectPost
-from ...models.osidb_api_v1_affects_create_response_201 import (
-    OsidbApiV1AffectsCreateResponse201,
+from ...models.affect import Affect
+from ...models.osidb_api_v1_affects_update_response_200 import (
+    OsidbApiV1AffectsUpdateResponse200,
 )
 from ...types import UNSET, Response, Unset
 
 QUERY_PARAMS = {}
-REQUEST_BODY_TYPE = AffectPost
+REQUEST_BODY_TYPE = Affect
 
 
 def _get_kwargs(
+    uuid: str,
     *,
     client: AuthenticatedClient,
-    form_data: AffectPost,
-    multipart_data: AffectPost,
-    json_body: AffectPost,
-    bugzilla_api_key: str,
+    form_data: Affect,
+    multipart_data: Affect,
+    json_body: Affect,
 ) -> Dict[str, Any]:
-    url = "{}/osidb/api/v1/affects".format(
+    url = "{}/osidb/api/v1/affects/{uuid}".format(
         client.base_url,
+        uuid=uuid,
     )
 
     headers: Dict[str, Any] = client.get_headers()
 
-    headers["bugzilla-api-key"] = bugzilla_api_key
-
     json_json_body: Dict[str, Any] = UNSET
     if not isinstance(json_body, Unset):
         json_body.to_dict()
 
     multipart_multipart_data: Dict[str, Any] = UNSET
     if not isinstance(multipart_data, Unset):
         multipart_data.to_multipart()
@@ -42,123 +41,123 @@
         "headers": headers,
         "data": form_data.to_dict(),
     }
 
 
 def _parse_response(
     *, response: requests.Response
-) -> Optional[OsidbApiV1AffectsCreateResponse201]:
-    if response.status_code == 201:
-        _response_201 = response.json()
-        response_201: OsidbApiV1AffectsCreateResponse201
-        if isinstance(_response_201, Unset):
-            response_201 = UNSET
+) -> Optional[OsidbApiV1AffectsUpdateResponse200]:
+    if response.status_code == 200:
+        _response_200 = response.json()
+        response_200: OsidbApiV1AffectsUpdateResponse200
+        if isinstance(_response_200, Unset):
+            response_200 = UNSET
         else:
-            response_201 = OsidbApiV1AffectsCreateResponse201.from_dict(_response_201)
+            response_200 = OsidbApiV1AffectsUpdateResponse200.from_dict(_response_200)
 
-        return response_201
+        return response_200
     return None
 
 
 def _build_response(
     *, response: requests.Response
-) -> Response[OsidbApiV1AffectsCreateResponse201]:
+) -> Response[OsidbApiV1AffectsUpdateResponse200]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
+    uuid: str,
     *,
     client: AuthenticatedClient,
-    form_data: AffectPost,
-    multipart_data: AffectPost,
-    json_body: AffectPost,
-    bugzilla_api_key: str,
-) -> Response[OsidbApiV1AffectsCreateResponse201]:
+    form_data: Affect,
+    multipart_data: Affect,
+    json_body: Affect,
+) -> Response[OsidbApiV1AffectsUpdateResponse200]:
     kwargs = _get_kwargs(
+        uuid=uuid,
         client=client,
         form_data=form_data,
         multipart_data=multipart_data,
         json_body=json_body,
-        bugzilla_api_key=bugzilla_api_key,
     )
 
-    response = requests.post(
+    response = requests.put(
         verify=client.verify_ssl,
         auth=client.auth,
         timeout=client.timeout,
         **kwargs,
     )
     response.raise_for_status()
 
     return _build_response(response=response)
 
 
 def sync(
+    uuid: str,
     *,
     client: AuthenticatedClient,
-    form_data: AffectPost,
-    multipart_data: AffectPost,
-    json_body: AffectPost,
-    bugzilla_api_key: str,
-) -> Optional[OsidbApiV1AffectsCreateResponse201]:
+    form_data: Affect,
+    multipart_data: Affect,
+    json_body: Affect,
+) -> Optional[OsidbApiV1AffectsUpdateResponse200]:
     """ """
 
     return sync_detailed(
+        uuid=uuid,
         client=client,
         form_data=form_data,
         multipart_data=multipart_data,
         json_body=json_body,
-        bugzilla_api_key=bugzilla_api_key,
     ).parsed
 
 
 async def async_detailed(
+    uuid: str,
     *,
     client: AuthenticatedClient,
-    form_data: AffectPost,
-    multipart_data: AffectPost,
-    json_body: AffectPost,
-    bugzilla_api_key: str,
-) -> Response[OsidbApiV1AffectsCreateResponse201]:
+    form_data: Affect,
+    multipart_data: Affect,
+    json_body: Affect,
+) -> Response[OsidbApiV1AffectsUpdateResponse200]:
     kwargs = _get_kwargs(
+        uuid=uuid,
         client=client,
         form_data=form_data,
         multipart_data=multipart_data,
         json_body=json_body,
-        bugzilla_api_key=bugzilla_api_key,
     )
 
-    async with client.get_async_session().post(
+    async with client.get_async_session().put(
         verify_ssl=client.verify_ssl, raise_for_status=True, **kwargs
     ) as response:
         content = await response.read()
         resp = requests.Response()
         resp.status_code = response.status
         resp._content = content
 
     return _build_response(response=resp)
 
 
 async def async_(
+    uuid: str,
     *,
     client: AuthenticatedClient,
-    form_data: AffectPost,
-    multipart_data: AffectPost,
-    json_body: AffectPost,
-    bugzilla_api_key: str,
-) -> Optional[OsidbApiV1AffectsCreateResponse201]:
+    form_data: Affect,
+    multipart_data: Affect,
+    json_body: Affect,
+) -> Optional[OsidbApiV1AffectsUpdateResponse200]:
     """ """
 
     return (
         await async_detailed(
+            uuid=uuid,
             client=client,
             form_data=form_data,
             multipart_data=multipart_data,
             json_body=json_body,
-            bugzilla_api_key=bugzilla_api_key,
         )
     ).parsed
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_cvss_scores_create.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_cvss_scores_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_cvss_scores_destroy.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_cvss_scores_destroy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, Optional
 
 import requests
 
 from ...client import AuthenticatedClient
-from ...models.osidb_api_v1_affects_cvss_scores_destroy_response_204 import (
-    OsidbApiV1AffectsCvssScoresDestroyResponse204,
+from ...models.osidb_api_v1_affects_cvss_scores_destroy_response_200 import (
+    OsidbApiV1AffectsCvssScoresDestroyResponse200,
 )
 from ...types import UNSET, Response, Unset
 
 QUERY_PARAMS = {}
 
 
 def _get_kwargs(
@@ -29,46 +29,46 @@
         "url": url,
         "headers": headers,
     }
 
 
 def _parse_response(
     *, response: requests.Response
-) -> Optional[OsidbApiV1AffectsCvssScoresDestroyResponse204]:
-    if response.status_code == 204:
-        _response_204 = response.json()
-        response_204: OsidbApiV1AffectsCvssScoresDestroyResponse204
-        if isinstance(_response_204, Unset):
-            response_204 = UNSET
+) -> Optional[OsidbApiV1AffectsCvssScoresDestroyResponse200]:
+    if response.status_code == 200:
+        _response_200 = response.json()
+        response_200: OsidbApiV1AffectsCvssScoresDestroyResponse200
+        if isinstance(_response_200, Unset):
+            response_200 = UNSET
         else:
-            response_204 = OsidbApiV1AffectsCvssScoresDestroyResponse204.from_dict(
-                _response_204
+            response_200 = OsidbApiV1AffectsCvssScoresDestroyResponse200.from_dict(
+                _response_200
             )
 
-        return response_204
+        return response_200
     return None
 
 
 def _build_response(
     *, response: requests.Response
-) -> Response[OsidbApiV1AffectsCvssScoresDestroyResponse204]:
+) -> Response[OsidbApiV1AffectsCvssScoresDestroyResponse200]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     affect_id: str,
     id: str,
     *,
     client: AuthenticatedClient,
-) -> Response[OsidbApiV1AffectsCvssScoresDestroyResponse204]:
+) -> Response[OsidbApiV1AffectsCvssScoresDestroyResponse200]:
     kwargs = _get_kwargs(
         affect_id=affect_id,
         id=id,
         client=client,
     )
 
     response = requests.delete(
@@ -83,30 +83,30 @@
 
 
 def sync(
     affect_id: str,
     id: str,
     *,
     client: AuthenticatedClient,
-) -> Optional[OsidbApiV1AffectsCvssScoresDestroyResponse204]:
+) -> Optional[OsidbApiV1AffectsCvssScoresDestroyResponse200]:
     """Destroy the instance and proxy the delete to Bugzilla."""
 
     return sync_detailed(
         affect_id=affect_id,
         id=id,
         client=client,
     ).parsed
 
 
 async def async_detailed(
     affect_id: str,
     id: str,
     *,
     client: AuthenticatedClient,
-) -> Response[OsidbApiV1AffectsCvssScoresDestroyResponse204]:
+) -> Response[OsidbApiV1AffectsCvssScoresDestroyResponse200]:
     kwargs = _get_kwargs(
         affect_id=affect_id,
         id=id,
         client=client,
     )
 
     async with client.get_async_session().delete(
@@ -121,15 +121,15 @@
 
 
 async def async_(
     affect_id: str,
     id: str,
     *,
     client: AuthenticatedClient,
-) -> Optional[OsidbApiV1AffectsCvssScoresDestroyResponse204]:
+) -> Optional[OsidbApiV1AffectsCvssScoresDestroyResponse200]:
     """Destroy the instance and proxy the delete to Bugzilla."""
 
     return (
         await async_detailed(
             affect_id=affect_id,
             id=id,
             client=client,
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_cvss_scores_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_cvss_scores_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_cvss_scores_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_cvss_scores_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_cvss_scores_update.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_cvss_scores_update.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_destroy.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_destroy.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,16 @@
     "cvss_scores__updated_dt__gte": datetime.datetime,
     "cvss_scores__updated_dt__lt": datetime.datetime,
     "cvss_scores__updated_dt__lte": datetime.datetime,
     "cvss_scores__uuid": str,
     "cvss_scores__vector": str,
     "embargoed": bool,
     "exclude_fields": List[str],
-    "flaw__component": str,
+    "flaw__component": List[str],
+    "flaw__components": List[str],
     "flaw__created_dt": datetime.datetime,
     "flaw__created_dt__date": datetime.date,
     "flaw__created_dt__date__gte": datetime.date,
     "flaw__created_dt__date__lte": datetime.date,
     "flaw__created_dt__gt": datetime.datetime,
     "flaw__created_dt__gte": datetime.datetime,
     "flaw__created_dt__lt": datetime.datetime,
@@ -218,15 +219,16 @@
     cvss_scores_updated_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     cvss_scores_updated_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
     cvss_scores_updated_dt_lte: Union[Unset, None, datetime.datetime] = UNSET,
     cvss_scores_uuid: Union[Unset, None, str] = UNSET,
     cvss_scores_vector: Union[Unset, None, str] = UNSET,
     embargoed: Union[Unset, None, bool] = UNSET,
     exclude_fields: Union[Unset, None, List[str]] = UNSET,
-    flaw_component: Union[Unset, None, str] = UNSET,
+    flaw_component: Union[Unset, None, List[str]] = UNSET,
+    flaw_components: Union[Unset, None, List[str]] = UNSET,
     flaw_created_dt: Union[Unset, None, datetime.datetime] = UNSET,
     flaw_created_dt_date: Union[Unset, None, datetime.date] = UNSET,
     flaw_created_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     flaw_created_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     flaw_created_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     flaw_created_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     flaw_created_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
@@ -492,14 +494,28 @@
     json_exclude_fields: Union[Unset, None, List[str]] = UNSET
     if not isinstance(exclude_fields, Unset):
         if exclude_fields is None:
             json_exclude_fields = None
         else:
             json_exclude_fields = exclude_fields
 
+    json_flaw_component: Union[Unset, None, List[str]] = UNSET
+    if not isinstance(flaw_component, Unset):
+        if flaw_component is None:
+            json_flaw_component = None
+        else:
+            json_flaw_component = flaw_component
+
+    json_flaw_components: Union[Unset, None, List[str]] = UNSET
+    if not isinstance(flaw_components, Unset):
+        if flaw_components is None:
+            json_flaw_components = None
+        else:
+            json_flaw_components = flaw_components
+
     json_flaw_created_dt: Union[Unset, None, str] = UNSET
     if not isinstance(flaw_created_dt, Unset):
         json_flaw_created_dt = flaw_created_dt.isoformat() if flaw_created_dt else None
 
     json_flaw_created_dt_date: Union[Unset, None, str] = UNSET
     if not isinstance(flaw_created_dt_date, Unset):
         json_flaw_created_dt_date = (
@@ -899,15 +915,16 @@
         "cvss_scores__updated_dt__gte": json_cvss_scores_updated_dt_gte,
         "cvss_scores__updated_dt__lt": json_cvss_scores_updated_dt_lt,
         "cvss_scores__updated_dt__lte": json_cvss_scores_updated_dt_lte,
         "cvss_scores__uuid": cvss_scores_uuid,
         "cvss_scores__vector": cvss_scores_vector,
         "embargoed": embargoed,
         "exclude_fields": json_exclude_fields,
-        "flaw__component": flaw_component,
+        "flaw__component": json_flaw_component,
+        "flaw__components": json_flaw_components,
         "flaw__created_dt": json_flaw_created_dt,
         "flaw__created_dt__date": json_flaw_created_dt_date,
         "flaw__created_dt__date__gte": json_flaw_created_dt_date_gte,
         "flaw__created_dt__date__lte": json_flaw_created_dt_date_lte,
         "flaw__created_dt__gt": json_flaw_created_dt_gt,
         "flaw__created_dt__gte": json_flaw_created_dt_gte,
         "flaw__created_dt__lt": json_flaw_created_dt_lt,
@@ -1075,15 +1092,16 @@
     cvss_scores_updated_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     cvss_scores_updated_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
     cvss_scores_updated_dt_lte: Union[Unset, None, datetime.datetime] = UNSET,
     cvss_scores_uuid: Union[Unset, None, str] = UNSET,
     cvss_scores_vector: Union[Unset, None, str] = UNSET,
     embargoed: Union[Unset, None, bool] = UNSET,
     exclude_fields: Union[Unset, None, List[str]] = UNSET,
-    flaw_component: Union[Unset, None, str] = UNSET,
+    flaw_component: Union[Unset, None, List[str]] = UNSET,
+    flaw_components: Union[Unset, None, List[str]] = UNSET,
     flaw_created_dt: Union[Unset, None, datetime.datetime] = UNSET,
     flaw_created_dt_date: Union[Unset, None, datetime.date] = UNSET,
     flaw_created_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     flaw_created_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     flaw_created_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     flaw_created_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     flaw_created_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
@@ -1214,14 +1232,15 @@
         cvss_scores_updated_dt_lt=cvss_scores_updated_dt_lt,
         cvss_scores_updated_dt_lte=cvss_scores_updated_dt_lte,
         cvss_scores_uuid=cvss_scores_uuid,
         cvss_scores_vector=cvss_scores_vector,
         embargoed=embargoed,
         exclude_fields=exclude_fields,
         flaw_component=flaw_component,
+        flaw_components=flaw_components,
         flaw_created_dt=flaw_created_dt,
         flaw_created_dt_date=flaw_created_dt_date,
         flaw_created_dt_date_gte=flaw_created_dt_date_gte,
         flaw_created_dt_date_lte=flaw_created_dt_date_lte,
         flaw_created_dt_gt=flaw_created_dt_gt,
         flaw_created_dt_gte=flaw_created_dt_gte,
         flaw_created_dt_lt=flaw_created_dt_lt,
@@ -1366,15 +1385,16 @@
     cvss_scores_updated_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     cvss_scores_updated_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
     cvss_scores_updated_dt_lte: Union[Unset, None, datetime.datetime] = UNSET,
     cvss_scores_uuid: Union[Unset, None, str] = UNSET,
     cvss_scores_vector: Union[Unset, None, str] = UNSET,
     embargoed: Union[Unset, None, bool] = UNSET,
     exclude_fields: Union[Unset, None, List[str]] = UNSET,
-    flaw_component: Union[Unset, None, str] = UNSET,
+    flaw_component: Union[Unset, None, List[str]] = UNSET,
+    flaw_components: Union[Unset, None, List[str]] = UNSET,
     flaw_created_dt: Union[Unset, None, datetime.datetime] = UNSET,
     flaw_created_dt_date: Union[Unset, None, datetime.date] = UNSET,
     flaw_created_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     flaw_created_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     flaw_created_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     flaw_created_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     flaw_created_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
@@ -1507,14 +1527,15 @@
         cvss_scores_updated_dt_lt=cvss_scores_updated_dt_lt,
         cvss_scores_updated_dt_lte=cvss_scores_updated_dt_lte,
         cvss_scores_uuid=cvss_scores_uuid,
         cvss_scores_vector=cvss_scores_vector,
         embargoed=embargoed,
         exclude_fields=exclude_fields,
         flaw_component=flaw_component,
+        flaw_components=flaw_components,
         flaw_created_dt=flaw_created_dt,
         flaw_created_dt_date=flaw_created_dt_date,
         flaw_created_dt_date_gte=flaw_created_dt_date_gte,
         flaw_created_dt_date_lte=flaw_created_dt_date_lte,
         flaw_created_dt_gt=flaw_created_dt_gt,
         flaw_created_dt_gte=flaw_created_dt_gte,
         flaw_created_dt_lt=flaw_created_dt_lt,
@@ -1649,15 +1670,16 @@
     cvss_scores_updated_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     cvss_scores_updated_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
     cvss_scores_updated_dt_lte: Union[Unset, None, datetime.datetime] = UNSET,
     cvss_scores_uuid: Union[Unset, None, str] = UNSET,
     cvss_scores_vector: Union[Unset, None, str] = UNSET,
     embargoed: Union[Unset, None, bool] = UNSET,
     exclude_fields: Union[Unset, None, List[str]] = UNSET,
-    flaw_component: Union[Unset, None, str] = UNSET,
+    flaw_component: Union[Unset, None, List[str]] = UNSET,
+    flaw_components: Union[Unset, None, List[str]] = UNSET,
     flaw_created_dt: Union[Unset, None, datetime.datetime] = UNSET,
     flaw_created_dt_date: Union[Unset, None, datetime.date] = UNSET,
     flaw_created_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     flaw_created_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     flaw_created_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     flaw_created_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     flaw_created_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
@@ -1788,14 +1810,15 @@
         cvss_scores_updated_dt_lt=cvss_scores_updated_dt_lt,
         cvss_scores_updated_dt_lte=cvss_scores_updated_dt_lte,
         cvss_scores_uuid=cvss_scores_uuid,
         cvss_scores_vector=cvss_scores_vector,
         embargoed=embargoed,
         exclude_fields=exclude_fields,
         flaw_component=flaw_component,
+        flaw_components=flaw_components,
         flaw_created_dt=flaw_created_dt,
         flaw_created_dt_date=flaw_created_dt_date,
         flaw_created_dt_date_gte=flaw_created_dt_date_gte,
         flaw_created_dt_date_lte=flaw_created_dt_date_lte,
         flaw_created_dt_gt=flaw_created_dt_gt,
         flaw_created_dt_gte=flaw_created_dt_gte,
         flaw_created_dt_lt=flaw_created_dt_lt,
@@ -1940,15 +1963,16 @@
     cvss_scores_updated_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     cvss_scores_updated_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
     cvss_scores_updated_dt_lte: Union[Unset, None, datetime.datetime] = UNSET,
     cvss_scores_uuid: Union[Unset, None, str] = UNSET,
     cvss_scores_vector: Union[Unset, None, str] = UNSET,
     embargoed: Union[Unset, None, bool] = UNSET,
     exclude_fields: Union[Unset, None, List[str]] = UNSET,
-    flaw_component: Union[Unset, None, str] = UNSET,
+    flaw_component: Union[Unset, None, List[str]] = UNSET,
+    flaw_components: Union[Unset, None, List[str]] = UNSET,
     flaw_created_dt: Union[Unset, None, datetime.datetime] = UNSET,
     flaw_created_dt_date: Union[Unset, None, datetime.date] = UNSET,
     flaw_created_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     flaw_created_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     flaw_created_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     flaw_created_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     flaw_created_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
@@ -2082,14 +2106,15 @@
             cvss_scores_updated_dt_lt=cvss_scores_updated_dt_lt,
             cvss_scores_updated_dt_lte=cvss_scores_updated_dt_lte,
             cvss_scores_uuid=cvss_scores_uuid,
             cvss_scores_vector=cvss_scores_vector,
             embargoed=embargoed,
             exclude_fields=exclude_fields,
             flaw_component=flaw_component,
+            flaw_components=flaw_components,
             flaw_created_dt=flaw_created_dt,
             flaw_created_dt_date=flaw_created_dt_date,
             flaw_created_dt_date_gte=flaw_created_dt_date_gte,
             flaw_created_dt_date_lte=flaw_created_dt_date_lte,
             flaw_created_dt_gt=flaw_created_dt_gt,
             flaw_created_dt_gte=flaw_created_dt_gte,
             flaw_created_dt_lt=flaw_created_dt_lt,
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_update.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_update.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 from typing import Any, Dict, Optional
 
 import requests
 
 from ...client import AuthenticatedClient
-from ...models.affect import Affect
-from ...models.osidb_api_v1_affects_update_response_200 import (
-    OsidbApiV1AffectsUpdateResponse200,
+from ...models.osidb_api_v1_trackers_update_response_200 import (
+    OsidbApiV1TrackersUpdateResponse200,
 )
+from ...models.tracker import Tracker
 from ...types import UNSET, Response, Unset
 
 QUERY_PARAMS = {}
-REQUEST_BODY_TYPE = Affect
+REQUEST_BODY_TYPE = Tracker
 
 
 def _get_kwargs(
     uuid: str,
     *,
     client: AuthenticatedClient,
-    form_data: Affect,
-    multipart_data: Affect,
-    json_body: Affect,
-    bugzilla_api_key: str,
+    form_data: Tracker,
+    multipart_data: Tracker,
+    json_body: Tracker,
 ) -> Dict[str, Any]:
-    url = "{}/osidb/api/v1/affects/{uuid}".format(
+    url = "{}/osidb/api/v1/trackers/{uuid}".format(
         client.base_url,
         uuid=uuid,
     )
 
     headers: Dict[str, Any] = client.get_headers()
 
-    headers["bugzilla-api-key"] = bugzilla_api_key
-
     json_json_body: Dict[str, Any] = UNSET
     if not isinstance(json_body, Unset):
         json_body.to_dict()
 
     multipart_multipart_data: Dict[str, Any] = UNSET
     if not isinstance(multipart_data, Unset):
         multipart_data.to_multipart()
@@ -44,54 +41,52 @@
         "headers": headers,
         "data": form_data.to_dict(),
     }
 
 
 def _parse_response(
     *, response: requests.Response
-) -> Optional[OsidbApiV1AffectsUpdateResponse200]:
+) -> Optional[OsidbApiV1TrackersUpdateResponse200]:
     if response.status_code == 200:
         _response_200 = response.json()
-        response_200: OsidbApiV1AffectsUpdateResponse200
+        response_200: OsidbApiV1TrackersUpdateResponse200
         if isinstance(_response_200, Unset):
             response_200 = UNSET
         else:
-            response_200 = OsidbApiV1AffectsUpdateResponse200.from_dict(_response_200)
+            response_200 = OsidbApiV1TrackersUpdateResponse200.from_dict(_response_200)
 
         return response_200
     return None
 
 
 def _build_response(
     *, response: requests.Response
-) -> Response[OsidbApiV1AffectsUpdateResponse200]:
+) -> Response[OsidbApiV1TrackersUpdateResponse200]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     uuid: str,
     *,
     client: AuthenticatedClient,
-    form_data: Affect,
-    multipart_data: Affect,
-    json_body: Affect,
-    bugzilla_api_key: str,
-) -> Response[OsidbApiV1AffectsUpdateResponse200]:
+    form_data: Tracker,
+    multipart_data: Tracker,
+    json_body: Tracker,
+) -> Response[OsidbApiV1TrackersUpdateResponse200]:
     kwargs = _get_kwargs(
         uuid=uuid,
         client=client,
         form_data=form_data,
         multipart_data=multipart_data,
         json_body=json_body,
-        bugzilla_api_key=bugzilla_api_key,
     )
 
     response = requests.put(
         verify=client.verify_ssl,
         auth=client.auth,
         timeout=client.timeout,
         **kwargs,
@@ -101,47 +96,43 @@
     return _build_response(response=response)
 
 
 def sync(
     uuid: str,
     *,
     client: AuthenticatedClient,
-    form_data: Affect,
-    multipart_data: Affect,
-    json_body: Affect,
-    bugzilla_api_key: str,
-) -> Optional[OsidbApiV1AffectsUpdateResponse200]:
+    form_data: Tracker,
+    multipart_data: Tracker,
+    json_body: Tracker,
+) -> Optional[OsidbApiV1TrackersUpdateResponse200]:
     """ """
 
     return sync_detailed(
         uuid=uuid,
         client=client,
         form_data=form_data,
         multipart_data=multipart_data,
         json_body=json_body,
-        bugzilla_api_key=bugzilla_api_key,
     ).parsed
 
 
 async def async_detailed(
     uuid: str,
     *,
     client: AuthenticatedClient,
-    form_data: Affect,
-    multipart_data: Affect,
-    json_body: Affect,
-    bugzilla_api_key: str,
-) -> Response[OsidbApiV1AffectsUpdateResponse200]:
+    form_data: Tracker,
+    multipart_data: Tracker,
+    json_body: Tracker,
+) -> Response[OsidbApiV1TrackersUpdateResponse200]:
     kwargs = _get_kwargs(
         uuid=uuid,
         client=client,
         form_data=form_data,
         multipart_data=multipart_data,
         json_body=json_body,
-        bugzilla_api_key=bugzilla_api_key,
     )
 
     async with client.get_async_session().put(
         verify_ssl=client.verify_ssl, raise_for_status=True, **kwargs
     ) as response:
         content = await response.read()
         resp = requests.Response()
@@ -151,24 +142,22 @@
     return _build_response(response=resp)
 
 
 async def async_(
     uuid: str,
     *,
     client: AuthenticatedClient,
-    form_data: Affect,
-    multipart_data: Affect,
-    json_body: Affect,
-    bugzilla_api_key: str,
-) -> Optional[OsidbApiV1AffectsUpdateResponse200]:
+    form_data: Tracker,
+    multipart_data: Tracker,
+    json_body: Tracker,
+) -> Optional[OsidbApiV1TrackersUpdateResponse200]:
     """ """
 
     return (
         await async_detailed(
             uuid=uuid,
             client=client,
             form_data=form_data,
             multipart_data=multipart_data,
             json_body=json_body,
-            bugzilla_api_key=bugzilla_api_key,
         )
     ).parsed
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_acknowledgments_create.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_acknowledgments_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_acknowledgments_destroy.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_acknowledgments_destroy.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_acknowledgments_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_acknowledgments_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_acknowledgments_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_acknowledgments_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_acknowledgments_update.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_acknowledgments_update.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_create.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_create.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_reject_create.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 from typing import Any, Dict, Optional
 
 import requests
 
 from ...client import AuthenticatedClient
-from ...models.flaw_post import FlawPost
-from ...models.osidb_api_v1_flaws_create_response_201 import (
-    OsidbApiV1FlawsCreateResponse201,
+from ...models.osidb_api_v1_flaws_reject_create_response_200 import (
+    OsidbApiV1FlawsRejectCreateResponse200,
 )
+from ...models.reject import Reject
 from ...types import UNSET, Response, Unset
 
 QUERY_PARAMS = {}
-REQUEST_BODY_TYPE = FlawPost
+REQUEST_BODY_TYPE = Reject
 
 
 def _get_kwargs(
+    flaw_id: str,
     *,
     client: AuthenticatedClient,
-    form_data: FlawPost,
-    multipart_data: FlawPost,
-    json_body: FlawPost,
-    bugzilla_api_key: str,
-    jira_api_key: str,
+    form_data: Reject,
+    multipart_data: Reject,
+    json_body: Reject,
 ) -> Dict[str, Any]:
-    url = "{}/osidb/api/v1/flaws".format(
+    url = "{}/osidb/api/v1/flaws/{flaw_id}/reject".format(
         client.base_url,
+        flaw_id=flaw_id,
     )
 
     headers: Dict[str, Any] = client.get_headers()
 
-    headers["bugzilla-api-key"] = bugzilla_api_key
-    headers["jira-api-key"] = jira_api_key
-
     json_json_body: Dict[str, Any] = UNSET
     if not isinstance(json_body, Unset):
         json_body.to_dict()
 
     multipart_multipart_data: Dict[str, Any] = UNSET
     if not isinstance(multipart_data, Unset):
         multipart_data.to_multipart()
@@ -44,131 +41,129 @@
         "headers": headers,
         "data": form_data.to_dict(),
     }
 
 
 def _parse_response(
     *, response: requests.Response
-) -> Optional[OsidbApiV1FlawsCreateResponse201]:
-    if response.status_code == 201:
-        _response_201 = response.json()
-        response_201: OsidbApiV1FlawsCreateResponse201
-        if isinstance(_response_201, Unset):
-            response_201 = UNSET
+) -> Optional[OsidbApiV1FlawsRejectCreateResponse200]:
+    if response.status_code == 200:
+        _response_200 = response.json()
+        response_200: OsidbApiV1FlawsRejectCreateResponse200
+        if isinstance(_response_200, Unset):
+            response_200 = UNSET
         else:
-            response_201 = OsidbApiV1FlawsCreateResponse201.from_dict(_response_201)
+            response_200 = OsidbApiV1FlawsRejectCreateResponse200.from_dict(
+                _response_200
+            )
 
-        return response_201
+        return response_200
     return None
 
 
 def _build_response(
     *, response: requests.Response
-) -> Response[OsidbApiV1FlawsCreateResponse201]:
+) -> Response[OsidbApiV1FlawsRejectCreateResponse200]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
+    flaw_id: str,
     *,
     client: AuthenticatedClient,
-    form_data: FlawPost,
-    multipart_data: FlawPost,
-    json_body: FlawPost,
-    bugzilla_api_key: str,
-    jira_api_key: str,
-) -> Response[OsidbApiV1FlawsCreateResponse201]:
+    form_data: Reject,
+    multipart_data: Reject,
+    json_body: Reject,
+) -> Response[OsidbApiV1FlawsRejectCreateResponse200]:
     kwargs = _get_kwargs(
+        flaw_id=flaw_id,
         client=client,
         form_data=form_data,
         multipart_data=multipart_data,
         json_body=json_body,
-        bugzilla_api_key=bugzilla_api_key,
-        jira_api_key=jira_api_key,
     )
 
     response = requests.post(
         verify=client.verify_ssl,
         auth=client.auth,
         timeout=client.timeout,
         **kwargs,
     )
     response.raise_for_status()
 
     return _build_response(response=response)
 
 
 def sync(
+    flaw_id: str,
     *,
     client: AuthenticatedClient,
-    form_data: FlawPost,
-    multipart_data: FlawPost,
-    json_body: FlawPost,
-    bugzilla_api_key: str,
-    jira_api_key: str,
-) -> Optional[OsidbApiV1FlawsCreateResponse201]:
-    """ """
+    form_data: Reject,
+    multipart_data: Reject,
+    json_body: Reject,
+) -> Optional[OsidbApiV1FlawsRejectCreateResponse200]:
+    """workflow promotion API endpoint
+
+    try to reject a flaw / task"""
 
     return sync_detailed(
+        flaw_id=flaw_id,
         client=client,
         form_data=form_data,
         multipart_data=multipart_data,
         json_body=json_body,
-        bugzilla_api_key=bugzilla_api_key,
-        jira_api_key=jira_api_key,
     ).parsed
 
 
 async def async_detailed(
+    flaw_id: str,
     *,
     client: AuthenticatedClient,
-    form_data: FlawPost,
-    multipart_data: FlawPost,
-    json_body: FlawPost,
-    bugzilla_api_key: str,
-    jira_api_key: str,
-) -> Response[OsidbApiV1FlawsCreateResponse201]:
+    form_data: Reject,
+    multipart_data: Reject,
+    json_body: Reject,
+) -> Response[OsidbApiV1FlawsRejectCreateResponse200]:
     kwargs = _get_kwargs(
+        flaw_id=flaw_id,
         client=client,
         form_data=form_data,
         multipart_data=multipart_data,
         json_body=json_body,
-        bugzilla_api_key=bugzilla_api_key,
-        jira_api_key=jira_api_key,
     )
 
     async with client.get_async_session().post(
         verify_ssl=client.verify_ssl, raise_for_status=True, **kwargs
     ) as response:
         content = await response.read()
         resp = requests.Response()
         resp.status_code = response.status
         resp._content = content
 
     return _build_response(response=resp)
 
 
 async def async_(
+    flaw_id: str,
     *,
     client: AuthenticatedClient,
-    form_data: FlawPost,
-    multipart_data: FlawPost,
-    json_body: FlawPost,
-    bugzilla_api_key: str,
-    jira_api_key: str,
-) -> Optional[OsidbApiV1FlawsCreateResponse201]:
-    """ """
+    form_data: Reject,
+    multipart_data: Reject,
+    json_body: Reject,
+) -> Optional[OsidbApiV1FlawsRejectCreateResponse200]:
+    """workflow promotion API endpoint
+
+    try to reject a flaw / task"""
 
     return (
         await async_detailed(
+            flaw_id=flaw_id,
             client=client,
             form_data=form_data,
             multipart_data=multipart_data,
             json_body=json_body,
-            bugzilla_api_key=bugzilla_api_key,
-            jira_api_key=jira_api_key,
         )
     ).parsed
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_cvss_scores_create.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_cvss_scores_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_cvss_scores_destroy.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_cvss_scores_destroy.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_cvss_scores_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_cvss_scores_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_cvss_scores_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_cvss_scores_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_cvss_scores_update.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_cvss_scores_update.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,17 @@
     OsidbApiV1FlawsListRequiresSummary,
 )
 from ...models.osidb_api_v1_flaws_list_response_200 import (
     OsidbApiV1FlawsListResponse200,
 )
 from ...models.osidb_api_v1_flaws_list_source import OsidbApiV1FlawsListSource
 from ...models.osidb_api_v1_flaws_list_type import OsidbApiV1FlawsListType
+from ...models.osidb_api_v1_flaws_list_workflow_state_item import (
+    OsidbApiV1FlawsListWorkflowStateItem,
+)
 from ...types import UNSET, Response, Unset
 
 QUERY_PARAMS = {
     "acknowledgments__affiliation": str,
     "acknowledgments__created_dt": datetime.datetime,
     "acknowledgments__created_dt__date": datetime.date,
     "acknowledgments__created_dt__date__gte": datetime.date,
@@ -132,15 +135,16 @@
     "affects__updated_dt__gte": datetime.datetime,
     "affects__updated_dt__lt": datetime.datetime,
     "affects__updated_dt__lte": datetime.datetime,
     "affects__uuid": str,
     "bz_id": float,
     "changed_after": datetime.datetime,
     "changed_before": datetime.datetime,
-    "component": str,
+    "component": List[str],
+    "components": List[str],
     "created_dt": datetime.datetime,
     "created_dt__date": datetime.date,
     "created_dt__date__gte": datetime.date,
     "created_dt__date__lte": datetime.date,
     "created_dt__gt": datetime.datetime,
     "created_dt__gte": datetime.datetime,
     "created_dt__lt": datetime.datetime,
@@ -192,14 +196,15 @@
     "limit": int,
     "major_incident_state": OsidbApiV1FlawsListMajorIncidentState,
     "nist_cvss_validation": OsidbApiV1FlawsListNistCvssValidation,
     "nvd_cvss2": str,
     "nvd_cvss3": str,
     "offset": int,
     "order": List[OsidbApiV1FlawsListOrderItem],
+    "owner": str,
     "references__created_dt": datetime.datetime,
     "references__created_dt__date": datetime.date,
     "references__created_dt__date__gte": datetime.date,
     "references__created_dt__date__lte": datetime.date,
     "references__created_dt__gt": datetime.datetime,
     "references__created_dt__gte": datetime.datetime,
     "references__created_dt__lt": datetime.datetime,
@@ -225,27 +230,29 @@
     "reported_dt__lt": datetime.datetime,
     "reported_dt__lte": datetime.datetime,
     "requires_summary": OsidbApiV1FlawsListRequiresSummary,
     "search": str,
     "source": OsidbApiV1FlawsListSource,
     "statement": str,
     "summary": str,
+    "team_id": str,
     "title": str,
     "tracker_ids": List[str],
     "type": OsidbApiV1FlawsListType,
     "unembargo_dt": datetime.datetime,
     "updated_dt": datetime.datetime,
     "updated_dt__date": datetime.date,
     "updated_dt__date__gte": datetime.date,
     "updated_dt__date__lte": datetime.date,
     "updated_dt__gt": datetime.datetime,
     "updated_dt__gte": datetime.datetime,
     "updated_dt__lt": datetime.datetime,
     "updated_dt__lte": datetime.datetime,
     "uuid": str,
+    "workflow_state": List[OsidbApiV1FlawsListWorkflowStateItem],
 }
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
     acknowledgments_affiliation: Union[Unset, None, str] = UNSET,
@@ -354,15 +361,16 @@
     affects_updated_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     affects_updated_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
     affects_updated_dt_lte: Union[Unset, None, datetime.datetime] = UNSET,
     affects_uuid: Union[Unset, None, str] = UNSET,
     bz_id: Union[Unset, None, float] = UNSET,
     changed_after: Union[Unset, None, datetime.datetime] = UNSET,
     changed_before: Union[Unset, None, datetime.datetime] = UNSET,
-    component: Union[Unset, None, str] = UNSET,
+    component: Union[Unset, None, List[str]] = UNSET,
+    components: Union[Unset, None, List[str]] = UNSET,
     created_dt: Union[Unset, None, datetime.datetime] = UNSET,
     created_dt_date: Union[Unset, None, datetime.date] = UNSET,
     created_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     created_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     created_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     created_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     created_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
@@ -418,14 +426,15 @@
     nist_cvss_validation: Union[
         Unset, None, OsidbApiV1FlawsListNistCvssValidation
     ] = UNSET,
     nvd_cvss2: Union[Unset, None, str] = UNSET,
     nvd_cvss3: Union[Unset, None, str] = UNSET,
     offset: Union[Unset, None, int] = UNSET,
     order: Union[Unset, None, List[OsidbApiV1FlawsListOrderItem]] = UNSET,
+    owner: Union[Unset, None, str] = UNSET,
     references_created_dt: Union[Unset, None, datetime.datetime] = UNSET,
     references_created_dt_date: Union[Unset, None, datetime.date] = UNSET,
     references_created_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     references_created_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     references_created_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     references_created_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     references_created_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
@@ -451,27 +460,31 @@
     reported_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
     reported_dt_lte: Union[Unset, None, datetime.datetime] = UNSET,
     requires_summary: Union[Unset, None, OsidbApiV1FlawsListRequiresSummary] = UNSET,
     search: Union[Unset, None, str] = UNSET,
     source: Union[Unset, None, OsidbApiV1FlawsListSource] = UNSET,
     statement: Union[Unset, None, str] = UNSET,
     summary: Union[Unset, None, str] = UNSET,
+    team_id: Union[Unset, None, str] = UNSET,
     title: Union[Unset, None, str] = UNSET,
     tracker_ids: Union[Unset, None, List[str]] = UNSET,
     type: Union[Unset, None, OsidbApiV1FlawsListType] = UNSET,
     unembargo_dt: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt_date: Union[Unset, None, datetime.date] = UNSET,
     updated_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     updated_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     updated_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt_lte: Union[Unset, None, datetime.datetime] = UNSET,
     uuid: Union[Unset, None, str] = UNSET,
+    workflow_state: Union[
+        Unset, None, List[OsidbApiV1FlawsListWorkflowStateItem]
+    ] = UNSET,
 ) -> Dict[str, Any]:
     url = "{}/osidb/api/v1/flaws".format(
         client.base_url,
     )
 
     headers: Dict[str, Any] = client.get_headers()
 
@@ -946,14 +959,28 @@
     if not isinstance(changed_after, Unset):
         json_changed_after = changed_after.isoformat() if changed_after else None
 
     json_changed_before: Union[Unset, None, str] = UNSET
     if not isinstance(changed_before, Unset):
         json_changed_before = changed_before.isoformat() if changed_before else None
 
+    json_component: Union[Unset, None, List[str]] = UNSET
+    if not isinstance(component, Unset):
+        if component is None:
+            json_component = None
+        else:
+            json_component = component
+
+    json_components: Union[Unset, None, List[str]] = UNSET
+    if not isinstance(components, Unset):
+        if components is None:
+            json_components = None
+        else:
+            json_components = components
+
     json_created_dt: Union[Unset, None, str] = UNSET
     if not isinstance(created_dt, Unset):
         json_created_dt = created_dt.isoformat() if created_dt else None
 
     json_created_dt_date: Union[Unset, None, str] = UNSET
     if not isinstance(created_dt_date, Unset):
         json_created_dt_date = created_dt_date.isoformat() if created_dt_date else None
@@ -1400,14 +1427,30 @@
     if not isinstance(updated_dt_lt, Unset):
         json_updated_dt_lt = updated_dt_lt.isoformat() if updated_dt_lt else None
 
     json_updated_dt_lte: Union[Unset, None, str] = UNSET
     if not isinstance(updated_dt_lte, Unset):
         json_updated_dt_lte = updated_dt_lte.isoformat() if updated_dt_lte else None
 
+    json_workflow_state: Union[Unset, None, List[str]] = UNSET
+    if not isinstance(workflow_state, Unset):
+        if workflow_state is None:
+            json_workflow_state = None
+        else:
+            json_workflow_state = []
+            for workflow_state_item_data in workflow_state:
+                workflow_state_item: str = UNSET
+                if not isinstance(workflow_state_item_data, Unset):
+
+                    workflow_state_item = OsidbApiV1FlawsListWorkflowStateItem(
+                        workflow_state_item_data
+                    ).value
+
+                json_workflow_state.append(workflow_state_item)
+
     params: Dict[str, Any] = {
         "acknowledgments__affiliation": acknowledgments_affiliation,
         "acknowledgments__created_dt": json_acknowledgments_created_dt,
         "acknowledgments__created_dt__date": json_acknowledgments_created_dt_date,
         "acknowledgments__created_dt__date__gte": json_acknowledgments_created_dt_date_gte,
         "acknowledgments__created_dt__date__lte": json_acknowledgments_created_dt_date_lte,
         "acknowledgments__created_dt__gt": json_acknowledgments_created_dt_gt,
@@ -1493,15 +1536,16 @@
         "affects__updated_dt__gte": json_affects_updated_dt_gte,
         "affects__updated_dt__lt": json_affects_updated_dt_lt,
         "affects__updated_dt__lte": json_affects_updated_dt_lte,
         "affects__uuid": affects_uuid,
         "bz_id": bz_id,
         "changed_after": json_changed_after,
         "changed_before": json_changed_before,
-        "component": component,
+        "component": json_component,
+        "components": json_components,
         "created_dt": json_created_dt,
         "created_dt__date": json_created_dt_date,
         "created_dt__date__gte": json_created_dt_date_gte,
         "created_dt__date__lte": json_created_dt_date_lte,
         "created_dt__gt": json_created_dt_gt,
         "created_dt__gte": json_created_dt_gte,
         "created_dt__lt": json_created_dt_lt,
@@ -1553,14 +1597,15 @@
         "limit": limit,
         "major_incident_state": json_major_incident_state,
         "nist_cvss_validation": json_nist_cvss_validation,
         "nvd_cvss2": nvd_cvss2,
         "nvd_cvss3": nvd_cvss3,
         "offset": offset,
         "order": json_order,
+        "owner": owner,
         "references__created_dt": json_references_created_dt,
         "references__created_dt__date": json_references_created_dt_date,
         "references__created_dt__date__gte": json_references_created_dt_date_gte,
         "references__created_dt__date__lte": json_references_created_dt_date_lte,
         "references__created_dt__gt": json_references_created_dt_gt,
         "references__created_dt__gte": json_references_created_dt_gte,
         "references__created_dt__lt": json_references_created_dt_lt,
@@ -1586,27 +1631,29 @@
         "reported_dt__lt": json_reported_dt_lt,
         "reported_dt__lte": json_reported_dt_lte,
         "requires_summary": json_requires_summary,
         "search": search,
         "source": json_source,
         "statement": statement,
         "summary": summary,
+        "team_id": team_id,
         "title": title,
         "tracker_ids": json_tracker_ids,
         "type": json_type,
         "unembargo_dt": json_unembargo_dt,
         "updated_dt": json_updated_dt,
         "updated_dt__date": json_updated_dt_date,
         "updated_dt__date__gte": json_updated_dt_date_gte,
         "updated_dt__date__lte": json_updated_dt_date_lte,
         "updated_dt__gt": json_updated_dt_gt,
         "updated_dt__gte": json_updated_dt_gte,
         "updated_dt__lt": json_updated_dt_lt,
         "updated_dt__lte": json_updated_dt_lte,
         "uuid": uuid,
+        "workflow_state": json_workflow_state,
     }
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "url": url,
         "headers": headers,
         "params": params,
@@ -1748,15 +1795,16 @@
     affects_updated_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     affects_updated_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
     affects_updated_dt_lte: Union[Unset, None, datetime.datetime] = UNSET,
     affects_uuid: Union[Unset, None, str] = UNSET,
     bz_id: Union[Unset, None, float] = UNSET,
     changed_after: Union[Unset, None, datetime.datetime] = UNSET,
     changed_before: Union[Unset, None, datetime.datetime] = UNSET,
-    component: Union[Unset, None, str] = UNSET,
+    component: Union[Unset, None, List[str]] = UNSET,
+    components: Union[Unset, None, List[str]] = UNSET,
     created_dt: Union[Unset, None, datetime.datetime] = UNSET,
     created_dt_date: Union[Unset, None, datetime.date] = UNSET,
     created_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     created_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     created_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     created_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     created_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
@@ -1812,14 +1860,15 @@
     nist_cvss_validation: Union[
         Unset, None, OsidbApiV1FlawsListNistCvssValidation
     ] = UNSET,
     nvd_cvss2: Union[Unset, None, str] = UNSET,
     nvd_cvss3: Union[Unset, None, str] = UNSET,
     offset: Union[Unset, None, int] = UNSET,
     order: Union[Unset, None, List[OsidbApiV1FlawsListOrderItem]] = UNSET,
+    owner: Union[Unset, None, str] = UNSET,
     references_created_dt: Union[Unset, None, datetime.datetime] = UNSET,
     references_created_dt_date: Union[Unset, None, datetime.date] = UNSET,
     references_created_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     references_created_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     references_created_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     references_created_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     references_created_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
@@ -1845,27 +1894,31 @@
     reported_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
     reported_dt_lte: Union[Unset, None, datetime.datetime] = UNSET,
     requires_summary: Union[Unset, None, OsidbApiV1FlawsListRequiresSummary] = UNSET,
     search: Union[Unset, None, str] = UNSET,
     source: Union[Unset, None, OsidbApiV1FlawsListSource] = UNSET,
     statement: Union[Unset, None, str] = UNSET,
     summary: Union[Unset, None, str] = UNSET,
+    team_id: Union[Unset, None, str] = UNSET,
     title: Union[Unset, None, str] = UNSET,
     tracker_ids: Union[Unset, None, List[str]] = UNSET,
     type: Union[Unset, None, OsidbApiV1FlawsListType] = UNSET,
     unembargo_dt: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt_date: Union[Unset, None, datetime.date] = UNSET,
     updated_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     updated_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     updated_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt_lte: Union[Unset, None, datetime.datetime] = UNSET,
     uuid: Union[Unset, None, str] = UNSET,
+    workflow_state: Union[
+        Unset, None, List[OsidbApiV1FlawsListWorkflowStateItem]
+    ] = UNSET,
 ) -> Response[OsidbApiV1FlawsListResponse200]:
     kwargs = _get_kwargs(
         client=client,
         acknowledgments_affiliation=acknowledgments_affiliation,
         acknowledgments_created_dt=acknowledgments_created_dt,
         acknowledgments_created_dt_date=acknowledgments_created_dt_date,
         acknowledgments_created_dt_date_gte=acknowledgments_created_dt_date_gte,
@@ -1954,14 +2007,15 @@
         affects_updated_dt_lt=affects_updated_dt_lt,
         affects_updated_dt_lte=affects_updated_dt_lte,
         affects_uuid=affects_uuid,
         bz_id=bz_id,
         changed_after=changed_after,
         changed_before=changed_before,
         component=component,
+        components=components,
         created_dt=created_dt,
         created_dt_date=created_dt_date,
         created_dt_date_gte=created_dt_date_gte,
         created_dt_date_lte=created_dt_date_lte,
         created_dt_gt=created_dt_gt,
         created_dt_gte=created_dt_gte,
         created_dt_lt=created_dt_lt,
@@ -2013,14 +2067,15 @@
         limit=limit,
         major_incident_state=major_incident_state,
         nist_cvss_validation=nist_cvss_validation,
         nvd_cvss2=nvd_cvss2,
         nvd_cvss3=nvd_cvss3,
         offset=offset,
         order=order,
+        owner=owner,
         references_created_dt=references_created_dt,
         references_created_dt_date=references_created_dt_date,
         references_created_dt_date_gte=references_created_dt_date_gte,
         references_created_dt_date_lte=references_created_dt_date_lte,
         references_created_dt_gt=references_created_dt_gt,
         references_created_dt_gte=references_created_dt_gte,
         references_created_dt_lt=references_created_dt_lt,
@@ -2046,27 +2101,29 @@
         reported_dt_lt=reported_dt_lt,
         reported_dt_lte=reported_dt_lte,
         requires_summary=requires_summary,
         search=search,
         source=source,
         statement=statement,
         summary=summary,
+        team_id=team_id,
         title=title,
         tracker_ids=tracker_ids,
         type=type,
         unembargo_dt=unembargo_dt,
         updated_dt=updated_dt,
         updated_dt_date=updated_dt_date,
         updated_dt_date_gte=updated_dt_date_gte,
         updated_dt_date_lte=updated_dt_date_lte,
         updated_dt_gt=updated_dt_gt,
         updated_dt_gte=updated_dt_gte,
         updated_dt_lt=updated_dt_lt,
         updated_dt_lte=updated_dt_lte,
         uuid=uuid,
+        workflow_state=workflow_state,
     )
 
     response = requests.get(
         verify=client.verify_ssl,
         auth=client.auth,
         timeout=client.timeout,
         **kwargs,
@@ -2185,15 +2242,16 @@
     affects_updated_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     affects_updated_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
     affects_updated_dt_lte: Union[Unset, None, datetime.datetime] = UNSET,
     affects_uuid: Union[Unset, None, str] = UNSET,
     bz_id: Union[Unset, None, float] = UNSET,
     changed_after: Union[Unset, None, datetime.datetime] = UNSET,
     changed_before: Union[Unset, None, datetime.datetime] = UNSET,
-    component: Union[Unset, None, str] = UNSET,
+    component: Union[Unset, None, List[str]] = UNSET,
+    components: Union[Unset, None, List[str]] = UNSET,
     created_dt: Union[Unset, None, datetime.datetime] = UNSET,
     created_dt_date: Union[Unset, None, datetime.date] = UNSET,
     created_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     created_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     created_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     created_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     created_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
@@ -2249,14 +2307,15 @@
     nist_cvss_validation: Union[
         Unset, None, OsidbApiV1FlawsListNistCvssValidation
     ] = UNSET,
     nvd_cvss2: Union[Unset, None, str] = UNSET,
     nvd_cvss3: Union[Unset, None, str] = UNSET,
     offset: Union[Unset, None, int] = UNSET,
     order: Union[Unset, None, List[OsidbApiV1FlawsListOrderItem]] = UNSET,
+    owner: Union[Unset, None, str] = UNSET,
     references_created_dt: Union[Unset, None, datetime.datetime] = UNSET,
     references_created_dt_date: Union[Unset, None, datetime.date] = UNSET,
     references_created_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     references_created_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     references_created_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     references_created_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     references_created_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
@@ -2282,27 +2341,31 @@
     reported_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
     reported_dt_lte: Union[Unset, None, datetime.datetime] = UNSET,
     requires_summary: Union[Unset, None, OsidbApiV1FlawsListRequiresSummary] = UNSET,
     search: Union[Unset, None, str] = UNSET,
     source: Union[Unset, None, OsidbApiV1FlawsListSource] = UNSET,
     statement: Union[Unset, None, str] = UNSET,
     summary: Union[Unset, None, str] = UNSET,
+    team_id: Union[Unset, None, str] = UNSET,
     title: Union[Unset, None, str] = UNSET,
     tracker_ids: Union[Unset, None, List[str]] = UNSET,
     type: Union[Unset, None, OsidbApiV1FlawsListType] = UNSET,
     unembargo_dt: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt_date: Union[Unset, None, datetime.date] = UNSET,
     updated_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     updated_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     updated_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt_lte: Union[Unset, None, datetime.datetime] = UNSET,
     uuid: Union[Unset, None, str] = UNSET,
+    workflow_state: Union[
+        Unset, None, List[OsidbApiV1FlawsListWorkflowStateItem]
+    ] = UNSET,
 ) -> Optional[OsidbApiV1FlawsListResponse200]:
     """ """
 
     return sync_detailed(
         client=client,
         acknowledgments_affiliation=acknowledgments_affiliation,
         acknowledgments_created_dt=acknowledgments_created_dt,
@@ -2393,14 +2456,15 @@
         affects_updated_dt_lt=affects_updated_dt_lt,
         affects_updated_dt_lte=affects_updated_dt_lte,
         affects_uuid=affects_uuid,
         bz_id=bz_id,
         changed_after=changed_after,
         changed_before=changed_before,
         component=component,
+        components=components,
         created_dt=created_dt,
         created_dt_date=created_dt_date,
         created_dt_date_gte=created_dt_date_gte,
         created_dt_date_lte=created_dt_date_lte,
         created_dt_gt=created_dt_gt,
         created_dt_gte=created_dt_gte,
         created_dt_lt=created_dt_lt,
@@ -2452,14 +2516,15 @@
         limit=limit,
         major_incident_state=major_incident_state,
         nist_cvss_validation=nist_cvss_validation,
         nvd_cvss2=nvd_cvss2,
         nvd_cvss3=nvd_cvss3,
         offset=offset,
         order=order,
+        owner=owner,
         references_created_dt=references_created_dt,
         references_created_dt_date=references_created_dt_date,
         references_created_dt_date_gte=references_created_dt_date_gte,
         references_created_dt_date_lte=references_created_dt_date_lte,
         references_created_dt_gt=references_created_dt_gt,
         references_created_dt_gte=references_created_dt_gte,
         references_created_dt_lt=references_created_dt_lt,
@@ -2485,27 +2550,29 @@
         reported_dt_lt=reported_dt_lt,
         reported_dt_lte=reported_dt_lte,
         requires_summary=requires_summary,
         search=search,
         source=source,
         statement=statement,
         summary=summary,
+        team_id=team_id,
         title=title,
         tracker_ids=tracker_ids,
         type=type,
         unembargo_dt=unembargo_dt,
         updated_dt=updated_dt,
         updated_dt_date=updated_dt_date,
         updated_dt_date_gte=updated_dt_date_gte,
         updated_dt_date_lte=updated_dt_date_lte,
         updated_dt_gt=updated_dt_gt,
         updated_dt_gte=updated_dt_gte,
         updated_dt_lt=updated_dt_lt,
         updated_dt_lte=updated_dt_lte,
         uuid=uuid,
+        workflow_state=workflow_state,
     ).parsed
 
 
 async def async_detailed(
     *,
     client: AuthenticatedClient,
     acknowledgments_affiliation: Union[Unset, None, str] = UNSET,
@@ -2614,15 +2681,16 @@
     affects_updated_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     affects_updated_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
     affects_updated_dt_lte: Union[Unset, None, datetime.datetime] = UNSET,
     affects_uuid: Union[Unset, None, str] = UNSET,
     bz_id: Union[Unset, None, float] = UNSET,
     changed_after: Union[Unset, None, datetime.datetime] = UNSET,
     changed_before: Union[Unset, None, datetime.datetime] = UNSET,
-    component: Union[Unset, None, str] = UNSET,
+    component: Union[Unset, None, List[str]] = UNSET,
+    components: Union[Unset, None, List[str]] = UNSET,
     created_dt: Union[Unset, None, datetime.datetime] = UNSET,
     created_dt_date: Union[Unset, None, datetime.date] = UNSET,
     created_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     created_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     created_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     created_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     created_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
@@ -2678,14 +2746,15 @@
     nist_cvss_validation: Union[
         Unset, None, OsidbApiV1FlawsListNistCvssValidation
     ] = UNSET,
     nvd_cvss2: Union[Unset, None, str] = UNSET,
     nvd_cvss3: Union[Unset, None, str] = UNSET,
     offset: Union[Unset, None, int] = UNSET,
     order: Union[Unset, None, List[OsidbApiV1FlawsListOrderItem]] = UNSET,
+    owner: Union[Unset, None, str] = UNSET,
     references_created_dt: Union[Unset, None, datetime.datetime] = UNSET,
     references_created_dt_date: Union[Unset, None, datetime.date] = UNSET,
     references_created_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     references_created_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     references_created_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     references_created_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     references_created_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
@@ -2711,27 +2780,31 @@
     reported_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
     reported_dt_lte: Union[Unset, None, datetime.datetime] = UNSET,
     requires_summary: Union[Unset, None, OsidbApiV1FlawsListRequiresSummary] = UNSET,
     search: Union[Unset, None, str] = UNSET,
     source: Union[Unset, None, OsidbApiV1FlawsListSource] = UNSET,
     statement: Union[Unset, None, str] = UNSET,
     summary: Union[Unset, None, str] = UNSET,
+    team_id: Union[Unset, None, str] = UNSET,
     title: Union[Unset, None, str] = UNSET,
     tracker_ids: Union[Unset, None, List[str]] = UNSET,
     type: Union[Unset, None, OsidbApiV1FlawsListType] = UNSET,
     unembargo_dt: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt_date: Union[Unset, None, datetime.date] = UNSET,
     updated_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     updated_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     updated_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt_lte: Union[Unset, None, datetime.datetime] = UNSET,
     uuid: Union[Unset, None, str] = UNSET,
+    workflow_state: Union[
+        Unset, None, List[OsidbApiV1FlawsListWorkflowStateItem]
+    ] = UNSET,
 ) -> Response[OsidbApiV1FlawsListResponse200]:
     kwargs = _get_kwargs(
         client=client,
         acknowledgments_affiliation=acknowledgments_affiliation,
         acknowledgments_created_dt=acknowledgments_created_dt,
         acknowledgments_created_dt_date=acknowledgments_created_dt_date,
         acknowledgments_created_dt_date_gte=acknowledgments_created_dt_date_gte,
@@ -2820,14 +2893,15 @@
         affects_updated_dt_lt=affects_updated_dt_lt,
         affects_updated_dt_lte=affects_updated_dt_lte,
         affects_uuid=affects_uuid,
         bz_id=bz_id,
         changed_after=changed_after,
         changed_before=changed_before,
         component=component,
+        components=components,
         created_dt=created_dt,
         created_dt_date=created_dt_date,
         created_dt_date_gte=created_dt_date_gte,
         created_dt_date_lte=created_dt_date_lte,
         created_dt_gt=created_dt_gt,
         created_dt_gte=created_dt_gte,
         created_dt_lt=created_dt_lt,
@@ -2879,14 +2953,15 @@
         limit=limit,
         major_incident_state=major_incident_state,
         nist_cvss_validation=nist_cvss_validation,
         nvd_cvss2=nvd_cvss2,
         nvd_cvss3=nvd_cvss3,
         offset=offset,
         order=order,
+        owner=owner,
         references_created_dt=references_created_dt,
         references_created_dt_date=references_created_dt_date,
         references_created_dt_date_gte=references_created_dt_date_gte,
         references_created_dt_date_lte=references_created_dt_date_lte,
         references_created_dt_gt=references_created_dt_gt,
         references_created_dt_gte=references_created_dt_gte,
         references_created_dt_lt=references_created_dt_lt,
@@ -2912,27 +2987,29 @@
         reported_dt_lt=reported_dt_lt,
         reported_dt_lte=reported_dt_lte,
         requires_summary=requires_summary,
         search=search,
         source=source,
         statement=statement,
         summary=summary,
+        team_id=team_id,
         title=title,
         tracker_ids=tracker_ids,
         type=type,
         unembargo_dt=unembargo_dt,
         updated_dt=updated_dt,
         updated_dt_date=updated_dt_date,
         updated_dt_date_gte=updated_dt_date_gte,
         updated_dt_date_lte=updated_dt_date_lte,
         updated_dt_gt=updated_dt_gt,
         updated_dt_gte=updated_dt_gte,
         updated_dt_lt=updated_dt_lt,
         updated_dt_lte=updated_dt_lte,
         uuid=uuid,
+        workflow_state=workflow_state,
     )
 
     async with client.get_async_session().get(
         verify_ssl=client.verify_ssl, raise_for_status=True, **kwargs
     ) as response:
         content = await response.read()
         resp = requests.Response()
@@ -3051,15 +3128,16 @@
     affects_updated_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     affects_updated_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
     affects_updated_dt_lte: Union[Unset, None, datetime.datetime] = UNSET,
     affects_uuid: Union[Unset, None, str] = UNSET,
     bz_id: Union[Unset, None, float] = UNSET,
     changed_after: Union[Unset, None, datetime.datetime] = UNSET,
     changed_before: Union[Unset, None, datetime.datetime] = UNSET,
-    component: Union[Unset, None, str] = UNSET,
+    component: Union[Unset, None, List[str]] = UNSET,
+    components: Union[Unset, None, List[str]] = UNSET,
     created_dt: Union[Unset, None, datetime.datetime] = UNSET,
     created_dt_date: Union[Unset, None, datetime.date] = UNSET,
     created_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     created_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     created_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     created_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     created_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
@@ -3115,14 +3193,15 @@
     nist_cvss_validation: Union[
         Unset, None, OsidbApiV1FlawsListNistCvssValidation
     ] = UNSET,
     nvd_cvss2: Union[Unset, None, str] = UNSET,
     nvd_cvss3: Union[Unset, None, str] = UNSET,
     offset: Union[Unset, None, int] = UNSET,
     order: Union[Unset, None, List[OsidbApiV1FlawsListOrderItem]] = UNSET,
+    owner: Union[Unset, None, str] = UNSET,
     references_created_dt: Union[Unset, None, datetime.datetime] = UNSET,
     references_created_dt_date: Union[Unset, None, datetime.date] = UNSET,
     references_created_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     references_created_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     references_created_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     references_created_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     references_created_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
@@ -3148,27 +3227,31 @@
     reported_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
     reported_dt_lte: Union[Unset, None, datetime.datetime] = UNSET,
     requires_summary: Union[Unset, None, OsidbApiV1FlawsListRequiresSummary] = UNSET,
     search: Union[Unset, None, str] = UNSET,
     source: Union[Unset, None, OsidbApiV1FlawsListSource] = UNSET,
     statement: Union[Unset, None, str] = UNSET,
     summary: Union[Unset, None, str] = UNSET,
+    team_id: Union[Unset, None, str] = UNSET,
     title: Union[Unset, None, str] = UNSET,
     tracker_ids: Union[Unset, None, List[str]] = UNSET,
     type: Union[Unset, None, OsidbApiV1FlawsListType] = UNSET,
     unembargo_dt: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt_date: Union[Unset, None, datetime.date] = UNSET,
     updated_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     updated_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     updated_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
     updated_dt_lte: Union[Unset, None, datetime.datetime] = UNSET,
     uuid: Union[Unset, None, str] = UNSET,
+    workflow_state: Union[
+        Unset, None, List[OsidbApiV1FlawsListWorkflowStateItem]
+    ] = UNSET,
 ) -> Optional[OsidbApiV1FlawsListResponse200]:
     """ """
 
     return (
         await async_detailed(
             client=client,
             acknowledgments_affiliation=acknowledgments_affiliation,
@@ -3260,14 +3343,15 @@
             affects_updated_dt_lt=affects_updated_dt_lt,
             affects_updated_dt_lte=affects_updated_dt_lte,
             affects_uuid=affects_uuid,
             bz_id=bz_id,
             changed_after=changed_after,
             changed_before=changed_before,
             component=component,
+            components=components,
             created_dt=created_dt,
             created_dt_date=created_dt_date,
             created_dt_date_gte=created_dt_date_gte,
             created_dt_date_lte=created_dt_date_lte,
             created_dt_gt=created_dt_gt,
             created_dt_gte=created_dt_gte,
             created_dt_lt=created_dt_lt,
@@ -3319,14 +3403,15 @@
             limit=limit,
             major_incident_state=major_incident_state,
             nist_cvss_validation=nist_cvss_validation,
             nvd_cvss2=nvd_cvss2,
             nvd_cvss3=nvd_cvss3,
             offset=offset,
             order=order,
+            owner=owner,
             references_created_dt=references_created_dt,
             references_created_dt_date=references_created_dt_date,
             references_created_dt_date_gte=references_created_dt_date_gte,
             references_created_dt_date_lte=references_created_dt_date_lte,
             references_created_dt_gt=references_created_dt_gt,
             references_created_dt_gte=references_created_dt_gte,
             references_created_dt_lt=references_created_dt_lt,
@@ -3352,22 +3437,24 @@
             reported_dt_lt=reported_dt_lt,
             reported_dt_lte=reported_dt_lte,
             requires_summary=requires_summary,
             search=search,
             source=source,
             statement=statement,
             summary=summary,
+            team_id=team_id,
             title=title,
             tracker_ids=tracker_ids,
             type=type,
             unembargo_dt=unembargo_dt,
             updated_dt=updated_dt,
             updated_dt_date=updated_dt_date,
             updated_dt_date_gte=updated_dt_date_gte,
             updated_dt_date_lte=updated_dt_date_lte,
             updated_dt_gt=updated_dt_gt,
             updated_dt_gte=updated_dt_gte,
             updated_dt_lt=updated_dt_lt,
             updated_dt_lte=updated_dt_lte,
             uuid=uuid,
+            workflow_state=workflow_state,
         )
     ).parsed
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_package_versions_create.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_package_versions_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_package_versions_destroy.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_package_versions_destroy.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_package_versions_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_package_versions_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_package_versions_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_package_versions_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_package_versions_update.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_package_versions_update.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_promote_create.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_promote_create.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,25 +11,22 @@
 QUERY_PARAMS = {}
 
 
 def _get_kwargs(
     flaw_id: str,
     *,
     client: AuthenticatedClient,
-    jira_api_key: str,
 ) -> Dict[str, Any]:
     url = "{}/osidb/api/v1/flaws/{flaw_id}/promote".format(
         client.base_url,
         flaw_id=flaw_id,
     )
 
     headers: Dict[str, Any] = client.get_headers()
 
-    headers["jira-api-key"] = jira_api_key
-
     return {
         "url": url,
         "headers": headers,
     }
 
 
 def _parse_response(
@@ -60,20 +57,18 @@
     )
 
 
 def sync_detailed(
     flaw_id: str,
     *,
     client: AuthenticatedClient,
-    jira_api_key: str,
 ) -> Response[OsidbApiV1FlawsPromoteCreateResponse200]:
     kwargs = _get_kwargs(
         flaw_id=flaw_id,
         client=client,
-        jira_api_key=jira_api_key,
     )
 
     response = requests.post(
         verify=client.verify_ssl,
         auth=client.auth,
         timeout=client.timeout,
         **kwargs,
@@ -83,38 +78,34 @@
     return _build_response(response=response)
 
 
 def sync(
     flaw_id: str,
     *,
     client: AuthenticatedClient,
-    jira_api_key: str,
 ) -> Optional[OsidbApiV1FlawsPromoteCreateResponse200]:
     """workflow promotion API endpoint
 
     try to adjust workflow classification of flaw to the next state available
     return its workflow:state classification or errors if not possible to promote"""
 
     return sync_detailed(
         flaw_id=flaw_id,
         client=client,
-        jira_api_key=jira_api_key,
     ).parsed
 
 
 async def async_detailed(
     flaw_id: str,
     *,
     client: AuthenticatedClient,
-    jira_api_key: str,
 ) -> Response[OsidbApiV1FlawsPromoteCreateResponse200]:
     kwargs = _get_kwargs(
         flaw_id=flaw_id,
         client=client,
-        jira_api_key=jira_api_key,
     )
 
     async with client.get_async_session().post(
         verify_ssl=client.verify_ssl, raise_for_status=True, **kwargs
     ) as response:
         content = await response.read()
         resp = requests.Response()
@@ -124,21 +115,19 @@
     return _build_response(response=resp)
 
 
 async def async_(
     flaw_id: str,
     *,
     client: AuthenticatedClient,
-    jira_api_key: str,
 ) -> Optional[OsidbApiV1FlawsPromoteCreateResponse200]:
     """workflow promotion API endpoint
 
     try to adjust workflow classification of flaw to the next state available
     return its workflow:state classification or errors if not possible to promote"""
 
     return (
         await async_detailed(
             flaw_id=flaw_id,
             client=client,
-            jira_api_key=jira_api_key,
         )
     ).parsed
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_create.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_destroy.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_destroy.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_update.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_update.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_reject_create.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_create.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 from typing import Any, Dict, Optional
 
 import requests
 
 from ...client import AuthenticatedClient
-from ...models.osidb_api_v1_flaws_reject_create_response_200 import (
-    OsidbApiV1FlawsRejectCreateResponse200,
+from ...models.flaw_post import FlawPost
+from ...models.osidb_api_v1_flaws_create_response_201 import (
+    OsidbApiV1FlawsCreateResponse201,
 )
-from ...models.reject import Reject
 from ...types import UNSET, Response, Unset
 
 QUERY_PARAMS = {}
-REQUEST_BODY_TYPE = Reject
+REQUEST_BODY_TYPE = FlawPost
 
 
 def _get_kwargs(
-    flaw_id: str,
     *,
     client: AuthenticatedClient,
-    form_data: Reject,
-    multipart_data: Reject,
-    json_body: Reject,
-    jira_api_key: str,
+    form_data: FlawPost,
+    multipart_data: FlawPost,
+    json_body: FlawPost,
 ) -> Dict[str, Any]:
-    url = "{}/osidb/api/v1/flaws/{flaw_id}/reject".format(
+    url = "{}/osidb/api/v1/flaws".format(
         client.base_url,
-        flaw_id=flaw_id,
     )
 
     headers: Dict[str, Any] = client.get_headers()
 
-    headers["jira-api-key"] = jira_api_key
-
     json_json_body: Dict[str, Any] = UNSET
     if not isinstance(json_body, Unset):
         json_body.to_dict()
 
     multipart_multipart_data: Dict[str, Any] = UNSET
     if not isinstance(multipart_data, Unset):
         multipart_data.to_multipart()
@@ -44,137 +39,115 @@
         "headers": headers,
         "data": form_data.to_dict(),
     }
 
 
 def _parse_response(
     *, response: requests.Response
-) -> Optional[OsidbApiV1FlawsRejectCreateResponse200]:
-    if response.status_code == 200:
-        _response_200 = response.json()
-        response_200: OsidbApiV1FlawsRejectCreateResponse200
-        if isinstance(_response_200, Unset):
-            response_200 = UNSET
+) -> Optional[OsidbApiV1FlawsCreateResponse201]:
+    if response.status_code == 201:
+        _response_201 = response.json()
+        response_201: OsidbApiV1FlawsCreateResponse201
+        if isinstance(_response_201, Unset):
+            response_201 = UNSET
         else:
-            response_200 = OsidbApiV1FlawsRejectCreateResponse200.from_dict(
-                _response_200
-            )
+            response_201 = OsidbApiV1FlawsCreateResponse201.from_dict(_response_201)
 
-        return response_200
+        return response_201
     return None
 
 
 def _build_response(
     *, response: requests.Response
-) -> Response[OsidbApiV1FlawsRejectCreateResponse200]:
+) -> Response[OsidbApiV1FlawsCreateResponse201]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    flaw_id: str,
     *,
     client: AuthenticatedClient,
-    form_data: Reject,
-    multipart_data: Reject,
-    json_body: Reject,
-    jira_api_key: str,
-) -> Response[OsidbApiV1FlawsRejectCreateResponse200]:
+    form_data: FlawPost,
+    multipart_data: FlawPost,
+    json_body: FlawPost,
+) -> Response[OsidbApiV1FlawsCreateResponse201]:
     kwargs = _get_kwargs(
-        flaw_id=flaw_id,
         client=client,
         form_data=form_data,
         multipart_data=multipart_data,
         json_body=json_body,
-        jira_api_key=jira_api_key,
     )
 
     response = requests.post(
         verify=client.verify_ssl,
         auth=client.auth,
         timeout=client.timeout,
         **kwargs,
     )
     response.raise_for_status()
 
     return _build_response(response=response)
 
 
 def sync(
-    flaw_id: str,
     *,
     client: AuthenticatedClient,
-    form_data: Reject,
-    multipart_data: Reject,
-    json_body: Reject,
-    jira_api_key: str,
-) -> Optional[OsidbApiV1FlawsRejectCreateResponse200]:
-    """workflow promotion API endpoint
-
-    try to reject a flaw / task"""
+    form_data: FlawPost,
+    multipart_data: FlawPost,
+    json_body: FlawPost,
+) -> Optional[OsidbApiV1FlawsCreateResponse201]:
+    """ """
 
     return sync_detailed(
-        flaw_id=flaw_id,
         client=client,
         form_data=form_data,
         multipart_data=multipart_data,
         json_body=json_body,
-        jira_api_key=jira_api_key,
     ).parsed
 
 
 async def async_detailed(
-    flaw_id: str,
     *,
     client: AuthenticatedClient,
-    form_data: Reject,
-    multipart_data: Reject,
-    json_body: Reject,
-    jira_api_key: str,
-) -> Response[OsidbApiV1FlawsRejectCreateResponse200]:
+    form_data: FlawPost,
+    multipart_data: FlawPost,
+    json_body: FlawPost,
+) -> Response[OsidbApiV1FlawsCreateResponse201]:
     kwargs = _get_kwargs(
-        flaw_id=flaw_id,
         client=client,
         form_data=form_data,
         multipart_data=multipart_data,
         json_body=json_body,
-        jira_api_key=jira_api_key,
     )
 
     async with client.get_async_session().post(
         verify_ssl=client.verify_ssl, raise_for_status=True, **kwargs
     ) as response:
         content = await response.read()
         resp = requests.Response()
         resp.status_code = response.status
         resp._content = content
 
     return _build_response(response=resp)
 
 
 async def async_(
-    flaw_id: str,
     *,
     client: AuthenticatedClient,
-    form_data: Reject,
-    multipart_data: Reject,
-    json_body: Reject,
-    jira_api_key: str,
-) -> Optional[OsidbApiV1FlawsRejectCreateResponse200]:
-    """workflow promotion API endpoint
-
-    try to reject a flaw / task"""
+    form_data: FlawPost,
+    multipart_data: FlawPost,
+    json_body: FlawPost,
+) -> Optional[OsidbApiV1FlawsCreateResponse201]:
+    """ """
 
     return (
         await async_detailed(
-            flaw_id=flaw_id,
             client=client,
             form_data=form_data,
             multipart_data=multipart_data,
             json_body=json_body,
-            jira_api_key=jira_api_key,
         )
     ).parsed
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_manifest_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_manifest_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_schema_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_schema_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_status_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_status_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_create.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_create.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,26 +15,21 @@
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
     form_data: TrackerPost,
     multipart_data: TrackerPost,
     json_body: TrackerPost,
-    bugzilla_api_key: str,
-    jira_api_key: str,
 ) -> Dict[str, Any]:
     url = "{}/osidb/api/v1/trackers".format(
         client.base_url,
     )
 
     headers: Dict[str, Any] = client.get_headers()
 
-    headers["bugzilla-api-key"] = bugzilla_api_key
-    headers["jira-api-key"] = jira_api_key
-
     json_json_body: Dict[str, Any] = UNSET
     if not isinstance(json_body, Unset):
         json_body.to_dict()
 
     multipart_multipart_data: Dict[str, Any] = UNSET
     if not isinstance(multipart_data, Unset):
         multipart_data.to_multipart()
@@ -74,24 +69,20 @@
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
     form_data: TrackerPost,
     multipart_data: TrackerPost,
     json_body: TrackerPost,
-    bugzilla_api_key: str,
-    jira_api_key: str,
 ) -> Response[OsidbApiV1TrackersCreateResponse201]:
     kwargs = _get_kwargs(
         client=client,
         form_data=form_data,
         multipart_data=multipart_data,
         json_body=json_body,
-        bugzilla_api_key=bugzilla_api_key,
-        jira_api_key=jira_api_key,
     )
 
     response = requests.post(
         verify=client.verify_ssl,
         auth=client.auth,
         timeout=client.timeout,
         **kwargs,
@@ -103,45 +94,37 @@
 
 def sync(
     *,
     client: AuthenticatedClient,
     form_data: TrackerPost,
     multipart_data: TrackerPost,
     json_body: TrackerPost,
-    bugzilla_api_key: str,
-    jira_api_key: str,
 ) -> Optional[OsidbApiV1TrackersCreateResponse201]:
     """ """
 
     return sync_detailed(
         client=client,
         form_data=form_data,
         multipart_data=multipart_data,
         json_body=json_body,
-        bugzilla_api_key=bugzilla_api_key,
-        jira_api_key=jira_api_key,
     ).parsed
 
 
 async def async_detailed(
     *,
     client: AuthenticatedClient,
     form_data: TrackerPost,
     multipart_data: TrackerPost,
     json_body: TrackerPost,
-    bugzilla_api_key: str,
-    jira_api_key: str,
 ) -> Response[OsidbApiV1TrackersCreateResponse201]:
     kwargs = _get_kwargs(
         client=client,
         form_data=form_data,
         multipart_data=multipart_data,
         json_body=json_body,
-        bugzilla_api_key=bugzilla_api_key,
-        jira_api_key=jira_api_key,
     )
 
     async with client.get_async_session().post(
         verify_ssl=client.verify_ssl, raise_for_status=True, **kwargs
     ) as response:
         content = await response.read()
         resp = requests.Response()
@@ -153,22 +136,18 @@
 
 async def async_(
     *,
     client: AuthenticatedClient,
     form_data: TrackerPost,
     multipart_data: TrackerPost,
     json_body: TrackerPost,
-    bugzilla_api_key: str,
-    jira_api_key: str,
 ) -> Optional[OsidbApiV1TrackersCreateResponse201]:
     """ """
 
     return (
         await async_detailed(
             client=client,
             form_data=form_data,
             multipart_data=multipart_data,
             json_body=json_body,
-            bugzilla_api_key=bugzilla_api_key,
-            jira_api_key=jira_api_key,
         )
     ).parsed
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,16 @@
     "affects__cvss3": str,
     "affects__cvss3_score": float,
     "affects__cvss3_score__gt": float,
     "affects__cvss3_score__gte": float,
     "affects__cvss3_score__lt": float,
     "affects__cvss3_score__lte": float,
     "affects__embargoed": bool,
-    "affects__flaw__component": str,
+    "affects__flaw__component": List[str],
+    "affects__flaw__components": List[str],
     "affects__flaw__created_dt": datetime.datetime,
     "affects__flaw__created_dt__date": datetime.date,
     "affects__flaw__created_dt__date__gte": datetime.date,
     "affects__flaw__created_dt__date__lte": datetime.date,
     "affects__flaw__created_dt__gt": datetime.datetime,
     "affects__flaw__created_dt__gte": datetime.datetime,
     "affects__flaw__created_dt__lt": datetime.datetime,
@@ -174,15 +175,16 @@
     affects_cvss3: Union[Unset, None, str] = UNSET,
     affects_cvss3_score: Union[Unset, None, float] = UNSET,
     affects_cvss3_score_gt: Union[Unset, None, float] = UNSET,
     affects_cvss3_score_gte: Union[Unset, None, float] = UNSET,
     affects_cvss3_score_lt: Union[Unset, None, float] = UNSET,
     affects_cvss3_score_lte: Union[Unset, None, float] = UNSET,
     affects_embargoed: Union[Unset, None, bool] = UNSET,
-    affects_flaw_component: Union[Unset, None, str] = UNSET,
+    affects_flaw_component: Union[Unset, None, List[str]] = UNSET,
+    affects_flaw_components: Union[Unset, None, List[str]] = UNSET,
     affects_flaw_created_dt: Union[Unset, None, datetime.datetime] = UNSET,
     affects_flaw_created_dt_date: Union[Unset, None, datetime.date] = UNSET,
     affects_flaw_created_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     affects_flaw_created_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     affects_flaw_created_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     affects_flaw_created_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     affects_flaw_created_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
@@ -341,14 +343,28 @@
 
     json_affects_created_dt_lte: Union[Unset, None, str] = UNSET
     if not isinstance(affects_created_dt_lte, Unset):
         json_affects_created_dt_lte = (
             affects_created_dt_lte.isoformat() if affects_created_dt_lte else None
         )
 
+    json_affects_flaw_component: Union[Unset, None, List[str]] = UNSET
+    if not isinstance(affects_flaw_component, Unset):
+        if affects_flaw_component is None:
+            json_affects_flaw_component = None
+        else:
+            json_affects_flaw_component = affects_flaw_component
+
+    json_affects_flaw_components: Union[Unset, None, List[str]] = UNSET
+    if not isinstance(affects_flaw_components, Unset):
+        if affects_flaw_components is None:
+            json_affects_flaw_components = None
+        else:
+            json_affects_flaw_components = affects_flaw_components
+
     json_affects_flaw_created_dt: Union[Unset, None, str] = UNSET
     if not isinstance(affects_flaw_created_dt, Unset):
         json_affects_flaw_created_dt = (
             affects_flaw_created_dt.isoformat() if affects_flaw_created_dt else None
         )
 
     json_affects_flaw_created_dt_date: Union[Unset, None, str] = UNSET
@@ -774,15 +790,16 @@
         "affects__cvss3": affects_cvss3,
         "affects__cvss3_score": affects_cvss3_score,
         "affects__cvss3_score__gt": affects_cvss3_score_gt,
         "affects__cvss3_score__gte": affects_cvss3_score_gte,
         "affects__cvss3_score__lt": affects_cvss3_score_lt,
         "affects__cvss3_score__lte": affects_cvss3_score_lte,
         "affects__embargoed": affects_embargoed,
-        "affects__flaw__component": affects_flaw_component,
+        "affects__flaw__component": json_affects_flaw_component,
+        "affects__flaw__components": json_affects_flaw_components,
         "affects__flaw__created_dt": json_affects_flaw_created_dt,
         "affects__flaw__created_dt__date": json_affects_flaw_created_dt_date,
         "affects__flaw__created_dt__date__gte": json_affects_flaw_created_dt_date_gte,
         "affects__flaw__created_dt__date__lte": json_affects_flaw_created_dt_date_lte,
         "affects__flaw__created_dt__gt": json_affects_flaw_created_dt_gt,
         "affects__flaw__created_dt__gte": json_affects_flaw_created_dt_gte,
         "affects__flaw__created_dt__lt": json_affects_flaw_created_dt_lt,
@@ -928,15 +945,16 @@
     affects_cvss3: Union[Unset, None, str] = UNSET,
     affects_cvss3_score: Union[Unset, None, float] = UNSET,
     affects_cvss3_score_gt: Union[Unset, None, float] = UNSET,
     affects_cvss3_score_gte: Union[Unset, None, float] = UNSET,
     affects_cvss3_score_lt: Union[Unset, None, float] = UNSET,
     affects_cvss3_score_lte: Union[Unset, None, float] = UNSET,
     affects_embargoed: Union[Unset, None, bool] = UNSET,
-    affects_flaw_component: Union[Unset, None, str] = UNSET,
+    affects_flaw_component: Union[Unset, None, List[str]] = UNSET,
+    affects_flaw_components: Union[Unset, None, List[str]] = UNSET,
     affects_flaw_created_dt: Union[Unset, None, datetime.datetime] = UNSET,
     affects_flaw_created_dt_date: Union[Unset, None, datetime.date] = UNSET,
     affects_flaw_created_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     affects_flaw_created_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     affects_flaw_created_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     affects_flaw_created_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     affects_flaw_created_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
@@ -1053,14 +1071,15 @@
         affects_cvss3_score=affects_cvss3_score,
         affects_cvss3_score_gt=affects_cvss3_score_gt,
         affects_cvss3_score_gte=affects_cvss3_score_gte,
         affects_cvss3_score_lt=affects_cvss3_score_lt,
         affects_cvss3_score_lte=affects_cvss3_score_lte,
         affects_embargoed=affects_embargoed,
         affects_flaw_component=affects_flaw_component,
+        affects_flaw_components=affects_flaw_components,
         affects_flaw_created_dt=affects_flaw_created_dt,
         affects_flaw_created_dt_date=affects_flaw_created_dt_date,
         affects_flaw_created_dt_date_gte=affects_flaw_created_dt_date_gte,
         affects_flaw_created_dt_date_lte=affects_flaw_created_dt_date_lte,
         affects_flaw_created_dt_gt=affects_flaw_created_dt_gt,
         affects_flaw_created_dt_gte=affects_flaw_created_dt_gte,
         affects_flaw_created_dt_lt=affects_flaw_created_dt_lt,
@@ -1183,15 +1202,16 @@
     affects_cvss3: Union[Unset, None, str] = UNSET,
     affects_cvss3_score: Union[Unset, None, float] = UNSET,
     affects_cvss3_score_gt: Union[Unset, None, float] = UNSET,
     affects_cvss3_score_gte: Union[Unset, None, float] = UNSET,
     affects_cvss3_score_lt: Union[Unset, None, float] = UNSET,
     affects_cvss3_score_lte: Union[Unset, None, float] = UNSET,
     affects_embargoed: Union[Unset, None, bool] = UNSET,
-    affects_flaw_component: Union[Unset, None, str] = UNSET,
+    affects_flaw_component: Union[Unset, None, List[str]] = UNSET,
+    affects_flaw_components: Union[Unset, None, List[str]] = UNSET,
     affects_flaw_created_dt: Union[Unset, None, datetime.datetime] = UNSET,
     affects_flaw_created_dt_date: Union[Unset, None, datetime.date] = UNSET,
     affects_flaw_created_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     affects_flaw_created_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     affects_flaw_created_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     affects_flaw_created_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     affects_flaw_created_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
@@ -1310,14 +1330,15 @@
         affects_cvss3_score=affects_cvss3_score,
         affects_cvss3_score_gt=affects_cvss3_score_gt,
         affects_cvss3_score_gte=affects_cvss3_score_gte,
         affects_cvss3_score_lt=affects_cvss3_score_lt,
         affects_cvss3_score_lte=affects_cvss3_score_lte,
         affects_embargoed=affects_embargoed,
         affects_flaw_component=affects_flaw_component,
+        affects_flaw_components=affects_flaw_components,
         affects_flaw_created_dt=affects_flaw_created_dt,
         affects_flaw_created_dt_date=affects_flaw_created_dt_date,
         affects_flaw_created_dt_date_gte=affects_flaw_created_dt_date_gte,
         affects_flaw_created_dt_date_lte=affects_flaw_created_dt_date_lte,
         affects_flaw_created_dt_gt=affects_flaw_created_dt_gt,
         affects_flaw_created_dt_gte=affects_flaw_created_dt_gte,
         affects_flaw_created_dt_lt=affects_flaw_created_dt_lt,
@@ -1430,15 +1451,16 @@
     affects_cvss3: Union[Unset, None, str] = UNSET,
     affects_cvss3_score: Union[Unset, None, float] = UNSET,
     affects_cvss3_score_gt: Union[Unset, None, float] = UNSET,
     affects_cvss3_score_gte: Union[Unset, None, float] = UNSET,
     affects_cvss3_score_lt: Union[Unset, None, float] = UNSET,
     affects_cvss3_score_lte: Union[Unset, None, float] = UNSET,
     affects_embargoed: Union[Unset, None, bool] = UNSET,
-    affects_flaw_component: Union[Unset, None, str] = UNSET,
+    affects_flaw_component: Union[Unset, None, List[str]] = UNSET,
+    affects_flaw_components: Union[Unset, None, List[str]] = UNSET,
     affects_flaw_created_dt: Union[Unset, None, datetime.datetime] = UNSET,
     affects_flaw_created_dt_date: Union[Unset, None, datetime.date] = UNSET,
     affects_flaw_created_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     affects_flaw_created_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     affects_flaw_created_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     affects_flaw_created_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     affects_flaw_created_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
@@ -1555,14 +1577,15 @@
         affects_cvss3_score=affects_cvss3_score,
         affects_cvss3_score_gt=affects_cvss3_score_gt,
         affects_cvss3_score_gte=affects_cvss3_score_gte,
         affects_cvss3_score_lt=affects_cvss3_score_lt,
         affects_cvss3_score_lte=affects_cvss3_score_lte,
         affects_embargoed=affects_embargoed,
         affects_flaw_component=affects_flaw_component,
+        affects_flaw_components=affects_flaw_components,
         affects_flaw_created_dt=affects_flaw_created_dt,
         affects_flaw_created_dt_date=affects_flaw_created_dt_date,
         affects_flaw_created_dt_date_gte=affects_flaw_created_dt_date_gte,
         affects_flaw_created_dt_date_lte=affects_flaw_created_dt_date_lte,
         affects_flaw_created_dt_gt=affects_flaw_created_dt_gt,
         affects_flaw_created_dt_gte=affects_flaw_created_dt_gte,
         affects_flaw_created_dt_lt=affects_flaw_created_dt_lt,
@@ -1685,15 +1708,16 @@
     affects_cvss3: Union[Unset, None, str] = UNSET,
     affects_cvss3_score: Union[Unset, None, float] = UNSET,
     affects_cvss3_score_gt: Union[Unset, None, float] = UNSET,
     affects_cvss3_score_gte: Union[Unset, None, float] = UNSET,
     affects_cvss3_score_lt: Union[Unset, None, float] = UNSET,
     affects_cvss3_score_lte: Union[Unset, None, float] = UNSET,
     affects_embargoed: Union[Unset, None, bool] = UNSET,
-    affects_flaw_component: Union[Unset, None, str] = UNSET,
+    affects_flaw_component: Union[Unset, None, List[str]] = UNSET,
+    affects_flaw_components: Union[Unset, None, List[str]] = UNSET,
     affects_flaw_created_dt: Union[Unset, None, datetime.datetime] = UNSET,
     affects_flaw_created_dt_date: Union[Unset, None, datetime.date] = UNSET,
     affects_flaw_created_dt_date_gte: Union[Unset, None, datetime.date] = UNSET,
     affects_flaw_created_dt_date_lte: Union[Unset, None, datetime.date] = UNSET,
     affects_flaw_created_dt_gt: Union[Unset, None, datetime.datetime] = UNSET,
     affects_flaw_created_dt_gte: Union[Unset, None, datetime.datetime] = UNSET,
     affects_flaw_created_dt_lt: Union[Unset, None, datetime.datetime] = UNSET,
@@ -1813,14 +1837,15 @@
             affects_cvss3_score=affects_cvss3_score,
             affects_cvss3_score_gt=affects_cvss3_score_gt,
             affects_cvss3_score_gte=affects_cvss3_score_gte,
             affects_cvss3_score_lt=affects_cvss3_score_lt,
             affects_cvss3_score_lte=affects_cvss3_score_lte,
             affects_embargoed=affects_embargoed,
             affects_flaw_component=affects_flaw_component,
+            affects_flaw_components=affects_flaw_components,
             affects_flaw_created_dt=affects_flaw_created_dt,
             affects_flaw_created_dt_date=affects_flaw_created_dt_date,
             affects_flaw_created_dt_date_gte=affects_flaw_created_dt_date_gte,
             affects_flaw_created_dt_date_lte=affects_flaw_created_dt_date_lte,
             affects_flaw_created_dt_gt=affects_flaw_created_dt_gt,
             affects_flaw_created_dt_gte=affects_flaw_created_dt_gte,
             affects_flaw_created_dt_lt=affects_flaw_created_dt_lt,
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_update.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_create.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,35 @@
 from typing import Any, Dict, Optional
 
 import requests
 
 from ...client import AuthenticatedClient
-from ...models.osidb_api_v1_trackers_update_response_200 import (
-    OsidbApiV1TrackersUpdateResponse200,
+from ...models.affect_post import AffectPost
+from ...models.osidb_api_v1_affects_create_response_201 import (
+    OsidbApiV1AffectsCreateResponse201,
 )
-from ...models.tracker import Tracker
 from ...types import UNSET, Response, Unset
 
 QUERY_PARAMS = {}
-REQUEST_BODY_TYPE = Tracker
+REQUEST_BODY_TYPE = AffectPost
 
 
 def _get_kwargs(
-    uuid: str,
     *,
     client: AuthenticatedClient,
-    form_data: Tracker,
-    multipart_data: Tracker,
-    json_body: Tracker,
-    bugzilla_api_key: str,
-    jira_api_key: str,
+    form_data: AffectPost,
+    multipart_data: AffectPost,
+    json_body: AffectPost,
 ) -> Dict[str, Any]:
-    url = "{}/osidb/api/v1/trackers/{uuid}".format(
+    url = "{}/osidb/api/v1/affects".format(
         client.base_url,
-        uuid=uuid,
     )
 
     headers: Dict[str, Any] = client.get_headers()
 
-    headers["bugzilla-api-key"] = bugzilla_api_key
-    headers["jira-api-key"] = jira_api_key
-
     json_json_body: Dict[str, Any] = UNSET
     if not isinstance(json_body, Unset):
         json_body.to_dict()
 
     multipart_multipart_data: Dict[str, Any] = UNSET
     if not isinstance(multipart_data, Unset):
         multipart_data.to_multipart()
@@ -46,139 +39,115 @@
         "headers": headers,
         "data": form_data.to_dict(),
     }
 
 
 def _parse_response(
     *, response: requests.Response
-) -> Optional[OsidbApiV1TrackersUpdateResponse200]:
-    if response.status_code == 200:
-        _response_200 = response.json()
-        response_200: OsidbApiV1TrackersUpdateResponse200
-        if isinstance(_response_200, Unset):
-            response_200 = UNSET
+) -> Optional[OsidbApiV1AffectsCreateResponse201]:
+    if response.status_code == 201:
+        _response_201 = response.json()
+        response_201: OsidbApiV1AffectsCreateResponse201
+        if isinstance(_response_201, Unset):
+            response_201 = UNSET
         else:
-            response_200 = OsidbApiV1TrackersUpdateResponse200.from_dict(_response_200)
+            response_201 = OsidbApiV1AffectsCreateResponse201.from_dict(_response_201)
 
-        return response_200
+        return response_201
     return None
 
 
 def _build_response(
     *, response: requests.Response
-) -> Response[OsidbApiV1TrackersUpdateResponse200]:
+) -> Response[OsidbApiV1AffectsCreateResponse201]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    uuid: str,
     *,
     client: AuthenticatedClient,
-    form_data: Tracker,
-    multipart_data: Tracker,
-    json_body: Tracker,
-    bugzilla_api_key: str,
-    jira_api_key: str,
-) -> Response[OsidbApiV1TrackersUpdateResponse200]:
+    form_data: AffectPost,
+    multipart_data: AffectPost,
+    json_body: AffectPost,
+) -> Response[OsidbApiV1AffectsCreateResponse201]:
     kwargs = _get_kwargs(
-        uuid=uuid,
         client=client,
         form_data=form_data,
         multipart_data=multipart_data,
         json_body=json_body,
-        bugzilla_api_key=bugzilla_api_key,
-        jira_api_key=jira_api_key,
     )
 
-    response = requests.put(
+    response = requests.post(
         verify=client.verify_ssl,
         auth=client.auth,
         timeout=client.timeout,
         **kwargs,
     )
     response.raise_for_status()
 
     return _build_response(response=response)
 
 
 def sync(
-    uuid: str,
     *,
     client: AuthenticatedClient,
-    form_data: Tracker,
-    multipart_data: Tracker,
-    json_body: Tracker,
-    bugzilla_api_key: str,
-    jira_api_key: str,
-) -> Optional[OsidbApiV1TrackersUpdateResponse200]:
+    form_data: AffectPost,
+    multipart_data: AffectPost,
+    json_body: AffectPost,
+) -> Optional[OsidbApiV1AffectsCreateResponse201]:
     """ """
 
     return sync_detailed(
-        uuid=uuid,
         client=client,
         form_data=form_data,
         multipart_data=multipart_data,
         json_body=json_body,
-        bugzilla_api_key=bugzilla_api_key,
-        jira_api_key=jira_api_key,
     ).parsed
 
 
 async def async_detailed(
-    uuid: str,
     *,
     client: AuthenticatedClient,
-    form_data: Tracker,
-    multipart_data: Tracker,
-    json_body: Tracker,
-    bugzilla_api_key: str,
-    jira_api_key: str,
-) -> Response[OsidbApiV1TrackersUpdateResponse200]:
+    form_data: AffectPost,
+    multipart_data: AffectPost,
+    json_body: AffectPost,
+) -> Response[OsidbApiV1AffectsCreateResponse201]:
     kwargs = _get_kwargs(
-        uuid=uuid,
         client=client,
         form_data=form_data,
         multipart_data=multipart_data,
         json_body=json_body,
-        bugzilla_api_key=bugzilla_api_key,
-        jira_api_key=jira_api_key,
     )
 
-    async with client.get_async_session().put(
+    async with client.get_async_session().post(
         verify_ssl=client.verify_ssl, raise_for_status=True, **kwargs
     ) as response:
         content = await response.read()
         resp = requests.Response()
         resp.status_code = response.status
         resp._content = content
 
     return _build_response(response=resp)
 
 
 async def async_(
-    uuid: str,
     *,
     client: AuthenticatedClient,
-    form_data: Tracker,
-    multipart_data: Tracker,
-    json_body: Tracker,
-    bugzilla_api_key: str,
-    jira_api_key: str,
-) -> Optional[OsidbApiV1TrackersUpdateResponse200]:
+    form_data: AffectPost,
+    multipart_data: AffectPost,
+    json_body: AffectPost,
+) -> Optional[OsidbApiV1AffectsCreateResponse201]:
     """ """
 
     return (
         await async_detailed(
-            uuid=uuid,
             client=client,
             form_data=form_data,
             multipart_data=multipart_data,
             json_body=json_body,
-            bugzilla_api_key=bugzilla_api_key,
-            jira_api_key=jira_api_key,
         )
     ).parsed
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_healthy_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_healthy_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osidb/osidb_whoami_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osidb/osidb_whoami_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_adjust_create.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_adjust_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve_2.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osim/osim_healthy_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osim/osim_healthy_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/osim/osim_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/osim/osim_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/trackers/trackers_api_v1_file_create.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/trackers/trackers_api_v1_file_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/workflows/workflows_api_v1_adjust_create.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/workflows/workflows_api_v1_adjust_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/workflows/workflows_api_v1_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/workflows/workflows_api_v1_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/workflows/workflows_api_v1_retrieve_2.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/workflows/workflows_api_v1_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/workflows/workflows_healthy_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/workflows/workflows_healthy_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/api/workflows/workflows_retrieve.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/api/workflows/workflows_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/client.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/client.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/__init__.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 """ Contains all the data models used in inputs/outputs """
 
 from .affect import Affect
+from .affect_alerts import AffectAlerts
 from .affect_cvss import AffectCVSS
+from .affect_cvss_alerts import AffectCVSSAlerts
 from .affect_cvss_post import AffectCVSSPost
+from .affect_cvss_post_alerts import AffectCVSSPostAlerts
 from .affect_cvss_put import AffectCVSSPut
+from .affect_cvss_put_alerts import AffectCVSSPutAlerts
 from .affect_meta_attr import AffectMetaAttr
 from .affect_post import AffectPost
+from .affect_post_alerts import AffectPostAlerts
 from .affect_post_meta_attr import AffectPostMetaAttr
 from .affect_report_data import AffectReportData
 from .affect_type import AffectType
 from .affectedness_enum import AffectednessEnum
 from .auth_token_create_response_200 import AuthTokenCreateResponse200
 from .auth_token_refresh_create_response_200 import AuthTokenRefreshCreateResponse200
 from .auth_token_retrieve_response_200 import AuthTokenRetrieveResponse200
@@ -31,15 +36,17 @@
     CollectorsApiV1StatusRetrieveResponse200CollectorsItemState,
 )
 from .collectors_healthy_retrieve_response_200 import (
     CollectorsHealthyRetrieveResponse200,
 )
 from .collectors_retrieve_response_200 import CollectorsRetrieveResponse200
 from .comment import Comment
+from .comment_alerts import CommentAlerts
 from .comment_meta_attr import CommentMetaAttr
+from .cvss_version_enum import CvssVersionEnum
 from .epss import EPSS
 from .erratum import Erratum
 from .exploit_only_report_data import ExploitOnlyReportData
 from .exploit_only_report_data_source_enum import ExploitOnlyReportDataSourceEnum
 from .exploits_api_v1_collect_update_response_200 import (
     ExploitsApiV1CollectUpdateResponse200,
 )
@@ -84,56 +91,70 @@
     ExploitsApiV1StatusRetrieveResponse200,
 )
 from .exploits_api_v1_supported_products_list_response_200 import (
     ExploitsApiV1SupportedProductsListResponse200,
 )
 from .flaw import Flaw
 from .flaw_acknowledgment import FlawAcknowledgment
+from .flaw_acknowledgment_alerts import FlawAcknowledgmentAlerts
 from .flaw_acknowledgment_post import FlawAcknowledgmentPost
+from .flaw_acknowledgment_post_alerts import FlawAcknowledgmentPostAlerts
 from .flaw_acknowledgment_put import FlawAcknowledgmentPut
+from .flaw_acknowledgment_put_alerts import FlawAcknowledgmentPutAlerts
+from .flaw_alerts import FlawAlerts
 from .flaw_classification import FlawClassification
 from .flaw_classification_state import FlawClassificationState
 from .flaw_comment import FlawComment
+from .flaw_comment_alerts import FlawCommentAlerts
 from .flaw_comment_post import FlawCommentPost
+from .flaw_comment_post_alerts import FlawCommentPostAlerts
 from .flaw_comment_post_meta_attr import FlawCommentPostMetaAttr
 from .flaw_comment_type import FlawCommentType
 from .flaw_cvss import FlawCVSS
+from .flaw_cvss_alerts import FlawCVSSAlerts
 from .flaw_cvss_post import FlawCVSSPost
+from .flaw_cvss_post_alerts import FlawCVSSPostAlerts
 from .flaw_cvss_put import FlawCVSSPut
+from .flaw_cvss_put_alerts import FlawCVSSPutAlerts
 from .flaw_meta_attr import FlawMetaAttr
 from .flaw_meta_type import FlawMetaType
 from .flaw_package_version import FlawPackageVersion
 from .flaw_package_version_post import FlawPackageVersionPost
 from .flaw_package_version_put import FlawPackageVersionPut
 from .flaw_post import FlawPost
+from .flaw_post_alerts import FlawPostAlerts
 from .flaw_post_classification import FlawPostClassification
 from .flaw_post_classification_state import FlawPostClassificationState
 from .flaw_post_meta_attr import FlawPostMetaAttr
 from .flaw_reference import FlawReference
+from .flaw_reference_alerts import FlawReferenceAlerts
 from .flaw_reference_post import FlawReferencePost
+from .flaw_reference_post_alerts import FlawReferencePostAlerts
 from .flaw_reference_put import FlawReferencePut
+from .flaw_reference_put_alerts import FlawReferencePutAlerts
 from .flaw_reference_type import FlawReferenceType
 from .flaw_report_data import FlawReportData
 from .flaw_type import FlawType
 from .flaw_uuid_list import FlawUUIDList
 from .flaw_version import FlawVersion
 from .impact_enum import ImpactEnum
 from .issuer_enum import IssuerEnum
 from .major_incident_state_enum import MajorIncidentStateEnum
 from .maturity_preliminary_enum import MaturityPreliminaryEnum
 from .meta import Meta
+from .meta_alerts import MetaAlerts
 from .meta_meta_attr import MetaMetaAttr
 from .module_component import ModuleComponent
 from .nist_cvss_validation_enum import NistCvssValidationEnum
 from .osidb_api_v1_affects_create_response_201 import OsidbApiV1AffectsCreateResponse201
 from .osidb_api_v1_affects_cvss_scores_create_response_201 import (
     OsidbApiV1AffectsCvssScoresCreateResponse201,
 )
-from .osidb_api_v1_affects_cvss_scores_destroy_response_204 import (
-    OsidbApiV1AffectsCvssScoresDestroyResponse204,
+from .osidb_api_v1_affects_cvss_scores_destroy_response_200 import (
+    OsidbApiV1AffectsCvssScoresDestroyResponse200,
 )
 from .osidb_api_v1_affects_cvss_scores_list_issuer import (
     OsidbApiV1AffectsCvssScoresListIssuer,
 )
 from .osidb_api_v1_affects_cvss_scores_list_response_200 import (
     OsidbApiV1AffectsCvssScoresListResponse200,
 )
@@ -229,14 +250,17 @@
 )
 from .osidb_api_v1_flaws_list_order_item import OsidbApiV1FlawsListOrderItem
 from .osidb_api_v1_flaws_list_references_type import OsidbApiV1FlawsListReferencesType
 from .osidb_api_v1_flaws_list_requires_summary import OsidbApiV1FlawsListRequiresSummary
 from .osidb_api_v1_flaws_list_response_200 import OsidbApiV1FlawsListResponse200
 from .osidb_api_v1_flaws_list_source import OsidbApiV1FlawsListSource
 from .osidb_api_v1_flaws_list_type import OsidbApiV1FlawsListType
+from .osidb_api_v1_flaws_list_workflow_state_item import (
+    OsidbApiV1FlawsListWorkflowStateItem,
+)
 from .osidb_api_v1_flaws_package_versions_create_response_201 import (
     OsidbApiV1FlawsPackageVersionsCreateResponse201,
 )
 from .osidb_api_v1_flaws_package_versions_destroy_response_200 import (
     OsidbApiV1FlawsPackageVersionsDestroyResponse200,
 )
 from .osidb_api_v1_flaws_package_versions_list_response_200 import (
@@ -333,14 +357,15 @@
 )
 from .osim_api_v1_workflows_retrieve_response_200 import (
     OsimApiV1WorkflowsRetrieveResponse200,
 )
 from .osim_healthy_retrieve_response_200 import OsimHealthyRetrieveResponse200
 from .osim_retrieve_response_200 import OsimRetrieveResponse200
 from .package import Package
+from .package_alerts import PackageAlerts
 from .package_ver import PackageVer
 from .paginated_affect_cvss_list import PaginatedAffectCVSSList
 from .paginated_affect_list import PaginatedAffectList
 from .paginated_epss_list import PaginatedEPSSList
 from .paginated_exploit_only_report_data_list import PaginatedExploitOnlyReportDataList
 from .paginated_flaw_acknowledgment_list import PaginatedFlawAcknowledgmentList
 from .paginated_flaw_comment_list import PaginatedFlawCommentList
@@ -357,16 +382,18 @@
 from .resolution_enum import ResolutionEnum
 from .source_8d8_enum import Source8D8Enum
 from .supported_products import SupportedProducts
 from .token_obtain_pair import TokenObtainPair
 from .token_refresh import TokenRefresh
 from .token_verify import TokenVerify
 from .tracker import Tracker
+from .tracker_alerts import TrackerAlerts
 from .tracker_meta_attr import TrackerMetaAttr
 from .tracker_post import TrackerPost
+from .tracker_post_alerts import TrackerPostAlerts
 from .tracker_post_meta_attr import TrackerPostMetaAttr
 from .tracker_report_data import TrackerReportData
 from .tracker_suggestion import TrackerSuggestion
 from .tracker_type import TrackerType
 from .workflows_api_v1_adjust_create_response_200 import (
     WorkflowsApiV1AdjustCreateResponse200,
 )
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/affect.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/affect.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 import json
 from typing import Any, Dict, List, Optional, Tuple, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.affect_alerts import AffectAlerts
 from ..models.affect_cvss import AffectCVSS
 from ..models.affect_meta_attr import AffectMetaAttr
 from ..models.affect_type import AffectType
 from ..models.affectedness_enum import AffectednessEnum
 from ..models.blank_enum import BlankEnum
 from ..models.impact_enum import ImpactEnum
 from ..models.resolution_enum import ResolutionEnum
@@ -20,20 +21,22 @@
 
 @attr.s(auto_attribs=True)
 class Affect(OSIDBModel):
     """Affect serializer"""
 
     uuid: str
     ps_module: str
+    ps_product: str
     ps_component: str
     trackers: List[Tracker]
     meta_attr: AffectMetaAttr
     delegated_resolution: str
     cvss_scores: List[AffectCVSS]
     embargoed: bool
+    alerts: AffectAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     flaw: Optional[str]
     type: Union[Unset, AffectType] = UNSET
     affectedness: Union[AffectednessEnum, BlankEnum, Unset] = UNSET
     resolution: Union[BlankEnum, ResolutionEnum, Unset] = UNSET
     impact: Union[BlankEnum, ImpactEnum, Unset] = UNSET
@@ -42,14 +45,15 @@
     cvss3: Union[Unset, str] = UNSET
     cvss3_score: Union[Unset, None, float] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         uuid = self.uuid
         ps_module = self.ps_module
+        ps_product = self.ps_product
         ps_component = self.ps_component
         trackers: List[Dict[str, Any]] = UNSET
         if not isinstance(self.trackers, Unset):
             trackers = []
             for trackers_item_data in self.trackers:
                 trackers_item: Dict[str, Any] = UNSET
                 if not isinstance(trackers_item_data, Unset):
@@ -69,14 +73,18 @@
                 cvss_scores_item: Dict[str, Any] = UNSET
                 if not isinstance(cvss_scores_item_data, Unset):
                     cvss_scores_item = cvss_scores_item_data.to_dict()
 
                 cvss_scores.append(cvss_scores_item)
 
         embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
@@ -139,26 +147,30 @@
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(ps_module, Unset):
             field_dict["ps_module"] = ps_module
+        if not isinstance(ps_product, Unset):
+            field_dict["ps_product"] = ps_product
         if not isinstance(ps_component, Unset):
             field_dict["ps_component"] = ps_component
         if not isinstance(trackers, Unset):
             field_dict["trackers"] = trackers
         if not isinstance(meta_attr, Unset):
             field_dict["meta_attr"] = meta_attr
         if not isinstance(delegated_resolution, Unset):
             field_dict["delegated_resolution"] = delegated_resolution
         if not isinstance(cvss_scores, Unset):
             field_dict["cvss_scores"] = cvss_scores
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(flaw, Unset):
             field_dict["flaw"] = flaw
         if not isinstance(type, Unset):
@@ -183,14 +195,19 @@
     def to_multipart(self) -> Dict[str, Any]:
         uuid = self.uuid if self.uuid is UNSET else (None, str(self.uuid), "text/plain")
         ps_module = (
             self.ps_module
             if self.ps_module is UNSET
             else (None, str(self.ps_module), "text/plain")
         )
+        ps_product = (
+            self.ps_product
+            if self.ps_product is UNSET
+            else (None, str(self.ps_product), "text/plain")
+        )
         ps_component = (
             self.ps_component
             if self.ps_component is UNSET
             else (None, str(self.ps_component), "text/plain")
         )
         trackers: Union[Unset, Tuple[None, str, str]] = UNSET
         if not isinstance(self.trackers, Unset):
@@ -224,14 +241,18 @@
             cvss_scores = (None, json.dumps(_temp_cvss_scores), "application/json")
 
         embargoed = (
             self.embargoed
             if self.embargoed is UNSET
             else (None, str(self.embargoed), "text/plain")
         )
+        alerts: Union[Unset, Tuple[None, str, str]] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = (None, json.dumps(self.alerts.to_dict()), "application/json")
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
@@ -311,26 +332,30 @@
                 for key, value in self.additional_properties.items()
             }
         )
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(ps_module, Unset):
             field_dict["ps_module"] = ps_module
+        if not isinstance(ps_product, Unset):
+            field_dict["ps_product"] = ps_product
         if not isinstance(ps_component, Unset):
             field_dict["ps_component"] = ps_component
         if not isinstance(trackers, Unset):
             field_dict["trackers"] = trackers
         if not isinstance(meta_attr, Unset):
             field_dict["meta_attr"] = meta_attr
         if not isinstance(delegated_resolution, Unset):
             field_dict["delegated_resolution"] = delegated_resolution
         if not isinstance(cvss_scores, Unset):
             field_dict["cvss_scores"] = cvss_scores
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(flaw, Unset):
             field_dict["flaw"] = flaw
         if not isinstance(type, Unset):
@@ -355,14 +380,16 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         uuid = d.pop("uuid", UNSET)
 
         ps_module = d.pop("ps_module", UNSET)
 
+        ps_product = d.pop("ps_product", UNSET)
+
         ps_component = d.pop("ps_component", UNSET)
 
         trackers = []
         _trackers = d.pop("trackers", UNSET)
         if _trackers is UNSET:
             trackers = UNSET
         else:
@@ -398,14 +425,21 @@
                 else:
                     cvss_scores_item = AffectCVSS.from_dict(_cvss_scores_item)
 
                 cvss_scores.append(cvss_scores_item)
 
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: AffectAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = AffectAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
@@ -521,20 +555,22 @@
         cvss3 = d.pop("cvss3", UNSET)
 
         cvss3_score = d.pop("cvss3_score", UNSET)
 
         affect = cls(
             uuid=uuid,
             ps_module=ps_module,
+            ps_product=ps_product,
             ps_component=ps_component,
             trackers=trackers,
             meta_attr=meta_attr,
             delegated_resolution=delegated_resolution,
             cvss_scores=cvss_scores,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
             flaw=flaw,
             type=type,
             affectedness=affectedness,
             resolution=resolution,
             impact=impact,
@@ -548,20 +584,22 @@
         return affect
 
     @staticmethod
     def get_fields():
         return {
             "uuid": str,
             "ps_module": str,
+            "ps_product": str,
             "ps_component": str,
             "trackers": List[Tracker],
             "meta_attr": AffectMetaAttr,
             "delegated_resolution": str,
             "cvss_scores": List[AffectCVSS],
             "embargoed": bool,
+            "alerts": AffectAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "flaw": str,
             "type": AffectType,
             "affectedness": Union[AffectednessEnum, BlankEnum],
             "resolution": Union[BlankEnum, ResolutionEnum],
             "impact": Union[BlankEnum, ImpactEnum],
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/affect_cvss.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_cvss.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,94 +1,114 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.cvss_version_enum import CvssVersionEnum
+from ..models.flaw_cvss_alerts import FlawCVSSAlerts
 from ..models.issuer_enum import IssuerEnum
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="AffectCVSS")
+T = TypeVar("T", bound="FlawCVSS")
 
 
 @attr.s(auto_attribs=True)
-class AffectCVSS(OSIDBModel):
-    """AffectCVSS serializer"""
+class FlawCVSS(OSIDBModel):
+    """FlawCVSS serializer"""
 
-    cvss_version: str
+    cvss_version: CvssVersionEnum
     issuer: IssuerEnum
+    score: float
     uuid: str
     vector: str
     embargoed: bool
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
-    affect: Union[Unset, str] = UNSET
+    alerts: FlawCVSSAlerts
     comment: Union[Unset, str] = UNSET
-    score: Union[Unset, float] = UNSET
+    flaw: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        cvss_version = self.cvss_version
+        cvss_version: str = UNSET
+        if not isinstance(self.cvss_version, Unset):
+
+            cvss_version = CvssVersionEnum(self.cvss_version).value
+
         issuer: str = UNSET
         if not isinstance(self.issuer, Unset):
 
             issuer = IssuerEnum(self.issuer).value
 
+        score = self.score
         uuid = self.uuid
         vector = self.vector
         embargoed = self.embargoed
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
-        affect = self.affect
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         comment = self.comment
-        score = self.score
+        flaw = self.flaw
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if not isinstance(cvss_version, Unset):
             field_dict["cvss_version"] = cvss_version
         if not isinstance(issuer, Unset):
             field_dict["issuer"] = issuer
+        if not isinstance(score, Unset):
+            field_dict["score"] = score
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(vector, Unset):
             field_dict["vector"] = vector
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
-        if not isinstance(affect, Unset):
-            field_dict["affect"] = affect
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(comment, Unset):
             field_dict["comment"] = comment
-        if not isinstance(score, Unset):
-            field_dict["score"] = score
+        if not isinstance(flaw, Unset):
+            field_dict["flaw"] = flaw
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        cvss_version = d.pop("cvss_version", UNSET)
+        _cvss_version = d.pop("cvss_version", UNSET)
+        cvss_version: CvssVersionEnum
+        if isinstance(_cvss_version, Unset):
+            cvss_version = UNSET
+        else:
+            cvss_version = CvssVersionEnum(_cvss_version)
 
         _issuer = d.pop("issuer", UNSET)
         issuer: IssuerEnum
         if isinstance(_issuer, Unset):
             issuer = UNSET
         else:
             issuer = IssuerEnum(_issuer)
 
+        score = d.pop("score", UNSET)
+
         uuid = d.pop("uuid", UNSET)
 
         vector = d.pop("vector", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
         _created_dt = d.pop("created_dt", UNSET)
@@ -101,49 +121,56 @@
         _updated_dt = d.pop("updated_dt", UNSET)
         updated_dt: datetime.datetime
         if isinstance(_updated_dt, Unset):
             updated_dt = UNSET
         else:
             updated_dt = isoparse(_updated_dt)
 
-        affect = d.pop("affect", UNSET)
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawCVSSAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawCVSSAlerts.from_dict(_alerts)
 
         comment = d.pop("comment", UNSET)
 
-        score = d.pop("score", UNSET)
+        flaw = d.pop("flaw", UNSET)
 
-        affect_cvss = cls(
+        flaw_cvss = cls(
             cvss_version=cvss_version,
             issuer=issuer,
+            score=score,
             uuid=uuid,
             vector=vector,
             embargoed=embargoed,
             created_dt=created_dt,
             updated_dt=updated_dt,
-            affect=affect,
+            alerts=alerts,
             comment=comment,
-            score=score,
+            flaw=flaw,
         )
 
-        affect_cvss.additional_properties = d
-        return affect_cvss
+        flaw_cvss.additional_properties = d
+        return flaw_cvss
 
     @staticmethod
     def get_fields():
         return {
-            "cvss_version": str,
+            "cvss_version": CvssVersionEnum,
             "issuer": IssuerEnum,
+            "score": float,
             "uuid": str,
             "vector": str,
             "embargoed": bool,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
-            "affect": str,
+            "alerts": FlawCVSSAlerts,
             "comment": str,
-            "score": float,
+            "flaw": str,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/affect_cvss_post.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/affect_cvss_post.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,186 +1,220 @@
 import datetime
+import json
 from typing import Any, Dict, List, Tuple, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.affect_cvss_post_alerts import AffectCVSSPostAlerts
+from ..models.cvss_version_enum import CvssVersionEnum
 from ..models.issuer_enum import IssuerEnum
 from ..types import UNSET, OSIDBModel, Unset
 
 T = TypeVar("T", bound="AffectCVSSPost")
 
 
 @attr.s(auto_attribs=True)
 class AffectCVSSPost(OSIDBModel):
     """AffectCVSS serializer"""
 
-    cvss_version: str
+    cvss_version: CvssVersionEnum
     issuer: IssuerEnum
+    score: float
     uuid: str
     vector: str
     embargoed: bool
+    alerts: AffectCVSSPostAlerts
     created_dt: datetime.datetime
     comment: Union[Unset, str] = UNSET
-    score: Union[Unset, float] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        cvss_version = self.cvss_version
+        cvss_version: str = UNSET
+        if not isinstance(self.cvss_version, Unset):
+
+            cvss_version = CvssVersionEnum(self.cvss_version).value
+
         issuer: str = UNSET
         if not isinstance(self.issuer, Unset):
 
             issuer = IssuerEnum(self.issuer).value
 
+        score = self.score
         uuid = self.uuid
         vector = self.vector
         embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         comment = self.comment
-        score = self.score
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if not isinstance(cvss_version, Unset):
             field_dict["cvss_version"] = cvss_version
         if not isinstance(issuer, Unset):
             field_dict["issuer"] = issuer
+        if not isinstance(score, Unset):
+            field_dict["score"] = score
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(vector, Unset):
             field_dict["vector"] = vector
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(comment, Unset):
             field_dict["comment"] = comment
-        if not isinstance(score, Unset):
-            field_dict["score"] = score
 
         return field_dict
 
     def to_multipart(self) -> Dict[str, Any]:
-        cvss_version = (
-            self.cvss_version
-            if self.cvss_version is UNSET
-            else (None, str(self.cvss_version), "text/plain")
-        )
+        cvss_version: Union[Unset, Tuple[None, str, str]] = UNSET
+        if not isinstance(self.cvss_version, Unset):
+
+            cvss_version = CvssVersionEnum(self.cvss_version).value
+
         issuer: Union[Unset, Tuple[None, str, str]] = UNSET
         if not isinstance(self.issuer, Unset):
 
             issuer = IssuerEnum(self.issuer).value
 
+        score = (
+            self.score if self.score is UNSET else (None, str(self.score), "text/plain")
+        )
         uuid = self.uuid if self.uuid is UNSET else (None, str(self.uuid), "text/plain")
         vector = (
             self.vector
             if self.vector is UNSET
             else (None, str(self.vector), "text/plain")
         )
         embargoed = (
             self.embargoed
             if self.embargoed is UNSET
             else (None, str(self.embargoed), "text/plain")
         )
+        alerts: Union[Unset, Tuple[None, str, str]] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = (None, json.dumps(self.alerts.to_dict()), "application/json")
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         comment = (
             self.comment
             if self.comment is UNSET
             else (None, str(self.comment), "text/plain")
         )
-        score = (
-            self.score if self.score is UNSET else (None, str(self.score), "text/plain")
-        )
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(
             {
                 key: (None, str(value), "text/plain")
                 for key, value in self.additional_properties.items()
             }
         )
         if not isinstance(cvss_version, Unset):
             field_dict["cvss_version"] = cvss_version
         if not isinstance(issuer, Unset):
             field_dict["issuer"] = issuer
+        if not isinstance(score, Unset):
+            field_dict["score"] = score
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(vector, Unset):
             field_dict["vector"] = vector
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(comment, Unset):
             field_dict["comment"] = comment
-        if not isinstance(score, Unset):
-            field_dict["score"] = score
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        cvss_version = d.pop("cvss_version", UNSET)
+        _cvss_version = d.pop("cvss_version", UNSET)
+        cvss_version: CvssVersionEnum
+        if isinstance(_cvss_version, Unset):
+            cvss_version = UNSET
+        else:
+            cvss_version = CvssVersionEnum(_cvss_version)
 
         _issuer = d.pop("issuer", UNSET)
         issuer: IssuerEnum
         if isinstance(_issuer, Unset):
             issuer = UNSET
         else:
             issuer = IssuerEnum(_issuer)
 
+        score = d.pop("score", UNSET)
+
         uuid = d.pop("uuid", UNSET)
 
         vector = d.pop("vector", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: AffectCVSSPostAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = AffectCVSSPostAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
         comment = d.pop("comment", UNSET)
 
-        score = d.pop("score", UNSET)
-
         affect_cvss_post = cls(
             cvss_version=cvss_version,
             issuer=issuer,
+            score=score,
             uuid=uuid,
             vector=vector,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             comment=comment,
-            score=score,
         )
 
         affect_cvss_post.additional_properties = d
         return affect_cvss_post
 
     @staticmethod
     def get_fields():
         return {
-            "cvss_version": str,
+            "cvss_version": CvssVersionEnum,
             "issuer": IssuerEnum,
+            "score": float,
             "uuid": str,
             "vector": str,
             "embargoed": bool,
+            "alerts": AffectCVSSPostAlerts,
             "created_dt": datetime.datetime,
             "comment": str,
-            "score": float,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/affect_cvss_put.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_cvss_put.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,89 +1,106 @@
 import datetime
+import json
 from typing import Any, Dict, List, Tuple, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.cvss_version_enum import CvssVersionEnum
+from ..models.flaw_cvss_put_alerts import FlawCVSSPutAlerts
 from ..models.issuer_enum import IssuerEnum
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="AffectCVSSPut")
+T = TypeVar("T", bound="FlawCVSSPut")
 
 
 @attr.s(auto_attribs=True)
-class AffectCVSSPut(OSIDBModel):
-    """AffectCVSS serializer"""
+class FlawCVSSPut(OSIDBModel):
+    """FlawCVSS serializer"""
 
-    cvss_version: str
+    cvss_version: CvssVersionEnum
     issuer: IssuerEnum
+    score: float
     uuid: str
     vector: str
     embargoed: bool
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
+    alerts: FlawCVSSPutAlerts
     comment: Union[Unset, str] = UNSET
-    score: Union[Unset, float] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        cvss_version = self.cvss_version
+        cvss_version: str = UNSET
+        if not isinstance(self.cvss_version, Unset):
+
+            cvss_version = CvssVersionEnum(self.cvss_version).value
+
         issuer: str = UNSET
         if not isinstance(self.issuer, Unset):
 
             issuer = IssuerEnum(self.issuer).value
 
+        score = self.score
         uuid = self.uuid
         vector = self.vector
         embargoed = self.embargoed
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         comment = self.comment
-        score = self.score
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if not isinstance(cvss_version, Unset):
             field_dict["cvss_version"] = cvss_version
         if not isinstance(issuer, Unset):
             field_dict["issuer"] = issuer
+        if not isinstance(score, Unset):
+            field_dict["score"] = score
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(vector, Unset):
             field_dict["vector"] = vector
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(comment, Unset):
             field_dict["comment"] = comment
-        if not isinstance(score, Unset):
-            field_dict["score"] = score
 
         return field_dict
 
     def to_multipart(self) -> Dict[str, Any]:
-        cvss_version = (
-            self.cvss_version
-            if self.cvss_version is UNSET
-            else (None, str(self.cvss_version), "text/plain")
-        )
+        cvss_version: Union[Unset, Tuple[None, str, str]] = UNSET
+        if not isinstance(self.cvss_version, Unset):
+
+            cvss_version = CvssVersionEnum(self.cvss_version).value
+
         issuer: Union[Unset, Tuple[None, str, str]] = UNSET
         if not isinstance(self.issuer, Unset):
 
             issuer = IssuerEnum(self.issuer).value
 
+        score = (
+            self.score if self.score is UNSET else (None, str(self.score), "text/plain")
+        )
         uuid = self.uuid if self.uuid is UNSET else (None, str(self.uuid), "text/plain")
         vector = (
             self.vector
             if self.vector is UNSET
             else (None, str(self.vector), "text/plain")
         )
         embargoed = (
@@ -95,63 +112,73 @@
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
+        alerts: Union[Unset, Tuple[None, str, str]] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = (None, json.dumps(self.alerts.to_dict()), "application/json")
+
         comment = (
             self.comment
             if self.comment is UNSET
             else (None, str(self.comment), "text/plain")
         )
-        score = (
-            self.score if self.score is UNSET else (None, str(self.score), "text/plain")
-        )
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(
             {
                 key: (None, str(value), "text/plain")
                 for key, value in self.additional_properties.items()
             }
         )
         if not isinstance(cvss_version, Unset):
             field_dict["cvss_version"] = cvss_version
         if not isinstance(issuer, Unset):
             field_dict["issuer"] = issuer
+        if not isinstance(score, Unset):
+            field_dict["score"] = score
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(vector, Unset):
             field_dict["vector"] = vector
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(comment, Unset):
             field_dict["comment"] = comment
-        if not isinstance(score, Unset):
-            field_dict["score"] = score
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        cvss_version = d.pop("cvss_version", UNSET)
+        _cvss_version = d.pop("cvss_version", UNSET)
+        cvss_version: CvssVersionEnum
+        if isinstance(_cvss_version, Unset):
+            cvss_version = UNSET
+        else:
+            cvss_version = CvssVersionEnum(_cvss_version)
 
         _issuer = d.pop("issuer", UNSET)
         issuer: IssuerEnum
         if isinstance(_issuer, Unset):
             issuer = UNSET
         else:
             issuer = IssuerEnum(_issuer)
 
+        score = d.pop("score", UNSET)
+
         uuid = d.pop("uuid", UNSET)
 
         vector = d.pop("vector", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
         _created_dt = d.pop("created_dt", UNSET)
@@ -164,45 +191,52 @@
         _updated_dt = d.pop("updated_dt", UNSET)
         updated_dt: datetime.datetime
         if isinstance(_updated_dt, Unset):
             updated_dt = UNSET
         else:
             updated_dt = isoparse(_updated_dt)
 
-        comment = d.pop("comment", UNSET)
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawCVSSPutAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawCVSSPutAlerts.from_dict(_alerts)
 
-        score = d.pop("score", UNSET)
+        comment = d.pop("comment", UNSET)
 
-        affect_cvss_put = cls(
+        flaw_cvss_put = cls(
             cvss_version=cvss_version,
             issuer=issuer,
+            score=score,
             uuid=uuid,
             vector=vector,
             embargoed=embargoed,
             created_dt=created_dt,
             updated_dt=updated_dt,
+            alerts=alerts,
             comment=comment,
-            score=score,
         )
 
-        affect_cvss_put.additional_properties = d
-        return affect_cvss_put
+        flaw_cvss_put.additional_properties = d
+        return flaw_cvss_put
 
     @staticmethod
     def get_fields():
         return {
-            "cvss_version": str,
+            "cvss_version": CvssVersionEnum,
             "issuer": IssuerEnum,
+            "score": float,
             "uuid": str,
             "vector": str,
             "embargoed": bool,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
+            "alerts": FlawCVSSPutAlerts,
             "comment": str,
-            "score": float,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/affect_meta_attr.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/affect_post_meta_attr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="AffectMetaAttr")
+T = TypeVar("T", bound="AffectPostMetaAttr")
 
 
 @attr.s(auto_attribs=True)
-class AffectMetaAttr(OSIDBModel):
+class AffectPostMetaAttr(OSIDBModel):
     """ """
 
     affectedness: Union[Unset, str] = UNSET
     component: Union[Unset, str] = UNSET
     cvss2: Union[Unset, str] = UNSET
     cvss3: Union[Unset, str] = UNSET
     impact: Union[Unset, str] = UNSET
     module_name: Union[Unset, str] = UNSET
     module_stream: Union[Unset, str] = UNSET
     ps_component: Union[Unset, str] = UNSET
     ps_module: Union[Unset, str] = UNSET
+    ps_product: Union[Unset, str] = UNSET
     resolution: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         affectedness = self.affectedness
         component = self.component
         cvss2 = self.cvss2
         cvss3 = self.cvss3
         impact = self.impact
         module_name = self.module_name
         module_stream = self.module_stream
         ps_component = self.ps_component
         ps_module = self.ps_module
+        ps_product = self.ps_product
         resolution = self.resolution
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if not isinstance(affectedness, Unset):
             field_dict["affectedness"] = affectedness
         if not isinstance(component, Unset):
@@ -51,14 +53,16 @@
             field_dict["module_name"] = module_name
         if not isinstance(module_stream, Unset):
             field_dict["module_stream"] = module_stream
         if not isinstance(ps_component, Unset):
             field_dict["ps_component"] = ps_component
         if not isinstance(ps_module, Unset):
             field_dict["ps_module"] = ps_module
+        if not isinstance(ps_product, Unset):
+            field_dict["ps_product"] = ps_product
         if not isinstance(resolution, Unset):
             field_dict["resolution"] = resolution
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
@@ -77,44 +81,48 @@
 
         module_stream = d.pop("module_stream", UNSET)
 
         ps_component = d.pop("ps_component", UNSET)
 
         ps_module = d.pop("ps_module", UNSET)
 
+        ps_product = d.pop("ps_product", UNSET)
+
         resolution = d.pop("resolution", UNSET)
 
-        affect_meta_attr = cls(
+        affect_post_meta_attr = cls(
             affectedness=affectedness,
             component=component,
             cvss2=cvss2,
             cvss3=cvss3,
             impact=impact,
             module_name=module_name,
             module_stream=module_stream,
             ps_component=ps_component,
             ps_module=ps_module,
+            ps_product=ps_product,
             resolution=resolution,
         )
 
-        affect_meta_attr.additional_properties = d
-        return affect_meta_attr
+        affect_post_meta_attr.additional_properties = d
+        return affect_post_meta_attr
 
     @staticmethod
     def get_fields():
         return {
             "affectedness": str,
             "component": str,
             "cvss2": str,
             "cvss3": str,
             "impact": str,
             "module_name": str,
             "module_stream": str,
             "ps_component": str,
             "ps_module": str,
+            "ps_product": str,
             "resolution": str,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/affect_post.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/affect_post.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 from typing import Any, Dict, List, Optional, Tuple, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.affect_cvss import AffectCVSS
+from ..models.affect_post_alerts import AffectPostAlerts
 from ..models.affect_post_meta_attr import AffectPostMetaAttr
 from ..models.affect_type import AffectType
 from ..models.affectedness_enum import AffectednessEnum
 from ..models.blank_enum import BlankEnum
 from ..models.impact_enum import ImpactEnum
 from ..models.resolution_enum import ResolutionEnum
 from ..models.tracker import Tracker
@@ -20,20 +21,22 @@
 
 @attr.s(auto_attribs=True)
 class AffectPost(OSIDBModel):
     """Affect serializer"""
 
     uuid: str
     ps_module: str
+    ps_product: str
     ps_component: str
     trackers: List[Tracker]
     meta_attr: AffectPostMetaAttr
     delegated_resolution: str
     cvss_scores: List[AffectCVSS]
     embargoed: bool
+    alerts: AffectPostAlerts
     created_dt: datetime.datetime
     flaw: Optional[str]
     type: Union[Unset, AffectType] = UNSET
     affectedness: Union[AffectednessEnum, BlankEnum, Unset] = UNSET
     resolution: Union[BlankEnum, ResolutionEnum, Unset] = UNSET
     impact: Union[BlankEnum, ImpactEnum, Unset] = UNSET
     cvss2: Union[Unset, str] = UNSET
@@ -41,14 +44,15 @@
     cvss3: Union[Unset, str] = UNSET
     cvss3_score: Union[Unset, None, float] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         uuid = self.uuid
         ps_module = self.ps_module
+        ps_product = self.ps_product
         ps_component = self.ps_component
         trackers: List[Dict[str, Any]] = UNSET
         if not isinstance(self.trackers, Unset):
             trackers = []
             for trackers_item_data in self.trackers:
                 trackers_item: Dict[str, Any] = UNSET
                 if not isinstance(trackers_item_data, Unset):
@@ -68,14 +72,18 @@
                 cvss_scores_item: Dict[str, Any] = UNSET
                 if not isinstance(cvss_scores_item_data, Unset):
                     cvss_scores_item = cvss_scores_item_data.to_dict()
 
                 cvss_scores.append(cvss_scores_item)
 
         embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         flaw = self.flaw
         type: Union[Unset, str] = UNSET
         if not isinstance(self.type, Unset):
@@ -134,26 +142,30 @@
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(ps_module, Unset):
             field_dict["ps_module"] = ps_module
+        if not isinstance(ps_product, Unset):
+            field_dict["ps_product"] = ps_product
         if not isinstance(ps_component, Unset):
             field_dict["ps_component"] = ps_component
         if not isinstance(trackers, Unset):
             field_dict["trackers"] = trackers
         if not isinstance(meta_attr, Unset):
             field_dict["meta_attr"] = meta_attr
         if not isinstance(delegated_resolution, Unset):
             field_dict["delegated_resolution"] = delegated_resolution
         if not isinstance(cvss_scores, Unset):
             field_dict["cvss_scores"] = cvss_scores
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(flaw, Unset):
             field_dict["flaw"] = flaw
         if not isinstance(type, Unset):
             field_dict["type"] = type
         if not isinstance(affectedness, Unset):
@@ -176,14 +188,19 @@
     def to_multipart(self) -> Dict[str, Any]:
         uuid = self.uuid if self.uuid is UNSET else (None, str(self.uuid), "text/plain")
         ps_module = (
             self.ps_module
             if self.ps_module is UNSET
             else (None, str(self.ps_module), "text/plain")
         )
+        ps_product = (
+            self.ps_product
+            if self.ps_product is UNSET
+            else (None, str(self.ps_product), "text/plain")
+        )
         ps_component = (
             self.ps_component
             if self.ps_component is UNSET
             else (None, str(self.ps_component), "text/plain")
         )
         trackers: Union[Unset, Tuple[None, str, str]] = UNSET
         if not isinstance(self.trackers, Unset):
@@ -217,14 +234,18 @@
             cvss_scores = (None, json.dumps(_temp_cvss_scores), "application/json")
 
         embargoed = (
             self.embargoed
             if self.embargoed is UNSET
             else (None, str(self.embargoed), "text/plain")
         )
+        alerts: Union[Unset, Tuple[None, str, str]] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = (None, json.dumps(self.alerts.to_dict()), "application/json")
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         flaw = self.flaw if self.flaw is UNSET else (None, str(self.flaw), "text/plain")
         type: Union[Unset, Tuple[None, str, str]] = UNSET
         if not isinstance(self.type, Unset):
@@ -300,26 +321,30 @@
                 for key, value in self.additional_properties.items()
             }
         )
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(ps_module, Unset):
             field_dict["ps_module"] = ps_module
+        if not isinstance(ps_product, Unset):
+            field_dict["ps_product"] = ps_product
         if not isinstance(ps_component, Unset):
             field_dict["ps_component"] = ps_component
         if not isinstance(trackers, Unset):
             field_dict["trackers"] = trackers
         if not isinstance(meta_attr, Unset):
             field_dict["meta_attr"] = meta_attr
         if not isinstance(delegated_resolution, Unset):
             field_dict["delegated_resolution"] = delegated_resolution
         if not isinstance(cvss_scores, Unset):
             field_dict["cvss_scores"] = cvss_scores
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(flaw, Unset):
             field_dict["flaw"] = flaw
         if not isinstance(type, Unset):
             field_dict["type"] = type
         if not isinstance(affectedness, Unset):
@@ -342,14 +367,16 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         uuid = d.pop("uuid", UNSET)
 
         ps_module = d.pop("ps_module", UNSET)
 
+        ps_product = d.pop("ps_product", UNSET)
+
         ps_component = d.pop("ps_component", UNSET)
 
         trackers = []
         _trackers = d.pop("trackers", UNSET)
         if _trackers is UNSET:
             trackers = UNSET
         else:
@@ -385,14 +412,21 @@
                 else:
                     cvss_scores_item = AffectCVSS.from_dict(_cvss_scores_item)
 
                 cvss_scores.append(cvss_scores_item)
 
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: AffectPostAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = AffectPostAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
@@ -501,20 +535,22 @@
         cvss3 = d.pop("cvss3", UNSET)
 
         cvss3_score = d.pop("cvss3_score", UNSET)
 
         affect_post = cls(
             uuid=uuid,
             ps_module=ps_module,
+            ps_product=ps_product,
             ps_component=ps_component,
             trackers=trackers,
             meta_attr=meta_attr,
             delegated_resolution=delegated_resolution,
             cvss_scores=cvss_scores,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             flaw=flaw,
             type=type,
             affectedness=affectedness,
             resolution=resolution,
             impact=impact,
             cvss2=cvss2,
@@ -527,20 +563,22 @@
         return affect_post
 
     @staticmethod
     def get_fields():
         return {
             "uuid": str,
             "ps_module": str,
+            "ps_product": str,
             "ps_component": str,
             "trackers": List[Tracker],
             "meta_attr": AffectPostMetaAttr,
             "delegated_resolution": str,
             "cvss_scores": List[AffectCVSS],
             "embargoed": bool,
+            "alerts": AffectPostAlerts,
             "created_dt": datetime.datetime,
             "flaw": str,
             "type": AffectType,
             "affectedness": Union[AffectednessEnum, BlankEnum],
             "resolution": Union[BlankEnum, ResolutionEnum],
             "impact": Union[BlankEnum, ImpactEnum],
             "cvss2": str,
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/affect_post_meta_attr.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/affect_meta_attr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="AffectPostMetaAttr")
+T = TypeVar("T", bound="AffectMetaAttr")
 
 
 @attr.s(auto_attribs=True)
-class AffectPostMetaAttr(OSIDBModel):
+class AffectMetaAttr(OSIDBModel):
     """ """
 
     affectedness: Union[Unset, str] = UNSET
     component: Union[Unset, str] = UNSET
     cvss2: Union[Unset, str] = UNSET
     cvss3: Union[Unset, str] = UNSET
     impact: Union[Unset, str] = UNSET
     module_name: Union[Unset, str] = UNSET
     module_stream: Union[Unset, str] = UNSET
     ps_component: Union[Unset, str] = UNSET
     ps_module: Union[Unset, str] = UNSET
+    ps_product: Union[Unset, str] = UNSET
     resolution: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         affectedness = self.affectedness
         component = self.component
         cvss2 = self.cvss2
         cvss3 = self.cvss3
         impact = self.impact
         module_name = self.module_name
         module_stream = self.module_stream
         ps_component = self.ps_component
         ps_module = self.ps_module
+        ps_product = self.ps_product
         resolution = self.resolution
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if not isinstance(affectedness, Unset):
             field_dict["affectedness"] = affectedness
         if not isinstance(component, Unset):
@@ -51,14 +53,16 @@
             field_dict["module_name"] = module_name
         if not isinstance(module_stream, Unset):
             field_dict["module_stream"] = module_stream
         if not isinstance(ps_component, Unset):
             field_dict["ps_component"] = ps_component
         if not isinstance(ps_module, Unset):
             field_dict["ps_module"] = ps_module
+        if not isinstance(ps_product, Unset):
+            field_dict["ps_product"] = ps_product
         if not isinstance(resolution, Unset):
             field_dict["resolution"] = resolution
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
@@ -77,44 +81,48 @@
 
         module_stream = d.pop("module_stream", UNSET)
 
         ps_component = d.pop("ps_component", UNSET)
 
         ps_module = d.pop("ps_module", UNSET)
 
+        ps_product = d.pop("ps_product", UNSET)
+
         resolution = d.pop("resolution", UNSET)
 
-        affect_post_meta_attr = cls(
+        affect_meta_attr = cls(
             affectedness=affectedness,
             component=component,
             cvss2=cvss2,
             cvss3=cvss3,
             impact=impact,
             module_name=module_name,
             module_stream=module_stream,
             ps_component=ps_component,
             ps_module=ps_module,
+            ps_product=ps_product,
             resolution=resolution,
         )
 
-        affect_post_meta_attr.additional_properties = d
-        return affect_post_meta_attr
+        affect_meta_attr.additional_properties = d
+        return affect_meta_attr
 
     @staticmethod
     def get_fields():
         return {
             "affectedness": str,
             "component": str,
             "cvss2": str,
             "cvss3": str,
             "impact": str,
             "module_name": str,
             "module_stream": str,
             "ps_component": str,
             "ps_module": str,
+            "ps_product": str,
             "resolution": str,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/affect_report_data.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/affect_report_data.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/auth_token_create_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/auth_token_create_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/auth_token_refresh_create_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/auth_token_refresh_create_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/auth_token_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/auth_token_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/auth_token_verify_create_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/auth_token_verify_create_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_error.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_error.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/collectors_healthy_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/collectors_healthy_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/collectors_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/collectors_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/comment.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/meta.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,133 +1,142 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.comment_meta_attr import CommentMetaAttr
-from ..models.flaw_comment_type import FlawCommentType
+from ..models.flaw_meta_type import FlawMetaType
+from ..models.meta_alerts import MetaAlerts
+from ..models.meta_meta_attr import MetaMetaAttr
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="Comment")
+T = TypeVar("T", bound="Meta")
 
 
 @attr.s(auto_attribs=True)
-class Comment(OSIDBModel):
-    """FlawComment serializer for use by FlawSerializer"""
+class Meta(OSIDBModel):
+    """FlawMeta serializer"""
 
     uuid: str
+    type: FlawMetaType
+    embargoed: bool
+    alerts: MetaAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
-    type: Union[Unset, FlawCommentType] = UNSET
-    external_system_id: Union[Unset, str] = UNSET
-    order: Union[Unset, None, int] = UNSET
-    meta_attr: Union[Unset, CommentMetaAttr] = UNSET
+    meta_attr: Union[Unset, MetaMetaAttr] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         uuid = self.uuid
+        type: str = UNSET
+        if not isinstance(self.type, Unset):
+
+            type = FlawMetaType(self.type).value
+
+        embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
-        type: Union[Unset, str] = UNSET
-        if not isinstance(self.type, Unset):
-
-            type = FlawCommentType(self.type).value
-
-        external_system_id = self.external_system_id
-        order = self.order
         meta_attr: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.meta_attr, Unset):
             meta_attr = self.meta_attr.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
+        if not isinstance(type, Unset):
+            field_dict["type"] = type
+        if not isinstance(embargoed, Unset):
+            field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
-        if not isinstance(type, Unset):
-            field_dict["type"] = type
-        if not isinstance(external_system_id, Unset):
-            field_dict["external_system_id"] = external_system_id
-        if not isinstance(order, Unset):
-            field_dict["order"] = order
         if not isinstance(meta_attr, Unset):
             field_dict["meta_attr"] = meta_attr
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         uuid = d.pop("uuid", UNSET)
 
+        _type = d.pop("type", UNSET)
+        type: FlawMetaType
+        if isinstance(_type, Unset):
+            type = UNSET
+        else:
+            type = FlawMetaType(_type)
+
+        embargoed = d.pop("embargoed", UNSET)
+
+        _alerts = d.pop("alerts", UNSET)
+        alerts: MetaAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = MetaAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
         _updated_dt = d.pop("updated_dt", UNSET)
         updated_dt: datetime.datetime
         if isinstance(_updated_dt, Unset):
             updated_dt = UNSET
         else:
             updated_dt = isoparse(_updated_dt)
 
-        _type = d.pop("type", UNSET)
-        type: Union[Unset, FlawCommentType]
-        if isinstance(_type, Unset):
-            type = UNSET
-        else:
-            type = FlawCommentType(_type)
-
-        external_system_id = d.pop("external_system_id", UNSET)
-
-        order = d.pop("order", UNSET)
-
         _meta_attr = d.pop("meta_attr", UNSET)
-        meta_attr: Union[Unset, CommentMetaAttr]
+        meta_attr: Union[Unset, MetaMetaAttr]
         if isinstance(_meta_attr, Unset):
             meta_attr = UNSET
         else:
-            meta_attr = CommentMetaAttr.from_dict(_meta_attr)
+            meta_attr = MetaMetaAttr.from_dict(_meta_attr)
 
-        comment = cls(
+        meta = cls(
             uuid=uuid,
+            type=type,
+            embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
-            type=type,
-            external_system_id=external_system_id,
-            order=order,
             meta_attr=meta_attr,
         )
 
-        comment.additional_properties = d
-        return comment
+        meta.additional_properties = d
+        return meta
 
     @staticmethod
     def get_fields():
         return {
             "uuid": str,
+            "type": FlawMetaType,
+            "embargoed": bool,
+            "alerts": MetaAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
-            "type": FlawCommentType,
-            "external_system_id": str,
-            "order": int,
-            "meta_attr": CommentMetaAttr,
+            "meta_attr": MetaMetaAttr,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/comment_meta_attr.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/comment_meta_attr.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/epss.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/epss.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/erratum.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/erratum.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploit_only_report_data.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploit_only_report_data.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_collect_update_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_collect_update_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200_cves.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200_cves.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_epss_list_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_epss_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_flaw_data_list_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_flaw_data_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_data_list_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_data_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_action_required_item.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_action_required_item.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_no_action_item.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_no_action_item.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_not_relevant_item.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_not_relevant_item.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200_explanations_item.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200_explanations_item.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200_pending_actions_item.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200_pending_actions_item.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_status_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_status_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_supported_products_list_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_supported_products_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import attr
 from dateutil.parser import isoparse
 
 from ..models.affect import Affect
 from ..models.blank_enum import BlankEnum
 from ..models.comment import Comment
 from ..models.flaw_acknowledgment import FlawAcknowledgment
+from ..models.flaw_alerts import FlawAlerts
 from ..models.flaw_classification import FlawClassification
 from ..models.flaw_cvss import FlawCVSS
 from ..models.flaw_meta_attr import FlawMetaAttr
 from ..models.flaw_reference import FlawReference
 from ..models.flaw_type import FlawType
 from ..models.impact_enum import ImpactEnum
 from ..models.major_incident_state_enum import MajorIncidentStateEnum
@@ -44,18 +45,20 @@
     acknowledgments: List[FlawAcknowledgment]
     references: List[FlawReference]
     cvss_scores: List[FlawCVSS]
     embargoed: bool
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     classification: FlawClassification
+    alerts: FlawAlerts
     type: Union[Unset, FlawType] = UNSET
     cve_id: Union[Unset, None, str] = UNSET
     impact: Union[BlankEnum, ImpactEnum, Unset] = UNSET
     component: Union[Unset, str] = UNSET
+    components: Union[Unset, List[str]] = UNSET
     summary: Union[Unset, str] = UNSET
     requires_summary: Union[BlankEnum, RequiresSummaryEnum, Unset] = UNSET
     statement: Union[Unset, str] = UNSET
     cwe_id: Union[Unset, str] = UNSET
     unembargo_dt: Union[Unset, None, datetime.datetime] = UNSET
     source: Union[BlankEnum, Source8D8Enum, Unset] = UNSET
     reported_dt: Union[Unset, None, datetime.datetime] = UNSET
@@ -168,14 +171,18 @@
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
         classification: Dict[str, Any] = UNSET
         if not isinstance(self.classification, Unset):
             classification = self.classification.to_dict()
 
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         type: Union[Unset, str] = UNSET
         if not isinstance(self.type, Unset):
 
             type = FlawType(self.type).value
 
         cve_id = self.cve_id
         impact: Union[Unset, str]
@@ -190,14 +197,18 @@
         else:
             impact = UNSET
             if not isinstance(self.impact, Unset):
 
                 impact = BlankEnum(self.impact).value
 
         component = self.component
+        components: Union[Unset, List[str]] = UNSET
+        if not isinstance(self.components, Unset):
+            components = self.components
+
         summary = self.summary
         requires_summary: Union[Unset, str]
         if isinstance(self.requires_summary, Unset):
             requires_summary = UNSET
         elif isinstance(self.requires_summary, RequiresSummaryEnum):
             requires_summary = UNSET
             if not isinstance(self.requires_summary, Unset):
@@ -316,22 +327,26 @@
             field_dict["embargoed"] = embargoed
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(classification, Unset):
             field_dict["classification"] = classification
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(type, Unset):
             field_dict["type"] = type
         if not isinstance(cve_id, Unset):
             field_dict["cve_id"] = cve_id
         if not isinstance(impact, Unset):
             field_dict["impact"] = impact
         if not isinstance(component, Unset):
             field_dict["component"] = component
+        if not isinstance(components, Unset):
+            field_dict["components"] = components
         if not isinstance(summary, Unset):
             field_dict["summary"] = summary
         if not isinstance(requires_summary, Unset):
             field_dict["requires_summary"] = requires_summary
         if not isinstance(statement, Unset):
             field_dict["statement"] = statement
         if not isinstance(cwe_id, Unset):
@@ -502,14 +517,18 @@
         if not isinstance(self.classification, Unset):
             classification = (
                 None,
                 json.dumps(self.classification.to_dict()),
                 "application/json",
             )
 
+        alerts: Union[Unset, Tuple[None, str, str]] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = (None, json.dumps(self.alerts.to_dict()), "application/json")
+
         type: Union[Unset, Tuple[None, str, str]] = UNSET
         if not isinstance(self.type, Unset):
 
             type = FlawType(self.type).value
 
         cve_id = (
             self.cve_id
@@ -532,14 +551,19 @@
                 impact = BlankEnum(self.impact).value
 
         component = (
             self.component
             if self.component is UNSET
             else (None, str(self.component), "text/plain")
         )
+        components: Union[Unset, Tuple[None, str, str]] = UNSET
+        if not isinstance(self.components, Unset):
+            _temp_components = self.components
+            components = (None, json.dumps(_temp_components), "application/json")
+
         summary = (
             self.summary
             if self.summary is UNSET
             else (None, str(self.summary), "text/plain")
         )
         requires_summary: Union[Unset, str]
         if isinstance(self.requires_summary, Unset):
@@ -717,22 +741,26 @@
             field_dict["embargoed"] = embargoed
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(classification, Unset):
             field_dict["classification"] = classification
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(type, Unset):
             field_dict["type"] = type
         if not isinstance(cve_id, Unset):
             field_dict["cve_id"] = cve_id
         if not isinstance(impact, Unset):
             field_dict["impact"] = impact
         if not isinstance(component, Unset):
             field_dict["component"] = component
+        if not isinstance(components, Unset):
+            field_dict["components"] = components
         if not isinstance(summary, Unset):
             field_dict["summary"] = summary
         if not isinstance(requires_summary, Unset):
             field_dict["requires_summary"] = requires_summary
         if not isinstance(statement, Unset):
             field_dict["statement"] = statement
         if not isinstance(cwe_id, Unset):
@@ -922,14 +950,21 @@
         _classification = d.pop("classification", UNSET)
         classification: FlawClassification
         if isinstance(_classification, Unset):
             classification = UNSET
         else:
             classification = FlawClassification.from_dict(_classification)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawAlerts.from_dict(_alerts)
+
         _type = d.pop("type", UNSET)
         type: Union[Unset, FlawType]
         if isinstance(_type, Unset):
             type = UNSET
         else:
             type = FlawType(_type)
 
@@ -962,14 +997,16 @@
 
             return impact_type_1
 
         impact = _parse_impact(d.pop("impact", UNSET))
 
         component = d.pop("component", UNSET)
 
+        components = cast(List[str], d.pop("components", UNSET))
+
         summary = d.pop("summary", UNSET)
 
         def _parse_requires_summary(
             data: object,
         ) -> Union[BlankEnum, RequiresSummaryEnum, Unset]:
             if isinstance(data, Unset):
                 return data
@@ -1161,18 +1198,20 @@
             acknowledgments=acknowledgments,
             references=references,
             cvss_scores=cvss_scores,
             embargoed=embargoed,
             created_dt=created_dt,
             updated_dt=updated_dt,
             classification=classification,
+            alerts=alerts,
             type=type,
             cve_id=cve_id,
             impact=impact,
             component=component,
+            components=components,
             summary=summary,
             requires_summary=requires_summary,
             statement=statement,
             cwe_id=cwe_id,
             unembargo_dt=unembargo_dt,
             source=source,
             reported_dt=reported_dt,
@@ -1212,18 +1251,20 @@
             "acknowledgments": List[FlawAcknowledgment],
             "references": List[FlawReference],
             "cvss_scores": List[FlawCVSS],
             "embargoed": bool,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "classification": FlawClassification,
+            "alerts": FlawAlerts,
             "type": FlawType,
             "cve_id": str,
             "impact": Union[BlankEnum, ImpactEnum],
             "component": str,
+            "components": List[str],
             "summary": str,
             "requires_summary": Union[BlankEnum, RequiresSummaryEnum],
             "statement": str,
             "cwe_id": str,
             "unembargo_dt": datetime.datetime,
             "source": Union[BlankEnum, Source8D8Enum],
             "reported_dt": datetime.datetime,
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_acknowledgment.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_acknowledgment.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.flaw_acknowledgment_alerts import FlawAcknowledgmentAlerts
 from ..types import UNSET, OSIDBModel, Unset
 
 T = TypeVar("T", bound="FlawAcknowledgment")
 
 
 @attr.s(auto_attribs=True)
 class FlawAcknowledgment(OSIDBModel):
@@ -15,25 +16,30 @@
 
     name: str
     affiliation: str
     from_upstream: bool
     flaw: str
     uuid: str
     embargoed: bool
+    alerts: FlawAcknowledgmentAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         name = self.name
         affiliation = self.affiliation
         from_upstream = self.from_upstream
         flaw = self.flaw
         uuid = self.uuid
         embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
@@ -48,14 +54,16 @@
             field_dict["from_upstream"] = from_upstream
         if not isinstance(flaw, Unset):
             field_dict["flaw"] = flaw
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
 
         return field_dict
 
@@ -70,14 +78,21 @@
 
         flaw = d.pop("flaw", UNSET)
 
         uuid = d.pop("uuid", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawAcknowledgmentAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawAcknowledgmentAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
@@ -91,14 +106,15 @@
         flaw_acknowledgment = cls(
             name=name,
             affiliation=affiliation,
             from_upstream=from_upstream,
             flaw=flaw,
             uuid=uuid,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
         )
 
         flaw_acknowledgment.additional_properties = d
         return flaw_acknowledgment
 
@@ -107,14 +123,15 @@
         return {
             "name": str,
             "affiliation": str,
             "from_upstream": bool,
             "flaw": str,
             "uuid": str,
             "embargoed": bool,
+            "alerts": FlawAcknowledgmentAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_acknowledgment_post.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_acknowledgment_post.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar
+import json
+from typing import Any, Dict, List, Tuple, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.flaw_acknowledgment_post_alerts import FlawAcknowledgmentPostAlerts
 from ..types import UNSET, OSIDBModel, Unset
 
 T = TypeVar("T", bound="FlawAcknowledgmentPost")
 
 
 @attr.s(auto_attribs=True)
 class FlawAcknowledgmentPost(OSIDBModel):
     """FlawAcknowledgment serializer"""
 
     name: str
     affiliation: str
     from_upstream: bool
     uuid: str
     embargoed: bool
+    alerts: FlawAcknowledgmentPostAlerts
     created_dt: datetime.datetime
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         name = self.name
         affiliation = self.affiliation
         from_upstream = self.from_upstream
         uuid = self.uuid
         embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if not isinstance(name, Unset):
@@ -39,14 +46,16 @@
             field_dict["affiliation"] = affiliation
         if not isinstance(from_upstream, Unset):
             field_dict["from_upstream"] = from_upstream
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
 
         return field_dict
 
     def to_multipart(self) -> Dict[str, Any]:
         name = self.name if self.name is UNSET else (None, str(self.name), "text/plain")
@@ -62,14 +71,18 @@
         )
         uuid = self.uuid if self.uuid is UNSET else (None, str(self.uuid), "text/plain")
         embargoed = (
             self.embargoed
             if self.embargoed is UNSET
             else (None, str(self.embargoed), "text/plain")
         )
+        alerts: Union[Unset, Tuple[None, str, str]] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = (None, json.dumps(self.alerts.to_dict()), "application/json")
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(
             {
@@ -83,14 +96,16 @@
             field_dict["affiliation"] = affiliation
         if not isinstance(from_upstream, Unset):
             field_dict["from_upstream"] = from_upstream
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
@@ -101,41 +116,50 @@
 
         from_upstream = d.pop("from_upstream", UNSET)
 
         uuid = d.pop("uuid", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawAcknowledgmentPostAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawAcknowledgmentPostAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
         flaw_acknowledgment_post = cls(
             name=name,
             affiliation=affiliation,
             from_upstream=from_upstream,
             uuid=uuid,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
         )
 
         flaw_acknowledgment_post.additional_properties = d
         return flaw_acknowledgment_post
 
     @staticmethod
     def get_fields():
         return {
             "name": str,
             "affiliation": str,
             "from_upstream": bool,
             "uuid": str,
             "embargoed": bool,
+            "alerts": FlawAcknowledgmentPostAlerts,
             "created_dt": datetime.datetime,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_acknowledgment_put.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_acknowledgments_retrieve_response_200.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,164 +1,182 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.flaw_acknowledgment_alerts import FlawAcknowledgmentAlerts
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="FlawAcknowledgmentPut")
+T = TypeVar("T", bound="OsidbApiV1FlawsAcknowledgmentsRetrieveResponse200")
 
 
 @attr.s(auto_attribs=True)
-class FlawAcknowledgmentPut(OSIDBModel):
-    """FlawAcknowledgment serializer"""
+class OsidbApiV1FlawsAcknowledgmentsRetrieveResponse200(OSIDBModel):
+    """ """
 
     name: str
     affiliation: str
     from_upstream: bool
+    flaw: str
     uuid: str
     embargoed: bool
+    alerts: FlawAcknowledgmentAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
+    dt: Union[Unset, datetime.datetime] = UNSET
+    env: Union[Unset, str] = UNSET
+    revision: Union[Unset, str] = UNSET
+    version: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         name = self.name
         affiliation = self.affiliation
         from_upstream = self.from_upstream
+        flaw = self.flaw
         uuid = self.uuid
         embargoed = self.embargoed
-        created_dt: str = UNSET
-        if not isinstance(self.created_dt, Unset):
-            created_dt = self.created_dt.isoformat()
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
 
-        updated_dt: str = UNSET
-        if not isinstance(self.updated_dt, Unset):
-            updated_dt = self.updated_dt.isoformat()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        if not isinstance(name, Unset):
-            field_dict["name"] = name
-        if not isinstance(affiliation, Unset):
-            field_dict["affiliation"] = affiliation
-        if not isinstance(from_upstream, Unset):
-            field_dict["from_upstream"] = from_upstream
-        if not isinstance(uuid, Unset):
-            field_dict["uuid"] = uuid
-        if not isinstance(embargoed, Unset):
-            field_dict["embargoed"] = embargoed
-        if not isinstance(created_dt, Unset):
-            field_dict["created_dt"] = created_dt
-        if not isinstance(updated_dt, Unset):
-            field_dict["updated_dt"] = updated_dt
-
-        return field_dict
-
-    def to_multipart(self) -> Dict[str, Any]:
-        name = self.name if self.name is UNSET else (None, str(self.name), "text/plain")
-        affiliation = (
-            self.affiliation
-            if self.affiliation is UNSET
-            else (None, str(self.affiliation), "text/plain")
-        )
-        from_upstream = (
-            self.from_upstream
-            if self.from_upstream is UNSET
-            else (None, str(self.from_upstream), "text/plain")
-        )
-        uuid = self.uuid if self.uuid is UNSET else (None, str(self.uuid), "text/plain")
-        embargoed = (
-            self.embargoed
-            if self.embargoed is UNSET
-            else (None, str(self.embargoed), "text/plain")
-        )
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
+        dt: Union[Unset, str] = UNSET
+        if not isinstance(self.dt, Unset):
+            dt = self.dt.isoformat()
+
+        env = self.env
+        revision = self.revision
+        version = self.version
+
         field_dict: Dict[str, Any] = {}
-        field_dict.update(
-            {
-                key: (None, str(value), "text/plain")
-                for key, value in self.additional_properties.items()
-            }
-        )
+        field_dict.update(self.additional_properties)
         if not isinstance(name, Unset):
             field_dict["name"] = name
         if not isinstance(affiliation, Unset):
             field_dict["affiliation"] = affiliation
         if not isinstance(from_upstream, Unset):
             field_dict["from_upstream"] = from_upstream
+        if not isinstance(flaw, Unset):
+            field_dict["flaw"] = flaw
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
+        if not isinstance(dt, Unset):
+            field_dict["dt"] = dt
+        if not isinstance(env, Unset):
+            field_dict["env"] = env
+        if not isinstance(revision, Unset):
+            field_dict["revision"] = revision
+        if not isinstance(version, Unset):
+            field_dict["version"] = version
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name", UNSET)
 
         affiliation = d.pop("affiliation", UNSET)
 
         from_upstream = d.pop("from_upstream", UNSET)
 
+        flaw = d.pop("flaw", UNSET)
+
         uuid = d.pop("uuid", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawAcknowledgmentAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawAcknowledgmentAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
         _updated_dt = d.pop("updated_dt", UNSET)
         updated_dt: datetime.datetime
         if isinstance(_updated_dt, Unset):
             updated_dt = UNSET
         else:
             updated_dt = isoparse(_updated_dt)
 
-        flaw_acknowledgment_put = cls(
+        _dt = d.pop("dt", UNSET)
+        dt: Union[Unset, datetime.datetime]
+        if isinstance(_dt, Unset):
+            dt = UNSET
+        else:
+            dt = isoparse(_dt)
+
+        env = d.pop("env", UNSET)
+
+        revision = d.pop("revision", UNSET)
+
+        version = d.pop("version", UNSET)
+
+        osidb_api_v1_flaws_acknowledgments_retrieve_response_200 = cls(
             name=name,
             affiliation=affiliation,
             from_upstream=from_upstream,
+            flaw=flaw,
             uuid=uuid,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
+            dt=dt,
+            env=env,
+            revision=revision,
+            version=version,
         )
 
-        flaw_acknowledgment_put.additional_properties = d
-        return flaw_acknowledgment_put
+        osidb_api_v1_flaws_acknowledgments_retrieve_response_200.additional_properties = (
+            d
+        )
+        return osidb_api_v1_flaws_acknowledgments_retrieve_response_200
 
     @staticmethod
     def get_fields():
         return {
             "name": str,
             "affiliation": str,
             "from_upstream": bool,
+            "flaw": str,
             "uuid": str,
             "embargoed": bool,
+            "alerts": FlawAcknowledgmentAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
+            "dt": datetime.datetime,
+            "env": str,
+            "revision": str,
+            "version": str,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_classification.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_classification.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_comment.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_package_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,88 +1,99 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.flaw_comment_type import FlawCommentType
+from ..models.flaw_version import FlawVersion
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="FlawComment")
+T = TypeVar("T", bound="FlawPackageVersion")
 
 
 @attr.s(auto_attribs=True)
-class FlawComment(OSIDBModel):
-    """FlawComment serializer for use by flaw_comments endpoint"""
+class FlawPackageVersion(OSIDBModel):
+    """Package model serializer"""
 
+    package: str
+    versions: List[FlawVersion]
     flaw: str
-    text: str
     uuid: str
-    external_system_id: str
+    embargoed: bool
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
-    embargoed: bool
-    type: Union[Unset, FlawCommentType] = UNSET
-    order: Union[Unset, None, int] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        package = self.package
+        versions: List[Dict[str, Any]] = UNSET
+        if not isinstance(self.versions, Unset):
+            versions = []
+            for versions_item_data in self.versions:
+                versions_item: Dict[str, Any] = UNSET
+                if not isinstance(versions_item_data, Unset):
+                    versions_item = versions_item_data.to_dict()
+
+                versions.append(versions_item)
+
         flaw = self.flaw
-        text = self.text
         uuid = self.uuid
-        external_system_id = self.external_system_id
+        embargoed = self.embargoed
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
-        embargoed = self.embargoed
-        type: Union[Unset, str] = UNSET
-        if not isinstance(self.type, Unset):
-
-            type = FlawCommentType(self.type).value
-
-        order = self.order
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
+        if not isinstance(package, Unset):
+            field_dict["package"] = package
+        if not isinstance(versions, Unset):
+            field_dict["versions"] = versions
         if not isinstance(flaw, Unset):
             field_dict["flaw"] = flaw
-        if not isinstance(text, Unset):
-            field_dict["text"] = text
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
-        if not isinstance(external_system_id, Unset):
-            field_dict["external_system_id"] = external_system_id
+        if not isinstance(embargoed, Unset):
+            field_dict["embargoed"] = embargoed
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
-        if not isinstance(embargoed, Unset):
-            field_dict["embargoed"] = embargoed
-        if not isinstance(type, Unset):
-            field_dict["type"] = type
-        if not isinstance(order, Unset):
-            field_dict["order"] = order
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        flaw = d.pop("flaw", UNSET)
+        package = d.pop("package", UNSET)
 
-        text = d.pop("text", UNSET)
+        versions = []
+        _versions = d.pop("versions", UNSET)
+        if _versions is UNSET:
+            versions = UNSET
+        else:
+            for versions_item_data in _versions or []:
+                _versions_item = versions_item_data
+                versions_item: FlawVersion
+                if isinstance(_versions_item, Unset):
+                    versions_item = UNSET
+                else:
+                    versions_item = FlawVersion.from_dict(_versions_item)
+
+                versions.append(versions_item)
+
+        flaw = d.pop("flaw", UNSET)
 
         uuid = d.pop("uuid", UNSET)
 
-        external_system_id = d.pop("external_system_id", UNSET)
+        embargoed = d.pop("embargoed", UNSET)
 
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
@@ -90,52 +101,37 @@
         _updated_dt = d.pop("updated_dt", UNSET)
         updated_dt: datetime.datetime
         if isinstance(_updated_dt, Unset):
             updated_dt = UNSET
         else:
             updated_dt = isoparse(_updated_dt)
 
-        embargoed = d.pop("embargoed", UNSET)
-
-        _type = d.pop("type", UNSET)
-        type: Union[Unset, FlawCommentType]
-        if isinstance(_type, Unset):
-            type = UNSET
-        else:
-            type = FlawCommentType(_type)
-
-        order = d.pop("order", UNSET)
-
-        flaw_comment = cls(
+        flaw_package_version = cls(
+            package=package,
+            versions=versions,
             flaw=flaw,
-            text=text,
             uuid=uuid,
-            external_system_id=external_system_id,
+            embargoed=embargoed,
             created_dt=created_dt,
             updated_dt=updated_dt,
-            embargoed=embargoed,
-            type=type,
-            order=order,
         )
 
-        flaw_comment.additional_properties = d
-        return flaw_comment
+        flaw_package_version.additional_properties = d
+        return flaw_package_version
 
     @staticmethod
     def get_fields():
         return {
+            "package": str,
+            "versions": List[FlawVersion],
             "flaw": str,
-            "text": str,
             "uuid": str,
-            "external_system_id": str,
+            "embargoed": bool,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
-            "embargoed": bool,
-            "type": FlawCommentType,
-            "order": int,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_comment_post.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_comment.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,161 +1,158 @@
 import datetime
-import json
-from typing import Any, Dict, List, Tuple, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.flaw_comment_post_meta_attr import FlawCommentPostMetaAttr
+from ..models.flaw_comment_alerts import FlawCommentAlerts
 from ..models.flaw_comment_type import FlawCommentType
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="FlawCommentPost")
+T = TypeVar("T", bound="FlawComment")
 
 
 @attr.s(auto_attribs=True)
-class FlawCommentPost(OSIDBModel):
+class FlawComment(OSIDBModel):
     """FlawComment serializer for use by flaw_comments endpoint"""
 
+    flaw: str
     text: str
     uuid: str
+    external_system_id: str
+    alerts: FlawCommentAlerts
     created_dt: datetime.datetime
+    updated_dt: datetime.datetime
     embargoed: bool
     type: Union[Unset, FlawCommentType] = UNSET
-    meta_attr: Union[Unset, FlawCommentPostMetaAttr] = UNSET
+    order: Union[Unset, None, int] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        flaw = self.flaw
         text = self.text
         uuid = self.uuid
+        external_system_id = self.external_system_id
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
+        updated_dt: str = UNSET
+        if not isinstance(self.updated_dt, Unset):
+            updated_dt = self.updated_dt.isoformat()
+
         embargoed = self.embargoed
         type: Union[Unset, str] = UNSET
         if not isinstance(self.type, Unset):
 
             type = FlawCommentType(self.type).value
 
-        meta_attr: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.meta_attr, Unset):
-            meta_attr = self.meta_attr.to_dict()
+        order = self.order
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
+        if not isinstance(flaw, Unset):
+            field_dict["flaw"] = flaw
         if not isinstance(text, Unset):
             field_dict["text"] = text
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
+        if not isinstance(external_system_id, Unset):
+            field_dict["external_system_id"] = external_system_id
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
+        if not isinstance(updated_dt, Unset):
+            field_dict["updated_dt"] = updated_dt
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
         if not isinstance(type, Unset):
             field_dict["type"] = type
-        if not isinstance(meta_attr, Unset):
-            field_dict["meta_attr"] = meta_attr
-
-        return field_dict
-
-    def to_multipart(self) -> Dict[str, Any]:
-        text = self.text if self.text is UNSET else (None, str(self.text), "text/plain")
-        uuid = self.uuid if self.uuid is UNSET else (None, str(self.uuid), "text/plain")
-        created_dt: str = UNSET
-        if not isinstance(self.created_dt, Unset):
-            created_dt = self.created_dt.isoformat()
-
-        embargoed = (
-            self.embargoed
-            if self.embargoed is UNSET
-            else (None, str(self.embargoed), "text/plain")
-        )
-        type: Union[Unset, Tuple[None, str, str]] = UNSET
-        if not isinstance(self.type, Unset):
-
-            type = FlawCommentType(self.type).value
-
-        meta_attr: Union[Unset, Tuple[None, str, str]] = UNSET
-        if not isinstance(self.meta_attr, Unset):
-            meta_attr = (None, json.dumps(self.meta_attr.to_dict()), "application/json")
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(
-            {
-                key: (None, str(value), "text/plain")
-                for key, value in self.additional_properties.items()
-            }
-        )
-        if not isinstance(text, Unset):
-            field_dict["text"] = text
-        if not isinstance(uuid, Unset):
-            field_dict["uuid"] = uuid
-        if not isinstance(created_dt, Unset):
-            field_dict["created_dt"] = created_dt
-        if not isinstance(embargoed, Unset):
-            field_dict["embargoed"] = embargoed
-        if not isinstance(type, Unset):
-            field_dict["type"] = type
-        if not isinstance(meta_attr, Unset):
-            field_dict["meta_attr"] = meta_attr
+        if not isinstance(order, Unset):
+            field_dict["order"] = order
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
+        flaw = d.pop("flaw", UNSET)
+
         text = d.pop("text", UNSET)
 
         uuid = d.pop("uuid", UNSET)
 
+        external_system_id = d.pop("external_system_id", UNSET)
+
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawCommentAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawCommentAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
+        _updated_dt = d.pop("updated_dt", UNSET)
+        updated_dt: datetime.datetime
+        if isinstance(_updated_dt, Unset):
+            updated_dt = UNSET
+        else:
+            updated_dt = isoparse(_updated_dt)
+
         embargoed = d.pop("embargoed", UNSET)
 
         _type = d.pop("type", UNSET)
         type: Union[Unset, FlawCommentType]
         if isinstance(_type, Unset):
             type = UNSET
         else:
             type = FlawCommentType(_type)
 
-        _meta_attr = d.pop("meta_attr", UNSET)
-        meta_attr: Union[Unset, FlawCommentPostMetaAttr]
-        if isinstance(_meta_attr, Unset):
-            meta_attr = UNSET
-        else:
-            meta_attr = FlawCommentPostMetaAttr.from_dict(_meta_attr)
+        order = d.pop("order", UNSET)
 
-        flaw_comment_post = cls(
+        flaw_comment = cls(
+            flaw=flaw,
             text=text,
             uuid=uuid,
+            external_system_id=external_system_id,
+            alerts=alerts,
             created_dt=created_dt,
+            updated_dt=updated_dt,
             embargoed=embargoed,
             type=type,
-            meta_attr=meta_attr,
+            order=order,
         )
 
-        flaw_comment_post.additional_properties = d
-        return flaw_comment_post
+        flaw_comment.additional_properties = d
+        return flaw_comment
 
     @staticmethod
     def get_fields():
         return {
+            "flaw": str,
             "text": str,
             "uuid": str,
+            "external_system_id": str,
+            "alerts": FlawCommentAlerts,
             "created_dt": datetime.datetime,
+            "updated_dt": datetime.datetime,
             "embargoed": bool,
             "type": FlawCommentType,
-            "meta_attr": FlawCommentPostMetaAttr,
+            "order": int,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_comment_post_meta_attr.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_comment_post_meta_attr.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_cvss.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/comment.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,92 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.issuer_enum import IssuerEnum
+from ..models.comment_alerts import CommentAlerts
+from ..models.comment_meta_attr import CommentMetaAttr
+from ..models.flaw_comment_type import FlawCommentType
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="FlawCVSS")
+T = TypeVar("T", bound="Comment")
 
 
 @attr.s(auto_attribs=True)
-class FlawCVSS(OSIDBModel):
-    """FlawCVSS serializer"""
+class Comment(OSIDBModel):
+    """FlawComment serializer for use by FlawSerializer"""
 
-    cvss_version: str
-    issuer: IssuerEnum
     uuid: str
-    vector: str
-    embargoed: bool
+    alerts: CommentAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
-    comment: Union[Unset, str] = UNSET
-    flaw: Union[Unset, str] = UNSET
-    score: Union[Unset, float] = UNSET
+    type: Union[Unset, FlawCommentType] = UNSET
+    external_system_id: Union[Unset, str] = UNSET
+    order: Union[Unset, None, int] = UNSET
+    meta_attr: Union[Unset, CommentMetaAttr] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        cvss_version = self.cvss_version
-        issuer: str = UNSET
-        if not isinstance(self.issuer, Unset):
-
-            issuer = IssuerEnum(self.issuer).value
-
         uuid = self.uuid
-        vector = self.vector
-        embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
-        comment = self.comment
-        flaw = self.flaw
-        score = self.score
+        type: Union[Unset, str] = UNSET
+        if not isinstance(self.type, Unset):
+
+            type = FlawCommentType(self.type).value
+
+        external_system_id = self.external_system_id
+        order = self.order
+        meta_attr: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.meta_attr, Unset):
+            meta_attr = self.meta_attr.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        if not isinstance(cvss_version, Unset):
-            field_dict["cvss_version"] = cvss_version
-        if not isinstance(issuer, Unset):
-            field_dict["issuer"] = issuer
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
-        if not isinstance(vector, Unset):
-            field_dict["vector"] = vector
-        if not isinstance(embargoed, Unset):
-            field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
-        if not isinstance(comment, Unset):
-            field_dict["comment"] = comment
-        if not isinstance(flaw, Unset):
-            field_dict["flaw"] = flaw
-        if not isinstance(score, Unset):
-            field_dict["score"] = score
+        if not isinstance(type, Unset):
+            field_dict["type"] = type
+        if not isinstance(external_system_id, Unset):
+            field_dict["external_system_id"] = external_system_id
+        if not isinstance(order, Unset):
+            field_dict["order"] = order
+        if not isinstance(meta_attr, Unset):
+            field_dict["meta_attr"] = meta_attr
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        cvss_version = d.pop("cvss_version", UNSET)
-
-        _issuer = d.pop("issuer", UNSET)
-        issuer: IssuerEnum
-        if isinstance(_issuer, Unset):
-            issuer = UNSET
-        else:
-            issuer = IssuerEnum(_issuer)
-
         uuid = d.pop("uuid", UNSET)
 
-        vector = d.pop("vector", UNSET)
-
-        embargoed = d.pop("embargoed", UNSET)
+        _alerts = d.pop("alerts", UNSET)
+        alerts: CommentAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = CommentAlerts.from_dict(_alerts)
 
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
@@ -101,49 +94,57 @@
         _updated_dt = d.pop("updated_dt", UNSET)
         updated_dt: datetime.datetime
         if isinstance(_updated_dt, Unset):
             updated_dt = UNSET
         else:
             updated_dt = isoparse(_updated_dt)
 
-        comment = d.pop("comment", UNSET)
+        _type = d.pop("type", UNSET)
+        type: Union[Unset, FlawCommentType]
+        if isinstance(_type, Unset):
+            type = UNSET
+        else:
+            type = FlawCommentType(_type)
+
+        external_system_id = d.pop("external_system_id", UNSET)
 
-        flaw = d.pop("flaw", UNSET)
+        order = d.pop("order", UNSET)
 
-        score = d.pop("score", UNSET)
+        _meta_attr = d.pop("meta_attr", UNSET)
+        meta_attr: Union[Unset, CommentMetaAttr]
+        if isinstance(_meta_attr, Unset):
+            meta_attr = UNSET
+        else:
+            meta_attr = CommentMetaAttr.from_dict(_meta_attr)
 
-        flaw_cvss = cls(
-            cvss_version=cvss_version,
-            issuer=issuer,
+        comment = cls(
             uuid=uuid,
-            vector=vector,
-            embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
-            comment=comment,
-            flaw=flaw,
-            score=score,
+            type=type,
+            external_system_id=external_system_id,
+            order=order,
+            meta_attr=meta_attr,
         )
 
-        flaw_cvss.additional_properties = d
-        return flaw_cvss
+        comment.additional_properties = d
+        return comment
 
     @staticmethod
     def get_fields():
         return {
-            "cvss_version": str,
-            "issuer": IssuerEnum,
             "uuid": str,
-            "vector": str,
-            "embargoed": bool,
+            "alerts": CommentAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
-            "comment": str,
-            "flaw": str,
-            "score": float,
+            "type": FlawCommentType,
+            "external_system_id": str,
+            "order": int,
+            "meta_attr": CommentMetaAttr,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_cvss_post.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_cvss_post.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,99 @@
 import datetime
+import json
 from typing import Any, Dict, List, Tuple, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.cvss_version_enum import CvssVersionEnum
+from ..models.flaw_cvss_post_alerts import FlawCVSSPostAlerts
 from ..models.issuer_enum import IssuerEnum
 from ..types import UNSET, OSIDBModel, Unset
 
 T = TypeVar("T", bound="FlawCVSSPost")
 
 
 @attr.s(auto_attribs=True)
 class FlawCVSSPost(OSIDBModel):
     """FlawCVSS serializer"""
 
-    cvss_version: str
+    cvss_version: CvssVersionEnum
     issuer: IssuerEnum
+    score: float
     uuid: str
     vector: str
     embargoed: bool
     created_dt: datetime.datetime
+    alerts: FlawCVSSPostAlerts
     comment: Union[Unset, str] = UNSET
-    score: Union[Unset, float] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        cvss_version = self.cvss_version
+        cvss_version: str = UNSET
+        if not isinstance(self.cvss_version, Unset):
+
+            cvss_version = CvssVersionEnum(self.cvss_version).value
+
         issuer: str = UNSET
         if not isinstance(self.issuer, Unset):
 
             issuer = IssuerEnum(self.issuer).value
 
+        score = self.score
         uuid = self.uuid
         vector = self.vector
         embargoed = self.embargoed
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         comment = self.comment
-        score = self.score
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if not isinstance(cvss_version, Unset):
             field_dict["cvss_version"] = cvss_version
         if not isinstance(issuer, Unset):
             field_dict["issuer"] = issuer
+        if not isinstance(score, Unset):
+            field_dict["score"] = score
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(vector, Unset):
             field_dict["vector"] = vector
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(comment, Unset):
             field_dict["comment"] = comment
-        if not isinstance(score, Unset):
-            field_dict["score"] = score
 
         return field_dict
 
     def to_multipart(self) -> Dict[str, Any]:
-        cvss_version = (
-            self.cvss_version
-            if self.cvss_version is UNSET
-            else (None, str(self.cvss_version), "text/plain")
-        )
+        cvss_version: Union[Unset, Tuple[None, str, str]] = UNSET
+        if not isinstance(self.cvss_version, Unset):
+
+            cvss_version = CvssVersionEnum(self.cvss_version).value
+
         issuer: Union[Unset, Tuple[None, str, str]] = UNSET
         if not isinstance(self.issuer, Unset):
 
             issuer = IssuerEnum(self.issuer).value
 
+        score = (
+            self.score if self.score is UNSET else (None, str(self.score), "text/plain")
+        )
         uuid = self.uuid if self.uuid is UNSET else (None, str(self.uuid), "text/plain")
         vector = (
             self.vector
             if self.vector is UNSET
             else (None, str(self.vector), "text/plain")
         )
         embargoed = (
@@ -84,103 +101,120 @@
             if self.embargoed is UNSET
             else (None, str(self.embargoed), "text/plain")
         )
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
+        alerts: Union[Unset, Tuple[None, str, str]] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = (None, json.dumps(self.alerts.to_dict()), "application/json")
+
         comment = (
             self.comment
             if self.comment is UNSET
             else (None, str(self.comment), "text/plain")
         )
-        score = (
-            self.score if self.score is UNSET else (None, str(self.score), "text/plain")
-        )
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(
             {
                 key: (None, str(value), "text/plain")
                 for key, value in self.additional_properties.items()
             }
         )
         if not isinstance(cvss_version, Unset):
             field_dict["cvss_version"] = cvss_version
         if not isinstance(issuer, Unset):
             field_dict["issuer"] = issuer
+        if not isinstance(score, Unset):
+            field_dict["score"] = score
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(vector, Unset):
             field_dict["vector"] = vector
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(comment, Unset):
             field_dict["comment"] = comment
-        if not isinstance(score, Unset):
-            field_dict["score"] = score
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        cvss_version = d.pop("cvss_version", UNSET)
+        _cvss_version = d.pop("cvss_version", UNSET)
+        cvss_version: CvssVersionEnum
+        if isinstance(_cvss_version, Unset):
+            cvss_version = UNSET
+        else:
+            cvss_version = CvssVersionEnum(_cvss_version)
 
         _issuer = d.pop("issuer", UNSET)
         issuer: IssuerEnum
         if isinstance(_issuer, Unset):
             issuer = UNSET
         else:
             issuer = IssuerEnum(_issuer)
 
+        score = d.pop("score", UNSET)
+
         uuid = d.pop("uuid", UNSET)
 
         vector = d.pop("vector", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
-        comment = d.pop("comment", UNSET)
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawCVSSPostAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawCVSSPostAlerts.from_dict(_alerts)
 
-        score = d.pop("score", UNSET)
+        comment = d.pop("comment", UNSET)
 
         flaw_cvss_post = cls(
             cvss_version=cvss_version,
             issuer=issuer,
+            score=score,
             uuid=uuid,
             vector=vector,
             embargoed=embargoed,
             created_dt=created_dt,
+            alerts=alerts,
             comment=comment,
-            score=score,
         )
 
         flaw_cvss_post.additional_properties = d
         return flaw_cvss_post
 
     @staticmethod
     def get_fields():
         return {
-            "cvss_version": str,
+            "cvss_version": CvssVersionEnum,
             "issuer": IssuerEnum,
+            "score": float,
             "uuid": str,
             "vector": str,
             "embargoed": bool,
             "created_dt": datetime.datetime,
+            "alerts": FlawCVSSPostAlerts,
             "comment": str,
-            "score": float,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_cvss_put.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/affect_cvss_put.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,163 +1,197 @@
 import datetime
+import json
 from typing import Any, Dict, List, Tuple, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.affect_cvss_put_alerts import AffectCVSSPutAlerts
+from ..models.cvss_version_enum import CvssVersionEnum
 from ..models.issuer_enum import IssuerEnum
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="FlawCVSSPut")
+T = TypeVar("T", bound="AffectCVSSPut")
 
 
 @attr.s(auto_attribs=True)
-class FlawCVSSPut(OSIDBModel):
-    """FlawCVSS serializer"""
+class AffectCVSSPut(OSIDBModel):
+    """AffectCVSS serializer"""
 
-    cvss_version: str
+    cvss_version: CvssVersionEnum
     issuer: IssuerEnum
+    score: float
     uuid: str
     vector: str
     embargoed: bool
+    alerts: AffectCVSSPutAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     comment: Union[Unset, str] = UNSET
-    score: Union[Unset, float] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        cvss_version = self.cvss_version
+        cvss_version: str = UNSET
+        if not isinstance(self.cvss_version, Unset):
+
+            cvss_version = CvssVersionEnum(self.cvss_version).value
+
         issuer: str = UNSET
         if not isinstance(self.issuer, Unset):
 
             issuer = IssuerEnum(self.issuer).value
 
+        score = self.score
         uuid = self.uuid
         vector = self.vector
         embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
         comment = self.comment
-        score = self.score
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if not isinstance(cvss_version, Unset):
             field_dict["cvss_version"] = cvss_version
         if not isinstance(issuer, Unset):
             field_dict["issuer"] = issuer
+        if not isinstance(score, Unset):
+            field_dict["score"] = score
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(vector, Unset):
             field_dict["vector"] = vector
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(comment, Unset):
             field_dict["comment"] = comment
-        if not isinstance(score, Unset):
-            field_dict["score"] = score
 
         return field_dict
 
     def to_multipart(self) -> Dict[str, Any]:
-        cvss_version = (
-            self.cvss_version
-            if self.cvss_version is UNSET
-            else (None, str(self.cvss_version), "text/plain")
-        )
+        cvss_version: Union[Unset, Tuple[None, str, str]] = UNSET
+        if not isinstance(self.cvss_version, Unset):
+
+            cvss_version = CvssVersionEnum(self.cvss_version).value
+
         issuer: Union[Unset, Tuple[None, str, str]] = UNSET
         if not isinstance(self.issuer, Unset):
 
             issuer = IssuerEnum(self.issuer).value
 
+        score = (
+            self.score if self.score is UNSET else (None, str(self.score), "text/plain")
+        )
         uuid = self.uuid if self.uuid is UNSET else (None, str(self.uuid), "text/plain")
         vector = (
             self.vector
             if self.vector is UNSET
             else (None, str(self.vector), "text/plain")
         )
         embargoed = (
             self.embargoed
             if self.embargoed is UNSET
             else (None, str(self.embargoed), "text/plain")
         )
+        alerts: Union[Unset, Tuple[None, str, str]] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = (None, json.dumps(self.alerts.to_dict()), "application/json")
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
         comment = (
             self.comment
             if self.comment is UNSET
             else (None, str(self.comment), "text/plain")
         )
-        score = (
-            self.score if self.score is UNSET else (None, str(self.score), "text/plain")
-        )
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(
             {
                 key: (None, str(value), "text/plain")
                 for key, value in self.additional_properties.items()
             }
         )
         if not isinstance(cvss_version, Unset):
             field_dict["cvss_version"] = cvss_version
         if not isinstance(issuer, Unset):
             field_dict["issuer"] = issuer
+        if not isinstance(score, Unset):
+            field_dict["score"] = score
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(vector, Unset):
             field_dict["vector"] = vector
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(comment, Unset):
             field_dict["comment"] = comment
-        if not isinstance(score, Unset):
-            field_dict["score"] = score
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        cvss_version = d.pop("cvss_version", UNSET)
+        _cvss_version = d.pop("cvss_version", UNSET)
+        cvss_version: CvssVersionEnum
+        if isinstance(_cvss_version, Unset):
+            cvss_version = UNSET
+        else:
+            cvss_version = CvssVersionEnum(_cvss_version)
 
         _issuer = d.pop("issuer", UNSET)
         issuer: IssuerEnum
         if isinstance(_issuer, Unset):
             issuer = UNSET
         else:
             issuer = IssuerEnum(_issuer)
 
+        score = d.pop("score", UNSET)
+
         uuid = d.pop("uuid", UNSET)
 
         vector = d.pop("vector", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: AffectCVSSPutAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = AffectCVSSPutAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
@@ -166,43 +200,43 @@
         if isinstance(_updated_dt, Unset):
             updated_dt = UNSET
         else:
             updated_dt = isoparse(_updated_dt)
 
         comment = d.pop("comment", UNSET)
 
-        score = d.pop("score", UNSET)
-
-        flaw_cvss_put = cls(
+        affect_cvss_put = cls(
             cvss_version=cvss_version,
             issuer=issuer,
+            score=score,
             uuid=uuid,
             vector=vector,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
             comment=comment,
-            score=score,
         )
 
-        flaw_cvss_put.additional_properties = d
-        return flaw_cvss_put
+        affect_cvss_put.additional_properties = d
+        return affect_cvss_put
 
     @staticmethod
     def get_fields():
         return {
-            "cvss_version": str,
+            "cvss_version": CvssVersionEnum,
             "issuer": IssuerEnum,
+            "score": float,
             "uuid": str,
             "vector": str,
             "embargoed": bool,
+            "alerts": AffectCVSSPutAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "comment": str,
-            "score": float,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_meta_attr.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_meta_attr.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_package_version.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_package_versions_retrieve_response_200.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.flaw_version import FlawVersion
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="FlawPackageVersion")
+T = TypeVar("T", bound="OsidbApiV1FlawsPackageVersionsRetrieveResponse200")
 
 
 @attr.s(auto_attribs=True)
-class FlawPackageVersion(OSIDBModel):
-    """Package model serializer"""
+class OsidbApiV1FlawsPackageVersionsRetrieveResponse200(OSIDBModel):
+    """ """
 
     package: str
     versions: List[FlawVersion]
     flaw: str
     uuid: str
     embargoed: bool
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
+    dt: Union[Unset, datetime.datetime] = UNSET
+    env: Union[Unset, str] = UNSET
+    revision: Union[Unset, str] = UNSET
+    version: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         package = self.package
         versions: List[Dict[str, Any]] = UNSET
         if not isinstance(self.versions, Unset):
             versions = []
@@ -42,14 +46,22 @@
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
+        dt: Union[Unset, str] = UNSET
+        if not isinstance(self.dt, Unset):
+            dt = self.dt.isoformat()
+
+        env = self.env
+        revision = self.revision
+        version = self.version
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if not isinstance(package, Unset):
             field_dict["package"] = package
         if not isinstance(versions, Unset):
             field_dict["versions"] = versions
         if not isinstance(flaw, Unset):
@@ -58,14 +70,22 @@
             field_dict["uuid"] = uuid
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
+        if not isinstance(dt, Unset):
+            field_dict["dt"] = dt
+        if not isinstance(env, Unset):
+            field_dict["env"] = env
+        if not isinstance(revision, Unset):
+            field_dict["revision"] = revision
+        if not isinstance(version, Unset):
+            field_dict["version"] = version
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         package = d.pop("package", UNSET)
@@ -101,37 +121,60 @@
         _updated_dt = d.pop("updated_dt", UNSET)
         updated_dt: datetime.datetime
         if isinstance(_updated_dt, Unset):
             updated_dt = UNSET
         else:
             updated_dt = isoparse(_updated_dt)
 
-        flaw_package_version = cls(
+        _dt = d.pop("dt", UNSET)
+        dt: Union[Unset, datetime.datetime]
+        if isinstance(_dt, Unset):
+            dt = UNSET
+        else:
+            dt = isoparse(_dt)
+
+        env = d.pop("env", UNSET)
+
+        revision = d.pop("revision", UNSET)
+
+        version = d.pop("version", UNSET)
+
+        osidb_api_v1_flaws_package_versions_retrieve_response_200 = cls(
             package=package,
             versions=versions,
             flaw=flaw,
             uuid=uuid,
             embargoed=embargoed,
             created_dt=created_dt,
             updated_dt=updated_dt,
+            dt=dt,
+            env=env,
+            revision=revision,
+            version=version,
         )
 
-        flaw_package_version.additional_properties = d
-        return flaw_package_version
+        osidb_api_v1_flaws_package_versions_retrieve_response_200.additional_properties = (
+            d
+        )
+        return osidb_api_v1_flaws_package_versions_retrieve_response_200
 
     @staticmethod
     def get_fields():
         return {
             "package": str,
             "versions": List[FlawVersion],
             "flaw": str,
             "uuid": str,
             "embargoed": bool,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
+            "dt": datetime.datetime,
+            "env": str,
+            "revision": str,
+            "version": str,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_package_version_post.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_package_version_post.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_package_version_put.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_package_version_put.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_post.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_post.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from dateutil.parser import isoparse
 
 from ..models.affect import Affect
 from ..models.blank_enum import BlankEnum
 from ..models.comment import Comment
 from ..models.flaw_acknowledgment import FlawAcknowledgment
 from ..models.flaw_cvss import FlawCVSS
+from ..models.flaw_post_alerts import FlawPostAlerts
 from ..models.flaw_post_classification import FlawPostClassification
 from ..models.flaw_post_meta_attr import FlawPostMetaAttr
 from ..models.flaw_reference import FlawReference
 from ..models.flaw_type import FlawType
 from ..models.impact_enum import ImpactEnum
 from ..models.major_incident_state_enum import MajorIncidentStateEnum
 from ..models.meta import Meta
@@ -43,18 +44,20 @@
     package_versions: List[Package]
     acknowledgments: List[FlawAcknowledgment]
     references: List[FlawReference]
     cvss_scores: List[FlawCVSS]
     embargoed: bool
     created_dt: datetime.datetime
     classification: FlawPostClassification
+    alerts: FlawPostAlerts
     type: Union[Unset, FlawType] = UNSET
     cve_id: Union[Unset, None, str] = UNSET
     impact: Union[BlankEnum, ImpactEnum, Unset] = UNSET
     component: Union[Unset, str] = UNSET
+    components: Union[Unset, List[str]] = UNSET
     summary: Union[Unset, str] = UNSET
     requires_summary: Union[BlankEnum, RequiresSummaryEnum, Unset] = UNSET
     statement: Union[Unset, str] = UNSET
     cwe_id: Union[Unset, str] = UNSET
     unembargo_dt: Union[Unset, None, datetime.datetime] = UNSET
     source: Union[BlankEnum, Source8D8Enum, Unset] = UNSET
     reported_dt: Union[Unset, None, datetime.datetime] = UNSET
@@ -163,14 +166,18 @@
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         classification: Dict[str, Any] = UNSET
         if not isinstance(self.classification, Unset):
             classification = self.classification.to_dict()
 
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         type: Union[Unset, str] = UNSET
         if not isinstance(self.type, Unset):
 
             type = FlawType(self.type).value
 
         cve_id = self.cve_id
         impact: Union[Unset, str]
@@ -185,14 +192,18 @@
         else:
             impact = UNSET
             if not isinstance(self.impact, Unset):
 
                 impact = BlankEnum(self.impact).value
 
         component = self.component
+        components: Union[Unset, List[str]] = UNSET
+        if not isinstance(self.components, Unset):
+            components = self.components
+
         summary = self.summary
         requires_summary: Union[Unset, str]
         if isinstance(self.requires_summary, Unset):
             requires_summary = UNSET
         elif isinstance(self.requires_summary, RequiresSummaryEnum):
             requires_summary = UNSET
             if not isinstance(self.requires_summary, Unset):
@@ -309,22 +320,26 @@
             field_dict["cvss_scores"] = cvss_scores
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(classification, Unset):
             field_dict["classification"] = classification
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(type, Unset):
             field_dict["type"] = type
         if not isinstance(cve_id, Unset):
             field_dict["cve_id"] = cve_id
         if not isinstance(impact, Unset):
             field_dict["impact"] = impact
         if not isinstance(component, Unset):
             field_dict["component"] = component
+        if not isinstance(components, Unset):
+            field_dict["components"] = components
         if not isinstance(summary, Unset):
             field_dict["summary"] = summary
         if not isinstance(requires_summary, Unset):
             field_dict["requires_summary"] = requires_summary
         if not isinstance(statement, Unset):
             field_dict["statement"] = statement
         if not isinstance(cwe_id, Unset):
@@ -491,14 +506,18 @@
         if not isinstance(self.classification, Unset):
             classification = (
                 None,
                 json.dumps(self.classification.to_dict()),
                 "application/json",
             )
 
+        alerts: Union[Unset, Tuple[None, str, str]] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = (None, json.dumps(self.alerts.to_dict()), "application/json")
+
         type: Union[Unset, Tuple[None, str, str]] = UNSET
         if not isinstance(self.type, Unset):
 
             type = FlawType(self.type).value
 
         cve_id = (
             self.cve_id
@@ -521,14 +540,19 @@
                 impact = BlankEnum(self.impact).value
 
         component = (
             self.component
             if self.component is UNSET
             else (None, str(self.component), "text/plain")
         )
+        components: Union[Unset, Tuple[None, str, str]] = UNSET
+        if not isinstance(self.components, Unset):
+            _temp_components = self.components
+            components = (None, json.dumps(_temp_components), "application/json")
+
         summary = (
             self.summary
             if self.summary is UNSET
             else (None, str(self.summary), "text/plain")
         )
         requires_summary: Union[Unset, str]
         if isinstance(self.requires_summary, Unset):
@@ -704,22 +728,26 @@
             field_dict["cvss_scores"] = cvss_scores
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(classification, Unset):
             field_dict["classification"] = classification
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(type, Unset):
             field_dict["type"] = type
         if not isinstance(cve_id, Unset):
             field_dict["cve_id"] = cve_id
         if not isinstance(impact, Unset):
             field_dict["impact"] = impact
         if not isinstance(component, Unset):
             field_dict["component"] = component
+        if not isinstance(components, Unset):
+            field_dict["components"] = components
         if not isinstance(summary, Unset):
             field_dict["summary"] = summary
         if not isinstance(requires_summary, Unset):
             field_dict["requires_summary"] = requires_summary
         if not isinstance(statement, Unset):
             field_dict["statement"] = statement
         if not isinstance(cwe_id, Unset):
@@ -902,14 +930,21 @@
         _classification = d.pop("classification", UNSET)
         classification: FlawPostClassification
         if isinstance(_classification, Unset):
             classification = UNSET
         else:
             classification = FlawPostClassification.from_dict(_classification)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawPostAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawPostAlerts.from_dict(_alerts)
+
         _type = d.pop("type", UNSET)
         type: Union[Unset, FlawType]
         if isinstance(_type, Unset):
             type = UNSET
         else:
             type = FlawType(_type)
 
@@ -942,14 +977,16 @@
 
             return impact_type_1
 
         impact = _parse_impact(d.pop("impact", UNSET))
 
         component = d.pop("component", UNSET)
 
+        components = cast(List[str], d.pop("components", UNSET))
+
         summary = d.pop("summary", UNSET)
 
         def _parse_requires_summary(
             data: object,
         ) -> Union[BlankEnum, RequiresSummaryEnum, Unset]:
             if isinstance(data, Unset):
                 return data
@@ -1140,18 +1177,20 @@
             package_versions=package_versions,
             acknowledgments=acknowledgments,
             references=references,
             cvss_scores=cvss_scores,
             embargoed=embargoed,
             created_dt=created_dt,
             classification=classification,
+            alerts=alerts,
             type=type,
             cve_id=cve_id,
             impact=impact,
             component=component,
+            components=components,
             summary=summary,
             requires_summary=requires_summary,
             statement=statement,
             cwe_id=cwe_id,
             unembargo_dt=unembargo_dt,
             source=source,
             reported_dt=reported_dt,
@@ -1190,18 +1229,20 @@
             "package_versions": List[Package],
             "acknowledgments": List[FlawAcknowledgment],
             "references": List[FlawReference],
             "cvss_scores": List[FlawCVSS],
             "embargoed": bool,
             "created_dt": datetime.datetime,
             "classification": FlawPostClassification,
+            "alerts": FlawPostAlerts,
             "type": FlawType,
             "cve_id": str,
             "impact": Union[BlankEnum, ImpactEnum],
             "component": str,
+            "components": List[str],
             "summary": str,
             "requires_summary": Union[BlankEnum, RequiresSummaryEnum],
             "statement": str,
             "cwe_id": str,
             "unembargo_dt": datetime.datetime,
             "source": Union[BlankEnum, Source8D8Enum],
             "reported_dt": datetime.datetime,
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_post_classification.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_post_classification.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_post_meta_attr.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_post_meta_attr.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_reference.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_reference.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.flaw_reference_alerts import FlawReferenceAlerts
 from ..models.flaw_reference_type import FlawReferenceType
 from ..types import UNSET, OSIDBModel, Unset
 
 T = TypeVar("T", bound="FlawReference")
 
 
 @attr.s(auto_attribs=True)
 class FlawReference(OSIDBModel):
     """FlawReference serializer"""
 
     flaw: str
     url: str
     uuid: str
     embargoed: bool
+    alerts: FlawReferenceAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     description: Union[Unset, str] = UNSET
     type: Union[Unset, FlawReferenceType] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         flaw = self.flaw
         url = self.url
         uuid = self.uuid
         embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
@@ -49,14 +55,16 @@
             field_dict["flaw"] = flaw
         if not isinstance(url, Unset):
             field_dict["url"] = url
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(description, Unset):
             field_dict["description"] = description
         if not isinstance(type, Unset):
@@ -71,14 +79,21 @@
 
         url = d.pop("url", UNSET)
 
         uuid = d.pop("uuid", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawReferenceAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawReferenceAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
@@ -99,14 +114,15 @@
             type = FlawReferenceType(_type)
 
         flaw_reference = cls(
             flaw=flaw,
             url=url,
             uuid=uuid,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
             description=description,
             type=type,
         )
 
         flaw_reference.additional_properties = d
@@ -115,14 +131,15 @@
     @staticmethod
     def get_fields():
         return {
             "flaw": str,
             "url": str,
             "uuid": str,
             "embargoed": bool,
+            "alerts": FlawReferenceAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "description": str,
             "type": FlawReferenceType,
         }
 
     @property
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_reference_post.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_reference_post.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 import datetime
+import json
 from typing import Any, Dict, List, Tuple, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.flaw_reference_post_alerts import FlawReferencePostAlerts
 from ..models.flaw_reference_type import FlawReferenceType
 from ..types import UNSET, OSIDBModel, Unset
 
 T = TypeVar("T", bound="FlawReferencePost")
 
 
 @attr.s(auto_attribs=True)
 class FlawReferencePost(OSIDBModel):
     """FlawReference serializer"""
 
     url: str
     uuid: str
     embargoed: bool
+    alerts: FlawReferencePostAlerts
     created_dt: datetime.datetime
     description: Union[Unset, str] = UNSET
     type: Union[Unset, FlawReferenceType] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         url = self.url
         uuid = self.uuid
         embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         description = self.description
         type: Union[Unset, str] = UNSET
         if not isinstance(self.type, Unset):
@@ -40,14 +47,16 @@
         field_dict.update(self.additional_properties)
         if not isinstance(url, Unset):
             field_dict["url"] = url
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(description, Unset):
             field_dict["description"] = description
         if not isinstance(type, Unset):
             field_dict["type"] = type
 
@@ -57,14 +66,18 @@
         url = self.url if self.url is UNSET else (None, str(self.url), "text/plain")
         uuid = self.uuid if self.uuid is UNSET else (None, str(self.uuid), "text/plain")
         embargoed = (
             self.embargoed
             if self.embargoed is UNSET
             else (None, str(self.embargoed), "text/plain")
         )
+        alerts: Union[Unset, Tuple[None, str, str]] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = (None, json.dumps(self.alerts.to_dict()), "application/json")
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         description = (
             self.description
             if self.description is UNSET
@@ -84,14 +97,16 @@
         )
         if not isinstance(url, Unset):
             field_dict["url"] = url
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(description, Unset):
             field_dict["description"] = description
         if not isinstance(type, Unset):
             field_dict["type"] = type
 
@@ -102,14 +117,21 @@
         d = src_dict.copy()
         url = d.pop("url", UNSET)
 
         uuid = d.pop("uuid", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawReferencePostAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawReferencePostAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
@@ -122,28 +144,30 @@
         else:
             type = FlawReferenceType(_type)
 
         flaw_reference_post = cls(
             url=url,
             uuid=uuid,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             description=description,
             type=type,
         )
 
         flaw_reference_post.additional_properties = d
         return flaw_reference_post
 
     @staticmethod
     def get_fields():
         return {
             "url": str,
             "uuid": str,
             "embargoed": bool,
+            "alerts": FlawReferencePostAlerts,
             "created_dt": datetime.datetime,
             "description": str,
             "type": FlawReferenceType,
         }
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_reference_put.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_package_versions_create_response_201.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,123 +1,115 @@
 import datetime
-from typing import Any, Dict, List, Tuple, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.flaw_reference_type import FlawReferenceType
+from ..models.flaw_version import FlawVersion
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="FlawReferencePut")
+T = TypeVar("T", bound="OsidbApiV1FlawsPackageVersionsCreateResponse201")
 
 
 @attr.s(auto_attribs=True)
-class FlawReferencePut(OSIDBModel):
-    """FlawReference serializer"""
+class OsidbApiV1FlawsPackageVersionsCreateResponse201(OSIDBModel):
+    """ """
 
-    url: str
+    package: str
+    versions: List[FlawVersion]
+    flaw: str
     uuid: str
     embargoed: bool
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
-    description: Union[Unset, str] = UNSET
-    type: Union[Unset, FlawReferenceType] = UNSET
+    dt: Union[Unset, datetime.datetime] = UNSET
+    env: Union[Unset, str] = UNSET
+    revision: Union[Unset, str] = UNSET
+    version: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        url = self.url
+        package = self.package
+        versions: List[Dict[str, Any]] = UNSET
+        if not isinstance(self.versions, Unset):
+            versions = []
+            for versions_item_data in self.versions:
+                versions_item: Dict[str, Any] = UNSET
+                if not isinstance(versions_item_data, Unset):
+                    versions_item = versions_item_data.to_dict()
+
+                versions.append(versions_item)
+
+        flaw = self.flaw
         uuid = self.uuid
         embargoed = self.embargoed
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
-        description = self.description
-        type: Union[Unset, str] = UNSET
-        if not isinstance(self.type, Unset):
-
-            type = FlawReferenceType(self.type).value
+        dt: Union[Unset, str] = UNSET
+        if not isinstance(self.dt, Unset):
+            dt = self.dt.isoformat()
+
+        env = self.env
+        revision = self.revision
+        version = self.version
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        if not isinstance(url, Unset):
-            field_dict["url"] = url
+        if not isinstance(package, Unset):
+            field_dict["package"] = package
+        if not isinstance(versions, Unset):
+            field_dict["versions"] = versions
+        if not isinstance(flaw, Unset):
+            field_dict["flaw"] = flaw
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
-        if not isinstance(description, Unset):
-            field_dict["description"] = description
-        if not isinstance(type, Unset):
-            field_dict["type"] = type
-
-        return field_dict
-
-    def to_multipart(self) -> Dict[str, Any]:
-        url = self.url if self.url is UNSET else (None, str(self.url), "text/plain")
-        uuid = self.uuid if self.uuid is UNSET else (None, str(self.uuid), "text/plain")
-        embargoed = (
-            self.embargoed
-            if self.embargoed is UNSET
-            else (None, str(self.embargoed), "text/plain")
-        )
-        created_dt: str = UNSET
-        if not isinstance(self.created_dt, Unset):
-            created_dt = self.created_dt.isoformat()
-
-        updated_dt: str = UNSET
-        if not isinstance(self.updated_dt, Unset):
-            updated_dt = self.updated_dt.isoformat()
-
-        description = (
-            self.description
-            if self.description is UNSET
-            else (None, str(self.description), "text/plain")
-        )
-        type: Union[Unset, Tuple[None, str, str]] = UNSET
-        if not isinstance(self.type, Unset):
-
-            type = FlawReferenceType(self.type).value
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(
-            {
-                key: (None, str(value), "text/plain")
-                for key, value in self.additional_properties.items()
-            }
-        )
-        if not isinstance(url, Unset):
-            field_dict["url"] = url
-        if not isinstance(uuid, Unset):
-            field_dict["uuid"] = uuid
-        if not isinstance(embargoed, Unset):
-            field_dict["embargoed"] = embargoed
-        if not isinstance(created_dt, Unset):
-            field_dict["created_dt"] = created_dt
-        if not isinstance(updated_dt, Unset):
-            field_dict["updated_dt"] = updated_dt
-        if not isinstance(description, Unset):
-            field_dict["description"] = description
-        if not isinstance(type, Unset):
-            field_dict["type"] = type
+        if not isinstance(dt, Unset):
+            field_dict["dt"] = dt
+        if not isinstance(env, Unset):
+            field_dict["env"] = env
+        if not isinstance(revision, Unset):
+            field_dict["revision"] = revision
+        if not isinstance(version, Unset):
+            field_dict["version"] = version
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        url = d.pop("url", UNSET)
+        package = d.pop("package", UNSET)
+
+        versions = []
+        _versions = d.pop("versions", UNSET)
+        if _versions is UNSET:
+            versions = UNSET
+        else:
+            for versions_item_data in _versions or []:
+                _versions_item = versions_item_data
+                versions_item: FlawVersion
+                if isinstance(_versions_item, Unset):
+                    versions_item = UNSET
+                else:
+                    versions_item = FlawVersion.from_dict(_versions_item)
+
+                versions.append(versions_item)
+
+        flaw = d.pop("flaw", UNSET)
 
         uuid = d.pop("uuid", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
@@ -129,46 +121,60 @@
         _updated_dt = d.pop("updated_dt", UNSET)
         updated_dt: datetime.datetime
         if isinstance(_updated_dt, Unset):
             updated_dt = UNSET
         else:
             updated_dt = isoparse(_updated_dt)
 
-        description = d.pop("description", UNSET)
-
-        _type = d.pop("type", UNSET)
-        type: Union[Unset, FlawReferenceType]
-        if isinstance(_type, Unset):
-            type = UNSET
+        _dt = d.pop("dt", UNSET)
+        dt: Union[Unset, datetime.datetime]
+        if isinstance(_dt, Unset):
+            dt = UNSET
         else:
-            type = FlawReferenceType(_type)
+            dt = isoparse(_dt)
 
-        flaw_reference_put = cls(
-            url=url,
+        env = d.pop("env", UNSET)
+
+        revision = d.pop("revision", UNSET)
+
+        version = d.pop("version", UNSET)
+
+        osidb_api_v1_flaws_package_versions_create_response_201 = cls(
+            package=package,
+            versions=versions,
+            flaw=flaw,
             uuid=uuid,
             embargoed=embargoed,
             created_dt=created_dt,
             updated_dt=updated_dt,
-            description=description,
-            type=type,
+            dt=dt,
+            env=env,
+            revision=revision,
+            version=version,
         )
 
-        flaw_reference_put.additional_properties = d
-        return flaw_reference_put
+        osidb_api_v1_flaws_package_versions_create_response_201.additional_properties = (
+            d
+        )
+        return osidb_api_v1_flaws_package_versions_create_response_201
 
     @staticmethod
     def get_fields():
         return {
-            "url": str,
+            "package": str,
+            "versions": List[FlawVersion],
+            "flaw": str,
             "uuid": str,
             "embargoed": bool,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
-            "description": str,
-            "type": FlawReferenceType,
+            "dt": datetime.datetime,
+            "env": str,
+            "revision": str,
+            "version": str,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_report_data.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_report_data.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_uuid_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_uuid_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/flaw_version.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_version.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/meta.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/token_obtain_pair.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,125 +1,113 @@
-import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
-from dateutil.parser import isoparse
 
-from ..models.flaw_meta_type import FlawMetaType
-from ..models.meta_meta_attr import MetaMetaAttr
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="Meta")
+T = TypeVar("T", bound="TokenObtainPair")
 
 
 @attr.s(auto_attribs=True)
-class Meta(OSIDBModel):
-    """FlawMeta serializer"""
+class TokenObtainPair(OSIDBModel):
+    """ """
 
-    uuid: str
-    type: FlawMetaType
-    embargoed: bool
-    created_dt: datetime.datetime
-    updated_dt: datetime.datetime
-    meta_attr: Union[Unset, MetaMetaAttr] = UNSET
+    username: str
+    password: str
+    access: str
+    refresh: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        uuid = self.uuid
-        type: str = UNSET
-        if not isinstance(self.type, Unset):
-
-            type = FlawMetaType(self.type).value
-
-        embargoed = self.embargoed
-        created_dt: str = UNSET
-        if not isinstance(self.created_dt, Unset):
-            created_dt = self.created_dt.isoformat()
-
-        updated_dt: str = UNSET
-        if not isinstance(self.updated_dt, Unset):
-            updated_dt = self.updated_dt.isoformat()
-
-        meta_attr: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.meta_attr, Unset):
-            meta_attr = self.meta_attr.to_dict()
+        username = self.username
+        password = self.password
+        access = self.access
+        refresh = self.refresh
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        if not isinstance(uuid, Unset):
-            field_dict["uuid"] = uuid
-        if not isinstance(type, Unset):
-            field_dict["type"] = type
-        if not isinstance(embargoed, Unset):
-            field_dict["embargoed"] = embargoed
-        if not isinstance(created_dt, Unset):
-            field_dict["created_dt"] = created_dt
-        if not isinstance(updated_dt, Unset):
-            field_dict["updated_dt"] = updated_dt
-        if not isinstance(meta_attr, Unset):
-            field_dict["meta_attr"] = meta_attr
+        if not isinstance(username, Unset):
+            field_dict["username"] = username
+        if not isinstance(password, Unset):
+            field_dict["password"] = password
+        if not isinstance(access, Unset):
+            field_dict["access"] = access
+        if not isinstance(refresh, Unset):
+            field_dict["refresh"] = refresh
+
+        return field_dict
+
+    def to_multipart(self) -> Dict[str, Any]:
+        username = (
+            self.username
+            if self.username is UNSET
+            else (None, str(self.username), "text/plain")
+        )
+        password = (
+            self.password
+            if self.password is UNSET
+            else (None, str(self.password), "text/plain")
+        )
+        access = (
+            self.access
+            if self.access is UNSET
+            else (None, str(self.access), "text/plain")
+        )
+        refresh = (
+            self.refresh
+            if self.refresh is UNSET
+            else (None, str(self.refresh), "text/plain")
+        )
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(
+            {
+                key: (None, str(value), "text/plain")
+                for key, value in self.additional_properties.items()
+            }
+        )
+        if not isinstance(username, Unset):
+            field_dict["username"] = username
+        if not isinstance(password, Unset):
+            field_dict["password"] = password
+        if not isinstance(access, Unset):
+            field_dict["access"] = access
+        if not isinstance(refresh, Unset):
+            field_dict["refresh"] = refresh
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        uuid = d.pop("uuid", UNSET)
+        username = d.pop("username", UNSET)
+
+        password = d.pop("password", UNSET)
+
+        access = d.pop("access", UNSET)
+
+        refresh = d.pop("refresh", UNSET)
 
-        _type = d.pop("type", UNSET)
-        type: FlawMetaType
-        if isinstance(_type, Unset):
-            type = UNSET
-        else:
-            type = FlawMetaType(_type)
-
-        embargoed = d.pop("embargoed", UNSET)
-
-        _created_dt = d.pop("created_dt", UNSET)
-        created_dt: datetime.datetime
-        if isinstance(_created_dt, Unset):
-            created_dt = UNSET
-        else:
-            created_dt = isoparse(_created_dt)
-
-        _updated_dt = d.pop("updated_dt", UNSET)
-        updated_dt: datetime.datetime
-        if isinstance(_updated_dt, Unset):
-            updated_dt = UNSET
-        else:
-            updated_dt = isoparse(_updated_dt)
-
-        _meta_attr = d.pop("meta_attr", UNSET)
-        meta_attr: Union[Unset, MetaMetaAttr]
-        if isinstance(_meta_attr, Unset):
-            meta_attr = UNSET
-        else:
-            meta_attr = MetaMetaAttr.from_dict(_meta_attr)
-
-        meta = cls(
-            uuid=uuid,
-            type=type,
-            embargoed=embargoed,
-            created_dt=created_dt,
-            updated_dt=updated_dt,
-            meta_attr=meta_attr,
+        token_obtain_pair = cls(
+            username=username,
+            password=password,
+            access=access,
+            refresh=refresh,
         )
 
-        meta.additional_properties = d
-        return meta
+        token_obtain_pair.additional_properties = d
+        return token_obtain_pair
 
     @staticmethod
     def get_fields():
         return {
-            "uuid": str,
-            "type": FlawMetaType,
-            "embargoed": bool,
-            "created_dt": datetime.datetime,
-            "updated_dt": datetime.datetime,
-            "meta_attr": MetaMetaAttr,
+            "username": str,
+            "password": str,
+            "access": str,
+            "refresh": str,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/meta_meta_attr.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/meta_meta_attr.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/module_component.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/module_component.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_create_response_201.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_update_response_200.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import datetime
 from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.affect_alerts import AffectAlerts
 from ..models.affect_cvss import AffectCVSS
 from ..models.affect_meta_attr import AffectMetaAttr
 from ..models.affect_type import AffectType
 from ..models.affectedness_enum import AffectednessEnum
 from ..models.blank_enum import BlankEnum
 from ..models.impact_enum import ImpactEnum
 from ..models.resolution_enum import ResolutionEnum
 from ..models.tracker import Tracker
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="OsidbApiV1AffectsCreateResponse201")
+T = TypeVar("T", bound="OsidbApiV1AffectsUpdateResponse200")
 
 
 @attr.s(auto_attribs=True)
-class OsidbApiV1AffectsCreateResponse201(OSIDBModel):
+class OsidbApiV1AffectsUpdateResponse200(OSIDBModel):
     """ """
 
     uuid: str
     ps_module: str
+    ps_product: str
     ps_component: str
     trackers: List[Tracker]
     meta_attr: AffectMetaAttr
     delegated_resolution: str
     cvss_scores: List[AffectCVSS]
     embargoed: bool
+    alerts: AffectAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     flaw: Optional[str]
     type: Union[Unset, AffectType] = UNSET
     affectedness: Union[AffectednessEnum, BlankEnum, Unset] = UNSET
     resolution: Union[BlankEnum, ResolutionEnum, Unset] = UNSET
     impact: Union[BlankEnum, ImpactEnum, Unset] = UNSET
@@ -45,14 +48,15 @@
     revision: Union[Unset, str] = UNSET
     version: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         uuid = self.uuid
         ps_module = self.ps_module
+        ps_product = self.ps_product
         ps_component = self.ps_component
         trackers: List[Dict[str, Any]] = UNSET
         if not isinstance(self.trackers, Unset):
             trackers = []
             for trackers_item_data in self.trackers:
                 trackers_item: Dict[str, Any] = UNSET
                 if not isinstance(trackers_item_data, Unset):
@@ -72,14 +76,18 @@
                 cvss_scores_item: Dict[str, Any] = UNSET
                 if not isinstance(cvss_scores_item_data, Unset):
                     cvss_scores_item = cvss_scores_item_data.to_dict()
 
                 cvss_scores.append(cvss_scores_item)
 
         embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
@@ -149,26 +157,30 @@
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(ps_module, Unset):
             field_dict["ps_module"] = ps_module
+        if not isinstance(ps_product, Unset):
+            field_dict["ps_product"] = ps_product
         if not isinstance(ps_component, Unset):
             field_dict["ps_component"] = ps_component
         if not isinstance(trackers, Unset):
             field_dict["trackers"] = trackers
         if not isinstance(meta_attr, Unset):
             field_dict["meta_attr"] = meta_attr
         if not isinstance(delegated_resolution, Unset):
             field_dict["delegated_resolution"] = delegated_resolution
         if not isinstance(cvss_scores, Unset):
             field_dict["cvss_scores"] = cvss_scores
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(flaw, Unset):
             field_dict["flaw"] = flaw
         if not isinstance(type, Unset):
@@ -201,14 +213,16 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         uuid = d.pop("uuid", UNSET)
 
         ps_module = d.pop("ps_module", UNSET)
 
+        ps_product = d.pop("ps_product", UNSET)
+
         ps_component = d.pop("ps_component", UNSET)
 
         trackers = []
         _trackers = d.pop("trackers", UNSET)
         if _trackers is UNSET:
             trackers = UNSET
         else:
@@ -244,14 +258,21 @@
                 else:
                     cvss_scores_item = AffectCVSS.from_dict(_cvss_scores_item)
 
                 cvss_scores.append(cvss_scores_item)
 
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: AffectAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = AffectAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
@@ -377,23 +398,25 @@
 
         env = d.pop("env", UNSET)
 
         revision = d.pop("revision", UNSET)
 
         version = d.pop("version", UNSET)
 
-        osidb_api_v1_affects_create_response_201 = cls(
+        osidb_api_v1_affects_update_response_200 = cls(
             uuid=uuid,
             ps_module=ps_module,
+            ps_product=ps_product,
             ps_component=ps_component,
             trackers=trackers,
             meta_attr=meta_attr,
             delegated_resolution=delegated_resolution,
             cvss_scores=cvss_scores,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
             flaw=flaw,
             type=type,
             affectedness=affectedness,
             resolution=resolution,
             impact=impact,
@@ -403,28 +426,30 @@
             cvss3_score=cvss3_score,
             dt=dt,
             env=env,
             revision=revision,
             version=version,
         )
 
-        osidb_api_v1_affects_create_response_201.additional_properties = d
-        return osidb_api_v1_affects_create_response_201
+        osidb_api_v1_affects_update_response_200.additional_properties = d
+        return osidb_api_v1_affects_update_response_200
 
     @staticmethod
     def get_fields():
         return {
             "uuid": str,
             "ps_module": str,
+            "ps_product": str,
             "ps_component": str,
             "trackers": List[Tracker],
             "meta_attr": AffectMetaAttr,
             "delegated_resolution": str,
             "cvss_scores": List[AffectCVSS],
             "embargoed": bool,
+            "alerts": AffectAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "flaw": str,
             "type": AffectType,
             "affectedness": Union[AffectednessEnum, BlankEnum],
             "resolution": Union[BlankEnum, ResolutionEnum],
             "impact": Union[BlankEnum, ImpactEnum],
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_create_response_201.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_acknowledgments_update_response_200.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,185 +1,176 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.issuer_enum import IssuerEnum
+from ..models.flaw_acknowledgment_alerts import FlawAcknowledgmentAlerts
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="OsidbApiV1AffectsCvssScoresCreateResponse201")
+T = TypeVar("T", bound="OsidbApiV1FlawsAcknowledgmentsUpdateResponse200")
 
 
 @attr.s(auto_attribs=True)
-class OsidbApiV1AffectsCvssScoresCreateResponse201(OSIDBModel):
+class OsidbApiV1FlawsAcknowledgmentsUpdateResponse200(OSIDBModel):
     """ """
 
-    cvss_version: str
-    issuer: IssuerEnum
+    name: str
+    affiliation: str
+    from_upstream: bool
+    flaw: str
     uuid: str
-    vector: str
     embargoed: bool
+    alerts: FlawAcknowledgmentAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
-    affect: Union[Unset, str] = UNSET
-    comment: Union[Unset, str] = UNSET
-    score: Union[Unset, float] = UNSET
     dt: Union[Unset, datetime.datetime] = UNSET
     env: Union[Unset, str] = UNSET
     revision: Union[Unset, str] = UNSET
     version: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        cvss_version = self.cvss_version
-        issuer: str = UNSET
-        if not isinstance(self.issuer, Unset):
-
-            issuer = IssuerEnum(self.issuer).value
-
+        name = self.name
+        affiliation = self.affiliation
+        from_upstream = self.from_upstream
+        flaw = self.flaw
         uuid = self.uuid
-        vector = self.vector
         embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
-        affect = self.affect
-        comment = self.comment
-        score = self.score
         dt: Union[Unset, str] = UNSET
         if not isinstance(self.dt, Unset):
             dt = self.dt.isoformat()
 
         env = self.env
         revision = self.revision
         version = self.version
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        if not isinstance(cvss_version, Unset):
-            field_dict["cvss_version"] = cvss_version
-        if not isinstance(issuer, Unset):
-            field_dict["issuer"] = issuer
+        if not isinstance(name, Unset):
+            field_dict["name"] = name
+        if not isinstance(affiliation, Unset):
+            field_dict["affiliation"] = affiliation
+        if not isinstance(from_upstream, Unset):
+            field_dict["from_upstream"] = from_upstream
+        if not isinstance(flaw, Unset):
+            field_dict["flaw"] = flaw
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
-        if not isinstance(vector, Unset):
-            field_dict["vector"] = vector
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
-        if not isinstance(affect, Unset):
-            field_dict["affect"] = affect
-        if not isinstance(comment, Unset):
-            field_dict["comment"] = comment
-        if not isinstance(score, Unset):
-            field_dict["score"] = score
         if not isinstance(dt, Unset):
             field_dict["dt"] = dt
         if not isinstance(env, Unset):
             field_dict["env"] = env
         if not isinstance(revision, Unset):
             field_dict["revision"] = revision
         if not isinstance(version, Unset):
             field_dict["version"] = version
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        cvss_version = d.pop("cvss_version", UNSET)
+        name = d.pop("name", UNSET)
 
-        _issuer = d.pop("issuer", UNSET)
-        issuer: IssuerEnum
-        if isinstance(_issuer, Unset):
-            issuer = UNSET
-        else:
-            issuer = IssuerEnum(_issuer)
+        affiliation = d.pop("affiliation", UNSET)
 
-        uuid = d.pop("uuid", UNSET)
+        from_upstream = d.pop("from_upstream", UNSET)
+
+        flaw = d.pop("flaw", UNSET)
 
-        vector = d.pop("vector", UNSET)
+        uuid = d.pop("uuid", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawAcknowledgmentAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawAcknowledgmentAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
         _updated_dt = d.pop("updated_dt", UNSET)
         updated_dt: datetime.datetime
         if isinstance(_updated_dt, Unset):
             updated_dt = UNSET
         else:
             updated_dt = isoparse(_updated_dt)
 
-        affect = d.pop("affect", UNSET)
-
-        comment = d.pop("comment", UNSET)
-
-        score = d.pop("score", UNSET)
-
         _dt = d.pop("dt", UNSET)
         dt: Union[Unset, datetime.datetime]
         if isinstance(_dt, Unset):
             dt = UNSET
         else:
             dt = isoparse(_dt)
 
         env = d.pop("env", UNSET)
 
         revision = d.pop("revision", UNSET)
 
         version = d.pop("version", UNSET)
 
-        osidb_api_v1_affects_cvss_scores_create_response_201 = cls(
-            cvss_version=cvss_version,
-            issuer=issuer,
+        osidb_api_v1_flaws_acknowledgments_update_response_200 = cls(
+            name=name,
+            affiliation=affiliation,
+            from_upstream=from_upstream,
+            flaw=flaw,
             uuid=uuid,
-            vector=vector,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
-            affect=affect,
-            comment=comment,
-            score=score,
             dt=dt,
             env=env,
             revision=revision,
             version=version,
         )
 
-        osidb_api_v1_affects_cvss_scores_create_response_201.additional_properties = d
-        return osidb_api_v1_affects_cvss_scores_create_response_201
+        osidb_api_v1_flaws_acknowledgments_update_response_200.additional_properties = d
+        return osidb_api_v1_flaws_acknowledgments_update_response_200
 
     @staticmethod
     def get_fields():
         return {
-            "cvss_version": str,
-            "issuer": IssuerEnum,
+            "name": str,
+            "affiliation": str,
+            "from_upstream": bool,
+            "flaw": str,
             "uuid": str,
-            "vector": str,
             "embargoed": bool,
+            "alerts": FlawAcknowledgmentAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
-            "affect": str,
-            "comment": str,
-            "score": float,
             "dt": datetime.datetime,
             "env": str,
             "revision": str,
             "version": str,
         }
 
     @property
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_destroy_response_204.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_destroy_response_200.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="OsidbApiV1AffectsCvssScoresDestroyResponse204")
+T = TypeVar("T", bound="OsidbApiV1AffectsCvssScoresDestroyResponse200")
 
 
 @attr.s(auto_attribs=True)
-class OsidbApiV1AffectsCvssScoresDestroyResponse204(OSIDBModel):
+class OsidbApiV1AffectsCvssScoresDestroyResponse200(OSIDBModel):
     """ """
 
     dt: Union[Unset, datetime.datetime] = UNSET
     env: Union[Unset, str] = UNSET
     revision: Union[Unset, str] = UNSET
     version: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -53,23 +53,23 @@
 
         env = d.pop("env", UNSET)
 
         revision = d.pop("revision", UNSET)
 
         version = d.pop("version", UNSET)
 
-        osidb_api_v1_affects_cvss_scores_destroy_response_204 = cls(
+        osidb_api_v1_affects_cvss_scores_destroy_response_200 = cls(
             dt=dt,
             env=env,
             revision=revision,
             version=version,
         )
 
-        osidb_api_v1_affects_cvss_scores_destroy_response_204.additional_properties = d
-        return osidb_api_v1_affects_cvss_scores_destroy_response_204
+        osidb_api_v1_affects_cvss_scores_destroy_response_200.additional_properties = d
+        return osidb_api_v1_affects_cvss_scores_destroy_response_200
 
     @staticmethod
     def get_fields():
         return {
             "dt": datetime.datetime,
             "env": str,
             "revision": str,
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_list_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_retrieve_response_200.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,185 +1,186 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.issuer_enum import IssuerEnum
+from ..models.flaw_reference_alerts import FlawReferenceAlerts
+from ..models.flaw_reference_type import FlawReferenceType
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="OsidbApiV1AffectsCvssScoresRetrieveResponse200")
+T = TypeVar("T", bound="OsidbApiV1FlawsReferencesRetrieveResponse200")
 
 
 @attr.s(auto_attribs=True)
-class OsidbApiV1AffectsCvssScoresRetrieveResponse200(OSIDBModel):
+class OsidbApiV1FlawsReferencesRetrieveResponse200(OSIDBModel):
     """ """
 
-    cvss_version: str
-    issuer: IssuerEnum
+    flaw: str
+    url: str
     uuid: str
-    vector: str
     embargoed: bool
+    alerts: FlawReferenceAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
-    affect: Union[Unset, str] = UNSET
-    comment: Union[Unset, str] = UNSET
-    score: Union[Unset, float] = UNSET
+    description: Union[Unset, str] = UNSET
+    type: Union[Unset, FlawReferenceType] = UNSET
     dt: Union[Unset, datetime.datetime] = UNSET
     env: Union[Unset, str] = UNSET
     revision: Union[Unset, str] = UNSET
     version: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        cvss_version = self.cvss_version
-        issuer: str = UNSET
-        if not isinstance(self.issuer, Unset):
-
-            issuer = IssuerEnum(self.issuer).value
-
+        flaw = self.flaw
+        url = self.url
         uuid = self.uuid
-        vector = self.vector
         embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
-        affect = self.affect
-        comment = self.comment
-        score = self.score
+        description = self.description
+        type: Union[Unset, str] = UNSET
+        if not isinstance(self.type, Unset):
+
+            type = FlawReferenceType(self.type).value
+
         dt: Union[Unset, str] = UNSET
         if not isinstance(self.dt, Unset):
             dt = self.dt.isoformat()
 
         env = self.env
         revision = self.revision
         version = self.version
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        if not isinstance(cvss_version, Unset):
-            field_dict["cvss_version"] = cvss_version
-        if not isinstance(issuer, Unset):
-            field_dict["issuer"] = issuer
+        if not isinstance(flaw, Unset):
+            field_dict["flaw"] = flaw
+        if not isinstance(url, Unset):
+            field_dict["url"] = url
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
-        if not isinstance(vector, Unset):
-            field_dict["vector"] = vector
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
-        if not isinstance(affect, Unset):
-            field_dict["affect"] = affect
-        if not isinstance(comment, Unset):
-            field_dict["comment"] = comment
-        if not isinstance(score, Unset):
-            field_dict["score"] = score
+        if not isinstance(description, Unset):
+            field_dict["description"] = description
+        if not isinstance(type, Unset):
+            field_dict["type"] = type
         if not isinstance(dt, Unset):
             field_dict["dt"] = dt
         if not isinstance(env, Unset):
             field_dict["env"] = env
         if not isinstance(revision, Unset):
             field_dict["revision"] = revision
         if not isinstance(version, Unset):
             field_dict["version"] = version
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        cvss_version = d.pop("cvss_version", UNSET)
+        flaw = d.pop("flaw", UNSET)
 
-        _issuer = d.pop("issuer", UNSET)
-        issuer: IssuerEnum
-        if isinstance(_issuer, Unset):
-            issuer = UNSET
-        else:
-            issuer = IssuerEnum(_issuer)
+        url = d.pop("url", UNSET)
 
         uuid = d.pop("uuid", UNSET)
 
-        vector = d.pop("vector", UNSET)
-
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawReferenceAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawReferenceAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
         _updated_dt = d.pop("updated_dt", UNSET)
         updated_dt: datetime.datetime
         if isinstance(_updated_dt, Unset):
             updated_dt = UNSET
         else:
             updated_dt = isoparse(_updated_dt)
 
-        affect = d.pop("affect", UNSET)
+        description = d.pop("description", UNSET)
 
-        comment = d.pop("comment", UNSET)
-
-        score = d.pop("score", UNSET)
+        _type = d.pop("type", UNSET)
+        type: Union[Unset, FlawReferenceType]
+        if isinstance(_type, Unset):
+            type = UNSET
+        else:
+            type = FlawReferenceType(_type)
 
         _dt = d.pop("dt", UNSET)
         dt: Union[Unset, datetime.datetime]
         if isinstance(_dt, Unset):
             dt = UNSET
         else:
             dt = isoparse(_dt)
 
         env = d.pop("env", UNSET)
 
         revision = d.pop("revision", UNSET)
 
         version = d.pop("version", UNSET)
 
-        osidb_api_v1_affects_cvss_scores_retrieve_response_200 = cls(
-            cvss_version=cvss_version,
-            issuer=issuer,
+        osidb_api_v1_flaws_references_retrieve_response_200 = cls(
+            flaw=flaw,
+            url=url,
             uuid=uuid,
-            vector=vector,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
-            affect=affect,
-            comment=comment,
-            score=score,
+            description=description,
+            type=type,
             dt=dt,
             env=env,
             revision=revision,
             version=version,
         )
 
-        osidb_api_v1_affects_cvss_scores_retrieve_response_200.additional_properties = d
-        return osidb_api_v1_affects_cvss_scores_retrieve_response_200
+        osidb_api_v1_flaws_references_retrieve_response_200.additional_properties = d
+        return osidb_api_v1_flaws_references_retrieve_response_200
 
     @staticmethod
     def get_fields():
         return {
-            "cvss_version": str,
-            "issuer": IssuerEnum,
+            "flaw": str,
+            "url": str,
             "uuid": str,
-            "vector": str,
             "embargoed": bool,
+            "alerts": FlawReferenceAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
-            "affect": str,
-            "comment": str,
-            "score": float,
+            "description": str,
+            "type": FlawReferenceType,
             "dt": datetime.datetime,
             "env": str,
             "revision": str,
             "version": str,
         }
 
     @property
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_update_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_acknowledgments_create_response_201.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,185 +1,176 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.issuer_enum import IssuerEnum
+from ..models.flaw_acknowledgment_alerts import FlawAcknowledgmentAlerts
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="OsidbApiV1AffectsCvssScoresUpdateResponse200")
+T = TypeVar("T", bound="OsidbApiV1FlawsAcknowledgmentsCreateResponse201")
 
 
 @attr.s(auto_attribs=True)
-class OsidbApiV1AffectsCvssScoresUpdateResponse200(OSIDBModel):
+class OsidbApiV1FlawsAcknowledgmentsCreateResponse201(OSIDBModel):
     """ """
 
-    cvss_version: str
-    issuer: IssuerEnum
+    name: str
+    affiliation: str
+    from_upstream: bool
+    flaw: str
     uuid: str
-    vector: str
     embargoed: bool
+    alerts: FlawAcknowledgmentAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
-    affect: Union[Unset, str] = UNSET
-    comment: Union[Unset, str] = UNSET
-    score: Union[Unset, float] = UNSET
     dt: Union[Unset, datetime.datetime] = UNSET
     env: Union[Unset, str] = UNSET
     revision: Union[Unset, str] = UNSET
     version: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        cvss_version = self.cvss_version
-        issuer: str = UNSET
-        if not isinstance(self.issuer, Unset):
-
-            issuer = IssuerEnum(self.issuer).value
-
+        name = self.name
+        affiliation = self.affiliation
+        from_upstream = self.from_upstream
+        flaw = self.flaw
         uuid = self.uuid
-        vector = self.vector
         embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
-        affect = self.affect
-        comment = self.comment
-        score = self.score
         dt: Union[Unset, str] = UNSET
         if not isinstance(self.dt, Unset):
             dt = self.dt.isoformat()
 
         env = self.env
         revision = self.revision
         version = self.version
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        if not isinstance(cvss_version, Unset):
-            field_dict["cvss_version"] = cvss_version
-        if not isinstance(issuer, Unset):
-            field_dict["issuer"] = issuer
+        if not isinstance(name, Unset):
+            field_dict["name"] = name
+        if not isinstance(affiliation, Unset):
+            field_dict["affiliation"] = affiliation
+        if not isinstance(from_upstream, Unset):
+            field_dict["from_upstream"] = from_upstream
+        if not isinstance(flaw, Unset):
+            field_dict["flaw"] = flaw
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
-        if not isinstance(vector, Unset):
-            field_dict["vector"] = vector
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
-        if not isinstance(affect, Unset):
-            field_dict["affect"] = affect
-        if not isinstance(comment, Unset):
-            field_dict["comment"] = comment
-        if not isinstance(score, Unset):
-            field_dict["score"] = score
         if not isinstance(dt, Unset):
             field_dict["dt"] = dt
         if not isinstance(env, Unset):
             field_dict["env"] = env
         if not isinstance(revision, Unset):
             field_dict["revision"] = revision
         if not isinstance(version, Unset):
             field_dict["version"] = version
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        cvss_version = d.pop("cvss_version", UNSET)
+        name = d.pop("name", UNSET)
 
-        _issuer = d.pop("issuer", UNSET)
-        issuer: IssuerEnum
-        if isinstance(_issuer, Unset):
-            issuer = UNSET
-        else:
-            issuer = IssuerEnum(_issuer)
+        affiliation = d.pop("affiliation", UNSET)
 
-        uuid = d.pop("uuid", UNSET)
+        from_upstream = d.pop("from_upstream", UNSET)
+
+        flaw = d.pop("flaw", UNSET)
 
-        vector = d.pop("vector", UNSET)
+        uuid = d.pop("uuid", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawAcknowledgmentAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawAcknowledgmentAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
         _updated_dt = d.pop("updated_dt", UNSET)
         updated_dt: datetime.datetime
         if isinstance(_updated_dt, Unset):
             updated_dt = UNSET
         else:
             updated_dt = isoparse(_updated_dt)
 
-        affect = d.pop("affect", UNSET)
-
-        comment = d.pop("comment", UNSET)
-
-        score = d.pop("score", UNSET)
-
         _dt = d.pop("dt", UNSET)
         dt: Union[Unset, datetime.datetime]
         if isinstance(_dt, Unset):
             dt = UNSET
         else:
             dt = isoparse(_dt)
 
         env = d.pop("env", UNSET)
 
         revision = d.pop("revision", UNSET)
 
         version = d.pop("version", UNSET)
 
-        osidb_api_v1_affects_cvss_scores_update_response_200 = cls(
-            cvss_version=cvss_version,
-            issuer=issuer,
+        osidb_api_v1_flaws_acknowledgments_create_response_201 = cls(
+            name=name,
+            affiliation=affiliation,
+            from_upstream=from_upstream,
+            flaw=flaw,
             uuid=uuid,
-            vector=vector,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
-            affect=affect,
-            comment=comment,
-            score=score,
             dt=dt,
             env=env,
             revision=revision,
             version=version,
         )
 
-        osidb_api_v1_affects_cvss_scores_update_response_200.additional_properties = d
-        return osidb_api_v1_affects_cvss_scores_update_response_200
+        osidb_api_v1_flaws_acknowledgments_create_response_201.additional_properties = d
+        return osidb_api_v1_flaws_acknowledgments_create_response_201
 
     @staticmethod
     def get_fields():
         return {
-            "cvss_version": str,
-            "issuer": IssuerEnum,
+            "name": str,
+            "affiliation": str,
+            "from_upstream": bool,
+            "flaw": str,
             "uuid": str,
-            "vector": str,
             "embargoed": bool,
+            "alerts": FlawAcknowledgmentAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
-            "affect": str,
-            "comment": str,
-            "score": float,
             "dt": datetime.datetime,
             "env": str,
             "revision": str,
             "version": str,
         }
 
     @property
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_destroy_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_destroy_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_flaw_source.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_flaw_source.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_order_item.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_order_item.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,86 +6,98 @@
     VALUE_1 = "-created_dt"
     VALUE_2 = "-cvss2"
     VALUE_3 = "-cvss2_score"
     VALUE_4 = "-cvss3"
     VALUE_5 = "-cvss3_score"
     VALUE_6 = "-cvss_scores__comment"
     VALUE_7 = "-cvss_scores__created_dt"
-    VALUE_8 = "-cvss_scores__issuer"
-    VALUE_9 = "-cvss_scores__score"
-    VALUE_10 = "-cvss_scores__updated_dt"
-    VALUE_11 = "-cvss_scores__uuid"
-    VALUE_12 = "-cvss_scores__vector"
-    VALUE_13 = "-flaw__component"
-    VALUE_14 = "-flaw__created_dt"
-    VALUE_15 = "-flaw__cve_id"
-    VALUE_16 = "-flaw__cvss2"
-    VALUE_17 = "-flaw__cvss2_score"
-    VALUE_18 = "-flaw__cvss3"
-    VALUE_19 = "-flaw__cvss3_score"
-    VALUE_20 = "-flaw__cwe_id"
-    VALUE_21 = "-flaw__impact"
-    VALUE_22 = "-flaw__nvd_cvss2"
-    VALUE_23 = "-flaw__nvd_cvss3"
-    VALUE_24 = "-flaw__reported_dt"
-    VALUE_25 = "-flaw__source"
-    VALUE_26 = "-flaw__type"
-    VALUE_27 = "-flaw__unembargo_dt"
-    VALUE_28 = "-flaw__updated_dt"
-    VALUE_29 = "-flaw__uuid"
-    VALUE_30 = "-impact"
-    VALUE_31 = "-ps_component"
-    VALUE_32 = "-ps_module"
-    VALUE_33 = "-resolution"
-    VALUE_34 = "-trackers__created_dt"
-    VALUE_35 = "-trackers__external_system_id"
-    VALUE_36 = "-trackers__ps_update_stream"
-    VALUE_37 = "-trackers__resolution"
-    VALUE_38 = "-trackers__status"
-    VALUE_39 = "-trackers__type"
-    VALUE_40 = "-trackers__updated_dt"
-    VALUE_41 = "-trackers__uuid"
-    VALUE_42 = "-type"
-    VALUE_43 = "-updated_dt"
-    VALUE_44 = "-uuid"
+    VALUE_8 = "-cvss_scores__cvss_version"
+    VALUE_9 = "-cvss_scores__issuer"
+    VALUE_10 = "-cvss_scores__score"
+    VALUE_11 = "-cvss_scores__updated_dt"
+    VALUE_12 = "-cvss_scores__uuid"
+    VALUE_13 = "-cvss_scores__vector"
+    VALUE_14 = "-embargoed"
+    VALUE_15 = "-flaw__component"
+    VALUE_16 = "-flaw__components"
+    VALUE_17 = "-flaw__created_dt"
+    VALUE_18 = "-flaw__cve_id"
+    VALUE_19 = "-flaw__cvss2"
+    VALUE_20 = "-flaw__cvss2_score"
+    VALUE_21 = "-flaw__cvss3"
+    VALUE_22 = "-flaw__cvss3_score"
+    VALUE_23 = "-flaw__cwe_id"
+    VALUE_24 = "-flaw__embargoed"
+    VALUE_25 = "-flaw__impact"
+    VALUE_26 = "-flaw__is_major_incident"
+    VALUE_27 = "-flaw__nvd_cvss2"
+    VALUE_28 = "-flaw__nvd_cvss3"
+    VALUE_29 = "-flaw__reported_dt"
+    VALUE_30 = "-flaw__source"
+    VALUE_31 = "-flaw__type"
+    VALUE_32 = "-flaw__unembargo_dt"
+    VALUE_33 = "-flaw__updated_dt"
+    VALUE_34 = "-flaw__uuid"
+    VALUE_35 = "-impact"
+    VALUE_36 = "-ps_component"
+    VALUE_37 = "-ps_module"
+    VALUE_38 = "-resolution"
+    VALUE_39 = "-trackers__created_dt"
+    VALUE_40 = "-trackers__embargoed"
+    VALUE_41 = "-trackers__external_system_id"
+    VALUE_42 = "-trackers__ps_update_stream"
+    VALUE_43 = "-trackers__resolution"
+    VALUE_44 = "-trackers__status"
+    VALUE_45 = "-trackers__type"
+    VALUE_46 = "-trackers__updated_dt"
+    VALUE_47 = "-trackers__uuid"
+    VALUE_48 = "-type"
+    VALUE_49 = "-updated_dt"
+    VALUE_50 = "-uuid"
     AFFECTEDNESS = "affectedness"
     CREATED_DT = "created_dt"
     CVSS2 = "cvss2"
     CVSS2_SCORE = "cvss2_score"
     CVSS3 = "cvss3"
     CVSS3_SCORE = "cvss3_score"
     CVSS_SCORES_COMMENT = "cvss_scores__comment"
     CVSS_SCORES_CREATED_DT = "cvss_scores__created_dt"
+    CVSS_SCORES_CVSS_VERSION = "cvss_scores__cvss_version"
     CVSS_SCORES_ISSUER = "cvss_scores__issuer"
     CVSS_SCORES_SCORE = "cvss_scores__score"
     CVSS_SCORES_UPDATED_DT = "cvss_scores__updated_dt"
     CVSS_SCORES_UUID = "cvss_scores__uuid"
     CVSS_SCORES_VECTOR = "cvss_scores__vector"
+    EMBARGOED = "embargoed"
     FLAW_COMPONENT = "flaw__component"
+    FLAW_COMPONENTS = "flaw__components"
     FLAW_CREATED_DT = "flaw__created_dt"
     FLAW_CVE_ID = "flaw__cve_id"
     FLAW_CVSS2 = "flaw__cvss2"
     FLAW_CVSS2_SCORE = "flaw__cvss2_score"
     FLAW_CVSS3 = "flaw__cvss3"
     FLAW_CVSS3_SCORE = "flaw__cvss3_score"
     FLAW_CWE_ID = "flaw__cwe_id"
+    FLAW_EMBARGOED = "flaw__embargoed"
     FLAW_IMPACT = "flaw__impact"
+    FLAW_IS_MAJOR_INCIDENT = "flaw__is_major_incident"
     FLAW_NVD_CVSS2 = "flaw__nvd_cvss2"
     FLAW_NVD_CVSS3 = "flaw__nvd_cvss3"
     FLAW_REPORTED_DT = "flaw__reported_dt"
     FLAW_SOURCE = "flaw__source"
     FLAW_TYPE = "flaw__type"
     FLAW_UNEMBARGO_DT = "flaw__unembargo_dt"
     FLAW_UPDATED_DT = "flaw__updated_dt"
     FLAW_UUID = "flaw__uuid"
     IMPACT = "impact"
     PS_COMPONENT = "ps_component"
     PS_MODULE = "ps_module"
     RESOLUTION = "resolution"
     TRACKERS_CREATED_DT = "trackers__created_dt"
+    TRACKERS_EMBARGOED = "trackers__embargoed"
     TRACKERS_EXTERNAL_SYSTEM_ID = "trackers__external_system_id"
     TRACKERS_PS_UPDATE_STREAM = "trackers__ps_update_stream"
     TRACKERS_RESOLUTION = "trackers__resolution"
     TRACKERS_STATUS = "trackers__status"
     TRACKERS_TYPE = "trackers__type"
     TRACKERS_UPDATED_DT = "trackers__updated_dt"
     TRACKERS_UUID = "trackers__uuid"
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_create_response_201.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import datetime
 from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.affect_alerts import AffectAlerts
 from ..models.affect_cvss import AffectCVSS
 from ..models.affect_meta_attr import AffectMetaAttr
 from ..models.affect_type import AffectType
 from ..models.affectedness_enum import AffectednessEnum
 from ..models.blank_enum import BlankEnum
 from ..models.impact_enum import ImpactEnum
 from ..models.resolution_enum import ResolutionEnum
 from ..models.tracker import Tracker
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="OsidbApiV1AffectsRetrieveResponse200")
+T = TypeVar("T", bound="OsidbApiV1AffectsCreateResponse201")
 
 
 @attr.s(auto_attribs=True)
-class OsidbApiV1AffectsRetrieveResponse200(OSIDBModel):
+class OsidbApiV1AffectsCreateResponse201(OSIDBModel):
     """ """
 
     uuid: str
     ps_module: str
+    ps_product: str
     ps_component: str
     trackers: List[Tracker]
     meta_attr: AffectMetaAttr
     delegated_resolution: str
     cvss_scores: List[AffectCVSS]
     embargoed: bool
+    alerts: AffectAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     flaw: Optional[str]
     type: Union[Unset, AffectType] = UNSET
     affectedness: Union[AffectednessEnum, BlankEnum, Unset] = UNSET
     resolution: Union[BlankEnum, ResolutionEnum, Unset] = UNSET
     impact: Union[BlankEnum, ImpactEnum, Unset] = UNSET
@@ -45,14 +48,15 @@
     revision: Union[Unset, str] = UNSET
     version: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         uuid = self.uuid
         ps_module = self.ps_module
+        ps_product = self.ps_product
         ps_component = self.ps_component
         trackers: List[Dict[str, Any]] = UNSET
         if not isinstance(self.trackers, Unset):
             trackers = []
             for trackers_item_data in self.trackers:
                 trackers_item: Dict[str, Any] = UNSET
                 if not isinstance(trackers_item_data, Unset):
@@ -72,14 +76,18 @@
                 cvss_scores_item: Dict[str, Any] = UNSET
                 if not isinstance(cvss_scores_item_data, Unset):
                     cvss_scores_item = cvss_scores_item_data.to_dict()
 
                 cvss_scores.append(cvss_scores_item)
 
         embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
@@ -149,26 +157,30 @@
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(ps_module, Unset):
             field_dict["ps_module"] = ps_module
+        if not isinstance(ps_product, Unset):
+            field_dict["ps_product"] = ps_product
         if not isinstance(ps_component, Unset):
             field_dict["ps_component"] = ps_component
         if not isinstance(trackers, Unset):
             field_dict["trackers"] = trackers
         if not isinstance(meta_attr, Unset):
             field_dict["meta_attr"] = meta_attr
         if not isinstance(delegated_resolution, Unset):
             field_dict["delegated_resolution"] = delegated_resolution
         if not isinstance(cvss_scores, Unset):
             field_dict["cvss_scores"] = cvss_scores
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(flaw, Unset):
             field_dict["flaw"] = flaw
         if not isinstance(type, Unset):
@@ -201,14 +213,16 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         uuid = d.pop("uuid", UNSET)
 
         ps_module = d.pop("ps_module", UNSET)
 
+        ps_product = d.pop("ps_product", UNSET)
+
         ps_component = d.pop("ps_component", UNSET)
 
         trackers = []
         _trackers = d.pop("trackers", UNSET)
         if _trackers is UNSET:
             trackers = UNSET
         else:
@@ -244,14 +258,21 @@
                 else:
                     cvss_scores_item = AffectCVSS.from_dict(_cvss_scores_item)
 
                 cvss_scores.append(cvss_scores_item)
 
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: AffectAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = AffectAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
@@ -377,23 +398,25 @@
 
         env = d.pop("env", UNSET)
 
         revision = d.pop("revision", UNSET)
 
         version = d.pop("version", UNSET)
 
-        osidb_api_v1_affects_retrieve_response_200 = cls(
+        osidb_api_v1_affects_create_response_201 = cls(
             uuid=uuid,
             ps_module=ps_module,
+            ps_product=ps_product,
             ps_component=ps_component,
             trackers=trackers,
             meta_attr=meta_attr,
             delegated_resolution=delegated_resolution,
             cvss_scores=cvss_scores,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
             flaw=flaw,
             type=type,
             affectedness=affectedness,
             resolution=resolution,
             impact=impact,
@@ -403,28 +426,30 @@
             cvss3_score=cvss3_score,
             dt=dt,
             env=env,
             revision=revision,
             version=version,
         )
 
-        osidb_api_v1_affects_retrieve_response_200.additional_properties = d
-        return osidb_api_v1_affects_retrieve_response_200
+        osidb_api_v1_affects_create_response_201.additional_properties = d
+        return osidb_api_v1_affects_create_response_201
 
     @staticmethod
     def get_fields():
         return {
             "uuid": str,
             "ps_module": str,
+            "ps_product": str,
             "ps_component": str,
             "trackers": List[Tracker],
             "meta_attr": AffectMetaAttr,
             "delegated_resolution": str,
             "cvss_scores": List[AffectCVSS],
             "embargoed": bool,
+            "alerts": AffectAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "flaw": str,
             "type": AffectType,
             "affectedness": Union[AffectednessEnum, BlankEnum],
             "resolution": Union[BlankEnum, ResolutionEnum],
             "impact": Union[BlankEnum, ImpactEnum],
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_update_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_retrieve_response_200.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import datetime
 from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.affect_alerts import AffectAlerts
 from ..models.affect_cvss import AffectCVSS
 from ..models.affect_meta_attr import AffectMetaAttr
 from ..models.affect_type import AffectType
 from ..models.affectedness_enum import AffectednessEnum
 from ..models.blank_enum import BlankEnum
 from ..models.impact_enum import ImpactEnum
 from ..models.resolution_enum import ResolutionEnum
 from ..models.tracker import Tracker
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="OsidbApiV1AffectsUpdateResponse200")
+T = TypeVar("T", bound="OsidbApiV1AffectsRetrieveResponse200")
 
 
 @attr.s(auto_attribs=True)
-class OsidbApiV1AffectsUpdateResponse200(OSIDBModel):
+class OsidbApiV1AffectsRetrieveResponse200(OSIDBModel):
     """ """
 
     uuid: str
     ps_module: str
+    ps_product: str
     ps_component: str
     trackers: List[Tracker]
     meta_attr: AffectMetaAttr
     delegated_resolution: str
     cvss_scores: List[AffectCVSS]
     embargoed: bool
+    alerts: AffectAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     flaw: Optional[str]
     type: Union[Unset, AffectType] = UNSET
     affectedness: Union[AffectednessEnum, BlankEnum, Unset] = UNSET
     resolution: Union[BlankEnum, ResolutionEnum, Unset] = UNSET
     impact: Union[BlankEnum, ImpactEnum, Unset] = UNSET
@@ -45,14 +48,15 @@
     revision: Union[Unset, str] = UNSET
     version: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         uuid = self.uuid
         ps_module = self.ps_module
+        ps_product = self.ps_product
         ps_component = self.ps_component
         trackers: List[Dict[str, Any]] = UNSET
         if not isinstance(self.trackers, Unset):
             trackers = []
             for trackers_item_data in self.trackers:
                 trackers_item: Dict[str, Any] = UNSET
                 if not isinstance(trackers_item_data, Unset):
@@ -72,14 +76,18 @@
                 cvss_scores_item: Dict[str, Any] = UNSET
                 if not isinstance(cvss_scores_item_data, Unset):
                     cvss_scores_item = cvss_scores_item_data.to_dict()
 
                 cvss_scores.append(cvss_scores_item)
 
         embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
@@ -149,26 +157,30 @@
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(ps_module, Unset):
             field_dict["ps_module"] = ps_module
+        if not isinstance(ps_product, Unset):
+            field_dict["ps_product"] = ps_product
         if not isinstance(ps_component, Unset):
             field_dict["ps_component"] = ps_component
         if not isinstance(trackers, Unset):
             field_dict["trackers"] = trackers
         if not isinstance(meta_attr, Unset):
             field_dict["meta_attr"] = meta_attr
         if not isinstance(delegated_resolution, Unset):
             field_dict["delegated_resolution"] = delegated_resolution
         if not isinstance(cvss_scores, Unset):
             field_dict["cvss_scores"] = cvss_scores
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(flaw, Unset):
             field_dict["flaw"] = flaw
         if not isinstance(type, Unset):
@@ -201,14 +213,16 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         uuid = d.pop("uuid", UNSET)
 
         ps_module = d.pop("ps_module", UNSET)
 
+        ps_product = d.pop("ps_product", UNSET)
+
         ps_component = d.pop("ps_component", UNSET)
 
         trackers = []
         _trackers = d.pop("trackers", UNSET)
         if _trackers is UNSET:
             trackers = UNSET
         else:
@@ -244,14 +258,21 @@
                 else:
                     cvss_scores_item = AffectCVSS.from_dict(_cvss_scores_item)
 
                 cvss_scores.append(cvss_scores_item)
 
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: AffectAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = AffectAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
@@ -377,23 +398,25 @@
 
         env = d.pop("env", UNSET)
 
         revision = d.pop("revision", UNSET)
 
         version = d.pop("version", UNSET)
 
-        osidb_api_v1_affects_update_response_200 = cls(
+        osidb_api_v1_affects_retrieve_response_200 = cls(
             uuid=uuid,
             ps_module=ps_module,
+            ps_product=ps_product,
             ps_component=ps_component,
             trackers=trackers,
             meta_attr=meta_attr,
             delegated_resolution=delegated_resolution,
             cvss_scores=cvss_scores,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
             flaw=flaw,
             type=type,
             affectedness=affectedness,
             resolution=resolution,
             impact=impact,
@@ -403,28 +426,30 @@
             cvss3_score=cvss3_score,
             dt=dt,
             env=env,
             revision=revision,
             version=version,
         )
 
-        osidb_api_v1_affects_update_response_200.additional_properties = d
-        return osidb_api_v1_affects_update_response_200
+        osidb_api_v1_affects_retrieve_response_200.additional_properties = d
+        return osidb_api_v1_affects_retrieve_response_200
 
     @staticmethod
     def get_fields():
         return {
             "uuid": str,
             "ps_module": str,
+            "ps_product": str,
             "ps_component": str,
             "trackers": List[Tracker],
             "meta_attr": AffectMetaAttr,
             "delegated_resolution": str,
             "cvss_scores": List[AffectCVSS],
             "embargoed": bool,
+            "alerts": AffectAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "flaw": str,
             "type": AffectType,
             "affectedness": Union[AffectednessEnum, BlankEnum],
             "resolution": Union[BlankEnum, ResolutionEnum],
             "impact": Union[BlankEnum, ImpactEnum],
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_acknowledgments_create_response_201.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_package_versions_update_response_200.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.flaw_version import FlawVersion
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="OsidbApiV1FlawsAcknowledgmentsCreateResponse201")
+T = TypeVar("T", bound="OsidbApiV1FlawsPackageVersionsUpdateResponse200")
 
 
 @attr.s(auto_attribs=True)
-class OsidbApiV1FlawsAcknowledgmentsCreateResponse201(OSIDBModel):
+class OsidbApiV1FlawsPackageVersionsUpdateResponse200(OSIDBModel):
     """ """
 
-    name: str
-    affiliation: str
-    from_upstream: bool
+    package: str
+    versions: List[FlawVersion]
     flaw: str
     uuid: str
     embargoed: bool
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     dt: Union[Unset, datetime.datetime] = UNSET
     env: Union[Unset, str] = UNSET
     revision: Union[Unset, str] = UNSET
     version: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        affiliation = self.affiliation
-        from_upstream = self.from_upstream
+        package = self.package
+        versions: List[Dict[str, Any]] = UNSET
+        if not isinstance(self.versions, Unset):
+            versions = []
+            for versions_item_data in self.versions:
+                versions_item: Dict[str, Any] = UNSET
+                if not isinstance(versions_item_data, Unset):
+                    versions_item = versions_item_data.to_dict()
+
+                versions.append(versions_item)
+
         flaw = self.flaw
         uuid = self.uuid
         embargoed = self.embargoed
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
@@ -48,20 +56,18 @@
 
         env = self.env
         revision = self.revision
         version = self.version
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        if not isinstance(name, Unset):
-            field_dict["name"] = name
-        if not isinstance(affiliation, Unset):
-            field_dict["affiliation"] = affiliation
-        if not isinstance(from_upstream, Unset):
-            field_dict["from_upstream"] = from_upstream
+        if not isinstance(package, Unset):
+            field_dict["package"] = package
+        if not isinstance(versions, Unset):
+            field_dict["versions"] = versions
         if not isinstance(flaw, Unset):
             field_dict["flaw"] = flaw
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
         if not isinstance(created_dt, Unset):
@@ -78,19 +84,30 @@
             field_dict["version"] = version
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        name = d.pop("name", UNSET)
+        package = d.pop("package", UNSET)
 
-        affiliation = d.pop("affiliation", UNSET)
+        versions = []
+        _versions = d.pop("versions", UNSET)
+        if _versions is UNSET:
+            versions = UNSET
+        else:
+            for versions_item_data in _versions or []:
+                _versions_item = versions_item_data
+                versions_item: FlawVersion
+                if isinstance(_versions_item, Unset):
+                    versions_item = UNSET
+                else:
+                    versions_item = FlawVersion.from_dict(_versions_item)
 
-        from_upstream = d.pop("from_upstream", UNSET)
+                versions.append(versions_item)
 
         flaw = d.pop("flaw", UNSET)
 
         uuid = d.pop("uuid", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
@@ -117,38 +134,38 @@
 
         env = d.pop("env", UNSET)
 
         revision = d.pop("revision", UNSET)
 
         version = d.pop("version", UNSET)
 
-        osidb_api_v1_flaws_acknowledgments_create_response_201 = cls(
-            name=name,
-            affiliation=affiliation,
-            from_upstream=from_upstream,
+        osidb_api_v1_flaws_package_versions_update_response_200 = cls(
+            package=package,
+            versions=versions,
             flaw=flaw,
             uuid=uuid,
             embargoed=embargoed,
             created_dt=created_dt,
             updated_dt=updated_dt,
             dt=dt,
             env=env,
             revision=revision,
             version=version,
         )
 
-        osidb_api_v1_flaws_acknowledgments_create_response_201.additional_properties = d
-        return osidb_api_v1_flaws_acknowledgments_create_response_201
+        osidb_api_v1_flaws_package_versions_update_response_200.additional_properties = (
+            d
+        )
+        return osidb_api_v1_flaws_package_versions_update_response_200
 
     @staticmethod
     def get_fields():
         return {
-            "name": str,
-            "affiliation": str,
-            "from_upstream": bool,
+            "package": str,
+            "versions": List[FlawVersion],
             "flaw": str,
             "uuid": str,
             "embargoed": bool,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "dt": datetime.datetime,
             "env": str,
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_acknowledgments_destroy_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_acknowledgments_destroy_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_acknowledgments_list_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_acknowledgments_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_acknowledgments_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_acknowledgment_put.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,165 +1,188 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union
+import json
+from typing import Any, Dict, List, Tuple, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.flaw_acknowledgment_put_alerts import FlawAcknowledgmentPutAlerts
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="OsidbApiV1FlawsAcknowledgmentsRetrieveResponse200")
+T = TypeVar("T", bound="FlawAcknowledgmentPut")
 
 
 @attr.s(auto_attribs=True)
-class OsidbApiV1FlawsAcknowledgmentsRetrieveResponse200(OSIDBModel):
-    """ """
+class FlawAcknowledgmentPut(OSIDBModel):
+    """FlawAcknowledgment serializer"""
 
     name: str
     affiliation: str
     from_upstream: bool
-    flaw: str
     uuid: str
     embargoed: bool
+    alerts: FlawAcknowledgmentPutAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
-    dt: Union[Unset, datetime.datetime] = UNSET
-    env: Union[Unset, str] = UNSET
-    revision: Union[Unset, str] = UNSET
-    version: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         name = self.name
         affiliation = self.affiliation
         from_upstream = self.from_upstream
-        flaw = self.flaw
         uuid = self.uuid
         embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
-        dt: Union[Unset, str] = UNSET
-        if not isinstance(self.dt, Unset):
-            dt = self.dt.isoformat()
-
-        env = self.env
-        revision = self.revision
-        version = self.version
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if not isinstance(name, Unset):
             field_dict["name"] = name
         if not isinstance(affiliation, Unset):
             field_dict["affiliation"] = affiliation
         if not isinstance(from_upstream, Unset):
             field_dict["from_upstream"] = from_upstream
-        if not isinstance(flaw, Unset):
-            field_dict["flaw"] = flaw
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
+        if not isinstance(created_dt, Unset):
+            field_dict["created_dt"] = created_dt
+        if not isinstance(updated_dt, Unset):
+            field_dict["updated_dt"] = updated_dt
+
+        return field_dict
+
+    def to_multipart(self) -> Dict[str, Any]:
+        name = self.name if self.name is UNSET else (None, str(self.name), "text/plain")
+        affiliation = (
+            self.affiliation
+            if self.affiliation is UNSET
+            else (None, str(self.affiliation), "text/plain")
+        )
+        from_upstream = (
+            self.from_upstream
+            if self.from_upstream is UNSET
+            else (None, str(self.from_upstream), "text/plain")
+        )
+        uuid = self.uuid if self.uuid is UNSET else (None, str(self.uuid), "text/plain")
+        embargoed = (
+            self.embargoed
+            if self.embargoed is UNSET
+            else (None, str(self.embargoed), "text/plain")
+        )
+        alerts: Union[Unset, Tuple[None, str, str]] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = (None, json.dumps(self.alerts.to_dict()), "application/json")
+
+        created_dt: str = UNSET
+        if not isinstance(self.created_dt, Unset):
+            created_dt = self.created_dt.isoformat()
+
+        updated_dt: str = UNSET
+        if not isinstance(self.updated_dt, Unset):
+            updated_dt = self.updated_dt.isoformat()
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(
+            {
+                key: (None, str(value), "text/plain")
+                for key, value in self.additional_properties.items()
+            }
+        )
+        if not isinstance(name, Unset):
+            field_dict["name"] = name
+        if not isinstance(affiliation, Unset):
+            field_dict["affiliation"] = affiliation
+        if not isinstance(from_upstream, Unset):
+            field_dict["from_upstream"] = from_upstream
+        if not isinstance(uuid, Unset):
+            field_dict["uuid"] = uuid
+        if not isinstance(embargoed, Unset):
+            field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
-        if not isinstance(dt, Unset):
-            field_dict["dt"] = dt
-        if not isinstance(env, Unset):
-            field_dict["env"] = env
-        if not isinstance(revision, Unset):
-            field_dict["revision"] = revision
-        if not isinstance(version, Unset):
-            field_dict["version"] = version
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name", UNSET)
 
         affiliation = d.pop("affiliation", UNSET)
 
         from_upstream = d.pop("from_upstream", UNSET)
 
-        flaw = d.pop("flaw", UNSET)
-
         uuid = d.pop("uuid", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawAcknowledgmentPutAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawAcknowledgmentPutAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
         _updated_dt = d.pop("updated_dt", UNSET)
         updated_dt: datetime.datetime
         if isinstance(_updated_dt, Unset):
             updated_dt = UNSET
         else:
             updated_dt = isoparse(_updated_dt)
 
-        _dt = d.pop("dt", UNSET)
-        dt: Union[Unset, datetime.datetime]
-        if isinstance(_dt, Unset):
-            dt = UNSET
-        else:
-            dt = isoparse(_dt)
-
-        env = d.pop("env", UNSET)
-
-        revision = d.pop("revision", UNSET)
-
-        version = d.pop("version", UNSET)
-
-        osidb_api_v1_flaws_acknowledgments_retrieve_response_200 = cls(
+        flaw_acknowledgment_put = cls(
             name=name,
             affiliation=affiliation,
             from_upstream=from_upstream,
-            flaw=flaw,
             uuid=uuid,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
-            dt=dt,
-            env=env,
-            revision=revision,
-            version=version,
         )
 
-        osidb_api_v1_flaws_acknowledgments_retrieve_response_200.additional_properties = (
-            d
-        )
-        return osidb_api_v1_flaws_acknowledgments_retrieve_response_200
+        flaw_acknowledgment_put.additional_properties = d
+        return flaw_acknowledgment_put
 
     @staticmethod
     def get_fields():
         return {
             "name": str,
             "affiliation": str,
             "from_upstream": bool,
-            "flaw": str,
             "uuid": str,
             "embargoed": bool,
+            "alerts": FlawAcknowledgmentPutAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
-            "dt": datetime.datetime,
-            "env": str,
-            "revision": str,
-            "version": str,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_acknowledgments_update_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_package_versions_list_response_200.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,159 +1,134 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.flaw_package_version import FlawPackageVersion
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="OsidbApiV1FlawsAcknowledgmentsUpdateResponse200")
+T = TypeVar("T", bound="OsidbApiV1FlawsPackageVersionsListResponse200")
 
 
 @attr.s(auto_attribs=True)
-class OsidbApiV1FlawsAcknowledgmentsUpdateResponse200(OSIDBModel):
+class OsidbApiV1FlawsPackageVersionsListResponse200(OSIDBModel):
     """ """
 
-    name: str
-    affiliation: str
-    from_upstream: bool
-    flaw: str
-    uuid: str
-    embargoed: bool
-    created_dt: datetime.datetime
-    updated_dt: datetime.datetime
+    count: Union[Unset, int] = UNSET
+    next_: Union[Unset, None, str] = UNSET
+    previous: Union[Unset, None, str] = UNSET
+    results: Union[Unset, List[FlawPackageVersion]] = UNSET
     dt: Union[Unset, datetime.datetime] = UNSET
     env: Union[Unset, str] = UNSET
     revision: Union[Unset, str] = UNSET
     version: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        affiliation = self.affiliation
-        from_upstream = self.from_upstream
-        flaw = self.flaw
-        uuid = self.uuid
-        embargoed = self.embargoed
-        created_dt: str = UNSET
-        if not isinstance(self.created_dt, Unset):
-            created_dt = self.created_dt.isoformat()
-
-        updated_dt: str = UNSET
-        if not isinstance(self.updated_dt, Unset):
-            updated_dt = self.updated_dt.isoformat()
+        count = self.count
+        next_ = self.next_
+        previous = self.previous
+        results: Union[Unset, List[Dict[str, Any]]] = UNSET
+        if not isinstance(self.results, Unset):
+            results = []
+            for results_item_data in self.results:
+                results_item: Dict[str, Any] = UNSET
+                if not isinstance(results_item_data, Unset):
+                    results_item = results_item_data.to_dict()
+
+                results.append(results_item)
 
         dt: Union[Unset, str] = UNSET
         if not isinstance(self.dt, Unset):
             dt = self.dt.isoformat()
 
         env = self.env
         revision = self.revision
         version = self.version
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        if not isinstance(name, Unset):
-            field_dict["name"] = name
-        if not isinstance(affiliation, Unset):
-            field_dict["affiliation"] = affiliation
-        if not isinstance(from_upstream, Unset):
-            field_dict["from_upstream"] = from_upstream
-        if not isinstance(flaw, Unset):
-            field_dict["flaw"] = flaw
-        if not isinstance(uuid, Unset):
-            field_dict["uuid"] = uuid
-        if not isinstance(embargoed, Unset):
-            field_dict["embargoed"] = embargoed
-        if not isinstance(created_dt, Unset):
-            field_dict["created_dt"] = created_dt
-        if not isinstance(updated_dt, Unset):
-            field_dict["updated_dt"] = updated_dt
+        if not isinstance(count, Unset):
+            field_dict["count"] = count
+        if not isinstance(next_, Unset):
+            field_dict["next"] = next_
+        if not isinstance(previous, Unset):
+            field_dict["previous"] = previous
+        if not isinstance(results, Unset):
+            field_dict["results"] = results
         if not isinstance(dt, Unset):
             field_dict["dt"] = dt
         if not isinstance(env, Unset):
             field_dict["env"] = env
         if not isinstance(revision, Unset):
             field_dict["revision"] = revision
         if not isinstance(version, Unset):
             field_dict["version"] = version
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        name = d.pop("name", UNSET)
-
-        affiliation = d.pop("affiliation", UNSET)
-
-        from_upstream = d.pop("from_upstream", UNSET)
+        count = d.pop("count", UNSET)
 
-        flaw = d.pop("flaw", UNSET)
+        next_ = d.pop("next", UNSET)
 
-        uuid = d.pop("uuid", UNSET)
+        previous = d.pop("previous", UNSET)
 
-        embargoed = d.pop("embargoed", UNSET)
-
-        _created_dt = d.pop("created_dt", UNSET)
-        created_dt: datetime.datetime
-        if isinstance(_created_dt, Unset):
-            created_dt = UNSET
+        results = []
+        _results = d.pop("results", UNSET)
+        if _results is UNSET:
+            results = UNSET
         else:
-            created_dt = isoparse(_created_dt)
+            for results_item_data in _results or []:
+                _results_item = results_item_data
+                results_item: FlawPackageVersion
+                if isinstance(_results_item, Unset):
+                    results_item = UNSET
+                else:
+                    results_item = FlawPackageVersion.from_dict(_results_item)
 
-        _updated_dt = d.pop("updated_dt", UNSET)
-        updated_dt: datetime.datetime
-        if isinstance(_updated_dt, Unset):
-            updated_dt = UNSET
-        else:
-            updated_dt = isoparse(_updated_dt)
+                results.append(results_item)
 
         _dt = d.pop("dt", UNSET)
         dt: Union[Unset, datetime.datetime]
         if isinstance(_dt, Unset):
             dt = UNSET
         else:
             dt = isoparse(_dt)
 
         env = d.pop("env", UNSET)
 
         revision = d.pop("revision", UNSET)
 
         version = d.pop("version", UNSET)
 
-        osidb_api_v1_flaws_acknowledgments_update_response_200 = cls(
-            name=name,
-            affiliation=affiliation,
-            from_upstream=from_upstream,
-            flaw=flaw,
-            uuid=uuid,
-            embargoed=embargoed,
-            created_dt=created_dt,
-            updated_dt=updated_dt,
+        osidb_api_v1_flaws_package_versions_list_response_200 = cls(
+            count=count,
+            next_=next_,
+            previous=previous,
+            results=results,
             dt=dt,
             env=env,
             revision=revision,
             version=version,
         )
 
-        osidb_api_v1_flaws_acknowledgments_update_response_200.additional_properties = d
-        return osidb_api_v1_flaws_acknowledgments_update_response_200
+        osidb_api_v1_flaws_package_versions_list_response_200.additional_properties = d
+        return osidb_api_v1_flaws_package_versions_list_response_200
 
     @staticmethod
     def get_fields():
         return {
-            "name": str,
-            "affiliation": str,
-            "from_upstream": bool,
-            "flaw": str,
-            "uuid": str,
-            "embargoed": bool,
-            "created_dt": datetime.datetime,
-            "updated_dt": datetime.datetime,
+            "count": int,
+            "next": str,
+            "previous": str,
+            "results": List[FlawPackageVersion],
             "dt": datetime.datetime,
             "env": str,
             "revision": str,
             "version": str,
         }
 
     @property
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_create_response_201.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_retrieve_response_200.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.flaw_comment_alerts import FlawCommentAlerts
 from ..models.flaw_comment_type import FlawCommentType
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="OsidbApiV1FlawsCommentsCreateResponse201")
+T = TypeVar("T", bound="OsidbApiV1FlawsCommentsRetrieveResponse200")
 
 
 @attr.s(auto_attribs=True)
-class OsidbApiV1FlawsCommentsCreateResponse201(OSIDBModel):
+class OsidbApiV1FlawsCommentsRetrieveResponse200(OSIDBModel):
     """ """
 
     flaw: str
     text: str
     uuid: str
     external_system_id: str
+    alerts: FlawCommentAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     embargoed: bool
     type: Union[Unset, FlawCommentType] = UNSET
     order: Union[Unset, None, int] = UNSET
     dt: Union[Unset, datetime.datetime] = UNSET
     env: Union[Unset, str] = UNSET
@@ -30,14 +32,18 @@
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         flaw = self.flaw
         text = self.text
         uuid = self.uuid
         external_system_id = self.external_system_id
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
@@ -63,14 +69,16 @@
             field_dict["flaw"] = flaw
         if not isinstance(text, Unset):
             field_dict["text"] = text
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(external_system_id, Unset):
             field_dict["external_system_id"] = external_system_id
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
         if not isinstance(type, Unset):
@@ -95,14 +103,21 @@
 
         text = d.pop("text", UNSET)
 
         uuid = d.pop("uuid", UNSET)
 
         external_system_id = d.pop("external_system_id", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawCommentAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawCommentAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
@@ -133,40 +148,42 @@
 
         env = d.pop("env", UNSET)
 
         revision = d.pop("revision", UNSET)
 
         version = d.pop("version", UNSET)
 
-        osidb_api_v1_flaws_comments_create_response_201 = cls(
+        osidb_api_v1_flaws_comments_retrieve_response_200 = cls(
             flaw=flaw,
             text=text,
             uuid=uuid,
             external_system_id=external_system_id,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
             embargoed=embargoed,
             type=type,
             order=order,
             dt=dt,
             env=env,
             revision=revision,
             version=version,
         )
 
-        osidb_api_v1_flaws_comments_create_response_201.additional_properties = d
-        return osidb_api_v1_flaws_comments_create_response_201
+        osidb_api_v1_flaws_comments_retrieve_response_200.additional_properties = d
+        return osidb_api_v1_flaws_comments_retrieve_response_200
 
     @staticmethod
     def get_fields():
         return {
             "flaw": str,
             "text": str,
             "uuid": str,
             "external_system_id": str,
+            "alerts": FlawCommentAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "embargoed": bool,
             "type": FlawCommentType,
             "order": int,
             "dt": datetime.datetime,
             "env": str,
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_list_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_create_response_201.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_create_response_201.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import attr
 from dateutil.parser import isoparse
 
 from ..models.affect import Affect
 from ..models.blank_enum import BlankEnum
 from ..models.comment import Comment
 from ..models.flaw_acknowledgment import FlawAcknowledgment
+from ..models.flaw_alerts import FlawAlerts
 from ..models.flaw_classification import FlawClassification
 from ..models.flaw_cvss import FlawCVSS
 from ..models.flaw_meta_attr import FlawMetaAttr
 from ..models.flaw_reference import FlawReference
 from ..models.flaw_type import FlawType
 from ..models.impact_enum import ImpactEnum
 from ..models.major_incident_state_enum import MajorIncidentStateEnum
@@ -43,18 +44,20 @@
     acknowledgments: List[FlawAcknowledgment]
     references: List[FlawReference]
     cvss_scores: List[FlawCVSS]
     embargoed: bool
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     classification: FlawClassification
+    alerts: FlawAlerts
     type: Union[Unset, FlawType] = UNSET
     cve_id: Union[Unset, None, str] = UNSET
     impact: Union[BlankEnum, ImpactEnum, Unset] = UNSET
     component: Union[Unset, str] = UNSET
+    components: Union[Unset, List[str]] = UNSET
     summary: Union[Unset, str] = UNSET
     requires_summary: Union[BlankEnum, RequiresSummaryEnum, Unset] = UNSET
     statement: Union[Unset, str] = UNSET
     cwe_id: Union[Unset, str] = UNSET
     unembargo_dt: Union[Unset, None, datetime.datetime] = UNSET
     source: Union[BlankEnum, Source8D8Enum, Unset] = UNSET
     reported_dt: Union[Unset, None, datetime.datetime] = UNSET
@@ -171,14 +174,18 @@
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
         classification: Dict[str, Any] = UNSET
         if not isinstance(self.classification, Unset):
             classification = self.classification.to_dict()
 
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         type: Union[Unset, str] = UNSET
         if not isinstance(self.type, Unset):
 
             type = FlawType(self.type).value
 
         cve_id = self.cve_id
         impact: Union[Unset, str]
@@ -193,14 +200,18 @@
         else:
             impact = UNSET
             if not isinstance(self.impact, Unset):
 
                 impact = BlankEnum(self.impact).value
 
         component = self.component
+        components: Union[Unset, List[str]] = UNSET
+        if not isinstance(self.components, Unset):
+            components = self.components
+
         summary = self.summary
         requires_summary: Union[Unset, str]
         if isinstance(self.requires_summary, Unset):
             requires_summary = UNSET
         elif isinstance(self.requires_summary, RequiresSummaryEnum):
             requires_summary = UNSET
             if not isinstance(self.requires_summary, Unset):
@@ -326,22 +337,26 @@
             field_dict["embargoed"] = embargoed
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(classification, Unset):
             field_dict["classification"] = classification
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(type, Unset):
             field_dict["type"] = type
         if not isinstance(cve_id, Unset):
             field_dict["cve_id"] = cve_id
         if not isinstance(impact, Unset):
             field_dict["impact"] = impact
         if not isinstance(component, Unset):
             field_dict["component"] = component
+        if not isinstance(components, Unset):
+            field_dict["components"] = components
         if not isinstance(summary, Unset):
             field_dict["summary"] = summary
         if not isinstance(requires_summary, Unset):
             field_dict["requires_summary"] = requires_summary
         if not isinstance(statement, Unset):
             field_dict["statement"] = statement
         if not isinstance(cwe_id, Unset):
@@ -539,14 +554,21 @@
         _classification = d.pop("classification", UNSET)
         classification: FlawClassification
         if isinstance(_classification, Unset):
             classification = UNSET
         else:
             classification = FlawClassification.from_dict(_classification)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawAlerts.from_dict(_alerts)
+
         _type = d.pop("type", UNSET)
         type: Union[Unset, FlawType]
         if isinstance(_type, Unset):
             type = UNSET
         else:
             type = FlawType(_type)
 
@@ -579,14 +601,16 @@
 
             return impact_type_1
 
         impact = _parse_impact(d.pop("impact", UNSET))
 
         component = d.pop("component", UNSET)
 
+        components = cast(List[str], d.pop("components", UNSET))
+
         summary = d.pop("summary", UNSET)
 
         def _parse_requires_summary(
             data: object,
         ) -> Union[BlankEnum, RequiresSummaryEnum, Unset]:
             if isinstance(data, Unset):
                 return data
@@ -791,18 +815,20 @@
             acknowledgments=acknowledgments,
             references=references,
             cvss_scores=cvss_scores,
             embargoed=embargoed,
             created_dt=created_dt,
             updated_dt=updated_dt,
             classification=classification,
+            alerts=alerts,
             type=type,
             cve_id=cve_id,
             impact=impact,
             component=component,
+            components=components,
             summary=summary,
             requires_summary=requires_summary,
             statement=statement,
             cwe_id=cwe_id,
             unembargo_dt=unembargo_dt,
             source=source,
             reported_dt=reported_dt,
@@ -846,18 +872,20 @@
             "acknowledgments": List[FlawAcknowledgment],
             "references": List[FlawReference],
             "cvss_scores": List[FlawCVSS],
             "embargoed": bool,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "classification": FlawClassification,
+            "alerts": FlawAlerts,
             "type": FlawType,
             "cve_id": str,
             "impact": Union[BlankEnum, ImpactEnum],
             "component": str,
+            "components": List[str],
             "summary": str,
             "requires_summary": Union[BlankEnum, RequiresSummaryEnum],
             "statement": str,
             "cwe_id": str,
             "unembargo_dt": datetime.datetime,
             "source": Union[BlankEnum, Source8D8Enum],
             "reported_dt": datetime.datetime,
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_cvss_scores_create_response_201.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_create_response_201.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,118 +1,122 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.issuer_enum import IssuerEnum
+from ..models.flaw_comment_alerts import FlawCommentAlerts
+from ..models.flaw_comment_type import FlawCommentType
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="OsidbApiV1FlawsCvssScoresCreateResponse201")
+T = TypeVar("T", bound="OsidbApiV1FlawsCommentsCreateResponse201")
 
 
 @attr.s(auto_attribs=True)
-class OsidbApiV1FlawsCvssScoresCreateResponse201(OSIDBModel):
+class OsidbApiV1FlawsCommentsCreateResponse201(OSIDBModel):
     """ """
 
-    cvss_version: str
-    issuer: IssuerEnum
+    flaw: str
+    text: str
     uuid: str
-    vector: str
-    embargoed: bool
+    external_system_id: str
+    alerts: FlawCommentAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
-    comment: Union[Unset, str] = UNSET
-    flaw: Union[Unset, str] = UNSET
-    score: Union[Unset, float] = UNSET
+    embargoed: bool
+    type: Union[Unset, FlawCommentType] = UNSET
+    order: Union[Unset, None, int] = UNSET
     dt: Union[Unset, datetime.datetime] = UNSET
     env: Union[Unset, str] = UNSET
     revision: Union[Unset, str] = UNSET
     version: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        cvss_version = self.cvss_version
-        issuer: str = UNSET
-        if not isinstance(self.issuer, Unset):
-
-            issuer = IssuerEnum(self.issuer).value
-
+        flaw = self.flaw
+        text = self.text
         uuid = self.uuid
-        vector = self.vector
-        embargoed = self.embargoed
+        external_system_id = self.external_system_id
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
-        comment = self.comment
-        flaw = self.flaw
-        score = self.score
+        embargoed = self.embargoed
+        type: Union[Unset, str] = UNSET
+        if not isinstance(self.type, Unset):
+
+            type = FlawCommentType(self.type).value
+
+        order = self.order
         dt: Union[Unset, str] = UNSET
         if not isinstance(self.dt, Unset):
             dt = self.dt.isoformat()
 
         env = self.env
         revision = self.revision
         version = self.version
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        if not isinstance(cvss_version, Unset):
-            field_dict["cvss_version"] = cvss_version
-        if not isinstance(issuer, Unset):
-            field_dict["issuer"] = issuer
+        if not isinstance(flaw, Unset):
+            field_dict["flaw"] = flaw
+        if not isinstance(text, Unset):
+            field_dict["text"] = text
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
-        if not isinstance(vector, Unset):
-            field_dict["vector"] = vector
-        if not isinstance(embargoed, Unset):
-            field_dict["embargoed"] = embargoed
+        if not isinstance(external_system_id, Unset):
+            field_dict["external_system_id"] = external_system_id
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
-        if not isinstance(comment, Unset):
-            field_dict["comment"] = comment
-        if not isinstance(flaw, Unset):
-            field_dict["flaw"] = flaw
-        if not isinstance(score, Unset):
-            field_dict["score"] = score
+        if not isinstance(embargoed, Unset):
+            field_dict["embargoed"] = embargoed
+        if not isinstance(type, Unset):
+            field_dict["type"] = type
+        if not isinstance(order, Unset):
+            field_dict["order"] = order
         if not isinstance(dt, Unset):
             field_dict["dt"] = dt
         if not isinstance(env, Unset):
             field_dict["env"] = env
         if not isinstance(revision, Unset):
             field_dict["revision"] = revision
         if not isinstance(version, Unset):
             field_dict["version"] = version
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        cvss_version = d.pop("cvss_version", UNSET)
+        flaw = d.pop("flaw", UNSET)
 
-        _issuer = d.pop("issuer", UNSET)
-        issuer: IssuerEnum
-        if isinstance(_issuer, Unset):
-            issuer = UNSET
-        else:
-            issuer = IssuerEnum(_issuer)
+        text = d.pop("text", UNSET)
 
         uuid = d.pop("uuid", UNSET)
 
-        vector = d.pop("vector", UNSET)
+        external_system_id = d.pop("external_system_id", UNSET)
 
-        embargoed = d.pop("embargoed", UNSET)
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawCommentAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawCommentAlerts.from_dict(_alerts)
 
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
@@ -120,66 +124,71 @@
         _updated_dt = d.pop("updated_dt", UNSET)
         updated_dt: datetime.datetime
         if isinstance(_updated_dt, Unset):
             updated_dt = UNSET
         else:
             updated_dt = isoparse(_updated_dt)
 
-        comment = d.pop("comment", UNSET)
+        embargoed = d.pop("embargoed", UNSET)
 
-        flaw = d.pop("flaw", UNSET)
+        _type = d.pop("type", UNSET)
+        type: Union[Unset, FlawCommentType]
+        if isinstance(_type, Unset):
+            type = UNSET
+        else:
+            type = FlawCommentType(_type)
 
-        score = d.pop("score", UNSET)
+        order = d.pop("order", UNSET)
 
         _dt = d.pop("dt", UNSET)
         dt: Union[Unset, datetime.datetime]
         if isinstance(_dt, Unset):
             dt = UNSET
         else:
             dt = isoparse(_dt)
 
         env = d.pop("env", UNSET)
 
         revision = d.pop("revision", UNSET)
 
         version = d.pop("version", UNSET)
 
-        osidb_api_v1_flaws_cvss_scores_create_response_201 = cls(
-            cvss_version=cvss_version,
-            issuer=issuer,
+        osidb_api_v1_flaws_comments_create_response_201 = cls(
+            flaw=flaw,
+            text=text,
             uuid=uuid,
-            vector=vector,
-            embargoed=embargoed,
+            external_system_id=external_system_id,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
-            comment=comment,
-            flaw=flaw,
-            score=score,
+            embargoed=embargoed,
+            type=type,
+            order=order,
             dt=dt,
             env=env,
             revision=revision,
             version=version,
         )
 
-        osidb_api_v1_flaws_cvss_scores_create_response_201.additional_properties = d
-        return osidb_api_v1_flaws_cvss_scores_create_response_201
+        osidb_api_v1_flaws_comments_create_response_201.additional_properties = d
+        return osidb_api_v1_flaws_comments_create_response_201
 
     @staticmethod
     def get_fields():
         return {
-            "cvss_version": str,
-            "issuer": IssuerEnum,
+            "flaw": str,
+            "text": str,
             "uuid": str,
-            "vector": str,
-            "embargoed": bool,
+            "external_system_id": str,
+            "alerts": FlawCommentAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
-            "comment": str,
-            "flaw": str,
-            "score": float,
+            "embargoed": bool,
+            "type": FlawCommentType,
+            "order": int,
             "dt": datetime.datetime,
             "env": str,
             "revision": str,
             "version": str,
         }
 
     @property
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_cvss_scores_destroy_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_cvss_scores_destroy_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_cvss_scores_list_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_cvss_scores_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_cvss_scores_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_cvss_scores_create_response_201.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,113 +1,133 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.cvss_version_enum import CvssVersionEnum
+from ..models.flaw_cvss_alerts import FlawCVSSAlerts
 from ..models.issuer_enum import IssuerEnum
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="OsidbApiV1FlawsCvssScoresRetrieveResponse200")
+T = TypeVar("T", bound="OsidbApiV1FlawsCvssScoresCreateResponse201")
 
 
 @attr.s(auto_attribs=True)
-class OsidbApiV1FlawsCvssScoresRetrieveResponse200(OSIDBModel):
+class OsidbApiV1FlawsCvssScoresCreateResponse201(OSIDBModel):
     """ """
 
-    cvss_version: str
+    cvss_version: CvssVersionEnum
     issuer: IssuerEnum
+    score: float
     uuid: str
     vector: str
     embargoed: bool
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
+    alerts: FlawCVSSAlerts
     comment: Union[Unset, str] = UNSET
     flaw: Union[Unset, str] = UNSET
-    score: Union[Unset, float] = UNSET
     dt: Union[Unset, datetime.datetime] = UNSET
     env: Union[Unset, str] = UNSET
     revision: Union[Unset, str] = UNSET
     version: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        cvss_version = self.cvss_version
+        cvss_version: str = UNSET
+        if not isinstance(self.cvss_version, Unset):
+
+            cvss_version = CvssVersionEnum(self.cvss_version).value
+
         issuer: str = UNSET
         if not isinstance(self.issuer, Unset):
 
             issuer = IssuerEnum(self.issuer).value
 
+        score = self.score
         uuid = self.uuid
         vector = self.vector
         embargoed = self.embargoed
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         comment = self.comment
         flaw = self.flaw
-        score = self.score
         dt: Union[Unset, str] = UNSET
         if not isinstance(self.dt, Unset):
             dt = self.dt.isoformat()
 
         env = self.env
         revision = self.revision
         version = self.version
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if not isinstance(cvss_version, Unset):
             field_dict["cvss_version"] = cvss_version
         if not isinstance(issuer, Unset):
             field_dict["issuer"] = issuer
+        if not isinstance(score, Unset):
+            field_dict["score"] = score
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(vector, Unset):
             field_dict["vector"] = vector
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(comment, Unset):
             field_dict["comment"] = comment
         if not isinstance(flaw, Unset):
             field_dict["flaw"] = flaw
-        if not isinstance(score, Unset):
-            field_dict["score"] = score
         if not isinstance(dt, Unset):
             field_dict["dt"] = dt
         if not isinstance(env, Unset):
             field_dict["env"] = env
         if not isinstance(revision, Unset):
             field_dict["revision"] = revision
         if not isinstance(version, Unset):
             field_dict["version"] = version
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        cvss_version = d.pop("cvss_version", UNSET)
+        _cvss_version = d.pop("cvss_version", UNSET)
+        cvss_version: CvssVersionEnum
+        if isinstance(_cvss_version, Unset):
+            cvss_version = UNSET
+        else:
+            cvss_version = CvssVersionEnum(_cvss_version)
 
         _issuer = d.pop("issuer", UNSET)
         issuer: IssuerEnum
         if isinstance(_issuer, Unset):
             issuer = UNSET
         else:
             issuer = IssuerEnum(_issuer)
 
+        score = d.pop("score", UNSET)
+
         uuid = d.pop("uuid", UNSET)
 
         vector = d.pop("vector", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
         _created_dt = d.pop("created_dt", UNSET)
@@ -120,66 +140,73 @@
         _updated_dt = d.pop("updated_dt", UNSET)
         updated_dt: datetime.datetime
         if isinstance(_updated_dt, Unset):
             updated_dt = UNSET
         else:
             updated_dt = isoparse(_updated_dt)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawCVSSAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawCVSSAlerts.from_dict(_alerts)
+
         comment = d.pop("comment", UNSET)
 
         flaw = d.pop("flaw", UNSET)
 
-        score = d.pop("score", UNSET)
-
         _dt = d.pop("dt", UNSET)
         dt: Union[Unset, datetime.datetime]
         if isinstance(_dt, Unset):
             dt = UNSET
         else:
             dt = isoparse(_dt)
 
         env = d.pop("env", UNSET)
 
         revision = d.pop("revision", UNSET)
 
         version = d.pop("version", UNSET)
 
-        osidb_api_v1_flaws_cvss_scores_retrieve_response_200 = cls(
+        osidb_api_v1_flaws_cvss_scores_create_response_201 = cls(
             cvss_version=cvss_version,
             issuer=issuer,
+            score=score,
             uuid=uuid,
             vector=vector,
             embargoed=embargoed,
             created_dt=created_dt,
             updated_dt=updated_dt,
+            alerts=alerts,
             comment=comment,
             flaw=flaw,
-            score=score,
             dt=dt,
             env=env,
             revision=revision,
             version=version,
         )
 
-        osidb_api_v1_flaws_cvss_scores_retrieve_response_200.additional_properties = d
-        return osidb_api_v1_flaws_cvss_scores_retrieve_response_200
+        osidb_api_v1_flaws_cvss_scores_create_response_201.additional_properties = d
+        return osidb_api_v1_flaws_cvss_scores_create_response_201
 
     @staticmethod
     def get_fields():
         return {
-            "cvss_version": str,
+            "cvss_version": CvssVersionEnum,
             "issuer": IssuerEnum,
+            "score": float,
             "uuid": str,
             "vector": str,
             "embargoed": bool,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
+            "alerts": FlawCVSSAlerts,
             "comment": str,
             "flaw": str,
-            "score": float,
             "dt": datetime.datetime,
             "env": str,
             "revision": str,
             "version": str,
         }
 
     @property
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_order_item.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_order_item.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,47 +28,58 @@
     VALUE_23 = "-affects__trackers__status"
     VALUE_24 = "-affects__trackers__type"
     VALUE_25 = "-affects__trackers__updated_dt"
     VALUE_26 = "-affects__trackers__uuid"
     VALUE_27 = "-affects__type"
     VALUE_28 = "-affects__updated_dt"
     VALUE_29 = "-affects__uuid"
-    VALUE_30 = "-component"
-    VALUE_31 = "-created_dt"
-    VALUE_32 = "-cve_id"
-    VALUE_33 = "-cvss2"
-    VALUE_34 = "-cvss2_score"
-    VALUE_35 = "-cvss3"
-    VALUE_36 = "-cvss3_score"
-    VALUE_37 = "-cvss_scores__comment"
-    VALUE_38 = "-cvss_scores__created_dt"
-    VALUE_39 = "-cvss_scores__issuer"
-    VALUE_40 = "-cvss_scores__score"
-    VALUE_41 = "-cvss_scores__updated_dt"
-    VALUE_42 = "-cvss_scores__uuid"
-    VALUE_43 = "-cvss_scores__vector"
-    VALUE_44 = "-cwe_id"
-    VALUE_45 = "-impact"
-    VALUE_46 = "-major_incident_state"
-    VALUE_47 = "-nist_cvss_validation"
-    VALUE_48 = "-nvd_cvss2"
-    VALUE_49 = "-nvd_cvss3"
-    VALUE_50 = "-references__created_dt"
-    VALUE_51 = "-references__description"
-    VALUE_52 = "-references__type"
-    VALUE_53 = "-references__updated_dt"
-    VALUE_54 = "-references__url"
-    VALUE_55 = "-references__uuid"
-    VALUE_56 = "-reported_dt"
-    VALUE_57 = "-requires_summary"
-    VALUE_58 = "-source"
-    VALUE_59 = "-type"
-    VALUE_60 = "-unembargo_dt"
-    VALUE_61 = "-updated_dt"
-    VALUE_62 = "-uuid"
+    VALUE_30 = "-bz_id"
+    VALUE_31 = "-component"
+    VALUE_32 = "-components"
+    VALUE_33 = "-created_dt"
+    VALUE_34 = "-cve_id"
+    VALUE_35 = "-cvss2"
+    VALUE_36 = "-cvss2_score"
+    VALUE_37 = "-cvss3"
+    VALUE_38 = "-cvss3_score"
+    VALUE_39 = "-cvss_scores__comment"
+    VALUE_40 = "-cvss_scores__created_dt"
+    VALUE_41 = "-cvss_scores__issuer"
+    VALUE_42 = "-cvss_scores__score"
+    VALUE_43 = "-cvss_scores__updated_dt"
+    VALUE_44 = "-cvss_scores__uuid"
+    VALUE_45 = "-cvss_scores__vector"
+    VALUE_46 = "-cwe_id"
+    VALUE_47 = "-description"
+    VALUE_48 = "-embargoed"
+    VALUE_49 = "-impact"
+    VALUE_50 = "-is_major_incident"
+    VALUE_51 = "-major_incident_state"
+    VALUE_52 = "-nist_cvss_validation"
+    VALUE_53 = "-nvd_cvss2"
+    VALUE_54 = "-nvd_cvss3"
+    VALUE_55 = "-owner"
+    VALUE_56 = "-references__created_dt"
+    VALUE_57 = "-references__description"
+    VALUE_58 = "-references__type"
+    VALUE_59 = "-references__updated_dt"
+    VALUE_60 = "-references__url"
+    VALUE_61 = "-references__uuid"
+    VALUE_62 = "-reported_dt"
+    VALUE_63 = "-requires_summary"
+    VALUE_64 = "-source"
+    VALUE_65 = "-statement"
+    VALUE_66 = "-summary"
+    VALUE_67 = "-team_id"
+    VALUE_68 = "-title"
+    VALUE_69 = "-type"
+    VALUE_70 = "-unembargo_dt"
+    VALUE_71 = "-updated_dt"
+    VALUE_72 = "-uuid"
+    VALUE_73 = "-workflow_state"
     ACKNOWLEDGMENTS_AFFILIATION = "acknowledgments__affiliation"
     ACKNOWLEDGMENTS_CREATED_DT = "acknowledgments__created_dt"
     ACKNOWLEDGMENTS_FROM_UPSTREAM = "acknowledgments__from_upstream"
     ACKNOWLEDGMENTS_NAME = "acknowledgments__name"
     ACKNOWLEDGMENTS_UPDATED_DT = "acknowledgments__updated_dt"
     ACKNOWLEDGMENTS_UUID = "acknowledgments__uuid"
     AFFECTS_AFFECTEDNESS = "affects__affectedness"
@@ -91,43 +102,54 @@
     AFFECTS_TRACKERS_STATUS = "affects__trackers__status"
     AFFECTS_TRACKERS_TYPE = "affects__trackers__type"
     AFFECTS_TRACKERS_UPDATED_DT = "affects__trackers__updated_dt"
     AFFECTS_TRACKERS_UUID = "affects__trackers__uuid"
     AFFECTS_TYPE = "affects__type"
     AFFECTS_UPDATED_DT = "affects__updated_dt"
     AFFECTS_UUID = "affects__uuid"
+    BZ_ID = "bz_id"
     COMPONENT = "component"
+    COMPONENTS = "components"
     CREATED_DT = "created_dt"
     CVE_ID = "cve_id"
     CVSS2 = "cvss2"
     CVSS2_SCORE = "cvss2_score"
     CVSS3 = "cvss3"
     CVSS3_SCORE = "cvss3_score"
     CVSS_SCORES_COMMENT = "cvss_scores__comment"
     CVSS_SCORES_CREATED_DT = "cvss_scores__created_dt"
     CVSS_SCORES_ISSUER = "cvss_scores__issuer"
     CVSS_SCORES_SCORE = "cvss_scores__score"
     CVSS_SCORES_UPDATED_DT = "cvss_scores__updated_dt"
     CVSS_SCORES_UUID = "cvss_scores__uuid"
     CVSS_SCORES_VECTOR = "cvss_scores__vector"
     CWE_ID = "cwe_id"
+    DESCRIPTION = "description"
+    EMBARGOED = "embargoed"
     IMPACT = "impact"
+    IS_MAJOR_INCIDENT = "is_major_incident"
     MAJOR_INCIDENT_STATE = "major_incident_state"
     NIST_CVSS_VALIDATION = "nist_cvss_validation"
     NVD_CVSS2 = "nvd_cvss2"
     NVD_CVSS3 = "nvd_cvss3"
+    OWNER = "owner"
     REFERENCES_CREATED_DT = "references__created_dt"
     REFERENCES_DESCRIPTION = "references__description"
     REFERENCES_TYPE = "references__type"
     REFERENCES_UPDATED_DT = "references__updated_dt"
     REFERENCES_URL = "references__url"
     REFERENCES_UUID = "references__uuid"
     REPORTED_DT = "reported_dt"
     REQUIRES_SUMMARY = "requires_summary"
     SOURCE = "source"
+    STATEMENT = "statement"
+    SUMMARY = "summary"
+    TEAM_ID = "team_id"
+    TITLE = "title"
     TYPE = "type"
     UNEMBARGO_DT = "unembargo_dt"
     UPDATED_DT = "updated_dt"
     UUID = "uuid"
+    WORKFLOW_STATE = "workflow_state"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_source.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_source.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_package_versions_destroy_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_package_versions_destroy_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_package_versions_list_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_list_response_200.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.flaw_package_version import FlawPackageVersion
+from ..models.flaw_reference import FlawReference
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="OsidbApiV1FlawsPackageVersionsListResponse200")
+T = TypeVar("T", bound="OsidbApiV1FlawsReferencesListResponse200")
 
 
 @attr.s(auto_attribs=True)
-class OsidbApiV1FlawsPackageVersionsListResponse200(OSIDBModel):
+class OsidbApiV1FlawsReferencesListResponse200(OSIDBModel):
     """ """
 
     count: Union[Unset, int] = UNSET
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List[FlawPackageVersion]] = UNSET
+    results: Union[Unset, List[FlawReference]] = UNSET
     dt: Union[Unset, datetime.datetime] = UNSET
     env: Union[Unset, str] = UNSET
     revision: Union[Unset, str] = UNSET
     version: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
@@ -79,19 +79,19 @@
         results = []
         _results = d.pop("results", UNSET)
         if _results is UNSET:
             results = UNSET
         else:
             for results_item_data in _results or []:
                 _results_item = results_item_data
-                results_item: FlawPackageVersion
+                results_item: FlawReference
                 if isinstance(_results_item, Unset):
                     results_item = UNSET
                 else:
-                    results_item = FlawPackageVersion.from_dict(_results_item)
+                    results_item = FlawReference.from_dict(_results_item)
 
                 results.append(results_item)
 
         _dt = d.pop("dt", UNSET)
         dt: Union[Unset, datetime.datetime]
         if isinstance(_dt, Unset):
             dt = UNSET
@@ -100,35 +100,35 @@
 
         env = d.pop("env", UNSET)
 
         revision = d.pop("revision", UNSET)
 
         version = d.pop("version", UNSET)
 
-        osidb_api_v1_flaws_package_versions_list_response_200 = cls(
+        osidb_api_v1_flaws_references_list_response_200 = cls(
             count=count,
             next_=next_,
             previous=previous,
             results=results,
             dt=dt,
             env=env,
             revision=revision,
             version=version,
         )
 
-        osidb_api_v1_flaws_package_versions_list_response_200.additional_properties = d
-        return osidb_api_v1_flaws_package_versions_list_response_200
+        osidb_api_v1_flaws_references_list_response_200.additional_properties = d
+        return osidb_api_v1_flaws_references_list_response_200
 
     @staticmethod
     def get_fields():
         return {
             "count": int,
             "next": str,
             "previous": str,
-            "results": List[FlawPackageVersion],
+            "results": List[FlawReference],
             "dt": datetime.datetime,
             "env": str,
             "revision": str,
             "version": str,
         }
 
     @property
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_promote_create_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_promote_create_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_create_response_201.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_create_response_201.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.flaw_reference_alerts import FlawReferenceAlerts
 from ..models.flaw_reference_type import FlawReferenceType
 from ..types import UNSET, OSIDBModel, Unset
 
 T = TypeVar("T", bound="OsidbApiV1FlawsReferencesCreateResponse201")
 
 
 @attr.s(auto_attribs=True)
 class OsidbApiV1FlawsReferencesCreateResponse201(OSIDBModel):
     """ """
 
     flaw: str
     url: str
     uuid: str
     embargoed: bool
+    alerts: FlawReferenceAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     description: Union[Unset, str] = UNSET
     type: Union[Unset, FlawReferenceType] = UNSET
     dt: Union[Unset, datetime.datetime] = UNSET
     env: Union[Unset, str] = UNSET
     revision: Union[Unset, str] = UNSET
@@ -29,14 +31,18 @@
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         flaw = self.flaw
         url = self.url
         uuid = self.uuid
         embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
@@ -61,14 +67,16 @@
             field_dict["flaw"] = flaw
         if not isinstance(url, Unset):
             field_dict["url"] = url
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(description, Unset):
             field_dict["description"] = description
         if not isinstance(type, Unset):
@@ -91,14 +99,21 @@
 
         url = d.pop("url", UNSET)
 
         uuid = d.pop("uuid", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawReferenceAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawReferenceAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
@@ -132,14 +147,15 @@
         version = d.pop("version", UNSET)
 
         osidb_api_v1_flaws_references_create_response_201 = cls(
             flaw=flaw,
             url=url,
             uuid=uuid,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
             description=description,
             type=type,
             dt=dt,
             env=env,
             revision=revision,
@@ -152,14 +168,15 @@
     @staticmethod
     def get_fields():
         return {
             "flaw": str,
             "url": str,
             "uuid": str,
             "embargoed": bool,
+            "alerts": FlawReferenceAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "description": str,
             "type": FlawReferenceType,
             "dt": datetime.datetime,
             "env": str,
             "revision": str,
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_destroy_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_destroy_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_list_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_response_200.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.flaw_reference import FlawReference
+from ..models.tracker import Tracker
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="OsidbApiV1FlawsReferencesListResponse200")
+T = TypeVar("T", bound="OsidbApiV1TrackersListResponse200")
 
 
 @attr.s(auto_attribs=True)
-class OsidbApiV1FlawsReferencesListResponse200(OSIDBModel):
+class OsidbApiV1TrackersListResponse200(OSIDBModel):
     """ """
 
     count: Union[Unset, int] = UNSET
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List[FlawReference]] = UNSET
+    results: Union[Unset, List[Tracker]] = UNSET
     dt: Union[Unset, datetime.datetime] = UNSET
     env: Union[Unset, str] = UNSET
     revision: Union[Unset, str] = UNSET
     version: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
@@ -79,19 +79,19 @@
         results = []
         _results = d.pop("results", UNSET)
         if _results is UNSET:
             results = UNSET
         else:
             for results_item_data in _results or []:
                 _results_item = results_item_data
-                results_item: FlawReference
+                results_item: Tracker
                 if isinstance(_results_item, Unset):
                     results_item = UNSET
                 else:
-                    results_item = FlawReference.from_dict(_results_item)
+                    results_item = Tracker.from_dict(_results_item)
 
                 results.append(results_item)
 
         _dt = d.pop("dt", UNSET)
         dt: Union[Unset, datetime.datetime]
         if isinstance(_dt, Unset):
             dt = UNSET
@@ -100,35 +100,35 @@
 
         env = d.pop("env", UNSET)
 
         revision = d.pop("revision", UNSET)
 
         version = d.pop("version", UNSET)
 
-        osidb_api_v1_flaws_references_list_response_200 = cls(
+        osidb_api_v1_trackers_list_response_200 = cls(
             count=count,
             next_=next_,
             previous=previous,
             results=results,
             dt=dt,
             env=env,
             revision=revision,
             version=version,
         )
 
-        osidb_api_v1_flaws_references_list_response_200.additional_properties = d
-        return osidb_api_v1_flaws_references_list_response_200
+        osidb_api_v1_trackers_list_response_200.additional_properties = d
+        return osidb_api_v1_trackers_list_response_200
 
     @staticmethod
     def get_fields():
         return {
             "count": int,
             "next": str,
             "previous": str,
-            "results": List[FlawReference],
+            "results": List[Tracker],
             "dt": datetime.datetime,
             "env": str,
             "revision": str,
             "version": str,
         }
 
     @property
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_update_response_200.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.flaw_reference_alerts import FlawReferenceAlerts
 from ..models.flaw_reference_type import FlawReferenceType
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="OsidbApiV1FlawsReferencesRetrieveResponse200")
+T = TypeVar("T", bound="OsidbApiV1FlawsReferencesUpdateResponse200")
 
 
 @attr.s(auto_attribs=True)
-class OsidbApiV1FlawsReferencesRetrieveResponse200(OSIDBModel):
+class OsidbApiV1FlawsReferencesUpdateResponse200(OSIDBModel):
     """ """
 
     flaw: str
     url: str
     uuid: str
     embargoed: bool
+    alerts: FlawReferenceAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     description: Union[Unset, str] = UNSET
     type: Union[Unset, FlawReferenceType] = UNSET
     dt: Union[Unset, datetime.datetime] = UNSET
     env: Union[Unset, str] = UNSET
     revision: Union[Unset, str] = UNSET
@@ -29,14 +31,18 @@
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         flaw = self.flaw
         url = self.url
         uuid = self.uuid
         embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
@@ -61,14 +67,16 @@
             field_dict["flaw"] = flaw
         if not isinstance(url, Unset):
             field_dict["url"] = url
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(description, Unset):
             field_dict["description"] = description
         if not isinstance(type, Unset):
@@ -91,14 +99,21 @@
 
         url = d.pop("url", UNSET)
 
         uuid = d.pop("uuid", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawReferenceAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawReferenceAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
@@ -127,39 +142,41 @@
 
         env = d.pop("env", UNSET)
 
         revision = d.pop("revision", UNSET)
 
         version = d.pop("version", UNSET)
 
-        osidb_api_v1_flaws_references_retrieve_response_200 = cls(
+        osidb_api_v1_flaws_references_update_response_200 = cls(
             flaw=flaw,
             url=url,
             uuid=uuid,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
             description=description,
             type=type,
             dt=dt,
             env=env,
             revision=revision,
             version=version,
         )
 
-        osidb_api_v1_flaws_references_retrieve_response_200.additional_properties = d
-        return osidb_api_v1_flaws_references_retrieve_response_200
+        osidb_api_v1_flaws_references_update_response_200.additional_properties = d
+        return osidb_api_v1_flaws_references_update_response_200
 
     @staticmethod
     def get_fields():
         return {
             "flaw": str,
             "url": str,
             "uuid": str,
             "embargoed": bool,
+            "alerts": FlawReferenceAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "description": str,
             "type": FlawReferenceType,
             "dt": datetime.datetime,
             "env": str,
             "revision": str,
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_update_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_comment_post.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,173 +1,184 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union
+import json
+from typing import Any, Dict, List, Tuple, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.flaw_reference_type import FlawReferenceType
+from ..models.flaw_comment_post_alerts import FlawCommentPostAlerts
+from ..models.flaw_comment_post_meta_attr import FlawCommentPostMetaAttr
+from ..models.flaw_comment_type import FlawCommentType
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="OsidbApiV1FlawsReferencesUpdateResponse200")
+T = TypeVar("T", bound="FlawCommentPost")
 
 
 @attr.s(auto_attribs=True)
-class OsidbApiV1FlawsReferencesUpdateResponse200(OSIDBModel):
-    """ """
+class FlawCommentPost(OSIDBModel):
+    """FlawComment serializer for use by flaw_comments endpoint"""
 
-    flaw: str
-    url: str
+    text: str
     uuid: str
-    embargoed: bool
+    alerts: FlawCommentPostAlerts
     created_dt: datetime.datetime
-    updated_dt: datetime.datetime
-    description: Union[Unset, str] = UNSET
-    type: Union[Unset, FlawReferenceType] = UNSET
-    dt: Union[Unset, datetime.datetime] = UNSET
-    env: Union[Unset, str] = UNSET
-    revision: Union[Unset, str] = UNSET
-    version: Union[Unset, str] = UNSET
+    embargoed: bool
+    type: Union[Unset, FlawCommentType] = UNSET
+    meta_attr: Union[Unset, FlawCommentPostMetaAttr] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        flaw = self.flaw
-        url = self.url
+        text = self.text
         uuid = self.uuid
-        embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
-        updated_dt: str = UNSET
-        if not isinstance(self.updated_dt, Unset):
-            updated_dt = self.updated_dt.isoformat()
-
-        description = self.description
+        embargoed = self.embargoed
         type: Union[Unset, str] = UNSET
         if not isinstance(self.type, Unset):
 
-            type = FlawReferenceType(self.type).value
+            type = FlawCommentType(self.type).value
 
-        dt: Union[Unset, str] = UNSET
-        if not isinstance(self.dt, Unset):
-            dt = self.dt.isoformat()
-
-        env = self.env
-        revision = self.revision
-        version = self.version
+        meta_attr: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.meta_attr, Unset):
+            meta_attr = self.meta_attr.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        if not isinstance(flaw, Unset):
-            field_dict["flaw"] = flaw
-        if not isinstance(url, Unset):
-            field_dict["url"] = url
+        if not isinstance(text, Unset):
+            field_dict["text"] = text
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
+        if not isinstance(created_dt, Unset):
+            field_dict["created_dt"] = created_dt
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(type, Unset):
+            field_dict["type"] = type
+        if not isinstance(meta_attr, Unset):
+            field_dict["meta_attr"] = meta_attr
+
+        return field_dict
+
+    def to_multipart(self) -> Dict[str, Any]:
+        text = self.text if self.text is UNSET else (None, str(self.text), "text/plain")
+        uuid = self.uuid if self.uuid is UNSET else (None, str(self.uuid), "text/plain")
+        alerts: Union[Unset, Tuple[None, str, str]] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = (None, json.dumps(self.alerts.to_dict()), "application/json")
+
+        created_dt: str = UNSET
+        if not isinstance(self.created_dt, Unset):
+            created_dt = self.created_dt.isoformat()
+
+        embargoed = (
+            self.embargoed
+            if self.embargoed is UNSET
+            else (None, str(self.embargoed), "text/plain")
+        )
+        type: Union[Unset, Tuple[None, str, str]] = UNSET
+        if not isinstance(self.type, Unset):
+
+            type = FlawCommentType(self.type).value
+
+        meta_attr: Union[Unset, Tuple[None, str, str]] = UNSET
+        if not isinstance(self.meta_attr, Unset):
+            meta_attr = (None, json.dumps(self.meta_attr.to_dict()), "application/json")
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(
+            {
+                key: (None, str(value), "text/plain")
+                for key, value in self.additional_properties.items()
+            }
+        )
+        if not isinstance(text, Unset):
+            field_dict["text"] = text
+        if not isinstance(uuid, Unset):
+            field_dict["uuid"] = uuid
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
-        if not isinstance(updated_dt, Unset):
-            field_dict["updated_dt"] = updated_dt
-        if not isinstance(description, Unset):
-            field_dict["description"] = description
+        if not isinstance(embargoed, Unset):
+            field_dict["embargoed"] = embargoed
         if not isinstance(type, Unset):
             field_dict["type"] = type
-        if not isinstance(dt, Unset):
-            field_dict["dt"] = dt
-        if not isinstance(env, Unset):
-            field_dict["env"] = env
-        if not isinstance(revision, Unset):
-            field_dict["revision"] = revision
-        if not isinstance(version, Unset):
-            field_dict["version"] = version
+        if not isinstance(meta_attr, Unset):
+            field_dict["meta_attr"] = meta_attr
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        flaw = d.pop("flaw", UNSET)
-
-        url = d.pop("url", UNSET)
+        text = d.pop("text", UNSET)
 
         uuid = d.pop("uuid", UNSET)
 
-        embargoed = d.pop("embargoed", UNSET)
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawCommentPostAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawCommentPostAlerts.from_dict(_alerts)
 
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
-        _updated_dt = d.pop("updated_dt", UNSET)
-        updated_dt: datetime.datetime
-        if isinstance(_updated_dt, Unset):
-            updated_dt = UNSET
-        else:
-            updated_dt = isoparse(_updated_dt)
-
-        description = d.pop("description", UNSET)
+        embargoed = d.pop("embargoed", UNSET)
 
         _type = d.pop("type", UNSET)
-        type: Union[Unset, FlawReferenceType]
+        type: Union[Unset, FlawCommentType]
         if isinstance(_type, Unset):
             type = UNSET
         else:
-            type = FlawReferenceType(_type)
+            type = FlawCommentType(_type)
 
-        _dt = d.pop("dt", UNSET)
-        dt: Union[Unset, datetime.datetime]
-        if isinstance(_dt, Unset):
-            dt = UNSET
+        _meta_attr = d.pop("meta_attr", UNSET)
+        meta_attr: Union[Unset, FlawCommentPostMetaAttr]
+        if isinstance(_meta_attr, Unset):
+            meta_attr = UNSET
         else:
-            dt = isoparse(_dt)
-
-        env = d.pop("env", UNSET)
-
-        revision = d.pop("revision", UNSET)
+            meta_attr = FlawCommentPostMetaAttr.from_dict(_meta_attr)
 
-        version = d.pop("version", UNSET)
-
-        osidb_api_v1_flaws_references_update_response_200 = cls(
-            flaw=flaw,
-            url=url,
+        flaw_comment_post = cls(
+            text=text,
             uuid=uuid,
-            embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
-            updated_dt=updated_dt,
-            description=description,
+            embargoed=embargoed,
             type=type,
-            dt=dt,
-            env=env,
-            revision=revision,
-            version=version,
+            meta_attr=meta_attr,
         )
 
-        osidb_api_v1_flaws_references_update_response_200.additional_properties = d
-        return osidb_api_v1_flaws_references_update_response_200
+        flaw_comment_post.additional_properties = d
+        return flaw_comment_post
 
     @staticmethod
     def get_fields():
         return {
-            "flaw": str,
-            "url": str,
+            "text": str,
             "uuid": str,
-            "embargoed": bool,
+            "alerts": FlawCommentPostAlerts,
             "created_dt": datetime.datetime,
-            "updated_dt": datetime.datetime,
-            "description": str,
-            "type": FlawReferenceType,
-            "dt": datetime.datetime,
-            "env": str,
-            "revision": str,
-            "version": str,
+            "embargoed": bool,
+            "type": FlawCommentType,
+            "meta_attr": FlawCommentPostMetaAttr,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_reject_create_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_reject_create_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_retrieve_response_200.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import attr
 from dateutil.parser import isoparse
 
 from ..models.affect import Affect
 from ..models.blank_enum import BlankEnum
 from ..models.comment import Comment
 from ..models.flaw_acknowledgment import FlawAcknowledgment
+from ..models.flaw_alerts import FlawAlerts
 from ..models.flaw_classification import FlawClassification
 from ..models.flaw_cvss import FlawCVSS
 from ..models.flaw_meta_attr import FlawMetaAttr
 from ..models.flaw_reference import FlawReference
 from ..models.flaw_type import FlawType
 from ..models.impact_enum import ImpactEnum
 from ..models.major_incident_state_enum import MajorIncidentStateEnum
@@ -43,18 +44,20 @@
     acknowledgments: List[FlawAcknowledgment]
     references: List[FlawReference]
     cvss_scores: List[FlawCVSS]
     embargoed: bool
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     classification: FlawClassification
+    alerts: FlawAlerts
     type: Union[Unset, FlawType] = UNSET
     cve_id: Union[Unset, None, str] = UNSET
     impact: Union[BlankEnum, ImpactEnum, Unset] = UNSET
     component: Union[Unset, str] = UNSET
+    components: Union[Unset, List[str]] = UNSET
     summary: Union[Unset, str] = UNSET
     requires_summary: Union[BlankEnum, RequiresSummaryEnum, Unset] = UNSET
     statement: Union[Unset, str] = UNSET
     cwe_id: Union[Unset, str] = UNSET
     unembargo_dt: Union[Unset, None, datetime.datetime] = UNSET
     source: Union[BlankEnum, Source8D8Enum, Unset] = UNSET
     reported_dt: Union[Unset, None, datetime.datetime] = UNSET
@@ -171,14 +174,18 @@
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
         classification: Dict[str, Any] = UNSET
         if not isinstance(self.classification, Unset):
             classification = self.classification.to_dict()
 
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         type: Union[Unset, str] = UNSET
         if not isinstance(self.type, Unset):
 
             type = FlawType(self.type).value
 
         cve_id = self.cve_id
         impact: Union[Unset, str]
@@ -193,14 +200,18 @@
         else:
             impact = UNSET
             if not isinstance(self.impact, Unset):
 
                 impact = BlankEnum(self.impact).value
 
         component = self.component
+        components: Union[Unset, List[str]] = UNSET
+        if not isinstance(self.components, Unset):
+            components = self.components
+
         summary = self.summary
         requires_summary: Union[Unset, str]
         if isinstance(self.requires_summary, Unset):
             requires_summary = UNSET
         elif isinstance(self.requires_summary, RequiresSummaryEnum):
             requires_summary = UNSET
             if not isinstance(self.requires_summary, Unset):
@@ -326,22 +337,26 @@
             field_dict["embargoed"] = embargoed
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(classification, Unset):
             field_dict["classification"] = classification
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(type, Unset):
             field_dict["type"] = type
         if not isinstance(cve_id, Unset):
             field_dict["cve_id"] = cve_id
         if not isinstance(impact, Unset):
             field_dict["impact"] = impact
         if not isinstance(component, Unset):
             field_dict["component"] = component
+        if not isinstance(components, Unset):
+            field_dict["components"] = components
         if not isinstance(summary, Unset):
             field_dict["summary"] = summary
         if not isinstance(requires_summary, Unset):
             field_dict["requires_summary"] = requires_summary
         if not isinstance(statement, Unset):
             field_dict["statement"] = statement
         if not isinstance(cwe_id, Unset):
@@ -539,14 +554,21 @@
         _classification = d.pop("classification", UNSET)
         classification: FlawClassification
         if isinstance(_classification, Unset):
             classification = UNSET
         else:
             classification = FlawClassification.from_dict(_classification)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawAlerts.from_dict(_alerts)
+
         _type = d.pop("type", UNSET)
         type: Union[Unset, FlawType]
         if isinstance(_type, Unset):
             type = UNSET
         else:
             type = FlawType(_type)
 
@@ -579,14 +601,16 @@
 
             return impact_type_1
 
         impact = _parse_impact(d.pop("impact", UNSET))
 
         component = d.pop("component", UNSET)
 
+        components = cast(List[str], d.pop("components", UNSET))
+
         summary = d.pop("summary", UNSET)
 
         def _parse_requires_summary(
             data: object,
         ) -> Union[BlankEnum, RequiresSummaryEnum, Unset]:
             if isinstance(data, Unset):
                 return data
@@ -791,18 +815,20 @@
             acknowledgments=acknowledgments,
             references=references,
             cvss_scores=cvss_scores,
             embargoed=embargoed,
             created_dt=created_dt,
             updated_dt=updated_dt,
             classification=classification,
+            alerts=alerts,
             type=type,
             cve_id=cve_id,
             impact=impact,
             component=component,
+            components=components,
             summary=summary,
             requires_summary=requires_summary,
             statement=statement,
             cwe_id=cwe_id,
             unembargo_dt=unembargo_dt,
             source=source,
             reported_dt=reported_dt,
@@ -846,18 +872,20 @@
             "acknowledgments": List[FlawAcknowledgment],
             "references": List[FlawReference],
             "cvss_scores": List[FlawCVSS],
             "embargoed": bool,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "classification": FlawClassification,
+            "alerts": FlawAlerts,
             "type": FlawType,
             "cve_id": str,
             "impact": Union[BlankEnum, ImpactEnum],
             "component": str,
+            "components": List[str],
             "summary": str,
             "requires_summary": Union[BlankEnum, RequiresSummaryEnum],
             "statement": str,
             "cwe_id": str,
             "unembargo_dt": datetime.datetime,
             "source": Union[BlankEnum, Source8D8Enum],
             "reported_dt": datetime.datetime,
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_update_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_update_response_200.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import attr
 from dateutil.parser import isoparse
 
 from ..models.affect import Affect
 from ..models.blank_enum import BlankEnum
 from ..models.comment import Comment
 from ..models.flaw_acknowledgment import FlawAcknowledgment
+from ..models.flaw_alerts import FlawAlerts
 from ..models.flaw_classification import FlawClassification
 from ..models.flaw_cvss import FlawCVSS
 from ..models.flaw_meta_attr import FlawMetaAttr
 from ..models.flaw_reference import FlawReference
 from ..models.flaw_type import FlawType
 from ..models.impact_enum import ImpactEnum
 from ..models.major_incident_state_enum import MajorIncidentStateEnum
@@ -43,18 +44,20 @@
     acknowledgments: List[FlawAcknowledgment]
     references: List[FlawReference]
     cvss_scores: List[FlawCVSS]
     embargoed: bool
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     classification: FlawClassification
+    alerts: FlawAlerts
     type: Union[Unset, FlawType] = UNSET
     cve_id: Union[Unset, None, str] = UNSET
     impact: Union[BlankEnum, ImpactEnum, Unset] = UNSET
     component: Union[Unset, str] = UNSET
+    components: Union[Unset, List[str]] = UNSET
     summary: Union[Unset, str] = UNSET
     requires_summary: Union[BlankEnum, RequiresSummaryEnum, Unset] = UNSET
     statement: Union[Unset, str] = UNSET
     cwe_id: Union[Unset, str] = UNSET
     unembargo_dt: Union[Unset, None, datetime.datetime] = UNSET
     source: Union[BlankEnum, Source8D8Enum, Unset] = UNSET
     reported_dt: Union[Unset, None, datetime.datetime] = UNSET
@@ -171,14 +174,18 @@
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
         classification: Dict[str, Any] = UNSET
         if not isinstance(self.classification, Unset):
             classification = self.classification.to_dict()
 
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         type: Union[Unset, str] = UNSET
         if not isinstance(self.type, Unset):
 
             type = FlawType(self.type).value
 
         cve_id = self.cve_id
         impact: Union[Unset, str]
@@ -193,14 +200,18 @@
         else:
             impact = UNSET
             if not isinstance(self.impact, Unset):
 
                 impact = BlankEnum(self.impact).value
 
         component = self.component
+        components: Union[Unset, List[str]] = UNSET
+        if not isinstance(self.components, Unset):
+            components = self.components
+
         summary = self.summary
         requires_summary: Union[Unset, str]
         if isinstance(self.requires_summary, Unset):
             requires_summary = UNSET
         elif isinstance(self.requires_summary, RequiresSummaryEnum):
             requires_summary = UNSET
             if not isinstance(self.requires_summary, Unset):
@@ -326,22 +337,26 @@
             field_dict["embargoed"] = embargoed
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(classification, Unset):
             field_dict["classification"] = classification
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(type, Unset):
             field_dict["type"] = type
         if not isinstance(cve_id, Unset):
             field_dict["cve_id"] = cve_id
         if not isinstance(impact, Unset):
             field_dict["impact"] = impact
         if not isinstance(component, Unset):
             field_dict["component"] = component
+        if not isinstance(components, Unset):
+            field_dict["components"] = components
         if not isinstance(summary, Unset):
             field_dict["summary"] = summary
         if not isinstance(requires_summary, Unset):
             field_dict["requires_summary"] = requires_summary
         if not isinstance(statement, Unset):
             field_dict["statement"] = statement
         if not isinstance(cwe_id, Unset):
@@ -539,14 +554,21 @@
         _classification = d.pop("classification", UNSET)
         classification: FlawClassification
         if isinstance(_classification, Unset):
             classification = UNSET
         else:
             classification = FlawClassification.from_dict(_classification)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: FlawAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = FlawAlerts.from_dict(_alerts)
+
         _type = d.pop("type", UNSET)
         type: Union[Unset, FlawType]
         if isinstance(_type, Unset):
             type = UNSET
         else:
             type = FlawType(_type)
 
@@ -579,14 +601,16 @@
 
             return impact_type_1
 
         impact = _parse_impact(d.pop("impact", UNSET))
 
         component = d.pop("component", UNSET)
 
+        components = cast(List[str], d.pop("components", UNSET))
+
         summary = d.pop("summary", UNSET)
 
         def _parse_requires_summary(
             data: object,
         ) -> Union[BlankEnum, RequiresSummaryEnum, Unset]:
             if isinstance(data, Unset):
                 return data
@@ -791,18 +815,20 @@
             acknowledgments=acknowledgments,
             references=references,
             cvss_scores=cvss_scores,
             embargoed=embargoed,
             created_dt=created_dt,
             updated_dt=updated_dt,
             classification=classification,
+            alerts=alerts,
             type=type,
             cve_id=cve_id,
             impact=impact,
             component=component,
+            components=components,
             summary=summary,
             requires_summary=requires_summary,
             statement=statement,
             cwe_id=cwe_id,
             unembargo_dt=unembargo_dt,
             source=source,
             reported_dt=reported_dt,
@@ -846,18 +872,20 @@
             "acknowledgments": List[FlawAcknowledgment],
             "references": List[FlawReference],
             "cvss_scores": List[FlawCVSS],
             "embargoed": bool,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "classification": FlawClassification,
+            "alerts": FlawAlerts,
             "type": FlawType,
             "cve_id": str,
             "impact": Union[BlankEnum, ImpactEnum],
             "component": str,
+            "components": List[str],
             "summary": str,
             "requires_summary": Union[BlankEnum, RequiresSummaryEnum],
             "statement": str,
             "cwe_id": str,
             "unembargo_dt": datetime.datetime,
             "source": Union[BlankEnum, Source8D8Enum],
             "reported_dt": datetime.datetime,
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_manifest_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_manifest_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_lang.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_lang.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_data.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_data.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_service.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_service.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_create_response_201.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_create_response_201.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.erratum import Erratum
+from ..models.tracker_alerts import TrackerAlerts
 from ..models.tracker_meta_attr import TrackerMetaAttr
 from ..models.tracker_type import TrackerType
 from ..types import UNSET, OSIDBModel, Unset
 
 T = TypeVar("T", bound="OsidbApiV1TrackersCreateResponse201")
 
 
@@ -19,14 +20,15 @@
     errata: List[Erratum]
     external_system_id: str
     meta_attr: TrackerMetaAttr
     status: str
     type: TrackerType
     uuid: str
     embargoed: bool
+    alerts: TrackerAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     affects: Union[Unset, List[str]] = UNSET
     ps_update_stream: Union[Unset, str] = UNSET
     resolution: Union[Unset, str] = UNSET
     dt: Union[Unset, datetime.datetime] = UNSET
     env: Union[Unset, str] = UNSET
@@ -54,14 +56,18 @@
         type: str = UNSET
         if not isinstance(self.type, Unset):
 
             type = TrackerType(self.type).value
 
         uuid = self.uuid
         embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
@@ -92,14 +98,16 @@
             field_dict["status"] = status
         if not isinstance(type, Unset):
             field_dict["type"] = type
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(affects, Unset):
             field_dict["affects"] = affects
         if not isinstance(ps_update_stream, Unset):
@@ -153,14 +161,21 @@
         else:
             type = TrackerType(_type)
 
         uuid = d.pop("uuid", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: TrackerAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = TrackerAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
@@ -194,14 +209,15 @@
             errata=errata,
             external_system_id=external_system_id,
             meta_attr=meta_attr,
             status=status,
             type=type,
             uuid=uuid,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
             affects=affects,
             ps_update_stream=ps_update_stream,
             resolution=resolution,
             dt=dt,
             env=env,
@@ -218,14 +234,15 @@
             "errata": List[Erratum],
             "external_system_id": str,
             "meta_attr": TrackerMetaAttr,
             "status": str,
             "type": TrackerType,
             "uuid": str,
             "embargoed": bool,
+            "alerts": TrackerAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "affects": List[str],
             "ps_update_stream": str,
             "resolution": str,
             "dt": datetime.datetime,
             "env": str,
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_flaw_source.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_flaw_source.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_order_item.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_order_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,61 +4,70 @@
 class OsidbApiV1TrackersListOrderItem(str, Enum):
     VALUE_0 = "-affects__affectedness"
     VALUE_1 = "-affects__created_dt"
     VALUE_2 = "-affects__cvss2"
     VALUE_3 = "-affects__cvss2_score"
     VALUE_4 = "-affects__cvss3"
     VALUE_5 = "-affects__cvss3_score"
-    VALUE_6 = "-affects__flaw__component"
-    VALUE_7 = "-affects__flaw__created_dt"
-    VALUE_8 = "-affects__flaw__cve_id"
-    VALUE_9 = "-affects__flaw__cvss2"
-    VALUE_10 = "-affects__flaw__cvss2_score"
-    VALUE_11 = "-affects__flaw__cvss3"
-    VALUE_12 = "-affects__flaw__cvss3_score"
-    VALUE_13 = "-affects__flaw__cwe_id"
-    VALUE_14 = "-affects__flaw__impact"
-    VALUE_15 = "-affects__flaw__nvd_cvss2"
-    VALUE_16 = "-affects__flaw__nvd_cvss3"
-    VALUE_17 = "-affects__flaw__reported_dt"
-    VALUE_18 = "-affects__flaw__source"
-    VALUE_19 = "-affects__flaw__type"
-    VALUE_20 = "-affects__flaw__unembargo_dt"
-    VALUE_21 = "-affects__flaw__updated_dt"
-    VALUE_22 = "-affects__flaw__uuid"
-    VALUE_23 = "-affects__impact"
-    VALUE_24 = "-affects__ps_component"
-    VALUE_25 = "-affects__ps_module"
-    VALUE_26 = "-affects__resolution"
-    VALUE_27 = "-affects__type"
-    VALUE_28 = "-affects__updated_dt"
-    VALUE_29 = "-affects__uuid"
-    VALUE_30 = "-created_dt"
-    VALUE_31 = "-external_system_id"
-    VALUE_32 = "-ps_update_stream"
-    VALUE_33 = "-resolution"
-    VALUE_34 = "-status"
-    VALUE_35 = "-type"
-    VALUE_36 = "-updated_dt"
-    VALUE_37 = "-uuid"
+    VALUE_6 = "-affects__embargoed"
+    VALUE_7 = "-affects__flaw__component"
+    VALUE_8 = "-affects__flaw__components"
+    VALUE_9 = "-affects__flaw__created_dt"
+    VALUE_10 = "-affects__flaw__cve_id"
+    VALUE_11 = "-affects__flaw__cvss2"
+    VALUE_12 = "-affects__flaw__cvss2_score"
+    VALUE_13 = "-affects__flaw__cvss3"
+    VALUE_14 = "-affects__flaw__cvss3_score"
+    VALUE_15 = "-affects__flaw__cwe_id"
+    VALUE_16 = "-affects__flaw__embargoed"
+    VALUE_17 = "-affects__flaw__impact"
+    VALUE_18 = "-affects__flaw__is_major_incident"
+    VALUE_19 = "-affects__flaw__nvd_cvss2"
+    VALUE_20 = "-affects__flaw__nvd_cvss3"
+    VALUE_21 = "-affects__flaw__reported_dt"
+    VALUE_22 = "-affects__flaw__source"
+    VALUE_23 = "-affects__flaw__type"
+    VALUE_24 = "-affects__flaw__unembargo_dt"
+    VALUE_25 = "-affects__flaw__updated_dt"
+    VALUE_26 = "-affects__flaw__uuid"
+    VALUE_27 = "-affects__impact"
+    VALUE_28 = "-affects__ps_component"
+    VALUE_29 = "-affects__ps_module"
+    VALUE_30 = "-affects__resolution"
+    VALUE_31 = "-affects__type"
+    VALUE_32 = "-affects__updated_dt"
+    VALUE_33 = "-affects__uuid"
+    VALUE_34 = "-created_dt"
+    VALUE_35 = "-embargoed"
+    VALUE_36 = "-external_system_id"
+    VALUE_37 = "-ps_update_stream"
+    VALUE_38 = "-resolution"
+    VALUE_39 = "-status"
+    VALUE_40 = "-type"
+    VALUE_41 = "-updated_dt"
+    VALUE_42 = "-uuid"
     AFFECTS_AFFECTEDNESS = "affects__affectedness"
     AFFECTS_CREATED_DT = "affects__created_dt"
     AFFECTS_CVSS2 = "affects__cvss2"
     AFFECTS_CVSS2_SCORE = "affects__cvss2_score"
     AFFECTS_CVSS3 = "affects__cvss3"
     AFFECTS_CVSS3_SCORE = "affects__cvss3_score"
+    AFFECTS_EMBARGOED = "affects__embargoed"
     AFFECTS_FLAW_COMPONENT = "affects__flaw__component"
+    AFFECTS_FLAW_COMPONENTS = "affects__flaw__components"
     AFFECTS_FLAW_CREATED_DT = "affects__flaw__created_dt"
     AFFECTS_FLAW_CVE_ID = "affects__flaw__cve_id"
     AFFECTS_FLAW_CVSS2 = "affects__flaw__cvss2"
     AFFECTS_FLAW_CVSS2_SCORE = "affects__flaw__cvss2_score"
     AFFECTS_FLAW_CVSS3 = "affects__flaw__cvss3"
     AFFECTS_FLAW_CVSS3_SCORE = "affects__flaw__cvss3_score"
     AFFECTS_FLAW_CWE_ID = "affects__flaw__cwe_id"
+    AFFECTS_FLAW_EMBARGOED = "affects__flaw__embargoed"
     AFFECTS_FLAW_IMPACT = "affects__flaw__impact"
+    AFFECTS_FLAW_IS_MAJOR_INCIDENT = "affects__flaw__is_major_incident"
     AFFECTS_FLAW_NVD_CVSS2 = "affects__flaw__nvd_cvss2"
     AFFECTS_FLAW_NVD_CVSS3 = "affects__flaw__nvd_cvss3"
     AFFECTS_FLAW_REPORTED_DT = "affects__flaw__reported_dt"
     AFFECTS_FLAW_SOURCE = "affects__flaw__source"
     AFFECTS_FLAW_TYPE = "affects__flaw__type"
     AFFECTS_FLAW_UNEMBARGO_DT = "affects__flaw__unembargo_dt"
     AFFECTS_FLAW_UPDATED_DT = "affects__flaw__updated_dt"
@@ -67,14 +76,15 @@
     AFFECTS_PS_COMPONENT = "affects__ps_component"
     AFFECTS_PS_MODULE = "affects__ps_module"
     AFFECTS_RESOLUTION = "affects__resolution"
     AFFECTS_TYPE = "affects__type"
     AFFECTS_UPDATED_DT = "affects__updated_dt"
     AFFECTS_UUID = "affects__uuid"
     CREATED_DT = "created_dt"
+    EMBARGOED = "embargoed"
     EXTERNAL_SYSTEM_ID = "external_system_id"
     PS_UPDATE_STREAM = "ps_update_stream"
     RESOLUTION = "resolution"
     STATUS = "status"
     TYPE = "type"
     UPDATED_DT = "updated_dt"
     UUID = "uuid"
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_retrieve_response_200.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.erratum import Erratum
+from ..models.tracker_alerts import TrackerAlerts
 from ..models.tracker_meta_attr import TrackerMetaAttr
 from ..models.tracker_type import TrackerType
 from ..types import UNSET, OSIDBModel, Unset
 
 T = TypeVar("T", bound="OsidbApiV1TrackersRetrieveResponse200")
 
 
@@ -19,14 +20,15 @@
     errata: List[Erratum]
     external_system_id: str
     meta_attr: TrackerMetaAttr
     status: str
     type: TrackerType
     uuid: str
     embargoed: bool
+    alerts: TrackerAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     affects: Union[Unset, List[str]] = UNSET
     ps_update_stream: Union[Unset, str] = UNSET
     resolution: Union[Unset, str] = UNSET
     dt: Union[Unset, datetime.datetime] = UNSET
     env: Union[Unset, str] = UNSET
@@ -54,14 +56,18 @@
         type: str = UNSET
         if not isinstance(self.type, Unset):
 
             type = TrackerType(self.type).value
 
         uuid = self.uuid
         embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
@@ -92,14 +98,16 @@
             field_dict["status"] = status
         if not isinstance(type, Unset):
             field_dict["type"] = type
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(affects, Unset):
             field_dict["affects"] = affects
         if not isinstance(ps_update_stream, Unset):
@@ -153,14 +161,21 @@
         else:
             type = TrackerType(_type)
 
         uuid = d.pop("uuid", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: TrackerAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = TrackerAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
@@ -194,14 +209,15 @@
             errata=errata,
             external_system_id=external_system_id,
             meta_attr=meta_attr,
             status=status,
             type=type,
             uuid=uuid,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
             affects=affects,
             ps_update_stream=ps_update_stream,
             resolution=resolution,
             dt=dt,
             env=env,
@@ -218,14 +234,15 @@
             "errata": List[Erratum],
             "external_system_id": str,
             "meta_attr": TrackerMetaAttr,
             "status": str,
             "type": TrackerType,
             "uuid": str,
             "embargoed": bool,
+            "alerts": TrackerAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "affects": List[str],
             "ps_update_stream": str,
             "resolution": str,
             "dt": datetime.datetime,
             "env": str,
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_update_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_update_response_200.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.erratum import Erratum
+from ..models.tracker_alerts import TrackerAlerts
 from ..models.tracker_meta_attr import TrackerMetaAttr
 from ..models.tracker_type import TrackerType
 from ..types import UNSET, OSIDBModel, Unset
 
 T = TypeVar("T", bound="OsidbApiV1TrackersUpdateResponse200")
 
 
@@ -19,14 +20,15 @@
     errata: List[Erratum]
     external_system_id: str
     meta_attr: TrackerMetaAttr
     status: str
     type: TrackerType
     uuid: str
     embargoed: bool
+    alerts: TrackerAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     affects: Union[Unset, List[str]] = UNSET
     ps_update_stream: Union[Unset, str] = UNSET
     resolution: Union[Unset, str] = UNSET
     dt: Union[Unset, datetime.datetime] = UNSET
     env: Union[Unset, str] = UNSET
@@ -54,14 +56,18 @@
         type: str = UNSET
         if not isinstance(self.type, Unset):
 
             type = TrackerType(self.type).value
 
         uuid = self.uuid
         embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
@@ -92,14 +98,16 @@
             field_dict["status"] = status
         if not isinstance(type, Unset):
             field_dict["type"] = type
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(affects, Unset):
             field_dict["affects"] = affects
         if not isinstance(ps_update_stream, Unset):
@@ -153,14 +161,21 @@
         else:
             type = TrackerType(_type)
 
         uuid = d.pop("uuid", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: TrackerAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = TrackerAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
@@ -194,14 +209,15 @@
             errata=errata,
             external_system_id=external_system_id,
             meta_attr=meta_attr,
             status=status,
             type=type,
             uuid=uuid,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
             affects=affects,
             ps_update_stream=ps_update_stream,
             resolution=resolution,
             dt=dt,
             env=env,
@@ -218,14 +234,15 @@
             "errata": List[Erratum],
             "external_system_id": str,
             "meta_attr": TrackerMetaAttr,
             "status": str,
             "type": TrackerType,
             "uuid": str,
             "embargoed": bool,
+            "alerts": TrackerAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "affects": List[str],
             "ps_update_stream": str,
             "resolution": str,
             "dt": datetime.datetime,
             "env": str,
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_healthy_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_healthy_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200_profile.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200_profile.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_adjust_create_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_adjust_create_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_2_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_2_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osim_healthy_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osim_healthy_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/osim_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/osim_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/package.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/package.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
+from ..models.package_alerts import PackageAlerts
 from ..models.package_ver import PackageVer
 from ..types import UNSET, OSIDBModel, Unset
 
 T = TypeVar("T", bound="Package")
 
 
 @attr.s(auto_attribs=True)
 class Package(OSIDBModel):
     """package_versions (Package model) serializer for read-only use in FlawSerializer."""
 
     package: str
     versions: List[PackageVer]
+    alerts: PackageAlerts
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         package = self.package
         versions: List[Dict[str, Any]] = UNSET
         if not isinstance(self.versions, Unset):
             versions = []
             for versions_item_data in self.versions:
                 versions_item: Dict[str, Any] = UNSET
                 if not isinstance(versions_item_data, Unset):
                     versions_item = versions_item_data.to_dict()
 
                 versions.append(versions_item)
 
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if not isinstance(package, Unset):
             field_dict["package"] = package
         if not isinstance(versions, Unset):
             field_dict["versions"] = versions
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         package = d.pop("package", UNSET)
@@ -53,27 +61,36 @@
                 if isinstance(_versions_item, Unset):
                     versions_item = UNSET
                 else:
                     versions_item = PackageVer.from_dict(_versions_item)
 
                 versions.append(versions_item)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: PackageAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = PackageAlerts.from_dict(_alerts)
+
         package = cls(
             package=package,
             versions=versions,
+            alerts=alerts,
         )
 
         package.additional_properties = d
         return package
 
     @staticmethod
     def get_fields():
         return {
             "package": str,
             "versions": List[PackageVer],
+            "alerts": PackageAlerts,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/package_ver.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/package_ver.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_affect_cvss_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_affect_cvss_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_affect_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_affect_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_epss_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_epss_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_exploit_only_report_data_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_exploit_only_report_data_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_flaw_acknowledgment_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_flaw_acknowledgment_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_flaw_comment_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_flaw_comment_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_flaw_cvss_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_flaw_cvss_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_flaw_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_flaw_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_flaw_package_version_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_flaw_package_version_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_flaw_reference_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_flaw_reference_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_flaw_report_data_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_flaw_report_data_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_supported_products_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_supported_products_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/paginated_tracker_list.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/paginated_tracker_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/ps_stream_selection.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/ps_stream_selection.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/reject.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/reject.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/source_8d8_enum.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/source_8d8_enum.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/supported_products.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/supported_products.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/token_obtain_pair.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/token_refresh.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,38 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="TokenObtainPair")
+T = TypeVar("T", bound="TokenRefresh")
 
 
 @attr.s(auto_attribs=True)
-class TokenObtainPair(OSIDBModel):
+class TokenRefresh(OSIDBModel):
     """ """
 
-    username: str
-    password: str
     access: str
     refresh: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        username = self.username
-        password = self.password
         access = self.access
         refresh = self.refresh
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        if not isinstance(username, Unset):
-            field_dict["username"] = username
-        if not isinstance(password, Unset):
-            field_dict["password"] = password
         if not isinstance(access, Unset):
             field_dict["access"] = access
         if not isinstance(refresh, Unset):
             field_dict["refresh"] = refresh
 
         return field_dict
 
     def to_multipart(self) -> Dict[str, Any]:
-        username = (
-            self.username
-            if self.username is UNSET
-            else (None, str(self.username), "text/plain")
-        )
-        password = (
-            self.password
-            if self.password is UNSET
-            else (None, str(self.password), "text/plain")
-        )
         access = (
             self.access
             if self.access is UNSET
             else (None, str(self.access), "text/plain")
         )
         refresh = (
             self.refresh
@@ -61,51 +43,39 @@
         field_dict: Dict[str, Any] = {}
         field_dict.update(
             {
                 key: (None, str(value), "text/plain")
                 for key, value in self.additional_properties.items()
             }
         )
-        if not isinstance(username, Unset):
-            field_dict["username"] = username
-        if not isinstance(password, Unset):
-            field_dict["password"] = password
         if not isinstance(access, Unset):
             field_dict["access"] = access
         if not isinstance(refresh, Unset):
             field_dict["refresh"] = refresh
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        username = d.pop("username", UNSET)
-
-        password = d.pop("password", UNSET)
-
         access = d.pop("access", UNSET)
 
         refresh = d.pop("refresh", UNSET)
 
-        token_obtain_pair = cls(
-            username=username,
-            password=password,
+        token_refresh = cls(
             access=access,
             refresh=refresh,
         )
 
-        token_obtain_pair.additional_properties = d
-        return token_obtain_pair
+        token_refresh.additional_properties = d
+        return token_refresh
 
     @staticmethod
     def get_fields():
         return {
-            "username": str,
-            "password": str,
             "access": str,
             "refresh": str,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/token_refresh.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/flaw_cvss_put_alerts.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,40 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..types import UNSET, OSIDBModel, Unset
+from ..types import OSIDBModel
 
-T = TypeVar("T", bound="TokenRefresh")
+T = TypeVar("T", bound="FlawCVSSPutAlerts")
 
 
 @attr.s(auto_attribs=True)
-class TokenRefresh(OSIDBModel):
+class FlawCVSSPutAlerts(OSIDBModel):
     """ """
 
-    access: str
-    refresh: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        access = self.access
-        refresh = self.refresh
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        if not isinstance(access, Unset):
-            field_dict["access"] = access
-        if not isinstance(refresh, Unset):
-            field_dict["refresh"] = refresh
-
-        return field_dict
-
-    def to_multipart(self) -> Dict[str, Any]:
-        access = (
-            self.access
-            if self.access is UNSET
-            else (None, str(self.access), "text/plain")
-        )
-        refresh = (
-            self.refresh
-            if self.refresh is UNSET
-            else (None, str(self.refresh), "text/plain")
-        )
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(
-            {
-                key: (None, str(value), "text/plain")
-                for key, value in self.additional_properties.items()
-            }
-        )
-        if not isinstance(access, Unset):
-            field_dict["access"] = access
-        if not isinstance(refresh, Unset):
-            field_dict["refresh"] = refresh
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        access = d.pop("access", UNSET)
-
-        refresh = d.pop("refresh", UNSET)
-
-        token_refresh = cls(
-            access=access,
-            refresh=refresh,
-        )
+        flaw_cvss_put_alerts = cls()
 
-        token_refresh.additional_properties = d
-        return token_refresh
+        flaw_cvss_put_alerts.additional_properties = d
+        return flaw_cvss_put_alerts
 
     @staticmethod
     def get_fields():
-        return {
-            "access": str,
-            "refresh": str,
-        }
+        return {}
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/token_verify.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/token_verify.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/tracker.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/tracker.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 from typing import Any, Dict, List, Tuple, Type, TypeVar, Union, cast
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.erratum import Erratum
+from ..models.tracker_alerts import TrackerAlerts
 from ..models.tracker_meta_attr import TrackerMetaAttr
 from ..models.tracker_type import TrackerType
 from ..types import UNSET, OSIDBModel, Unset
 
 T = TypeVar("T", bound="Tracker")
 
 
@@ -20,14 +21,15 @@
     errata: List[Erratum]
     external_system_id: str
     meta_attr: TrackerMetaAttr
     status: str
     type: TrackerType
     uuid: str
     embargoed: bool
+    alerts: TrackerAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     affects: Union[Unset, List[str]] = UNSET
     ps_update_stream: Union[Unset, str] = UNSET
     resolution: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -51,14 +53,18 @@
         type: str = UNSET
         if not isinstance(self.type, Unset):
 
             type = TrackerType(self.type).value
 
         uuid = self.uuid
         embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
@@ -82,14 +88,16 @@
             field_dict["status"] = status
         if not isinstance(type, Unset):
             field_dict["type"] = type
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(affects, Unset):
             field_dict["affects"] = affects
         if not isinstance(ps_update_stream, Unset):
@@ -132,14 +140,18 @@
 
         uuid = self.uuid if self.uuid is UNSET else (None, str(self.uuid), "text/plain")
         embargoed = (
             self.embargoed
             if self.embargoed is UNSET
             else (None, str(self.embargoed), "text/plain")
         )
+        alerts: Union[Unset, Tuple[None, str, str]] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = (None, json.dumps(self.alerts.to_dict()), "application/json")
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
@@ -177,14 +189,16 @@
             field_dict["status"] = status
         if not isinstance(type, Unset):
             field_dict["type"] = type
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(affects, Unset):
             field_dict["affects"] = affects
         if not isinstance(ps_update_stream, Unset):
@@ -230,14 +244,21 @@
         else:
             type = TrackerType(_type)
 
         uuid = d.pop("uuid", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: TrackerAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = TrackerAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
@@ -258,14 +279,15 @@
             errata=errata,
             external_system_id=external_system_id,
             meta_attr=meta_attr,
             status=status,
             type=type,
             uuid=uuid,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
             affects=affects,
             ps_update_stream=ps_update_stream,
             resolution=resolution,
         )
 
@@ -278,14 +300,15 @@
             "errata": List[Erratum],
             "external_system_id": str,
             "meta_attr": TrackerMetaAttr,
             "status": str,
             "type": TrackerType,
             "uuid": str,
             "embargoed": bool,
+            "alerts": TrackerAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "affects": List[str],
             "ps_update_stream": str,
             "resolution": str,
         }
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/tracker_meta_attr.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/tracker_meta_attr.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/tracker_post.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/tracker_post.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 from typing import Any, Dict, List, Tuple, Type, TypeVar, Union, cast
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.erratum import Erratum
+from ..models.tracker_post_alerts import TrackerPostAlerts
 from ..models.tracker_post_meta_attr import TrackerPostMetaAttr
 from ..models.tracker_type import TrackerType
 from ..types import UNSET, OSIDBModel, Unset
 
 T = TypeVar("T", bound="TrackerPost")
 
 
@@ -19,14 +20,15 @@
 
     errata: List[Erratum]
     meta_attr: TrackerPostMetaAttr
     status: str
     type: TrackerType
     uuid: str
     embargoed: bool
+    alerts: TrackerPostAlerts
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     affects: Union[Unset, List[str]] = UNSET
     ps_update_stream: Union[Unset, str] = UNSET
     resolution: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -49,14 +51,18 @@
         type: str = UNSET
         if not isinstance(self.type, Unset):
 
             type = TrackerType(self.type).value
 
         uuid = self.uuid
         embargoed = self.embargoed
+        alerts: Dict[str, Any] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = self.alerts.to_dict()
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
@@ -78,14 +84,16 @@
             field_dict["status"] = status
         if not isinstance(type, Unset):
             field_dict["type"] = type
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(affects, Unset):
             field_dict["affects"] = affects
         if not isinstance(ps_update_stream, Unset):
@@ -123,14 +131,18 @@
 
         uuid = self.uuid if self.uuid is UNSET else (None, str(self.uuid), "text/plain")
         embargoed = (
             self.embargoed
             if self.embargoed is UNSET
             else (None, str(self.embargoed), "text/plain")
         )
+        alerts: Union[Unset, Tuple[None, str, str]] = UNSET
+        if not isinstance(self.alerts, Unset):
+            alerts = (None, json.dumps(self.alerts.to_dict()), "application/json")
+
         created_dt: str = UNSET
         if not isinstance(self.created_dt, Unset):
             created_dt = self.created_dt.isoformat()
 
         updated_dt: str = UNSET
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
@@ -166,14 +178,16 @@
             field_dict["status"] = status
         if not isinstance(type, Unset):
             field_dict["type"] = type
         if not isinstance(uuid, Unset):
             field_dict["uuid"] = uuid
         if not isinstance(embargoed, Unset):
             field_dict["embargoed"] = embargoed
+        if not isinstance(alerts, Unset):
+            field_dict["alerts"] = alerts
         if not isinstance(created_dt, Unset):
             field_dict["created_dt"] = created_dt
         if not isinstance(updated_dt, Unset):
             field_dict["updated_dt"] = updated_dt
         if not isinstance(affects, Unset):
             field_dict["affects"] = affects
         if not isinstance(ps_update_stream, Unset):
@@ -217,14 +231,21 @@
         else:
             type = TrackerType(_type)
 
         uuid = d.pop("uuid", UNSET)
 
         embargoed = d.pop("embargoed", UNSET)
 
+        _alerts = d.pop("alerts", UNSET)
+        alerts: TrackerPostAlerts
+        if isinstance(_alerts, Unset):
+            alerts = UNSET
+        else:
+            alerts = TrackerPostAlerts.from_dict(_alerts)
+
         _created_dt = d.pop("created_dt", UNSET)
         created_dt: datetime.datetime
         if isinstance(_created_dt, Unset):
             created_dt = UNSET
         else:
             created_dt = isoparse(_created_dt)
 
@@ -244,14 +265,15 @@
         tracker_post = cls(
             errata=errata,
             meta_attr=meta_attr,
             status=status,
             type=type,
             uuid=uuid,
             embargoed=embargoed,
+            alerts=alerts,
             created_dt=created_dt,
             updated_dt=updated_dt,
             affects=affects,
             ps_update_stream=ps_update_stream,
             resolution=resolution,
         )
 
@@ -263,14 +285,15 @@
         return {
             "errata": List[Erratum],
             "meta_attr": TrackerPostMetaAttr,
             "status": str,
             "type": TrackerType,
             "uuid": str,
             "embargoed": bool,
+            "alerts": TrackerPostAlerts,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "affects": List[str],
             "ps_update_stream": str,
             "resolution": str,
         }
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/tracker_post_meta_attr.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/tracker_post_meta_attr.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/tracker_report_data.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/tracker_report_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 @attr.s(auto_attribs=True)
 class TrackerReportData(OSIDBModel):
     """ """
 
     type: TrackerType
     external_system_id: str
-    status: str
+    status: Union[Unset, str] = UNSET
     resolution: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         type: str = UNSET
         if not isinstance(self.type, Unset):
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/tracker_suggestion.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/tracker_suggestion.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/workflows_api_v1_adjust_create_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/workflows_api_v1_adjust_create_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/workflows_api_v1_retrieve_2_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/workflows_api_v1_retrieve_2_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/workflows_api_v1_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/workflows_api_v1_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/workflows_healthy_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/workflows_healthy_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/models/workflows_retrieve_response_200.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/models/workflows_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/bindings/python_client/types.py` & `osidb_bindings-3.7.0/osidb_bindings/bindings/python_client/types.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/constants.py` & `osidb_bindings-3.7.0/osidb_bindings/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 osidb-bindings constants
 """
 
 
 from typing import List
 
 OSIDB_API_VERSION: str = "v1"
-OSIDB_BINDINGS_VERSION: str = "3.6.0"
+OSIDB_BINDINGS_VERSION: str = "3.7.0"
 OSIDB_BINDINGS_USERAGENT: str = f"osidb-bindings-{OSIDB_BINDINGS_VERSION}"
 OSIDB_BINDINGS_API_PATH: str = ".bindings.python_client.api.osidb"
 OSIDB_BINDINGS_PLACEHOLDER_FIELD: str = (
     f'__placeholder_field{OSIDB_BINDINGS_VERSION.replace(".","")}'
 )
 
 DEFAULT_LIMIT: int = 50
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/helpers.py` & `osidb_bindings-3.7.0/osidb_bindings/helpers.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/iterators.py` & `osidb_bindings-3.7.0/osidb_bindings/iterators.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings/session.py` & `osidb_bindings-3.7.0/osidb_bindings/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,15 @@
         self.auth = auth
 
         self.__client = AuthenticatedClient(
             base_url=base_url,
             headers={
                 "User-Agent": OSIDB_BINDINGS_USERAGENT,
                 "Bugzilla-Api-Key": get_env("BUGZILLA_API_KEY", ""),
+                "Jira-Api-Key": get_env("JIRA_ACCESS_TOKEN", ""),
             },
             verify_ssl=verify_ssl,
         )
 
         self.flaws = SessionOperationsGroup(
             self.__get_client_with_new_access_token,
             "flaws",
@@ -194,14 +195,16 @@
         )
         self.trackers = SessionOperationsGroup(
             self.__get_client_with_new_access_token,
             "trackers",
             allowed_operations=(
                 "retrieve",
                 "list",
+                "update",
+                "create",
             ),
         )
 
         self.refresh_token = self.__get_refresh_token()
 
     def status(self):
         status_fn = get_sync_function(osidb_status_retrieve)
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings/utils.py` & `osidb_bindings-3.7.0/osidb_bindings/utils.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.6.0/osidb_bindings.egg-info/PKG-INFO` & `osidb_bindings-3.7.0/osidb_bindings.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osidb-bindings
-Version: 3.6.0
+Version: 3.7.0
 Summary: Python bindings for accessing OSIDB API
 Home-page: https://github.com/RedHatProductSecurity/osidb-bindings
 Author: Jakub Frejlach, Red Hat Product Security
 Author-email: jfrejlac@redhat.com
 Project-URL: Changelog, https://github.com/RedHatProductSecurity/osidb-bindings/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/RedHatProductSecurity/osidb-bindings/blob/master/TUTORIAL.md
 Project-URL: Source, https://github.com/RedHatProductSecurity/osidb-bindings
```

### Comparing `osidb-bindings-3.6.0/osidb_bindings.egg-info/SOURCES.txt` & `osidb_bindings-3.7.0/osidb_bindings.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -100,19 +100,24 @@
 osidb_bindings/bindings/python_client/api/workflows/workflows_api_v1_adjust_create.py
 osidb_bindings/bindings/python_client/api/workflows/workflows_api_v1_retrieve.py
 osidb_bindings/bindings/python_client/api/workflows/workflows_api_v1_retrieve_2.py
 osidb_bindings/bindings/python_client/api/workflows/workflows_healthy_retrieve.py
 osidb_bindings/bindings/python_client/api/workflows/workflows_retrieve.py
 osidb_bindings/bindings/python_client/models/__init__.py
 osidb_bindings/bindings/python_client/models/affect.py
+osidb_bindings/bindings/python_client/models/affect_alerts.py
 osidb_bindings/bindings/python_client/models/affect_cvss.py
+osidb_bindings/bindings/python_client/models/affect_cvss_alerts.py
 osidb_bindings/bindings/python_client/models/affect_cvss_post.py
+osidb_bindings/bindings/python_client/models/affect_cvss_post_alerts.py
 osidb_bindings/bindings/python_client/models/affect_cvss_put.py
+osidb_bindings/bindings/python_client/models/affect_cvss_put_alerts.py
 osidb_bindings/bindings/python_client/models/affect_meta_attr.py
 osidb_bindings/bindings/python_client/models/affect_post.py
+osidb_bindings/bindings/python_client/models/affect_post_alerts.py
 osidb_bindings/bindings/python_client/models/affect_post_meta_attr.py
 osidb_bindings/bindings/python_client/models/affect_report_data.py
 osidb_bindings/bindings/python_client/models/affect_type.py
 osidb_bindings/bindings/python_client/models/affectedness_enum.py
 osidb_bindings/bindings/python_client/models/auth_token_create_response_200.py
 osidb_bindings/bindings/python_client/models/auth_token_refresh_create_response_200.py
 osidb_bindings/bindings/python_client/models/auth_token_retrieve_response_200.py
@@ -122,15 +127,17 @@
 osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item.py
 osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_data.py
 osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_error.py
 osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_state.py
 osidb_bindings/bindings/python_client/models/collectors_healthy_retrieve_response_200.py
 osidb_bindings/bindings/python_client/models/collectors_retrieve_response_200.py
 osidb_bindings/bindings/python_client/models/comment.py
+osidb_bindings/bindings/python_client/models/comment_alerts.py
 osidb_bindings/bindings/python_client/models/comment_meta_attr.py
+osidb_bindings/bindings/python_client/models/cvss_version_enum.py
 osidb_bindings/bindings/python_client/models/epss.py
 osidb_bindings/bindings/python_client/models/erratum.py
 osidb_bindings/bindings/python_client/models/exploit_only_report_data.py
 osidb_bindings/bindings/python_client/models/exploit_only_report_data_source_enum.py
 osidb_bindings/bindings/python_client/models/exploits_api_v1_collect_update_response_200.py
 osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200.py
 osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200_cves.py
@@ -145,53 +152,67 @@
 osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200_explanations_item.py
 osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200.py
 osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200_pending_actions_item.py
 osidb_bindings/bindings/python_client/models/exploits_api_v1_status_retrieve_response_200.py
 osidb_bindings/bindings/python_client/models/exploits_api_v1_supported_products_list_response_200.py
 osidb_bindings/bindings/python_client/models/flaw.py
 osidb_bindings/bindings/python_client/models/flaw_acknowledgment.py
+osidb_bindings/bindings/python_client/models/flaw_acknowledgment_alerts.py
 osidb_bindings/bindings/python_client/models/flaw_acknowledgment_post.py
+osidb_bindings/bindings/python_client/models/flaw_acknowledgment_post_alerts.py
 osidb_bindings/bindings/python_client/models/flaw_acknowledgment_put.py
+osidb_bindings/bindings/python_client/models/flaw_acknowledgment_put_alerts.py
+osidb_bindings/bindings/python_client/models/flaw_alerts.py
 osidb_bindings/bindings/python_client/models/flaw_classification.py
 osidb_bindings/bindings/python_client/models/flaw_classification_state.py
 osidb_bindings/bindings/python_client/models/flaw_comment.py
+osidb_bindings/bindings/python_client/models/flaw_comment_alerts.py
 osidb_bindings/bindings/python_client/models/flaw_comment_post.py
+osidb_bindings/bindings/python_client/models/flaw_comment_post_alerts.py
 osidb_bindings/bindings/python_client/models/flaw_comment_post_meta_attr.py
 osidb_bindings/bindings/python_client/models/flaw_comment_type.py
 osidb_bindings/bindings/python_client/models/flaw_cvss.py
+osidb_bindings/bindings/python_client/models/flaw_cvss_alerts.py
 osidb_bindings/bindings/python_client/models/flaw_cvss_post.py
+osidb_bindings/bindings/python_client/models/flaw_cvss_post_alerts.py
 osidb_bindings/bindings/python_client/models/flaw_cvss_put.py
+osidb_bindings/bindings/python_client/models/flaw_cvss_put_alerts.py
 osidb_bindings/bindings/python_client/models/flaw_meta_attr.py
 osidb_bindings/bindings/python_client/models/flaw_meta_type.py
 osidb_bindings/bindings/python_client/models/flaw_package_version.py
 osidb_bindings/bindings/python_client/models/flaw_package_version_post.py
 osidb_bindings/bindings/python_client/models/flaw_package_version_put.py
 osidb_bindings/bindings/python_client/models/flaw_post.py
+osidb_bindings/bindings/python_client/models/flaw_post_alerts.py
 osidb_bindings/bindings/python_client/models/flaw_post_classification.py
 osidb_bindings/bindings/python_client/models/flaw_post_classification_state.py
 osidb_bindings/bindings/python_client/models/flaw_post_meta_attr.py
 osidb_bindings/bindings/python_client/models/flaw_reference.py
+osidb_bindings/bindings/python_client/models/flaw_reference_alerts.py
 osidb_bindings/bindings/python_client/models/flaw_reference_post.py
+osidb_bindings/bindings/python_client/models/flaw_reference_post_alerts.py
 osidb_bindings/bindings/python_client/models/flaw_reference_put.py
+osidb_bindings/bindings/python_client/models/flaw_reference_put_alerts.py
 osidb_bindings/bindings/python_client/models/flaw_reference_type.py
 osidb_bindings/bindings/python_client/models/flaw_report_data.py
 osidb_bindings/bindings/python_client/models/flaw_type.py
 osidb_bindings/bindings/python_client/models/flaw_uuid_list.py
 osidb_bindings/bindings/python_client/models/flaw_version.py
 osidb_bindings/bindings/python_client/models/impact_enum.py
 osidb_bindings/bindings/python_client/models/issuer_enum.py
 osidb_bindings/bindings/python_client/models/major_incident_state_enum.py
 osidb_bindings/bindings/python_client/models/maturity_preliminary_enum.py
 osidb_bindings/bindings/python_client/models/meta.py
+osidb_bindings/bindings/python_client/models/meta_alerts.py
 osidb_bindings/bindings/python_client/models/meta_meta_attr.py
 osidb_bindings/bindings/python_client/models/module_component.py
 osidb_bindings/bindings/python_client/models/nist_cvss_validation_enum.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_create_response_201.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_create_response_201.py
-osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_destroy_response_204.py
+osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_destroy_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_list_issuer.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_list_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_retrieve_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_cvss_scores_update_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_destroy_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_affectedness.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_cvss_scores_issuer.py
@@ -232,14 +253,15 @@
 osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_nist_cvss_validation.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_order_item.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_references_type.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_requires_summary.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_source.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_type.py
+osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_workflow_state_item.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_package_versions_create_response_201.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_package_versions_destroy_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_package_versions_list_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_package_versions_retrieve_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_package_versions_update_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_promote_create_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_create_response_201.py
@@ -276,14 +298,15 @@
 osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200_profile.py
 osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_adjust_create_response_200.py
 osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_2_response_200.py
 osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_response_200.py
 osidb_bindings/bindings/python_client/models/osim_healthy_retrieve_response_200.py
 osidb_bindings/bindings/python_client/models/osim_retrieve_response_200.py
 osidb_bindings/bindings/python_client/models/package.py
+osidb_bindings/bindings/python_client/models/package_alerts.py
 osidb_bindings/bindings/python_client/models/package_ver.py
 osidb_bindings/bindings/python_client/models/paginated_affect_cvss_list.py
 osidb_bindings/bindings/python_client/models/paginated_affect_list.py
 osidb_bindings/bindings/python_client/models/paginated_epss_list.py
 osidb_bindings/bindings/python_client/models/paginated_exploit_only_report_data_list.py
 osidb_bindings/bindings/python_client/models/paginated_flaw_acknowledgment_list.py
 osidb_bindings/bindings/python_client/models/paginated_flaw_comment_list.py
@@ -300,16 +323,18 @@
 osidb_bindings/bindings/python_client/models/resolution_enum.py
 osidb_bindings/bindings/python_client/models/source_8d8_enum.py
 osidb_bindings/bindings/python_client/models/supported_products.py
 osidb_bindings/bindings/python_client/models/token_obtain_pair.py
 osidb_bindings/bindings/python_client/models/token_refresh.py
 osidb_bindings/bindings/python_client/models/token_verify.py
 osidb_bindings/bindings/python_client/models/tracker.py
+osidb_bindings/bindings/python_client/models/tracker_alerts.py
 osidb_bindings/bindings/python_client/models/tracker_meta_attr.py
 osidb_bindings/bindings/python_client/models/tracker_post.py
+osidb_bindings/bindings/python_client/models/tracker_post_alerts.py
 osidb_bindings/bindings/python_client/models/tracker_post_meta_attr.py
 osidb_bindings/bindings/python_client/models/tracker_report_data.py
 osidb_bindings/bindings/python_client/models/tracker_suggestion.py
 osidb_bindings/bindings/python_client/models/tracker_type.py
 osidb_bindings/bindings/python_client/models/workflows_api_v1_adjust_create_response_200.py
 osidb_bindings/bindings/python_client/models/workflows_api_v1_retrieve_2_response_200.py
 osidb_bindings/bindings/python_client/models/workflows_api_v1_retrieve_response_200.py
```

### Comparing `osidb-bindings-3.6.0/setup.py` & `osidb_bindings-3.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="osidb-bindings",
-    version="3.6.0",
+    version="3.7.0",
     author="Jakub Frejlach, Red Hat Product Security",
     author_email="jfrejlac@redhat.com",
     description="Python bindings for accessing OSIDB API",
     url="https://github.com/RedHatProductSecurity/osidb-bindings",
     project_urls={
         "Changelog": "https://github.com/RedHatProductSecurity/osidb-bindings/blob/master/CHANGELOG.md",
         "Documentation": "https://github.com/RedHatProductSecurity/osidb-bindings/blob/master/TUTORIAL.md",
```

