# Comparing `tmp/alphaz-next-0.7.3.tar.gz` & `tmp/alphaz-next-0.7.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphaz-next-0.7.3.tar", last modified: Wed May 22 14:13:16 2024, max compression
+gzip compressed data, was "alphaz-next-0.7.3.1.tar", last modified: Wed May 22 22:10:02 2024, max compression
```

## Comparing `alphaz-next-0.7.3.tar` & `alphaz-next-0.7.3.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.943364 alphaz-next-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-22 14:13:16.943364 alphaz-next-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.935365 alphaz-next-0.7.3/alphaz_next/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.935365 alphaz-next-0.7.3/alphaz_next/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/asyncio/async_database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.935365 alphaz-next-0.7.3/alphaz_next/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.939365 alphaz-next-0.7.3/alphaz_next/core/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/exception_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.939365 alphaz-next-0.7.3/alphaz_next/core/responses/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/responses/file_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/responses/html_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/responses/json_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/responses/orjson_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/responses/plaintext_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/responses/redirect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/responses/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/responses/streaming_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/core/responses/ujson_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.939365 alphaz-next-0.7.3/alphaz_next/libs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/libs/file_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/libs/httpx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.939365 alphaz-next-0.7.3/alphaz_next/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.939365 alphaz-next-0.7.3/alphaz_next/models/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/auth/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.939365 alphaz-next-0.7.3/alphaz_next/models/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.943364 alphaz-next-0.7.3/alphaz_next/models/config/_base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/_base/internal_config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/_base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/alpha_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/api_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/apm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/database_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/directories_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/models/config/openapi_config_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.943364 alphaz-next-0.7.3/alphaz_next/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.943364 alphaz-next-0.7.3/alphaz_next/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/tests/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.943364 alphaz-next-0.7.3/alphaz_next/tests/utils/mocking/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/tests/utils/mocking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/tests/utils/mocking/mock_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    26256 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/tests/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.943364 alphaz-next-0.7.3/alphaz_next/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/utils/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/utils/logging_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/alphaz_next/utils/loguru.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:13:16.935365 alphaz-next-0.7.3/alphaz_next.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-22 14:13:16.000000 alphaz-next-0.7.3/alphaz_next.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-22 14:13:16.000000 alphaz-next-0.7.3/alphaz_next.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:13:16.000000 alphaz-next-0.7.3/alphaz_next.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-22 14:13:16.000000 alphaz-next-0.7.3/alphaz_next.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 14:13:16.000000 alphaz-next-0.7.3/alphaz_next.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-22 14:13:10.000000 alphaz-next-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 14:13:16.943364 alphaz-next-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-22 14:13:14.000000 alphaz-next-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.312518 alphaz-next-0.7.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-22 22:10:02.312518 alphaz-next-0.7.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.300517 alphaz-next-0.7.3.1/alphaz_next/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.304517 alphaz-next-0.7.3.1/alphaz_next/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/asyncio/async_database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.304517 alphaz-next-0.7.3.1/alphaz_next/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.304517 alphaz-next-0.7.3.1/alphaz_next/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10602 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/exception_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.304517 alphaz-next-0.7.3.1/alphaz_next/core/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/responses/file_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/responses/html_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/responses/json_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/responses/orjson_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/responses/plaintext_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/responses/redirect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/responses/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/responses/streaming_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/responses/ujson_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.304517 alphaz-next-0.7.3.1/alphaz_next/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/libs/file_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/libs/httpx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.304517 alphaz-next-0.7.3.1/alphaz_next/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.304517 alphaz-next-0.7.3.1/alphaz_next/models/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/auth/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.308517 alphaz-next-0.7.3.1/alphaz_next/models/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.308517 alphaz-next-0.7.3.1/alphaz_next/models/config/_base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/_base/internal_config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/_base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/alpha_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/api_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/apm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/database_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/directories_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/openapi_config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.308517 alphaz-next-0.7.3.1/alphaz_next/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.308517 alphaz-next-0.7.3.1/alphaz_next/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.308517 alphaz-next-0.7.3.1/alphaz_next/tests/utils/mocking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/tests/utils/mocking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/tests/utils/mocking/mock_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26163 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/tests/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.308517 alphaz-next-0.7.3.1/alphaz_next/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/utils/logging_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/utils/loguru.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.304517 alphaz-next-0.7.3.1/alphaz_next.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-22 22:10:02.000000 alphaz-next-0.7.3.1/alphaz_next.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-22 22:10:02.000000 alphaz-next-0.7.3.1/alphaz_next.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:10:02.000000 alphaz-next-0.7.3.1/alphaz_next.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-22 22:10:02.000000 alphaz-next-0.7.3.1/alphaz_next.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 22:10:02.000000 alphaz-next-0.7.3.1/alphaz_next.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 22:10:02.312518 alphaz-next-0.7.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-22 22:10:01.000000 alphaz-next-0.7.3.1/setup.py
```

### Comparing `alphaz-next-0.7.3/PKG-INFO` & `alphaz-next-0.7.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.7.3
+Version: 0.7.3.1
 Summary: A project to make a lib to start FastAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.7.3.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.7.3.1.tar.gz
 Author: Maxime MARTIN
 Author-email: Maxime MARTIN <maxime.martin02@hotmail.fr>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alphaz-next-0.7.3/README.md` & `alphaz-next-0.7.3.1/README.md`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/alphaz_next/asyncio/async_database.py` & `alphaz-next-0.7.3.1/alphaz_next/utils/database.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,41 +2,43 @@
 from typing import (
     List as _List,
     Optional as _Optional,
     Type as _Type,
 )
 
 # PYSQL_REPO
-from pysql_repo.asyncio import AsyncDataBase as _AsyncDataBase
+from pysql_repo import DataBase as _DataBase
 from pysql_repo._database_base import (
     DataBaseConfigTypedDict as _DataBaseConfigTypedDict,
 )
 
 # SQLALCHEMY
-from sqlalchemy import MetaData
-from sqlalchemy.orm import DeclarativeBase
+from sqlalchemy import MetaData as _MetaData
+from sqlalchemy.orm import DeclarativeBase as _DeclarativeBase
 
 # OPENTELEMETRY
-from opentelemetry.instrumentation.sqlalchemy import SQLAlchemyInstrumentor
+from opentelemetry.instrumentation.sqlalchemy import (
+    SQLAlchemyInstrumentor as _SQLAlchemyInstrumentor,
+)
 
 
-class AsyncDataBase(_AsyncDataBase):
+class DataBase(_DataBase):
 
     def __init__(
         self,
         databases_config: _DataBaseConfigTypedDict,
-        base: _Type[DeclarativeBase],
-        metadata_views: _Optional[_List[MetaData]] = None,
+        base: _Type[_DeclarativeBase],
+        metadata_views: _Optional[_List[_MetaData]] = None,
         autoflush: bool = False,
         expire_on_commit: bool = False,
         echo: bool = False,
     ) -> None:
         super().__init__(
             databases_config=databases_config,
             base=base,
             metadata_views=metadata_views,
             autoflush=autoflush,
             expire_on_commit=expire_on_commit,
             echo=echo,
         )
 
-        SQLAlchemyInstrumentor().instrument(engine=self._engine.sync_engine)
+        _SQLAlchemyInstrumentor().instrument(engine=self._engine)
```

### Comparing `alphaz-next-0.7.3/alphaz_next/auth/auth.py` & `alphaz-next-0.7.3.1/alphaz_next/auth/auth.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/alphaz_next/core/_base.py` & `alphaz-next-0.7.3.1/alphaz_next/core/_base.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/alphaz_next/core/_middleware.py` & `alphaz-next-0.7.3.1/alphaz_next/core/_middleware.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/alphaz_next/core/_telemetry.py` & `alphaz-next-0.7.3.1/alphaz_next/core/_telemetry.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/alphaz_next/core/application.py` & `alphaz-next-0.7.3.1/alphaz_next/core/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # MODULES
-from logging.handlers import TimedRotatingFileHandler
-from pathlib import Path
+import logging as _logging
+from logging.handlers import TimedRotatingFileHandler as _TimedRotatingFileHandler
+from pathlib import Path as _Path
 import sys as _sys
 from typing import (
-    Annotated,
     Any as _Any,
     Dict as _Dict,
     List as _List,
     Optional as _Optional,
     Sequence as _Sequence,
     Union as _Union,
 )
-import logging as _logging
 
 # FASTAPI
 from fastapi import (
     APIRouter as _APIRouter,
     FastAPI as _FastAPI,
     HTTPException as _HTTPException,
     Request as _Request,
@@ -181,18 +180,18 @@
         and config.api_config.logging.retention is not None
     ):
         uvicorn_formatter = _logging.Formatter(
             config.api_config.logging.uvicorn_format,
             datefmt=config.api_config.logging.date_format,
         )
 
-        directory_path = Path(config.api_config.directories.logs)
+        directory_path = _Path(config.api_config.directories.logs)
         directory_path.mkdir(parents=True, exist_ok=True)
 
-        handler = TimedRotatingFileHandler(
+        handler = _TimedRotatingFileHandler(
             filename=directory_path / "uvicorn.log",
             when=config.api_config.logging.rotation,
             backupCount=config.api_config.logging.retention,
         )
         handler.setFormatter(uvicorn_formatter)
 
         uvicorn_logger.addHandler(handler)
```

### Comparing `alphaz-next-0.7.3/alphaz_next/core/exception_handlers.py` & `alphaz-next-0.7.3.1/alphaz_next/core/exception_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+# FASTAPI
 from fastapi.encoders import jsonable_encoder as _jsonable_encoder
 from fastapi.exceptions import (
     RequestValidationError as _RequestValidationError,
     WebSocketRequestValidationError as _WebSocketRequestValidationError,
 )
 from fastapi.utils import (
     is_body_allowed_for_status_code as _is_body_allowed_for_status_code,
 )
 from fastapi.websockets import WebSocket as _WebSocket
+
+# STARLETTE
 from starlette.exceptions import HTTPException as _HTTPException
 from starlette.requests import Request as _Request
 from starlette.responses import JSONResponse as _JSONResponse, Response as _Response
 from starlette.status import (
     HTTP_422_UNPROCESSABLE_ENTITY as _HTTP_422_UNPROCESSABLE_ENTITY,
     WS_1008_POLICY_VIOLATION as _WS_1008_POLICY_VIOLATION,
 )
```

### Comparing `alphaz-next-0.7.3/alphaz_next/core/exceptions.py` & `alphaz-next-0.7.3.1/alphaz_next/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/alphaz_next/core/responses/file_response.py` & `alphaz-next-0.7.3.1/alphaz_next/core/responses/file_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/alphaz_next/core/responses/html_response.py` & `alphaz-next-0.7.3.1/alphaz_next/core/responses/html_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/alphaz_next/core/responses/json_response.py` & `alphaz-next-0.7.3.1/alphaz_next/core/responses/json_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/alphaz_next/core/responses/orjson_response.py` & `alphaz-next-0.7.3.1/alphaz_next/core/responses/orjson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/alphaz_next/core/responses/plaintext_response.py` & `alphaz-next-0.7.3.1/alphaz_next/core/responses/plaintext_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/alphaz_next/core/responses/redirect_response.py` & `alphaz-next-0.7.3.1/alphaz_next/core/responses/redirect_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/alphaz_next/core/responses/response.py` & `alphaz-next-0.7.3.1/alphaz_next/core/responses/response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/alphaz_next/core/responses/streaming_response.py` & `alphaz-next-0.7.3.1/alphaz_next/core/responses/streaming_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/alphaz_next/core/responses/ujson_response.py` & `alphaz-next-0.7.3.1/alphaz_next/core/responses/ujson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/alphaz_next/libs/httpx.py` & `alphaz-next-0.7.3.1/alphaz_next/libs/httpx.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # MODULES
-import asyncio
-import time
+import asyncio as _asyncio
+import time as _time
 from typing import (
     Any as _Any,
-    Dict as _Dict,
     List as _List,
     Literal as _Literal,
     Optional as _Optional,
     Type as _Type,
     TypeVar as _TypeVar,
     Union as _Union,
 )
 
 # FASTAPI
-from fastapi import HTTPException
+from fastapi import HTTPException as _HTTPException
 
 # PYDANTIC
-from pydantic import BaseModel
+from pydantic import BaseModel as _BaseModel
 
 # HTTPX
-import httpx
+import httpx as _httpx
 
 
 def make_request_with_retry(
     method: _Literal["POST", "PATCH", "PUT", "DELETE", "GET"],
     url: str,
     max_retries: int = 3,
     retry_on_status: _Optional[_List[int]] = None,
     timeout: _Optional[float] = None,
     **kwargs: _Any,
-) -> httpx.Response:
+) -> _httpx.Response:
     """
     Makes an HTTP request with retries in case of a timeout error.
 
     Args:
         method (Literal["POST", "PATCH", "PUT", "DELETE", "GET"]): The HTTP method to use.
         url (str): The URL to make the request to.
         max_retries (int, optional): The maximum number of retries to attempt. Defaults to 3.
@@ -53,30 +52,30 @@
         "kwargs": {k: v for k, v in kwargs.items() if k in ["params", "headers"]},
     }
 
     retry_statuses = retry_on_status or []
 
     for retry_count in range(max_retries + 1):
         try:
-            with httpx.Client(timeout=timeout) as client:
-                response: httpx.Response = getattr(client, method.lower())(
+            with _httpx.Client(timeout=timeout) as client:
+                response: _httpx.Response = getattr(client, method.lower())(
                     url, **kwargs
                 )
-        except httpx.ReadTimeout as ex:
+        except _httpx.ReadTimeout as ex:
             if retry_count == max_retries:
                 raise RuntimeError(
                     f"Unable to contact server after {retry_count} retries {item_repr}"
                 )
 
             wait_time = 2**retry_count
-            time.sleep(wait_time)
-        except httpx.HTTPStatusError as ex:
+            _time.sleep(wait_time)
+        except _httpx.HTTPStatusError as ex:
             if ex.response.status_code in retry_statuses and retry_count < max_retries:
                 wait_time = 2**retry_count
-                time.sleep(wait_time)
+                _time.sleep(wait_time)
             else:
                 raise ex
         except Exception as ex:
             raise RuntimeError(
                 f"An unknown error occurs while contacting external server {item_repr}"
             ) from ex
         else:
@@ -88,15 +87,15 @@
 async def make_async_request_with_retry(
     method: _Literal["POST", "PATCH", "PUT", "DELETE", "GET"],
     url: str,
     max_retries: int = 3,
     retry_on_status: _Optional[_List[int]] = None,
     timeout: _Optional[float] = None,
     **kwargs: _Any,
-) -> httpx.Response:
+) -> _httpx.Response:
     """
     Makes an HTTP request with retries in case of a timeout error.
 
     Args:
         method (Literal["POST", "PATCH", "PUT", "DELETE", "GET"]): The HTTP method to use.
         url (str): The URL to make the request to.
         max_retries (int, optional): The maximum number of retries to attempt. Defaults to 3.
@@ -116,47 +115,47 @@
         "kwargs": {k: v for k, v in kwargs.items() if k in ["params", "headers"]},
     }
 
     retry_statuses = retry_on_status or []
 
     for retry_count in range(max_retries + 1):
         try:
-            async with httpx.AsyncClient(timeout=timeout) as client:
-                response: httpx.Response = await getattr(client, method.lower())(
+            async with _httpx.AsyncClient(timeout=timeout) as client:
+                response: _httpx.Response = await getattr(client, method.lower())(
                     url, **kwargs
                 )
-        except httpx.ReadTimeout as ex:
+        except _httpx.ReadTimeout as ex:
             if retry_count == max_retries:
                 raise RuntimeError(
                     f"Unable to contact server after {retry_count} retries {item_repr}"
                 )
 
             wait_time = 2**retry_count
-            await asyncio.sleep(wait_time)
-        except httpx.HTTPStatusError as ex:
+            await _asyncio.sleep(wait_time)
+        except _httpx.HTTPStatusError as ex:
             if ex.response.status_code in retry_statuses and retry_count < max_retries:
                 wait_time = 2**retry_count
-                await asyncio.sleep(wait_time)
+                await _asyncio.sleep(wait_time)
             else:
                 raise ex
         except Exception as ex:
             raise RuntimeError(
                 f"An unknown error occurs while contacting external server {item_repr}"
             ) from ex
         else:
             return response
 
     raise RuntimeError(f"Maximum number of retries exceeded {item_repr}")
 
 
-_T = _TypeVar("_T", bound=BaseModel)
+_T = _TypeVar("_T", bound=_BaseModel)
 
 
 def post_process_http_response(
-    response: httpx.Response,
+    response: _httpx.Response,
     schema: _Optional[_Type[_T]] = None,
     mode_alpha: bool = False,
 ) -> _Union[_T, _List[_T], _Any]:
     """
     Processes an HTTP response and returns the response body as a validated object or a list of validated objects.
 
     Args:
@@ -167,15 +166,15 @@
     Returns:
         The validated response body as an object or a list of objects.
 
     Raises:
         HTTPException: If the response is not a success.
     """
     if not response.is_success:
-        raise HTTPException(
+        raise _HTTPException(
             status_code=response.status_code,
             detail=response.text,
             headers={k: v for k, v in response.headers.items()},
         )
 
     response_json = response.json()
     if mode_alpha:
```

### Comparing `alphaz-next-0.7.3/alphaz_next/models/config/_base/internal_config_settings.py` & `alphaz-next-0.7.3.1/alphaz_next/models/config/_base/internal_config_settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,45 @@
-from typing import Protocol as _Protocol
-
 # PYDANTIC
 from pydantic import Field
 from pydantic_settings import BaseSettings
 
 
-class AlphaInternalConfigProtocol(_Protocol):
+class AlphaInternalConfigSettingsSchema:
     token_url: str
     user_me_url: str
     api_key_me_url: str
     secret_key: str
     algorithm: str
 
 
 def create_internal_config(
     token_url_alias: str = "ALPHA_TOKEN_URL",
     user_me_url_alias: str = "ALPHA_USER_ME_URL",
     api_key_me_url_alias: str = "ALPHA_API_KEY_ME_URL",
     secret_key_alias: str = "ALPHA_SECRET_KEY",
     algorithm_alias: str = "ALPHA_ALGORITHM",
-) -> AlphaInternalConfigProtocol:
+) -> AlphaInternalConfigSettingsSchema:
     """
     Create an instance of the AlphaInternalConfigSettingsSchema class with the provided configuration settings.
 
     Args:
         token_url_alias (str, optional): The alias for the token URL. Defaults to "ALPHA_TOKEN_URL".
         user_me_url_alias (str, optional): The alias for the user me URL. Defaults to "ALPHA_USER_ME_URL".
         api_key_me_url_alias (str, optional): The alias for the API key me URL. Defaults to "ALPHA_API_KEY_ME_URL".
         secret_key_alias (str, optional): The alias for the secret key. Defaults to "ALPHA_SECRET_KEY".
         algorithm_alias (str, optional): The alias for the algorithm. Defaults to "ALPHA_ALGORITHM".
 
     Returns:
         AlphaInternalConfigSettingsSchema: An instance of the AlphaInternalConfigSettingsSchema class.
     """
 
-    class AlphaInternalConfigSettingsSchema(BaseSettings, AlphaInternalConfigProtocol):
+    class _AlphaInternalConfigSettingsSchema(
+        BaseSettings,
+        AlphaInternalConfigSettingsSchema,
+    ):
         token_url: str = Field(
             default="/auth",
             validation_alias=token_url_alias,
         )
         user_me_url: str = Field(
             default="user/me",
             validation_alias=user_me_url_alias,
@@ -52,8 +53,8 @@
             validation_alias=secret_key_alias,
         )
         algorithm: str = Field(
             default="",
             validation_alias=algorithm_alias,
         )
 
-    return AlphaInternalConfigSettingsSchema()
+    return _AlphaInternalConfigSettingsSchema()
```

### Comparing `alphaz-next-0.7.3/alphaz_next/models/config/_base/utils.py` & `alphaz-next-0.7.3.1/alphaz_next/models/config/_base/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/alphaz_next/models/config/alpha_config.py` & `alphaz-next-0.7.3.1/alphaz_next/models/config/alpha_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/alphaz_next/models/config/api_config.py` & `alphaz-next-0.7.3.1/alphaz_next/models/config/api_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/alphaz_next/models/config/apm_config.py` & `alphaz-next-0.7.3.1/alphaz_next/models/config/apm_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/alphaz_next/models/config/config_settings.py` & `alphaz-next-0.7.3.1/alphaz_next/models/config/config_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # MODULES
 from pathlib import Path as _Path
-from typing import Any, Dict, Type as _Type, TypeVar as _TypeVar, cast
+from typing import (
+    Any as _Any,
+    Dict as _Dict,
+    Type as _Type,
+    TypeVar as _TypeVar,
+    cast as _cast,
+)
 
 # PYDANTIC
 from pydantic import Field as _Field, computed_field as _computed_field
 from pydantic_settings import BaseSettings as _BaseSettings
 
 # LIBS
 from alphaz_next.libs.file_lib import open_json_file as _open_json_file
@@ -43,15 +49,15 @@
         root: str = _Field(default=str(_Path.cwd()), validation_alias=root_alias)
         port: int = _Field(default=8000, validation_alias=port_alias)
         workers: int = _Field(default=1, validation_alias=workers_alias)
 
         @_computed_field  # type: ignore
         @property
         def main_config(self) -> _T:
-            data = cast(Dict[str, Any], _open_json_file(path=_Path(path)))
+            data = _cast(_Dict[str, _Any], _open_json_file(path=_Path(path)))
 
             data_ext = {
                 "environment": self.environment,
                 "root": self.root,
                 "port": self.port,
                 "workers": self.workers,
             }
```

### Comparing `alphaz-next-0.7.3/alphaz_next/models/config/database_config.py` & `alphaz-next-0.7.3.1/alphaz_next/models/config/database_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/alphaz_next/models/config/logging_config.py` & `alphaz-next-0.7.3.1/alphaz_next/models/config/logging_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # MODULES
 import logging as _logging
 from typing import Annotated as _Annotated, List as _List, Optional as _Optional
 
 # OPENTELEMETRY
-from opentelemetry.instrumentation.logging import LoggingInstrumentor
+from opentelemetry.instrumentation.logging import (
+    LoggingInstrumentor as _LoggingInstrumentor,
+)
 
 # PYDANTIC
 from pydantic_core.core_schema import FieldValidationInfo as _FieldValidationInfo
 from pydantic import (
     BaseModel as _BaseModel,
     ConfigDict as _ConfigDict,
     Field as _Field,
@@ -55,15 +57,15 @@
     retention: _Optional[int] = _Field(default=None)
     excluded_routers: _List[str] = _Field(default_factory=lambda: [])
 
     @_field_validator("format")
     @classmethod
     def validate_format(cls, value: str, info: _FieldValidationInfo) -> str:
         if value is not None:
-            LoggingInstrumentor().instrument(logging_format=value)
+            _LoggingInstrumentor().instrument(logging_format=value)
 
         return value
 
     @_field_validator("level")
     @classmethod
     def validate_level(cls, value: str, info: _FieldValidationInfo) -> str:
         if value not in LOGGING_LEVEL:
```

### Comparing `alphaz-next-0.7.3/alphaz_next/models/config/openapi_config_schema.py` & `alphaz-next-0.7.3.1/alphaz_next/models/config/openapi_config_schema.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # MODULES
-from typing import Dict, List, Optional
+from typing import Dict as _Dict, List as _List, Optional as _Optional
 
 # PYDANTIC
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import BaseModel as _BaseModel, ConfigDict as _ConfigDict, Field as _Field
 
 
-class ContactSchema(BaseModel):
-    name: Optional[str] = Field(default=None)
-    email: Optional[str] = Field(default=None)
+class ContactSchema(_BaseModel):
+    name: _Optional[str] = _Field(default=None)
+    email: _Optional[str] = _Field(default=None)
 
 
-class OpenApiSchema(BaseModel):
-    model_config = ConfigDict(from_attributes=True)
+class OpenApiSchema(_BaseModel):
+    model_config = _ConfigDict(from_attributes=True)
 
-    description: Optional[str] = Field(default=None)
-    contact: Optional[ContactSchema] = Field(default=None)
-    swagger_favicon_url: Optional[str] = Field(default=None)
-    redoc_favicon_url: Optional[str] = Field(default=None)
-    tags: List[Dict[str, str]] = Field(default_factory=lambda: [])
+    description: _Optional[str] = _Field(default=None)
+    contact: _Optional[ContactSchema] = _Field(default=None)
+    swagger_favicon_url: _Optional[str] = _Field(default=None)
+    redoc_favicon_url: _Optional[str] = _Field(default=None)
+    tags: _List[_Dict[str, str]] = _Field(default_factory=lambda: [])
```

### Comparing `alphaz-next-0.7.3/alphaz_next/tests/utils/utils.py` & `alphaz-next-0.7.3.1/alphaz_next/tests/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # MODULES
 from enum import Enum as _Enum
 import json as _json
-import os
+import os as _os
 import re as _re
 from pathlib import Path as _Path
 from typing import (
     Any as _Any,
     Callable as _Callable,
     Dict as _Dict,
     List as _List,
@@ -35,25 +35,22 @@
 
 # PYDANTIC
 from pydantic import BaseModel as _BaseModel, Field as _Field
 
 # HTTPX
 from httpx import Response as _Response
 from httpx._types import (
-    HeaderTypes as _HeaderTypes,
     QueryParamTypes as _QueryParamTypes,
 )
 from alphaz_next.core.constants import HeaderEnum as _HeaderEnum
 
 # LIBS
 from alphaz_next.libs.file_lib import (
     save_file as _save_file,
     save_json_file as _save_json_file,
-    open_json_file as _open_json_file,
-    open_file as _open_file,
 )
 
 
 class ExpectedResponse(_BaseModel):
     """
     Represents the expected response from an API request.
 
@@ -721,15 +718,15 @@
             file_path = (
                 saved_dir_path / f"{qualname.replace('.', '__')}.{format}"
                 if saved_file_path is None
                 else saved_dir_path / saved_file_path
             )
 
             expected_data: _Union[_List[_Dict[str, _Any]], _Dict[str, _Any], bytes] = {}
-            if os.path.exists(file_path):
+            if _os.path.exists(file_path):
                 with open(file_path, encoding=encoding) as file:
                     match format:
                         case "json":
                             expected_data = _cast(
                                 _Union[_List[_Dict[str, _Any]], _Dict[str, _Any]],
                                 _json.load(file),
                             )
```

### Comparing `alphaz-next-0.7.3/alphaz_next/utils/database.py` & `alphaz-next-0.7.3.1/alphaz_next/asyncio/async_database.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,41 +2,43 @@
 from typing import (
     List as _List,
     Optional as _Optional,
     Type as _Type,
 )
 
 # PYSQL_REPO
-from pysql_repo import DataBase as _DataBase
+from pysql_repo.asyncio import AsyncDataBase as _AsyncDataBase
 from pysql_repo._database_base import (
     DataBaseConfigTypedDict as _DataBaseConfigTypedDict,
 )
 
 # SQLALCHEMY
-from sqlalchemy import MetaData
-from sqlalchemy.orm import DeclarativeBase
+from sqlalchemy import MetaData as _MetaData
+from sqlalchemy.orm import DeclarativeBase as _DeclarativeBase
 
 # OPENTELEMETRY
-from opentelemetry.instrumentation.sqlalchemy import SQLAlchemyInstrumentor
+from opentelemetry.instrumentation.sqlalchemy import (
+    SQLAlchemyInstrumentor as _SQLAlchemyInstrumentor,
+)
 
 
-class DataBase(_DataBase):
+class AsyncDataBase(_AsyncDataBase):
 
     def __init__(
         self,
         databases_config: _DataBaseConfigTypedDict,
-        base: _Type[DeclarativeBase],
-        metadata_views: _Optional[_List[MetaData]] = None,
+        base: _Type[_DeclarativeBase],
+        metadata_views: _Optional[_List[_MetaData]] = None,
         autoflush: bool = False,
         expire_on_commit: bool = False,
         echo: bool = False,
     ) -> None:
         super().__init__(
             databases_config=databases_config,
             base=base,
             metadata_views=metadata_views,
             autoflush=autoflush,
             expire_on_commit=expire_on_commit,
             echo=echo,
         )
 
-        SQLAlchemyInstrumentor().instrument(engine=self._engine)
+        _SQLAlchemyInstrumentor().instrument(engine=self._engine.sync_engine)
```

### Comparing `alphaz-next-0.7.3/alphaz_next/utils/format.py` & `alphaz-next-0.7.3.1/alphaz_next/utils/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 )
 
 # PYDANTIC
 from pydantic import BaseModel as _BaseModel
 
 # SQLALCHEMY
 from sqlalchemy.orm import (
-    DeclarativeBase,
+    DeclarativeBase as _DeclarativeBase,
     InstrumentedAttribute as _InstrumentedAttribute,
     RelationshipProperty as _RelationshipProperty,
 )
 
-_T = _TypeVar("_T", bound=DeclarativeBase)
+_T = _TypeVar("_T", bound=_DeclarativeBase)
 
 
 def uppercase(
     items: _Optional[_Union[_List[str], _Set[str], str]],
 ) -> _Optional[_Union[_List[str], _Set[str], str]]:
     """
     Converts the given string or list of strings to uppercase.
```

### Comparing `alphaz-next-0.7.3/alphaz_next/utils/logger.py` & `alphaz-next-0.7.3.1/alphaz_next/utils/logger.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/alphaz_next/utils/logging_filters.py` & `alphaz-next-0.7.3.1/alphaz_next/utils/logging_filters.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/alphaz_next/utils/loguru.py` & `alphaz-next-0.7.3.1/alphaz_next/utils/loguru.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # MODULES
 import sys as _sys
-from typing import Dict, Optional as _Optional, cast as _cast
+from typing import Dict as _Dict, Optional as _Optional, cast as _cast
 from loguru import logger as _logger, Logger as _Logger, _defaults
 
 # OPENTELEMETRY
 from opentelemetry import trace as _trace
 
-_LOGGERS: Dict[str, "Logger"] = {}
+_LOGGERS: _Dict[str, "Logger"] = {}
 
 
 class Logger:
 
     def __init__(
         self,
         name: str,
```

### Comparing `alphaz-next-0.7.3/alphaz_next.egg-info/PKG-INFO` & `alphaz-next-0.7.3.1/alphaz_next.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.7.3
+Version: 0.7.3.1
 Summary: A project to make a lib to start FastAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.7.3.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.7.3.1.tar.gz
 Author: Maxime MARTIN
 Author-email: Maxime MARTIN <maxime.martin02@hotmail.fr>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alphaz-next-0.7.3/alphaz_next.egg-info/SOURCES.txt` & `alphaz-next-0.7.3.1/alphaz_next.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3/setup.py` & `alphaz-next-0.7.3.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "0.7.3"
+version = "0.7.3.1"
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 
 EXTRAS_REQUIRE = {
     "dependency-injector": ["dependency-injector"],
```

