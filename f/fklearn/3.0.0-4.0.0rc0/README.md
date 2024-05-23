# Comparing `tmp/fklearn-3.0.0.tar.gz` & `tmp/fklearn-4.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fklearn-3.0.0.tar", last modified: Thu Nov  9 12:59:33 2023, max compression
+gzip compressed data, was "fklearn-4.0.0rc0.tar", last modified: Thu May 23 14:10:35 2024, max compression
```

## Comparing `fklearn-3.0.0.tar` & `fklearn-4.0.0rc0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:33.705347 fklearn-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2023-11-09 12:59:12.000000 fklearn-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-11-09 12:59:12.000000 fklearn-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2023-11-09 12:59:33.705347 fklearn-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2023-11-09 12:59:12.000000 fklearn-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-11-09 12:59:12.000000 fklearn-3.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-11-09 12:59:12.000000 fklearn-3.0.0/requirements_catboost.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-09 12:59:12.000000 fklearn-3.0.0/requirements_demos.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-09 12:59:12.000000 fklearn-3.0.0/requirements_lgbm.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-11-09 12:59:12.000000 fklearn-3.0.0/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-11-09 12:59:12.000000 fklearn-3.0.0/requirements_tools.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-09 12:59:12.000000 fklearn-3.0.0/requirements_xgboost.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-09 12:59:33.705347 fklearn-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-11-09 12:59:12.000000 fklearn-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:33.689348 fklearn-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:33.693348 fklearn-3.0.0/src/fklearn/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:33.693348 fklearn-3.0.0/src/fklearn/causal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/causal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:33.693348 fklearn-3.0.0/src/fklearn/causal/cate_learning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/causal/cate_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7897 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/causal/cate_learning/double_machine_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)    14729 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/causal/cate_learning/meta_learners.py
--rw-r--r--   0 runner    (1001) docker     (127)     8895 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/causal/debias.py
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/causal/effects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:33.697347 fklearn-3.0.0/src/fklearn/causal/validation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/causal/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6623 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/causal/validation/auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6793 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/causal/validation/cate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9808 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/causal/validation/curves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/common_docstrings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:33.697347 fklearn-3.0.0/src/fklearn/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/data/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:33.697347 fklearn-3.0.0/src/fklearn/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:33.697347 fklearn-3.0.0/src/fklearn/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/metrics/pd_extractors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:33.697347 fklearn-3.0.0/src/fklearn/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/preprocessing/rebalancing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/preprocessing/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     8511 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/preprocessing/splitting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:33.697347 fklearn-3.0.0/src/fklearn/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/resources/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:33.697347 fklearn-3.0.0/src/fklearn/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/training/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)    31195 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/training/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     7024 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/training/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/training/imputation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/training/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    27167 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/training/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    36612 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/training/transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/training/unsupervised.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/training/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:33.701347 fklearn-3.0.0/src/fklearn/tuning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/tuning/model_agnostic_fc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8606 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/tuning/parameter_tuners.py
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/tuning/samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17970 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/tuning/selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5743 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/tuning/stoppers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/tuning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:33.701347 fklearn-3.0.0/src/fklearn/types/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/types/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:33.701347 fklearn-3.0.0/src/fklearn/validation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36847 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/validation/evaluators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/validation/perturbators.py
--rw-r--r--   0 runner    (1001) docker     (127)    32870 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/validation/splitters.py
--rw-r--r--   0 runner    (1001) docker     (127)    12367 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/validation/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-11-09 12:59:12.000000 fklearn-3.0.0/src/fklearn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 12:59:33.693348 fklearn-3.0.0/src/fklearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2023-11-09 12:59:33.000000 fklearn-3.0.0/src/fklearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2023-11-09 12:59:33.000000 fklearn-3.0.0/src/fklearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-09 12:59:33.000000 fklearn-3.0.0/src/fklearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-09 12:59:33.000000 fklearn-3.0.0/src/fklearn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      724 2023-11-09 12:59:33.000000 fklearn-3.0.0/src/fklearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-09 12:59:33.000000 fklearn-3.0.0/src/fklearn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:35.145338 fklearn-4.0.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-23 14:10:35.141338 fklearn-4.0.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/requirements_catboost.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/requirements_demos.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/requirements_lgbm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/requirements_tools.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/requirements_xgboost.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 14:10:35.145338 fklearn-4.0.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:35.125338 fklearn-4.0.0rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:35.129338 fklearn-4.0.0rc0/src/fklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:35.133338 fklearn-4.0.0rc0/src/fklearn/causal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/causal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:35.133338 fklearn-4.0.0rc0/src/fklearn/causal/cate_learning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/causal/cate_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7897 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/causal/cate_learning/double_machine_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14729 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/causal/cate_learning/meta_learners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/causal/debias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/causal/effects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:35.133338 fklearn-4.0.0rc0/src/fklearn/causal/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/causal/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/causal/validation/auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/causal/validation/cate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/causal/validation/curves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/common_docstrings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:35.133338 fklearn-4.0.0rc0/src/fklearn/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/data/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:35.133338 fklearn-4.0.0rc0/src/fklearn/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:35.133338 fklearn-4.0.0rc0/src/fklearn/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/metrics/pd_extractors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:35.133338 fklearn-4.0.0rc0/src/fklearn/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/preprocessing/rebalancing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/preprocessing/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/preprocessing/splitting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:35.133338 fklearn-4.0.0rc0/src/fklearn/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/resources/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:35.137338 fklearn-4.0.0rc0/src/fklearn/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/training/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31195 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/training/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/training/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/training/imputation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/training/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27167 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/training/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36612 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/training/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/training/unsupervised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/training/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:35.137338 fklearn-4.0.0rc0/src/fklearn/tuning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/tuning/model_agnostic_fc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8606 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/tuning/parameter_tuners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/tuning/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17970 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/tuning/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/tuning/stoppers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/tuning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:35.137338 fklearn-4.0.0rc0/src/fklearn/types/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/types/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:35.137338 fklearn-4.0.0rc0/src/fklearn/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36847 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/validation/evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/validation/perturbators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32870 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/validation/splitters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12370 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/validation/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-23 14:10:31.000000 fklearn-4.0.0rc0/src/fklearn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:10:35.137338 fklearn-4.0.0rc0/src/fklearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-23 14:10:35.000000 fklearn-4.0.0rc0/src/fklearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-23 14:10:35.000000 fklearn-4.0.0rc0/src/fklearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:10:35.000000 fklearn-4.0.0rc0/src/fklearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:10:34.000000 fklearn-4.0.0rc0/src/fklearn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-23 14:10:35.000000 fklearn-4.0.0rc0/src/fklearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 14:10:35.000000 fklearn-4.0.0rc0/src/fklearn.egg-info/top_level.txt
```

### Comparing `fklearn-3.0.0/LICENSE` & `fklearn-4.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/PKG-INFO` & `fklearn-4.0.0rc0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: fklearn
-Version: 3.0.0
+Version: 4.0.0rc0
 Summary: Functional machine learning
 Home-page: https://github.com/nubank/fklearn
 Author: Nubank
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8,<3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8,<3.12,!=3.10.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: joblib<2,>=1.3.2
 Requires-Dist: numpy<2,>=1.24.4
 Requires-Dist: pandas<3,>=2
-Requires-Dist: scikit-learn<2,>=1
+Requires-Dist: scikit-learn<1.4,>=1
 Requires-Dist: statsmodels<1,>=0.14.0
 Requires-Dist: toolz<1,>=0.12.0
 Provides-Extra: test-deps
 Requires-Dist: pytest<8,>=7.4.3; extra == "test-deps"
 Requires-Dist: pytest-cov<3,>=2.6.1; extra == "test-deps"
 Requires-Dist: pytest-xdist<4,>=3.3.1; extra == "test-deps"
 Requires-Dist: mypy<2,>=1.6.1; extra == "test-deps"
@@ -26,38 +27,38 @@
 Provides-Extra: lgbm
 Requires-Dist: lightgbm<5,>=4; extra == "lgbm"
 Provides-Extra: xgboost
 Requires-Dist: xgboost<3,>=2; extra == "xgboost"
 Provides-Extra: catboost
 Requires-Dist: catboost<2,>=1.2.2; extra == "catboost"
 Provides-Extra: tools
-Requires-Dist: shap<1,>=0.43; extra == "tools"
+Requires-Dist: shap<0.45,>=0.43; extra == "tools"
 Requires-Dist: swifter<2,>=0.24; extra == "tools"
 Provides-Extra: devel
 Requires-Dist: pytest<8,>=7.4.3; extra == "devel"
 Requires-Dist: pytest-cov<3,>=2.6.1; extra == "devel"
 Requires-Dist: pytest-xdist<4,>=3.3.1; extra == "devel"
 Requires-Dist: mypy<2,>=1.6.1; extra == "devel"
 Requires-Dist: coverage<5; extra == "devel"
 Requires-Dist: codecov<3,>=2.0; extra == "devel"
 Requires-Dist: hypothesis<7,>=6.88.3; extra == "devel"
 Requires-Dist: lightgbm<5,>=4; extra == "devel"
 Requires-Dist: xgboost<3,>=2; extra == "devel"
 Requires-Dist: catboost<2,>=1.2.2; extra == "devel"
-Requires-Dist: shap<1,>=0.43; extra == "devel"
+Requires-Dist: shap<0.45,>=0.43; extra == "devel"
 Requires-Dist: swifter<2,>=0.24; extra == "devel"
 Provides-Extra: all-models
 Requires-Dist: lightgbm<5,>=4; extra == "all-models"
 Requires-Dist: xgboost<3,>=2; extra == "all-models"
 Requires-Dist: catboost<2,>=1.2.2; extra == "all-models"
 Provides-Extra: all
 Requires-Dist: lightgbm<5,>=4; extra == "all"
 Requires-Dist: xgboost<3,>=2; extra == "all"
 Requires-Dist: catboost<2,>=1.2.2; extra == "all"
-Requires-Dist: shap<1,>=0.43; extra == "all"
+Requires-Dist: shap<0.45,>=0.43; extra == "all"
 Requires-Dist: swifter<2,>=0.24; extra == "all"
 
 # fklearn: Functional Machine Learning
 
 ![PyPI](https://img.shields.io/pypi/v/fklearn.svg?style=flat-square)
 [![Documentation Status](https://readthedocs.org/projects/fklearn/badge/?version=latest)](https://fklearn.readthedocs.io/en/latest/?badge=latest)
 [![Gitter](https://badges.gitter.im/fklearn-python/community.svg)](https://gitter.im/fklearn-python/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
```

### Comparing `fklearn-3.0.0/README.md` & `fklearn-4.0.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/setup.py` & `fklearn-4.0.0rc0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     long_description = fh.read()
 
 setup(name=MODULE_NAME,
       description="Functional machine learning",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/nubank/{:s}'.format(REPO_NAME),
-      python_requires='>=3.8,<3.10',
+      python_requires='>=3.8,<3.12,!=3.10.*',
       author="Nubank",
       package_dir={'': 'src'},
       packages=find_packages('src'),
       version=(open(join('src', MODULE_NAME, 'resources', 'VERSION'))
                .read().strip()),
       install_requires=core_deps,
       extras_require={"test_deps": test_deps,
@@ -49,9 +49,10 @@
                       "devel": devel_deps,
                       "all_models": all_models_deps,
                       "all": all_deps},
       include_package_data=True,
       zip_safe=False,
       classifiers=[
           'Programming Language :: Python :: 3.8',
-          'Programming Language :: Python :: 3.9'
+          'Programming Language :: Python :: 3.9',
+          'Programming Language :: Python :: 3.11',
           ])
```

### Comparing `fklearn-3.0.0/src/fklearn/causal/cate_learning/double_machine_learning.py` & `fklearn-4.0.0rc0/src/fklearn/causal/cate_learning/double_machine_learning.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/causal/cate_learning/meta_learners.py` & `fklearn-4.0.0rc0/src/fklearn/causal/cate_learning/meta_learners.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/causal/debias.py` & `fklearn-4.0.0rc0/src/fklearn/causal/debias.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/causal/effects.py` & `fklearn-4.0.0rc0/src/fklearn/causal/effects.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/causal/validation/auc.py` & `fklearn-4.0.0rc0/src/fklearn/causal/validation/auc.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/causal/validation/cate.py` & `fklearn-4.0.0rc0/src/fklearn/causal/validation/cate.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/causal/validation/curves.py` & `fklearn-4.0.0rc0/src/fklearn/causal/validation/curves.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/common_docstrings.py` & `fklearn-4.0.0rc0/src/fklearn/common_docstrings.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/data/datasets.py` & `fklearn-4.0.0rc0/src/fklearn/data/datasets.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/exceptions/exceptions.py` & `fklearn-4.0.0rc0/src/fklearn/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/metrics/pd_extractors.py` & `fklearn-4.0.0rc0/src/fklearn/metrics/pd_extractors.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/preprocessing/rebalancing.py` & `fklearn-4.0.0rc0/src/fklearn/preprocessing/rebalancing.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/preprocessing/schema.py` & `fklearn-4.0.0rc0/src/fklearn/preprocessing/schema.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/preprocessing/splitting.py` & `fklearn-4.0.0rc0/src/fklearn/preprocessing/splitting.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/training/calibration.py` & `fklearn-4.0.0rc0/src/fklearn/training/calibration.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/training/classification.py` & `fklearn-4.0.0rc0/src/fklearn/training/classification.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/training/ensemble.py` & `fklearn-4.0.0rc0/src/fklearn/training/ensemble.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/training/imputation.py` & `fklearn-4.0.0rc0/src/fklearn/training/imputation.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/training/pipeline.py` & `fklearn-4.0.0rc0/src/fklearn/training/pipeline.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/training/regression.py` & `fklearn-4.0.0rc0/src/fklearn/training/regression.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/training/transformation.py` & `fklearn-4.0.0rc0/src/fklearn/training/transformation.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/training/unsupervised.py` & `fklearn-4.0.0rc0/src/fklearn/training/unsupervised.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/training/utils.py` & `fklearn-4.0.0rc0/src/fklearn/training/utils.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/tuning/model_agnostic_fc.py` & `fklearn-4.0.0rc0/src/fklearn/tuning/model_agnostic_fc.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/tuning/parameter_tuners.py` & `fklearn-4.0.0rc0/src/fklearn/tuning/parameter_tuners.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/tuning/samplers.py` & `fklearn-4.0.0rc0/src/fklearn/tuning/samplers.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/tuning/selectors.py` & `fklearn-4.0.0rc0/src/fklearn/tuning/selectors.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/tuning/stoppers.py` & `fklearn-4.0.0rc0/src/fklearn/tuning/stoppers.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/tuning/utils.py` & `fklearn-4.0.0rc0/src/fklearn/tuning/utils.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/types/types.py` & `fklearn-4.0.0rc0/src/fklearn/types/types.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/validation/evaluators.py` & `fklearn-4.0.0rc0/src/fklearn/validation/evaluators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1061,11 +1061,11 @@
     log: dict
         A log-like dictionary with the logistic coefficient
     """
 
     if eval_name is None:
         eval_name = "logistic_coefficient_evaluator__" + target_column
 
-    score = LogisticRegression(penalty="none", multi_class="ovr").fit(test_data[[prediction_column]],
+    score = LogisticRegression(penalty='none', multi_class="ovr").fit(test_data[[prediction_column]],
                                                                       test_data[target_column]).coef_[0][0]
 
     return {eval_name: score}
```

### Comparing `fklearn-3.0.0/src/fklearn/validation/perturbators.py` & `fklearn-4.0.0rc0/src/fklearn/validation/perturbators.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/validation/splitters.py` & `fklearn-4.0.0rc0/src/fklearn/validation/splitters.py`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn/validation/validator.py` & `fklearn-4.0.0rc0/src/fklearn/validation/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,19 +204,19 @@
         train_log["train_log"] = validator_log["train_log"]
         return train_log, assoc(dissoc(validator_log, "train_log"), "split_log", split_log)
 
     def get_perturbed_columns(perturbator: PerturbFnType) -> List[str]:
         args = inspect.getfullargspec(perturbator).kwonlydefaults
         return args['cols'] if args else []
 
-    train_logs, validator_logs = zip(*map(_join_split_log, zipped_logs))
+    train_logs_, validator_logs = zip(*map(_join_split_log, zipped_logs))
     if return_all_train_logs:
-        train_logs = {"train_log": [log["train_log"] for log in train_logs]}
+        train_logs = {"train_log": [log["train_log"] for log in train_logs_]}
     else:
-        train_logs = first(train_logs)
+        train_logs = first(train_logs_)
 
     perturbator_log = {'perturbated_train': [], 'perturbated_test': []}  # type: LogType
     if perturb_fn_train != identity:
         perturbator_log['perturbated_train'] = get_perturbed_columns(perturb_fn_train)
     if perturb_fn_test != identity:
         perturbator_log['perturbated_test'] = get_perturbed_columns(perturb_fn_test)
     train_logs = assoc(train_logs, "perturbator_log", perturbator_log)
```

### Comparing `fklearn-3.0.0/src/fklearn.egg-info/PKG-INFO` & `fklearn-4.0.0rc0/src/fklearn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: fklearn
-Version: 3.0.0
+Version: 4.0.0rc0
 Summary: Functional machine learning
 Home-page: https://github.com/nubank/fklearn
 Author: Nubank
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8,<3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8,<3.12,!=3.10.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: joblib<2,>=1.3.2
 Requires-Dist: numpy<2,>=1.24.4
 Requires-Dist: pandas<3,>=2
-Requires-Dist: scikit-learn<2,>=1
+Requires-Dist: scikit-learn<1.4,>=1
 Requires-Dist: statsmodels<1,>=0.14.0
 Requires-Dist: toolz<1,>=0.12.0
 Provides-Extra: test-deps
 Requires-Dist: pytest<8,>=7.4.3; extra == "test-deps"
 Requires-Dist: pytest-cov<3,>=2.6.1; extra == "test-deps"
 Requires-Dist: pytest-xdist<4,>=3.3.1; extra == "test-deps"
 Requires-Dist: mypy<2,>=1.6.1; extra == "test-deps"
@@ -26,38 +27,38 @@
 Provides-Extra: lgbm
 Requires-Dist: lightgbm<5,>=4; extra == "lgbm"
 Provides-Extra: xgboost
 Requires-Dist: xgboost<3,>=2; extra == "xgboost"
 Provides-Extra: catboost
 Requires-Dist: catboost<2,>=1.2.2; extra == "catboost"
 Provides-Extra: tools
-Requires-Dist: shap<1,>=0.43; extra == "tools"
+Requires-Dist: shap<0.45,>=0.43; extra == "tools"
 Requires-Dist: swifter<2,>=0.24; extra == "tools"
 Provides-Extra: devel
 Requires-Dist: pytest<8,>=7.4.3; extra == "devel"
 Requires-Dist: pytest-cov<3,>=2.6.1; extra == "devel"
 Requires-Dist: pytest-xdist<4,>=3.3.1; extra == "devel"
 Requires-Dist: mypy<2,>=1.6.1; extra == "devel"
 Requires-Dist: coverage<5; extra == "devel"
 Requires-Dist: codecov<3,>=2.0; extra == "devel"
 Requires-Dist: hypothesis<7,>=6.88.3; extra == "devel"
 Requires-Dist: lightgbm<5,>=4; extra == "devel"
 Requires-Dist: xgboost<3,>=2; extra == "devel"
 Requires-Dist: catboost<2,>=1.2.2; extra == "devel"
-Requires-Dist: shap<1,>=0.43; extra == "devel"
+Requires-Dist: shap<0.45,>=0.43; extra == "devel"
 Requires-Dist: swifter<2,>=0.24; extra == "devel"
 Provides-Extra: all-models
 Requires-Dist: lightgbm<5,>=4; extra == "all-models"
 Requires-Dist: xgboost<3,>=2; extra == "all-models"
 Requires-Dist: catboost<2,>=1.2.2; extra == "all-models"
 Provides-Extra: all
 Requires-Dist: lightgbm<5,>=4; extra == "all"
 Requires-Dist: xgboost<3,>=2; extra == "all"
 Requires-Dist: catboost<2,>=1.2.2; extra == "all"
-Requires-Dist: shap<1,>=0.43; extra == "all"
+Requires-Dist: shap<0.45,>=0.43; extra == "all"
 Requires-Dist: swifter<2,>=0.24; extra == "all"
 
 # fklearn: Functional Machine Learning
 
 ![PyPI](https://img.shields.io/pypi/v/fklearn.svg?style=flat-square)
 [![Documentation Status](https://readthedocs.org/projects/fklearn/badge/?version=latest)](https://fklearn.readthedocs.io/en/latest/?badge=latest)
 [![Gitter](https://badges.gitter.im/fklearn-python/community.svg)](https://gitter.im/fklearn-python/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
```

### Comparing `fklearn-3.0.0/src/fklearn.egg-info/SOURCES.txt` & `fklearn-4.0.0rc0/src/fklearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fklearn-3.0.0/src/fklearn.egg-info/requires.txt` & `fklearn-4.0.0rc0/src/fklearn.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 joblib<2,>=1.3.2
 numpy<2,>=1.24.4
 pandas<3,>=2
-scikit-learn<2,>=1
+scikit-learn<1.4,>=1
 statsmodels<1,>=0.14.0
 toolz<1,>=0.12.0
 
 [all]
 lightgbm<5,>=4
 xgboost<3,>=2
 catboost<2,>=1.2.2
-shap<1,>=0.43
+shap<0.45,>=0.43
 swifter<2,>=0.24
 
 [all_models]
 lightgbm<5,>=4
 xgboost<3,>=2
 catboost<2,>=1.2.2
 
@@ -27,15 +27,15 @@
 mypy<2,>=1.6.1
 coverage<5
 codecov<3,>=2.0
 hypothesis<7,>=6.88.3
 lightgbm<5,>=4
 xgboost<3,>=2
 catboost<2,>=1.2.2
-shap<1,>=0.43
+shap<0.45,>=0.43
 swifter<2,>=0.24
 
 [lgbm]
 lightgbm<5,>=4
 
 [test_deps]
 pytest<8,>=7.4.3
@@ -43,12 +43,12 @@
 pytest-xdist<4,>=3.3.1
 mypy<2,>=1.6.1
 coverage<5
 codecov<3,>=2.0
 hypothesis<7,>=6.88.3
 
 [tools]
-shap<1,>=0.43
+shap<0.45,>=0.43
 swifter<2,>=0.24
 
 [xgboost]
 xgboost<3,>=2
```

