# Comparing `tmp/csle_ryu-0.5.3.tar.gz` & `tmp/csle_ryu-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_ryu-0.5.3.tar", last modified: Mon May 13 17:19:26 2024, max compression
+gzip compressed data, was "csle_ryu-0.6.0.tar", last modified: Thu May 23 17:43:02 2024, max compression
```

## Comparing `csle_ryu-0.5.3.tar` & `csle_ryu-0.6.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:26.090410 csle_ryu-0.5.3/
--rw-rw-r--   0 kim       (1000) kim       (1000)      629 2024-05-13 17:19:26.090410 csle_ryu-0.5.3/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     3869 2024-01-29 11:24:00.000000 csle_ryu-0.5.3/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      669 2023-08-08 14:54:06.000000 csle_ryu-0.5.3/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1798 2024-05-13 17:19:26.090410 csle_ryu-0.5.3/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_ryu-0.5.3/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:26.086410 csle_ryu-0.5.3/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:26.086410 csle_ryu-0.5.3/src/csle_ryu/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_ryu-0.5.3/src/csle_ryu/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-05-13 17:19:17.000000 csle_ryu-0.5.3/src/csle_ryu/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:26.086410 csle_ryu-0.5.3/src/csle_ryu/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_ryu-0.5.3/src/csle_ryu/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2484 2023-03-28 14:03:22.000000 csle_ryu-0.5.3/src/csle_ryu/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:26.086410 csle_ryu-0.5.3/src/csle_ryu/controllers/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_ryu-0.5.3/src/csle_ryu/controllers/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8327 2024-01-29 11:24:00.000000 csle_ryu-0.5.3/src/csle_ryu/controllers/learning_switch_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11778 2024-01-29 11:24:00.000000 csle_ryu-0.5.3/src/csle_ryu/controllers/learning_switch_stp_controller.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:26.090410 csle_ryu-0.5.3/src/csle_ryu/dao/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_ryu-0.5.3/src/csle_ryu/dao/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4127 2023-07-28 08:44:18.000000 csle_ryu-0.5.3/src/csle_ryu/dao/agg_flow_statistic.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8185 2023-07-28 08:44:18.000000 csle_ryu-0.5.3/src/csle_ryu/dao/avg_flow_statistic.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    14674 2023-07-28 08:44:18.000000 csle_ryu-0.5.3/src/csle_ryu/dao/avg_port_statistic.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6529 2023-07-28 08:44:18.000000 csle_ryu-0.5.3/src/csle_ryu/dao/flow_statistic.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10151 2023-07-28 08:44:18.000000 csle_ryu-0.5.3/src/csle_ryu/dao/port_statistic.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      253 2023-03-28 14:03:22.000000 csle_ryu-0.5.3/src/csle_ryu/dao/ryu_controller_type.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:26.090410 csle_ryu-0.5.3/src/csle_ryu/monitor/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_ryu-0.5.3/src/csle_ryu/monitor/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    15114 2024-01-29 11:24:00.000000 csle_ryu-0.5.3/src/csle_ryu/monitor/flow_and_port_stats_monitor.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:26.086410 csle_ryu-0.5.3/src/csle_ryu.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      629 2024-05-13 17:19:26.000000 csle_ryu-0.5.3/src/csle_ryu.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      914 2024-05-13 17:19:26.000000 csle_ryu-0.5.3/src/csle_ryu.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-05-13 17:19:26.000000 csle_ryu-0.5.3/src/csle_ryu.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:35:28.000000 csle_ryu-0.5.3/src/csle_ryu.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      565 2024-05-13 17:19:26.000000 csle_ryu-0.5.3/src/csle_ryu.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        9 2024-05-13 17:19:26.000000 csle_ryu-0.5.3/src/csle_ryu.egg-info/top_level.txt
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:26.090410 csle_ryu-0.5.3/tests/
--rw-rw-r--   0 kim       (1000) kim       (1000)      716 2024-01-29 11:24:00.000000 csle_ryu-0.5.3/tests/test_learning_switch_controller.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:02.035044 csle_ryu-0.6.0/
+-rw-r--r--   0 kim        (501) staff       (20)      629 2024-05-23 17:43:02.035088 csle_ryu-0.6.0/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)     3869 2024-02-13 12:24:16.000000 csle_ryu-0.6.0/README.md
+-rw-r--r--   0 kim        (501) staff       (20)      669 2023-08-15 10:44:03.000000 csle_ryu-0.6.0/pyproject.toml
+-rw-r--r--   0 kim        (501) staff       (20)     1798 2024-05-23 17:43:02.035343 csle_ryu-0.6.0/setup.cfg
+-rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_ryu-0.6.0/setup.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:02.029939 csle_ryu-0.6.0/src/
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:02.031168 csle_ryu-0.6.0/src/csle_ryu/
+-rw-r--r--   0 kim        (501) staff       (20)       37 2023-08-15 10:44:03.000000 csle_ryu-0.6.0/src/csle_ryu/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-23 17:42:57.000000 csle_ryu-0.6.0/src/csle_ryu/__version__.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:02.032205 csle_ryu-0.6.0/src/csle_ryu/constants/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_ryu-0.6.0/src/csle_ryu/constants/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     2484 2023-08-15 10:44:03.000000 csle_ryu-0.6.0/src/csle_ryu/constants/constants.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:02.032927 csle_ryu-0.6.0/src/csle_ryu/controllers/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_ryu-0.6.0/src/csle_ryu/controllers/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     8327 2023-09-20 12:38:03.000000 csle_ryu-0.6.0/src/csle_ryu/controllers/learning_switch_controller.py
+-rw-r--r--   0 kim        (501) staff       (20)    11778 2023-09-20 12:38:03.000000 csle_ryu-0.6.0/src/csle_ryu/controllers/learning_switch_stp_controller.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:02.034366 csle_ryu-0.6.0/src/csle_ryu/dao/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_ryu-0.6.0/src/csle_ryu/dao/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     4127 2023-08-15 10:44:03.000000 csle_ryu-0.6.0/src/csle_ryu/dao/agg_flow_statistic.py
+-rw-r--r--   0 kim        (501) staff       (20)     8185 2023-08-15 10:44:03.000000 csle_ryu-0.6.0/src/csle_ryu/dao/avg_flow_statistic.py
+-rw-r--r--   0 kim        (501) staff       (20)    14674 2023-08-15 10:44:03.000000 csle_ryu-0.6.0/src/csle_ryu/dao/avg_port_statistic.py
+-rw-r--r--   0 kim        (501) staff       (20)     6529 2023-08-15 10:44:03.000000 csle_ryu-0.6.0/src/csle_ryu/dao/flow_statistic.py
+-rw-r--r--   0 kim        (501) staff       (20)    10151 2023-08-15 10:44:03.000000 csle_ryu-0.6.0/src/csle_ryu/dao/port_statistic.py
+-rw-r--r--   0 kim        (501) staff       (20)      253 2023-08-15 10:44:03.000000 csle_ryu-0.6.0/src/csle_ryu/dao/ryu_controller_type.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:02.034610 csle_ryu-0.6.0/src/csle_ryu/monitor/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_ryu-0.6.0/src/csle_ryu/monitor/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)    15114 2023-09-20 12:38:03.000000 csle_ryu-0.6.0/src/csle_ryu/monitor/flow_and_port_stats_monitor.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:02.032011 csle_ryu-0.6.0/src/csle_ryu.egg-info/
+-rw-r--r--   0 kim        (501) staff       (20)      629 2024-05-23 17:43:02.000000 csle_ryu-0.6.0/src/csle_ryu.egg-info/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)      914 2024-05-23 17:43:02.000000 csle_ryu-0.6.0/src/csle_ryu.egg-info/SOURCES.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-23 17:43:02.000000 csle_ryu-0.6.0/src/csle_ryu.egg-info/dependency_links.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:39:24.000000 csle_ryu-0.6.0/src/csle_ryu.egg-info/not-zip-safe
+-rw-r--r--   0 kim        (501) staff       (20)      565 2024-05-23 17:43:02.000000 csle_ryu-0.6.0/src/csle_ryu.egg-info/requires.txt
+-rw-r--r--   0 kim        (501) staff       (20)        9 2024-05-23 17:43:02.000000 csle_ryu-0.6.0/src/csle_ryu.egg-info/top_level.txt
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:02.034765 csle_ryu-0.6.0/tests/
+-rw-r--r--   0 kim        (501) staff       (20)      716 2023-08-17 14:41:40.000000 csle_ryu-0.6.0/tests/test_learning_switch_controller.py
```

### Comparing `csle_ryu-0.5.3/PKG-INFO` & `csle_ryu-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_ryu
-Version: 0.5.3
+Version: 0.6.0
 Summary: RYU SDN Controllers in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_ryu-0.5.3/README.md` & `csle_ryu-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.5.3/pyproject.toml` & `csle_ryu-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.5.3/setup.cfg` & `csle_ryu-0.6.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-base>=0.5.3
-	csle-collector>=0.5.3
+	csle-base>=0.6.0
+	csle-collector>=0.6.0
 	csle-ryu-fork>=4.37.0.dev3357
 	dnspython==2.2.1
 	eventlet>=0.33.2
 	confluent-kafka>=1.9.2
 python_requires = >=3.8
 package_dir = 
 	=src
```

### Comparing `csle_ryu-0.5.3/src/csle_ryu/constants/constants.py` & `csle_ryu-0.6.0/src/csle_ryu/constants/constants.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.5.3/src/csle_ryu/controllers/learning_switch_controller.py` & `csle_ryu-0.6.0/src/csle_ryu/controllers/learning_switch_controller.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.5.3/src/csle_ryu/controllers/learning_switch_stp_controller.py` & `csle_ryu-0.6.0/src/csle_ryu/controllers/learning_switch_stp_controller.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.5.3/src/csle_ryu/dao/agg_flow_statistic.py` & `csle_ryu-0.6.0/src/csle_ryu/dao/agg_flow_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.5.3/src/csle_ryu/dao/avg_flow_statistic.py` & `csle_ryu-0.6.0/src/csle_ryu/dao/avg_flow_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.5.3/src/csle_ryu/dao/avg_port_statistic.py` & `csle_ryu-0.6.0/src/csle_ryu/dao/avg_port_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.5.3/src/csle_ryu/dao/flow_statistic.py` & `csle_ryu-0.6.0/src/csle_ryu/dao/flow_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.5.3/src/csle_ryu/dao/port_statistic.py` & `csle_ryu-0.6.0/src/csle_ryu/dao/port_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.5.3/src/csle_ryu/monitor/flow_and_port_stats_monitor.py` & `csle_ryu-0.6.0/src/csle_ryu/monitor/flow_and_port_stats_monitor.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.5.3/src/csle_ryu.egg-info/PKG-INFO` & `csle_ryu-0.6.0/src/csle_ryu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-ryu
-Version: 0.5.3
+Version: 0.6.0
 Summary: RYU SDN Controllers in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_ryu-0.5.3/src/csle_ryu.egg-info/SOURCES.txt` & `csle_ryu-0.6.0/src/csle_ryu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.5.3/src/csle_ryu.egg-info/requires.txt` & `csle_ryu-0.6.0/src/csle_ryu.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-csle-base>=0.5.3
-csle-collector>=0.5.3
+csle-base>=0.6.0
+csle-collector>=0.6.0
 csle-ryu-fork>=4.37.0.dev3357
 dnspython==2.2.1
 eventlet>=0.33.2
 confluent-kafka>=1.9.2
 
 [testing]
 pytest>=6.0
```

### Comparing `csle_ryu-0.5.3/tests/test_learning_switch_controller.py` & `csle_ryu-0.6.0/tests/test_learning_switch_controller.py`

 * *Files identical despite different names*

