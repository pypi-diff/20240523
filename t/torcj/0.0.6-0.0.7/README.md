# Comparing `tmp/torcj-0.0.6.tar.gz` & `tmp/torcj-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torcj-0.0.6.tar", last modified: Thu May 23 11:07:08 2024, max compression
+gzip compressed data, was "torcj-0.0.7.tar", last modified: Thu May 23 11:16:00 2024, max compression
```

## Comparing `torcj-0.0.6.tar` & `torcj-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:07:08.270337 torcj-0.0.6/
--rw-r--r--   0 castle    (1000) castle    (1000)       93 2024-05-23 11:07:08.269337 torcj-0.0.6/PKG-INFO
--rw-r--r--   0 castle    (1000) castle    (1000)       59 2024-05-23 10:33:25.000000 torcj-0.0.6/README.md
--rw-r--r--   0 castle    (1000) castle    (1000)       38 2024-05-23 11:07:08.270337 torcj-0.0.6/setup.cfg
--rw-r--r--   0 castle    (1000) castle    (1000)      215 2024-05-23 11:07:04.000000 torcj-0.0.6/setup.py
-drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:07:08.268336 torcj-0.0.6/torcj/
--rw-r--r--   0 castle    (1000) castle    (1000)       29 2024-05-23 10:53:35.000000 torcj-0.0.6/torcj/__init__.py
--rw-r--r--   0 castle    (1000) castle    (1000)     1494 2024-05-23 11:03:27.000000 torcj-0.0.6/torcj/main.py
-drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:07:08.269337 torcj-0.0.6/torcj.egg-info/
--rw-r--r--   0 castle    (1000) castle    (1000)       93 2024-05-23 11:07:08.000000 torcj-0.0.6/torcj.egg-info/PKG-INFO
--rw-r--r--   0 castle    (1000) castle    (1000)      166 2024-05-23 11:07:08.000000 torcj-0.0.6/torcj.egg-info/SOURCES.txt
--rw-r--r--   0 castle    (1000) castle    (1000)        1 2024-05-23 11:07:08.000000 torcj-0.0.6/torcj.egg-info/dependency_links.txt
--rw-r--r--   0 castle    (1000) castle    (1000)        6 2024-05-23 11:07:08.000000 torcj-0.0.6/torcj.egg-info/top_level.txt
+drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:16:00.656245 torcj-0.0.7/
+-rw-r--r--   0 castle    (1000) castle    (1000)       93 2024-05-23 11:16:00.656245 torcj-0.0.7/PKG-INFO
+-rw-r--r--   0 castle    (1000) castle    (1000)       59 2024-05-23 10:33:25.000000 torcj-0.0.7/README.md
+-rw-r--r--   0 castle    (1000) castle    (1000)       38 2024-05-23 11:16:00.656245 torcj-0.0.7/setup.cfg
+-rw-r--r--   0 castle    (1000) castle    (1000)      209 2024-05-23 11:15:58.000000 torcj-0.0.7/setup.py
+drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:16:00.654245 torcj-0.0.7/torcj/
+-rw-r--r--   0 castle    (1000) castle    (1000)       29 2024-05-23 10:53:35.000000 torcj-0.0.7/torcj/__init__.py
+-rw-r--r--   0 castle    (1000) castle    (1000)     1494 2024-05-23 11:03:27.000000 torcj-0.0.7/torcj/main.py
+-rw-r--r--   0 castle    (1000) castle    (1000)   106896 2024-05-23 10:29:40.000000 torcj-0.0.7/torcj/storage.json
+drwxr-xr-x   0 castle    (1000) castle    (1000)        0 2024-05-23 11:16:00.656245 torcj-0.0.7/torcj.egg-info/
+-rw-r--r--   0 castle    (1000) castle    (1000)       93 2024-05-23 11:16:00.000000 torcj-0.0.7/torcj.egg-info/PKG-INFO
+-rw-r--r--   0 castle    (1000) castle    (1000)      185 2024-05-23 11:16:00.000000 torcj-0.0.7/torcj.egg-info/SOURCES.txt
+-rw-r--r--   0 castle    (1000) castle    (1000)        1 2024-05-23 11:16:00.000000 torcj-0.0.7/torcj.egg-info/dependency_links.txt
+-rw-r--r--   0 castle    (1000) castle    (1000)        6 2024-05-23 11:16:00.000000 torcj-0.0.7/torcj.egg-info/top_level.txt
```

### Comparing `torcj-0.0.6/torcj/main.py` & `torcj-0.0.7/torcj/main.py`

 * *Files identical despite different names*

