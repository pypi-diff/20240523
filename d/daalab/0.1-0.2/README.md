# Comparing `tmp/daalab-0.1.tar.gz` & `tmp/daalab-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daalab-0.1.tar", last modified: Thu May 23 10:55:19 2024, max compression
+gzip compressed data, was "daalab-0.2.tar", last modified: Thu May 23 11:34:07 2024, max compression
```

## Comparing `daalab-0.1.tar` & `daalab-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 10:55:19.149698 daalab-0.1/
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-23 10:55:19.149558 daalab-0.1/PKG-INFO
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      568 2024-05-23 10:49:22.000000 daalab-0.1/README.md
-drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 10:55:19.148393 daalab-0.1/daalab/
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)       48 2024-05-23 10:44:33.000000 daalab-0.1/daalab/__init__.py
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      458 2024-05-23 10:44:25.000000 daalab-0.1/daalab/knapsack.py
-drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 10:55:19.149301 daalab-0.1/daalab.egg-info/
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-23 10:55:19.000000 daalab-0.1/daalab.egg-info/PKG-INFO
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      176 2024-05-23 10:55:19.000000 daalab-0.1/daalab.egg-info/SOURCES.txt
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        1 2024-05-23 10:55:19.000000 daalab-0.1/daalab.egg-info/dependency_links.txt
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        7 2024-05-23 10:55:19.000000 daalab-0.1/daalab.egg-info/top_level.txt
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)       38 2024-05-23 10:55:19.149760 daalab-0.1/setup.cfg
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      311 2024-05-23 10:55:08.000000 daalab-0.1/setup.py
+drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 11:34:07.298356 daalab-0.2/
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-23 11:34:07.298222 daalab-0.2/PKG-INFO
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      568 2024-05-23 10:49:22.000000 daalab-0.2/README.md
+drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 11:34:07.297394 daalab-0.2/daalab/
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      189 2024-05-23 11:29:39.000000 daalab-0.2/daalab/__init__.py
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)     5043 2024-05-23 11:32:05.000000 daalab-0.2/daalab/codes.py
+drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 11:34:07.298060 daalab-0.2/daalab.egg-info/
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-23 11:34:07.000000 daalab-0.2/daalab.egg-info/PKG-INFO
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      173 2024-05-23 11:34:07.000000 daalab-0.2/daalab.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        1 2024-05-23 11:34:07.000000 daalab-0.2/daalab.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        7 2024-05-23 11:34:07.000000 daalab-0.2/daalab.egg-info/top_level.txt
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)       38 2024-05-23 11:34:07.298406 daalab-0.2/setup.cfg
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      311 2024-05-23 11:33:15.000000 daalab-0.2/setup.py
```

### Comparing `daalab-0.1/README.md` & `daalab-0.2/README.md`

 * *Files identical despite different names*

