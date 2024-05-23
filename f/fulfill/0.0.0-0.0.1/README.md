# Comparing `tmp/fulfill-0.0.0.tar.gz` & `tmp/fulfill-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fulfill-0.0.0.tar", last modified: Thu May 23 12:00:36 2024, max compression
+gzip compressed data, was "fulfill-0.0.1.tar", last modified: Thu May 23 12:18:54 2024, max compression
```

## Comparing `fulfill-0.0.0.tar` & `fulfill-0.0.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
-drwxr-xr-x   0 pawamoy   (1000) users      (985)        0 2024-05-23 12:00:36.216504 fulfill-0.0.0/
--rw-r--r--   0 pawamoy   (1000) users      (985)      490 2024-05-23 12:00:36.216504 fulfill-0.0.0/PKG-INFO
--rw-r--r--   0 pawamoy   (1000) users      (985)      195 2024-05-23 12:00:30.000000 fulfill-0.0.0/README.md
-drwxr-xr-x   0 pawamoy   (1000) users      (985)        0 2024-05-23 12:00:36.213171 fulfill-0.0.0/fulfill.egg-info/
--rw-r--r--   0 pawamoy   (1000) users      (985)      490 2024-05-23 12:00:36.000000 fulfill-0.0.0/fulfill.egg-info/PKG-INFO
--rw-r--r--   0 pawamoy   (1000) users      (985)      148 2024-05-23 12:00:36.000000 fulfill-0.0.0/fulfill.egg-info/SOURCES.txt
--rw-r--r--   0 pawamoy   (1000) users      (985)        1 2024-05-23 12:00:36.000000 fulfill-0.0.0/fulfill.egg-info/dependency_links.txt
--rw-r--r--   0 pawamoy   (1000) users      (985)        1 2024-05-23 12:00:36.000000 fulfill-0.0.0/fulfill.egg-info/top_level.txt
--rw-r--r--   0 pawamoy   (1000) users      (985)      303 2024-05-23 12:00:30.000000 fulfill-0.0.0/pyproject.toml
--rw-r--r--   0 pawamoy   (1000) users      (985)       38 2024-05-23 12:00:36.216504 fulfill-0.0.0/setup.cfg
+-rw-r--r--   0        0        0      754 2024-05-23 12:06:50.912853 fulfill-0.0.1/LICENSE
+-rw-r--r--   0        0        0      826 2024-05-23 12:06:50.919519 fulfill-0.0.1/README.md
+-rw-r--r--   0        0        0     1685 2024-05-23 12:18:54.854150 fulfill-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      128 2024-05-23 12:06:50.996185 fulfill-0.0.1/src/fulfill/__init__.py
+-rw-r--r--   0        0        0      339 2024-05-23 12:06:51.006185 fulfill-0.0.1/src/fulfill/__main__.py
+-rw-r--r--   0        0        0     1721 2024-05-23 12:06:51.009518 fulfill-0.0.1/src/fulfill/cli.py
+-rw-r--r--   0        0        0     2822 2024-05-23 12:06:50.999518 fulfill-0.0.1/src/fulfill/debug.py
+-rw-r--r--   0        0        0        0 2024-05-23 12:06:51.002852 fulfill-0.0.1/src/fulfill/py.typed
+-rw-r--r--   0        0        0     2213 1970-01-01 00:00:00.000000 fulfill-0.0.1/PKG-INFO
```

