# Comparing `tmp/daalab-0.3.tar.gz` & `tmp/daalab-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daalab-0.3.tar", last modified: Thu May 23 12:31:46 2024, max compression
+gzip compressed data, was "daalab-0.4.tar", last modified: Thu May 23 12:48:48 2024, max compression
```

## Comparing `daalab-0.3.tar` & `daalab-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 12:31:46.126523 daalab-0.3/
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-23 12:31:46.126368 daalab-0.3/PKG-INFO
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      568 2024-05-23 10:49:22.000000 daalab-0.3/README.md
-drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 12:31:46.125509 daalab-0.3/daalab/
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)     2020 2024-05-23 12:30:29.000000 daalab-0.3/daalab/__init__.py
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)    21976 2024-05-23 12:30:57.000000 daalab-0.3/daalab/codes.py
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)     1281 2024-05-23 12:02:22.000000 daalab-0.3/daalab/testing.py
-drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 12:31:46.126185 daalab-0.3/daalab.egg-info/
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-23 12:31:46.000000 daalab-0.3/daalab.egg-info/PKG-INFO
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      191 2024-05-23 12:31:46.000000 daalab-0.3/daalab.egg-info/SOURCES.txt
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        1 2024-05-23 12:31:46.000000 daalab-0.3/daalab.egg-info/dependency_links.txt
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        7 2024-05-23 12:31:46.000000 daalab-0.3/daalab.egg-info/top_level.txt
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)       38 2024-05-23 12:31:46.126574 daalab-0.3/setup.cfg
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      311 2024-05-23 12:31:24.000000 daalab-0.3/setup.py
+drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 12:48:48.041705 daalab-0.4/
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-23 12:48:48.041432 daalab-0.4/PKG-INFO
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      568 2024-05-23 10:49:22.000000 daalab-0.4/README.md
+drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 12:48:48.039838 daalab-0.4/daalab/
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)     2030 2024-05-23 12:44:31.000000 daalab-0.4/daalab/__init__.py
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)    21976 2024-05-23 12:30:57.000000 daalab-0.4/daalab/codes.py
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)     1330 2024-05-23 12:39:22.000000 daalab-0.4/daalab/testing.py
+drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 12:48:48.041125 daalab-0.4/daalab.egg-info/
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-23 12:48:48.000000 daalab-0.4/daalab.egg-info/PKG-INFO
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      191 2024-05-23 12:48:48.000000 daalab-0.4/daalab.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        1 2024-05-23 12:48:48.000000 daalab-0.4/daalab.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        7 2024-05-23 12:48:48.000000 daalab-0.4/daalab.egg-info/top_level.txt
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)       38 2024-05-23 12:48:48.041760 daalab-0.4/setup.cfg
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      269 2024-05-23 12:47:43.000000 daalab-0.4/setup.py
```

### Comparing `daalab-0.3/README.md` & `daalab-0.4/README.md`

 * *Files identical despite different names*

### Comparing `daalab-0.3/daalab/codes.py` & `daalab-0.4/daalab/codes.py`

 * *Files identical despite different names*

