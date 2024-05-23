# Comparing `tmp/picopy-1.0.0.tar.gz` & `tmp/picopy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picopy-1.0.0.tar", last modified: Thu May 23 20:20:35 2024, max compression
+gzip compressed data, was "picopy-1.0.1.tar", last modified: Thu May 23 20:53:28 2024, max compression
```

## Comparing `picopy-1.0.0.tar` & `picopy-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:20:35.515354 picopy-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 20:20:31.000000 picopy-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-23 20:20:35.515354 picopy-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:20:31.000000 picopy-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:20:35.515354 picopy-1.0.0/picopy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:20:31.000000 picopy-1.0.0/picopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-23 20:20:31.000000 picopy-1.0.0/picopy/picopy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:20:35.515354 picopy-1.0.0/picopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-23 20:20:35.000000 picopy-1.0.0/picopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-23 20:20:35.000000 picopy-1.0.0/picopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:20:35.000000 picopy-1.0.0/picopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 20:20:35.000000 picopy-1.0.0/picopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:20:31.000000 picopy-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 20:20:35.515354 picopy-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-23 20:20:31.000000 picopy-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:20:35.515354 picopy-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 20:20:31.000000 picopy-1.0.0/tests/test_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:53:28.144954 picopy-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 20:53:23.000000 picopy-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-23 20:53:28.144954 picopy-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-23 20:53:23.000000 picopy-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:53:28.140954 picopy-1.0.1/picopy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:53:23.000000 picopy-1.0.1/picopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-23 20:53:23.000000 picopy-1.0.1/picopy/picopy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:53:28.140954 picopy-1.0.1/picopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-23 20:53:28.000000 picopy-1.0.1/picopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-23 20:53:28.000000 picopy-1.0.1/picopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:53:28.000000 picopy-1.0.1/picopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 20:53:28.000000 picopy-1.0.1/picopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:53:23.000000 picopy-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 20:53:28.144954 picopy-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-23 20:53:23.000000 picopy-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:53:28.140954 picopy-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 20:53:23.000000 picopy-1.0.1/tests/test_package.py
```

### Comparing `picopy-1.0.0/picopy/picopy.py` & `picopy-1.0.1/picopy/picopy.py`

 * *Files identical despite different names*

