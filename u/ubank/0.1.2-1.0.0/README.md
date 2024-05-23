# Comparing `tmp/ubank-0.1.2.tar.gz` & `tmp/ubank-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubank-0.1.2.tar", max compression
+gzip compressed data, was "ubank-1.0.0.tar", max compression
```

## Comparing `ubank-0.1.2.tar` & `ubank-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1074 2022-06-25 04:59:38.156921 ubank-0.1.2/LICENSE
--rw-r--r--   0        0        0     3042 2024-02-23 06:41:09.886915 ubank-0.1.2/README.md
--rw-r--r--   0        0        0      304 2024-02-23 06:41:09.887163 ubank-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4655 2024-02-23 06:41:09.887420 ubank-0.1.2/ubank.py
--rw-r--r--   0        0        0     3624 1970-01-01 00:00:00.000000 ubank-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2022-06-25 04:59:38.156921 ubank-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5183 2024-05-23 05:15:33.820250 ubank-1.0.0/README.md
+-rw-r--r--   0        0        0      289 2024-05-23 05:15:33.820957 ubank-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10766 2024-05-23 05:15:33.821504 ubank-1.0.0/ubank.py
+-rw-r--r--   0        0        0     5751 1970-01-01 00:00:00.000000 ubank-1.0.0/PKG-INFO
```

### Comparing `ubank-0.1.2/LICENSE` & `ubank-1.0.0/LICENSE`

 * *Files identical despite different names*

