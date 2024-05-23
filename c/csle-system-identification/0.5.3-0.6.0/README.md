# Comparing `tmp/csle_system_identification-0.5.3.tar.gz` & `tmp/csle_system_identification-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_system_identification-0.5.3.tar", last modified: Mon May 13 17:19:52 2024, max compression
+gzip compressed data, was "csle_system_identification-0.6.0.tar", last modified: Thu May 23 17:43:16 2024, max compression
```

## Comparing `csle_system_identification-0.5.3.tar` & `csle_system_identification-0.6.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:52.318570 csle_system_identification-0.5.3/
--rw-rw-r--   0 kim       (1000) kim       (1000)      661 2024-05-13 17:19:52.318570 csle_system_identification-0.5.3/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     4330 2024-01-29 11:24:00.000000 csle_system_identification-0.5.3/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      686 2023-08-08 14:54:06.000000 csle_system_identification-0.5.3/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     2012 2024-05-13 17:19:52.318570 csle_system_identification-0.5.3/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_system_identification-0.5.3/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:52.314571 csle_system_identification-0.5.3/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:52.314571 csle_system_identification-0.5.3/src/csle_system_identification/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_system_identification-0.5.3/src/csle_system_identification/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-05-13 17:19:17.000000 csle_system_identification-0.5.3/src/csle_system_identification/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:52.314571 csle_system_identification-0.5.3/src/csle_system_identification/base/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.5.3/src/csle_system_identification/base/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2398 2023-07-11 06:36:56.000000 csle_system_identification-0.5.3/src/csle_system_identification/base/base_system_identification_algorithm.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:52.314571 csle_system_identification-0.5.3/src/csle_system_identification/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.5.3/src/csle_system_identification/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      984 2023-07-11 06:36:56.000000 csle_system_identification-0.5.3/src/csle_system_identification/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:52.318570 csle_system_identification-0.5.3/src/csle_system_identification/empirical/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.5.3/src/csle_system_identification/empirical/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7360 2023-07-28 08:44:18.000000 csle_system_identification-0.5.3/src/csle_system_identification/empirical/empirical_algorithm.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    17176 2024-01-29 11:24:00.000000 csle_system_identification-0.5.3/src/csle_system_identification/emulator.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:52.318570 csle_system_identification-0.5.3/src/csle_system_identification/expectation_maximization/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.5.3/src/csle_system_identification/expectation_maximization/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7604 2023-07-28 08:44:18.000000 csle_system_identification-0.5.3/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:52.318570 csle_system_identification-0.5.3/src/csle_system_identification/gp/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.5.3/src/csle_system_identification/gp/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     9926 2024-01-29 11:24:00.000000 csle_system_identification-0.5.3/src/csle_system_identification/gp/gp_regression_algorithm.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:52.318570 csle_system_identification-0.5.3/src/csle_system_identification/job_controllers/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.5.3/src/csle_system_identification/job_controllers/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2159 2024-01-29 11:24:00.000000 csle_system_identification-0.5.3/src/csle_system_identification/job_controllers/data_collection_job_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2212 2023-03-28 14:03:22.000000 csle_system_identification-0.5.3/src/csle_system_identification/job_controllers/system_identification_job_manager.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:52.318570 csle_system_identification-0.5.3/src/csle_system_identification/mcmc/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-07-04 07:24:50.000000 csle_system_identification-0.5.3/src/csle_system_identification/mcmc/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7967 2023-07-28 08:44:18.000000 csle_system_identification-0.5.3/src/csle_system_identification/mcmc/mcmc.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:52.314571 csle_system_identification-0.5.3/src/csle_system_identification.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      661 2024-05-13 17:19:52.000000 csle_system_identification-0.5.3/src/csle_system_identification.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     1461 2024-05-13 17:19:52.000000 csle_system_identification-0.5.3/src/csle_system_identification.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-05-13 17:19:52.000000 csle_system_identification-0.5.3/src/csle_system_identification.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:36:14.000000 csle_system_identification-0.5.3/src/csle_system_identification.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      604 2024-05-13 17:19:52.000000 csle_system_identification-0.5.3/src/csle_system_identification.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       27 2024-05-13 17:19:52.000000 csle_system_identification-0.5.3/src/csle_system_identification.egg-info/top_level.txt
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:52.318570 csle_system_identification-0.5.3/tests/
--rw-rw-r--   0 kim       (1000) kim       (1000)     2226 2024-01-29 11:24:00.000000 csle_system_identification-0.5.3/tests/test_empirical_algorithm.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:16.899074 csle_system_identification-0.6.0/
+-rw-r--r--   0 kim        (501) staff       (20)      661 2024-05-23 17:43:16.899148 csle_system_identification-0.6.0/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)     4330 2024-02-13 12:24:16.000000 csle_system_identification-0.6.0/README.md
+-rw-r--r--   0 kim        (501) staff       (20)      686 2023-08-15 10:44:03.000000 csle_system_identification-0.6.0/pyproject.toml
+-rw-r--r--   0 kim        (501) staff       (20)     2012 2024-05-23 17:43:16.899408 csle_system_identification-0.6.0/setup.cfg
+-rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_system_identification-0.6.0/setup.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:16.893351 csle_system_identification-0.6.0/src/
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:16.894700 csle_system_identification-0.6.0/src/csle_system_identification/
+-rw-r--r--   0 kim        (501) staff       (20)       37 2023-08-15 10:44:03.000000 csle_system_identification-0.6.0/src/csle_system_identification/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-23 17:42:57.000000 csle_system_identification-0.6.0/src/csle_system_identification/__version__.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:16.896132 csle_system_identification-0.6.0/src/csle_system_identification/base/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_system_identification-0.6.0/src/csle_system_identification/base/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     2398 2023-08-15 10:44:03.000000 csle_system_identification-0.6.0/src/csle_system_identification/base/base_system_identification_algorithm.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:16.896683 csle_system_identification-0.6.0/src/csle_system_identification/constants/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_system_identification-0.6.0/src/csle_system_identification/constants/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)      984 2023-08-15 10:44:03.000000 csle_system_identification-0.6.0/src/csle_system_identification/constants/constants.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:16.897081 csle_system_identification-0.6.0/src/csle_system_identification/empirical/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_system_identification-0.6.0/src/csle_system_identification/empirical/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     7360 2023-08-15 10:44:03.000000 csle_system_identification-0.6.0/src/csle_system_identification/empirical/empirical_algorithm.py
+-rw-r--r--   0 kim        (501) staff       (20)    17176 2024-02-13 12:24:16.000000 csle_system_identification-0.6.0/src/csle_system_identification/emulator.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:16.897492 csle_system_identification-0.6.0/src/csle_system_identification/expectation_maximization/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_system_identification-0.6.0/src/csle_system_identification/expectation_maximization/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     7604 2023-08-15 10:44:03.000000 csle_system_identification-0.6.0/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:16.897765 csle_system_identification-0.6.0/src/csle_system_identification/gp/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_system_identification-0.6.0/src/csle_system_identification/gp/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     9926 2023-08-26 12:55:18.000000 csle_system_identification-0.6.0/src/csle_system_identification/gp/gp_regression_algorithm.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:16.898404 csle_system_identification-0.6.0/src/csle_system_identification/job_controllers/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_system_identification-0.6.0/src/csle_system_identification/job_controllers/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     2159 2023-08-22 07:27:08.000000 csle_system_identification-0.6.0/src/csle_system_identification/job_controllers/data_collection_job_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)     2212 2023-08-15 10:44:03.000000 csle_system_identification-0.6.0/src/csle_system_identification/job_controllers/system_identification_job_manager.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:16.898659 csle_system_identification-0.6.0/src/csle_system_identification/mcmc/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_system_identification-0.6.0/src/csle_system_identification/mcmc/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     7967 2023-08-15 10:44:03.000000 csle_system_identification-0.6.0/src/csle_system_identification/mcmc/mcmc.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:16.895928 csle_system_identification-0.6.0/src/csle_system_identification.egg-info/
+-rw-r--r--   0 kim        (501) staff       (20)      661 2024-05-23 17:43:16.000000 csle_system_identification-0.6.0/src/csle_system_identification.egg-info/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)     1461 2024-05-23 17:43:16.000000 csle_system_identification-0.6.0/src/csle_system_identification.egg-info/SOURCES.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-23 17:43:16.000000 csle_system_identification-0.6.0/src/csle_system_identification.egg-info/dependency_links.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:39:52.000000 csle_system_identification-0.6.0/src/csle_system_identification.egg-info/not-zip-safe
+-rw-r--r--   0 kim        (501) staff       (20)      604 2024-05-23 17:43:16.000000 csle_system_identification-0.6.0/src/csle_system_identification.egg-info/requires.txt
+-rw-r--r--   0 kim        (501) staff       (20)       27 2024-05-23 17:43:16.000000 csle_system_identification-0.6.0/src/csle_system_identification.egg-info/top_level.txt
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:16.898805 csle_system_identification-0.6.0/tests/
+-rw-r--r--   0 kim        (501) staff       (20)     2226 2023-08-17 14:55:58.000000 csle_system_identification-0.6.0/tests/test_empirical_algorithm.py
```

### Comparing `csle_system_identification-0.5.3/PKG-INFO` & `csle_system_identification-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_system_identification
-Version: 0.5.3
+Version: 0.6.0
 Summary: Scripts for system identification in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_system_identification-0.5.3/README.md` & `csle_system_identification-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.5.3/pyproject.toml` & `csle_system_identification-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.5.3/setup.cfg` & `csle_system_identification-0.6.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-base>=0.5.3
-	csle-common>=0.5.3
-	csle-collector>=0.5.3
-	csle-attacker>=0.5.3
-	csle-defender>=0.5.3
+	csle-base>=0.6.0
+	csle-common>=0.6.0
+	csle-collector>=0.6.0
+	csle-attacker>=0.6.0
+	csle-defender>=0.6.0
 	gpytorch>=1.9.0
 	pymc>=5.5.0
 	pytensor>=2.12.3
 	scikit-learn>=1.3.0
 python_requires = >=3.8
 package_dir = 
 	=src
```

### Comparing `csle_system_identification-0.5.3/src/csle_system_identification/base/base_system_identification_algorithm.py` & `csle_system_identification-0.6.0/src/csle_system_identification/base/base_system_identification_algorithm.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.5.3/src/csle_system_identification/constants/constants.py` & `csle_system_identification-0.6.0/src/csle_system_identification/constants/constants.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.5.3/src/csle_system_identification/empirical/empirical_algorithm.py` & `csle_system_identification-0.6.0/src/csle_system_identification/empirical/empirical_algorithm.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.5.3/src/csle_system_identification/emulator.py` & `csle_system_identification-0.6.0/src/csle_system_identification/emulator.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.5.3/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py` & `csle_system_identification-0.6.0/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.5.3/src/csle_system_identification/gp/gp_regression_algorithm.py` & `csle_system_identification-0.6.0/src/csle_system_identification/gp/gp_regression_algorithm.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.5.3/src/csle_system_identification/job_controllers/data_collection_job_manager.py` & `csle_system_identification-0.6.0/src/csle_system_identification/job_controllers/data_collection_job_manager.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.5.3/src/csle_system_identification/job_controllers/system_identification_job_manager.py` & `csle_system_identification-0.6.0/src/csle_system_identification/job_controllers/system_identification_job_manager.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.5.3/src/csle_system_identification/mcmc/mcmc.py` & `csle_system_identification-0.6.0/src/csle_system_identification/mcmc/mcmc.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.5.3/src/csle_system_identification.egg-info/PKG-INFO` & `csle_system_identification-0.6.0/src/csle_system_identification.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-system-identification
-Version: 0.5.3
+Version: 0.6.0
 Summary: Scripts for system identification in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_system_identification-0.5.3/src/csle_system_identification.egg-info/SOURCES.txt` & `csle_system_identification-0.6.0/src/csle_system_identification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.5.3/src/csle_system_identification.egg-info/requires.txt` & `csle_system_identification-0.6.0/src/csle_system_identification.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-csle-base>=0.5.3
-csle-common>=0.5.3
-csle-collector>=0.5.3
-csle-attacker>=0.5.3
-csle-defender>=0.5.3
+csle-base>=0.6.0
+csle-common>=0.6.0
+csle-collector>=0.6.0
+csle-attacker>=0.6.0
+csle-defender>=0.6.0
 gpytorch>=1.9.0
 pymc>=5.5.0
 pytensor>=2.12.3
 scikit-learn>=1.3.0
 
 [testing]
 pytest>=6.0
```

### Comparing `csle_system_identification-0.5.3/tests/test_empirical_algorithm.py` & `csle_system_identification-0.6.0/tests/test_empirical_algorithm.py`

 * *Files identical despite different names*

