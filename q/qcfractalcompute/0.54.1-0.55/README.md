# Comparing `tmp/qcfractalcompute-0.54.1.tar.gz` & `tmp/qcfractalcompute-0.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcfractalcompute-0.54.1.tar", last modified: Fri Apr 12 13:20:47 2024, max compression
+gzip compressed data, was "qcfractalcompute-0.55.tar", last modified: Thu May 23 18:50:47 2024, max compression
```

## Comparing `qcfractalcompute-0.54.1.tar` & `qcfractalcompute-0.55.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-12 13:20:47.327032 qcfractalcompute-0.54.1/
--rw-r--r--   0 ben       (1000) users      (984)      655 2024-04-12 13:20:47.327032 qcfractalcompute-0.54.1/PKG-INFO
--rw-r--r--   0 ben       (1000) users      (984)     1093 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/pyproject.toml
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-12 13:20:47.327032 qcfractalcompute-0.54.1/qcfractalcompute/
--rw-r--r--   0 ben       (1000) users      (984)      238 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/qcfractalcompute/__init__.py
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-12 13:20:47.327032 qcfractalcompute-0.54.1/qcfractalcompute/apps/
--rw-r--r--   0 ben       (1000) users      (984)        0 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/qcfractalcompute/apps/__init__.py
--rw-r--r--   0 ben       (1000) users      (984)     6741 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/qcfractalcompute/apps/app_manager.py
--rw-r--r--   0 ben       (1000) users      (984)     2016 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/qcfractalcompute/apps/geometric.py
--rw-r--r--   0 ben       (1000) users      (984)     2592 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/qcfractalcompute/apps/helpers.py
--rw-r--r--   0 ben       (1000) users      (984)      464 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/qcfractalcompute/apps/models.py
--rw-r--r--   0 ben       (1000) users      (984)     3128 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/qcfractalcompute/apps/qcengine.py
--rw-r--r--   0 ben       (1000) users      (984)     4149 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/qcfractalcompute/compress.py
--rw-r--r--   0 ben       (1000) users      (984)    26916 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/qcfractalcompute/compute_manager.py
--rw-r--r--   0 ben       (1000) users      (984)     2214 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/qcfractalcompute/compute_manager_cli.py
--rw-r--r--   0 ben       (1000) users      (984)     8549 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/qcfractalcompute/config.py
--rw-r--r--   0 ben       (1000) users      (984)     8054 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/qcfractalcompute/executors.py
--rw-r--r--   0 ben       (1000) users      (984)     1868 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/qcfractalcompute/generic_wrapper.py
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-12 13:20:47.327032 qcfractalcompute-0.54.1/qcfractalcompute/run_scripts/
--rw-r--r--   0 ben       (1000) users      (984)      193 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/qcfractalcompute/run_scripts/__init__.py
--rw-r--r--   0 ben       (1000) users      (984)      230 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/qcfractalcompute/run_scripts/conda_list_env.sh
--rw-r--r--   0 ben       (1000) users      (984)     1484 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/qcfractalcompute/run_scripts/generic_script.py
--rw-r--r--   0 ben       (1000) users      (984)     2590 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/qcfractalcompute/run_scripts/geometric_nextchain.py
--rw-r--r--   0 ben       (1000) users      (984)     3529 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/qcfractalcompute/run_scripts/qcengine_compute.py
--rw-r--r--   0 ben       (1000) users      (984)      644 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/qcfractalcompute/run_scripts/qcengine_list.py
--rw-r--r--   0 ben       (1000) users      (984)     7930 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/qcfractalcompute/test_compute_manager.py
--rw-r--r--   0 ben       (1000) users      (984)     1132 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/qcfractalcompute/test_manager_config.py
--rw-r--r--   0 ben       (1000) users      (984)     6420 2024-04-12 13:20:33.000000 qcfractalcompute-0.54.1/qcfractalcompute/testing_helpers.py
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-12 13:20:47.327032 qcfractalcompute-0.54.1/qcfractalcompute.egg-info/
--rw-r--r--   0 ben       (1000) users      (984)      655 2024-04-12 13:20:47.000000 qcfractalcompute-0.54.1/qcfractalcompute.egg-info/PKG-INFO
--rw-r--r--   0 ben       (1000) users      (984)     1087 2024-04-12 13:20:47.000000 qcfractalcompute-0.54.1/qcfractalcompute.egg-info/SOURCES.txt
--rw-r--r--   0 ben       (1000) users      (984)        1 2024-04-12 13:20:47.000000 qcfractalcompute-0.54.1/qcfractalcompute.egg-info/dependency_links.txt
--rw-r--r--   0 ben       (1000) users      (984)       88 2024-04-12 13:20:47.000000 qcfractalcompute-0.54.1/qcfractalcompute.egg-info/entry_points.txt
--rw-r--r--   0 ben       (1000) users      (984)       15 2024-04-12 13:20:47.000000 qcfractalcompute-0.54.1/qcfractalcompute.egg-info/requires.txt
--rw-r--r--   0 ben       (1000) users      (984)       17 2024-04-12 13:20:47.000000 qcfractalcompute-0.54.1/qcfractalcompute.egg-info/top_level.txt
--rw-r--r--   0 ben       (1000) users      (984)       38 2024-04-12 13:20:47.327032 qcfractalcompute-0.54.1/setup.cfg
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-05-23 18:50:47.063626 qcfractalcompute-0.55/
+-rw-r--r--   0 ben       (1000) users      (984)      653 2024-05-23 18:50:47.063626 qcfractalcompute-0.55/PKG-INFO
+-rw-r--r--   0 ben       (1000) users      (984)     1093 2024-05-07 13:50:39.000000 qcfractalcompute-0.55/pyproject.toml
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-05-23 18:50:47.060293 qcfractalcompute-0.55/qcfractalcompute/
+-rw-r--r--   0 ben       (1000) users      (984)      238 2024-05-07 13:50:39.000000 qcfractalcompute-0.55/qcfractalcompute/__init__.py
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-05-23 18:50:47.063626 qcfractalcompute-0.55/qcfractalcompute/apps/
+-rw-r--r--   0 ben       (1000) users      (984)        0 2023-09-11 13:38:01.000000 qcfractalcompute-0.55/qcfractalcompute/apps/__init__.py
+-rw-r--r--   0 ben       (1000) users      (984)     6741 2024-05-07 13:50:39.000000 qcfractalcompute-0.55/qcfractalcompute/apps/app_manager.py
+-rw-r--r--   0 ben       (1000) users      (984)     2016 2024-03-11 20:25:46.000000 qcfractalcompute-0.55/qcfractalcompute/apps/geometric.py
+-rw-r--r--   0 ben       (1000) users      (984)     2592 2024-05-07 13:50:39.000000 qcfractalcompute-0.55/qcfractalcompute/apps/helpers.py
+-rw-r--r--   0 ben       (1000) users      (984)      464 2024-05-07 13:50:39.000000 qcfractalcompute-0.55/qcfractalcompute/apps/models.py
+-rw-r--r--   0 ben       (1000) users      (984)     3128 2024-05-07 13:50:39.000000 qcfractalcompute-0.55/qcfractalcompute/apps/qcengine.py
+-rw-r--r--   0 ben       (1000) users      (984)     4149 2024-03-11 20:25:46.000000 qcfractalcompute-0.55/qcfractalcompute/compress.py
+-rw-r--r--   0 ben       (1000) users      (984)    26916 2024-05-07 13:50:39.000000 qcfractalcompute-0.55/qcfractalcompute/compute_manager.py
+-rw-r--r--   0 ben       (1000) users      (984)     2214 2024-05-07 13:50:39.000000 qcfractalcompute-0.55/qcfractalcompute/compute_manager_cli.py
+-rw-r--r--   0 ben       (1000) users      (984)     8549 2024-05-07 13:50:39.000000 qcfractalcompute-0.55/qcfractalcompute/config.py
+-rw-r--r--   0 ben       (1000) users      (984)     8054 2024-05-07 13:50:39.000000 qcfractalcompute-0.55/qcfractalcompute/executors.py
+-rw-r--r--   0 ben       (1000) users      (984)     1868 2024-05-07 13:50:39.000000 qcfractalcompute-0.55/qcfractalcompute/generic_wrapper.py
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-05-23 18:50:47.063626 qcfractalcompute-0.55/qcfractalcompute/run_scripts/
+-rw-r--r--   0 ben       (1000) users      (984)      193 2023-09-11 13:38:01.000000 qcfractalcompute-0.55/qcfractalcompute/run_scripts/__init__.py
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-05-23 18:50:47.063626 qcfractalcompute-0.55/qcfractalcompute/run_scripts/__pycache__/
+-rw-r--r--   0 ben       (1000) users      (984)      791 2024-05-14 15:22:26.000000 qcfractalcompute-0.55/qcfractalcompute/run_scripts/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 ben       (1000) users      (984)      230 2023-09-11 13:38:01.000000 qcfractalcompute-0.55/qcfractalcompute/run_scripts/conda_list_env.sh
+-rw-r--r--   0 ben       (1000) users      (984)     1484 2024-05-07 13:50:39.000000 qcfractalcompute-0.55/qcfractalcompute/run_scripts/generic_script.py
+-rw-r--r--   0 ben       (1000) users      (984)     2590 2024-05-07 13:50:39.000000 qcfractalcompute-0.55/qcfractalcompute/run_scripts/geometric_nextchain.py
+-rw-r--r--   0 ben       (1000) users      (984)     3529 2024-05-07 13:50:39.000000 qcfractalcompute-0.55/qcfractalcompute/run_scripts/qcengine_compute.py
+-rw-r--r--   0 ben       (1000) users      (984)      644 2024-05-07 13:50:39.000000 qcfractalcompute-0.55/qcfractalcompute/run_scripts/qcengine_list.py
+-rw-r--r--   0 ben       (1000) users      (984)     7930 2024-05-23 18:47:51.000000 qcfractalcompute-0.55/qcfractalcompute/test_compute_manager.py
+-rw-r--r--   0 ben       (1000) users      (984)     1132 2024-05-19 15:35:34.000000 qcfractalcompute-0.55/qcfractalcompute/test_manager_config.py
+-rw-r--r--   0 ben       (1000) users      (984)     6420 2024-05-07 13:50:39.000000 qcfractalcompute-0.55/qcfractalcompute/testing_helpers.py
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-05-23 18:50:47.063626 qcfractalcompute-0.55/qcfractalcompute.egg-info/
+-rw-r--r--   0 ben       (1000) users      (984)      653 2024-05-23 18:50:47.000000 qcfractalcompute-0.55/qcfractalcompute.egg-info/PKG-INFO
+-rw-r--r--   0 ben       (1000) users      (984)     1153 2024-05-23 18:50:47.000000 qcfractalcompute-0.55/qcfractalcompute.egg-info/SOURCES.txt
+-rw-r--r--   0 ben       (1000) users      (984)        1 2024-05-23 18:50:47.000000 qcfractalcompute-0.55/qcfractalcompute.egg-info/dependency_links.txt
+-rw-r--r--   0 ben       (1000) users      (984)       88 2024-05-23 18:50:47.000000 qcfractalcompute-0.55/qcfractalcompute.egg-info/entry_points.txt
+-rw-r--r--   0 ben       (1000) users      (984)       15 2024-05-23 18:50:47.000000 qcfractalcompute-0.55/qcfractalcompute.egg-info/requires.txt
+-rw-r--r--   0 ben       (1000) users      (984)       17 2024-05-23 18:50:47.000000 qcfractalcompute-0.55/qcfractalcompute.egg-info/top_level.txt
+-rw-r--r--   0 ben       (1000) users      (984)       38 2024-05-23 18:50:47.063626 qcfractalcompute-0.55/setup.cfg
```

### Comparing `qcfractalcompute-0.54.1/PKG-INFO` & `qcfractalcompute-0.55/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcfractalcompute
-Version: 0.54.1
+Version: 0.55
 Summary: A distributed compute and database platform for quantum chemistry.
 Author-email: Benjamin Pritchard <qcarchive@molssi.org>
 Project-URL: Homepage, https://github.com/MolSSI/QCFractal
 Project-URL: Bug Tracker, https://github.com/MolSSI/QCFractal/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `qcfractalcompute-0.54.1/pyproject.toml` & `qcfractalcompute-0.55/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.54.1/qcfractalcompute/apps/app_manager.py` & `qcfractalcompute-0.55/qcfractalcompute/apps/app_manager.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.54.1/qcfractalcompute/apps/geometric.py` & `qcfractalcompute-0.55/qcfractalcompute/apps/geometric.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.54.1/qcfractalcompute/apps/helpers.py` & `qcfractalcompute-0.55/qcfractalcompute/apps/helpers.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.54.1/qcfractalcompute/apps/qcengine.py` & `qcfractalcompute-0.55/qcfractalcompute/apps/qcengine.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.54.1/qcfractalcompute/compress.py` & `qcfractalcompute-0.55/qcfractalcompute/compress.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.54.1/qcfractalcompute/compute_manager.py` & `qcfractalcompute-0.55/qcfractalcompute/compute_manager.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.54.1/qcfractalcompute/compute_manager_cli.py` & `qcfractalcompute-0.55/qcfractalcompute/compute_manager_cli.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.54.1/qcfractalcompute/config.py` & `qcfractalcompute-0.55/qcfractalcompute/config.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.54.1/qcfractalcompute/executors.py` & `qcfractalcompute-0.55/qcfractalcompute/executors.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.54.1/qcfractalcompute/generic_wrapper.py` & `qcfractalcompute-0.55/qcfractalcompute/generic_wrapper.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.54.1/qcfractalcompute/run_scripts/generic_script.py` & `qcfractalcompute-0.55/qcfractalcompute/run_scripts/generic_script.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.54.1/qcfractalcompute/run_scripts/geometric_nextchain.py` & `qcfractalcompute-0.55/qcfractalcompute/run_scripts/geometric_nextchain.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.54.1/qcfractalcompute/run_scripts/qcengine_compute.py` & `qcfractalcompute-0.55/qcfractalcompute/run_scripts/qcengine_compute.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.54.1/qcfractalcompute/run_scripts/qcengine_list.py` & `qcfractalcompute-0.55/qcfractalcompute/run_scripts/qcengine_list.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.54.1/qcfractalcompute/test_compute_manager.py` & `qcfractalcompute-0.55/qcfractalcompute/test_compute_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,17 +222,17 @@
 
 def test_manager_missed_heartbeats_shutdown(snowflake: QCATestingSnowflake):
     compute_thread = QCATestingComputeThread(snowflake._qcf_config)
     compute_thread.start(manual_updates=False)
 
     snowflake.stop_api()
 
-    for i in range(60):
+    for i in range(90):
         time.sleep(1)
 
         if not compute_thread.is_alive():
             break
     else:
-        raise RuntimeError("Compute thread did not stop in 60 seconds")
+        raise RuntimeError("Compute thread did not stop in 90 seconds")
 
     compute_thread._compute_thread.join(5)
     assert compute_thread.is_alive() is False
```

### Comparing `qcfractalcompute-0.54.1/qcfractalcompute/test_manager_config.py` & `qcfractalcompute-0.55/qcfractalcompute/test_manager_config.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
+import pytest
 import yaml
 
-import pytest
 from qcfractalcompute.config import SlurmExecutorConfig
 
 
 @pytest.mark.parametrize("time_str", ["02:01:59", "72:00:00", "10:00:00"])
 def test_manager_config_walltime(time_str):
     # Walltimes in a yaml can be parsed as seconds. Test we convert that correctly
```

### Comparing `qcfractalcompute-0.54.1/qcfractalcompute/testing_helpers.py` & `qcfractalcompute-0.55/qcfractalcompute/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.54.1/qcfractalcompute.egg-info/PKG-INFO` & `qcfractalcompute-0.55/qcfractalcompute.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcfractalcompute
-Version: 0.54.1
+Version: 0.55
 Summary: A distributed compute and database platform for quantum chemistry.
 Author-email: Benjamin Pritchard <qcarchive@molssi.org>
 Project-URL: Homepage, https://github.com/MolSSI/QCFractal
 Project-URL: Bug Tracker, https://github.com/MolSSI/QCFractal/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `qcfractalcompute-0.54.1/qcfractalcompute.egg-info/SOURCES.txt` & `qcfractalcompute-0.55/qcfractalcompute.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -22,8 +22,9 @@
 qcfractalcompute/apps/models.py
 qcfractalcompute/apps/qcengine.py
 qcfractalcompute/run_scripts/__init__.py
 qcfractalcompute/run_scripts/conda_list_env.sh
 qcfractalcompute/run_scripts/generic_script.py
 qcfractalcompute/run_scripts/geometric_nextchain.py
 qcfractalcompute/run_scripts/qcengine_compute.py
-qcfractalcompute/run_scripts/qcengine_list.py
+qcfractalcompute/run_scripts/qcengine_list.py
+qcfractalcompute/run_scripts/__pycache__/__init__.cpython-311.pyc
```

