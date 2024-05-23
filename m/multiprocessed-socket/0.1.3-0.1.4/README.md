# Comparing `tmp/multiprocessed-socket-0.1.3.tar.gz` & `tmp/multiprocessed-socket-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiprocessed-socket-0.1.3.tar", last modified: Thu May 23 03:25:52 2024, max compression
+gzip compressed data, was "multiprocessed-socket-0.1.4.tar", last modified: Thu May 23 03:26:39 2024, max compression
```

## Comparing `multiprocessed-socket-0.1.3.tar` & `multiprocessed-socket-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 03:25:52.738818 multiprocessed-socket-0.1.3/
--rw-rw-rw-   0        0        0      400 2024-05-23 03:25:52.737818 multiprocessed-socket-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       23 2024-05-23 03:07:15.000000 multiprocessed-socket-0.1.3/README.md
--rw-rw-rw-   0        0        0     1091 2024-05-23 03:07:57.000000 multiprocessed-socket-0.1.3/license.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 03:25:52.716819 multiprocessed-socket-0.1.3/multiprocessed_socket/
--rw-rw-rw-   0        0        0     8563 2024-05-23 02:55:22.000000 multiprocessed-socket-0.1.3/multiprocessed_socket/multiprocessed-socket.py
-drwxrwxrwx   0        0        0        0 2024-05-23 03:25:52.735817 multiprocessed-socket-0.1.3/multiprocessed_socket.egg-info/
--rw-rw-rw-   0        0        0      400 2024-05-23 03:25:52.000000 multiprocessed-socket-0.1.3/multiprocessed_socket.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2024-05-23 03:25:52.000000 multiprocessed-socket-0.1.3/multiprocessed_socket.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 03:25:52.000000 multiprocessed-socket-0.1.3/multiprocessed_socket.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-23 03:25:52.000000 multiprocessed-socket-0.1.3/multiprocessed_socket.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 03:25:52.000000 multiprocessed-socket-0.1.3/multiprocessed_socket.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 03:25:52.739818 multiprocessed-socket-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      446 2024-05-23 03:25:43.000000 multiprocessed-socket-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:26:39.127634 multiprocessed-socket-0.1.4/
+-rw-rw-rw-   0        0        0      400 2024-05-23 03:26:39.125636 multiprocessed-socket-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       23 2024-05-23 03:07:15.000000 multiprocessed-socket-0.1.4/README.md
+-rw-rw-rw-   0        0        0     1091 2024-05-23 03:07:57.000000 multiprocessed-socket-0.1.4/license.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 03:26:39.112635 multiprocessed-socket-0.1.4/multiprocessed_socket/
+-rw-rw-rw-   0        0        0     8563 2024-05-23 02:55:22.000000 multiprocessed-socket-0.1.4/multiprocessed_socket/multiprocessed-socket.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:26:39.124635 multiprocessed-socket-0.1.4/multiprocessed_socket.egg-info/
+-rw-rw-rw-   0        0        0      400 2024-05-23 03:26:38.000000 multiprocessed-socket-0.1.4/multiprocessed_socket.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2024-05-23 03:26:39.000000 multiprocessed-socket-0.1.4/multiprocessed_socket.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 03:26:38.000000 multiprocessed-socket-0.1.4/multiprocessed_socket.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 03:26:38.000000 multiprocessed-socket-0.1.4/multiprocessed_socket.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 03:26:38.000000 multiprocessed-socket-0.1.4/multiprocessed_socket.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 03:26:39.127634 multiprocessed-socket-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      446 2024-05-23 03:26:32.000000 multiprocessed-socket-0.1.4/setup.py
```

### Comparing `multiprocessed-socket-0.1.3/license.txt` & `multiprocessed-socket-0.1.4/license.txt`

 * *Files identical despite different names*

### Comparing `multiprocessed-socket-0.1.3/multiprocessed_socket/multiprocessed-socket.py` & `multiprocessed-socket-0.1.4/multiprocessed_socket/multiprocessed-socket.py`

 * *Files identical despite different names*

