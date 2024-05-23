# Comparing `tmp/volkswagencarnet-5.0.0b1.tar.gz` & `tmp/volkswagencarnet-5.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volkswagencarnet-5.0.0b1.tar", last modified: Tue May 14 13:31:17 2024, max compression
+gzip compressed data, was "volkswagencarnet-5.0.0b2.tar", last modified: Thu May 23 15:08:16 2024, max compression
```

## Comparing `volkswagencarnet-5.0.0b1.tar` & `volkswagencarnet-5.0.0b2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.653037 volkswagencarnet-5.0.0b1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.641037 volkswagencarnet-5.0.0b1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.github/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.github/renovate.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.645038 volkswagencarnet-5.0.0b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.github/workflows/snyk.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.github/workflows/testrelease.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.github/workflows/validate.yml
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.github/workflows/validate_pr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    34876 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-05-14 13:31:17.653037 volkswagencarnet-5.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-14 13:31:17.653037 volkswagencarnet-5.0.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.645038 volkswagencarnet-5.0.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/credentials.py.sample
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/dummy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.645038 volkswagencarnet-5.0.0b1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/mock_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.645038 volkswagencarnet-5.0.0b1/tests/fixtures/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/dummy_cookies.pickle
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.649037 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.649037 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/arteon_2023_diesel/
--rw-r--r--   0 runner    (1001) docker     (127)    10385 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/arteon_2023_diesel/capabilities.json
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/arteon_2023_diesel/last_trip.json
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/arteon_2023_diesel/parkingposition.json
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/arteon_2023_diesel/selectivestatus_by_app.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.649037 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/egolf/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/egolf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    18541 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/egolf/capabilities.json
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/egolf/last_trip.json
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/egolf/parkingposition.json
--rw-r--r--   0 runner    (1001) docker     (127)    13737 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/egolf/selectivestatus_by_app.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.649037 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/eup_electric/
--rw-r--r--   0 runner    (1001) docker     (127)    14921 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/eup_electric/capabilities.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/eup_electric/last_trip.json
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/eup_electric/parkingposition.json
--rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/eup_electric/selectivestatus_by_app.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.649037 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/golf_gte_hybrid/
--rw-r--r--   0 runner    (1001) docker     (127)    19440 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/golf_gte_hybrid/capabilities.json
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/golf_gte_hybrid/last_trip.json
--rw-r--r--   0 runner    (1001) docker     (127)    14352 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/golf_gte_hybrid/selectivestatus_by_app.json
--rw-r--r--   0 runner    (1001) docker     (127)    20847 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/status.json
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/timer.json
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/timer_without_settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/integration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/vw_connection_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/vw_utilities_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/tests/vw_vehicle_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.653037 volkswagencarnet-5.0.0b1/volkswagencarnet/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/volkswagencarnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-14 13:31:17.000000 volkswagencarnet-5.0.0b1/volkswagencarnet/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    45931 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/volkswagencarnet/vw_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/volkswagencarnet/vw_const.py
--rw-r--r--   0 runner    (1001) docker     (127)    49000 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/volkswagencarnet/vw_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/volkswagencarnet/vw_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)   146387 2024-05-14 13:31:01.000000 volkswagencarnet-5.0.0b1/volkswagencarnet/vw_vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:31:17.653037 volkswagencarnet-5.0.0b1/volkswagencarnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-05-14 13:31:17.000000 volkswagencarnet-5.0.0b1/volkswagencarnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-14 13:31:17.000000 volkswagencarnet-5.0.0b1/volkswagencarnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:31:17.000000 volkswagencarnet-5.0.0b1/volkswagencarnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-14 13:31:17.000000 volkswagencarnet-5.0.0b1/volkswagencarnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 13:31:17.000000 volkswagencarnet-5.0.0b1/volkswagencarnet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:08:16.092445 volkswagencarnet-5.0.0b2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:08:16.084445 volkswagencarnet-5.0.0b2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/.github/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/.github/renovate.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:08:16.084445 volkswagencarnet-5.0.0b2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/.github/workflows/snyk.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/.github/workflows/testrelease.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/.github/workflows/validate.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/.github/workflows/validate_pr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    34876 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-05-23 15:08:16.092445 volkswagencarnet-5.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-23 15:08:16.092445 volkswagencarnet-5.0.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:08:16.084445 volkswagencarnet-5.0.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/credentials.py.sample
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/dummy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:08:16.084445 volkswagencarnet-5.0.0b2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/mock_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:08:16.084445 volkswagencarnet-5.0.0b2/tests/fixtures/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/resources/dummy_cookies.pickle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:08:16.088446 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:08:16.088446 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/arteon_2023_diesel/
+-rw-r--r--   0 runner    (1001) docker     (127)    10385 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/arteon_2023_diesel/capabilities.json
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/arteon_2023_diesel/last_trip.json
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/arteon_2023_diesel/parkingposition.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/arteon_2023_diesel/selectivestatus_by_app.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:08:16.088446 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/egolf/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/egolf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18541 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/egolf/capabilities.json
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/egolf/last_trip.json
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/egolf/parkingposition.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13737 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/egolf/selectivestatus_by_app.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:08:16.088446 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/eup_electric/
+-rw-r--r--   0 runner    (1001) docker     (127)    14921 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/eup_electric/capabilities.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/eup_electric/last_trip.json
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/eup_electric/parkingposition.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/eup_electric/selectivestatus_by_app.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:08:16.088446 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/golf_gte_hybrid/
+-rw-r--r--   0 runner    (1001) docker     (127)    19440 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/golf_gte_hybrid/capabilities.json
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/golf_gte_hybrid/last_trip.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14352 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/golf_gte_hybrid/selectivestatus_by_app.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20847 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/status.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/timer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/timer_without_settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/vw_connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/vw_utilities_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/tests/vw_vehicle_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:08:16.088446 volkswagencarnet-5.0.0b2/volkswagencarnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/volkswagencarnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-23 15:08:16.000000 volkswagencarnet-5.0.0b2/volkswagencarnet/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45931 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/volkswagencarnet/vw_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/volkswagencarnet/vw_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49675 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/volkswagencarnet/vw_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/volkswagencarnet/vw_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)   152993 2024-05-23 15:07:59.000000 volkswagencarnet-5.0.0b2/volkswagencarnet/vw_vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:08:16.092445 volkswagencarnet-5.0.0b2/volkswagencarnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-05-23 15:08:16.000000 volkswagencarnet-5.0.0b2/volkswagencarnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-23 15:08:16.000000 volkswagencarnet-5.0.0b2/volkswagencarnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:08:16.000000 volkswagencarnet-5.0.0b2/volkswagencarnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-23 15:08:16.000000 volkswagencarnet-5.0.0b2/volkswagencarnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 15:08:16.000000 volkswagencarnet-5.0.0b2/volkswagencarnet.egg-info/top_level.txt
```

### Comparing `volkswagencarnet-5.0.0b1/.github/release-drafter.yml` & `volkswagencarnet-5.0.0b2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/.github/workflows/codeql-analysis.yml` & `volkswagencarnet-5.0.0b2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/.github/workflows/release.yaml` & `volkswagencarnet-5.0.0b2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/.github/workflows/snyk.yaml` & `volkswagencarnet-5.0.0b2/.github/workflows/snyk.yaml`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/.github/workflows/testrelease.yaml` & `volkswagencarnet-5.0.0b2/.github/workflows/testrelease.yaml`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/.github/workflows/validate.yml` & `volkswagencarnet-5.0.0b2/.github/workflows/validate.yml`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/.github/workflows/validate_pr.yaml` & `volkswagencarnet-5.0.0b2/.github/workflows/validate_pr.yaml`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/.pre-commit-config.yaml` & `volkswagencarnet-5.0.0b2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/LICENSE.txt` & `volkswagencarnet-5.0.0b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/PKG-INFO` & `volkswagencarnet-5.0.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volkswagencarnet
-Version: 5.0.0b1
+Version: 5.0.0b2
 Summary: Communicate with Volkswagen Connect
 Home-page: https://github.com/robinostlund/volkswagencarnet
 Author: Robin Ostlund
 Author-email: me@robinostlund.name
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/robinostlund/volkswagencarnet/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `volkswagencarnet-5.0.0b1/README.md` & `volkswagencarnet-5.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/setup.cfg` & `volkswagencarnet-5.0.0b2/setup.cfg`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/tests/dummy_test.py` & `volkswagencarnet-5.0.0b2/tests/dummy_test.py`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/tests/fixtures/connection.py` & `volkswagencarnet-5.0.0b2/tests/fixtures/connection.py`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/tests/fixtures/mock_server.py` & `volkswagencarnet-5.0.0b2/tests/fixtures/mock_server.py`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/README.md` & `volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/README.md`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/arteon_2023_diesel/capabilities.json` & `volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/arteon_2023_diesel/capabilities.json`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/arteon_2023_diesel/selectivestatus_by_app.json` & `volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/arteon_2023_diesel/selectivestatus_by_app.json`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/egolf/README.md` & `volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/egolf/README.md`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/egolf/capabilities.json` & `volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/egolf/capabilities.json`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/egolf/selectivestatus_by_app.json` & `volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/egolf/selectivestatus_by_app.json`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/eup_electric/capabilities.json` & `volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/eup_electric/capabilities.json`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/eup_electric/selectivestatus_by_app.json` & `volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/eup_electric/selectivestatus_by_app.json`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/golf_gte_hybrid/capabilities.json` & `volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/golf_gte_hybrid/capabilities.json`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/golf_gte_hybrid/selectivestatus_by_app.json` & `volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/golf_gte_hybrid/selectivestatus_by_app.json`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/status.json` & `volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/status.json`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/timer.json` & `volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/timer.json`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/tests/fixtures/resources/responses/timer_without_settings.json` & `volkswagencarnet-5.0.0b2/tests/fixtures/resources/responses/timer_without_settings.json`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/tests/integration_test.py` & `volkswagencarnet-5.0.0b2/tests/integration_test.py`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/tests/vw_connection_test.py` & `volkswagencarnet-5.0.0b2/tests/vw_connection_test.py`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/tests/vw_utilities_test.py` & `volkswagencarnet-5.0.0b2/tests/vw_utilities_test.py`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/tests/vw_vehicle_test.py` & `volkswagencarnet-5.0.0b2/tests/vw_vehicle_test.py`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/volkswagencarnet/vw_connection.py` & `volkswagencarnet-5.0.0b2/volkswagencarnet/vw_connection.py`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/volkswagencarnet/vw_const.py` & `volkswagencarnet-5.0.0b2/volkswagencarnet/vw_const.py`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/volkswagencarnet/vw_dashboard.py` & `volkswagencarnet-5.0.0b2/volkswagencarnet/vw_dashboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -1360,14 +1360,20 @@
         Sensor(
             attr="fuel_level",
             name="Fuel level",
             icon="mdi:fuel",
             unit="%",
         ),
         Sensor(
+            attr="gas_level",
+            name="Gas level",
+            icon="mdi:gas-cylinder",
+            unit="%",
+        ),
+        Sensor(
             attr="service_inspection",
             name="Service inspection days",
             icon="mdi:garage",
             unit="days",
         ),
         Sensor(
             attr="service_inspection_distance",
@@ -1418,14 +1424,26 @@
         Sensor(
             attr="combustion_range",
             name="Combustion range",
             icon="mdi:car",
             unit="km",
         ),
         Sensor(
+            attr="fuel_range",
+            name="Fuel range",
+            icon="mdi:car",
+            unit="km",
+        ),
+        Sensor(
+            attr="gas_range",
+            name="Gas range",
+            icon="mdi:car",
+            unit="km",
+        ),
+        Sensor(
             attr="combined_range",
             name="Combined range",
             icon="mdi:car",
             unit="km",
         ),
         Sensor(
             attr="battery_cruising_range",
@@ -1489,14 +1507,21 @@
             attr="trip_last_average_fuel_consumption",
             name="Last trip average fuel consumption",
             icon="mdi:fuel",
             unit="l/100 km",
             state_class=VWStateClass.MEASUREMENT,
         ),
         Sensor(
+            attr="trip_last_average_gas_consumption",
+            name="Last trip average gas consumption",
+            icon="mdi:gas-cylinder",
+            unit="m3/100km",
+            state_class=VWStateClass.MEASUREMENT,
+        ),
+        Sensor(
             attr="trip_last_duration",
             name="Last trip duration",
             icon="mdi:clock",
             unit="min",
             state_class=VWStateClass.MEASUREMENT,
         ),
         Sensor(
```

### Comparing `volkswagencarnet-5.0.0b1/volkswagencarnet/vw_utilities.py` & `volkswagencarnet-5.0.0b2/volkswagencarnet/vw_utilities.py`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-5.0.0b1/volkswagencarnet/vw_vehicle.py` & `volkswagencarnet-5.0.0b2/volkswagencarnet/vw_vehicle.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,22 @@
 BACKEND_RECEIVED_TIMESTAMP = "BACKEND_RECEIVED_TIMESTAMP"
 
 _LOGGER = logging.getLogger(__name__)
 
 ENGINE_TYPE_ELECTRIC = "electric"
 ENGINE_TYPE_DIESEL = "diesel"
 ENGINE_TYPE_GASOLINE = "gasoline"
+ENGINE_TYPE_CNG = "cng"
 ENGINE_TYPE_HYBRID = "hybrid"
-ENGINE_TYPE_COMBUSTION = [ENGINE_TYPE_DIESEL, ENGINE_TYPE_GASOLINE]
+ENGINE_TYPE_COMBUSTION = [
+    ENGINE_TYPE_DIESEL,
+    ENGINE_TYPE_GASOLINE,
+    ENGINE_TYPE_CNG,
+]
+ENGINE_TYPE_GAS = [ENGINE_TYPE_CNG]
 DEFAULT_TARGET_TEMP = 24
 
 
 class Vehicle:
     """Vehicle contains the state of sensors and methods for interacting with the car."""
 
     def __init__(self, conn, url) -> None:
@@ -1640,14 +1646,18 @@
     def combustion_range(self) -> int:
         """Return combustion engine range.
 
         :return:
         """
         DIESEL_RANGE = f"{Services.MEASUREMENTS}.rangeStatus.value.dieselRange"
         GASOLINE_RANGE = f"{Services.MEASUREMENTS}.rangeStatus.value.gasolineRange"
+        CNG_RANGE = f"{Services.MEASUREMENTS}.rangeStatus.value.cngRange"
+        TOTAL_RANGE = f"{Services.MEASUREMENTS}.rangeStatus.value.totalRange_km"
+        if is_valid_path(self.attrs, CNG_RANGE):
+            return find_path(self.attrs, TOTAL_RANGE)
         if is_valid_path(self.attrs, DIESEL_RANGE):
             return find_path(self.attrs, DIESEL_RANGE)
         if is_valid_path(self.attrs, GASOLINE_RANGE):
             return find_path(self.attrs, GASOLINE_RANGE)
         return -1
 
     @property
@@ -1660,21 +1670,90 @@
 
     @property
     def is_combustion_range_supported(self) -> bool:
         """Return true if combustion range is supported, i.e. false for EVs.
 
         :return:
         """
+        return (
+            is_valid_path(
+                self.attrs, f"{Services.MEASUREMENTS}.rangeStatus.value.dieselRange"
+            )
+            or is_valid_path(
+                self.attrs, f"{Services.MEASUREMENTS}.rangeStatus.value.gasolineRange"
+            )
+            or is_valid_path(
+                self.attrs, f"{Services.MEASUREMENTS}.rangeStatus.value.cngRange"
+            )
+        )
+
+    @property
+    def fuel_range(self) -> int:
+        """Return fuel engine range.
+
+        :return:
+        """
+        DIESEL_RANGE = f"{Services.MEASUREMENTS}.rangeStatus.value.dieselRange"
+        GASOLINE_RANGE = f"{Services.MEASUREMENTS}.rangeStatus.value.gasolineRange"
+        if is_valid_path(self.attrs, DIESEL_RANGE):
+            return find_path(self.attrs, DIESEL_RANGE)
+        if is_valid_path(self.attrs, GASOLINE_RANGE):
+            return find_path(self.attrs, GASOLINE_RANGE)
+        return -1
+
+    @property
+    def fuel_range_last_updated(self) -> datetime | None:
+        """Return fuel engine range last updated."""
+        return find_path(
+            self.attrs,
+            f"{Services.MEASUREMENTS}.rangeStatus.value.carCapturedTimestamp",
+        )
+
+    @property
+    def is_fuel_range_supported(self) -> bool:
+        """Return true if fuel range is supported, i.e. false for EVs.
+
+        :return:
+        """
         return is_valid_path(
             self.attrs, f"{Services.MEASUREMENTS}.rangeStatus.value.dieselRange"
         ) or is_valid_path(
             self.attrs, f"{Services.MEASUREMENTS}.rangeStatus.value.gasolineRange"
         )
 
     @property
+    def gas_range(self) -> int:
+        """Return gas engine range.
+
+        :return:
+        """
+        CNG_RANGE = f"{Services.MEASUREMENTS}.rangeStatus.value.cngRange"
+        if is_valid_path(self.attrs, CNG_RANGE):
+            return find_path(self.attrs, CNG_RANGE)
+        return -1
+
+    @property
+    def gas_range_last_updated(self) -> datetime | None:
+        """Return gas engine range last updated."""
+        return find_path(
+            self.attrs,
+            f"{Services.MEASUREMENTS}.rangeStatus.value.carCapturedTimestamp",
+        )
+
+    @property
+    def is_gas_range_supported(self) -> bool:
+        """Return true if gas range is supported, i.e. false for EVs.
+
+        :return:
+        """
+        return is_valid_path(
+            self.attrs, f"{Services.MEASUREMENTS}.rangeStatus.value.cngRange"
+        )
+
+    @property
     def combined_range(self) -> int:
         """Return combined range.
 
         :return:
         """
         return find_path(
             self.attrs, f"{Services.MEASUREMENTS}.rangeStatus.value.totalRange_km"
@@ -1734,17 +1813,20 @@
     @property
     def fuel_level(self) -> int:
         """Return fuel level.
 
         :return:
         """
         fuel_level_pct = ""
-        if is_valid_path(
-            self.attrs,
-            f"{Services.FUEL_STATUS}.rangeStatus.value.primaryEngine.currentFuelLevel_pct",
+        if (
+            is_valid_path(
+                self.attrs,
+                f"{Services.FUEL_STATUS}.rangeStatus.value.primaryEngine.currentFuelLevel_pct",
+            )
+            and not self.is_primary_drive_gas()
         ):
             fuel_level_pct = find_path(
                 self.attrs,
                 f"{Services.FUEL_STATUS}.rangeStatus.value.primaryEngine.currentFuelLevel_pct",
             )
 
         if is_valid_path(
@@ -1781,20 +1863,95 @@
 
     @property
     def is_fuel_level_supported(self) -> bool:
         """Return true if fuel level reporting is supported.
 
         :return:
         """
-        return is_valid_path(
+        return (
+            is_valid_path(
+                self.attrs,
+                f"{Services.FUEL_STATUS}.rangeStatus.value.primaryEngine.currentFuelLevel_pct",
+            )
+            and not self.is_primary_drive_gas()
+        ) or is_valid_path(
             self.attrs,
             f"{Services.MEASUREMENTS}.fuelLevelStatus.value.currentFuelLevel_pct",
+        )
+
+    @property
+    def gas_level(self) -> int:
+        """Return gas level.
+
+        :return:
+        """
+        gas_level_pct = ""
+        if (
+            is_valid_path(
+                self.attrs,
+                f"{Services.FUEL_STATUS}.rangeStatus.value.primaryEngine.currentFuelLevel_pct",
+            )
+            and self.is_primary_drive_gas()
+        ):
+            gas_level_pct = find_path(
+                self.attrs,
+                f"{Services.FUEL_STATUS}.rangeStatus.value.primaryEngine.currentFuelLevel_pct",
+            )
+
+        if is_valid_path(
+            self.attrs,
+            f"{Services.MEASUREMENTS}.fuelLevelStatus.value.currentCngLevel_pct",
+        ):
+            gas_level_pct = find_path(
+                self.attrs,
+                f"{Services.MEASUREMENTS}.fuelLevelStatus.value.currentCngLevel_pct",
+            )
+        return gas_level_pct
+
+    @property
+    def gas_level_last_updated(self) -> datetime:
+        """Return gas level last updated."""
+        gas_level_lastupdated = ""
+        if (
+            is_valid_path(
+                self.attrs,
+                f"{Services.FUEL_STATUS}.rangeStatus.value.carCapturedTimestamp",
+            )
+            and self.is_primary_drive_gas()
+        ):
+            gas_level_lastupdated = find_path(
+                self.attrs,
+                f"{Services.FUEL_STATUS}.rangeStatus.value.carCapturedTimestamp",
+            )
+
+        if is_valid_path(
+            self.attrs,
+            f"{Services.MEASUREMENTS}.fuelLevelStatus.value.carCapturedTimestamp",
+        ):
+            gas_level_lastupdated = find_path(
+                self.attrs,
+                f"{Services.MEASUREMENTS}.fuelLevelStatus.value.carCapturedTimestamp",
+            )
+        return gas_level_lastupdated
+
+    @property
+    def is_gas_level_supported(self) -> bool:
+        """Return true if gas level reporting is supported.
+
+        :return:
+        """
+        return (
+            is_valid_path(
+                self.attrs,
+                f"{Services.FUEL_STATUS}.rangeStatus.value.primaryEngine.currentFuelLevel_pct",
+            )
+            and self.is_primary_drive_gas()
         ) or is_valid_path(
             self.attrs,
-            f"{Services.FUEL_STATUS}.rangeStatus.value.primaryEngine.currentFuelLevel_pct",
+            f"{Services.MEASUREMENTS}.fuelLevelStatus.value.currentCngLevel_pct",
         )
 
     @property
     def car_type(self) -> str:
         """Return car type.
 
         :return:
@@ -3307,14 +3464,41 @@
         return is_valid_path(
             self.attrs, f"{Services.TRIP_LAST}.averageFuelConsumption"
         ) and type(
             find_path(self.attrs, f"{Services.TRIP_LAST}.averageFuelConsumption")
         ) in (float, int)
 
     @property
+    def trip_last_average_gas_consumption(self):
+        """Return last trip average gas consumption.
+
+        :return:
+        """
+        return float(
+            find_path(self.attrs, f"{Services.TRIP_LAST}.averageGasConsumption")
+        )
+
+    @property
+    def trip_last_average_gas_consumption_last_updated(self) -> datetime:
+        """Return last updated timestamp."""
+        return find_path(self.attrs, f"{Services.TRIP_LAST}.tripEndTimestamp")
+
+    @property
+    def is_trip_last_average_gas_consumption_supported(self) -> bool:
+        """Return true if supported.
+
+        :return:
+        """
+        return is_valid_path(
+            self.attrs, f"{Services.TRIP_LAST}.averageGasConsumption"
+        ) and type(
+            find_path(self.attrs, f"{Services.TRIP_LAST}.averageGasConsumption")
+        ) in (float, int)
+
+    @property
     def trip_last_average_auxillary_consumption(self):
         """Return last trip average auxiliary consumption.
 
         :return:
         """
         # no example verified yet
         return self.trip_last_entry.get("averageAuxiliaryConsumption")
@@ -3691,14 +3875,36 @@
             engine_type = find_path(
                 self.attrs,
                 f"{Services.MEASUREMENTS}.fuelLevelStatus.value.secondaryEngineType",
             )
 
         return engine_type in ENGINE_TYPE_COMBUSTION
 
+    def is_primary_drive_gas(self):
+        """Check if primary engine is gas."""
+        if is_valid_path(
+            self.attrs, f"{Services.FUEL_STATUS}.rangeStatus.value.carType"
+        ):
+            return (
+                find_path(
+                    self.attrs, f"{Services.FUEL_STATUS}.rangeStatus.value.carType"
+                )
+                == ENGINE_TYPE_GAS
+            )
+        if is_valid_path(
+            self.attrs, f"{Services.MEASUREMENTS}.fuelLevelStatus.value.carType"
+        ):
+            return (
+                find_path(
+                    self.attrs, f"{Services.MEASUREMENTS}.fuelLevelStatus.value.carType"
+                )
+                == ENGINE_TYPE_GAS
+            )
+        return False
+
     @property
     def is_car_type_electric(self):
         """Check if car type is electric."""
         if is_valid_path(
             self.attrs, f"{Services.FUEL_STATUS}.rangeStatus.value.carType"
         ):
             return (
```

### Comparing `volkswagencarnet-5.0.0b1/volkswagencarnet.egg-info/PKG-INFO` & `volkswagencarnet-5.0.0b2/volkswagencarnet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volkswagencarnet
-Version: 5.0.0b1
+Version: 5.0.0b2
 Summary: Communicate with Volkswagen Connect
 Home-page: https://github.com/robinostlund/volkswagencarnet
 Author: Robin Ostlund
 Author-email: me@robinostlund.name
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/robinostlund/volkswagencarnet/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `volkswagencarnet-5.0.0b1/volkswagencarnet.egg-info/SOURCES.txt` & `volkswagencarnet-5.0.0b2/volkswagencarnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

