# Comparing `tmp/cvat_sdk_i_digit-0.0.3.tar.gz` & `tmp/cvat_sdk_i_digit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvat_sdk_i_digit-0.0.3.tar", last modified: Wed May 22 12:43:28 2024, max compression
+gzip compressed data, was "cvat_sdk_i_digit-0.0.4.tar", last modified: Thu May 23 03:09:19 2024, max compression
```

## Comparing `cvat_sdk_i_digit-0.0.3.tar` & `cvat_sdk_i_digit-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,7 @@
-drwxrwxr-x   0 dima      (1000) dima      (1000)        0 2024-05-22 12:43:28.343921 cvat_sdk_i_digit-0.0.3/
--rw-r--r--   0 dima      (1000) dima      (1000)      311 2024-05-22 12:43:28.343921 cvat_sdk_i_digit-0.0.3/PKG-INFO
--rw-rw-r--   0 dima      (1000) dima      (1000)        0 2024-05-22 11:23:00.000000 cvat_sdk_i_digit-0.0.3/README.md
-drwxrwxr-x   0 dima      (1000) dima      (1000)        0 2024-05-22 12:43:28.343921 cvat_sdk_i_digit-0.0.3/cvat_sdk_i_digit.egg-info/
--rw-r--r--   0 dima      (1000) dima      (1000)      311 2024-05-22 12:43:28.000000 cvat_sdk_i_digit-0.0.3/cvat_sdk_i_digit.egg-info/PKG-INFO
--rw-rw-r--   0 dima      (1000) dima      (1000)      223 2024-05-22 12:43:28.000000 cvat_sdk_i_digit-0.0.3/cvat_sdk_i_digit.egg-info/SOURCES.txt
--rw-rw-r--   0 dima      (1000) dima      (1000)        1 2024-05-22 12:43:28.000000 cvat_sdk_i_digit-0.0.3/cvat_sdk_i_digit.egg-info/dependency_links.txt
--rw-rw-r--   0 dima      (1000) dima      (1000)       71 2024-05-22 12:43:28.000000 cvat_sdk_i_digit-0.0.3/cvat_sdk_i_digit.egg-info/requires.txt
--rw-rw-r--   0 dima      (1000) dima      (1000)        1 2024-05-22 12:43:28.000000 cvat_sdk_i_digit-0.0.3/cvat_sdk_i_digit.egg-info/top_level.txt
--rw-rw-r--   0 dima      (1000) dima      (1000)      704 2024-05-22 12:42:57.000000 cvat_sdk_i_digit-0.0.3/pyproject.toml
--rw-rw-r--   0 dima      (1000) dima      (1000)       38 2024-05-22 12:43:28.343921 cvat_sdk_i_digit-0.0.3/setup.cfg
+-rw-r--r--   0        0        0     1073 2024-05-23 02:59:28.391193 cvat_sdk_i_digit-0.0.4/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-22 11:23:00.438197 cvat_sdk_i_digit-0.0.4/README.md
+-rw-r--r--   0        0        0      658 2024-05-23 03:09:19.858501 cvat_sdk_i_digit-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-22 11:19:44.471973 cvat_sdk_i_digit-0.0.4/src/cvat_sdk_i_digit/__init__.py
+-rw-r--r--   0        0        0     6031 2024-05-23 03:06:00.080006 cvat_sdk_i_digit-0.0.4/src/cvat_sdk_i_digit/config.py
+-rw-r--r--   0        0        0     3482 2024-05-23 03:04:49.807111 cvat_sdk_i_digit-0.0.4/src/cvat_sdk_i_digit/cvat_api.py
+-rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 cvat_sdk_i_digit-0.0.4/PKG-INFO
```

