# Comparing `tmp/neural-commons-0.3.1.tar.gz` & `tmp/neural-commons-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural-commons-0.3.1.tar", last modified: Mon May 20 01:11:01 2024, max compression
+gzip compressed data, was "neural-commons-0.3.2.tar", last modified: Thu May 23 13:59:39 2024, max compression
```

## Comparing `neural-commons-0.3.1.tar` & `neural-commons-0.3.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 01:11:01.276176 neural-commons-0.3.1/
--rw-rw-rw-   0        0        0      745 2024-05-20 01:11:01.276176 neural-commons-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-28 15:46:56.000000 neural-commons-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 01:11:01.213677 neural-commons-0.3.1/neural_commons/
--rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.3.1/neural_commons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 01:11:01.213677 neural-commons-0.3.1/neural_commons/cf_nn/
--rw-rw-rw-   0        0        0     3302 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/cf_nn/CFConv2d.py
--rw-rw-rw-   0        0        0     1575 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/cf_nn/CFLinear.py
--rw-rw-rw-   0        0        0     1228 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/cf_nn/CFModule.py
--rw-rw-rw-   0        0        0    10584 2024-05-20 01:06:32.000000 neural-commons-0.3.1/neural_commons/cf_nn/CFOptimizer.py
--rw-rw-rw-   0        0        0      363 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/cf_nn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 01:11:01.229304 neural-commons-0.3.1/neural_commons/cf_nn/lrs/
--rw-rw-rw-   0        0        0     2832 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/cf_nn/lrs/AdaptiveLRS.py
--rw-rw-rw-   0        0        0      985 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/cf_nn/lrs/CrossEntropyLossLRS.py
--rw-rw-rw-   0        0        0      989 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/cf_nn/lrs/MSELossLRS.py
--rw-rw-rw-   0        0        0     1437 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/cf_nn/lrs/SlideLRS.py
--rw-rw-rw-   0        0        0      160 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/cf_nn/lrs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 01:11:01.229304 neural-commons-0.3.1/neural_commons/cf_nn/tests/
--rw-rw-rw-   0        0        0        0 2024-05-18 16:33:26.000000 neural-commons-0.3.1/neural_commons/cf_nn/tests/__init__.py
--rw-rw-rw-   0        0        0     7672 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/cf_nn/tests/test_cf_optimizer.py
--rw-rw-rw-   0        0        0     1073 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/cf_nn/tests/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-20 01:11:01.229304 neural-commons-0.3.1/neural_commons/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.3.1/neural_commons/helpers/__init__.py
--rw-rw-rw-   0        0        0     5844 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/helpers/torch_helper.py
-drwxrwxrwx   0        0        0        0 2024-05-20 01:11:01.260556 neural-commons-0.3.1/neural_commons/modules/
--rw-rw-rw-   0        0        0      699 2024-04-28 15:00:31.000000 neural-commons-0.3.1/neural_commons/modules/AdaptiveSimpleNorm.py
--rw-rw-rw-   0        0        0      288 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/modules/ArgMax.py
--rw-rw-rw-   0        0        0     1791 2024-04-10 19:02:18.000000 neural-commons-0.3.1/neural_commons/modules/ConvMixer2d.py
--rw-rw-rw-   0        0        0      248 2024-04-07 23:57:05.000000 neural-commons-0.3.1/neural_commons/modules/GTanh.py
--rw-rw-rw-   0        0        0      283 2024-04-07 23:57:05.000000 neural-commons-0.3.1/neural_commons/modules/GaELU.py
--rw-rw-rw-   0        0        0      312 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/modules/GaussianNoise.py
--rw-rw-rw-   0        0        0     1266 2024-04-28 15:00:31.000000 neural-commons-0.3.1/neural_commons/modules/InputEncoder.py
--rw-rw-rw-   0        0        0      463 2024-04-07 23:57:05.000000 neural-commons-0.3.1/neural_commons/modules/LogShape.py
--rw-rw-rw-   0        0        0      203 2024-05-02 14:19:58.000000 neural-commons-0.3.1/neural_commons/modules/MAELoss.py
--rw-rw-rw-   0        0        0     2188 2024-04-28 15:00:31.000000 neural-commons-0.3.1/neural_commons/modules/NeuralLayer.py
--rw-rw-rw-   0        0        0      842 2024-04-28 15:00:31.000000 neural-commons-0.3.1/neural_commons/modules/NeuralLayer2d.py
--rw-rw-rw-   0        0        0      477 2024-04-07 23:57:05.000000 neural-commons-0.3.1/neural_commons/modules/ParametricReLU.py
--rw-rw-rw-   0        0        0      225 2024-04-10 19:01:12.000000 neural-commons-0.3.1/neural_commons/modules/Permute.py
--rw-rw-rw-   0        0        0      286 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/modules/Plus.py
--rw-rw-rw-   0        0        0      472 2024-04-28 15:00:31.000000 neural-commons-0.3.1/neural_commons/modules/Quadratic.py
--rw-rw-rw-   0        0        0      235 2024-04-28 15:00:31.000000 neural-commons-0.3.1/neural_commons/modules/RMSELoss.py
--rw-rw-rw-   0        0        0      470 2024-04-28 15:00:31.000000 neural-commons-0.3.1/neural_commons/modules/RndNonLinearFunction.py
--rw-rw-rw-   0        0        0     1708 2024-04-07 23:57:05.000000 neural-commons-0.3.1/neural_commons/modules/RndProjection.py
--rw-rw-rw-   0        0        0     2952 2024-04-08 16:14:56.000000 neural-commons-0.3.1/neural_commons/modules/SMoE.py
--rw-rw-rw-   0        0        0      750 2024-04-07 23:57:05.000000 neural-commons-0.3.1/neural_commons/modules/SMoEMixIn.py
--rw-rw-rw-   0        0        0      232 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/modules/View.py
--rw-rw-rw-   0        0        0      714 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 01:11:01.260556 neural-commons-0.3.1/neural_commons/opt/
--rw-rw-rw-   0        0        0     1909 2024-04-28 15:00:31.000000 neural-commons-0.3.1/neural_commons/opt/CosineScheduleOptimizer.py
--rw-rw-rw-   0        0        0     1428 2024-04-28 15:00:31.000000 neural-commons-0.3.1/neural_commons/opt/CosineScheduler.py
--rw-rw-rw-   0        0        0     2066 2024-04-28 15:00:31.000000 neural-commons-0.3.1/neural_commons/opt/TBCosineScheduleOptimizer.py
--rw-rw-rw-   0        0        0      174 2024-04-28 15:00:31.000000 neural-commons-0.3.1/neural_commons/opt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 01:11:01.260556 neural-commons-0.3.1/neural_commons/q_nn/
--rw-rw-rw-   0        0        0     2287 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/q_nn/ParamModule.py
--rw-rw-rw-   0        0        0     7158 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/q_nn/QGRFOptimizer.py
--rw-rw-rw-   0        0        0     1196 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/q_nn/QLinear.py
--rw-rw-rw-   0        0        0      342 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/q_nn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 01:11:01.276176 neural-commons-0.3.1/neural_commons/q_nn/tests/
--rw-rw-rw-   0        0        0        0 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/q_nn/tests/__init__.py
--rw-rw-rw-   0        0        0     5786 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/q_nn/tests/test_qgrf_optimizer.py
--rw-rw-rw-   0        0        0     1073 2024-05-19 22:28:27.000000 neural-commons-0.3.1/neural_commons/q_nn/tests/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-20 01:11:01.213677 neural-commons-0.3.1/neural_commons.egg-info/
--rw-rw-rw-   0        0        0      745 2024-05-20 01:11:01.000000 neural-commons-0.3.1/neural_commons.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2023 2024-05-20 01:11:01.000000 neural-commons-0.3.1/neural_commons.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 01:11:01.000000 neural-commons-0.3.1/neural_commons.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-05-20 01:11:01.000000 neural-commons-0.3.1/neural_commons.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-20 01:11:01.000000 neural-commons-0.3.1/neural_commons.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 01:11:01.276176 neural-commons-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      969 2024-05-20 01:10:40.000000 neural-commons-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:59:39.650250 neural-commons-0.3.2/
+-rw-rw-rw-   0        0        0      622 2024-05-23 13:59:39.650250 neural-commons-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      155 2024-05-23 13:58:37.000000 neural-commons-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 13:59:39.556498 neural-commons-0.3.2/neural_commons/
+-rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.3.2/neural_commons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:59:39.572123 neural-commons-0.3.2/neural_commons/cf_nn/
+-rw-rw-rw-   0        0        0     3302 2024-05-19 22:28:27.000000 neural-commons-0.3.2/neural_commons/cf_nn/CFConv2d.py
+-rw-rw-rw-   0        0        0     1575 2024-05-19 22:28:27.000000 neural-commons-0.3.2/neural_commons/cf_nn/CFLinear.py
+-rw-rw-rw-   0        0        0     1228 2024-05-19 22:28:27.000000 neural-commons-0.3.2/neural_commons/cf_nn/CFModule.py
+-rw-rw-rw-   0        0        0    10584 2024-05-20 01:06:32.000000 neural-commons-0.3.2/neural_commons/cf_nn/CFOptimizer.py
+-rw-rw-rw-   0        0        0      363 2024-05-19 22:28:27.000000 neural-commons-0.3.2/neural_commons/cf_nn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:59:39.587750 neural-commons-0.3.2/neural_commons/cf_nn/lrs/
+-rw-rw-rw-   0        0        0     2832 2024-05-19 22:28:27.000000 neural-commons-0.3.2/neural_commons/cf_nn/lrs/AdaptiveLRS.py
+-rw-rw-rw-   0        0        0      985 2024-05-19 22:28:27.000000 neural-commons-0.3.2/neural_commons/cf_nn/lrs/CrossEntropyLossLRS.py
+-rw-rw-rw-   0        0        0      989 2024-05-19 22:28:27.000000 neural-commons-0.3.2/neural_commons/cf_nn/lrs/MSELossLRS.py
+-rw-rw-rw-   0        0        0     1437 2024-05-19 22:28:27.000000 neural-commons-0.3.2/neural_commons/cf_nn/lrs/SlideLRS.py
+-rw-rw-rw-   0        0        0      160 2024-05-19 22:28:27.000000 neural-commons-0.3.2/neural_commons/cf_nn/lrs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:59:39.587750 neural-commons-0.3.2/neural_commons/cf_nn/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-18 16:33:26.000000 neural-commons-0.3.2/neural_commons/cf_nn/tests/__init__.py
+-rw-rw-rw-   0        0        0     7672 2024-05-19 22:28:27.000000 neural-commons-0.3.2/neural_commons/cf_nn/tests/test_cf_optimizer.py
+-rw-rw-rw-   0        0        0     1073 2024-05-19 22:28:27.000000 neural-commons-0.3.2/neural_commons/cf_nn/tests/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:59:39.587750 neural-commons-0.3.2/neural_commons/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.3.2/neural_commons/helpers/__init__.py
+-rw-rw-rw-   0        0        0     5844 2024-05-19 22:28:27.000000 neural-commons-0.3.2/neural_commons/helpers/torch_helper.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:59:39.634624 neural-commons-0.3.2/neural_commons/modules/
+-rw-rw-rw-   0        0        0      699 2024-04-28 15:00:31.000000 neural-commons-0.3.2/neural_commons/modules/AdaptiveSimpleNorm.py
+-rw-rw-rw-   0        0        0      288 2024-05-19 22:28:27.000000 neural-commons-0.3.2/neural_commons/modules/ArgMax.py
+-rw-rw-rw-   0        0        0     1791 2024-04-10 19:02:18.000000 neural-commons-0.3.2/neural_commons/modules/ConvMixer2d.py
+-rw-rw-rw-   0        0        0      248 2024-04-07 23:57:05.000000 neural-commons-0.3.2/neural_commons/modules/GTanh.py
+-rw-rw-rw-   0        0        0      283 2024-04-07 23:57:05.000000 neural-commons-0.3.2/neural_commons/modules/GaELU.py
+-rw-rw-rw-   0        0        0      312 2024-05-19 22:28:27.000000 neural-commons-0.3.2/neural_commons/modules/GaussianNoise.py
+-rw-rw-rw-   0        0        0     1266 2024-04-28 15:00:31.000000 neural-commons-0.3.2/neural_commons/modules/InputEncoder.py
+-rw-rw-rw-   0        0        0      463 2024-04-07 23:57:05.000000 neural-commons-0.3.2/neural_commons/modules/LogShape.py
+-rw-rw-rw-   0        0        0      203 2024-05-02 14:19:58.000000 neural-commons-0.3.2/neural_commons/modules/MAELoss.py
+-rw-rw-rw-   0        0        0     2188 2024-04-28 15:00:31.000000 neural-commons-0.3.2/neural_commons/modules/NeuralLayer.py
+-rw-rw-rw-   0        0        0      842 2024-04-28 15:00:31.000000 neural-commons-0.3.2/neural_commons/modules/NeuralLayer2d.py
+-rw-rw-rw-   0        0        0      477 2024-04-07 23:57:05.000000 neural-commons-0.3.2/neural_commons/modules/ParametricReLU.py
+-rw-rw-rw-   0        0        0      225 2024-04-10 19:01:12.000000 neural-commons-0.3.2/neural_commons/modules/Permute.py
+-rw-rw-rw-   0        0        0      286 2024-05-19 22:28:27.000000 neural-commons-0.3.2/neural_commons/modules/Plus.py
+-rw-rw-rw-   0        0        0      472 2024-04-28 15:00:31.000000 neural-commons-0.3.2/neural_commons/modules/Quadratic.py
+-rw-rw-rw-   0        0        0      235 2024-04-28 15:00:31.000000 neural-commons-0.3.2/neural_commons/modules/RMSELoss.py
+-rw-rw-rw-   0        0        0      470 2024-04-28 15:00:31.000000 neural-commons-0.3.2/neural_commons/modules/RndNonLinearFunction.py
+-rw-rw-rw-   0        0        0     1708 2024-04-07 23:57:05.000000 neural-commons-0.3.2/neural_commons/modules/RndProjection.py
+-rw-rw-rw-   0        0        0     2952 2024-04-08 16:14:56.000000 neural-commons-0.3.2/neural_commons/modules/SMoE.py
+-rw-rw-rw-   0        0        0      750 2024-04-07 23:57:05.000000 neural-commons-0.3.2/neural_commons/modules/SMoEMixIn.py
+-rw-rw-rw-   0        0        0      232 2024-05-19 22:28:27.000000 neural-commons-0.3.2/neural_commons/modules/View.py
+-rw-rw-rw-   0        0        0      714 2024-05-19 22:28:27.000000 neural-commons-0.3.2/neural_commons/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:59:39.634624 neural-commons-0.3.2/neural_commons/opt/
+-rw-rw-rw-   0        0        0     1909 2024-04-28 15:00:31.000000 neural-commons-0.3.2/neural_commons/opt/CosineScheduleOptimizer.py
+-rw-rw-rw-   0        0        0     1428 2024-04-28 15:00:31.000000 neural-commons-0.3.2/neural_commons/opt/CosineScheduler.py
+-rw-rw-rw-   0        0        0     2066 2024-04-28 15:00:31.000000 neural-commons-0.3.2/neural_commons/opt/TBCosineScheduleOptimizer.py
+-rw-rw-rw-   0        0        0      174 2024-04-28 15:00:31.000000 neural-commons-0.3.2/neural_commons/opt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:59:39.634624 neural-commons-0.3.2/neural_commons/q_nn/
+-rw-rw-rw-   0        0        0     2157 2024-05-23 13:56:40.000000 neural-commons-0.3.2/neural_commons/q_nn/ParamModule.py
+-rw-rw-rw-   0        0        0     7468 2024-05-23 13:53:33.000000 neural-commons-0.3.2/neural_commons/q_nn/QGRFOptimizer.py
+-rw-rw-rw-   0        0        0     1207 2024-05-22 19:47:30.000000 neural-commons-0.3.2/neural_commons/q_nn/QLinear.py
+-rw-rw-rw-   0        0        0      342 2024-05-22 19:46:27.000000 neural-commons-0.3.2/neural_commons/q_nn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:59:39.650250 neural-commons-0.3.2/neural_commons/q_nn/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-19 22:28:27.000000 neural-commons-0.3.2/neural_commons/q_nn/tests/__init__.py
+-rw-rw-rw-   0        0        0     5786 2024-05-19 22:28:27.000000 neural-commons-0.3.2/neural_commons/q_nn/tests/test_qgrf_optimizer.py
+-rw-rw-rw-   0        0        0     1073 2024-05-19 22:28:27.000000 neural-commons-0.3.2/neural_commons/q_nn/tests/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:59:39.556498 neural-commons-0.3.2/neural_commons.egg-info/
+-rw-rw-rw-   0        0        0      622 2024-05-23 13:59:39.000000 neural-commons-0.3.2/neural_commons.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2023 2024-05-23 13:59:39.000000 neural-commons-0.3.2/neural_commons.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 13:59:39.000000 neural-commons-0.3.2/neural_commons.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-05-23 13:59:39.000000 neural-commons-0.3.2/neural_commons.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-23 13:59:39.000000 neural-commons-0.3.2/neural_commons.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 13:59:39.650250 neural-commons-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      969 2024-05-23 13:57:50.000000 neural-commons-0.3.2/setup.py
```

### Comparing `neural-commons-0.3.1/PKG-INFO` & `neural-commons-0.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-commons
-Version: 0.3.1
+Version: 0.3.2
 Summary: A neural network utility library for PyTorch.
 Author: Jose Solorzano
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.23
@@ -19,8 +19,7 @@
 
 ## Installation
 
     pip install neural-commons
 
 ## Features and Utilities
 
-- [Closed-Form Optimization](https://github.com/jose-solorzano/neural-commons/blob/main/doc/closed-form-optimization.md)
```

### Comparing `neural-commons-0.3.1/neural_commons/cf_nn/CFConv2d.py` & `neural-commons-0.3.2/neural_commons/cf_nn/CFConv2d.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/cf_nn/CFLinear.py` & `neural-commons-0.3.2/neural_commons/cf_nn/CFLinear.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/cf_nn/CFModule.py` & `neural-commons-0.3.2/neural_commons/cf_nn/CFModule.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/cf_nn/CFOptimizer.py` & `neural-commons-0.3.2/neural_commons/cf_nn/CFOptimizer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/cf_nn/lrs/AdaptiveLRS.py` & `neural-commons-0.3.2/neural_commons/cf_nn/lrs/AdaptiveLRS.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/cf_nn/lrs/CrossEntropyLossLRS.py` & `neural-commons-0.3.2/neural_commons/cf_nn/lrs/CrossEntropyLossLRS.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/cf_nn/lrs/MSELossLRS.py` & `neural-commons-0.3.2/neural_commons/cf_nn/lrs/MSELossLRS.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/cf_nn/lrs/SlideLRS.py` & `neural-commons-0.3.2/neural_commons/cf_nn/lrs/SlideLRS.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/cf_nn/tests/test_cf_optimizer.py` & `neural-commons-0.3.2/neural_commons/cf_nn/tests/test_cf_optimizer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/cf_nn/tests/utils.py` & `neural-commons-0.3.2/neural_commons/cf_nn/tests/utils.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/helpers/torch_helper.py` & `neural-commons-0.3.2/neural_commons/helpers/torch_helper.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/modules/AdaptiveSimpleNorm.py` & `neural-commons-0.3.2/neural_commons/modules/AdaptiveSimpleNorm.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/modules/ConvMixer2d.py` & `neural-commons-0.3.2/neural_commons/modules/ConvMixer2d.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/modules/InputEncoder.py` & `neural-commons-0.3.2/neural_commons/modules/InputEncoder.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/modules/NeuralLayer.py` & `neural-commons-0.3.2/neural_commons/modules/NeuralLayer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/modules/NeuralLayer2d.py` & `neural-commons-0.3.2/neural_commons/modules/NeuralLayer2d.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/modules/RndProjection.py` & `neural-commons-0.3.2/neural_commons/modules/RndProjection.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/modules/SMoE.py` & `neural-commons-0.3.2/neural_commons/modules/SMoE.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/modules/SMoEMixIn.py` & `neural-commons-0.3.2/neural_commons/modules/SMoEMixIn.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/modules/__init__.py` & `neural-commons-0.3.2/neural_commons/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/opt/CosineScheduleOptimizer.py` & `neural-commons-0.3.2/neural_commons/opt/CosineScheduleOptimizer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/opt/CosineScheduler.py` & `neural-commons-0.3.2/neural_commons/opt/CosineScheduler.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/opt/TBCosineScheduleOptimizer.py` & `neural-commons-0.3.2/neural_commons/opt/TBCosineScheduleOptimizer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/q_nn/ParamModule.py` & `neural-commons-0.3.2/neural_commons/q_nn/ParamModule.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,33 @@
-from typing import Optional
+from typing import Optional, Sequence
 import torch
 from torch import nn, autograd
 
+from neural_commons.helpers.torch_helper import rms
+
 
 class ParamModule(nn.Module):
     gradients: Optional[tuple[torch.Tensor, ...]]
     lr: Optional[torch.Tensor]
 
-    def __init__(self, *tensors: torch.Tensor, approx_lr: float = None,
-                 alpha: float = 0.3, scale: float = None):
+    def __init__(self, tensors: Sequence[torch.Tensor],
+                 approx_lr: float = None,
+                 alpha: float = 0.3):
         super().__init__()
         num_tensors = len(tensors)
         if num_tensors == 0:
             raise ValueError("At least one tensor must be provided.")
         for i, t in enumerate(tensors):
             self.register_buffer(f"tensor{i}", t.requires_grad_())
         first_tensor = tensors[0]
         self.num_tensors = num_tensors
         self.gradients = None
         self.lr = None
         self.alpha = alpha
         self.approx_lr_ma = approx_lr or 0.5 * first_tensor.size(0)
-        if scale is not None:
-            self.scale = scale
-        else:
-            rms = torch.sqrt(torch.mean(first_tensor.pow(2))).item()
-            self.scale = 1.0 if rms == 0 else rms
 
     def update_approx_lr(self, lr: float):
         self.approx_lr_ma = lr * self.alpha + self.approx_lr_ma * (1 - self.alpha)
 
     def get_approx_lr(self) -> float:
         return self.approx_lr_ma
 
@@ -41,15 +39,15 @@
         self.gradients = None
         self.lr = None
 
     @property
     def tensors(self) -> tuple[torch.Tensor, ...]:
         return tuple(getattr(self, f"tensor{i}") for i in range(self.num_tensors))
 
-    def increment_tensors(self, offsets: tuple[torch.Tensor, ...]):
+    def increment_tensors(self, offsets: Sequence[torch.Tensor]):
         for i in range(self.num_tensors):
             attr = f"tensor{i}"
             tensor = getattr(self, attr)
             setattr(self, attr, (tensor + offsets[i]).detach().requires_grad_())
 
     def grad(self, loss: torch.Tensor) -> tuple[torch.Tensor, ...]:
         return autograd.grad(loss, self.tensors)
```

### Comparing `neural-commons-0.3.1/neural_commons/q_nn/QGRFOptimizer.py` & `neural-commons-0.3.2/neural_commons/q_nn/QGRFOptimizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import math
 from typing import Iterable, Protocol, Union, Optional
 import torch
 from torch import autograd
 
+from neural_commons.helpers.torch_helper import rms
 from neural_commons.q_nn import ParamModule
 
 
 class _TLossFn1(Protocol):
     def __call__(self) -> torch.Tensor:
         ...
 
@@ -16,24 +17,19 @@
         ...
 
 
 _TLossFn = Union[_TLossFn1, _TLossFn2]
 
 
 class QGRFOptimizer:
-    def __init__(self, p_modules: Iterable[ParamModule], stochastic_selection: bool = False,
-                 initial_lr: float = 1.0,
-                 alpha: float = 0.1, global_lr_weight: float = 0):
+    def __init__(self, p_modules: Iterable[ParamModule], stochastic_selection: bool = False):
         self.p_modules = list(p_modules)
         if len(self.p_modules) == 0:
             raise ValueError("Empty collection of ParamModules provided.")
         self.selected_index = -1
-        self.global_lr_ma = initial_lr
-        self.global_lr_weight = global_lr_weight
-        self.alpha = alpha
         self.stochastic_selection = stochastic_selection
 
     @classmethod
     def _lr_loss_grad(cls, fwd_fn: _TLossFn, sm: ParamModule, p_grads: tuple[torch.Tensor, ...],
                       lr: float, l1_lambda: float, l2_lambda: float, dev: torch.device,
                       **kwargs) -> tuple[float, float]:
         lr_t = torch.tensor(lr, device=dev, dtype=torch.float).requires_grad_()
@@ -56,95 +52,107 @@
                 lr_loss = cls._fwd_loss(fwd_fn, sm, l1_lambda, l2_lambda, **kwargs)
                 return lr_loss.item()
             finally:
                 sm.clear_gradient()
 
     @staticmethod
     def _optimal_lr(lr1: float, lr2: float, lr_loss1: float, lr_loss2: float,
-                    lr_grad1: float, lr_grad2: float, lr_expansion=2.0) -> tuple[float, Optional[float]]:
+                    lr_grad1: float, lr_grad2: float, lr_expansion: float) -> tuple[float, Optional[float]]:
         if math.isinf(lr_grad2) or math.isnan(lr_grad2):
             return lr1, 1.0 / lr_expansion,
         elif math.copysign(1, lr_grad1) != math.copysign(1, lr_grad2):
             # Secant root-finding method
             return (lr1 * lr_grad2 - lr2 * lr_grad1) / (lr_grad2 - lr_grad1), None,
         elif lr_loss2 == lr_loss1:
             return lr1, 1.0,
         elif lr_loss2 < lr_loss1:
             return lr2, lr_expansion,
         else:
             return lr1, 1.0 / lr_expansion,
 
     def _update_pm(self, pm: ParamModule, p_grads: tuple[torch.Tensor, ...],
                    lr: float, update_rate: float,
-                   prior_approx_lr: float, approx_lr_factor: float):
+                   prior_approx_lr: float, approx_lr_factor: float,
+                   max_change: float):
         if approx_lr_factor is not None:
             new_approx_lr = prior_approx_lr * approx_lr_factor
         else:
             new_approx_lr = lr
         pm.update_approx_lr(new_approx_lr)
-        self.global_lr_ma = new_approx_lr * self.alpha + self.global_lr_ma * (1 - self.alpha)
         if lr == 0:
             return
-        eff_lr = lr * update_rate
-        increments = tuple(-g * eff_lr for g in p_grads)
-        pm.increment_tensors(increments)
+        with torch.no_grad():
+            eff_lr = lr * update_rate
+            increments = []
+            m_tensors = pm.tensors
+            g: torch.Tensor
+            for g, t in zip(p_grads, m_tensors):
+                change = -g * eff_lr
+                max_change_rms = rms(t) * max_change
+                change_rms = rms(change)
+                if change_rms > max_change_rms:
+                    change *= max_change_rms / change_rms
+                increments.append(change)
+            pm.increment_tensors(increments)
 
     @staticmethod
     def _get_extra_loss(sm: ParamModule, l1_lambda: float,
                         l2_lambda: float) -> torch.Tensor:
         fixed_tensors = sm.tensors
         live_tensors = sm()
         elem_count = 0
         sq_value_sums = []
         abs_value_sums = []
         for lt, ft in zip(live_tensors, fixed_tensors):
             elem_count += torch.numel(lt)
-            diff = lt - ft.detach()
-            sq_value_sums.append(torch.sum(diff.pow(2)).view(1))
-            abs_value_sums.append(torch.sum(torch.abs(diff)).view(1))
+            sq_value_sums.append(torch.sum(lt.pow(2)).view(1))
+            abs_value_sums.append(torch.sum(torch.abs(lt)).view(1))
         mean_sq_value = torch.sum(torch.cat(sq_value_sums)) / elem_count
         mean_abs_value = torch.sum(torch.cat(abs_value_sums)) / elem_count
         return l1_lambda * mean_abs_value + l2_lambda * mean_sq_value
 
     @classmethod
     def _fwd_loss(cls, fwd_fn: _TLossFn, sm: ParamModule,
                   l1_lambda: float, l2_lambda: float, **kwargs):
         return fwd_fn(**kwargs) + cls._get_extra_loss(sm, l1_lambda, l2_lambda)
 
     def get_approx_lr(self, sm: ParamModule):
-        sm_approx_lr = sm.approx_lr_ma
-        return self.global_lr_ma * self.global_lr_weight + sm_approx_lr * (1 - self.global_lr_weight)
+        return sm.approx_lr_ma
 
     def _step(self, fwd_fn: _TLossFn, sm: ParamModule, update_rate: float,
-              l1_lambda: float, l2_lambda: float, lr_expansion=2.0, **kwargs):
+              l1_lambda: float, l2_lambda: float, max_change: float,
+              lr_expansion: float = 2.0, **kwargs):
         loss = self._fwd_loss(fwd_fn, sm, l1_lambda, l2_lambda, **kwargs)
         dev = loss.device
         p_grads = sm.grad(loss)
         p_grads = tuple(g.detach() for g in p_grads)
         loss = loss.item()
         approx_lr = self.get_approx_lr(sm)
         lr1 = 0
         lr2 = approx_lr * 2.0
         lr_loss1, lr_grad1 = self._lr_loss_grad(fwd_fn, sm, p_grads, lr1,
                                                 l1_lambda, l2_lambda,
                                                 dev, **kwargs)
         lr_loss2, lr_grad2 = self._lr_loss_grad(fwd_fn, sm, p_grads, lr2,
                                                 l1_lambda, l2_lambda,
                                                 dev, **kwargs)
-        opt_lr, approx_lr_factor = self._optimal_lr(lr1, lr2, lr_loss1, lr_loss2, lr_grad1, lr_grad2)
+        opt_lr, approx_lr_factor = self._optimal_lr(lr1, lr2, lr_loss1, lr_loss2, lr_grad1, lr_grad2,
+                                                    lr_expansion=lr_expansion)
         if approx_lr_factor is None:
-            if self._simple_loss(fwd_fn, sm, p_grads, opt_lr, l1_lambda, l2_lambda, dev, **kwargs) > lr_loss1:
+            if self._simple_loss(fwd_fn, sm, p_grads, opt_lr, l1_lambda, l2_lambda,
+                                 dev, **kwargs) > lr_loss1:
                 # Failed to decrease loss. Reduce approx LR.
                 opt_lr = lr1
                 approx_lr_factor = 1.0 / lr_expansion
-        self._update_pm(sm, p_grads, opt_lr, update_rate, approx_lr, approx_lr_factor)
+        self._update_pm(sm, p_grads, opt_lr, update_rate, approx_lr, approx_lr_factor,
+                        max_change=max_change)
         return loss
 
     def step(self, fwd_fn: _TLossFn, update_rate: float = 1.0, l1_lambda: float = 0.001,
-             l2_lambda: float = 0.001, **kwargs) -> float:
+             l2_lambda: float = 0.001, max_change: float = 0.3, **kwargs) -> float:
         if update_rate <= 0 or update_rate > 1.0:
             raise ValueError("update_rate expected to be in ]0, 1].")
         p_modules = self.p_modules
         num_modules = len(p_modules)
         if self.stochastic_selection:
             m_lr = [m.approx_lr_ma for m in p_modules]
             m_lr = torch.tensor(m_lr, dtype=torch.float)
@@ -152,8 +160,9 @@
             self.selected_index = torch.multinomial(m_weight, 1).item()
         else:
             self.selected_index = (self.selected_index + 1) % num_modules
         selected_module = p_modules[self.selected_index]
         return self._step(fwd_fn, selected_module,
                           update_rate=update_rate,
                           l1_lambda=l1_lambda, l2_lambda=l2_lambda,
+                          max_change=max_change,
                           **kwargs)
```

### Comparing `neural-commons-0.3.1/neural_commons/q_nn/QLinear.py` & `neural-commons-0.3.2/neural_commons/q_nn/QLinear.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 
 
 class QLinear(nn.Module):
     __constants__ = ["in_features", "out_features"]
 
     def __init__(self, in_features: int, out_features: int, bias: bool = True):
         super().__init__()
-        scale = math.sqrt(in_features)
+        inv_scale = math.sqrt(in_features)
         if bias:
-            scale *= _sqrt_2
-        weight = torch.randn((out_features, in_features)) / scale
+            inv_scale *= _sqrt_2
+        weight = torch.randn((out_features, in_features)) / inv_scale
         bias_param = torch.randn((out_features,)) / _sqrt_2 if bias else None
         p_tensors = [weight]
         if bias_param is not None:
             p_tensors.append(bias_param)
-        self.p_module = ParamModule(*p_tensors)
+        self.p_module = ParamModule(p_tensors)
         self.bias = bias
         self.in_features = in_features
         self.out_features = out_features
 
     def forward(self, x: torch.Tensor):
         if self.bias:
             w, b = self.p_module()
```

### Comparing `neural-commons-0.3.1/neural_commons/q_nn/tests/test_qgrf_optimizer.py` & `neural-commons-0.3.2/neural_commons/q_nn/tests/test_qgrf_optimizer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons/q_nn/tests/utils.py` & `neural-commons-0.3.2/neural_commons/q_nn/tests/utils.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/neural_commons.egg-info/PKG-INFO` & `neural-commons-0.3.2/neural_commons.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-commons
-Version: 0.3.1
+Version: 0.3.2
 Summary: A neural network utility library for PyTorch.
 Author: Jose Solorzano
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.23
@@ -19,8 +19,7 @@
 
 ## Installation
 
     pip install neural-commons
 
 ## Features and Utilities
 
-- [Closed-Form Optimization](https://github.com/jose-solorzano/neural-commons/blob/main/doc/closed-form-optimization.md)
```

### Comparing `neural-commons-0.3.1/neural_commons.egg-info/SOURCES.txt` & `neural-commons-0.3.2/neural_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.1/setup.py` & `neural-commons-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import codecs
 
 from setuptools import setup, find_packages
 
 # Define project metadata
 NAME = 'neural-commons'
-VERSION = '0.3.1'
+VERSION = '0.3.2'
 DESCRIPTION = 'A neural network utility library for PyTorch.'
 AUTHOR = 'Jose Solorzano'
 
 REQUIRES = [
     'numpy>=1.23',
     'tqdm>=4.0.0',
     'torch>=2.1.0',
```

