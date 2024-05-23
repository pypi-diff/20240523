# Comparing `tmp/csle_cluster-0.5.3.tar.gz` & `tmp/csle_cluster-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_cluster-0.5.3.tar", last modified: Mon May 13 17:20:39 2024, max compression
+gzip compressed data, was "csle_cluster-0.6.0.tar", last modified: Thu May 23 17:43:47 2024, max compression
```

## Comparing `csle_cluster-0.5.3.tar` & `csle_cluster-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:39.978861 csle_cluster-0.5.3/
--rw-rw-r--   0 kim       (1000) kim       (1000)      794 2024-05-13 17:20:39.978861 csle_cluster-0.5.3/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     4307 2024-01-29 12:14:49.000000 csle_cluster-0.5.3/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      672 2023-08-08 14:54:06.000000 csle_cluster-0.5.3/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     2067 2024-05-13 17:20:39.978861 csle_cluster-0.5.3/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_cluster-0.5.3/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:39.970861 csle_cluster-0.5.3/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:39.970861 csle_cluster-0.5.3/src/csle_cluster/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_cluster-0.5.3/src/csle_cluster/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-05-13 17:19:17.000000 csle_cluster-0.5.3/src/csle_cluster/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:39.974861 csle_cluster-0.5.3/src/csle_cluster/cluster_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_cluster-0.5.3/src/csle_cluster/cluster_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   240982 2024-04-30 09:37:30.000000 csle_cluster-0.5.3/src/csle_cluster/cluster_manager/cluster_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   270830 2024-05-13 17:10:17.000000 csle_cluster-0.5.3/src/csle_cluster/cluster_manager/cluster_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    94763 2024-01-29 11:24:00.000000 csle_cluster-0.5.3/src/csle_cluster/cluster_manager/cluster_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   349493 2024-01-29 11:24:00.000000 csle_cluster-0.5.3/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   207915 2024-01-29 11:24:00.000000 csle_cluster-0.5.3/src/csle_cluster/cluster_manager/cluster_manager_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   204861 2024-01-29 11:24:00.000000 csle_cluster-0.5.3/src/csle_cluster/cluster_manager/query_cluster_manager.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:39.978861 csle_cluster-0.5.3/src/csle_cluster/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_cluster-0.5.3/src/csle_cluster/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      459 2023-08-08 14:54:06.000000 csle_cluster-0.5.3/src/csle_cluster/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:39.970861 csle_cluster-0.5.3/src/csle_cluster.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      794 2024-05-13 17:20:39.000000 csle_cluster-0.5.3/src/csle_cluster.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      835 2024-05-13 17:20:39.000000 csle_cluster-0.5.3/src/csle_cluster.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-05-13 17:20:39.000000 csle_cluster-0.5.3/src/csle_cluster.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-04 13:33:55.000000 csle_cluster-0.5.3/src/csle_cluster.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      689 2024-05-13 17:20:39.000000 csle_cluster-0.5.3/src/csle_cluster.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       13 2024-05-13 17:20:39.000000 csle_cluster-0.5.3/src/csle_cluster.egg-info/top_level.txt
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:39.978861 csle_cluster-0.5.3/tests/
--rw-rw-r--   0 kim       (1000) kim       (1000)   355781 2024-01-29 11:24:00.000000 csle_cluster-0.5.3/tests/test_cluster_manager.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:47.503430 csle_cluster-0.6.0/
+-rw-r--r--   0 kim        (501) staff       (20)      794 2024-05-23 17:43:47.503475 csle_cluster-0.6.0/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)     4307 2024-02-13 12:24:16.000000 csle_cluster-0.6.0/README.md
+-rw-r--r--   0 kim        (501) staff       (20)      672 2023-08-15 10:44:03.000000 csle_cluster-0.6.0/pyproject.toml
+-rw-r--r--   0 kim        (501) staff       (20)     2067 2024-05-23 17:43:47.503723 csle_cluster-0.6.0/setup.cfg
+-rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_cluster-0.6.0/setup.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:47.496249 csle_cluster-0.6.0/src/
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:47.497146 csle_cluster-0.6.0/src/csle_cluster/
+-rw-r--r--   0 kim        (501) staff       (20)       37 2023-08-15 10:44:03.000000 csle_cluster-0.6.0/src/csle_cluster/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-23 17:42:57.000000 csle_cluster-0.6.0/src/csle_cluster/__version__.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:47.501578 csle_cluster-0.6.0/src/csle_cluster/cluster_manager/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_cluster-0.6.0/src/csle_cluster/cluster_manager/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)   240982 2024-04-10 18:29:55.000000 csle_cluster-0.6.0/src/csle_cluster/cluster_manager/cluster_controller.py
+-rw-r--r--   0 kim        (501) staff       (20)   270830 2024-04-17 08:32:22.000000 csle_cluster-0.6.0/src/csle_cluster/cluster_manager/cluster_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)    94763 2023-08-26 08:04:28.000000 csle_cluster-0.6.0/src/csle_cluster/cluster_manager/cluster_manager_pb2.py
+-rw-r--r--   0 kim        (501) staff       (20)   349493 2023-08-26 08:04:28.000000 csle_cluster-0.6.0/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py
+-rw-r--r--   0 kim        (501) staff       (20)   207915 2023-08-26 08:04:28.000000 csle_cluster-0.6.0/src/csle_cluster/cluster_manager/cluster_manager_util.py
+-rw-r--r--   0 kim        (501) staff       (20)   204861 2023-08-23 08:52:10.000000 csle_cluster-0.6.0/src/csle_cluster/cluster_manager/query_cluster_manager.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:47.502430 csle_cluster-0.6.0/src/csle_cluster/constants/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_cluster-0.6.0/src/csle_cluster/constants/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)      459 2023-08-15 10:44:03.000000 csle_cluster-0.6.0/src/csle_cluster/constants/constants.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:47.498040 csle_cluster-0.6.0/src/csle_cluster.egg-info/
+-rw-r--r--   0 kim        (501) staff       (20)      794 2024-05-23 17:43:47.000000 csle_cluster-0.6.0/src/csle_cluster.egg-info/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)      835 2024-05-23 17:43:47.000000 csle_cluster-0.6.0/src/csle_cluster.egg-info/SOURCES.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-23 17:43:47.000000 csle_cluster-0.6.0/src/csle_cluster.egg-info/dependency_links.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:40:37.000000 csle_cluster-0.6.0/src/csle_cluster.egg-info/not-zip-safe
+-rw-r--r--   0 kim        (501) staff       (20)      689 2024-05-23 17:43:47.000000 csle_cluster-0.6.0/src/csle_cluster.egg-info/requires.txt
+-rw-r--r--   0 kim        (501) staff       (20)       13 2024-05-23 17:43:47.000000 csle_cluster-0.6.0/src/csle_cluster.egg-info/top_level.txt
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:47.502668 csle_cluster-0.6.0/tests/
+-rw-r--r--   0 kim        (501) staff       (20)   355781 2023-08-30 12:52:39.000000 csle_cluster-0.6.0/tests/test_cluster_manager.py
```

### Comparing `csle_cluster-0.5.3/PKG-INFO` & `csle_cluster-0.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_cluster
-Version: 0.5.3
+Version: 0.6.0
 Summary: Scripts for cluster management in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cluster-0.5.3/README.md` & `csle_cluster-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.5.3/pyproject.toml` & `csle_cluster-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.5.3/setup.cfg` & `csle_cluster-0.6.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	grpcio>=1.57.0
 	grpcio-tools>=1.57.0
-	csle-base>=0.5.3
-	csle-collector>=0.5.3
-	csle-common>=0.5.3
-	csle-ryu>=0.5.3
-	gym-csle-stopping-game>=0.5.3
-	gym-csle-intrusion-response-game>=0.5.3
-	gym-csle-apt-game>=0.5.3
-	gym-csle-cyborg>=0.5.3
-	csle-tolerance>=0.5.3
+	csle-base>=0.6.0
+	csle-collector>=0.6.0
+	csle-common>=0.6.0
+	csle-ryu>=0.6.0
+	gym-csle-stopping-game>=0.6.0
+	gym-csle-intrusion-response-game>=0.6.0
+	gym-csle-apt-game>=0.6.0
+	gym-csle-cyborg>=0.6.0
+	csle-tolerance>=0.6.0
 python_requires = >=3.5
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_cluster-0.5.3/src/csle_cluster/cluster_manager/cluster_controller.py` & `csle_cluster-0.6.0/src/csle_cluster/cluster_manager/cluster_controller.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.5.3/src/csle_cluster/cluster_manager/cluster_manager.py` & `csle_cluster-0.6.0/src/csle_cluster/cluster_manager/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.5.3/src/csle_cluster/cluster_manager/cluster_manager_pb2.py` & `csle_cluster-0.6.0/src/csle_cluster/cluster_manager/cluster_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.5.3/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py` & `csle_cluster-0.6.0/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.5.3/src/csle_cluster/cluster_manager/cluster_manager_util.py` & `csle_cluster-0.6.0/src/csle_cluster/cluster_manager/cluster_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.5.3/src/csle_cluster/cluster_manager/query_cluster_manager.py` & `csle_cluster-0.6.0/src/csle_cluster/cluster_manager/query_cluster_manager.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.5.3/src/csle_cluster.egg-info/PKG-INFO` & `csle_cluster-0.6.0/src/csle_cluster.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-cluster
-Version: 0.5.3
+Version: 0.6.0
 Summary: Scripts for cluster management in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cluster-0.5.3/src/csle_cluster.egg-info/SOURCES.txt` & `csle_cluster-0.6.0/src/csle_cluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.5.3/tests/test_cluster_manager.py` & `csle_cluster-0.6.0/tests/test_cluster_manager.py`

 * *Files identical despite different names*

