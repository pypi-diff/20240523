# Comparing `tmp/python-cloudkittyclient-5.0.0.tar.gz` & `tmp/python-cloudkittyclient-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-cloudkittyclient-5.0.0.tar", last modified: Thu Feb 29 13:19:24 2024, max compression
+gzip compressed data, was "python-cloudkittyclient-5.1.0.tar", last modified: Thu May 23 08:00:06 2024, max compression
```

## Comparing `python-cloudkittyclient-5.0.0.tar` & `python-cloudkittyclient-5.1.0.tar`

### file list

```diff
@@ -1,177 +1,179 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.056728 python-cloudkittyclient-5.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1928 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2570 2024-02-29 13:19:23.000000 python-cloudkittyclient-5.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      667 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7649 2024-02-29 13:19:23.000000 python-cloudkittyclient-5.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1791 2024-02-29 13:19:24.056728 python-cloudkittyclient-5.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      632 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.044728 python-cloudkittyclient-5.0.0/cloudkittyclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1571 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.044728 python-cloudkittyclient-5.0.0/cloudkittyclient/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2543 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/common/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1540 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/common/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3173 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/exc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3204 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/format.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1527 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/osc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5633 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.044728 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.044728 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3395 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.044728 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2419 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v1/test_collector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13022 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v1/test_hashmap.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1622 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v1/test_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2171 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v1/test_pyscripts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1677 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v1/test_rating.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1509 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v1/test_report.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v1/test_storage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.044728 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5844 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v2/test_dataframes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1492 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v2/test_scope.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1257 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v2/test_summary.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.044728 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.044728 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1584 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v1/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2911 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v1/test_collector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13514 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v1/test_hashmap.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1191 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v1/test_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2884 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v1/test_pyscripts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1788 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v1/test_rating.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2685 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v1/test_report.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2299 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v1/test_report_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1337 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v1/test_storage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.048728 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1247 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v2/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6032 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v2/test_dataframes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1401 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v2/test_rating.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3114 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v2/test_scope.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1503 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v2/test_summary.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1353 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/tests/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2956 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.048728 python-cloudkittyclient-5.0.0/cloudkittyclient/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1598 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v1/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4374 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v1/collector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5278 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v1/collector_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1357 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v1/info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2195 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v1/info_cli.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.048728 python-cloudkittyclient-5.0.0/cloudkittyclient/v1/rating/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5766 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v1/rating/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17967 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v1/rating/hashmap.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20514 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v1/rating/hashmap_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3287 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v1/rating/pyscripts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4232 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v1/rating/pyscripts_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2848 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v1/report.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5390 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v1/report_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1385 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v1/storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2760 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v1/storage_cli.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.048728 python-cloudkittyclient-5.0.0/cloudkittyclient/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1732 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v2/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2654 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v2/dataframes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4282 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v2/dataframes_cli.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.048728 python-cloudkittyclient-5.0.0/cloudkittyclient/v2/rating/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v2/rating/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2165 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v2/rating/modules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1026 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v2/rating/modules_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2862 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v2/reprocessing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4021 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v2/reprocessing_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5415 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v2/scope.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4437 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v2/scope_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2116 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v2/summary.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2681 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/cloudkittyclient/v2/summary_cli.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.048728 python-cloudkittyclient-5.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.048728 python-cloudkittyclient-5.0.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.048728 python-cloudkittyclient-5.0.0/doc/source/api_reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/doc/source/api_reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.052728 python-cloudkittyclient-5.0.0/doc/source/api_reference/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/doc/source/api_reference/v1/collector.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/doc/source/api_reference/v1/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/doc/source/api_reference/v1/info.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/doc/source/api_reference/v1/rating.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/doc/source/api_reference/v1/report.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/doc/source/api_reference/v1/storage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.052728 python-cloudkittyclient-5.0.0/doc/source/api_reference/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/doc/source/api_reference/v2/dataframes.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/doc/source/api_reference/v2/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/doc/source/api_reference/v2/scope.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/doc/source/api_reference/v2/summary.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/doc/source/cli_reference.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3419 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.052728 python-cloudkittyclient-5.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1970 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/doc/source/install.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5942 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/doc/source/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.040727 python-cloudkittyclient-5.0.0/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.052728 python-cloudkittyclient-5.0.0/etc/cloudkitty/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/etc/cloudkitty/csv_config.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/etc/cloudkitty/legacy_csv_config.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.040727 python-cloudkittyclient-5.0.0/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.052728 python-cloudkittyclient-5.0.0/playbooks/cloudkittyclient-devstack-functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/playbooks/cloudkittyclient-devstack-functional/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/playbooks/cloudkittyclient-devstack-functional/pre.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/playbooks/cloudkittyclient-devstack-functional/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.052728 python-cloudkittyclient-5.0.0/python_cloudkittyclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1791 2024-02-29 13:19:23.000000 python-cloudkittyclient-5.0.0/python_cloudkittyclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5501 2024-02-29 13:19:24.000000 python-cloudkittyclient-5.0.0/python_cloudkittyclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-29 13:19:23.000000 python-cloudkittyclient-5.0.0/python_cloudkittyclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16185 2024-02-29 13:19:23.000000 python-cloudkittyclient-5.0.0/python_cloudkittyclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-29 13:19:23.000000 python-cloudkittyclient-5.0.0/python_cloudkittyclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-02-29 13:19:23.000000 python-cloudkittyclient-5.0.0/python_cloudkittyclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2024-02-29 13:19:23.000000 python-cloudkittyclient-5.0.0/python_cloudkittyclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-02-29 13:19:23.000000 python-cloudkittyclient-5.0.0/python_cloudkittyclient.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.040727 python-cloudkittyclient-5.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.052728 python-cloudkittyclient-5.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/notes/adapt-client-to-v2-api-c870d5ca49af6341.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/notes/add-patch-scope-support-04c408f982d7d352.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/notes/add-reprocess-api-support-dafc30d0d08a34fd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/notes/add-support-v2-dataframes-baa398fe5ea1b891.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/notes/add-support-v2-dataframes-be3a17271f3c7188.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/notes/add-support-v2-summary-7c1ff903f21f057b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/notes/drop-py27-27ea9fb3e40d4987.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/notes/fix-create_threshold-method-validation-f193e883e82214c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/notes/fix-get-quotation-1d2c18a979f85fe6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/notes/fix-zero-cost-mapping-7a4247cf1c6815f8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1426 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/notes/rewrite-client-5e99a6d3c7302630.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.056728 python-cloudkittyclient-5.0.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.056728 python-cloudkittyclient-5.0.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:19:24.056728 python-cloudkittyclient-5.0.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8195 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      703 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17401 2024-02-29 13:19:24.056728 python-cloudkittyclient-5.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2687 2024-02-29 13:18:53.000000 python-cloudkittyclient-5.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.048485 python-cloudkittyclient-5.1.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1928 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2602 2024-05-23 08:00:05.000000 python-cloudkittyclient-5.1.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      667 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7911 2024-05-23 08:00:05.000000 python-cloudkittyclient-5.1.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1791 2024-05-23 08:00:06.048485 python-cloudkittyclient-5.1.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      632 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.024483 python-cloudkittyclient-5.1.0/cloudkittyclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1571 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.024483 python-cloudkittyclient-5.1.0/cloudkittyclient/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2543 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/common/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1540 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/common/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3173 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/exc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3204 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/format.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1527 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/osc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5633 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.024483 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.024483 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3395 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.024483 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2419 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v1/test_collector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13022 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v1/test_hashmap.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1622 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v1/test_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2171 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v1/test_pyscripts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1677 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v1/test_rating.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1509 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v1/test_report.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v1/test_storage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.028483 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5844 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v2/test_dataframes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1492 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v2/test_scope.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1257 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v2/test_summary.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.028483 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.028483 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1584 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v1/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2911 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v1/test_collector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13514 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v1/test_hashmap.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1191 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v1/test_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2884 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v1/test_pyscripts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1788 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v1/test_rating.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2685 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v1/test_report.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2299 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v1/test_report_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1337 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v1/test_storage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.028483 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1247 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v2/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6032 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v2/test_dataframes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1401 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v2/test_rating.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3114 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v2/test_scope.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1503 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v2/test_summary.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1353 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/tests/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2956 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.032484 python-cloudkittyclient-5.1.0/cloudkittyclient/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1598 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v1/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4374 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v1/collector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5278 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v1/collector_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1357 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v1/info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2195 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v1/info_cli.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.032484 python-cloudkittyclient-5.1.0/cloudkittyclient/v1/rating/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5766 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v1/rating/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17967 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v1/rating/hashmap.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20514 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v1/rating/hashmap_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3287 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v1/rating/pyscripts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4232 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v1/rating/pyscripts_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2848 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v1/report.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5390 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v1/report_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1385 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v1/storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2760 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v1/storage_cli.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.036484 python-cloudkittyclient-5.1.0/cloudkittyclient/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1732 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v2/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2654 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v2/dataframes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4282 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v2/dataframes_cli.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.036484 python-cloudkittyclient-5.1.0/cloudkittyclient/v2/rating/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v2/rating/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2165 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v2/rating/modules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1026 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v2/rating/modules_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2814 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v2/reprocessing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4021 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v2/reprocessing_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5415 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v2/scope.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4437 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v2/scope_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2116 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v2/summary.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2681 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/cloudkittyclient/v2/summary_cli.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.036484 python-cloudkittyclient-5.1.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.036484 python-cloudkittyclient-5.1.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.036484 python-cloudkittyclient-5.1.0/doc/source/api_reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/doc/source/api_reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.036484 python-cloudkittyclient-5.1.0/doc/source/api_reference/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/doc/source/api_reference/v1/collector.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/doc/source/api_reference/v1/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/doc/source/api_reference/v1/info.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/doc/source/api_reference/v1/rating.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/doc/source/api_reference/v1/report.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/doc/source/api_reference/v1/storage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.040484 python-cloudkittyclient-5.1.0/doc/source/api_reference/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/doc/source/api_reference/v2/dataframes.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/doc/source/api_reference/v2/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/doc/source/api_reference/v2/scope.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/doc/source/api_reference/v2/summary.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/doc/source/cli_reference.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3419 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.040484 python-cloudkittyclient-5.1.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1970 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/doc/source/install.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5942 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/doc/source/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.016482 python-cloudkittyclient-5.1.0/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.040484 python-cloudkittyclient-5.1.0/etc/cloudkitty/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/etc/cloudkitty/csv_config.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/etc/cloudkitty/legacy_csv_config.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.016482 python-cloudkittyclient-5.1.0/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.040484 python-cloudkittyclient-5.1.0/playbooks/cloudkittyclient-devstack-functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/playbooks/cloudkittyclient-devstack-functional/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/playbooks/cloudkittyclient-devstack-functional/pre.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/playbooks/cloudkittyclient-devstack-functional/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.040484 python-cloudkittyclient-5.1.0/python_cloudkittyclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1791 2024-05-23 08:00:05.000000 python-cloudkittyclient-5.1.0/python_cloudkittyclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5603 2024-05-23 08:00:06.000000 python-cloudkittyclient-5.1.0/python_cloudkittyclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:00:05.000000 python-cloudkittyclient-5.1.0/python_cloudkittyclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16185 2024-05-23 08:00:05.000000 python-cloudkittyclient-5.1.0/python_cloudkittyclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:00:05.000000 python-cloudkittyclient-5.1.0/python_cloudkittyclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-23 08:00:05.000000 python-cloudkittyclient-5.1.0/python_cloudkittyclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2024-05-23 08:00:05.000000 python-cloudkittyclient-5.1.0/python_cloudkittyclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-05-23 08:00:05.000000 python-cloudkittyclient-5.1.0/python_cloudkittyclient.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.016482 python-cloudkittyclient-5.1.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.044485 python-cloudkittyclient-5.1.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/notes/adapt-client-to-v2-api-c870d5ca49af6341.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/notes/add-patch-scope-support-04c408f982d7d352.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/notes/add-reprocess-api-support-dafc30d0d08a34fd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/notes/add-support-v2-dataframes-baa398fe5ea1b891.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/notes/add-support-v2-dataframes-be3a17271f3c7188.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/notes/add-support-v2-summary-7c1ff903f21f057b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/notes/drop-py27-27ea9fb3e40d4987.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/notes/fix-create_threshold-method-validation-f193e883e82214c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/notes/fix-get-quotation-1d2c18a979f85fe6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/notes/fix-reprocessing-post-request-95512686754ee271.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/notes/fix-zero-cost-mapping-7a4247cf1c6815f8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1426 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/notes/rewrite-client-5e99a6d3c7302630.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.048485 python-cloudkittyclient-5.1.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/source/2023.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/source/2024.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.048485 python-cloudkittyclient-5.1.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:00:06.048485 python-cloudkittyclient-5.1.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8195 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      703 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17401 2024-05-23 08:00:06.052485 python-cloudkittyclient-5.1.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2687 2024-05-23 07:59:37.000000 python-cloudkittyclient-5.1.0/tox.ini
```

### Comparing `python-cloudkittyclient-5.0.0/.zuul.yaml` & `python-cloudkittyclient-5.1.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/AUTHORS` & `python-cloudkittyclient-5.1.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 HaiJieZhang <zhanghj@gohighsec.com>
 Jeremy Liu <liujiong@gohighsec.com>
 Jeremy Stanley <fungi@yuggoth.org>
 Justin Ferrieu <jferrieu@objectif-libre.com>
 Kiran_totad <kiran.totad@nectechnologies.in>
 Luka Peschke <luka.peschke@epitech.eu>
 Luka Peschke <luka.peschke@objectif-libre.com>
+Matt Crees <mattc@stackhpc.com>
 Matthias Bastian <bastian@strato.de>
 Maxime Cottret <maxime.cottret@objectif-libre.com>
 Monty Taylor <mordred@inaugust.com>
 OpenStack Release Bot <infra-root@openstack.org>
 Pierre Riteau <pierre@stackhpc.com>
 Pierre-Alexandre Bardina <pa.bardina@objectif-libre.com>
 Quentin Anglade <quentin.anglade@objectif-libre.com>
```

### Comparing `python-cloudkittyclient-5.0.0/CONTRIBUTING.rst` & `python-cloudkittyclient-5.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/ChangeLog` & `python-cloudkittyclient-5.1.0/ChangeLog`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 CHANGES
 =======
 
+5.1.0
+-----
+
+* reno: Update master for unmaintained/zed
+* Fix reprocessing POST request
+* Update master for stable/2024.1
+* reno: Update master for unmaintained/xena
+* reno: Update master for unmaintained/wallaby
+* reno: Update master for unmaintained/victoria
+
 5.0.0
 -----
 
 * reno: Update master for unmaintained/yoga
 * Update python classifier in setup.cfg
 * Update master for stable/2023.2
```

### Comparing `python-cloudkittyclient-5.0.0/LICENSE` & `python-cloudkittyclient-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/PKG-INFO` & `python-cloudkittyclient-5.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-cloudkittyclient
-Version: 5.0.0
+Version: 5.1.0
 Summary: API client of cloudkitty, Rating as a Service project.
 Home-page: https://docs.openstack.org/python-cloudkittyclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ================
         CloudKittyClient
```

### Comparing `python-cloudkittyclient-5.0.0/README.rst` & `python-cloudkittyclient-5.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/__init__.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/auth.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/auth.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/client.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/client.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/common/base.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/common/base.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/common/client.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/common/client.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/exc.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/exc.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/format.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/format.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/osc.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/osc.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/shell.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/shell.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/base.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v1/test_collector.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v1/test_collector.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v1/test_hashmap.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v1/test_hashmap.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v1/test_info.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v1/test_info.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v1/test_pyscripts.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v1/test_pyscripts.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v1/test_rating.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v1/test_rating.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v1/test_report.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v1/test_report.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v1/test_storage.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v1/test_storage.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v2/test_dataframes.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v2/test_dataframes.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v2/test_scope.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v2/test_scope.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/functional/v2/test_summary.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/functional/v2/test_summary.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v1/base.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v1/base.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v1/test_collector.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v1/test_collector.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v1/test_hashmap.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v1/test_hashmap.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v1/test_info.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v1/test_info.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v1/test_pyscripts.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v1/test_pyscripts.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v1/test_rating.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v1/test_rating.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v1/test_report.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v1/test_report.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v1/test_report_cli.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v1/test_report_cli.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v1/test_storage.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v1/test_storage.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v2/base.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v2/base.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v2/test_dataframes.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v2/test_dataframes.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v2/test_rating.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v2/test_rating.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v2/test_scope.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v2/test_scope.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/unit/v2/test_summary.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/unit/v2/test_summary.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/tests/utils.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/tests/utils.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/utils.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/utils.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v1/client.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v1/client.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v1/collector.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v1/collector.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v1/collector_cli.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v1/collector_cli.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v1/info.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v1/info.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v1/info_cli.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v1/info_cli.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v1/rating/__init__.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v1/rating/__init__.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v1/rating/hashmap.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v1/rating/hashmap.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v1/rating/hashmap_cli.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v1/rating/hashmap_cli.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v1/rating/pyscripts.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v1/rating/pyscripts.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v1/rating/pyscripts_cli.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v1/rating/pyscripts_cli.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v1/report.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v1/report.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v1/report_cli.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v1/report_cli.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v1/storage.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v1/storage.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v1/storage_cli.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v1/storage_cli.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v2/client.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v2/client.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v2/dataframes.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v2/dataframes.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v2/dataframes_cli.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v2/dataframes_cli.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v2/rating/modules.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v2/rating/modules.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v2/rating/modules_cli.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v2/rating/modules_cli.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v2/reprocessing.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v2/reprocessing.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 
 
 class ReprocessingManager(base.BaseManager):
     """Class used to handle /v2/task/reprocesses endpoint"""
 
     url = '/v2/task/reprocesses'
 
-    url_to_post = '/v2/task/reprocess'
-
     def get_reprocessing_tasks(self, offset=0, limit=100, scope_ids=[],
                                order="DESC", **kwargs):
         """Returns a paginated list of reprocessing tasks.
 
         Some optional filters can be provided.
 
         :param offset: Index of the first reprocessing task
@@ -71,8 +69,8 @@
             start_reprocess_time=start,
             end_reprocess_time=end,
             reason=reason
         )
 
         body = dict(filter(lambda elem: bool(elem[1]), body.items()))
 
-        return self.api_client.post(self.url_to_post, json=body).json()
+        return self.api_client.post(self.url, json=body).json()
```

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v2/reprocessing_cli.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v2/reprocessing_cli.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v2/scope.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v2/scope.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v2/scope_cli.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v2/scope_cli.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v2/summary.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v2/summary.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/cloudkittyclient/v2/summary_cli.py` & `python-cloudkittyclient-5.1.0/cloudkittyclient/v2/summary_cli.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/doc/source/conf.py` & `python-cloudkittyclient-5.1.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/doc/source/contributor/contributing.rst` & `python-cloudkittyclient-5.1.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/doc/source/index.rst` & `python-cloudkittyclient-5.1.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/doc/source/usage.rst` & `python-cloudkittyclient-5.1.0/doc/source/usage.rst`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/etc/cloudkitty/legacy_csv_config.yml` & `python-cloudkittyclient-5.1.0/etc/cloudkitty/legacy_csv_config.yml`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/python_cloudkittyclient.egg-info/PKG-INFO` & `python-cloudkittyclient-5.1.0/python_cloudkittyclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-cloudkittyclient
-Version: 5.0.0
+Version: 5.1.0
 Summary: API client of cloudkitty, Rating as a Service project.
 Home-page: https://docs.openstack.org/python-cloudkittyclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ================
         CloudKittyClient
```

### Comparing `python-cloudkittyclient-5.0.0/python_cloudkittyclient.egg-info/SOURCES.txt` & `python-cloudkittyclient-5.1.0/python_cloudkittyclient.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -121,18 +121,20 @@
 releasenotes/notes/add-reprocess-api-support-dafc30d0d08a34fd.yaml
 releasenotes/notes/add-support-v2-dataframes-baa398fe5ea1b891.yaml
 releasenotes/notes/add-support-v2-dataframes-be3a17271f3c7188.yaml
 releasenotes/notes/add-support-v2-summary-7c1ff903f21f057b.yaml
 releasenotes/notes/drop-py27-27ea9fb3e40d4987.yaml
 releasenotes/notes/fix-create_threshold-method-validation-f193e883e82214c9.yaml
 releasenotes/notes/fix-get-quotation-1d2c18a979f85fe6.yaml
+releasenotes/notes/fix-reprocessing-post-request-95512686754ee271.yaml
 releasenotes/notes/fix-zero-cost-mapping-7a4247cf1c6815f8.yaml
 releasenotes/notes/rewrite-client-5e99a6d3c7302630.yaml
 releasenotes/source/2023.1.rst
 releasenotes/source/2023.2.rst
+releasenotes/source/2024.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
 releasenotes/source/stein.rst
 releasenotes/source/train.rst
 releasenotes/source/unreleased.rst
```

### Comparing `python-cloudkittyclient-5.0.0/python_cloudkittyclient.egg-info/entry_points.txt` & `python-cloudkittyclient-5.1.0/python_cloudkittyclient.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/releasenotes/notes/rewrite-client-5e99a6d3c7302630.yaml` & `python-cloudkittyclient-5.1.0/releasenotes/notes/rewrite-client-5e99a6d3c7302630.yaml`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/releasenotes/source/conf.py` & `python-cloudkittyclient-5.1.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/requirements.txt` & `python-cloudkittyclient-5.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/setup.cfg` & `python-cloudkittyclient-5.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/setup.py` & `python-cloudkittyclient-5.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/test-requirements.txt` & `python-cloudkittyclient-5.1.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `python-cloudkittyclient-5.0.0/tox.ini` & `python-cloudkittyclient-5.1.0/tox.ini`

 * *Files identical despite different names*

