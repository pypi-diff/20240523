# Comparing `tmp/djangorestframework-simple-apikey-1.0.2.tar.gz` & `tmp/djangorestframework_simple_apikey-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangorestframework-simple-apikey-1.0.2.tar", last modified: Sat Sep 16 20:09:24 2023, max compression
+gzip compressed data, was "djangorestframework_simple_apikey-1.1.1.tar", last modified: Thu May 23 02:14:52 2024, max compression
```

## Comparing `djangorestframework-simple-apikey-1.0.2.tar` & `djangorestframework_simple_apikey-1.1.1.tar`

### file list

```diff
@@ -1,53 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 20:09:24.937704 djangorestframework-simple-apikey-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2023-09-16 20:09:24.937704 djangorestframework-simple-apikey-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 20:09:24.933704 djangorestframework-simple-apikey-1.0.2/djangorestframework_simple_apikey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2023-09-16 20:09:24.000000 djangorestframework-simple-apikey-1.0.2/djangorestframework_simple_apikey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2023-09-16 20:09:24.000000 djangorestframework-simple-apikey-1.0.2/djangorestframework_simple_apikey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-16 20:09:24.000000 djangorestframework-simple-apikey-1.0.2/djangorestframework_simple_apikey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-16 20:09:24.000000 djangorestframework-simple-apikey-1.0.2/djangorestframework_simple_apikey.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-09-16 20:09:24.000000 djangorestframework-simple-apikey-1.0.2/djangorestframework_simple_apikey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-09-16 20:09:24.000000 djangorestframework-simple-apikey-1.0.2/djangorestframework_simple_apikey.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 20:09:24.933704 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 20:09:24.933704 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 20:09:24.933704 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/management/commands/generate_fernet_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/management/commands/rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 20:09:24.933704 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/migrations/0002_alter_apikey_options.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/mutli_api_crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 20:09:24.933704 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/rotation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/rotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/rotation/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/rotation/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 20:09:24.933704 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/rotation/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/rotation/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/rotation/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/rotation/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/rotation/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2023-09-16 20:09:24.937704 djangorestframework-simple-apikey-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 20:09:24.933704 djangorestframework-simple-apikey-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/tests/test_api_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/tests/test_api_key_crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/tests/test_api_key_multi_crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/tests/test_custom_django_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-09-16 20:09:15.000000 djangorestframework-simple-apikey-1.0.2/tests/test_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:14:52.961760 djangorestframework_simple_apikey-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-05-23 02:14:52.961760 djangorestframework_simple_apikey-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:14:52.957760 djangorestframework_simple_apikey-1.1.1/djangorestframework_simple_apikey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-05-23 02:14:52.000000 djangorestframework_simple_apikey-1.1.1/djangorestframework_simple_apikey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-23 02:14:52.000000 djangorestframework_simple_apikey-1.1.1/djangorestframework_simple_apikey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 02:14:52.000000 djangorestframework_simple_apikey-1.1.1/djangorestframework_simple_apikey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 02:14:52.000000 djangorestframework_simple_apikey-1.1.1/djangorestframework_simple_apikey.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-23 02:14:52.000000 djangorestframework_simple_apikey-1.1.1/djangorestframework_simple_apikey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-23 02:14:52.000000 djangorestframework_simple_apikey-1.1.1/djangorestframework_simple_apikey.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:14:52.953760 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:14:52.953760 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/analytics/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/analytics/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/analytics/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:14:52.953760 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/analytics/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/analytics/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/analytics/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/analytics/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:14:52.957760 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:14:52.957760 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/management/commands/generate_fernet_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/management/commands/rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:14:52.957760 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/migrations/0002_alter_apikey_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/mutli_api_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:14:52.957760 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/rotation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/rotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/rotation/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/rotation/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:14:52.957760 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/rotation/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/rotation/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/rotation/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/rotation/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/rotation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-23 02:14:52.961760 djangorestframework_simple_apikey-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:14:52.957760 djangorestframework_simple_apikey-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/tests/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/tests/test_analytics_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/tests/test_api_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/tests/test_api_key_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/tests/test_api_key_multi_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/tests/test_custom_django_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-23 02:14:49.000000 djangorestframework_simple_apikey-1.1.1/tests/test_permissions.py
```

### Comparing `djangorestframework-simple-apikey-1.0.2/LICENSE` & `djangorestframework_simple_apikey-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `djangorestframework-simple-apikey-1.0.2/PKG-INFO` & `djangorestframework_simple_apikey-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestframework-simple-apikey
-Version: 1.0.2
+Version: 1.1.1
 Summary: API Key authentication and permissions for Django REST.
 Home-page: https://github.com/koladev32/djangorestframework-simple-apikey
 Author: Kolawole Mangabo
 Author-email: onaelmangabo@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -38,15 +38,24 @@
       <img src="https://badge.fury.io/py/djangorestframework-simple-apikey.svg" alt="Version"/>
   </a>
   <a href="https://github.com/koladev32/djangorestframework-simple-apikey/actions/workflows/ci-cd.yml">
       <img src="https://github.com/koladev32/djangorestframework-simple-apikey/actions/workflows/ci-cd.yml/badge.svg" alt="Testing"/>
   </a>
 </div>
 
-For the full documentation, visit [https://djangorestframework-simple-apikey.readthedocs.io/en/latest/](https://djangorestframework-simple-apikey.readthedocs.io/en/latest/).
+For the full documentation, visit [https://drf-apikey.readthedocs.io/en/latest/](https://djangorestframework-simple-apikey.readthedocs.io/en/latest/).
+
+## Package Renaming Notice
+
+**Notice:** The `djangorestframework-simple-apikey` package is being renamed to `drf-apikey` to improve usability and align with common naming conventions. Please update your installations:
+
+1. Replace the old package:
+   ```bash
+   pip uninstall djangorestframework-simple-apikey
+   pip install drf-apikey
 
 ## Introduction
 
 Django REST Simple Api Key is a package built upon Django, Django REST Framework, and the fernet cryptography module to generate, encrypt, and decrypt API keys. It provides fast, secure and customizable API Key authentication.
 
 ### Benefits
```

### Comparing `djangorestframework-simple-apikey-1.0.2/README.md` & `djangorestframework_simple_apikey-1.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,24 @@
       <img src="https://badge.fury.io/py/djangorestframework-simple-apikey.svg" alt="Version"/>
   </a>
   <a href="https://github.com/koladev32/djangorestframework-simple-apikey/actions/workflows/ci-cd.yml">
       <img src="https://github.com/koladev32/djangorestframework-simple-apikey/actions/workflows/ci-cd.yml/badge.svg" alt="Testing"/>
   </a>
 </div>
 
-For the full documentation, visit [https://djangorestframework-simple-apikey.readthedocs.io/en/latest/](https://djangorestframework-simple-apikey.readthedocs.io/en/latest/).
+For the full documentation, visit [https://drf-apikey.readthedocs.io/en/latest/](https://djangorestframework-simple-apikey.readthedocs.io/en/latest/).
+
+## Package Renaming Notice
+
+**Notice:** The `djangorestframework-simple-apikey` package is being renamed to `drf-apikey` to improve usability and align with common naming conventions. Please update your installations:
+
+1. Replace the old package:
+   ```bash
+   pip uninstall djangorestframework-simple-apikey
+   pip install drf-apikey
 
 ## Introduction
 
 Django REST Simple Api Key is a package built upon Django, Django REST Framework, and the fernet cryptography module to generate, encrypt, and decrypt API keys. It provides fast, secure and customizable API Key authentication.
 
 ### Benefits
```

### Comparing `djangorestframework-simple-apikey-1.0.2/djangorestframework_simple_apikey.egg-info/PKG-INFO` & `djangorestframework_simple_apikey-1.1.1/djangorestframework_simple_apikey.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestframework-simple-apikey
-Version: 1.0.2
+Version: 1.1.1
 Summary: API Key authentication and permissions for Django REST.
 Home-page: https://github.com/koladev32/djangorestframework-simple-apikey
 Author: Kolawole Mangabo
 Author-email: onaelmangabo@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -38,15 +38,24 @@
       <img src="https://badge.fury.io/py/djangorestframework-simple-apikey.svg" alt="Version"/>
   </a>
   <a href="https://github.com/koladev32/djangorestframework-simple-apikey/actions/workflows/ci-cd.yml">
       <img src="https://github.com/koladev32/djangorestframework-simple-apikey/actions/workflows/ci-cd.yml/badge.svg" alt="Testing"/>
   </a>
 </div>
 
-For the full documentation, visit [https://djangorestframework-simple-apikey.readthedocs.io/en/latest/](https://djangorestframework-simple-apikey.readthedocs.io/en/latest/).
+For the full documentation, visit [https://drf-apikey.readthedocs.io/en/latest/](https://djangorestframework-simple-apikey.readthedocs.io/en/latest/).
+
+## Package Renaming Notice
+
+**Notice:** The `djangorestframework-simple-apikey` package is being renamed to `drf-apikey` to improve usability and align with common naming conventions. Please update your installations:
+
+1. Replace the old package:
+   ```bash
+   pip uninstall djangorestframework-simple-apikey
+   pip install drf-apikey
 
 ## Introduction
 
 Django REST Simple Api Key is a package built upon Django, Django REST Framework, and the fernet cryptography module to generate, encrypt, and decrypt API keys. It provides fast, secure and customizable API Key authentication.
 
 ### Benefits
```

### Comparing `djangorestframework-simple-apikey-1.0.2/djangorestframework_simple_apikey.egg-info/SOURCES.txt` & `djangorestframework_simple_apikey-1.1.1/djangorestframework_simple_apikey.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -15,15 +15,23 @@
 rest_framework_simple_api_key/backends.py
 rest_framework_simple_api_key/crypto.py
 rest_framework_simple_api_key/models.py
 rest_framework_simple_api_key/mutli_api_crypto.py
 rest_framework_simple_api_key/parser.py
 rest_framework_simple_api_key/permissions.py
 rest_framework_simple_api_key/settings.py
+rest_framework_simple_api_key/utils.py
 rest_framework_simple_api_key/version.py
+rest_framework_simple_api_key/analytics/__init__.py
+rest_framework_simple_api_key/analytics/admin.py
+rest_framework_simple_api_key/analytics/apps.py
+rest_framework_simple_api_key/analytics/middleware.py
+rest_framework_simple_api_key/analytics/models.py
+rest_framework_simple_api_key/analytics/migrations/0001_initial.py
+rest_framework_simple_api_key/analytics/migrations/__init__.py
 rest_framework_simple_api_key/management/__init__.py
 rest_framework_simple_api_key/management/commands/__init__.py
 rest_framework_simple_api_key/management/commands/generate_fernet_key.py
 rest_framework_simple_api_key/management/commands/rotation.py
 rest_framework_simple_api_key/migrations/0001_initial.py
 rest_framework_simple_api_key/migrations/0002_alter_apikey_options.py
 rest_framework_simple_api_key/migrations/__init__.py
@@ -31,13 +39,15 @@
 rest_framework_simple_api_key/rotation/admin.py
 rest_framework_simple_api_key/rotation/apps.py
 rest_framework_simple_api_key/rotation/models.py
 rest_framework_simple_api_key/rotation/utils.py
 rest_framework_simple_api_key/rotation/migrations/0001_initial.py
 rest_framework_simple_api_key/rotation/migrations/__init__.py
 tests/test_admin.py
+tests/test_analytics.py
+tests/test_analytics_middleware.py
 tests/test_api_authentication.py
 tests/test_api_key_crypto.py
 tests/test_api_key_multi_crypto.py
 tests/test_custom_django_command.py
 tests/test_models.py
 tests/test_permissions.py
```

### Comparing `djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/admin.py` & `djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         self,
         request: HttpRequest,
         obj: APIKey,
         form: typing.Any = None,
         change: bool = False,
     ) -> None:
         """
-        If there is obj.pk, it means that the object is been created. We need then to display the
+        If there is obj.pk, it means that the object is being created. We need then to display the
         `api_key` value in the Django admin dashboard.
         """
 
         if not obj.pk:
             obj.save()
 
             key = self.model.objects.assign_api_key(obj)
```

### Comparing `djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/backends.py` & `djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/backends.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/crypto.py` & `djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/crypto.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/management/commands/rotation.py` & `djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/management/commands/rotation.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,34 +4,40 @@
 from django.utils import timezone
 
 from rest_framework_simple_api_key.rotation.models import Rotation
 from rest_framework_simple_api_key.settings import package_settings
 
 
 class Command(BaseCommand):
-    help = 'Starts or stops a rotation based on command arguments'
+    help = "Starts or stops a rotation based on command arguments"
 
     def add_arguments(self, parser):
         parser.add_argument(
-            '--stop',
-            action='store_true',
-            help='Stops the rotation (Default is to start)',
+            "--stop",
+            action="store_true",
+            help="Stops the rotation (Default is to start)",
         )
 
     def handle(self, *args, **options):
-        if options['stop']:
+        if options["stop"]:
             # Stop the rotation logic
             try:
-                rotation = Rotation.objects.filter(is_rotation_enabled=True).latest('started')
+                rotation = Rotation.objects.filter(is_rotation_enabled=True).latest(
+                    "started"
+                )
                 rotation.is_rotation_enabled = False
                 rotation.ended = timezone.now()
                 rotation.save()
-                self.stdout.write(self.style.SUCCESS('Successfully stopped rotation'))
+                self.stdout.write(self.style.SUCCESS("Successfully stopped rotation"))
             except Rotation.DoesNotExist:
-                raise CommandError('No active rotation found to stop')
+                raise CommandError("No active rotation found to stop")
         else:
             # Start the rotation logic
             obj = Rotation()
             obj.is_rotation_enabled = True
             obj.ended = timezone.now() + package_settings.ROTATION_PERIOD
             obj.save()
-            self.stdout.write(self.style.SUCCESS(f'Successfully started rotation ending at {obj.ended}'))
+            self.stdout.write(
+                self.style.SUCCESS(
+                    f"Successfully started rotation ending at {obj.ended}"
+                )
+            )
```

### Comparing `djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/migrations/0001_initial.py` & `djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/migrations/0001_initial.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 import rest_framework_simple_api_key.models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
     ]
 
     operations = [
```

### Comparing `djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/models.py` & `djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,14 +81,17 @@
     has_expired = property(_has_expired)
 
     class Meta:
         abstract = True
         verbose_name = "API key"
         verbose_name_plural = "API keys"
 
+    def __str__(self):
+        return self.name
+
 
 class APIKey(AbstractAPIKey):
     """
     API KEY model
     """
 
     pass
```

### Comparing `djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/mutli_api_crypto.py` & `djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/mutli_api_crypto.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/parser.py` & `djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     authorization header. You can add custom parsing validation here.
     """
 
     keyword = package_settings.AUTHENTICATION_KEYWORD_HEADER
     message = "No API key provided."
 
     def get(self, request: HttpRequest) -> typing.Optional[str]:
-
         return self.get_from_authorization(request)
 
     def get_from_authorization(self, request: HttpRequest) -> typing.Optional[str]:
         authorization = request.META.get("HTTP_AUTHORIZATION")
 
         if not authorization:
             raise NotAuthenticated(self.message)
```

### Comparing `djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/permissions.py` & `djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,13 @@
     A base permission that only checks if the entity (by default, the Django user) is
     active or not.
     """
 
     message = "Entity is not active."
 
     def has_permission(self, request: HttpRequest, view: typing.Any) -> bool:
-
         return request.user.is_active
 
     def has_object_permission(
         self, request: HttpRequest, view: typing.Any, obj
     ) -> bool:
-
         return request.user.is_active
```

### Comparing `djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/rotation/admin.py` & `djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/rotation/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,29 +18,29 @@
     list_filter = (
         "is_rotation_enabled",
         "started",
         "ended",
     )
 
     def get_readonly_fields(
-            self, request: HttpRequest, obj: Rotation = None
+        self, request: HttpRequest, obj: Rotation = None
     ) -> typing.Tuple[str, ...]:
         fields = (
             "started",
             "ended",
         )
 
         return fields
 
     def save_model(
-            self,
-            request: HttpRequest,
-            obj: Rotation,
-            form: typing.Any = None,
-            change: bool = False,
+        self,
+        request: HttpRequest,
+        obj: Rotation,
+        form: typing.Any = None,
+        change: bool = False,
     ) -> None:
         """
         If there is obj.pk, it means that the object has been created already.
         """
 
         if not obj.pk:
             obj.is_rotation_enabled = True
```

### Comparing `djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/rotation/migrations/0001_initial.py` & `djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/rotation/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 4.1.6 on 2023-09-16 17:54
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="Rotation",
```

### Comparing `djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/rotation/utils.py` & `djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/rotation/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,26 @@
 
 from rest_framework_simple_api_key.settings import package_settings
 
 
 def get_rotation_status():
     rotation_status = cache.get("rotation_status")
 
-    if rotation_status is None:  # We should check for 'None' specifically because the cached value could be False
+    if (
+        rotation_status is None
+    ):  # We should check for 'None' specifically because the cached value could be False
         # Lazy load the Rotation model
-        Rotation = apps.get_model('rest_framework_simple_api_key_rotation', 'Rotation')
+        Rotation = apps.get_model("rest_framework_simple_api_key_rotation", "Rotation")
 
         # Filter the latest rotation that is enabled
-        config = Rotation.objects.filter(is_rotation_enabled=True).order_by('-started').first()
+        config = (
+            Rotation.objects.filter(is_rotation_enabled=True)
+            .order_by("-started")
+            .first()
+        )
 
         # If we have a rotation config and its 'ended' date has passed, update it
         if config and config.ended and config.ended <= timezone.now():
             config.is_rotation_enabled = False
             config.save()
             rotation_status = False
         elif config:
@@ -25,11 +31,13 @@
         else:
             rotation_status = False
 
         # Cache the rotation status
         cache.set(
             "rotation_status",
             rotation_status,
-            package_settings.ROTATION_PERIOD.total_seconds() if rotation_status else None,
+            package_settings.ROTATION_PERIOD.total_seconds()
+            if rotation_status
+            else None,
         )  # Cache for the rotation period if true
 
     return rotation_status
```

### Comparing `djangorestframework-simple-apikey-1.0.2/rest_framework_simple_api_key/settings.py` & `djangorestframework_simple_apikey-1.1.1/rest_framework_simple_api_key/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 DEFAULTS = {
     "FERNET_SECRET": "",
     "ROTATION_FERNET_SECRET": "",
     "API_KEY_LIFETIME": 365,
     "AUTHENTICATION_KEYWORD_HEADER": "Api-Key",
     "ROTATION_PERIOD": timedelta(days=7),
+    "API_KEY_CLASS": "rest_framework_simple_api_key.Apikey",
 }
 
 REMOVED_SETTINGS = ()
 
 
 class PackageSettings(_APISettings):
     @property
```

### Comparing `djangorestframework-simple-apikey-1.0.2/setup.cfg` & `djangorestframework_simple_apikey-1.1.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.0.2
+current_version = 1.1.1
 commit = True
 tag = True
 
 [bumpversion:file:pyproject.toml]
 search = version = "{current_version}"
 replace = version = "{new_version}"
```

### Comparing `djangorestframework-simple-apikey-1.0.2/tests/test_admin.py` & `djangorestframework_simple_apikey-1.1.1/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-simple-apikey-1.0.2/tests/test_api_authentication.py` & `djangorestframework_simple_apikey-1.1.1/tests/test_api_authentication.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-simple-apikey-1.0.2/tests/test_api_key_crypto.py` & `djangorestframework_simple_apikey-1.1.1/tests/test_api_key_crypto.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-simple-apikey-1.0.2/tests/test_api_key_multi_crypto.py` & `djangorestframework_simple_apikey-1.1.1/tests/test_api_key_multi_crypto.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 from rest_framework_simple_api_key.crypto import ApiCrypto
 from rest_framework_simple_api_key.mutli_api_crypto import MultiApiCrypto
 
 
 @pytest.mark.django_db
 class TestCryptoFunctions:
-
-    @pytest.fixture(scope='class')
+    @pytest.fixture(scope="class")
     def key_crypto(self):
         from rest_framework_simple_api_key.crypto import get_crypto
+
         return get_crypto()
 
     def test_encryption_and_decryption(self, key_crypto):
         payload = {"test": "data"}
         encrypted = key_crypto.encrypt(json.dumps(payload))
         decrypted = key_crypto.decrypt(encrypted)
         assert decrypted == payload
```

### Comparing `djangorestframework-simple-apikey-1.0.2/tests/test_models.py` & `djangorestframework_simple_apikey-1.1.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-simple-apikey-1.0.2/tests/test_permissions.py` & `djangorestframework_simple_apikey-1.1.1/tests/test_permissions.py`

 * *Files identical despite different names*

