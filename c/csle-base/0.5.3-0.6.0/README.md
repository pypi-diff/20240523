# Comparing `tmp/csle_base-0.5.3.tar.gz` & `tmp/csle_base-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_base-0.5.3.tar", last modified: Mon May 13 17:19:20 2024, max compression
+gzip compressed data, was "csle_base-0.6.0.tar", last modified: Thu May 23 17:42:59 2024, max compression
```

## Comparing `csle_base-0.5.3.tar` & `csle_base-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:20.102373 csle_base-0.5.3/
--rw-rw-r--   0 kim       (1000) kim       (1000)      653 2024-05-13 17:19:20.102373 csle_base-0.5.3/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     3716 2024-01-29 11:24:00.000000 csle_base-0.5.3/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      670 2023-08-08 14:54:06.000000 csle_base-0.5.3/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1671 2024-05-13 17:19:20.102373 csle_base-0.5.3/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_base-0.5.3/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:20.098373 csle_base-0.5.3/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:20.102373 csle_base-0.5.3/src/csle_base/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_base-0.5.3/src/csle_base/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-05-13 17:19:17.000000 csle_base-0.5.3/src/csle_base/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:20.102373 csle_base-0.5.3/src/csle_base/encoding/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_base-0.5.3/src/csle_base/encoding/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      571 2024-01-29 11:24:00.000000 csle_base-0.5.3/src/csle_base/encoding/np_encoder.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      574 2023-06-13 15:27:33.000000 csle_base-0.5.3/src/csle_base/grpc_serializable.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2017 2024-01-29 11:24:00.000000 csle_base-0.5.3/src/csle_base/json_serializable.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      713 2023-06-13 15:27:33.000000 csle_base-0.5.3/src/csle_base/kafka_serializable.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:20.102373 csle_base-0.5.3/src/csle_base.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      653 2024-05-13 17:19:20.000000 csle_base-0.5.3/src/csle_base.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      496 2024-05-13 17:19:20.000000 csle_base-0.5.3/src/csle_base.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-05-13 17:19:20.000000 csle_base-0.5.3/src/csle_base.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-10 13:43:53.000000 csle_base-0.5.3/src/csle_base.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      439 2024-05-13 17:19:20.000000 csle_base-0.5.3/src/csle_base.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       10 2024-05-13 17:19:20.000000 csle_base-0.5.3/src/csle_base.egg-info/top_level.txt
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:42:59.172580 csle_base-0.6.0/
+-rw-r--r--   0 kim        (501) staff       (20)      653 2024-05-23 17:42:59.172632 csle_base-0.6.0/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)     3716 2024-02-13 12:24:16.000000 csle_base-0.6.0/README.md
+-rw-r--r--   0 kim        (501) staff       (20)      670 2023-08-15 10:44:03.000000 csle_base-0.6.0/pyproject.toml
+-rw-r--r--   0 kim        (501) staff       (20)     1671 2024-05-23 17:42:59.172871 csle_base-0.6.0/setup.cfg
+-rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_base-0.6.0/setup.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:42:59.169776 csle_base-0.6.0/src/
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:42:59.171297 csle_base-0.6.0/src/csle_base/
+-rw-r--r--   0 kim        (501) staff       (20)       37 2023-08-15 10:44:03.000000 csle_base-0.6.0/src/csle_base/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-23 17:42:57.000000 csle_base-0.6.0/src/csle_base/__version__.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:42:59.172335 csle_base-0.6.0/src/csle_base/encoding/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-09-14 08:14:52.000000 csle_base-0.6.0/src/csle_base/encoding/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)      571 2023-09-14 08:14:52.000000 csle_base-0.6.0/src/csle_base/encoding/np_encoder.py
+-rw-r--r--   0 kim        (501) staff       (20)      574 2023-08-15 10:44:03.000000 csle_base-0.6.0/src/csle_base/grpc_serializable.py
+-rw-r--r--   0 kim        (501) staff       (20)     2017 2023-09-14 08:14:52.000000 csle_base-0.6.0/src/csle_base/json_serializable.py
+-rw-r--r--   0 kim        (501) staff       (20)      713 2023-08-15 10:44:03.000000 csle_base-0.6.0/src/csle_base/kafka_serializable.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:42:59.172155 csle_base-0.6.0/src/csle_base.egg-info/
+-rw-r--r--   0 kim        (501) staff       (20)      653 2024-05-23 17:42:59.000000 csle_base-0.6.0/src/csle_base.egg-info/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)      496 2024-05-23 17:42:59.000000 csle_base-0.6.0/src/csle_base.egg-info/SOURCES.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-23 17:42:59.000000 csle_base-0.6.0/src/csle_base.egg-info/dependency_links.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:39:18.000000 csle_base-0.6.0/src/csle_base.egg-info/not-zip-safe
+-rw-r--r--   0 kim        (501) staff       (20)      439 2024-05-23 17:42:59.000000 csle_base-0.6.0/src/csle_base.egg-info/requires.txt
+-rw-r--r--   0 kim        (501) staff       (20)       10 2024-05-23 17:42:59.000000 csle_base-0.6.0/src/csle_base.egg-info/top_level.txt
```

### Comparing `csle_base-0.5.3/PKG-INFO` & `csle_base-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_base
-Version: 0.5.3
+Version: 0.6.0
 Summary: Library with base classes and definitions for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_base-0.5.3/README.md` & `csle_base-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `csle_base-0.5.3/pyproject.toml` & `csle_base-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_base-0.5.3/setup.cfg` & `csle_base-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `csle_base-0.5.3/src/csle_base/encoding/np_encoder.py` & `csle_base-0.6.0/src/csle_base/encoding/np_encoder.py`

 * *Files identical despite different names*

### Comparing `csle_base-0.5.3/src/csle_base/grpc_serializable.py` & `csle_base-0.6.0/src/csle_base/grpc_serializable.py`

 * *Files identical despite different names*

### Comparing `csle_base-0.5.3/src/csle_base/json_serializable.py` & `csle_base-0.6.0/src/csle_base/json_serializable.py`

 * *Files identical despite different names*

### Comparing `csle_base-0.5.3/src/csle_base/kafka_serializable.py` & `csle_base-0.6.0/src/csle_base/kafka_serializable.py`

 * *Files identical despite different names*

### Comparing `csle_base-0.5.3/src/csle_base.egg-info/PKG-INFO` & `csle_base-0.6.0/src/csle_base.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-base
-Version: 0.5.3
+Version: 0.6.0
 Summary: Library with base classes and definitions for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

