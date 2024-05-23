# Comparing `tmp/gym_csle_stopping_game-0.5.3.tar.gz` & `tmp/gym_csle_stopping_game-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym_csle_stopping_game-0.5.3.tar", last modified: Mon May 13 17:20:00 2024, max compression
+gzip compressed data, was "gym_csle_stopping_game-0.6.0.tar", last modified: Thu May 23 17:43:22 2024, max compression
```

## Comparing `gym_csle_stopping_game-0.5.3.tar` & `gym_csle_stopping_game-0.6.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:00.386620 gym_csle_stopping_game-0.5.3/
--rw-rw-r--   0 kim       (1000) kim       (1000)      705 2024-05-13 17:20:00.386620 gym_csle_stopping_game-0.5.3/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      703 2023-08-08 14:54:06.000000 gym_csle_stopping_game-0.5.3/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1894 2024-05-13 17:20:00.386620 gym_csle_stopping_game-0.5.3/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.5.3/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:00.382620 gym_csle_stopping_game-0.5.3/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:00.382620 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/
--rw-rw-r--   0 kim       (1000) kim       (1000)      657 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-05-13 17:19:17.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:00.382620 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1030 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:00.386620 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/dao/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/dao/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3494 2024-04-30 03:46:58.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6640 2024-04-30 09:37:30.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/dao/stopping_game_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3753 2024-04-30 03:46:58.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2828 2024-04-30 03:46:58.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/dao/stopping_game_state.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:00.386620 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/envs/
--rw-rw-r--   0 kim       (1000) kim       (1000)       74 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/envs/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    22753 2024-04-30 09:37:30.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/envs/stopping_game_env.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10877 2024-04-30 09:37:30.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10580 2024-04-30 09:37:30.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:00.386620 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/util/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/util/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11363 2024-04-30 09:37:30.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/util/stopping_game_util.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:00.382620 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      705 2024-05-13 17:20:00.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     1195 2024-05-13 17:20:00.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-05-13 17:20:00.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:50:52.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      557 2024-05-13 17:20:00.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       23 2024-05-13 17:20:00.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game.egg-info/top_level.txt
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:00.386620 gym_csle_stopping_game-0.5.3/tests/
--rw-rw-r--   0 kim       (1000) kim       (1000)     4825 2024-01-29 12:14:49.000000 gym_csle_stopping_game-0.5.3/tests/test_stopping_game_dao.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8353 2024-01-29 12:14:49.000000 gym_csle_stopping_game-0.5.3/tests/test_stopping_game_util.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:22.623604 gym_csle_stopping_game-0.6.0/
+-rw-r--r--   0 kim        (501) staff       (20)      705 2024-05-23 17:43:22.623698 gym_csle_stopping_game-0.6.0/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)      703 2023-08-15 10:44:03.000000 gym_csle_stopping_game-0.6.0/pyproject.toml
+-rw-r--r--   0 kim        (501) staff       (20)     1894 2024-05-23 17:43:22.624115 gym_csle_stopping_game-0.6.0/setup.cfg
+-rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 gym_csle_stopping_game-0.6.0/setup.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:22.607828 gym_csle_stopping_game-0.6.0/src/
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:22.612750 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/
+-rw-r--r--   0 kim        (501) staff       (20)      657 2023-09-15 16:41:55.000000 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-23 17:42:57.000000 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/__version__.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:22.616626 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/constants/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/constants/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     1030 2023-08-15 10:44:03.000000 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/constants/constants.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:22.619200 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/dao/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:04.000000 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/dao/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     3494 2024-05-04 07:32:27.000000 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     6640 2024-05-04 07:32:27.000000 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/dao/stopping_game_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     3753 2024-05-04 07:32:27.000000 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     2828 2024-05-04 07:32:27.000000 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/dao/stopping_game_state.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:22.621364 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/envs/
+-rw-r--r--   0 kim        (501) staff       (20)       74 2023-08-15 10:44:04.000000 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/envs/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)    22753 2024-05-04 07:32:27.000000 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/envs/stopping_game_env.py
+-rw-r--r--   0 kim        (501) staff       (20)    10877 2024-03-05 13:14:47.000000 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py
+-rw-r--r--   0 kim        (501) staff       (20)    10580 2024-05-04 07:32:27.000000 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:22.622037 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/util/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:04.000000 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/util/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)    11363 2024-05-04 07:32:27.000000 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/util/stopping_game_util.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:22.615945 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game.egg-info/
+-rw-r--r--   0 kim        (501) staff       (20)      705 2024-05-23 17:43:22.000000 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game.egg-info/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)     1195 2024-05-23 17:43:22.000000 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game.egg-info/SOURCES.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-23 17:43:22.000000 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game.egg-info/dependency_links.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:40:00.000000 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game.egg-info/not-zip-safe
+-rw-r--r--   0 kim        (501) staff       (20)      557 2024-05-23 17:43:22.000000 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game.egg-info/requires.txt
+-rw-r--r--   0 kim        (501) staff       (20)       23 2024-05-23 17:43:22.000000 gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game.egg-info/top_level.txt
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:22.623101 gym_csle_stopping_game-0.6.0/tests/
+-rw-r--r--   0 kim        (501) staff       (20)     4825 2024-02-13 12:24:16.000000 gym_csle_stopping_game-0.6.0/tests/test_stopping_game_dao.py
+-rw-r--r--   0 kim        (501) staff       (20)     8353 2024-02-13 12:24:16.000000 gym_csle_stopping_game-0.6.0/tests/test_stopping_game_util.py
```

### Comparing `gym_csle_stopping_game-0.5.3/PKG-INFO` & `gym_csle_stopping_game-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym_csle_stopping_game
-Version: 0.5.3
+Version: 0.6.0
 Summary: OpenAI gym reinforcement learning environment of a Dynkin (Optimal stopping) game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_stopping_game-0.5.3/pyproject.toml` & `gym_csle_stopping_game-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.3/setup.cfg` & `gym_csle_stopping_game-0.6.0/setup.cfg`

 * *Files 2% similar despite different names*

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

### Comparing `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/__init__.py` & `gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/__init__.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/constants/constants.py` & `gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/constants/constants.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py` & `gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/dao/stopping_game_config.py` & `gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/dao/stopping_game_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py` & `gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/dao/stopping_game_state.py` & `gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/dao/stopping_game_state.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/envs/stopping_game_env.py` & `gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/envs/stopping_game_env.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py` & `gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py` & `gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/util/stopping_game_util.py` & `gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game/util/stopping_game_util.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game.egg-info/PKG-INFO` & `gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-csle-stopping-game
-Version: 0.5.3
+Version: 0.6.0
 Summary: OpenAI gym reinforcement learning environment of a Dynkin (Optimal stopping) game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game.egg-info/SOURCES.txt` & `gym_csle_stopping_game-0.6.0/src/gym_csle_stopping_game.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.3/tests/test_stopping_game_dao.py` & `gym_csle_stopping_game-0.6.0/tests/test_stopping_game_dao.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.3/tests/test_stopping_game_util.py` & `gym_csle_stopping_game-0.6.0/tests/test_stopping_game_util.py`

 * *Files identical despite different names*

