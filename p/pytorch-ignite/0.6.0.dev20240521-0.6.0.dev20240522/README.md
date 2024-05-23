# Comparing `tmp/pytorch_ignite-0.6.0.dev20240521.tar.gz` & `tmp/pytorch_ignite-0.6.0.dev20240522.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_ignite-0.6.0.dev20240521.tar", last modified: Tue May 21 00:13:37 2024, max compression
+gzip compressed data, was "pytorch_ignite-0.6.0.dev20240522.tar", last modified: Wed May 22 00:13:49 2024, max compression
```

## Comparing `pytorch_ignite-0.6.0.dev20240521.tar` & `pytorch_ignite-0.6.0.dev20240522.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:13:37.969632 pytorch_ignite-0.6.0.dev20240521/
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    27828 2024-05-21 00:13:37.969632 pytorch_ignite-0.6.0.dev20240521/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27322 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:13:37.945632 pytorch_ignite-0.6.0.dev20240521/ignite/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-21 00:11:19.000000 pytorch_ignite-0.6.0.dev20240521/ignite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:13:37.945632 pytorch_ignite-0.6.0.dev20240521/ignite/base/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/base/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:13:37.945632 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:13:37.949632 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/engines/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28430 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/engines/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/engines/tbptt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:13:37.949632 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/clearml_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/neptune_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/param_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/polyaxon_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/time_profilers.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/tqdm_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/visdom_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:13:37.949632 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/cohen_kappa.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/gpu_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/precision_recall_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:13:37.953632 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/canberra_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/fractional_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/fractional_bias.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/manhattan_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/maximum_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/mean_absolute_relative_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/mean_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/mean_normalized_bias.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/median_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/median_absolute_percentage_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/median_relative_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/r2_score.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/wave_hedges_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/roc_auc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:13:37.953632 pytorch_ignite-0.6.0.dev20240521/ignite/distributed/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15401 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/distributed/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:13:37.953632 pytorch_ignite-0.6.0.dev20240521/ignite/distributed/comp_models/
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/distributed/comp_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14021 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/distributed/comp_models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/distributed/comp_models/horovod.py
--rw-r--r--   0 runner    (1001) docker     (127)    27705 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/distributed/comp_models/native.py
--rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/distributed/comp_models/xla.py
--rw-r--r--   0 runner    (1001) docker     (127)    13492 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/distributed/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    22608 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/distributed/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:13:37.957632 pytorch_ignite-0.6.0.dev20240521/ignite/engine/
--rw-r--r--   0 runner    (1001) docker     (127)    36118 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11632 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/engine/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (127)    56579 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    21213 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/engine/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/engine/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:13:37.961632 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11793 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    44882 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    37473 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/clearml_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/ema_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/fbresearch_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    22143 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    27366 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/neptune_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    68285 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/param_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/polyaxon_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    20745 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/state_param_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/stores.py
--rw-r--r--   0 runner    (1001) docker     (127)    26381 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/terminate_on_nan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)    30228 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/time_profilers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)    13040 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/tqdm_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21551 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/visdom_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    14346 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/handlers/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:13:37.965632 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10988 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/accumulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/classification_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/cohen_kappa.py
--rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/epoch_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/fbeta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/frequency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:13:37.965632 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/gan/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/gan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/gan/fid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/gan/inception_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/gan/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/gpu_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/js_divergence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/kl_divergence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/maximum_mean_discrepancy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/mean_pairwise_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    32127 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/metrics_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/multilabel_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/mutual_information.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:13:37.965632 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/nlp/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/nlp/bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)    15364 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/nlp/rouge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/nlp/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18160 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/psnr.py
--rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/recall.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:13:37.969632 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/canberra_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/fractional_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/fractional_bias.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/geometric_mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/geometric_mean_relative_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/manhattan_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/maximum_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/mean_absolute_relative_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/mean_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/mean_normalized_bias.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/median_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/median_absolute_percentage_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/median_relative_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/pearson_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/r2_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/wave_hedges_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/root_mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/running_average.py
--rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/ssim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/metrics/top_k_categorical_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/ignite/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:13:37.969632 pytorch_ignite-0.6.0.dev20240521/pytorch_ignite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27828 2024-05-21 00:13:37.000000 pytorch_ignite-0.6.0.dev20240521/pytorch_ignite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-21 00:13:37.000000 pytorch_ignite-0.6.0.dev20240521/pytorch_ignite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 00:13:37.000000 pytorch_ignite-0.6.0.dev20240521/pytorch_ignite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 00:13:37.000000 pytorch_ignite-0.6.0.dev20240521/pytorch_ignite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 00:13:37.000000 pytorch_ignite-0.6.0.dev20240521/pytorch_ignite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-21 00:13:37.000000 pytorch_ignite-0.6.0.dev20240521/pytorch_ignite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-21 00:13:37.969632 pytorch_ignite-0.6.0.dev20240521/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-21 00:11:01.000000 pytorch_ignite-0.6.0.dev20240521/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:13:49.058862 pytorch_ignite-0.6.0.dev20240522/
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    27828 2024-05-22 00:13:49.058862 pytorch_ignite-0.6.0.dev20240522/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27322 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:13:49.034862 pytorch_ignite-0.6.0.dev20240522/ignite/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-22 00:11:09.000000 pytorch_ignite-0.6.0.dev20240522/ignite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:13:49.034862 pytorch_ignite-0.6.0.dev20240522/ignite/base/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/base/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:13:49.034862 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:13:49.034862 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28430 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/engines/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/engines/tbptt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:13:49.038862 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/clearml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/neptune_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/polyaxon_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/time_profilers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/tqdm_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/visdom_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:13:49.038862 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/cohen_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/gpu_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/precision_recall_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:13:49.042862 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/canberra_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/fractional_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/fractional_bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/manhattan_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/maximum_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/mean_absolute_relative_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/mean_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/mean_normalized_bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/median_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/median_absolute_percentage_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/median_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/r2_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/wave_hedges_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/roc_auc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:13:49.042862 pytorch_ignite-0.6.0.dev20240522/ignite/distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15401 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/distributed/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:13:49.042862 pytorch_ignite-0.6.0.dev20240522/ignite/distributed/comp_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/distributed/comp_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14021 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/distributed/comp_models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/distributed/comp_models/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27705 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/distributed/comp_models/native.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/distributed/comp_models/xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13492 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/distributed/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22608 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/distributed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:13:49.042862 pytorch_ignite-0.6.0.dev20240522/ignite/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)    36118 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11632 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/engine/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56579 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21213 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/engine/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/engine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:13:49.046862 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11793 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44882 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37473 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/clearml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/ema_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/fbresearch_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27366 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/neptune_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68261 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/polyaxon_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20745 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/state_param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/stores.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26381 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/terminate_on_nan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30228 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/time_profilers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13040 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/tqdm_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21551 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/visdom_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14346 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/handlers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:13:49.054862 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10988 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/accumulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/classification_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/cohen_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/epoch_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/fbeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/frequency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:13:49.054862 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/gan/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/gan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/gan/fid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/gan/inception_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/gan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/gpu_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/js_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/kl_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/maximum_mean_discrepancy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/mean_pairwise_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32127 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/metrics_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/multilabel_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/mutual_information.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:13:49.054862 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/nlp/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/nlp/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15364 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/nlp/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/nlp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18160 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/recall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:13:49.058862 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/canberra_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/fractional_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/fractional_bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/geometric_mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/geometric_mean_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/manhattan_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/maximum_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/mean_absolute_relative_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/mean_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/mean_normalized_bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/median_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/median_absolute_percentage_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/median_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/pearson_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/r2_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/wave_hedges_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/root_mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/running_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/metrics/top_k_categorical_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/ignite/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:13:49.058862 pytorch_ignite-0.6.0.dev20240522/pytorch_ignite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27828 2024-05-22 00:13:48.000000 pytorch_ignite-0.6.0.dev20240522/pytorch_ignite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-22 00:13:49.000000 pytorch_ignite-0.6.0.dev20240522/pytorch_ignite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 00:13:48.000000 pytorch_ignite-0.6.0.dev20240522/pytorch_ignite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 00:13:48.000000 pytorch_ignite-0.6.0.dev20240522/pytorch_ignite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 00:13:48.000000 pytorch_ignite-0.6.0.dev20240522/pytorch_ignite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 00:13:48.000000 pytorch_ignite-0.6.0.dev20240522/pytorch_ignite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-22 00:13:49.062862 pytorch_ignite-0.6.0.dev20240522/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-22 00:10:44.000000 pytorch_ignite-0.6.0.dev20240522/setup.py
```

### Comparing `pytorch_ignite-0.6.0.dev20240521/LICENSE` & `pytorch_ignite-0.6.0.dev20240522/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/PKG-INFO` & `pytorch_ignite-0.6.0.dev20240522/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-ignite
-Version: 0.6.0.dev20240521
+Version: 0.6.0.dev20240522
 Summary: A lightweight library to help with training neural networks in PyTorch.
 Home-page: https://github.com/pytorch/ignite
 Author: PyTorch-Ignite Team
 Author-email: contact@pytorch-ignite.ai
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pytorch_ignite-0.6.0.dev20240521/README.md` & `pytorch_ignite-0.6.0.dev20240522/README.md`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/base/mixins.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/base/mixins.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/engines/common.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/engines/common.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/engines/tbptt.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/engines/tbptt.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/__init__.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/base_logger.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/base_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/clearml_logger.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/clearml_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/lr_finder.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/mlflow_logger.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/neptune_logger.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/neptune_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/param_scheduler.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/param_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/polyaxon_logger.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/polyaxon_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/tensorboard_logger.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/time_profilers.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/time_profilers.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/tqdm_logger.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/tqdm_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/visdom_logger.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/visdom_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/handlers/wandb_logger.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/handlers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/average_precision.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/average_precision.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/cohen_kappa.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/cohen_kappa.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/gpu_info.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/gpu_info.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/precision_recall_curve.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/__init__.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/_base.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/_base.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/canberra_metric.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/canberra_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/fractional_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/fractional_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/fractional_bias.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/fractional_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/manhattan_distance.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/manhattan_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/maximum_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/maximum_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/mean_absolute_relative_error.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/mean_absolute_relative_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/mean_error.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/mean_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/mean_normalized_bias.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/mean_normalized_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/median_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/median_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/median_absolute_percentage_error.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/median_absolute_percentage_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/median_relative_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/median_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/r2_score.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/r2_score.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/regression/wave_hedges_distance.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/regression/wave_hedges_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/contrib/metrics/roc_auc.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/contrib/metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/distributed/auto.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/distributed/auto.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/distributed/comp_models/__init__.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/distributed/comp_models/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/distributed/comp_models/base.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/distributed/comp_models/base.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/distributed/comp_models/horovod.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/distributed/comp_models/horovod.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/distributed/comp_models/native.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/distributed/comp_models/native.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/distributed/comp_models/xla.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/distributed/comp_models/xla.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/distributed/launcher.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/distributed/launcher.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/distributed/utils.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/distributed/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/engine/__init__.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/engine/deterministic.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/engine/deterministic.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/engine/engine.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/engine/engine.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/engine/events.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/engine/events.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/engine/utils.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/engine/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/__init__.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/base_logger.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/base_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/checkpoint.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/checkpoint.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/clearml_logger.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/clearml_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/early_stopping.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/ema_handler.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/ema_handler.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/fbresearch_logger.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/fbresearch_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/lr_finder.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/lr_finder.py`

 * *Files 0% similar despite different names*

```diff
@@ -538,11 +538,11 @@
         self.end_lrs = end_lrs
         self.num_iter = num_iter
         super(_ExponentialLR, self).__init__(optimizer, last_epoch)
 
         # override base_lrs
         self.base_lrs = start_lrs
 
-    def get_lr(self) -> List[float]:  # type: ignore[override]
+    def get_lr(self) -> List[float]:
         curr_iter = self.last_epoch + 1
         r = curr_iter / self.num_iter
         return [base_lr * (end_lr / base_lr) ** r for end_lr, base_lr in zip(self.end_lrs, self.base_lrs)]
```

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/mlflow_logger.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/neptune_logger.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/neptune_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/param_scheduler.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/param_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numbers
 import tempfile
 import warnings
 from abc import ABCMeta, abstractmethod
 from collections import OrderedDict
 from copy import copy
 from pathlib import Path
-from typing import Any, cast, Dict, List, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import Any, Dict, List, Mapping, Optional, Sequence, Tuple, Type, Union
 
 import torch
 from torch.optim.lr_scheduler import CosineAnnealingWarmRestarts, ReduceLROnPlateau
 from torch.optim.optimizer import Optimizer
 
 # https://github.com/pytorch/ignite/issues/2773
 try:
@@ -988,15 +988,15 @@
         super(LRScheduler, self).__call__(engine, name)
         self.lr_scheduler.last_epoch += 1
 
     def get_param(self) -> Union[float, List[float]]:
         """Method to get current optimizer's parameter value"""
         # Emulate context manager for pytorch>=1.4
         self.lr_scheduler._get_lr_called_within_step = True  # type: ignore[union-attr]
-        lr_list = cast(List[float], self.lr_scheduler.get_lr())
+        lr_list = self.lr_scheduler.get_lr()
         self.lr_scheduler._get_lr_called_within_step = False  # type: ignore[union-attr]
         if len(lr_list) == 1:
             return lr_list[0]
         else:
             return lr_list
 
     @classmethod
@@ -1666,15 +1666,15 @@
             warnings.warn(
                 "Found verbose=True in provided scheduler_kwargs. "
                 "It would be set to False. Please use save_history instead."
             )
             _scheduler_kwargs["verbose"] = False
 
         self.scheduler = ReduceLROnPlateau(optimizer, **_scheduler_kwargs)
-        self.scheduler._reduce_lr = self._reduce_lr  # type: ignore[attr-defined]
+        self.scheduler._reduce_lr = self._reduce_lr  # type: ignore[method-assign]
 
         self._state_attrs += ["metric_name", "scheduler"]
 
     def __call__(self, engine: Engine, name: Optional[str] = None) -> None:  # type: ignore[override]
         if not hasattr(engine.state, "metrics") or self.metric_name not in engine.state.metrics:
             raise ValueError(
                 "Argument engine should have in its 'state', attribute 'metrics' "
```

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/polyaxon_logger.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/polyaxon_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/state_param_scheduler.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/state_param_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/stores.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/stores.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/tensorboard_logger.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/terminate_on_nan.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/time_limit.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/time_limit.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/time_profilers.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/time_profilers.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/timing.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/timing.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/tqdm_logger.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/tqdm_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/utils.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/visdom_logger.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/visdom_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/handlers/wandb_logger.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/handlers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/__init__.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/accumulation.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/accumulation.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/accuracy.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/average_precision.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/average_precision.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/classification_report.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/classification_report.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/cohen_kappa.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/cohen_kappa.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/confusion_matrix.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/cosine_similarity.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/entropy.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/entropy.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/epoch_metric.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/epoch_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/fbeta.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/fbeta.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/frequency.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/frequency.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/gan/fid.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/gan/fid.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/gan/inception_score.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/gan/inception_score.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/gan/utils.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/gan/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/gpu_info.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/gpu_info.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/js_divergence.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/js_divergence.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/kl_divergence.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/kl_divergence.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/loss.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/loss.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/maximum_mean_discrepancy.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/maximum_mean_discrepancy.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/mean_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/mean_pairwise_distance.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/mean_pairwise_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/mean_squared_error.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/metric.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/metrics_lambda.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/metrics_lambda.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/multilabel_confusion_matrix.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/multilabel_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/mutual_information.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/mutual_information.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/nlp/bleu.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/nlp/bleu.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/nlp/rouge.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/nlp/rouge.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/nlp/utils.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/precision.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/precision_recall_curve.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/psnr.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/psnr.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/recall.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/__init__.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/_base.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/_base.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/canberra_metric.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/canberra_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/fractional_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/fractional_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/fractional_bias.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/fractional_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/geometric_mean_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/geometric_mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/geometric_mean_relative_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/geometric_mean_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/manhattan_distance.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/manhattan_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/maximum_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/maximum_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/mean_absolute_relative_error.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/mean_absolute_relative_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/mean_error.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/mean_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/mean_normalized_bias.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/mean_normalized_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/median_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/median_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/median_absolute_percentage_error.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/median_absolute_percentage_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/median_relative_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/median_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/pearson_correlation.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/pearson_correlation.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/r2_score.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/r2_score.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/regression/wave_hedges_distance.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/regression/wave_hedges_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/roc_auc.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/root_mean_squared_error.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/root_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/running_average.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/running_average.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/ssim.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/ssim.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/metrics/top_k_categorical_accuracy.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/metrics/top_k_categorical_accuracy.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/ignite/utils.py` & `pytorch_ignite-0.6.0.dev20240522/ignite/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/pyproject.toml` & `pytorch_ignite-0.6.0.dev20240522/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/pytorch_ignite.egg-info/PKG-INFO` & `pytorch_ignite-0.6.0.dev20240522/pytorch_ignite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-ignite
-Version: 0.6.0.dev20240521
+Version: 0.6.0.dev20240522
 Summary: A lightweight library to help with training neural networks in PyTorch.
 Home-page: https://github.com/pytorch/ignite
 Author: PyTorch-Ignite Team
 Author-email: contact@pytorch-ignite.ai
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pytorch_ignite-0.6.0.dev20240521/pytorch_ignite.egg-info/SOURCES.txt` & `pytorch_ignite-0.6.0.dev20240522/pytorch_ignite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/setup.cfg` & `pytorch_ignite-0.6.0.dev20240522/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240521/setup.py` & `pytorch_ignite-0.6.0.dev20240522/setup.py`

 * *Files identical despite different names*

