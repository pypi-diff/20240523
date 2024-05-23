# Comparing `tmp/argilla_sdk-0.1.0a2.tar.gz` & `tmp/argilla_sdk-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argilla_sdk-0.1.0a2.tar", last modified: Thu May 23 09:54:48 2024, max compression
+gzip compressed data, was "argilla_sdk-0.1.0a3.tar", last modified: Thu May 23 10:41:53 2024, max compression
```

## Comparing `argilla_sdk-0.1.0a2.tar` & `argilla_sdk-0.1.0a3.tar`

### file list

```diff
@@ -1,121 +1,121 @@
--rw-r--r--   0        0        0    11357 2024-05-23 09:52:46.014905 argilla_sdk-0.1.0a2/LICENSE
--rw-r--r--   0        0        0      563 2024-05-23 09:52:46.014905 argilla_sdk-0.1.0a2/LICENSE_HEADER
--rw-r--r--   0        0        0     1670 2024-05-23 09:52:46.014905 argilla_sdk-0.1.0a2/README.md
--rw-r--r--   0        0        0     1310 2024-05-23 09:54:48.759026 argilla_sdk-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0     1019 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/__init__.py
--rw-r--r--   0        0        0     1002 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_api/__init__.py
--rw-r--r--   0        0        0     1756 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_base.py
--rw-r--r--   0        0        0     4675 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_client.py
--rw-r--r--   0        0        0     4816 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_datasets.py
--rw-r--r--   0        0        0     3733 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_fields.py
--rw-r--r--   0        0        0      716 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_http/__init__.py
--rw-r--r--   0        0        0     1498 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_http/_client.py
--rw-r--r--   0        0        0     1152 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_http/_helpers.py
--rw-r--r--   0        0        0     3865 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_metadata.py
--rw-r--r--   0        0        0     4397 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_questions.py
--rw-r--r--   0        0        0     9357 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_records.py
--rw-r--r--   0        0        0     4618 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_users.py
--rw-r--r--   0        0        0     3214 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_vectors.py
--rw-r--r--   0        0        0     5137 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_workspaces.py
--rw-r--r--   0        0        0      666 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_constants.py
--rw-r--r--   0        0        0      835 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_exceptions/__init__.py
--rw-r--r--   0        0        0     2519 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_exceptions/_api.py
--rw-r--r--   0        0        0     1305 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_exceptions/_base.py
--rw-r--r--   0        0        0      749 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_exceptions/_metadata.py
--rw-r--r--   0        0        0      704 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_exceptions/_serialization.py
--rw-r--r--   0        0        0      696 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_exceptions/_settings.py
--rw-r--r--   0        0        0      655 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_helpers/__init__.py
--rw-r--r--   0        0        0     1033 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_helpers/_dataclasses.py
--rw-r--r--   0        0        0     1156 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_helpers/_iterator.py
--rw-r--r--   0        0        0     1096 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_helpers/_log.py
--rw-r--r--   0        0        0     2393 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_helpers/_mixins.py
--rw-r--r--   0        0        0     2530 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_helpers/_resource_repr.py
--rw-r--r--   0        0        0     2224 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/__init__.py
--rw-r--r--   0        0        0     1260 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_base.py
--rw-r--r--   0        0        0     1570 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_dataset.py
--rw-r--r--   0        0        0      587 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_record/__init__.py
--rw-r--r--   0        0        0      978 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_record/_metadata.py
--rw-r--r--   0        0        0     2790 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_record/_record.py
--rw-r--r--   0        0        0     1744 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_record/_response.py
--rw-r--r--   0        0        0     1373 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_record/_suggestion.py
--rw-r--r--   0        0        0     1088 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_record/_vector.py
--rw-r--r--   0        0        0     1320 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_resource.py
--rw-r--r--   0        0        0     2574 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_search.py
--rw-r--r--   0        0        0      587 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_settings/__init__.py
--rw-r--r--   0        0        0     2202 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_settings/_fields.py
--rw-r--r--   0        0        0     4022 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_settings/_metadata.py
--rw-r--r--   0        0        0     1562 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_settings/_questions/__init__.py
--rw-r--r--   0        0        0     2148 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_settings/_questions/_base.py
--rw-r--r--   0        0        0     1986 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_settings/_questions/_label_selection.py
--rw-r--r--   0        0        0     1138 2024-05-23 09:52:46.038905 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_settings/_questions/_multi_label_selection.py
--rw-r--r--   0        0        0     1453 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_settings/_questions/_ranking.py
--rw-r--r--   0        0        0     1356 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_settings/_questions/_rating.py
--rw-r--r--   0        0        0     2041 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_settings/_questions/_span.py
--rw-r--r--   0        0        0      866 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_settings/_questions/_text.py
--rw-r--r--   0        0        0     1671 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_user.py
--rw-r--r--   0        0        0     1135 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_workspace.py
--rw-r--r--   0        0        0     4713 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/_resource.py
--rw-r--r--   0        0        0    10069 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/client.py
--rw-r--r--   0        0        0      669 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/datasets/__init__.py
--rw-r--r--   0        0        0     6133 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/datasets/_export.py
--rw-r--r--   0        0        0     8210 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/datasets/_resource.py
--rw-r--r--   0        0        0      837 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/records/__init__.py
--rw-r--r--   0        0        0    15701 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/records/_dataset_records.py
--rw-r--r--   0        0        0      663 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/records/_export/__init__.py
--rw-r--r--   0        0        0      587 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/records/_export/_datasets.py
--rw-r--r--   0        0        0     5979 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/records/_export/_generic.py
--rw-r--r--   0        0        0     1802 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/records/_helpers.py
--rw-r--r--   0        0        0    17795 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/records/_resource.py
--rw-r--r--   0        0        0     4627 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/records/_search.py
--rw-r--r--   0        0        0     7113 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/responses.py
--rw-r--r--   0        0        0      820 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/settings/__init__.py
--rw-r--r--   0        0        0     3301 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/settings/_common.py
--rw-r--r--   0        0        0     4727 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/settings/_field.py
--rw-r--r--   0        0        0     7790 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/settings/_metadata.py
--rw-r--r--   0        0        0    15550 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/settings/_question.py
--rw-r--r--   0        0        0    14873 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/settings/_resource.py
--rw-r--r--   0        0        0     5625 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/suggestions.py
--rw-r--r--   0        0        0      652 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/users/__init__.py
--rw-r--r--   0        0        0     6373 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/users/_resource.py
--rw-r--r--   0        0        0     2523 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/vectors.py
--rw-r--r--   0        0        0      667 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/workspaces/__init__.py
--rw-r--r--   0        0        0     6768 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/src/argilla_sdk/workspaces/_resource.py
--rw-r--r--   0        0        0     1099 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/tests/integration/conftest.py
--rw-r--r--   0        0        0    21227 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/tests/integration/test_add_records.py
--rw-r--r--   0        0        0     3541 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/tests/integration/test_create_datasets.py
--rw-r--r--   0        0        0     4459 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/tests/integration/test_dataset_workspace.py
--rw-r--r--   0        0        0     2401 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/tests/integration/test_empty_settings.py
--rw-r--r--   0        0        0     3941 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/tests/integration/test_export_dataset.py
--rw-r--r--   0        0        0     8052 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/tests/integration/test_export_records.py
--rw-r--r--   0        0        0     2789 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/tests/integration/test_list_records.py
--rw-r--r--   0        0        0     1360 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/tests/integration/test_listing_datasets.py
--rw-r--r--   0        0        0     1426 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/tests/integration/test_manage_users.py
--rw-r--r--   0        0        0     1833 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/tests/integration/test_manage_workspaces.py
--rw-r--r--   0        0        0     4722 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/tests/integration/test_metadata.py
--rw-r--r--   0        0        0     2758 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/tests/integration/test_publish_datasets.py
--rw-r--r--   0        0        0     3457 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/tests/integration/test_query_records.py
--rw-r--r--   0        0        0     1967 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/tests/integration/test_ranking_questions.py
--rw-r--r--   0        0        0     3919 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/tests/integration/test_update_records.py
--rw-r--r--   0        0        0     5056 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/tests/integration/test_vectors.py
--rw-r--r--   0        0        0     2620 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/tests/unit/api/http/test_http_client.py
--rw-r--r--   0        0        0      834 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/tests/unit/conftest.py
--rw-r--r--   0        0        0     2479 2024-05-23 09:52:46.042904 argilla_sdk-0.1.0a2/tests/unit/export/test_record_export_import_compatibillity.py
--rw-r--r--   0        0        0     2466 2024-05-23 09:52:46.046904 argilla_sdk-0.1.0a2/tests/unit/export/test_settings_export_import_compatibillity.py
--rw-r--r--   0        0        0     2322 2024-05-23 09:52:46.046904 argilla_sdk-0.1.0a2/tests/unit/helpers/test_resource_repr.py
--rw-r--r--   0        0        0     1607 2024-05-23 09:52:46.046904 argilla_sdk-0.1.0a2/tests/unit/test_interface.py
--rw-r--r--   0        0        0     6854 2024-05-23 09:52:46.046904 argilla_sdk-0.1.0a2/tests/unit/test_record_ingestion.py
--rw-r--r--   0        0        0     5377 2024-05-23 09:52:46.046904 argilla_sdk-0.1.0a2/tests/unit/test_record_responses.py
--rw-r--r--   0        0        0     1392 2024-05-23 09:52:46.046904 argilla_sdk-0.1.0a2/tests/unit/test_record_suggestions.py
--rw-r--r--   0        0        0    12204 2024-05-23 09:52:46.046904 argilla_sdk-0.1.0a2/tests/unit/test_resources/test_datasets.py
--rw-r--r--   0        0        0     1989 2024-05-23 09:52:46.046904 argilla_sdk-0.1.0a2/tests/unit/test_resources/test_fields.py
--rw-r--r--   0        0        0     5608 2024-05-23 09:52:46.046904 argilla_sdk-0.1.0a2/tests/unit/test_resources/test_questions.py
--rw-r--r--   0        0        0     2451 2024-05-23 09:52:46.046904 argilla_sdk-0.1.0a2/tests/unit/test_resources/test_records.py
--rw-r--r--   0        0        0    10785 2024-05-23 09:52:46.046904 argilla_sdk-0.1.0a2/tests/unit/test_resources/test_users.py
--rw-r--r--   0        0        0    10469 2024-05-23 09:52:46.046904 argilla_sdk-0.1.0a2/tests/unit/test_resources/test_workspaces.py
--rw-r--r--   0        0        0     1508 2024-05-23 09:52:46.046904 argilla_sdk-0.1.0a2/tests/unit/test_settings/test_multi_label_question.py
--rw-r--r--   0        0        0     4380 2024-05-23 09:52:46.046904 argilla_sdk-0.1.0a2/tests/unit/test_settings/test_settings.py
--rw-r--r--   0        0        0     2411 2024-05-23 09:52:46.046904 argilla_sdk-0.1.0a2/tests/unit/test_settings/test_settings_fields.py
--rw-r--r--   0        0        0     3248 2024-05-23 09:52:46.046904 argilla_sdk-0.1.0a2/tests/unit/test_settings/test_settings_questions.py
--rw-r--r--   0        0        0     1986 2024-05-23 09:52:46.046904 argilla_sdk-0.1.0a2/tests/unit/test_settings/test_span_question.py
--rw-r--r--   0        0        0     2868 2024-05-23 09:52:46.046904 argilla_sdk-0.1.0a2/tests/unit/test_settings/test_terms_metadata.py
--rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 argilla_sdk-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-23 10:39:54.810728 argilla_sdk-0.1.0a3/LICENSE
+-rw-r--r--   0        0        0      563 2024-05-23 10:39:54.810728 argilla_sdk-0.1.0a3/LICENSE_HEADER
+-rw-r--r--   0        0        0     1670 2024-05-23 10:39:54.810728 argilla_sdk-0.1.0a3/README.md
+-rw-r--r--   0        0        0     1310 2024-05-23 10:41:53.170630 argilla_sdk-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0     1019 2024-05-23 10:39:54.830728 argilla_sdk-0.1.0a3/src/argilla_sdk/__init__.py
+-rw-r--r--   0        0        0     1002 2024-05-23 10:39:54.830728 argilla_sdk-0.1.0a3/src/argilla_sdk/_api/__init__.py
+-rw-r--r--   0        0        0     1756 2024-05-23 10:39:54.830728 argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_base.py
+-rw-r--r--   0        0        0     4675 2024-05-23 10:39:54.830728 argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_client.py
+-rw-r--r--   0        0        0     4816 2024-05-23 10:39:54.830728 argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_datasets.py
+-rw-r--r--   0        0        0     3733 2024-05-23 10:39:54.830728 argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_fields.py
+-rw-r--r--   0        0        0      716 2024-05-23 10:39:54.830728 argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_http/__init__.py
+-rw-r--r--   0        0        0     1498 2024-05-23 10:39:54.830728 argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_http/_client.py
+-rw-r--r--   0        0        0     1152 2024-05-23 10:39:54.830728 argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_http/_helpers.py
+-rw-r--r--   0        0        0     3865 2024-05-23 10:39:54.830728 argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_metadata.py
+-rw-r--r--   0        0        0     4397 2024-05-23 10:39:54.830728 argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_questions.py
+-rw-r--r--   0        0        0     9357 2024-05-23 10:39:54.830728 argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_records.py
+-rw-r--r--   0        0        0     4618 2024-05-23 10:39:54.830728 argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_users.py
+-rw-r--r--   0        0        0     3214 2024-05-23 10:39:54.830728 argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_vectors.py
+-rw-r--r--   0        0        0     5137 2024-05-23 10:39:54.830728 argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_workspaces.py
+-rw-r--r--   0        0        0      666 2024-05-23 10:39:54.830728 argilla_sdk-0.1.0a3/src/argilla_sdk/_constants.py
+-rw-r--r--   0        0        0      835 2024-05-23 10:39:54.830728 argilla_sdk-0.1.0a3/src/argilla_sdk/_exceptions/__init__.py
+-rw-r--r--   0        0        0     2519 2024-05-23 10:39:54.830728 argilla_sdk-0.1.0a3/src/argilla_sdk/_exceptions/_api.py
+-rw-r--r--   0        0        0     1305 2024-05-23 10:39:54.830728 argilla_sdk-0.1.0a3/src/argilla_sdk/_exceptions/_base.py
+-rw-r--r--   0        0        0      749 2024-05-23 10:39:54.830728 argilla_sdk-0.1.0a3/src/argilla_sdk/_exceptions/_metadata.py
+-rw-r--r--   0        0        0      704 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_exceptions/_serialization.py
+-rw-r--r--   0        0        0      696 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_exceptions/_settings.py
+-rw-r--r--   0        0        0      655 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_helpers/__init__.py
+-rw-r--r--   0        0        0     1033 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_helpers/_dataclasses.py
+-rw-r--r--   0        0        0     1156 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_helpers/_iterator.py
+-rw-r--r--   0        0        0     1096 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_helpers/_log.py
+-rw-r--r--   0        0        0     2393 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_helpers/_mixins.py
+-rw-r--r--   0        0        0     2530 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_helpers/_resource_repr.py
+-rw-r--r--   0        0        0     2224 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/__init__.py
+-rw-r--r--   0        0        0     1260 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_base.py
+-rw-r--r--   0        0        0     1570 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_dataset.py
+-rw-r--r--   0        0        0      587 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_record/__init__.py
+-rw-r--r--   0        0        0      978 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_record/_metadata.py
+-rw-r--r--   0        0        0     2790 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_record/_record.py
+-rw-r--r--   0        0        0     1744 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_record/_response.py
+-rw-r--r--   0        0        0     1373 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_record/_suggestion.py
+-rw-r--r--   0        0        0     1088 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_record/_vector.py
+-rw-r--r--   0        0        0     1320 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_resource.py
+-rw-r--r--   0        0        0     2574 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_search.py
+-rw-r--r--   0        0        0      587 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_settings/__init__.py
+-rw-r--r--   0        0        0     2202 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_settings/_fields.py
+-rw-r--r--   0        0        0     4022 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_settings/_metadata.py
+-rw-r--r--   0        0        0     1562 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_settings/_questions/__init__.py
+-rw-r--r--   0        0        0     2148 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_settings/_questions/_base.py
+-rw-r--r--   0        0        0     1986 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_settings/_questions/_label_selection.py
+-rw-r--r--   0        0        0     1138 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_settings/_questions/_multi_label_selection.py
+-rw-r--r--   0        0        0     1453 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_settings/_questions/_ranking.py
+-rw-r--r--   0        0        0     1356 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_settings/_questions/_rating.py
+-rw-r--r--   0        0        0     2041 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_settings/_questions/_span.py
+-rw-r--r--   0        0        0      866 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_settings/_questions/_text.py
+-rw-r--r--   0        0        0     1671 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_user.py
+-rw-r--r--   0        0        0     1135 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_workspace.py
+-rw-r--r--   0        0        0     4713 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/_resource.py
+-rw-r--r--   0        0        0    10069 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/client.py
+-rw-r--r--   0        0        0      669 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/datasets/__init__.py
+-rw-r--r--   0        0        0     6133 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/datasets/_export.py
+-rw-r--r--   0        0        0     8210 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/datasets/_resource.py
+-rw-r--r--   0        0        0      837 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/records/__init__.py
+-rw-r--r--   0        0        0    15701 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/records/_dataset_records.py
+-rw-r--r--   0        0        0      663 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/records/_export/__init__.py
+-rw-r--r--   0        0        0      587 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/records/_export/_datasets.py
+-rw-r--r--   0        0        0     5979 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/records/_export/_generic.py
+-rw-r--r--   0        0        0     1802 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/records/_helpers.py
+-rw-r--r--   0        0        0    17795 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/records/_resource.py
+-rw-r--r--   0        0        0     4627 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/records/_search.py
+-rw-r--r--   0        0        0     7113 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/responses.py
+-rw-r--r--   0        0        0      820 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/settings/__init__.py
+-rw-r--r--   0        0        0     3301 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/settings/_common.py
+-rw-r--r--   0        0        0     4727 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/settings/_field.py
+-rw-r--r--   0        0        0     7790 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/settings/_metadata.py
+-rw-r--r--   0        0        0    15550 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/settings/_question.py
+-rw-r--r--   0        0        0    14873 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/settings/_resource.py
+-rw-r--r--   0        0        0     5625 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/suggestions.py
+-rw-r--r--   0        0        0      652 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/users/__init__.py
+-rw-r--r--   0        0        0     6373 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/users/_resource.py
+-rw-r--r--   0        0        0     2523 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/vectors.py
+-rw-r--r--   0        0        0      667 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/workspaces/__init__.py
+-rw-r--r--   0        0        0     6768 2024-05-23 10:39:54.834728 argilla_sdk-0.1.0a3/src/argilla_sdk/workspaces/_resource.py
+-rw-r--r--   0        0        0     1099 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/integration/conftest.py
+-rw-r--r--   0        0        0    21227 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/integration/test_add_records.py
+-rw-r--r--   0        0        0     3541 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/integration/test_create_datasets.py
+-rw-r--r--   0        0        0     4459 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/integration/test_dataset_workspace.py
+-rw-r--r--   0        0        0     2401 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/integration/test_empty_settings.py
+-rw-r--r--   0        0        0     3941 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/integration/test_export_dataset.py
+-rw-r--r--   0        0        0     8052 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/integration/test_export_records.py
+-rw-r--r--   0        0        0     2789 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/integration/test_list_records.py
+-rw-r--r--   0        0        0     1360 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/integration/test_listing_datasets.py
+-rw-r--r--   0        0        0     1426 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/integration/test_manage_users.py
+-rw-r--r--   0        0        0     1833 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/integration/test_manage_workspaces.py
+-rw-r--r--   0        0        0     4722 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/integration/test_metadata.py
+-rw-r--r--   0        0        0     2758 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/integration/test_publish_datasets.py
+-rw-r--r--   0        0        0     3457 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/integration/test_query_records.py
+-rw-r--r--   0        0        0     1967 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/integration/test_ranking_questions.py
+-rw-r--r--   0        0        0     3919 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/integration/test_update_records.py
+-rw-r--r--   0        0        0     5056 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/integration/test_vectors.py
+-rw-r--r--   0        0        0     2620 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/unit/api/http/test_http_client.py
+-rw-r--r--   0        0        0      834 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/unit/conftest.py
+-rw-r--r--   0        0        0     2479 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/unit/export/test_record_export_import_compatibillity.py
+-rw-r--r--   0        0        0     2466 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/unit/export/test_settings_export_import_compatibillity.py
+-rw-r--r--   0        0        0     2322 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/unit/helpers/test_resource_repr.py
+-rw-r--r--   0        0        0     1607 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/unit/test_interface.py
+-rw-r--r--   0        0        0     6854 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/unit/test_record_ingestion.py
+-rw-r--r--   0        0        0     5377 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/unit/test_record_responses.py
+-rw-r--r--   0        0        0     1392 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/unit/test_record_suggestions.py
+-rw-r--r--   0        0        0    12204 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/unit/test_resources/test_datasets.py
+-rw-r--r--   0        0        0     1989 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/unit/test_resources/test_fields.py
+-rw-r--r--   0        0        0     5608 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/unit/test_resources/test_questions.py
+-rw-r--r--   0        0        0     2451 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/unit/test_resources/test_records.py
+-rw-r--r--   0        0        0    10785 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/unit/test_resources/test_users.py
+-rw-r--r--   0        0        0    10469 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/unit/test_resources/test_workspaces.py
+-rw-r--r--   0        0        0     1508 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/unit/test_settings/test_multi_label_question.py
+-rw-r--r--   0        0        0     4380 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/unit/test_settings/test_settings.py
+-rw-r--r--   0        0        0     2411 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/unit/test_settings/test_settings_fields.py
+-rw-r--r--   0        0        0     3248 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/unit/test_settings/test_settings_questions.py
+-rw-r--r--   0        0        0     1986 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/unit/test_settings/test_span_question.py
+-rw-r--r--   0        0        0     2868 2024-05-23 10:39:54.838728 argilla_sdk-0.1.0a3/tests/unit/test_settings/test_terms_metadata.py
+-rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 argilla_sdk-0.1.0a3/PKG-INFO
```

### Comparing `argilla_sdk-0.1.0a2/LICENSE` & `argilla_sdk-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/LICENSE_HEADER` & `argilla_sdk-0.1.0a3/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/README.md` & `argilla_sdk-0.1.0a3/README.md`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/pyproject.toml` & `argilla_sdk-0.1.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 requires-python = ">=3.10,<3.12"
 readme = "README.md"
 dynamic = []
 dependencies = [
     "httpx>=0.26.0",
     "pydantic>=2.6.0, <3.0.0",
 ]
-version = "0.1.0a2"
+version = "0.1.0a3"
 
 [project.license]
 text = "Apache 2.0"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/__init__.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 from argilla_sdk.settings import *  # noqa
 from argilla_sdk.suggestions import *  # noqa
 from argilla_sdk.responses import *  # noqa
 from argilla_sdk.records import *  # noqa
 from argilla_sdk.vectors import *  # noqa
 
 
-__version__ = "0.1.0a2"
+__version__ = "0.1.0a3"
```

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_api/__init__.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_base.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_base.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_client.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_client.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_datasets.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_datasets.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_fields.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_fields.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_http/__init__.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_http/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_http/_client.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_http/_client.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_http/_helpers.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_http/_helpers.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_metadata.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_metadata.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_questions.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_questions.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_records.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_records.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_users.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_users.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_vectors.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_vectors.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_api/_workspaces.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_api/_workspaces.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_constants.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_constants.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_exceptions/__init__.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_exceptions/_api.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_exceptions/_api.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_exceptions/_base.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_exceptions/_base.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_exceptions/_metadata.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_exceptions/_metadata.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_exceptions/_serialization.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_exceptions/_serialization.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_exceptions/_settings.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_exceptions/_settings.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_helpers/__init__.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_helpers/_dataclasses.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_helpers/_dataclasses.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_helpers/_iterator.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_helpers/_iterator.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_helpers/_log.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_helpers/_log.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_helpers/_mixins.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_helpers/_mixins.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_helpers/_resource_repr.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_helpers/_resource_repr.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/__init__.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_base.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_base.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_dataset.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_dataset.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_record/__init__.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_record/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_record/_metadata.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_record/_metadata.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_record/_record.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_record/_record.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_record/_response.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_record/_response.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_record/_suggestion.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_record/_suggestion.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_record/_vector.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_record/_vector.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_resource.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_resource.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_search.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_search.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_settings/__init__.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_settings/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_settings/_fields.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_settings/_fields.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_settings/_metadata.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_settings/_metadata.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_settings/_questions/__init__.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_settings/_questions/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_settings/_questions/_base.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_settings/_questions/_base.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_settings/_questions/_label_selection.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_settings/_questions/_label_selection.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_settings/_questions/_multi_label_selection.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_settings/_questions/_multi_label_selection.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_settings/_questions/_ranking.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_settings/_questions/_ranking.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_settings/_questions/_rating.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_settings/_questions/_rating.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_settings/_questions/_span.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_settings/_questions/_span.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_settings/_questions/_text.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_settings/_questions/_text.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_user.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_user.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_models/_workspace.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_models/_workspace.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/_resource.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/_resource.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/client.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/client.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/datasets/__init__.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/datasets/_export.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/datasets/_export.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/datasets/_resource.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/datasets/_resource.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/records/__init__.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/records/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/records/_dataset_records.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/records/_dataset_records.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/records/_export/__init__.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/records/_export/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/records/_export/_datasets.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/records/_export/_datasets.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/records/_export/_generic.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/records/_export/_generic.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/records/_helpers.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/records/_helpers.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/records/_resource.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/records/_resource.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/records/_search.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/records/_search.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/responses.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/responses.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/settings/__init__.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/settings/_common.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/settings/_common.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/settings/_field.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/settings/_field.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/settings/_metadata.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/settings/_metadata.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/settings/_question.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/settings/_question.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/settings/_resource.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/settings/_resource.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/suggestions.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/suggestions.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/users/__init__.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/users/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/users/_resource.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/users/_resource.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/vectors.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/vectors.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/workspaces/__init__.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/src/argilla_sdk/workspaces/_resource.py` & `argilla_sdk-0.1.0a3/src/argilla_sdk/workspaces/_resource.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/integration/conftest.py` & `argilla_sdk-0.1.0a3/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/integration/test_add_records.py` & `argilla_sdk-0.1.0a3/tests/integration/test_add_records.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/integration/test_create_datasets.py` & `argilla_sdk-0.1.0a3/tests/integration/test_create_datasets.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/integration/test_dataset_workspace.py` & `argilla_sdk-0.1.0a3/tests/integration/test_dataset_workspace.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/integration/test_empty_settings.py` & `argilla_sdk-0.1.0a3/tests/integration/test_empty_settings.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/integration/test_export_dataset.py` & `argilla_sdk-0.1.0a3/tests/integration/test_export_dataset.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/integration/test_export_records.py` & `argilla_sdk-0.1.0a3/tests/integration/test_export_records.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/integration/test_list_records.py` & `argilla_sdk-0.1.0a3/tests/integration/test_list_records.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/integration/test_listing_datasets.py` & `argilla_sdk-0.1.0a3/tests/integration/test_listing_datasets.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/integration/test_manage_users.py` & `argilla_sdk-0.1.0a3/tests/integration/test_manage_users.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/integration/test_manage_workspaces.py` & `argilla_sdk-0.1.0a3/tests/integration/test_manage_workspaces.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/integration/test_metadata.py` & `argilla_sdk-0.1.0a3/tests/integration/test_metadata.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/integration/test_publish_datasets.py` & `argilla_sdk-0.1.0a3/tests/integration/test_publish_datasets.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/integration/test_query_records.py` & `argilla_sdk-0.1.0a3/tests/integration/test_query_records.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/integration/test_ranking_questions.py` & `argilla_sdk-0.1.0a3/tests/integration/test_ranking_questions.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/integration/test_update_records.py` & `argilla_sdk-0.1.0a3/tests/integration/test_update_records.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/integration/test_vectors.py` & `argilla_sdk-0.1.0a3/tests/integration/test_vectors.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/unit/api/http/test_http_client.py` & `argilla_sdk-0.1.0a3/tests/unit/api/http/test_http_client.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/unit/conftest.py` & `argilla_sdk-0.1.0a3/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/unit/export/test_record_export_import_compatibillity.py` & `argilla_sdk-0.1.0a3/tests/unit/export/test_record_export_import_compatibillity.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/unit/export/test_settings_export_import_compatibillity.py` & `argilla_sdk-0.1.0a3/tests/unit/export/test_settings_export_import_compatibillity.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/unit/helpers/test_resource_repr.py` & `argilla_sdk-0.1.0a3/tests/unit/helpers/test_resource_repr.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/unit/test_interface.py` & `argilla_sdk-0.1.0a3/tests/unit/test_interface.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/unit/test_record_ingestion.py` & `argilla_sdk-0.1.0a3/tests/unit/test_record_ingestion.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/unit/test_record_responses.py` & `argilla_sdk-0.1.0a3/tests/unit/test_record_responses.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/unit/test_record_suggestions.py` & `argilla_sdk-0.1.0a3/tests/unit/test_record_suggestions.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/unit/test_resources/test_datasets.py` & `argilla_sdk-0.1.0a3/tests/unit/test_resources/test_datasets.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/unit/test_resources/test_fields.py` & `argilla_sdk-0.1.0a3/tests/unit/test_resources/test_fields.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/unit/test_resources/test_questions.py` & `argilla_sdk-0.1.0a3/tests/unit/test_resources/test_questions.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/unit/test_resources/test_records.py` & `argilla_sdk-0.1.0a3/tests/unit/test_resources/test_records.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/unit/test_resources/test_users.py` & `argilla_sdk-0.1.0a3/tests/unit/test_resources/test_users.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/unit/test_resources/test_workspaces.py` & `argilla_sdk-0.1.0a3/tests/unit/test_resources/test_workspaces.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/unit/test_settings/test_multi_label_question.py` & `argilla_sdk-0.1.0a3/tests/unit/test_settings/test_multi_label_question.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/unit/test_settings/test_settings.py` & `argilla_sdk-0.1.0a3/tests/unit/test_settings/test_settings.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/unit/test_settings/test_settings_fields.py` & `argilla_sdk-0.1.0a3/tests/unit/test_settings/test_settings_fields.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/unit/test_settings/test_settings_questions.py` & `argilla_sdk-0.1.0a3/tests/unit/test_settings/test_settings_questions.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/unit/test_settings/test_span_question.py` & `argilla_sdk-0.1.0a3/tests/unit/test_settings/test_span_question.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/tests/unit/test_settings/test_terms_metadata.py` & `argilla_sdk-0.1.0a3/tests/unit/test_settings/test_terms_metadata.py`

 * *Files identical despite different names*

### Comparing `argilla_sdk-0.1.0a2/PKG-INFO` & `argilla_sdk-0.1.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argilla-sdk
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: The Argilla python server SDK
 Author-Email: Argilla <contact@argilla.io>
 License: Apache 2.0
 Requires-Python: <3.12,>=3.10
 Requires-Dist: httpx>=0.26.0
 Requires-Dist: pydantic<3.0.0,>=2.6.0
 Description-Content-Type: text/markdown
```

