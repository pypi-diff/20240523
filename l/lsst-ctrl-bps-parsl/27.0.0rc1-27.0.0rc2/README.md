# Comparing `tmp/lsst_ctrl_bps_parsl-27.0.0rc1.tar.gz` & `tmp/lsst_ctrl_bps_parsl-27.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst_ctrl_bps_parsl-27.0.0rc1.tar", last modified: Wed May  1 21:16:34 2024, max compression
+gzip compressed data, was "lsst_ctrl_bps_parsl-27.0.0rc2.tar", last modified: Thu May 23 01:51:54 2024, max compression
```

## Comparing `lsst_ctrl_bps_parsl-27.0.0rc1.tar` & `lsst_ctrl_bps_parsl-27.0.0rc2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:34.793176 lsst_ctrl_bps_parsl-27.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-01 21:16:34.793176 lsst_ctrl_bps_parsl-27.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/bsd_license.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:34.785175 lsst_ctrl_bps_parsl-27.0.0rc1/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:34.785175 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:34.785175 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:34.785175 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:34.789176 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    11724 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/site.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:34.789176 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/sites/
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/sites/ccin2p3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/sites/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/sites/nersc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/sites/princeton.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/sites/slac.py
--rw-r--r--   0 runner    (1001) docker     (127)    12665 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/sites/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/sites/work_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 21:16:34.000000 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11434 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:34.793176 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst_ctrl_bps_parsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-01 21:16:34.000000 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst_ctrl_bps_parsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-01 21:16:34.000000 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst_ctrl_bps_parsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:16:34.000000 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst_ctrl_bps_parsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-01 21:16:34.000000 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst_ctrl_bps_parsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 21:16:34.000000 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst_ctrl_bps_parsl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:16:34.000000 lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst_ctrl_bps_parsl.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-01 21:16:34.793176 lsst_ctrl_bps_parsl-27.0.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:34.793176 lsst_ctrl_bps_parsl-27.0.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-01 21:16:28.000000 lsst_ctrl_bps_parsl-27.0.0rc1/tests/test_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:54.329880 lsst_ctrl_bps_parsl-27.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-23 01:51:54.329880 lsst_ctrl_bps_parsl-27.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/bsd_license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:54.325880 lsst_ctrl_bps_parsl-27.0.0rc2/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:54.321880 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:54.321880 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:54.325880 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:54.325880 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11724 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/site.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:54.329880 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/sites/
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/sites/ccin2p3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/sites/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/sites/nersc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/sites/princeton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/sites/slac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12665 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/sites/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/sites/work_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 01:51:54.000000 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11434 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:54.329880 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst_ctrl_bps_parsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-23 01:51:54.000000 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst_ctrl_bps_parsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-23 01:51:54.000000 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst_ctrl_bps_parsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:51:54.000000 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst_ctrl_bps_parsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-23 01:51:54.000000 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst_ctrl_bps_parsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 01:51:54.000000 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst_ctrl_bps_parsl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:51:54.000000 lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst_ctrl_bps_parsl.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-23 01:51:54.329880 lsst_ctrl_bps_parsl-27.0.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:54.329880 lsst_ctrl_bps_parsl-27.0.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-23 01:51:48.000000 lsst_ctrl_bps_parsl-27.0.0rc2/tests/test_job.py
```

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/PKG-INFO` & `lsst_ctrl_bps_parsl-27.0.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-bps-parsl
-Version: 27.0.0rc1
+Version: 27.0.0rc2
 Summary: Parsl-based plugin for lsst-ctrl-bps.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_bps_parsl
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/README.md` & `lsst_ctrl_bps_parsl-27.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/bsd_license.txt` & `lsst_ctrl_bps_parsl-27.0.0rc2/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/gpl-v3.0.txt` & `lsst_ctrl_bps_parsl-27.0.0rc2/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/pyproject.toml` & `lsst_ctrl_bps_parsl-27.0.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/__init__.py` & `lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/configuration.py` & `lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/configuration.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/environment.py` & `lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/environment.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/job.py` & `lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/job.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/service.py` & `lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/service.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/site.py` & `lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/site.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/sites/__init__.py` & `lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/sites/ccin2p3.py` & `lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/sites/ccin2p3.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/sites/local.py` & `lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/sites/local.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/sites/nersc.py` & `lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/sites/nersc.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/sites/princeton.py` & `lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/sites/princeton.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/sites/slac.py` & `lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/sites/slac.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/sites/slurm.py` & `lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/sites/slurm.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/sites/work_queue.py` & `lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/sites/work_queue.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst/ctrl/bps/parsl/workflow.py` & `lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst/ctrl/bps/parsl/workflow.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst_ctrl_bps_parsl.egg-info/PKG-INFO` & `lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst_ctrl_bps_parsl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-bps-parsl
-Version: 27.0.0rc1
+Version: 27.0.0rc2
 Summary: Parsl-based plugin for lsst-ctrl-bps.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_bps_parsl
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/python/lsst_ctrl_bps_parsl.egg-info/SOURCES.txt` & `lsst_ctrl_bps_parsl-27.0.0rc2/python/lsst_ctrl_bps_parsl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/tests/test_config.py` & `lsst_ctrl_bps_parsl-27.0.0rc2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/tests/test_import.py` & `lsst_ctrl_bps_parsl-27.0.0rc2/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_parsl-27.0.0rc1/tests/test_job.py` & `lsst_ctrl_bps_parsl-27.0.0rc2/tests/test_job.py`

 * *Files identical despite different names*

