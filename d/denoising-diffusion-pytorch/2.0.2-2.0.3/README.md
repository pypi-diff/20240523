# Comparing `tmp/denoising_diffusion_pytorch-2.0.2.tar.gz` & `tmp/denoising_diffusion_pytorch-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising_diffusion_pytorch-2.0.2.tar", last modified: Wed May 22 14:59:03 2024, max compression
+gzip compressed data, was "denoising_diffusion_pytorch-2.0.3.tar", last modified: Wed May 22 21:39:33 2024, max compression
```

## Comparing `denoising_diffusion_pytorch-2.0.2.tar` & `denoising_diffusion_pytorch-2.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:59:03.027214 denoising_diffusion_pytorch-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-22 14:58:58.000000 denoising_diffusion_pytorch-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-22 14:59:03.027214 denoising_diffusion_pytorch-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11457 2024-05-22 14:58:58.000000 denoising_diffusion_pytorch-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:59:03.027214 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-22 14:58:58.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-22 14:58:58.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (127)    27964 2024-05-22 14:58:58.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-22 14:58:58.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    38426 2024-05-22 14:58:58.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    30051 2024-05-22 14:58:58.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-05-22 14:58:58.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-22 14:58:58.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/fid_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    35678 2024-05-22 14:58:58.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    18413 2024-05-22 14:58:58.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/karras_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)    18224 2024-05-22 14:58:58.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/karras_unet_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)    23187 2024-05-22 14:58:58.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/karras_unet_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-22 14:58:58.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    39828 2024-05-22 14:58:58.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/repaint.py
--rw-r--r--   0 runner    (1001) docker     (127)    21071 2024-05-22 14:58:58.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-22 14:58:58.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 14:58:58.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-22 14:58:58.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:59:03.027214 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-22 14:59:03.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-22 14:59:03.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:59:03.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-22 14:59:03.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 14:59:03.000000 denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 14:59:03.027214 denoising_diffusion_pytorch-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-22 14:58:58.000000 denoising_diffusion_pytorch-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:39:33.385388 denoising_diffusion_pytorch-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-22 21:39:33.385388 denoising_diffusion_pytorch-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11457 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:39:33.381389 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27964 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38426 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30051 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/fid_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35678 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18413 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/karras_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18224 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/karras_unet_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23187 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/karras_unet_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40310 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/repaint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21071 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:39:33.385388 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-22 21:39:33.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-22 21:39:33.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 21:39:33.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-22 21:39:33.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 21:39:33.000000 denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 21:39:33.385388 denoising_diffusion_pytorch-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-22 21:39:29.000000 denoising_diffusion_pytorch-2.0.3/setup.py
```

### Comparing `denoising_diffusion_pytorch-2.0.2/LICENSE` & `denoising_diffusion_pytorch-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.2/PKG-INFO` & `denoising_diffusion_pytorch-2.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 2.0.2
+Version: 2.0.3
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising_diffusion_pytorch-2.0.2/README.md` & `denoising_diffusion_pytorch-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/__init__.py` & `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/attend.py` & `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/fid_evaluation.py` & `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/fid_evaluation.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/karras_unet.py` & `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/karras_unet.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/karras_unet_1d.py` & `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/karras_unet_1d.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/karras_unet_3d.py` & `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/karras_unet_3d.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/repaint.py` & `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/repaint.py`

 * *Files 3% similar despite different names*

```diff
@@ -679,43 +679,49 @@
         batched_times = torch.full((b,), t, device = device, dtype = torch.long)
         model_mean, _, model_log_variance, x_start = self.p_mean_variance(x = x, t = batched_times, x_self_cond = x_self_cond, clip_denoised = True)
         noise = torch.randn_like(x) if t > 0 else 0. # no noise if t == 0
         pred_img = model_mean + (0.5 * model_log_variance).exp() * noise
         return pred_img, x_start
 
     @torch.inference_mode()
-    def p_sample_loop(self, shape, return_all_timesteps = False, gt=None, mask=None,resample = True,resample_iter = 10,resample_jump = 3):
+    def p_sample_loop(
+        self,
+        shape,
+        return_all_timesteps=False,
+        gt=None,
+        mask=None,
+        resample=True,
+        resample_iter=10,
+        resample_jump=3,
+        resample_every=50,
+    ):
         batch, device = shape[0], self.device
 
         img = torch.randn(shape, device = device)
         imgs = [img]
 
         x_start = None
 
         for t in tqdm(reversed(range(0, self.num_timesteps)), desc = 'sampling loop time step', total = self.num_timesteps):
             self_cond = x_start if self.self_condition else None
-            img, x_start = self.p_sample(img, t, self_cond, gt, mask)
+            img, x_start = self.p_sample(x=img, t=t, x_self_cond=self_cond, gt=gt, mask=mask)
             imgs.append(img)
 
-        if resample is True and t == 0:
-            #Jump back for resample_jump timesteps and resample_iter times
-
-            for iter in tqdm(range(resample_iter), desc = 'resample loop', total = resample_iter):
-                t = resample_jump
-
-                beta = self.betas[t]
-                img = torch.sqrt(1 - beta) * img + torch.sqrt(beta) * torch.randn_like(img)
-                for j in reversed(range(0, resample_jump)):
-                    img, x_start = self.p_sample(img, t,gt,mask)
-            imgs.append(img)
-        
-
+            # Resampling loop: line 9 of Algorithm 1 in https://arxiv.org/pdf/2201.09865
+            if resample is True and (t > 0) and (t % resample_every == 0):
+                # Jump back for resample_jump timesteps and resample_iter times
+                for iter in tqdm(range(resample_iter), desc = 'resample loop', total = resample_iter):
+                    t = resample_jump
+                    beta = self.betas[t]
+                    img = torch.sqrt(1 - beta) * img + torch.sqrt(beta) * torch.randn_like(img)
+                    for j in reversed(range(0, resample_jump)):
+                        img, x_start = self.p_sample(x=img, t=t, gt=gt, mask=mask)
+                imgs.append(img)
 
         ret = img if not return_all_timesteps else torch.stack(imgs, dim = 1)
-
         ret = self.unnormalize(ret)
         return ret
 
     @torch.inference_mode()
     def ddim_sample(self, shape, return_all_timesteps = False):
         batch, device, total_timesteps, sampling_timesteps, eta, objective = shape[0], self.device, self.num_timesteps, self.sampling_timesteps, self.ddim_sampling_eta, self.objective
 
@@ -754,19 +760,37 @@
 
         ret = img if not return_all_timesteps else torch.stack(imgs, dim = 1)
 
         ret = self.unnormalize(ret)
         return ret
 
     @torch.inference_mode()
-    def sample(self, batch_size = 16, return_all_timesteps = False, gt=None, mask=None,resample = True,resample_iter = 10,resample_jump = 10):
+    def sample(
+        self,
+        batch_size=16,
+        return_all_timesteps=False,
+        gt=None,
+        mask=None,
+        resample=True,
+        resample_iter=10,
+        resample_jump=10,
+        resample_every=50,
+    ):
         (h, w), channels = self.image_size, self.channels
         batch_size = mask.shape[0] if mask is not None else batch_size
-        sample_fn = self.p_sample_loop
-        return sample_fn((batch_size, channels, h, w), return_all_timesteps = return_all_timesteps, gt=gt, mask=mask,resample=resample,resample_iter=resample_iter,resample_jump=resample_jump)
+        return self.p_sample_loop(
+            shape=(batch_size, channels, h, w),
+            return_all_timesteps=return_all_timesteps,
+            gt=gt,
+            mask=mask,
+            resample=resample,
+            resample_iter=resample_iter,
+            resample_jump=resample_jump,
+            resample_every=resample_every,
+        )
 
     @torch.inference_mode()
     def interpolate(self, x1, x2, t = None, lam = 0.5):
         b, *_, device = *x1.shape, x1.device
         t = default(t, self.num_timesteps - 1)
 
         assert x1.shape == x2.shape
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 2.0.2
+Version: 2.0.3
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising_diffusion_pytorch-2.0.2/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising_diffusion_pytorch-2.0.3/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.2/setup.py` & `denoising_diffusion_pytorch-2.0.3/setup.py`

 * *Files identical despite different names*

