# Comparing `tmp/micro-manager-precice-0.3.0rc2.tar.gz` & `tmp/micro-manager-precice-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micro-manager-precice-0.3.0rc2.tar", last modified: Sat Aug 26 16:40:03 2023, max compression
+gzip compressed data, was "micro-manager-precice-0.4.0.tar", last modified: Thu Mar 21 16:13:00 2024, max compression
```

## Comparing `micro-manager-precice-0.3.0rc2.tar` & `micro-manager-precice-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 16:40:03.719540 micro-manager-precice-0.3.0rc2/
--rw-r--r--   0 runner    (1001) docker     (999)     7651 2023-08-26 16:39:53.000000 micro-manager-precice-0.3.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     1889 2023-08-26 16:40:03.719540 micro-manager-precice-0.3.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1490 2023-08-26 16:39:53.000000 micro-manager-precice-0.3.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 16:40:03.719540 micro-manager-precice-0.3.0rc2/micro_manager/
--rw-r--r--   0 runner    (1001) docker     (999)       67 2023-08-26 16:39:53.000000 micro-manager-precice-0.3.0rc2/micro_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 16:40:03.719540 micro-manager-precice-0.3.0rc2/micro_manager/adaptivity/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-26 16:39:53.000000 micro-manager-precice-0.3.0rc2/micro_manager/adaptivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    11347 2023-08-26 16:39:53.000000 micro-manager-precice-0.3.0rc2/micro_manager/adaptivity/adaptivity.py
--rw-r--r--   0 runner    (1001) docker     (999)    14274 2023-08-26 16:39:53.000000 micro-manager-precice-0.3.0rc2/micro_manager/adaptivity/global_adaptivity.py
--rw-r--r--   0 runner    (1001) docker     (999)     5075 2023-08-26 16:39:53.000000 micro-manager-precice-0.3.0rc2/micro_manager/adaptivity/local_adaptivity.py
--rw-r--r--   0 runner    (1001) docker     (999)    14256 2023-08-26 16:39:53.000000 micro-manager-precice-0.3.0rc2/micro_manager/config.py
--rw-r--r--   0 runner    (1001) docker     (999)     3603 2023-08-26 16:39:53.000000 micro-manager-precice-0.3.0rc2/micro_manager/domain_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (999)    25303 2023-08-26 16:39:53.000000 micro-manager-precice-0.3.0rc2/micro_manager/micro_manager.py
--rw-r--r--   0 runner    (1001) docker     (999)     1047 2023-08-26 16:39:53.000000 micro-manager-precice-0.3.0rc2/micro_manager/micro_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 16:40:03.719540 micro-manager-precice-0.3.0rc2/micro_manager_precice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     1889 2023-08-26 16:40:03.000000 micro-manager-precice-0.3.0rc2/micro_manager_precice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      662 2023-08-26 16:40:03.000000 micro-manager-precice-0.3.0rc2/micro_manager_precice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-26 16:40:03.000000 micro-manager-precice-0.3.0rc2/micro_manager_precice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       67 2023-08-26 16:40:03.000000 micro-manager-precice-0.3.0rc2/micro_manager_precice.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-26 16:40:03.000000 micro-manager-precice-0.3.0rc2/micro_manager_precice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (999)       40 2023-08-26 16:40:03.000000 micro-manager-precice-0.3.0rc2/micro_manager_precice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       14 2023-08-26 16:40:03.000000 micro-manager-precice-0.3.0rc2/micro_manager_precice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-26 16:40:03.719540 micro-manager-precice-0.3.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1221 2023-08-26 16:39:53.000000 micro-manager-precice-0.3.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:13:00.645823 micro-manager-precice-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-03-21 16:12:52.000000 micro-manager-precice-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-03-21 16:13:00.645823 micro-manager-precice-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-03-21 16:12:52.000000 micro-manager-precice-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:13:00.641823 micro-manager-precice-0.4.0/micro_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-21 16:12:52.000000 micro-manager-precice-0.4.0/micro_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:13:00.641823 micro-manager-precice-0.4.0/micro_manager/adaptivity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 16:12:52.000000 micro-manager-precice-0.4.0/micro_manager/adaptivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11695 2024-03-21 16:12:52.000000 micro-manager-precice-0.4.0/micro_manager/adaptivity/adaptivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15158 2024-03-21 16:12:52.000000 micro-manager-precice-0.4.0/micro_manager/adaptivity/global_adaptivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-03-21 16:12:52.000000 micro-manager-precice-0.4.0/micro_manager/adaptivity/local_adaptivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14536 2024-03-21 16:12:52.000000 micro-manager-precice-0.4.0/micro_manager/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-03-21 16:12:52.000000 micro-manager-precice-0.4.0/micro_manager/domain_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23681 2024-03-21 16:12:52.000000 micro-manager-precice-0.4.0/micro_manager/micro_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-21 16:12:52.000000 micro-manager-precice-0.4.0/micro_manager/micro_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:13:00.645823 micro-manager-precice-0.4.0/micro_manager_precice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-03-21 16:13:00.000000 micro-manager-precice-0.4.0/micro_manager_precice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-21 16:13:00.000000 micro-manager-precice-0.4.0/micro_manager_precice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 16:13:00.000000 micro-manager-precice-0.4.0/micro_manager_precice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-21 16:13:00.000000 micro-manager-precice-0.4.0/micro_manager_precice.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 16:13:00.000000 micro-manager-precice-0.4.0/micro_manager_precice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-21 16:13:00.000000 micro-manager-precice-0.4.0/micro_manager_precice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-21 16:13:00.000000 micro-manager-precice-0.4.0/micro_manager_precice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 16:13:00.645823 micro-manager-precice-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-21 16:12:52.000000 micro-manager-precice-0.4.0/setup.py
```

### Comparing `micro-manager-precice-0.3.0rc2/LICENSE` & `micro-manager-precice-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `micro-manager-precice-0.3.0rc2/PKG-INFO` & `micro-manager-precice-0.4.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: micro-manager-precice
-Version: 0.3.0rc2
+Version: 0.4.0
 Summary: micro-manager-precice is a package which facilitates two-scale macro-micro coupled simulations using preCICE
 Home-page: https://precice.org/tooling-micro-manager-overview.html
 Author: Ishaan Desai
 Author-email: ishaan.desai@uni-stuttgart.de
 License: LGPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyprecice>=3.0.0.0
+Requires-Dist: numpy>=1.13.3
+Requires-Dist: mpi4py
 
 # Micro Manager
 
 <a style="text-decoration: none" href="https://github.com/precice/micro-manager/blob/develop/LICENSE" target="_blank">
     <img src="https://img.shields.io/github/license/precice/micro-manager.svg" alt="GNU LGPL license">
 </a>
 
@@ -19,14 +22,14 @@
     <img src="https://github.com/precice/micro-manager/actions/workflows/run-adaptivity-test.yml/badge.svg" alt="Test Adaptivity">
 </a>
 
 <a style="text-decoration: none" href="https://pypi.org/project/micro-manager-precice/" target="_blank">
     <img src="https://github.com/precice/micro-manager/actions/workflows/pythonpublish.yml/badge.svg" alt="Upload Python Package">
 </a>
 
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05842/status.svg)](https://doi.org/10.21105/joss.05842)
+
 A tool to facilitate solving two-scale (macro-micro) coupled problems using the coupling library [preCICE](https://www.precice.org/).
 
 The main documentation is rendered on the [preCICE website](https://precice.org/tooling-micro-manager-overview.html).
 
 Please report any [issues](https://github.com/precice/micro-manager/issues) and give us feedback through [one of our community channels](https://precice.org/community-channels.html).
-
-The concept and initial design of the Micro Manager is described in *Desai, Ishaan, & Bringedal, Carina & Uekermann, Benjamin. A flexible software approach to simulate two-scale coupled problems. ECCOMAS Congress 2022. [10.23967/eccomas.2022.037](https://doi.org/10.23967/eccomas.2022.037)*.
```

### Comparing `micro-manager-precice-0.3.0rc2/README.md` & `micro-manager-precice-0.4.0/micro_manager_precice.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,35 @@
+Metadata-Version: 2.1
+Name: micro-manager-precice
+Version: 0.4.0
+Summary: micro-manager-precice is a package which facilitates two-scale macro-micro coupled simulations using preCICE
+Home-page: https://precice.org/tooling-micro-manager-overview.html
+Author: Ishaan Desai
+Author-email: ishaan.desai@uni-stuttgart.de
+License: LGPL-3.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pyprecice>=3.0.0.0
+Requires-Dist: numpy>=1.13.3
+Requires-Dist: mpi4py
+
 # Micro Manager
 
 <a style="text-decoration: none" href="https://github.com/precice/micro-manager/blob/develop/LICENSE" target="_blank">
     <img src="https://img.shields.io/github/license/precice/micro-manager.svg" alt="GNU LGPL license">
 </a>
 
 <a style="text-decoration: none" href="https://github.com/precice/fenics-adapter/actions/workflows/build-and-test.yml" target="_blank">
     <img src="https://github.com/precice/micro-manager/actions/workflows/run-adaptivity-test.yml/badge.svg" alt="Test Adaptivity">
 </a>
 
 <a style="text-decoration: none" href="https://pypi.org/project/micro-manager-precice/" target="_blank">
     <img src="https://github.com/precice/micro-manager/actions/workflows/pythonpublish.yml/badge.svg" alt="Upload Python Package">
 </a>
 
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05842/status.svg)](https://doi.org/10.21105/joss.05842)
+
 A tool to facilitate solving two-scale (macro-micro) coupled problems using the coupling library [preCICE](https://www.precice.org/).
 
 The main documentation is rendered on the [preCICE website](https://precice.org/tooling-micro-manager-overview.html).
 
 Please report any [issues](https://github.com/precice/micro-manager/issues) and give us feedback through [one of our community channels](https://precice.org/community-channels.html).
-
-The concept and initial design of the Micro Manager is described in *Desai, Ishaan, & Bringedal, Carina & Uekermann, Benjamin. A flexible software approach to simulate two-scale coupled problems. ECCOMAS Congress 2022. [10.23967/eccomas.2022.037](https://doi.org/10.23967/eccomas.2022.037)*.
```

### Comparing `micro-manager-precice-0.3.0rc2/micro_manager/adaptivity/adaptivity.py` & `micro-manager-precice-0.4.0/micro_manager/adaptivity/adaptivity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Functionality for adaptive initialization and control of micro simulations
 """
 import sys
 import numpy as np
 from math import exp
 from typing import Callable
+from warnings import warn
 
 
 class AdaptivityCalculator:
     def __init__(self, configurator, logger) -> None:
         """
         Class constructor.
 
@@ -48,15 +49,15 @@
         -------
         similarity_dists : numpy array
             Updated 2D array having similarity distances between each micro simulation pair
         """
         _similarity_dists = np.copy(similarity_dists)
 
         data_diff = np.zeros_like(_similarity_dists)
-        for name in self._adaptivity_data_names:
+        for name in data.keys():
             data_vals = data[name]
             if data_vals.ndim == 1:
                 # If the adaptivity-data is a scalar for each simulation,
                 # expand the dimension to make it a 2D array to unify the calculation.
                 # The axis is later reduced with a norm.
                 data_vals = np.expand_dims(data_vals, axis=1)
 
@@ -80,15 +81,21 @@
             1D array having state (active or inactive) of each micro simulation
 
         Returns
         -------
         _is_sim_active : numpy array
             Updated 1D array having state (active or inactive) of each micro simulation
         """
-        self._coarse_tol = self._coarse_const * self._refine_const * np.amax(similarity_dists)
+        max_similarity_dist = np.amax(similarity_dists)
+
+        if max_similarity_dist == 0.0:
+            warn("All similarity distances are zero, probably because all the data for adaptivity is the same. Coarsening tolerance will be manually set to minimum float number.")
+            self._coarse_tol = sys.float_info.min
+        else:
+            self._coarse_tol = self._coarse_const * self._refine_const * max_similarity_dist
 
         _is_sim_active = np.copy(is_sim_active)  # Input is_sim_active is not longer used after this point
 
         # Update the set of active micro sims
         for i in range(_is_sim_active.size):
             if _is_sim_active[i]:  # if sim is active
                 if self._check_for_deactivation(i, similarity_dists, _is_sim_active):
```

### Comparing `micro-manager-precice-0.3.0rc2/micro_manager/adaptivity/global_adaptivity.py` & `micro-manager-precice-0.4.0/micro_manager/adaptivity/global_adaptivity.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,46 +14,57 @@
 
 
 class GlobalAdaptivityCalculator(AdaptivityCalculator):
     def __init__(
             self,
             configurator,
             logger,
-            is_sim_on_this_rank: list,
-            rank_of_sim: np.ndarray,
+            global_number_of_sims: float,
             global_ids: list,
             rank: int,
             comm) -> None:
         """
         Class constructor.
 
         Parameters
         ----------
         configurator : object of class Config
             Object which has getter functions to get parameters defined in the configuration file.
         logger : object of logging
             Logger defined from the standard package logging
-        is_sim_on_this_rank : list
+        global_number_of_sims : float
             List of booleans. True if simulation is on this rank, False otherwise.
-        rank_of_sim : numpy array
-            1D array consisting of rank on which the simulation lives.
         global_ids : list
             List of global IDs of simulations living on this rank.
         rank : int
             MPI rank.
         comm : MPI.COMM_WORLD
             Global communicator of MPI.
         """
         super().__init__(configurator, logger)
-        self._is_sim_on_this_rank = is_sim_on_this_rank
-        self._rank_of_sim = rank_of_sim
         self._global_ids = global_ids
         self._comm = comm
         self._rank = rank
 
+        local_number_of_sims = len(global_ids)
+
+        # Create a map of micro simulation global IDs and the ranks on which they are
+        micro_sims_on_this_rank = np.zeros(local_number_of_sims, dtype=np.intc)
+        for i in range(local_number_of_sims):
+            micro_sims_on_this_rank[i] = self._rank
+
+        self._rank_of_sim = np.zeros(global_number_of_sims, dtype=np.intc)  # DECLARATION
+
+        self._comm.Allgatherv(micro_sims_on_this_rank, self._rank_of_sim)
+
+        self._is_sim_on_this_rank = [False] * global_number_of_sims  # DECLARATION
+        for i in range(global_number_of_sims):
+            if self._rank_of_sim[i] == self._rank:
+                self._is_sim_on_this_rank[i] = True
+
     def compute_adaptivity(
             self,
             dt: float,
             micro_sims: list,
             similarity_dists_nm1: np.ndarray,
             is_sim_active_nm1: np.ndarray,
             sim_is_associated_to_nm1: np.ndarray,
@@ -79,27 +90,32 @@
         Results
         -------
         similarity_dists : numpy array
             2D array having similarity distances between each micro simulation pair
         is_sim_active : numpy array
             1D array having state (active or inactive) of each micro simulation
         """
+        for name in data_for_adaptivity.keys():
+            if name not in self._adaptivity_data_names:
+                raise ValueError(
+                    "Data for adaptivity must be one of the following: {}".format(
+                        self._adaptivity_data_names.keys()))
+
         # Gather adaptivity data from all ranks
         global_data_for_adaptivity = dict()
-        for name in self._adaptivity_data_names.keys():
+        for name in data_for_adaptivity.keys():
             data_as_list = self._comm.allgather(data_for_adaptivity[name])
             global_data_for_adaptivity[name] = np.concatenate((data_as_list[:]), axis=0)
 
         similarity_dists = self._get_similarity_dists(dt, similarity_dists_nm1, global_data_for_adaptivity)
 
         is_sim_active = self._update_active_sims(similarity_dists, is_sim_active_nm1)
 
         is_sim_active, sim_is_associated_to = self._update_inactive_sims(
-            similarity_dists, is_sim_active_nm1, sim_is_associated_to_nm1, micro_sims)
-
+            similarity_dists, is_sim_active, sim_is_associated_to_nm1, micro_sims)
         sim_is_associated_to = self._associate_inactive_to_active(
             similarity_dists, is_sim_active, sim_is_associated_to)
 
         self._logger.info(
             "{} active simulations, {} inactive simulations".format(
                 np.count_nonzero(
                     is_sim_active[self._global_ids[0]:self._global_ids[-1] + 1]),
@@ -308,14 +324,15 @@
                 req = self._comm.isend(data[local_id], dest=send_rank, tag=tag)
                 send_reqs.append(req)
 
         # Asynchronous receive operations
         recv_reqs = []
         for global_id, recv_rank in recv_map.items():
             tag = self._create_tag(global_id, recv_rank, self._rank)
-            req = self._comm.irecv(source=recv_rank, tag=tag)
+            bufsize = 1 << 30  # allocate and use a temporary 1 MiB buffer size https://github.com/mpi4py/mpi4py/issues/389
+            req = self._comm.irecv(bufsize, source=recv_rank, tag=tag)
             recv_reqs.append(req)
 
         # Wait for all non-blocking communication to complete
         MPI.Request.Waitall(send_reqs)
 
         return recv_reqs
```

### Comparing `micro-manager-precice-0.3.0rc2/micro_manager/adaptivity/local_adaptivity.py` & `micro-manager-precice-0.4.0/micro_manager/adaptivity/local_adaptivity.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def compute_adaptivity(
             self,
             dt,
             micro_sims,
             similarity_dists_nm1: np.ndarray,
             is_sim_active_nm1: np.ndarray,
             sim_is_associated_to_nm1: np.ndarray,
-            data_for_adaptivity: dict):
+            data_for_adaptivity: dict) -> tuple:
         """
         Compute adaptivity locally (within a rank).
 
         Parameters
         ----------
         dt : float
             Current time step
@@ -51,21 +51,27 @@
         Returns
         -------
         similarity_dists : numpy array
             2D array having similarity distances between each micro simulation pair.
         is_sim_active : numpy array
             1D array, True is sim is active, False if sim is inactive.
         """
+        for name in data_for_adaptivity.keys():
+            if name not in self._adaptivity_data_names:
+                raise ValueError(
+                    "Data for adaptivity must be one of the following: {}".format(
+                        self._adaptivity_data_names.keys()))
+
         similarity_dists = self._get_similarity_dists(dt, similarity_dists_nm1, data_for_adaptivity)
 
         # Operation done globally if global adaptivity is chosen
         is_sim_active = self._update_active_sims(similarity_dists, is_sim_active_nm1)
 
         is_sim_active, sim_is_associated_to = self._update_inactive_sims(
-            similarity_dists, is_sim_active_nm1, sim_is_associated_to_nm1, micro_sims)
+            similarity_dists, is_sim_active, sim_is_associated_to_nm1, micro_sims)
 
         sim_is_associated_to = self._associate_inactive_to_active(
             similarity_dists, is_sim_active, sim_is_associated_to)
 
         self._logger.info(
             "{} active simulations, {} inactive simulations".format(
                 np.count_nonzero(is_sim_active), np.count_nonzero(is_sim_active == False)))
```

### Comparing `micro-manager-precice-0.3.0rc2/micro_manager/config.py` & `micro-manager-precice-0.4.0/micro_manager/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Class Config provides functionality to read a JSON file and pass the values to the Micro Manager.
 """
 
 import json
 import os
+from warnings import warn
 
 
 class Config:
     """
     Handles the reading of parameters in the JSON configuration file provided by the user. This class is based on
     the config class in https://github.com/precice/fenics-adapter/tree/develop/fenicsadapter
     """
@@ -112,23 +113,27 @@
                 "Micro Manager will not adaptively run micro simulations, but instead will run all micro simulations in all time steps.")
 
         if self._adaptivity:
             if data["simulation_params"]["adaptivity"]["type"] == "local":
                 self._adaptivity_type = "local"
             elif data["simulation_params"]["adaptivity"]["type"] == "global":
                 self._adaptivity_type = "global"
-                self._logger.warning(
-                    "Global adaptivity is still experimental. We recommend using it for small (<50 macro vertices) cases only.")
             else:
                 raise Exception("Adaptivity type can be either local or global.")
 
             exchange_data = {**self._read_data_names, **self._write_data_names}
             for dname in data["simulation_params"]["adaptivity"]["data"]:
                 self._data_for_adaptivity[dname] = exchange_data[dname]
 
+            if self._data_for_adaptivity.keys() == self._write_data_names.keys():
+                warn(
+                    "Only micro simulation data is used for similarity computation in adaptivity. This would lead to the"
+                    " same set of active and inactive simulations for the entire simulation time. If this is not intended,"
+                    " please include macro simulation data as well.")
+
             self._adaptivity_history_param = data["simulation_params"]["adaptivity"]["history_param"]
             self._adaptivity_coarsening_constant = data["simulation_params"]["adaptivity"]["coarsening_constant"]
             self._adaptivity_refining_constant = data["simulation_params"]["adaptivity"]["refining_constant"]
 
             if "similarity_measure" in data["simulation_params"]["adaptivity"]:
                 self._adaptivity_similarity_measure = data["simulation_params"]["adaptivity"]["similarity_measure"]
             else:
```

### Comparing `micro-manager-precice-0.3.0rc2/micro_manager/domain_decomposition.py` & `micro-manager-precice-0.4.0/micro_manager/domain_decomposition.py`

 * *Files identical despite different names*

### Comparing `micro-manager-precice-0.3.0rc2/micro_manager/micro_manager.py` & `micro-manager-precice-0.4.0/micro_manager/micro_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 """
 Micro Manager is a tool to initialize and adaptively control micro simulations and couple them via preCICE to a macro simulation.
 This files the class MicroManager which has the following callable public methods:
 
-- initialize
 - solve
 
 This file is directly executable as it consists of a main() function. Upon execution, an object of the class MicroManager is created using a given JSON file,
 and the initialize and solve methods are called.
 
 Detailed documentation: https://precice.org/tooling-micro-manager-overview.html
 """
@@ -18,14 +17,15 @@
 import precice
 from mpi4py import MPI
 import numpy as np
 import logging
 import time
 from copy import deepcopy
 from typing import Dict
+from warnings import warn
 
 from .config import Config
 from .micro_simulation import create_simulation_class
 from .adaptivity.local_adaptivity import LocalAdaptivityCalculator
 from .adaptivity.global_adaptivity import GlobalAdaptivityCalculator
 from .domain_decomposition import DomainDecomposer
 
@@ -60,34 +60,30 @@
 
         self._is_parallel = self._size > 1
         self._micro_sims_have_output = False
 
         self._logger.info("Provided configuration file: {}".format(config_file))
         self._config = Config(self._logger, config_file)
 
-        # Define the preCICE interface
-        self._interface = precice.Interface(
+        # Define the preCICE Participant
+        self._participant = precice.Participant(
             "Micro-Manager",
             self._config.get_config_file_name(),
             self._rank,
             self._size)
 
-        self._macro_mesh_id = self._interface.get_mesh_id(self._config.get_macro_mesh_name())
+        micro_file_name = self._config.get_micro_file_name()
 
-        # Data names and ids of data written to preCICE
+        self._macro_mesh_name = self._config.get_macro_mesh_name()
+
+        # Data names of data written to preCICE
         self._write_data_names = self._config.get_write_data_names()
-        self._write_data_ids = dict()
-        for name in self._write_data_names.keys():
-            self._write_data_ids[name] = self._interface.get_data_id(name, self._macro_mesh_id)
 
-        # Data names and ids of data read from preCICE
+        # Data names of data read from preCICE
         self._read_data_names = self._config.get_read_data_names()
-        self._read_data_ids = dict()
-        for name in self._read_data_names.keys():
-            self._read_data_ids[name] = self._interface.get_data_id(name, self._macro_mesh_id)
 
         self._macro_bounds = self._config.get_macro_domain_bounds()
 
         if self._is_parallel:  # Simulation is run in parallel
             self._ranks_per_axis = self._config.get_ranks_per_axis()
 
         self._is_micro_solve_time_required = self._config.write_micro_solve_time()
@@ -115,202 +111,64 @@
             self._adaptivity_micro_data_names = dict()
             for name, is_data_vector in self._adaptivity_data_names.items():
                 if name in self._read_data_names:
                     self._adaptivity_macro_data_names[name] = is_data_vector
                 if name in self._write_data_names:
                     self._adaptivity_micro_data_names[name] = is_data_vector
 
-            self._is_adaptivity_required_in_every_implicit_iteration = self._config.is_adaptivity_required_in_every_implicit_iteration()
+            self._adaptivity_in_every_implicit_step = self._config.is_adaptivity_required_in_every_implicit_iteration()
             self._micro_sims_active_steps = None
 
+        self._initialize()
+
     # **************
     # Public methods
     # **************
 
-    def initialize(self) -> None:
-        """
-        Initialize the Micro Manager by performing the following tasks:
-        - Decompose the domain if the Micro Manager is executed in parallel.
-        - Initialize preCICE.
-        - Gets the macro mesh information from preCICE.
-        - Create all micro simulation objects and initialize them if an initialize() method is available.
-        - If required, write initial data to preCICE.
-        """
-        # Decompose the macro-domain and set the mesh access region for each partition in preCICE
-        assert len(self._macro_bounds) / \
-            2 == self._interface.get_dimensions(), "Provided macro mesh bounds are of incorrect dimension"
-        if self._is_parallel:
-            domain_decomposer = DomainDecomposer(self._logger, self._interface.get_dimensions(), self._rank, self._size)
-            coupling_mesh_bounds = domain_decomposer.decompose_macro_domain(self._macro_bounds, self._ranks_per_axis)
-        else:
-            coupling_mesh_bounds = self._macro_bounds
-
-        self._interface.set_mesh_access_region(self._macro_mesh_id, coupling_mesh_bounds)
-
-        # Initialize preCICE
-        self._dt = self._interface.initialize()
-
-        self._mesh_vertex_ids, mesh_vertex_coords = self._interface.get_mesh_vertices_and_ids(self._macro_mesh_id)
-        self._local_number_of_sims, _ = mesh_vertex_coords.shape
-        self._logger.info("Number of local micro simulations = {}".format(self._local_number_of_sims))
-
-        if self._local_number_of_sims == 0:
-            if self._is_parallel:
-                self._logger.info(
-                    "Rank {} has no micro simulations and hence will not do any computation.".format(
-                        self._rank))
-                self._is_rank_empty = True
-            else:
-                raise Exception("Micro Manager has no micro simulations.")
-
-        nms_all_ranks = np.zeros(self._size, dtype=np.int64)
-        # Gather number of micro simulations that each rank has, because this rank needs to know how many micro
-        # simulations have been created by previous ranks, so that it can set
-        # the correct global IDs
-        self._comm.Allgather(np.array(self._local_number_of_sims), nms_all_ranks)
-
-        # Get global number of micro simulations
-        self._global_number_of_sims = np.sum(nms_all_ranks)
-
-        if self._is_adaptivity_on:
-            for name, is_data_vector in self._adaptivity_data_names.items():
-                if is_data_vector:
-                    self._data_for_adaptivity[name] = np.zeros(
-                        (self._local_number_of_sims, self._interface.get_dimensions()))
-                else:
-                    self._data_for_adaptivity[name] = np.zeros((self._local_number_of_sims))
-
-        # Create lists of local and global IDs
-        sim_id = np.sum(nms_all_ranks[:self._rank])
-        self._global_ids_of_local_sims = []  # DECLARATION
-        for i in range(self._local_number_of_sims):
-            self._global_ids_of_local_sims.append(sim_id)
-            sim_id += 1
-
-        self._micro_sims = [None] * self._local_number_of_sims  # DECLARATION
-        micro_sims_output = [None] * self._local_number_of_sims
-
-        micro_problem = getattr(
-            __import__(
-                self._config.get_micro_file_name(),
-                fromlist=["MicroSimulation"]),
-            "MicroSimulation")
-
-        if self._is_adaptivity_on:
-            # Create micro simulation objects
-            for i in range(self._local_number_of_sims):
-                self._micro_sims[i] = create_simulation_class(
-                    micro_problem)(self._global_ids_of_local_sims[i])
-
-            # Create a map of micro simulation global IDs and the ranks on which they are
-            micro_sims_on_this_rank = np.zeros(self._local_number_of_sims, dtype=np.intc)
-            for i in range(self._local_number_of_sims):
-                micro_sims_on_this_rank[i] = self._rank
-
-            self._rank_of_sim = np.zeros(self._global_number_of_sims, dtype=np.intc)  # DECLARATION
-            self._comm.Allgather(micro_sims_on_this_rank, self._rank_of_sim)
-
-            self._is_sim_on_this_rank = [False] * self._global_number_of_sims  # DECLARATION
-            for i in range(self._global_number_of_sims):
-                if self._rank_of_sim[i] == self._rank:
-                    self._is_sim_on_this_rank[i] = True
-
-            if self._adaptivity_type == "local":
-                self._adaptivity_controller = LocalAdaptivityCalculator(
-                    self._config, self._logger)
-                self._number_of_sims_for_adaptivity = self._local_number_of_sims
-            elif self._adaptivity_type == "global":
-                self._adaptivity_controller = GlobalAdaptivityCalculator(
-                    self._config,
-                    self._logger,
-                    self._is_sim_on_this_rank,
-                    self._rank_of_sim,
-                    self._global_ids_of_local_sims,
-                    self._rank,
-                    self._comm)
-                self._number_of_sims_for_adaptivity = self._global_number_of_sims
-
-            self._micro_sims_active_steps = np.zeros(self._local_number_of_sims)
-        else:
-            for i in range(self._local_number_of_sims):
-                self._micro_sims[i] = (
-                    create_simulation_class(micro_problem)(self._global_ids_of_local_sims[i]))
-
-        # Initialize micro simulations if initialize() method exists
-        if hasattr(micro_problem, 'initialize') and callable(getattr(micro_problem, 'initialize')):
-            for i in range(self._local_number_of_sims):
-                micro_sims_output[i] = self._micro_sims[i].initialize()
-                if micro_sims_output[i] is not None:
-                    if self._is_micro_solve_time_required:
-                        micro_sims_output[i]["micro_sim_time"] = 0.0
-                    if self._is_adaptivity_on:
-                        micro_sims_output[i]["active_state"] = 0
-                        micro_sims_output[i]["active_steps"] = 0
-                else:
-                    micro_sims_output[i] = dict()
-                    for name, is_data_vector in self._write_data_names.items():
-                        if is_data_vector:
-                            micro_sims_output[i][name] = np.zeros(self._interface.get_dimensions())
-                        else:
-                            micro_sims_output[i][name] = 0.0
-
-        self._logger.info("Micro simulations with global IDs {} - {} initialized.".format(
-            self._global_ids_of_local_sims[0], self._global_ids_of_local_sims[-1]))
-
-        self._micro_sims_have_output = False
-        if hasattr(micro_problem, 'output') and callable(getattr(micro_problem, 'output')):
-            self._micro_sims_have_output = True
-
-        # Write initial data if required
-        if self._interface.is_action_required(precice.action_write_initial_data()):
-            self._write_data_to_precice(micro_sims_output)
-            self._interface.mark_action_fulfilled(precice.action_write_initial_data())
-
-        self._interface.initialize_data()
-
     def solve(self) -> None:
         """
         Solve the problem using preCICE.
         - Handle checkpointing is implicit coupling is done.
         - Read data from preCICE, solve micro simulations, and write data to preCICE
         - If adaptivity is on, compute micro simulations adaptively.
         """
         t, n = 0, 0
         t_checkpoint, n_checkpoint = 0, 0
+        similarity_dists_cp = None
+        is_sim_active_cp = None
+        sim_is_associated_to_cp = None
+        sim_states_cp = [None] * self._local_number_of_sims
 
         if self._is_adaptivity_on:
             similarity_dists = np.zeros(
                 (self._number_of_sims_for_adaptivity,
                  self._number_of_sims_for_adaptivity))
 
-            # Start adaptivity calculation with all sims inactive
-            is_sim_active = np.array([False] * self._number_of_sims_for_adaptivity)
-
-            # Activate the first one (a random choice)
-            is_sim_active[0] = True
+            # Start adaptivity calculation with all sims active
+            is_sim_active = np.array([True] * self._number_of_sims_for_adaptivity)
 
-            # Associate all sims to the one active sim
-            sim_is_associated_to = np.zeros((self._number_of_sims_for_adaptivity), dtype=np.intc)
-            sim_is_associated_to[0] = -2  # An active sim does not have an associated sim
+            # Active sims do not have an associated sim
+            sim_is_associated_to = np.full((self._number_of_sims_for_adaptivity), -2, dtype=np.intc)
 
-        similarity_dists_cp = None
-        is_sim_active_cp = None
-        sim_is_associated_to_cp = None
-        sim_states_cp = [None] * self._local_number_of_sims
+            # If micro simulations have been initialized, compute adaptivity based on initial data
+            if self._micro_sims_init:
+                # Compute adaptivity based on initial data of micro sims
+                similarity_dists, is_sim_active, sim_is_associated_to = self._adaptivity_controller.compute_adaptivity(
+                    self._dt, self._micro_sims, similarity_dists, is_sim_active, sim_is_associated_to, self._data_for_adaptivity)
 
-        while self._interface.is_coupling_ongoing():
+        while self._participant.is_coupling_ongoing():
             # Write a checkpoint
-            if self._interface.is_action_required(precice.action_write_iteration_checkpoint()):
+            if self._participant.requires_writing_checkpoint():
                 for i in range(self._local_number_of_sims):
                     sim_states_cp[i] = self._micro_sims[i].get_state()
                 t_checkpoint = t
                 n_checkpoint = n
 
                 if self._is_adaptivity_on:
-                    if not self._is_adaptivity_required_in_every_implicit_iteration:
+                    if not self._adaptivity_in_every_implicit_step:
                         similarity_dists, is_sim_active, sim_is_associated_to = self._adaptivity_controller.compute_adaptivity(
                             self._dt, self._micro_sims, similarity_dists, is_sim_active, sim_is_associated_to, self._data_for_adaptivity)
 
                         # Only checkpoint the adaptivity configuration if adaptivity is computed
                         # once in every time window
                         similarity_dists_cp = np.copy(similarity_dists)
                         is_sim_active_cp = np.copy(is_sim_active)
@@ -321,21 +179,18 @@
                     elif self._adaptivity_type == "global":
                         active_sim_ids = np.where(
                             is_sim_active[self._global_ids_of_local_sims[0]:self._global_ids_of_local_sims[-1] + 1])[0]
 
                     for active_id in active_sim_ids:
                         self._micro_sims_active_steps[active_id] += 1
 
-                self._interface.mark_action_fulfilled(
-                    precice.action_write_iteration_checkpoint())
-
             micro_sims_input = self._read_data_from_precice()
 
             if self._is_adaptivity_on:
-                if self._is_adaptivity_required_in_every_implicit_iteration:
+                if self._adaptivity_in_every_implicit_step:
                     similarity_dists, is_sim_active, sim_is_associated_to = self._adaptivity_controller.compute_adaptivity(
                         self._dt, self._micro_sims, similarity_dists, is_sim_active, sim_is_associated_to, self._data_for_adaptivity)
 
                     if self._adaptivity_type == "local":
                         active_sim_ids = np.where(is_sim_active)[0]
                     elif self._adaptivity_type == "global":
                         active_sim_ids = np.where(
@@ -347,70 +202,194 @@
                 micro_sims_output = self._solve_micro_simulations_with_adaptivity(
                     micro_sims_input, is_sim_active, sim_is_associated_to)
             else:
                 micro_sims_output = self._solve_micro_simulations(micro_sims_input)
 
             self._write_data_to_precice(micro_sims_output)
 
-            self._dt = self._interface.advance(self._dt)
+            self._participant.advance(self._dt)
+            self._dt = self._participant.get_max_time_step_size()
 
             t += self._dt
             n += 1
 
             # Revert micro simulations to their last checkpoints if required
-            if self._interface.is_action_required(precice.action_read_iteration_checkpoint()):
+            if self._participant.requires_reading_checkpoint():
                 for i in range(self._local_number_of_sims):
                     self._micro_sims[i].set_state(sim_states_cp[i])
                 n = n_checkpoint
                 t = t_checkpoint
 
                 # If adaptivity is computed only once per time window, the states of sims need to be reset too
                 if self._is_adaptivity_on:
-                    if not self._is_adaptivity_required_in_every_implicit_iteration:
+                    if not self._adaptivity_in_every_implicit_step:
                         similarity_dists = np.copy(similarity_dists_cp)
                         is_sim_active = np.copy(is_sim_active_cp)
                         sim_is_associated_to = np.copy(sim_is_associated_to_cp)
 
-                self._interface.mark_action_fulfilled(
-                    precice.action_read_iteration_checkpoint())
             else:  # Time window has converged, now micro output can be generated
                 self._logger.info("Micro simulations {} - {} have converged at t = {}".format(
                     self._micro_sims[0].get_global_id(), self._micro_sims[-1].get_global_id(), t))
 
                 if self._micro_sims_have_output:
                     if n % self._micro_n_out == 0:
                         for sim in self._micro_sims:
                             sim.output()
 
-        self._interface.finalize()
+        self._participant.finalize()
 
     # ***************
     # Private methods
     # ***************
 
+    def _initialize(self) -> None:
+        """
+        Initialize the Micro Manager by performing the following tasks:
+        - Decompose the domain if the Micro Manager is executed in parallel.
+        - Initialize preCICE.
+        - Gets the macro mesh information from preCICE.
+        - Create all micro simulation objects and initialize them if an initialize() method is available.
+        - If required, write initial data to preCICE.
+        """
+        # Decompose the macro-domain and set the mesh access region for each partition in preCICE
+        assert len(self._macro_bounds) / 2 == self._participant.get_mesh_dimensions(
+            self._macro_mesh_name), "Provided macro mesh bounds are of incorrect dimension"
+        if self._is_parallel:
+            domain_decomposer = DomainDecomposer(
+                self._logger, self._participant.get_mesh_dimensions(self._macro_mesh_name), self._rank, self._size)
+            coupling_mesh_bounds = domain_decomposer.decompose_macro_domain(self._macro_bounds, self._ranks_per_axis)
+        else:
+            coupling_mesh_bounds = self._macro_bounds
+
+        self._participant.set_mesh_access_region(self._macro_mesh_name, coupling_mesh_bounds)
+
+        # initialize preCICE
+        self._participant.initialize()
+
+        self._mesh_vertex_ids, mesh_vertex_coords = self._participant.get_mesh_vertex_ids_and_coordinates(
+            self._macro_mesh_name)
+        assert (mesh_vertex_coords.size != 0), "Macro mesh has no vertices."
+
+        self._local_number_of_sims, _ = mesh_vertex_coords.shape
+        self._logger.info("Number of local micro simulations = {}".format(self._local_number_of_sims))
+
+        if self._local_number_of_sims == 0:
+            if self._is_parallel:
+                self._logger.info(
+                    "Rank {} has no micro simulations and hence will not do any computation.".format(
+                        self._rank))
+                self._is_rank_empty = True
+            else:
+                raise Exception("Micro Manager has no micro simulations.")
+
+        nms_all_ranks = np.zeros(self._size, dtype=np.int64)
+        # Gather number of micro simulations that each rank has, because this rank needs to know how many micro
+        # simulations have been created by previous ranks, so that it can set
+        # the correct global IDs
+        self._comm.Allgatherv(np.array(self._local_number_of_sims), nms_all_ranks)
+
+        # Get global number of micro simulations
+        self._global_number_of_sims = np.sum(nms_all_ranks)
+
+        if self._is_adaptivity_on:
+            for name, is_data_vector in self._adaptivity_data_names.items():
+                if is_data_vector:
+                    self._data_for_adaptivity[name] = np.zeros(
+                        (self._local_number_of_sims, self._participant.get_data_dimensions(
+                            self._macro_mesh_name, name)))
+                else:
+                    self._data_for_adaptivity[name] = np.zeros((self._local_number_of_sims))
+
+        # Create lists of local and global IDs
+        sim_id = np.sum(nms_all_ranks[:self._rank])
+        self._global_ids_of_local_sims = []  # DECLARATION
+        for i in range(self._local_number_of_sims):
+            self._global_ids_of_local_sims.append(sim_id)
+            sim_id += 1
+
+        self._micro_sims = [None] * self._local_number_of_sims  # DECLARATION
+
+        micro_problem = getattr(
+            __import__(
+                self._config.get_micro_file_name(),
+                fromlist=["MicroSimulation"]),
+            "MicroSimulation")
+
+        # Create micro simulation objects
+        for i in range(self._local_number_of_sims):
+            self._micro_sims[i] = create_simulation_class(
+                micro_problem)(self._global_ids_of_local_sims[i])
+
+        self._logger.info("Micro simulations with global IDs {} - {} created.".format(
+            self._global_ids_of_local_sims[0], self._global_ids_of_local_sims[-1]))
+
+        if self._is_adaptivity_on:
+            if self._adaptivity_type == "local":
+                self._adaptivity_controller = LocalAdaptivityCalculator(
+                    self._config, self._logger)
+                self._number_of_sims_for_adaptivity = self._local_number_of_sims
+            elif self._adaptivity_type == "global":
+                self._adaptivity_controller = GlobalAdaptivityCalculator(
+                    self._config,
+                    self._logger,
+                    self._global_number_of_sims,
+                    self._global_ids_of_local_sims,
+                    self._rank,
+                    self._comm)
+                self._number_of_sims_for_adaptivity = self._global_number_of_sims
+
+            self._micro_sims_active_steps = np.zeros(self._local_number_of_sims)
+
+        self._micro_sims_init = False  # DECLARATION
+
+        # Get initial data from micro simulations if initialize() method exists
+        if hasattr(micro_problem, 'initialize') and callable(getattr(micro_problem, 'initialize')):
+            if self._is_adaptivity_on:
+                self._micro_sims_init = True
+                initial_micro_output = self._micro_sims[0].initialize()  # Call initialize() of the first simulation
+                if initial_micro_output is None:  # Check if the detected initialize() method returns any data
+                    warn("The initialize() call of the Micro simulation has not returned any initial data."
+                         " The initialize call is stopped.")
+                    self._micro_sims_init = False
+                else:
+                    # Save initial data from first micro simulation as we anyway have it
+                    for name in initial_micro_output.keys():
+                        self._data_for_adaptivity[name][0] = initial_micro_output[name]
+
+                    # Gather initial data from the rest of the micro simulations
+                    for i in range(1, self._local_number_of_sims):
+                        initial_micro_output = self._micro_sims[i].initialize()
+                        for name in self._adaptivity_micro_data_names:
+                            self._data_for_adaptivity[name][i] = initial_micro_output[name]
+            else:
+                self._logger.info(
+                    "Micro simulation has the method initialize(), but it is not called, because adaptivity is off.")
+
+        self._micro_sims_have_output = False
+        if hasattr(micro_problem, 'output') and callable(getattr(micro_problem, 'output')):
+            self._micro_sims_have_output = True
+
+        self._dt = self._participant.get_max_time_step_size()
+
     def _read_data_from_precice(self) -> list:
         """
         Read data from preCICE.
 
         Returns
         -------
         local_read_data : list
             List of dicts in which keys are names of data being read and the values are the data from preCICE.
         """
         read_data: Dict[str, list] = dict()
         for name in self._read_data_names.keys():
             read_data[name] = []
 
-        for name, is_data_vector in self._read_data_names.items():
-            if is_data_vector:
-                read_data.update({name: self._interface.read_block_vector_data(
-                    self._read_data_ids[name], self._mesh_vertex_ids)})
-            else:
-                read_data.update({name: self._interface.read_block_scalar_data(
-                    self._read_data_ids[name], self._mesh_vertex_ids)})
+        for name in self._read_data_names.keys():
+            read_data.update({name: self._participant.read_data(
+                self._macro_mesh_name, name, self._mesh_vertex_ids, self._dt)})
 
             if self._is_adaptivity_on:
                 if name in self._adaptivity_macro_data_names:
                     self._data_for_adaptivity[name] = read_data[name]
 
         return [dict(zip(read_data, t)) for t in zip(*read_data.values())]
 
@@ -424,33 +403,24 @@
             List of dicts in which keys are names of data and the values are the data to be written to preCICE.
         """
         data_dict: Dict[str, list] = dict()
         if not self._is_rank_empty:
             for name in data[0]:
                 data_dict[name] = []
 
-            for output_dict in data:
-                for name, values in output_dict.items():
+            for d in data:
+                for name, values in d.items():
                     data_dict[name].append(values)
 
-            for dname, is_data_vector in self._write_data_names.items():
-                if is_data_vector:
-                    self._interface.write_block_vector_data(
-                        self._write_data_ids[dname], self._mesh_vertex_ids, data_dict[dname])
-                else:
-                    self._interface.write_block_scalar_data(
-                        self._write_data_ids[dname], self._mesh_vertex_ids, data_dict[dname])
+            for dname in self._write_data_names.keys():
+                self._participant.write_data(
+                    self._macro_mesh_name, dname, self._mesh_vertex_ids, data_dict[dname])
         else:
-            for dname, is_data_vector in self._write_data_names.items():
-                if is_data_vector:
-                    self._interface.write_block_vector_data(
-                        self._write_data_ids[dname], [], np.array([]))
-                else:
-                    self._interface.write_block_scalar_data(
-                        self._write_data_ids[dname], [], np.array([]))
+            for dname in self._write_data_names.keys():
+                self._participant.write_data(self._macro_mesh_name, dname, [], np.array([]))
 
     def _solve_micro_simulations(self, micro_sims_input: list) -> list:
         """
         Solve all micro simulations and assemble the micro simulations outputs in a list of dicts format.
 
         Parameters
         ----------
@@ -558,14 +528,12 @@
     args = parser.parse_args()
     config_file_path = args.config_file
     if not os.path.isabs(config_file_path):
         config_file_path = os.getcwd() + "/" + config_file_path
 
     manager = MicroManager(config_file_path)
 
-    manager.initialize()
-
     manager.solve()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `micro-manager-precice-0.3.0rc2/micro_manager/micro_simulation.py` & `micro-manager-precice-0.4.0/micro_manager/micro_simulation.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,17 +17,14 @@
     Returns
     -------
     Simulation : class
         Definition of class Simulation defined in this function.
     """
     class Simulation(micro_simulation_class):
         def __init__(self, global_id):
-            micro_simulation_class.__init__(self)
+            micro_simulation_class.__init__(self, global_id)
             self._global_id = global_id
 
         def get_global_id(self) -> int:
             return self._global_id
 
-        def set_global_id(self, global_id) -> None:
-            self._global_id = global_id
-
     return Simulation
```

### Comparing `micro-manager-precice-0.3.0rc2/micro_manager_precice.egg-info/SOURCES.txt` & `micro-manager-precice-0.4.0/micro_manager_precice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micro-manager-precice-0.3.0rc2/setup.py` & `micro-manager-precice-0.4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='micro-manager-precice',
-    version='v0.3.0rc2',
+    version='v0.4.0',
     description='micro-manager-precice is a package which facilitates two-scale macro-micro coupled simulations using preCICE',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://precice.org/tooling-micro-manager-overview.html',
     entry_points={
         'console_scripts': ['micro_manager=micro_manager.micro_manager:main']},
     author='Ishaan Desai',
     author_email='ishaan.desai@uni-stuttgart.de',
     license='LGPL-3.0',
     packages=find_packages(
         exclude=['examples']),
     install_requires=[
-        'pyprecice==2.5.0.4',
+        'pyprecice>=3.0.0.0',
         'numpy>=1.13.3',
         'mpi4py'],
     test_suite='tests',
     zip_safe=False)
```

