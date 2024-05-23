# Comparing `tmp/live_score_api_com-0.1.tar.gz` & `tmp/live_score_api_com-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "live_score_api_com-0.1.tar", last modified: Sat May 18 05:48:11 2024, max compression
+gzip compressed data, was "live_score_api_com-1.0.tar", last modified: Thu May 23 16:15:19 2024, max compression
```

## Comparing `live_score_api_com-0.1.tar` & `live_score_api_com-1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 hristopetev   (501) staff       (20)        0 2024-05-18 05:48:11.098230 live_score_api_com-0.1/
--rw-r--r--   0 hristopetev   (501) staff       (20)      141 2024-05-18 05:48:11.097874 live_score_api_com-0.1/PKG-INFO
--rw-r--r--   0 hristopetev   (501) staff       (20)      432 2024-05-18 05:39:53.000000 live_score_api_com-0.1/README.md
-drwxr-xr-x   0 hristopetev   (501) staff       (20)        0 2024-05-18 05:48:11.096084 live_score_api_com-0.1/live_score_api_com/
--rw-r--r--   0 hristopetev   (501) staff       (20)       30 2024-05-17 12:07:22.000000 live_score_api_com-0.1/live_score_api_com/__init__.py
--rw-r--r--   0 hristopetev   (501) staff       (20)     1280 2024-05-17 12:07:22.000000 live_score_api_com-0.1/live_score_api_com/main.py
-drwxr-xr-x   0 hristopetev   (501) staff       (20)        0 2024-05-18 05:48:11.097472 live_score_api_com-0.1/live_score_api_com.egg-info/
--rw-r--r--   0 hristopetev   (501) staff       (20)      141 2024-05-18 05:48:11.000000 live_score_api_com-0.1/live_score_api_com.egg-info/PKG-INFO
--rw-r--r--   0 hristopetev   (501) staff       (20)      285 2024-05-18 05:48:11.000000 live_score_api_com-0.1/live_score_api_com.egg-info/SOURCES.txt
--rw-r--r--   0 hristopetev   (501) staff       (20)        1 2024-05-18 05:48:11.000000 live_score_api_com-0.1/live_score_api_com.egg-info/dependency_links.txt
--rw-r--r--   0 hristopetev   (501) staff       (20)        9 2024-05-18 05:48:11.000000 live_score_api_com-0.1/live_score_api_com.egg-info/requires.txt
--rw-r--r--   0 hristopetev   (501) staff       (20)       19 2024-05-18 05:48:11.000000 live_score_api_com-0.1/live_score_api_com.egg-info/top_level.txt
--rw-r--r--   0 hristopetev   (501) staff       (20)       38 2024-05-18 05:48:11.098323 live_score_api_com-0.1/setup.cfg
--rw-r--r--   0 hristopetev   (501) staff       (20)      168 2024-05-18 05:27:20.000000 live_score_api_com-0.1/setup.py
+drwxr-xr-x   0 hristopetev   (501) staff       (20)        0 2024-05-23 16:15:19.715423 live_score_api_com-1.0/
+-rw-r--r--   0 hristopetev   (501) staff       (20)      141 2024-05-23 16:15:19.713211 live_score_api_com-1.0/PKG-INFO
+-rw-r--r--   0 hristopetev   (501) staff       (20)      474 2024-05-23 15:36:49.000000 live_score_api_com-1.0/README.md
+drwxr-xr-x   0 hristopetev   (501) staff       (20)        0 2024-05-23 16:15:19.696661 live_score_api_com-1.0/live_score_api_com/
+-rw-r--r--   0 hristopetev   (501) staff       (20)       30 2024-05-23 15:36:49.000000 live_score_api_com-1.0/live_score_api_com/__init__.py
+-rw-r--r--   0 hristopetev   (501) staff       (20)     2738 2024-05-23 15:36:58.000000 live_score_api_com-1.0/live_score_api_com/main.py
+drwxr-xr-x   0 hristopetev   (501) staff       (20)        0 2024-05-23 16:15:19.710595 live_score_api_com-1.0/live_score_api_com.egg-info/
+-rw-r--r--   0 hristopetev   (501) staff       (20)      141 2024-05-23 16:15:19.000000 live_score_api_com-1.0/live_score_api_com.egg-info/PKG-INFO
+-rw-r--r--   0 hristopetev   (501) staff       (20)      285 2024-05-23 16:15:19.000000 live_score_api_com-1.0/live_score_api_com.egg-info/SOURCES.txt
+-rw-r--r--   0 hristopetev   (501) staff       (20)        1 2024-05-23 16:15:19.000000 live_score_api_com-1.0/live_score_api_com.egg-info/dependency_links.txt
+-rw-r--r--   0 hristopetev   (501) staff       (20)        9 2024-05-23 16:15:19.000000 live_score_api_com-1.0/live_score_api_com.egg-info/requires.txt
+-rw-r--r--   0 hristopetev   (501) staff       (20)       19 2024-05-23 16:15:19.000000 live_score_api_com-1.0/live_score_api_com.egg-info/top_level.txt
+-rw-r--r--   0 hristopetev   (501) staff       (20)       38 2024-05-23 16:15:19.716507 live_score_api_com-1.0/setup.cfg
+-rw-r--r--   0 hristopetev   (501) staff       (20)      168 2024-05-23 16:15:01.000000 live_score_api_com-1.0/setup.py
```

