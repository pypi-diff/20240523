# Comparing `tmp/gym_csle_intrusion_response_game-0.5.3.tar.gz` & `tmp/gym_csle_intrusion_response_game-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym_csle_intrusion_response_game-0.5.3.tar", last modified: Mon May 13 17:20:10 2024, max compression
+gzip compressed data, was "gym_csle_intrusion_response_game-0.6.0.tar", last modified: Thu May 23 17:43:30 2024, max compression
```

## Comparing `gym_csle_intrusion_response_game-0.5.3.tar` & `gym_csle_intrusion_response_game-0.6.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:10.986685 gym_csle_intrusion_response_game-0.5.3/
--rw-rw-r--   0 kim       (1000) kim       (1000)      709 2024-05-13 17:20:10.986685 gym_csle_intrusion_response_game-0.5.3/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      713 2023-08-08 14:54:06.000000 gym_csle_intrusion_response_game-0.5.3/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1918 2024-05-13 17:20:10.986685 gym_csle_intrusion_response_game-0.5.3/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.5.3/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:10.982685 gym_csle_intrusion_response_game-0.5.3/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:10.982685 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/
--rw-rw-r--   0 kim       (1000) kim       (1000)     1479 2023-04-23 07:07:00.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-05-13 17:19:17.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:10.982685 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1841 2023-04-30 06:59:23.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:10.986685 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4661 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_attacker_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4392 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_defender_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4160 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_state_local.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6988 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/local_intrusion_response_game_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5336 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_game_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3445 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_attacker_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3445 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_defender_config.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:10.986685 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/
--rw-rw-r--   0 kim       (1000) kim       (1000)      749 2023-04-23 07:07:00.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    15417 2024-01-29 12:14:49.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_attacker.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    18684 2024-04-30 09:37:30.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_defender.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    14261 2024-01-29 12:14:49.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_stopping_pomdp_defender.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    13470 2024-01-29 12:14:49.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_attacker.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    17124 2024-01-29 12:14:49.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_defender.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:10.986685 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/util/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/util/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    55338 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/util/intrusion_response_game_util.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:10.982685 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      709 2024-05-13 17:20:10.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     1979 2024-05-13 17:20:10.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-05-13 17:20:10.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 11:24:24.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      557 2024-05-13 17:20:10.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       33 2024-05-13 17:20:10.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game.egg-info/top_level.txt
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:10.986685 gym_csle_intrusion_response_game-0.5.3/tests/
--rw-rw-r--   0 kim       (1000) kim       (1000)      732 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.3/tests/test_intrusion_response_game_util.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:30.945248 gym_csle_intrusion_response_game-0.6.0/
+-rw-r--r--   0 kim        (501) staff       (20)      709 2024-05-23 17:43:30.945358 gym_csle_intrusion_response_game-0.6.0/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)      713 2023-08-15 10:44:03.000000 gym_csle_intrusion_response_game-0.6.0/pyproject.toml
+-rw-r--r--   0 kim        (501) staff       (20)     1918 2024-05-23 17:43:30.945829 gym_csle_intrusion_response_game-0.6.0/setup.cfg
+-rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 gym_csle_intrusion_response_game-0.6.0/setup.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:30.921289 gym_csle_intrusion_response_game-0.6.0/src/
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:30.929751 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/
+-rw-r--r--   0 kim        (501) staff       (20)     1479 2023-08-15 10:44:03.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-23 17:42:57.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/__version__.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:30.934420 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/constants/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/constants/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     1841 2023-08-15 10:44:03.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/constants/constants.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:30.938228 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/dao/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/dao/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     4661 2023-08-15 10:44:03.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_attacker_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     4392 2023-08-15 10:44:03.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_defender_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     4160 2023-08-15 10:44:03.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_state_local.py
+-rw-r--r--   0 kim        (501) staff       (20)     6988 2023-09-14 08:32:02.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/dao/local_intrusion_response_game_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     5336 2023-09-14 08:41:35.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_game_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     3445 2023-08-15 10:44:03.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_attacker_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     3445 2023-08-15 10:44:03.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_defender_config.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:30.941266 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/envs/
+-rw-r--r--   0 kim        (501) staff       (20)      749 2023-08-15 10:44:03.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/envs/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)    15417 2024-02-13 12:24:16.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_attacker.py
+-rw-r--r--   0 kim        (501) staff       (20)    18684 2024-03-05 13:14:43.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_defender.py
+-rw-r--r--   0 kim        (501) staff       (20)    14261 2024-02-13 12:24:16.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_stopping_pomdp_defender.py
+-rw-r--r--   0 kim        (501) staff       (20)    13470 2024-02-13 12:24:16.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_attacker.py
+-rw-r--r--   0 kim        (501) staff       (20)    17124 2024-02-13 12:24:16.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_defender.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:30.942062 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/util/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/util/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)    55338 2023-08-15 10:44:03.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/util/intrusion_response_game_util.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:30.933043 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game.egg-info/
+-rw-r--r--   0 kim        (501) staff       (20)      709 2024-05-23 17:43:30.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game.egg-info/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)     1979 2024-05-23 17:43:30.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game.egg-info/SOURCES.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-23 17:43:30.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game.egg-info/dependency_links.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:40:10.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game.egg-info/not-zip-safe
+-rw-r--r--   0 kim        (501) staff       (20)      557 2024-05-23 17:43:30.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game.egg-info/requires.txt
+-rw-r--r--   0 kim        (501) staff       (20)       33 2024-05-23 17:43:30.000000 gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game.egg-info/top_level.txt
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:30.944654 gym_csle_intrusion_response_game-0.6.0/tests/
+-rw-r--r--   0 kim        (501) staff       (20)      732 2023-08-17 15:07:57.000000 gym_csle_intrusion_response_game-0.6.0/tests/test_intrusion_response_game_util.py
```

### Comparing `gym_csle_intrusion_response_game-0.5.3/PKG-INFO` & `gym_csle_intrusion_response_game-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym_csle_intrusion_response_game
-Version: 0.5.3
+Version: 0.6.0
 Summary: OpenAI gym reinforcement learning environment of an intrusion response game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_intrusion_response_game-0.5.3/pyproject.toml` & `gym_csle_intrusion_response_game-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.3/setup.cfg` & `gym_csle_intrusion_response_game-0.6.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	gymnasium>=0.27.1
-	csle-base>=0.5.3
-	csle-common>=0.5.3
-	csle-attacker>=0.5.3
-	csle-defender>=0.5.3
-	csle-collector>=0.5.3
+	csle-base>=0.6.0
+	csle-common>=0.6.0
+	csle-attacker>=0.6.0
+	csle-defender>=0.6.0
+	csle-collector>=0.6.0
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/__init__.py` & `gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/__init__.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/constants/constants.py` & `gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/constants/constants.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_attacker_config.py` & `gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_attacker_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_defender_config.py` & `gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_defender_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_state_local.py` & `gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_state_local.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/local_intrusion_response_game_config.py` & `gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/dao/local_intrusion_response_game_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_game_config.py` & `gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_game_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_attacker_config.py` & `gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_attacker_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_defender_config.py` & `gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_defender_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/__init__.py` & `gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_attacker.py` & `gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_attacker.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_defender.py` & `gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_defender.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_stopping_pomdp_defender.py` & `gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_stopping_pomdp_defender.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_attacker.py` & `gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_attacker.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_defender.py` & `gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_defender.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/util/intrusion_response_game_util.py` & `gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game/util/intrusion_response_game_util.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game.egg-info/PKG-INFO` & `gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-csle-intrusion-response-game
-Version: 0.5.3
+Version: 0.6.0
 Summary: OpenAI gym reinforcement learning environment of an intrusion response game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game.egg-info/SOURCES.txt` & `gym_csle_intrusion_response_game-0.6.0/src/gym_csle_intrusion_response_game.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.3/tests/test_intrusion_response_game_util.py` & `gym_csle_intrusion_response_game-0.6.0/tests/test_intrusion_response_game_util.py`

 * *Files identical despite different names*

