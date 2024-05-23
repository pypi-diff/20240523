# Comparing `tmp/keymorph-1.0.0.tar.gz` & `tmp/keymorph-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keymorph-1.0.0.tar", last modified: Fri May 10 15:29:53 2024, max compression
+gzip compressed data, was "keymorph-1.0.1.tar", last modified: Thu May 23 14:14:45 2024, max compression
```

## Comparing `keymorph-1.0.0.tar` & `keymorph-1.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 alw4013  (1158043) wmcstaff   (538)        0 2024-05-10 15:29:53.770180 keymorph-1.0.0/
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     1068 2023-10-17 18:20:30.000000 keymorph-1.0.0/LICENSE
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    14400 2024-05-10 15:29:53.770180 keymorph-1.0.0/PKG-INFO
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    13786 2024-05-10 15:28:05.000000 keymorph-1.0.0/README.md
-drwxr-xr-x   0 alw4013  (1158043) wmcstaff   (538)        0 2024-05-10 15:29:53.730180 keymorph-1.0.0/keymorph/
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)       50 2024-05-10 15:29:17.000000 keymorph-1.0.0/keymorph/__init__.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    10299 2024-05-10 14:19:13.000000 keymorph-1.0.0/keymorph/augmentation.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    20976 2024-04-20 17:29:13.000000 keymorph-1.0.0/keymorph/keypoint_aligners.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     5327 2024-04-18 18:04:36.000000 keymorph-1.0.0/keymorph/layers.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    17717 2024-04-17 14:01:55.000000 keymorph-1.0.0/keymorph/loss_ops.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    19960 2024-04-20 17:42:34.000000 keymorph-1.0.0/keymorph/model.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     1345 2024-05-10 14:17:23.000000 keymorph-1.0.0/keymorph/net.py
-drwxr-xr-x   0 alw4013  (1158043) wmcstaff   (538)        0 2024-05-10 15:29:53.766180 keymorph-1.0.0/keymorph/unet3d/
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)        0 2024-04-17 14:01:55.000000 keymorph-1.0.0/keymorph/unet3d/__init__.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    20881 2024-04-20 17:23:30.000000 keymorph-1.0.0/keymorph/unet3d/buildingblocks.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)      885 2024-04-17 14:01:55.000000 keymorph-1.0.0/keymorph/unet3d/config.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    13344 2024-04-17 14:01:55.000000 keymorph-1.0.0/keymorph/unet3d/losses.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    16873 2024-04-17 14:01:55.000000 keymorph-1.0.0/keymorph/unet3d/metrics.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    14982 2024-04-19 20:00:16.000000 keymorph-1.0.0/keymorph/unet3d/model.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    11935 2024-04-17 14:01:55.000000 keymorph-1.0.0/keymorph/unet3d/predictor.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     3992 2024-04-17 14:01:55.000000 keymorph-1.0.0/keymorph/unet3d/se.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     3890 2024-04-17 14:01:55.000000 keymorph-1.0.0/keymorph/unet3d/seg_metrics.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    16068 2024-04-17 14:01:55.000000 keymorph-1.0.0/keymorph/unet3d/trainer.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     9784 2024-04-17 14:01:55.000000 keymorph-1.0.0/keymorph/unet3d/utils.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    11273 2024-05-09 19:20:24.000000 keymorph-1.0.0/keymorph/utils.py
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    12921 2024-05-02 16:12:24.000000 keymorph-1.0.0/keymorph/viz_tools.py
-drwxr-xr-x   0 alw4013  (1158043) wmcstaff   (538)        0 2024-05-10 15:29:53.742180 keymorph-1.0.0/keymorph.egg-info/
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    14400 2024-05-10 15:29:53.000000 keymorph-1.0.0/keymorph.egg-info/PKG-INFO
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)      689 2024-05-10 15:29:53.000000 keymorph-1.0.0/keymorph.egg-info/SOURCES.txt
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)        1 2024-05-10 15:29:53.000000 keymorph-1.0.0/keymorph.egg-info/dependency_links.txt
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)      161 2024-05-10 15:29:53.000000 keymorph-1.0.0/keymorph.egg-info/requires.txt
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)        9 2024-05-10 15:29:53.000000 keymorph-1.0.0/keymorph.egg-info/top_level.txt
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)       38 2024-05-10 15:29:53.770180 keymorph-1.0.0/setup.cfg
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     1413 2024-05-10 15:29:10.000000 keymorph-1.0.0/setup.py
-drwxr-xr-x   0 alw4013  (1158043) wmcstaff   (538)        0 2024-05-10 15:29:53.766180 keymorph-1.0.0/tests/
--rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    13696 2024-04-17 14:01:56.000000 keymorph-1.0.0/tests/test.py
+drwxr-xr-x   0 alw4013  (1158043) wmcstaff   (538)        0 2024-05-23 14:14:45.769303 keymorph-1.0.1/
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     1068 2023-10-17 18:20:30.000000 keymorph-1.0.1/LICENSE
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    15759 2024-05-23 14:14:45.769303 keymorph-1.0.1/PKG-INFO
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    15145 2024-05-21 13:58:38.000000 keymorph-1.0.1/README.md
+drwxr-xr-x   0 alw4013  (1158043) wmcstaff   (538)        0 2024-05-23 14:14:45.741303 keymorph-1.0.1/keymorph/
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)       50 2024-05-23 14:13:37.000000 keymorph-1.0.1/keymorph/__init__.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    10299 2024-05-10 14:19:13.000000 keymorph-1.0.1/keymorph/augmentation.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    20976 2024-04-20 17:29:13.000000 keymorph-1.0.1/keymorph/keypoint_aligners.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     5327 2024-04-18 18:04:36.000000 keymorph-1.0.1/keymorph/layers.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    17717 2024-04-17 14:01:55.000000 keymorph-1.0.1/keymorph/loss_ops.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    19960 2024-05-15 02:30:56.000000 keymorph-1.0.1/keymorph/model.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     1345 2024-05-10 14:17:23.000000 keymorph-1.0.1/keymorph/net.py
+drwxr-xr-x   0 alw4013  (1158043) wmcstaff   (538)        0 2024-05-23 14:14:45.765303 keymorph-1.0.1/keymorph/unet3d/
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)        0 2024-04-17 14:01:55.000000 keymorph-1.0.1/keymorph/unet3d/__init__.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    20881 2024-04-20 17:23:30.000000 keymorph-1.0.1/keymorph/unet3d/buildingblocks.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)      885 2024-04-17 14:01:55.000000 keymorph-1.0.1/keymorph/unet3d/config.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    13344 2024-04-17 14:01:55.000000 keymorph-1.0.1/keymorph/unet3d/losses.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    16873 2024-04-17 14:01:55.000000 keymorph-1.0.1/keymorph/unet3d/metrics.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    14982 2024-04-19 20:00:16.000000 keymorph-1.0.1/keymorph/unet3d/model.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    11935 2024-04-17 14:01:55.000000 keymorph-1.0.1/keymorph/unet3d/predictor.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     3992 2024-04-17 14:01:55.000000 keymorph-1.0.1/keymorph/unet3d/se.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     3890 2024-04-17 14:01:55.000000 keymorph-1.0.1/keymorph/unet3d/seg_metrics.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    16068 2024-04-17 14:01:55.000000 keymorph-1.0.1/keymorph/unet3d/trainer.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     9784 2024-04-17 14:01:55.000000 keymorph-1.0.1/keymorph/unet3d/utils.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    11303 2024-05-23 14:09:35.000000 keymorph-1.0.1/keymorph/utils.py
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    12970 2024-05-23 13:53:56.000000 keymorph-1.0.1/keymorph/viz_tools.py
+drwxr-xr-x   0 alw4013  (1158043) wmcstaff   (538)        0 2024-05-23 14:14:45.749303 keymorph-1.0.1/keymorph.egg-info/
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    15759 2024-05-23 14:14:45.000000 keymorph-1.0.1/keymorph.egg-info/PKG-INFO
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)      689 2024-05-23 14:14:45.000000 keymorph-1.0.1/keymorph.egg-info/SOURCES.txt
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)        1 2024-05-23 14:14:45.000000 keymorph-1.0.1/keymorph.egg-info/dependency_links.txt
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)      161 2024-05-23 14:14:45.000000 keymorph-1.0.1/keymorph.egg-info/requires.txt
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)        9 2024-05-23 14:14:45.000000 keymorph-1.0.1/keymorph.egg-info/top_level.txt
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)       38 2024-05-23 14:14:45.769303 keymorph-1.0.1/setup.cfg
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)     1413 2024-05-23 14:13:09.000000 keymorph-1.0.1/setup.py
+drwxr-xr-x   0 alw4013  (1158043) wmcstaff   (538)        0 2024-05-23 14:14:45.769303 keymorph-1.0.1/tests/
+-rw-r--r--   0 alw4013  (1158043) wmcstaff   (538)    13696 2024-04-17 14:01:56.000000 keymorph-1.0.1/tests/test.py
```

### Comparing `keymorph-1.0.0/LICENSE` & `keymorph-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.0/PKG-INFO` & `keymorph-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,88 +1,97 @@
 Metadata-Version: 2.1
 Name: keymorph
-Version: 1.0.0
+Version: 1.0.1
 Summary: KeyMorph is a deep learning-based image registration framework that relies on automatically extracting corresponding keypoints.
 Home-page: https://github.com/alanqrwang/keymorph
 Author: Alan Q. Wang
 Author-email: alanqrwang@gmail.com
 License: MIT
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# KeyMorph: Robust Multi-modal Registration via Keypoint Detection
+# KeyMorph: Robust and Flexible Multi-modal Registration via Keypoint Detection
 
 KeyMorph is a deep learning-based image registration framework that relies on automatically extracting corresponding keypoints. 
+It supports unimodal/multimodal pairwise and groupwise registration using rigid, affine, or nonlinear transformations.
+
+This repository contains the code for KeyMorph, as well as example scripts for training your own KeyMorph model.
+As an example, it uses data from the [IXI dataset](https://brain-development.org/ixi-dataset/) to train and evaluate the model.
+
+[BrainMorph](https://github.com/alanqrwang/brainmorph) is a foundation model based on the KeyMorph framework, trained on over 100,000 brain MR images at full resolution (256x256x256).
+The model is robust to normal and diseased brains, a variety of MRI modalities, and skullstripped and non-skullstripped images.
+Check out the dedicated repository for the latest updates and models!
 
 ## Updates
-- [May 2024] Released full set of foundation models on [Box](https://cornell.box.com/s/2mw4ey1u7waqrpylnxf49rck7u3nnr7i). Detailed instructions under "Foundation model".
-- [Apr 2024] Released foundational model of KeyMorph for brain MRIs which is trained on over 100K images at full resolution (256^3). Instructions under "Foundation model".
+- [May 2024] [BrainMorph](https://github.com/alanqrwang/brainmorph) has been moved to its own dedicated repository. See the repository for the latest updates and models.
+- [May 2024] [BrainMorph](https://github.com/alanqrwang/brainmorph) is released, a foundational keypoint model based on KeyMorph for robust and flexible brain MRI registration!
 - [Dec 2023] [Journal paper](https://arxiv.org/abs/2304.09941) extension of MIDL paper published in Medical Image Analysis. Instructions under "IXI-trained, half-resolution models".
 - [Feb 2022] [Conference paper](https://openreview.net/forum?id=OrNzjERFybh) published in MIDL 2021.
 
 ## Installation
 
 We recommend using pip to install keymorph:
 ```bash
 pip install keymorph
 ```
 
 To run scripts and/or contribute to keymorph, you should install from source:
 ```bash
-git clone git@github.com:alanqrwang/keymorph.git
+git clone https://github.com/alanqrwang/keymorph.git
 cd keymorph
 pip install -e .
 ```
 
 ### Requirements
 The keymorph package depends on the following requirements:
 
 - numpy>=1.19.1
 - ogb>=1.2.6
 - outdated>=0.2.0
 - pandas>=1.1.0
-- ogb>=1.2.6
 - pytz>=2020.4
 - torch>=1.7.0
 - torchvision>=0.8.2
 - scikit-learn>=0.20.0
 - scipy>=1.5.4
 - torchio>=0.19.6
 
 Running `pip install keymorph` or `pip install -e .` will automatically check for and install all of these requirements.
 
 ## Downloading Trained Weights
-You can find all full-resolution trained weights [here](https://cornell.box.com/s/2mw4ey1u7waqrpylnxf49rck7u3nnr7i).
+You can find all full-resolution, BrainMorph trained weights [here](https://cornell.box.com/s/2mw4ey1u7waqrpylnxf49rck7u3nnr7i).
 Half-resolution trained weights are under [Releases](https://github.com/alanqrwang/keymorph/releases).
-Download them and put them in the `./weights/` folder.
+Download your preferred model(s) and put them in the folder specified by `--weights_dir` in the commands below.
 
 ## Registering brain volumes 
-### Foundation model
-The foundation model is trained on over 100,000 brain MR images at full resolution (256x256x256). 
+### BrainMorph
+Warning: Please see the [BrainMorph repository](https://github.com/alanqrwang/brainmorph) for the latest updates and models! This is a legacy version of the code and is not guaranteed to be maintained.
+
+BrainMorph is trained on over 100,000 brain MR images at full resolution (256x256x256). 
 The script will automatically min-max normalize the images and resample to 1mm isotropic resolution.
 
 `--num_keypoints` and `num_levels_for_unet` will determine which model will be used to perform the registration.
 Make sure the corresponding weights are present in `--weights_dir`.
 `--num_keypoints` can be set to `128, 256, 512` and `--num_levels_for_unet` can be set to `4, 5, 6, 7`, respectively (corresponding to 'S', 'M', 'L', 'H' in the paper).
 
 To register a single pair of volumes:
 ```
 python scripts/register.py \
     --num_keypoints 256 \
     --num_levels_for_unet 4 \
     --weights_dir ./weights/ \
-    --moving ./example_data/images/IXI_000001_0000.nii.gz \
-    --fixed ./example_data/images/IXI_000002_0000.nii.gz \
-    --moving_seg ./example_data/labels/IXI_000001_0000.nii.gz \
-    --fixed_seg ./example_data/labels/IXI_000002_0000.nii.gz \
+    --moving ./example_data/img_m/IXI_000001_0000.nii.gz \
+    --fixed ./example_data/img_m/IXI_000002_0000.nii.gz \
+    --moving_seg ./example_data/seg_m/IXI_000001_0000.nii.gz \
+    --fixed_seg ./example_data/seg_m/IXI_000002_0000.nii.gz \
     --list_of_aligns rigid affine tps_1 \
     --list_of_metrics mse harddice \
     --save_eval_to_disk \
     --visualize
 ```
 
 Description of other important flags:
@@ -91,57 +100,74 @@
 + `--list_of_aligns` specifies the types of alignment to perform. Options are `rigid`, `affine` and `tps_<lambda>` (TPS with hyperparameter value equal to lambda). lambda=0 corresponds to exact keypoint alignment. lambda=10 is very similar to affine.
 + `--list_of_metrics` specifies the metrics to report. Options are `mse`, `harddice`, `softdice`, `hausd`, `jdstd`, `jdlessthan0`. To compute Dice scores and surface distances, `--moving_seg` and `--fixed_seg` must be provided.
 + `--save_eval_to_disk` saves all outputs to disk. The default location is `./register_output/`.
 + `--visualize` plots a matplotlib figure of moving, fixed, and registered images overlaid with corresponding points.
 
 You can also replace filenames with directories to register all images in the directory.
 Note that the script expects corresponding image and segmentation pairs to have the same filename.
+```bash
+python scripts/register.py \
+    --num_keypoints 256 \
+    --num_levels_for_unet 4 \
+    --weights_dir ./weights/ \
+    --moving ./example_data/img_m/ \
+    --fixed ./example_data/img_m/ \
+    --moving_seg ./example_data/seg_m/ \
+    --fixed_seg ./example_data/seg_m/ \
+    --list_of_aligns rigid affine tps_1 \
+    --list_of_metrics mse harddice \
+    --save_eval_to_disk \
+    --visualize
 ```
+
+### Groupwise registration
+```bash
 python scripts/register.py \
+    --groupwise \
     --num_keypoints 256 \
     --num_levels_for_unet 4 \
     --weights_dir ./weights/ \
-    --moving ./example_data/images/ \
-    --fixed ./example_data/images/ \
-    --moving_seg ./example_data/labels/ \
-    --fixed_seg ./example_data/labels/ \
+    --moving ./example_data/ \
+    --fixed ./example_data/ \
+    --moving_seg ./example_data/ \
+    --fixed_seg ./example_data/ \
     --list_of_aligns rigid affine tps_1 \
     --list_of_metrics mse harddice \
     --save_eval_to_disk \
     --visualize
 ```
 
 
 
 ### IXI-trained, half-resolution models
 All other model weights are trained on half-resolution (128x128x128) on the (smaller) IXI dataset. 
 The script will automatically min-max normalize the images.
 To register two volumes with our best-performing model:
 
-```
+```bash
 python scripts/register.py \
     --half_resolution \
     --num_keypoints 512 \
     --backbone conv \
-    --moving ./example_data/images_half/IXI_001_128x128x128.nii.gz \
-    --fixed ./example_data/images_half/IXI_002_128x128x128.nii.gz \
+    --moving ./example_data_half/img_m/IXI_001_128x128x128.nii.gz \
+    --fixed ./example_data_half/img_m/IXI_002_128x128x128.nii.gz \
     --load_path ./weights/numkey512_tps0_dice.4760.h5 \
-    --moving_seg ./example_data/labels_half/IXI_001_128x128x128.nii.gz \
-    --fixed_seg ./example_data/labels_half/IXI_002_128x128x128.nii.gz \
+    --moving_seg ./example_data_half/seg_m/IXI_001_128x128x128.nii.gz \
+    --fixed_seg ./example_data_half/seg_m/IXI_002_128x128x128.nii.gz \
     --list_of_aligns affine tps_1 \
     --list_of_metrics mse harddice \
     --save_eval_to_disk \
     --visualize
 ```
 
 ## TLDR in code
 The crux of the code is in the `forward()` function in `keymorph/model.py`, which performs one forward pass through the entire KeyMorph pipeline.
 
 Here's a pseudo-code version of the function:
-```
+```python
 def forward(img_f, img_m, seg_f, seg_m, network, optimizer, kp_aligner):
     '''Forward pass for one mini-batch step. 
     Variables with (_f, _m, _a) denotes (fixed, moving, aligned).
     
     Args:
         img_f, img_m: Fixed and moving intensity image (bs, 1, l, w, h)
         seg_f, seg_m: Fixed and moving one-hot segmentation map (bs, num_classes, l, w, h)
@@ -171,21 +197,17 @@
     loss.backward()
     optimizer.step()
 ```
 The `network` variable is a CNN with center-of-mass layer which extracts keypoints from the input images.
 The `kp_aligner` variable is a keypoint alignment module. It has a function `grid_from_points()` which returns a flow-field grid encoding the transformation to perform on the moving image. The transformation can either be rigid, affine, or nonlinear (TPS).
 
 ## Training KeyMorph
-Use `scripts/run.py` to train KeyMorph.
-<!-- Some example bash commands are provided in `bash_scripts/`. -->
+Use `scripts/run.py` with `--run_mode train` to train KeyMorph.
 
-I'm in the process of updating the code to make it more user-friendly, and will update this repository soon.
-In the meantime, feel free to open an issue if you have any training questions.
-
-<!-- We use the weights from the pretraining step to initialize our model. 
+We use the weights from the pretraining step to initialize our model.
 Our pretraining weights are provided in [Releases](https://github.com/evanmy/keymorph/releases/tag/weights).
 
 The `--num_keypoints <num_key>` flag specifies the number of keypoints to extract per image as `<num_key>`.
 For all commands, optionally add the `--use_wandb` flag to log results to Weights & Biases.
 
 This repository supports several variants of training KeyMorph.
 Here's a overview of the variants:
@@ -206,61 +228,84 @@
 To specify tps, set `--kp_align_method tps` and the lmbda value `--tps_lmbda 0`.
 
 ### Example commands
 **Affine, Unsupervised**
 
 To train unsupervised KeyMorph with affine transformation and 128 keypoints, use `mse` as the loss function:
 
-```
-python run.py --num_keypoints 128 --kp_align_method affine --loss_fn mse \
-                --data_dir ./data/centered_IXI/ \
-                --load_path ./weights/numkey128_pretrain.2500.h5
-```
-
-For unsupervised KeyMorph, optionally add `--kpconsistency_coeff` to optimize keypoint consistency across modalities for same subject:
-
-```
-python run.py --num_keypoints 128 --kp_align_method affine --loss_fn mse --kpconsistency_coeff 10 \
-                --data_dir ./data/centered_IXI/ \
-                --load_path ./weights/numkey128_pretrain.2500.h5
-```
+```bash
+python scripts/run.py \
+    --run_mode train \
+    --num_keypoints 128 \
+    --loss_fn mse \
+    --transform_type affine \
+    --data_dir ./data/centered_IXI/ \
+    --load_path ./weights/numkey128_pretrain.2500.h5
+```
+
+<!-- For unsupervised KeyMorph, optionally add `--kpconsistency_coeff` to optimize keypoint consistency across modalities for same subject: -->
+
+<!-- ```bash
+python scripts/run.py \
+    --run_mode train \
+    --num_keypoints 128 \
+    --kp_align_method affine \
+    --loss_fn mse \
+    --kpconsistency_coeff 10 \
+    --data_dir ./data/centered_IXI/ \
+    --load_path ./weights/numkey128_pretrain.2500.h5
+``` -->
 
 **Affine, Supervised**
 
 To train supervised KeyMorph, use `dice` as the loss function:
 
-```
-python run.py --num_keypoints 128 --kp_align_method affine --loss_fn dice --mix_modalities \
-                --data_dir ./data/centered_IXI/ \
-                --load_path ./weights/numkey128_pretrain.2500.h5
+```bash
+python scripts/run.py \
+    --run_mode train \
+    --num_keypoints 128 \
+    --kp_align_method affine \
+    --loss_fn dice \
+    --mix_modalities \
+    --data_dir ./data/centered_IXI/ \
+    --load_path ./weights/numkey128_pretrain.2500.h5
 ```
 
 Note that the `--mix_modalities` flag allows fixed and moving images to be of different modalities during training. This should not be set for unsupervised training, which uses MSE as the loss function.
 
 **Nonlinear thin-plate-spline (TPS)**
 
 To train the TPS variant of KeyMorph which allows for nonlinear registrations, specify `tps` as the keypoint alignment method and specify the tps lambda value: 
 
 ```
-python run.py --num_keypoints 128 --kp_align_method tps --tps_lmbda 0 --loss_fn dice \
-                --data_dir ./data/centered_IXI/ \
-                --load_path ./weights/numkey128_pretrain.2500.h5
+python scripts/run.py \
+    --run_mode train \
+    --num_keypoints 128 \
+    --kp_align_method tps \
+    --tps_lmbda 0 \
+    --loss_fn dice \
+    --data_dir ./data/centered_IXI/ \
+    --load_path ./weights/numkey128_pretrain.2500.h5
 ```
 
 The code also supports sampling lambda according to some distribution (`uniform`, `lognormal`, `loguniform`). For example, to sample from the `loguniform` distribution during training:
 
 ```
-python run.py --num_keypoints 128 --kp_align_method tps --tps_lmbda loguniform --loss_fn dice \
-                --data_dir ./data/centered_IXI/ \
-                --load_path ./weights/numkey128_pretrain.2500.h5
+python scripts/run.py \
+    --num_keypoints 128 \
+    --kp_align_method tps \
+    --tps_lmbda loguniform \
+    --loss_fn dice \
+    --data_dir ./data/centered_IXI/ \
+    --load_path ./weights/numkey128_pretrain.2500.h5
 ```
 
-Note that supervised/unsupervised variants can be run similarly to affine, as described above. -->
+Note that supervised/unsupervised variants can be run similarly to affine, as described above. 
 
-<!-- ## Step-by-step guide for reproducing our results
+## Step-by-step guide for reproducing our results
 
 ### Dataset 
 [A] Scripts in `./notebooks/[A] Download Data` will download the IXI data and perform some basic preprocessing
 
 [B] Once the data is downloaded `./notebooks/[B] Brain extraction` can be used to extract remove non-brain tissue. 
 
 [C] Once the brain has been extracted, we center the brain using `./notebooks/[C] Centering`. During training, we randomly introduce affine augmentation to the dataset. This ensure that the brain stays within the volume given the affine augmentation we introduce. It also helps during the pretraining step of our algorithm.
@@ -268,15 +313,15 @@
 ### Pretraining KeyMorph
 
 This step helps with the convergence of our model. We pick 1 subject and random points within the brain of that subject. We then introduce affine transformation to the subject brain and same transformation to the keypoints. In other words, this is a self-supervised task in where the network learns to predict the keypoints on a brain under random affine transformation. We found that initializing our model with these weights helps with the training.
 
 To pretrain, run:
  
 ```
-python pretraining.py --num_keypoints 128 --data_dir ./data/centered_IXI/ 
+python scripts/run.py --run_mode pretrain --num_keypoints 128 --data_dir ./data/centered_IXI/ 
 ```
 
 ### Training KeyMorph
 Follow instructions for "Training KeyMorph" above, depending on the variant you want.
 
 ### Evaluating KeyMorph
 To evaluate on the test set, simply add the `--eval` flag to any of the above commands. For example, for affine, unsupervised KeyMorph evaluation:
@@ -287,15 +332,15 @@
 ```
 
 Evaluation proceeds by looping through all test augmentations in `list_of_test_augs`, all test modality pairs in `list_of_test_mods`, and all pairs of volumes in the test set.
 Set `--save_preds` flag to save all outputs to disk.
 
 **Automatic Delineation/Segmentation of the Brain**
 
-For evaluation, we use [SynthSeg](https://github.com/BBillot/SynthSeg) to automatically segment different brain regions. Follow their repository for detailed intruction on how to use the model. -->
+For evaluation, we use [SynthSeg](https://github.com/BBillot/SynthSeg) to automatically segment different brain regions. Follow their repository for detailed intruction on how to use the model. 
 
 ## Issues
 This repository is being actively maintained. Feel free to open an issue for any problems or questions.
 
 ## Legacy code
 For a legacy version of the code, see our [legacy branch](https://github.com/alanqrwang/keymorph/tree/legacy).
```

### Comparing `keymorph-1.0.0/README.md` & `keymorph-1.0.1/keymorph.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,72 +1,97 @@
-# KeyMorph: Robust Multi-modal Registration via Keypoint Detection
+Metadata-Version: 2.1
+Name: keymorph
+Version: 1.0.1
+Summary: KeyMorph is a deep learning-based image registration framework that relies on automatically extracting corresponding keypoints.
+Home-page: https://github.com/alanqrwang/keymorph
+Author: Alan Q. Wang
+Author-email: alanqrwang@gmail.com
+License: MIT
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# KeyMorph: Robust and Flexible Multi-modal Registration via Keypoint Detection
 
 KeyMorph is a deep learning-based image registration framework that relies on automatically extracting corresponding keypoints. 
+It supports unimodal/multimodal pairwise and groupwise registration using rigid, affine, or nonlinear transformations.
+
+This repository contains the code for KeyMorph, as well as example scripts for training your own KeyMorph model.
+As an example, it uses data from the [IXI dataset](https://brain-development.org/ixi-dataset/) to train and evaluate the model.
+
+[BrainMorph](https://github.com/alanqrwang/brainmorph) is a foundation model based on the KeyMorph framework, trained on over 100,000 brain MR images at full resolution (256x256x256).
+The model is robust to normal and diseased brains, a variety of MRI modalities, and skullstripped and non-skullstripped images.
+Check out the dedicated repository for the latest updates and models!
 
 ## Updates
-- [May 2024] Released full set of foundation models on [Box](https://cornell.box.com/s/2mw4ey1u7waqrpylnxf49rck7u3nnr7i). Detailed instructions under "Foundation model".
-- [Apr 2024] Released foundational model of KeyMorph for brain MRIs which is trained on over 100K images at full resolution (256^3). Instructions under "Foundation model".
+- [May 2024] [BrainMorph](https://github.com/alanqrwang/brainmorph) has been moved to its own dedicated repository. See the repository for the latest updates and models.
+- [May 2024] [BrainMorph](https://github.com/alanqrwang/brainmorph) is released, a foundational keypoint model based on KeyMorph for robust and flexible brain MRI registration!
 - [Dec 2023] [Journal paper](https://arxiv.org/abs/2304.09941) extension of MIDL paper published in Medical Image Analysis. Instructions under "IXI-trained, half-resolution models".
 - [Feb 2022] [Conference paper](https://openreview.net/forum?id=OrNzjERFybh) published in MIDL 2021.
 
 ## Installation
 
 We recommend using pip to install keymorph:
 ```bash
 pip install keymorph
 ```
 
 To run scripts and/or contribute to keymorph, you should install from source:
 ```bash
-git clone git@github.com:alanqrwang/keymorph.git
+git clone https://github.com/alanqrwang/keymorph.git
 cd keymorph
 pip install -e .
 ```
 
 ### Requirements
 The keymorph package depends on the following requirements:
 
 - numpy>=1.19.1
 - ogb>=1.2.6
 - outdated>=0.2.0
 - pandas>=1.1.0
-- ogb>=1.2.6
 - pytz>=2020.4
 - torch>=1.7.0
 - torchvision>=0.8.2
 - scikit-learn>=0.20.0
 - scipy>=1.5.4
 - torchio>=0.19.6
 
 Running `pip install keymorph` or `pip install -e .` will automatically check for and install all of these requirements.
 
 ## Downloading Trained Weights
-You can find all full-resolution trained weights [here](https://cornell.box.com/s/2mw4ey1u7waqrpylnxf49rck7u3nnr7i).
+You can find all full-resolution, BrainMorph trained weights [here](https://cornell.box.com/s/2mw4ey1u7waqrpylnxf49rck7u3nnr7i).
 Half-resolution trained weights are under [Releases](https://github.com/alanqrwang/keymorph/releases).
-Download them and put them in the `./weights/` folder.
+Download your preferred model(s) and put them in the folder specified by `--weights_dir` in the commands below.
 
 ## Registering brain volumes 
-### Foundation model
-The foundation model is trained on over 100,000 brain MR images at full resolution (256x256x256). 
+### BrainMorph
+Warning: Please see the [BrainMorph repository](https://github.com/alanqrwang/brainmorph) for the latest updates and models! This is a legacy version of the code and is not guaranteed to be maintained.
+
+BrainMorph is trained on over 100,000 brain MR images at full resolution (256x256x256). 
 The script will automatically min-max normalize the images and resample to 1mm isotropic resolution.
 
 `--num_keypoints` and `num_levels_for_unet` will determine which model will be used to perform the registration.
 Make sure the corresponding weights are present in `--weights_dir`.
 `--num_keypoints` can be set to `128, 256, 512` and `--num_levels_for_unet` can be set to `4, 5, 6, 7`, respectively (corresponding to 'S', 'M', 'L', 'H' in the paper).
 
 To register a single pair of volumes:
 ```
 python scripts/register.py \
     --num_keypoints 256 \
     --num_levels_for_unet 4 \
     --weights_dir ./weights/ \
-    --moving ./example_data/images/IXI_000001_0000.nii.gz \
-    --fixed ./example_data/images/IXI_000002_0000.nii.gz \
-    --moving_seg ./example_data/labels/IXI_000001_0000.nii.gz \
-    --fixed_seg ./example_data/labels/IXI_000002_0000.nii.gz \
+    --moving ./example_data/img_m/IXI_000001_0000.nii.gz \
+    --fixed ./example_data/img_m/IXI_000002_0000.nii.gz \
+    --moving_seg ./example_data/seg_m/IXI_000001_0000.nii.gz \
+    --fixed_seg ./example_data/seg_m/IXI_000002_0000.nii.gz \
     --list_of_aligns rigid affine tps_1 \
     --list_of_metrics mse harddice \
     --save_eval_to_disk \
     --visualize
 ```
 
 Description of other important flags:
@@ -75,57 +100,74 @@
 + `--list_of_aligns` specifies the types of alignment to perform. Options are `rigid`, `affine` and `tps_<lambda>` (TPS with hyperparameter value equal to lambda). lambda=0 corresponds to exact keypoint alignment. lambda=10 is very similar to affine.
 + `--list_of_metrics` specifies the metrics to report. Options are `mse`, `harddice`, `softdice`, `hausd`, `jdstd`, `jdlessthan0`. To compute Dice scores and surface distances, `--moving_seg` and `--fixed_seg` must be provided.
 + `--save_eval_to_disk` saves all outputs to disk. The default location is `./register_output/`.
 + `--visualize` plots a matplotlib figure of moving, fixed, and registered images overlaid with corresponding points.
 
 You can also replace filenames with directories to register all images in the directory.
 Note that the script expects corresponding image and segmentation pairs to have the same filename.
+```bash
+python scripts/register.py \
+    --num_keypoints 256 \
+    --num_levels_for_unet 4 \
+    --weights_dir ./weights/ \
+    --moving ./example_data/img_m/ \
+    --fixed ./example_data/img_m/ \
+    --moving_seg ./example_data/seg_m/ \
+    --fixed_seg ./example_data/seg_m/ \
+    --list_of_aligns rigid affine tps_1 \
+    --list_of_metrics mse harddice \
+    --save_eval_to_disk \
+    --visualize
 ```
+
+### Groupwise registration
+```bash
 python scripts/register.py \
+    --groupwise \
     --num_keypoints 256 \
     --num_levels_for_unet 4 \
     --weights_dir ./weights/ \
-    --moving ./example_data/images/ \
-    --fixed ./example_data/images/ \
-    --moving_seg ./example_data/labels/ \
-    --fixed_seg ./example_data/labels/ \
+    --moving ./example_data/ \
+    --fixed ./example_data/ \
+    --moving_seg ./example_data/ \
+    --fixed_seg ./example_data/ \
     --list_of_aligns rigid affine tps_1 \
     --list_of_metrics mse harddice \
     --save_eval_to_disk \
     --visualize
 ```
 
 
 
 ### IXI-trained, half-resolution models
 All other model weights are trained on half-resolution (128x128x128) on the (smaller) IXI dataset. 
 The script will automatically min-max normalize the images.
 To register two volumes with our best-performing model:
 
-```
+```bash
 python scripts/register.py \
     --half_resolution \
     --num_keypoints 512 \
     --backbone conv \
-    --moving ./example_data/images_half/IXI_001_128x128x128.nii.gz \
-    --fixed ./example_data/images_half/IXI_002_128x128x128.nii.gz \
+    --moving ./example_data_half/img_m/IXI_001_128x128x128.nii.gz \
+    --fixed ./example_data_half/img_m/IXI_002_128x128x128.nii.gz \
     --load_path ./weights/numkey512_tps0_dice.4760.h5 \
-    --moving_seg ./example_data/labels_half/IXI_001_128x128x128.nii.gz \
-    --fixed_seg ./example_data/labels_half/IXI_002_128x128x128.nii.gz \
+    --moving_seg ./example_data_half/seg_m/IXI_001_128x128x128.nii.gz \
+    --fixed_seg ./example_data_half/seg_m/IXI_002_128x128x128.nii.gz \
     --list_of_aligns affine tps_1 \
     --list_of_metrics mse harddice \
     --save_eval_to_disk \
     --visualize
 ```
 
 ## TLDR in code
 The crux of the code is in the `forward()` function in `keymorph/model.py`, which performs one forward pass through the entire KeyMorph pipeline.
 
 Here's a pseudo-code version of the function:
-```
+```python
 def forward(img_f, img_m, seg_f, seg_m, network, optimizer, kp_aligner):
     '''Forward pass for one mini-batch step. 
     Variables with (_f, _m, _a) denotes (fixed, moving, aligned).
     
     Args:
         img_f, img_m: Fixed and moving intensity image (bs, 1, l, w, h)
         seg_f, seg_m: Fixed and moving one-hot segmentation map (bs, num_classes, l, w, h)
@@ -155,21 +197,17 @@
     loss.backward()
     optimizer.step()
 ```
 The `network` variable is a CNN with center-of-mass layer which extracts keypoints from the input images.
 The `kp_aligner` variable is a keypoint alignment module. It has a function `grid_from_points()` which returns a flow-field grid encoding the transformation to perform on the moving image. The transformation can either be rigid, affine, or nonlinear (TPS).
 
 ## Training KeyMorph
-Use `scripts/run.py` to train KeyMorph.
-<!-- Some example bash commands are provided in `bash_scripts/`. -->
+Use `scripts/run.py` with `--run_mode train` to train KeyMorph.
 
-I'm in the process of updating the code to make it more user-friendly, and will update this repository soon.
-In the meantime, feel free to open an issue if you have any training questions.
-
-<!-- We use the weights from the pretraining step to initialize our model. 
+We use the weights from the pretraining step to initialize our model.
 Our pretraining weights are provided in [Releases](https://github.com/evanmy/keymorph/releases/tag/weights).
 
 The `--num_keypoints <num_key>` flag specifies the number of keypoints to extract per image as `<num_key>`.
 For all commands, optionally add the `--use_wandb` flag to log results to Weights & Biases.
 
 This repository supports several variants of training KeyMorph.
 Here's a overview of the variants:
@@ -190,61 +228,84 @@
 To specify tps, set `--kp_align_method tps` and the lmbda value `--tps_lmbda 0`.
 
 ### Example commands
 **Affine, Unsupervised**
 
 To train unsupervised KeyMorph with affine transformation and 128 keypoints, use `mse` as the loss function:
 
-```
-python run.py --num_keypoints 128 --kp_align_method affine --loss_fn mse \
-                --data_dir ./data/centered_IXI/ \
-                --load_path ./weights/numkey128_pretrain.2500.h5
-```
-
-For unsupervised KeyMorph, optionally add `--kpconsistency_coeff` to optimize keypoint consistency across modalities for same subject:
-
-```
-python run.py --num_keypoints 128 --kp_align_method affine --loss_fn mse --kpconsistency_coeff 10 \
-                --data_dir ./data/centered_IXI/ \
-                --load_path ./weights/numkey128_pretrain.2500.h5
-```
+```bash
+python scripts/run.py \
+    --run_mode train \
+    --num_keypoints 128 \
+    --loss_fn mse \
+    --transform_type affine \
+    --data_dir ./data/centered_IXI/ \
+    --load_path ./weights/numkey128_pretrain.2500.h5
+```
+
+<!-- For unsupervised KeyMorph, optionally add `--kpconsistency_coeff` to optimize keypoint consistency across modalities for same subject: -->
+
+<!-- ```bash
+python scripts/run.py \
+    --run_mode train \
+    --num_keypoints 128 \
+    --kp_align_method affine \
+    --loss_fn mse \
+    --kpconsistency_coeff 10 \
+    --data_dir ./data/centered_IXI/ \
+    --load_path ./weights/numkey128_pretrain.2500.h5
+``` -->
 
 **Affine, Supervised**
 
 To train supervised KeyMorph, use `dice` as the loss function:
 
-```
-python run.py --num_keypoints 128 --kp_align_method affine --loss_fn dice --mix_modalities \
-                --data_dir ./data/centered_IXI/ \
-                --load_path ./weights/numkey128_pretrain.2500.h5
+```bash
+python scripts/run.py \
+    --run_mode train \
+    --num_keypoints 128 \
+    --kp_align_method affine \
+    --loss_fn dice \
+    --mix_modalities \
+    --data_dir ./data/centered_IXI/ \
+    --load_path ./weights/numkey128_pretrain.2500.h5
 ```
 
 Note that the `--mix_modalities` flag allows fixed and moving images to be of different modalities during training. This should not be set for unsupervised training, which uses MSE as the loss function.
 
 **Nonlinear thin-plate-spline (TPS)**
 
 To train the TPS variant of KeyMorph which allows for nonlinear registrations, specify `tps` as the keypoint alignment method and specify the tps lambda value: 
 
 ```
-python run.py --num_keypoints 128 --kp_align_method tps --tps_lmbda 0 --loss_fn dice \
-                --data_dir ./data/centered_IXI/ \
-                --load_path ./weights/numkey128_pretrain.2500.h5
+python scripts/run.py \
+    --run_mode train \
+    --num_keypoints 128 \
+    --kp_align_method tps \
+    --tps_lmbda 0 \
+    --loss_fn dice \
+    --data_dir ./data/centered_IXI/ \
+    --load_path ./weights/numkey128_pretrain.2500.h5
 ```
 
 The code also supports sampling lambda according to some distribution (`uniform`, `lognormal`, `loguniform`). For example, to sample from the `loguniform` distribution during training:
 
 ```
-python run.py --num_keypoints 128 --kp_align_method tps --tps_lmbda loguniform --loss_fn dice \
-                --data_dir ./data/centered_IXI/ \
-                --load_path ./weights/numkey128_pretrain.2500.h5
+python scripts/run.py \
+    --num_keypoints 128 \
+    --kp_align_method tps \
+    --tps_lmbda loguniform \
+    --loss_fn dice \
+    --data_dir ./data/centered_IXI/ \
+    --load_path ./weights/numkey128_pretrain.2500.h5
 ```
 
-Note that supervised/unsupervised variants can be run similarly to affine, as described above. -->
+Note that supervised/unsupervised variants can be run similarly to affine, as described above. 
 
-<!-- ## Step-by-step guide for reproducing our results
+## Step-by-step guide for reproducing our results
 
 ### Dataset 
 [A] Scripts in `./notebooks/[A] Download Data` will download the IXI data and perform some basic preprocessing
 
 [B] Once the data is downloaded `./notebooks/[B] Brain extraction` can be used to extract remove non-brain tissue. 
 
 [C] Once the brain has been extracted, we center the brain using `./notebooks/[C] Centering`. During training, we randomly introduce affine augmentation to the dataset. This ensure that the brain stays within the volume given the affine augmentation we introduce. It also helps during the pretraining step of our algorithm.
@@ -252,15 +313,15 @@
 ### Pretraining KeyMorph
 
 This step helps with the convergence of our model. We pick 1 subject and random points within the brain of that subject. We then introduce affine transformation to the subject brain and same transformation to the keypoints. In other words, this is a self-supervised task in where the network learns to predict the keypoints on a brain under random affine transformation. We found that initializing our model with these weights helps with the training.
 
 To pretrain, run:
  
 ```
-python pretraining.py --num_keypoints 128 --data_dir ./data/centered_IXI/ 
+python scripts/run.py --run_mode pretrain --num_keypoints 128 --data_dir ./data/centered_IXI/ 
 ```
 
 ### Training KeyMorph
 Follow instructions for "Training KeyMorph" above, depending on the variant you want.
 
 ### Evaluating KeyMorph
 To evaluate on the test set, simply add the `--eval` flag to any of the above commands. For example, for affine, unsupervised KeyMorph evaluation:
@@ -271,15 +332,15 @@
 ```
 
 Evaluation proceeds by looping through all test augmentations in `list_of_test_augs`, all test modality pairs in `list_of_test_mods`, and all pairs of volumes in the test set.
 Set `--save_preds` flag to save all outputs to disk.
 
 **Automatic Delineation/Segmentation of the Brain**
 
-For evaluation, we use [SynthSeg](https://github.com/BBillot/SynthSeg) to automatically segment different brain regions. Follow their repository for detailed intruction on how to use the model. -->
+For evaluation, we use [SynthSeg](https://github.com/BBillot/SynthSeg) to automatically segment different brain regions. Follow their repository for detailed intruction on how to use the model. 
 
 ## Issues
 This repository is being actively maintained. Feel free to open an issue for any problems or questions.
 
 ## Legacy code
 For a legacy version of the code, see our [legacy branch](https://github.com/alanqrwang/keymorph/tree/legacy).
```

### Comparing `keymorph-1.0.0/keymorph/augmentation.py` & `keymorph-1.0.1/keymorph/augmentation.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.0/keymorph/keypoint_aligners.py` & `keymorph-1.0.1/keymorph/keypoint_aligners.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.0/keymorph/layers.py` & `keymorph-1.0.1/keymorph/layers.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.0/keymorph/loss_ops.py` & `keymorph-1.0.1/keymorph/loss_ops.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.0/keymorph/model.py` & `keymorph-1.0.1/keymorph/model.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.0/keymorph/net.py` & `keymorph-1.0.1/keymorph/net.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.0/keymorph/unet3d/buildingblocks.py` & `keymorph-1.0.1/keymorph/unet3d/buildingblocks.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.0/keymorph/unet3d/config.py` & `keymorph-1.0.1/keymorph/unet3d/config.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.0/keymorph/unet3d/losses.py` & `keymorph-1.0.1/keymorph/unet3d/losses.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.0/keymorph/unet3d/metrics.py` & `keymorph-1.0.1/keymorph/unet3d/metrics.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.0/keymorph/unet3d/model.py` & `keymorph-1.0.1/keymorph/unet3d/model.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.0/keymorph/unet3d/predictor.py` & `keymorph-1.0.1/keymorph/unet3d/predictor.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.0/keymorph/unet3d/se.py` & `keymorph-1.0.1/keymorph/unet3d/se.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.0/keymorph/unet3d/seg_metrics.py` & `keymorph-1.0.1/keymorph/unet3d/seg_metrics.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.0/keymorph/unet3d/trainer.py` & `keymorph-1.0.1/keymorph/unet3d/trainer.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.0/keymorph/unet3d/utils.py` & `keymorph-1.0.1/keymorph/unet3d/utils.py`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.0/keymorph/utils.py` & `keymorph-1.0.1/keymorph/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import re
 import torch
 import torch.nn.functional as F
 import math
 import numpy as np
 from collections import defaultdict
-import wandb
 import os
 import argparse
 import json
 
-# import itk
+try:
+    import wandb
+except ImportError as e:
+    pass
 
 
 def align_img(grid, x, mode="bilinear"):
     return F.grid_sample(
         x,
         grid=grid,
         mode=mode,
```

### Comparing `keymorph-1.0.0/keymorph/viz_tools.py` & `keymorph-1.0.1/keymorph/viz_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -143,36 +143,39 @@
     all_weights=None,
     projection=False,
     center_slices=(128, 128, 128),
     slab_thickness=10,
     axes=None,
     rotate_90_deg=0,
     img_dims=(256, 256, 256),
+    markers=(".", "x"),
 ):
     """
     Plots 3 orthogonal slices of a 3D image and overlays points on them.
 
     img: (H, W, D) image
-    all_points: (N, 3) or (B, N, 3) array of points.
+    all_points: (N, 3) or (1, N, 3) or (2, N, 3) array of points.
         Points can be defined on:
          1. the Pytorch grid, i.e. in [-1, 1]
          2. the image grid, e.g. in [0, 256]
         The code converts Pytorch grids to image grids by internally checking if
-    all_weights: (N,) or (B, N) array of weights
+    all_weights: (N,) or (1, N) or (2, N) array of weights
     """
 
     def normalize(data):
         return (data - np.min(data)) / (np.max(data) - np.min(data))
 
     plot_img = True if img is not None else None
     plot_points = True if all_points is not None else None
 
     if plot_points:
         if len(all_points.shape) == 2:
             all_points = all_points[None]
+        if isinstance(markers, str):
+            markers = (markers,)
 
         # If points are in [-1, 1], convert to image coordinates
         if np.all(all_points >= -1) or np.all(all_points <= 1):
             print("Converting points from [-1, 1] to image coordinates")
             all_points = (all_points + 1) / 2 * img_dims[-1]
         if np.any(all_points < 0):
             raise ValueError("Points must be non-negative")
@@ -205,15 +208,14 @@
             img_yz = np.rot90(img_yz, k=rotate_90_deg)
 
         axes[0].imshow(img_xy, cmap="gray", vmin=vmin, vmax=vmax)
         axes[1].imshow(img_xz, cmap="gray", vmin=vmin, vmax=vmax)
         axes[2].imshow(img_yz, cmap="gray", vmin=vmin, vmax=vmax)
 
     if plot_points:
-        markers = [".", "+", "x"]
         for points, weights, marker in zip(all_points, all_weights, markers):
             points_xy, depth_xy = points[:, 1:], points[:, 0]
             points_xz, depth_xz = (
                 np.stack((points[:, 0], points[:, 2]), axis=-1),
                 points[:, 1],
             )
             points_yz, depth_yz = points[:, :2], points[:, 2]
@@ -294,14 +296,15 @@
     img_a,
     points_m=None,
     points_f=None,
     points_a=None,
     weights=None,
     suptitle=None,
     save_path=None,
+    **kwargs,
 ):
     """
     Moved, aligned, and fixed should be volumes with 3 dimensions.
     Points should be normalized in [-1,1].
 
     Convention is that (-1, -1, -1) is on the top left, front-most
     corner. x-values get bigger to the right, y-values get bigger
@@ -324,29 +327,29 @@
     fig, axes = plt.subplots(3, 3, figsize=(16, 16))
 
     imshow_img_and_points_3d(
         img_m,
         points_m,
         weights,
         axes=(axes[0, 0], axes[1, 0], axes[2, 0]),
-        img_dims=(256, 256, 256),
+        **kwargs,
     )
     imshow_img_and_points_3d(
         img_f,
         points_f,
         weights,
         axes=(axes[0, 1], axes[1, 1], axes[2, 1]),
-        img_dims=(256, 256, 256),
+        **kwargs,
     )
     imshow_img_and_points_3d(
         img_a,
         points_af,
         weights,
         axes=(axes[0, 2], axes[1, 2], axes[2, 2]),
-        img_dims=(256, 256, 256),
+        **kwargs,
     )
 
     axes[0, 0].set_title("Moving")
     axes[0, 1].set_title("Fixed")
     axes[0, 2].set_title("Warped")
     if suptitle:
         fig.suptitle(suptitle)
```

### Comparing `keymorph-1.0.0/keymorph.egg-info/PKG-INFO` & `keymorph-1.0.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,88 +1,81 @@
-Metadata-Version: 2.1
-Name: keymorph
-Version: 1.0.0
-Summary: KeyMorph is a deep learning-based image registration framework that relies on automatically extracting corresponding keypoints.
-Home-page: https://github.com/alanqrwang/keymorph
-Author: Alan Q. Wang
-Author-email: alanqrwang@gmail.com
-License: MIT
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# KeyMorph: Robust Multi-modal Registration via Keypoint Detection
+# KeyMorph: Robust and Flexible Multi-modal Registration via Keypoint Detection
 
 KeyMorph is a deep learning-based image registration framework that relies on automatically extracting corresponding keypoints. 
+It supports unimodal/multimodal pairwise and groupwise registration using rigid, affine, or nonlinear transformations.
+
+This repository contains the code for KeyMorph, as well as example scripts for training your own KeyMorph model.
+As an example, it uses data from the [IXI dataset](https://brain-development.org/ixi-dataset/) to train and evaluate the model.
+
+[BrainMorph](https://github.com/alanqrwang/brainmorph) is a foundation model based on the KeyMorph framework, trained on over 100,000 brain MR images at full resolution (256x256x256).
+The model is robust to normal and diseased brains, a variety of MRI modalities, and skullstripped and non-skullstripped images.
+Check out the dedicated repository for the latest updates and models!
 
 ## Updates
-- [May 2024] Released full set of foundation models on [Box](https://cornell.box.com/s/2mw4ey1u7waqrpylnxf49rck7u3nnr7i). Detailed instructions under "Foundation model".
-- [Apr 2024] Released foundational model of KeyMorph for brain MRIs which is trained on over 100K images at full resolution (256^3). Instructions under "Foundation model".
+- [May 2024] [BrainMorph](https://github.com/alanqrwang/brainmorph) has been moved to its own dedicated repository. See the repository for the latest updates and models.
+- [May 2024] [BrainMorph](https://github.com/alanqrwang/brainmorph) is released, a foundational keypoint model based on KeyMorph for robust and flexible brain MRI registration!
 - [Dec 2023] [Journal paper](https://arxiv.org/abs/2304.09941) extension of MIDL paper published in Medical Image Analysis. Instructions under "IXI-trained, half-resolution models".
 - [Feb 2022] [Conference paper](https://openreview.net/forum?id=OrNzjERFybh) published in MIDL 2021.
 
 ## Installation
 
 We recommend using pip to install keymorph:
 ```bash
 pip install keymorph
 ```
 
 To run scripts and/or contribute to keymorph, you should install from source:
 ```bash
-git clone git@github.com:alanqrwang/keymorph.git
+git clone https://github.com/alanqrwang/keymorph.git
 cd keymorph
 pip install -e .
 ```
 
 ### Requirements
 The keymorph package depends on the following requirements:
 
 - numpy>=1.19.1
 - ogb>=1.2.6
 - outdated>=0.2.0
 - pandas>=1.1.0
-- ogb>=1.2.6
 - pytz>=2020.4
 - torch>=1.7.0
 - torchvision>=0.8.2
 - scikit-learn>=0.20.0
 - scipy>=1.5.4
 - torchio>=0.19.6
 
 Running `pip install keymorph` or `pip install -e .` will automatically check for and install all of these requirements.
 
 ## Downloading Trained Weights
-You can find all full-resolution trained weights [here](https://cornell.box.com/s/2mw4ey1u7waqrpylnxf49rck7u3nnr7i).
+You can find all full-resolution, BrainMorph trained weights [here](https://cornell.box.com/s/2mw4ey1u7waqrpylnxf49rck7u3nnr7i).
 Half-resolution trained weights are under [Releases](https://github.com/alanqrwang/keymorph/releases).
-Download them and put them in the `./weights/` folder.
+Download your preferred model(s) and put them in the folder specified by `--weights_dir` in the commands below.
 
 ## Registering brain volumes 
-### Foundation model
-The foundation model is trained on over 100,000 brain MR images at full resolution (256x256x256). 
+### BrainMorph
+Warning: Please see the [BrainMorph repository](https://github.com/alanqrwang/brainmorph) for the latest updates and models! This is a legacy version of the code and is not guaranteed to be maintained.
+
+BrainMorph is trained on over 100,000 brain MR images at full resolution (256x256x256). 
 The script will automatically min-max normalize the images and resample to 1mm isotropic resolution.
 
 `--num_keypoints` and `num_levels_for_unet` will determine which model will be used to perform the registration.
 Make sure the corresponding weights are present in `--weights_dir`.
 `--num_keypoints` can be set to `128, 256, 512` and `--num_levels_for_unet` can be set to `4, 5, 6, 7`, respectively (corresponding to 'S', 'M', 'L', 'H' in the paper).
 
 To register a single pair of volumes:
 ```
 python scripts/register.py \
     --num_keypoints 256 \
     --num_levels_for_unet 4 \
     --weights_dir ./weights/ \
-    --moving ./example_data/images/IXI_000001_0000.nii.gz \
-    --fixed ./example_data/images/IXI_000002_0000.nii.gz \
-    --moving_seg ./example_data/labels/IXI_000001_0000.nii.gz \
-    --fixed_seg ./example_data/labels/IXI_000002_0000.nii.gz \
+    --moving ./example_data/img_m/IXI_000001_0000.nii.gz \
+    --fixed ./example_data/img_m/IXI_000002_0000.nii.gz \
+    --moving_seg ./example_data/seg_m/IXI_000001_0000.nii.gz \
+    --fixed_seg ./example_data/seg_m/IXI_000002_0000.nii.gz \
     --list_of_aligns rigid affine tps_1 \
     --list_of_metrics mse harddice \
     --save_eval_to_disk \
     --visualize
 ```
 
 Description of other important flags:
@@ -91,57 +84,74 @@
 + `--list_of_aligns` specifies the types of alignment to perform. Options are `rigid`, `affine` and `tps_<lambda>` (TPS with hyperparameter value equal to lambda). lambda=0 corresponds to exact keypoint alignment. lambda=10 is very similar to affine.
 + `--list_of_metrics` specifies the metrics to report. Options are `mse`, `harddice`, `softdice`, `hausd`, `jdstd`, `jdlessthan0`. To compute Dice scores and surface distances, `--moving_seg` and `--fixed_seg` must be provided.
 + `--save_eval_to_disk` saves all outputs to disk. The default location is `./register_output/`.
 + `--visualize` plots a matplotlib figure of moving, fixed, and registered images overlaid with corresponding points.
 
 You can also replace filenames with directories to register all images in the directory.
 Note that the script expects corresponding image and segmentation pairs to have the same filename.
+```bash
+python scripts/register.py \
+    --num_keypoints 256 \
+    --num_levels_for_unet 4 \
+    --weights_dir ./weights/ \
+    --moving ./example_data/img_m/ \
+    --fixed ./example_data/img_m/ \
+    --moving_seg ./example_data/seg_m/ \
+    --fixed_seg ./example_data/seg_m/ \
+    --list_of_aligns rigid affine tps_1 \
+    --list_of_metrics mse harddice \
+    --save_eval_to_disk \
+    --visualize
 ```
+
+### Groupwise registration
+```bash
 python scripts/register.py \
+    --groupwise \
     --num_keypoints 256 \
     --num_levels_for_unet 4 \
     --weights_dir ./weights/ \
-    --moving ./example_data/images/ \
-    --fixed ./example_data/images/ \
-    --moving_seg ./example_data/labels/ \
-    --fixed_seg ./example_data/labels/ \
+    --moving ./example_data/ \
+    --fixed ./example_data/ \
+    --moving_seg ./example_data/ \
+    --fixed_seg ./example_data/ \
     --list_of_aligns rigid affine tps_1 \
     --list_of_metrics mse harddice \
     --save_eval_to_disk \
     --visualize
 ```
 
 
 
 ### IXI-trained, half-resolution models
 All other model weights are trained on half-resolution (128x128x128) on the (smaller) IXI dataset. 
 The script will automatically min-max normalize the images.
 To register two volumes with our best-performing model:
 
-```
+```bash
 python scripts/register.py \
     --half_resolution \
     --num_keypoints 512 \
     --backbone conv \
-    --moving ./example_data/images_half/IXI_001_128x128x128.nii.gz \
-    --fixed ./example_data/images_half/IXI_002_128x128x128.nii.gz \
+    --moving ./example_data_half/img_m/IXI_001_128x128x128.nii.gz \
+    --fixed ./example_data_half/img_m/IXI_002_128x128x128.nii.gz \
     --load_path ./weights/numkey512_tps0_dice.4760.h5 \
-    --moving_seg ./example_data/labels_half/IXI_001_128x128x128.nii.gz \
-    --fixed_seg ./example_data/labels_half/IXI_002_128x128x128.nii.gz \
+    --moving_seg ./example_data_half/seg_m/IXI_001_128x128x128.nii.gz \
+    --fixed_seg ./example_data_half/seg_m/IXI_002_128x128x128.nii.gz \
     --list_of_aligns affine tps_1 \
     --list_of_metrics mse harddice \
     --save_eval_to_disk \
     --visualize
 ```
 
 ## TLDR in code
 The crux of the code is in the `forward()` function in `keymorph/model.py`, which performs one forward pass through the entire KeyMorph pipeline.
 
 Here's a pseudo-code version of the function:
-```
+```python
 def forward(img_f, img_m, seg_f, seg_m, network, optimizer, kp_aligner):
     '''Forward pass for one mini-batch step. 
     Variables with (_f, _m, _a) denotes (fixed, moving, aligned).
     
     Args:
         img_f, img_m: Fixed and moving intensity image (bs, 1, l, w, h)
         seg_f, seg_m: Fixed and moving one-hot segmentation map (bs, num_classes, l, w, h)
@@ -171,21 +181,17 @@
     loss.backward()
     optimizer.step()
 ```
 The `network` variable is a CNN with center-of-mass layer which extracts keypoints from the input images.
 The `kp_aligner` variable is a keypoint alignment module. It has a function `grid_from_points()` which returns a flow-field grid encoding the transformation to perform on the moving image. The transformation can either be rigid, affine, or nonlinear (TPS).
 
 ## Training KeyMorph
-Use `scripts/run.py` to train KeyMorph.
-<!-- Some example bash commands are provided in `bash_scripts/`. -->
+Use `scripts/run.py` with `--run_mode train` to train KeyMorph.
 
-I'm in the process of updating the code to make it more user-friendly, and will update this repository soon.
-In the meantime, feel free to open an issue if you have any training questions.
-
-<!-- We use the weights from the pretraining step to initialize our model. 
+We use the weights from the pretraining step to initialize our model.
 Our pretraining weights are provided in [Releases](https://github.com/evanmy/keymorph/releases/tag/weights).
 
 The `--num_keypoints <num_key>` flag specifies the number of keypoints to extract per image as `<num_key>`.
 For all commands, optionally add the `--use_wandb` flag to log results to Weights & Biases.
 
 This repository supports several variants of training KeyMorph.
 Here's a overview of the variants:
@@ -206,61 +212,84 @@
 To specify tps, set `--kp_align_method tps` and the lmbda value `--tps_lmbda 0`.
 
 ### Example commands
 **Affine, Unsupervised**
 
 To train unsupervised KeyMorph with affine transformation and 128 keypoints, use `mse` as the loss function:
 
-```
-python run.py --num_keypoints 128 --kp_align_method affine --loss_fn mse \
-                --data_dir ./data/centered_IXI/ \
-                --load_path ./weights/numkey128_pretrain.2500.h5
-```
-
-For unsupervised KeyMorph, optionally add `--kpconsistency_coeff` to optimize keypoint consistency across modalities for same subject:
-
-```
-python run.py --num_keypoints 128 --kp_align_method affine --loss_fn mse --kpconsistency_coeff 10 \
-                --data_dir ./data/centered_IXI/ \
-                --load_path ./weights/numkey128_pretrain.2500.h5
-```
+```bash
+python scripts/run.py \
+    --run_mode train \
+    --num_keypoints 128 \
+    --loss_fn mse \
+    --transform_type affine \
+    --data_dir ./data/centered_IXI/ \
+    --load_path ./weights/numkey128_pretrain.2500.h5
+```
+
+<!-- For unsupervised KeyMorph, optionally add `--kpconsistency_coeff` to optimize keypoint consistency across modalities for same subject: -->
+
+<!-- ```bash
+python scripts/run.py \
+    --run_mode train \
+    --num_keypoints 128 \
+    --kp_align_method affine \
+    --loss_fn mse \
+    --kpconsistency_coeff 10 \
+    --data_dir ./data/centered_IXI/ \
+    --load_path ./weights/numkey128_pretrain.2500.h5
+``` -->
 
 **Affine, Supervised**
 
 To train supervised KeyMorph, use `dice` as the loss function:
 
-```
-python run.py --num_keypoints 128 --kp_align_method affine --loss_fn dice --mix_modalities \
-                --data_dir ./data/centered_IXI/ \
-                --load_path ./weights/numkey128_pretrain.2500.h5
+```bash
+python scripts/run.py \
+    --run_mode train \
+    --num_keypoints 128 \
+    --kp_align_method affine \
+    --loss_fn dice \
+    --mix_modalities \
+    --data_dir ./data/centered_IXI/ \
+    --load_path ./weights/numkey128_pretrain.2500.h5
 ```
 
 Note that the `--mix_modalities` flag allows fixed and moving images to be of different modalities during training. This should not be set for unsupervised training, which uses MSE as the loss function.
 
 **Nonlinear thin-plate-spline (TPS)**
 
 To train the TPS variant of KeyMorph which allows for nonlinear registrations, specify `tps` as the keypoint alignment method and specify the tps lambda value: 
 
 ```
-python run.py --num_keypoints 128 --kp_align_method tps --tps_lmbda 0 --loss_fn dice \
-                --data_dir ./data/centered_IXI/ \
-                --load_path ./weights/numkey128_pretrain.2500.h5
+python scripts/run.py \
+    --run_mode train \
+    --num_keypoints 128 \
+    --kp_align_method tps \
+    --tps_lmbda 0 \
+    --loss_fn dice \
+    --data_dir ./data/centered_IXI/ \
+    --load_path ./weights/numkey128_pretrain.2500.h5
 ```
 
 The code also supports sampling lambda according to some distribution (`uniform`, `lognormal`, `loguniform`). For example, to sample from the `loguniform` distribution during training:
 
 ```
-python run.py --num_keypoints 128 --kp_align_method tps --tps_lmbda loguniform --loss_fn dice \
-                --data_dir ./data/centered_IXI/ \
-                --load_path ./weights/numkey128_pretrain.2500.h5
+python scripts/run.py \
+    --num_keypoints 128 \
+    --kp_align_method tps \
+    --tps_lmbda loguniform \
+    --loss_fn dice \
+    --data_dir ./data/centered_IXI/ \
+    --load_path ./weights/numkey128_pretrain.2500.h5
 ```
 
-Note that supervised/unsupervised variants can be run similarly to affine, as described above. -->
+Note that supervised/unsupervised variants can be run similarly to affine, as described above. 
 
-<!-- ## Step-by-step guide for reproducing our results
+## Step-by-step guide for reproducing our results
 
 ### Dataset 
 [A] Scripts in `./notebooks/[A] Download Data` will download the IXI data and perform some basic preprocessing
 
 [B] Once the data is downloaded `./notebooks/[B] Brain extraction` can be used to extract remove non-brain tissue. 
 
 [C] Once the brain has been extracted, we center the brain using `./notebooks/[C] Centering`. During training, we randomly introduce affine augmentation to the dataset. This ensure that the brain stays within the volume given the affine augmentation we introduce. It also helps during the pretraining step of our algorithm.
@@ -268,15 +297,15 @@
 ### Pretraining KeyMorph
 
 This step helps with the convergence of our model. We pick 1 subject and random points within the brain of that subject. We then introduce affine transformation to the subject brain and same transformation to the keypoints. In other words, this is a self-supervised task in where the network learns to predict the keypoints on a brain under random affine transformation. We found that initializing our model with these weights helps with the training.
 
 To pretrain, run:
  
 ```
-python pretraining.py --num_keypoints 128 --data_dir ./data/centered_IXI/ 
+python scripts/run.py --run_mode pretrain --num_keypoints 128 --data_dir ./data/centered_IXI/ 
 ```
 
 ### Training KeyMorph
 Follow instructions for "Training KeyMorph" above, depending on the variant you want.
 
 ### Evaluating KeyMorph
 To evaluate on the test set, simply add the `--eval` flag to any of the above commands. For example, for affine, unsupervised KeyMorph evaluation:
@@ -287,15 +316,15 @@
 ```
 
 Evaluation proceeds by looping through all test augmentations in `list_of_test_augs`, all test modality pairs in `list_of_test_mods`, and all pairs of volumes in the test set.
 Set `--save_preds` flag to save all outputs to disk.
 
 **Automatic Delineation/Segmentation of the Brain**
 
-For evaluation, we use [SynthSeg](https://github.com/BBillot/SynthSeg) to automatically segment different brain regions. Follow their repository for detailed intruction on how to use the model. -->
+For evaluation, we use [SynthSeg](https://github.com/BBillot/SynthSeg) to automatically segment different brain regions. Follow their repository for detailed intruction on how to use the model. 
 
 ## Issues
 This repository is being actively maintained. Feel free to open an issue for any problems or questions.
 
 ## Legacy code
 For a legacy version of the code, see our [legacy branch](https://github.com/alanqrwang/keymorph/tree/legacy).
```

### Comparing `keymorph-1.0.0/keymorph.egg-info/SOURCES.txt` & `keymorph-1.0.1/keymorph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keymorph-1.0.0/setup.py` & `keymorph-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 sys.path.insert(0, os.path.join(here, "keymorph"))
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="keymorph",
-    version="1.0.0",
+    version="1.0.1",
     author="Alan Q. Wang",
     author_email="alanqrwang@gmail.com",
     url="https://github.com/alanqrwang/keymorph",
     description="KeyMorph is a deep learning-based image registration framework that relies on automatically extracting corresponding keypoints.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
```

### Comparing `keymorph-1.0.0/tests/test.py` & `keymorph-1.0.1/tests/test.py`

 * *Files identical despite different names*

