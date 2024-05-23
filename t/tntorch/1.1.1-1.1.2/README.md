# Comparing `tmp/tntorch-1.1.1.tar.gz` & `tmp/tntorch-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tntorch-1.1.1.tar", last modified: Thu May 23 10:44:32 2024, max compression
+gzip compressed data, was "tntorch-1.1.2.tar", last modified: Thu May 23 11:48:40 2024, max compression
```

## Comparing `tntorch-1.1.1.tar` & `tntorch-1.1.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 rballester  (1000) rballester  (1000)        0 2024-05-23 10:44:32.068362 tntorch-1.1.1/
--rw-r--r--   0 rballester  (1000) rballester  (1000)     7652 2020-03-06 08:50:47.000000 tntorch-1.1.1/LICENSE
--rw-r--r--   0 rballester  (1000) rballester  (1000)      997 2024-05-23 10:44:32.068362 tntorch-1.1.1/PKG-INFO
--rw-r--r--   0 rballester  (1000) rballester  (1000)     6543 2022-11-23 11:38:14.000000 tntorch-1.1.1/README.md
--rw-rw-r--   0 rballester  (1000) rballester  (1000)       38 2024-05-23 10:44:32.068362 tntorch-1.1.1/setup.cfg
--rw-r--r--   0 rballester  (1000) rballester  (1000)     1427 2024-05-23 10:44:22.000000 tntorch-1.1.1/setup.py
-drwxrwxr-x   0 rballester  (1000) rballester  (1000)        0 2024-05-23 10:44:32.064362 tntorch-1.1.1/tests/
--rw-r--r--   0 rballester  (1000) rballester  (1000)      732 2022-02-07 12:49:29.000000 tntorch-1.1.1/tests/test_automata.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)     1188 2022-09-16 15:06:04.000000 tntorch-1.1.1/tests/test_cross.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)      791 2020-10-14 07:43:34.000000 tntorch-1.1.1/tests/test_gpu.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)     3798 2020-03-06 08:50:47.000000 tntorch-1.1.1/tests/test_indexing.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)      345 2020-03-06 08:50:47.000000 tntorch-1.1.1/tests/test_init.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)      324 2020-10-11 07:45:43.000000 tntorch-1.1.1/tests/test_interpolation.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)     1303 2022-09-16 15:06:04.000000 tntorch-1.1.1/tests/test_matrix.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)     2788 2020-03-06 08:50:47.000000 tntorch-1.1.1/tests/test_ops.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)     2083 2020-03-06 08:50:47.000000 tntorch-1.1.1/tests/test_round.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)    15691 2022-04-22 06:43:13.000000 tntorch-1.1.1/tests/test_tensor.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)     1188 2021-08-13 16:56:39.000000 tntorch-1.1.1/tests/test_tools.py
-drwxrwxr-x   0 rballester  (1000) rballester  (1000)        0 2024-05-23 10:44:32.068362 tntorch-1.1.1/tntorch/
--rw-r--r--   0 rballester  (1000) rballester  (1000)      317 2022-09-16 15:06:04.000000 tntorch-1.1.1/tntorch/__init__.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)     7354 2024-05-23 10:39:03.000000 tntorch-1.1.1/tntorch/anova.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)     3881 2024-05-23 10:39:38.000000 tntorch-1.1.1/tntorch/autodiff.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)     3517 2024-05-23 10:39:34.000000 tntorch-1.1.1/tntorch/automata.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)    10186 2024-05-23 10:39:33.000000 tntorch-1.1.1/tntorch/create.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)    23111 2024-05-23 10:39:36.000000 tntorch-1.1.1/tntorch/cross.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)    10198 2024-05-23 10:39:31.000000 tntorch-1.1.1/tntorch/derivatives.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)    23015 2024-05-23 10:39:15.000000 tntorch-1.1.1/tntorch/interpolation.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)     5758 2024-05-23 10:39:14.000000 tntorch-1.1.1/tntorch/logic.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)    15602 2024-05-23 10:39:13.000000 tntorch-1.1.1/tntorch/matrix.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)     6028 2024-05-23 10:39:12.000000 tntorch-1.1.1/tntorch/maxvol.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)    15386 2024-05-23 10:39:09.000000 tntorch-1.1.1/tntorch/metrics.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)     7733 2024-05-23 10:39:08.000000 tntorch-1.1.1/tntorch/ops.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)     5227 2024-05-23 10:39:06.000000 tntorch-1.1.1/tntorch/round.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)    84077 2024-05-23 10:39:39.000000 tntorch-1.1.1/tntorch/tensor.py
--rw-r--r--   0 rballester  (1000) rballester  (1000)    21004 2024-05-23 10:39:29.000000 tntorch-1.1.1/tntorch/tools.py
-drwxrwxr-x   0 rballester  (1000) rballester  (1000)        0 2024-05-23 10:44:32.068362 tntorch-1.1.1/tntorch.egg-info/
--rw-r--r--   0 rballester  (1000) rballester  (1000)      997 2024-05-23 10:44:32.000000 tntorch-1.1.1/tntorch.egg-info/PKG-INFO
--rw-r--r--   0 rballester  (1000) rballester  (1000)      740 2024-05-23 10:44:32.000000 tntorch-1.1.1/tntorch.egg-info/SOURCES.txt
--rw-r--r--   0 rballester  (1000) rballester  (1000)        1 2024-05-23 10:44:32.000000 tntorch-1.1.1/tntorch.egg-info/dependency_links.txt
--rw-r--r--   0 rballester  (1000) rballester  (1000)        1 2021-02-05 18:23:50.000000 tntorch-1.1.1/tntorch.egg-info/not-zip-safe
--rw-r--r--   0 rballester  (1000) rballester  (1000)       24 2024-05-23 10:44:32.000000 tntorch-1.1.1/tntorch.egg-info/requires.txt
--rw-r--r--   0 rballester  (1000) rballester  (1000)        8 2024-05-23 10:44:32.000000 tntorch-1.1.1/tntorch.egg-info/top_level.txt
+drwxrwxr-x   0 rballester  (1000) rballester  (1000)        0 2024-05-23 11:48:40.842180 tntorch-1.1.2/
+-rw-r--r--   0 rballester  (1000) rballester  (1000)     7652 2020-03-06 08:50:47.000000 tntorch-1.1.2/LICENSE
+-rw-r--r--   0 rballester  (1000) rballester  (1000)      997 2024-05-23 11:48:40.842180 tntorch-1.1.2/PKG-INFO
+-rw-r--r--   0 rballester  (1000) rballester  (1000)     6543 2022-11-23 11:38:14.000000 tntorch-1.1.2/README.md
+-rw-rw-r--   0 rballester  (1000) rballester  (1000)       38 2024-05-23 11:48:40.842180 tntorch-1.1.2/setup.cfg
+-rw-r--r--   0 rballester  (1000) rballester  (1000)     1427 2024-05-23 11:47:54.000000 tntorch-1.1.2/setup.py
+drwxrwxr-x   0 rballester  (1000) rballester  (1000)        0 2024-05-23 11:48:40.838180 tntorch-1.1.2/tests/
+-rw-r--r--   0 rballester  (1000) rballester  (1000)      732 2022-02-07 12:49:29.000000 tntorch-1.1.2/tests/test_automata.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)     1188 2022-09-16 15:06:04.000000 tntorch-1.1.2/tests/test_cross.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)      791 2020-10-14 07:43:34.000000 tntorch-1.1.2/tests/test_gpu.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)     3798 2020-03-06 08:50:47.000000 tntorch-1.1.2/tests/test_indexing.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)      345 2020-03-06 08:50:47.000000 tntorch-1.1.2/tests/test_init.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)      324 2020-10-11 07:45:43.000000 tntorch-1.1.2/tests/test_interpolation.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)     1303 2022-09-16 15:06:04.000000 tntorch-1.1.2/tests/test_matrix.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)     2788 2020-03-06 08:50:47.000000 tntorch-1.1.2/tests/test_ops.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)     2083 2020-03-06 08:50:47.000000 tntorch-1.1.2/tests/test_round.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)    15691 2022-04-22 06:43:13.000000 tntorch-1.1.2/tests/test_tensor.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)     1188 2021-08-13 16:56:39.000000 tntorch-1.1.2/tests/test_tools.py
+drwxrwxr-x   0 rballester  (1000) rballester  (1000)        0 2024-05-23 11:48:40.838180 tntorch-1.1.2/tntorch/
+-rw-r--r--   0 rballester  (1000) rballester  (1000)      317 2022-09-16 15:06:04.000000 tntorch-1.1.2/tntorch/__init__.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)     7354 2024-05-23 10:39:03.000000 tntorch-1.1.2/tntorch/anova.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)     3881 2024-05-23 10:39:38.000000 tntorch-1.1.2/tntorch/autodiff.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)     3517 2024-05-23 10:39:34.000000 tntorch-1.1.2/tntorch/automata.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)    10186 2024-05-23 10:39:33.000000 tntorch-1.1.2/tntorch/create.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)    23111 2024-05-23 10:39:36.000000 tntorch-1.1.2/tntorch/cross.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)    10198 2024-05-23 10:39:31.000000 tntorch-1.1.2/tntorch/derivatives.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)    23015 2024-05-23 10:39:15.000000 tntorch-1.1.2/tntorch/interpolation.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)     5758 2024-05-23 10:39:14.000000 tntorch-1.1.2/tntorch/logic.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)    15602 2024-05-23 10:39:13.000000 tntorch-1.1.2/tntorch/matrix.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)     6028 2024-05-23 10:39:12.000000 tntorch-1.1.2/tntorch/maxvol.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)    15386 2024-05-23 10:39:09.000000 tntorch-1.1.2/tntorch/metrics.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)     7733 2024-05-23 10:39:08.000000 tntorch-1.1.2/tntorch/ops.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)     5227 2024-05-23 10:39:06.000000 tntorch-1.1.2/tntorch/round.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)    84077 2024-05-23 10:39:39.000000 tntorch-1.1.2/tntorch/tensor.py
+-rw-r--r--   0 rballester  (1000) rballester  (1000)    21004 2024-05-23 10:39:29.000000 tntorch-1.1.2/tntorch/tools.py
+drwxrwxr-x   0 rballester  (1000) rballester  (1000)        0 2024-05-23 11:48:40.842180 tntorch-1.1.2/tntorch.egg-info/
+-rw-r--r--   0 rballester  (1000) rballester  (1000)      997 2024-05-23 11:48:40.000000 tntorch-1.1.2/tntorch.egg-info/PKG-INFO
+-rw-r--r--   0 rballester  (1000) rballester  (1000)      740 2024-05-23 11:48:40.000000 tntorch-1.1.2/tntorch.egg-info/SOURCES.txt
+-rw-r--r--   0 rballester  (1000) rballester  (1000)        1 2024-05-23 11:48:40.000000 tntorch-1.1.2/tntorch.egg-info/dependency_links.txt
+-rw-r--r--   0 rballester  (1000) rballester  (1000)        1 2021-02-05 18:23:50.000000 tntorch-1.1.2/tntorch.egg-info/not-zip-safe
+-rw-r--r--   0 rballester  (1000) rballester  (1000)       24 2024-05-23 11:48:40.000000 tntorch-1.1.2/tntorch.egg-info/requires.txt
+-rw-r--r--   0 rballester  (1000) rballester  (1000)        8 2024-05-23 11:48:40.000000 tntorch-1.1.2/tntorch.egg-info/top_level.txt
```

### Comparing `tntorch-1.1.1/LICENSE` & `tntorch-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/PKG-INFO` & `tntorch-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tntorch
-Version: 1.1.1
+Version: 1.1.2
 Summary: Tensor Network Learning with PyTorch
 Home-page: https://github.com/rballester/tntorch
 Author: Rafael Ballester-Ripoll
 Author-email: rafael.ballester@ie.edu
 License: LGPL
 Keywords: tntorch
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

### Comparing `tntorch-1.1.1/README.md` & `tntorch-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/setup.py` & `tntorch-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='tntorch',
-    version='1.1.1',
+    version='1.1.2',
     description="Tensor Network Learning with PyTorch",
     long_description="tntorch is a PyTorch-powered modeling and learning library using tensor networks. Features include basic and fancy indexing of tensors, broadcasting, assignment, etc.; tensor decomposition and arithmetics; adaptive sampling (cross-approximation); global optimization of tensors; sensitivity analysis; and more.",
     url='https://github.com/rballester/tntorch',
     author="Rafael Ballester-Ripoll",
     author_email='rafael.ballester@ie.edu',
     packages=[
         'tntorch',
```

### Comparing `tntorch-1.1.1/tests/test_automata.py` & `tntorch-1.1.2/tests/test_automata.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tests/test_cross.py` & `tntorch-1.1.2/tests/test_cross.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tests/test_gpu.py` & `tntorch-1.1.2/tests/test_gpu.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tests/test_indexing.py` & `tntorch-1.1.2/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tests/test_matrix.py` & `tntorch-1.1.2/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tests/test_ops.py` & `tntorch-1.1.2/tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tests/test_round.py` & `tntorch-1.1.2/tests/test_round.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tests/test_tensor.py` & `tntorch-1.1.2/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tests/test_tools.py` & `tntorch-1.1.2/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tntorch/anova.py` & `tntorch-1.1.2/tntorch/anova.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tntorch/autodiff.py` & `tntorch-1.1.2/tntorch/autodiff.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tntorch/automata.py` & `tntorch-1.1.2/tntorch/automata.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tntorch/create.py` & `tntorch-1.1.2/tntorch/create.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tntorch/cross.py` & `tntorch-1.1.2/tntorch/cross.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tntorch/derivatives.py` & `tntorch-1.1.2/tntorch/derivatives.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tntorch/interpolation.py` & `tntorch-1.1.2/tntorch/interpolation.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tntorch/logic.py` & `tntorch-1.1.2/tntorch/logic.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tntorch/matrix.py` & `tntorch-1.1.2/tntorch/matrix.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tntorch/maxvol.py` & `tntorch-1.1.2/tntorch/maxvol.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tntorch/metrics.py` & `tntorch-1.1.2/tntorch/metrics.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tntorch/ops.py` & `tntorch-1.1.2/tntorch/ops.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tntorch/round.py` & `tntorch-1.1.2/tntorch/round.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tntorch/tensor.py` & `tntorch-1.1.2/tntorch/tensor.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tntorch/tools.py` & `tntorch-1.1.2/tntorch/tools.py`

 * *Files identical despite different names*

### Comparing `tntorch-1.1.1/tntorch.egg-info/PKG-INFO` & `tntorch-1.1.2/tntorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tntorch
-Version: 1.1.1
+Version: 1.1.2
 Summary: Tensor Network Learning with PyTorch
 Home-page: https://github.com/rballester/tntorch
 Author: Rafael Ballester-Ripoll
 Author-email: rafael.ballester@ie.edu
 License: LGPL
 Keywords: tntorch
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

### Comparing `tntorch-1.1.1/tntorch.egg-info/SOURCES.txt` & `tntorch-1.1.2/tntorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

