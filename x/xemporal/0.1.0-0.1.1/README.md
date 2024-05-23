# Comparing `tmp/xemporal-0.1.0.tar.gz` & `tmp/xemporal-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xemporal-0.1.0.tar", max compression
+gzip compressed data, was "xemporal-0.1.1.tar", max compression
```

## Comparing `xemporal-0.1.0.tar` & `xemporal-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0       98 2024-05-21 15:53:51.025565 xemporal-0.1.0/README.md
--rw-r--r--   0        0        0      261 2024-05-22 17:37:20.731022 xemporal-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-22 17:21:35.888441 xemporal-0.1.0/xemporal/__init__.py
--rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 xemporal-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      110 2024-05-22 18:00:08.502577 xemporal-0.1.1/README.md
+-rw-r--r--   0        0        0      317 2024-05-22 18:13:33.312826 xemporal-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-22 17:21:35.888441 xemporal-0.1.1/xemporal/__init__.py
+-rw-r--r--   0        0        0      369 2024-05-22 17:42:44.583361 xemporal-0.1.1/xemporal/validator.py
+-rw-r--r--   0        0        0      390 1970-01-01 00:00:00.000000 xemporal-0.1.1/PKG-INFO
```

