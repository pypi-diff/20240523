# Comparing `tmp/horama-0.0.2.tar.gz` & `tmp/horama-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horama-0.0.2.tar", last modified: Tue Apr 23 02:45:23 2024, max compression
+gzip compressed data, was "horama-0.0.3.tar", last modified: Thu May 23 15:48:29 2024, max compression
```

## Comparing `horama-0.0.2.tar` & `horama-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:45:23.439537 horama-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:45:23.439537 horama-0.0.2/Horama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-23 02:45:23.000000 horama-0.0.2/Horama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-23 02:45:23.000000 horama-0.0.2/Horama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:45:23.000000 horama-0.0.2/Horama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-23 02:45:23.000000 horama-0.0.2/Horama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 02:45:23.000000 horama-0.0.2/Horama.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-23 02:45:15.000000 horama-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-23 02:45:23.439537 horama-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-23 02:45:15.000000 horama-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:45:23.439537 horama-0.0.2/horama/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-23 02:45:15.000000 horama-0.0.2/horama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-23 02:45:15.000000 horama-0.0.2/horama/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-23 02:45:15.000000 horama-0.0.2/horama/fourier_fv.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-23 02:45:15.000000 horama-0.0.2/horama/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-23 02:45:15.000000 horama-0.0.2/horama/maco_fv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-23 02:45:15.000000 horama-0.0.2/horama/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 02:45:23.439537 horama-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-23 02:45:15.000000 horama-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:48:29.992818 horama-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:48:29.992818 horama-0.0.3/Horama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-23 15:48:29.000000 horama-0.0.3/Horama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-23 15:48:29.000000 horama-0.0.3/Horama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:48:29.000000 horama-0.0.3/Horama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-23 15:48:29.000000 horama-0.0.3/Horama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 15:48:29.000000 horama-0.0.3/Horama.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-23 15:48:18.000000 horama-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-23 15:48:29.992818 horama-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-23 15:48:18.000000 horama-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:48:29.992818 horama-0.0.3/horama/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-23 15:48:18.000000 horama-0.0.3/horama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-23 15:48:18.000000 horama-0.0.3/horama/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-23 15:48:18.000000 horama-0.0.3/horama/fourier_fv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-23 15:48:18.000000 horama-0.0.3/horama/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-23 15:48:18.000000 horama-0.0.3/horama/maco_fv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-23 15:48:18.000000 horama-0.0.3/horama/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:48:29.992818 horama-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-23 15:48:18.000000 horama-0.0.3/setup.py
```

### Comparing `horama-0.0.2/Horama.egg-info/PKG-INFO` & `horama-0.0.3/Horama.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Horama
-Version: 0.0.2
+Version: 0.0.3
 Summary: Personal toolbox for experimenting with Feature Visualization
 Author: Thomas FEL, Thibaut BOISSIN, Victor BOUTIN, Agustin PICARD, Paul NOVELLO
 Author-email: thomas_fel@brown.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `horama-0.0.2/LICENSE` & `horama-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `horama-0.0.2/PKG-INFO` & `horama-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Horama
-Version: 0.0.2
+Version: 0.0.3
 Summary: Personal toolbox for experimenting with Feature Visualization
 Author: Thomas FEL, Thibaut BOISSIN, Victor BOUTIN, Agustin PICARD, Paul NOVELLO
 Author-email: thomas_fel@brown.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `horama-0.0.2/README.md` & `horama-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `horama-0.0.2/horama/common.py` & `horama-0.0.3/horama/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import torch
 from torchvision.ops import roi_align
 
-# tensor for color correlation svd square root
-color_correlation_svd_sqrt = torch.tensor(
-    [[0.56282854, 0.58447580, 0.58447580],
-     [0.19482528, 0.00000000, -0.19482528],
-     [0.04329450, -0.10823626, 0.06494176]],
-    dtype=torch.float32
-).cuda()
-
 def standardize(tensor):
     # standardizes the tensor to have 0 mean and unit variance
     tensor = tensor - torch.mean(tensor)
     tensor = tensor / (torch.std(tensor) + 1e-4)
     return tensor
 
-def recorrelate_colors(image):
+def recorrelate_colors(image, device):
+
+    # tensor for color correlation svd square root
+    color_correlation_svd_sqrt = torch.tensor(
+        [[0.56282854, 0.58447580, 0.58447580],
+         [0.19482528, 0.00000000, -0.19482528],
+         [0.04329450, -0.10823626, 0.06494176]],
+        dtype=torch.float32
+    ).to(device)
+
     # recorrelates the colors of the images
     assert len(image.shape) == 3
 
     permuted_image = image.permute(1, 2, 0).contiguous()
     flat_image = permuted_image.view(-1, 3)
 
     recorrelated_image = torch.matmul(flat_image, color_correlation_svd_sqrt)
```

### Comparing `horama-0.0.2/horama/fourier_fv.py` & `horama-0.0.3/horama/fourier_fv.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,24 +22,24 @@
 
 def init_olah_buffer(width, height, std=1.0):
     # initialize the Olah buffer with a random spectrum
     spectrum_shape = (3, width, height // 2 + 1)
     random_spectrum = torch.complex(torch.randn(spectrum_shape) * std, torch.randn(spectrum_shape) * std)
     return random_spectrum
 
-def fourier_preconditionner(spectrum, spectrum_scaler, values_range):
+def fourier_preconditionner(spectrum, spectrum_scaler, values_range, device):
     # precondition the Fourier spectrum and convert it to spatial domain
     assert spectrum.shape[0] == 3
 
     spectrum = standardize(spectrum)
     spectrum = spectrum * spectrum_scaler
 
     spatial_image = torch.fft.irfft2(spectrum)
     spatial_image = standardize(spatial_image)
-    color_recorrelated_image = recorrelate_colors(spatial_image)
+    color_recorrelated_image = recorrelate_colors(spatial_image, device)
 
     image = torch.sigmoid(color_recorrelated_image) * (values_range[1] - values_range[0]) + values_range[0]
     return image
 
 def fourier(objective_function, decay_power=1.5, total_steps=1000, learning_rate=1.0, image_size=1280, model_input_size=224,
          noise=0.05, values_range=(-2.5, 2.5), crops_per_iteration=6, box_size=(0.20, 0.25), device='cuda'):
     # perform the Olah optimization process
@@ -55,15 +55,15 @@
 
     optimizer = torch.optim.NAdam([spectrum], lr=learning_rate)
     transparency_accumulator = torch.zeros((3, image_size, image_size)).to(device)
 
     for step in tqdm(range(total_steps)):
         optimizer.zero_grad()
 
-        image = fourier_preconditionner(spectrum, spectrum_scaler, values_range)
+        image = fourier_preconditionner(spectrum, spectrum_scaler, values_range, device)
         loss, img = optimization_step(objective_function, image, box_size, noise, crops_per_iteration, model_input_size)
         loss.backward()
         transparency_accumulator += torch.abs(img.grad)
         optimizer.step()
 
-    final_image = fourier_preconditionner(spectrum, spectrum_scaler, values_range)
+    final_image = fourier_preconditionner(spectrum, spectrum_scaler, values_range, device)
     return final_image, transparency_accumulator
```

### Comparing `horama-0.0.2/horama/losses.py` & `horama-0.0.3/horama/losses.py`

 * *Files identical despite different names*

### Comparing `horama-0.0.2/horama/maco_fv.py` & `horama-0.0.3/horama/maco_fv.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                                      torch.sin(standardized_phase) * magnitude_template)
 
     # transform to spatial domain and standardize
     spatial_image = torch.fft.irfft2(complex_spectrum)
     spatial_image = standardize(spatial_image)
 
     # recorrelate colors and adjust value range
-    color_recorrelated_image = recorrelate_colors(spatial_image)
+    color_recorrelated_image = recorrelate_colors(spatial_image, device)
     final_image = torch.sigmoid(color_recorrelated_image) * (values_range[1] - values_range[0]) + values_range[0]
     return final_image
 
 def maco(objective_function, total_steps=1000, learning_rate=1.0, image_size=1280, model_input_size=224,
          noise=0.05, values_range=(-2.5, 2.5), crops_per_iteration=6, box_size=(0.20, 0.25), device='cuda'):
     # perform the maco optimization process
     assert values_range[1] >= values_range[0]
@@ -58,17 +58,17 @@
     transparency_accumulator = torch.zeros((3, image_size, image_size)).to(device)
 
     for step in tqdm(range(total_steps)):
         optimizer.zero_grad()
 
         # preprocess and compute loss
         img = maco_preconditioner(magnitude, phase, values_range)
-        loss, img = optimization_step(objective_function, img, box_size, noise, crops_per_iteration, model_input_size)
+        loss, img = optimization_step(objective_function, img, box_size, noise, crops_per_iteration, model_input_size, device)
 
         loss.backward()
         # get dy/dx to update transparency mask
         transparency_accumulator += torch.abs(img.grad)
         optimizer.step()
 
-    final_image = maco_preconditioner(magnitude, phase, values_range)
+    final_image = maco_preconditioner(magnitude, phase, values_range, device)
 
     return final_image, transparency_accumulator
```

### Comparing `horama-0.0.2/horama/plots.py` & `horama-0.0.3/horama/plots.py`

 * *Files identical despite different names*

### Comparing `horama-0.0.2/setup.py` & `horama-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as fh:
     README = fh.read()
 
 setup(
     name="Horama",
-    version="0.0.2",
+    version="0.0.3",
     description="Personal toolbox for experimenting with Feature Visualization",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Thomas FEL, Thibaut BOISSIN, Victor BOUTIN, Agustin PICARD, Paul NOVELLO",
     author_email="thomas_fel@brown.edu",
     license="MIT",
     install_requires=['numpy','matplotlib', 'torch', 'torchvision'],
```

