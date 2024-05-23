# Comparing `tmp/emec-api-0.1.6.tar.gz` & `tmp/emec_api-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/emec-api-0.1.6.tar", last modified: Fri May 12 01:02:15 2017, max compression
+gzip compressed data, was "emec_api-0.1.8.tar", max compression
```

## Comparing `emec-api-0.1.6.tar` & `emec_api-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 pavan      (501) staff       (20)        0 2017-05-12 01:02:15.000000 emec-api-0.1.6/
-drwxr-xr-x   0 pavan      (501) staff       (20)        0 2017-05-12 01:02:15.000000 emec-api-0.1.6/emec/
--rw-r--r--   0 pavan      (501) staff       (20)      293 2017-05-12 00:55:09.000000 emec-api-0.1.6/emec/__init__.py
--rw-r--r--   0 pavan      (501) staff       (20)     6076 2017-05-12 00:48:33.000000 emec-api-0.1.6/emec/emec.py
--rw-r--r--   0 pavan      (501) staff       (20)      484 2017-05-12 00:47:34.000000 emec-api-0.1.6/emec/utils.py
-drwxr-xr-x   0 pavan      (501) staff       (20)        0 2017-05-12 01:02:15.000000 emec-api-0.1.6/emec_api.egg-info/
--rw-r--r--   0 pavan      (501) staff       (20)        1 2017-05-12 01:02:15.000000 emec-api-0.1.6/emec_api.egg-info/dependency_links.txt
--rw-r--r--   0 pavan      (501) staff       (20)      351 2017-05-12 01:02:15.000000 emec-api-0.1.6/emec_api.egg-info/PKG-INFO
--rw-r--r--   0 pavan      (501) staff       (20)       38 2017-05-12 01:02:15.000000 emec-api-0.1.6/emec_api.egg-info/requires.txt
--rw-r--r--   0 pavan      (501) staff       (20)      221 2017-05-12 01:02:15.000000 emec-api-0.1.6/emec_api.egg-info/SOURCES.txt
--rw-r--r--   0 pavan      (501) staff       (20)        5 2017-05-12 01:02:15.000000 emec-api-0.1.6/emec_api.egg-info/top_level.txt
--rw-r--r--   0 pavan      (501) staff       (20)      351 2017-05-12 01:02:15.000000 emec-api-0.1.6/PKG-INFO
--rw-r--r--   0 pavan      (501) staff       (20)      100 2017-05-12 01:02:15.000000 emec-api-0.1.6/setup.cfg
--rw-r--r--   0 pavan      (501) staff       (20)      504 2017-05-12 00:54:58.000000 emec-api-0.1.6/setup.py
+-rw-r--r--   0        0        0     1070 2024-05-22 21:47:27.179154 emec_api-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1641 2024-05-22 21:59:37.816856 emec_api-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2024-05-22 21:47:27.179154 emec_api-0.1.8/emec_api/__init__.py
+-rw-r--r--   0        0        0      145 2024-05-23 01:46:56.740761 emec_api-0.1.8/emec_api/__main__.py
+-rw-r--r--   0        0        0      251 2024-05-23 02:09:18.078597 emec_api-0.1.8/emec_api/__version__.py
+-rw-r--r--   0        0        0        0 2024-05-22 21:47:27.179154 emec_api-0.1.8/emec_api/api/__init__.py
+-rw-r--r--   0        0        0    11019 2024-05-22 21:47:27.179154 emec_api-0.1.8/emec_api/api/client.py
+-rw-r--r--   0        0        0      446 2024-05-22 21:47:27.179154 emec_api-0.1.8/emec_api/api/utils.py
+-rw-r--r--   0        0        0      582 2024-05-23 01:46:56.740761 emec_api-0.1.8/emec_api/application.py
+-rw-r--r--   0        0        0        0 2024-05-22 21:47:27.179154 emec_api-0.1.8/emec_api/commands/__init__.py
+-rw-r--r--   0        0        0      421 2024-05-22 21:47:27.179154 emec_api-0.1.8/emec_api/commands/about.py
+-rw-r--r--   0        0        0     4170 2024-05-23 01:46:56.740761 emec_api-0.1.8/emec_api/commands/scraper.py
+-rw-r--r--   0        0        0      808 2024-05-23 02:09:01.066641 emec_api-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2622 1970-01-01 00:00:00.000000 emec_api-0.1.8/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

