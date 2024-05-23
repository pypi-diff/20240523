# Comparing `tmp/legopack-0.1.tar.gz` & `tmp/legopack-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legopack-0.1.tar", last modified: Wed Jan 24 09:26:32 2024, max compression
+gzip compressed data, was "legopack-0.11.tar", last modified: Thu May 23 14:04:32 2024, max compression
```

## Comparing `legopack-0.1.tar` & `legopack-0.11.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0 remi      (1000) remi      (1000)        0 2024-01-24 09:26:32.875981 legopack-0.1/
--rwxrwxrwx   0 remi      (1000) remi      (1000)      143 2024-01-24 09:26:32.869981 legopack-0.1/PKG-INFO
--rwxrwxrwx   0 remi      (1000) remi      (1000)       29 2024-01-24 07:43:04.000000 legopack-0.1/README.md
-drwxrwxrwx   0 remi      (1000) remi      (1000)        0 2024-01-24 09:26:32.689075 legopack-0.1/legopack/
--rwxrwxrwx   0 remi      (1000) remi      (1000)        0 2024-01-24 07:51:07.000000 legopack-0.1/legopack/__init__.py
-drwxrwxrwx   0 remi      (1000) remi      (1000)        0 2024-01-24 09:26:32.839100 legopack-0.1/legopack/models/
--rwxrwxrwx   0 remi      (1000) remi      (1000)        0 2024-01-24 08:06:16.000000 legopack-0.1/legopack/models/__init__.py
--rwxrwxrwx   0 remi      (1000) remi      (1000)     5718 2024-01-24 07:59:56.000000 legopack-0.1/legopack/models/custom.py
--rwxrwxrwx   0 remi      (1000) remi      (1000)     2807 2024-01-24 07:58:27.000000 legopack-0.1/legopack/models/iforestasd.py
-drwxrwxrwx   0 remi      (1000) remi      (1000)        0 2024-01-24 09:26:32.862147 legopack-0.1/legopack.egg-info/
--rwxrwxrwx   0 remi      (1000) remi      (1000)      143 2024-01-24 09:26:32.000000 legopack-0.1/legopack.egg-info/PKG-INFO
--rwxrwxrwx   0 remi      (1000) remi      (1000)      313 2024-01-24 09:26:32.000000 legopack-0.1/legopack.egg-info/SOURCES.txt
--rwxrwxrwx   0 remi      (1000) remi      (1000)        1 2024-01-24 09:26:32.000000 legopack-0.1/legopack.egg-info/dependency_links.txt
--rwxrwxrwx   0 remi      (1000) remi      (1000)        1 2024-01-24 08:32:20.000000 legopack-0.1/legopack.egg-info/not-zip-safe
--rwxrwxrwx   0 remi      (1000) remi      (1000)       28 2024-01-24 09:26:32.000000 legopack-0.1/legopack.egg-info/requires.txt
--rwxrwxrwx   0 remi      (1000) remi      (1000)        9 2024-01-24 09:26:32.000000 legopack-0.1/legopack.egg-info/top_level.txt
--rwxrwxrwx   0 remi      (1000) remi      (1000)       38 2024-01-24 09:26:32.876980 legopack-0.1/setup.cfg
--rwxrwxrwx   0 remi      (1000) remi      (1000)      280 2024-01-24 08:11:24.000000 legopack-0.1/setup.py
+drwxrwxrwx   0 remi      (1000) remi      (1000)        0 2024-05-23 14:04:32.308826 legopack-0.11/
+-rwxrwxrwx   0 remi      (1000) remi      (1000)      258 2024-05-23 14:04:32.306825 legopack-0.11/PKG-INFO
+-rwxrwxrwx   0 remi      (1000) remi      (1000)       29 2024-01-24 07:43:04.000000 legopack-0.11/README.md
+drwxrwxrwx   0 remi      (1000) remi      (1000)        0 2024-05-23 14:04:32.163431 legopack-0.11/legopack/
+-rwxrwxrwx   0 remi      (1000) remi      (1000)        0 2024-01-24 07:51:07.000000 legopack-0.11/legopack/__init__.py
+drwxrwxrwx   0 remi      (1000) remi      (1000)        0 2024-05-23 14:04:32.289658 legopack-0.11/legopack/models/
+-rwxrwxrwx   0 remi      (1000) remi      (1000)        0 2024-01-24 08:06:16.000000 legopack-0.11/legopack/models/__init__.py
+-rwxrwxrwx   0 remi      (1000) remi      (1000)     2738 2024-03-12 13:16:21.000000 legopack-0.11/legopack/models/adaptators.py
+-rwxrwxrwx   0 remi      (1000) remi      (1000)    13360 2024-03-14 16:39:31.000000 legopack-0.11/legopack/models/custom.py
+-rwxrwxrwx   0 remi      (1000) remi      (1000)     3907 2024-03-25 10:52:20.000000 legopack-0.11/legopack/tools.py
+drwxrwxrwx   0 remi      (1000) remi      (1000)        0 2024-05-23 14:04:32.244450 legopack-0.11/legopack.egg-info/
+-rwxrwxrwx   0 remi      (1000) remi      (1000)      258 2024-05-23 14:04:31.000000 legopack-0.11/legopack.egg-info/PKG-INFO
+-rwxrwxrwx   0 remi      (1000) remi      (1000)      331 2024-05-23 14:04:32.000000 legopack-0.11/legopack.egg-info/SOURCES.txt
+-rwxrwxrwx   0 remi      (1000) remi      (1000)        1 2024-05-23 14:04:31.000000 legopack-0.11/legopack.egg-info/dependency_links.txt
+-rwxrwxrwx   0 remi      (1000) remi      (1000)        1 2024-01-24 08:32:20.000000 legopack-0.11/legopack.egg-info/not-zip-safe
+-rwxrwxrwx   0 remi      (1000) remi      (1000)       28 2024-05-23 14:04:31.000000 legopack-0.11/legopack.egg-info/requires.txt
+-rwxrwxrwx   0 remi      (1000) remi      (1000)        9 2024-05-23 14:04:32.000000 legopack-0.11/legopack.egg-info/top_level.txt
+-rwxrwxrwx   0 remi      (1000) remi      (1000)       38 2024-05-23 14:04:32.309826 legopack-0.11/setup.cfg
+-rwxrwxrwx   0 remi      (1000) remi      (1000)      541 2024-05-23 14:04:25.000000 legopack-0.11/setup.py
```

