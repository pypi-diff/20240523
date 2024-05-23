# Comparing `tmp/hema-0.0.2.tar.gz` & `tmp/hema-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hema-0.0.2.tar", last modified: Tue May 21 17:34:21 2024, max compression
+gzip compressed data, was "hema-0.0.3.tar", last modified: Thu May 23 08:58:02 2024, max compression
```

## Comparing `hema-0.0.2.tar` & `hema-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 qinhanhou   (501) staff       (20)        0 2024-05-21 17:34:21.296753 hema-0.0.2/
--rw-r--r--   0 qinhanhou   (501) staff       (20)      243 2024-05-21 17:34:21.296487 hema-0.0.2/PKG-INFO
-drwxr-xr-x   0 qinhanhou   (501) staff       (20)        0 2024-05-21 17:34:21.296226 hema-0.0.2/hema.egg-info/
--rw-r--r--   0 qinhanhou   (501) staff       (20)      243 2024-05-21 17:34:21.000000 hema-0.0.2/hema.egg-info/PKG-INFO
--rw-r--r--   0 qinhanhou   (501) staff       (20)      166 2024-05-21 17:34:21.000000 hema-0.0.2/hema.egg-info/SOURCES.txt
--rw-r--r--   0 qinhanhou   (501) staff       (20)        1 2024-05-21 17:34:21.000000 hema-0.0.2/hema.egg-info/dependency_links.txt
--rw-r--r--   0 qinhanhou   (501) staff       (20)       29 2024-05-21 17:34:21.000000 hema-0.0.2/hema.egg-info/requires.txt
--rw-r--r--   0 qinhanhou   (501) staff       (20)        7 2024-05-21 17:34:21.000000 hema-0.0.2/hema.egg-info/top_level.txt
-drwxr-xr-x   0 qinhanhou   (501) staff       (20)        0 2024-05-21 17:34:21.296052 hema-0.0.2/models/
--rw-r--r--   0 qinhanhou   (501) staff       (20)        0 2024-05-21 10:37:02.000000 hema-0.0.2/models/__init__.py
--rw-r--r--   0 qinhanhou   (501) staff       (20)       38 2024-05-21 17:34:21.296798 hema-0.0.2/setup.cfg
--rw-r--r--   0 qinhanhou   (501) staff       (20)      414 2024-05-21 17:34:18.000000 hema-0.0.2/setup.py
+drwxr-xr-x   0 qinhanhou   (501) staff       (20)        0 2024-05-23 08:58:02.762207 hema-0.0.3/
+-rw-r--r--   0 qinhanhou   (501) staff       (20)      243 2024-05-23 08:58:02.761916 hema-0.0.3/PKG-INFO
+drwxr-xr-x   0 qinhanhou   (501) staff       (20)        0 2024-05-23 08:58:02.760378 hema-0.0.3/hema/
+-rw-r--r--   0 qinhanhou   (501) staff       (20)        0 2024-05-23 08:53:50.000000 hema-0.0.3/hema/__init__.py
+drwxr-xr-x   0 qinhanhou   (501) staff       (20)        0 2024-05-23 08:58:02.761221 hema-0.0.3/hema/models/
+-rw-r--r--   0 qinhanhou   (501) staff       (20)       16 2024-05-23 08:50:47.000000 hema-0.0.3/hema/models/__init__.py
+drwxr-xr-x   0 qinhanhou   (501) staff       (20)        0 2024-05-23 08:58:02.761650 hema-0.0.3/hema.egg-info/
+-rw-r--r--   0 qinhanhou   (501) staff       (20)      243 2024-05-23 08:58:02.000000 hema-0.0.3/hema.egg-info/PKG-INFO
+-rw-r--r--   0 qinhanhou   (501) staff       (20)      188 2024-05-23 08:58:02.000000 hema-0.0.3/hema.egg-info/SOURCES.txt
+-rw-r--r--   0 qinhanhou   (501) staff       (20)        1 2024-05-23 08:58:02.000000 hema-0.0.3/hema.egg-info/dependency_links.txt
+-rw-r--r--   0 qinhanhou   (501) staff       (20)       29 2024-05-23 08:58:02.000000 hema-0.0.3/hema.egg-info/requires.txt
+-rw-r--r--   0 qinhanhou   (501) staff       (20)        5 2024-05-23 08:58:02.000000 hema-0.0.3/hema.egg-info/top_level.txt
+-rw-r--r--   0 qinhanhou   (501) staff       (20)       38 2024-05-23 08:58:02.762257 hema-0.0.3/setup.cfg
+-rw-r--r--   0 qinhanhou   (501) staff       (20)      414 2024-05-23 08:57:11.000000 hema-0.0.3/setup.py
```

