# Comparing `tmp/xaitk_saliency-0.7.0.tar.gz` & `tmp/xaitk_saliency-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xaitk_saliency-0.7.0.tar", max compression
+gzip compressed data, was "xaitk_saliency-0.8.0.tar", max compression
```

## Comparing `xaitk_saliency-0.7.0.tar` & `xaitk_saliency-0.8.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1476 2023-06-19 06:56:54.438357 xaitk_saliency-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     4559 2023-06-19 06:56:54.438357 xaitk_saliency-0.7.0/README.md
--rw-r--r--   0        0        0     5506 2023-06-19 06:56:54.486358 xaitk_saliency-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      943 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/__init__.py
--rw-r--r--   0        0        0      425 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_classifier_conf_sal/__init__.py
--rw-r--r--   0        0        0     2172 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_classifier_conf_sal/occlusion_scoring.py
--rw-r--r--   0        0        0     2808 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_classifier_conf_sal/rise_scoring.py
--rw-r--r--   0        0        0     1957 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_classifier_conf_sal/squared_difference_scoring.py
--rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_descriptor_sim_sal/__init__.py
--rw-r--r--   0        0        0     3876 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_descriptor_sim_sal/similarity_scoring.py
--rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_detector_prop_sal/__init__.py
--rw-r--r--   0        0        0     5017 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_detector_prop_sal/drise_scoring.py
--rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/__init__.py
--rw-r--r--   0        0        0     4215 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/occlusion_based.py
--rw-r--r--   0        0        0     3110 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/rise.py
--rw-r--r--   0        0        0     2926 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/slidingwindow.py
--rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_similarity_blackbox_sal/__init__.py
--rw-r--r--   0        0        0     3970 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_similarity_blackbox_sal/occlusion_based.py
--rw-r--r--   0        0        0     3876 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_similarity_blackbox_sal/sbsm.py
--rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_object_detector_blackbox_sal/__init__.py
--rw-r--r--   0        0        0     5843 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_object_detector_blackbox_sal/drise.py
--rw-r--r--   0        0        0     7008 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_object_detector_blackbox_sal/occlusion_based.py
--rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/perturb_image/__init__.py
--rw-r--r--   0        0        0     4038 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/perturb_image/random_grid.py
--rw-r--r--   0        0        0     4689 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/perturb_image/rise.py
--rw-r--r--   0        0        0     3704 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/perturb_image/sliding_radial.py
--rw-r--r--   0        0        0     3054 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/impls/perturb_image/sliding_window.py
--rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/interfaces/__init__.py
--rw-r--r--   0        0        0     4221 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_classifier_conf_sal.py
--rw-r--r--   0        0        0     3811 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_descriptor_sim_sal.py
--rw-r--r--   0        0        0     5054 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_detector_prop_sal.py
--rw-r--r--   0        0        0     4635 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_image_classifier_blackbox_sal.py
--rw-r--r--   0        0        0     5245 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_image_similarity_blackbox_sal.py
--rw-r--r--   0        0        0     9837 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_object_detector_blackbox_sal.py
--rw-r--r--   0        0        0     1651 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/interfaces/perturb_image.py
--rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/py.typed
--rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/utils/bin/__init__.py
--rw-r--r--   0        0        0     5732 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/utils/bin/sal_on_coco_dets.py
--rw-r--r--   0        0        0     2706 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/utils/coco.py
--rw-r--r--   0        0        0     2759 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/utils/detection.py
--rw-r--r--   0        0        0    14129 2023-06-19 06:56:54.490358 xaitk_saliency-0.7.0/xaitk_saliency/utils/masking.py
--rw-r--r--   0        0        0     6513 1970-01-01 00:00:00.000000 xaitk_saliency-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1476 2024-05-23 18:59:21.350088 xaitk_saliency-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     4559 2024-05-23 18:59:21.350088 xaitk_saliency-0.8.0/README.md
+-rw-r--r--   0        0        0     6049 2024-05-23 18:59:21.390088 xaitk_saliency-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      943 2024-05-23 18:59:21.394088 xaitk_saliency-0.8.0/xaitk_saliency/__init__.py
+-rw-r--r--   0        0        0      425 2024-05-23 18:59:21.394088 xaitk_saliency-0.8.0/xaitk_saliency/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:59:21.394088 xaitk_saliency-0.8.0/xaitk_saliency/impls/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:59:21.394088 xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_classifier_conf_sal/__init__.py
+-rw-r--r--   0        0        0     2172 2024-05-23 18:59:21.394088 xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_classifier_conf_sal/occlusion_scoring.py
+-rw-r--r--   0        0        0     2808 2024-05-23 18:59:21.394088 xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_classifier_conf_sal/rise_scoring.py
+-rw-r--r--   0        0        0     1957 2024-05-23 18:59:21.394088 xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_classifier_conf_sal/squared_difference_scoring.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:59:21.394088 xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_descriptor_sim_sal/__init__.py
+-rw-r--r--   0        0        0     3876 2024-05-23 18:59:21.394088 xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_descriptor_sim_sal/similarity_scoring.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:59:21.394088 xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_detector_prop_sal/__init__.py
+-rw-r--r--   0        0        0     5017 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_detector_prop_sal/drise_scoring.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/__init__.py
+-rw-r--r--   0        0        0     4215 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/occlusion_based.py
+-rw-r--r--   0        0        0     3110 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/rise.py
+-rw-r--r--   0        0        0     2926 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/slidingwindow.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_image_similarity_blackbox_sal/__init__.py
+-rw-r--r--   0        0        0     3970 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_image_similarity_blackbox_sal/occlusion_based.py
+-rw-r--r--   0        0        0     3876 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_image_similarity_blackbox_sal/sbsm.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_object_detector_blackbox_sal/__init__.py
+-rw-r--r--   0        0        0     5843 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_object_detector_blackbox_sal/drise.py
+-rw-r--r--   0        0        0     7008 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_object_detector_blackbox_sal/occlusion_based.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/impls/perturb_image/__init__.py
+-rw-r--r--   0        0        0     4038 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/impls/perturb_image/random_grid.py
+-rw-r--r--   0        0        0     4689 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/impls/perturb_image/rise.py
+-rw-r--r--   0        0        0     3704 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/impls/perturb_image/sliding_radial.py
+-rw-r--r--   0        0        0     3054 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/impls/perturb_image/sliding_window.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/interfaces/__init__.py
+-rw-r--r--   0        0        0     4221 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/interfaces/gen_classifier_conf_sal.py
+-rw-r--r--   0        0        0     3811 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/interfaces/gen_descriptor_sim_sal.py
+-rw-r--r--   0        0        0     5054 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/interfaces/gen_detector_prop_sal.py
+-rw-r--r--   0        0        0     4635 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/interfaces/gen_image_classifier_blackbox_sal.py
+-rw-r--r--   0        0        0     5245 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/interfaces/gen_image_similarity_blackbox_sal.py
+-rw-r--r--   0        0        0     9837 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/interfaces/gen_object_detector_blackbox_sal.py
+-rw-r--r--   0        0        0     1651 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/interfaces/perturb_image.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/py.typed
+-rw-r--r--   0        0        0        0 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/utils/bin/__init__.py
+-rw-r--r--   0        0        0     6016 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/utils/bin/sal_on_coco_dets.py
+-rw-r--r--   0        0        0     2706 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/utils/coco.py
+-rw-r--r--   0        0        0     2759 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/utils/detection.py
+-rw-r--r--   0        0        0    14343 2024-05-23 18:59:21.398088 xaitk_saliency-0.8.0/xaitk_saliency/utils/masking.py
+-rw-r--r--   0        0        0     7208 1970-01-01 00:00:00.000000 xaitk_saliency-0.8.0/PKG-INFO
```

### Comparing `xaitk_saliency-0.7.0/LICENSE.txt` & `xaitk_saliency-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/README.md` & `xaitk_saliency-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/pyproject.toml` & `xaitk_saliency-0.8.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ###############################################################################
 [tool.poetry]
 name = "xaitk_saliency"
 # REMEMBER: `distutils.version.*Version` types can be used to compare versions
 # from strings like this.
 # This package prefers to use the strict numbering standard when possible.
-version = "0.7.0"
+version = "0.8.0"
 description = """\
     Visual saliency map generation interfaces and baseline implementations \
     for explainable AI."""
 license = "BSD-3-Clause"
 authors = ["Kitware, Inc. <xaitk@kitware.com>"]
 readme = "README.md"
 repository = "https://github.com/XAITK/xaitk-saliency"
@@ -25,45 +25,58 @@
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Unix',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-numpy = ">=1.22"
+numpy = [
+    {version = ">=1.22,<1.26", python = ">=3.8,<3.12"},
+    {version = ">=1.26", python = ">=3.12"}
+]
 scikit-image = [
     # Hinge because minimum support 0.20.0 for py3.11
     { version = ">=0.18.1", python = "<3.11" },
-    { version = ">=0.20.0", python = ">=3.11" }
+    { version = ">=0.20.0", python = ">=3.11, <3.12" },
+    { version = ">=0.22.0", python = ">=3.12" }
+]
+scikit-learn = [
+    {version = ">=1.2, <1.4", python = ">=3.8,<3.12"},
+    {version = ">=1.4", python = ">=3.12"}
 ]
-scikit-learn = ">=1.2"
 smqtk-classifier = ">=0.17.0"
 smqtk-core = ">=0.18.0"
 smqtk-descriptors = ">=0.16.0"
 smqtk-detection = ">=0.19.0"
-scipy = ">=1.8.1"
+scipy = [
+    {version = ">=1.8.1,<1.9", python = ">=3.8,<3.11"},
+    {version = ">=1.9", python = "^3.11"}
+]
 click = ">=8.0.3"
 setuptools = "*"
 # Optionals for "example" extra
 jupyter = { version = ">=1.0.0", optional = true }
 matplotlib = { version=">=3.4.1", optional = true }
 papermill = { version = ">=2.3.3", optional = true }
 torch = {version = ">=1.9.0,!=2.0.1", optional = true}
 torchvision = {version = ">=0.10.0", optional = true}
 tqdm = { version = ">=4.45.0", optional = true }
 # Optionals for "tools" extra"
 kwcoco = { version = ">=0.2.18", optional = true}
+pyyaml = {version = ">=6.0.1", optional = true, python = ">=3.12"}
+shapely = {version = ">=2.0.2", optional = true, python = ">=3.12"}
 
 [tool.poetry.extras]
 example_deps = [ "jupyter", "matplotlib", "papermill", "torch", "torchvision", "tqdm" ]
-tools = [ "kwcoco", "matplotlib" ]
+tools = [ "kwcoco", "matplotlib", "pyyaml", "shapely" ]
 
 [tool.poetry.dev-dependencies]
 # CI
 flake8 = [
     # Hinge because 6.0 minimum supported python version is 3.8.1
     { version = ">=5", python = "<3.8.1" },
     { version = ">=6", python = ">=3.8.1" }
```

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/__init__.py` & `xaitk_saliency-0.8.0/xaitk_saliency/__init__.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_classifier_conf_sal/occlusion_scoring.py` & `xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_classifier_conf_sal/occlusion_scoring.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_classifier_conf_sal/rise_scoring.py` & `xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_classifier_conf_sal/rise_scoring.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_classifier_conf_sal/squared_difference_scoring.py` & `xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_classifier_conf_sal/squared_difference_scoring.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_descriptor_sim_sal/similarity_scoring.py` & `xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_descriptor_sim_sal/similarity_scoring.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_detector_prop_sal/drise_scoring.py` & `xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_detector_prop_sal/drise_scoring.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/occlusion_based.py` & `xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/occlusion_based.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/rise.py` & `xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/rise.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/slidingwindow.py` & `xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_image_classifier_blackbox_sal/slidingwindow.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_similarity_blackbox_sal/occlusion_based.py` & `xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_image_similarity_blackbox_sal/occlusion_based.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_image_similarity_blackbox_sal/sbsm.py` & `xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_image_similarity_blackbox_sal/sbsm.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_object_detector_blackbox_sal/drise.py` & `xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_object_detector_blackbox_sal/drise.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/impls/gen_object_detector_blackbox_sal/occlusion_based.py` & `xaitk_saliency-0.8.0/xaitk_saliency/impls/gen_object_detector_blackbox_sal/occlusion_based.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/impls/perturb_image/random_grid.py` & `xaitk_saliency-0.8.0/xaitk_saliency/impls/perturb_image/random_grid.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/impls/perturb_image/rise.py` & `xaitk_saliency-0.8.0/xaitk_saliency/impls/perturb_image/rise.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/impls/perturb_image/sliding_radial.py` & `xaitk_saliency-0.8.0/xaitk_saliency/impls/perturb_image/sliding_radial.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/impls/perturb_image/sliding_window.py` & `xaitk_saliency-0.8.0/xaitk_saliency/impls/perturb_image/sliding_window.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_classifier_conf_sal.py` & `xaitk_saliency-0.8.0/xaitk_saliency/interfaces/gen_classifier_conf_sal.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_descriptor_sim_sal.py` & `xaitk_saliency-0.8.0/xaitk_saliency/interfaces/gen_descriptor_sim_sal.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_detector_prop_sal.py` & `xaitk_saliency-0.8.0/xaitk_saliency/interfaces/gen_detector_prop_sal.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_image_classifier_blackbox_sal.py` & `xaitk_saliency-0.8.0/xaitk_saliency/interfaces/gen_image_classifier_blackbox_sal.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_image_similarity_blackbox_sal.py` & `xaitk_saliency-0.8.0/xaitk_saliency/interfaces/gen_image_similarity_blackbox_sal.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/interfaces/gen_object_detector_blackbox_sal.py` & `xaitk_saliency-0.8.0/xaitk_saliency/interfaces/gen_object_detector_blackbox_sal.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/interfaces/perturb_image.py` & `xaitk_saliency-0.8.0/xaitk_saliency/interfaces/perturb_image.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/utils/bin/sal_on_coco_dets.py` & `xaitk_saliency-0.8.0/xaitk_saliency/utils/bin/sal_on_coco_dets.py`

 * *Files 8% similar despite different names*

```diff
@@ -108,17 +108,19 @@
             blackbox_detector
         ) for ref_img, bboxes, scores in parse_coco_dset(dets_dset)
     ]
 
     # The outputs of pase_coco_dset() are constructed using gid_to_aids, so we
     # can assume the order of image and annotation ids in gid_to_aids here
     # correspond correctly to that of the generated saliency maps.
+    img_skip_counter = 0
     for img_idx, (img_id, det_ids) in enumerate(dets_dset.gid_to_aids.items()):
         # skip if there are no dets for this image
         if len(det_ids) == 0:
+            img_skip_counter += 1
             continue  # pragma: no cover
 
         img_file = dets_dset.get_image_fpath(img_id)
         ref_img = np.asarray(Image.open(img_file))
 
         img_file = dets_dset.imgs[img_id]['file_name']
 
@@ -127,17 +129,22 @@
         # split off file extension
         img_name = os.path.splitext(img_name)[0]
 
         sub_dir = os.path.join(output_dir, img_name)
 
         os.makedirs(sub_dir, exist_ok=True)
 
+        sal_skip_counter = 0
         for sal_idx, det_id in enumerate(det_ids):
+            ann = dets_dset.anns[det_id]
+            if not ('score' in ann or 'prob' in ann):
+                sal_skip_counter += 1
+                continue
 
-            sal_map = img_sal_maps[img_idx][sal_idx]
+            sal_map = img_sal_maps[img_idx - img_skip_counter][sal_idx - sal_skip_counter]
 
             fig = plt.figure()
             plt.axis('off')
             if overlay_image:
                 gray_img = np.asarray(Image.fromarray(ref_img).convert("L"))
                 plt.imshow(gray_img, alpha=0.7, cmap='gray')
```

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/utils/coco.py` & `xaitk_saliency-0.8.0/xaitk_saliency/utils/coco.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/utils/detection.py` & `xaitk_saliency-0.8.0/xaitk_saliency/utils/detection.py`

 * *Files identical despite different names*

### Comparing `xaitk_saliency-0.7.0/xaitk_saliency/utils/masking.py` & `xaitk_saliency-0.8.0/xaitk_saliency/utils/masking.py`

 * *Files 3% similar despite different names*

```diff
@@ -223,64 +223,68 @@
 ) -> None:
     """
     Simple benchmark for the two above `occlude_image_*` functions above w.r.t.
     the given reference image matrix, which should be of the shape
     `[H x W [x C]]`.
     """
     img_mat = np.ones((*img_shape, img_channels), dtype=np.uint8)
-    masks = (np.random.rand(num_masks, *img_shape[:2]) < 0.5)
+    rng = np.random.default_rng(seed=0)
+    masks = (rng.standard_normal((num_masks, *img_shape[:2])) < 0.5)
     fill_1c: int = 0
     fill_mc = [0] * img_channels
     perf_counter = time.perf_counter
     print(f"Image shape={img_mat.shape}, masks={masks.shape}, fill_1c={fill_1c}, fill_{img_channels}c={fill_mc}")
 
+    def log_line(op: str, mode: str, cores: int, fill: str, seconds: float) -> None:
+        print(f"{op:12s}{mode:16s}{cores:2d}  {fill:9s}{seconds} s")
+
     s = perf_counter()
     occlude_image_batch(img_mat, masks)
     e = perf_counter()
-    print(f"Batch - no-fill - {e-s} s")
+    log_line("Batch", "main", 0, "no-fill", e-s)
     for threads in threading_tests:
         s = perf_counter()
         occlude_image_batch(img_mat, masks, threads=threads)
         e = perf_counter()
-        print(f"Batch - threads={threads:2d} - no-fill - {e-s} s")
+        log_line("Batch", "threads", threads, "no-fill", e - s)
     for threads in threading_tests:
         s = perf_counter()
         np.asarray(list(occlude_image_streaming(img_mat, masks, threads=threads)))
         e = perf_counter()
-        print(f"Streaming - threads={threads:2d} - no-fill - {e-s} s")
+        log_line("Streaming", "threads", threads, "no-fill", e - s)
 
     s = perf_counter()
     occlude_image_batch(img_mat, masks, fill=fill_1c)
     e = perf_counter()
-    print(f"Batch - fill-1c - {e-s} s")
+    log_line("Batch", "main", 0, "fill-1c", e-s)
     for threads in threading_tests:
         s = perf_counter()
         occlude_image_batch(img_mat, masks, fill=fill_1c, threads=threads)
         e = perf_counter()
-        print(f"Batch - threads={threads:2d} - fill-1c - {e-s} s")
+        log_line("Batch", "threads", threads, "fill-1c", e - s)
     for threads in threading_tests:
         s = perf_counter()
         np.asarray(list(occlude_image_streaming(img_mat, masks, fill=fill_1c, threads=threads)))
         e = perf_counter()
-        print(f"Streaming - threads={threads:2d} - fill-1c - {e-s} s")
+        log_line("Streaming", "threads", threads, "fill-1c", e - s)
 
     s = perf_counter()
     occlude_image_batch(img_mat, masks, fill=fill_mc)
     e = perf_counter()
-    print(f"Batch - fill-{img_channels}c - {e-s} s")
+    log_line("Batch", "main", 0, f"fill-{img_channels}c", e-s)
     for threads in threading_tests:
         s = perf_counter()
         occlude_image_batch(img_mat, masks, fill=fill_mc, threads=threads)
         e = perf_counter()
-        print(f"Batch - threads={threads:2d} - fill-{img_channels}c - {e-s} s")
+        log_line("Batch", "threads", threads, f"fill-{img_channels}c", e - s)
     for threads in threading_tests:
         s = perf_counter()
         np.asarray(list(occlude_image_streaming(img_mat, masks, fill=fill_mc, threads=threads)))
         e = perf_counter()
-        print(f"Streaming - threads={threads:2d} - fill-{img_channels}c - {e-s} s")
+        log_line("Streaming", "threads", threads, f"fill-{img_channels}c", e - s)
 
 
 def weight_regions_by_scalar(
     scalar_vec: np.ndarray,
     masks: np.ndarray,
     inv_masks: bool = True,
     normalize: bool = True,
```

### Comparing `xaitk_saliency-0.7.0/PKG-INFO` & `xaitk_saliency-0.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xaitk-saliency
-Version: 0.7.0
+Name: xaitk_saliency
+Version: 0.8.0
 Summary: Visual saliency map generation interfaces and baseline implementations for explainable AI.
 Home-page: https://github.com/XAITK/xaitk-saliency
 License: BSD-3-Clause
 Author: Kitware, Inc.
 Author-email: xaitk@kitware.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -14,27 +14,34 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: example-deps
 Provides-Extra: tools
 Requires-Dist: click (>=8.0.3)
 Requires-Dist: jupyter (>=1.0.0) ; extra == "example-deps"
 Requires-Dist: kwcoco (>=0.2.18) ; extra == "tools"
 Requires-Dist: matplotlib (>=3.4.1) ; extra == "example-deps" or extra == "tools"
-Requires-Dist: numpy (>=1.22)
+Requires-Dist: numpy (>=1.22,<1.26) ; python_version >= "3.8" and python_version < "3.12"
+Requires-Dist: numpy (>=1.26) ; python_version >= "3.12"
 Requires-Dist: papermill (>=2.3.3) ; extra == "example-deps"
+Requires-Dist: pyyaml (>=6.0.1) ; (python_version >= "3.12") and (extra == "tools")
 Requires-Dist: scikit-image (>=0.18.1) ; python_version < "3.11"
-Requires-Dist: scikit-image (>=0.20.0) ; python_version >= "3.11"
-Requires-Dist: scikit-learn (>=1.2)
-Requires-Dist: scipy (>=1.8.1)
+Requires-Dist: scikit-image (>=0.20.0) ; python_version >= "3.11" and python_version < "3.12"
+Requires-Dist: scikit-image (>=0.22.0) ; python_version >= "3.12"
+Requires-Dist: scikit-learn (>=1.2,<1.4) ; python_version >= "3.8" and python_version < "3.12"
+Requires-Dist: scikit-learn (>=1.4) ; python_version >= "3.12"
+Requires-Dist: scipy (>=1.8.1,<1.9) ; python_version >= "3.8" and python_version < "3.11"
+Requires-Dist: scipy (>=1.9) ; python_version >= "3.11" and python_version < "4.0"
 Requires-Dist: setuptools
+Requires-Dist: shapely (>=2.0.2) ; (python_version >= "3.12") and (extra == "tools")
 Requires-Dist: smqtk-classifier (>=0.17.0)
 Requires-Dist: smqtk-core (>=0.18.0)
 Requires-Dist: smqtk-descriptors (>=0.16.0)
 Requires-Dist: smqtk-detection (>=0.19.0)
 Requires-Dist: torch (>=1.9.0,!=2.0.1) ; extra == "example-deps"
 Requires-Dist: torchvision (>=0.10.0) ; extra == "example-deps"
 Requires-Dist: tqdm (>=4.45.0) ; extra == "example-deps"
```

