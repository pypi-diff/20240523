# Comparing `tmp/csle_tolerance-0.5.3.tar.gz` & `tmp/csle_tolerance-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_tolerance-0.5.3.tar", last modified: Mon May 13 17:20:45 2024, max compression
+gzip compressed data, was "csle_tolerance-0.6.0.tar", last modified: Thu May 23 17:43:50 2024, max compression
```

## Comparing `csle_tolerance-0.5.3.tar` & `csle_tolerance-0.6.0.tar`

### file list

```diff
@@ -1,36 +1,44 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:45.178893 csle_tolerance-0.5.3/
--rw-rw-r--   0 kim       (1000) kim       (1000)      741 2024-05-13 17:20:45.178893 csle_tolerance-0.5.3/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      674 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1929 2024-05-13 17:20:45.178893 csle_tolerance-0.5.3/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:45.174893 csle_tolerance-0.5.3/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:45.174893 csle_tolerance-0.5.3/src/csle_tolerance/
--rw-rw-r--   0 kim       (1000) kim       (1000)       39 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/src/csle_tolerance/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-05-13 17:19:17.000000 csle_tolerance-0.5.3/src/csle_tolerance/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:45.174893 csle_tolerance-0.5.3/src/csle_tolerance/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/src/csle_tolerance/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      315 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/src/csle_tolerance/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:45.174893 csle_tolerance-0.5.3/src/csle_tolerance/dao/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/src/csle_tolerance/dao/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5370 2024-05-13 17:10:17.000000 csle_tolerance-0.5.3/src/csle_tolerance/dao/intrusion_recovery_game_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5699 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/src/csle_tolerance/dao/intrusion_recovery_pomdp_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5231 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/src/csle_tolerance/dao/intrusion_response_cmdp_config.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:45.178893 csle_tolerance-0.5.3/src/csle_tolerance/envs/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/src/csle_tolerance/envs/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11235 2024-01-29 12:14:49.000000 csle_tolerance-0.5.3/src/csle_tolerance/envs/intrusion_recovery_pomdp_env.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8025 2024-01-29 12:14:49.000000 csle_tolerance-0.5.3/src/csle_tolerance/envs/intrusion_response_cmdp_env.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:45.178893 csle_tolerance-0.5.3/src/csle_tolerance/util/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/src/csle_tolerance/util/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2587 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/src/csle_tolerance/util/general_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    20399 2024-05-13 17:10:17.000000 csle_tolerance-0.5.3/src/csle_tolerance/util/intrusion_recovery_pomdp_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5895 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/src/csle_tolerance/util/intrusion_response_cmdp_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2058 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/src/csle_tolerance/util/pomdp_solve_parser.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:45.174893 csle_tolerance-0.5.3/src/csle_tolerance.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      741 2024-05-13 17:20:45.000000 csle_tolerance-0.5.3/src/csle_tolerance.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     1064 2024-05-13 17:20:45.000000 csle_tolerance-0.5.3/src/csle_tolerance.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-05-13 17:20:45.000000 csle_tolerance-0.5.3/src/csle_tolerance.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-09-16 07:31:36.000000 csle_tolerance-0.5.3/src/csle_tolerance.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      571 2024-05-13 17:20:45.000000 csle_tolerance-0.5.3/src/csle_tolerance.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       15 2024-05-13 17:20:45.000000 csle_tolerance-0.5.3/src/csle_tolerance.egg-info/top_level.txt
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:45.178893 csle_tolerance-0.5.3/tests/
--rw-rw-r--   0 kim       (1000) kim       (1000)      405 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/tests/test_intrusion_recovery_pomdp_util.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:50.321020 csle_tolerance-0.6.0/
+-rw-r--r--   0 kim        (501) staff       (20)      741 2024-05-23 17:43:50.321061 csle_tolerance-0.6.0/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)      674 2023-09-06 08:43:30.000000 csle_tolerance-0.6.0/pyproject.toml
+-rw-r--r--   0 kim        (501) staff       (20)     1929 2024-05-23 17:43:50.321297 csle_tolerance-0.6.0/setup.cfg
+-rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_tolerance-0.6.0/setup.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:50.315791 csle_tolerance-0.6.0/src/
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:50.316516 csle_tolerance-0.6.0/src/csle_tolerance/
+-rw-r--r--   0 kim        (501) staff       (20)       39 2023-09-15 16:43:44.000000 csle_tolerance-0.6.0/src/csle_tolerance/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-23 17:42:57.000000 csle_tolerance-0.6.0/src/csle_tolerance/__version__.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:50.317574 csle_tolerance-0.6.0/src/csle_tolerance/constants/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_tolerance-0.6.0/src/csle_tolerance/constants/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)      315 2023-10-09 07:12:58.000000 csle_tolerance-0.6.0/src/csle_tolerance/constants/constants.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:50.318326 csle_tolerance-0.6.0/src/csle_tolerance/dao/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-09-12 15:45:28.000000 csle_tolerance-0.6.0/src/csle_tolerance/dao/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     5364 2024-05-17 08:02:11.000000 csle_tolerance-0.6.0/src/csle_tolerance/dao/intrusion_recovery_game_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     5751 2024-05-17 08:02:11.000000 csle_tolerance-0.6.0/src/csle_tolerance/dao/intrusion_recovery_pomdp_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     5231 2023-09-15 15:32:19.000000 csle_tolerance-0.6.0/src/csle_tolerance/dao/intrusion_response_cmdp_config.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:50.319003 csle_tolerance-0.6.0/src/csle_tolerance/envs/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-09-12 15:44:05.000000 csle_tolerance-0.6.0/src/csle_tolerance/envs/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)    11235 2024-05-15 11:12:28.000000 csle_tolerance-0.6.0/src/csle_tolerance/envs/intrusion_recovery_pomdp_env.py
+-rw-r--r--   0 kim        (501) staff       (20)     8025 2024-02-13 12:24:16.000000 csle_tolerance-0.6.0/src/csle_tolerance/envs/intrusion_response_cmdp_env.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:50.319719 csle_tolerance-0.6.0/src/csle_tolerance/util/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-09-08 12:46:59.000000 csle_tolerance-0.6.0/src/csle_tolerance/util/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     2693 2024-05-17 08:02:11.000000 csle_tolerance-0.6.0/src/csle_tolerance/util/general_util.py
+-rw-r--r--   0 kim        (501) staff       (20)    21542 2024-05-17 08:02:11.000000 csle_tolerance-0.6.0/src/csle_tolerance/util/intrusion_recovery_pomdp_util.py
+-rw-r--r--   0 kim        (501) staff       (20)     5612 2024-05-23 15:58:41.000000 csle_tolerance-0.6.0/src/csle_tolerance/util/intrusion_response_cmdp_util.py
+-rw-r--r--   0 kim        (501) staff       (20)     2058 2023-10-09 07:12:58.000000 csle_tolerance-0.6.0/src/csle_tolerance/util/pomdp_solve_parser.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:50.317376 csle_tolerance-0.6.0/src/csle_tolerance.egg-info/
+-rw-r--r--   0 kim        (501) staff       (20)      741 2024-05-23 17:43:50.000000 csle_tolerance-0.6.0/src/csle_tolerance.egg-info/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)     1389 2024-05-23 17:43:50.000000 csle_tolerance-0.6.0/src/csle_tolerance.egg-info/SOURCES.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-23 17:43:50.000000 csle_tolerance-0.6.0/src/csle_tolerance.egg-info/dependency_links.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2023-09-14 11:59:31.000000 csle_tolerance-0.6.0/src/csle_tolerance.egg-info/not-zip-safe
+-rw-r--r--   0 kim        (501) staff       (20)      571 2024-05-23 17:43:50.000000 csle_tolerance-0.6.0/src/csle_tolerance.egg-info/requires.txt
+-rw-r--r--   0 kim        (501) staff       (20)       15 2024-05-23 17:43:50.000000 csle_tolerance-0.6.0/src/csle_tolerance.egg-info/top_level.txt
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:50.320892 csle_tolerance-0.6.0/tests/
+-rw-r--r--   0 kim        (501) staff       (20)     1977 2024-05-17 08:02:11.000000 csle_tolerance-0.6.0/tests/test_general_util.py
+-rw-r--r--   0 kim        (501) staff       (20)     8827 2024-05-17 08:02:11.000000 csle_tolerance-0.6.0/tests/test_intrusion_recovery_game_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     9323 2024-05-17 08:02:11.000000 csle_tolerance-0.6.0/tests/test_intrusion_recovery_pomdp_config.py
+-rw-r--r--   0 kim        (501) staff       (20)    10854 2024-05-17 08:02:11.000000 csle_tolerance-0.6.0/tests/test_intrusion_recovery_pomdp_env.py
+-rw-r--r--   0 kim        (501) staff       (20)     9259 2024-05-17 08:02:11.000000 csle_tolerance-0.6.0/tests/test_intrusion_recovery_pomdp_util.py
+-rw-r--r--   0 kim        (501) staff       (20)     9291 2024-05-17 08:02:11.000000 csle_tolerance-0.6.0/tests/test_intrusion_response_cmdp_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     4276 2024-05-17 08:02:11.000000 csle_tolerance-0.6.0/tests/test_intrusion_response_cmdp_util.py
+-rw-r--r--   0 kim        (501) staff       (20)     9753 2024-05-17 08:02:11.000000 csle_tolerance-0.6.0/tests/test_intrusion_response_pomdp_env.py
+-rw-r--r--   0 kim        (501) staff       (20)     1962 2024-05-17 08:02:11.000000 csle_tolerance-0.6.0/tests/test_pomdp_solve_parser.py
```

### Comparing `csle_tolerance-0.5.3/PKG-INFO` & `csle_tolerance-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_tolerance
-Version: 0.5.3
+Version: 0.6.0
 Summary: An intrusion-tolerant system: Tolerance: (T)w(o)-(l)ev(e)l (r)ecovery (a)nd respo(n)se (c)ontrol with f(e)edback.
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes Intrusion-tolerance
 Platform: unix
 Platform: linux
```

### Comparing `csle_tolerance-0.5.3/pyproject.toml` & `csle_tolerance-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.3/setup.cfg` & `csle_tolerance-0.6.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	gymnasium>=0.27.1
 	numpy>=1.23.5
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

### Comparing `csle_tolerance-0.5.3/src/csle_tolerance/dao/intrusion_recovery_game_config.py` & `csle_tolerance-0.6.0/src/csle_tolerance/dao/intrusion_recovery_game_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         self.gym_env_name = gym_env_name
         self.max_horizon = max_horizon
 
     def __str__(self) -> str:
         """
         :return: a string representation of the DTO
         """
-        return (f"eta: {self.eta}, p_a: {self.p_a}, p_c_1: {self.p_c_1},"
+        return (f"eta: {self.eta}, p_a: {self.p_a}, p_c_1: {self.p_c_1}, "
                 f"BTR: {self.BTR}, negate_costs: {self.negate_costs}, seed: {self.seed}, "
                 f"discount_factor: {self.discount_factor}, states: {self.states}, actions: {self.actions}, "
                 f"observations: {self.observation_tensor}, cost_tensor: {self.cost_tensor}, "
                 f"observation_tensor: {self.observation_tensor}, transition_tensor: {self.transition_tensor}, "
                 f"b1:{self.b1}, T: {self.T}, simulation_env_name: {self.simulation_env_name}, "
                 f"gym_env_name: {self.gym_env_name}, max_horizon: {self.max_horizon}")
 
@@ -101,15 +101,15 @@
         d["observations"] = self.observations
         d["cost_tensor"] = self.cost_tensor
         d["observation_tensor"] = self.observation_tensor
         d["transition_tensor"] = self.transition_tensor
         d["b1"] = self.b1
         d["T"] = self.T
         d["simulation_env_name"] = self.simulation_env_name
-        d["gym_env_name"] = self.simulation_env_name
+        d["gym_env_name"] = self.gym_env_name
         return d
 
     @staticmethod
     def from_json_file(json_file_path: str) -> "IntrusionRecoveryGameConfig":
         """
         Reads a json file and converts it to a DTO
```

### Comparing `csle_tolerance-0.5.3/src/csle_tolerance/dao/intrusion_recovery_pomdp_config.py` & `csle_tolerance-0.6.0/src/csle_tolerance/dao/intrusion_recovery_pomdp_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from typing import List, Dict, Any
 import numpy as np
+import logging
+import io
+import json
 from csle_common.dao.simulation_config.simulation_env_input_config import SimulationEnvInputConfig
 
 
 class IntrusionRecoveryPomdpConfig(SimulationEnvInputConfig):
     """
     DTO containing the configuration of an intrusion recovery POMDP
     """
@@ -107,23 +110,23 @@
         d["observations"] = self.observations
         d["cost_tensor"] = self.cost_tensor
         d["observation_tensor"] = self.observation_tensor
         d["transition_tensor"] = self.transition_tensor
         d["b1"] = self.b1
         d["T"] = self.T
         d["simulation_env_name"] = self.simulation_env_name
-        d["gym_env_name"] = self.simulation_env_name
+        d["gym_env_name"] = self.gym_env_name
         return d
 
     @staticmethod
     def from_json_file(json_file_path: str) -> "IntrusionRecoveryPomdpConfig":
         """
         Reads a json file and converts it to a DTO
 
         :param json_file_path: the json file path
         :return: the converted DTO
         """
-        import io
-        import json
+        logging.info(msg="msg")
         with io.open(json_file_path, 'r') as f:
             json_str = f.read()
+            print(json_str)
         return IntrusionRecoveryPomdpConfig.from_dict(json.loads(json_str))
```

### Comparing `csle_tolerance-0.5.3/src/csle_tolerance/dao/intrusion_response_cmdp_config.py` & `csle_tolerance-0.6.0/src/csle_tolerance/dao/intrusion_response_cmdp_config.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.3/src/csle_tolerance/envs/intrusion_recovery_pomdp_env.py` & `csle_tolerance-0.6.0/src/csle_tolerance/envs/intrusion_recovery_pomdp_env.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.3/src/csle_tolerance/envs/intrusion_response_cmdp_env.py` & `csle_tolerance-0.6.0/src/csle_tolerance/envs/intrusion_response_cmdp_env.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.3/src/csle_tolerance/util/general_util.py` & `csle_tolerance-0.6.0/src/csle_tolerance/util/general_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import List
-from gymnasium.envs.registration import register
 import math
 import numpy as np
 
 
 class GeneralUtil:
     """
     Class with general utility functions related to csle-tolerance
@@ -18,17 +17,22 @@
         :param threshold: the threshold
         :return: the stopping probability
         """
         if (1 - round(b1, 2)) == 0:
             return 1.0
         if round(b1, 2) == 0:
             return 0.0
-        if (threshold * (1 - b1)) > 0 and (b1 * (1 - threshold)) / (threshold * (1 - b1)) > 0:
+        if (threshold * (1 - b1)) > 0 and (b1 * (1 - threshold)) / (
+            threshold * (1 - b1)
+        ) > 0:
             try:
-                return math.pow(1 + math.pow(((b1 * (1 - threshold)) / (threshold * (1 - b1))), k), -1)
+                return math.pow(
+                    1 + math.pow(((b1 * (1 - threshold)) / (threshold * (1 - b1))), k),
+                    -1,
+                )
             except Exception:
                 return 0.0
         else:
             return 0.0
 
     @staticmethod
     def sigmoid(x) -> float:
@@ -47,15 +51,17 @@
 
         :param y: sigmoid(x)
         :return: sigmoid(x)^(-1)
         """
         return math.log(y / (1 - y), math.e)
 
     @staticmethod
-    def sample_next_state(transition_tensor: List[List[List[float]]], s: int, a: int, states: List[int]) -> int:
+    def sample_next_state(
+        transition_tensor: List[List[List[float]]], s: int, a: int, states: List[int]
+    ) -> int:
         """
         Samples the next state of a MDP or POMDP
 
         :param transition_tensor: the transition tensor
         :param s: the current state
         :param a: the current action
         :param states: the list of states
@@ -69,17 +75,19 @@
     @staticmethod
     def register_envs() -> None:
         """
         Utility method for registering Gymnasium environments
 
         :return: None
         """
+        from gymnasium.envs.registration import register
+
         register(
-            id='csle-tolerance-intrusion-recovery-pomdp-v1',
-            entry_point='csle_tolerance.envs.intrusion_recovery_pomdp_env:IntrusionRecoveryPomdpEnv',
-            kwargs={'config': None}
+            id="csle-tolerance-intrusion-recovery-pomdp-v1",
+            entry_point="csle_tolerance.envs.intrusion_recovery_pomdp_env:IntrusionRecoveryPomdpEnv",
+            kwargs={"config": None},
         )
         register(
-            id='csle-tolerance-intrusion-response-cmdp-v1',
-            entry_point='csle_tolerance.envs.intrusion_response_cmdp_env:IntrusionResponseCmdpEnv',
-            kwargs={'config': None}
+            id="csle-tolerance-intrusion-response-cmdp-v1",
+            entry_point="csle_tolerance.envs.intrusion_response_cmdp_env:IntrusionResponseCmdpEnv",
+            kwargs={"config": None},
         )
```

### Comparing `csle_tolerance-0.5.3/src/csle_tolerance/util/intrusion_recovery_pomdp_util.py` & `csle_tolerance-0.6.0/src/csle_tolerance/util/intrusion_recovery_pomdp_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from typing import List
 from scipy.stats import betabinom
 import numpy as np
-from csle_tolerance.dao.intrusion_recovery_pomdp_config import IntrusionRecoveryPomdpConfig
-from csle_tolerance.dao.intrusion_recovery_game_config import IntrusionRecoveryGameConfig
+from csle_tolerance.dao.intrusion_recovery_pomdp_config import (
+    IntrusionRecoveryPomdpConfig,
+)
+from csle_tolerance.dao.intrusion_recovery_game_config import (
+    IntrusionRecoveryGameConfig,
+)
 
 
 class IntrusionRecoveryPomdpUtil:
     """
     Class with utility functions for the intrusion-recovery POMDP
     """
 
@@ -64,29 +68,35 @@
         cost = eta * s - eta * a * s + a
         if negate:
             return -cost
         else:
             return cost
 
     @staticmethod
-    def cost_tensor(eta: float, states: List[int], actions: List[int], negate: bool = False) -> List[List[float]]:
+    def cost_tensor(
+        eta: float, states: List[int], actions: List[int], negate: bool = False
+    ) -> List[List[float]]:
         """
         Creates a |A|x|S| tensor with the costs (or rewards) of the POMDP
 
         :param eta: the cost scaling factor
         :param states: the list of states
         :param actions: the list of actions
         :param negate: a boolean flag indicating whether the cost should be negated as a reward or not
         :return: A tensor with the costs (or rewards)
         """
         cost_tensor = []
         for a in actions:
             a_costs = []
             for s in states:
-                a_costs.append(IntrusionRecoveryPomdpUtil.cost_function(s=s, a=a, eta=eta, negate=negate))
+                a_costs.append(
+                    IntrusionRecoveryPomdpUtil.cost_function(
+                        s=s, a=a, eta=eta, negate=negate
+                    )
+                )
             cost_tensor.append(a_costs)
         return cost_tensor
 
     @staticmethod
     def observation_function(s: int, o: int, num_observations: int) -> float:
         """
         The observation function of the POMDP
@@ -105,34 +115,41 @@
         else:
             if o == num_observations - 1:
                 return 1.0
             else:
                 return 0.0
 
     @staticmethod
-    def observation_tensor(states: List[int], observations: List[int]) -> List[List[float]]:
+    def observation_tensor(
+        states: List[int], observations: List[int]
+    ) -> List[List[float]]:
         """
         Creates a |S|x|O| tensor with the observation probabilities
 
         :param states: the list of states
         :param observations: the list of observations
         :return: the observation tensor
         """
         observation_tensor = []
         num_observations = len(observations)
         for s in states:
             s_observations = []
             for o in observations:
-                s_observations.append(IntrusionRecoveryPomdpUtil.observation_function(
-                    s=s, o=o, num_observations=num_observations))
+                s_observations.append(
+                    IntrusionRecoveryPomdpUtil.observation_function(
+                        s=s, o=o, num_observations=num_observations
+                    )
+                )
             observation_tensor.append(s_observations)
         return observation_tensor
 
     @staticmethod
-    def transition_function(s: int, s_prime: int, a: int, p_a: float, p_c_1: float, p_u: float, p_c_2: float) -> float:
+    def transition_function(
+        s: int, s_prime: int, a: int, p_a: float, p_c_1: float, p_u: float, p_c_2: float
+    ) -> float:
         """
         The transition function of the POMDP
 
         :param s: the state
         :param s_prime: the next state
         :param a: the action
         :param p_a: the intrusion probability
@@ -163,15 +180,17 @@
             return (1.0 - p_c_1) * p_a
         elif s_prime == 1 and s == 1 and a == 0:
             return (1 - p_c_2) * (1 - p_u)
         else:
             return 0
 
     @staticmethod
-    def transition_function_game(s: int, s_prime: int, a1: int, a2: int, p_a: float, p_c_1: float) -> float:
+    def transition_function_game(
+        s: int, s_prime: int, a1: int, a2: int, p_a: float, p_c_1: float
+    ) -> float:
         """
         The transition function of the POSG
 
         :param s: the state
         :param s_prime: the next state
         :param a1: the defender action
         :param a2: the attacker action
@@ -181,52 +200,75 @@
         """
         if s == 2 and s_prime == 2:
             return 1.0
         elif s_prime == 2 and s in [0, 1]:
             return p_c_1
         elif s_prime == 0 and a1 == 0 and a2 == 1 and s == 0:
             return (1 - p_a) * (1 - p_c_1)
-        elif (s_prime == 0 and a2 == 0 and s == 0) or (s_prime == 0 and s == 1 and a1 == 1) \
-                or (s_prime == 1 and s == 1 and a1 == 0):
-            return (1 - p_c_1)
-        elif (s_prime == 1 and s == 0 and a2 == 1):
+        elif (
+            (s_prime == 0 and a2 == 0 and s == 0)
+            or (s_prime == 0 and s == 1 and a1 == 1)
+            or (s_prime == 1 and s == 1 and a1 == 0)
+        ):
+            return 1 - p_c_1
+        elif s_prime == 1 and s == 0 and a2 == 1:
             return (1 - p_c_1) * p_a
         else:
             return 0
 
     @staticmethod
-    def transition_tensor(states: List[int], actions: List[int], p_a: float, p_c_1: float, p_c_2: float, p_u: float) \
-            -> List[List[List[float]]]:
+    def transition_tensor(
+        states: List[int],
+        actions: List[int],
+        p_a: float,
+        p_c_1: float,
+        p_c_2: float,
+        p_u: float,
+    ) -> List[List[List[float]]]:
         """
         Creates a |A|x|S|x|S| tensor with the transition probabilities of the POMDP
 
         :param states: the list of states
         :param actions: the list of actions
         :param p_a: the intrusion probability
         :param p_c_1: the crash probability in the healthy state
         :param p_c_2: the crash probability in the compromised state
         :param p_u: the upgrade probability
         :return: the transition tensor
         """
+        assert states == [0, 1, 2]
         transition_tensor = []
         for a in actions:
             a_transitions = []
             for s in states:
                 s_a_transitions = []
                 for s_prime in states:
-                    s_a_transitions.append(IntrusionRecoveryPomdpUtil.transition_function(
-                        s=s, s_prime=s_prime, a=a, p_a=p_a, p_c_1=p_c_1, p_c_2=p_c_2, p_u=p_u))
-                assert round(sum(s_a_transitions), 2) == 1.0
+                    s_a_transitions.append(
+                        IntrusionRecoveryPomdpUtil.transition_function(
+                            s=s,
+                            s_prime=s_prime,
+                            a=a,
+                            p_a=p_a,
+                            p_c_1=p_c_1,
+                            p_c_2=p_c_2,
+                            p_u=p_u,
+                        )
+                    )
                 a_transitions.append(s_a_transitions)
             transition_tensor.append(a_transitions)
         return transition_tensor
 
     @staticmethod
-    def transition_tensor_game(states: List[int], defender_actions: List[int], attacker_actions: List[int],
-                               p_a: float, p_c_1: float) -> List[List[List[List[float]]]]:
+    def transition_tensor_game(
+        states: List[int],
+        defender_actions: List[int],
+        attacker_actions: List[int],
+        p_a: float,
+        p_c_1: float,
+    ) -> List[List[List[List[float]]]]:
         """
         Creates a |A|x|A|x|S|x|S| tensor with the transition probabilities of the POSG
 
         :param states: the list of states
         :param defender_actions: the list of defender actions
         :param attacker_actions: the list of attacker actions
         :param p_a: the intrusion probability
@@ -237,16 +279,19 @@
         for a1 in defender_actions:
             a1_transitions = []
             for a2 in attacker_actions:
                 a2_transitions = []
                 for s in states:
                     s_a1_a2_transitions = []
                     for s_prime in states:
-                        s_a1_a2_transitions.append(IntrusionRecoveryPomdpUtil.transition_function_game(
-                            s=s, s_prime=s_prime, a1=a1, a2=a2, p_a=p_a, p_c_1=p_c_1))
+                        s_a1_a2_transitions.append(
+                            IntrusionRecoveryPomdpUtil.transition_function_game(
+                                s=s, s_prime=s_prime, a1=a1, a2=a2, p_a=p_a, p_c_1=p_c_1
+                            )
+                        )
                     a2_transitions.append(s_a1_a2_transitions)
                 a1_transitions.append(a2_transitions)
             transition_tensor.append(a1_transitions)
         return transition_tensor
 
     @staticmethod
     def sample_initial_state(b1: List[float]) -> int:
@@ -255,15 +300,17 @@
 
         :param b1: the initial belief
         :return: the initial state
         """
         return int(np.random.choice(np.arange(0, len(b1)), p=b1))
 
     @staticmethod
-    def sample_next_observation(observation_tensor: List[List[float]], s_prime: int, observations: List[int]) -> int:
+    def sample_next_observation(
+        observation_tensor: List[List[float]], s_prime: int, observations: List[int]
+    ) -> int:
         """
         Samples the next observation
 
         :param s_prime: the new state
         :param observations: the observation space
         :param observation_tensor: the observation tensor
         :return: the next observation o
@@ -271,30 +318,43 @@
         observation_probs = []
         for o in observations:
             observation_probs.append(observation_tensor[s_prime][o])
         o = np.random.choice(np.arange(0, len(observations)), p=observation_probs)
         return int(o)
 
     @staticmethod
-    def sample_next_state_game(transition_tensor: List[List[List[List[float]]]], s: int, a1: int, a2: int) -> int:
+    def sample_next_state_game(
+        transition_tensor: List[List[List[List[float]]]], s: int, a1: int, a2: int
+    ) -> int:
         """
         Samples the next observation
 
         :param s: the current state
         :param a1: the defender action
         :param a2: the attacker action
         :param transition_tensor: the transition tensor
         :return: the next state a
         """
-        s_prime = np.random.choice(np.arange(0, len(transition_tensor[a1][a2][s])), p=transition_tensor[a1][a2][s])
+        s_prime = np.random.choice(
+            np.arange(0, len(transition_tensor[a1][a2][s])),
+            p=transition_tensor[a1][a2][s],
+        )
         return int(s_prime)
 
     @staticmethod
-    def bayes_filter(s_prime: int, o: int, a: int, b: List[float], states: List[int], observations: List[int],
-                     observation_tensor: List[List[float]], transition_tensor: List[List[List[float]]]) -> float:
+    def bayes_filter(
+        s_prime: int,
+        o: int,
+        a: int,
+        b: List[float],
+        states: List[int],
+        observations: List[int],
+        observation_tensor: List[List[float]],
+        transition_tensor: List[List[List[float]]],
+    ) -> float:
         """
         A Bayesian filter to compute b[s_prime] of the POMDP
 
         :param s_prime: the state to compute the belief for
         :param o: the latest observation
         :param a: the latest action
         :param b: the current belief
@@ -310,47 +370,66 @@
                 prob_1 = observation_tensor[s_prime_1][o]
                 norm += b[s] * prob_1 * transition_tensor[a][s][s_prime_1]
         if norm == 0.0:
             return 0.0
         temp = 0.0
 
         for s in states:
-            temp += observation_tensor[s_prime][o] * transition_tensor[a][s][s_prime] * b[s]
+            temp += (
+                observation_tensor[s_prime][o] * transition_tensor[a][s][s_prime] * b[s]
+            )
         b_prime_s_prime = temp / norm
         if round(b_prime_s_prime, 2) > 1:
             print(f"b_prime_s_prime >= 1: {b_prime_s_prime}, a1:{a}, s_prime:{s_prime}")
         assert round(b_prime_s_prime, 2) <= 1
         if s_prime == 2 and o != observations[-1]:
             assert round(b_prime_s_prime, 2) <= 0.01
         return b_prime_s_prime
 
     @staticmethod
-    def p_o_given_b_a1_a2(o: int, b: List[float], a: int, states: List[int],
-                          transition_tensor: List[List[List[float]]], observation_tensor: List[List[float]]) -> float:
+    def p_o_given_b_a1_a2(
+        o: int,
+        b: List[float],
+        a: int,
+        states: List[int],
+        transition_tensor: List[List[List[float]]],
+        observation_tensor: List[List[float]],
+    ) -> float:
         """
         Computes P[o|a,b] of the POMDP
 
         :param o: the observation
         :param b: the belief point
         :param a: the action
         :param states: the list of states
         :param transition_tensor: the transition tensor
         :param observation_tensor: the observation tensor
         :return: the probability of observing o when taking action a in belief point b
         """
         prob = 0.0
         for s in states:
             for s_prime in states:
-                prob += b[s] * transition_tensor[a][s][s_prime] * observation_tensor[s_prime][o]
+                prob += (
+                    b[s]
+                    * transition_tensor[a][s][s_prime]
+                    * observation_tensor[s_prime][o]
+                )
         assert prob < 1
         return prob
 
     @staticmethod
-    def next_belief(o: int, a: int, b: List[float], states: List[int], observations: List[int],
-                    observation_tensor: List[List[float]], transition_tensor: List[List[List[float]]]) -> List[float]:
+    def next_belief(
+        o: int,
+        a: int,
+        b: List[float],
+        states: List[int],
+        observations: List[int],
+        observation_tensor: List[List[float]],
+        transition_tensor: List[List[List[float]]],
+    ) -> List[float]:
         """
         Computes the next belief using a Bayesian filter
 
         :param o: the latest observation
         :param a: the latest action of player 1
         :param b: the current belief
         :param states: the list of states
@@ -358,16 +437,23 @@
         :param observation_tensor: the observation tensor
         :param transition_tensor: the transition tensor
         :return: the new belief
         """
         b_prime = [0.0] * len(states)
         for s_prime in states:
             b_prime[s_prime] = IntrusionRecoveryPomdpUtil.bayes_filter(
-                s_prime=s_prime, o=o, a=a, b=b, states=states, observations=observations,
-                transition_tensor=transition_tensor, observation_tensor=observation_tensor)
+                s_prime=s_prime,
+                o=o,
+                a=a,
+                b=b,
+                states=states,
+                observations=observations,
+                transition_tensor=transition_tensor,
+                observation_tensor=observation_tensor,
+            )
         if round(sum(b_prime), 2) != 1:
             print(f"error, b_prime:{b_prime}, o:{o}, a:{a}, b:{b}")
         assert round(sum(b_prime), 2) == 1
         return b_prime
 
     @staticmethod
     def pomdp_solver_file(config: IntrusionRecoveryPomdpConfig) -> str:
@@ -407,15 +493,17 @@
                 assert round(sum(probs), 3) == 1
         file_str = file_str + "\n\n"
         for s in config.states:
             for a in config.actions:
                 for s_prime in config.states:
                     for o in config.observations:
                         c = config.cost_tensor[a][s]
-                        file_str = file_str + f"R: {a} : {s} : {s_prime} : {o} {c:.80f}\n"
+                        file_str = (
+                            file_str + f"R: {a} : {s} : {s_prime} : {o} {c:.80f}\n"
+                        )
         return file_str
 
     @staticmethod
     def generate_transitions(game_config: IntrusionRecoveryGameConfig) -> List[str]:
         """
         Generates the transition rows of the POSG config file of HSVI
 
@@ -460,45 +548,55 @@
         """
         Generates the POSG game file for HSVI
 
         :param game_config: the game configuration
         :return: a string with the contents of the config file
         """
         num_partitions = 1
-        transitions = IntrusionRecoveryPomdpUtil.generate_transitions(game_config=game_config)
+        transitions = IntrusionRecoveryPomdpUtil.generate_transitions(
+            game_config=game_config
+        )
         rewards = IntrusionRecoveryPomdpUtil.generate_rewards(game_config=game_config)
-        game_description = f"{len(game_config.states)} {num_partitions} {len(game_config.actions)} " \
-                           f"{len(game_config.actions)} " \
-                           f"{len(game_config.observations)} {len(transitions)} " \
-                           f"{len(rewards)} {game_config.discount_factor}"
+        game_description = (
+            f"{len(game_config.states)} {num_partitions} {len(game_config.actions)} "
+            f"{len(game_config.actions)} "
+            f"{len(game_config.observations)} {len(transitions)} "
+            f"{len(rewards)} {game_config.discount_factor}"
+        )
         state_desriptions = []
         for s in game_config.states:
             state_desriptions.append(f"{s} {0}")
         player_1_actions = ["WAIT", "RECOVER"]
         player_2_actions = ["FALSEALARM", "ATTACK"]
 
         player_2_legal_actions = []
         for _ in game_config.states:
-            player_2_legal_actions.append(" ".join(list(map(lambda x: str(x), game_config.actions))))
+            player_2_legal_actions.append(
+                " ".join(list(map(lambda x: str(x), game_config.actions)))
+            )
 
         player_1_legal_actions = []
-        player_1_legal_actions.append(" ".join(list(map(lambda x: str(x), game_config.actions))))
+        player_1_legal_actions.append(
+            " ".join(list(map(lambda x: str(x), game_config.actions)))
+        )
 
         obs_desriptions = []
         for i, o in enumerate(game_config.observations):
             obs_desriptions.append(f"o_{o}")
 
-        initial_belief_str = f"{0} {' '.join(list(map(lambda x: str(x), game_config.b1)))}"
+        initial_belief_str = (
+            f"{0} {' '.join(list(map(lambda x: str(x), game_config.b1)))}"
+        )
         game_file_str = ""
         game_file_str = game_file_str + game_description + "\n"
         game_file_str = game_file_str + "\n".join(state_desriptions) + "\n"
         game_file_str = game_file_str + "\n".join(player_1_actions) + "\n"
         game_file_str = game_file_str + "\n".join(player_2_actions) + "\n"
         game_file_str = game_file_str + "\n".join(obs_desriptions) + "\n"
         game_file_str = game_file_str + "\n".join(player_2_legal_actions) + "\n"
         game_file_str = game_file_str + "\n".join(player_1_legal_actions) + "\n"
         game_file_str = game_file_str + "\n".join(transitions) + "\n"
         game_file_str = game_file_str + "\n".join(rewards) + "\n"
         game_file_str = game_file_str + initial_belief_str
-        with open('recovery_game.txt', 'w') as f:
+        with open("recovery_game.txt", "w") as f:
             f.write(game_file_str)
         return game_file_str
```

### Comparing `csle_tolerance-0.5.3/src/csle_tolerance/util/intrusion_response_cmdp_util.py` & `csle_tolerance-0.6.0/src/csle_tolerance/util/intrusion_response_cmdp_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,17 +138,14 @@
         """
         transition_tensor = []
         for a in actions:
             a_transitions = []
             for s in states:
                 s_a_transitions = []
                 normalizing_constant = 0.0
-                for delta in range(-s_max, s_max + 1):
-                    normalizing_constant += IntrusionResponseCmdpUtil.delta_function(s=s, p_a=p_a, p_c=p_c, p_u=p_u,
-                                                                                     delta=delta, s_max=s_max)
                 for s_prime in states:
                     s_a_transitions.append(IntrusionResponseCmdpUtil.transition_function(
                         s=s, s_prime=s_prime, a=a, p_a=p_a, p_c=p_c, p_u=p_u, s_max=s_max))
                 normalizing_constant = sum(s_a_transitions)
                 s_a_transitions = list(np.array(s_a_transitions) * (1 / normalizing_constant))
                 if not round(sum(s_a_transitions), 2) == 1:
                     print(f"{sum(s_a_transitions)}, s:{s}, a:{a}, normalizing constant: {normalizing_constant}, "
```

### Comparing `csle_tolerance-0.5.3/src/csle_tolerance/util/pomdp_solve_parser.py` & `csle_tolerance-0.6.0/src/csle_tolerance/util/pomdp_solve_parser.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.3/src/csle_tolerance.egg-info/PKG-INFO` & `csle_tolerance-0.6.0/src/csle_tolerance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-tolerance
-Version: 0.5.3
+Version: 0.6.0
 Summary: An intrusion-tolerant system: Tolerance: (T)w(o)-(l)ev(e)l (r)ecovery (a)nd respo(n)se (c)ontrol with f(e)edback.
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes Intrusion-tolerance
 Platform: unix
 Platform: linux
```

### Comparing `csle_tolerance-0.5.3/src/csle_tolerance.egg-info/requires.txt` & `csle_tolerance-0.6.0/src/csle_tolerance.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 gymnasium>=0.27.1
 numpy>=1.23.5
-csle-base>=0.5.3
-csle-common>=0.5.3
-csle-attacker>=0.5.3
-csle-defender>=0.5.3
-csle-collector>=0.5.3
+csle-base>=0.6.0
+csle-common>=0.6.0
+csle-attacker>=0.6.0
+csle-defender>=0.6.0
+csle-collector>=0.6.0
 
 [testing]
 pytest>=6.0
 pytest-cov>=2.0
 pytest-mock>=3.6.0
 grpcio>=1.57.0
 grpcio-tools>=1.57.0
```

