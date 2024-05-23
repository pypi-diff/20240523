# Comparing `tmp/dsse-1.1.7.tar.gz` & `tmp/dsse-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsse-1.1.7.tar", last modified: Thu May  2 18:42:55 2024, max compression
+gzip compressed data, was "dsse-1.1.8.tar", last modified: Thu May 23 21:03:27 2024, max compression
```

## Comparing `dsse-1.1.7.tar` & `dsse-1.1.8.tar`

### file list

```diff
@@ -1,44 +1,51 @@
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:42:55.746854 dsse-1.1.7/
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:42:55.738854 dsse-1.1.7/DSSE/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      322 2024-04-18 19:38:11.000000 dsse-1.1.7/DSSE/__init__.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:42:55.742854 dsse-1.1.7/DSSE/environment/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 14:40:14.000000 dsse-1.1.7/DSSE/environment/__init__.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      490 2024-04-18 19:38:11.000000 dsse-1.1.7/DSSE/environment/constants.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     7166 2024-05-02 18:19:41.000000 dsse-1.1.7/DSSE/environment/coverage_env.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:42:55.742854 dsse-1.1.7/DSSE/environment/entities/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-04-18 19:38:11.000000 dsse-1.1.7/DSSE/environment/entities/__init__.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      686 2024-04-18 19:38:11.000000 dsse-1.1.7/DSSE/environment/entities/drone.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     8070 2024-04-18 19:38:11.000000 dsse-1.1.7/DSSE/environment/entities/person.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    13639 2024-05-02 18:19:41.000000 dsse-1.1.7/DSSE/environment/env.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     8213 2024-05-02 18:19:41.000000 dsse-1.1.7/DSSE/environment/env_base.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:42:55.742854 dsse-1.1.7/DSSE/environment/imgs/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:19:41.000000 dsse-1.1.7/DSSE/environment/imgs/__init__.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    14774 2024-03-12 14:40:14.000000 dsse-1.1.7/DSSE/environment/imgs/drone.png
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    13193 2024-03-12 14:40:14.000000 dsse-1.1.7/DSSE/environment/imgs/person-swimming.png
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     4765 2024-04-18 19:38:11.000000 dsse-1.1.7/DSSE/environment/pygame_interface.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:42:55.742854 dsse-1.1.7/DSSE/environment/simulation/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-04-18 19:38:11.000000 dsse-1.1.7/DSSE/environment/simulation/__init__.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     4890 2024-04-18 19:38:11.000000 dsse-1.1.7/DSSE/environment/simulation/dynamic_probability.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     6390 2024-05-02 18:19:41.000000 dsse-1.1.7/DSSE/environment/simulation/particle_simulation.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1205 2024-04-18 19:38:11.000000 dsse-1.1.7/DSSE/environment/simulation/time_step.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:42:55.742854 dsse-1.1.7/DSSE/environment/wrappers/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1587 2024-04-18 19:38:11.000000 dsse-1.1.7/DSSE/environment/wrappers/all_positions_wrapper.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:42:55.742854 dsse-1.1.7/DSSE/tests/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 14:40:14.000000 dsse-1.1.7/DSSE/tests/__init__.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1488 2024-04-18 19:38:11.000000 dsse-1.1.7/DSSE/tests/drone_policy.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    12849 2024-05-02 18:19:41.000000 dsse-1.1.7/DSSE/tests/test_env.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     6996 2024-05-02 18:19:41.000000 dsse-1.1.7/DSSE/tests/test_env_coverage.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      581 2024-04-18 19:38:11.000000 dsse-1.1.7/DSSE/tests/test_matrix.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:42:55.742854 dsse-1.1.7/DSSE.egg-info/
--rw-r--r--   0 ricardo   (1000) ricardo   (1000)     7437 2024-05-02 18:42:55.000000 dsse-1.1.7/DSSE.egg-info/PKG-INFO
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      973 2024-05-02 18:42:55.000000 dsse-1.1.7/DSSE.egg-info/SOURCES.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        1 2024-05-02 18:42:55.000000 dsse-1.1.7/DSSE.egg-info/dependency_links.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      257 2024-05-02 18:42:55.000000 dsse-1.1.7/DSSE.egg-info/requires.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        5 2024-05-02 18:42:55.000000 dsse-1.1.7/DSSE.egg-info/top_level.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1094 2024-04-18 19:38:11.000000 dsse-1.1.7/LICENSE
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       32 2024-05-02 18:21:55.000000 dsse-1.1.7/MANIFEST.in
--rw-r--r--   0 ricardo   (1000) ricardo   (1000)     7437 2024-05-02 18:42:55.746854 dsse-1.1.7/PKG-INFO
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     5280 2024-05-02 18:19:41.000000 dsse-1.1.7/README.md
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     2225 2024-05-02 18:19:41.000000 dsse-1.1.7/pyproject.toml
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       38 2024-05-02 18:42:55.746854 dsse-1.1.7/setup.cfg
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      188 2024-05-02 18:42:35.000000 dsse-1.1.7/setup.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-23 21:03:27.545635 dsse-1.1.8/
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-23 21:03:27.537635 dsse-1.1.8/DSSE/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      322 2024-04-18 19:38:11.000000 dsse-1.1.8/DSSE/__init__.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-23 21:03:27.541635 dsse-1.1.8/DSSE/environment/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 14:40:14.000000 dsse-1.1.8/DSSE/environment/__init__.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      490 2024-04-18 19:38:11.000000 dsse-1.1.8/DSSE/environment/constants.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     7797 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/coverage_env.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-23 21:03:27.541635 dsse-1.1.8/DSSE/environment/entities/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-04-18 19:38:11.000000 dsse-1.1.8/DSSE/environment/entities/__init__.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      686 2024-04-18 19:38:11.000000 dsse-1.1.8/DSSE/environment/entities/drone.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     8070 2024-04-18 19:38:11.000000 dsse-1.1.8/DSSE/environment/entities/person.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    13388 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/env.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     7509 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/env_base.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-23 21:03:27.541635 dsse-1.1.8/DSSE/environment/imgs/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:19:41.000000 dsse-1.1.8/DSSE/environment/imgs/__init__.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    14774 2024-03-12 14:40:14.000000 dsse-1.1.8/DSSE/environment/imgs/drone.png
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    13193 2024-03-12 14:40:14.000000 dsse-1.1.8/DSSE/environment/imgs/person-swimming.png
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     4973 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/pygame_interface.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-23 21:03:27.541635 dsse-1.1.8/DSSE/environment/simulation/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-04-18 19:38:11.000000 dsse-1.1.8/DSSE/environment/simulation/__init__.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     4890 2024-04-18 19:38:11.000000 dsse-1.1.8/DSSE/environment/simulation/dynamic_probability.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     7794 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/simulation/particle_simulation.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1205 2024-04-18 19:38:11.000000 dsse-1.1.8/DSSE/environment/simulation/time_step.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-23 21:03:27.545635 dsse-1.1.8/DSSE/environment/wrappers/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      417 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/wrappers/__init__.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1505 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/wrappers/all_flatten_wrapper.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1701 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/wrappers/all_positions_wrapper.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1901 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/wrappers/communication_wrapper.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1391 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/wrappers/gaussian_wrapper.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1483 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/wrappers/matrix_encode_wrapper.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      975 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/wrappers/retain_drone_pos_wrapper.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1963 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/wrappers/top_n_cells_wrapper.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-23 21:03:27.545635 dsse-1.1.8/DSSE/tests/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 14:40:14.000000 dsse-1.1.8/DSSE/tests/__init__.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1488 2024-04-18 19:38:11.000000 dsse-1.1.8/DSSE/tests/drone_policy.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    17985 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/tests/test_env.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     6142 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/tests/test_env_coverage.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      581 2024-04-18 19:38:11.000000 dsse-1.1.8/DSSE/tests/test_matrix.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-23 21:03:27.545635 dsse-1.1.8/DSSE.egg-info/
+-rw-r--r--   0 ricardo   (1000) ricardo   (1000)     8639 2024-05-23 21:03:27.000000 dsse-1.1.8/DSSE.egg-info/PKG-INFO
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1311 2024-05-23 21:03:27.000000 dsse-1.1.8/DSSE.egg-info/SOURCES.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        1 2024-05-23 21:03:27.000000 dsse-1.1.8/DSSE.egg-info/dependency_links.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      257 2024-05-23 21:03:27.000000 dsse-1.1.8/DSSE.egg-info/requires.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        5 2024-05-23 21:03:27.000000 dsse-1.1.8/DSSE.egg-info/top_level.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1094 2024-04-18 19:38:11.000000 dsse-1.1.8/LICENSE
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       32 2024-05-02 18:21:55.000000 dsse-1.1.8/MANIFEST.in
+-rw-r--r--   0 ricardo   (1000) ricardo   (1000)     8639 2024-05-23 21:03:27.545635 dsse-1.1.8/PKG-INFO
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     6482 2024-05-23 20:55:10.000000 dsse-1.1.8/README.md
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     2225 2024-05-23 20:55:10.000000 dsse-1.1.8/pyproject.toml
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       38 2024-05-23 21:03:27.545635 dsse-1.1.8/setup.cfg
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      188 2024-05-23 21:02:01.000000 dsse-1.1.8/setup.py
```

### Comparing `dsse-1.1.7/DSSE/environment/coverage_env.py` & `dsse-1.1.8/DSSE/environment/coverage_env.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,58 @@
+import datetime
 from gymnasium.spaces import Discrete
 from .env_base import DroneSwarmSearchBase
 from .simulation.particle_simulation import ParticleSimulation
 from .constants import Reward
 import numpy as np
 import functools
 
 
 class CoverageDroneSwarmSearch(DroneSwarmSearchBase):
     metadata = {
         "name": "DroneSwarmSearchCPP",
     }
-    reward_scheme = Reward(
-        default=0,
-        leave_grid=-10,
-        exceed_timestep=-100,
-        drones_collision=-10,
-        search_cell=10,
-        search_and_find=100,
-    )
+    reward_scheme = {
+        "default": -0.2,
+        "exceed_timestep": 0.0,
+        "search_cell": 1.0,
+        "done": 60,
+        "reward_poc": 45.0
+    }
 
     def __init__(
         self,
         render_mode="ansi",
         render_grid=True,
         render_gradient=True,
         timestep_limit=100,
         disaster_position=(-24.04, -46.17),
         drone_amount=1,
         drone_speed=10,
         drone_probability_of_detection=0.9,
         pre_render_time=10,
         prob_matrix_path=None,
+        particle_amount=50_000,
+        particle_radius=800,
+        num_particle_to_filter_as_noise=1,
+        start_time: datetime = None,
+        grid_cell_size=130,
     ) -> None:
-
-        # Prob matrix
+        
+        if start_time is None:
+            start_time = datetime.datetime.now()
+        
         self.probability_matrix = ParticleSimulation(
             disaster_lat=disaster_position[0],
             disaster_long=disaster_position[1],
+            start_time=start_time,
             duration_hours=pre_render_time,
+            particle_amount=particle_amount,
+            particle_radius=particle_radius,
+            num_particle_to_filter_as_noise=num_particle_to_filter_as_noise
         )
         if prob_matrix_path is not None:
             if not isinstance(prob_matrix_path, str):
                 raise ValueError("prob_matrix_path must be a string")
             self.probability_matrix.load_state(prob_matrix_path)
         else: 
             self.probability_matrix.run_or_get_simulation()
@@ -52,14 +63,15 @@
             render_mode=render_mode,
             render_grid=render_grid,
             render_gradient=render_gradient,
             timestep_limit=timestep_limit,
             drone_amount=drone_amount,
             drone_speed=drone_speed,
             probability_of_detection=drone_probability_of_detection,
+            grid_cell_size=grid_cell_size,
         )
         self.disaster_position = disaster_position
         # Sets used to keep track of the seen and not seen states for reward calculation
         self.seen_states = None
         self.not_seen_states = None
         self.all_states = {
             (x, y) for x in range(self.grid_size) for y in range(self.grid_size)
@@ -68,127 +80,130 @@
         self.cumm_pos = 0
 
     def reset(self, seed=None, options=None):
         obs, _ = super().reset(seed=seed, options=options)
 
         self.reset_search_state()
 
+        self.reward_scheme["done"] = len(self.not_seen_states) / len(self.agents)
+        self.reward_scheme["reward_poc"] = len(self.not_seen_states)
         self.cumm_pos = 0
         self.repeated_coverage = 0
         infos = self.compute_infos(False)
         return obs, infos
 
     def reset_search_state(self):
         # This is in (x, y)
-        self.seen_states = {pos for pos in self.agents_positions}
+        self.seen_states = set()
+        self.not_seen_states: set = self.all_states.copy()
 
         mat = self.probability_matrix.get_matrix()
         # (row, col)
         close_to_zero = np.argwhere(np.abs(mat) < 1e-10)
-
+        
         # Remove the need to visit cells with POC near to 0
         for y, x in close_to_zero:
-            self.seen_states.add((x, y))
+            point = (x, y)
+            if point in self.not_seen_states:
+                self.not_seen_states.remove(point)
 
-        self.not_seen_states = self.all_states - self.seen_states
 
     def create_observations(self):
         observations = {}
 
         probability_matrix = self.probability_matrix.get_matrix()
+        prob_max = probability_matrix.max()
+        norm = probability_matrix / prob_max
         for idx, agent in enumerate(self.agents):
             observation = (
                 self.agents_positions[idx],
-                probability_matrix,
+                norm,
             )
             observations[agent] = observation
 
         return observations
 
     def pre_search_simulate(self):
         self.probability_matrix.run_or_get_simulation()
 
     def step(self, actions: dict[str, int]) -> tuple:
         if not self._was_reset:
             raise ValueError("Please reset the env before interacting with it")
 
         terminations = {a: False for a in self.agents}
-        rewards = {a: self.reward_scheme.default for a in self.agents}
+        rewards = {a: self.reward_scheme["default"] for a in self.agents}
         truncations = {a: False for a in self.agents}
         self.timestep += 1
 
         prob_matrix = self.probability_matrix.get_matrix()
         for idx, agent in enumerate(self.agents):
             if agent not in actions:
                 raise ValueError("Missing action for " + agent)
 
             drone_action = actions[agent]
             if drone_action not in self.action_space(agent):
                 raise ValueError("Invalid action for " + agent)
 
 
             if self.timestep >= self.timestep_limit:
-                rewards[agent] = self.reward_scheme.exceed_timestep
+                rewards[agent] = self.reward_scheme["exceed_timestep"]
                 truncations[agent] = True
                 continue
-
-            # Action 8 is to stay in the same position, default reward.
-            if drone_action == 8:
-                continue
         
             drone_x, drone_y = self.agents_positions[idx]
             new_position = self.move_drone((drone_x, drone_y), drone_action)
             if not self.is_valid_position(new_position):
-                rewards[agent] = self.reward_scheme.leave_grid
                 continue
 
             self.agents_positions[idx] = new_position
             new_x, new_y = new_position
             if new_position in self.not_seen_states:
-                reward_poc = (1 / (self.timestep)) * prob_matrix[new_y, new_x] * 1_000
-                rewards[agent] = self.reward_scheme.search_cell + reward_poc
+                time_multiplier = (1 - self.timestep / self.timestep_limit)
+                reward_poc = time_multiplier * prob_matrix[new_y, new_x] * self.reward_scheme["reward_poc"]
+                rewards[agent] = self.reward_scheme["search_cell"] + reward_poc
                 self.seen_states.add(new_position)
                 self.not_seen_states.remove(new_position)
                 # Probability of sucess (POS) = POC * POD
                 self.cumm_pos += prob_matrix[new_y, new_x] * self.drone.pod
                 # Remove the probability of the visited cell.
                 prob_matrix[new_y, new_x] = 0.0
             else:
+                # rewards[agent] = -
                 self.repeated_coverage += 1
 
         # Get dummy infos
         is_completed = len(self.not_seen_states) == 0
         if self.render_mode == "human":
             self.render()
 
         if is_completed:
-            # TODO: Proper define reward for completing the search (R_done)
+            # (R_done)
+            time_adjusted = (1 - self.timestep / self.timestep_limit) * self.reward_scheme["done"]
+            r_done = self.reward_scheme["done"] + time_adjusted
             rewards = {
-                drone: self.reward_scheme.search_and_find for drone in self.agents
+                drone: r_done for drone in self.agents
             }
             terminations = {drone: True for drone in self.agents}
         infos = self.compute_infos(is_completed)
 
-        self.compute_drone_collision(terminations, rewards)
         # Get observations
         observations = self.create_observations()
         # If terminted, reset the agents (pettingzoo parallel env requirement)
         if any(terminations.values()) or any(truncations.values()):
             self.agents = []
         return observations, rewards, terminations, truncations, infos
 
     def compute_infos(self, is_completed: bool) -> dict[str, dict]:
-        # TODO: Is this the best way to inform the coverage rate, Cum_pos and repetitions?
         total_states = len(self.seen_states) + len(self.not_seen_states)
         coverage_rate = len(self.seen_states) / total_states
         infos = {
             "is_completed": is_completed,
             "coverage_rate": coverage_rate,
             "repeated_coverage": self.repeated_coverage / total_states,
-            "acumulated_pos": self.cumm_pos,
+            "accumulated_pos": self.cumm_pos,
         }
         return {drone: infos for drone in self.agents}
     
     def save_matrix(self, path: str):
         self.probability_matrix.save_state(path)
 
     @functools.lru_cache(maxsize=None)
```

### Comparing `dsse-1.1.7/DSSE/environment/entities/drone.py` & `dsse-1.1.8/DSSE/environment/entities/drone.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.7/DSSE/environment/entities/person.py` & `dsse-1.1.8/DSSE/environment/entities/person.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.7/DSSE/environment/env.py` & `dsse-1.1.8/DSSE/environment/env.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 
     possible_actions = {action for action in Actions}
     metadata = {
         "name": "DroneSwarmSearchV0",
     }
 
     reward_scheme = Reward(
-        default=0.1,
-        leave_grid=-200,
-        exceed_timestep=-200,
-        drones_collision=-200,
-        search_cell=1,
-        search_and_find=200,
+        default=0.0,
+        leave_grid=0,
+        exceed_timestep=0,
+        drones_collision=0,
+        search_cell=0,
+        search_and_find=1,
     )
 
     def __init__(
         self,
         grid_size=20,
         render_mode="ansi",
         render_grid=False,
@@ -37,30 +37,32 @@
         dispersion_inc=0.1,
         dispersion_start=0.5,
         timestep_limit=100,
         person_amount=1,
         person_initial_position=(0, 0),
         drone_amount=1,
         drone_speed=10,
-        probability_of_detection=1,
+        probability_of_detection=1.0,
         pre_render_time=0,
+        grid_cell_size=130,
     ):
         if person_amount <= 0:
             raise ValueError("The number of persons must be greater than 0.")
         self.person_amount = person_amount
 
         super().__init__(
             grid_size=grid_size,
             render_mode=render_mode,
             render_grid=render_grid,
             render_gradient=render_gradient,
             timestep_limit=timestep_limit,
             drone_amount=drone_amount,
             drone_speed=drone_speed,
             probability_of_detection=probability_of_detection,
+            grid_cell_size=grid_cell_size,
         )
 
         self.pre_render_steps = round(
             (pre_render_time * 60)
             / (self.calculate_simulation_time_step(drone_speed, self.cell_size))
         )
         print(f"Pre render time: {pre_render_time} minutes")
@@ -237,16 +239,14 @@
             drone_action = actions[agent]
             if drone_action not in self.action_space(agent):
                 raise ValueError("Invalid action for " + agent)
 
             # Check truncation conditions (overwrites termination conditions)
             if self.timestep >= self.timestep_limit:
                 rewards[agent] = self.reward_scheme.exceed_timestep
-                if self.rewards_sum[agent] > 0:
-                    rewards[agent] += self.rewards_sum[agent] // 2
                 truncations[agent] = True
                 terminations[agent] = True
                 continue
 
             drone_x, drone_y = self.agents_positions[idx]
             is_searching = drone_action == Actions.SEARCH.value
 
@@ -284,28 +284,24 @@
                     )
 
                 if len(self.persons_set) == 0:
                     person_found = True
                     for agent in self.agents:
                         terminations[agent] = True
                         truncations[agent] = True
-            elif is_searching:
-                prob_matrix = self.probability_matrix.get_matrix()
-                rewards[agent] = (
-                    prob_matrix[drone_y][drone_x]
-                )
 
             self.rewards_sum[agent] += rewards[agent]
 
         self.timestep += 1
         # Get dummy infos
         infos = {drone: {"Found": person_found} for drone in self.agents}
 
         # CHECK COLISION - Drone
-        self.compute_drone_collision(terminations, rewards)
+        # self.compute_drone_collision(terminations, rewards)
+
 
         self.render_step(any(terminations.values()), person_found)
 
         # Get observations
         observations = self.create_observations()
         # If terminated, reset the agents (pettingzoo parallel env requirement)
         if any(terminations.values()) or any(truncations.values()):
```

### Comparing `dsse-1.1.7/DSSE/environment/env_base.py` & `dsse-1.1.8/DSSE/environment/env_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import functools
 import numpy as np
 from abc import ABC, abstractmethod
 from pettingzoo import ParallelEnv
 from .entities.drone import DroneData
 from .pygame_interface import PygameInterface
-from .simulation.dynamic_probability import ProbabilityMatrix
 from .constants import Actions
 from gymnasium.spaces import MultiDiscrete, Discrete, Tuple, Box
 from copy import copy
 
 
 class DroneSwarmSearchBase(ABC, ParallelEnv):
     def __init__(
@@ -17,16 +16,17 @@
         render_mode="ansi",
         render_grid=False,
         render_gradient=True,
         timestep_limit=100,
         drone_amount=1,
         drone_speed=10,
         probability_of_detection=1,
+        grid_cell_size=130,
     ) -> None:
-        self.cell_size = 130  # in meters
+        self.cell_size = grid_cell_size  # in meters
         self.grid_size = grid_size
         self._was_reset = False
         if not isinstance(drone_amount, int):
             raise ValueError("Drone amount must be an integer")
     
         self.drone = DroneData(
             amount=drone_amount,
@@ -56,15 +56,15 @@
             agent_name = "drone" + str(i)
             self.possible_agents.append(agent_name)
 
         self.render_mode = render_mode
 
         # Initializing render
         self.pygame_renderer = PygameInterface(
-            self.grid_size, render_gradient, render_grid
+            self.grid_size, render_gradient, render_grid, self.metadata["name"]
         )
 
     def calculate_simulation_time_step(
         self, drone_max_speed: float, cell_size: float, wind_resistance: float = 0.0
     ) -> float:
         """
         Calculate the time step for the simulation based on the maximum speed of the drones and the cell size
@@ -159,29 +159,14 @@
     def create_observations(self):
         raise NotImplementedError("Method not implemented")
 
     @abstractmethod
     def step(self, actions):
         raise NotImplementedError("Method not implemented")
 
-    def compute_drone_collision(self, terminations, rewards):
-        """
-        Check for drone collision and compute terminations, rewards and truncations.
-        """
-        for drone_1_id in range(len(self.agents)):
-            for drone_2_id in range(drone_1_id + 1, len(self.agents)):
-                drone_1_name = self.agents[drone_1_id]
-                drone_2_name = self.agents[drone_2_id]
-                if self.agents_positions[drone_1_id] == self.agents_positions[drone_2_id]:
-                    terminations[drone_1_name] = True
-                    terminations[drone_2_name] = True
-                    rewards[drone_1_name] = self.reward_scheme.drones_collision
-                    rewards[drone_2_name] = self.reward_scheme.drones_collision
-
-
     def move_drone(self, position, action):
         """
         Returns a tuple with (is_terminal, new_position, reward)
         """
         match action:
             case Actions.LEFT.value:  # LEFT
                 new_position = (position[0] - 1, position[1])
@@ -195,14 +180,16 @@
                 new_position = (position[0] - 1, position[1] - 1)
             case Actions.UP_RIGHT.value:  # UP_RIGHT
                 new_position = (position[0] + 1, position[1] - 1)
             case Actions.DOWN_LEFT.value:  # DOWN_LEFT
                 new_position = (position[0] - 1, position[1] + 1)
             case Actions.DOWN_RIGHT.value:  # DOWN_RIGHT
                 new_position = (position[0] + 1, position[1] + 1)
+            case _:
+                new_position = position
 
         return new_position
 
     def get_agents(self):
         return self.possible_agents
 
     @functools.lru_cache(maxsize=None)
@@ -213,15 +200,15 @@
         return Tuple(
             (
                 MultiDiscrete([self.grid_size, self.grid_size]),
                 Box(
                     low=0,
                     high=1,
                     shape=(self.grid_size, self.grid_size),
-                    dtype=np.float32,
+                    dtype=np.float64,
                 ),
             )
         )
 
     @functools.lru_cache(maxsize=None)
     def action_space(self, agent):
         return Discrete(len(self.possible_actions))
```

### Comparing `dsse-1.1.7/DSSE/environment/imgs/drone.png` & `dsse-1.1.8/DSSE/environment/imgs/drone.png`

 * *Files identical despite different names*

### Comparing `dsse-1.1.7/DSSE/environment/imgs/person-swimming.png` & `dsse-1.1.8/DSSE/environment/imgs/person-swimming.png`

 * *Files identical despite different names*

### Comparing `dsse-1.1.7/DSSE/environment/pygame_interface.py` & `dsse-1.1.8/DSSE/environment/pygame_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,25 @@
     """
     Class for rendering the grafical interface of the simulation
     """
 
     FPS = 5
 
     def __init__(
-        self, grid_size: int, render_gradient: bool, render_grid: bool
+        self, grid_size: int, render_gradient: bool, render_grid: bool, env_name: str
     ) -> None:
         pygame.init()
         self.grid_size = grid_size
         self.render_gradient = render_gradient
         self.render_grid = render_grid
         self.window_size = 700
         self.screen = None
         self.render_on = False
         self.probability_matrix = None
+        self.env_name = env_name
 
         self.block_size = self.window_size / self.grid_size
         self.drone_img = None
         self.person_img = None
         self.clock = None
 
     def render_map(self):
@@ -122,15 +123,21 @@
             green = 0
             if normalized_prob >= 0.75:
                 red = 0
                 green = 255
             elif normalized_prob >= 0.25:
                 red = 255
                 green = 255
-        return (red, green, 0)
+        
+        if self.env_name == "DroneSwarmSearchCPP":
+            blue = 255 if normalized_prob > 0 else 0
+        else:
+            blue = 0
+        
+        return (red, green, blue)
 
     def render_episode_end_screen(self, message: str, color: tuple):
         font = pygame.font.SysFont(None, 50)
         text = font.render(message, True, BLACK)
         text_rect = text.get_rect(center=(self.window_size // 2, self.window_size // 2))
         self.screen.fill(color)
         self.screen.blit(text, text_rect)
```

### Comparing `dsse-1.1.7/DSSE/environment/simulation/dynamic_probability.py` & `dsse-1.1.8/DSSE/environment/simulation/dynamic_probability.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.7/DSSE/environment/simulation/particle_simulation.py` & `dsse-1.1.8/DSSE/environment/simulation/particle_simulation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,84 @@
 import math
 import numpy as np
 from datetime import datetime, timedelta
 from typing import List, Tuple
 
-
 EARTH_MEAN_RADIUS = 6373.0
 
 
 class ParticleSimulation:
     def __init__(
         self,
         disaster_lat: float,
         disaster_long: float,
+        start_time: datetime,
         duration_hours: int = 10,
         loglevel: int = 20,
         animate: bool = False,
         cell_size: int = 130,
+        particle_amount: int = 50_000,
+        particle_radius: int = 1000,
+        num_particle_to_filter_as_noise: int = 0,
     ) -> None:
         try:
             from opendrift.models.oceandrift import OceanDrift
+
             self.ocean_drift = OceanDrift
         except ImportError:
-            raise ImportError("OpenDrift not installed. Install the environment with the 'coverage' extra: pip install DSSE[coverage]")
-        
+            raise ImportError(
+                "OpenDrift not installed. Install the environment with the 'coverage' extra: pip install DSSE[coverage]"
+            )
+
         self.disaster_lat = disaster_lat
         self.disaster_long = disaster_long
+        self.start_time = start_time
         self.loglevel = loglevel
         self.animate = animate
         self.duration_hours = duration_hours
         self.cell_size = cell_size
+        self.particle_amount = particle_amount
+        self.particle_radius = particle_radius
+        self.particles_as_noise = num_particle_to_filter_as_noise
 
         # Internal variables
         self.map_size = 0
         self.original_map = None
         self.probability_map = None
 
     def run_or_get_simulation(self):
         if self.probability_map is None:
             self.run_simulation()
         self.probability_map = self.original_map.copy()
 
     def run_simulation(self):
         duration = timedelta(hours=self.duration_hours)
-        start_time = datetime.now() - duration
-        number = 50_000
-        radius = 1000
 
-        coordinates = self.simulate(start_time, number, radius, duration)
+        coordinates = self.simulate(duration)
         self.map_size = self.calculate_map_size(coordinates)
         cartesian = self.convert_lat_lon_to_xy(coordinates)
         self.probability_map = self.create_probability_map(cartesian)
         # Maintain always a copy of the original map
         self.original_map = self.probability_map.copy()
 
-    def simulate(
-        self,
-        time: datetime,
-        number: int,
-        radius: int,
-        duration: timedelta,
-    ) -> List[Tuple[float, float]]:
+    def simulate(self, duration: timedelta) -> List[Tuple[float, float]]:
         o = self.ocean_drift(loglevel=self.loglevel)
+        # Add Wind & Ocean data
         o.add_readers_from_list(
-            ["https://tds.hycom.org/thredds/dodsC/GLBy0.08/expt_93.0/uv3z"]
+            [
+                "https://tds.hycom.org/thredds/dodsC/GLBy0.08/expt_93.0/uv3z",
+                "https://pae-paha.pacioos.hawaii.edu/thredds/dodsC/ncep_global/NCEP_Global_Atmospheric_Model_best.ncd",
+            ]
         )
         o.seed_elements(
             lat=self.disaster_lat,
             lon=self.disaster_long,
-            time=time,
-            number=number,
-            radius=radius,
+            time=self.start_time,
+            number=self.particle_amount,
+            radius=self.particle_radius,
         )
 
         o.run(duration=duration, time_step=1800)
         if self.animate:
             o.animation(filename="animation.mp4")
 
         lat_final = o.elements.lat
@@ -164,33 +169,62 @@
 
     def create_probability_map(
         self, cartesian_coords: List[Tuple[float, float]]
     ) -> List[List[int]]:
         """
         Creates a probability map based on the coordinates of the particles.
         """
-        prob_map = np.zeros((self.map_size, self.map_size))
+        prob_map = np.zeros((self.map_size, self.map_size), dtype=np.float64)
 
         for x, y in cartesian_coords:
             prob_map[y][x] += 1
 
-        particle_sum = max(np.sum(prob_map), 1)
+        prob_map[prob_map <= self.particles_as_noise] = 0.0
+        prob_map = self.trimm_map(prob_map)
+        self.map_size = len(prob_map)
 
+        particle_sum = max(np.sum(prob_map), 1)
         probability_map = prob_map / particle_sum
         return probability_map
 
+    def trimm_map(self, prob_map) -> np.ndarray:
+        """
+        Trims map to fit cells with particles.
+        """
+        zero_values = np.argwhere(prob_map > 0)
+        row_min, col_min = zero_values.min(axis=0)
+        row_max, col_max = zero_values.max(axis=0)
+
+        new_width = row_max - row_min
+        new_height = col_max - col_min
+
+        # Pad the map to make it square
+        padding = ((0, 0), (0, 0))
+        if new_width > new_height:
+            padding = ((0, 0), (0, new_width - new_height))
+        elif new_height > new_width:
+            padding = ((0, new_height - new_width), (0, 0))
+
+        # Pads with zeros (there were no particles there anyway)
+        res = np.pad(
+            prob_map[row_min:row_max, col_min:col_max],
+            padding,
+            mode="constant",
+            constant_values=0.0,
+        )
+        return res
+
     def get_matrix(self):
         return self.probability_map
 
     def get_map_size(self):
         return self.map_size
-    
+
     def save_state(self, output_path: str):
         with open(output_path, "wb") as f:
             np.save(f, self.original_map)
-        
-    
+
     def load_state(self, input_path: str):
         with open(input_path, "rb") as f:
             self.probability_map = np.load(f)
             self.original_map = self.probability_map.copy()
-            self.map_size = len(self.probability_map)
+            self.map_size = len(self.probability_map)
```

### Comparing `dsse-1.1.7/DSSE/environment/simulation/time_step.py` & `dsse-1.1.8/DSSE/environment/simulation/time_step.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.7/DSSE/environment/wrappers/all_positions_wrapper.py` & `dsse-1.1.8/DSSE/environment/wrappers/all_positions_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,45 +6,49 @@
 
 class AllPositionsWrapper(BaseParallelWrapper):
     """
     Wrapper that modifies the observation space to include the positions of all agents in all observations
     """
     def __init__(self, env: DroneSwarmSearch):
         super().__init__(env)
+
+        self.observation_spaces = {
+            agent: self.observation_space(agent)
+            for agent in self.env.possible_agents
+        }
     
     def step(self, actions):
         obs, reward, terminated, truncated, infos = self.env.step(actions)
         self.add_other_positions_obs(obs)
         return obs, reward, terminated, truncated, infos
     
     def add_other_positions_obs(self, obs):
-        prob_matrix = obs["drone0"][1]
-        for idx, agent in enumerate(self.env.agents):
+        for idx, agent in enumerate(obs.keys()):
             agents_positions = np.array(self.env.agents_positions, dtype=np.int64)
-            agents_positions[[0, idx]] = agents_positions[[idx, 0]]            
+            agents_positions[[0, idx]] = agents_positions[[idx, 0]]         
             obs[agent] = (
-                agents_positions,
-                prob_matrix
+                agents_positions.flatten(),
+                obs[agent][1]
             )
 
     
     def reset(self, **kwargs):
         obs, infos = self.env.reset(**kwargs)
         self.add_other_positions_obs(obs)
         return obs, infos
 
     def observation_space(self, agent):
         return Tuple(
             (
-                Box(0, self.env.grid_size, shape=(len(self.env.possible_agents), 2), dtype=np.int64),
+                Box(0, self.env.grid_size, shape=(len(self.env.possible_agents) * 2, ), dtype=np.int64),
                 Box(
                     low=0,
                     high=1,
                     shape=(self.env.grid_size, self.env.grid_size),
-                    dtype=np.float32,
+                    dtype=np.float64,
                 )
             )
         )
```

### Comparing `dsse-1.1.7/DSSE/tests/drone_policy.py` & `dsse-1.1.8/DSSE/tests/drone_policy.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.7/DSSE/tests/test_env.py` & `dsse-1.1.8/DSSE/tests/test_env.py`

 * *Files 15% similar despite different names*

```diff
@@ -77,40 +77,14 @@
 
     assert (
         len(env.get_agents()) == drone_amount
     ), f"There should be {drone_amount} drones, but found {len(env.get_agents())}."
 
 
 @pytest.mark.parametrize(
-    "drone_amount",
-    [
-        2,
-    ],
-)
-def test_drone_collision_termination(drone_amount):
-
-    env = init_drone_swarm_search(drone_amount=drone_amount)
-    _ = env.reset()
-
-    done = False
-    while not done:
-        actions = {"drone0": Actions.SEARCH.value, "drone1": Actions.LEFT.value}
-        _, reward, terminations, truncations, _ = env.step(actions)
-        done = any(truncations.values()) or any(terminations.values())
-
-        assert done, "The simulation should terminate upon drone collision."
-        assert any(
-            terminations.values()
-        ), "There should be a termination flag set due to the collision."
-        assert (
-            sum(reward.values()) < 0
-        ), "The total reward should be negative after a collision."
-
-
-@pytest.mark.parametrize(
     "timestep_limit",
     [
         10,
         20,
         30,
         40,
         50,
@@ -140,43 +114,41 @@
         timestep_counter += 1
     assert (
         timestep_counter > timestep_limit
     ), "The simulation should run beyond the timestep limit before terminating."
 
 
 @pytest.mark.parametrize(
-    "grid_size, person_initial_position",
+    "grid_size, person_initial_position, timestep_limit",
     [
-        (15, (4, 4)),
-        (20, (10, 10)),
-        (25, (15, 15)),
-        (30, (20, 20)),
+        (15, (4, 4), 200),
+        (20, (10, 10), 100),
+        (25, (15, 15), 50),
+        (30, (20, 20), 25),
     ],
 )
-def test_leave_grid_get_negative_reward(grid_size, person_initial_position):
+def test_leave_grid_dont_finish(grid_size, person_initial_position, timestep_limit):
     env = init_drone_swarm_search(
-        grid_size=grid_size, person_initial_position=person_initial_position
+        render_mode="ansi", grid_size=grid_size, person_initial_position=person_initial_position, timestep_limit=timestep_limit
     )
     opt = {"drones_positions": [(0, 0)]}
     _ = env.reset(options=opt)
 
     done = False
     reward_sum = 0
-    while not done and reward_sum >= env.reward_scheme.leave_grid * (env.timestep_limit - 1):
+    steps = 0
+    while not done and steps < timestep_limit:
         actions = {"drone0": Actions.UP.value}
         _, reward, terminations, done, _ = env.step(actions)
         done = any(done.values())
-        reward_sum += sum(reward.values())
+        steps += 1
 
     assert (
         not done
     ), "The simulation should not end, indicating the drone left the grid or another termination condition was met."
-    assert (
-        sum(reward.values()) < 0
-    ), "The total reward should be negative, indicating a penalty was applied."
     assert not any(
         terminations.values()
     ), "There not should be at least one termination condition met."
 
 
 @pytest.mark.parametrize(
     "grid_size, person_position",
@@ -239,14 +211,223 @@
 @pytest.mark.parametrize(
     "drone_amount, drones_positions",
     [
         (1, [(-1, 3)]),
         (2, [(12, 0), (25, 13)]),
         (3, [(0, 0), (19, 19), (25, -10)]),
         (4, [(5, 0), (0, 0), (10, 10), (10, 10)]),
+    ],
+)
+def test_invalid_drone_position_raises_error(drone_amount, drones_positions):
+    with pytest.raises(ValueError):
+        env = init_drone_swarm_search(drone_amount=drone_amount)
+        opt = {"drones_positions": drones_positions}
+        _ = env.reset(options=opt)
+
+
+@pytest.mark.parametrize(
+    "drone_amount",
+    [
+        1,
+        20,
+        35,
+        48,
+    ],
+)
+def test_if_all_drones_are_created_with_default_positions(drone_amount):
+    env = init_drone_swarm_search(drone_amount=drone_amount)
+
+    _ = env.reset()
+
+    assert (
+        len(env.get_agents()) == drone_amount
+    ), f"Should have {drone_amount} drones, but found {len(env.get_agents())}."
+
+
+@pytest.mark.parametrize(
+    "drone_amount, grid_size",
+    [
+        (1, 10),
+        (2, 15),
+        (5, 20),
+        (15, 25),
+    ],
+)
+def test_with_the_observation_size_is_correct_for_all_drones(drone_amount, grid_size):
+    env = init_drone_swarm_search(grid_size=grid_size, drone_amount=drone_amount)
+
+    observations, _ = env.reset()
+
+    for drone in range(drone_amount):
+        drone_id = f"drone{drone}"
+        observation_matriz = observations[drone_id][1]
+
+        assert observation_matriz.shape == (
+            grid_size,
+            grid_size,
+        ), f"The observation matrix for {drone_id} should have a shape of ({grid_size}, {grid_size}), but was {observation_matriz.shape}."
+
+
+def test_petting_zoo_interface_works():
+    env = init_drone_swarm_search()
+    parallel_api_test(env)
+    env.close()
+
+
+@pytest.mark.parametrize(
+    "person_initial_position, person_amount",
+    [
+        ((10, 10), 10),
+        ((10, 10), 15),
+        ((10, 10), 20),
+        ((10, 10), 25),
+    ],
+)
+def test_castaway_count_after_reset(person_initial_position, person_amount):
+    env = init_drone_swarm_search(
+        person_amount=person_amount, person_initial_position=person_initial_position
+    )
+    _ = env.reset()
+
+    assert (
+        len(env.get_persons()) == person_amount
+    ), f"Should have {person_amount} castaways, but found {len(env.get_persons())}."
+
+
+@pytest.mark.parametrize(
+    "person_initial_position, person_amount, drone_amount",
+    [
+        ((10, 10), 1, 1),
+        ((1, 10), 5, 1),
+        ((19, 5), 10, 1),
+        ((5, 16), 15, 1),
+    ],
+)
+def test_castaway_count_after_reset(
+    person_initial_position, person_amount, drone_amount
+):
+    env = init_drone_swarm_search(
+        person_amount=person_amount,
+        person_initial_position=person_initial_position,
+        drone_amount=drone_amount,
+    )
+    observations = env.reset()
+
+    rewards = 0
+    done = False
+    while not done:
+        actions = policy(observations, env.get_agents(), env)
+        observations, reward, _, done, info = env.step(actions)
+        rewards += sum(reward.values())
+        done = any(done.values())
+
+    _ = env.reset()
+
+    assert (
+        rewards >= DroneSwarmSearch.reward_scheme.search_and_find * person_amount
+    ), f"The total reward should be positive after finding all castaways. But the total reward was: {rewards}."
+    assert done, "The simulation should end after finding all castaways."
+    assert (
+        len(env.get_persons()) == person_amount
+    ), f"Should have {person_amount} castaways, but found {len(env.get_persons())}."
+    assert (
+        len(env.get_agents()) == drone_amount
+    ), f"Should have {drone_amount} drones, but found {len(env.get_agents())}."
+
+
+@pytest.mark.parametrize(
+    "pre_render_time, cell_size, drone_max_speed, wind_resistance",
+    [
+        (1, 130, 10, 0.0),
+        (5, 130, 20, 0.0),
+        (10, 130, 30, 0.0),
+        (15, 130, 40, 0.0),
+        (20, 130, 50, 0.0),
+    ],
+)
+def test_pre_render_work_after_reset(
+    pre_render_time, cell_size, drone_max_speed, wind_resistance
+):
+    env = init_drone_swarm_search(
+        pre_render_time=pre_render_time, drone_speed=drone_max_speed
+    )
+    _ = env.reset()
+    pre_render_steps = round(
+        (pre_render_time * 60) / (cell_size / (drone_max_speed - wind_resistance))
+    )
+
+    assert (
+        env.pre_render_steps == pre_render_steps
+    ), f"The pre-render time should be {pre_render_steps}, but was {env.pre_render_time}."
+
+    _ = env.reset()
+
+    assert (
+        env.pre_render_steps == pre_render_steps
+    ), f"The pre-render time should be {pre_render_steps}, but was {env.pre_render_time}."
+
+
+@pytest.mark.parametrize(
+    "person_amount, mult",
+    [
+        (1, ["1"]),
+        (2, [1, "0.8"]),
+        (3, [1, "0.8", 0.7]),
+        (4, ["1", 0.8, "0.7", 0.6]),
+        (5, ["1", "0.8", "0.7", "0.6", "0.5"]),
+    ],
+)
+def test_get_wrong_if_scale_pod_is_not_a_number(person_amount, mult):
+    with pytest.raises(Exception):
+        env = init_drone_swarm_search(person_amount=person_amount)
+        opt = {"person_pod_multipliers": mult}
+        _ = env.reset(options=opt)
+
+
+@pytest.mark.parametrize(
+    "person_amount, mult",
+    [
+        (1, [-1.2]),
+        (2, [1, -0.8]),
+        (3, [1, -0.8, 1.7]),
+        (4, [1, 0.8, -0.7, 0.6]),
+        (5, [1, 0.8, -0, 0.6, -3.5]),
+    ],
+)
+def test_get_wrong_if_scale_mult_is_not_greater_than_0(person_amount, mult):
+    with pytest.raises(Exception):
+        env = init_drone_swarm_search(person_amount=person_amount)
+        opt = {"person_pod_multipliers": mult}
+        _ = env.reset(options=opt)
+
+
+@pytest.mark.parametrize(
+    "person_amount, mult",
+    [
+        (1, [1, 0.1]),
+        (2, [1]),
+        (3, [1, 0.8, 0.7, 1]),
+        (4, [1, 0.8]),
+        (5, [1, 0.8, 0.7, 0.6, 0.5, 0.6, 0.5]),
+    ],
+)
+def test_get_wrong_if_number_of_mults_is_not_equal_to_person_amount(
+    person_amount, mult
+):
+    with pytest.raises(Exception):
+        env = init_drone_swarm_search(person_amount=person_amount)
+        opt = {"person_pod_multipliers": mult}
+        _ = env.reset(options=opt)
+@pytest.mark.parametrize(
+    "drone_amount, drones_positions",
+    [
+        (1, [(-1, 3)]),
+        (2, [(12, 0), (25, 13)]),
+        (3, [(0, 0), (19, 19), (25, -10)]),
+        (4, [(5, 0), (0, 0), (10, 10), (10, 10)]),
     ],
 )
 def test_invalid_drone_position_raises_error(drone_amount, drones_positions):
     with pytest.raises(ValueError):
         env = init_drone_swarm_search(drone_amount=drone_amount)
         opt = {"drones_positions": drones_positions}
         _ = env.reset(options=opt)
```

### Comparing `dsse-1.1.7/DSSE/tests/test_env_coverage.py` & `dsse-1.1.8/DSSE/tests/test_env_coverage.py`

 * *Files 19% similar despite different names*

```diff
@@ -41,68 +41,41 @@
         4901,
     ],
 )
 def test_wrong_drone_number(drone_amount):
     with pytest.raises(ValueError):
         init_Coverage_drone_swarm_search(drone_amount=drone_amount)
 
-
-@pytest.mark.parametrize(
-    "drone_amount, drones_positions",
-    [
-        (2, [(0, 0), (2, 0),]),
-    ],
-)
-def test_drone_collision_termination(drone_amount, drones_positions):
-
-    env = init_Coverage_drone_swarm_search(drone_amount=drone_amount)
-    opt = {
-    "drones_positions": drones_positions,
-    }
-    _ = env.reset(options=opt)
-
-    done = False
-    while not done:
-        actions = {"drone0": Actions.RIGHT.value, "drone1": Actions.LEFT.value}
-        _, reward, terminations, truncations, _ = env.step(actions)
-        done = any(terminations.values()) or any(truncations.values())
-
-        assert done, "The simulation should terminate upon drone collision."
-        assert any(
-            terminations.values()
-        ), "There should be a termination flag set due to the collision."
-        assert (
-            sum(reward.values()) < 0
-        ), "The total reward should be negative after a collision."
-
 @pytest.mark.parametrize(
-    "drone_amount, drones_positions",
+    "drone_amount, drones_positions, timestep_limit",
     [
-        (1, [(0, 0)]),
+        (1, [(0, 0)], 100),
     ],
 )
-def test_leave_grid_get_negative_reward(drone_amount, drones_positions):
-    env = init_Coverage_drone_swarm_search(drone_amount=drone_amount)
+def test_leave_grid_get_negative_reward(drone_amount, drones_positions, timestep_limit):
+    env = init_Coverage_drone_swarm_search(drone_amount=drone_amount, timestep_limit=timestep_limit)
     opt = {"drones_positions": drones_positions}
     _ = env.reset(options=opt)
 
     done = False
     reward_sum = 0
-    while not done and reward_sum >=  (env.reward_scheme.leave_grid * (env.timestep_limit-1)) +1:
+    steps = 0
+    while not done and steps < timestep_limit - 1:
         actions = {"drone0": Actions.UP.value}
         _, reward, terminations, done, _ = env.step(actions)
         done = any(done.values())
         reward_sum += sum(reward.values())
+        steps += 1
 
     assert (
         not done
     ), "The simulation should not end, indicating the drone left the grid or another termination condition was met."
     assert (
         sum(reward.values()) < 0
-    ), "The total reward should be negative, indicating a penalty was applied."
+    ), f"The total reward should be negative, indicating a penalty was applied. reward: {reward_sum}"
     assert not any(
         terminations.values()
     ), "There not should be at least one termination condition met."
 
 @pytest.mark.parametrize(
     "drone_amount",
     [
```

### Comparing `dsse-1.1.7/DSSE/tests/test_matrix.py` & `dsse-1.1.8/DSSE/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.7/DSSE.egg-info/PKG-INFO` & `dsse-1.1.8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,90 +1,54 @@
-Metadata-Version: 2.1
-Name: DSSE
-Version: 1.1.7
-Summary: The Drone Swarm Search project provides an environment for SAR missions built on PettingZoo, where agents, represented by drones, are tasked with locating targets identified as shipwrecked individuals.
-Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/1.1.7.tar.gz
-Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta
-Author-email: Ricardo Ribeiro Rodrigues <ricardorr7@al.insper.edu.br>, Renato Laffranchi Falcão <renatolf1@al.insper.edu.br>, Pedro Henrique Britto Aragão Andrade <pedroa3@al.insper.edu.br>, Jorás Oliveira <jorascco@al.insper.edu.br>, Fabricio Barth <fabriciojb@insper.edu.br>
-License: MIT License
-Project-URL: Homepage, https://pfeinsper.github.io/drone-swarm-search/
-Project-URL: Repository, https://github.com/pfeinsper/drone-swarm-search/
-Project-URL: Documentation, https://pfeinsper.github.io/drone-swarm-search/
-Project-URL: Bug Report, https://github.com/pfeinsper/drone-swarm-search/issues/
-Keywords: Reinforcement Learning,AI,SAR,Multi Agent Reinforcement Learning
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.10.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy>=1.23.1
-Requires-Dist: gymnasium>=0.27.1
-Requires-Dist: pygame>=2.3.0
-Requires-Dist: pettingzoo>=1.22.3
-Requires-Dist: matplotlib>=3.7.0
-Requires-Dist: numba>=0.59.0
-Provides-Extra: all
-Requires-Dist: numpy>=1.23.1; extra == "all"
-Requires-Dist: gymnasium>=0.27.1; extra == "all"
-Requires-Dist: pygame>=2.3.0; extra == "all"
-Requires-Dist: pettingzoo>=1.22.3; extra == "all"
-Requires-Dist: matplotlib>=3.7.0; extra == "all"
-Requires-Dist: numba>=0.59.0; extra == "all"
-Requires-Dist: GDAL==3.4.1; extra == "all"
-Requires-Dist: opendrift; extra == "all"
-Provides-Extra: coverage
-Requires-Dist: GDAL==3.4.1; extra == "coverage"
-Requires-Dist: opendrift; extra == "coverage"
-
 [![Tests Status 🧪](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml/badge.svg)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml)
 [![Docs Deployment 📝](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/deploy.yml/badge.svg?branch=vitepress_docs)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/deploy.yml)
 [![PyPI Release 🚀](https://badge.fury.io/py/DSSE.svg)](https://badge.fury.io/py/DSSE)
 [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg?style=flat)](https://github.com/pfeinsper/drone-swarm-search/blob/main/LICENSE)
 [![PettingZoo version dependency](https://img.shields.io/badge/PettingZoo-v1.22.3-blue)]()
 ![GitHub stars](https://img.shields.io/github/stars/pfeinsper/drone-swarm-search)
 
 # <img src="https://github.com/pfeinsper/drone-swarm-search/blob/main/docs/public/pics/drone.svg" alt="DSSE Icon" width="45" height="25"> Drone Swarm Search Environment (DSSE)
 
-Welcome to the official GitHub repository for the Drone Swarm Search Environment (DSSE). This project is dedicated to providing a comprehensive simulation environment designed to develop, test, and refine drone swarm search strategies. Here, researchers and developers can access a versatile platform that supports a wide range of drone swarm simulations, enabling the exploration of complex behaviors and interactions within dynamic, real-world scenarios.
+Welcome to the official GitHub repository for the Drone Swarm Search Environment (DSSE). This project offers a comprehensive simulation platform designed for developing, testing, and refining search strategies using drone swarms. Researchers and developers will find a versatile toolset supporting a broad spectrum of simulations, which facilitates the exploration of complex drone behaviors and interactions in dynamic, real-world scenarios.
+
+In this repository, we have implemented two distinct types of environments. The first is a dynamic environment that simulates maritime search and rescue operations for shipwreck survivors. It models the movement of individuals in the sea using a dynamic probability matrix, with the objective for drones being to locate and identify these individuals. The second is a environment utilizing the Lagrangian particle simulation from the open-source [Opendrift library](https://github.com/OpenDrift/opendrift), which incorporates real-world ocean and wind data to create a probability matrix for drone SAR tasks. In this scenario, drones are tasked with covering the full search area within the lowest time possible, while prioritizing higher probability areas.
 
 
 ## 📚 Documentation Links
 
 - **[Documentation Site](https://pfeinsper.github.io/drone-swarm-search/)**: Access comprehensive documentation including tutorials, and usage examples for the Drone Swarm Search Environment (DSSE). Ideal for users seeking detailed information about the project's capabilities and how to integrate them into their own applications.
 
 - **[Algorithm Details](https://github.com/pfeinsper/drone-swarm-search-algorithms)**: Explore in-depth discussions and source code for the algorithms powering the DSSE. This section is perfect for developers interested in the technical underpinnings and enhancements of the search algorithms.
 
 - **[PyPI Repository](https://pypi.org/project/DSSE/)**: Visit the PyPI page for DSSE to download the latest release, view release histories, and read additional installation instructions.
 
+# DSSE - Search Environment
+
 ## 🎥 Visual Demonstrations
 <p align="center">
-    <img src="https://raw.github.com/PFE-Embraer/drone-swarm-search/env-cleanup/docs/gifs/render_with_grid_gradient.gif" width="400" height="400" align="center">
+    <img src="docs/public/gifs/render_with_grid_gradient.gif" width="400" height="400" align="center">
     <br>
     <em>Above: A simulation showing how drones adjust their search pattern over a grid.</em>
 </p>
 
-## ⚡Quick Start
-
-### ⚙️ Installation
-Install DSSE quickly with pip:
-```bash
-pip install DSSE
-````
-
 ## 🎯 Outcome
 
 | If target is found       | If target is not found   |
 :-------------------------:|:-------------------------:
 | ![](https://raw.githubusercontent.com/PFE-Embraer/drone-swarm-search/main/docs/public/pics/victory_render.png)     | ![](https://raw.github.com/PFE-Embraer/drone-swarm-search/main/docs/public/pics/fail_render.png) |
 
+## ⚡ Quick Start
+
+### ⚙️ Installation
+Quickly install DSSE using pip:
+```bash
+pip install DSSE
+````
+
 
-## 🛠️ Basic Env Usage
+## 🛠️ Basic Env Search Usage
 ```python
 from DSSE import DroneSwarmSearch
 
 env = DroneSwarmSearch(
     grid_size=40,
     render_mode="human",
     render_grid=True,
@@ -107,35 +71,55 @@
         actions[agent] = env.action_space(agent).sample()
     return actions
 
 
 opt = {
     "drones_positions": [(10, 5), (10, 10)],
     "person_pod_multipliers": [0.1, 0.4, 0.5, 1.2],
+    "vector": (0.3, 0.3),
 }
 observations, info = env.reset(options=opt)
 
 rewards = 0
 done = False
 while not done:
     actions = random_policy(observations, env.get_agents())
     observations, rewards, terminations, truncations, infos = env.step(actions)
     done = any(terminations.values()) or any(truncations.values())
+
 ```
 
+
+# DSSE - Coverage Environment
+
+## 🎥 Visual Demonstrations
+<p align="center">
+    <img src="docs/public/gifs/basic_coverage.gif" width="400" height="400" align="center">
+    <br>
+    <em>Above: A simulation showing how drones adjust their search pattern over a grid.</em>
+</p>
+
+## ⚡ Quick Start
+
+### ⚙️ Installation
+Install DSSE with coverage support using pip:
+```bash
+pip install DSSE[coverage]
+````
+
+
 ## 🛠️ Basic Coverage Usage
 ```python
 from DSSE import CoverageDroneSwarmSearch
 
 env = CoverageDroneSwarmSearch(
-    grid_size=40,
     drone_amount=3,
-    dispersion_inc=0.1,
-    vector=(1, 1),
     render_mode="human",
+    disaster_position=(-24.04, -46.17),  # (lat, long)
+    pre_render_time=10, # hours to simulate
 )
 
 opt = {
     "drones_positions": [(0, 10), (10, 10), (20, 10)],
 }
 obs, info = env.reset(options=opt)
```

### Comparing `dsse-1.1.7/DSSE.egg-info/SOURCES.txt` & `dsse-1.1.8/DSSE.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -21,13 +21,20 @@
 DSSE/environment/imgs/__init__.py
 DSSE/environment/imgs/drone.png
 DSSE/environment/imgs/person-swimming.png
 DSSE/environment/simulation/__init__.py
 DSSE/environment/simulation/dynamic_probability.py
 DSSE/environment/simulation/particle_simulation.py
 DSSE/environment/simulation/time_step.py
+DSSE/environment/wrappers/__init__.py
+DSSE/environment/wrappers/all_flatten_wrapper.py
 DSSE/environment/wrappers/all_positions_wrapper.py
+DSSE/environment/wrappers/communication_wrapper.py
+DSSE/environment/wrappers/gaussian_wrapper.py
+DSSE/environment/wrappers/matrix_encode_wrapper.py
+DSSE/environment/wrappers/retain_drone_pos_wrapper.py
+DSSE/environment/wrappers/top_n_cells_wrapper.py
 DSSE/tests/__init__.py
 DSSE/tests/drone_policy.py
 DSSE/tests/test_env.py
 DSSE/tests/test_env_coverage.py
 DSSE/tests/test_matrix.py
```

### Comparing `dsse-1.1.7/LICENSE` & `dsse-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dsse-1.1.7/PKG-INFO` & `dsse-1.1.8/DSSE.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: DSSE
-Version: 1.1.7
+Version: 1.1.8
 Summary: The Drone Swarm Search project provides an environment for SAR missions built on PettingZoo, where agents, represented by drones, are tasked with locating targets identified as shipwrecked individuals.
-Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/1.1.7.tar.gz
+Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/1.1.8.tar.gz
 Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta
 Author-email: Ricardo Ribeiro Rodrigues <ricardorr7@al.insper.edu.br>, Renato Laffranchi Falcão <renatolf1@al.insper.edu.br>, Pedro Henrique Britto Aragão Andrade <pedroa3@al.insper.edu.br>, Jorás Oliveira <jorascco@al.insper.edu.br>, Fabricio Barth <fabriciojb@insper.edu.br>
 License: MIT License
 Project-URL: Homepage, https://pfeinsper.github.io/drone-swarm-search/
 Project-URL: Repository, https://github.com/pfeinsper/drone-swarm-search/
 Project-URL: Documentation, https://pfeinsper.github.io/drone-swarm-search/
 Project-URL: Bug Report, https://github.com/pfeinsper/drone-swarm-search/issues/
@@ -19,22 +19,22 @@
 Requires-Python: >=3.10.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.23.1
 Requires-Dist: gymnasium>=0.27.1
 Requires-Dist: pygame>=2.3.0
 Requires-Dist: pettingzoo>=1.22.3
-Requires-Dist: matplotlib>=3.7.0
+Requires-Dist: matplotlib==3.8.4
 Requires-Dist: numba>=0.59.0
 Provides-Extra: all
 Requires-Dist: numpy>=1.23.1; extra == "all"
 Requires-Dist: gymnasium>=0.27.1; extra == "all"
 Requires-Dist: pygame>=2.3.0; extra == "all"
 Requires-Dist: pettingzoo>=1.22.3; extra == "all"
-Requires-Dist: matplotlib>=3.7.0; extra == "all"
+Requires-Dist: matplotlib==3.8.4; extra == "all"
 Requires-Dist: numba>=0.59.0; extra == "all"
 Requires-Dist: GDAL==3.4.1; extra == "all"
 Requires-Dist: opendrift; extra == "all"
 Provides-Extra: coverage
 Requires-Dist: GDAL==3.4.1; extra == "coverage"
 Requires-Dist: opendrift; extra == "coverage"
 
@@ -43,48 +43,52 @@
 [![PyPI Release 🚀](https://badge.fury.io/py/DSSE.svg)](https://badge.fury.io/py/DSSE)
 [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg?style=flat)](https://github.com/pfeinsper/drone-swarm-search/blob/main/LICENSE)
 [![PettingZoo version dependency](https://img.shields.io/badge/PettingZoo-v1.22.3-blue)]()
 ![GitHub stars](https://img.shields.io/github/stars/pfeinsper/drone-swarm-search)
 
 # <img src="https://github.com/pfeinsper/drone-swarm-search/blob/main/docs/public/pics/drone.svg" alt="DSSE Icon" width="45" height="25"> Drone Swarm Search Environment (DSSE)
 
-Welcome to the official GitHub repository for the Drone Swarm Search Environment (DSSE). This project is dedicated to providing a comprehensive simulation environment designed to develop, test, and refine drone swarm search strategies. Here, researchers and developers can access a versatile platform that supports a wide range of drone swarm simulations, enabling the exploration of complex behaviors and interactions within dynamic, real-world scenarios.
+Welcome to the official GitHub repository for the Drone Swarm Search Environment (DSSE). This project offers a comprehensive simulation platform designed for developing, testing, and refining search strategies using drone swarms. Researchers and developers will find a versatile toolset supporting a broad spectrum of simulations, which facilitates the exploration of complex drone behaviors and interactions in dynamic, real-world scenarios.
+
+In this repository, we have implemented two distinct types of environments. The first is a dynamic environment that simulates maritime search and rescue operations for shipwreck survivors. It models the movement of individuals in the sea using a dynamic probability matrix, with the objective for drones being to locate and identify these individuals. The second is a environment utilizing the Lagrangian particle simulation from the open-source [Opendrift library](https://github.com/OpenDrift/opendrift), which incorporates real-world ocean and wind data to create a probability matrix for drone SAR tasks. In this scenario, drones are tasked with covering the full search area within the lowest time possible, while prioritizing higher probability areas.
 
 
 ## 📚 Documentation Links
 
 - **[Documentation Site](https://pfeinsper.github.io/drone-swarm-search/)**: Access comprehensive documentation including tutorials, and usage examples for the Drone Swarm Search Environment (DSSE). Ideal for users seeking detailed information about the project's capabilities and how to integrate them into their own applications.
 
 - **[Algorithm Details](https://github.com/pfeinsper/drone-swarm-search-algorithms)**: Explore in-depth discussions and source code for the algorithms powering the DSSE. This section is perfect for developers interested in the technical underpinnings and enhancements of the search algorithms.
 
 - **[PyPI Repository](https://pypi.org/project/DSSE/)**: Visit the PyPI page for DSSE to download the latest release, view release histories, and read additional installation instructions.
 
+# DSSE - Search Environment
+
 ## 🎥 Visual Demonstrations
 <p align="center">
-    <img src="https://raw.github.com/PFE-Embraer/drone-swarm-search/env-cleanup/docs/gifs/render_with_grid_gradient.gif" width="400" height="400" align="center">
+    <img src="docs/public/gifs/render_with_grid_gradient.gif" width="400" height="400" align="center">
     <br>
     <em>Above: A simulation showing how drones adjust their search pattern over a grid.</em>
 </p>
 
-## ⚡Quick Start
-
-### ⚙️ Installation
-Install DSSE quickly with pip:
-```bash
-pip install DSSE
-````
-
 ## 🎯 Outcome
 
 | If target is found       | If target is not found   |
 :-------------------------:|:-------------------------:
 | ![](https://raw.githubusercontent.com/PFE-Embraer/drone-swarm-search/main/docs/public/pics/victory_render.png)     | ![](https://raw.github.com/PFE-Embraer/drone-swarm-search/main/docs/public/pics/fail_render.png) |
 
+## ⚡ Quick Start
 
-## 🛠️ Basic Env Usage
+### ⚙️ Installation
+Quickly install DSSE using pip:
+```bash
+pip install DSSE
+````
+
+
+## 🛠️ Basic Env Search Usage
 ```python
 from DSSE import DroneSwarmSearch
 
 env = DroneSwarmSearch(
     grid_size=40,
     render_mode="human",
     render_grid=True,
@@ -107,35 +111,55 @@
         actions[agent] = env.action_space(agent).sample()
     return actions
 
 
 opt = {
     "drones_positions": [(10, 5), (10, 10)],
     "person_pod_multipliers": [0.1, 0.4, 0.5, 1.2],
+    "vector": (0.3, 0.3),
 }
 observations, info = env.reset(options=opt)
 
 rewards = 0
 done = False
 while not done:
     actions = random_policy(observations, env.get_agents())
     observations, rewards, terminations, truncations, infos = env.step(actions)
     done = any(terminations.values()) or any(truncations.values())
+
 ```
 
+
+# DSSE - Coverage Environment
+
+## 🎥 Visual Demonstrations
+<p align="center">
+    <img src="docs/public/gifs/basic_coverage.gif" width="400" height="400" align="center">
+    <br>
+    <em>Above: A simulation showing how drones adjust their search pattern over a grid.</em>
+</p>
+
+## ⚡ Quick Start
+
+### ⚙️ Installation
+Install DSSE with coverage support using pip:
+```bash
+pip install DSSE[coverage]
+````
+
+
 ## 🛠️ Basic Coverage Usage
 ```python
 from DSSE import CoverageDroneSwarmSearch
 
 env = CoverageDroneSwarmSearch(
-    grid_size=40,
     drone_amount=3,
-    dispersion_inc=0.1,
-    vector=(1, 1),
     render_mode="human",
+    disaster_position=(-24.04, -46.17),  # (lat, long)
+    pre_render_time=10, # hours to simulate
 )
 
 opt = {
     "drones_positions": [(0, 10), (10, 10), (20, 10)],
 }
 obs, info = env.reset(options=opt)
```

### Comparing `dsse-1.1.7/pyproject.toml` & `dsse-1.1.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -29,25 +29,25 @@
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
 ]
 dependencies = [
     "numpy>=1.23.1",
     "gymnasium>=0.27.1",
     "pygame>=2.3.0",
     "pettingzoo>=1.22.3",
-    "matplotlib>=3.7.0",
+    "matplotlib==3.8.4",
     "numba>=0.59.0",
 ]
 
 [project.optional-dependencies]
 all = [
     "numpy>=1.23.1",
     "gymnasium>=0.27.1",
     "pygame>=2.3.0",
     "pettingzoo>=1.22.3",
-    "matplotlib>=3.7.0",
+    "matplotlib==3.8.4",
     "numba>=0.59.0",
     "GDAL==3.4.1",
     "opendrift",
 ]
 coverage = [
     "GDAL==3.4.1",
     "opendrift",
```

