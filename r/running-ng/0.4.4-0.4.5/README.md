# Comparing `tmp/running-ng-0.4.4.tar.gz` & `tmp/running_ng-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "running-ng-0.4.4.tar", last modified: Thu Nov 23 01:04:45 2023, max compression
+gzip compressed data, was "running_ng-0.4.5.tar", last modified: Thu May 23 03:33:13 2024, max compression
```

## Comparing `running-ng-0.4.4.tar` & `running_ng-0.4.5.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-11-23 01:04:45.150179 running-ng-0.4.4/
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-11-23 01:04:45.136914 running-ng-0.4.4/.github/
--rw-r--r--   0 caizixian   (501) staff       (20)      106 2021-10-11 12:28:38.000000 running-ng-0.4.4/.github/dependabot.yml
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-11-23 01:04:45.137458 running-ng-0.4.4/.github/workflows/
--rw-r--r--   0 caizixian   (501) staff       (20)      470 2022-02-20 06:52:54.000000 running-ng-0.4.4/.github/workflows/mdbook.yml
--rw-r--r--   0 caizixian   (501) staff       (20)     1801 2023-11-20 11:11:19.000000 running-ng-0.4.4/.github/workflows/python.yml
--rw-r--r--   0 caizixian   (501) staff       (20)     1818 2023-11-20 12:33:42.000000 running-ng-0.4.4/.gitignore
--rw-r--r--   0 caizixian   (501) staff       (20)    11357 2022-02-20 06:52:54.000000 running-ng-0.4.4/LICENSE
--rw-r--r--   0 caizixian   (501) staff       (20)     1832 2023-11-23 01:04:45.149945 running-ng-0.4.4/PKG-INFO
--rw-r--r--   0 caizixian   (501) staff       (20)      954 2022-10-12 05:14:15.000000 running-ng-0.4.4/README.md
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-11-23 01:04:45.137968 running-ng-0.4.4/docs/
--rw-r--r--   0 caizixian   (501) staff       (20)        5 2021-10-11 12:28:38.000000 running-ng-0.4.4/docs/.gitignore
--rw-r--r--   0 caizixian   (501) staff       (20)      116 2021-10-11 12:28:38.000000 running-ng-0.4.4/docs/book.toml
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-11-23 01:04:45.139380 running-ng-0.4.4/docs/src/
--rw-r--r--   0 caizixian   (501) staff       (20)      689 2021-11-06 11:26:31.000000 running-ng-0.4.4/docs/src/SUMMARY.md
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-11-23 01:04:45.139820 running-ng-0.4.4/docs/src/basics/
--rw-r--r--   0 caizixian   (501) staff       (20)     1619 2021-11-06 11:26:31.000000 running-ng-0.4.4/docs/src/basics/design.md
--rw-r--r--   0 caizixian   (501) staff       (20)      221 2021-10-11 12:28:38.000000 running-ng-0.4.4/docs/src/basics/index.md
--rw-r--r--   0 caizixian   (501) staff       (20)    10766 2023-11-23 01:04:09.000000 running-ng-0.4.4/docs/src/changelog.md
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-11-23 01:04:45.140811 running-ng-0.4.4/docs/src/commands/
--rw-r--r--   0 caizixian   (501) staff       (20)       11 2021-10-11 12:28:38.000000 running-ng-0.4.4/docs/src/commands/fillin.md
--rw-r--r--   0 caizixian   (501) staff       (20)      878 2021-11-06 11:26:31.000000 running-ng-0.4.4/docs/src/commands/index.md
--rw-r--r--   0 caizixian   (501) staff       (20)     2389 2022-02-16 02:25:49.000000 running-ng-0.4.4/docs/src/commands/minheap.md
--rw-r--r--   0 caizixian   (501) staff       (20)     6311 2023-11-20 06:04:52.000000 running-ng-0.4.4/docs/src/commands/runbms.md
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-11-23 01:04:45.141223 running-ng-0.4.4/docs/src/cookbook/
--rw-r--r--   0 caizixian   (501) staff       (20)       40 2021-11-06 11:26:31.000000 running-ng-0.4.4/docs/src/cookbook/index.md
--rw-r--r--   0 caizixian   (501) staff       (20)     4650 2023-07-25 06:10:45.000000 running-ng-0.4.4/docs/src/cookbook/perf_events.md
--rw-r--r--   0 caizixian   (501) staff       (20)       29 2021-11-06 11:26:31.000000 running-ng-0.4.4/docs/src/faq.md
--rw-r--r--   0 caizixian   (501) staff       (20)     1429 2022-02-20 07:25:27.000000 running-ng-0.4.4/docs/src/install.md
--rw-r--r--   0 caizixian   (501) staff       (20)     2910 2021-11-06 11:26:31.000000 running-ng-0.4.4/docs/src/intro.md
--rw-r--r--   0 caizixian   (501) staff       (20)     5119 2023-08-16 03:26:37.000000 running-ng-0.4.4/docs/src/quickstart.md
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-11-23 01:04:45.142100 running-ng-0.4.4/docs/src/references/
--rw-r--r--   0 caizixian   (501) staff       (20)     6476 2023-09-10 10:19:13.000000 running-ng-0.4.4/docs/src/references/index.md
--rw-r--r--   0 caizixian   (501) staff       (20)     3171 2023-11-20 12:20:43.000000 running-ng-0.4.4/docs/src/references/modifier.md
--rw-r--r--   0 caizixian   (501) staff       (20)     1062 2023-11-20 12:22:38.000000 running-ng-0.4.4/docs/src/references/runtime.md
--rw-r--r--   0 caizixian   (501) staff       (20)     8435 2023-11-20 12:23:55.000000 running-ng-0.4.4/docs/src/references/suite.md
--rw-r--r--   0 caizixian   (501) staff       (20)     1146 2023-11-20 11:11:19.000000 running-ng-0.4.4/pyproject.toml
--rw-r--r--   0 caizixian   (501) staff       (20)       38 2023-11-23 01:04:45.150218 running-ng-0.4.4/setup.cfg
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-11-23 01:04:45.135931 running-ng-0.4.4/src/
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-11-23 01:04:45.143427 running-ng-0.4.4/src/running/
--rw-r--r--   0 caizixian   (501) staff       (20)        0 2022-02-20 06:52:54.000000 running-ng-0.4.4/src/running/__init__.py
--rw-r--r--   0 caizixian   (501) staff       (20)     1543 2023-11-20 11:11:19.000000 running-ng-0.4.4/src/running/__main__.py
--rw-r--r--   0 caizixian   (501) staff       (20)       62 2023-11-23 01:04:16.000000 running-ng-0.4.4/src/running/__version__.py
--rw-r--r--   0 caizixian   (501) staff       (20)    11760 2023-11-20 11:11:19.000000 running-ng-0.4.4/src/running/benchmark.py
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-11-23 01:04:45.144264 running-ng-0.4.4/src/running/command/
--rw-r--r--   0 caizixian   (501) staff       (20)        0 2022-02-20 06:52:54.000000 running-ng-0.4.4/src/running/command/__init__.py
--rw-r--r--   0 caizixian   (501) staff       (20)     2064 2023-11-20 11:11:19.000000 running-ng-0.4.4/src/running/command/fillin.py
--rw-r--r--   0 caizixian   (501) staff       (20)     2836 2023-11-20 11:11:19.000000 running-ng-0.4.4/src/running/command/genadvice.py
--rw-r--r--   0 caizixian   (501) staff       (20)     7402 2023-11-20 11:11:19.000000 running-ng-0.4.4/src/running/command/log_preprocessor.py
--rw-r--r--   0 caizixian   (501) staff       (20)     7008 2023-11-20 11:11:19.000000 running-ng-0.4.4/src/running/command/minheap.py
--rw-r--r--   0 caizixian   (501) staff       (20)    16984 2023-11-20 11:11:19.000000 running-ng-0.4.4/src/running/command/runbms.py
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-11-23 01:04:45.144689 running-ng-0.4.4/src/running/config/
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-11-23 01:04:45.146908 running-ng-0.4.4/src/running/config/base/
--rw-r--r--   0 caizixian   (501) staff       (20)     4877 2023-11-20 12:10:17.000000 running-ng-0.4.4/src/running/config/base/dacapo.yml
--rw-r--r--   0 caizixian   (501) staff       (20)       28 2022-09-06 03:25:59.000000 running-ng-0.4.4/src/running/config/base/jvms.yml
--rw-r--r--   0 caizixian   (501) staff       (20)       95 2022-02-20 06:52:54.000000 running-ng-0.4.4/src/running/config/base/minheap.yml
--rw-r--r--   0 caizixian   (501) staff       (20)     1022 2023-11-20 12:10:17.000000 running-ng-0.4.4/src/running/config/base/modifiers.yml
--rw-r--r--   0 caizixian   (501) staff       (20)       74 2023-08-16 03:26:37.000000 running-ng-0.4.4/src/running/config/base/runbms-anu.yml
--rw-r--r--   0 caizixian   (501) staff       (20)      248 2023-08-16 03:26:37.000000 running-ng-0.4.4/src/running/config/base/runbms.yml
--rw-r--r--   0 caizixian   (501) staff       (20)      127 2022-02-20 06:52:54.000000 running-ng-0.4.4/src/running/config/base/specjbb2015.yml
--rw-r--r--   0 caizixian   (501) staff       (20)      132 2022-03-19 05:22:35.000000 running-ng-0.4.4/src/running/config/base/specjvm98.yml
--rw-r--r--   0 caizixian   (501) staff       (20)       75 2022-03-19 05:22:35.000000 running-ng-0.4.4/src/running/config/base/suites.yml
--rw-r--r--   0 caizixian   (501) staff       (20)      375 2023-11-20 11:11:19.000000 running-ng-0.4.4/src/running/config/base/temurin.yml
--rw-r--r--   0 caizixian   (501) staff       (20)      214 2022-09-06 03:25:59.000000 running-ng-0.4.4/src/running/config/minheap_example.yml
--rw-r--r--   0 caizixian   (501) staff       (20)      964 2022-09-06 03:25:59.000000 running-ng-0.4.4/src/running/config/runbms_example.yml
--rw-r--r--   0 caizixian   (501) staff       (20)     5744 2023-11-20 11:11:19.000000 running-ng-0.4.4/src/running/config.py
--rw-r--r--   0 caizixian   (501) staff       (20)     5843 2023-11-20 11:11:19.000000 running-ng-0.4.4/src/running/modifier.py
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-11-23 01:04:45.147147 running-ng-0.4.4/src/running/plugin/
--rw-r--r--   0 caizixian   (501) staff       (20)        0 2022-02-20 06:52:54.000000 running-ng-0.4.4/src/running/plugin/__init__.py
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-11-23 01:04:45.147476 running-ng-0.4.4/src/running/plugin/runbms/
--rw-r--r--   0 caizixian   (501) staff       (20)     3004 2023-11-20 11:11:19.000000 running-ng-0.4.4/src/running/plugin/runbms/__init__.py
--rw-r--r--   0 caizixian   (501) staff       (20)     3335 2023-11-20 11:11:19.000000 running-ng-0.4.4/src/running/plugin/runbms/copyfile.py
--rw-r--r--   0 caizixian   (501) staff       (20)     6108 2023-11-20 11:11:19.000000 running-ng-0.4.4/src/running/plugin/runbms/zulip.py
--rw-r--r--   0 caizixian   (501) staff       (20)     7813 2023-11-20 11:11:19.000000 running-ng-0.4.4/src/running/runtime.py
--rw-r--r--   0 caizixian   (501) staff       (20)    18507 2023-11-23 01:02:50.000000 running-ng-0.4.4/src/running/suite.py
--rw-r--r--   0 caizixian   (501) staff       (20)     5112 2023-11-20 11:11:19.000000 running-ng-0.4.4/src/running/util.py
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-11-23 01:04:45.149261 running-ng-0.4.4/src/running_ng.egg-info/
--rw-r--r--   0 caizixian   (501) staff       (20)     1832 2023-11-23 01:04:45.000000 running-ng-0.4.4/src/running_ng.egg-info/PKG-INFO
--rw-r--r--   0 caizixian   (501) staff       (20)     2016 2023-11-23 01:04:45.000000 running-ng-0.4.4/src/running_ng.egg-info/SOURCES.txt
--rw-r--r--   0 caizixian   (501) staff       (20)        1 2023-11-23 01:04:45.000000 running-ng-0.4.4/src/running_ng.egg-info/dependency_links.txt
--rw-r--r--   0 caizixian   (501) staff       (20)       50 2023-11-23 01:04:45.000000 running-ng-0.4.4/src/running_ng.egg-info/entry_points.txt
--rw-r--r--   0 caizixian   (501) staff       (20)       92 2023-11-23 01:04:45.000000 running-ng-0.4.4/src/running_ng.egg-info/requires.txt
--rw-r--r--   0 caizixian   (501) staff       (20)        8 2023-11-23 01:04:45.000000 running-ng-0.4.4/src/running_ng.egg-info/top_level.txt
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-11-23 01:04:45.149090 running-ng-0.4.4/tests/
--rw-r--r--   0 caizixian   (501) staff       (20)     2191 2023-11-20 11:11:19.000000 running-ng-0.4.4/tests/test_config.py
--rw-r--r--   0 caizixian   (501) staff       (20)      644 2023-11-20 11:11:19.000000 running-ng-0.4.4/tests/test_fillin.py
--rw-r--r--   0 caizixian   (501) staff       (20)     1981 2023-11-20 11:11:19.000000 running-ng-0.4.4/tests/test_log_preprocessor.py
--rw-r--r--   0 caizixian   (501) staff       (20)     5017 2023-11-20 11:11:19.000000 running-ng-0.4.4/tests/test_modifier.py
--rw-r--r--   0 caizixian   (501) staff       (20)      464 2023-11-20 11:11:19.000000 running-ng-0.4.4/tests/test_runbms.py
--rw-r--r--   0 caizixian   (501) staff       (20)      950 2023-11-20 11:11:19.000000 running-ng-0.4.4/tests/test_runtime.py
--rw-r--r--   0 caizixian   (501) staff       (20)     3529 2023-11-20 12:10:17.000000 running-ng-0.4.4/tests/test_suite.py
--rw-r--r--   0 caizixian   (501) staff       (20)     1087 2023-11-20 11:11:19.000000 running-ng-0.4.4/tests/test_util.py
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2024-05-23 03:33:13.661544 running_ng-0.4.5/
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2024-05-23 03:33:13.643922 running_ng-0.4.5/.github/
+-rw-r--r--   0 caizixian   (501) staff       (20)      106 2021-10-11 12:28:38.000000 running_ng-0.4.5/.github/dependabot.yml
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2024-05-23 03:33:13.644532 running_ng-0.4.5/.github/workflows/
+-rw-r--r--   0 caizixian   (501) staff       (20)      470 2022-02-20 06:52:54.000000 running_ng-0.4.5/.github/workflows/mdbook.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)     1841 2024-01-06 01:11:45.000000 running_ng-0.4.5/.github/workflows/python.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)     1818 2023-11-20 12:33:42.000000 running_ng-0.4.5/.gitignore
+-rw-r--r--   0 caizixian   (501) staff       (20)    11357 2022-02-20 06:52:54.000000 running_ng-0.4.5/LICENSE
+-rw-r--r--   0 caizixian   (501) staff       (20)     1843 2024-05-23 03:33:13.661270 running_ng-0.4.5/PKG-INFO
+-rw-r--r--   0 caizixian   (501) staff       (20)      954 2022-10-12 05:14:15.000000 running_ng-0.4.5/README.md
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2024-05-23 03:33:13.645048 running_ng-0.4.5/docs/
+-rw-r--r--   0 caizixian   (501) staff       (20)        5 2021-10-11 12:28:38.000000 running_ng-0.4.5/docs/.gitignore
+-rw-r--r--   0 caizixian   (501) staff       (20)      116 2021-10-11 12:28:38.000000 running_ng-0.4.5/docs/book.toml
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2024-05-23 03:33:13.647277 running_ng-0.4.5/docs/src/
+-rw-r--r--   0 caizixian   (501) staff       (20)      689 2021-11-06 11:26:31.000000 running_ng-0.4.5/docs/src/SUMMARY.md
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2024-05-23 03:33:13.648166 running_ng-0.4.5/docs/src/basics/
+-rw-r--r--   0 caizixian   (501) staff       (20)     1619 2021-11-06 11:26:31.000000 running_ng-0.4.5/docs/src/basics/design.md
+-rw-r--r--   0 caizixian   (501) staff       (20)      221 2021-10-11 12:28:38.000000 running_ng-0.4.5/docs/src/basics/index.md
+-rw-r--r--   0 caizixian   (501) staff       (20)    10908 2024-05-23 03:32:45.000000 running_ng-0.4.5/docs/src/changelog.md
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2024-05-23 03:33:13.649260 running_ng-0.4.5/docs/src/commands/
+-rw-r--r--   0 caizixian   (501) staff       (20)       11 2021-10-11 12:28:38.000000 running_ng-0.4.5/docs/src/commands/fillin.md
+-rw-r--r--   0 caizixian   (501) staff       (20)      878 2021-11-06 11:26:31.000000 running_ng-0.4.5/docs/src/commands/index.md
+-rw-r--r--   0 caizixian   (501) staff       (20)     2389 2022-02-16 02:25:49.000000 running_ng-0.4.5/docs/src/commands/minheap.md
+-rw-r--r--   0 caizixian   (501) staff       (20)     6311 2023-11-20 06:04:52.000000 running_ng-0.4.5/docs/src/commands/runbms.md
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2024-05-23 03:33:13.649803 running_ng-0.4.5/docs/src/cookbook/
+-rw-r--r--   0 caizixian   (501) staff       (20)       40 2021-11-06 11:26:31.000000 running_ng-0.4.5/docs/src/cookbook/index.md
+-rw-r--r--   0 caizixian   (501) staff       (20)     4650 2023-07-25 06:10:45.000000 running_ng-0.4.5/docs/src/cookbook/perf_events.md
+-rw-r--r--   0 caizixian   (501) staff       (20)       29 2021-11-06 11:26:31.000000 running_ng-0.4.5/docs/src/faq.md
+-rw-r--r--   0 caizixian   (501) staff       (20)     1429 2022-02-20 07:25:27.000000 running_ng-0.4.5/docs/src/install.md
+-rw-r--r--   0 caizixian   (501) staff       (20)     2910 2021-11-06 11:26:31.000000 running_ng-0.4.5/docs/src/intro.md
+-rw-r--r--   0 caizixian   (501) staff       (20)     5119 2023-08-16 03:26:37.000000 running_ng-0.4.5/docs/src/quickstart.md
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2024-05-23 03:33:13.650916 running_ng-0.4.5/docs/src/references/
+-rw-r--r--   0 caizixian   (501) staff       (20)     6476 2023-09-10 10:19:13.000000 running_ng-0.4.5/docs/src/references/index.md
+-rw-r--r--   0 caizixian   (501) staff       (20)     3650 2024-05-23 03:32:45.000000 running_ng-0.4.5/docs/src/references/modifier.md
+-rw-r--r--   0 caizixian   (501) staff       (20)     1062 2023-11-20 12:22:38.000000 running_ng-0.4.5/docs/src/references/runtime.md
+-rw-r--r--   0 caizixian   (501) staff       (20)     8435 2023-11-20 12:23:55.000000 running_ng-0.4.5/docs/src/references/suite.md
+-rw-r--r--   0 caizixian   (501) staff       (20)     1157 2024-05-23 03:01:52.000000 running_ng-0.4.5/pyproject.toml
+-rw-r--r--   0 caizixian   (501) staff       (20)       38 2024-05-23 03:33:13.661592 running_ng-0.4.5/setup.cfg
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2024-05-23 03:33:13.642289 running_ng-0.4.5/src/
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2024-05-23 03:33:13.653040 running_ng-0.4.5/src/running/
+-rw-r--r--   0 caizixian   (501) staff       (20)        0 2022-02-20 06:52:54.000000 running_ng-0.4.5/src/running/__init__.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     1543 2023-11-20 11:11:19.000000 running_ng-0.4.5/src/running/__main__.py
+-rw-r--r--   0 caizixian   (501) staff       (20)       62 2024-05-23 03:32:45.000000 running_ng-0.4.5/src/running/__version__.py
+-rw-r--r--   0 caizixian   (501) staff       (20)    11769 2024-01-06 01:11:45.000000 running_ng-0.4.5/src/running/benchmark.py
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2024-05-23 03:33:13.654021 running_ng-0.4.5/src/running/command/
+-rw-r--r--   0 caizixian   (501) staff       (20)        0 2022-02-20 06:52:54.000000 running_ng-0.4.5/src/running/command/__init__.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     2064 2023-11-20 11:11:19.000000 running_ng-0.4.5/src/running/command/fillin.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     2836 2023-11-20 11:11:19.000000 running_ng-0.4.5/src/running/command/genadvice.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     7402 2023-11-20 11:11:19.000000 running_ng-0.4.5/src/running/command/log_preprocessor.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     7008 2023-11-20 11:11:19.000000 running_ng-0.4.5/src/running/command/minheap.py
+-rw-r--r--   0 caizixian   (501) staff       (20)    18348 2024-05-23 03:32:45.000000 running_ng-0.4.5/src/running/command/runbms.py
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2024-05-23 03:33:13.654952 running_ng-0.4.5/src/running/config/
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2024-05-23 03:33:13.657634 running_ng-0.4.5/src/running/config/base/
+-rw-r--r--   0 caizixian   (501) staff       (20)     4877 2023-11-20 12:10:17.000000 running_ng-0.4.5/src/running/config/base/dacapo.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)       28 2022-09-06 03:25:59.000000 running_ng-0.4.5/src/running/config/base/jvms.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)       95 2022-02-20 06:52:54.000000 running_ng-0.4.5/src/running/config/base/minheap.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)     1022 2023-11-20 12:10:17.000000 running_ng-0.4.5/src/running/config/base/modifiers.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)       74 2023-08-16 03:26:37.000000 running_ng-0.4.5/src/running/config/base/runbms-anu.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)      248 2023-08-16 03:26:37.000000 running_ng-0.4.5/src/running/config/base/runbms.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)      127 2022-02-20 06:52:54.000000 running_ng-0.4.5/src/running/config/base/specjbb2015.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)      132 2022-03-19 05:22:35.000000 running_ng-0.4.5/src/running/config/base/specjvm98.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)       75 2022-03-19 05:22:35.000000 running_ng-0.4.5/src/running/config/base/suites.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)      375 2023-11-20 11:11:19.000000 running_ng-0.4.5/src/running/config/base/temurin.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)      214 2022-09-06 03:25:59.000000 running_ng-0.4.5/src/running/config/minheap_example.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)      318 2024-05-23 03:32:45.000000 running_ng-0.4.5/src/running/config/runbms_example.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)      964 2024-05-23 03:32:45.000000 running_ng-0.4.5/src/running/config/runbms_example_probes.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)     5744 2023-11-20 11:11:19.000000 running_ng-0.4.5/src/running/config.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     6111 2024-05-23 03:32:45.000000 running_ng-0.4.5/src/running/modifier.py
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2024-05-23 03:33:13.657879 running_ng-0.4.5/src/running/plugin/
+-rw-r--r--   0 caizixian   (501) staff       (20)        0 2022-02-20 06:52:54.000000 running_ng-0.4.5/src/running/plugin/__init__.py
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2024-05-23 03:33:13.658344 running_ng-0.4.5/src/running/plugin/runbms/
+-rw-r--r--   0 caizixian   (501) staff       (20)     3004 2023-11-20 11:11:19.000000 running_ng-0.4.5/src/running/plugin/runbms/__init__.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     3335 2023-11-20 11:11:19.000000 running_ng-0.4.5/src/running/plugin/runbms/copyfile.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     6108 2023-11-20 11:11:19.000000 running_ng-0.4.5/src/running/plugin/runbms/zulip.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     7813 2023-11-20 11:11:19.000000 running_ng-0.4.5/src/running/runtime.py
+-rw-r--r--   0 caizixian   (501) staff       (20)    18400 2024-01-06 01:11:45.000000 running_ng-0.4.5/src/running/suite.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     5438 2024-05-23 03:32:45.000000 running_ng-0.4.5/src/running/util.py
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2024-05-23 03:33:13.660526 running_ng-0.4.5/src/running_ng.egg-info/
+-rw-r--r--   0 caizixian   (501) staff       (20)     1843 2024-05-23 03:33:13.000000 running_ng-0.4.5/src/running_ng.egg-info/PKG-INFO
+-rw-r--r--   0 caizixian   (501) staff       (20)     2061 2024-05-23 03:33:13.000000 running_ng-0.4.5/src/running_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 caizixian   (501) staff       (20)        1 2024-05-23 03:33:13.000000 running_ng-0.4.5/src/running_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 caizixian   (501) staff       (20)       50 2024-05-23 03:33:13.000000 running_ng-0.4.5/src/running_ng.egg-info/entry_points.txt
+-rw-r--r--   0 caizixian   (501) staff       (20)      103 2024-05-23 03:33:13.000000 running_ng-0.4.5/src/running_ng.egg-info/requires.txt
+-rw-r--r--   0 caizixian   (501) staff       (20)        8 2024-05-23 03:33:13.000000 running_ng-0.4.5/src/running_ng.egg-info/top_level.txt
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2024-05-23 03:33:13.660341 running_ng-0.4.5/tests/
+-rw-r--r--   0 caizixian   (501) staff       (20)     2191 2023-11-20 11:11:19.000000 running_ng-0.4.5/tests/test_config.py
+-rw-r--r--   0 caizixian   (501) staff       (20)      644 2023-11-20 11:11:19.000000 running_ng-0.4.5/tests/test_fillin.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     1981 2023-11-20 11:11:19.000000 running_ng-0.4.5/tests/test_log_preprocessor.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     5629 2024-05-23 03:32:45.000000 running_ng-0.4.5/tests/test_modifier.py
+-rw-r--r--   0 caizixian   (501) staff       (20)      464 2023-11-20 11:11:19.000000 running_ng-0.4.5/tests/test_runbms.py
+-rw-r--r--   0 caizixian   (501) staff       (20)      950 2023-11-20 11:11:19.000000 running_ng-0.4.5/tests/test_runtime.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     3529 2023-11-20 12:10:17.000000 running_ng-0.4.5/tests/test_suite.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     1087 2024-05-23 03:03:30.000000 running_ng-0.4.5/tests/test_util.py
```

### Comparing `running-ng-0.4.4/.github/workflows/python.yml` & `running_ng-0.4.5/.github/workflows/python.yml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip setuptools build[virtualenv]
           pip install .[tests]
       - name: Test with pytest
         run: |
-          pytest
+          for f in tests/test_*.py; do pytest "$f"; done
   mypy:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.12"]
 
     steps:
```

### Comparing `running-ng-0.4.4/.gitignore` & `running_ng-0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/LICENSE` & `running_ng-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/PKG-INFO` & `running_ng-0.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: running-ng
-Version: 0.4.4
+Version: 0.4.5
 Summary: Running: Next Generation
 Author-email: Zixian Cai <u5937495@anu.edu.au>
 License: Apache
 Project-URL: Homepage, https://github.com/anupli/running-ng
 Project-URL: Bug Tracker, https://github.com/anupli/running-ng/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -14,17 +14,17 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml~=6.0.1
 Provides-Extra: zulip
 Requires-Dist: zulip~=0.9.0; extra == "zulip"
 Provides-Extra: tests
-Requires-Dist: pytest~=7.4.3; extra == "tests"
+Requires-Dist: pytest<8.3.0,>=7.4.4; extra == "tests"
 Requires-Dist: types-PyYAML~=6.0.12; extra == "tests"
-Requires-Dist: mypy~=1.7.0; extra == "tests"
+Requires-Dist: mypy<1.10,>=1.8; extra == "tests"
 
 # `running-ng`
 `running-ng` is a collection of scripts that help people run workloads in a methodologically sound settings.
 
 ## Installation
 `pip3 install running-ng`
```

### Comparing `running-ng-0.4.4/README.md` & `running_ng-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/docs/src/SUMMARY.md` & `running_ng-0.4.5/docs/src/SUMMARY.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/docs/src/basics/design.md` & `running_ng-0.4.5/docs/src/basics/design.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/docs/src/changelog.md` & `running_ng-0.4.5/docs/src/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 
 ### Removed
 
 ### Fixed
 
 ### Security
 
+## [`v0.4.5` (2024-05-23)](https://github.com/anupli/running-ng/releases/tag/v0.4.5)
+### Added
+#### Modifiers
+- `NoImplicitHeapsizeModifier`
+
 ## [`v0.4.4` (2023-11-23)](https://github.com/anupli/running-ng/releases/tag/v0.4.4)
 ### Fixed
 #### Benchmark Suites
 - `DaCapo` correctly accepts the `23.11` `release` specified in `dacapo.yml`.
 
 ## [`v0.4.3` (2023-11-20)](https://github.com/anupli/running-ng/releases/tag/v0.4.3)
 ### Added
```

### Comparing `running-ng-0.4.4/docs/src/commands/index.md` & `running_ng-0.4.5/docs/src/commands/index.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/docs/src/commands/minheap.md` & `running_ng-0.4.5/docs/src/commands/minheap.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/docs/src/commands/runbms.md` & `running_ng-0.4.5/docs/src/commands/runbms.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/docs/src/cookbook/perf_events.md` & `running_ng-0.4.5/docs/src/cookbook/perf_events.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/docs/src/install.md` & `running_ng-0.4.5/docs/src/install.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/docs/src/intro.md` & `running_ng-0.4.5/docs/src/intro.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/docs/src/quickstart.md` & `running_ng-0.4.5/docs/src/quickstart.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/docs/src/references/index.md` & `running_ng-0.4.5/docs/src/references/index.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/docs/src/references/modifier.md` & `running_ng-0.4.5/docs/src/references/modifier.md`

 * *Files 27% similar despite different names*

```diff
@@ -92,7 +92,18 @@
 
 ## `JuliaArg` (preview ⚠️)
 `JuliaMMTk` and `JuliaStock` specific.
 ### Keys
 `val`: a single string with [shell-like syntax](https://docs.python.org/3/library/shlex.html#shlex.split).
 Multiple arguments are space separated.
 Environment variables will be expanded.
+
+## `NoImplicitHeapsizeModifier` (preview ⚠️)
+`runbms` specific.
+
+### Description
+Normally `runbms` will iterate through a set of heap sizes, either specific multiples of the minheap of each benchmark via `-s`, or spreading the multiples across 1~`heap_range` (using `N` and optionally `ns`).
+
+This modifier prevents `runbms` from applying the heap sizes for certain configs, which is useful, for example, for running `NoGC` or `EpsilonGC`.
+
+### Keys
+No argument is allowed.
```

### Comparing `running-ng-0.4.4/docs/src/references/runtime.md` & `running_ng-0.4.5/docs/src/references/runtime.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/docs/src/references/suite.md` & `running_ng-0.4.5/docs/src/references/suite.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/pyproject.toml` & `running_ng-0.4.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 "Bug Tracker" = "https://github.com/anupli/running-ng/issues"
 
 [project.optional-dependencies]
 zulip = [
     "zulip~=0.9.0"
 ]
 tests = [
-    "pytest~=7.4.3",
+    "pytest>=7.4.4,<8.3.0",
     "types-PyYAML~=6.0.12",
-    "mypy~=1.7.0"
+    "mypy>=1.8,<1.10"
 ]
 
 [project.scripts]
 running = "running.__main__:main"
 
 [tool.setuptools.dynamic]
 version = {attr = "running.__version__.__VERSION__"}
```

### Comparing `running-ng-0.4.4/src/running/__main__.py` & `running_ng-0.4.5/src/running/__main__.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/src/running/benchmark.py` & `running_ng-0.4.5/src/running/benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from time import sleep
 from typing import Callable, Sequence, TypeVar, List, Optional, Tuple, Union, Dict
 from running.runtime import D8, JavaScriptCore, Runtime, DummyRuntime, SpiderMonkey
 from running.modifier import *
 from running.util import smart_quote, split_quoted
 from pathlib import Path
 from copy import deepcopy
-from running import suite
 import os
 from enum import Enum
 
 COMPANION_WAIT_START = 2.0
 
 
 class SubprocessrExit(Enum):
@@ -107,14 +106,16 @@
                 ]
             ),
         )
 
     def run(
         self, runtime: Runtime, cwd: Optional[Path] = None
     ) -> Tuple[bytes, bytes, SubprocessrExit]:
+        from running import suite
+
         if suite.is_dry_run():
             print(self.to_string(runtime), file=sys.stderr)
             return b"", b"", SubprocessrExit.Dryrun
         else:
             cmd = self.get_full_args(runtime)
             cmd = [os.path.expandvars(x) for x in cmd]
             env_args_to_add = {
```

### Comparing `running-ng-0.4.4/src/running/command/fillin.py` & `running_ng-0.4.5/src/running/command/fillin.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/src/running/command/genadvice.py` & `running_ng-0.4.5/src/running/command/genadvice.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/src/running/command/log_preprocessor.py` & `running_ng-0.4.5/src/running/command/log_preprocessor.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/src/running/command/minheap.py` & `running_ng-0.4.5/src/running/command/minheap.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/src/running/command/runbms.py` & `running_ng-0.4.5/src/running/command/runbms.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from pathlib import Path
 from running.util import (
     parse_config_str,
     system,
     get_logged_in_users,
     config_index_to_chr,
     config_str_encode,
+    dont_emit_heapsize_modifier,
 )
 import socket
 from datetime import datetime
 from running.runtime import Runtime
 import tempfile
 import subprocess
 import os
@@ -449,49 +450,81 @@
                 raise TypeError("plugins must be a dictionary")
             plugins = {k: RunbmsPlugin.from_config(k, v) for k, v in plugins.items()}
             for p in plugins.values():
                 p.set_run_id(run_id)
                 p.set_runbms_dir(runbms_dir)
                 p.set_log_dir(log_dir)
 
+        configs_no_heapsize = [
+            c for c in configs if dont_emit_heapsize_modifier(configuration, c)
+        ]
+        configs_with_heapsize = [
+            c for c in configs if not dont_emit_heapsize_modifier(configuration, c)
+        ]
+
+        # Simple case
+        if not slice and N is None:
+            # run all configs without specifying heap size
+            run_one_hfac(
+                invocations,
+                None,  # not specifying heap size
+                suites,
+                benchmarks,
+                configs,
+                Path(runbms_dir),
+                log_dir,
+            )
+            # early return
+            return True
+
+        # In all other cases, we will first run configs that don't want
+        # implicit heapsize modifiers
+        logging.info("Running all configs with NoImplicitHeapSizeModifier set")
+        run_one_hfac(
+            invocations,
+            None,  # not specifying heap size
+            suites,
+            benchmarks,
+            configs_no_heapsize,
+            Path(runbms_dir),
+            log_dir,
+        )
+
+        # Helper function for running benchmarks using multiple heap factors
         def run_hfacs(hfacs):
             logging.info(
                 "hfacs: {}".format(", ".join([hfac_str(hfac) for hfac in hfacs]))
             )
             for hfac in hfacs:
                 run_one_hfac(
                     invocations,
                     hfac,
                     suites,
                     benchmarks,
-                    configs,
+                    configs_with_heapsize,
                     Path(runbms_dir),
                     log_dir,
                 )
                 print()
 
+        # Helper function for using the heap factor spreading algorithm
         def run_N_ns(N, ns):
             hfacs = get_hfacs(heap_range, spread_factor, N, ns)
             run_hfacs(hfacs)
 
-        if slice:
+        if slice:  # specified -s, we respect that first
+            if N is not None:
+                logging.warning(
+                    "You specified both N={} and -s {}, N is ignored.".format(
+                        N,
+                        ",".join([str(s) for s in slice]),
+                    )
+                )
             run_hfacs(slice)
-            return True
-
-        if N is None:
-            run_one_hfac(
-                invocations,
-                None,
-                suites,
-                benchmarks,
-                configs,
-                Path(runbms_dir),
-                log_dir,
-            )
-            return True
-
-        if len(ns) == 0:
-            fillin(run_N_ns, round(math.log2(N)))
         else:
-            run_N_ns(N, ns)
+            assert N is not None
+            if len(ns) == 0:
+                fillin(run_N_ns, round(math.log2(N)))
+            else:
+                run_N_ns(N, ns)
 
         return True
```

### Comparing `running-ng-0.4.4/src/running/config/base/dacapo.yml` & `running_ng-0.4.5/src/running/config/base/dacapo.yml`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/src/running/config/base/modifiers.yml` & `running_ng-0.4.5/src/running/config/base/modifiers.yml`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/src/running/config/runbms_example.yml` & `running_ng-0.4.5/src/running/config/runbms_example_probes.yml`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/src/running/config.py` & `running_ng-0.4.5/src/running/config.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/src/running/modifier.py` & `running_ng-0.4.5/src/running/modifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,7 +176,16 @@
 class JuliaArg(Modifier):
     def __init__(self, value_opts=None, **kwargs):
         super().__init__(value_opts, **kwargs)
         self.val = split_quoted(self._kwargs["val"])
 
     def __str__(self) -> str:
         return "{} JuliaArg {}".format(super().__str__(), self.val)
+
+
+@register(Modifier)
+class NoImplicitHeapsizeModifier(Modifier):
+    def __init__(self, value_opts=None, **kwargs):
+        super().__init__(value_opts, **kwargs)
+
+    def __str__(self) -> str:
+        return "{} NoImplicitHeapsizeModifier".format(super().__str__())
```

### Comparing `running-ng-0.4.4/src/running/plugin/runbms/__init__.py` & `running_ng-0.4.5/src/running/plugin/runbms/__init__.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/src/running/plugin/runbms/copyfile.py` & `running_ng-0.4.5/src/running/plugin/runbms/copyfile.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/src/running/plugin/runbms/zulip.py` & `running_ng-0.4.5/src/running/plugin/runbms/zulip.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/src/running/runtime.py` & `running_ng-0.4.5/src/running/runtime.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/src/running/suite.py` & `running_ng-0.4.5/src/running/suite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from pathlib import Path
-from typing import Any, Dict, Optional, Union, List, Sequence
+from typing import Any, Dict, Optional, Union
 from running.benchmark import (
     JavaBenchmark,
     BinaryBenchmark,
     Benchmark,
     JavaScriptBenchmark,
     JuliaBenchmark,
 )
-from running.runtime import OpenJDK, Runtime
-from running.modifier import JVMArg, Modifier
 import logging
 from running.util import register, split_quoted
 import os.path
 
 __DRY_RUN = False
 __DEFAULT_MINHEAP = 4096
```

### Comparing `running-ng-0.4.4/src/running/util.py` & `running_ng-0.4.5/src/running/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,24 @@
     configuration: "Configuration", c: str
 ) -> Tuple["Runtime", List["Modifier"]]:
     runtime = configuration.get("runtimes")[c.split("|")[0].strip()]
     mods = parse_modifier_strs(configuration, c.split("|")[1:])
     return runtime, mods
 
 
+def dont_emit_heapsize_modifier(configuration: "Configuration", c: str) -> bool:
+    mods = parse_modifier_strs(configuration, c.split("|")[1:])
+    from running.modifier import NoImplicitHeapsizeModifier
+
+    for mod in mods:
+        if isinstance(mod, NoImplicitHeapsizeModifier):
+            return True
+    return False
+
+
 def config_str_encode(c: str) -> str:
     return ".".join([x.strip() for x in c.split("|")])
 
 
 def split_quoted(s: str) -> List[str]:
     return shlex.split(s)
```

### Comparing `running-ng-0.4.4/src/running_ng.egg-info/PKG-INFO` & `running_ng-0.4.5/src/running_ng.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: running-ng
-Version: 0.4.4
+Version: 0.4.5
 Summary: Running: Next Generation
 Author-email: Zixian Cai <u5937495@anu.edu.au>
 License: Apache
 Project-URL: Homepage, https://github.com/anupli/running-ng
 Project-URL: Bug Tracker, https://github.com/anupli/running-ng/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -14,17 +14,17 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml~=6.0.1
 Provides-Extra: zulip
 Requires-Dist: zulip~=0.9.0; extra == "zulip"
 Provides-Extra: tests
-Requires-Dist: pytest~=7.4.3; extra == "tests"
+Requires-Dist: pytest<8.3.0,>=7.4.4; extra == "tests"
 Requires-Dist: types-PyYAML~=6.0.12; extra == "tests"
-Requires-Dist: mypy~=1.7.0; extra == "tests"
+Requires-Dist: mypy<1.10,>=1.8; extra == "tests"
 
 # `running-ng`
 `running-ng` is a collection of scripts that help people run workloads in a methodologically sound settings.
 
 ## Installation
 `pip3 install running-ng`
```

### Comparing `running-ng-0.4.4/src/running_ng.egg-info/SOURCES.txt` & `running_ng-0.4.5/src/running_ng.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 src/running/command/fillin.py
 src/running/command/genadvice.py
 src/running/command/log_preprocessor.py
 src/running/command/minheap.py
 src/running/command/runbms.py
 src/running/config/minheap_example.yml
 src/running/config/runbms_example.yml
+src/running/config/runbms_example_probes.yml
 src/running/config/base/dacapo.yml
 src/running/config/base/jvms.yml
 src/running/config/base/minheap.yml
 src/running/config/base/modifiers.yml
 src/running/config/base/runbms-anu.yml
 src/running/config/base/runbms.yml
 src/running/config/base/specjbb2015.yml
```

### Comparing `running-ng-0.4.4/tests/test_config.py` & `running_ng-0.4.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/tests/test_fillin.py` & `running_ng-0.4.5/tests/test_fillin.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/tests/test_log_preprocessor.py` & `running_ng-0.4.5/tests/test_log_preprocessor.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/tests/test_modifier.py` & `running_ng-0.4.5/tests/test_modifier.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from running.benchmark import JavaBenchmark
 from running.modifier import *
 from running.config import Configuration
 from running.runtime import OpenJDK
+from running.util import dont_emit_heapsize_modifier
 
 
 def test_jvm_arg():
     j = JVMArg(name="j", val='-Xms100M -D"foo bar"')
     assert j.val == ["-Xms100M", "-Dfoo bar"]
 
 
@@ -159,7 +160,27 @@
         ]
     )
     openjdk = OpenJDK(
         release=11, home="/usr/lib/jvm/temurin-11-jdk-amd64", name="temurin-11"
     )
     assert "$HOME" not in jb.to_string(openjdk)
     assert "$DAHKDLHDIWHEIUWHEIWEHIJHDJKAGDKJADGUQDGIQUWDGI" in jb.to_string(openjdk)
+
+
+def test_no_implicit_heapsize_modifier():
+    c = Configuration(
+        {
+            "modifiers": {
+                "no_hfac": {"type": "NoImplicitHeapsizeModifier"},
+            },
+            "runtimes": {
+                "jdk8": {
+                    "type": "OpenJDK",
+                    "release": 8,
+                    "home": "/usr/lib/jvm/temurin-8-jdk-amd64",
+                }
+            },
+        }
+    )
+    c.resolve_class()
+    assert not dont_emit_heapsize_modifier(c, "jdk8|")
+    assert dont_emit_heapsize_modifier(c, "jdk8|no_hfac")
```

### Comparing `running-ng-0.4.4/tests/test_runtime.py` & `running_ng-0.4.5/tests/test_runtime.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/tests/test_suite.py` & `running_ng-0.4.5/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.4.4/tests/test_util.py` & `running_ng-0.4.5/tests/test_util.py`

 * *Files identical despite different names*

