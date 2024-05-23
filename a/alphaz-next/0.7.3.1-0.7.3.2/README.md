# Comparing `tmp/alphaz-next-0.7.3.1.tar.gz` & `tmp/alphaz-next-0.7.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphaz-next-0.7.3.1.tar", last modified: Wed May 22 22:10:02 2024, max compression
+gzip compressed data, was "alphaz-next-0.7.3.2.tar", last modified: Wed May 22 22:16:44 2024, max compression
```

## Comparing `alphaz-next-0.7.3.1.tar` & `alphaz-next-0.7.3.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.312518 alphaz-next-0.7.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-22 22:10:02.312518 alphaz-next-0.7.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.300517 alphaz-next-0.7.3.1/alphaz_next/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.304517 alphaz-next-0.7.3.1/alphaz_next/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/asyncio/async_database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.304517 alphaz-next-0.7.3.1/alphaz_next/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.304517 alphaz-next-0.7.3.1/alphaz_next/core/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10602 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/exception_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.304517 alphaz-next-0.7.3.1/alphaz_next/core/responses/
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/responses/file_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/responses/html_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/responses/json_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/responses/orjson_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/responses/plaintext_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/responses/redirect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/responses/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/responses/streaming_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/core/responses/ujson_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.304517 alphaz-next-0.7.3.1/alphaz_next/libs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/libs/file_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/libs/httpx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.304517 alphaz-next-0.7.3.1/alphaz_next/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.304517 alphaz-next-0.7.3.1/alphaz_next/models/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/auth/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.308517 alphaz-next-0.7.3.1/alphaz_next/models/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.308517 alphaz-next-0.7.3.1/alphaz_next/models/config/_base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/_base/internal_config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/_base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/alpha_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/api_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/apm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/database_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/directories_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/models/config/openapi_config_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.308517 alphaz-next-0.7.3.1/alphaz_next/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.308517 alphaz-next-0.7.3.1/alphaz_next/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/tests/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.308517 alphaz-next-0.7.3.1/alphaz_next/tests/utils/mocking/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/tests/utils/mocking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/tests/utils/mocking/mock_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    26163 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/tests/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.308517 alphaz-next-0.7.3.1/alphaz_next/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/utils/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/utils/logging_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/alphaz_next/utils/loguru.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:10:02.304517 alphaz-next-0.7.3.1/alphaz_next.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-22 22:10:02.000000 alphaz-next-0.7.3.1/alphaz_next.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-22 22:10:02.000000 alphaz-next-0.7.3.1/alphaz_next.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:10:02.000000 alphaz-next-0.7.3.1/alphaz_next.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-22 22:10:02.000000 alphaz-next-0.7.3.1/alphaz_next.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 22:10:02.000000 alphaz-next-0.7.3.1/alphaz_next.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-22 22:09:59.000000 alphaz-next-0.7.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 22:10:02.312518 alphaz-next-0.7.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-22 22:10:01.000000 alphaz-next-0.7.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:44.943890 alphaz-next-0.7.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-22 22:16:44.943890 alphaz-next-0.7.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:44.935890 alphaz-next-0.7.3.2/alphaz_next/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:44.939890 alphaz-next-0.7.3.2/alphaz_next/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/asyncio/async_database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:44.939890 alphaz-next-0.7.3.2/alphaz_next/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:44.939890 alphaz-next-0.7.3.2/alphaz_next/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/core/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/core/_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/core/_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10602 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/core/exception_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:44.939890 alphaz-next-0.7.3.2/alphaz_next/core/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/core/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/core/responses/file_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/core/responses/html_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/core/responses/json_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/core/responses/orjson_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/core/responses/plaintext_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/core/responses/redirect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/core/responses/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/core/responses/streaming_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/core/responses/ujson_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:44.939890 alphaz-next-0.7.3.2/alphaz_next/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/libs/file_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/libs/httpx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:44.939890 alphaz-next-0.7.3.2/alphaz_next/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:44.939890 alphaz-next-0.7.3.2/alphaz_next/models/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/models/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/models/auth/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:44.943890 alphaz-next-0.7.3.2/alphaz_next/models/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/models/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:44.943890 alphaz-next-0.7.3.2/alphaz_next/models/config/_base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/models/config/_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/models/config/_base/internal_config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/models/config/_base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/models/config/alpha_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/models/config/api_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/models/config/apm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/models/config/config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/models/config/database_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/models/config/directories_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/models/config/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/models/config/openapi_config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:44.943890 alphaz-next-0.7.3.2/alphaz_next/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:44.943890 alphaz-next-0.7.3.2/alphaz_next/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:44.943890 alphaz-next-0.7.3.2/alphaz_next/tests/utils/mocking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/tests/utils/mocking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/tests/utils/mocking/mock_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26157 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/tests/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:44.943890 alphaz-next-0.7.3.2/alphaz_next/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/utils/logging_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/alphaz_next/utils/loguru.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:16:44.939890 alphaz-next-0.7.3.2/alphaz_next.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-22 22:16:44.000000 alphaz-next-0.7.3.2/alphaz_next.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-22 22:16:44.000000 alphaz-next-0.7.3.2/alphaz_next.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:16:44.000000 alphaz-next-0.7.3.2/alphaz_next.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-22 22:16:44.000000 alphaz-next-0.7.3.2/alphaz_next.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 22:16:44.000000 alphaz-next-0.7.3.2/alphaz_next.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-22 22:16:40.000000 alphaz-next-0.7.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 22:16:44.943890 alphaz-next-0.7.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-22 22:16:43.000000 alphaz-next-0.7.3.2/setup.py
```

### Comparing `alphaz-next-0.7.3.1/PKG-INFO` & `alphaz-next-0.7.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.7.3.1
+Version: 0.7.3.2
 Summary: A project to make a lib to start FastAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.7.3.1.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.7.3.2.tar.gz
 Author: Maxime MARTIN
 Author-email: Maxime MARTIN <maxime.martin02@hotmail.fr>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alphaz-next-0.7.3.1/README.md` & `alphaz-next-0.7.3.2/README.md`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/asyncio/async_database.py` & `alphaz-next-0.7.3.2/alphaz_next/asyncio/async_database.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/auth/auth.py` & `alphaz-next-0.7.3.2/alphaz_next/auth/auth.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/core/_base.py` & `alphaz-next-0.7.3.2/alphaz_next/core/_base.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/core/_middleware.py` & `alphaz-next-0.7.3.2/alphaz_next/core/_middleware.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/core/_telemetry.py` & `alphaz-next-0.7.3.2/alphaz_next/core/_telemetry.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/core/application.py` & `alphaz-next-0.7.3.2/alphaz_next/core/application.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/core/exception_handlers.py` & `alphaz-next-0.7.3.2/alphaz_next/core/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/core/exceptions.py` & `alphaz-next-0.7.3.2/alphaz_next/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/core/responses/__init__.py` & `alphaz-next-0.7.3.2/alphaz_next/core/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/core/responses/file_response.py` & `alphaz-next-0.7.3.2/alphaz_next/core/responses/file_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/core/responses/html_response.py` & `alphaz-next-0.7.3.2/alphaz_next/core/responses/html_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/core/responses/json_response.py` & `alphaz-next-0.7.3.2/alphaz_next/core/responses/json_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/core/responses/orjson_response.py` & `alphaz-next-0.7.3.2/alphaz_next/core/responses/orjson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/core/responses/plaintext_response.py` & `alphaz-next-0.7.3.2/alphaz_next/core/responses/plaintext_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/core/responses/redirect_response.py` & `alphaz-next-0.7.3.2/alphaz_next/core/responses/redirect_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/core/responses/response.py` & `alphaz-next-0.7.3.2/alphaz_next/core/responses/response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/core/responses/streaming_response.py` & `alphaz-next-0.7.3.2/alphaz_next/core/responses/streaming_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/core/responses/ujson_response.py` & `alphaz-next-0.7.3.2/alphaz_next/core/responses/ujson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/libs/httpx.py` & `alphaz-next-0.7.3.2/alphaz_next/libs/httpx.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/models/config/_base/internal_config_settings.py` & `alphaz-next-0.7.3.2/alphaz_next/models/config/_base/internal_config_settings.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/models/config/_base/utils.py` & `alphaz-next-0.7.3.2/alphaz_next/models/config/_base/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/models/config/alpha_config.py` & `alphaz-next-0.7.3.2/alphaz_next/models/config/alpha_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/models/config/api_config.py` & `alphaz-next-0.7.3.2/alphaz_next/models/config/api_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/models/config/apm_config.py` & `alphaz-next-0.7.3.2/alphaz_next/models/config/apm_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/models/config/config_settings.py` & `alphaz-next-0.7.3.2/alphaz_next/models/config/config_settings.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/models/config/database_config.py` & `alphaz-next-0.7.3.2/alphaz_next/models/config/database_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/models/config/logging_config.py` & `alphaz-next-0.7.3.2/alphaz_next/models/config/logging_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/models/config/openapi_config_schema.py` & `alphaz-next-0.7.3.2/alphaz_next/models/config/openapi_config_schema.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/tests/utils/utils.py` & `alphaz-next-0.7.3.2/alphaz_next/tests/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,15 +460,15 @@
             response_format: The format in which the response should be processed (default: JSON).
             saved_path: The path where the processed response should be saved (default: None).
 
         Returns:
             The status code of the response and the processed data.
         """
 
-        match response_format.value:
+        match response_format:
             case response_format.JSON:
                 data = response.json()
                 if saved_path is not None:
                     _save_json_file(saved_path, data)
             case response_format.BYTES:
                 data = response.content
                 if saved_path is not None:
```

### Comparing `alphaz-next-0.7.3.1/alphaz_next/utils/database.py` & `alphaz-next-0.7.3.2/alphaz_next/utils/database.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/utils/format.py` & `alphaz-next-0.7.3.2/alphaz_next/utils/format.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/utils/logger.py` & `alphaz-next-0.7.3.2/alphaz_next/utils/logger.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/utils/logging_filters.py` & `alphaz-next-0.7.3.2/alphaz_next/utils/logging_filters.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next/utils/loguru.py` & `alphaz-next-0.7.3.2/alphaz_next/utils/loguru.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/alphaz_next.egg-info/PKG-INFO` & `alphaz-next-0.7.3.2/alphaz_next.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.7.3.1
+Version: 0.7.3.2
 Summary: A project to make a lib to start FastAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.7.3.1.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.7.3.2.tar.gz
 Author: Maxime MARTIN
 Author-email: Maxime MARTIN <maxime.martin02@hotmail.fr>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alphaz-next-0.7.3.1/alphaz_next.egg-info/SOURCES.txt` & `alphaz-next-0.7.3.2/alphaz_next.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.1/setup.py` & `alphaz-next-0.7.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "0.7.3.1"
+version = "0.7.3.2"
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 
 EXTRAS_REQUIRE = {
     "dependency-injector": ["dependency-injector"],
```

