# Comparing `tmp/pricecypher_sdk-2.1.0.tar.gz` & `tmp/pricecypher_sdk-2.1.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pricecypher_sdk-2.1.0.tar", last modified: Thu Apr 25 11:28:05 2024, max compression
+gzip compressed data, was "pricecypher_sdk-2.1.1.dev8.tar", last modified: Thu May 23 12:56:08 2024, max compression
```

## Comparing `pricecypher_sdk-2.1.0.tar` & `pricecypher_sdk-2.1.1.dev8.tar`

### file list

```diff
@@ -1,72 +1,76 @@
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.987990 pricecypher_sdk-2.1.0/
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.719811 pricecypher_sdk-2.1.0/.github/
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.727433 pricecypher_sdk-2.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      968 2022-03-25 10:57:36.000000 pricecypher_sdk-2.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      595 2022-03-25 10:57:36.000000 pricecypher_sdk-2.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1129 2022-03-25 10:57:36.000000 pricecypher_sdk-2.1.0/.github/pull_request_template.md
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.791678 pricecypher_sdk-2.1.0/.idea/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      176 2022-05-17 11:22:56.000000 pricecypher_sdk-2.1.0/.idea/.gitignore
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.796941 pricecypher_sdk-2.1.0/.idea/inspectionProfiles/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      174 2022-05-17 11:22:56.000000 pricecypher_sdk-2.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      283 2024-04-25 08:49:40.000000 pricecypher_sdk-2.1.0/.idea/misc.xml
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      519 2024-04-25 08:39:04.000000 pricecypher_sdk-2.1.0/.idea/modules.xml
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      504 2022-05-17 11:22:56.000000 pricecypher_sdk-2.1.0/.idea/pricecypher_python_api.iml
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      603 2024-04-25 08:49:40.000000 pricecypher_sdk-2.1.0/.idea/pricecypher_python_sdk.iml
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      167 2024-04-25 08:39:04.000000 pricecypher_sdk-2.1.0/.idea/vcs.xml
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1544 2024-04-25 11:28:05.000000 pricecypher_sdk-2.1.0/ChangeLog
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1080 2022-03-25 10:57:36.000000 pricecypher_sdk-2.1.0/LICENSE
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      895 2024-04-25 11:28:05.987613 pricecypher_sdk-2.1.0/PKG-INFO
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     3241 2023-09-28 11:29:21.000000 pricecypher_sdk-2.1.0/README.md
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      110 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.0/pyproject.toml
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      121 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.0/requirements.txt
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      781 2024-04-25 11:28:05.992354 pricecypher_sdk-2.1.0/setup.cfg
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      104 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.0/setup.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.707491 pricecypher_sdk-2.1.0/src/
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.819284 pricecypher_sdk-2.1.0/src/pricecypher/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      298 2024-04-25 09:35:27.000000 pricecypher_sdk-2.1.0/src/pricecypher/__init__.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.840663 pricecypher_sdk-2.1.0/src/pricecypher/collections/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      666 2022-05-17 11:22:56.000000 pricecypher_sdk-2.1.0/src/pricecypher/collections/base_collection.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1179 2024-04-25 09:37:26.000000 pricecypher_sdk-2.1.0/src/pricecypher/collections/scope_collection.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1131 2024-04-25 09:38:50.000000 pricecypher_sdk-2.1.0/src/pricecypher/collections/scope_value_collection.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     2337 2023-08-22 09:53:07.000000 pricecypher_sdk-2.1.0/src/pricecypher/config_sections.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.862416 pricecypher_sdk-2.1.0/src/pricecypher/contracts/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1240 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.0/src/pricecypher/contracts/QualityTestScript.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1824 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.0/src/pricecypher/contracts/ScopeScript.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     2448 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.0/src/pricecypher/contracts/Script.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      161 2022-10-07 15:03:39.000000 pricecypher_sdk-2.1.0/src/pricecypher/contracts/__init__.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.872661 pricecypher_sdk-2.1.0/src/pricecypher/contracts/dataclasses/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     3054 2022-11-02 15:42:11.000000 pricecypher_sdk-2.1.0/src/pricecypher/contracts/dataclasses/TestResult.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)       26 2022-10-07 15:34:17.000000 pricecypher_sdk-2.1.0/src/pricecypher/contracts/dataclasses/__init__.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.880055 pricecypher_sdk-2.1.0/src/pricecypher/contracts/enums/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      119 2022-10-07 14:52:35.000000 pricecypher_sdk-2.1.0/src/pricecypher/contracts/enums/TestStatus.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)       35 2022-10-07 15:03:58.000000 pricecypher_sdk-2.1.0/src/pricecypher/contracts/enums/__init__.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)    17731 2024-04-25 10:19:01.000000 pricecypher_sdk-2.1.0/src/pricecypher/datasets.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.887802 pricecypher_sdk-2.1.0/src/pricecypher/encoders/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      572 2022-10-20 11:57:22.000000 pricecypher_sdk-2.1.0/src/pricecypher/encoders/JsonEncoder.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)       48 2022-10-20 11:55:13.000000 pricecypher_sdk-2.1.0/src/pricecypher/encoders/__init__.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.919247 pricecypher_sdk-2.1.0/src/pricecypher/endpoints/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      107 2023-08-22 09:53:07.000000 pricecypher_sdk-2.1.0/src/pricecypher/endpoints/__init__.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      808 2022-09-30 14:31:36.000000 pricecypher_sdk-2.1.0/src/pricecypher/endpoints/base_endpoint.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     2156 2023-08-22 09:53:08.000000 pricecypher_sdk-2.1.0/src/pricecypher/endpoints/config.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     5245 2024-04-25 08:28:14.000000 pricecypher_sdk-2.1.0/src/pricecypher/endpoints/datasets.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1517 2023-09-28 11:29:21.000000 pricecypher_sdk-2.1.0/src/pricecypher/endpoints/users.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      509 2022-09-30 14:31:36.000000 pricecypher_sdk-2.1.0/src/pricecypher/exceptions.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.949211 pricecypher_sdk-2.1.0/src/pricecypher/models/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      238 2023-08-22 09:53:08.000000 pricecypher_sdk-2.1.0/src/pricecypher/models/__init__.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1355 2023-08-22 09:53:08.000000 pricecypher_sdk-2.1.0/src/pricecypher/models/config.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     3493 2023-08-22 09:53:08.000000 pricecypher_sdk-2.1.0/src/pricecypher/models/datasets.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      843 2022-07-29 09:08:07.000000 pricecypher_sdk-2.1.0/src/pricecypher/models/namespaced_schema.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      667 2023-08-22 09:53:08.000000 pricecypher_sdk-2.1.0/src/pricecypher/models/users.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)    12425 2023-09-28 11:29:21.000000 pricecypher_sdk-2.1.0/src/pricecypher/rest.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.985868 pricecypher_sdk-2.1.0/src/pricecypher_sdk.egg-info/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      895 2024-04-25 11:28:05.000000 pricecypher_sdk-2.1.0/src/pricecypher_sdk.egg-info/PKG-INFO
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1838 2024-04-25 11:28:05.000000 pricecypher_sdk-2.1.0/src/pricecypher_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 marvanderhorst   (502) staff       (20)        1 2024-04-25 11:28:05.000000 pricecypher_sdk-2.1.0/src/pricecypher_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 marvanderhorst   (502) staff       (20)       50 2024-04-25 11:28:05.000000 pricecypher_sdk-2.1.0/src/pricecypher_sdk.egg-info/entry_points.txt
--rw-r--r--   0 marvanderhorst   (502) staff       (20)        1 2023-09-28 15:14:04.000000 pricecypher_sdk-2.1.0/src/pricecypher_sdk.egg-info/not-zip-safe
--rw-r--r--   0 marvanderhorst   (502) staff       (20)       47 2024-04-25 11:28:05.000000 pricecypher_sdk-2.1.0/src/pricecypher_sdk.egg-info/pbr.json
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      145 2024-04-25 11:28:05.000000 pricecypher_sdk-2.1.0/src/pricecypher_sdk.egg-info/requires.txt
--rw-r--r--   0 marvanderhorst   (502) staff       (20)       12 2024-04-25 11:28:05.000000 pricecypher_sdk-2.1.0/src/pricecypher_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.984225 pricecypher_sdk-2.1.0/tests/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)        0 2022-05-17 11:22:56.000000 pricecypher_sdk-2.1.0/tests/__init__.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)    25448 2022-05-17 11:22:56.000000 pricecypher_sdk-2.1.0/tests/test_rest.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.772449 pricecypher_sdk-2.1.1.dev8/
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.705824 pricecypher_sdk-2.1.1.dev8/.github/
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.711556 pricecypher_sdk-2.1.1.dev8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      968 2022-03-25 10:57:36.000000 pricecypher_sdk-2.1.1.dev8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      595 2022-03-25 10:57:36.000000 pricecypher_sdk-2.1.1.dev8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1129 2022-03-25 10:57:36.000000 pricecypher_sdk-2.1.1.dev8/.github/pull_request_template.md
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.717175 pricecypher_sdk-2.1.1.dev8/.idea/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      372 2024-05-23 11:12:21.000000 pricecypher_sdk-2.1.1.dev8/.idea/.gitignore
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.720323 pricecypher_sdk-2.1.1.dev8/.idea/inspectionProfiles/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      174 2022-05-17 11:22:56.000000 pricecypher_sdk-2.1.1.dev8/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      181 2024-05-23 12:45:46.000000 pricecypher_sdk-2.1.1.dev8/.idea/vcs.xml
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1756 2024-05-23 12:56:07.000000 pricecypher_sdk-2.1.1.dev8/ChangeLog
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1080 2022-03-25 10:57:36.000000 pricecypher_sdk-2.1.1.dev8/LICENSE
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1805 2024-05-23 12:56:08.772073 pricecypher_sdk-2.1.1.dev8/PKG-INFO
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      385 2024-05-23 11:12:22.000000 pricecypher_sdk-2.1.1.dev8/Pipfile
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)    68635 2024-05-23 11:12:22.000000 pricecypher_sdk-2.1.1.dev8/Pipfile.lock
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     3241 2023-09-28 11:29:21.000000 pricecypher_sdk-2.1.1.dev8/README.md
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      110 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.1.dev8/pyproject.toml
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      781 2024-05-23 12:56:08.775492 pricecypher_sdk-2.1.1.dev8/setup.cfg
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      104 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.1.dev8/setup.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.688001 pricecypher_sdk-2.1.1.dev8/src/
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.723861 pricecypher_sdk-2.1.1.dev8/src/pricecypher/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      484 2024-05-23 12:35:35.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/__init__.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.725973 pricecypher_sdk-2.1.1.dev8/src/pricecypher/collections/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      666 2022-05-17 11:22:56.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/collections/base_collection.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1179 2024-05-23 11:12:21.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/collections/scope_collection.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1131 2024-05-23 11:12:21.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/collections/scope_value_collection.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     2337 2023-08-22 09:53:07.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/config_sections.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.730771 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1639 2024-05-23 12:48:40.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/BaseHandler.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      760 2024-05-23 12:53:16.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/InferenceHandler.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1240 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/QualityTestScript.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1824 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/ScopeScript.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1664 2024-05-23 12:54:10.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/Script.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      245 2024-05-23 12:54:46.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/__init__.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.733413 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/dataclasses/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     3349 2024-05-23 12:46:35.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/dataclasses/PredictResult.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     3054 2022-11-02 15:42:11.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/dataclasses/TestResult.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)       54 2024-05-23 12:46:35.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/dataclasses/__init__.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.735691 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/enums/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      109 2024-05-23 12:01:21.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/enums/Accuracy.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      119 2022-10-07 14:52:35.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/enums/TestStatus.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)       66 2024-05-23 12:46:35.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/enums/__init__.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)    17732 2024-05-23 11:12:21.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/datasets.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.737162 pricecypher_sdk-2.1.1.dev8/src/pricecypher/encoders/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      572 2022-10-20 11:57:22.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/encoders/JsonEncoder.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)       48 2022-10-20 11:55:13.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/encoders/__init__.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.740864 pricecypher_sdk-2.1.1.dev8/src/pricecypher/endpoints/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      107 2023-08-22 09:53:07.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/endpoints/__init__.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      808 2022-09-30 14:31:36.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/endpoints/base_endpoint.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     2150 2024-05-23 11:12:22.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/endpoints/config.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     5245 2024-04-25 08:28:14.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/endpoints/datasets.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1517 2023-09-28 11:29:21.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/endpoints/users.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     4068 2024-05-23 12:45:00.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/exceptions.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.744545 pricecypher_sdk-2.1.1.dev8/src/pricecypher/models/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      238 2023-08-22 09:53:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/models/__init__.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1355 2023-08-22 09:53:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/models/config.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     3493 2023-08-22 09:53:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/models/datasets.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      843 2022-07-29 09:08:07.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/models/namespaced_schema.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      667 2023-08-22 09:53:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/models/users.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.745919 pricecypher_sdk-2.1.1.dev8/src/pricecypher/oidc/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)       61 2024-05-23 11:12:22.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/oidc/__init__.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     2657 2024-05-23 11:12:22.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/oidc/auth.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)    12259 2024-05-23 11:12:22.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/rest.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.770678 pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1805 2024-05-23 12:56:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1991 2024-05-23 12:56:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)        1 2024-05-23 12:56:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)       50 2024-05-23 12:56:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)        1 2024-05-23 12:56:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)       47 2024-05-23 12:56:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/pbr.json
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      645 2024-05-23 12:56:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/requires.txt
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)       12 2024-05-23 12:56:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.768997 pricecypher_sdk-2.1.1.dev8/tests/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)        0 2022-05-17 11:22:56.000000 pricecypher_sdk-2.1.1.dev8/tests/__init__.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)    25578 2024-05-23 11:12:22.000000 pricecypher_sdk-2.1.1.dev8/tests/test_rest.py
```

### Comparing `pricecypher_sdk-2.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `pricecypher_sdk-2.1.1.dev8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `pricecypher_sdk-2.1.1.dev8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.0/.github/pull_request_template.md` & `pricecypher_sdk-2.1.1.dev8/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.0/ChangeLog` & `pricecypher_sdk-2.1.1.dev8/ChangeLog`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 CHANGES
 =======
 
+* Refactor contracts
+* Update contracts and exceptions
+* Update gitignore
+* Add access token generator
+* Update dependencies
+* Update exceptions
+* Restructure location of collections module
+* Update .idea files
+
 v2.1.0
 ------
 
 * Release v2.1.0 to master (#34)
 * Add dataset environment parameter to \`get\_transactions\` (#33)
 
 v2.0.0
```

### Comparing `pricecypher_sdk-2.1.0/LICENSE` & `pricecypher_sdk-2.1.1.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.0/PKG-INFO` & `pricecypher_sdk-2.1.1.dev8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,51 @@
 Metadata-Version: 2.1
 Name: pricecypher-sdk
-Version: 2.1.0
+Version: 2.1.1.dev8
 Summary: Python wrapper around the different PriceCypher APIs
 Home-page: https://github.com/marketredesign/pricecypher_python_sdk
 Author: Deloitte Consulting B.V.
 Project-URL: Bug Tracker, https://github.com/marketredesign/pricecypher_python_sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: better-abc>=0.0.3
-Requires-Dist: requests>=2.14.0
-Requires-Dist: marshmallow-dataclass>=8.5.3
-Requires-Dist: pandas>=1.4.1
-Requires-Dist: numpy>=1.18.5
-Requires-Dist: typeguard>=2.13.3
-Requires-Dist: pbr>=5.11.1
+Requires-Dist: annotated-types==0.7.0
+Requires-Dist: better-abc==0.0.3
+Requires-Dist: certifi==2024.2.2
+Requires-Dist: cffi==1.16.0
+Requires-Dist: charset-normalizer==3.3.2
+Requires-Dist: cryptography==42.0.7
+Requires-Dist: defusedxml==0.7.1
+Requires-Dist: future==1.0.0
+Requires-Dist: idna==3.7
+Requires-Dist: mako==1.3.5
+Requires-Dist: markupsafe==2.1.5
+Requires-Dist: marshmallow==3.21.2
+Requires-Dist: marshmallow-dataclass==8.6.1
+Requires-Dist: mypy-extensions==1.0.0
+Requires-Dist: numpy==1.26.4
+Requires-Dist: oic==1.7.0
+Requires-Dist: packaging==24.0
+Requires-Dist: pandas==2.2.2
+Requires-Dist: pycparser==2.22
+Requires-Dist: pycryptodomex==3.20.0
+Requires-Dist: pydantic==2.7.1
+Requires-Dist: pydantic-core==2.18.2
+Requires-Dist: pydantic-settings==2.2.1
+Requires-Dist: pyjwkest==1.4.2
+Requires-Dist: python-dateutil==2.9.0.post0
+Requires-Dist: python-dotenv==1.0.1
+Requires-Dist: pytz==2024.1
+Requires-Dist: requests==2.32.2
+Requires-Dist: six==1.16.0
+Requires-Dist: typeguard==4.2.1
+Requires-Dist: typing-extensions==4.11.0
+Requires-Dist: typing-inspect==0.9.0
+Requires-Dist: tzdata==2024.1
+Requires-Dist: urllib3==2.2.1
 Provides-Extra: testing
 Requires-Dist: mock>=1.3.0; extra == "testing"
 
 Python wrapper around the different PriceCypher APIs
```

### Comparing `pricecypher_sdk-2.1.0/README.md` & `pricecypher_sdk-2.1.1.dev8/README.md`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.0/setup.cfg` & `pricecypher_sdk-2.1.1.dev8/setup.cfg`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.0/src/pricecypher/collections/base_collection.py` & `pricecypher_sdk-2.1.1.dev8/src/pricecypher/collections/base_collection.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.0/src/pricecypher/collections/scope_collection.py` & `pricecypher_sdk-2.1.1.dev8/src/pricecypher/collections/scope_collection.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from .base_collection import BaseCollection
 from pricecypher.models import Scope
+from .base_collection import BaseCollection
 
 
 class ScopeCollection(BaseCollection):
     _type = Scope
 
     def __repr__(self):
         return f"<{self.__class__.__name__} {self._list}>"
```

### Comparing `pricecypher_sdk-2.1.0/src/pricecypher/collections/scope_value_collection.py` & `pricecypher_sdk-2.1.1.dev8/src/pricecypher/collections/scope_value_collection.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from .base_collection import BaseCollection
 from pricecypher.models import ScopeValue
+from .base_collection import BaseCollection
 
 
 class ScopeValueCollection(BaseCollection):
     _type = ScopeValue
 
     def __repr__(self):
         return f"<{self.__class__.__name__} {self._list}>"
```

### Comparing `pricecypher_sdk-2.1.0/src/pricecypher/config_sections.py` & `pricecypher_sdk-2.1.1.dev8/src/pricecypher/config_sections.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.0/src/pricecypher/contracts/QualityTestScript.py` & `pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/QualityTestScript.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.0/src/pricecypher/contracts/ScopeScript.py` & `pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/ScopeScript.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.0/src/pricecypher/contracts/Script.py` & `pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/Script.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,34 @@
 from abc import ABC, abstractmethod
-from typing import Any, Optional, Annotated, Callable
+from typing import Any, Optional, Callable
 
+from pricecypher import BaseHandler
 
-class Script(ABC):
+
+class Script(BaseHandler, ABC):
     """
     The abstract Script class serves as an interaction contract such that by extending it with its methods implemented,
         a script can be created that can be used in a generalized yet controlled setting.
     """
 
-    dataset_id: Annotated[int, "The dataset ID"]
-    settings: dict[str, Any]
-    config: dict[str, dict[str, Any]]
-
-    def __init__(self, dataset_id: int, settings: dict[str, Any], config: dict[str, dict[str, Any]]):
-        self.dataset_id = dataset_id
-        self.settings = settings
-        self.config = config
-
-    @abstractmethod
-    def get_config_dependencies(self) -> dict[str, list[str]]:
-        """
-        Fetch the configuration sections and keys in the sections that the script will use that are not yet provided.
-
-        NB: It is not needed to return all required sections and keys, only at least one that has not been provided yet.
-        If all required config is provided, an empty dictionary is to be returned.
-
-        :return: dictionary mapping from section key (string) to a (potentially empty) list of keys of that section
-            that the script requires additionally.
-        """
-        raise NotImplementedError
-
     @abstractmethod
     def get_scope_dependencies(self) -> list[dict[str, Any]]:
         """
         Fetch the scopes that the script will use and requires to be present in the dataset.
 
         NB: All required config is assumed to be present.
 
         :return: List of required scopes, where each is a dictionary containing either
             a 'representation' or a 'scope_id'.
         """
         raise NotImplementedError
 
+    def handle(self, user_input: dict[Any: Any]) -> any:
+        return self.execute('all', self._get_access_token, user_input)
+
     @abstractmethod
     def execute(
         self,
         business_cell_id: Optional[int],
         get_bearer_token: Callable[[], str],
         user_input: dict[Any: Any],
     ) -> Any:
```

### Comparing `pricecypher_sdk-2.1.0/src/pricecypher/contracts/dataclasses/TestResult.py` & `pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/dataclasses/TestResult.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.0/src/pricecypher/datasets.py` & `pricecypher_sdk-2.1.1.dev8/src/pricecypher/datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import datetime
+
 from pandas import DataFrame
 
 from pricecypher.endpoints import DatasetsEndpoint, UsersEndpoint
 from .collections.scope_collection import ScopeCollection
 from .collections.scope_value_collection import ScopeValueCollection
```

### Comparing `pricecypher_sdk-2.1.0/src/pricecypher/encoders/JsonEncoder.py` & `pricecypher_sdk-2.1.1.dev8/src/pricecypher/encoders/JsonEncoder.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.0/src/pricecypher/endpoints/base_endpoint.py` & `pricecypher_sdk-2.1.1.dev8/src/pricecypher/endpoints/base_endpoint.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.0/src/pricecypher/endpoints/config.py` & `pricecypher_sdk-2.1.1.dev8/src/pricecypher/endpoints/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 
 from pricecypher.endpoints.base_endpoint import BaseEndpoint
-from pricecypher.exceptions import PriceCypherError
+from pricecypher.exceptions import HttpException
 from pricecypher.models import ConfigSection, ConfigSectionWithKeys
 
 
 class ConfigEndpoint(BaseEndpoint):
     """PriceCypher config service endpoints.
 
     :param RestClient client: HTTP client for making API requests.
@@ -48,12 +48,12 @@
 
         :param str section_key: Key of the section to retrieve.
         :return: The requested config section with its contained key-value pairs, or `None` if no such section exists.
         :rtype Optional[ConfigSectionWithKeys]
         """
         try:
             return self.client.get(self._url(section_key), schema=ConfigSectionWithKeys.Schema(many=False))
-        except PriceCypherError as e:
+        except HttpException as e:
             if e.status_code == 404:
                 return None
             else:
                 raise e
```

### Comparing `pricecypher_sdk-2.1.0/src/pricecypher/endpoints/datasets.py` & `pricecypher_sdk-2.1.1.dev8/src/pricecypher/endpoints/datasets.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.0/src/pricecypher/endpoints/users.py` & `pricecypher_sdk-2.1.1.dev8/src/pricecypher/endpoints/users.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.0/src/pricecypher/models/config.py` & `pricecypher_sdk-2.1.1.dev8/src/pricecypher/models/config.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.0/src/pricecypher/models/datasets.py` & `pricecypher_sdk-2.1.1.dev8/src/pricecypher/models/datasets.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.0/src/pricecypher/models/namespaced_schema.py` & `pricecypher_sdk-2.1.1.dev8/src/pricecypher/models/namespaced_schema.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.0/src/pricecypher/models/users.py` & `pricecypher_sdk-2.1.1.dev8/src/pricecypher/models/users.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.0/src/pricecypher/rest.py` & `pricecypher_sdk-2.1.1.dev8/src/pricecypher/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import datetime
 from random import randint
 from time import sleep
 
 import requests
 from marshmallow import Schema, EXCLUDE
 
-from .exceptions import PriceCypherError, RateLimitError
+from .exceptions import RateLimitError, HttpException
 
 UNKNOWN_ERROR = 'pricecypher.sdk.internal.unknown'
 
 # Mapping from (wildcard) domains to IP addresses to resolve manually.
 dns_cache = {}
 # Keep track of original getaddrinfo function to use for domain names not in our custom cache.
 prv_getaddrinfo = socket.getaddrinfo
@@ -277,21 +277,17 @@
         self._content = content
         self._headers = headers
 
     def content(self):
         if self._is_error():
             if self._status_code == 429:
                 reset_at = int(self._headers.get('x-ratelimit-reset', '-1'))
-                raise RateLimitError(error_code=self._error_code(),
-                                     message=self._error_message(),
-                                     reset_at=reset_at)
-
-            raise PriceCypherError(status_code=self._status_code,
-                                   error_code=self._error_code(),
-                                   message=self._error_message())
+                raise RateLimitError(self._error_message(), error_code=self._error_code(), reset_at=reset_at)
+
+            raise HttpException(self._error_message(), status_code=self._status_code, error_code=self._error_code())
         else:
             return self._content
 
     def _is_error(self):
         return self._status_code is None or self._status_code >= 400
 
     # Force implementation in subclasses
```

### Comparing `pricecypher_sdk-2.1.0/src/pricecypher_sdk.egg-info/PKG-INFO` & `pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,51 @@
 Metadata-Version: 2.1
 Name: pricecypher-sdk
-Version: 2.1.0
+Version: 2.1.1.dev8
 Summary: Python wrapper around the different PriceCypher APIs
 Home-page: https://github.com/marketredesign/pricecypher_python_sdk
 Author: Deloitte Consulting B.V.
 Project-URL: Bug Tracker, https://github.com/marketredesign/pricecypher_python_sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: better-abc>=0.0.3
-Requires-Dist: requests>=2.14.0
-Requires-Dist: marshmallow-dataclass>=8.5.3
-Requires-Dist: pandas>=1.4.1
-Requires-Dist: numpy>=1.18.5
-Requires-Dist: typeguard>=2.13.3
-Requires-Dist: pbr>=5.11.1
+Requires-Dist: annotated-types==0.7.0
+Requires-Dist: better-abc==0.0.3
+Requires-Dist: certifi==2024.2.2
+Requires-Dist: cffi==1.16.0
+Requires-Dist: charset-normalizer==3.3.2
+Requires-Dist: cryptography==42.0.7
+Requires-Dist: defusedxml==0.7.1
+Requires-Dist: future==1.0.0
+Requires-Dist: idna==3.7
+Requires-Dist: mako==1.3.5
+Requires-Dist: markupsafe==2.1.5
+Requires-Dist: marshmallow==3.21.2
+Requires-Dist: marshmallow-dataclass==8.6.1
+Requires-Dist: mypy-extensions==1.0.0
+Requires-Dist: numpy==1.26.4
+Requires-Dist: oic==1.7.0
+Requires-Dist: packaging==24.0
+Requires-Dist: pandas==2.2.2
+Requires-Dist: pycparser==2.22
+Requires-Dist: pycryptodomex==3.20.0
+Requires-Dist: pydantic==2.7.1
+Requires-Dist: pydantic-core==2.18.2
+Requires-Dist: pydantic-settings==2.2.1
+Requires-Dist: pyjwkest==1.4.2
+Requires-Dist: python-dateutil==2.9.0.post0
+Requires-Dist: python-dotenv==1.0.1
+Requires-Dist: pytz==2024.1
+Requires-Dist: requests==2.32.2
+Requires-Dist: six==1.16.0
+Requires-Dist: typeguard==4.2.1
+Requires-Dist: typing-extensions==4.11.0
+Requires-Dist: typing-inspect==0.9.0
+Requires-Dist: tzdata==2024.1
+Requires-Dist: urllib3==2.2.1
 Provides-Extra: testing
 Requires-Dist: mock>=1.3.0; extra == "testing"
 
 Python wrapper around the different PriceCypher APIs
```

### Comparing `pricecypher_sdk-2.1.0/src/pricecypher_sdk.egg-info/SOURCES.txt` & `pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 ChangeLog
 LICENSE
+Pipfile
+Pipfile.lock
 README.md
 pyproject.toml
-requirements.txt
 setup.cfg
 setup.py
 .github/pull_request_template.md
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .idea/.gitignore
-.idea/misc.xml
-.idea/modules.xml
-.idea/pricecypher_python_api.iml
-.idea/pricecypher_python_sdk.iml
 .idea/vcs.xml
 .idea/inspectionProfiles/profiles_settings.xml
 src/pricecypher/__init__.py
 src/pricecypher/config_sections.py
 src/pricecypher/datasets.py
 src/pricecypher/exceptions.py
 src/pricecypher/rest.py
 src/pricecypher/collections/base_collection.py
 src/pricecypher/collections/scope_collection.py
 src/pricecypher/collections/scope_value_collection.py
+src/pricecypher/contracts/BaseHandler.py
+src/pricecypher/contracts/InferenceHandler.py
 src/pricecypher/contracts/QualityTestScript.py
 src/pricecypher/contracts/ScopeScript.py
 src/pricecypher/contracts/Script.py
 src/pricecypher/contracts/__init__.py
+src/pricecypher/contracts/dataclasses/PredictResult.py
 src/pricecypher/contracts/dataclasses/TestResult.py
 src/pricecypher/contracts/dataclasses/__init__.py
+src/pricecypher/contracts/enums/Accuracy.py
 src/pricecypher/contracts/enums/TestStatus.py
 src/pricecypher/contracts/enums/__init__.py
 src/pricecypher/encoders/JsonEncoder.py
 src/pricecypher/encoders/__init__.py
 src/pricecypher/endpoints/__init__.py
 src/pricecypher/endpoints/base_endpoint.py
 src/pricecypher/endpoints/config.py
 src/pricecypher/endpoints/datasets.py
 src/pricecypher/endpoints/users.py
 src/pricecypher/models/__init__.py
 src/pricecypher/models/config.py
 src/pricecypher/models/datasets.py
 src/pricecypher/models/namespaced_schema.py
 src/pricecypher/models/users.py
+src/pricecypher/oidc/__init__.py
+src/pricecypher/oidc/auth.py
 src/pricecypher_sdk.egg-info/PKG-INFO
 src/pricecypher_sdk.egg-info/SOURCES.txt
 src/pricecypher_sdk.egg-info/dependency_links.txt
 src/pricecypher_sdk.egg-info/entry_points.txt
 src/pricecypher_sdk.egg-info/not-zip-safe
 src/pricecypher_sdk.egg-info/pbr.json
 src/pricecypher_sdk.egg-info/requires.txt
```

### Comparing `pricecypher_sdk-2.1.0/tests/test_rest.py` & `pricecypher_sdk-2.1.1.dev8/tests/test_rest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import unittest
 import json
+import unittest
 
 import mock
 import requests
 
+from pricecypher.exceptions import RateLimitError, HttpException
 from pricecypher.rest import RestClient, RestClientOptions
-from pricecypher.exceptions import PriceCypherError, RateLimitError
 
 
 class TestRest(unittest.TestCase):
     TIMEOUT_DEF = 300.0
 
     @classmethod
     def setUpClass(cls):
@@ -56,78 +56,78 @@
         headers = self.static_response_headers | {
             'Authorization': 'Bearer a-token',
         }
         mock_get.return_value.text = '["a", "b"]'
         mock_get.return_value.status_code = 200
 
         rc.get('the-url')
-        mock_get.assert_called_with('the-url', params=None, headers=headers, timeout=(10, 2))
+        mock_get.assert_called_with('the-url', params=None, headers=headers, timeout=(10, 2), verify=True)
 
     @mock.patch('requests.post')
     def test_post_custom_timeout(self, mock_post):
         rc = RestClient(jwt='a-token', options=self.tuple_timeout_options)
         headers = self.static_response_headers | {
             'Authorization': 'Bearer a-token',
         }
         mock_post.return_value.text = '["a", "b"]'
         mock_post.return_value.status_code = 200
 
         rc.post('the-url')
-        mock_post.assert_called_with('the-url', data='null', headers=headers, timeout=(10, 2))
+        mock_post.assert_called_with('the-url', data='null', headers=headers, timeout=(10, 2), verify=True)
 
     @mock.patch('requests.put')
     def test_put_custom_timeout(self, mock_put):
         rc = RestClient(jwt='a-token', options=self.tuple_timeout_options)
         headers = self.static_response_headers | {'Authorization': 'Bearer a-token'}
 
         mock_put.return_value.text = '["a", "b"]'
         mock_put.return_value.status_code = 200
 
         rc.put('the-url')
-        mock_put.assert_called_with('the-url', json=None, headers=headers, timeout=(10, 2))
+        mock_put.assert_called_with('the-url', json=None, headers=headers, timeout=(10, 2), verify=True)
 
     @mock.patch('requests.patch')
     def test_patch_custom_timeout(self, mock_patch):
         rc = RestClient(jwt='a-token', options=self.tuple_timeout_options)
         headers = self.static_response_headers | {'Authorization': 'Bearer a-token'}
 
         mock_patch.return_value.text = '["a", "b"]'
         mock_patch.return_value.status_code = 200
 
         rc.patch('the-url')
-        mock_patch.assert_called_with('the-url', json=None, headers=headers, timeout=(10, 2))
+        mock_patch.assert_called_with('the-url', json=None, headers=headers, timeout=(10, 2), verify=True)
 
     @mock.patch('requests.delete')
     def test_delete_custom_timeout(self, mock_delete):
         rc = RestClient(jwt='a-token', options=self.tuple_timeout_options)
         headers = self.static_response_headers | {'Authorization': 'Bearer a-token'}
 
         mock_delete.return_value.text = '["a", "b"]'
         mock_delete.return_value.status_code = 200
 
         rc.delete('the-url')
-        mock_delete.assert_called_with('the-url', params={}, json=None, headers=headers, timeout=(10, 2))
+        mock_delete.assert_called_with('the-url', params={}, json=None, headers=headers, timeout=(10, 2), verify=True)
 
     @mock.patch('requests.get')
     def test_get(self, mock_get):
         rc = RestClient(jwt='a-token')
         headers = self.static_response_headers | {'Authorization': 'Bearer a-token'}
 
         mock_get.return_value.text = '["a", "b"]'
         mock_get.return_value.status_code = 200
 
         response = rc.get('the-url')
-        mock_get.assert_called_with('the-url', params=None, headers=headers, timeout=self.TIMEOUT_DEF)
+        mock_get.assert_called_with('the-url', params=None, headers=headers, timeout=self.TIMEOUT_DEF, verify=True)
 
         self.assertEqual(response, ['a', 'b'])
 
         response = rc.get(url='the/url', params={'A': 'param', 'B': 'param'})
         mock_get.assert_called_with('the/url', params={'A': 'param',
                                                        'B': 'param'},
-                                    headers=headers, timeout=self.TIMEOUT_DEF)
+                                    headers=headers, timeout=self.TIMEOUT_DEF, verify=True)
         self.assertEqual(response, ['a', 'b'])
 
         mock_get.return_value.text = ''
         response = rc.get('the/url')
         self.assertEqual(response, '')
 
     @mock.patch('requests.get')
@@ -135,19 +135,19 @@
         rc = RestClient(jwt='a-token')
 
         mock_get.return_value.text = '{"statusCode": 999,' \
                                      ' "errorCode": "code",' \
                                      ' "message": "message"}'
         mock_get.return_value.status_code = 999
 
-        with self.assertRaises(PriceCypherError) as context:
+        with self.assertRaises(HttpException) as context:
             rc.get('the/url')
 
         self.assertEqual(context.exception.status_code, 999)
-        self.assertEqual(context.exception.error_code, 'code')
+        self.assertEqual(context.exception.code, 'code')
         self.assertEqual(context.exception.message, 'message')
 
     @mock.patch('requests.get')
     def test_get_rate_limit_error(self, mock_get):
         options = RestClientOptions(retries=0)
         rc = RestClient(jwt='a-token', options=options)
         rc._skip_sleep = True
@@ -158,19 +158,19 @@
         mock_get.return_value.status_code = 429
         mock_get.return_value.headers = {
             'x-ratelimit-limit': '3',
             'x-ratelimit-remaining': '6',
             'x-ratelimit-reset': '9',
         }
 
-        with self.assertRaises(PriceCypherError) as context:
+        with self.assertRaises(HttpException) as context:
             rc.get('the/url')
 
         self.assertEqual(context.exception.status_code, 429)
-        self.assertEqual(context.exception.error_code, 'code')
+        self.assertEqual(context.exception.code, 'code')
         self.assertEqual(context.exception.message, 'message')
         self.assertIsInstance(context.exception, RateLimitError)
         self.assertEqual(context.exception.reset_at, 9)
 
         self.assertEqual(rc._metrics['retries'], 0)
 
     @mock.patch('requests.get')
@@ -180,19 +180,19 @@
 
         mock_get.return_value.text = '{"statusCode": 429,' \
                                      ' "errorCode": "code",' \
                                      ' "message": "message"}'
         mock_get.return_value.status_code = 429
 
         mock_get.return_value.headers = {}
-        with self.assertRaises(PriceCypherError) as context:
+        with self.assertRaises(HttpException) as context:
             rc.get('the/url')
 
         self.assertEqual(context.exception.status_code, 429)
-        self.assertEqual(context.exception.error_code, 'code')
+        self.assertEqual(context.exception.code, 'code')
         self.assertEqual(context.exception.message, 'message')
         self.assertIsInstance(context.exception, RateLimitError)
         self.assertEqual(context.exception.reset_at, -1)
 
         self.assertEqual(rc._metrics['retries'], 1)
 
     @mock.patch('requests.get')
@@ -207,19 +207,19 @@
         mock_get.return_value.status_code = 429
         mock_get.return_value.headers = {
             'x-ratelimit-limit': '3',
             'x-ratelimit-remaining': '6',
             'x-ratelimit-reset': '9',
         }
 
-        with self.assertRaises(PriceCypherError) as context:
+        with self.assertRaises(HttpException) as context:
             rc.get('the/url')
 
         self.assertEqual(context.exception.status_code, 429)
-        self.assertEqual(context.exception.error_code, 'code')
+        self.assertEqual(context.exception.code, 'code')
         self.assertEqual(context.exception.message, 'message')
         self.assertIsInstance(context.exception, RateLimitError)
         self.assertEqual(context.exception.reset_at, 9)
 
         self.assertEqual(rc._metrics['retries'], 5)
         self.assertEqual(rc._metrics['retries'], len(rc._metrics['backoff']))
 
@@ -235,19 +235,19 @@
         mock_get.return_value.status_code = 429
         mock_get.return_value.headers = {
             'x-ratelimit-limit': '3',
             'x-ratelimit-remaining': '6',
             'x-ratelimit-reset': '9',
         }
 
-        with self.assertRaises(PriceCypherError) as context:
+        with self.assertRaises(HttpException) as context:
             rc.get('the/url')
 
         self.assertEqual(context.exception.status_code, 429)
-        self.assertEqual(context.exception.error_code, 'code')
+        self.assertEqual(context.exception.code, 'code')
         self.assertEqual(context.exception.message, 'message')
         self.assertIsInstance(context.exception, RateLimitError)
         self.assertEqual(context.exception.reset_at, 9)
 
         self.assertEqual(rc._metrics['retries'], 0)
 
     @mock.patch('requests.get')
@@ -262,19 +262,19 @@
         mock_get.return_value.status_code = 429
         mock_get.return_value.headers = {
             'x-ratelimit-limit': '3',
             'x-ratelimit-remaining': '6',
             'x-ratelimit-reset': '9',
         }
 
-        with self.assertRaises(PriceCypherError) as context:
+        with self.assertRaises(HttpException) as context:
             rc.get('the/url')
 
         self.assertEqual(context.exception.status_code, 429)
-        self.assertEqual(context.exception.error_code, 'code')
+        self.assertEqual(context.exception.code, 'code')
         self.assertEqual(context.exception.message, 'message')
         self.assertIsInstance(context.exception, RateLimitError)
         self.assertEqual(context.exception.reset_at, 9)
 
         self.assertEqual(rc._metrics['retries'], 10)
         self.assertEqual(rc._metrics['retries'], len(rc._metrics['backoff']))
 
@@ -346,235 +346,237 @@
         mock_post.return_value.text = '{"a": "b"}'
 
         data = {'some': 'data'}
         j_data = '{"some": "data"}'
 
         mock_post.return_value.status_code = 200
         response = rc.post('the/url', data=data)
-        mock_post.assert_called_with('the/url', data=j_data, headers=headers, timeout=self.TIMEOUT_DEF)
+        mock_post.assert_called_with('the/url', data=j_data, headers=headers, timeout=self.TIMEOUT_DEF, verify=True)
 
         self.assertEqual(response, {'a': 'b'})
 
     @mock.patch('requests.post')
     def test_post_errors(self, mock_post):
         rc = RestClient(jwt='a-token')
 
         mock_post.return_value.text = '{"statusCode": 999,' \
                                       ' "errorCode": "code",' \
                                       ' "message": "message"}'
         mock_post.return_value.status_code = 999
 
-        with self.assertRaises(PriceCypherError) as context:
+        with self.assertRaises(HttpException) as context:
             rc.post('the-url')
 
         self.assertEqual(context.exception.status_code, 999)
-        self.assertEqual(context.exception.error_code, 'code')
+        self.assertEqual(context.exception.code, 'code')
         self.assertEqual(context.exception.message, 'message')
 
     @mock.patch('requests.post')
     def test_post_errors_with_no_message_property(self, mock_post):
         rc = RestClient(jwt='a-token')
 
         mock_post.return_value.text = json.dumps({
             "statusCode": 999,
             "errorCode": "code",
             "error": "error"
         })
         mock_post.return_value.status_code = 999
 
-        with self.assertRaises(PriceCypherError) as context:
+        with self.assertRaises(HttpException) as context:
             rc.post('the-url')
 
         self.assertEqual(context.exception.status_code, 999)
-        self.assertEqual(context.exception.error_code, 'code')
+        self.assertEqual(context.exception.code, 'code')
         self.assertEqual(context.exception.message, 'error')
 
     @mock.patch('requests.post')
     def test_post_errors_with_no_message_or_error_property(self, mock_post):
         rc = RestClient(jwt='a-token')
 
         mock_post.return_value.text = json.dumps({
             "statusCode": 999,
             "errorCode": "code"
         })
         mock_post.return_value.status_code = 999
 
-        with self.assertRaises(PriceCypherError) as context:
+        with self.assertRaises(HttpException) as context:
             rc.post('the-url')
 
         self.assertEqual(context.exception.status_code, 999)
-        self.assertEqual(context.exception.error_code, 'code')
+        self.assertEqual(context.exception.code, 'code')
         self.assertEqual(context.exception.message, '')
 
     @mock.patch('requests.post')
     def test_post_errors_with_message_and_error_property(self, mock_post):
         rc = RestClient(jwt='a-token')
 
         mock_post.return_value.text = json.dumps({
             "statusCode": 999,
             "errorCode": "code",
             "error": "error",
             "message": "message"
         })
         mock_post.return_value.status_code = 999
 
-        with self.assertRaises(PriceCypherError) as context:
+        with self.assertRaises(HttpException) as context:
             rc.post('the-url')
 
         self.assertEqual(context.exception.status_code, 999)
-        self.assertEqual(context.exception.error_code, 'code')
+        self.assertEqual(context.exception.code, 'code')
         self.assertEqual(context.exception.message, 'message')
 
     @mock.patch('requests.post')
     def test_post_error_with_code_property(self, mock_post):
         rc = RestClient(jwt='a-token')
 
         for error_status in [400, 500, None]:
             mock_post.return_value.status_code = error_status
             mock_post.return_value.text = '{"errorCode": "e0",' \
                                           '"message": "desc"}'
 
-            with self.assertRaises(PriceCypherError) as context:
+            with self.assertRaises(HttpException) as context:
                 rc.post('the-url')
 
             self.assertEqual(context.exception.status_code, error_status)
-            self.assertEqual(context.exception.error_code, 'e0')
+            self.assertEqual(context.exception.code, 'e0')
             self.assertEqual(context.exception.message, 'desc')
 
     @mock.patch('requests.post')
     def test_post_error_with_no_error_code(self, mock_post):
         rc = RestClient(jwt='a-token')
 
         for error_status in [400, 500, None]:
             mock_post.return_value.status_code = error_status
             mock_post.return_value.text = '{"message": "desc"}'
 
-            with self.assertRaises(PriceCypherError) as context:
+            with self.assertRaises(HttpException) as context:
                 rc.post('the-url')
 
             self.assertEqual(context.exception.status_code, error_status)
-            self.assertEqual(context.exception.error_code, 'pricecypher.sdk.internal.unknown')
+            self.assertEqual(context.exception.code, 'pricecypher.sdk.internal.unknown')
             self.assertEqual(context.exception.message, 'desc')
 
     @mock.patch('requests.post')
     def test_post_error_with_text_response(self, mock_post):
         rc = RestClient(jwt='a-token')
 
         for error_status in [400, 500, None]:
             mock_post.return_value.status_code = error_status
             mock_post.return_value.text = 'there has been a terrible error'
 
-            with self.assertRaises(PriceCypherError) as context:
+            with self.assertRaises(HttpException) as context:
                 rc.post('the-url')
 
             self.assertEqual(context.exception.status_code, error_status)
-            self.assertEqual(context.exception.error_code, 'pricecypher.sdk.internal.unknown')
+            self.assertEqual(context.exception.code, 'pricecypher.sdk.internal.unknown')
             self.assertEqual(context.exception.message, 'there has been a terrible error')
 
     @mock.patch('requests.post')
     def test_post_error_with_no_response_text(self, mock_post):
         rc = RestClient(jwt='a-token')
 
         for error_status in [400, 500, None]:
             mock_post.return_value.status_code = error_status
             mock_post.return_value.text = None
 
-            with self.assertRaises(PriceCypherError) as context:
+            with self.assertRaises(HttpException) as context:
                 rc.post('the-url')
 
             self.assertEqual(context.exception.status_code, error_status)
-            self.assertEqual(context.exception.error_code, 'pricecypher.sdk.internal.unknown')
+            self.assertEqual(context.exception.code, 'pricecypher.sdk.internal.unknown')
             self.assertEqual(context.exception.message, '')
 
     @mock.patch('requests.post')
     def test_file_post_content_type_is_none(self, mock_post):
         rc = RestClient(jwt='a-token')
         headers = {'Authorization': 'Bearer a-token', 'Accept': 'application/json'}
         mock_post.return_value.status_code = 200
         mock_post.return_value.text = 'Success'
 
         data = {'some': 'data'}
         files = [mock.Mock()]
 
         rc.file_post('the-url', data=data, files=files)
 
-        mock_post.assert_called_once_with('the-url', data=data, files=files, headers=headers, timeout=self.TIMEOUT_DEF)
+        mock_post.assert_called_once_with('the-url', data=data, files=files, headers=headers, timeout=self.TIMEOUT_DEF,
+                                          verify=True)
 
     @mock.patch('requests.put')
     def test_put(self, mock_put):
         rc = RestClient(jwt='a-token')
         headers = self.static_response_headers | {'Authorization': 'Bearer a-token'}
 
         mock_put.return_value.text = '["a", "b"]'
         mock_put.return_value.status_code = 200
 
         data = {'some': 'data'}
 
         response = rc.put(url='the-url', data=data)
-        mock_put.assert_called_with('the-url', json=data, headers=headers, timeout=self.TIMEOUT_DEF)
+        mock_put.assert_called_with('the-url', json=data, headers=headers, timeout=self.TIMEOUT_DEF, verify=True)
 
         self.assertEqual(response, ['a', 'b'])
 
     @mock.patch('requests.put')
     def test_put_errors(self, mock_put):
         rc = RestClient(jwt='a-token')
 
         mock_put.return_value.text = '{"statusCode": 999,' \
                                      ' "errorCode": "code",' \
                                      ' "message": "message"}'
         mock_put.return_value.status_code = 999
 
-        with self.assertRaises(PriceCypherError) as context:
+        with self.assertRaises(HttpException) as context:
             rc.put(url='the/url')
 
         self.assertEqual(context.exception.status_code, 999)
-        self.assertEqual(context.exception.error_code, 'code')
+        self.assertEqual(context.exception.code, 'code')
         self.assertEqual(context.exception.message, 'message')
 
     @mock.patch('requests.patch')
     def test_patch(self, mock_patch):
         rc = RestClient(jwt='a-token')
         headers = self.static_response_headers | {'Authorization': 'Bearer a-token'}
 
         mock_patch.return_value.text = '["a", "b"]'
         mock_patch.return_value.status_code = 200
 
         data = {'some': 'data'}
 
         response = rc.patch(url='the-url', data=data)
-        mock_patch.assert_called_with('the-url', json=data, headers=headers, timeout=self.TIMEOUT_DEF)
+        mock_patch.assert_called_with('the-url', json=data, headers=headers, timeout=self.TIMEOUT_DEF, verify=True)
 
         self.assertEqual(response, ['a', 'b'])
 
     @mock.patch('requests.patch')
     def test_patch_errors(self, mock_patch):
         rc = RestClient(jwt='a-token')
 
         mock_patch.return_value.text = '{"statusCode": 999,' \
                                        ' "errorCode": "code",' \
                                        ' "message": "message"}'
         mock_patch.return_value.status_code = 999
 
-        with self.assertRaises(PriceCypherError) as context:
+        with self.assertRaises(HttpException) as context:
             rc.patch(url='the/url')
 
         self.assertEqual(context.exception.status_code, 999)
-        self.assertEqual(context.exception.error_code, 'code')
+        self.assertEqual(context.exception.code, 'code')
         self.assertEqual(context.exception.message, 'message')
 
     @mock.patch('requests.delete')
     def test_delete(self, mock_delete):
         rc = RestClient(jwt='a-token')
         headers = self.static_response_headers | {'Authorization': 'Bearer a-token'}
 
         mock_delete.return_value.text = '["a", "b"]'
         mock_delete.return_value.status_code = 200
 
         response = rc.delete(url='the-url/ID')
-        mock_delete.assert_called_with('the-url/ID', headers=headers, params={}, json=None, timeout=self.TIMEOUT_DEF)
+        mock_delete.assert_called_with('the-url/ID', headers=headers, params={}, json=None, timeout=self.TIMEOUT_DEF,
+                                       verify=True)
 
         self.assertEqual(response, ['a', 'b'])
 
     @mock.patch('requests.delete')
     def test_delete_with_body_and_params(self, mock_del):
         rc = RestClient(jwt='a-token')
         headers = self.static_response_headers | {'Authorization': 'Bearer a-token'}
@@ -582,32 +584,33 @@
         mock_del.return_value.text = '["a", "b"]'
         mock_del.return_value.status_code = 200
 
         data = {'some': 'data'}
         params = {'A': 'param', 'B': 'param'}
 
         response = rc.delete(url='the-url/ID', params=params, data=data)
-        mock_del.assert_called_with('the-url/ID', headers=headers, params=params, json=data, timeout=self.TIMEOUT_DEF)
+        mock_del.assert_called_with('the-url/ID', headers=headers, params=params, json=data, timeout=self.TIMEOUT_DEF,
+                                    verify=True)
 
         self.assertEqual(response, ['a', 'b'])
 
     @mock.patch('requests.delete')
     def test_delete_errors(self, mock_delete):
         rc = RestClient(jwt='a-token')
 
         mock_delete.return_value.text = '{"statusCode": 999,' \
                                         ' "errorCode": "code",' \
                                         ' "message": "message"}'
         mock_delete.return_value.status_code = 999
 
-        with self.assertRaises(PriceCypherError) as context:
+        with self.assertRaises(HttpException) as context:
             rc.delete(url='the-url')
 
         self.assertEqual(context.exception.status_code, 999)
-        self.assertEqual(context.exception.error_code, 'code')
+        self.assertEqual(context.exception.code, 'code')
         self.assertEqual(context.exception.message, 'message')
 
     def test_disabled_telemetry(self):
         rc = RestClient(jwt='a-token')
         expected_headers = self.static_response_headers | {'Authorization': 'Bearer a-token'}
 
         self.assertEqual(rc.base_headers, expected_headers)
```

