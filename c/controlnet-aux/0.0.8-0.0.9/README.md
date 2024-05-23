# Comparing `tmp/controlnet_aux-0.0.8.tar.gz` & `tmp/controlnet_aux-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "controlnet_aux-0.0.8.tar", last modified: Fri Apr 12 08:22:28 2024, max compression
+gzip compressed data, was "controlnet_aux-0.0.9.tar", last modified: Thu May 23 03:25:10 2024, max compression
```

## Comparing `controlnet_aux-0.0.8.tar` & `controlnet_aux-0.0.9.tar`

### file list

```diff
@@ -1,203 +1,212 @@
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.908465 controlnet_aux-0.0.8/
--rw-r--r--   0 sayakpaul   (501) staff       (20)    11357 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/LICENSE.txt
--rw-r--r--   0 sayakpaul   (501) staff       (20)     6095 2024-04-12 08:22:28.908296 controlnet_aux-0.0.8/PKG-INFO
--rw-r--r--   0 sayakpaul   (501) staff       (20)     4848 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/README.md
--rw-r--r--   0 sayakpaul   (501) staff       (20)       38 2024-04-12 08:22:28.908511 controlnet_aux-0.0.8/setup.cfg
--rw-r--r--   0 sayakpaul   (501) staff       (20)     8785 2024-04-12 08:20:48.000000 controlnet_aux-0.0.8/setup.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.883269 controlnet_aux-0.0.8/src/
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.888376 controlnet_aux-0.0.8/src/controlnet_aux/
--rw-r--r--   0 sayakpaul   (501) staff       (20)      582 2024-04-12 08:21:02.000000 controlnet_aux-0.0.8/src/controlnet_aux/__init__.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.889364 controlnet_aux-0.0.8/src/controlnet_aux/canny/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     1353 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/canny/__init__.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.889858 controlnet_aux-0.0.8/src/controlnet_aux/dwpose/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     2996 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/dwpose/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    10660 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/dwpose/util.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     4576 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/dwpose/wholebody.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.890039 controlnet_aux-0.0.8/src/controlnet_aux/hed/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     5791 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/hed/__init__.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.890207 controlnet_aux-0.0.8/src/controlnet_aux/leres/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     4465 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/__init__.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.891222 controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     6241 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/Resnet.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     8547 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/Resnext_torch.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    22911 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/depthmap.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     1122 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/multi_depth_model_woauxi.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     2029 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/net_tools.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    16887 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/network_auxi.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.891379 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/
--rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/__init__.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.892070 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/models/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     3095 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/models/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    10714 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/models/base_model.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     1660 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/models/base_model_hg.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    28960 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/models/networks.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     7404 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/models/pix2pix4depth_model.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.892468 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/options/
--rw-r--r--   0 sayakpaul   (501) staff       (20)      136 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/options/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     9364 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/options/base_options.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     1062 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/options/test_options.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.892769 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/util/
--rw-r--r--   0 sayakpaul   (501) staff       (20)       83 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/util/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     3110 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/util/util.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.892905 controlnet_aux-0.0.8/src/controlnet_aux/lineart/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     5899 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/lineart/__init__.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.893035 controlnet_aux-0.0.8/src/controlnet_aux/lineart_anime/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     8263 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/lineart_anime/__init__.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.893285 controlnet_aux-0.0.8/src/controlnet_aux/mediapipe_face/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     1944 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/mediapipe_face/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     7118 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/mediapipe_face/mediapipe_face_common.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.893661 controlnet_aux-0.0.8/src/controlnet_aux/midas/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     3640 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/midas/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     5276 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/midas/api.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.894660 controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/
--rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)      367 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/base_model.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     9242 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/blocks.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     3154 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/dpt_depth.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     2709 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/midas_net.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     5207 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/midas_net_custom.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     7869 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/transforms.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    14625 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/vit.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     4582 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/midas/utils.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.894932 controlnet_aux-0.0.8/src/controlnet_aux/mlsd/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     2875 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/mlsd/__init__.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.895314 controlnet_aux-0.0.8/src/controlnet_aux/mlsd/models/
--rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/mlsd/models/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     9678 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     9180 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    24189 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/mlsd/utils.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.895434 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     3706 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/__init__.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.895802 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/
--rw-r--r--   0 sayakpaul   (501) staff       (20)      597 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/NNET.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     2980 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/baseline.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.896317 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/
--rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    10480 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/decoder.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.897665 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/
--rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     2428 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     5993 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.898884 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/
--rw-r--r--   0 sayakpaul   (501) staff       (20)      206 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/__init__.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.899440 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     4170 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     2690 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     2294 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     4549 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     3350 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    12093 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    26514 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    59925 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     2833 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    15009 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)      707 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)       22 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/version.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     2730 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     5821 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     2932 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)      843 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     4905 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     1737 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     1297 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     6632 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     1060 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/encoder.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     5703 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/submodules.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.900193 controlnet_aux-0.0.8/src/controlnet_aux/open_pose/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     9606 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/open_pose/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    12428 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/open_pose/body.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    13491 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/open_pose/face.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     3210 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/open_pose/hand.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     8743 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/open_pose/model.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    13742 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/open_pose/util.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.900441 controlnet_aux-0.0.8/src/controlnet_aux/pidi/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     3190 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/pidi/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    21813 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/pidi/model.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     6259 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/processor.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.900950 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     3364 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    15148 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/automatic_mask_generator.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     4695 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/build_sam.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.902023 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/
--rw-r--r--   0 sayakpaul   (501) staff       (20)      419 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     1479 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/common.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    14420 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/image_encoder.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     6615 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/mask_decoder.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     8594 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/prompt_encoder.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     7283 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/sam.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    24707 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/tiny_vit_sam.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     8397 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/transformer.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    11633 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/predictor.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.902530 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/utils/
--rw-r--r--   0 sayakpaul   (501) staff       (20)      197 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/utils/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    12712 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/utils/amg.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     5812 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/utils/onnx.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     3972 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/utils/transforms.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.902661 controlnet_aux-0.0.8/src/controlnet_aux/shuffle/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     3330 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/shuffle/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     5434 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/util.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.902786 controlnet_aux-0.0.8/src/controlnet_aux/zoe/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     2972 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/__init__.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.902907 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/
--rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/__init__.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.903387 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     1154 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/__init__.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.903650 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     1154 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    15248 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.903866 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/
--rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    13757 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.904876 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/
--rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/__init__.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.905962 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/
--rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     6909 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     3436 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     1045 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)      333 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)      931 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     1576 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     7284 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     6899 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)      367 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/base_model.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    12792 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     6099 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     2709 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     5207 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     8552 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     7869 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     2390 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/builder.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     7362 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/depth_model.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.906572 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/layers/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     1153 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/layers/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     8693 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/layers/attractor.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     4838 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     6733 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     4163 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     3438 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/model_io.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.907033 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     1270 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     1587 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth.json
--rw-r--r--   0 sayakpaul   (501) staff       (20)      556 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth_kitti.json
--rw-r--r--   0 sayakpaul   (501) staff       (20)    12630 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.907400 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     1276 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)     1968 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/config_zoedepth_nk.json
--rw-r--r--   0 sayakpaul   (501) staff       (20)    16264 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.907821 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/utils/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     1154 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/utils/__init__.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)      624 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/utils/arg_utils.py
--rw-r--r--   0 sayakpaul   (501) staff       (20)    16310 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/utils/config.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.907963 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/utils/easydict/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     3426 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.889199 controlnet_aux-0.0.8/src/controlnet_aux.egg-info/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     6095 2024-04-12 08:22:28.000000 controlnet_aux-0.0.8/src/controlnet_aux.egg-info/PKG-INFO
--rw-r--r--   0 sayakpaul   (501) staff       (20)     8989 2024-04-12 08:22:28.000000 controlnet_aux-0.0.8/src/controlnet_aux.egg-info/SOURCES.txt
--rw-r--r--   0 sayakpaul   (501) staff       (20)        1 2024-04-12 08:22:28.000000 controlnet_aux-0.0.8/src/controlnet_aux.egg-info/dependency_links.txt
--rw-r--r--   0 sayakpaul   (501) staff       (20)      136 2024-04-12 08:22:28.000000 controlnet_aux-0.0.8/src/controlnet_aux.egg-info/requires.txt
--rw-r--r--   0 sayakpaul   (501) staff       (20)       15 2024-04-12 08:22:28.000000 controlnet_aux-0.0.8/src/controlnet_aux.egg-info/top_level.txt
-drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.908070 controlnet_aux-0.0.8/tests/
--rw-r--r--   0 sayakpaul   (501) staff       (20)     4855 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/tests/test_controlnet_aux.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.034411 controlnet_aux-0.0.9/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    11357 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/LICENSE.txt
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     6218 2024-05-23 03:25:10.034282 controlnet_aux-0.0.9/PKG-INFO
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     5287 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/README.md
+-rw-r--r--   0 sayakpaul   (501) staff       (20)       38 2024-05-23 03:25:10.034454 controlnet_aux-0.0.9/setup.cfg
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     8785 2024-05-23 03:24:04.000000 controlnet_aux-0.0.9/setup.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.001876 controlnet_aux-0.0.9/src/
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.007340 controlnet_aux-0.0.9/src/controlnet_aux/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      704 2024-05-23 03:24:04.000000 controlnet_aux-0.0.9/src/controlnet_aux/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.008272 controlnet_aux-0.0.9/src/controlnet_aux/anyline/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3986 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/anyline/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.008419 controlnet_aux-0.0.9/src/controlnet_aux/canny/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1353 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/canny/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.008833 controlnet_aux-0.0.9/src/controlnet_aux/dwpose/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2996 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/dwpose/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    10660 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/dwpose/util.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     4576 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/dwpose/wholebody.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.008982 controlnet_aux-0.0.9/src/controlnet_aux/hed/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     5791 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/hed/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.009132 controlnet_aux-0.0.9/src/controlnet_aux/leres/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     4465 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/leres/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.010102 controlnet_aux-0.0.9/src/controlnet_aux/leres/leres/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     6241 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/leres/leres/Resnet.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     8547 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/leres/leres/Resnext_torch.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/leres/leres/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    22911 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/leres/leres/depthmap.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1122 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/leres/leres/multi_depth_model_woauxi.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2029 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/leres/leres/net_tools.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    16887 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/leres/leres/network_auxi.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.010248 controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.010837 controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/models/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3095 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/models/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    10714 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/models/base_model.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1660 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/models/base_model_hg.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    28960 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/models/networks.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     7404 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/models/pix2pix4depth_model.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.011221 controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/options/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      136 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/options/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     9364 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/options/base_options.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1062 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/options/test_options.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.011447 controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/util/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)       83 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/util/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3110 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/util/util.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.011565 controlnet_aux-0.0.9/src/controlnet_aux/lineart/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     5899 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/lineart/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.011677 controlnet_aux-0.0.9/src/controlnet_aux/lineart_anime/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     8263 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/lineart_anime/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.011790 controlnet_aux-0.0.9/src/controlnet_aux/lineart_standard/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1482 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/lineart_standard/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.012062 controlnet_aux-0.0.9/src/controlnet_aux/mediapipe_face/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1944 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/mediapipe_face/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     7118 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/mediapipe_face/mediapipe_face_common.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.012431 controlnet_aux-0.0.9/src/controlnet_aux/midas/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3640 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/midas/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     5276 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/midas/api.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.013390 controlnet_aux-0.0.9/src/controlnet_aux/midas/midas/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/midas/midas/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      367 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/midas/midas/base_model.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     9242 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/midas/midas/blocks.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3154 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/midas/midas/dpt_depth.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2709 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/midas/midas/midas_net.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     5207 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/midas/midas/midas_net_custom.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     7869 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/midas/midas/transforms.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    14625 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/midas/midas/vit.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     4582 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/midas/utils.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.013634 controlnet_aux-0.0.9/src/controlnet_aux/mlsd/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2875 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/mlsd/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.013985 controlnet_aux-0.0.9/src/controlnet_aux/mlsd/models/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/mlsd/models/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     9678 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     9180 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    24189 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/mlsd/utils.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.014107 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3706 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.014482 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      597 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/NNET.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2980 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/baseline.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.014955 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    10480 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/decoder.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.016328 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2428 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     5993 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.017528 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      206 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.018023 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     4170 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2690 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2294 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     4549 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3350 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    12093 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    26514 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    59925 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2833 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    15009 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      707 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)       22 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/version.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2730 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     5821 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2932 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      843 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     4905 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1737 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1297 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     6632 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1060 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/encoder.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     5703 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/submodules.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.018766 controlnet_aux-0.0.9/src/controlnet_aux/open_pose/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     9606 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/open_pose/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    12428 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/open_pose/body.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    13491 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/open_pose/face.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3210 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/open_pose/hand.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     8743 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/open_pose/model.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    13742 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/open_pose/util.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.019000 controlnet_aux-0.0.9/src/controlnet_aux/pidi/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3190 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/pidi/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    21813 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/pidi/model.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     6259 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/processor.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.019515 controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3364 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    15148 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/automatic_mask_generator.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     4695 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/build_sam.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.020533 controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/modeling/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      419 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/modeling/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1479 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/modeling/common.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    14420 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/modeling/image_encoder.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     6615 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/modeling/mask_decoder.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     8594 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/modeling/prompt_encoder.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     7283 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/modeling/sam.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    24707 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/modeling/tiny_vit_sam.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     8397 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/modeling/transformer.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    11633 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/predictor.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.027603 controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/utils/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      197 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/utils/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    12712 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/utils/amg.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     5812 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/utils/onnx.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3972 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/utils/transforms.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.027738 controlnet_aux-0.0.9/src/controlnet_aux/shuffle/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3330 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/shuffle/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.028196 controlnet_aux-0.0.9/src/controlnet_aux/teed/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      483 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/teed/Fsmish.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1017 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/teed/Xsmish.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2632 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/teed/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    10516 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/teed/ted.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     5434 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/util.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.028313 controlnet_aux-0.0.9/src/controlnet_aux/zoe/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2972 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.028432 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.029033 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1154 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.029310 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1154 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    15248 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.029534 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    13757 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.030494 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.031565 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     6909 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3436 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1045 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      333 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      931 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1576 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     7284 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     6899 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      367 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/base_model.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    12792 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     6099 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2709 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     5207 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     8552 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     7869 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2390 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/builder.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     7362 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/depth_model.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.032193 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/layers/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1153 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/layers/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     8693 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/layers/attractor.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     4838 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     6733 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     4163 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3438 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/model_io.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.032928 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/zoedepth/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1270 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1587 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth.json
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      556 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth_kitti.json
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    12630 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.033368 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1276 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1968 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/config_zoedepth_nk.json
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    16264 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.033764 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/utils/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1154 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/utils/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      624 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/utils/arg_utils.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    16310 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/utils/config.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.033903 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/utils/easydict/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3426 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.008131 controlnet_aux-0.0.9/src/controlnet_aux.egg-info/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     6218 2024-05-23 03:25:09.000000 controlnet_aux-0.0.9/src/controlnet_aux.egg-info/PKG-INFO
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     9211 2024-05-23 03:25:09.000000 controlnet_aux-0.0.9/src/controlnet_aux.egg-info/SOURCES.txt
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        1 2024-05-23 03:25:09.000000 controlnet_aux-0.0.9/src/controlnet_aux.egg-info/dependency_links.txt
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      136 2024-05-23 03:25:09.000000 controlnet_aux-0.0.9/src/controlnet_aux.egg-info/requires.txt
+-rw-r--r--   0 sayakpaul   (501) staff       (20)       15 2024-05-23 03:25:09.000000 controlnet_aux-0.0.9/src/controlnet_aux.egg-info/top_level.txt
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-05-23 03:25:10.034049 controlnet_aux-0.0.9/tests/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     4855 2024-05-23 03:21:27.000000 controlnet_aux-0.0.9/tests/test_controlnet_aux.py
```

### Comparing `controlnet_aux-0.0.8/LICENSE.txt` & `controlnet_aux-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/PKG-INFO` & `controlnet_aux-0.0.9/src/controlnet_aux.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: controlnet_aux
-Version: 0.0.8
+Name: controlnet-aux
+Version: 0.0.9
 Summary: Auxillary models for controlnet
 Home-page: https://github.com/patrickvonplaten/controlnet_aux
 Author: The HuggingFace team
 Author-email: patrick@huggingface.co
 License: Apache
 Keywords: deep learning
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,53 +17,43 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: torch
-Requires-Dist: importlib_metadata
-Requires-Dist: huggingface_hub
-Requires-Dist: scipy
-Requires-Dist: opencv-python-headless
-Requires-Dist: filelock
-Requires-Dist: numpy
-Requires-Dist: Pillow
-Requires-Dist: einops
-Requires-Dist: torchvision
-Requires-Dist: timm<=0.6.7
-Requires-Dist: scikit-image
 
 # ControlNet auxiliary models
 
 This is a PyPi installable package of [lllyasviel's ControlNet Annotators](https://github.com/lllyasviel/ControlNet/tree/main/annotator)
 
-The code is copy-pasted from the respective folders in https://github.com/lllyasviel/ControlNet/tree/main/annotator and connected to [the 🤗 Hub](https://huggingface.co/lllyasviel/Annotators).
+The code is copy-pasted from the respective folders in <https://github.com/lllyasviel/ControlNet/tree/main/annotator> and connected to [the 🤗 Hub](https://huggingface.co/lllyasviel/Annotators).
 
-All credit & copyright goes to https://github.com/lllyasviel .
+All credit & copyright goes to <https://github.com/lllyasviel> .
 
 ## Install
 
 ```
-pip install controlnet-aux==0.0.7
+pip install -U controlnet-aux
 ```
 
 To support DWPose which is dependent on MMDetection, MMCV and MMPose
+
 ```
 pip install -U openmim
 mim install mmengine
 mim install "mmcv>=2.0.1"
 mim install "mmdet>=3.1.0"
 mim install "mmpose>=1.1.0"
 ```
-## Usage
 
+## Usage
 
 You can use the processor class, which can load each of the auxiliary models with the following code
+
 ```python
 import requests
 from PIL import Image
 from io import BytesIO
 
 from controlnet_aux.processor import Processor
 
@@ -83,14 +73,15 @@
 processor_id = 'scribble_hed'
 processor = Processor(processor_id)
 
 processed_image = processor(img, to_pil=True)
 ```
 
 Each model can be loaded individually by importing and instantiating them as follows
+
 ```python
 from PIL import Image
 import requests
 from io import BytesIO
 from controlnet_aux import HEDdetector, MidasDetector, MLSDdetector, OpenposeDetector, PidiNetDetector, NormalBaeDetector, LineartDetector, LineartAnimeDetector, CannyDetector, ContentShuffleDetector, ZoeDetector, MediapipeFaceDetector, SamDetector, LeresDetector, DWposeDetector
 
 # load image
@@ -108,45 +99,53 @@
 normal_bae = NormalBaeDetector.from_pretrained("lllyasviel/Annotators")
 lineart = LineartDetector.from_pretrained("lllyasviel/Annotators")
 lineart_anime = LineartAnimeDetector.from_pretrained("lllyasviel/Annotators")
 zoe = ZoeDetector.from_pretrained("lllyasviel/Annotators")
 sam = SamDetector.from_pretrained("ybelkada/segment-anything", subfolder="checkpoints")
 mobile_sam = SamDetector.from_pretrained("dhkim2810/MobileSAM", model_type="vit_t", filename="mobile_sam.pt")
 leres = LeresDetector.from_pretrained("lllyasviel/Annotators")
+teed = TEEDdetector.from_pretrained("fal-ai/teed", filename="5_model.pth")
+anyline = AnylineDetector.from_pretrained(
+    "TheMistoAI/MistoLine", filename="MTEED.pth", subfolder="Anyline"
+)
 
 # specify configs, ckpts and device, or it will be downloaded automatically and use cpu by default
 # det_config: ./src/controlnet_aux/dwpose/yolox_config/yolox_l_8xb8-300e_coco.py
 # det_ckpt: https://download.openmmlab.com/mmdetection/v2.0/yolox/yolox_l_8x8_300e_coco/yolox_l_8x8_300e_coco_20211126_140236-d3bd2b23.pth
 # pose_config: ./src/controlnet_aux/dwpose/dwpose_config/dwpose-l_384x288.py
 # pose_ckpt: https://huggingface.co/wanghaofan/dw-ll_ucoco_384/resolve/main/dw-ll_ucoco_384.pth
 import torch
 device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
 dwpose = DWposeDetector(det_config=det_config, det_ckpt=det_ckpt, pose_config=pose_config, pose_ckpt=pose_ckpt, device=device)
 
 # instantiate
 canny = CannyDetector()
 content = ContentShuffleDetector()
 face_detector = MediapipeFaceDetector()
+lineart_standard = LineartStandardDetector()
 
 
 # process
 processed_image_hed = hed(img)
 processed_image_midas = midas(img)
 processed_image_mlsd = mlsd(img)
 processed_image_open_pose = open_pose(img, hand_and_face=True)
 processed_image_pidi = pidi(img, safe=True)
 processed_image_normal_bae = normal_bae(img)
 processed_image_lineart = lineart(img, coarse=True)
 processed_image_lineart_anime = lineart_anime(img)
 processed_image_zoe = zoe(img)
 processed_image_sam = sam(img)
 processed_image_leres = leres(img)
+processed_image_teed = teed(img, detect_resolution=1024)
+processed_image_anyline = anyline(img, detect_resolution=1280)
 
 processed_image_canny = canny(img)
 processed_image_content = content(img)
 processed_image_mediapipe_face = face_detector(img)
 processed_image_dwpose = dwpose(img)
+processed_image_lineart_standard = lineart_standard(img, detect_resolution=1024)
 ```
 
 ### Image resolution
 
 In order to maintain the image aspect ratio, `detect_resolution`, `image_resolution` and images sizes need to be using multiple of `64`.
```

### Comparing `controlnet_aux-0.0.8/README.md` & `controlnet_aux-0.0.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 # ControlNet auxiliary models
 
 This is a PyPi installable package of [lllyasviel's ControlNet Annotators](https://github.com/lllyasviel/ControlNet/tree/main/annotator)
 
-The code is copy-pasted from the respective folders in https://github.com/lllyasviel/ControlNet/tree/main/annotator and connected to [the 🤗 Hub](https://huggingface.co/lllyasviel/Annotators).
+The code is copy-pasted from the respective folders in <https://github.com/lllyasviel/ControlNet/tree/main/annotator> and connected to [the 🤗 Hub](https://huggingface.co/lllyasviel/Annotators).
 
-All credit & copyright goes to https://github.com/lllyasviel .
+All credit & copyright goes to <https://github.com/lllyasviel> .
 
 ## Install
 
 ```
-pip install controlnet-aux==0.0.7
+pip install -U controlnet-aux
 ```
 
 To support DWPose which is dependent on MMDetection, MMCV and MMPose
+
 ```
 pip install -U openmim
 mim install mmengine
 mim install "mmcv>=2.0.1"
 mim install "mmdet>=3.1.0"
 mim install "mmpose>=1.1.0"
 ```
-## Usage
 
+## Usage
 
 You can use the processor class, which can load each of the auxiliary models with the following code
+
 ```python
 import requests
 from PIL import Image
 from io import BytesIO
 
 from controlnet_aux.processor import Processor
 
@@ -47,14 +49,15 @@
 processor_id = 'scribble_hed'
 processor = Processor(processor_id)
 
 processed_image = processor(img, to_pil=True)
 ```
 
 Each model can be loaded individually by importing and instantiating them as follows
+
 ```python
 from PIL import Image
 import requests
 from io import BytesIO
 from controlnet_aux import HEDdetector, MidasDetector, MLSDdetector, OpenposeDetector, PidiNetDetector, NormalBaeDetector, LineartDetector, LineartAnimeDetector, CannyDetector, ContentShuffleDetector, ZoeDetector, MediapipeFaceDetector, SamDetector, LeresDetector, DWposeDetector
 
 # load image
@@ -72,45 +75,53 @@
 normal_bae = NormalBaeDetector.from_pretrained("lllyasviel/Annotators")
 lineart = LineartDetector.from_pretrained("lllyasviel/Annotators")
 lineart_anime = LineartAnimeDetector.from_pretrained("lllyasviel/Annotators")
 zoe = ZoeDetector.from_pretrained("lllyasviel/Annotators")
 sam = SamDetector.from_pretrained("ybelkada/segment-anything", subfolder="checkpoints")
 mobile_sam = SamDetector.from_pretrained("dhkim2810/MobileSAM", model_type="vit_t", filename="mobile_sam.pt")
 leres = LeresDetector.from_pretrained("lllyasviel/Annotators")
+teed = TEEDdetector.from_pretrained("fal-ai/teed", filename="5_model.pth")
+anyline = AnylineDetector.from_pretrained(
+    "TheMistoAI/MistoLine", filename="MTEED.pth", subfolder="Anyline"
+)
 
 # specify configs, ckpts and device, or it will be downloaded automatically and use cpu by default
 # det_config: ./src/controlnet_aux/dwpose/yolox_config/yolox_l_8xb8-300e_coco.py
 # det_ckpt: https://download.openmmlab.com/mmdetection/v2.0/yolox/yolox_l_8x8_300e_coco/yolox_l_8x8_300e_coco_20211126_140236-d3bd2b23.pth
 # pose_config: ./src/controlnet_aux/dwpose/dwpose_config/dwpose-l_384x288.py
 # pose_ckpt: https://huggingface.co/wanghaofan/dw-ll_ucoco_384/resolve/main/dw-ll_ucoco_384.pth
 import torch
 device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
 dwpose = DWposeDetector(det_config=det_config, det_ckpt=det_ckpt, pose_config=pose_config, pose_ckpt=pose_ckpt, device=device)
 
 # instantiate
 canny = CannyDetector()
 content = ContentShuffleDetector()
 face_detector = MediapipeFaceDetector()
+lineart_standard = LineartStandardDetector()
 
 
 # process
 processed_image_hed = hed(img)
 processed_image_midas = midas(img)
 processed_image_mlsd = mlsd(img)
 processed_image_open_pose = open_pose(img, hand_and_face=True)
 processed_image_pidi = pidi(img, safe=True)
 processed_image_normal_bae = normal_bae(img)
 processed_image_lineart = lineart(img, coarse=True)
 processed_image_lineart_anime = lineart_anime(img)
 processed_image_zoe = zoe(img)
 processed_image_sam = sam(img)
 processed_image_leres = leres(img)
+processed_image_teed = teed(img, detect_resolution=1024)
+processed_image_anyline = anyline(img, detect_resolution=1280)
 
 processed_image_canny = canny(img)
 processed_image_content = content(img)
 processed_image_mediapipe_face = face_detector(img)
 processed_image_dwpose = dwpose(img)
+processed_image_lineart_standard = lineart_standard(img, detect_resolution=1024)
 ```
 
 ### Image resolution
 
 In order to maintain the image aspect ratio, `detect_resolution`, `image_resolution` and images sizes need to be using multiple of `64`.
```

### Comparing `controlnet_aux-0.0.8/setup.py` & `controlnet_aux-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
     deps["torchvision"],
     deps["timm"],
     deps["scikit-image"],
 ]
 
 setup(
     name="controlnet_aux",
-    version="0.0.8",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
+    version="0.0.9",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
     description="Auxillary models for controlnet",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning",
     license="Apache",
     author="The HuggingFace team",
     author_email="patrick@huggingface.co",
```

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
+from .anyline import AnylineDetector
+from .canny import CannyDetector
+from .dwpose import DWposeDetector
 from .hed import HEDdetector
 from .leres import LeresDetector
 from .lineart import LineartDetector
 from .lineart_anime import LineartAnimeDetector
+from .lineart_standard import LineartStandardDetector
+from .mediapipe_face import MediapipeFaceDetector
 from .midas import MidasDetector
 from .mlsd import MLSDdetector
 from .normalbae import NormalBaeDetector
 from .open_pose import OpenposeDetector
 from .pidi import PidiNetDetector
-from .zoe import ZoeDetector
-
-from .canny import CannyDetector
-from .mediapipe_face import MediapipeFaceDetector
 from .segment_anything import SamDetector
 from .shuffle import ContentShuffleDetector
-from .dwpose import DWposeDetector
+from .teed import TEEDdetector
+from .zoe import ZoeDetector
```

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/canny/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/canny/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/dwpose/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/dwpose/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/dwpose/util.py` & `controlnet_aux-0.0.9/src/controlnet_aux/dwpose/util.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/dwpose/wholebody.py` & `controlnet_aux-0.0.9/src/controlnet_aux/dwpose/wholebody.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/hed/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/hed/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/leres/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/leres/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/Resnet.py` & `controlnet_aux-0.0.9/src/controlnet_aux/leres/leres/Resnet.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/Resnext_torch.py` & `controlnet_aux-0.0.9/src/controlnet_aux/leres/leres/Resnext_torch.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/depthmap.py` & `controlnet_aux-0.0.9/src/controlnet_aux/leres/leres/depthmap.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/multi_depth_model_woauxi.py` & `controlnet_aux-0.0.9/src/controlnet_aux/leres/leres/multi_depth_model_woauxi.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/net_tools.py` & `controlnet_aux-0.0.9/src/controlnet_aux/leres/leres/net_tools.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/network_auxi.py` & `controlnet_aux-0.0.9/src/controlnet_aux/leres/leres/network_auxi.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/models/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/models/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/models/base_model.py` & `controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/models/base_model.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/models/base_model_hg.py` & `controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/models/base_model_hg.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/models/networks.py` & `controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/models/networks.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/models/pix2pix4depth_model.py` & `controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/models/pix2pix4depth_model.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/options/base_options.py` & `controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/options/base_options.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/options/test_options.py` & `controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/options/test_options.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/util/util.py` & `controlnet_aux-0.0.9/src/controlnet_aux/leres/pix2pix/util/util.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/lineart/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/lineart/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/lineart_anime/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/lineart_anime/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/mediapipe_face/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/mediapipe_face/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/mediapipe_face/mediapipe_face_common.py` & `controlnet_aux-0.0.9/src/controlnet_aux/mediapipe_face/mediapipe_face_common.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/midas/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/midas/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/midas/api.py` & `controlnet_aux-0.0.9/src/controlnet_aux/midas/api.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/blocks.py` & `controlnet_aux-0.0.9/src/controlnet_aux/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/dpt_depth.py` & `controlnet_aux-0.0.9/src/controlnet_aux/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/midas_net.py` & `controlnet_aux-0.0.9/src/controlnet_aux/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/midas_net_custom.py` & `controlnet_aux-0.0.9/src/controlnet_aux/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/transforms.py` & `controlnet_aux-0.0.9/src/controlnet_aux/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/vit.py` & `controlnet_aux-0.0.9/src/controlnet_aux/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/midas/utils.py` & `controlnet_aux-0.0.9/src/controlnet_aux/midas/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/mlsd/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/mlsd/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py` & `controlnet_aux-0.0.9/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py` & `controlnet_aux-0.0.9/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/mlsd/utils.py` & `controlnet_aux-0.0.9/src/controlnet_aux/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/NNET.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/NNET.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/baseline.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/baseline.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/decoder.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/decoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/encoder.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/encoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/submodules.py` & `controlnet_aux-0.0.9/src/controlnet_aux/normalbae/nets/submodules/submodules.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/open_pose/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/open_pose/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/open_pose/body.py` & `controlnet_aux-0.0.9/src/controlnet_aux/open_pose/body.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/open_pose/face.py` & `controlnet_aux-0.0.9/src/controlnet_aux/open_pose/face.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/open_pose/hand.py` & `controlnet_aux-0.0.9/src/controlnet_aux/open_pose/hand.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/open_pose/model.py` & `controlnet_aux-0.0.9/src/controlnet_aux/open_pose/model.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/open_pose/util.py` & `controlnet_aux-0.0.9/src/controlnet_aux/open_pose/util.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/pidi/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/pidi/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/pidi/model.py` & `controlnet_aux-0.0.9/src/controlnet_aux/pidi/model.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/processor.py` & `controlnet_aux-0.0.9/src/controlnet_aux/processor.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/automatic_mask_generator.py` & `controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/build_sam.py` & `controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/common.py` & `controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/image_encoder.py` & `controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/mask_decoder.py` & `controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/prompt_encoder.py` & `controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/sam.py` & `controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/tiny_vit_sam.py` & `controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/modeling/tiny_vit_sam.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/transformer.py` & `controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/predictor.py` & `controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/utils/amg.py` & `controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/utils/onnx.py` & `controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/utils/transforms.py` & `controlnet_aux-0.0.9/src/controlnet_aux/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/shuffle/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/shuffle/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/util.py` & `controlnet_aux-0.0.9/src/controlnet_aux/util.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/builder.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/builder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/depth_model.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/depth_model.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/layers/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/layers/attractor.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/layers/attractor.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/model_io.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/model_io.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth.json` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth.json`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth_kitti.json` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth_kitti.json`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/config_zoedepth_nk.json` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/config_zoedepth_nk.json`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/utils/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/utils/arg_utils.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/utils/arg_utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/utils/config.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/utils/config.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py` & `controlnet_aux-0.0.9/src/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux.egg-info/PKG-INFO` & `controlnet_aux-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: controlnet-aux
-Version: 0.0.8
+Name: controlnet_aux
+Version: 0.0.9
 Summary: Auxillary models for controlnet
 Home-page: https://github.com/patrickvonplaten/controlnet_aux
 Author: The HuggingFace team
 Author-email: patrick@huggingface.co
 License: Apache
 Keywords: deep learning
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,53 +17,43 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: torch
-Requires-Dist: importlib_metadata
-Requires-Dist: huggingface_hub
-Requires-Dist: scipy
-Requires-Dist: opencv-python-headless
-Requires-Dist: filelock
-Requires-Dist: numpy
-Requires-Dist: Pillow
-Requires-Dist: einops
-Requires-Dist: torchvision
-Requires-Dist: timm<=0.6.7
-Requires-Dist: scikit-image
 
 # ControlNet auxiliary models
 
 This is a PyPi installable package of [lllyasviel's ControlNet Annotators](https://github.com/lllyasviel/ControlNet/tree/main/annotator)
 
-The code is copy-pasted from the respective folders in https://github.com/lllyasviel/ControlNet/tree/main/annotator and connected to [the 🤗 Hub](https://huggingface.co/lllyasviel/Annotators).
+The code is copy-pasted from the respective folders in <https://github.com/lllyasviel/ControlNet/tree/main/annotator> and connected to [the 🤗 Hub](https://huggingface.co/lllyasviel/Annotators).
 
-All credit & copyright goes to https://github.com/lllyasviel .
+All credit & copyright goes to <https://github.com/lllyasviel> .
 
 ## Install
 
 ```
-pip install controlnet-aux==0.0.7
+pip install -U controlnet-aux
 ```
 
 To support DWPose which is dependent on MMDetection, MMCV and MMPose
+
 ```
 pip install -U openmim
 mim install mmengine
 mim install "mmcv>=2.0.1"
 mim install "mmdet>=3.1.0"
 mim install "mmpose>=1.1.0"
 ```
-## Usage
 
+## Usage
 
 You can use the processor class, which can load each of the auxiliary models with the following code
+
 ```python
 import requests
 from PIL import Image
 from io import BytesIO
 
 from controlnet_aux.processor import Processor
 
@@ -83,14 +73,15 @@
 processor_id = 'scribble_hed'
 processor = Processor(processor_id)
 
 processed_image = processor(img, to_pil=True)
 ```
 
 Each model can be loaded individually by importing and instantiating them as follows
+
 ```python
 from PIL import Image
 import requests
 from io import BytesIO
 from controlnet_aux import HEDdetector, MidasDetector, MLSDdetector, OpenposeDetector, PidiNetDetector, NormalBaeDetector, LineartDetector, LineartAnimeDetector, CannyDetector, ContentShuffleDetector, ZoeDetector, MediapipeFaceDetector, SamDetector, LeresDetector, DWposeDetector
 
 # load image
@@ -108,45 +99,53 @@
 normal_bae = NormalBaeDetector.from_pretrained("lllyasviel/Annotators")
 lineart = LineartDetector.from_pretrained("lllyasviel/Annotators")
 lineart_anime = LineartAnimeDetector.from_pretrained("lllyasviel/Annotators")
 zoe = ZoeDetector.from_pretrained("lllyasviel/Annotators")
 sam = SamDetector.from_pretrained("ybelkada/segment-anything", subfolder="checkpoints")
 mobile_sam = SamDetector.from_pretrained("dhkim2810/MobileSAM", model_type="vit_t", filename="mobile_sam.pt")
 leres = LeresDetector.from_pretrained("lllyasviel/Annotators")
+teed = TEEDdetector.from_pretrained("fal-ai/teed", filename="5_model.pth")
+anyline = AnylineDetector.from_pretrained(
+    "TheMistoAI/MistoLine", filename="MTEED.pth", subfolder="Anyline"
+)
 
 # specify configs, ckpts and device, or it will be downloaded automatically and use cpu by default
 # det_config: ./src/controlnet_aux/dwpose/yolox_config/yolox_l_8xb8-300e_coco.py
 # det_ckpt: https://download.openmmlab.com/mmdetection/v2.0/yolox/yolox_l_8x8_300e_coco/yolox_l_8x8_300e_coco_20211126_140236-d3bd2b23.pth
 # pose_config: ./src/controlnet_aux/dwpose/dwpose_config/dwpose-l_384x288.py
 # pose_ckpt: https://huggingface.co/wanghaofan/dw-ll_ucoco_384/resolve/main/dw-ll_ucoco_384.pth
 import torch
 device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
 dwpose = DWposeDetector(det_config=det_config, det_ckpt=det_ckpt, pose_config=pose_config, pose_ckpt=pose_ckpt, device=device)
 
 # instantiate
 canny = CannyDetector()
 content = ContentShuffleDetector()
 face_detector = MediapipeFaceDetector()
+lineart_standard = LineartStandardDetector()
 
 
 # process
 processed_image_hed = hed(img)
 processed_image_midas = midas(img)
 processed_image_mlsd = mlsd(img)
 processed_image_open_pose = open_pose(img, hand_and_face=True)
 processed_image_pidi = pidi(img, safe=True)
 processed_image_normal_bae = normal_bae(img)
 processed_image_lineart = lineart(img, coarse=True)
 processed_image_lineart_anime = lineart_anime(img)
 processed_image_zoe = zoe(img)
 processed_image_sam = sam(img)
 processed_image_leres = leres(img)
+processed_image_teed = teed(img, detect_resolution=1024)
+processed_image_anyline = anyline(img, detect_resolution=1280)
 
 processed_image_canny = canny(img)
 processed_image_content = content(img)
 processed_image_mediapipe_face = face_detector(img)
 processed_image_dwpose = dwpose(img)
+processed_image_lineart_standard = lineart_standard(img, detect_resolution=1024)
 ```
 
 ### Image resolution
 
 In order to maintain the image aspect ratio, `detect_resolution`, `image_resolution` and images sizes need to be using multiple of `64`.
```

### Comparing `controlnet_aux-0.0.8/src/controlnet_aux.egg-info/SOURCES.txt` & `controlnet_aux-0.0.9/src/controlnet_aux.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/controlnet_aux/processor.py
 src/controlnet_aux/util.py
 src/controlnet_aux.egg-info/PKG-INFO
 src/controlnet_aux.egg-info/SOURCES.txt
 src/controlnet_aux.egg-info/dependency_links.txt
 src/controlnet_aux.egg-info/requires.txt
 src/controlnet_aux.egg-info/top_level.txt
+src/controlnet_aux/anyline/__init__.py
 src/controlnet_aux/canny/__init__.py
 src/controlnet_aux/dwpose/__init__.py
 src/controlnet_aux/dwpose/util.py
 src/controlnet_aux/dwpose/wholebody.py
 src/controlnet_aux/hed/__init__.py
 src/controlnet_aux/leres/__init__.py
 src/controlnet_aux/leres/leres/Resnet.py
@@ -31,14 +32,15 @@
 src/controlnet_aux/leres/pix2pix/options/__init__.py
 src/controlnet_aux/leres/pix2pix/options/base_options.py
 src/controlnet_aux/leres/pix2pix/options/test_options.py
 src/controlnet_aux/leres/pix2pix/util/__init__.py
 src/controlnet_aux/leres/pix2pix/util/util.py
 src/controlnet_aux/lineart/__init__.py
 src/controlnet_aux/lineart_anime/__init__.py
+src/controlnet_aux/lineart_standard/__init__.py
 src/controlnet_aux/mediapipe_face/__init__.py
 src/controlnet_aux/mediapipe_face/mediapipe_face_common.py
 src/controlnet_aux/midas/__init__.py
 src/controlnet_aux/midas/api.py
 src/controlnet_aux/midas/utils.py
 src/controlnet_aux/midas/midas/__init__.py
 src/controlnet_aux/midas/midas/base_model.py
@@ -106,14 +108,18 @@
 src/controlnet_aux/segment_anything/modeling/tiny_vit_sam.py
 src/controlnet_aux/segment_anything/modeling/transformer.py
 src/controlnet_aux/segment_anything/utils/__init__.py
 src/controlnet_aux/segment_anything/utils/amg.py
 src/controlnet_aux/segment_anything/utils/onnx.py
 src/controlnet_aux/segment_anything/utils/transforms.py
 src/controlnet_aux/shuffle/__init__.py
+src/controlnet_aux/teed/Fsmish.py
+src/controlnet_aux/teed/Xsmish.py
+src/controlnet_aux/teed/__init__.py
+src/controlnet_aux/teed/ted.py
 src/controlnet_aux/zoe/__init__.py
 src/controlnet_aux/zoe/zoedepth/__init__.py
 src/controlnet_aux/zoe/zoedepth/models/__init__.py
 src/controlnet_aux/zoe/zoedepth/models/builder.py
 src/controlnet_aux/zoe/zoedepth/models/depth_model.py
 src/controlnet_aux/zoe/zoedepth/models/model_io.py
 src/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py
```

### Comparing `controlnet_aux-0.0.8/tests/test_controlnet_aux.py` & `controlnet_aux-0.0.9/tests/test_controlnet_aux.py`

 * *Files identical despite different names*

