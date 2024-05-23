# Comparing `tmp/bbrl_gymnasium-0.3.4.tar.gz` & `tmp/bbrl_gymnasium-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbrl_gymnasium-0.3.4.tar", last modified: Thu Apr 11 06:57:24 2024, max compression
+gzip compressed data, was "bbrl_gymnasium-0.3.5.tar", last modified: Thu May 23 08:34:46 2024, max compression
```

## Comparing `bbrl_gymnasium-0.3.4.tar` & `bbrl_gymnasium-0.3.5.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:57:24.076448 bbrl_gymnasium-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:57:24.068448 bbrl_gymnasium-0.3.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:57:24.072448 bbrl_gymnasium-0.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/.pre-commit-config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1071 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (127)       25 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/MANIFEST.in
--rwxr-xr-x   0 runner    (1001) docker     (127)     1388 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-11 06:57:24.076448 bbrl_gymnasium-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:57:24.072448 bbrl_gymnasium-0.3.4/bbrl_gymnasium/
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-11 06:57:23.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:57:24.076448 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/
--rwxr-xr-x   0 runner    (1001) docker     (127)      684 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12173 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/cartpole_pixels.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2706 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/continuous_2D_mdp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3061 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/continuous_cartpole.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2606 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/continuous_line_mdp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1799 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/debug_env.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2404 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/line_mdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/maze_mdp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/pendulum_frottements.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21855 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/rocket_lander.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/single_state_mdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/swimmer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:57:24.076448 bbrl_gymnasium-0.3.4/bbrl_gymnasium/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      966 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:57:24.076448 bbrl_gymnasium-0.3.4/bbrl_gymnasium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-11 06:57:24.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-11 06:57:24.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 06:57:24.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 06:57:24.000000 bbrl_gymnasium-0.3.4/bbrl_gymnasium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 06:57:24.076448 bbrl_gymnasium-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:57:24.076448 bbrl_gymnasium-0.3.4/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      811 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/tests/test_bbrl_gym.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2811 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/tests/test_maze.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      144 2024-04-11 06:57:15.000000 bbrl_gymnasium-0.3.4/tests/test_rocket_lander.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:34:46.681580 bbrl_gymnasium-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:34:46.673580 bbrl_gymnasium-0.3.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:34:46.677580 bbrl_gymnasium-0.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/.pre-commit-config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1071 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (127)       25 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/MANIFEST.in
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1388 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-23 08:34:46.681580 bbrl_gymnasium-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 08:34:46.681580 bbrl_gymnasium-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:34:46.673580 bbrl_gymnasium-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:34:46.677580 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 08:34:46.000000 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:34:46.677580 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      684 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12173 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/cartpole_pixels.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2706 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/continuous_2D_mdp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3061 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/continuous_cartpole.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2606 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/continuous_line_mdp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1799 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/debug_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2404 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/line_mdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/maze_mdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/pendulum_frottements.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21855 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/rocket_lander.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/single_state_mdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/swimmer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:34:46.677580 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      966 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:34:46.681580 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-23 08:34:46.000000 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-23 08:34:46.000000 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 08:34:46.000000 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 08:34:46.000000 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 08:34:46.000000 bbrl_gymnasium-0.3.5/src/bbrl_gymnasium.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:34:46.681580 bbrl_gymnasium-0.3.5/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      811 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/tests/test_bbrl_gym.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2811 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/tests/test_maze.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      144 2024-05-23 08:34:38.000000 bbrl_gymnasium-0.3.5/tests/test_rocket_lander.py
```

### Comparing `bbrl_gymnasium-0.3.4/.flake8` & `bbrl_gymnasium-0.3.5/.flake8`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.4/.github/workflows/python-publish.yml` & `bbrl_gymnasium-0.3.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.4/.pre-commit-config.yaml` & `bbrl_gymnasium-0.3.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.4/LICENSE` & `bbrl_gymnasium-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.4/Makefile` & `bbrl_gymnasium-0.3.5/Makefile`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.4/PKG-INFO` & `bbrl_gymnasium-0.3.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: bbrl_gymnasium
-Version: 0.3.4
+Version: 0.3.5
 Summary: A set of additional gym environments
-Home-page: https://github.com/osigaud/bbrl_gym
-Author: Olivier Sigaud
-Author-email: Olivier.Sigaud@isir.upmc.fr
+Author-email: Olivier Sigaud <olivier.sigaud@isir.upmc.fr>
 License: MIT
+Project-URL: Repository, https://github.com/osigaud/bbrl_gym
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.19.1
+Requires-Dist: gymnasium
+Requires-Dist: gymnasium[box2d]
+Requires-Dist: mazemdp
 
 The bbrl_gymnasium library is the place where I put additional gym-like environments.
 
 So far, it contains the following environments:
 - CartPoleContinuous-v0 (with timit limit = 200 steps)
 - CartPoleContinuous-v1 (with timit limit = 500 steps)
 - MazeMDP, a Maze environment for Tabular RL
```

### Comparing `bbrl_gymnasium-0.3.4/README.md` & `bbrl_gymnasium-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.4/bbrl_gymnasium/__init__.py` & `bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/__init__.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/__init__.py` & `bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/cartpole_pixels.py` & `bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/cartpole_pixels.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/continuous_2D_mdp.py` & `bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/continuous_2D_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/continuous_cartpole.py` & `bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/continuous_cartpole.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/continuous_line_mdp.py` & `bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/continuous_line_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/debug_env.py` & `bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/debug_env.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/line_mdp.py` & `bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/line_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/maze_mdp.py` & `bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/maze_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/pendulum_frottements.py` & `bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/pendulum_frottements.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/rocket_lander.py` & `bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/rocket_lander.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/single_state_mdp.py` & `bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/single_state_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.4/bbrl_gymnasium/envs/swimmer.py` & `bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/envs/swimmer.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.4/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py` & `bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.4/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py` & `bbrl_gymnasium-0.3.5/src/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.4/bbrl_gymnasium.egg-info/PKG-INFO` & `bbrl_gymnasium-0.3.5/src/bbrl_gymnasium.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: bbrl_gymnasium
-Version: 0.3.4
+Version: 0.3.5
 Summary: A set of additional gym environments
-Home-page: https://github.com/osigaud/bbrl_gym
-Author: Olivier Sigaud
-Author-email: Olivier.Sigaud@isir.upmc.fr
+Author-email: Olivier Sigaud <olivier.sigaud@isir.upmc.fr>
 License: MIT
+Project-URL: Repository, https://github.com/osigaud/bbrl_gym
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.19.1
+Requires-Dist: gymnasium
+Requires-Dist: gymnasium[box2d]
+Requires-Dist: mazemdp
 
 The bbrl_gymnasium library is the place where I put additional gym-like environments.
 
 So far, it contains the following environments:
 - CartPoleContinuous-v0 (with timit limit = 200 steps)
 - CartPoleContinuous-v1 (with timit limit = 500 steps)
 - MazeMDP, a Maze environment for Tabular RL
```

### Comparing `bbrl_gymnasium-0.3.4/tests/test_bbrl_gym.py` & `bbrl_gymnasium-0.3.5/tests/test_bbrl_gym.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.3.4/tests/test_maze.py` & `bbrl_gymnasium-0.3.5/tests/test_maze.py`

 * *Files identical despite different names*

