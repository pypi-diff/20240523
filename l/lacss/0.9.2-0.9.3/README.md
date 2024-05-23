# Comparing `tmp/lacss-0.9.2.tar.gz` & `tmp/lacss-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacss-0.9.2.tar", max compression
+gzip compressed data, was "lacss-0.9.3.tar", max compression
```

## Comparing `lacss-0.9.2.tar` & `lacss-0.9.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1062 2024-05-22 13:27:25.378820 lacss-0.9.2/LICENSE
--rw-r--r--   0        0        0     2552 2024-05-22 13:27:25.378820 lacss-0.9.2/README.md
--rw-r--r--   0        0        0      157 2024-05-22 13:27:25.378820 lacss-0.9.2/lacss/__init__.py
--rw-r--r--   0        0        0       48 2024-05-22 13:27:25.378820 lacss-0.9.2/lacss/data/__init__.py
--rw-r--r--   0        0        0    14546 2024-05-22 13:27:25.378820 lacss-0.9.2/lacss/data/augment.py
--rw-r--r--   0        0        0    13109 2024-05-22 13:27:25.378820 lacss-0.9.2/lacss/data/generator.py
--rw-r--r--   0        0        0       43 2024-05-22 13:27:25.378820 lacss-0.9.2/lacss/deploy/__init__.py
--rw-r--r--   0        0        0    21615 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/deploy/predict.py
--rw-r--r--   0        0        0        0 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/deploy/proto/__init__.py
--rw-r--r--   0        0        0     1035 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/deploy/proto/lacss.proto
--rw-r--r--   0        0        0     3382 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/deploy/proto/lacss_pb2.py
--rw-r--r--   0        0        0     4000 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/deploy/proto/lacss_pb2.pyi
--rw-r--r--   0        0        0     2382 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/deploy/proto/lacss_pb2_grpc.py
--rw-r--r--   0        0        0     4484 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/deploy/remote_server.py
--rw-r--r--   0        0        0     4139 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/deploy/server.py
--rw-r--r--   0        0        0       74 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/losses/__init__.py
--rw-r--r--   0        0        0     6125 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/losses/auxiliary.py
--rw-r--r--   0        0        0      965 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/losses/common.py
--rw-r--r--   0        0        0     1748 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/losses/detection.py
--rw-r--r--   0        0        0     5415 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/losses/instance.py
--rw-r--r--   0        0        0       22 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/metrics/__init__.py
--rw-r--r--   0        0        0     5569 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/metrics/ranked.py
--rw-r--r--   0        0        0      330 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/modules/__init__.py
--rw-r--r--   0        0        0     2355 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/modules/common.py
--rw-r--r--   0        0        0     7968 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/modules/convnext.py
--rw-r--r--   0        0        0     7808 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/modules/detector.py
--rw-r--r--   0        0        0     3899 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/modules/lacss.py
--rw-r--r--   0        0        0     3292 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/modules/lpn.py
--rw-r--r--   0        0        0     3830 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/modules/resnet.py
--rw-r--r--   0        0        0     5557 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/modules/segmentor.py
--rw-r--r--   0        0        0     2297 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/modules/unet.py
--rw-r--r--   0        0        0      153 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/ops/__init__.py
--rw-r--r--   0        0        0     2474 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/ops/boxes.py
--rw-r--r--   0        0        0     3551 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/ops/image.py
--rw-r--r--   0        0        0     3136 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/ops/locations.py
--rw-r--r--   0        0        0     5961 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/ops/nms.py
--rw-r--r--   0        0        0    11822 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/ops/patches.py
--rw-r--r--   0        0        0      482 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/ops/uda.py
--rw-r--r--   0        0        0       63 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/tracking/__init__.py
--rw-r--r--   0        0        0     3340 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/tracking/predict.py
--rw-r--r--   0        0        0    12670 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/tracking/seqnms.py
--rw-r--r--   0        0        0     6741 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/tracking/smc.py
--rw-r--r--   0        0        0     5646 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/tracking/utils.py
--rw-r--r--   0        0        0      203 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/train/__init__.py
--rw-r--r--   0        0        0    10358 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/train/base_trainer.py
--rw-r--r--   0        0        0    10549 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/train/lacss_trainer.py
--rw-r--r--   0        0        0     1170 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/train/loss.py
--rw-r--r--   0        0        0     4564 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/train/strategy.py
--rw-r--r--   0        0        0     5541 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/train/utils.py
--rw-r--r--   0        0        0      931 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/typing.py
--rw-r--r--   0        0        0     5151 2024-05-22 13:27:25.382820 lacss-0.9.2/lacss/utils.py
--rw-r--r--   0        0        0     1057 2024-05-22 13:27:42.142731 lacss-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     3300 1970-01-01 00:00:00.000000 lacss-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-23 17:02:48.361604 lacss-0.9.3/LICENSE
+-rw-r--r--   0        0        0     2552 2024-05-23 17:02:48.361604 lacss-0.9.3/README.md
+-rw-r--r--   0        0        0      157 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/__init__.py
+-rw-r--r--   0        0        0       48 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/data/__init__.py
+-rw-r--r--   0        0        0    14546 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/data/augment.py
+-rw-r--r--   0        0        0    13109 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/data/generator.py
+-rw-r--r--   0        0        0       43 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/deploy/__init__.py
+-rw-r--r--   0        0        0    21615 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/deploy/predict.py
+-rw-r--r--   0        0        0        0 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/deploy/proto/__init__.py
+-rw-r--r--   0        0        0     1035 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/deploy/proto/lacss.proto
+-rw-r--r--   0        0        0     3382 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/deploy/proto/lacss_pb2.py
+-rw-r--r--   0        0        0     4000 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/deploy/proto/lacss_pb2.pyi
+-rw-r--r--   0        0        0     2382 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/deploy/proto/lacss_pb2_grpc.py
+-rw-r--r--   0        0        0     4484 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/deploy/remote_server.py
+-rw-r--r--   0        0        0     4139 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/deploy/server.py
+-rw-r--r--   0        0        0       74 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/losses/__init__.py
+-rw-r--r--   0        0        0     6125 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/losses/auxiliary.py
+-rw-r--r--   0        0        0      965 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/losses/common.py
+-rw-r--r--   0        0        0     1748 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/losses/detection.py
+-rw-r--r--   0        0        0     5415 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/losses/instance.py
+-rw-r--r--   0        0        0       22 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/metrics/__init__.py
+-rw-r--r--   0        0        0     5569 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/metrics/ranked.py
+-rw-r--r--   0        0        0      330 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/modules/__init__.py
+-rw-r--r--   0        0        0     2355 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/modules/common.py
+-rw-r--r--   0        0        0     7968 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/modules/convnext.py
+-rw-r--r--   0        0        0     7808 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/modules/detector.py
+-rw-r--r--   0        0        0     3899 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/modules/lacss.py
+-rw-r--r--   0        0        0     3292 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/modules/lpn.py
+-rw-r--r--   0        0        0     3830 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/modules/resnet.py
+-rw-r--r--   0        0        0     5557 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/modules/segmentor.py
+-rw-r--r--   0        0        0     2297 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/modules/unet.py
+-rw-r--r--   0        0        0      153 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/ops/__init__.py
+-rw-r--r--   0        0        0     2474 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/ops/boxes.py
+-rw-r--r--   0        0        0     3551 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/ops/image.py
+-rw-r--r--   0        0        0     3136 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/ops/locations.py
+-rw-r--r--   0        0        0     5961 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/ops/nms.py
+-rw-r--r--   0        0        0    11822 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/ops/patches.py
+-rw-r--r--   0        0        0      482 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/ops/uda.py
+-rw-r--r--   0        0        0       63 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/tracking/__init__.py
+-rw-r--r--   0        0        0     3340 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/tracking/predict.py
+-rw-r--r--   0        0        0    12670 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/tracking/seqnms.py
+-rw-r--r--   0        0        0     6741 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/tracking/smc.py
+-rw-r--r--   0        0        0     5646 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/tracking/utils.py
+-rw-r--r--   0        0        0      203 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/train/__init__.py
+-rw-r--r--   0        0        0    10358 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/train/base_trainer.py
+-rw-r--r--   0        0        0    10549 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/train/lacss_trainer.py
+-rw-r--r--   0        0        0     1170 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/train/loss.py
+-rw-r--r--   0        0        0     4564 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/train/strategy.py
+-rw-r--r--   0        0        0     5541 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/train/utils.py
+-rw-r--r--   0        0        0      931 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/typing.py
+-rw-r--r--   0        0        0     5151 2024-05-23 17:02:48.365604 lacss-0.9.3/lacss/utils.py
+-rw-r--r--   0        0        0     1114 2024-05-23 17:03:04.453490 lacss-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     3358 1970-01-01 00:00:00.000000 lacss-0.9.3/PKG-INFO
```

### Comparing `lacss-0.9.2/LICENSE` & `lacss-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/README.md` & `lacss-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/data/augment.py` & `lacss-0.9.3/lacss/data/augment.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/data/generator.py` & `lacss-0.9.3/lacss/data/generator.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/deploy/predict.py` & `lacss-0.9.3/lacss/deploy/predict.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/deploy/proto/lacss.proto` & `lacss-0.9.3/lacss/deploy/proto/lacss.proto`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/deploy/proto/lacss_pb2.py` & `lacss-0.9.3/lacss/deploy/proto/lacss_pb2.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/deploy/proto/lacss_pb2.pyi` & `lacss-0.9.3/lacss/deploy/proto/lacss_pb2.pyi`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/deploy/proto/lacss_pb2_grpc.py` & `lacss-0.9.3/lacss/deploy/proto/lacss_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/deploy/remote_server.py` & `lacss-0.9.3/lacss/deploy/remote_server.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/deploy/server.py` & `lacss-0.9.3/lacss/deploy/server.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/losses/auxiliary.py` & `lacss-0.9.3/lacss/losses/auxiliary.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/losses/common.py` & `lacss-0.9.3/lacss/losses/common.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/losses/detection.py` & `lacss-0.9.3/lacss/losses/detection.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/losses/instance.py` & `lacss-0.9.3/lacss/losses/instance.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/metrics/ranked.py` & `lacss-0.9.3/lacss/metrics/ranked.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/modules/common.py` & `lacss-0.9.3/lacss/modules/common.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/modules/convnext.py` & `lacss-0.9.3/lacss/modules/convnext.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/modules/detector.py` & `lacss-0.9.3/lacss/modules/detector.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/modules/lacss.py` & `lacss-0.9.3/lacss/modules/lacss.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/modules/lpn.py` & `lacss-0.9.3/lacss/modules/lpn.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/modules/resnet.py` & `lacss-0.9.3/lacss/modules/resnet.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/modules/segmentor.py` & `lacss-0.9.3/lacss/modules/segmentor.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/modules/unet.py` & `lacss-0.9.3/lacss/modules/unet.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/ops/boxes.py` & `lacss-0.9.3/lacss/ops/boxes.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/ops/image.py` & `lacss-0.9.3/lacss/ops/image.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/ops/locations.py` & `lacss-0.9.3/lacss/ops/locations.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/ops/nms.py` & `lacss-0.9.3/lacss/ops/nms.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/ops/patches.py` & `lacss-0.9.3/lacss/ops/patches.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/tracking/predict.py` & `lacss-0.9.3/lacss/tracking/predict.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/tracking/seqnms.py` & `lacss-0.9.3/lacss/tracking/seqnms.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/tracking/smc.py` & `lacss-0.9.3/lacss/tracking/smc.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/tracking/utils.py` & `lacss-0.9.3/lacss/tracking/utils.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/train/base_trainer.py` & `lacss-0.9.3/lacss/train/base_trainer.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/train/lacss_trainer.py` & `lacss-0.9.3/lacss/train/lacss_trainer.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/train/loss.py` & `lacss-0.9.3/lacss/train/loss.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/train/strategy.py` & `lacss-0.9.3/lacss/train/strategy.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/train/utils.py` & `lacss-0.9.3/lacss/train/utils.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/typing.py` & `lacss-0.9.3/lacss/typing.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/lacss/utils.py` & `lacss-0.9.3/lacss/utils.py`

 * *Files identical despite different names*

### Comparing `lacss-0.9.2/pyproject.toml` & `lacss-0.9.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 [tool.poetry]
 name = "lacss"
-version = "0.9.2"
-description = "Cell segmentation and tracking"
+version = "0.9.3"
+description = "Tools for cell segmentation"
 authors = ["Ji Yu <jyu@uchc.edu>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.10, <3.12"
-flax = "^0.7.2"
+python = "^3.10"
 tqdm = "^4.65.0"
 imageio = "^2.9.0"
 scikit-image = ">=0.19.0"
-typer = ">=0.4.0"
 imagecodecs = "^2023.3.16"
 opencv-python = "^4.8.1.78"
-orbax-checkpoint = "^0.5"
+xtrain = "^0.3.2"
+protoc-wheel-0 = "^24.4"
+typer = "^0.12.3"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.2"
 jupyterlab = "^3.6.1"
-jax = {extras = ["cuda11-pip"], version = "^0.4.14"}
-tensorflow = "^2.13.0"
-protoc-wheel-0 = "^24.4"
+pytest = "^7.4.0"
+jax = {extras = ["cuda11_pip"], version = "^0.4, <=0.4.24"}
+nvidia-cudnn-cu11 = "^8.0" # bypass jax packaging error
+orbax-checkpoint = "0.5.3"
+ott-jax = "^0.4.0"
+tensorflow = "^2.16.1"
+ml-collections = "^0.1.1"
+matplotlib = "^3.8.4"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.2.3"
 mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 mkdocs-gen-files = "^0.5.0"
 
-
-[tool.poetry.group.grpc.dependencies]
-grpcio-tools = "^1.62.0"
-
 [[tool.poetry.source]]
 name = "jax"
 url = "https://storage.googleapis.com/jax-releases/jax_cuda_releases.html"
 priority = "supplemental"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `lacss-0.9.2/PKG-INFO` & `lacss-0.9.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: lacss
-Version: 0.9.2
-Summary: Cell segmentation and tracking
+Version: 0.9.3
+Summary: Tools for cell segmentation
 License: MIT
 Author: Ji Yu
 Author-email: jyu@uchc.edu
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flax (>=0.7.2,<0.8.0)
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: imagecodecs (>=2023.3.16,<2024.0.0)
 Requires-Dist: imageio (>=2.9.0,<3.0.0)
 Requires-Dist: opencv-python (>=4.8.1.78,<5.0.0.0)
-Requires-Dist: orbax-checkpoint (>=0.5,<0.6)
+Requires-Dist: protoc-wheel-0 (>=24.4,<25.0)
 Requires-Dist: scikit-image (>=0.19.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Requires-Dist: typer (>=0.4.0)
+Requires-Dist: typer (>=0.12.3,<0.13.0)
+Requires-Dist: xtrain (>=0.3.2,<0.4.0)
 Description-Content-Type: text/markdown
 
 ## LACSS
 
 _LACSS is a deep-learning model for single-cell segmentation from microscopy images._ 
 
 References:
```

