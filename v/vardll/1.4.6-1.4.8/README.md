# Comparing `tmp/vardll-1.4.6.tar.gz` & `tmp/vardll-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vardll-1.4.6.tar", last modified: Wed May 22 20:46:56 2024, max compression
+gzip compressed data, was "vardll-1.4.8.tar", last modified: Thu May 23 21:27:18 2024, max compression
```

## Comparing `vardll-1.4.6.tar` & `vardll-1.4.8.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 20:46:56.245805 vardll-1.4.6/
--rw-rw-rw-   0        0        0      280 2024-05-22 20:46:56.242224 vardll-1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     1103 2024-05-15 20:32:47.000000 vardll-1.4.6/license
--rw-rw-rw-   0        0        0       42 2024-05-22 20:46:56.246772 vardll-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0      507 2024-05-22 20:46:42.000000 vardll-1.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 20:46:56.239635 vardll-1.4.6/vardll.egg-info/
--rw-rw-rw-   0        0        0      280 2024-05-22 20:46:55.000000 vardll-1.4.6/vardll.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      169 2024-05-22 20:46:55.000000 vardll-1.4.6/vardll.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 20:46:55.000000 vardll-1.4.6/vardll.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-22 20:46:55.000000 vardll-1.4.6/vardll.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 20:46:55.000000 vardll-1.4.6/vardll.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 21:27:18.943946 vardll-1.4.8/
+-rw-rw-rw-   0        0        0     1422 2024-05-23 21:27:18.940945 vardll-1.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1103 2024-05-15 20:32:47.000000 vardll-1.4.8/license
+-rw-rw-rw-   0        0        0       42 2024-05-23 21:27:18.944947 vardll-1.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      748 2024-05-23 21:26:48.000000 vardll-1.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:27:18.937946 vardll-1.4.8/vardll.egg-info/
+-rw-rw-rw-   0        0        0     1422 2024-05-23 21:27:18.000000 vardll-1.4.8/vardll.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      136 2024-05-23 21:27:18.000000 vardll-1.4.8/vardll.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 21:27:18.000000 vardll-1.4.8/vardll.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 21:27:18.000000 vardll-1.4.8/vardll.egg-info/top_level.txt
```

### Comparing `vardll-1.4.6/license` & `vardll-1.4.8/license`

 * *Files identical despite different names*

