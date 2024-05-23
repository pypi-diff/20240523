# Comparing `tmp/autogluon.tabular-1.1.1b20240521.tar.gz` & `tmp/autogluon.tabular-1.1.1b20240522.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.tabular-1.1.1b20240521.tar", last modified: Tue May 21 09:04:48 2024, max compression
+gzip compressed data, was "autogluon.tabular-1.1.1b20240522.tar", last modified: Wed May 22 09:05:24 2024, max compression
```

## Comparing `autogluon.tabular-1.1.1b20240521.tar` & `autogluon.tabular-1.1.1b20240522.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.144139 autogluon.tabular-1.1.1b20240521/
--rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-05-21 09:04:48.144139 autogluon.tabular-1.1.1b20240521/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:04:48.144139 autogluon.tabular-1.1.1b20240521/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.124139 autogluon.tabular-1.1.1b20240521/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.124139 autogluon.tabular-1.1.1b20240521/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.128139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.132139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21132 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/configs/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/configs/feature_generator_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    16315 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/configs/hyperparameter_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.132139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/configs/zeroshot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/configs/zeroshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/configs/zeroshot/zeroshot_portfolio_2023.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.132139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/experimental/_scikit_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/experimental/_tabular_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/experimental/_tabular_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.132139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/learner/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51900 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/learner/abstract_learner.py
--rw-r--r--   0 runner    (1001) docker     (127)    23537 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/learner/default_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.132139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.132139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/_utils/rapids_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/_utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.132139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/automm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/automm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/automm/automm_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/automm/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.132139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/catboost/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/catboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/catboost/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    16575 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/catboost/catboost_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/catboost/catboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.132139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/catboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.132139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fastainn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fastainn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fastainn/callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1379 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fastainn/fastai_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.132139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fastainn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fastainn/imports_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fastainn/quantile_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27704 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.136139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fasttext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fasttext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fasttext/fasttext_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.136139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fasttext/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.136139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/image_prediction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/image_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/image_prediction/image_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.136139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/imodels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/imodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/imodels/imodels_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.136139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/knn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/knn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/knn/_knn_loo_variants.py
--rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/knn/knn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/knn/knn_rapids_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/knn/knn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.136139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lgb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lgb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lgb/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.136139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lgb/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    19709 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lgb/lgb_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lgb/lgb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.136139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.136139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lr/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    14076 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lr/lr_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lr/lr_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.136139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/rf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/rf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.136139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/rf/compilers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/rf/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/rf/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/rf/compilers/onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)    20606 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/rf/rf_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    36460 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/rf/rf_quantile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/rf/rf_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.140139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tab_transformer/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tab_transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.140139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tab_transformer/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    22903 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tab_transformer/pretexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24707 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    22651 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tab_transformer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.140139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabpfn/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabpfn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabpfn/tabpfn_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.140139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.140139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/compilers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (127)    14804 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.140139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.140139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/torch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32664 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
--rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.140139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34250 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.140139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/text_prediction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/text_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.140139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/vowpalwabbit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/vowpalwabbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.140139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/xgboost/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/xgboost/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.144139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/xgboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/xgboost/xgboost_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/xgboost/xgboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.144139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/xt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/xt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/xt/xt_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.144139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/predictor/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/predictor/_deprecated_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/predictor/interpretable_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)   317268 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/predictor/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.144139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.144139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/trainer/model_presets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/trainer/model_presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17843 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/trainer/model_presets/presets.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/trainer/model_presets/presets_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/trainer/model_presets/presets_distill.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.144139 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/tuning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-21 09:03:46.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/tuning/feature_pruner.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-21 09:04:47.000000 autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:04:48.128139 autogluon.tabular-1.1.1b20240521/src/autogluon.tabular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-05-21 09:04:48.000000 autogluon.tabular-1.1.1b20240521/src/autogluon.tabular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-05-21 09:04:48.000000 autogluon.tabular-1.1.1b20240521/src/autogluon.tabular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:04:48.000000 autogluon.tabular-1.1.1b20240521/src/autogluon.tabular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 09:04:48.000000 autogluon.tabular-1.1.1b20240521/src/autogluon.tabular.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-21 09:04:48.000000 autogluon.tabular-1.1.1b20240521/src/autogluon.tabular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 09:04:48.000000 autogluon.tabular-1.1.1b20240521/src/autogluon.tabular.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:04:48.000000 autogluon.tabular-1.1.1b20240521/src/autogluon.tabular.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.153293 autogluon.tabular-1.1.1b20240522/
+-rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-05-22 09:05:24.153293 autogluon.tabular-1.1.1b20240522/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 09:05:24.153293 autogluon.tabular-1.1.1b20240522/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.133293 autogluon.tabular-1.1.1b20240522/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.133293 autogluon.tabular-1.1.1b20240522/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.137293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.137293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21132 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/configs/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/configs/feature_generator_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16315 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/configs/hyperparameter_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.137293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/configs/zeroshot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/configs/zeroshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/configs/zeroshot/zeroshot_portfolio_2023.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.137293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/experimental/_scikit_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/experimental/_tabular_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/experimental/_tabular_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.137293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/learner/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51900 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/learner/abstract_learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23263 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/learner/default_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.137293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.141293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/_utils/rapids_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/_utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.141293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/automm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/automm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/automm/automm_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/automm/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.141293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/catboost/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/catboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/catboost/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16575 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/catboost/catboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/catboost/catboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.141293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/catboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.141293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fastainn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fastainn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fastainn/callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1379 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fastainn/fastai_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.141293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fastainn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fastainn/imports_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fastainn/quantile_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27704 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.141293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fasttext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fasttext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fasttext/fasttext_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.141293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fasttext/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.141293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/image_prediction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/image_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/image_prediction/image_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.141293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/imodels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/imodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/imodels/imodels_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.141293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/knn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/knn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/knn/_knn_loo_variants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/knn/knn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/knn/knn_rapids_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/knn/knn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.145293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lgb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lgb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lgb/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.145293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lgb/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19709 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lgb/lgb_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lgb/lgb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.145293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.145293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lr/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14076 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lr/lr_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lr/lr_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.145293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/rf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/rf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.145293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/rf/compilers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/rf/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/rf/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/rf/compilers/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20606 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/rf/rf_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36460 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/rf/rf_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/rf/rf_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.145293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tab_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tab_transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.145293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tab_transformer/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22903 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tab_transformer/pretexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24707 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22651 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tab_transformer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.145293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabpfn/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabpfn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabpfn/tabpfn_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.145293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.145293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/compilers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14804 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.149293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.149293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32664 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.149293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34250 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.149293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/text_prediction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/text_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.149293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/vowpalwabbit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/vowpalwabbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.149293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/xgboost/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.149293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/xgboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/xgboost/xgboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/xgboost/xgboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.149293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/xt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/xt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/xt/xt_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.149293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/predictor/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/predictor/_deprecated_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/predictor/interpretable_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)   322666 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/predictor/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.149293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.149293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/trainer/model_presets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/trainer/model_presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17843 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/trainer/model_presets/presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/trainer/model_presets/presets_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/trainer/model_presets/presets_distill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.153293 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/tuning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-22 09:04:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/tuning/feature_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-22 09:05:23.000000 autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:05:24.137293 autogluon.tabular-1.1.1b20240522/src/autogluon.tabular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-05-22 09:05:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon.tabular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-05-22 09:05:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon.tabular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 09:05:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon.tabular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 09:05:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon.tabular.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-22 09:05:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon.tabular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 09:05:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon.tabular.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 09:05:24.000000 autogluon.tabular-1.1.1b20240522/src/autogluon.tabular.egg-info/zip-safe
```

### Comparing `autogluon.tabular-1.1.1b20240521/PKG-INFO` & `autogluon.tabular-1.1.1b20240522/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 1.1.1b20240521
+Version: 1.1.1b20240522
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.tabular-1.1.1b20240521/setup.py` & `autogluon.tabular-1.1.1b20240522/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/configs/config_helper.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/configs/config_helper.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/configs/feature_generator_presets.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/configs/feature_generator_presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/configs/hyperparameter_configs.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/configs/hyperparameter_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/configs/presets_configs.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/configs/zeroshot/zeroshot_portfolio_2023.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/configs/zeroshot/zeroshot_portfolio_2023.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/experimental/_scikit_mixin.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/experimental/_scikit_mixin.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/experimental/_tabular_classifier.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/experimental/_tabular_classifier.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/experimental/_tabular_regressor.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/experimental/_tabular_regressor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/learner/abstract_learner.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/learner/default_learner.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/learner/default_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import time
 
 import numpy as np
 import pandas as pd
 from pandas import DataFrame
 
 from autogluon.common.utils.log_utils import convert_time_in_s_to_log_friendly
-from autogluon.common.utils.system_info import get_ag_system_info
 from autogluon.core.constants import AUTO_WEIGHT, BALANCE_WEIGHT, BINARY, MULTICLASS, QUANTILE, REGRESSION
 from autogluon.core.data import LabelCleaner
 from autogluon.core.data.cleaner import Cleaner
 from autogluon.core.utils.time import sample_df_for_time_func, time_func
 from autogluon.core.utils.utils import augment_rare_classes, extract_column
 
 from ..trainer import AutoTrainer
@@ -61,23 +60,18 @@
         num_bag_folds (int): kfolds used for bagging of models, roughly increases model training time by a factor of k (0: disabled)
         num_bag_sets (int): number of repeats of kfold bagging to perform (values must be >= 1),
             total number of models trained during bagging = num_bag_folds * num_bag_sets
         """
         # TODO: if provided, feature_types in X, X_val are ignored right now, need to pass to Learner/trainer and update this documentation.
         self._time_limit = time_limit
         if time_limit:
-            logger.log(20, f"Beginning AutoGluon training ... Time limit = {time_limit}s")
+            logger.log(20, f"Beginning AutoGluon training ... Time limit = {time_limit:.0f}s")
         else:
             logger.log(20, "Beginning AutoGluon training ...")
         logger.log(20, f'AutoGluon will save models to "{self.path}"')
-        include_gpu_count = False
-        if verbosity >= 3:
-            include_gpu_count = True
-        msg = get_ag_system_info(path=self.path, include_gpu_count=include_gpu_count)
-        logger.log(20, msg)
         logger.log(20, f"Train Data Rows:    {len(X)}")
         logger.log(20, f"Train Data Columns: {len([column for column in X.columns if column != self.label])}")
         if X_val is not None:
             logger.log(20, f"Tuning Data Rows:    {len(X_val)}")
             logger.log(20, f"Tuning Data Columns: {len([column for column in X_val.columns if column != self.label])}")
         logger.log(20, f"Label Column:       {self.label}")
         time_preprocessing_start = time.time()
```

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/__init__.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/_utils/rapids_utils.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/_utils/rapids_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/_utils/torch_utils.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/_utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/automm/automm_model.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/automm/automm_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/automm/ft_transformer.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/automm/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/catboost/callbacks.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/catboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/catboost/catboost_model.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/catboost/catboost_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/catboost/catboost_utils.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/catboost/catboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fastainn/callbacks.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fastainn/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fastainn/fastai_helpers.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fastainn/fastai_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fastainn/quantile_helpers.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fastainn/quantile_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fasttext/fasttext_model.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fasttext/fasttext_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/image_prediction/image_predictor.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/image_prediction/image_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/imodels/imodels_models.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/imodels/imodels_models.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/knn/_knn_loo_variants.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/knn/_knn_loo_variants.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/knn/knn_model.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/knn/knn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/knn/knn_rapids_model.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/knn/knn_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/knn/knn_utils.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/knn/knn_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lgb/callbacks.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lgb/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lgb/lgb_model.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lgb/lgb_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lgb/lgb_utils.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lgb/lgb_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lr/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lr/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lr/lr_model.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lr/lr_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/lr/lr_rapids_model.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/lr/lr_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/rf/compilers/native.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/rf/compilers/native.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/rf/compilers/onnx.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/rf/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/rf/rf_model.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/rf/rf_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/rf/rf_quantile.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/rf/rf_quantile.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/rf/rf_rapids_model.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/rf/rf_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tab_transformer/modified_transformer.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tab_transformer/modified_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tab_transformer/pretexts.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tab_transformer/pretexts.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tab_transformer/tab_model_base.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tab_transformer/tab_model_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tab_transformer/tab_transformer.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tab_transformer/tab_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tab_transformer/utils.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tab_transformer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabpfn/tabpfn_model.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabpfn/tabpfn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/compilers/native.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/compilers/native.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/xgboost/callbacks.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/xgboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/xgboost/xgboost_model.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/xgboost/xgboost_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/xgboost/xgboost_utils.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/xgboost/xgboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/models/xt/xt_model.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/models/xt/xt_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/predictor/_deprecated_methods.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/predictor/_deprecated_methods.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/predictor/interpretable_predictor.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/predictor/interpretable_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/predictor/predictor.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/predictor/predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import pandas as pd
 
 from autogluon.common.loaders import load_json
 from autogluon.common.savers import save_json
 from autogluon.common.utils.file_utils import get_directory_size, get_directory_size_per_file
 from autogluon.common.utils.log_utils import add_log_to_file, set_logger_verbosity
 from autogluon.common.utils.pandas_utils import get_approximate_df_mem_usage
+from autogluon.common.utils.system_info import get_ag_system_info
 from autogluon.common.utils.try_import import try_import_ray
 from autogluon.common.utils.utils import (
     check_saved_predictor_version,
     compare_autogluon_metadata,
     get_autogluon_metadata,
     setup_outputdir,
 )
@@ -436,23 +437,23 @@
             Users can specify custom presets by passing in a dictionary of argument values as an element to the list.
 
             Available Presets: ['best_quality', 'high_quality', 'good_quality', 'medium_quality', 'optimize_for_deployment', 'interpretable', 'ignore_text']
 
             It is recommended to only use one `quality` based preset in a given call to `fit()` as they alter many of the same arguments and are not compatible with each-other.
 
             In-depth Preset Info:
-                best_quality={'auto_stack': True}
+                best_quality={'auto_stack': True, 'dynamic_stacking': 'auto', 'hyperparameters': 'zeroshot'}
                     Best predictive accuracy with little consideration to inference time or disk usage. Achieve even better results by specifying a large time_limit value.
                     Recommended for applications that benefit from the best possible model accuracy.
 
-                high_quality={'auto_stack': True, 'refit_full': True, 'set_best_to_refit_full': True, 'save_bag_folds': False}
-                    High predictive accuracy with fast inference. ~10x-200x faster inference and ~10x-200x lower disk usage than `best_quality`.
+                high_quality={'auto_stack': True, 'dynamic_stacking': 'auto', 'hyperparameters': 'zeroshot', 'refit_full': True, 'set_best_to_refit_full': True, 'save_bag_folds': False}
+                    High predictive accuracy with fast inference. ~8x faster inference and ~8x lower disk usage than `best_quality`.
                     Recommended for applications that require reasonable inference speed and/or model size.
 
-                good_quality={'auto_stack': True, 'refit_full': True, 'set_best_to_refit_full': True, 'save_bag_folds': False, 'hyperparameters': 'light'}
+                good_quality={'auto_stack': True, 'dynamic_stacking': 'auto', 'hyperparameters': 'light', 'refit_full': True, 'set_best_to_refit_full': True, 'save_bag_folds': False}
                     Good predictive accuracy with very fast inference. ~4x faster inference and ~4x lower disk usage than `high_quality`.
                     Recommended for applications that require fast inference speed.
 
                 medium_quality={'auto_stack': False}
                     Medium predictive accuracy with very fast inference and very fast training time. ~20x faster training than `good_quality`.
                     This is the default preset in AutoGluon, but should generally only be used for quick prototyping, as `good_quality` results in significantly better predictive accuracy and faster inference time.
 
@@ -474,17 +475,18 @@
                     Disables automated feature generation when text features are detected.
                     This is useful to determine how beneficial text features are to the end result, as well as to ensure features are not mistaken for text when they are not.
                     Ignored if `feature_generator` was also specified.
 
         hyperparameters : str or dict, default = 'default'
             Determines the hyperparameters used by the models.
             If `str` is passed, will use a preset hyperparameter configuration.
-                Valid `str` options: ['default', 'light', 'very_light', 'toy', 'multimodal']
-                    'default': Default AutoGluon hyperparameters intended to maximize accuracy without significant regard to inference time or disk usage.
-                    'light': Results in smaller models. Generally will make inference speed much faster and disk usage much lower, but with worse accuracy.
+                Valid `str` options: ['default', 'zeroshot', 'light', 'very_light', 'toy', 'multimodal']
+                    'default': Default AutoGluon hyperparameters intended to get strong accuracy with reasonable disk usage and inference time. Used in the 'medium_quality' preset.
+                    'zeroshot': A powerful model portfolio learned from TabRepo's ensemble simulation on 200 datasets. Contains ~100 models and is used in 'best_quality' and 'high_quality' presets.
+                    'light': Results in smaller models. Generally will make inference speed much faster and disk usage much lower, but with worse accuracy. Used in the 'good_quality' preset.
                     'very_light': Results in much smaller models. Behaves similarly to 'light', but in many cases with over 10x less disk usage and a further reduction in accuracy.
                     'toy': Results in extremely small models. Only use this when prototyping, as the model quality will be severely reduced.
                     'multimodal': [EXPERIMENTAL] Trains a multimodal transformer model alongside tabular models. Requires that some text columns appear in the data and GPU.
                         When combined with 'best_quality' `presets` option, this can achieve extremely strong results in multimodal data tables that contain columns with text in addition to numeric/categorical columns.
                 Reference `autogluon/tabular/configs/hyperparameter_configs.py` for information on the hyperparameters associated with each preset.
             Keys are strings that indicate which model types to train.
                 Stable model options include:
@@ -496,16 +498,17 @@
                     'KNN' (k-nearest neighbors)
                     'LR' (linear regression)
                     'NN_TORCH' (neural network implemented in Pytorch)
                     'FASTAI' (neural network with FastAI backend)
                     'AG_AUTOMM' (`MultimodalPredictor` from `autogluon.multimodal`. Supports Tabular, Text, and Image modalities. GPU is required.)
                 Experimental model options include:
                     'FT_TRANSFORMER' (Tabular Transformer, GPU is recommended. Does not scale well to >100 features.)
-                    'FASTTEXT' (FastText)
-                    'VW' (VowpalWabbit)
+                    'FASTTEXT' (FastText. Note: Has not been tested for a long time.)
+                    'TABPFN' (TabPFN. Does not scale well to >100 features or >1000 rows, and does not support regression. Extremely slow inference speed.)
+                    'VW' (VowpalWabbit. Note: Has not been tested for a long time.)
                     'AG_TEXT_NN' (Multimodal Text+Tabular model, GPU is required. Recommended to instead use its successor, 'AG_AUTOMM'.)
                     'AG_IMAGE_NN' (Image model, GPU is required. Recommended to instead use its successor, 'AG_AUTOMM'.)
                 If a certain key is missing from hyperparameters, then `fit()` will not train any models of that type. Omitting a model key from hyperparameters is equivalent to including this model key in `excluded_model_types`.
                 For example, set `hyperparameters = { 'NN_TORCH':{...} }` if say you only want to train (PyTorch) neural networks and no other types of models.
             Values = dict of hyperparameter settings for each model type, or list of dicts.
                 Each hyperparameter can either be a single fixed value or a search space containing many possible values.
                 Unspecified hyperparameters will be set to default values (or default search spaces if `hyperparameter_tune_kwargs='auto'`).
@@ -791,14 +794,17 @@
                     `memory_safe_fits` : bool, default = True
                         If True, AutoGluon runs each sub-fit in a ray-based subprocess to avoid memory leakage that exist due to Python's lackluster
                         garbage collector.
                     `clean_up_fits` : bool, default = True
                         If True, AutoGluon will remove all saved information from sub-fits from disk.
                         If False, the sub-fits are kept on disk and `self._sub_fits` will store paths to the sub-fits, which can be loaded just like any other
                         predictor from disk using `TabularPredictor.load()`.
+                    `force_ray_logging` : bool, default = False
+                        If True, will log the dynamic stacking sub-fit when ray is used (`memory_safe_fits=True`).
+                        Note that because of how ray works, this may cause extra unwanted logging in the main fit process after dynamic stacking completes.
                     `holdout_data`: str or :class:`TabularDataset` or :class:`pd.DataFrame`, default = None
                         Another dataset containing validation data reserved for detecting stacked overfitting. This dataset should be in the same format as
                         `train_data`. If str is passed, `holdout_data` will be loaded using the str value as the file path.
                         If `holdout_data` is not None, the sub-fit is fit on all of `train_data` and the full fit is fit on all of `train_data` and
                         `holdout_data` combined.
             included_model_types : list, default = None
                 To only include listed model types for training during `fit()`.
@@ -938,14 +944,26 @@
         """
         if self.is_fit:
             raise AssertionError("Predictor is already fit! To fit additional models, refer to `predictor.fit_extra`, or create a new `Predictor`.")
 
         verbosity = kwargs.get("verbosity", self.verbosity)
         set_logger_verbosity(verbosity)
 
+        if verbosity >= 2:
+            if verbosity == 2:
+                logger.log(20, f"Verbosity: 2 (Standard Logging)")
+            elif verbosity == 3:
+                logger.log(20, f"Verbosity: 3 (Detailed Logging)")
+            elif verbosity >= 4:
+                logger.log(20, f"Verbosity: {verbosity} (Maximum Logging)")
+
+        include_gpu_count = verbosity >= 3
+        sys_msg = get_ag_system_info(path=self.path, include_gpu_count=include_gpu_count)
+        logger.log(20, sys_msg)
+
         if presets:
             if not isinstance(presets, list):
                 presets = [presets]
             logger.log(20, f"Presets specified: {presets}")
         else:
             logger.log(
                 20,
@@ -1123,22 +1141,28 @@
             calibrate=kwargs["calibrate"],
             calibrate_decision_threshold=calibrate_decision_threshold,
             infer_limit=infer_limit,
         )
         if dynamic_stacking:
             logger.log(
                 20,
-                f"Dynamic stacking is enabled (dynamic_stacking={dynamic_stacking}). "
+                f"DyStack is enabled (dynamic_stacking={dynamic_stacking}). "
                 "AutoGluon will try to determine whether the input data is affected by stacked overfitting and enable or disable stacking as a consequence.",
             )
             num_stack_levels, time_limit = self._dynamic_stacking(**ds_args, ag_fit_kwargs=ag_fit_kwargs, ag_post_fit_kwargs=ag_post_fit_kwargs)
+            logger.info(
+                f"Starting main fit with num_stack_levels={num_stack_levels}.\n"
+                f"\tFor future fit calls on this dataset, you can skip dynamic stacking to save time: "
+                f"`predictor.fit(..., dynamic_stacking=False, num_stack_levels={num_stack_levels})`"
+            )
 
             if (time_limit is not None) and (time_limit <= 0):
-                raise ValueError(
-                    f"Not enough time left to train models for the full fit. Consider specifying a larger time_limit. Time remaining: {time_limit}s"
+                raise AssertionError(
+                    f"Not enough time left to train models for the full fit. "
+                    f"Consider specifying a larger time_limit or setting `dynamic_stacking=False`. Time remaining: {time_limit:.2f}s"
                 )
 
             ag_fit_kwargs["num_stack_levels"] = num_stack_levels
             ag_fit_kwargs["time_limit"] = time_limit
 
         self._fit(ag_fit_kwargs=ag_fit_kwargs, ag_post_fit_kwargs=ag_post_fit_kwargs)
 
@@ -1159,33 +1183,34 @@
         validation_procedure: bool,
         detection_time_frac: float,
         holdout_frac: float,
         n_folds: int,
         n_repeats: int,
         memory_safe_fits: bool,
         clean_up_fits: bool,
+        force_ray_logging: bool,
         holdout_data: Optional[Union[str, pd.DataFrame, None]] = None,
     ):
         """Dynamically determines if stacking is used or not by validating the behavior of a sub-fit of AutoGluon that uses stacking on held out data.
         See `ds_args` in the docstring of `fit()` for details on the parameters."""
         time_start = time.time()
         time_limit_og = ag_fit_kwargs["time_limit"]
         org_num_stack_levels = ag_fit_kwargs["num_stack_levels"]
         ds_fit_context = os.path.join(self._learner.path_context_og, "ds_sub_fit")
         logger.info(
-            "Detecting stacked overfitting by sub-fitting AutoGluon on the input data. "
-            "That is, copies of AutoGluon will be sub-fit on subset(s) of the data. "
-            "Then, the holdout validation data is used to detect stacked overfitting."
+            "\tThis is used to identify the optimal `num_stack_levels` value. "
+            "Copies of AutoGluon will be fit on subsets of the data. "
+            "Then holdout validation data is used to detect stacked overfitting."
         )
 
         if time_limit_og is not None:
-            logger.info(f"Sub-fit(s) time limit is: {time_limit_og} seconds.")
             time_limit = int(time_limit_og * detection_time_frac)
+            logger.info(f"\tRunning DyStack for up to {time_limit}s of the {time_limit_og}s of remaining time ({detection_time_frac*100:.0f}%).")
         else:
-            logger.info(f"No time limit provided.")
+            logger.info(f"\tWarning: No time limit provided for DyStack. This could take awhile.")
             time_limit = None
 
         # -- Avoid copying data
         X = ag_fit_kwargs.pop("X")
         X_val = ag_fit_kwargs.pop("X_val")
         X_unlabeled = ag_fit_kwargs.pop("X_unlabeled")
         inner_ag_fit_kwargs = copy.deepcopy(ag_fit_kwargs)
@@ -1199,136 +1224,167 @@
         # Verify problem type is set
         if self.problem_type is None:
             self._learner.problem_type = self._learner.infer_problem_type(y=X[self.label], silent=True)
 
         ds_fit_kwargs = dict(
             clean_up_fits=clean_up_fits,
             memory_safe_fits=memory_safe_fits,
+            force_ray_logging=force_ray_logging,
         )
 
         # -- Validation Method
         if validation_procedure == "holdout":
             if holdout_data is None:
                 ds_fit_kwargs.update(dict(holdout_frac=holdout_frac, ds_fit_context=os.path.join(ds_fit_context, "sub_fit_ho")))
-                logger.info(f"Starting holdout-based sub-fit for dynamic stacking. Context path is: {ds_fit_kwargs['ds_fit_context']}.")
             else:
                 _, holdout_data, _ = self._validate_fit_data(train_data=X, tuning_data=holdout_data)
                 ds_fit_kwargs["ds_fit_context"] = os.path.join(ds_fit_context, "sub_fit_custom_ho")
-                logger.info(
-                    f"Starting holdout-based sub-fit for dynamic stacking with custom validation data. Context path is: {ds_fit_kwargs['ds_fit_context']}."
-                )
 
             stacked_overfitting = self._sub_fit_memory_save_wrapper(
                 train_data=X,
                 time_limit=time_limit,
+                time_start=time_start,
                 ds_fit_kwargs=ds_fit_kwargs,
                 ag_fit_kwargs=inner_ag_fit_kwargs,
                 ag_post_fit_kwargs=inner_ag_post_fit_kwargs,
                 holdout_data=holdout_data,
             )
         else:
             # Holdout is false, use (repeated) cross-validation
             is_stratified = self.problem_type in [REGRESSION, QUANTILE, SOFTCLASS]
             self._learner._validate_groups(X=X, X_val=X_val)  # Validate splits before splitting
             splits = CVSplitter(n_splits=n_folds, n_repeats=n_repeats, groups=self._learner.groups, stratified=is_stratified, random_state=42).split(
                 X=X.drop(self.label, axis=1), y=X[self.label]
             )
             n_splits = len(splits)
             logger.info(
-                f"Starting (repeated-)cross-validation-based sub-fits for dynamic stacking. Context path is: {ds_fit_context}. "
+                f'\tStarting (repeated-)cross-validation-based sub-fits for dynamic stacking. Context path: "{ds_fit_context}"'
                 f"Run at most {n_splits} sub-fits based on {n_repeats}-repeated {n_folds}-fold cross-validation."
             )
             np.random.RandomState(42).shuffle(splits)  # shuffle splits to mix up order such that if only one of the repeats shows leakage we might stop early.
             for split_index, (train_indices, val_indices) in enumerate(splits):
                 if time_limit is None:
                     sub_fit_time = None
                 else:
                     time_spend_sub_fits_so_far = int(time.time() - time_start)
                     rest_time = time_limit - time_spend_sub_fits_so_far
                     sub_fit_time = int(1 / (n_splits - split_index) * rest_time)  # if we are faster, give more time to rest of the folds.
                     if sub_fit_time <= 0:
-                        logger.info(f"Stop cross-validation during dynamic stacking early as no more time left. Consider specifying a larger time_limit.")
+                        logger.info(f"\tStop cross-validation during dynamic stacking early as no more time left. Consider specifying a larger time_limit.")
                         break
                 ds_fit_kwargs.update(
                     dict(
                         train_indices=train_indices,
                         val_indices=val_indices,
                         ds_fit_context=os.path.join(ds_fit_context, f"sub_fit_{split_index}"),
                     )
                 )
                 logger.info(
-                    f"Starting sub-fit {split_index + 1}. Time limit for the sub-fit of this split is: {'unlimited' if sub_fit_time is None else sub_fit_time}."
+                    f"\tStarting sub-fit {split_index + 1}. Time limit for the sub-fit of this split is: {'unlimited' if sub_fit_time is None else sub_fit_time}."
                 )
                 stacked_overfitting = self._sub_fit_memory_save_wrapper(
                     train_data=X,
                     time_limit=time_limit,
+                    time_start=time_start,
                     ds_fit_kwargs=ds_fit_kwargs,
                     ag_fit_kwargs=inner_ag_fit_kwargs,
                     ag_post_fit_kwargs=inner_ag_post_fit_kwargs,
                     holdout_data=holdout_data,
                 )
                 if stacked_overfitting:
                     break
 
             del splits
 
         if clean_up_fits:
-            shutil.rmtree(path=ds_fit_context)
+            try:
+                shutil.rmtree(path=ds_fit_context)
+            except FileNotFoundError as e:
+                pass
 
         # -- Determine rest time and new num_stack_levels
-        time_spend_sub_fits = int(time.time() - time_start)
-        logger.info(f"Spend {time_spend_sub_fits} seconds for the sub-fit(s) during dynamic stacking.")
+        time_spend_sub_fits = time.time() - time_start
+        num_stack_levels = 0 if stacked_overfitting else org_num_stack_levels
+        self._stacked_overfitting_occurred = stacked_overfitting
+
+        logger.info(f"\t{num_stack_levels}\t = Optimal   num_stack_levels (Stacked Overfitting Occurred: {self._stacked_overfitting_occurred})")
+        log_str = f"\t{round(time_spend_sub_fits)}s\t = DyStack   runtime"
         if time_limit_og is None:
             time_limit_fit_full = None
         else:
-            time_limit_fit_full = int(time_limit_og - time_spend_sub_fits)
-            logger.info(f"Time left for full fit of AutoGluon: {time_limit_fit_full} seconds.")
-
-        num_stack_levels = 0 if stacked_overfitting else org_num_stack_levels
-        self._stacked_overfitting_occurred = stacked_overfitting
+            time_limit_fit_full = time_limit_og - time_spend_sub_fits
+            log_str += f" |\t{round(time_limit_fit_full)}s\t = Remaining runtime"
+        logger.info(log_str)
 
         # -- Revert back
         del inner_ag_fit_kwargs
         if holdout_data is None:
             ag_fit_kwargs["X"] = X
         else:
-            logger.log(20, "Concatenating holdout data from dynamic stacking to the training data for the full fit (and reset the index).")
+            logger.log(20, "\tConcatenating holdout data from dynamic stacking to the training data for the full fit (and reset the index).")
             ag_fit_kwargs["X"] = pd.concat([X, holdout_data], ignore_index=True)
 
         ag_fit_kwargs["X_val"] = X_val
         ag_fit_kwargs["X_unlabeled"] = X_unlabeled
 
-        logger.info(f"Starting full fit now with num_stack_levels {num_stack_levels}.")
         return num_stack_levels, time_limit_fit_full
 
     def _sub_fit_memory_save_wrapper(
         self,
         train_data: Union[str, pd.DataFrame],
         time_limit: int,
+        time_start: float,
         ds_fit_kwargs: dict,
         ag_fit_kwargs: dict,
         ag_post_fit_kwargs: dict,
         holdout_data=Union[str, pd.DataFrame, None],
     ):
         """Tries to run the sub-fit in a subprocess (managed by ray). Similar to AutoGluon's parallel fold fitting strategies,
         this code does not shut down ray after usage. Otherwise, we would also kill outer-scope ray usage."""
         memory_safe_fits = ds_fit_kwargs.get("memory_safe_fits", True)
+        force_ray_logging = ds_fit_kwargs.get("force_ray_logging", False)
         normal_fit = False
         if memory_safe_fits:
             try:
                 _ds_ray = try_import_ray()
                 if not _ds_ray.is_initialized():
-                    _ds_ray.init(logging_level=logging.ERROR, log_to_driver=False)
+                    if force_ray_logging:
+                        logger.info(
+                            f"\tRunning DyStack sub-fit in a ray process to avoid memory leakage. "
+                            "Force enabling ray logging (force_ray_logging=True). "
+                            "This may lead to unwanted logging post-DyStack due to a limitation in ray."
+                        )
+                        _ds_ray.init()  # TODO: This will propagate to the main fit call too, which isn't ideal.
+                    else:
+                        logger.info(
+                            f"\tRunning DyStack sub-fit in a ray process to avoid memory leakage. "
+                            "Logs will not be shown until this process is complete, due to a limitation in ray. "
+                            "You can force logging by specifying `ds_args={'force_ray_logging': True}`."
+                        )
+                        _ds_ray.init(
+                            logging_level=logging.ERROR,
+                            log_to_driver=False,
+                        )
             except Exception as e:
                 warnings.warn(f"Failed to use ray for memory safe fits. Falling back to normal fit. Error: {repr(e)}", stacklevel=2)
                 _ds_ray = None
 
-            if _ds_ray is not None:
-                logger.info(f"Running the sub-fit in a ray process to avoid memory leakage.")
+            if time_limit is not None:
+                # Subtract time taken to initialize ray
+                time_limit -= time.time() - time_start
+                if time_limit <= 0:
+                    logger.log(30, f"Warning: Not enough time to fit DyStack! Skipping...")
+                    return False
 
+            if holdout_data is None:
+                logger.info(f"\t\tContext path: \"{ds_fit_kwargs['ds_fit_context']}\"")
+            else:
+                logger.info(f"\t\tRunning DyStack holdout-based sub-fit with custom validation data. Context path: \"{ds_fit_kwargs['ds_fit_context']}\"")
+
+            if _ds_ray is not None:
                 # Handle resources
                 from autogluon.common.utils.resource_utils import ResourceManager
 
                 total_resources = ag_fit_kwargs["core_kwargs"]["total_resources"]
 
                 num_cpus = total_resources.get("num_cpus", "auto")
                 num_gpus = total_resources.get("num_gpus", "auto")
@@ -1347,41 +1403,61 @@
                 if holdout_data is not None:
                     holdout_data_ref = _ds_ray.put(holdout_data)
                 else:
                     holdout_data_ref = None
 
                 # Call sub fit in its own subprocess via ray
                 sub_fit_caller = _ds_ray.remote(max_calls=1)(_sub_fit)
-                ref = sub_fit_caller.options(num_cpus=num_cpus, num_gpus=num_gpus).remote(
+                # FIXME: For some reason ray does not treat `num_cpus` and `num_gpus` the same.
+                #  For `num_gpus`, the process will reserve the capacity and is unable to share it to child ray processes, causing a deadlock.
+                #  For `num_cpus`, the value is completely ignored by children, and they can even use more num_cpus than the parent.
+                #  Because of this, num_gpus is set to 0 here to avoid a deadlock, but num_cpus does not need to be changed.
+                #  For more info, refer to Ray documentation: https://docs.ray.io/en/latest/ray-core/tasks/nested-tasks.html#yielding-resources-while-blocked
+                ref = sub_fit_caller.options(num_cpus=num_cpus, num_gpus=0).remote(
                     predictor=predictor_ref,
                     train_data=train_data_ref,
                     time_limit=time_limit,
                     ds_fit_kwargs=ds_fit_kwargs,
                     ag_fit_kwargs=ag_fit_kwargs_ref,
                     ag_post_fit_kwargs=ag_post_fit_kwargs,
                     holdout_data=holdout_data_ref,
                 )
                 finished, unfinished = _ds_ray.wait([ref], num_returns=1)
-                stacked_overfitting = _ds_ray.get(finished[0])
+                stacked_overfitting, ho_leaderboard, exception = _ds_ray.get(finished[0])
+
+                # FIXME: Add logic that does the following to switch ray's logging verbosity without adding a 5+ second overhead from shutting down the cluster.
+                # _ds_ray.shutdown()
+                # _ds_ray.init(
+                #     logging_level=logging.ERROR,
+                #     log_to_driver=False,
+                # )
             else:
                 normal_fit = True
         else:
             normal_fit = True
 
         if normal_fit:
-            stacked_overfitting = _sub_fit(
+            stacked_overfitting, ho_leaderboard, exception = _sub_fit(
                 predictor=self,
                 train_data=train_data,
                 time_limit=time_limit,
                 ds_fit_kwargs=ds_fit_kwargs,
                 ag_fit_kwargs=ag_fit_kwargs,
                 ag_post_fit_kwargs=ag_post_fit_kwargs,
                 holdout_data=holdout_data,
             )
 
+        if exception is not None:
+            logger.log(40, f"Warning: Exception encountered during DyStack sub-fit:\n\t{exception}")
+        if ho_leaderboard is not None:
+            logger.log(20, "Leaderboard on holdout data from dynamic stacking:")
+            with pd.option_context("display.max_rows", None, "display.max_columns", None, "display.width", 1000):
+                # Rename to avoid confusion for the user
+                logger.log(20, ho_leaderboard.rename({"score_test": "score_holdout"}, axis=1))
+
         return stacked_overfitting
 
     def _post_fit(
         self,
         keep_only_best=False,
         refit_full=False,
         set_best_to_refit_full=False,
@@ -1476,15 +1552,15 @@
         base_model_names: List[str] = None,
         fit_weighted_ensemble: bool = True,
         fit_full_last_level_weighted_ensemble: bool = True,
         full_weighted_ensemble_additionally: bool = False,
         num_cpus: str | int = "auto",
         num_gpus: str | int = "auto",
         **kwargs,
-    ):
+    ) -> "TabularPredictor":
         """
         Fits additional models after the original :meth:`TabularPredictor.fit` call.
         The original train_data and tuning_data will be used to train the models.
 
         Parameters
         ----------
         hyperparameters : str or dict
@@ -4423,22 +4499,22 @@
         kwargs, ds_valid_keys = self._sanitize_dynamic_stacking_kwargs(kwargs)
         kwargs = self._validate_fit_extra_kwargs(kwargs, extra_valid_keys=list(fit_kwargs_default.keys()) + ds_valid_keys)
         kwargs_sanitized = fit_kwargs_default.copy()
         kwargs_sanitized.update(kwargs)
 
         return kwargs_sanitized
 
-    def _validate_calibrate_decision_threshold(self, calibrate_decision_threshold):
+    def _validate_calibrate_decision_threshold(self, calibrate_decision_threshold: bool | str):
         valid_calibrate_decision_threshold_options = [True, False, "auto"]
         if calibrate_decision_threshold not in valid_calibrate_decision_threshold_options:
             raise ValueError(
                 f"`calibrate_decision_threshold` must be a value in " f"{valid_calibrate_decision_threshold_options}, but is: {calibrate_decision_threshold}"
             )
 
-    def _fit_extra_kwargs_dict(self):
+    def _fit_extra_kwargs_dict(self) -> dict:
         """
         Returns:
         --------
         dict of fit_extra args:
             verbosity: Which levels of logger should be printed
             pseudo_data: pseudo labeled data to be incorporated into train
                          but not used in validation
@@ -4481,29 +4557,30 @@
             detection_time_frac=1 / 4,
             holdout_frac=1 / 9,
             n_folds=2,
             n_repeats=1,
             memory_safe_fits=True,
             clean_up_fits=True,
             holdout_data=None,
+            force_ray_logging=False,
         )
         allowed_kes = set(ds_args.keys())
 
         if ds_kwargs_key in kwargs:
             kwargs[ds_kwargs_key] = copy.deepcopy(kwargs[ds_kwargs_key])
             ds_args.update(kwargs[ds_kwargs_key])
 
         key_missmatch = set(ds_args.keys()) - allowed_kes
         if key_missmatch:
             raise ValueError(f"Got invalid keys for `ds_args`. Allowed: {allowed_kes}. Got: {key_missmatch}")
         if ("validation_procedure" in ds_args) and (
             (not isinstance(ds_args["validation_procedure"], str)) or (ds_args["validation_procedure"] not in ["holdout", "cv"])
         ):
             raise ValueError("`validation_procedure` in `ds_args` must be str in {'holdout','cv'}. " + f"Got: {ds_args['validation_procedure']}")
-        for arg_name in ["memory_safe_fits", "clean_up_fits"]:
+        for arg_name in ["memory_safe_fits", "clean_up_fits", "force_ray_logging"]:
             if (arg_name in ds_args) and (not isinstance(ds_args[arg_name], bool)):
                 raise ValueError(f"`{arg_name}` in `ds_args` must be bool.  Got: {type(ds_args[arg_name])}")
         for arg_name in ["detection_time_frac", "holdout_frac"]:
             if (arg_name in ds_args) and ((not isinstance(ds_args[arg_name], float)) or (ds_args[arg_name] >= 1) or (ds_args[arg_name] <= 0)):
                 raise ValueError(f"`{arg_name}` in `ds_args` must be float in (0,1).  Got: {type(ds_args[arg_name])}, {ds_args[arg_name]}")
         if ("n_folds" in ds_args) and ((not isinstance(ds_args["n_folds"], int)) or (ds_args["n_folds"] < 2)):
             raise ValueError(f"`n_folds` in `ds_args` must be int in [2, +inf).  Got: {type(ds_args['n_folds'])}, {ds_args['n_folds']}")
@@ -4515,15 +4592,15 @@
             raise ValueError(
                 "`validation_procedure` in `ds_args` is 'cv' but `holdout_data` in `ds_args` is specified."
                 "You must decide for either (repeated) cross-validation or holdout validation."
             )
         kwargs[ds_kwargs_key] = ds_args
         return kwargs, [ds_kwargs_key]
 
-    def _validate_fit_extra_kwargs(self, kwargs, extra_valid_keys=None):
+    def _validate_fit_extra_kwargs(self, kwargs: dict, extra_valid_keys: List[str] | None = None):
         fit_extra_kwargs_default = self._fit_extra_kwargs_dict()
 
         allowed_kwarg_names = list(fit_extra_kwargs_default.keys())
         if extra_valid_keys is not None:
             allowed_kwarg_names += extra_valid_keys
         for kwarg_name in kwargs.keys():
             if kwarg_name not in allowed_kwarg_names:
@@ -4550,15 +4627,15 @@
         valid_calibrate_options = [True, False, "auto"]
         calibrate = kwargs_sanitized["calibrate"]
         if calibrate not in valid_calibrate_options:
             raise ValueError(f"`calibrate` must be a value in {valid_calibrate_options}, but is: {calibrate}")
 
         return kwargs_sanitized
 
-    def _prune_data_features(self, train_features: list, other_features: list, is_labeled: bool):
+    def _prune_data_features(self, train_features: list, other_features: list, is_labeled: bool) -> Tuple[list, list]:
         """
         Removes certain columns from the provided datasets that do not contain predictive features.
 
         Parameters
         ----------
         train_features : list
             The features/columns for the incoming training data
@@ -4574,15 +4651,20 @@
             if self.sample_weight in other_features:
                 other_features.remove(self.sample_weight)
         if self._learner.groups is not None and is_labeled:
             train_features.remove(self._learner.groups)
 
         return train_features, other_features
 
-    def _validate_fit_data(self, train_data, tuning_data=None, unlabeled_data=None):
+    def _validate_fit_data(
+        self,
+        train_data: str | pd.DataFrame,
+        tuning_data: str | pd.DataFrame | None = None,
+        unlabeled_data: str | pd.DataFrame | None = None,
+    ) -> Tuple[pd.DataFrame, pd.DataFrame | None, pd.DataFrame | None]:
         if isinstance(train_data, str):
             train_data = TabularDataset(train_data)
         if tuning_data is not None and isinstance(tuning_data, str):
             tuning_data = TabularDataset(tuning_data)
         if unlabeled_data is not None and isinstance(unlabeled_data, str):
             unlabeled_data = TabularDataset(unlabeled_data)
 
@@ -4629,15 +4711,15 @@
             if np.any(train_features != unlabeled_features):
                 raise ValueError(
                     "Column names must match between training and unlabeled data.\n" "Unlabeled data must have not the label column specified in it.\n"
                 )
         return train_data, tuning_data, unlabeled_data
 
     @staticmethod
-    def _validate_unique_indices(data, name: str):
+    def _validate_unique_indices(data: pd.DataFrame, name: str):
         is_duplicate_index = data.index.duplicated(keep=False)
         if is_duplicate_index.any():
             duplicate_count = is_duplicate_index.sum()
             raise AssertionError(
                 f"{name} contains {duplicate_count} duplicated indices. "
                 "Please ensure DataFrame indices are unique.\n"
                 f"\tYou can identify the indices which are duplicated via `{name}.index.duplicated(keep=False)`"
@@ -5064,34 +5146,36 @@
 
     ag_fit_kwargs["X"] = train_data
     ag_fit_kwargs["time_limit"] = time_limit
     ds_fit_context = ds_fit_kwargs.get("ds_fit_context")
     clean_up_fits = ds_fit_kwargs.get("clean_up_fits")
 
     predictor._learner.set_contexts(path_context=ds_fit_context)
-    predictor._fit(ag_fit_kwargs=ag_fit_kwargs, ag_post_fit_kwargs=ag_post_fit_kwargs)
+    logger.log(20, f"Running DyStack sub-fit ...")
+    try:
+        predictor._fit(ag_fit_kwargs=ag_fit_kwargs, ag_post_fit_kwargs=ag_post_fit_kwargs)
+    except Exception as e:
+        return False, None, e
 
+    if clean_up_fits:
+        logger.log(20, f"Deleting DyStack predictor artifacts (clean_up_fits={clean_up_fits}) ...")
     if not predictor.model_names():
-        logger.info(f"Unable to determine stacked overfitting. AutoGluon's sub-fit did not successfully train any models!")
+        logger.log(20, f"Unable to determine stacked overfitting. AutoGluon's sub-fit did not successfully train any models!")
         stacked_overfitting = False
+        ho_leaderboard = None
     else:
         leaderboard_kwargs = dict()
         if predictor.model_best in predictor.model_refit_map(inverse=True):
             leaderboard_kwargs = dict(refit_full=True, set_refit_score_to_parent=True)
         # Determine stacked overfitting
         ho_leaderboard = predictor.leaderboard(data=val_data, **leaderboard_kwargs).reset_index(drop=True)
-        logger.info("Leaderboard on holdout data from dynamic stacking:")
-        with pd.option_context("display.max_rows", None, "display.max_columns", None, "display.width", 1000):
-            # Rename to avoid confusion for the user
-            logger.info(ho_leaderboard.rename({"score_test": "score_holdout"}, axis=1))
         stacked_overfitting = check_stacked_overfitting_from_leaderboard(ho_leaderboard)
 
-    logger.info(f"Stacked overfitting occurred: {stacked_overfitting}.")
     del predictor._learner
     predictor._learner = learner_og
 
     if clean_up_fits:
         shutil.rmtree(path=ds_fit_context)
     else:
         predictor._sub_fits.append(ds_fit_context)
 
-    return stacked_overfitting
+    return stacked_overfitting, ho_leaderboard, None
```

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/trainer/auto_trainer.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/trainer/model_presets/presets.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/trainer/model_presets/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/trainer/model_presets/presets_custom.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/trainer/model_presets/presets_custom.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/trainer/model_presets/presets_distill.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/trainer/model_presets/presets_distill.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon/tabular/tuning/feature_pruner.py` & `autogluon.tabular-1.1.1b20240522/src/autogluon/tabular/tuning/feature_pruner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon.tabular.egg-info/PKG-INFO` & `autogluon.tabular-1.1.1b20240522/src/autogluon.tabular.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 1.1.1b20240521
+Version: 1.1.1b20240522
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon.tabular.egg-info/SOURCES.txt` & `autogluon.tabular-1.1.1b20240522/src/autogluon.tabular.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-1.1.1b20240521/src/autogluon.tabular.egg-info/requires.txt` & `autogluon.tabular-1.1.1b20240522/src/autogluon.tabular.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 numpy<1.29,>=1.21
 scipy<1.13,>=1.5.4
 pandas<2.3.0,>=2.0.0
 scikit-learn<1.4.1,>=1.3.0
 networkx<4,>=3.0
-autogluon.core==1.1.1b20240521
-autogluon.features==1.1.1b20240521
+autogluon.core==1.1.1b20240522
+autogluon.features==1.1.1b20240522
 
 [all]
-torch<2.2,>=2.1
-lightgbm<4.4,>=3.3
-fastai<2.8,>=2.3.1
-autogluon.core[all]==1.1.1b20240521
 xgboost<2.1,>=1.6
+torch<2.3,>=2.2
+fastai<2.8,>=2.3.1
+lightgbm<4.4,>=3.3
+autogluon.core[all]==1.1.1b20240522
 
 [all:sys_platform != "darwin"]
 catboost<1.3,>=1.1
 
 [all:sys_platform == "darwin" and python_version < "3.11"]
 catboost<1.2,>=1.1
 
@@ -24,25 +24,25 @@
 [catboost:sys_platform != "darwin"]
 catboost<1.3,>=1.1
 
 [catboost:sys_platform == "darwin" and python_version < "3.11"]
 catboost<1.2,>=1.1
 
 [fastai]
-torch<2.2,>=2.1
+torch<2.3,>=2.2
 fastai<2.8,>=2.3.1
 
 [imodels]
 imodels<1.4.0,>=1.3.10
 
 [lightgbm]
 lightgbm<4.4,>=3.3
 
 [ray]
-autogluon.core[all]==1.1.1b20240521
+autogluon.core[all]==1.1.1b20240522
 
 [skex]
 scikit-learn-intelex<2024.3,>=2023.0
 
 [skl2onnx]
 skl2onnx<1.17.0,>=1.15.0
 onnxruntime-gpu<1.18.0,>=1.15.0
```

