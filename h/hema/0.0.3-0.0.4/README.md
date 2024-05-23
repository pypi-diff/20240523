# Comparing `tmp/hema-0.0.3.tar.gz` & `tmp/hema-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hema-0.0.3.tar", last modified: Thu May 23 08:58:02 2024, max compression
+gzip compressed data, was "hema-0.0.4.tar", last modified: Thu May 23 09:02:11 2024, max compression
```

## Comparing `hema-0.0.3.tar` & `hema-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,25 @@
-drwxr-xr-x   0 qinhanhou   (501) staff       (20)        0 2024-05-23 08:58:02.762207 hema-0.0.3/
--rw-r--r--   0 qinhanhou   (501) staff       (20)      243 2024-05-23 08:58:02.761916 hema-0.0.3/PKG-INFO
-drwxr-xr-x   0 qinhanhou   (501) staff       (20)        0 2024-05-23 08:58:02.760378 hema-0.0.3/hema/
--rw-r--r--   0 qinhanhou   (501) staff       (20)        0 2024-05-23 08:53:50.000000 hema-0.0.3/hema/__init__.py
-drwxr-xr-x   0 qinhanhou   (501) staff       (20)        0 2024-05-23 08:58:02.761221 hema-0.0.3/hema/models/
--rw-r--r--   0 qinhanhou   (501) staff       (20)       16 2024-05-23 08:50:47.000000 hema-0.0.3/hema/models/__init__.py
-drwxr-xr-x   0 qinhanhou   (501) staff       (20)        0 2024-05-23 08:58:02.761650 hema-0.0.3/hema.egg-info/
--rw-r--r--   0 qinhanhou   (501) staff       (20)      243 2024-05-23 08:58:02.000000 hema-0.0.3/hema.egg-info/PKG-INFO
--rw-r--r--   0 qinhanhou   (501) staff       (20)      188 2024-05-23 08:58:02.000000 hema-0.0.3/hema.egg-info/SOURCES.txt
--rw-r--r--   0 qinhanhou   (501) staff       (20)        1 2024-05-23 08:58:02.000000 hema-0.0.3/hema.egg-info/dependency_links.txt
--rw-r--r--   0 qinhanhou   (501) staff       (20)       29 2024-05-23 08:58:02.000000 hema-0.0.3/hema.egg-info/requires.txt
--rw-r--r--   0 qinhanhou   (501) staff       (20)        5 2024-05-23 08:58:02.000000 hema-0.0.3/hema.egg-info/top_level.txt
--rw-r--r--   0 qinhanhou   (501) staff       (20)       38 2024-05-23 08:58:02.762257 hema-0.0.3/setup.cfg
--rw-r--r--   0 qinhanhou   (501) staff       (20)      414 2024-05-23 08:57:11.000000 hema-0.0.3/setup.py
+drwxr-xr-x   0 qinhanhou   (501) staff       (20)        0 2024-05-23 09:02:11.011281 hema-0.0.4/
+-rw-r--r--   0 qinhanhou   (501) staff       (20)      243 2024-05-23 09:02:11.010962 hema-0.0.4/PKG-INFO
+drwxr-xr-x   0 qinhanhou   (501) staff       (20)        0 2024-05-23 09:02:11.006308 hema-0.0.4/hema/
+-rw-r--r--   0 qinhanhou   (501) staff       (20)        0 2024-05-23 08:53:50.000000 hema-0.0.4/hema/__init__.py
+drwxr-xr-x   0 qinhanhou   (501) staff       (20)        0 2024-05-23 09:02:11.007117 hema-0.0.4/hema/models/
+-rw-r--r--   0 qinhanhou   (501) staff       (20)       16 2024-05-23 08:50:47.000000 hema-0.0.4/hema/models/__init__.py
+drwxr-xr-x   0 qinhanhou   (501) staff       (20)        0 2024-05-23 09:02:11.010080 hema-0.0.4/hema/models/conformer/
+-rw-r--r--   0 qinhanhou   (501) staff       (20)        0 2024-05-23 09:01:30.000000 hema-0.0.4/hema/models/conformer/__init__.py
+-rw-r--r--   0 qinhanhou   (501) staff       (20)      935 2024-05-21 10:37:02.000000 hema-0.0.4/hema/models/conformer/activation.py
+-rw-r--r--   0 qinhanhou   (501) staff       (20)     5864 2024-05-21 17:22:09.000000 hema-0.0.4/hema/models/conformer/attention.py
+-rw-r--r--   0 qinhanhou   (501) staff       (20)     1277 2024-05-21 17:23:23.000000 hema-0.0.4/hema/models/conformer/basic.py
+-rw-r--r--   0 qinhanhou   (501) staff       (20)        0 2024-05-21 10:37:02.000000 hema-0.0.4/hema/models/conformer/conformer.py
+-rw-r--r--   0 qinhanhou   (501) staff       (20)     4978 2024-05-21 10:37:02.000000 hema-0.0.4/hema/models/conformer/convolution.py
+-rw-r--r--   0 qinhanhou   (501) staff       (20)     2008 2024-05-21 10:41:20.000000 hema-0.0.4/hema/models/conformer/embedding.py
+-rw-r--r--   0 qinhanhou   (501) staff       (20)     8085 2024-05-21 17:22:49.000000 hema-0.0.4/hema/models/conformer/encoder.py
+-rw-r--r--   0 qinhanhou   (501) staff       (20)     1458 2024-05-21 10:44:02.000000 hema-0.0.4/hema/models/conformer/feedforward.py
+-rw-r--r--   0 qinhanhou   (501) staff       (20)     4168 2024-05-21 17:27:08.000000 hema-0.0.4/hema/models/conformer/model.py
+drwxr-xr-x   0 qinhanhou   (501) staff       (20)        0 2024-05-23 09:02:11.010555 hema-0.0.4/hema.egg-info/
+-rw-r--r--   0 qinhanhou   (501) staff       (20)      243 2024-05-23 09:02:10.000000 hema-0.0.4/hema.egg-info/PKG-INFO
+-rw-r--r--   0 qinhanhou   (501) staff       (20)      532 2024-05-23 09:02:11.000000 hema-0.0.4/hema.egg-info/SOURCES.txt
+-rw-r--r--   0 qinhanhou   (501) staff       (20)        1 2024-05-23 09:02:10.000000 hema-0.0.4/hema.egg-info/dependency_links.txt
+-rw-r--r--   0 qinhanhou   (501) staff       (20)       29 2024-05-23 09:02:10.000000 hema-0.0.4/hema.egg-info/requires.txt
+-rw-r--r--   0 qinhanhou   (501) staff       (20)        5 2024-05-23 09:02:10.000000 hema-0.0.4/hema.egg-info/top_level.txt
+-rw-r--r--   0 qinhanhou   (501) staff       (20)       38 2024-05-23 09:02:11.011330 hema-0.0.4/setup.cfg
+-rw-r--r--   0 qinhanhou   (501) staff       (20)      414 2024-05-23 09:01:41.000000 hema-0.0.4/setup.py
```

