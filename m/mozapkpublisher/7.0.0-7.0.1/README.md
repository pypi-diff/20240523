# Comparing `tmp/mozapkpublisher-7.0.0.tar.gz` & `tmp/mozapkpublisher-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozapkpublisher-7.0.0.tar", last modified: Fri Nov 17 16:27:12 2023, max compression
+gzip compressed data, was "mozapkpublisher-7.0.1.tar", last modified: Thu May 23 19:33:50 2024, max compression
```

## Comparing `mozapkpublisher-7.0.0.tar` & `mozapkpublisher-7.0.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-11-17 16:27:12.655948 mozapkpublisher-7.0.0/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    16725 2019-08-14 14:51:54.000000 mozapkpublisher-7.0.0/LICENSE
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      248 2019-08-14 14:51:54.000000 mozapkpublisher-7.0.0/MANIFEST.in
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      509 2023-11-17 16:27:12.655948 mozapkpublisher-7.0.0/PKG-INFO
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2749 2023-11-17 16:23:05.000000 mozapkpublisher-7.0.0/README.md
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-11-17 16:27:12.651948 mozapkpublisher-7.0.0/mozapkpublisher/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)        0 2017-01-17 13:49:23.000000 mozapkpublisher-7.0.0/mozapkpublisher/__init__.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      746 2019-08-14 14:51:54.000000 mozapkpublisher-7.0.0/mozapkpublisher/check_apks.py
--rwxr-xr-x   0 jcristau  (1000) jcristau  (1000)     1947 2023-11-17 16:23:05.000000 mozapkpublisher-7.0.0/mozapkpublisher/check_rollout.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-11-17 16:27:12.651948 mozapkpublisher-7.0.0/mozapkpublisher/common/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)        0 2017-10-27 10:10:25.000000 mozapkpublisher-7.0.0/mozapkpublisher/common/__init__.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-11-17 16:27:12.651948 mozapkpublisher-7.0.0/mozapkpublisher/common/aab/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      447 2023-09-21 08:48:05.000000 mozapkpublisher-7.0.0/mozapkpublisher/common/aab/__init__.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1383 2023-09-21 08:48:05.000000 mozapkpublisher-7.0.0/mozapkpublisher/common/aab/extractor.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-11-17 16:27:12.651948 mozapkpublisher-7.0.0/mozapkpublisher/common/apk/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2258 2022-03-03 10:46:46.000000 mozapkpublisher-7.0.0/mozapkpublisher/common/apk/__init__.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     6799 2022-03-03 10:46:46.000000 mozapkpublisher-7.0.0/mozapkpublisher/common/apk/checker.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     4615 2022-03-03 10:46:46.000000 mozapkpublisher-7.0.0/mozapkpublisher/common/apk/extractor.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3838 2019-08-14 14:51:54.000000 mozapkpublisher-7.0.0/mozapkpublisher/common/apk/history.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1139 2022-03-03 10:46:46.000000 mozapkpublisher-7.0.0/mozapkpublisher/common/exceptions.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      287 2018-05-17 16:14:22.000000 mozapkpublisher-7.0.0/mozapkpublisher/common/main_logging.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    10257 2023-11-17 16:23:05.000000 mozapkpublisher-7.0.0/mozapkpublisher/common/store.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2681 2023-11-17 16:23:05.000000 mozapkpublisher-7.0.0/mozapkpublisher/common/utils.py
--rwxr-xr-x   0 jcristau  (1000) jcristau  (1000)     9898 2019-08-14 14:51:54.000000 mozapkpublisher-7.0.0/mozapkpublisher/get_apk.py
--rwxr-xr-x   0 jcristau  (1000) jcristau  (1000)     2476 2023-11-17 16:23:05.000000 mozapkpublisher-7.0.0/mozapkpublisher/push_aab.py
--rwxr-xr-x   0 jcristau  (1000) jcristau  (1000)     3601 2023-11-17 16:23:05.000000 mozapkpublisher-7.0.0/mozapkpublisher/push_apk.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-11-17 16:27:12.655948 mozapkpublisher-7.0.0/mozapkpublisher/test/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)       88 2019-08-14 14:51:54.000000 mozapkpublisher-7.0.0/mozapkpublisher/test/__init__.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-11-17 16:27:12.655948 mozapkpublisher-7.0.0/mozapkpublisher/test/common/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)        0 2017-10-27 10:10:25.000000 mozapkpublisher-7.0.0/mozapkpublisher/test/common/__init__.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-11-17 16:27:12.655948 mozapkpublisher-7.0.0/mozapkpublisher/test/common/aab/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)        0 2023-09-21 08:48:05.000000 mozapkpublisher-7.0.0/mozapkpublisher/test/common/aab/__init__.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      352 2023-09-21 08:48:05.000000 mozapkpublisher-7.0.0/mozapkpublisher/test/common/aab/test_init.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-11-17 16:27:12.655948 mozapkpublisher-7.0.0/mozapkpublisher/test/common/apk/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)        0 2018-05-17 16:14:22.000000 mozapkpublisher-7.0.0/mozapkpublisher/test/common/apk/__init__.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    34840 2022-03-03 10:46:46.000000 mozapkpublisher-7.0.0/mozapkpublisher/test/common/apk/test_checker.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7954 2022-03-03 10:46:46.000000 mozapkpublisher-7.0.0/mozapkpublisher/test/common/apk/test_extractor.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3602 2019-08-14 14:51:54.000000 mozapkpublisher-7.0.0/mozapkpublisher/test/common/apk/test_history.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      489 2019-08-14 14:51:54.000000 mozapkpublisher-7.0.0/mozapkpublisher/test/common/apk/test_init.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    14612 2023-11-17 16:23:05.000000 mozapkpublisher-7.0.0/mozapkpublisher/test/common/test_store.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3256 2023-09-21 08:48:05.000000 mozapkpublisher-7.0.0/mozapkpublisher/test/common/test_utils.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-11-17 16:27:12.655948 mozapkpublisher-7.0.0/mozapkpublisher/test/data/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      477 2018-06-18 16:12:28.000000 mozapkpublisher-7.0.0/mozapkpublisher/test/data/SHA512SUMS
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)       15 2017-03-09 17:50:46.000000 mozapkpublisher-7.0.0/mozapkpublisher/test/data/blob
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     4071 2017-03-09 17:50:46.000000 mozapkpublisher-7.0.0/mozapkpublisher/test/data/checksums.broken
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      134 2017-03-09 17:50:46.000000 mozapkpublisher-7.0.0/mozapkpublisher/test/data/checksums.old
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     4071 2017-03-09 17:50:46.000000 mozapkpublisher-7.0.0/mozapkpublisher/test/data/checksums.tc
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3644 2022-03-03 10:46:46.000000 mozapkpublisher-7.0.0/mozapkpublisher/test/test_check_rollout.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     6911 2019-03-29 08:54:55.000000 mozapkpublisher-7.0.0/mozapkpublisher/test/test_get_apk.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3083 2023-11-17 16:23:05.000000 mozapkpublisher-7.0.0/mozapkpublisher/test/test_push_aab.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     4971 2023-11-17 16:23:05.000000 mozapkpublisher-7.0.0/mozapkpublisher/test/test_push_apk.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-11-17 16:27:12.651948 mozapkpublisher-7.0.0/mozapkpublisher.egg-info/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      509 2023-11-17 16:27:12.000000 mozapkpublisher-7.0.0/mozapkpublisher.egg-info/PKG-INFO
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1664 2023-11-17 16:27:12.000000 mozapkpublisher-7.0.0/mozapkpublisher.egg-info/SOURCES.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)        1 2023-11-17 16:27:12.000000 mozapkpublisher-7.0.0/mozapkpublisher.egg-info/dependency_links.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      101 2023-11-17 16:27:12.000000 mozapkpublisher-7.0.0/mozapkpublisher.egg-info/requires.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)       16 2023-11-17 16:27:12.000000 mozapkpublisher-7.0.0/mozapkpublisher.egg-info/top_level.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)       67 2023-11-17 16:27:12.655948 mozapkpublisher-7.0.0/setup.cfg
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      981 2023-11-17 16:25:32.000000 mozapkpublisher-7.0.0/setup.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)        6 2023-11-17 16:23:05.000000 mozapkpublisher-7.0.0/version.txt
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2024-05-23 19:33:50.919814 mozapkpublisher-7.0.1/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)    16725 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/LICENSE
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      248 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/MANIFEST.in
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      509 2024-05-23 19:33:50.919814 mozapkpublisher-7.0.1/PKG-INFO
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     2749 2024-05-18 00:26:48.000000 mozapkpublisher-7.0.1/README.md
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2024-05-23 19:33:50.915814 mozapkpublisher-7.0.1/mozapkpublisher/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        0 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/__init__.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      746 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/check_apks.py
+-rwxrwxr-x   0 gbrown    (1000) gbrown    (1000)     1947 2024-05-18 00:26:48.000000 mozapkpublisher-7.0.1/mozapkpublisher/check_rollout.py
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2024-05-23 19:33:50.919814 mozapkpublisher-7.0.1/mozapkpublisher/common/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        0 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/common/__init__.py
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2024-05-23 19:33:50.919814 mozapkpublisher-7.0.1/mozapkpublisher/common/aab/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      447 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/common/aab/__init__.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     1386 2024-05-23 19:31:22.000000 mozapkpublisher-7.0.1/mozapkpublisher/common/aab/extractor.py
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2024-05-23 19:33:50.919814 mozapkpublisher-7.0.1/mozapkpublisher/common/apk/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     2258 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/common/apk/__init__.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     6799 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/common/apk/checker.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     4615 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/common/apk/extractor.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     3837 2024-05-23 19:31:22.000000 mozapkpublisher-7.0.1/mozapkpublisher/common/apk/history.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     1139 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/common/exceptions.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      287 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/common/main_logging.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)    10238 2024-05-23 19:31:22.000000 mozapkpublisher-7.0.1/mozapkpublisher/common/store.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     2681 2024-05-18 00:26:48.000000 mozapkpublisher-7.0.1/mozapkpublisher/common/utils.py
+-rwxrwxr-x   0 gbrown    (1000) gbrown    (1000)     9898 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/get_apk.py
+-rwxrwxr-x   0 gbrown    (1000) gbrown    (1000)     2476 2024-05-18 00:26:48.000000 mozapkpublisher-7.0.1/mozapkpublisher/push_aab.py
+-rwxrwxr-x   0 gbrown    (1000) gbrown    (1000)     3601 2024-05-18 00:26:48.000000 mozapkpublisher-7.0.1/mozapkpublisher/push_apk.py
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2024-05-23 19:33:50.919814 mozapkpublisher-7.0.1/mozapkpublisher/test/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       88 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/test/__init__.py
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2024-05-23 19:33:50.919814 mozapkpublisher-7.0.1/mozapkpublisher/test/common/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        0 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/test/common/__init__.py
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2024-05-23 19:33:50.919814 mozapkpublisher-7.0.1/mozapkpublisher/test/common/aab/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        0 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/test/common/aab/__init__.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      352 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/test/common/aab/test_init.py
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2024-05-23 19:33:50.919814 mozapkpublisher-7.0.1/mozapkpublisher/test/common/apk/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        0 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/test/common/apk/__init__.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)    34840 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/test/common/apk/test_checker.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     7954 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/test/common/apk/test_extractor.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     3602 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/test/common/apk/test_history.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      489 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/test/common/apk/test_init.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)    14612 2024-05-18 00:26:48.000000 mozapkpublisher-7.0.1/mozapkpublisher/test/common/test_store.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     3256 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/test/common/test_utils.py
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2024-05-23 19:33:50.919814 mozapkpublisher-7.0.1/mozapkpublisher/test/data/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      477 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/test/data/SHA512SUMS
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       15 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/test/data/blob
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     4071 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/test/data/checksums.broken
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      134 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/test/data/checksums.old
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     4071 2023-09-14 15:50:25.000000 mozapkpublisher-7.0.1/mozapkpublisher/test/data/checksums.tc
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     3644 2023-09-14 15:50:26.000000 mozapkpublisher-7.0.1/mozapkpublisher/test/test_check_rollout.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     6911 2023-09-14 15:50:26.000000 mozapkpublisher-7.0.1/mozapkpublisher/test/test_get_apk.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     3083 2024-05-18 00:26:48.000000 mozapkpublisher-7.0.1/mozapkpublisher/test/test_push_aab.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     4971 2024-05-18 00:26:48.000000 mozapkpublisher-7.0.1/mozapkpublisher/test/test_push_apk.py
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2024-05-23 19:33:50.915814 mozapkpublisher-7.0.1/mozapkpublisher.egg-info/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      509 2024-05-23 19:33:50.000000 mozapkpublisher-7.0.1/mozapkpublisher.egg-info/PKG-INFO
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     1664 2024-05-23 19:33:50.000000 mozapkpublisher-7.0.1/mozapkpublisher.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        1 2024-05-23 19:33:50.000000 mozapkpublisher-7.0.1/mozapkpublisher.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      103 2024-05-23 19:33:50.000000 mozapkpublisher-7.0.1/mozapkpublisher.egg-info/requires.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       16 2024-05-23 19:33:50.000000 mozapkpublisher-7.0.1/mozapkpublisher.egg-info/top_level.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       67 2024-05-23 19:33:50.919814 mozapkpublisher-7.0.1/setup.cfg
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      981 2024-05-18 00:26:48.000000 mozapkpublisher-7.0.1/setup.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        6 2024-05-23 19:31:22.000000 mozapkpublisher-7.0.1/version.txt
```

### Comparing `mozapkpublisher-7.0.0/LICENSE` & `mozapkpublisher-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/README.md` & `mozapkpublisher-7.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/check_apks.py` & `mozapkpublisher-7.0.1/mozapkpublisher/check_apks.py`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/check_rollout.py` & `mozapkpublisher-7.0.1/mozapkpublisher/check_rollout.py`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/common/aab/extractor.py` & `mozapkpublisher-7.0.1/mozapkpublisher/common/aab/extractor.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,25 +19,28 @@
         metadata['package_name'] = _extract_package_name(aab_copy.name)
         logger.info('Found package name "{}"'.format(metadata['package_name']))
         metadata['version_code'] = _extract_version_code(aab_copy.name)
         logger.info('Found version code "{}"'.format(metadata['version_code']))
 
     return metadata
 
+
 def _run_bundletool(bundletool_args):
     bundletool_path = os.environ.get("BUNDLETOOL_PATH", "./bundletool.jar")
     cmd = ['java', '-jar', bundletool_path] + bundletool_args
     logger.debug(f'Running command: {cmd}')
     out = subprocess.check_output(cmd, text=True)
     out = out.strip('\n')
     logger.debug(f'Output: {out}')
     return out
 
+
 def _extract_package_name(aab_path):
     args = ['dump', 'manifest', f'--bundle={aab_path}', '--xpath=/manifest/@package']
     out = _run_bundletool(args)
     return out
 
+
 def _extract_version_code(aab_path):
     args = ['dump', 'manifest', f'--bundle={aab_path}', '--xpath=/manifest/@android:versionCode']
     out = _run_bundletool(args)
     return out
```

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/common/apk/__init__.py` & `mozapkpublisher-7.0.1/mozapkpublisher/common/apk/__init__.py`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/common/apk/checker.py` & `mozapkpublisher-7.0.1/mozapkpublisher/common/apk/checker.py`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/common/apk/extractor.py` & `mozapkpublisher-7.0.1/mozapkpublisher/common/apk/extractor.py`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/common/apk/history.py` & `mozapkpublisher-7.0.1/mozapkpublisher/common/apk/history.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     for architecture in _MAJOR_FIREFOX_VERSIONS_PER_ARCHITECTURE_AND_API_LEVEL:
         api_levels = get_expected_api_levels(firefox_version, architecture, package_name)
 
         for api_level in api_levels:
             combos.add((architecture, api_level))
 
     if not combos:
-        raise ValueError('No combos found for Firefox version {}. Current rules: {2}'.format(
+        raise ValueError('No combos found for Firefox version {}. Current rules: {}'.format(
             firefox_version, _MAJOR_FIREFOX_VERSIONS_PER_ARCHITECTURE_AND_API_LEVEL
         ))
 
     logger.debug(
         'Expected to find these combos for Firefox {}: {}'.format(
             firefox_version, craft_combos_pretty_names(combos)
         )
```

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/common/exceptions.py` & `mozapkpublisher-7.0.1/mozapkpublisher/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/common/store.py` & `mozapkpublisher-7.0.1/mozapkpublisher/common/store.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from contextlib import contextmanager
 
 import json
 import logging
 
-import google.auth
 import httplib2
 
 from apiclient.discovery import build
 from googleapiclient.errors import HttpError
 from google.oauth2 import service_account
 # HACK: importing mock in production is useful for option `--do-not-contact-google-play`
 from unittest.mock import MagicMock
```

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/common/utils.py` & `mozapkpublisher-7.0.1/mozapkpublisher/common/utils.py`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/get_apk.py` & `mozapkpublisher-7.0.1/mozapkpublisher/get_apk.py`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/push_aab.py` & `mozapkpublisher-7.0.1/mozapkpublisher/push_aab.py`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/push_apk.py` & `mozapkpublisher-7.0.1/mozapkpublisher/push_apk.py`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/test/common/apk/test_checker.py` & `mozapkpublisher-7.0.1/mozapkpublisher/test/common/apk/test_checker.py`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/test/common/apk/test_extractor.py` & `mozapkpublisher-7.0.1/mozapkpublisher/test/common/apk/test_extractor.py`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/test/common/apk/test_history.py` & `mozapkpublisher-7.0.1/mozapkpublisher/test/common/apk/test_history.py`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/test/common/test_store.py` & `mozapkpublisher-7.0.1/mozapkpublisher/test/common/test_store.py`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/test/common/test_utils.py` & `mozapkpublisher-7.0.1/mozapkpublisher/test/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/test/data/checksums.broken` & `mozapkpublisher-7.0.1/mozapkpublisher/test/data/checksums.broken`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/test/data/checksums.tc` & `mozapkpublisher-7.0.1/mozapkpublisher/test/data/checksums.tc`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/test/test_check_rollout.py` & `mozapkpublisher-7.0.1/mozapkpublisher/test/test_check_rollout.py`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/test/test_get_apk.py` & `mozapkpublisher-7.0.1/mozapkpublisher/test/test_get_apk.py`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/test/test_push_aab.py` & `mozapkpublisher-7.0.1/mozapkpublisher/test/test_push_aab.py`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher/test/test_push_apk.py` & `mozapkpublisher-7.0.1/mozapkpublisher/test/test_push_apk.py`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/mozapkpublisher.egg-info/SOURCES.txt` & `mozapkpublisher-7.0.1/mozapkpublisher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozapkpublisher-7.0.0/setup.py` & `mozapkpublisher-7.0.1/setup.py`

 * *Files identical despite different names*

