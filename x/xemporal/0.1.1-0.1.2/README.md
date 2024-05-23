# Comparing `tmp/xemporal-0.1.1.tar.gz` & `tmp/xemporal-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xemporal-0.1.1.tar", max compression
+gzip compressed data, was "xemporal-0.1.2.tar", max compression
```

## Comparing `xemporal-0.1.1.tar` & `xemporal-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0      110 2024-05-22 18:00:08.502577 xemporal-0.1.1/README.md
--rw-r--r--   0        0        0      317 2024-05-22 18:13:33.312826 xemporal-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-22 17:21:35.888441 xemporal-0.1.1/xemporal/__init__.py
--rw-r--r--   0        0        0      369 2024-05-22 17:42:44.583361 xemporal-0.1.1/xemporal/validator.py
--rw-r--r--   0        0        0      390 1970-01-01 00:00:00.000000 xemporal-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      490 2024-05-23 15:10:21.383131 xemporal-0.1.2/README.md
+-rw-r--r--   0        0        0       96 2024-05-23 15:22:50.662717 xemporal-0.1.2/build.py
+-rw-r--r--   0        0        0      644 2024-05-23 16:20:22.717969 xemporal-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      514 2024-05-23 15:43:47.068085 xemporal-0.1.2/src/main.zig
+-rw-r--r--   0        0        0        0 2024-05-22 20:09:18.712785 xemporal-0.1.2/xemporal/__init__.py
+-rwxr-xr-x   0        0        0   420144 2024-05-23 16:18:26.007861 xemporal-0.1.2/xemporal/main.abi3.so
+-rw-r--r--   0        0        0      770 1970-01-01 00:00:00.000000 xemporal-0.1.2/PKG-INFO
```

