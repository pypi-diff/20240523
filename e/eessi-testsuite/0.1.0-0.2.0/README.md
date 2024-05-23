# Comparing `tmp/eessi-testsuite-0.1.0.tar.gz` & `tmp/eessi_testsuite-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eessi-testsuite-0.1.0.tar", last modified: Thu Oct  5 11:35:03 2023, max compression
+gzip compressed data, was "eessi_testsuite-0.2.0.tar", last modified: Thu May 23 13:14:50 2024, max compression
```

## Comparing `eessi-testsuite-0.1.0.tar` & `eessi_testsuite-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-10-05 11:35:03.324331 eessi-testsuite-0.1.0/
--rw-r--r--   0 kehoste    (501) staff       (20)    18092 2023-05-31 07:12:46.000000 eessi-testsuite-0.1.0/LICENSE
--rw-r--r--   0 kehoste    (501) staff       (20)     3156 2023-10-05 11:35:03.324430 eessi-testsuite-0.1.0/PKG-INFO
--rw-r--r--   0 kehoste    (501) staff       (20)     2728 2023-10-05 07:12:59.000000 eessi-testsuite-0.1.0/README.md
-drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-10-05 11:35:03.320578 eessi-testsuite-0.1.0/eessi/
--rw-r--r--   0 kehoste    (501) staff       (20)       56 2023-09-21 11:34:50.000000 eessi-testsuite-0.1.0/eessi/__init__.py
-drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-10-05 11:35:03.321768 eessi-testsuite-0.1.0/eessi/testsuite/
--rw-r--r--   0 kehoste    (501) staff       (20)        0 2023-09-21 11:34:50.000000 eessi-testsuite-0.1.0/eessi/testsuite/__init__.py
--rw-r--r--   0 kehoste    (501) staff       (20)     2039 2023-09-21 11:34:50.000000 eessi-testsuite-0.1.0/eessi/testsuite/common_config.py
--rw-r--r--   0 kehoste    (501) staff       (20)     1307 2023-09-06 13:13:10.000000 eessi-testsuite-0.1.0/eessi/testsuite/constants.py
--rw-r--r--   0 kehoste    (501) staff       (20)    17386 2023-09-06 13:13:10.000000 eessi-testsuite-0.1.0/eessi/testsuite/hooks.py
-drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-10-05 11:35:03.321923 eessi-testsuite-0.1.0/eessi/testsuite/tests/
--rw-r--r--   0 kehoste    (501) staff       (20)        0 2023-09-21 11:34:50.000000 eessi-testsuite-0.1.0/eessi/testsuite/tests/__init__.py
-drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-10-05 11:35:03.322152 eessi-testsuite-0.1.0/eessi/testsuite/tests/apps/
--rw-r--r--   0 kehoste    (501) staff       (20)        0 2023-09-21 11:34:50.000000 eessi-testsuite-0.1.0/eessi/testsuite/tests/apps/__init__.py
--rw-r--r--   0 kehoste    (501) staff       (20)     4776 2023-06-16 08:58:04.000000 eessi-testsuite-0.1.0/eessi/testsuite/tests/apps/gromacs.py
-drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-10-05 11:35:03.322737 eessi-testsuite-0.1.0/eessi/testsuite/tests/apps/tensorflow/
--rw-r--r--   0 kehoste    (501) staff       (20)        0 2023-09-21 11:34:50.000000 eessi-testsuite-0.1.0/eessi/testsuite/tests/apps/tensorflow/__init__.py
-drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-10-05 11:35:03.323179 eessi-testsuite-0.1.0/eessi/testsuite/tests/apps/tensorflow/src/
--rw-r--r--   0 kehoste    (501) staff       (20)        0 2023-09-21 11:34:50.000000 eessi-testsuite-0.1.0/eessi/testsuite/tests/apps/tensorflow/src/__init__.py
--rw-r--r--   0 kehoste    (501) staff       (20)     1277 2023-09-06 13:13:10.000000 eessi-testsuite-0.1.0/eessi/testsuite/tests/apps/tensorflow/src/mnist_setup.py
--rw-r--r--   0 kehoste    (501) staff       (20)     8914 2023-09-06 13:13:10.000000 eessi-testsuite-0.1.0/eessi/testsuite/tests/apps/tensorflow/src/tf_test.py
--rw-r--r--   0 kehoste    (501) staff       (20)     4781 2023-09-06 13:13:10.000000 eessi-testsuite-0.1.0/eessi/testsuite/tests/apps/tensorflow/tensorflow.py
--rw-r--r--   0 kehoste    (501) staff       (20)     5931 2023-09-06 13:13:10.000000 eessi-testsuite-0.1.0/eessi/testsuite/utils.py
-drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-10-05 11:35:03.324099 eessi-testsuite-0.1.0/eessi_testsuite.egg-info/
--rw-r--r--   0 kehoste    (501) staff       (20)     3156 2023-10-05 11:35:03.000000 eessi-testsuite-0.1.0/eessi_testsuite.egg-info/PKG-INFO
--rw-r--r--   0 kehoste    (501) staff       (20)      828 2023-10-05 11:35:03.000000 eessi-testsuite-0.1.0/eessi_testsuite.egg-info/SOURCES.txt
--rw-r--r--   0 kehoste    (501) staff       (20)        1 2023-10-05 11:35:03.000000 eessi-testsuite-0.1.0/eessi_testsuite.egg-info/dependency_links.txt
--rw-r--r--   0 kehoste    (501) staff       (20)        6 2023-10-05 11:35:03.000000 eessi-testsuite-0.1.0/eessi_testsuite.egg-info/namespace_packages.txt
--rw-r--r--   0 kehoste    (501) staff       (20)       11 2023-10-05 11:35:03.000000 eessi-testsuite-0.1.0/eessi_testsuite.egg-info/requires.txt
--rw-r--r--   0 kehoste    (501) staff       (20)        6 2023-10-05 11:35:03.000000 eessi-testsuite-0.1.0/eessi_testsuite.egg-info/top_level.txt
--rw-r--r--   0 kehoste    (501) staff       (20)      499 2023-10-05 07:13:01.000000 eessi-testsuite-0.1.0/pyproject.toml
--rw-r--r--   0 kehoste    (501) staff       (20)      571 2023-10-05 11:35:03.324890 eessi-testsuite-0.1.0/setup.cfg
--rw-r--r--   0 kehoste    (501) staff       (20)       37 2023-06-07 19:06:38.000000 eessi-testsuite-0.1.0/setup.py
+drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2024-05-23 13:14:50.746534 eessi_testsuite-0.2.0/
+-rw-r--r--   0 kehoste    (501) staff       (20)    18092 2023-05-31 07:12:46.000000 eessi_testsuite-0.2.0/LICENSE
+-rw-r--r--   0 kehoste    (501) staff       (20)    23904 2024-05-23 13:14:50.746453 eessi_testsuite-0.2.0/PKG-INFO
+-rw-r--r--   0 kehoste    (501) staff       (20)     2728 2024-05-23 13:13:00.000000 eessi_testsuite-0.2.0/README.md
+drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2024-05-23 13:14:50.742115 eessi_testsuite-0.2.0/eessi/
+-rw-r--r--   0 kehoste    (501) staff       (20)       56 2023-09-21 11:34:50.000000 eessi_testsuite-0.2.0/eessi/__init__.py
+drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2024-05-23 13:14:50.743462 eessi_testsuite-0.2.0/eessi/testsuite/
+-rw-r--r--   0 kehoste    (501) staff       (20)        0 2023-09-21 11:34:50.000000 eessi_testsuite-0.2.0/eessi/testsuite/__init__.py
+-rw-r--r--   0 kehoste    (501) staff       (20)     4382 2024-05-23 12:42:44.000000 eessi_testsuite-0.2.0/eessi/testsuite/common_config.py
+-rw-r--r--   0 kehoste    (501) staff       (20)     1894 2024-05-23 13:13:00.000000 eessi_testsuite-0.2.0/eessi/testsuite/constants.py
+-rw-r--r--   0 kehoste    (501) staff       (20)    22884 2024-05-23 13:13:00.000000 eessi_testsuite-0.2.0/eessi/testsuite/hooks.py
+drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2024-05-23 13:14:50.743828 eessi_testsuite-0.2.0/eessi/testsuite/tests/
+-rw-r--r--   0 kehoste    (501) staff       (20)        0 2023-09-21 11:34:50.000000 eessi_testsuite-0.2.0/eessi/testsuite/tests/__init__.py
+drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2024-05-23 13:14:50.744264 eessi_testsuite-0.2.0/eessi/testsuite/tests/apps/
+-rw-r--r--   0 kehoste    (501) staff       (20)        0 2023-09-21 11:34:50.000000 eessi_testsuite-0.2.0/eessi/testsuite/tests/apps/__init__.py
+-rw-r--r--   0 kehoste    (501) staff       (20)     5017 2024-05-23 13:13:00.000000 eessi_testsuite-0.2.0/eessi/testsuite/tests/apps/gromacs.py
+-rw-r--r--   0 kehoste    (501) staff       (20)    11987 2024-05-23 13:13:00.000000 eessi_testsuite-0.2.0/eessi/testsuite/tests/apps/osu.py
+drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2024-05-23 13:14:50.744535 eessi_testsuite-0.2.0/eessi/testsuite/tests/apps/tensorflow/
+-rw-r--r--   0 kehoste    (501) staff       (20)        0 2023-09-21 11:34:50.000000 eessi_testsuite-0.2.0/eessi/testsuite/tests/apps/tensorflow/__init__.py
+drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2024-05-23 13:14:50.745173 eessi_testsuite-0.2.0/eessi/testsuite/tests/apps/tensorflow/src/
+-rw-r--r--   0 kehoste    (501) staff       (20)        0 2023-09-21 11:34:50.000000 eessi_testsuite-0.2.0/eessi/testsuite/tests/apps/tensorflow/src/__init__.py
+-rw-r--r--   0 kehoste    (501) staff       (20)     1329 2024-05-23 12:42:44.000000 eessi_testsuite-0.2.0/eessi/testsuite/tests/apps/tensorflow/src/mnist_setup.py
+-rw-r--r--   0 kehoste    (501) staff       (20)     8995 2024-05-23 12:42:44.000000 eessi_testsuite-0.2.0/eessi/testsuite/tests/apps/tensorflow/src/tf_test.py
+-rw-r--r--   0 kehoste    (501) staff       (20)     4988 2024-05-23 12:42:44.000000 eessi_testsuite-0.2.0/eessi/testsuite/tests/apps/tensorflow/tensorflow.py
+-rw-r--r--   0 kehoste    (501) staff       (20)     5873 2024-05-23 13:13:00.000000 eessi_testsuite-0.2.0/eessi/testsuite/utils.py
+drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2024-05-23 13:14:50.746147 eessi_testsuite-0.2.0/eessi_testsuite.egg-info/
+-rw-r--r--   0 kehoste    (501) staff       (20)    23904 2024-05-23 13:14:50.000000 eessi_testsuite-0.2.0/eessi_testsuite.egg-info/PKG-INFO
+-rw-r--r--   0 kehoste    (501) staff       (20)      824 2024-05-23 13:14:50.000000 eessi_testsuite-0.2.0/eessi_testsuite.egg-info/SOURCES.txt
+-rw-r--r--   0 kehoste    (501) staff       (20)        1 2024-05-23 13:14:50.000000 eessi_testsuite-0.2.0/eessi_testsuite.egg-info/dependency_links.txt
+-rw-r--r--   0 kehoste    (501) staff       (20)        6 2024-05-23 13:14:50.000000 eessi_testsuite-0.2.0/eessi_testsuite.egg-info/namespace_packages.txt
+-rw-r--r--   0 kehoste    (501) staff       (20)        6 2024-05-23 13:14:50.000000 eessi_testsuite-0.2.0/eessi_testsuite.egg-info/top_level.txt
+-rw-r--r--   0 kehoste    (501) staff       (20)      499 2024-05-23 13:12:00.000000 eessi_testsuite-0.2.0/pyproject.toml
+-rw-r--r--   0 kehoste    (501) staff       (20)      629 2024-05-23 13:14:50.746820 eessi_testsuite-0.2.0/setup.cfg
+-rw-r--r--   0 kehoste    (501) staff       (20)       37 2023-06-07 19:06:38.000000 eessi_testsuite-0.2.0/setup.py
```

### Comparing `eessi-testsuite-0.1.0/LICENSE` & `eessi_testsuite-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eessi-testsuite-0.1.0/PKG-INFO` & `eessi_testsuite-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: eessi-testsuite
-Version: 0.1.0
-Summary: Test suite for the EESSI software stack
-Home-page: UNKNOWN
-License: GPL-2.0-only
-Project-URL: Homepage, https://eessi.io/docs/test-suite
-Project-URL: Bug Tracker, https://github.com/EESSI/test-suite/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # test-suite
 
 A portable test suite for software installations, using ReFrame.
 
 ## Documentation
 
 For documentation on installing, configuring, and using the EESSI test suite, see https://eessi.io/docs/test-suite/.
@@ -99,9 +85,7 @@
 
 While the initial setup is a bit more involved, the advantage of this approach
 is that it is easy to pull in updates from a feature branch using `git pull`.
 
 You can also push back changes to the feature branch directly, but note that
 you are pushing to the Github fork of another Github user, so _make sure they
 are ok with that_ before doing so!
-
-
```

### Comparing `eessi-testsuite-0.1.0/eessi/testsuite/hooks.py` & `eessi_testsuite-0.2.0/eessi/testsuite/hooks.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,65 @@
 """
 Hooks for adding tags, filtering and setting job resources in ReFrame tests
 """
 import math
 import shlex
+import warnings
 
 import reframe as rfm
 
 from eessi.testsuite.constants import *
-from eessi.testsuite.utils import get_max_avail_gpus_per_node, is_cuda_required_module, log, check_proc_attribute_defined
+from eessi.testsuite.utils import (get_max_avail_gpus_per_node, is_cuda_required_module, log,
+                                   check_proc_attribute_defined)
 
-def assign_one_task_per_compute_unit(test: rfm.RegressionTest, compute_unit: str):
+
+def _assign_default_num_cpus_per_node(test: rfm.RegressionTest):
+    """
+    Check if the default number of cpus per node is already defined in the test
+    (e.g. by earlier hooks like set_tag_scale).
+    If so, check if it doesn't exceed the maximum available.
+    If not, set default_num_cpus_per_node based on the maximum available cpus and node_part
+    """
+
+    if test.default_num_cpus_per_node:
+        # may skip if not enough CPUs
+        test.skip_if(
+            test.default_num_cpus_per_node > test.max_avail_cpus_per_node,
+            f'Requested CPUs per node ({test.default_num_cpus_per_node}) is higher than max available'
+            f' ({test.max_avail_cpus_per_node}) in current partition ({test.current_partition.name}).'
+        )
+    else:
+        # no default set yet, so setting one
+        test.default_num_cpus_per_node = int(test.max_avail_cpus_per_node / test.node_part)
+
+    log(f'default_num_cpus_per_node set to {test.default_num_cpus_per_node}')
+
+
+def _assign_default_num_gpus_per_node(test: rfm.RegressionTest):
+    """
+    Check if the default number of gpus per node is already defined in the test
+    (e.g. by earlier hooks like set_tag_scale).
+    If so, check if it doesn't exceed the maximum available.
+    If not, set default_num_gpus_per_node based on the maximum available gpus and node_part
+    """
+
+    test.max_avail_gpus_per_node = get_max_avail_gpus_per_node(test)
+    if test.default_num_gpus_per_node:
+        # may skip if not enough GPUs
+        test.skip_if(
+            test.default_num_gpus_per_node > test.max_avail_gpus_per_node,
+            f'Number of GPUs per node in selected scale ({test.default_num_gpus_per_node}) is higher than max available'
+            f' ({test.max_avail_gpus_per_node}) in current partition ({test.current_partition.name}).'
+        )
+    else:
+        # no default set yet, so setting one
+        test.default_num_gpus_per_node = math.ceil(test.max_avail_gpus_per_node / test.node_part)
+
+
+def assign_tasks_per_compute_unit(test: rfm.RegressionTest, compute_unit: str, num_per: int = 1):
     """
     Assign one task per compute unit (COMPUTE_UNIT[CPU], COMPUTE_UNIT[CPU_SOCKET] or COMPUTE_UNIT[GPU]).
     Automatically sets num_tasks, num_tasks_per_node, num_cpus_per_task, and num_gpus_per_node,
     based on the current scale and the current partition’s num_cpus, max_avail_gpus_per_node and num_nodes.
     For GPU tests, one task per GPU is set, and num_cpus_per_task is based on the ratio of CPU-cores/GPUs.
     For CPU tests, one task per CPU is set, and num_cpus_per_task is set to 1.
     Total task count is determined based on the number of nodes to be used in the test.
@@ -21,86 +67,117 @@
 
     Arguments:
     - test: the ReFrame test to which this hook should apply
     - compute_unit: a device as listed in eessi.testsuite.constants.COMPUTE_UNIT
 
     Examples:
     On a single node with 2 sockets, 64 cores and 128 hyperthreads:
-    - assign_one_task_per_compute_unit(test, COMPUTE_UNIT[CPU]) will launch 64 tasks with 1 thread
-    - assign_one_task_per_compute_unit(test, COMPUTE_UNIT[CPU_SOCKET]) will launch 2 tasks with 32 threads per task
+    - assign_tasks_per_compute_unit(test, COMPUTE_UNIT[CPU]) will launch 64 tasks with 1 thread
+    - assign_tasks_per_compute_unit(test, COMPUTE_UNIT[CPU_SOCKET]) will launch 2 tasks with 32 threads per task
 
-    Future work: 
+    Future work:
     Currently, on a single node with 2 sockets, 64 cores and 128 hyperthreads, this
-    - assign_one_task_per_compute_unit(test, COMPUTE_UNIT[CPU], true) will launch 128 tasks with 1 thread
-    - assign_one_task_per_compute_unit(test, COMPUTE_UNIT[CPU_SOCKET], true) will launch 2 tasks with 64 threads per task
+    - assign_one_task_per_compute_unit(test, COMPUTE_UNIT[CPU], true) launches 128 tasks with 1 thread
+    - assign_one_task_per_compute_unit(test, COMPUTE_UNIT[CPU_SOCKET], true) launches 2 tasks with 64 threads per task
     In the future, we'd like to add an arugment that disables spawning tasks for hyperthreads.
     """
+    if num_per != 1 and compute_unit in [COMPUTE_UNIT[GPU], COMPUTE_UNIT[CPU], COMPUTE_UNIT[CPU_SOCKET]]:
+        raise NotImplementedError(
+            f'Non-default num_per {num_per} is not implemented for compute_unit {compute_unit}.')
+
     check_proc_attribute_defined(test, 'num_cpus')
     test.max_avail_cpus_per_node = test.current_partition.processor.num_cpus
     log(f'max_avail_cpus_per_node set to {test.max_avail_cpus_per_node}')
 
     # Check if either node_part, or default_num_cpus_per_node and default_num_gpus_per_node are set correctly
     if not (
-        type(test.node_part) == int or
-        (type(test.default_num_cpus_per_node) == int and type(test.default_num_gpus_per_node) == int)
+        isinstance(test.node_part, int)
+        or (isinstance(test.default_num_cpus_per_node, int) and isinstance(test.default_num_gpus_per_node, int))
     ):
         raise ValueError(
             f'Either node_part ({test.node_part}), or default_num_cpus_per_node ({test.default_num_cpus_per_node}) and'
             f' default num_gpus_per_node ({test.default_num_gpus_per_node}) must be defined and have integer values.'
         )
 
-    # Check if the default number of cpus per node is already defined in the test
-    # (e.g. by earlier hooks like set_tag_scale).
-    # If so, check if it doesn't exceed the maximum available.
-    # If not, set default_num_cpus_per_node based on the maximum available cpus and node_part
-    if test.default_num_cpus_per_node:
-        # may skip if not enough CPUs
-        test.skip_if(
-            test.default_num_cpus_per_node > test.max_avail_cpus_per_node,
-            f'Requested CPUs per node ({test.default_num_cpus_per_node}) is higher than max available'
-            f' ({test.max_avail_cpus_per_node}) in current partition ({test.current_partition.name}).'
-        )
-    else:
-        # no default set yet, so setting one
-        test.default_num_cpus_per_node = int(test.max_avail_cpus_per_node / test.node_part)
+    _assign_default_num_cpus_per_node(test)
 
-    log(f'default_num_cpus_per_node set to {test.default_num_cpus_per_node}')
+    if FEATURES[GPU] in test.current_partition.features:
+        _assign_default_num_gpus_per_node(test)
 
     if compute_unit == COMPUTE_UNIT[GPU]:
         _assign_one_task_per_gpu(test)
     elif compute_unit == COMPUTE_UNIT[CPU]:
         _assign_one_task_per_cpu(test)
     elif compute_unit == COMPUTE_UNIT[CPU_SOCKET]:
         _assign_one_task_per_cpu_socket(test)
+    elif compute_unit == COMPUTE_UNIT[NODE]:
+        _assign_num_tasks_per_node(test, num_per)
     else:
         raise ValueError(f'compute unit {compute_unit} is currently not supported')
 
+    _check_always_request_gpus(test)
+
+
+def _assign_num_tasks_per_node(test: rfm.RegressionTest, num_per: int = 1):
+    """
+    Sets num_tasks_per_node and num_cpus_per_task such that it will run
+    'num_per' tasks per node, unless specified with:
+    --setvar num_tasks_per_node=<x>
+    --setvar num_cpus_per_task=<y>.
+    In those cases, those take precedence, and the remaining variable, if any
+    (num_cpus_per task or num_tasks_per_node respectively), is calculated based
+    on the equality test.num_tasks_per_node * test.num_cpus_per_task ==
+    test.default_num_cpus_per_node.
+
+    Default resources requested:
+    - num_tasks_per_node = num_per
+    - num_cpus_per_task = test.default_num_cpus_per_node / num_tasks_per_node
+    """
+
+    # neither num_tasks_per_node nor num_cpus_per_task are set
+    if not test.num_tasks_per_node and not test.num_cpus_per_task:
+        test.num_tasks_per_node = num_per
+        test.num_cpus_per_task = int(test.default_num_cpus_per_node / test.num_tasks_per_node)
+
+    # num_tasks_per_node is not set, but num_cpus_per_task is
+    elif not test.num_tasks_per_node:
+        test.num_tasks_per_node = int(test.default_num_cpus_per_node / test.num_cpus_per_task)
+
+    # num_cpus_per_task is not set, but num_tasks_per_node is
+    elif not test.num_cpus_per_task:
+        test.num_cpus_per_task = int(test.default_num_cpus_per_node / test.num_tasks_per_node)
+
+    else:
+        pass  # both num_tasks_per_node and num_cpus_per_task are already set
+
+    test.num_tasks = test.num_nodes * test.num_tasks_per_node
+
+    log(f'num_tasks_per_node set to {test.num_tasks_per_node}')
+    log(f'num_cpus_per_task set to {test.num_cpus_per_task}')
+    log(f'num_tasks set to {test.num_tasks}')
+
+
 def _assign_one_task_per_cpu_socket(test: rfm.RegressionTest):
     """
     Determines the number of tasks per node by dividing the default_num_cpus_per_node by
-    the number of cpus available per socket, and rounding up. The result is that for full-node jobs the default 
+    the number of cpus available per socket, and rounding up. The result is that for full-node jobs the default
     will spawn one task per socket, with a number of cpus per task equal to the number of cpus per socket.
     Other examples:
     - half a node (i.e. node_part=2) on a 4-socket system would result in 2 tasks per node,
     with number of cpus per task equal to the number of cpus per socket.
-    - 2 cores (i.e. default_num_cpus_per_node=2) on a 16 core system with 2 sockets would result in 
+    - 2 cores (i.e. default_num_cpus_per_node=2) on a 16 core system with 2 sockets would result in
     1 task per node, with 2 cpus per task
 
     This default is set unless the test is run with:
     --setvar num_tasks_per_node=<x> and/or
     --setvar num_cpus_per_task=<y>.
-    In those cases, those take precedence, and the remaining variable (num_cpus_per task or 
+    In those cases, those take precedence, and the remaining variable (num_cpus_per task or
     num_tasks_per_node respectively) is calculated based on the equality
     test.num_tasks_per_node * test.num_cpus_per_task == test.default_num_cpus_per_node.
 
-    Variables:
-    - default_num_cpus_per_node: default number of CPUs per node as defined in the test
-    (e.g. by earlier hooks like set_tag_scale)
-
-
     Default resources requested:
     - num_tasks_per_node = default_num_cpus_per_node
     - num_cpus_per_task = default_num_cpus_per_node / num_tasks_per_node
     """
     # neither num_tasks_per_node nor num_cpus_per_task are set
     if not test.num_tasks_per_node and not test.num_cpus_per_task:
         check_proc_attribute_defined(test, 'num_cpus')
@@ -124,40 +201,36 @@
         pass  # both num_tasks_per_node and num_cpus_per_node are already set
 
     test.num_tasks = test.num_nodes * test.num_tasks_per_node
     log(f'Number of tasks per node set to: {test.num_tasks_per_node}')
     log(f'Number of cpus per task set to {test.num_cpus_per_task}')
     log(f'num_tasks set to {test.num_tasks}')
 
+
 def _assign_one_task_per_cpu(test: rfm.RegressionTest):
     """
     Sets num_tasks_per_node and num_cpus_per_task such that it will run one task per core,
     unless specified with:
     --setvar num_tasks_per_node=<x> and/or
     --setvar num_cpus_per_task=<y>.
 
-    Variables:
-    - default_num_cpus_per_node: default number of CPUs per node as defined in the test
-    (e.g. by earlier hooks like set_tag_scale)
-
-
     Default resources requested:
     - num_tasks_per_node = default_num_cpus_per_node
     - num_cpus_per_task = default_num_cpus_per_node / num_tasks_per_node
     """
-    # neither num_tasks_per_node nor num_cpus_per_node are set
+    # neither num_tasks_per_node nor num_cpus_per_task are set
     if not test.num_tasks_per_node and not test.num_cpus_per_task:
         test.num_tasks_per_node = test.default_num_cpus_per_node
         test.num_cpus_per_task = 1
 
-    # num_tasks_per_node is not set, but num_cpus_per_node is
+    # num_tasks_per_node is not set, but num_cpus_per_task is
     elif not test.num_tasks_per_node:
         test.num_tasks_per_node = int(test.default_num_cpus_per_node / test.num_cpus_per_task)
 
-    # num_cpus_per_node is not set, but num_tasks_per_node is
+    # num_cpus_per_task is not set, but num_tasks_per_node is
     elif not test.num_cpus_per_task:
         test.num_cpus_per_task = int(test.default_num_cpus_per_node / test.num_tasks_per_node)
 
     else:
         pass  # both num_tasks_per_node and num_cpus_per_node are already set
 
     test.num_tasks = test.num_nodes * test.num_tasks_per_node
@@ -170,43 +243,22 @@
 def _assign_one_task_per_gpu(test: rfm.RegressionTest):
     """
     Sets num_tasks_per_node, num_cpus_per_task, and num_gpus_per_node, unless specified with:
     --setvar num_tasks_per_node=<x> and/or
     --setvar num_cpus_per_task=<y> and/or
     --setvar num_gpus_per_node=<z>.
 
-    Variables:
-    - max_avail_gpus_per_node: maximum available number of GPUs per node
-    - default_num_gpus_per_node: default number of GPUs per node as defined in the test
-    (e.g. by earlier hooks like set_tag_scale)
-
     Default resources requested:
     - num_gpus_per_node = default_num_gpus_per_node
     - num_tasks_per_node = num_gpus_per_node
     - num_cpus_per_task = default_num_cpus_per_node / num_tasks_per_node
 
     If num_tasks_per_node is set, set num_gpus_per_node equal to either num_tasks_per_node or default_num_gpus_per_node
     (whichever is smallest), unless num_gpus_per_node is also set.
     """
-    max_avail_gpus_per_node = get_max_avail_gpus_per_node(test)
-
-    # Check if the default number of gpus per node is already defined in the test
-    # (e.g. by earlier hooks like set_tag_scale).
-    # If so, check if it doesn't exceed the maximum available.
-    # If not, set default_num_gpus_per_node based on the maximum available gpus and node_part
-    if test.default_num_gpus_per_node:
-        # may skip if not enough GPUs
-        test.skip_if(
-            test.default_num_gpus_per_node > max_avail_gpus_per_node,
-            f'Requested GPUs per node ({test.default_num_gpus_per_node}) is higher than max available'
-            f' ({max_avail_gpus_per_node}) in current partition ({test.current_partition.name}).'
-        )
-    else:
-        # no default set yet, so setting one
-        test.default_num_gpus_per_node = math.ceil(max_avail_gpus_per_node / test.node_part)
 
     # neither num_tasks_per_node nor num_gpus_per_node are set
     if not test.num_tasks_per_node and not test.num_gpus_per_node:
         test.num_gpus_per_node = test.default_num_gpus_per_node
         test.num_tasks_per_node = test.num_gpus_per_node
 
     # num_tasks_per_node is not set, but num_gpus_per_node is
@@ -221,52 +273,106 @@
         pass  # both num_tasks_per_node and num_gpus_per_node are already set
 
     # num_cpus_per_task is not set
     if not test.num_cpus_per_task:
         # limit num_cpus_per_task to the maximum available cpus per gpu
         test.num_cpus_per_task = min(
             int(test.default_num_cpus_per_node / test.num_tasks_per_node),
-            int(test.max_avail_cpus_per_node / max_avail_gpus_per_node)
+            int(test.max_avail_cpus_per_node / test.max_avail_gpus_per_node)
         )
 
     test.num_tasks = test.num_nodes * test.num_tasks_per_node
 
     log(f'num_gpus_per_node set to {test.num_gpus_per_node}')
     log(f'num_tasks_per_node set to {test.num_tasks_per_node}')
     log(f'num_cpus_per_task set to {test.num_cpus_per_task}')
     log(f'num_tasks set to {test.num_tasks}')
 
 
+def _set_or_append_valid_systems(test: rfm.RegressionTest, valid_systems: str):
+    """
+    Sets test.valid_systems based on the valid_systems argument.
+    - If valid_systems is an empty string, test.valid_systems is set equal to eessi.testsuite.constants.INVALID_SYSTEM
+    - If test.valid_systems was an empty list, leave it as is (test should not be run)
+    - If test.valid_systems was at the default value ['*'], it is overwritten by [valid_system]
+    - If test.valid_systems was already set and is a list of one element, valid_system is appended to it,
+    which allows adding requests for multiple partition features by different hooks.
+    - If test.valid_systems was already set and is a list of multiple elements, we warn that the use has to take
+    care of filtering him/herself. This is typically the case when someone overrides the valid_systems on command line.
+    In this scenario, this function leaves test.valid_systems as it is.
+    """
+
+    # This indicates an invalid test that always has to be filtered
+    if valid_systems == '':
+        test.valid_systems = [INVALID_SYSTEM]
+        return
+
+    # test.valid_systems wasn't set yet, so set it
+    if len(test.valid_systems) == 0 or test.valid_systems == [INVALID_SYSTEM]:
+        # test.valid_systems is empty or invalid, meaning all tests are filtered out. This hook shouldn't change that
+        return
+    # test.valid_systems still at default value, so overwrite
+    elif len(test.valid_systems) == 1 and test.valid_systems[0] == '*':
+        test.valid_systems = [valid_systems]
+    # test.valid_systems was set before, so append
+    elif len(test.valid_systems) == 1:
+        test.valid_systems[0] = f'{test.valid_systems[0]} {valid_systems}'
+    else:
+        warn_msg = f"valid_systems has multiple ({len(test.valid_systems)}) items,"
+        warn_msg += " which is not supported by this hook."
+        warn_msg += " Make sure to handle filtering yourself."
+        warnings.warn(warn_msg)
+        return
+
+
+def filter_supported_scales(test: rfm.RegressionTest):
+    """
+    Filter tests scales based on which scales are supported by each partition in the ReFrame configuration.
+    Filtering is done using features, i.e. the current test scale is requested as a feature.
+    Any partition that does not include this feature in the ReFrame configuration file will effectively be filtered out.
+    """
+    valid_systems = f'+{test.scale}'
+
+    # Change test.valid_systems accordingly:
+    _set_or_append_valid_systems(test, valid_systems)
+
+    log(f'valid_systems set to {test.valid_systems}')
+
+
 def filter_valid_systems_by_device_type(test: rfm.RegressionTest, required_device_type: str):
     """
     Filter valid_systems by required device type and by whether the module supports CUDA,
     unless valid_systems is specified with --setvar valid_systems=<comma-separated-list>.
-    """
-    if test.valid_systems:
-        # valid_systems is specified, so don't filter
-        return
 
+    Any invalid combination (e.g. a non-CUDA module with a required_device_type GPU) will
+    cause the valid_systems to be set to an empty string, and consequently the
+    test.valid_systems to an invalid system name (eessi.testsuite.constants.INVALID_SYSTEM).
+    """
     is_cuda_module = is_cuda_required_module(test.module_name)
 
     if is_cuda_module and required_device_type == DEVICE_TYPES[GPU]:
         # CUDA modules and when using a GPU require partitions with FEATURES[GPU] feature and
         # GPU_VENDOR=GPU_VENDORS[NVIDIA] extras
         valid_systems = f'+{FEATURES[GPU]} %{GPU_VENDOR}={GPU_VENDORS[NVIDIA]}'
 
-    elif required_device_type == DEVICE_TYPES[CPU]:
+    elif not is_cuda_module and required_device_type == DEVICE_TYPES[CPU]:
         # Using the CPU requires partitions with FEATURES[CPU] feature
         # Note: making FEATURES[CPU] an explicit feature allows e.g. skipping CPU-based tests on GPU partitions
         valid_systems = f'+{FEATURES[CPU]}'
 
+    elif is_cuda_module and required_device_type == DEVICE_TYPES[CPU]:
+        # Note: This applies for CUDA module tests that want to test only on cpus on gpu partitions.
+        valid_systems = f'+{FEATURES[CPU]} +{FEATURES[GPU]} %{GPU_VENDOR}={GPU_VENDORS[NVIDIA]}'
+
     elif not is_cuda_module and required_device_type == DEVICE_TYPES[GPU]:
         # Invalid combination: a module without GPU support cannot use a GPU
         valid_systems = ''
 
-    if valid_systems:
-        test.valid_systems = [valid_systems]
+    # Change test.valid_systems accordingly:
+    _set_or_append_valid_systems(test, valid_systems)
 
     log(f'valid_systems set to {test.valid_systems}')
 
 
 def set_modules(test: rfm.RegressionTest):
     """
     Skip current test if module_name is not among a list of modules,
@@ -331,15 +437,16 @@
     test.env_vars['I_MPI_PIN_CELL'] = 'core'  # Don't bind to hyperthreads, only to physcial cores
     test.env_vars['I_MPI_PIN_DOMAIN'] = '%s:compact' % physical_cpus_per_task
     test.env_vars['OMPI_MCA_rmaps_base_mapping_policy'] = 'node:PE=%s' % physical_cpus_per_task
     # Default binding for SLURM. Only effective if the task/affinity plugin is enabled
     # and when number of tasks times cpus per task equals either socket, core or thread count
     test.env_vars['SLURM_CPU_BIND'] = 'verbose'
     log(f'Set environment variable I_MPI_PIN_DOMAIN to {test.env_vars["I_MPI_PIN_DOMAIN"]}')
-    log(f'Set environment variable OMPI_MCA_rmaps_base_mapping_policy to {test.env_vars["OMPI_MCA_rmaps_base_mapping_policy"]}')
+    log('Set environment variable OMPI_MCA_rmaps_base_mapping_policy to '
+        f'{test.env_vars["OMPI_MCA_rmaps_base_mapping_policy"]}')
     log(f'Set environment variable SLURM_CPU_BIND to {test.env_vars["SLURM_CPU_BIND"]}')
 
 
 def set_compact_thread_binding(test: rfm.RegressionTest):
     """
     This hook sets a binding policy for thread binding.
     It sets a number of environment variables to try and set a sensible binding for OPENMP tasks.
@@ -348,12 +455,21 @@
     - GNU OpenMP (through OMP_NUM_THREADS, OMP_PLACES and OMP_PROC_BIND)
     - Intel OpenMP (through KMP_AFFINITY)
     """
 
     # Set thread binding
     test.env_vars['OMP_PLACES'] = 'cores'
     test.env_vars['OMP_PROC_BIND'] = 'close'
-    # See https://www.intel.com/content/www/us/en/docs/cpp-compiler/developer-guide-reference/2021-8/thread-affinity-interface.html
+    # See https://www.intel.com/content/www/us/en/docs/cpp-compiler/developer-guide-reference/2021-8/thread-affinity-interface.html  # noqa
     test.env_vars['KMP_AFFINITY'] = 'granularity=fine,compact,1,0'
     log(f'Set environment variable OMP_PLACES to {test.env_vars["OMP_PLACES"]}')
     log(f'Set environment variable OMP_PROC_BIND to {test.env_vars["OMP_PROC_BIND"]}')
     log(f'Set environment variable KMP_AFFINITY to {test.env_vars["KMP_AFFINITY"]}')
+
+
+def _check_always_request_gpus(test: rfm.RegressionTest):
+    """
+    Make sure we always request enough GPUs if required for the current GPU partition (cluster-specific policy)
+    """
+    if FEATURES[ALWAYS_REQUEST_GPUS] in test.current_partition.features and not test.num_gpus_per_node:
+        test.num_gpus_per_node = test.default_num_gpus_per_node
+        log(f'num_gpus_per_node set to {test.num_gpus_per_node} for partition {test.current_partition.name}')
```

### Comparing `eessi-testsuite-0.1.0/eessi/testsuite/tests/apps/gromacs.py` & `eessi_testsuite-0.2.0/eessi/testsuite/tests/apps/gromacs.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,34 +26,38 @@
 Hooks acting on all possible test combinations (before filtering) are called after the 'init' stage.
 Hooks acting on concrete test cases (after filtering) are called after the 'setup' stage.
 
 See also https://reframe-hpc.readthedocs.io/en/stable/pipeline.html
 """
 
 import reframe as rfm
+from reframe.core.builtins import parameter, run_after  # added only to make the linter happy
 
 from hpctestlib.sciapps.gromacs.benchmarks import gromacs_check
 
 from eessi.testsuite import hooks
 from eessi.testsuite.constants import SCALES, TAGS
 from eessi.testsuite.utils import find_modules, log
 
 
 @rfm.simple_test
-class GROMACS_EESSI(gromacs_check):
+class EESSI_GROMACS(gromacs_check):
     scale = parameter(SCALES.keys())
     valid_prog_environs = ['default']
-    valid_systems = []
+    valid_systems = ['*']
     time_limit = '30m'
     module_name = parameter(find_modules('GROMACS'))
 
     @run_after('init')
     def run_after_init(self):
         """Hooks to run after the init phase"""
 
+        # Filter on which scales are supported by the partitions defined in the ReFrame configuration
+        hooks.filter_supported_scales(self)
+
         # Make sure that GPU tests run in partitions that support running on a GPU,
         # and that CPU-only tests run in partitions that support running CPU-only.
         # Also support setting valid_systems on the cmd line.
         hooks.filter_valid_systems_by_device_type(self, required_device_type=self.nb_impl)
 
         # Support selecting modules on the cmd line.
         hooks.set_modules(self)
@@ -85,15 +89,15 @@
     @run_after('setup')
     def run_after_setup(self):
         """Hooks to run after the setup phase"""
 
         # Calculate default requested resources based on the scale:
         # 1 task per CPU for CPU-only tests, 1 task per GPU for GPU tests.
         # Also support setting the resources on the cmd line.
-        hooks.assign_one_task_per_compute_unit(test=self, compute_unit=self.nb_impl)
+        hooks.assign_tasks_per_compute_unit(test=self, compute_unit=self.nb_impl)
 
     @run_after('setup')
     def set_omp_num_threads(self):
         """
         Set number of OpenMP threads.
         Set both OMP_NUM_THREADS and -ntomp explicitly to avoid conflicting values.
         Set default number of OpenMP threads equal to number of CPUs per task.
```

### Comparing `eessi-testsuite-0.1.0/eessi/testsuite/tests/apps/tensorflow/src/mnist_setup.py` & `eessi_testsuite-0.2.0/eessi/testsuite/tests/apps/tensorflow/src/mnist_setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import tensorflow as tf
 import numpy as np
 
+
 def mnist_dataset(batch_size, test_batch_size):
-  (x_train, y_train), (x_test, y_test) = tf.keras.datasets.mnist.load_data()
-  # The `x` arrays are in uint8 and have values in the [0, 255] range.
-  # You need to convert them to float32 with values in the [0, 1] range.
-  x_train = x_train / np.float32(255)
-  y_train = y_train.astype(np.int64)
-  x_test = x_test / np.float32(255)
-  y_test = y_test.astype(np.int64)
-  train_dataset = tf.data.Dataset.from_tensor_slices(
-      (x_train, y_train)).shuffle(60000).repeat().batch(batch_size)
-  test_dataset = tf.data.Dataset.from_tensor_slices(
-      (x_test, y_test)).batch(test_batch_size)
-  return train_dataset, test_dataset
+    (x_train, y_train), (x_test, y_test) = tf.keras.datasets.mnist.load_data()
+    # The `x` arrays are in uint8 and have values in the [0, 255] range.
+    # You need to convert them to float32 with values in the [0, 1] range.
+    x_train = x_train / np.float32(255)
+    y_train = y_train.astype(np.int64)
+    x_test = x_test / np.float32(255)
+    y_test = y_test.astype(np.int64)
+    train_dataset = tf.data.Dataset.from_tensor_slices(
+        (x_train, y_train)).shuffle(60000).repeat().batch(batch_size)
+    test_dataset = tf.data.Dataset.from_tensor_slices(
+        (x_test, y_test)).batch(test_batch_size)
+    return train_dataset, test_dataset
+
 
 def build_and_compile_cnn_model():
-  model = tf.keras.Sequential([
-      tf.keras.layers.InputLayer(input_shape=(28, 28)),
-      tf.keras.layers.Reshape(target_shape=(28, 28, 1)),
-      tf.keras.layers.Conv2D(32, 3, activation='relu'),
-      tf.keras.layers.Flatten(),
-      tf.keras.layers.Dense(128, activation='relu'),
-      tf.keras.layers.Dense(10)
-  ])
-  model.compile(
-      loss=tf.keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-      optimizer=tf.keras.optimizers.Adam(learning_rate=0.001),
-      metrics=['accuracy'])
-  return model
+    model = tf.keras.Sequential([
+        tf.keras.layers.InputLayer(input_shape=(28, 28)),
+        tf.keras.layers.Reshape(target_shape=(28, 28, 1)),
+        tf.keras.layers.Conv2D(32, 3, activation='relu'),
+        tf.keras.layers.Flatten(),
+        tf.keras.layers.Dense(128, activation='relu'),
+        tf.keras.layers.Dense(10)
+    ])
+    model.compile(
+        loss=tf.keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+        optimizer=tf.keras.optimizers.Adam(learning_rate=0.001),
+        metrics=['accuracy'])
+    return model
```

### Comparing `eessi-testsuite-0.1.0/eessi/testsuite/tests/apps/tensorflow/src/tf_test.py` & `eessi_testsuite-0.2.0/eessi/testsuite/tests/apps/tensorflow/src/tf_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,85 +10,100 @@
 
 from contextlib import closing
 from mpi4py import MPI
 from timeit import default_timer as timer
 
 import tensorflow as tf
 
+
 def print0(msg, comm=MPI.COMM_WORLD):
     '''Prints string "msg" from rank 0'''
     output = comm.gather(msg, root=0)
     rank = comm.Get_rank()
     # Print elements per rank
     if rank == 0:
         for (rank, rank_out) in enumerate(output):
             print(f'Rank {rank}: {rank_out}')
 
+
 def find_free_port():
     '''Function that gets a free port for the current process'''
     with closing(socket.socket()) as s:
         s.bind(('', 0))
-        s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR,1)
+        s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         return s.getsockname()[1]
 
+
 def get_local_rank(rank_info, rank_info_list):
     '''Function that figures out the local rank based on a list of rank,
     hostname, and port gathered from each of the workers'''
     # Note that rank_info_list is sorted by rank, by definition of the MPI allgather routine.
     # Thus, if our current rank is the n-th item in rank_info_list for which the hostname matches,
     # our local rank is n
     for index, item in enumerate(rank_info_list):
         if item['hostname'] == rank_info['hostname'] and item['rank'] == rank_info['rank']:
-                return index
+            return index
+
 
 def get_rank_info(comm=MPI.COMM_WORLD):
     '''Create a dict for this worker containing rank, hostname and port to be used by this worker'''
     rank = comm.Get_rank()
     hostname = socket.gethostname()
     port = find_free_port()
-    
+
     return {
         'rank': rank,
         'hostname': hostname,
         'port': port,
     }
 
+
 def set_tf_config(rank_info, rank_info_list):
     '''Sets the TF_CONFIG environment variable for the current worker, based on the rank_info_list'''
     worker_list = ['%s:%s' % (item['hostname'], item['port']) for item in rank_info_list]
-    
+
     tf_config = {
         'cluster': {
             'worker': worker_list,
         },
         'task': {'type': 'worker', 'index': rank_info['rank']}
     }
     os.environ["TF_CONFIG"] = json.dumps(tf_config)
-    
+
     # logger.info(f"Set TF_CONFIG for rank {rank_info['rank']} to {tf_config}.")
     print0(f"Set TF_CONFIG for rank {rank_info['rank']} to {tf_config}.")
     return tf_config
 
+
 parser = argparse.ArgumentParser(
-                    prog='Tensorflow Distributed Test',
-                    description='This program runs a distributed TensorFlow test using the tf.distribute.MultiWorkerMirroredStrategy and the Keras fit API'
-)
-parser.add_argument('-d', '--device', type=str, default='cpu', choices=['cpu', 'gpu'], help='Device to use for training')
-parser.add_argument('--inter-op-parallelism', type=int, default=1, help='Sets tf.config.threading.set_inter_op_parallelism_threads')
-parser.add_argument('--intra-op-parallelism', type=int, default=0, help='Sets tf.config.threading.set_intra_op_parallelism_threads')
-parser.add_argument('--per-worker-batch-size', type=int, default=4096, help='Batch size processed by each worker')
-parser.add_argument('--per-worker-test-batch-size', type=int, default=512, help='Batch size for computing accuracy on the validation set')
-parser.add_argument('--epochs-to-train', type=int, default=4, help='Number of epochs to train')
-parser.add_argument('--steps-per-epoch', type=int, default=25, help='Number of steps to train per epoch')
+    prog='Tensorflow Distributed Test',
+    description='This program runs a distributed TensorFlow test using the tf.distribute.MultiWorkerMirroredStrategy'
+                ' and the Keras fit API')
+
+parser.add_argument(
+    '-d', '--device', type=str, default='cpu', choices=['cpu', 'gpu'], help='Device to use for training')
+parser.add_argument(
+    '--inter-op-parallelism', type=int, default=1, help='Sets tf.config.threading.set_inter_op_parallelism_threads')
+parser.add_argument(
+    '--intra-op-parallelism', type=int, default=0, help='Sets tf.config.threading.set_intra_op_parallelism_threads')
+parser.add_argument(
+    '--per-worker-batch-size', type=int, default=4096, help='Batch size processed by each worker')
+parser.add_argument(
+    '--per-worker-test-batch-size', type=int, default=512,
+    help='Batch size for computing accuracy on the validation set')
+parser.add_argument(
+    '--epochs-to-train', type=int, default=4, help='Number of epochs to train')
+parser.add_argument(
+    '--steps-per-epoch', type=int, default=25, help='Number of steps to train per epoch')
 args = parser.parse_args()
 
 # Make sure we can import mnist_setup from current dir
 if '.' not in sys.path:
-  sys.path.insert(0, '.')
-import mnist_setup
+    sys.path.insert(0, '.')
+import mnist_setup  # noqa: E402
 
 os.environ.pop('TF_CONFIG', None)
 
 # Set number of threads to use. Needs to be set early, before initialization
 tf.config.threading.set_inter_op_parallelism_threads(args.inter_op_parallelism)
 tf.config.threading.set_intra_op_parallelism_threads(args.intra_op_parallelism)
 
@@ -97,51 +112,53 @@
 # and allreduce that information to create a TF_CONFIG
 comm = MPI.COMM_WORLD
 rank_info = get_rank_info(comm)
 rank_info_list = comm.allgather(rank_info)
 local_rank = get_local_rank(rank_info, rank_info_list)
 
 # Create logger per rank
-#logging.basicConfig(
-#    filename='rank_%s.out' % local_rank,
-#    format='%(asctime)s %(levelname)s %(message)s',
-#    datefmt='%Y-%m-%d %H:%M:%S'
-#)
-#logging.info(f"Rank {rank_info['rank']} has local_rank {local_rank}, hostname {rank_info['hostname']} and port {rank_info['port']}")
-print0(f"Rank {rank_info['rank']} has local_rank {local_rank}, hostname {rank_info['hostname']} and port {rank_info['port']}")
+# logging.basicConfig(
+#     filename='rank_%s.out' % local_rank,
+#     format='%(asctime)s %(levelname)s %(message)s',
+#     datefmt='%Y-%m-%d %H:%M:%S'
+# )
+# logging.info(f"Rank {rank_info['rank']} has local_rank {local_rank}, hostname {rank_info['hostname']}"
+#              " and port {rank_info['port']}")
+print0(f"Rank {rank_info['rank']} has local_rank {local_rank}, hostname {rank_info['hostname']}"
+       " and port {rank_info['port']}")
 
 # Turn off tensorflow info and warnings for rank != 0
 if local_rank != 0:
     print("Turning off logging")
-    #tf.get_logger().setLevel('ERROR')
-    #tf.autograph.set_verbosity(1)
-    #tf.compat.v1.logging.set_verbosity(tf.compat.v1.logging.ERROR)
+    # tf.get_logger().setLevel('ERROR')
+    # tf.autograph.set_verbosity(1)
+    # tf.compat.v1.logging.set_verbosity(tf.compat.v1.logging.ERROR)
     os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'
 
 tf_config = set_tf_config(rank_info, rank_info_list)
 num_workers = len(tf_config['cluster']['worker'])
 
 # Set visible devices and create MultiWorkerMirroredStrategy
-#logging.info(f"Selecting device: {args.device}")
+# logging.info(f"Selecting device: {args.device}")
 print0(f"Selecting device: {args.device}")
 if args.device == 'gpu':
     # Limit each local rank to its own GPU.
     physical_devices = tf.config.list_physical_devices('GPU')
     try:
         # We could do local_rank % len(physical_devices) if we wanted to support running more than one rank per device
         # The current code doesn't support that
         tf.config.set_visible_devices(physical_devices[local_rank], 'GPU')
         visible_devices = tf.config.get_visible_devices('GPU')
         # logging.info("Local rank: %s, visible_devices: %s" % (local_rank, visible_devices))
         print0("Local rank: %s, visible_devices: %s" % (local_rank, visible_devices))
         assert len(visible_devices) == 1
-    except:
+    except Exception:
         print0("ERROR: Selection of GPU device based on local rank failed. Local rank: %s. Selected devices: %s"
-                      % (local_rank, visible_devices))
-        # logging.error("Selection of GPU device based on local rank failed. Local rank: %s. Selected devices: %s" 
+               % (local_rank, visible_devices))
+        # logging.error("Selection of GPU device based on local rank failed. Local rank: %s. Selected devices: %s"
         #       % (local_rank, visible_devices))
 
     # Should now have 1 GPU per process. Set memory growth for that device to avoid issues similar to
     # https://github.com/tensorflow/tensorflow/issues/45044
     # TODO: I have the feeling this is only needed because rank 0 somehow erroneously starts on CPU?
     # The fact that rank 0 started on CPU was triggered by setting OMP_PROC_BIND. I need to test if the following
     # line is still needed if we don't set OMP* binding variables
@@ -152,37 +169,38 @@
         implementation=tf.distribute.experimental.CommunicationImplementation.NCCL)
     strategy = tf.distribute.MultiWorkerMirroredStrategy(communication_options=communication_options)
 elif args.device == 'cpu':
     # Run on CPU, so make sure no GPU devices are visible
     tf.config.set_visible_devices([], 'GPU')
     visible_devices = tf.config.get_visible_devices()
     print0("Local rank: %s, visible_devices: %s" % (local_rank, visible_devices))
-    # logging.info("Local rank: %s, visible_devices: %s" % (local_rank, visible_devices))    
+    # logging.info("Local rank: %s, visible_devices: %s" % (local_rank, visible_devices))
     strategy = tf.distribute.MultiWorkerMirroredStrategy()
 # logging.info("Multiworker strategy created")
 print0("Multiworker strategy created")
 
 # Get datasets
 global_batch_size = args.per_worker_batch_size * num_workers
 global_test_batch_size = args.per_worker_test_batch_size * num_workers
 multi_worker_dataset, multi_worker_test_dataset = mnist_setup.mnist_dataset(global_batch_size, global_test_batch_size)
 
 with strategy.scope():
     multi_worker_model = mnist_setup.build_and_compile_cnn_model()
 
 # Run the training
 starttime = timer()
-multi_worker_model.fit(multi_worker_dataset, epochs=args.epochs_to_train, steps_per_epoch=args.steps_per_epoch, verbose=2)
+multi_worker_model.fit(
+    multi_worker_dataset, epochs=args.epochs_to_train, steps_per_epoch=args.steps_per_epoch, verbose=2)
 endtime = timer()
-#logging.info("Keras fit completed!")
+# logging.info("Keras fit completed!")
 print0("Keras fit completed!")
 
 # Compute performance
-training_time = endtime-starttime
-total_samples_trained = global_batch_size*args.steps_per_epoch*args.epochs_to_train
+training_time = endtime - starttime
+total_samples_trained = global_batch_size * args.steps_per_epoch * args.epochs_to_train
 throughput = total_samples_trained / training_time
 if local_rank == 0:
     print(f"Total training time: {training_time}")
     print(f"Performance: {throughput} img/s")
 
 # Run evaluation to check accuracy on validation set
 logging.info("Run evaluation")
```

### Comparing `eessi-testsuite-0.1.0/eessi/testsuite/tests/apps/tensorflow/tensorflow.py` & `eessi_testsuite-0.2.0/eessi/testsuite/tests/apps/tensorflow/tensorflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,56 +4,58 @@
 https://www.tensorflow.org/tutorials/distribute/multi_worker_with_keras
 """
 
 import reframe as rfm
 import reframe.utility.sanity as sn
 
 from eessi.testsuite import hooks, utils
-from eessi.testsuite.constants import *
+from eessi.testsuite.constants import *  # noqa
+
 
 @rfm.simple_test
-class TENSORFLOW_EESSI(rfm.RunOnlyRegressionTest):
+class EESSI_TensorFlow(rfm.RunOnlyRegressionTest):
 
     # This test can run at any scale, so parameterize over all known SCALES
     scale = parameter(SCALES.keys())
     valid_prog_environs = ['default']
-    valid_systems = []
+    valid_systems = ['*']
 
     # Parameterize over all modules that start with TensorFlow
     module_name = parameter(utils.find_modules('TensorFlow'))
 
     # Make CPU and GPU versions of this test
     device_type = parameter(['cpu', 'gpu'])
-    
+
     executable = 'python tf_test.py'
 
     time_limit = '30m'
 
     # This test should be run as part of EESSI CI
     tags = {TAGS['CI']}
 
     @deferrable
     def assert_tf_config_ranks(self):
         '''Assert that each rank sets a TF_CONFIG'''
-        n_ranks = sn.count(sn.extractall('^Rank [0-9]+: Set TF_CONFIG for rank (?P<rank>[0-9]+)', self.stdout, tag='rank'))
+        n_ranks = sn.count(sn.extractall(
+            '^Rank [0-9]+: Set TF_CONFIG for rank (?P<rank>[0-9]+)', self.stdout, tag='rank'))
         return sn.assert_eq(n_ranks, self.num_tasks)
 
     @deferrable
     def assert_completion(self):
         '''Assert that the test ran until completion'''
         n_fit_completed = sn.count(sn.extractall('^Rank [0-9]+: Keras fit completed', self.stdout))
-        
+
         return sn.all([
             sn.assert_eq(n_fit_completed, self.num_tasks),
         ])
 
     @deferrable
     def assert_convergence(self):
         '''Assert that the network learned _something_ during training'''
-        accuracy=sn.extractsingle('^Final accuracy: (?P<accuracy>\S+)', self.stdout, 'accuracy', float)
+        accuracy = sn.extractsingle('^Final accuracy: (?P<accuracy>\S+)', self.stdout, 'accuracy', float)  # noqa: W605
         # mnist is a 10-class classification problem, so if accuracy >> 0.2 the network 'learned' something
         return sn.assert_gt(accuracy, 0.2)
 
     @sanity_function
     def assert_sanity(self):
         '''Check all sanity criteria'''
         return sn.all([
@@ -65,14 +67,17 @@
     @performance_function('img/s')
     def perf(self):
         return sn.extractsingle(r'^Performance:\s+(?P<perf>\S+)', self.stdout, 'perf', float)
 
     @run_after('init')
     def run_after_init(self):
         """hooks to run after the init phase"""
+        # Filter on which scales are supported by the partitions defined in the ReFrame configuration
+        hooks.filter_supported_scales(self)
+
         hooks.filter_valid_systems_by_device_type(self, required_device_type=self.device_type)
         hooks.set_modules(self)
         hooks.set_tag_scale(self)
 
     @run_after('init')
     def set_executable_opts(self):
         """Set executable opts based on device_type parameter"""
@@ -87,28 +92,32 @@
         self.descr = f'TensorFlow benchmark on {self.device_type}'
 
     @run_after('setup')
     def run_after_setup(self):
         """hooks to run after the setup phase"""
         # TODO: implement
         # It should bind to socket, but different MPIs may have different arguments to do that...
-        # We should at very least prevent that it binds to single core per process, as that results in many threads being scheduled to one core
+        # We should at very least prevent that it binds to single core per process,
+        # as that results in many threads being scheduled to one core.
         # binding may also differ per launcher used. It'll be hard to support a wide range and still get proper binding
         if self.device_type == 'cpu':
-            hooks.assign_one_task_per_compute_unit(test=self, compute_unit=COMPUTE_UNIT['CPU_SOCKET'])
+            hooks.assign_tasks_per_compute_unit(test=self, compute_unit=COMPUTE_UNIT['CPU_SOCKET'])
         elif self.device_type == 'gpu':
-            hooks.assign_one_task_per_compute_unit(test=self, compute_unit=COMPUTE_UNIT['GPU'])
+            hooks.assign_tasks_per_compute_unit(test=self, compute_unit=COMPUTE_UNIT['GPU'])
         else:
             raise NotImplementedError(f'Failed to set number of tasks and cpus per task for device {self.device_type}')
 
     @run_after('setup')
     def set_thread_count_args(self):
         """Set exectuable opts defining the thread count"""
         if not self.has_custom_executable_opts:
             self.executable_opts += ['--intra-op-parallelism', '%s' % self.num_cpus_per_task]
             self.executable_opts += ['--inter-op-parallelism', '1']
             utils.log(f'executable_opts set to {self.executable_opts}')
 
     @run_after('setup')
     def set_binding_policy(self):
-        """Sets a binding policy for tasks. We don't bind threads because of https://github.com/tensorflow/tensorflow/issues/60843"""
+        """
+        Sets a binding policy for tasks. We don't bind threads because of
+        https://github.com/tensorflow/tensorflow/issues/60843
+        """
         hooks.set_compact_process_binding(self)
```

### Comparing `eessi-testsuite-0.1.0/eessi/testsuite/utils.py` & `eessi_testsuite-0.2.0/eessi/testsuite/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import re
 import sys
 from typing import Iterator
 
 import reframe as rfm
 import reframe.core.runtime as rt
 from reframe.frontend.printer import PrettyPrinter
-from reframe.utility import OrderedSet
 
 from eessi.testsuite.constants import *
 
 printer = PrettyPrinter()
 
 
 def log(msg, logger=printer.debug):
@@ -58,19 +57,19 @@
 
 
 def find_modules(regex: str, name_only=True) -> Iterator[str]:
     """
     Return all modules matching the regular expression regex. Note that since we use re.search,
     a module matches if the regex matches the module name at any place. I.e. the match does
     not have to be at the start of the smodule name
-    
+
     Arguments:
     - regex: a regular expression
     - name_only: regular expressions will only be matched on the module name, not the version (default: True).
-    
+
     Note: the name_only feature assumes anything after the last forward '/' is the version,
     and strips that before doing a match.
 
     Example
 
     Suppose we have the following modules on a system:
 
@@ -105,31 +104,32 @@
             # Remove trailing slashes from the regex (in case the callee forgot)
             regex = regex.rstrip('/')
             # Remove part after the last forward slash, as we assume this is the version
             mod = re.sub('/[^/]*$', '', mod)
         # Match the actual regular expression
         log(f"Matching module {mod} with regex {regex}")
         if re.search(regex, mod):
-            log(f"Match!")
+            log("Match!")
             yield orig_mod
 
+
 def check_proc_attribute_defined(test: rfm.RegressionTest, attribute) -> bool:
     """
     Checks if a processor feature is defined (i.e. if test.current_partition.processor.<somefeature> is defined)
-    If not, throws an informative error message. 
-    
+    If not, throws an informative error message.
+
     Arguments:
     - test: the reframe regression test instance for which should be checked if the processor feature is defined
     - attribute: attribute of the processor object, as defined by systems.partitions.processor
 
     Return:
     - True (bool) if the attribute is defined
     - Function does not return (but raises an error) if the attribute is undefined
 
-    Current known attributes in ReFrame are arch, num_cpus, num_cpus_per_core and topology, 
+    Current known attributes in ReFrame are arch, num_cpus, num_cpus_per_core and topology,
     but this may change in the future.
 
     If ReFrame's autodetect feature is used, all of these should be properly defined, so that's what we advice.
     """
 
     if test.current_partition:
         if getattr(test.current_partition.processor, attribute):
@@ -145,8 +145,7 @@
     else:
         msg = (
             "This test's current_partition is not set yet. "
             "The function utils.proc_attribute_defined should only be called after the setup() phase of ReFrame."
             "This is a programming error, please report this issue."
         )
         raise AttributeError(msg)
-
```

### Comparing `eessi-testsuite-0.1.0/eessi_testsuite.egg-info/SOURCES.txt` & `eessi_testsuite-0.2.0/eessi_testsuite.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 eessi/testsuite/common_config.py
 eessi/testsuite/constants.py
 eessi/testsuite/hooks.py
 eessi/testsuite/utils.py
 eessi/testsuite/tests/__init__.py
 eessi/testsuite/tests/apps/__init__.py
 eessi/testsuite/tests/apps/gromacs.py
+eessi/testsuite/tests/apps/osu.py
 eessi/testsuite/tests/apps/tensorflow/__init__.py
 eessi/testsuite/tests/apps/tensorflow/tensorflow.py
 eessi/testsuite/tests/apps/tensorflow/src/__init__.py
 eessi/testsuite/tests/apps/tensorflow/src/mnist_setup.py
 eessi/testsuite/tests/apps/tensorflow/src/tf_test.py
 eessi_testsuite.egg-info/PKG-INFO
 eessi_testsuite.egg-info/SOURCES.txt
 eessi_testsuite.egg-info/dependency_links.txt
 eessi_testsuite.egg-info/namespace_packages.txt
-eessi_testsuite.egg-info/requires.txt
 eessi_testsuite.egg-info/top_level.txt
```

### Comparing `eessi-testsuite-0.1.0/setup.cfg` & `eessi_testsuite-0.2.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eessi-testsuite
-version = 0.1.0
+version = 0.2.0
 description = Test suite for the EESSI software stack
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GPL-2.0-only
 classifiers = 
 	Programming Language :: Python :: 3
 project_urls = 
@@ -17,11 +17,15 @@
 python_requires = >=3.6
 packages = find:
 namespace_packages = eessi
 
 [options.packages.find]
 include = eessi*
 
+[flake8]
+max-line-length = 120
+ignore = F403, F405, W503
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

