# Comparing `tmp/singlestoredb-1.3.0.tar.gz` & `tmp/singlestoredb-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singlestoredb-1.3.0.tar", last modified: Fri May 10 21:29:57 2024, max compression
+gzip compressed data, was "singlestoredb-1.3.1.tar", last modified: Thu May 23 20:13:51 2024, max compression
```

## Comparing `singlestoredb-1.3.0.tar` & `singlestoredb-1.3.1.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.152995 singlestoredb-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-10 21:29:57.152995 singlestoredb-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   161827 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/accel.c
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-10 21:29:57.152995 singlestoredb-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.136995 singlestoredb-1.3.0/singlestoredb/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.136995 singlestoredb-1.3.0/singlestoredb/alchemy/
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/alchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    44958 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20681 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.140995 singlestoredb-1.3.0/singlestoredb/functions/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/functions/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    31408 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/functions/dtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.140995 singlestoredb-1.3.0/singlestoredb/functions/ext/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/functions/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/functions/ext/arrow.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    40088 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/functions/ext/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/functions/ext/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/functions/ext/mmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    22306 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/functions/ext/rowdat_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/functions/ext/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18866 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/functions/signature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.140995 singlestoredb-1.3.0/singlestoredb/fusion/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/fusion/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)    21581 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/fusion/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.140995 singlestoredb-1.3.0/singlestoredb/fusion/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/fusion/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13643 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/fusion/handlers/stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/fusion/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25000 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/fusion/handlers/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/fusion/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/fusion/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.140995 singlestoredb-1.3.0/singlestoredb/http/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39349 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/http/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.140995 singlestoredb-1.3.0/singlestoredb/management/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/management/billing_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/management/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     8810 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/management/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/management/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/management/region.py
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/management/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    61632 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/management/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.144996 singlestoredb-1.3.0/singlestoredb/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/charset.py
--rw-r--r--   0 runner    (1001) docker     (127)    70301 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.144996 singlestoredb-1.3.0/singlestoredb/mysql/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/constants/CLIENT.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/constants/COMMAND.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/constants/CR.py
--rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/constants/ER.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/constants/EXTENDED_TYPE.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/constants/FIELD_TYPE.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/constants/FLAG.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/constants/SERVER_STATUS.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/constants/VECTOR_TYPE.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)    26794 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/cursors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/err.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/optionfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    14451 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.144996 singlestoredb-1.3.0/singlestoredb/mysql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/test_DictCursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/test_SSCursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15465 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    32297 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/test_cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/test_err.py
--rw-r--r--   0 runner    (1001) docker     (127)    18965 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/test_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/test_load_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/test_nextset.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/test_optionfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.144996 singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.148995 singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    31414 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/times.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.148995 singlestoredb-1.3.0/singlestoredb/notebook/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/notebook/_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/pytest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.148995 singlestoredb-1.3.0/singlestoredb/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/empty.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.148995 singlestoredb-1.3.0/singlestoredb/tests/ext_funcs/
--rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/ext_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/local_infile.csv
--rw-r--r--   0 runner    (1001) docker     (127)    17679 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test.sql
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test2.sql
--rwxr-xr-x   0 runner    (1001) docker     (127)    44180 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_basics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11184 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   117405 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_dbapi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1131 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    37357 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_ext_func.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    47695 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_ext_func_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_fusion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8580 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_http.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28223 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_plugin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6582 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_results.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4500 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_types.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28075 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_udf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10408 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_xdict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.152995 singlestoredb-1.3.0/singlestoredb/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24503 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/utils/convert_rows.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/utils/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/utils/mogrify.py
--rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/utils/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    12896 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/utils/xdict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.136995 singlestoredb-1.3.0/singlestoredb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-10 21:29:57.000000 singlestoredb-1.3.0/singlestoredb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-10 21:29:57.000000 singlestoredb-1.3.0/singlestoredb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 21:29:57.000000 singlestoredb-1.3.0/singlestoredb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-10 21:29:57.000000 singlestoredb-1.3.0/singlestoredb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-10 21:29:57.000000 singlestoredb-1.3.0/singlestoredb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 21:29:57.000000 singlestoredb-1.3.0/singlestoredb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:51.383731 singlestoredb-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-23 20:13:51.387731 singlestoredb-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   161827 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/accel.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-23 20:13:51.387731 singlestoredb-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:51.371731 singlestoredb-1.3.1/singlestoredb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:51.371731 singlestoredb-1.3.1/singlestoredb/alchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/alchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44958 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20681 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:51.371731 singlestoredb-1.3.1/singlestoredb/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/functions/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31408 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/functions/dtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:51.371731 singlestoredb-1.3.1/singlestoredb/functions/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/functions/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/functions/ext/arrow.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    40017 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/functions/ext/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/functions/ext/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/functions/ext/mmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22306 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/functions/ext/rowdat_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/functions/ext/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18866 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/functions/signature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:51.375731 singlestoredb-1.3.1/singlestoredb/fusion/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/fusion/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21581 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/fusion/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:51.375731 singlestoredb-1.3.1/singlestoredb/fusion/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/fusion/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13643 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/fusion/handlers/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/fusion/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25000 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/fusion/handlers/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/fusion/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/fusion/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:51.375731 singlestoredb-1.3.1/singlestoredb/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39349 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/http/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:51.375731 singlestoredb-1.3.1/singlestoredb/management/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/management/billing_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/management/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8810 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/management/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/management/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/management/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/management/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61642 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/management/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:51.375731 singlestoredb-1.3.1/singlestoredb/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/charset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70361 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:51.379731 singlestoredb-1.3.1/singlestoredb/mysql/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/constants/CLIENT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/constants/COMMAND.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/constants/CR.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/constants/ER.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/constants/EXTENDED_TYPE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/constants/FIELD_TYPE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/constants/FLAG.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/constants/SERVER_STATUS.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/constants/VECTOR_TYPE.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26794 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/cursors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/err.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/optionfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14451 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:51.379731 singlestoredb-1.3.1/singlestoredb/mysql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/tests/test_DictCursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/tests/test_SSCursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15465 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32297 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/tests/test_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/tests/test_err.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18965 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/tests/test_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/tests/test_load_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/tests/test_nextset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/tests/test_optionfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:51.379731 singlestoredb-1.3.1/singlestoredb/mysql/tests/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/tests/thirdparty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:51.379731 singlestoredb-1.3.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31414 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/mysql/times.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:51.379731 singlestoredb-1.3.1/singlestoredb/notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/notebook/_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/pytest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:51.383731 singlestoredb-1.3.1/singlestoredb/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/tests/empty.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:51.383731 singlestoredb-1.3.1/singlestoredb/tests/ext_funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/tests/ext_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/tests/local_infile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    17679 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/tests/test.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/tests/test2.sql
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44180 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/tests/test_basics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11184 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   117405 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/tests/test_dbapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1131 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/tests/test_exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37357 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/tests/test_ext_func.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    47695 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/tests/test_ext_func_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/tests/test_fusion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8580 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/tests/test_http.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28223 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/tests/test_plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6582 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/tests/test_results.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4500 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/tests/test_types.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28075 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/tests/test_udf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10408 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/tests/test_xdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:51.383731 singlestoredb-1.3.1/singlestoredb/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24503 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/utils/convert_rows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/utils/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/utils/mogrify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/utils/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12896 2024-05-23 20:13:29.000000 singlestoredb-1.3.1/singlestoredb/utils/xdict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:13:51.371731 singlestoredb-1.3.1/singlestoredb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-23 20:13:51.000000 singlestoredb-1.3.1/singlestoredb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-23 20:13:51.000000 singlestoredb-1.3.1/singlestoredb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:13:51.000000 singlestoredb-1.3.1/singlestoredb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-23 20:13:51.000000 singlestoredb-1.3.1/singlestoredb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-23 20:13:51.000000 singlestoredb-1.3.1/singlestoredb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-23 20:13:51.000000 singlestoredb-1.3.1/singlestoredb.egg-info/top_level.txt
```

### Comparing `singlestoredb-1.3.0/LICENSE` & `singlestoredb-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/PKG-INFO` & `singlestoredb-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singlestoredb
-Version: 1.3.0
+Version: 1.3.1
 Summary: Interface to the SingleStoreDB database and workspace management APIs
 Home-page: https://github.com/singlestore-labs/singlestoredb-python
 Author: SingleStore
 Author-email: support@singlestore.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `singlestoredb-1.3.0/README.md` & `singlestoredb-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/accel.c` & `singlestoredb-1.3.1/accel.c`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/setup.cfg` & `singlestoredb-1.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = singlestoredb
-version = 1.3.0
+version = 1.3.1
 description = Interface to the SingleStoreDB database and workspace management APIs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/singlestore-labs/singlestoredb-python
 author = SingleStore
 author_email = support@singlestore.com
 license = Apache-2.0
```

### Comparing `singlestoredb-1.3.0/setup.py` & `singlestoredb-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/__init__.py` & `singlestoredb-1.3.1/singlestoredb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 >>> cur = conn.cursor()
 >>> cur.execute('select * from customers')
 >>> for row in cur:
 ...     print(row)
 
 """
 
-__version__ = '1.3.0'
+__version__ = '1.3.1'
 
 from typing import Any
 
 from .config import options, get_option, set_option, describe_option
 from .connection import connect, apilevel, threadsafety, paramstyle
 from .exceptions import (
     Warning, Error, InterfaceError, DatabaseError, OperationalError,
```

### Comparing `singlestoredb-1.3.0/singlestoredb/alchemy/__init__.py` & `singlestoredb-1.3.1/singlestoredb/alchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/auth.py` & `singlestoredb-1.3.1/singlestoredb/auth.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/config.py` & `singlestoredb-1.3.1/singlestoredb/config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/connection.py` & `singlestoredb-1.3.1/singlestoredb/connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/converters.py` & `singlestoredb-1.3.1/singlestoredb/converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/exceptions.py` & `singlestoredb-1.3.1/singlestoredb/exceptions.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/functions/decorator.py` & `singlestoredb-1.3.1/singlestoredb/functions/decorator.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/functions/dtypes.py` & `singlestoredb-1.3.1/singlestoredb/functions/dtypes.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/functions/ext/arrow.py` & `singlestoredb-1.3.1/singlestoredb/functions/ext/arrow.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/functions/ext/asgi.py` & `singlestoredb-1.3.1/singlestoredb/functions/ext/asgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -558,24 +558,23 @@
 
             await send(output_handler['response'])
 
         # Handle api reflection
         elif method == 'GET' and path == self.show_create_function_path:
             host = headers.get(b'host', b'localhost:80')
             reflected_url = f'{scope["scheme"]}://{host.decode("utf-8")}/invoke'
-            data_format = 'json' if b'json' in content_type else 'rowdat_1'
 
             syntax = []
             for key, (endpoint, endpoint_info) in self.endpoints.items():
                 if not func_name or key == func_name:
                     syntax.append(
                         signature_to_sql(
                             endpoint_info['signature'],
                             url=self.url or reflected_url,
-                            data_format=data_format,
+                            data_format=self.data_format,
                         ),
                     )
             body = '\n'.join(syntax).encode('utf-8')
 
             await send(self.text_response_dict)
 
         # Path not found
```

### Comparing `singlestoredb-1.3.0/singlestoredb/functions/ext/json.py` & `singlestoredb-1.3.1/singlestoredb/functions/ext/json.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/functions/ext/mmap.py` & `singlestoredb-1.3.1/singlestoredb/functions/ext/mmap.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/functions/ext/rowdat_1.py` & `singlestoredb-1.3.1/singlestoredb/functions/ext/rowdat_1.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/functions/ext/utils.py` & `singlestoredb-1.3.1/singlestoredb/functions/ext/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/functions/signature.py` & `singlestoredb-1.3.1/singlestoredb/functions/signature.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/fusion/graphql.py` & `singlestoredb-1.3.1/singlestoredb/fusion/graphql.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/fusion/handler.py` & `singlestoredb-1.3.1/singlestoredb/fusion/handler.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/fusion/handlers/stage.py` & `singlestoredb-1.3.1/singlestoredb/fusion/handlers/stage.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/fusion/handlers/utils.py` & `singlestoredb-1.3.1/singlestoredb/fusion/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/fusion/handlers/workspace.py` & `singlestoredb-1.3.1/singlestoredb/fusion/handlers/workspace.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/fusion/registry.py` & `singlestoredb-1.3.1/singlestoredb/fusion/registry.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/fusion/result.py` & `singlestoredb-1.3.1/singlestoredb/fusion/result.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/http/__init__.py` & `singlestoredb-1.3.1/singlestoredb/http/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/http/connection.py` & `singlestoredb-1.3.1/singlestoredb/http/connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/management/billing_usage.py` & `singlestoredb-1.3.1/singlestoredb/management/billing_usage.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/management/cluster.py` & `singlestoredb-1.3.1/singlestoredb/management/cluster.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/management/manager.py` & `singlestoredb-1.3.1/singlestoredb/management/manager.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/management/organization.py` & `singlestoredb-1.3.1/singlestoredb/management/organization.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,19 +31,19 @@
     of API calls on the :class:`Organization`. See :meth:`Organization.get_secret`.
     """
 
     def __init__(
         self,
         id: str,
         name: str,
-        value: str,
         created_by: str,
         created_at: Union[str, datetime.datetime],
         last_updated_by: str,
         last_updated_at: Union[str, datetime.datetime],
+        value: Optional[str] = None,
         deleted_by: Optional[str] = None,
         deleted_at: Optional[Union[str, datetime.datetime]] = None,
     ):
         # UUID of the secret
         self.id = id
 
         # Name of the secret
@@ -84,19 +84,19 @@
         -------
         :class:`Secret`
 
         """
         out = cls(
             id=obj['secretID'],
             name=obj['name'],
-            value=obj['value'],
             created_by=obj['createdBy'],
             created_at=obj['createdAt'],
             last_updated_by=obj['lastUpdatedBy'],
             last_updated_at=obj['lastUpdatedAt'],
+            value=obj.get('value'),
             deleted_by=obj.get('deletedBy'),
             deleted_at=obj.get('deletedAt'),
         )
 
         return out
 
     def __str__(self) -> str:
```

### Comparing `singlestoredb-1.3.0/singlestoredb/management/region.py` & `singlestoredb-1.3.1/singlestoredb/management/region.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/management/utils.py` & `singlestoredb-1.3.1/singlestoredb/management/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/management/workspace.py` & `singlestoredb-1.3.1/singlestoredb/management/workspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 
 def get_organization() -> Organization:
     """Get the organization."""
     return manage_workspaces().organization
 
 
-def get_secret(name: str) -> str:
+def get_secret(name: str) -> Optional[str]:
     """Get a secret from the organization."""
     return get_organization().get_secret(name).value
 
 
 def get_workspace_group(
     workspace_group: Optional[Union[WorkspaceGroup, str]] = None,
 ) -> WorkspaceGroup:
```

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/__init__.py` & `singlestoredb-1.3.1/singlestoredb/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/_auth.py` & `singlestoredb-1.3.1/singlestoredb/mysql/_auth.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/charset.py` & `singlestoredb-1.3.1/singlestoredb/mysql/charset.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/connection.py` & `singlestoredb-1.3.1/singlestoredb/mysql/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1854,14 +1854,15 @@
         self.options = {
             k: v for k, v in dict(
                 default_converters=converters.decoders,
                 results_type=connection.results_type,
                 parse_json=connection.parse_json,
                 invalid_values=connection.invalid_values,
                 unbuffered=unbuffered,
+                encoding_errors=connection.encoding_errors,
             ).items() if v is not UNSET
         }
         self._read_rowdata_packet = functools.partial(
             _singlestoredb_accel.read_rowdata_packet, self, False,
         )
         self._read_rowdata_packet_unbuffered = functools.partial(
             _singlestoredb_accel.read_rowdata_packet, self, True,
```

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/constants/CLIENT.py` & `singlestoredb-1.3.1/singlestoredb/mysql/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/constants/COMMAND.py` & `singlestoredb-1.3.1/singlestoredb/mysql/constants/COMMAND.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/constants/CR.py` & `singlestoredb-1.3.1/singlestoredb/mysql/constants/CR.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/constants/ER.py` & `singlestoredb-1.3.1/singlestoredb/mysql/constants/ER.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/constants/FIELD_TYPE.py` & `singlestoredb-1.3.1/singlestoredb/mysql/constants/FIELD_TYPE.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/converters.py` & `singlestoredb-1.3.1/singlestoredb/mysql/converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/cursors.py` & `singlestoredb-1.3.1/singlestoredb/mysql/cursors.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/err.py` & `singlestoredb-1.3.1/singlestoredb/mysql/err.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/optionfile.py` & `singlestoredb-1.3.1/singlestoredb/mysql/optionfile.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/protocol.py` & `singlestoredb-1.3.1/singlestoredb/mysql/protocol.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/tests/__init__.py` & `singlestoredb-1.3.1/singlestoredb/mysql/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/tests/base.py` & `singlestoredb-1.3.1/singlestoredb/mysql/tests/base.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/tests/conftest.py` & `singlestoredb-1.3.1/singlestoredb/mysql/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/tests/test_DictCursor.py` & `singlestoredb-1.3.1/singlestoredb/mysql/tests/test_DictCursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/tests/test_SSCursor.py` & `singlestoredb-1.3.1/singlestoredb/mysql/tests/test_SSCursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/tests/test_basic.py` & `singlestoredb-1.3.1/singlestoredb/mysql/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/tests/test_connection.py` & `singlestoredb-1.3.1/singlestoredb/mysql/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/tests/test_converters.py` & `singlestoredb-1.3.1/singlestoredb/mysql/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/tests/test_cursor.py` & `singlestoredb-1.3.1/singlestoredb/mysql/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/tests/test_issues.py` & `singlestoredb-1.3.1/singlestoredb/mysql/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/tests/test_load_local.py` & `singlestoredb-1.3.1/singlestoredb/mysql/tests/test_load_local.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/tests/test_nextset.py` & `singlestoredb-1.3.1/singlestoredb/mysql/tests/test_nextset.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/tests/test_optionfile.py` & `singlestoredb-1.3.1/singlestoredb/mysql/tests/test_optionfile.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py` & `singlestoredb-1.3.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py` & `singlestoredb-1.3.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py` & `singlestoredb-1.3.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py` & `singlestoredb-1.3.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py` & `singlestoredb-1.3.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/notebook/_objects.py` & `singlestoredb-1.3.1/singlestoredb/notebook/_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/env python
 import functools
 from typing import Any
+from typing import Optional
 
 from ..management import workspace as _ws
 
 
 class Secrets(object):
     """Wrapper for accessing secrets as object attributes."""
 
-    def __getattr__(self, name: str) -> str:
+    def __getattr__(self, name: str) -> Optional[str]:
         if name.startswith('_ipython') or name.startswith('_repr_'):
             raise AttributeError(name)
         return _ws.get_secret(name)
 
-    def __getitem__(self, name: str) -> str:
+    def __getitem__(self, name: str) -> Optional[str]:
         return _ws.get_secret(name)
 
 
 class Stage(object):
 
     def __new__(cls, *args: Any, **kwargs: Any) -> Any:
         # We are remapping the methods and attributes here so that
```

### Comparing `singlestoredb-1.3.0/singlestoredb/pytest.py` & `singlestoredb-1.3.1/singlestoredb/pytest.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/tests/ext_funcs/__init__.py` & `singlestoredb-1.3.1/singlestoredb/tests/ext_funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/tests/test.sql` & `singlestoredb-1.3.1/singlestoredb/tests/test.sql`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/tests/test_basics.py` & `singlestoredb-1.3.1/singlestoredb/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/tests/test_config.py` & `singlestoredb-1.3.1/singlestoredb/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/tests/test_connection.py` & `singlestoredb-1.3.1/singlestoredb/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/tests/test_dbapi.py` & `singlestoredb-1.3.1/singlestoredb/tests/test_dbapi.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/tests/test_exceptions.py` & `singlestoredb-1.3.1/singlestoredb/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/tests/test_ext_func.py` & `singlestoredb-1.3.1/singlestoredb/tests/test_ext_func.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/tests/test_ext_func_data.py` & `singlestoredb-1.3.1/singlestoredb/tests/test_ext_func_data.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/tests/test_fusion.py` & `singlestoredb-1.3.1/singlestoredb/tests/test_fusion.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/tests/test_http.py` & `singlestoredb-1.3.1/singlestoredb/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/tests/test_management.py` & `singlestoredb-1.3.1/singlestoredb/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/tests/test_plugin.py` & `singlestoredb-1.3.1/singlestoredb/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/tests/test_results.py` & `singlestoredb-1.3.1/singlestoredb/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/tests/test_types.py` & `singlestoredb-1.3.1/singlestoredb/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/tests/test_udf.py` & `singlestoredb-1.3.1/singlestoredb/tests/test_udf.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/tests/test_xdict.py` & `singlestoredb-1.3.1/singlestoredb/tests/test_xdict.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/tests/utils.py` & `singlestoredb-1.3.1/singlestoredb/tests/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/types.py` & `singlestoredb-1.3.1/singlestoredb/types.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/utils/config.py` & `singlestoredb-1.3.1/singlestoredb/utils/config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/utils/convert_rows.py` & `singlestoredb-1.3.1/singlestoredb/utils/convert_rows.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/utils/dtypes.py` & `singlestoredb-1.3.1/singlestoredb/utils/dtypes.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/utils/mogrify.py` & `singlestoredb-1.3.1/singlestoredb/utils/mogrify.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/utils/results.py` & `singlestoredb-1.3.1/singlestoredb/utils/results.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb/utils/xdict.py` & `singlestoredb-1.3.1/singlestoredb/utils/xdict.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.3.0/singlestoredb.egg-info/PKG-INFO` & `singlestoredb-1.3.1/singlestoredb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singlestoredb
-Version: 1.3.0
+Version: 1.3.1
 Summary: Interface to the SingleStoreDB database and workspace management APIs
 Home-page: https://github.com/singlestore-labs/singlestoredb-python
 Author: SingleStore
 Author-email: support@singlestore.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `singlestoredb-1.3.0/singlestoredb.egg-info/SOURCES.txt` & `singlestoredb-1.3.1/singlestoredb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

