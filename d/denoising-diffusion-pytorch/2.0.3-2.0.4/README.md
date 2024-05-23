# Comparing `tmp/denoising_diffusion_pytorch-2.0.3.tar.gz` & `tmp/denoising_diffusion_pytorch-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising_diffusion_pytorch-2.0.3.tar", last modified: Wed May 22 21:39:33 2024, max compression
+gzip compressed data, was "denoising_diffusion_pytorch-2.0.4.tar", last modified: Thu May 23 17:01:59 2024, max compression
```

## Comparing `denoising_diffusion_pytorch-2.0.3.tar` & `denoising_diffusion_pytorch-2.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:39:33.385388 denoising_diffusion_pytorch-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-22 21:39:33.385388 denoising_diffusion_pytorch-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11457 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:39:33.381389 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (127)    27964 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    38426 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    30051 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/fid_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    35678 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    18413 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/karras_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)    18224 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/karras_unet_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)    23187 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/karras_unet_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    40310 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/repaint.py
--rw-r--r--   0 runner    (1001) docker     (127)    21071 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:39:33.385388 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-22 21:39:33.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-22 21:39:33.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 21:39:33.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-22 21:39:33.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 21:39:33.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 21:39:33.385388 denoising_diffusion_pytorch-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:01:59.028934 denoising_diffusion_pytorch-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-23 17:01:55.000000 denoising_diffusion_pytorch-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-23 17:01:59.028934 denoising_diffusion_pytorch-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11457 2024-05-23 17:01:55.000000 denoising_diffusion_pytorch-2.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:01:59.024934 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-23 17:01:55.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-23 17:01:55.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27964 2024-05-23 17:01:55.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-23 17:01:55.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38426 2024-05-23 17:01:55.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30051 2024-05-23 17:01:55.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-05-23 17:01:55.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-23 17:01:55.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/fid_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35670 2024-05-23 17:01:55.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18413 2024-05-23 17:01:55.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/karras_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18224 2024-05-23 17:01:55.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/karras_unet_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23187 2024-05-23 17:01:55.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/karras_unet_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-23 17:01:55.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40310 2024-05-23 17:01:55.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/repaint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21071 2024-05-23 17:01:55.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-23 17:01:55.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-23 17:01:55.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-23 17:01:55.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:01:59.024934 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-23 17:01:59.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-23 17:01:59.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 17:01:59.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-23 17:01:59.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 17:01:59.000000 denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 17:01:59.028934 denoising_diffusion_pytorch-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-23 17:01:55.000000 denoising_diffusion_pytorch-2.0.4/setup.py
```

### Comparing `denoising_diffusion_pytorch-2.0.3/LICENSE` & `denoising_diffusion_pytorch-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.3/PKG-INFO` & `denoising_diffusion_pytorch-2.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 2.0.3
+Version: 2.0.4
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising_diffusion_pytorch-2.0.3/README.md` & `denoising_diffusion_pytorch-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/__init__.py` & `denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/attend.py` & `denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/fid_evaluation.py` & `denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/fid_evaluation.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 
 # building block modules
 
 class Block(nn.Module):
     def __init__(self, dim, dim_out):
         super().__init__()
         self.proj = nn.Conv2d(dim, dim_out, 3, padding = 1)
-        self.norm = RMSNorm(groups, dim_out)
+        self.norm = RMSNorm(dim_out)
         self.act = nn.SiLU()
 
     def forward(self, x, scale_shift = None):
         x = self.proj(x)
         x = self.norm(x)
 
         if exists(scale_shift):
```

### Comparing `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/karras_unet.py` & `denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/karras_unet.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/karras_unet_1d.py` & `denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/karras_unet_1d.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/karras_unet_3d.py` & `denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/karras_unet_3d.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/repaint.py` & `denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/repaint.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 2.0.3
+Version: 2.0.4
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising_diffusion_pytorch-2.0.4/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.3/setup.py` & `denoising_diffusion_pytorch-2.0.4/setup.py`

 * *Files identical despite different names*

