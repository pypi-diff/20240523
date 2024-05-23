# Comparing `tmp/multiprocessed-socket-0.1.1.tar.gz` & `tmp/multiprocessed-socket-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiprocessed-socket-0.1.1.tar", last modified: Thu May 23 03:19:25 2024, max compression
+gzip compressed data, was "multiprocessed-socket-0.1.2.tar", last modified: Thu May 23 03:24:17 2024, max compression
```

## Comparing `multiprocessed-socket-0.1.1.tar` & `multiprocessed-socket-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 03:19:25.883231 multiprocessed-socket-0.1.1/
--rw-rw-rw-   0        0        0      400 2024-05-23 03:19:25.881229 multiprocessed-socket-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       23 2024-05-23 03:07:15.000000 multiprocessed-socket-0.1.1/README.md
--rw-rw-rw-   0        0        0     1091 2024-05-23 03:07:57.000000 multiprocessed-socket-0.1.1/license.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 03:19:25.870229 multiprocessed-socket-0.1.1/multiprocessed_socket/
--rw-rw-rw-   0        0        0       45 2024-05-23 03:18:37.000000 multiprocessed-socket-0.1.1/multiprocessed_socket/__init__.py
--rw-rw-rw-   0        0        0     8563 2024-05-23 02:55:22.000000 multiprocessed-socket-0.1.1/multiprocessed_socket/multiprocessed-socket.py
-drwxrwxrwx   0        0        0        0 2024-05-23 03:19:25.880231 multiprocessed-socket-0.1.1/multiprocessed_socket.egg-info/
--rw-rw-rw-   0        0        0      400 2024-05-23 03:19:25.000000 multiprocessed-socket-0.1.1/multiprocessed_socket.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2024-05-23 03:19:25.000000 multiprocessed-socket-0.1.1/multiprocessed_socket.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 03:19:25.000000 multiprocessed-socket-0.1.1/multiprocessed_socket.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-23 03:19:25.000000 multiprocessed-socket-0.1.1/multiprocessed_socket.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-05-23 03:19:25.000000 multiprocessed-socket-0.1.1/multiprocessed_socket.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 03:19:25.883231 multiprocessed-socket-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      446 2024-05-23 03:19:14.000000 multiprocessed-socket-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:24:17.275550 multiprocessed-socket-0.1.2/
+-rw-rw-rw-   0        0        0      400 2024-05-23 03:24:17.273550 multiprocessed-socket-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       23 2024-05-23 03:07:15.000000 multiprocessed-socket-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1091 2024-05-23 03:07:57.000000 multiprocessed-socket-0.1.2/license.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 03:24:17.253549 multiprocessed-socket-0.1.2/multiprocessed_socket/
+-rw-rw-rw-   0        0        0       28 2024-05-23 03:24:01.000000 multiprocessed-socket-0.1.2/multiprocessed_socket/__init__.py
+-rw-rw-rw-   0        0        0     8563 2024-05-23 02:55:22.000000 multiprocessed-socket-0.1.2/multiprocessed_socket/multiprocessed-socket.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:24:17.272551 multiprocessed-socket-0.1.2/multiprocessed_socket.egg-info/
+-rw-rw-rw-   0        0        0      400 2024-05-23 03:24:17.000000 multiprocessed-socket-0.1.2/multiprocessed_socket.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-05-23 03:24:17.000000 multiprocessed-socket-0.1.2/multiprocessed_socket.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 03:24:17.000000 multiprocessed-socket-0.1.2/multiprocessed_socket.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 03:24:17.000000 multiprocessed-socket-0.1.2/multiprocessed_socket.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-23 03:24:17.000000 multiprocessed-socket-0.1.2/multiprocessed_socket.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 03:24:17.275550 multiprocessed-socket-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      446 2024-05-23 03:24:15.000000 multiprocessed-socket-0.1.2/setup.py
```

### Comparing `multiprocessed-socket-0.1.1/license.txt` & `multiprocessed-socket-0.1.2/license.txt`

 * *Files identical despite different names*

### Comparing `multiprocessed-socket-0.1.1/multiprocessed_socket/multiprocessed-socket.py` & `multiprocessed-socket-0.1.2/multiprocessed_socket/multiprocessed-socket.py`

 * *Files identical despite different names*

