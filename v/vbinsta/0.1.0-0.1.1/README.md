# Comparing `tmp/vbinsta-0.1.0.tar.gz` & `tmp/vbinsta-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbinsta-0.1.0.tar", max compression
+gzip compressed data, was "vbinsta-0.1.1.tar", max compression
```

## Comparing `vbinsta-0.1.0.tar` & `vbinsta-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-05-23 06:30:54.662078 vbinsta-0.1.0/README.md
--rw-r--r--   0        0        0      368 2024-05-23 07:38:30.161517 vbinsta-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-23 06:30:54.661978 vbinsta-0.1.0/vbinsta/__init__.py
--rw-r--r--   0        0        0       49 2024-05-23 07:38:03.656860 vbinsta-0.1.0/vbinsta/__main__.py
--rw-r--r--   0        0        0      281 2024-05-23 08:10:44.936004 vbinsta-0.1.0/vbinsta/functions.py
--rw-r--r--   0        0        0      261 2024-05-23 08:10:25.061042 vbinsta-0.1.0/vbinsta/main.py
--rw-r--r--   0        0        0      477 2024-05-23 08:10:00.789500 vbinsta-0.1.0/vbinsta/upload.py
--rw-r--r--   0        0        0      372 1970-01-01 00:00:00.000000 vbinsta-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-23 06:30:54.662078 vbinsta-0.1.1/README.md
+-rw-r--r--   0        0        0      368 2024-05-23 19:19:03.191503 vbinsta-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-23 06:30:54.661978 vbinsta-0.1.1/vbinsta/__init__.py
+-rw-r--r--   0        0        0       49 2024-05-23 07:38:03.656860 vbinsta-0.1.1/vbinsta/__main__.py
+-rw-r--r--   0        0        0      281 2024-05-23 19:18:57.580597 vbinsta-0.1.1/vbinsta/functions.py
+-rw-r--r--   0        0        0      261 2024-05-23 08:10:25.061042 vbinsta-0.1.1/vbinsta/main.py
+-rw-r--r--   0        0        0      793 2024-05-23 19:18:52.953812 vbinsta-0.1.1/vbinsta/upload.py
+-rw-r--r--   0        0        0      372 1970-01-01 00:00:00.000000 vbinsta-0.1.1/PKG-INFO
```

