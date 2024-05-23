# Comparing `tmp/rootdir-0.1.2.post7.tar.gz` & `tmp/rootdir-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rootdir-0.1.2.post7.tar", last modified: Mon May 13 15:25:19 2024, max compression
+gzip compressed data, was "rootdir-0.1.3.tar", last modified: Thu May 23 02:16:24 2024, max compression
```

## Comparing `rootdir-0.1.2.post7.tar` & `rootdir-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:25:19.108672 rootdir-0.1.2.post7/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-13 15:25:19.108672 rootdir-0.1.2.post7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-13 15:25:10.000000 rootdir-0.1.2.post7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:25:19.108672 rootdir-0.1.2.post7/rootdir/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-13 15:25:10.000000 rootdir-0.1.2.post7/rootdir/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:25:19.108672 rootdir-0.1.2.post7/rootdir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-13 15:25:19.000000 rootdir-0.1.2.post7/rootdir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:25:19.000000 rootdir-0.1.2.post7/rootdir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:25:19.000000 rootdir-0.1.2.post7/rootdir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 15:25:19.000000 rootdir-0.1.2.post7/rootdir.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:25:19.108672 rootdir-0.1.2.post7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-13 15:25:10.000000 rootdir-0.1.2.post7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:16:24.341873 rootdir-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-23 02:16:24.337873 rootdir-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-23 02:16:16.000000 rootdir-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:16:24.337873 rootdir-0.1.3/rootdir/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-23 02:16:16.000000 rootdir-0.1.3/rootdir/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:16:24.337873 rootdir-0.1.3/rootdir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-23 02:16:24.000000 rootdir-0.1.3/rootdir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-23 02:16:24.000000 rootdir-0.1.3/rootdir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 02:16:24.000000 rootdir-0.1.3/rootdir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 02:16:24.000000 rootdir-0.1.3/rootdir.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 02:16:24.341873 rootdir-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-23 02:16:16.000000 rootdir-0.1.3/setup.py
```

### Comparing `rootdir-0.1.2.post7/rootdir/__init__.py` & `rootdir-0.1.3/rootdir/__init__.py`

 * *Files identical despite different names*

