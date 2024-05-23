# Comparing `tmp/picopy-1.0.1.tar.gz` & `tmp/picopy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picopy-1.0.1.tar", last modified: Thu May 23 20:53:28 2024, max compression
+gzip compressed data, was "picopy-1.0.3.tar", last modified: Thu May 23 21:19:23 2024, max compression
```

## Comparing `picopy-1.0.1.tar` & `picopy-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:53:28.144954 picopy-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 20:53:23.000000 picopy-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-23 20:53:28.144954 picopy-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-23 20:53:23.000000 picopy-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:53:28.140954 picopy-1.0.1/picopy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:53:23.000000 picopy-1.0.1/picopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-23 20:53:23.000000 picopy-1.0.1/picopy/picopy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:53:28.140954 picopy-1.0.1/picopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-23 20:53:28.000000 picopy-1.0.1/picopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-23 20:53:28.000000 picopy-1.0.1/picopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:53:28.000000 picopy-1.0.1/picopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 20:53:28.000000 picopy-1.0.1/picopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:53:23.000000 picopy-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 20:53:28.144954 picopy-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-23 20:53:23.000000 picopy-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:53:28.140954 picopy-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 20:53:23.000000 picopy-1.0.1/tests/test_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:19:23.664076 picopy-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 21:19:19.000000 picopy-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-23 21:19:23.664076 picopy-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-23 21:19:19.000000 picopy-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:19:23.664076 picopy-1.0.3/picopy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 21:19:19.000000 picopy-1.0.3/picopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-23 21:19:19.000000 picopy-1.0.3/picopy/picopy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:19:23.664076 picopy-1.0.3/picopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-23 21:19:23.000000 picopy-1.0.3/picopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-23 21:19:23.000000 picopy-1.0.3/picopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:19:23.000000 picopy-1.0.3/picopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 21:19:23.000000 picopy-1.0.3/picopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 21:19:19.000000 picopy-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:19:23.664076 picopy-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-23 21:19:19.000000 picopy-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:19:23.664076 picopy-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 21:19:19.000000 picopy-1.0.3/tests/test_package.py
```

### Comparing `picopy-1.0.1/picopy/picopy.py` & `picopy-1.0.3/picopy/picopy.py`

 * *Files identical despite different names*

