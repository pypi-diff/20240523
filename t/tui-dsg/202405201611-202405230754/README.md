# Comparing `tmp/tui_dsg-202405201611.tar.gz` & `tmp/tui_dsg-202405230754.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui_dsg-202405201611.tar", last modified: Mon May 20 16:11:40 2024, max compression
+gzip compressed data, was "tui_dsg-202405230754.tar", last modified: Thu May 23 07:54:01 2024, max compression
```

## Comparing `tui_dsg-202405201611.tar` & `tui_dsg-202405230754.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 16:11:40.497300 tui_dsg-202405201611/
--rw-r--r--   0 root         (0) root         (0)     1188 2024-05-20 16:11:40.493300 tui_dsg-202405201611/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 16:11:40.497300 tui_dsg-202405201611/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1524 2024-05-20 14:34:34.000000 tui_dsg-202405201611/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 16:11:40.493300 tui_dsg-202405201611/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 16:11:40.493300 tui_dsg-202405201611/src/tui_dsg/
--rw-rw-rw-   0 root         (0) root         (0)        5 2024-05-20 07:56:05.000000 tui_dsg-202405201611/src/tui_dsg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 16:11:40.493300 tui_dsg-202405201611/src/tui_dsg.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1188 2024-05-20 16:11:40.000000 tui_dsg-202405201611/src/tui_dsg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      206 2024-05-20 16:11:40.000000 tui_dsg-202405201611/src/tui_dsg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 16:11:40.000000 tui_dsg-202405201611/src/tui_dsg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      348 2024-05-20 16:11:40.000000 tui_dsg-202405201611/src/tui_dsg.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-20 16:11:40.000000 tui_dsg-202405201611/src/tui_dsg.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:54:01.643395 tui_dsg-202405230754/
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-05-23 07:54:01.643395 tui_dsg-202405230754/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 07:54:01.643395 tui_dsg-202405230754/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1524 2024-05-20 14:34:34.000000 tui_dsg-202405230754/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:54:01.639395 tui_dsg-202405230754/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:54:01.639395 tui_dsg-202405230754/src/tui_dsg/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2024-05-20 07:56:05.000000 tui_dsg-202405230754/src/tui_dsg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:54:01.643395 tui_dsg-202405230754/src/tui_dsg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-05-23 07:54:01.000000 tui_dsg-202405230754/src/tui_dsg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      206 2024-05-23 07:54:01.000000 tui_dsg-202405230754/src/tui_dsg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 07:54:01.000000 tui_dsg-202405230754/src/tui_dsg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      348 2024-05-23 07:54:01.000000 tui_dsg-202405230754/src/tui_dsg.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-23 07:54:01.000000 tui_dsg-202405230754/src/tui_dsg.egg-info/top_level.txt
```

### Comparing `tui_dsg-202405201611/PKG-INFO` & `tui_dsg-202405230754/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsg
-Version: 202405201611
+Version: 202405230754
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-grundlagen
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tui_dsg-202405201611/setup.py` & `tui_dsg-202405230754/setup.py`

 * *Files identical despite different names*

### Comparing `tui_dsg-202405201611/src/tui_dsg.egg-info/PKG-INFO` & `tui_dsg-202405230754/src/tui_dsg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsg
-Version: 202405201611
+Version: 202405230754
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-grundlagen
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

