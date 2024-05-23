# Comparing `tmp/tardis_em-0.2.4.tar.gz` & `tmp/tardis_em-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tardis_em-0.2.4.tar", last modified: Fri May 10 09:30:59 2024, max compression
+gzip compressed data, was "tardis_em-0.2.5.tar", last modified: Thu May 23 07:21:35 2024, max compression
```

## Comparing `tardis_em-0.2.4.tar` & `tardis_em-0.2.5.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-10 09:30:59.809619 tardis_em-0.2.4/
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     1108 2022-10-24 14:55:09.000000 tardis_em-0.2.4/LICENSE
--rw-r--r--   0 robertkiewisz   (501) staff       (20)      103 2023-11-22 08:39:36.000000 tardis_em-0.2.4/MANIFEST.in
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     3027 2024-05-10 09:30:59.809536 tardis_em-0.2.4/PKG-INFO
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     5054 2024-05-10 09:30:49.000000 tardis_em-0.2.4/README.rst
--rw-r--r--   0 robertkiewisz   (501) staff       (20)      200 2023-11-22 08:39:31.000000 tardis_em-0.2.4/pyproject.toml
--rw-r--r--   0 robertkiewisz   (501) staff       (20)      592 2024-05-09 13:48:31.000000 tardis_em-0.2.4/requirements.txt
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     1806 2024-05-10 09:30:59.809960 tardis_em-0.2.4/setup.cfg
--rw-r--r--   0 robertkiewisz   (501) staff       (20)      686 2024-01-05 09:11:55.000000 tardis_em-0.2.4/setup.py
-drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-10 09:30:59.781141 tardis_em-0.2.4/tardis_em/
--rw-r--r--   0 robertkiewisz   (501) staff       (20)      239 2024-05-09 09:38:12.000000 tardis_em-0.2.4/tardis_em/__init__.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)      667 2024-05-10 09:30:49.000000 tardis_em-0.2.4/tardis_em/_version.py
-drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-10 09:30:59.782768 tardis_em-0.2.4/tardis_em/benchmarks/
--rw-r--r--   0 robertkiewisz   (501) staff       (20)        0 2023-03-22 15:14:45.000000 tardis_em-0.2.4/tardis_em/benchmarks/__init__.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     8279 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tardis_em/benchmarks/benchmarks.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    12326 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tardis_em/benchmarks/predictor.py
-drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-10 09:30:59.783913 tardis_em-0.2.4/tardis_em/cnn/
--rw-r--r--   0 robertkiewisz   (501) staff       (20)        0 2023-01-04 16:06:13.000000 tardis_em-0.2.4/tardis_em/cnn/__init__.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     4927 2024-01-10 08:08:53.000000 tardis_em-0.2.4/tardis_em/cnn/cnn.py
-drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-10 09:30:59.785399 tardis_em-0.2.4/tardis_em/cnn/data_processing/
--rw-r--r--   0 robertkiewisz   (501) staff       (20)        0 2023-01-04 16:07:43.000000 tardis_em-0.2.4/tardis_em/cnn/data_processing/__init__.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    12073 2024-05-07 15:06:01.000000 tardis_em-0.2.4/tardis_em/cnn/data_processing/draw_mask.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     5445 2024-02-15 16:58:53.000000 tardis_em-0.2.4/tardis_em/cnn/data_processing/interpolation.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    12894 2024-02-06 10:54:05.000000 tardis_em-0.2.4/tardis_em/cnn/data_processing/stitch.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    13470 2024-02-26 19:54:52.000000 tardis_em-0.2.4/tardis_em/cnn/data_processing/trim.py
-drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-10 09:30:59.786372 tardis_em-0.2.4/tardis_em/cnn/datasets/
--rw-r--r--   0 robertkiewisz   (501) staff       (20)        0 2023-01-04 16:07:24.000000 tardis_em-0.2.4/tardis_em/cnn/datasets/__init__.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     9105 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tardis_em/cnn/datasets/augmentation.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    15300 2024-01-18 14:25:52.000000 tardis_em-0.2.4/tardis_em/cnn/datasets/build_dataset.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     5450 2024-01-16 12:33:40.000000 tardis_em-0.2.4/tardis_em/cnn/datasets/dataloader.py
-drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-10 09:30:59.787891 tardis_em-0.2.4/tardis_em/cnn/model/
--rw-r--r--   0 robertkiewisz   (501) staff       (20)        0 2023-01-04 16:07:20.000000 tardis_em-0.2.4/tardis_em/cnn/model/__init__.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    13542 2024-01-17 08:23:39.000000 tardis_em-0.2.4/tardis_em/cnn/model/convolution.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    14686 2024-02-06 10:54:05.000000 tardis_em-0.2.4/tardis_em/cnn/model/decoder_blocks.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     6302 2024-02-06 10:54:05.000000 tardis_em-0.2.4/tardis_em/cnn/model/encoder_blocks.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     1897 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tardis_em/cnn/model/init_weights.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     5930 2024-01-07 16:42:10.000000 tardis_em-0.2.4/tardis_em/cnn/train.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     4398 2024-02-06 10:54:05.000000 tardis_em-0.2.4/tardis_em/cnn/trainer.py
-drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-10 09:30:59.788770 tardis_em-0.2.4/tardis_em/cnn/utils/
--rw-r--r--   0 robertkiewisz   (501) staff       (20)        0 2023-01-04 16:06:33.000000 tardis_em-0.2.4/tardis_em/cnn/utils/__init__.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    18740 2024-01-18 15:47:53.000000 tardis_em-0.2.4/tardis_em/cnn/utils/build_cnn.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    14552 2024-02-24 14:27:36.000000 tardis_em-0.2.4/tardis_em/cnn/utils/utils.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     8828 2024-05-09 09:14:43.000000 tardis_em-0.2.4/tardis_em/compare_spatial_graphs.py
-drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-10 09:30:59.790072 tardis_em-0.2.4/tardis_em/dist_pytorch/
--rw-r--r--   0 robertkiewisz   (501) staff       (20)        0 2023-01-04 16:08:56.000000 tardis_em-0.2.4/tardis_em/dist_pytorch/__init__.py
-drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-10 09:30:59.791263 tardis_em-0.2.4/tardis_em/dist_pytorch/datasets/
--rw-r--r--   0 robertkiewisz   (501) staff       (20)        0 2023-01-04 16:10:04.000000 tardis_em-0.2.4/tardis_em/dist_pytorch/datasets/__init__.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    13939 2024-02-15 16:58:53.000000 tardis_em-0.2.4/tardis_em/dist_pytorch/datasets/augmentation.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    32154 2024-02-21 13:01:04.000000 tardis_em-0.2.4/tardis_em/dist_pytorch/datasets/dataloader.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    20479 2024-02-15 16:58:53.000000 tardis_em-0.2.4/tardis_em/dist_pytorch/datasets/patches.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     9281 2024-05-03 07:51:14.000000 tardis_em-0.2.4/tardis_em/dist_pytorch/dist.py
-drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-10 09:30:59.792282 tardis_em-0.2.4/tardis_em/dist_pytorch/model/
--rw-r--r--   0 robertkiewisz   (501) staff       (20)        0 2023-01-04 16:09:41.000000 tardis_em-0.2.4/tardis_em/dist_pytorch/model/__init__.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     4993 2024-02-24 14:27:36.000000 tardis_em-0.2.4/tardis_em/dist_pytorch/model/embedding.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    12217 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tardis_em/dist_pytorch/model/layers.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    30389 2024-02-15 16:58:54.000000 tardis_em-0.2.4/tardis_em/dist_pytorch/model/modules.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     4076 2024-02-15 16:58:53.000000 tardis_em-0.2.4/tardis_em/dist_pytorch/sparse_dist.py
-drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-10 09:30:59.793388 tardis_em-0.2.4/tardis_em/dist_pytorch/sparse_model/
--rw-r--r--   0 robertkiewisz   (501) staff       (20)        0 2023-08-12 17:42:31.000000 tardis_em-0.2.4/tardis_em/dist_pytorch/sparse_model/__init__.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     7048 2024-02-15 16:58:53.000000 tardis_em-0.2.4/tardis_em/dist_pytorch/sparse_model/embedding.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     6224 2024-02-15 16:58:53.000000 tardis_em-0.2.4/tardis_em/dist_pytorch/sparse_model/layers.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     3627 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tardis_em/dist_pytorch/sparse_model/modules.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     9399 2024-02-06 10:54:05.000000 tardis_em-0.2.4/tardis_em/dist_pytorch/train.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    29804 2024-02-15 16:58:54.000000 tardis_em-0.2.4/tardis_em/dist_pytorch/trainer.py
-drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-10 09:30:59.794689 tardis_em-0.2.4/tardis_em/dist_pytorch/utils/
--rw-r--r--   0 robertkiewisz   (501) staff       (20)      648 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tardis_em/dist_pytorch/utils/__init__.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    16671 2024-05-10 09:28:06.000000 tardis_em-0.2.4/tardis_em/dist_pytorch/utils/build_point_cloud.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    18487 2024-02-26 19:54:52.000000 tardis_em-0.2.4/tardis_em/dist_pytorch/utils/segment_point_cloud.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    13528 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tardis_em/dist_pytorch/utils/utils.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     5458 2024-05-09 09:38:12.000000 tardis_em-0.2.4/tardis_em/predict_mem.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     6741 2024-05-09 09:38:12.000000 tardis_em-0.2.4/tardis_em/predict_mem_2d.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     8476 2024-05-09 09:38:12.000000 tardis_em-0.2.4/tardis_em/predict_mt.py
-drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-10 09:30:59.795572 tardis_em-0.2.4/tardis_em/scripts/
--rw-r--r--   0 robertkiewisz   (501) staff       (20)       62 2024-02-23 10:17:26.000000 tardis_em-0.2.4/tardis_em/scripts/__init__.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    16353 2024-05-08 09:23:38.000000 tardis_em-0.2.4/tardis_em/scripts/czi_predict.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     3506 2024-05-10 09:01:02.000000 tardis_em-0.2.4/tardis_em/scripts/visualize.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     2909 2024-05-09 13:54:14.000000 tardis_em-0.2.4/tardis_em/tardis.py
-drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-10 09:30:59.796088 tardis_em-0.2.4/tardis_em/tardis_helper/
--rw-r--r--   0 robertkiewisz   (501) staff       (20)        0 2023-08-13 14:46:27.000000 tardis_em-0.2.4/tardis_em/tardis_helper/__init__.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     2220 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tardis_em/tardis_helper/helper_func.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    11059 2024-05-03 07:47:21.000000 tardis_em-0.2.4/tardis_em/train_DIST.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    10248 2024-05-03 07:47:21.000000 tardis_em-0.2.4/tardis_em/train_cnn.py
-drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-10 09:30:59.802591 tardis_em-0.2.4/tardis_em/utils/
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     1192 2023-04-12 16:41:09.000000 tardis_em-0.2.4/tardis_em/utils/__init__.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    11389 2024-05-07 13:49:20.000000 tardis_em-0.2.4/tardis_em/utils/aws.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     5934 2024-01-20 14:47:45.000000 tardis_em-0.2.4/tardis_em/utils/dataset.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     2137 2024-02-21 11:14:53.000000 tardis_em-0.2.4/tardis_em/utils/device.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     5812 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tardis_em/utils/errors.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    20802 2024-05-07 14:01:05.000000 tardis_em-0.2.4/tardis_em/utils/export_data.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    29405 2024-05-07 14:01:05.000000 tardis_em-0.2.4/tardis_em/utils/load_data.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     9423 2024-02-21 11:14:53.000000 tardis_em-0.2.4/tardis_em/utils/logo.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    20740 2024-02-15 16:58:54.000000 tardis_em-0.2.4/tardis_em/utils/losses.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    12729 2024-05-07 14:01:05.000000 tardis_em-0.2.4/tardis_em/utils/metrics.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     9473 2024-02-06 10:54:05.000000 tardis_em-0.2.4/tardis_em/utils/normalization.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     4830 2024-05-03 07:34:22.000000 tardis_em-0.2.4/tardis_em/utils/ota_update.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    51965 2024-05-08 12:25:15.000000 tardis_em-0.2.4/tardis_em/utils/predictor.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     5756 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tardis_em/utils/setup_envir.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    36279 2024-02-23 20:37:05.000000 tardis_em-0.2.4/tardis_em/utils/spline_metric.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    12177 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tardis_em/utils/trainer.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     3628 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tardis_em/utils/utils.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    12260 2024-01-18 07:34:07.000000 tardis_em-0.2.4/tardis_em/utils/visualize_pc.py
-drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-10 09:30:59.808939 tardis_em-0.2.4/tardis_em.egg-info/
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     3027 2024-05-10 09:30:59.000000 tardis_em-0.2.4/tardis_em.egg-info/PKG-INFO
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     3426 2024-05-10 09:30:59.000000 tardis_em-0.2.4/tardis_em.egg-info/SOURCES.txt
--rw-r--r--   0 robertkiewisz   (501) staff       (20)        1 2024-05-10 09:30:59.000000 tardis_em-0.2.4/tardis_em.egg-info/dependency_links.txt
--rw-r--r--   0 robertkiewisz   (501) staff       (20)      515 2024-05-10 09:30:59.000000 tardis_em-0.2.4/tardis_em.egg-info/entry_points.txt
--rw-r--r--   0 robertkiewisz   (501) staff       (20)      570 2024-05-10 09:30:59.000000 tardis_em-0.2.4/tardis_em.egg-info/requires.txt
--rw-r--r--   0 robertkiewisz   (501) staff       (20)       10 2024-05-10 09:30:59.000000 tardis_em-0.2.4/tardis_em.egg-info/top_level.txt
-drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-10 09:30:59.808605 tardis_em-0.2.4/tests/
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     3863 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tests/run_all_tests.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     2209 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tests/test_cnn_build_dataset.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     3223 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tests/test_cnn_dataset.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    10136 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tests/test_cnn_draw_mask.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     1384 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tests/test_cnn_interpolation.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     7744 2024-05-08 08:58:34.000000 tardis_em-0.2.4/tests/test_cnn_nn.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     4851 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tests/test_cnn_trim_stitch.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)      648 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tests/test_cnn_utils.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     8411 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tests/test_dist_augmentation.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     7653 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tests/test_dist_data_loader.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     2828 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tests/test_dist_embedding.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     4636 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tests/test_dist_graph_cut.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     1583 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tests/test_dist_img_to_pc.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     3112 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tests/test_dist_modules.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     3412 2024-05-08 08:39:51.000000 tardis_em-0.2.4/tests/test_dist_nn.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     5233 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tests/test_dist_trainer.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     1555 2024-05-10 09:28:03.000000 tardis_em-0.2.4/tests/test_dist_utils.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     3744 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tests/test_losses.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)     2971 2024-01-05 09:11:55.000000 tardis_em-0.2.4/tests/test_trainer.py
--rw-r--r--   0 robertkiewisz   (501) staff       (20)    11123 2024-05-08 08:44:15.000000 tardis_em-0.2.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.987546 tardis_em-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-23 07:21:31.000000 tardis_em-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-23 07:21:31.000000 tardis_em-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-23 07:21:35.987546 tardis_em-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-05-23 07:21:31.000000 tardis_em-0.2.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-23 07:21:31.000000 tardis_em-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-23 07:21:31.000000 tardis_em-0.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-23 07:21:35.987546 tardis_em-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-23 07:21:31.000000 tardis_em-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.971546 tardis_em-0.2.5/tardis_em/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.975546 tardis_em-0.2.5/tardis_em/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/benchmarks/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/benchmarks/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.975546 tardis_em-0.2.5/tardis_em/cnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/cnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.975546 tardis_em-0.2.5/tardis_em/cnn/data_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/data_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12073 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/data_processing/draw_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/data_processing/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12894 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/data_processing/stitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/data_processing/trim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.975546 tardis_em-0.2.5/tardis_em/cnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/datasets/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15300 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/datasets/build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/datasets/dataloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.975546 tardis_em-0.2.5/tardis_em/cnn/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13542 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/model/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14686 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/model/decoder_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/model/encoder_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/model/init_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.979546 tardis_em-0.2.5/tardis_em/cnn/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18740 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/utils/build_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14593 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/compare_spatial_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.979546 tardis_em-0.2.5/tardis_em/dist_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.979546 tardis_em-0.2.5/tardis_em/dist_pytorch/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/datasets/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32154 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/datasets/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20479 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/datasets/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/dist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.979546 tardis_em-0.2.5/tardis_em/dist_pytorch/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/model/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30389 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/model/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/sparse_dist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.979546 tardis_em-0.2.5/tardis_em/dist_pytorch/sparse_model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/sparse_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/sparse_model/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/sparse_model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/sparse_model/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9399 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29804 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.979546 tardis_em-0.2.5/tardis_em/dist_pytorch/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16498 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/utils/build_point_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18487 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/utils/segment_point_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/predict_actin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/predict_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/predict_mem_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/predict_mt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.979546 tardis_em-0.2.5/tardis_em/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16330 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/scripts/czi_predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/scripts/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/tardis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.983546 tardis_em-0.2.5/tardis_em/tardis_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/tardis_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/tardis_helper/helper_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11061 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/train_DIST.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/train_cnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.983546 tardis_em-0.2.5/tardis_em/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20802 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/export_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29405 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20740 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/ota_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53166 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/setup_envir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38169 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/spline_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/visualize_pc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.987546 tardis_em-0.2.5/tardis_em.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-23 07:21:35.000000 tardis_em-0.2.5/tardis_em.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-23 07:21:35.000000 tardis_em-0.2.5/tardis_em.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 07:21:35.000000 tardis_em-0.2.5/tardis_em.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-23 07:21:35.000000 tardis_em-0.2.5/tardis_em.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-23 07:21:35.000000 tardis_em-0.2.5/tardis_em.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 07:21:35.000000 tardis_em-0.2.5/tardis_em.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.987546 tardis_em-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_cnn_build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_cnn_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_cnn_draw_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_cnn_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_cnn_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_cnn_trim_stitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_cnn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_dist_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_dist_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_dist_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_dist_graph_cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_dist_img_to_pc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_dist_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_dist_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_dist_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11123 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_utils.py
```

### Comparing `tardis_em-0.2.4/LICENSE` & `tardis_em-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/PKG-INFO` & `tardis_em-0.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tardis_em
-Version: 0.2.4
+Version: 0.2.5
 Summary: PyTorch segmentation of 2D/3D images such as electron tomography (ET),Cryo-EM or fluorescent microscopy data into 3D segmented point cloud.
 Home-page: https://github.com/SMLC-NYSBC/TARDIS
 Author: Robert Kiewisz, Tristan Bepler
 Author-email: rkiewisz@nysbc.org
 License: MIT
 Keywords: semantic segmentation,instance segmentation,MT segmentation,membrane segmentation,CNN,FNet,DIST
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,20 +25,18 @@
 Requires-Dist: imagecodecs>2021.11.00
 Requires-Dist: scikit-learn>1.0.1
 Requires-Dist: scikit-image>0.19.2
 Requires-Dist: scipy>=1.8.1
 Requires-Dist: pillow>10.0.0
 Requires-Dist: plyfile>=0.9
 Requires-Dist: pyvista>=0.40.0; platform_machine != "aarch64"
-Requires-Dist: open3d==0.9.0; sys_platform != "linux" and python_version < "3.8"
-Requires-Dist: open3d>=0.9.0; sys_platform != "linux" and python_version >= "3.8"
+Requires-Dist: open3d>=0.9.0; sys_platform != "linux"
 Requires-Dist: requests>2.28.0
 Requires-Dist: ipython>8.0.0
 Requires-Dist: click>8.0.4
-Requires-Dist: nvidia-smi>=0.1.3; sys_platform != "darwin"
 Requires-Dist: setuptools>=67.6.0
 Provides-Extra: docs
 Requires-Dist: sphinx<5.0; extra == "docs"
 Requires-Dist: myst_parser; extra == "docs"
 Requires-Dist: pydata_sphinx_theme; extra == "docs"
 Requires-Dist: sphinx_markdown_tables; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
```

### Comparing `tardis_em-0.2.4/README.rst` & `tardis_em-0.2.5/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 .. image:: resources/Tardis_logo_2.png
     :width: 512
     :align: center
     :target: https://smlc-nysbc.github.io/TARDIS/
 
 ========
 
-.. image:: https://img.shields.io/badge/Release-0.2.4-success
-    :target: https://shields.io
-
 .. image:: https://github.com/SMLC-NYSBC/TARDIS/actions/workflows/python_pytest.yml/badge.svg
         :target: https://github.com/SMLC-NYSBC/TARDIS/actions/workflows/python_pytest.yml
 
 .. image:: https://github.com/SMLC-NYSBC/TARDIS/actions/workflows/licensed.yml/badge.svg
         :target: https://github.com/SMLC-NYSBC/TARDIS/actions/workflows/licensed.yml
 
 .. image:: https://github.com/SMLC-NYSBC/TARDIS/actions/workflows/sphinx_documentation.yml/badge.svg
@@ -37,14 +34,15 @@
     - 2D micrograph modality microtubule segmentation will come soon!
 
 - Robust and high-throughput semantic/instance segmentation of membranes:
     - Supported file formats: [.tif, .mrc, .rec, .am]
     - Supported modality: [EM, ET, Cryo-EM, Cryo-ET]
     - Supported Å resolution: [all]
 
+- High-throughput semantic/instance segmentation of actin [Beta]
 - Fully automatic segmentation solution!
 - Napari plugin [Coming soon]
 - Cloud computing [Coming soon]
 
 Citation
 ========
 
@@ -57,15 +55,16 @@
 Kiewisz R., Bepler T. 2022. Membrane and microtubule rapid instance segmentation with dimensionless instance segmentation by learning graph representations of point clouds. Neurips 2022 - Machine Learning for Structural Biology Workshop.
 
 What's new?
 ===========
 
 `Full History <https://smlc-nysbc.github.io/TARDIS/HISTORY.html>`__
 
-TARDIS-em v0.2.4 (2024-08):
+TARDIS-em v0.2.5 (2024-05-22):
+    * Added actin segmentation
     * Improvement from Microtubule and Membrane prediction with updated models
     * Added option for scripting TARDIS predictions
     * Added visualization for semantic and instance predictions
     * TARDIS build in results visualization
     * Bug fixes
     * Documentation tutorials
     * Pypi and Conda releases
@@ -75,25 +74,57 @@
         * 3D objects like membranes mitochondria LiDAR data etc.
 
 Quick Start
 ===========
 
 For more examples and advanced usage please find more details in our `Documentation <https://smlc-nysbc.github.io/TARDIS/>`__
 
-Microtubule Prediction
-----------------------
+1) Install TARDIS-em:
 
-2D prediction
-^^^^^^^^^^^^^
+.. code-block:: bash
+
+    pip install tardis-em
+
+or
+
+.. code-block:: bash
+
+    conda install tardis-em -c rrobert92
+
+2) Verifies installation:
+
+.. code-block:: bash
+
+    tardis
+
+Filaments Prediction
+--------------------
+
+3D Actin prediction
+^^^^^^^^^^^^^^^^^^^
+Full tutorial: `3D Actin Prediction <https://smlc-nysbc.github.io/TARDIS/usage/3d_actin.html>`__
+
+Usage:
+""""""
+
+.. code-block:: bash
+
+    recommended usage: tardis_actin [-dir path/to/folder/with/input/tomogram]
+    advance usage: tardis_actin [-dir str] [-out str] [-ps int] [-ct float] [-dt float]
+                             [-pv int] [-px float] ...
+
+
+2D Microtubule prediction
+^^^^^^^^^^^^^^^^^^^^^^^^^
 
 TBD
 
-3D prediction
-^^^^^^^^^^^^^
-Full tutorial: Full tutorial: `3D Microtubules Prediction <https://smlc-nysbc.github.io/TARDIS/usage/3d_mt.html>`__
+3D Microtubule prediction
+^^^^^^^^^^^^^^^^^^^^^^^^^
+Full tutorial: `3D Microtubules Prediction <https://smlc-nysbc.github.io/TARDIS/usage/3d_mt.html>`__
 
 
 Example:
 """"""""
 
 .. image:: resources/3d_mt.jpg
 
@@ -111,15 +142,15 @@
 
 
 Membrane Prediction
 -------------------
 
 2D prediction
 ^^^^^^^^^^^^^
-Full tutorial: Full tutorial: `2D Membrane Prediction <https://smlc-nysbc.github.io/TARDIS/usage/2d_membrane.html>`__
+Full tutorial: `2D Membrane Prediction <https://smlc-nysbc.github.io/TARDIS/usage/2d_membrane.html>`__
 
 Example:
 """"""""
 
 .. image:: resources/2d_mem.jpg
 
 Data source: Dr. Victor Kostyuchenko and Prof. Dr. Shee-Mei Lok, DUKE-NUS Medical School Singapore
```

### Comparing `tardis_em-0.2.4/setup.cfg` & `tardis_em-0.2.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 	tardis_czi = tardis_em.scripts.czi_predict:main
 	tardis_vis = tardis_em.scripts.visualize:main
 	
 	tardis_cnn_train = tardis_em.train_cnn:main
 	tardis_dist_train = tardis_em.train_DIST:main
 	
 	tardis_mt = tardis_em.predict_mt:main
+	tardis_actin = tardis_em.predict_actin:main
 	tardis_compare_sg = tardis_em.compare_spatial_graphs:main
 	
 	tardis_mem = tardis_em.predict_mem:main
 	tardis_mem2d = tardis_em.predict_mem_2d:main
 	
 	tardis_benchmark = tardis_em.benchmarks.benchmarks:main
```

### Comparing `tardis_em-0.2.4/setup.py` & `tardis_em-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/_version.py` & `tardis_em-0.2.5/tests/test_cnn_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,9 +3,7 @@
 #                                                                     #
 #  New York Structural Biology Center                                 #
 #  Simons Machine Learning Center                                     #
 #                                                                     #
 #  Robert Kiewisz, Tristan Bepler                                     #
 #  MIT License 2021 - 2024                                            #
 # #####################################################################
-
-version = "0.2.4"
```

### Comparing `tardis_em-0.2.4/tardis_em/benchmarks/benchmarks.py` & `tardis_em-0.2.5/tardis_em/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/benchmarks/predictor.py` & `tardis_em-0.2.5/tardis_em/benchmarks/predictor.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/cnn/cnn.py` & `tardis_em-0.2.5/tardis_em/cnn/cnn.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/cnn/data_processing/draw_mask.py` & `tardis_em-0.2.5/tardis_em/cnn/data_processing/draw_mask.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/cnn/data_processing/interpolation.py` & `tardis_em-0.2.5/tardis_em/cnn/data_processing/interpolation.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/cnn/data_processing/stitch.py` & `tardis_em-0.2.5/tardis_em/cnn/data_processing/stitch.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/cnn/data_processing/trim.py` & `tardis_em-0.2.5/tardis_em/cnn/data_processing/trim.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/cnn/datasets/augmentation.py` & `tardis_em-0.2.5/tardis_em/cnn/datasets/augmentation.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/cnn/datasets/build_dataset.py` & `tardis_em-0.2.5/tardis_em/cnn/datasets/build_dataset.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/cnn/datasets/dataloader.py` & `tardis_em-0.2.5/tardis_em/cnn/datasets/dataloader.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,168 +1,168 @@
-#######################################################################
-#  TARDIS - Transformer And Rapid Dimensionless Instance Segmentation #
-#                                                                     #
-#  New York Structural Biology Center                                 #
-#  Simons Machine Learning Center                                     #
-#                                                                     #
-#  Robert Kiewisz, Tristan Bepler                                     #
-#  MIT License 2021 - 2024                                            #
-#######################################################################
-
-import os
-from os import listdir
-from os.path import join, splitext
-from typing import Tuple
-
-import numpy as np
-import torch
-from torch.utils.data import Dataset
-
-from tardis_em.cnn.datasets.augmentation import preprocess
-from tardis_em.utils.errors import TardisError
-from tardis_em.utils.load_data import load_image
-from tardis_em.utils.normalization import MinMaxNormalize
-
-
-class CNNDataset(Dataset):
-    """
-    DATASET BUILDER FOR IMAGES AND SEMANTIC LABEL MASKS FOR TRAINING
-
-    Args:
-        img_dir (str): Source of the 2D/3D .tif file.
-        mask_dir (str): Source of the 2D/3D .tif  images masks.
-        size (int): Output patch size for image and mask.
-        mask_suffix (str): Suffix name for mask images.
-        transform (bool): Call for random transformation on img and mask.
-        out_channels (int): Number of output channels.
-    """
-
-    def __init__(
-        self,
-        img_dir: str,
-        mask_dir: str,
-        size=64,
-        mask_suffix="_mask",
-        transform=True,
-        out_channels=1,
-    ):
-        self.img_dir = img_dir
-        self.mask_dir = mask_dir
-        self.size = size
-        self.mask_suffix = mask_suffix
-        self.transform = transform
-        self.out_channels = out_channels
-        self.minmax = MinMaxNormalize()
-
-        self.ids = [
-            splitext(file)[0] for file in listdir(img_dir) if not file.startswith(".")
-        ]
-        self.format = [
-            splitext(file)[1]
-            for file in listdir(img_dir)[:5]
-            if not file.startswith(".")
-        ][1]
-
-    def __len__(self):
-        return len(self.ids)
-
-    def __getitem__(self, i: int) -> Tuple[torch.Tensor, torch.Tensor]:
-        """
-        Select and process dataset for CNN.
-
-        Args:
-            i (int): Image ID number.
-
-        Returns:
-            torch.Tensor, torch.Tensor: Tensor of processed image and mask.
-        """
-        # Find next image and corresponding label mask image
-        idx = self.ids[i]
-        mask_file = os.path.join(self.mask_dir, str(idx) + "_mask" + self.format)
-        img_file = os.path.join(self.img_dir, str(idx) + self.format)
-
-        # Load image and corresponding label mask
-        img, _ = load_image(img_file)
-        mask, _ = load_image(mask_file)
-
-        if mask.dtype != np.uint8:
-            TardisError(
-                "147",
-                "tardis_em/cnn/dataset/dataloader.py",
-                f"Mask should be of np.uint8 dtype but is {mask.dtype}!",
-            )
-
-        # Process image and mask
-        img, mask = preprocess(
-            image=img,
-            mask=mask,
-            size=self.size,
-            transformation=self.transform,
-            output_dim_mask=self.out_channels,
-        )
-
-        if img.dtype != np.float32 and mask.dtype != np.uint8:
-            TardisError(
-                "147",
-                "tardis_em/cnn/dataset/dataloader.py",
-                f"Mask {mask.dtype} and image  {img.dtype} has wrong dtype!",
-            )
-        if not img.min() >= -1 and not img.max() <= 1:
-            TardisError(
-                "147",
-                "tardis_em/cnn/dataset/dataloader.py",
-                "Image file is not binary!",
-            )
-
-        return torch.from_numpy(img.copy()).type(torch.float32), torch.from_numpy(
-            mask.copy()
-        ).type(torch.float32)
-
-
-class PredictionDataset(Dataset):
-    """
-    DATASET BUILDER FOR IMAGES AND SEMANTIC LABEL MASKS FOR PREDICTION
-
-    Module has turn off all transformations.
-
-    Args:
-        img_dir (str): Source of the 2D/3D .tif file.
-        out_channels (int): Number of output channels.
-    """
-
-    def __init__(self, img_dir: str, out_channels=1):
-        self.img_dir = img_dir
-        self.out_channels = out_channels
-
-        self.ids = [
-            splitext(file)[0] for file in listdir(img_dir) if not file.startswith(".")
-        ]
-
-    def __len__(self):
-        return len(self.ids)
-
-    def __getitem__(self, i: int):
-        """
-        Select and process dataset for CNN.
-
-        Args:
-            i (int): Image ID number.
-
-        Returns:
-            torch.Tensor, str: Tensor of processed image and image file name.
-        """
-        idx = self.ids[i]
-        img_file = join(self.img_dir, str(idx) + ".tif")
-
-        # Load image
-        img, _ = load_image(img_file)
-        img = img.astype(np.float32)
-
-        # Process image and mask
-        img = preprocess(
-            image=img,
-            size=img.shape,
-            transformation=False,
-            output_dim_mask=self.out_channels,
-        )
-
-        return torch.from_numpy(img).type(torch.float32), idx
+#######################################################################
+#  TARDIS - Transformer And Rapid Dimensionless Instance Segmentation #
+#                                                                     #
+#  New York Structural Biology Center                                 #
+#  Simons Machine Learning Center                                     #
+#                                                                     #
+#  Robert Kiewisz, Tristan Bepler                                     #
+#  MIT License 2021 - 2024                                            #
+#######################################################################
+
+import os
+from os import listdir
+from os.path import join, splitext
+from typing import Tuple
+
+import numpy as np
+import torch
+from torch.utils.data import Dataset
+
+from tardis_em.cnn.datasets.augmentation import preprocess
+from tardis_em.utils.errors import TardisError
+from tardis_em.utils.load_data import load_image
+from tardis_em.utils.normalization import MinMaxNormalize
+
+
+class CNNDataset(Dataset):
+    """
+    DATASET BUILDER FOR IMAGES AND SEMANTIC LABEL MASKS FOR TRAINING
+
+    Args:
+        img_dir (str): Source of the 2D/3D .tif file.
+        mask_dir (str): Source of the 2D/3D .tif  images masks.
+        size (int): Output patch size for image and mask.
+        mask_suffix (str): Suffix name for mask images.
+        transform (bool): Call for random transformation on img and mask.
+        out_channels (int): Number of output channels.
+    """
+
+    def __init__(
+        self,
+        img_dir: str,
+        mask_dir: str,
+        size=64,
+        mask_suffix="_mask",
+        transform=True,
+        out_channels=1,
+    ):
+        self.img_dir = img_dir
+        self.mask_dir = mask_dir
+        self.size = size
+        self.mask_suffix = mask_suffix
+        self.transform = transform
+        self.out_channels = out_channels
+        self.minmax = MinMaxNormalize()
+
+        self.ids = [
+            splitext(file)[0] for file in listdir(img_dir) if not file.startswith(".")
+        ]
+        self.format = [
+            splitext(file)[1]
+            for file in listdir(img_dir)[:5]
+            if not file.startswith(".")
+        ][1]
+
+    def __len__(self):
+        return len(self.ids)
+
+    def __getitem__(self, i: int) -> Tuple[torch.Tensor, torch.Tensor]:
+        """
+        Select and process dataset for CNN.
+
+        Args:
+            i (int): Image ID number.
+
+        Returns:
+            torch.Tensor, torch.Tensor: Tensor of processed image and mask.
+        """
+        # Find next image and corresponding label mask image
+        idx = self.ids[i]
+        mask_file = os.path.join(self.mask_dir, str(idx) + "_mask" + self.format)
+        img_file = os.path.join(self.img_dir, str(idx) + self.format)
+
+        # Load image and corresponding label mask
+        img, _ = load_image(img_file)
+        mask, _ = load_image(mask_file)
+
+        if mask.dtype != np.uint8:
+            TardisError(
+                "147",
+                "tardis_em/cnn/dataset/dataloader.py",
+                f"Mask should be of np.uint8 dtype but is {mask.dtype}!",
+            )
+
+        # Process image and mask
+        img, mask = preprocess(
+            image=img,
+            mask=mask,
+            size=self.size,
+            transformation=self.transform,
+            output_dim_mask=self.out_channels,
+        )
+
+        if img.dtype != np.float32 and mask.dtype != np.uint8:
+            TardisError(
+                "147",
+                "tardis_em/cnn/dataset/dataloader.py",
+                f"Mask {mask.dtype} and image  {img.dtype} has wrong dtype!",
+            )
+        if not img.min() >= -1 and not img.max() <= 1:
+            TardisError(
+                "147",
+                "tardis_em/cnn/dataset/dataloader.py",
+                "Image file is not binary!",
+            )
+
+        return torch.from_numpy(img.copy()).type(torch.float32), torch.from_numpy(
+            mask.copy()
+        ).type(torch.float32)
+
+
+class PredictionDataset(Dataset):
+    """
+    DATASET BUILDER FOR IMAGES AND SEMANTIC LABEL MASKS FOR PREDICTION
+
+    Module has turn off all transformations.
+
+    Args:
+        img_dir (str): Source of the 2D/3D .tif file.
+        out_channels (int): Number of output channels.
+    """
+
+    def __init__(self, img_dir: str, out_channels=1):
+        self.img_dir = img_dir
+        self.out_channels = out_channels
+
+        self.ids = [
+            splitext(file)[0] for file in listdir(img_dir) if not file.startswith(".")
+        ]
+
+    def __len__(self):
+        return len(self.ids)
+
+    def __getitem__(self, i: int):
+        """
+        Select and process dataset for CNN.
+
+        Args:
+            i (int): Image ID number.
+
+        Returns:
+            torch.Tensor, str: Tensor of processed image and image file name.
+        """
+        idx = self.ids[i]
+        img_file = join(self.img_dir, str(idx) + ".tif")
+
+        # Load image
+        img, _ = load_image(img_file)
+        img = img.astype(np.float32)
+
+        # Process image and mask
+        img = preprocess(
+            image=img,
+            size=img.shape,
+            transformation=False,
+            output_dim_mask=self.out_channels,
+        )
+
+        return torch.from_numpy(img).type(torch.float32), idx
```

### Comparing `tardis_em-0.2.4/tardis_em/cnn/model/convolution.py` & `tardis_em-0.2.5/tardis_em/cnn/model/convolution.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/cnn/model/decoder_blocks.py` & `tardis_em-0.2.5/tardis_em/cnn/model/decoder_blocks.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/cnn/model/encoder_blocks.py` & `tardis_em-0.2.5/tardis_em/cnn/model/encoder_blocks.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/cnn/model/init_weights.py` & `tardis_em-0.2.5/tardis_em/cnn/model/init_weights.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/cnn/train.py` & `tardis_em-0.2.5/tardis_em/cnn/train.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/cnn/trainer.py` & `tardis_em-0.2.5/tardis_em/cnn/trainer.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/cnn/utils/build_cnn.py` & `tardis_em-0.2.5/tardis_em/cnn/utils/build_cnn.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/cnn/utils/utils.py` & `tardis_em-0.2.5/tardis_em/cnn/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 
     Expect 2D (XY/YX), 3D (ZYX)
 
     Args:
         image (np.ndarray, Optional): image data
         mask (np.ndarray, Optional): Optional binary mask image data
         scale (tuple): scale value for image
+        nn (bool):
+        device (str):
     """
     dim = 1
     type_i = image.dtype
     type_m = None
     if mask is not None:
         type_m = mask.dtype
```

### Comparing `tardis_em-0.2.4/tardis_em/compare_spatial_graphs.py` & `tardis_em-0.2.5/tardis_em/compare_spatial_graphs.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/dist_pytorch/datasets/augmentation.py` & `tardis_em-0.2.5/tardis_em/dist_pytorch/datasets/augmentation.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/dist_pytorch/datasets/dataloader.py` & `tardis_em-0.2.5/tardis_em/dist_pytorch/datasets/dataloader.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/dist_pytorch/datasets/patches.py` & `tardis_em-0.2.5/tardis_em/dist_pytorch/datasets/patches.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/dist_pytorch/dist.py` & `tardis_em-0.2.5/tardis_em/dist_pytorch/dist.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/dist_pytorch/model/embedding.py` & `tardis_em-0.2.5/tardis_em/dist_pytorch/model/embedding.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/dist_pytorch/model/layers.py` & `tardis_em-0.2.5/tardis_em/dist_pytorch/model/layers.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/dist_pytorch/model/modules.py` & `tardis_em-0.2.5/tardis_em/dist_pytorch/model/modules.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/dist_pytorch/sparse_dist.py` & `tardis_em-0.2.5/tardis_em/dist_pytorch/sparse_dist.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/dist_pytorch/sparse_model/embedding.py` & `tardis_em-0.2.5/tardis_em/dist_pytorch/sparse_model/embedding.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/dist_pytorch/sparse_model/layers.py` & `tardis_em-0.2.5/tardis_em/dist_pytorch/sparse_model/layers.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/dist_pytorch/sparse_model/modules.py` & `tardis_em-0.2.5/tardis_em/dist_pytorch/sparse_model/modules.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/dist_pytorch/train.py` & `tardis_em-0.2.5/tardis_em/dist_pytorch/train.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/dist_pytorch/trainer.py` & `tardis_em-0.2.5/tardis_em/dist_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/dist_pytorch/utils/__init__.py` & `tardis_em-0.2.5/tardis_em/dist_pytorch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/dist_pytorch/utils/build_point_cloud.py` & `tardis_em-0.2.5/tardis_em/dist_pytorch/utils/build_point_cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,26 +98,22 @@
                 )
 
         return image
 
     def build_point_cloud(
         self,
         image: Union[str, np.ndarray],
-        EDT=False,
-        mask_size=1.5,
         down_sampling: Union[float, None] = None,
         as_2d=False,
     ) -> Union[Tuple[ndarray, ndarray], np.ndarray]:
         """
         Build point cloud data from semantic mask.
 
         Args:
             image (np.ndarray): Predicted semantic mask.
-            EDT (bool): If True, compute EDT to extract line centers.
-            mask_size (float): Mask size to filter with EDT.
             down_sampling (float, None): If not None, down-sample point cloud with open3d.
             as_2d: Treat data as 2D not 3D.
 
         Returns:
             Union[Tuple[ndarray, ndarray], np.ndarray]: Point cloud of 2D/3D
             semantic objects.
         """
```

### Comparing `tardis_em-0.2.4/tardis_em/dist_pytorch/utils/segment_point_cloud.py` & `tardis_em-0.2.5/tardis_em/dist_pytorch/utils/segment_point_cloud.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/dist_pytorch/utils/utils.py` & `tardis_em-0.2.5/tardis_em/dist_pytorch/utils/utils.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/predict_mem.py` & `tardis_em-0.2.5/tardis_em/predict_mem.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/predict_mem_2d.py` & `tardis_em-0.2.5/tardis_em/predict_mem_2d.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/predict_mt.py` & `tardis_em-0.2.5/tardis_em/predict_mt.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/scripts/czi_predict.py` & `tardis_em-0.2.5/tardis_em/scripts/czi_predict.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,14 @@
             text_3=f"Dataset: [{name}]",
             text_4=f"Pixel_size: {px}",
             text_6=print_progress_bar(progress[0], progress[1]),
         )
 
         _, pc_ld = BuildPointCloud().build_point_cloud(
             image=data,
-            EDT=False,
             down_sampling=5,
             as_2d=True if self.predict == "Membrane" else False,
         )
         if len(pc_ld) > 100:
             coords_df, _, output_idx, _ = self.patch_pc.patched_dataset(coord=pc_ld)
             x = self.predict_dist(coords_df)
```

### Comparing `tardis_em-0.2.4/tardis_em/scripts/visualize.py` & `tardis_em-0.2.5/tardis_em/scripts/visualize.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/tardis.py` & `tardis_em-0.2.5/tardis_em/tardis.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/tardis_helper/helper_func.py` & `tardis_em-0.2.5/tardis_em/tardis_helper/helper_func.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/train_DIST.py` & `tardis_em-0.2.5/tardis_em/train_DIST.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from tardis_em.dist_pytorch.train import train_dist
 from tardis_em.utils.dataset import build_test_dataset, move_train_dataset
 from tardis_em.utils.device import get_device
 from tardis_em.utils.errors import TardisError
 from tardis_em.utils.logo import TardisLogo
 from tardis_em.utils.setup_envir import check_dir
 from tardis_em._version import version
-from tardis_em.utils.ota_update import ota_update
+# from tardis_em.utils.ota_update import ota_update
 
 # ota = ota_update()
 
 
 @click.command()
 @click.option(
     "-dir",
```

### Comparing `tardis_em-0.2.4/tardis_em/train_cnn.py` & `tardis_em-0.2.5/tardis_em/train_cnn.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/utils/__init__.py` & `tardis_em-0.2.5/tardis_em/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/utils/aws.py` & `tardis_em-0.2.5/tardis_em/utils/aws.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         network (str): Type of network for which weights are requested.
         subtype (str): Sub-name of the network or sub-parameter for the network.
         model (str): Additional dataset name used for the DIST.
     """
     ALL_MODELS = ["unet", "unet3plus", "fnet_attn", "dist"]
     ALL_SUBTYPE = ["16", "32", "64", "96", "128", "triang", "full"]
     CNN = ["unet", "unet3plus", "fnet", "fnet_attn"]
-    CNN_DATASET = ["microtubules_3d", "microtubules_2d", "membrane_3d", "membrane_2d"]
+    CNN_DATASET = ["microtubules_3d", "microtubules_2d", "membrane_3d", "membrane_2d", "actin_3d"]
     DIST_DATASET = ["microtubules", "s3dis", "membrane_2d", "2d", "3d"]
 
     """Chech dir"""
     if not isdir(join(expanduser("~"), ".tardis_em")):
         mkdir(join(expanduser("~"), ".tardis_em"))
     if not isdir(join(expanduser("~"), ".tardis_em", f"{network}_{subtype}")):
         mkdir(join(expanduser("~"), ".tardis_em", f"{network}_{subtype}"))
```

### Comparing `tardis_em-0.2.4/tardis_em/utils/dataset.py` & `tardis_em-0.2.5/tardis_em/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/utils/device.py` & `tardis_em-0.2.5/tardis_em/utils/device.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/utils/errors.py` & `tardis_em-0.2.5/tardis_em/utils/errors.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/utils/export_data.py` & `tardis_em-0.2.5/tardis_em/utils/export_data.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/utils/load_data.py` & `tardis_em-0.2.5/tardis_em/utils/load_data.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/utils/logo.py` & `tardis_em-0.2.5/tardis_em/utils/logo.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/utils/losses.py` & `tardis_em-0.2.5/tardis_em/utils/losses.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/utils/metrics.py` & `tardis_em-0.2.5/tardis_em/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/utils/normalization.py` & `tardis_em-0.2.5/tardis_em/utils/normalization.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/utils/ota_update.py` & `tardis_em-0.2.5/tardis_em/utils/ota_update.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/utils/predictor.py` & `tardis_em-0.2.5/tardis_em/utils/predictor.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from typing import Optional, Union, List
 import platform
 
 import numpy as np
 import pandas as pd
 import tifffile.tifffile as tif
 import torch
+from tardis_em.dist_pytorch.utils.utils import VoxelDownSampling
 
 from tardis_em.dist_pytorch.datasets.patches import PatchDataSet
 from tardis_em.dist_pytorch.dist import build_dist_network
 from tardis_em.dist_pytorch.utils.build_point_cloud import BuildPointCloud
 from tardis_em.dist_pytorch.utils.segment_point_cloud import PropGreedyGraphCut
 from tardis_em.cnn.data_processing.draw_mask import (
     draw_semantic_membrane,
@@ -42,15 +43,15 @@
 from tardis_em.utils.setup_envir import build_temp_dir, clean_up
 from tardis_em.utils.spline_metric import (
     FilterSpatialGraph,
     FilterConnectedNearSegments,
     SpatialGraphCompare,
     sort_by_length,
     ComputeConfidenceScore,
-    length_list,
+    length_list, resample_filament,
 )
 from tardis_em._version import version
 
 # try:
 #     from tardis_em.utils.ota_update import ota_update
 #
 #     ota = ota_update(status=True)
@@ -190,15 +191,15 @@
 
         # Build handler's for DIST input and output
         if self.predict_instance:
             self.patch_pc = PatchDataSet(
                 max_number_of_points=points_in_patch, graph=False
             )
 
-            if predict in ["Filament", "Microtubule", "Membrane2D"]:
+            if predict in ["Actin", "Microtubule", "Membrane2D"]:
                 self.GraphToSegment = PropGreedyGraphCut(
                     threshold=dist_threshold, connection=2, smooth=True
                 )
 
                 if predict == "Membrane2D":
                     self.filter_splines = FilterConnectedNearSegments(
                         distance_th=connect_splines,
@@ -232,15 +233,15 @@
         self.build_NN(NN=self.predict)
 
     def init_check(self):
         """
         All sanity checks before TARDIS initialize prediction
         """
         msg = f"TARDIS v.{version} supports only MT and Mem segmentation!"
-        assert_ = self.predict in ["Filament", "Membrane2D", "Membrane", "Microtubule"]
+        assert_ = self.predict in ["Actin", "Membrane2D", "Membrane", "Microtubule"]
         if self.tardis_logo:
             # Check if user ask to predict correct structure
             if not assert_:
                 TardisError(
                     id_="01",
                     py="tardis_em/utils/predictor.py",
                     desc=msg,
@@ -303,27 +304,27 @@
                     desc=msg,
                 )
                 sys.exit()
             else:
                 assert not assert_, msg
 
     def build_NN(self, NN: str):
-        if NN == "Microtubule":
+        if NN in ["Microtubule", "Actin"]:
             self.normalize_px = 25
         else:
             self.normalize_px = 15
 
-        if NN in ["Filament", "Microtubule"]:
+        if NN in ["Actin", "Microtubule"]:
             # Build CNN network with loaded pre-trained weights
-            if not self.output_format.startswith("None") or not self.binary_mask:
+            if not self.output_format.startswith("None") and not self.binary_mask:
                 self.cnn = Predictor(
                     checkpoint=self.checkpoint[0],
                     network=self.convolution_nn,
                     subtype="32",
-                    model_type="microtubules_3d",
+                    model_type="microtubules_3d" if NN == "Microtubule" else "actin_3d",
                     img_size=self.patch_size,
                     sigmoid=False,
                     device=self.device,
                 )
 
             # Build DIST network with loaded pre-trained weights
             if not self.output_format.endswith("None"):
@@ -333,15 +334,15 @@
                     subtype="triang",
                     model_type="2d",
                     device=self.device,
                 )
         elif NN in ["Membrane2D", "Membrane"]:
             # Build CNN network with loaded pre-trained weights
             if NN == "Membrane2D":
-                if not self.output_format.startswith("None") or not self.binary_mask:
+                if not self.output_format.startswith("None") and not self.binary_mask:
                     self.cnn = Predictor(
                         checkpoint=self.checkpoint[0],
                         network=self.convolution_nn,
                         subtype="32",
                         model_type="membrane_2d",
                         img_size=self.patch_size,
                         sigmoid=False,
@@ -355,15 +356,15 @@
                         checkpoint=self.checkpoint[1],
                         network="dist",
                         subtype="triang",
                         model_type="2d",
                         device=self.device,
                     )
             else:
-                if not self.output_format.startswith("None") or not self.binary_mask:
+                if not self.output_format.startswith("None") and not self.binary_mask:
                     self.cnn = Predictor(
                         checkpoint=self.checkpoint[0],
                         network=self.convolution_nn,
                         subtype="32",
                         model_type="membrane_3d",
                         img_size=self.patch_size,
                         sigmoid=False,
@@ -383,28 +384,53 @@
     def load_data(self, id_name: Union[str, np.ndarray]):
         # Build temp dir
         build_temp_dir(dir_=self.dir)
 
         if isinstance(id_name, str):
             # Load image file
             if id_name.endswith(".am"):
-                self.image, self.px, _, self.transformation = import_am(
-                    am_file=join(self.dir, id_name)
-                )
+                am = open(join(self.dir, id_name), "r", encoding="iso-8859-1").read(500)
+
+                if "AmiraMesh 3D ASCII" in am:
+                    self.amira_image = False
+                    self.pc_hd = ImportDataFromAmira(join(self.dir, id_name)).get_segmented_points()
+
+                    self.image = None
+                    self.px = self.correct_px
+                    self.transformation = [0, 0, 0]
+
+                    assert_ = self.pc_hd.shape[1] == 4
+                    msg = f'Amira Spatial Graph has wrong dimension. Given {self.pc_hd.shape[1]}, but expected 4.'
+                    if self.tardis_logo:
+                        if not assert_:
+                            TardisError(
+                                id_="11",
+                                py="tardis_em/utils/predictor.py",
+                                desc=msg,
+                            )
+                            sys.exit()
+                    else:
+                        assert assert_, msg
+                else:
+                    self.amira_image = True
+                    self.image, self.px, _, self.transformation = import_am(
+                        am_file=join(self.dir, id_name)
+                    )
             else:
+                self.amira_image = True
                 self.image, self.px = load_image(join(self.dir, id_name))
                 self.transformation = [0, 0, 0]
         else:
             self.image = id_name
             self.px = self.correct_px
             self.transformation = [0, 0, 0]
 
         # Normalize image histogram
         msg = f"Error while loading image {id_name}. Image loaded correctly, but output format "
-        if not self.output_format.startswith("None") or not self.binary_mask:
+        if self.amira_image and not self.binary_mask:
             self.image = self.normalize(self.mean_std(self.image)).astype(np.float32)
 
             # Sanity check image histogram
             if (
                 not self.image.min() >= -1 or not self.image.max() <= 1
             ):  # Image not between in -1 and 1
                 if self.image.min() >= 0 and self.image.max() <= 1:
@@ -420,15 +446,30 @@
                         id_="11",
                         py="tardis_em/utils/predictor.py",
                         desc=msg + f" {self.image.dtype} is not float32!",
                     )
                     sys.exit()
             else:
                 assert assert_, msg
-        else:
+
+            # Calculate parameters for image pixel size with optional scaling
+            if self.correct_px is not None:
+                self.px = self.correct_px
+
+            if self.normalize_px is not None:
+                self.scale_factor = self.px / self.normalize_px
+            else:
+                self.scale_factor = 1.0
+
+            self.org_shape = self.image.shape
+            self.scale_shape = np.multiply(self.org_shape, self.scale_factor).astype(
+                np.int16
+            )
+            self.scale_shape = [int(i) for i in self.scale_shape]
+        elif self.amira_image and self.binary_mask:
             # Check image structure
             self.image = np.where(self.image > 0, 1, 0).astype(np.int8)
 
             assert_ = self.image.dtype == np.int8 or self.image.dtype == np.uint8
             if self.tardis_logo:
                 if not assert_:
                     TardisError(
@@ -436,29 +477,14 @@
                         py="tardis_em/utils/predictor.py",
                         desc=msg + f" {self.image.dtype} is not int8!",
                     )
                     sys.exit()
             else:
                 assert assert_, msg
 
-        # Calculate parameters for image pixel size with optional scaling
-        if self.correct_px is not None:
-            self.px = self.correct_px
-
-        if self.normalize_px is not None:
-            self.scale_factor = self.px / self.normalize_px
-        else:
-            self.scale_factor = 1.0
-
-        self.org_shape = self.image.shape
-        self.scale_shape = np.multiply(self.org_shape, self.scale_factor).astype(
-            np.int16
-        )
-        self.scale_shape = [int(i) for i in self.scale_shape]
-
     def predict_cnn(self, id_: int, id_name: str, dataloader):
         iter_time = 1
         if self.rotate:
             pred_title = f"CNN prediction with four 90 degree rotations with {self.convolution_nn}"
         else:
             pred_title = f"CNN prediction with {self.convolution_nn}"
 
@@ -524,31 +550,36 @@
                 )
                 self.image = None
 
         """Clean-up temp dir"""
         clean_up(dir_=self.dir)
 
     def preprocess_DIST(self, id_name: str):
-        # Post-process predicted image patches
-        if self.predict in ["Filament", "Microtubule"]:
-            self.pc_hd, self.pc_ld = self.post_processes.build_point_cloud(
-                image=self.image, EDT=False, down_sampling=5
-            )
-        elif self.predict == "Membrane2D":
-            self.pc_hd, self.pc_ld = self.post_processes.build_point_cloud(
-                image=self.image, EDT=False, down_sampling=5, as_2d=True
-            )
-        else:
-            self.pc_hd, self.pc_ld = self.post_processes.build_point_cloud(
-                image=self.image, EDT=False, down_sampling=5, as_2d=True
-            )
+        if self.amira_image:
+            # Post-process predicted image patches
+            if self.predict in ["Actin", "Microtubule"]:
+                self.pc_hd, self.pc_ld = self.post_processes.build_point_cloud(
+                    image=self.image, down_sampling=5
+                )
+            elif self.predict == "Membrane2D":
+                self.pc_hd, self.pc_ld = self.post_processes.build_point_cloud(
+                    image=self.image, down_sampling=5, as_2d=True
+                )
+            else:
+                self.pc_hd, self.pc_ld = self.post_processes.build_point_cloud(
+                    image=self.image, down_sampling=5, as_2d=True
+                )
 
-        if not self.output_format.startswith("return"):
-            self.image = None
-        self._debug(id_name=id_name, debug_id="pc")
+            if not self.output_format.startswith("return"):
+                self.image = None
+            self._debug(id_name=id_name, debug_id="pc")
+        else:
+            self.pc_hd = resample_filament(self.pc_hd, self.px)
+            down_sample = VoxelDownSampling(voxel=5, labels=False, KNN=True)
+            self.pc_ld = down_sample(coord=self.pc_hd[:, 1:])
 
     def predict_DIST(self, id_: int, id_name: str):
         iter_time = int(round(len(self.coords_df) / 10))
         if iter_time == 0:
             iter_time = 1
         if iter_time >= len(self.coords_df):
             iter_time = 10
@@ -589,21 +620,21 @@
         self.pc_ld = (
             self.pc_ld * self.px
             if self.correct_px is None
             else self.pc_ld * self.correct_px
         )
         self.pc_ld = self.pc_ld + self.transformation
 
-        if self.predict in ["Filament", "Microtubule"]:
+        if self.predict in ["Actin", "Microtubule"]:
             self.log_tardis(id_, i, log_id=6.1)
         else:
             self.log_tardis(id_, i, log_id=6.2)
 
         try:
-            if self.predict in ["Filament", "Microtubule", "Membrane2D"]:
+            if self.predict in ["Actin", "Microtubule", "Membrane2D"]:
                 sort = True
                 prune = 5
             else:
                 sort = False
                 prune = 15
 
             self.segments = self.GraphToSegment.patch_to_segment(
@@ -613,49 +644,42 @@
                 sort=sort,
                 prune=prune,
             )
             self.segments = sort_by_length(self.segments)
         except:
             self.segments = None
 
-    def get_file_list(self, output=True):
+    def get_file_list(self):
         # Pickup files for the prediction
         if not isinstance(self.dir, str):
             if isinstance(self.dir, tuple) or isinstance(self.dir, list):
                 self.predict_list = self.dir
             else:
                 self.predict_list = [self.dir]
-            self.dir = "."
+            self.dir = getcwd()
         else:
             if isdir(self.dir):
                 self.predict_list = [
                     f
                     for f in listdir(self.dir)
                     if f.endswith(self.available_format)
                     and not f.endswith(self.omit_format)
                 ]
             else:
-                if dirname(self.dir) == "":
-                    self.dir = self.dir
-
                 self.predict_list = [
                     f
                     for f in [self.dir]
                     if f.endswith(self.available_format)
                     and not f.endswith(self.omit_format)
                 ]
                 self.dir = getcwd()
 
         # Update Dir paths
-        if output:
-            self.output = join(self.dir, "temp", "Predictions")
-            self.am_output = join(self.dir, "Predictions")
-        else:
-            self.output = None
-            self.am_output = None
+        self.output = join(self.dir, "temp", "Predictions")
+        self.am_output = join(self.dir, "Predictions")
 
         # Check if there is anything to predict in user indicated folder
         msg = f"Given {self.dir} does not contain any recognizable file!"
         assert_ = len(self.predict_list) == 0
         if self.tardis_logo:
             if assert_:
                 TardisError(
@@ -782,15 +806,15 @@
         elif self.output_format.startswith("npy"):
             np.save(
                 join(self.am_output, f"{i[:-self.in_format]}_semantic.npy"), self.image
             )
 
     def save_instance_PC(self, i):
         if self.output_format.endswith("amSG") and self.predict in [
-            "Filament",
+            "Actin",
             "Microtubule",
         ]:
             self.amira_file.export_amira(
                 coords=self.segments,
                 file_dir=join(self.am_output, f"{i[:-self.in_format]}_SpatialGraph.am"),
                 labels=["TardisPrediction"],
                 scores=[
@@ -851,15 +875,15 @@
             segments.to_csv(
                 join(self.am_output, f"{i[:-self.in_format]}_instances.csv"),
                 header=["IDs", "X [A]", "Y [A]", "Z [A]"],
                 index=False,
                 sep=",",
             )
 
-            if self.predict in ["Filament", "Microtubule", "Membrane2D"]:
+            if self.predict in ["Actin", "Microtubule", "Membrane2D"]:
                 self.segments = sort_by_length(self.filter_splines(self.segments))
                 self.segments = pd.DataFrame(self.segments)
                 self.segments.to_csv(
                     join(
                         self.am_output,
                         f"{i[:-self.in_format]}_instances_filter.csv",
                     ),
@@ -1000,26 +1024,22 @@
                 np.save(
                     join(
                         self.am_output, f"{id_name[:-self.in_format]}_instance_mask.npy"
                     ),
                     self.mask_semantic,
                 )
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self):
         """Process each image with CNN and DIST"""
         self.get_file_list()
 
         semantic_output, instance_output, instance_filter_output = [], [], []
         for id_, i in enumerate(self.predict_list):
             """CNN Pre-Processing"""
             if isinstance(i, str):
-                if i.endswith("CorrelationLines.am"):
-                    # Skip .am files which are spatial graphs not images
-                    continue
-
                 # Find file format
                 self.in_format = 0
                 if i.endswith((".tif", ".mrc", ".rec", ".map", ".npy")):
                     self.in_format = 4
                 elif i.endswith(".tiff"):
                     self.in_format = 5
                 elif i.endswith(".am"):
@@ -1043,15 +1063,15 @@
                 else:
                     assert not assert_, msg
 
             # Tardis progress bar update
             self.log_tardis(id_, i, log_id=1)
 
             """Semantic Segmentation"""
-            if not self.output_format.startswith("None") or not self.binary_mask:
+            if not self.output_format.startswith("None") and not self.binary_mask:
                 # Cut image for fix patch size and normalizing image pixel size
                 trim_with_stride(
                     image=self.image,
                     scale=self.scale_shape,
                     trim_size_xy=self.patch_size,
                     trim_size_z=self.patch_size,
                     output=join(self.dir, "temp", "Patches"),
```

### Comparing `tardis_em-0.2.4/tardis_em/utils/setup_envir.py` & `tardis_em-0.2.5/tardis_em/utils/setup_envir.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/utils/spline_metric.py` & `tardis_em-0.2.5/tardis_em/utils/spline_metric.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,61 @@
 from scipy.spatial.distance import cdist
 from sklearn.neighbors import KDTree
 
 from tardis_em.dist_pytorch.utils.utils import pc_median_dist
 from tardis_em.utils.errors import TardisError
 
 
+def resample_filament(points, spacing_size):
+    """
+    Resamples points for each filament so they have the given spacing size.
+
+    Parameters:
+    points (np.array): Array of shape [N, 4] where each column is [ID, X, Y, Z].
+    spacing_size (float): Desired spacing size between points.
+
+    Returns:
+    np.array: Resampled array with the same structure.
+    """
+    unique_ids = np.unique(points[:, 0])
+    resampled_points = []
+
+    for filament_id in unique_ids:
+        filament_points = points[points[:, 0] == filament_id][:, 1:]
+        if filament_points.shape[0] < 2:
+            resampled_points.append(points[points[:, 0] == filament_id])
+            continue
+
+        cumulative_distances = np.cumsum(np.sqrt(np.sum(np.diff(filament_points, axis=0) ** 2, axis=1)))
+        cumulative_distances = np.insert(cumulative_distances, 0, 0)
+
+        num_new_points = int(cumulative_distances[-1] // spacing_size)
+        new_points = [filament_points[0]]
+
+        for i in range(1, num_new_points + 1):
+            target_distance = i * spacing_size
+            idx = np.searchsorted(cumulative_distances, target_distance)
+            if idx >= len(cumulative_distances):
+                continue
+
+            if cumulative_distances[idx] == target_distance:
+                new_points.append(filament_points[idx])
+            else:
+                ratio = (target_distance - cumulative_distances[idx - 1]) / (
+                            cumulative_distances[idx] - cumulative_distances[idx - 1])
+                new_point = filament_points[idx - 1] + ratio * (filament_points[idx] - filament_points[idx - 1])
+                new_points.append(new_point)
+
+        new_points = np.array(new_points)
+        filament_ids = np.full((new_points.shape[0], 1), filament_id)
+        resampled_points.append(np.hstack((filament_ids, new_points)))
+
+    return np.vstack(resampled_points)
+
+
 class FilterConnectedNearSegments:
     """
     Connect splines based on spline trajectory and splines end distances.
     """
 
     def __init__(self, distance_th=1000, cylinder_radius=150):
         """
```

### Comparing `tardis_em-0.2.4/tardis_em/utils/trainer.py` & `tardis_em-0.2.5/tardis_em/utils/trainer.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/utils/utils.py` & `tardis_em-0.2.5/tardis_em/utils/utils.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em/utils/visualize_pc.py` & `tardis_em-0.2.5/tardis_em/utils/visualize_pc.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tardis_em.egg-info/PKG-INFO` & `tardis_em-0.2.5/tardis_em.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tardis_em
-Version: 0.2.4
+Version: 0.2.5
 Summary: PyTorch segmentation of 2D/3D images such as electron tomography (ET),Cryo-EM or fluorescent microscopy data into 3D segmented point cloud.
 Home-page: https://github.com/SMLC-NYSBC/TARDIS
 Author: Robert Kiewisz, Tristan Bepler
 Author-email: rkiewisz@nysbc.org
 License: MIT
 Keywords: semantic segmentation,instance segmentation,MT segmentation,membrane segmentation,CNN,FNet,DIST
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,20 +25,18 @@
 Requires-Dist: imagecodecs>2021.11.00
 Requires-Dist: scikit-learn>1.0.1
 Requires-Dist: scikit-image>0.19.2
 Requires-Dist: scipy>=1.8.1
 Requires-Dist: pillow>10.0.0
 Requires-Dist: plyfile>=0.9
 Requires-Dist: pyvista>=0.40.0; platform_machine != "aarch64"
-Requires-Dist: open3d==0.9.0; sys_platform != "linux" and python_version < "3.8"
-Requires-Dist: open3d>=0.9.0; sys_platform != "linux" and python_version >= "3.8"
+Requires-Dist: open3d>=0.9.0; sys_platform != "linux"
 Requires-Dist: requests>2.28.0
 Requires-Dist: ipython>8.0.0
 Requires-Dist: click>8.0.4
-Requires-Dist: nvidia-smi>=0.1.3; sys_platform != "darwin"
 Requires-Dist: setuptools>=67.6.0
 Provides-Extra: docs
 Requires-Dist: sphinx<5.0; extra == "docs"
 Requires-Dist: myst_parser; extra == "docs"
 Requires-Dist: pydata_sphinx_theme; extra == "docs"
 Requires-Dist: sphinx_markdown_tables; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
```

### Comparing `tardis_em-0.2.4/tardis_em.egg-info/SOURCES.txt` & `tardis_em-0.2.5/tardis_em.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 tardis_em/__init__.py
 tardis_em/_version.py
 tardis_em/compare_spatial_graphs.py
+tardis_em/predict_actin.py
 tardis_em/predict_mem.py
 tardis_em/predict_mem_2d.py
 tardis_em/predict_mt.py
 tardis_em/tardis.py
 tardis_em/train_DIST.py
 tardis_em/train_cnn.py
 tardis_em.egg-info/PKG-INFO
@@ -84,15 +85,14 @@
 tardis_em/utils/ota_update.py
 tardis_em/utils/predictor.py
 tardis_em/utils/setup_envir.py
 tardis_em/utils/spline_metric.py
 tardis_em/utils/trainer.py
 tardis_em/utils/utils.py
 tardis_em/utils/visualize_pc.py
-tests/run_all_tests.py
 tests/test_cnn_build_dataset.py
 tests/test_cnn_dataset.py
 tests/test_cnn_draw_mask.py
 tests/test_cnn_interpolation.py
 tests/test_cnn_nn.py
 tests/test_cnn_trim_stitch.py
 tests/test_cnn_utils.py
```

### Comparing `tardis_em-0.2.4/tardis_em.egg-info/entry_points.txt` & `tardis_em-0.2.5/tardis_em.egg-info/entry_points.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [console_scripts]
 tardis = tardis_em.tardis:main
+tardis_actin = tardis_em.predict_actin:main
 tardis_benchmark = tardis_em.benchmarks.benchmarks:main
 tardis_cnn_train = tardis_em.train_cnn:main
 tardis_compare_sg = tardis_em.compare_spatial_graphs:main
 tardis_czi = tardis_em.scripts.czi_predict:main
 tardis_dist_train = tardis_em.train_DIST:main
 tardis_mem = tardis_em.predict_mem:main
 tardis_mem2d = tardis_em.predict_mem_2d:main
```

### Comparing `tardis_em-0.2.4/tests/test_cnn_build_dataset.py` & `tardis_em-0.2.5/tests/test_cnn_build_dataset.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tests/test_cnn_dataset.py` & `tardis_em-0.2.5/tests/test_cnn_dataset.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tests/test_cnn_draw_mask.py` & `tardis_em-0.2.5/tests/test_cnn_draw_mask.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tests/test_cnn_interpolation.py` & `tardis_em-0.2.5/tests/test_cnn_interpolation.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tests/test_cnn_nn.py` & `tardis_em-0.2.5/tests/test_cnn_nn.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tests/test_cnn_trim_stitch.py` & `tardis_em-0.2.5/tests/test_cnn_trim_stitch.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tests/test_dist_augmentation.py` & `tardis_em-0.2.5/tests/test_dist_augmentation.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tests/test_dist_data_loader.py` & `tardis_em-0.2.5/tests/test_dist_data_loader.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tests/test_dist_embedding.py` & `tardis_em-0.2.5/tests/test_dist_embedding.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tests/test_dist_graph_cut.py` & `tardis_em-0.2.5/tests/test_dist_graph_cut.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tests/test_dist_img_to_pc.py` & `tardis_em-0.2.5/tests/test_dist_img_to_pc.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tests/test_dist_modules.py` & `tardis_em-0.2.5/tests/test_dist_modules.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tests/test_dist_nn.py` & `tardis_em-0.2.5/tests/test_dist_nn.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tests/test_dist_trainer.py` & `tardis_em-0.2.5/tests/test_dist_trainer.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tests/test_dist_utils.py` & `tardis_em-0.2.5/tests/test_dist_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,19 +25,19 @@
     y = m * x[:, np.newaxis] + b
     y = np.where(y[:, :50] > 5.5, 1, 0)
 
     pc = builder.build_point_cloud(image=y)
     assert pc.ndim == 2
     assert len(pc) > 0
 
-    pc = builder.build_point_cloud(image=y, EDT=True)
+    pc = builder.build_point_cloud(image=y)
     assert pc.ndim == 2
     assert len(pc) > 0
 
-    pc = builder.build_point_cloud(image=y, EDT=True, as_2d=True)
+    pc = builder.build_point_cloud(image=y, as_2d=True)
     assert pc.ndim == 2
     assert len(pc) > 0
 
-    pc_hd, pc_ld = builder.build_point_cloud(image=y, EDT=True, down_sampling=1)
+    pc_hd, pc_ld = builder.build_point_cloud(image=y, down_sampling=1)
     assert pc_hd.ndim == 2 and pc_ld.ndim == 2
     assert len(pc_hd) > 0
     assert len(pc_ld) > 0
```

### Comparing `tardis_em-0.2.4/tests/test_losses.py` & `tardis_em-0.2.5/tests/test_losses.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tests/test_trainer.py` & `tardis_em-0.2.5/tests/test_trainer.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.4/tests/test_utils.py` & `tardis_em-0.2.5/tests/test_utils.py`

 * *Files identical despite different names*

