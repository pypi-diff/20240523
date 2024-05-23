# Comparing `tmp/pysmarthashtag-0.3.5.tar.gz` & `tmp/pysmarthashtag-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmarthashtag-0.3.5.tar", last modified: Thu May  2 17:37:01 2024, max compression
+gzip compressed data, was "pysmarthashtag-0.3.6.tar", last modified: Thu May 23 18:41:11 2024, max compression
```

## Comparing `pysmarthashtag-0.3.5.tar` & `pysmarthashtag-0.3.6.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:37:01.220019 pysmarthashtag-0.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:37:01.212020 pysmarthashtag-0.3.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:37:01.212020 pysmarthashtag-0.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:37:01.212020 pysmarthashtag-0.3.5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-02 17:37:01.000000 pysmarthashtag-0.3.5/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-02 17:37:01.000000 pysmarthashtag-0.3.5/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-02 17:37:01.220019 pysmarthashtag-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:37:01.220019 pysmarthashtag-0.3.5/pySmartHashtag.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-02 17:37:01.000000 pysmarthashtag-0.3.5/pySmartHashtag.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-02 17:37:01.000000 pysmarthashtag-0.3.5/pySmartHashtag.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:37:01.000000 pysmarthashtag-0.3.5/pySmartHashtag.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:37:01.000000 pysmarthashtag-0.3.5/pySmartHashtag.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 17:37:01.000000 pysmarthashtag-0.3.5/pySmartHashtag.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 17:37:01.000000 pysmarthashtag-0.3.5/pySmartHashtag.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:37:01.216019 pysmarthashtag-0.3.5/pysmarthashtag/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/account.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:37:01.216019 pysmarthashtag-0.3.5/pysmarthashtag/api/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16136 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/api/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/api/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5613 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:37:01.216019 pysmarthashtag-0.3.5/pysmarthashtag/control/
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/control/climate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:37:01.216019 pysmarthashtag-0.3.5/pysmarthashtag/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:37:01.216019 pysmarthashtag-0.3.5/pysmarthashtag/tests/replys/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/tests/replys/Human_and_vehicle_relationship_does_not_exist.json
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/tests/replys/api_access.json
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/tests/replys/auth_context.url
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/tests/replys/auth_intermediate.url
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/tests/replys/auth_result.url
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/tests/replys/climate_success.json
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/tests/replys/login_result.json
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/tests/replys/token_expired.json
--rw-r--r--   0 runner    (1001) docker     (127)     8156 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/tests/replys/vehicle_info.json
--rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/tests/replys/vehicle_info2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/tests/replys/vehicle_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/tests/replys/vehicle_result.json
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/tests/test_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/tests/test_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:37:01.220019 pysmarthashtag-0.3.5/pysmarthashtag/vehicle/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/vehicle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/vehicle/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/vehicle/climate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/vehicle/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/vehicle/position.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/vehicle/running.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/vehicle/safety.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/vehicle/tires.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/pysmarthashtag/vehicle/vehicle.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/requirements-cli.txt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       36 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/run.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-02 17:37:01.220019 pysmarthashtag-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-02 17:36:53.000000 pysmarthashtag-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:41:11.556908 pysmarthashtag-0.3.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:41:11.548908 pysmarthashtag-0.3.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:41:11.548908 pysmarthashtag-0.3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:41:11.548908 pysmarthashtag-0.3.6/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 18:41:11.000000 pysmarthashtag-0.3.6/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-23 18:41:11.000000 pysmarthashtag-0.3.6/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-23 18:41:11.556908 pysmarthashtag-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:41:11.556908 pysmarthashtag-0.3.6/pySmartHashtag.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-23 18:41:11.000000 pysmarthashtag-0.3.6/pySmartHashtag.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-23 18:41:11.000000 pysmarthashtag-0.3.6/pySmartHashtag.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:41:11.000000 pysmarthashtag-0.3.6/pySmartHashtag.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:41:11.000000 pysmarthashtag-0.3.6/pySmartHashtag.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-23 18:41:11.000000 pysmarthashtag-0.3.6/pySmartHashtag.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 18:41:11.000000 pysmarthashtag-0.3.6/pySmartHashtag.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:41:11.548908 pysmarthashtag-0.3.6/pysmarthashtag/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/account.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:41:11.552908 pysmarthashtag-0.3.6/pysmarthashtag/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16136 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/api/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/api/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5613 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:41:11.552908 pysmarthashtag-0.3.6/pysmarthashtag/control/
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/control/climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:41:11.552908 pysmarthashtag-0.3.6/pysmarthashtag/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:41:11.552908 pysmarthashtag-0.3.6/pysmarthashtag/tests/replys/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/tests/replys/Human_and_vehicle_relationship_does_not_exist.json
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/tests/replys/api_access.json
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/tests/replys/auth_context.url
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/tests/replys/auth_intermediate.url
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/tests/replys/auth_result.url
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/tests/replys/climate_success.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/tests/replys/login_result.json
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/tests/replys/token_expired.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8156 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/tests/replys/vehicle_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/tests/replys/vehicle_info2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/tests/replys/vehicle_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/tests/replys/vehicle_result.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/tests/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/tests/test_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:41:11.556908 pysmarthashtag-0.3.6/pysmarthashtag/vehicle/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/vehicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/vehicle/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/vehicle/climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/vehicle/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/vehicle/position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/vehicle/running.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/vehicle/safety.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/vehicle/tires.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/pysmarthashtag/vehicle/vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/requirements-cli.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       36 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-23 18:41:11.556908 pysmarthashtag-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-23 18:40:58.000000 pysmarthashtag-0.3.6/setup.py
```

### Comparing `pysmarthashtag-0.3.5/.github/dependabot.yml` & `pysmarthashtag-0.3.6/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/.github/workflows/python-package.yml` & `pysmarthashtag-0.3.6/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/.github/workflows/python-publish.yml` & `pysmarthashtag-0.3.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/.pre-commit-config.yaml` & `pysmarthashtag-0.3.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/.vscode/launch.json` & `pysmarthashtag-0.3.6/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/CODE_OF_CONDUCT.md` & `pysmarthashtag-0.3.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/CONTRIBUTING.md` & `pysmarthashtag-0.3.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/LICENSE` & `pysmarthashtag-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pySmartHashtag.egg-info/SOURCES.txt` & `pysmarthashtag-0.3.6/pySmartHashtag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pyproject.toml` & `pysmarthashtag-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pySmartHashtag"
-version = "0.3.5"
+version = "0.3.6"
 authors = [
     {"name" = "Bastian Neumann", "email" = "neumann.bastian@gmail.com"},
 ]
 description = "A python library to get information from Smart #1 and #3 web API"
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/account.py` & `pysmarthashtag-0.3.6/pysmarthashtag/account.py`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/api/authentication.py` & `pysmarthashtag-0.3.6/pysmarthashtag/api/authentication.py`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/api/client.py` & `pysmarthashtag-0.3.6/pysmarthashtag/api/client.py`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/api/utils.py` & `pysmarthashtag-0.3.6/pysmarthashtag/api/utils.py`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/cli.py` & `pysmarthashtag-0.3.6/pysmarthashtag/cli.py`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/const.py` & `pysmarthashtag-0.3.6/pysmarthashtag/const.py`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/control/climate.py` & `pysmarthashtag-0.3.6/pysmarthashtag/control/climate.py`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/models.py` & `pysmarthashtag-0.3.6/pysmarthashtag/models.py`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/tests/common.py` & `pysmarthashtag-0.3.6/pysmarthashtag/tests/common.py`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/tests/conftest.py` & `pysmarthashtag-0.3.6/pysmarthashtag/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/tests/replys/api_access.json` & `pysmarthashtag-0.3.6/pysmarthashtag/tests/replys/api_access.json`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/tests/replys/auth_result.url` & `pysmarthashtag-0.3.6/pysmarthashtag/tests/replys/auth_result.url`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/tests/replys/login_result.json` & `pysmarthashtag-0.3.6/pysmarthashtag/tests/replys/login_result.json`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/tests/replys/vehicle_info.json` & `pysmarthashtag-0.3.6/pysmarthashtag/tests/replys/vehicle_info.json`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/tests/replys/vehicle_info2.json` & `pysmarthashtag-0.3.6/pysmarthashtag/tests/replys/vehicle_info2.json`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/tests/replys/vehicle_response.json` & `pysmarthashtag-0.3.6/pysmarthashtag/tests/replys/vehicle_response.json`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/tests/replys/vehicle_result.json` & `pysmarthashtag-0.3.6/pysmarthashtag/tests/replys/vehicle_result.json`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/tests/test_account.py` & `pysmarthashtag-0.3.6/pysmarthashtag/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/tests/test_actions.py` & `pysmarthashtag-0.3.6/pysmarthashtag/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/vehicle/battery.py` & `pysmarthashtag-0.3.6/pysmarthashtag/vehicle/battery.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,17 @@
     "FINISHED_FULLY_CHARGED",
     "FINISHED_NOT_FULL",
     "INVALID",
     "PLUGGED_IN",
     "WAITING_FOR_CHARGING",
     "TARGET_REACHED",
     "UNKNOWN",
+    "UNKNOWN",
+    "UNKNOWN",
+    "DC_CHARGING",
 ]
 
 
 @dataclass
 class Battery(VehicleDataBase):
     """Provides an accessible version of the vehicle's battery data."""
 
@@ -84,15 +87,16 @@
         try:
             evStatus = vehicle_data["vehicleStatus"]["additionalVehicleStatus"]["electricVehicleStatus"]
             retval["remaining_range"] = ValueWithUnit(int(evStatus["distanceToEmptyOnBatteryOnly"]), "km")
             retval["remaining_range_at_full_charge"] = ValueWithUnit(
                 int(evStatus["distanceToEmptyOnBattery100Soc"]), "km"
             )
             retval["remaining_battery_percent"] = ValueWithUnit(int(evStatus["chargeLevel"]), "%")
-            retval["charging_status"] = ChargingState[int(evStatus["chargerState"])] or "UNKNOWN"
+            status = int(evStatus["chargerState"])
+            retval["charging_status"] = ChargingState[status] if status < len(ChargingState) else "UNKNOWN"
             retval["charging_status_raw"] = int(evStatus["chargerState"])
             retval["charger_connection_status"] = int(evStatus["statusOfChargerConnection"])
             retval["is_charger_connected"] = (
                 retval["charging_status"] == "PLUGGED_IN"
                 or retval["charging_status"] == "CHARGING"
                 or retval["charging_status"] == "COMPLETE"
             )
```

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/vehicle/climate.py` & `pysmarthashtag-0.3.6/pysmarthashtag/vehicle/climate.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,23 +127,17 @@
 
     window_passenger_status: Optional[bool] = None
     """The state of the passenger's window."""
 
     window_passenger_rear_status: Optional[bool] = None
     """The state of the rear passenger's window."""
 
-    interior_PM25_level: Optional[ValueWithUnit] = ValueWithUnit(None, None)
+    interior_PM25: Optional[ValueWithUnit] = ValueWithUnit(None, None)
     """The interior PM2.5 value."""
 
-    interior_PM25_2_level: Optional[ValueWithUnit] = ValueWithUnit(None, None)
-    """The second interior PM2.5 value."""
-
-    exterior_PM25_level: Optional[ValueWithUnit] = ValueWithUnit(None, None)
-    """The exterior PM2.5 value."""
-
     relative_humidity: Optional[ValueWithUnit] = ValueWithUnit(None, None)
     """The relative humidity."""
 
     @classmethod
     def from_vehicle_data(self, vehicle_data: Dict):
         """Create a new instance based on data from API."""
         parsed = self._parse_vehicle_data(vehicle_data) or {}
@@ -201,17 +195,15 @@
             retval["window_driver_status"] = int(evStatus["winStatusDriver"])
             retval["window_driver_rear_status"] = int(evStatus["winStatusDriverRear"])
             retval["window_passenger_status"] = int(evStatus["winStatusPassenger"])
             retval["window_passenger_rear_status"] = int(evStatus["winStatusPassengerRear"])
 
             evStatus = vehicle_data["vehicleStatus"]["additionalVehicleStatus"]["pollutionStatus"]
 
-            retval["interior_PM25_level"] = ValueWithUnit(float(evStatus["interiorPM25Level"]), "μg/m³")
-            retval["interior_PM25_2_level"] = ValueWithUnit(float(evStatus["interiorSecondPM25Level"]), "μg/m³")
-            retval["exterior_PM25_level"] = ValueWithUnit(float(evStatus["exteriorPM25Level"]), "μg/m³")
+            retval["interior_PM25"] = ValueWithUnit(float(evStatus["interiorPM25"]), "μg/m³")
             retval["relative_humidity"] = ValueWithUnit(float(evStatus["relHumSts"]), "%")
 
             retval["timestamp"] = datetime.fromtimestamp(int(vehicle_data["vehicleStatus"]["updateTime"]) / 1000)
         except KeyError as e:
             _LOGGER.warning(f"Climate info not available: {e}")
         finally:
             return retval
```

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/vehicle/maintenance.py` & `pysmarthashtag-0.3.6/pysmarthashtag/vehicle/maintenance.py`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/vehicle/position.py` & `pysmarthashtag-0.3.6/pysmarthashtag/vehicle/position.py`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/vehicle/running.py` & `pysmarthashtag-0.3.6/pysmarthashtag/vehicle/running.py`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/vehicle/safety.py` & `pysmarthashtag-0.3.6/pysmarthashtag/vehicle/safety.py`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/vehicle/tires.py` & `pysmarthashtag-0.3.6/pysmarthashtag/vehicle/tires.py`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/pysmarthashtag/vehicle/vehicle.py` & `pysmarthashtag-0.3.6/pysmarthashtag/vehicle/vehicle.py`

 * *Files identical despite different names*

### Comparing `pysmarthashtag-0.3.5/setup.cfg` & `pysmarthashtag-0.3.6/setup.cfg`

 * *Files identical despite different names*

