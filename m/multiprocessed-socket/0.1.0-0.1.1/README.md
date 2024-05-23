# Comparing `tmp/multiprocessed-socket-0.1.0.tar.gz` & `tmp/multiprocessed-socket-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiprocessed-socket-0.1.0.tar", last modified: Thu May 23 03:04:00 2024, max compression
+gzip compressed data, was "multiprocessed-socket-0.1.1.tar", last modified: Thu May 23 03:19:25 2024, max compression
```

## Comparing `multiprocessed-socket-0.1.0.tar` & `multiprocessed-socket-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 03:04:00.380854 multiprocessed-socket-0.1.0/
--rw-rw-rw-   0        0        0      373 2024-05-23 03:04:00.378854 multiprocessed-socket-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-23 03:04:00.377855 multiprocessed-socket-0.1.0/multiprocessed_socket.egg-info/
--rw-rw-rw-   0        0        0      373 2024-05-23 03:04:00.000000 multiprocessed-socket-0.1.0/multiprocessed_socket.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2024-05-23 03:04:00.000000 multiprocessed-socket-0.1.0/multiprocessed_socket.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 03:04:00.000000 multiprocessed-socket-0.1.0/multiprocessed_socket.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-23 03:04:00.000000 multiprocessed-socket-0.1.0/multiprocessed_socket.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 03:04:00.000000 multiprocessed-socket-0.1.0/multiprocessed_socket.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 03:04:00.380854 multiprocessed-socket-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      446 2024-05-23 02:59:46.000000 multiprocessed-socket-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:19:25.883231 multiprocessed-socket-0.1.1/
+-rw-rw-rw-   0        0        0      400 2024-05-23 03:19:25.881229 multiprocessed-socket-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       23 2024-05-23 03:07:15.000000 multiprocessed-socket-0.1.1/README.md
+-rw-rw-rw-   0        0        0     1091 2024-05-23 03:07:57.000000 multiprocessed-socket-0.1.1/license.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 03:19:25.870229 multiprocessed-socket-0.1.1/multiprocessed_socket/
+-rw-rw-rw-   0        0        0       45 2024-05-23 03:18:37.000000 multiprocessed-socket-0.1.1/multiprocessed_socket/__init__.py
+-rw-rw-rw-   0        0        0     8563 2024-05-23 02:55:22.000000 multiprocessed-socket-0.1.1/multiprocessed_socket/multiprocessed-socket.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:19:25.880231 multiprocessed-socket-0.1.1/multiprocessed_socket.egg-info/
+-rw-rw-rw-   0        0        0      400 2024-05-23 03:19:25.000000 multiprocessed-socket-0.1.1/multiprocessed_socket.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-05-23 03:19:25.000000 multiprocessed-socket-0.1.1/multiprocessed_socket.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 03:19:25.000000 multiprocessed-socket-0.1.1/multiprocessed_socket.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 03:19:25.000000 multiprocessed-socket-0.1.1/multiprocessed_socket.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-23 03:19:25.000000 multiprocessed-socket-0.1.1/multiprocessed_socket.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 03:19:25.883231 multiprocessed-socket-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      446 2024-05-23 03:19:14.000000 multiprocessed-socket-0.1.1/setup.py
```

