# Comparing `tmp/alphaz-next-0.7.2.tar.gz` & `tmp/alphaz-next-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphaz-next-0.7.2.tar", last modified: Wed May 22 13:45:20 2024, max compression
+gzip compressed data, was "alphaz-next-0.7.3.tar", last modified: Wed May 22 14:13:16 2024, max compression
```

## Comparing `alphaz-next-0.7.2.tar` & `alphaz-next-0.7.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:20.892017 alphaz-next-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-22 13:45:20.892017 alphaz-next-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:20.884017 alphaz-next-0.7.2/alphaz_next/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:20.884017 alphaz-next-0.7.2/alphaz_next/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/asyncio/async_database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:20.884017 alphaz-next-0.7.2/alphaz_next/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:20.884017 alphaz-next-0.7.2/alphaz_next/core/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/core/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/core/_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/core/_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/core/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/core/exception_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:20.888017 alphaz-next-0.7.2/alphaz_next/core/responses/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/core/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/core/responses/file_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/core/responses/html_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/core/responses/json_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/core/responses/orjson_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/core/responses/plaintext_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/core/responses/redirect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/core/responses/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/core/responses/streaming_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/core/responses/ujson_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:20.888017 alphaz-next-0.7.2/alphaz_next/libs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/libs/file_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/libs/httpx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:20.888017 alphaz-next-0.7.2/alphaz_next/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:20.888017 alphaz-next-0.7.2/alphaz_next/models/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/models/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/models/auth/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:20.888017 alphaz-next-0.7.2/alphaz_next/models/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/models/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:20.888017 alphaz-next-0.7.2/alphaz_next/models/config/_base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/models/config/_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/models/config/_base/internal_config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/models/config/_base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/models/config/alpha_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/models/config/api_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/models/config/apm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/models/config/config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/models/config/database_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/models/config/directories_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/models/config/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/models/config/openapi_config_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:20.888017 alphaz-next-0.7.2/alphaz_next/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:20.888017 alphaz-next-0.7.2/alphaz_next/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/tests/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:20.888017 alphaz-next-0.7.2/alphaz_next/tests/utils/mocking/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/tests/utils/mocking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/tests/utils/mocking/mock_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    26256 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/tests/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:20.892017 alphaz-next-0.7.2/alphaz_next/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/utils/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/utils/logging_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/alphaz_next/utils/loguru.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:45:20.884017 alphaz-next-0.7.2/alphaz_next.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-22 13:45:20.000000 alphaz-next-0.7.2/alphaz_next.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-22 13:45:20.000000 alphaz-next-0.7.2/alphaz_next.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:45:20.000000 alphaz-next-0.7.2/alphaz_next.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-22 13:45:20.000000 alphaz-next-0.7.2/alphaz_next.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 13:45:20.000000 alphaz-next-0.7.2/alphaz_next.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-22 13:45:18.000000 alphaz-next-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:45:20.892017 alphaz-next-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-22 13:45:19.000000 alphaz-next-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.943364 alphaz-next-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-22 14:13:16.943364 alphaz-next-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.935365 alphaz-next-0.7.3/alphaz_next/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.935365 alphaz-next-0.7.3/alphaz_next/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/asyncio/async_database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.935365 alphaz-next-0.7.3/alphaz_next/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.939365 alphaz-next-0.7.3/alphaz_next/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/exception_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.939365 alphaz-next-0.7.3/alphaz_next/core/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/responses/file_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/responses/html_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/responses/json_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/responses/orjson_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/responses/plaintext_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/responses/redirect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/responses/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/responses/streaming_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/responses/ujson_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.939365 alphaz-next-0.7.3/alphaz_next/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/libs/file_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/libs/httpx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.939365 alphaz-next-0.7.3/alphaz_next/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.939365 alphaz-next-0.7.3/alphaz_next/models/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/auth/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.939365 alphaz-next-0.7.3/alphaz_next/models/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.943364 alphaz-next-0.7.3/alphaz_next/models/config/_base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/_base/internal_config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/_base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/alpha_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/api_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/apm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/database_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/directories_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/openapi_config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.943364 alphaz-next-0.7.3/alphaz_next/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.943364 alphaz-next-0.7.3/alphaz_next/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.943364 alphaz-next-0.7.3/alphaz_next/tests/utils/mocking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/tests/utils/mocking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/tests/utils/mocking/mock_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26256 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/tests/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.943364 alphaz-next-0.7.3/alphaz_next/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/utils/logging_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/utils/loguru.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.935365 alphaz-next-0.7.3/alphaz_next.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-22 14:13:16.000000 alphaz-next-0.7.3/alphaz_next.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-22 14:13:16.000000 alphaz-next-0.7.3/alphaz_next.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:13:16.000000 alphaz-next-0.7.3/alphaz_next.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-22 14:13:16.000000 alphaz-next-0.7.3/alphaz_next.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 14:13:16.000000 alphaz-next-0.7.3/alphaz_next.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 14:13:16.943364 alphaz-next-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-22 14:13:14.000000 alphaz-next-0.7.3/setup.py
```

### Comparing `alphaz-next-0.7.2/PKG-INFO` & `alphaz-next-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.7.2
+Version: 0.7.3
 Summary: A project to make a lib to start FastAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.7.2.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.7.3.tar.gz
 Author: Maxime MARTIN
 Author-email: Maxime MARTIN <maxime.martin02@hotmail.fr>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alphaz-next-0.7.2/README.md` & `alphaz-next-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/asyncio/async_database.py` & `alphaz-next-0.7.3/alphaz_next/asyncio/async_database.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/auth/auth.py` & `alphaz-next-0.7.3/alphaz_next/auth/auth.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/core/_base.py` & `alphaz-next-0.7.3/alphaz_next/core/_base.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/core/_middleware.py` & `alphaz-next-0.7.3/alphaz_next/core/_middleware.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/core/_telemetry.py` & `alphaz-next-0.7.3/alphaz_next/core/_telemetry.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/core/application.py` & `alphaz-next-0.7.3/alphaz_next/core/application.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/core/exception_handlers.py` & `alphaz-next-0.7.3/alphaz_next/core/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/core/exceptions.py` & `alphaz-next-0.7.3/alphaz_next/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/core/responses/__init__.py` & `alphaz-next-0.7.3/alphaz_next/core/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/core/responses/file_response.py` & `alphaz-next-0.7.3/alphaz_next/core/responses/file_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/core/responses/html_response.py` & `alphaz-next-0.7.3/alphaz_next/core/responses/html_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/core/responses/json_response.py` & `alphaz-next-0.7.3/alphaz_next/core/responses/json_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/core/responses/orjson_response.py` & `alphaz-next-0.7.3/alphaz_next/core/responses/orjson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/core/responses/plaintext_response.py` & `alphaz-next-0.7.3/alphaz_next/core/responses/plaintext_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/core/responses/redirect_response.py` & `alphaz-next-0.7.3/alphaz_next/core/responses/redirect_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/core/responses/response.py` & `alphaz-next-0.7.3/alphaz_next/core/responses/response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/core/responses/streaming_response.py` & `alphaz-next-0.7.3/alphaz_next/core/responses/streaming_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/core/responses/ujson_response.py` & `alphaz-next-0.7.3/alphaz_next/core/responses/ujson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/libs/httpx.py` & `alphaz-next-0.7.3/alphaz_next/libs/httpx.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/models/config/_base/internal_config_settings.py` & `alphaz-next-0.7.3/alphaz_next/models/config/_base/internal_config_settings.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/models/config/_base/utils.py` & `alphaz-next-0.7.3/alphaz_next/models/config/_base/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/models/config/alpha_config.py` & `alphaz-next-0.7.3/alphaz_next/models/config/alpha_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/models/config/api_config.py` & `alphaz-next-0.7.3/alphaz_next/models/config/api_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/models/config/apm_config.py` & `alphaz-next-0.7.3/alphaz_next/models/config/apm_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/models/config/config_settings.py` & `alphaz-next-0.7.3/alphaz_next/models/config/config_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 
     class AlphaConfigSettingsSchema(_BaseSettings):
         environment: str = _Field(default="local", validation_alias=environment_alias)
         root: str = _Field(default=str(_Path.cwd()), validation_alias=root_alias)
         port: int = _Field(default=8000, validation_alias=port_alias)
         workers: int = _Field(default=1, validation_alias=workers_alias)
 
+        @_computed_field  # type: ignore
         @property
-        @_computed_field
         def main_config(self) -> _T:
             data = cast(Dict[str, Any], _open_json_file(path=_Path(path)))
 
             data_ext = {
                 "environment": self.environment,
                 "root": self.root,
                 "port": self.port,
```

### Comparing `alphaz-next-0.7.2/alphaz_next/models/config/database_config.py` & `alphaz-next-0.7.3/alphaz_next/models/config/database_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 
     host: str
     username: str
     password: str
     port: int
     service_name: str
 
+    @_computed_field  # type: ignore
     @property
-    @_computed_field
     def connection_string(self) -> str:
         """
         Returns the connection string for the Oracle database.
         """
         return (
             f"oracle+cx_oracle://{self.username}:{self.password}@"
             f"{self.host}:{self.port}/{self.service_name}"
@@ -59,16 +59,16 @@
 
     host: str
     username: str
     password: str
     port: int
     service_name: str
 
+    @_computed_field  # type: ignore
     @property
-    @_computed_field
     def connection_string(self) -> str:
         """
         Returns the connection string for the Oracle database.
         """
         return (
             f"oracle+oracledb://{self.username}:{self.password}@"
             f"{self.host}:{self.port}/{self.service_name}"
@@ -82,16 +82,16 @@
 
     host: str
     username: str
     password: str
     port: int
     service_name: str
 
+    @_computed_field  # type: ignore
     @property
-    @_computed_field
     def connection_string(self) -> str:
         """
         Returns the connection string for the Oracle database.
         """
         return (
             f"oracle+oracledb_async://{self.username}:{self.password}@"
             f"{self.host}:{self.port}/{self.service_name}"
@@ -101,16 +101,16 @@
 class _DatabaseSqliteConfigSchema(_DatabaseConfigBaseSchema):
     """
     Represents the configuration schema for an SQLite database connection.
     """
 
     path: str
 
+    @_computed_field  # type: ignore
     @property
-    @_computed_field
     def connection_string(self) -> str:
         """
         Returns the connection string for the SQLite database.
         Creates the parent directory if it doesn't exist.
         """
         _Path(self.path).parent.mkdir(parents=True, exist_ok=True)
         return f"sqlite:///{self.path}"
@@ -119,16 +119,16 @@
 class _DatabaseAioSqliteConfigSchema(_DatabaseConfigBaseSchema):
     """
     Represents the configuration schema for an SQLite database connection using aiosqlite driver.
     """
 
     path: str
 
+    @_computed_field  # type: ignore
     @property
-    @_computed_field
     def connection_string(self) -> str:
         """
         Returns the connection string for the SQLite database.
         """
         _Path(self.path).parent.mkdir(parents=True, exist_ok=True)
         return f"sqlite+aiosqlite:///{self.path}"
```

### Comparing `alphaz-next-0.7.2/alphaz_next/models/config/logging_config.py` & `alphaz-next-0.7.3/alphaz_next/models/config/logging_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,11 +67,11 @@
     @classmethod
     def validate_level(cls, value: str, info: _FieldValidationInfo) -> str:
         if value not in LOGGING_LEVEL:
             raise ValueError(f"{info.field_name} is not valid")
 
         return value
 
+    @_computed_field  # type: ignore
     @property
-    @_computed_field
     def level_code(self) -> int:
         return LOGGING_LEVEL.get(self.level.upper(), 0)
```

### Comparing `alphaz-next-0.7.2/alphaz_next/models/config/openapi_config_schema.py` & `alphaz-next-0.7.3/alphaz_next/models/config/openapi_config_schema.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/tests/utils/utils.py` & `alphaz-next-0.7.3/alphaz_next/tests/utils/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/utils/database.py` & `alphaz-next-0.7.3/alphaz_next/utils/database.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/utils/format.py` & `alphaz-next-0.7.3/alphaz_next/utils/format.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/utils/logger.py` & `alphaz-next-0.7.3/alphaz_next/utils/logger.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/utils/logging_filters.py` & `alphaz-next-0.7.3/alphaz_next/utils/logging_filters.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next/utils/loguru.py` & `alphaz-next-0.7.3/alphaz_next/utils/loguru.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/alphaz_next.egg-info/PKG-INFO` & `alphaz-next-0.7.3/alphaz_next.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.7.2
+Version: 0.7.3
 Summary: A project to make a lib to start FastAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.7.2.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.7.3.tar.gz
 Author: Maxime MARTIN
 Author-email: Maxime MARTIN <maxime.martin02@hotmail.fr>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alphaz-next-0.7.2/alphaz_next.egg-info/SOURCES.txt` & `alphaz-next-0.7.3/alphaz_next.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.2/setup.py` & `alphaz-next-0.7.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "0.7.2"
+version = "0.7.3"
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 
 EXTRAS_REQUIRE = {
     "dependency-injector": ["dependency-injector"],
```

