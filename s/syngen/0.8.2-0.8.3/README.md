# Comparing `tmp/syngen-0.8.2.tar.gz` & `tmp/syngen-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngen-0.8.2.tar", last modified: Wed May 22 10:36:02 2024, max compression
+gzip compressed data, was "syngen-0.8.3.tar", last modified: Thu May 23 16:15:45 2024, max compression
```

## Comparing `syngen-0.8.2.tar` & `syngen-0.8.3.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.741406 syngen-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-22 10:34:41.000000 syngen-0.8.2/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 10:34:41.000000 syngen-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 10:34:41.000000 syngen-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    26933 2024-05-22 10:36:02.741406 syngen-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24991 2024-05-22 10:34:41.000000 syngen-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-22 10:34:41.000000 syngen-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-22 10:36:02.745406 syngen-0.8.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.725406 syngen-0.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.729406 syngen-0.8.2/src/syngen/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.733406 syngen-0.8.2/src/syngen/ml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.733406 syngen-0.8.2/src/syngen/ml/config/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/config/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/config/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.733406 syngen-0.8.2/src/syngen/ml/context/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/context/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.733406 syngen-0.8.2/src/syngen/ml/convertor/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/convertor/convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.733406 syngen-0.8.2/src/syngen/ml/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17252 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/data_loaders/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.733406 syngen-0.8.2/src/syngen/ml/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18411 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/handlers/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.733406 syngen-0.8.2/src/syngen/ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.733406 syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   723510 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
--rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.733406 syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.737406 syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   528976 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.737406 syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/src/img/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/src/main.css
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/src/script.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.737406 syngen-0.8.2/src/syngen/ml/metrics/metrics_classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/metrics_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46709 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/metrics_classes/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.737406 syngen-0.8.2/src/syngen/ml/metrics/sample_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/sample_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   708975 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/sample_test/sample_report_template.html
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/sample_test/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.737406 syngen-0.8.2/src/syngen/ml/mlflow_tracker/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/mlflow_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/mlflow_tracker/mlflow_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.737406 syngen-0.8.2/src/syngen/ml/reporters/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9796 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/reporters/reporters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.737406 syngen-0.8.2/src/syngen/ml/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/strategies/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.737406 syngen-0.8.2/src/syngen/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12235 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.737406 syngen-0.8.2/src/syngen/ml/vae/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/vae/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/vae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.737406 syngen-0.8.2/src/syngen/ml/vae/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/vae/models/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/vae/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/vae/models/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    46231 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/vae/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    24260 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/vae/models/features.py
--rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/vae/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.741406 syngen-0.8.2/src/syngen/ml/vae/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/vae/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/vae/wrappers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.741406 syngen-0.8.2/src/syngen/ml/validation_schema/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/validation_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/validation_schema/validation_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.741406 syngen-0.8.2/src/syngen/ml/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15659 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/ml/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.741406 syngen-0.8.2/src/syngen/streamlit_app/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.741406 syngen-0.8.2/src/syngen/streamlit_app/.streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/streamlit_app/.streamlit/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/streamlit_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.741406 syngen-0.8.2/src/syngen/streamlit_app/css/
--rw-r--r--   0 runner    (1001) docker     (127)   707122 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/streamlit_app/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.741406 syngen-0.8.2/src/syngen/streamlit_app/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/streamlit_app/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/streamlit_app/handlers/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.741406 syngen-0.8.2/src/syngen/streamlit_app/img/
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/streamlit_app/img/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/streamlit_app/img/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/streamlit_app/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/streamlit_app/start.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.741406 syngen-0.8.2/src/syngen/streamlit_app/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/streamlit_app/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/streamlit_app/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-22 10:34:41.000000 syngen-0.8.2/src/syngen/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:36:02.741406 syngen-0.8.2/src/syngen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26933 2024-05-22 10:36:02.000000 syngen-0.8.2/src/syngen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-22 10:36:02.000000 syngen-0.8.2/src/syngen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:36:02.000000 syngen-0.8.2/src/syngen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-22 10:36:02.000000 syngen-0.8.2/src/syngen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-22 10:36:02.000000 syngen-0.8.2/src/syngen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 10:36:02.000000 syngen-0.8.2/src/syngen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.198746 syngen-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-23 16:14:28.000000 syngen-0.8.3/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 16:14:28.000000 syngen-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 16:14:28.000000 syngen-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    26894 2024-05-23 16:15:45.198746 syngen-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24991 2024-05-23 16:14:28.000000 syngen-0.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-23 16:14:29.000000 syngen-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-23 16:15:45.198746 syngen-0.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.178746 syngen-0.8.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.186746 syngen-0.8.3/src/syngen/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.186746 syngen-0.8.3/src/syngen/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.186746 syngen-0.8.3/src/syngen/ml/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/config/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/config/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.186746 syngen-0.8.3/src/syngen/ml/context/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/context/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.186746 syngen-0.8.3/src/syngen/ml/convertor/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/convertor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/convertor/convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.186746 syngen-0.8.3/src/syngen/ml/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17252 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/data_loaders/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.186746 syngen-0.8.3/src/syngen/ml/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18411 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/handlers/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.186746 syngen-0.8.3/src/syngen/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.190746 syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   723510 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.190746 syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.190746 syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   528976 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.190746 syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/src/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/src/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/src/script.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.190746 syngen-0.8.3/src/syngen/ml/metrics/metrics_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/metrics_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46709 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/metrics_classes/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.190746 syngen-0.8.3/src/syngen/ml/metrics/sample_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/sample_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   708975 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/sample_test/sample_report_template.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/sample_test/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.190746 syngen-0.8.3/src/syngen/ml/mlflow_tracker/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/mlflow_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/mlflow_tracker/mlflow_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.190746 syngen-0.8.3/src/syngen/ml/reporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9796 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/reporters/reporters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.190746 syngen-0.8.3/src/syngen/ml/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/strategies/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.194746 syngen-0.8.3/src/syngen/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12235 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.194746 syngen-0.8.3/src/syngen/ml/vae/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/vae/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/vae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.194746 syngen-0.8.3/src/syngen/ml/vae/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/vae/models/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/vae/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/vae/models/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46231 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/vae/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24260 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/vae/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/vae/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.194746 syngen-0.8.3/src/syngen/ml/vae/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/vae/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/vae/wrappers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.194746 syngen-0.8.3/src/syngen/ml/validation_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/validation_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/validation_schema/validation_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.194746 syngen-0.8.3/src/syngen/ml/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15659 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.194746 syngen-0.8.3/src/syngen/streamlit_app/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.194746 syngen-0.8.3/src/syngen/streamlit_app/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/streamlit_app/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/streamlit_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.194746 syngen-0.8.3/src/syngen/streamlit_app/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   707122 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/streamlit_app/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.198746 syngen-0.8.3/src/syngen/streamlit_app/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/streamlit_app/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/streamlit_app/handlers/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.198746 syngen-0.8.3/src/syngen/streamlit_app/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/streamlit_app/img/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/streamlit_app/img/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/streamlit_app/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/streamlit_app/start.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.198746 syngen-0.8.3/src/syngen/streamlit_app/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/streamlit_app/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/streamlit_app/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.198746 syngen-0.8.3/src/syngen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26894 2024-05-23 16:15:45.000000 syngen-0.8.3/src/syngen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-23 16:15:45.000000 syngen-0.8.3/src/syngen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 16:15:45.000000 syngen-0.8.3/src/syngen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-23 16:15:45.000000 syngen-0.8.3/src/syngen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-23 16:15:45.000000 syngen-0.8.3/src/syngen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 16:15:45.000000 syngen-0.8.3/src/syngen.egg-info/top_level.txt
```

### Comparing `syngen-0.8.2/LICENSE` & `syngen-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/PKG-INFO` & `syngen-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.8.2
+Version: 0.8.3
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,15 +51,14 @@
 Requires-Dist: tqdm==4.64.*
 Requires-Dist: Werkzeug==3.0.1
 Requires-Dist: xlrd
 Requires-Dist: xlwt
 Provides-Extra: ui
 Requires-Dist: streamlit==1.31.*; extra == "ui"
 Requires-Dist: streamlit_option_menu; extra == "ui"
-Requires-Dist: altair>5; extra == "ui"
 
 [![CI/CD](https://github.com/tdspora/syngen/actions/workflows/action-build-deploy.yml/badge.svg?branch=main)](https://github.com/tdspora/syngen/actions/workflows/action-build-deploy.yml)
 
 # EPAM Syngen
 
 EPAM Syngen is an unsupervised tabular data generation tool. It is useful for generation of test data with a given table as a template. Most datatypes including floats, integers, datetime, text, categorical, binary are supported. The linked tables i.e., tables sharing a key can also be generated using the simple statistical approach.
 The source of data might be in CSV, Avro and Excel format and should be located locally and be in UTF-8 encoding.
```

### Comparing `syngen-0.8.2/README.md` & `syngen-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/setup.cfg` & `syngen-0.8.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,14 @@
 	xlrd
 	xlwt
 
 [options.extras_require]
 ui = 
 	streamlit==1.31.*
 	streamlit_option_menu
-	altair>5
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 * = *.py, *.html, *.ttf, *.svg, *.css, *.js
```

### Comparing `syngen-0.8.2/src/syngen/infer.py` & `syngen-0.8.3/src/syngen/infer.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/config/configurations.py` & `syngen-0.8.3/src/syngen/ml/config/configurations.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/config/validation.py` & `syngen-0.8.3/src/syngen/ml/config/validation.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/context/context.py` & `syngen-0.8.3/src/syngen/ml/context/context.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/convertor/convertor.py` & `syngen-0.8.3/src/syngen/ml/convertor/convertor.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/data_loaders/data_loaders.py` & `syngen-0.8.3/src/syngen/ml/data_loaders/data_loaders.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/handlers/handlers.py` & `syngen-0.8.3/src/syngen/ml/handlers/handlers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/accuracy_report.html` & `syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/accuracy_report.html`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/accuracy_test.py` & `syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/accuracy_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf` & `syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg` & `syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/metrics/accuracy_test/src/main.css` & `syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/src/main.css`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/metrics/metrics_classes/metrics.py` & `syngen-0.8.3/src/syngen/ml/metrics/metrics_classes/metrics.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/metrics/sample_test/sample_report_template.html` & `syngen-0.8.3/src/syngen/ml/metrics/sample_test/sample_report_template.html`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/metrics/sample_test/sample_test.py` & `syngen-0.8.3/src/syngen/ml/metrics/sample_test/sample_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/metrics/utils.py` & `syngen-0.8.3/src/syngen/ml/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/mlflow_tracker/mlflow_tracker.py` & `syngen-0.8.3/src/syngen/ml/mlflow_tracker/mlflow_tracker.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/reporters/reporters.py` & `syngen-0.8.3/src/syngen/ml/reporters/reporters.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/strategies/strategies.py` & `syngen-0.8.3/src/syngen/ml/strategies/strategies.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/utils/__init__.py` & `syngen-0.8.3/src/syngen/ml/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/utils/utils.py` & `syngen-0.8.3/src/syngen/ml/utils/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/vae/models/custom_layers.py` & `syngen-0.8.3/src/syngen/ml/vae/models/custom_layers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/vae/models/dataset.py` & `syngen-0.8.3/src/syngen/ml/vae/models/dataset.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/vae/models/features.py` & `syngen-0.8.3/src/syngen/ml/vae/models/features.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/vae/models/model.py` & `syngen-0.8.3/src/syngen/ml/vae/models/model.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/vae/wrappers/wrappers.py` & `syngen-0.8.3/src/syngen/ml/vae/wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/validation_schema/validation_schema.py` & `syngen-0.8.3/src/syngen/ml/validation_schema/validation_schema.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/ml/worker/worker.py` & `syngen-0.8.3/src/syngen/ml/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/streamlit_app/css/style.css` & `syngen-0.8.3/src/syngen/streamlit_app/css/style.css`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/streamlit_app/handlers/handlers.py` & `syngen-0.8.3/src/syngen/streamlit_app/handlers/handlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,64 +40,89 @@
         self.progress_handler = ProgressBarHandler()
         self.log_queue = Queue()
         self.log_error_queue = Queue()
         self.path_to_generated_data = (f"model_artifacts/tmp_store/{self.sl_table_name}/"
                                        f"merged_infer_{self.sl_table_name}.csv")
         self.path_to_report = (f"model_artifacts/tmp_store/{self.sl_table_name}/"
                                f"draws/accuracy_report.html")
+        self.train_settings = {
+            "source": self.file_path,
+            "epochs": self.epochs,
+            "row_limit": 10000,
+            "drop_null": False,
+            "batch_size": 32,
+            "print_report": False
+        }
+        self.infer_settings = {
+            "size": self.size_limit,
+            "batch_size": 32,
+            "run_parallel": False,
+            "random_seed": None,
+            "print_report": self.print_report,
+            "get_infer_metrics": False
+        }
 
     def set_logger(self):
         """
         Set a logger to see logs, and collect log messages
         with the log level - 'INFO' in a log file and stdout
         """
         logger.remove()
         logger.add(self.console_sink, colorize=True, level="INFO")
         logger.add(self.file_sink, level="INFO")
 
-    def console_sink(self, message):
+    def console_sink(self, message: str):
         """
         Put log messages to a log queue
         """
         log_message = fetch_log_message(message)
         sys.stdout.write(log_message + "\n")
         self.log_queue.put(log_message)
 
-    def file_sink(self, message):
+    def file_sink(self, message: str):
         """
         Write log messages to a log file
         """
         path_to_logs = f"model_artifacts/tmp_store/{self.sl_table_name}_{TIMESTAMP}.log"
         os.environ["SUCCESS_LOG_FILE"] = path_to_logs
         os.makedirs(os.path.dirname(path_to_logs), exist_ok=True)
         with open(path_to_logs, "a") as log_file:
             log_message = fetch_log_message(message)
             log_file.write(log_message + "\n")
 
+    def _get_worker(self, process_type: str):
+        """
+        Get a Worker object
+
+        Parameters
+        ----------
+        process_type : str
+            The type of process ("train" or "infer").
+
+        Returns
+        -------
+        Worker
+            The Worker object.
+        """
+        worker = Worker(
+            table_name=self.table_name,
+            settings=self.train_settings if process_type == "train" else self.infer_settings,
+            metadata_path=None,
+            log_level="INFO",
+            type_of_process=process_type
+        )
+        return worker
+
     def train_model(self):
         """
         Launch a model training
         """
         try:
             logger.info("Starting model training...")
-            settings = {
-                "source": self.file_path,
-                "epochs": self.epochs,
-                "row_limit": 10000,
-                "drop_null": False,
-                "batch_size": 32,
-                "print_report": False
-            }
-            worker = Worker(
-                table_name=self.table_name,
-                settings=settings,
-                metadata_path=None,
-                log_level="INFO",
-                type_of_process="train"
-            )
+            worker = self._get_worker("train")
             ProgressBarHandler().set_progress(0.01)
             worker.launch_train()
             logger.info("Model training completed")
         except Exception as e:
             error_message = (f"The error raised during the training process - "
                              f"{traceback.format_exc()}")
             logger.error(error_message)
@@ -106,49 +131,41 @@
 
     def infer_model(self):
         """
         Launch a data generation
         """
         try:
             logger.info("Starting data generation...")
-            settings = {
-                "size": self.size_limit,
-                "batch_size": 32,
-                "run_parallel": False,
-                "random_seed": None,
-                "print_report": self.print_report,
-                "get_infer_metrics": False
-            }
-            worker = Worker(
-                table_name=self.table_name,
-                settings=settings,
-                metadata_path=None,
-                log_level="INFO",
-                type_of_process="infer"
-            )
+            worker = self._get_worker("infer")
             worker.launch_infer()
             logger.info("Data generation completed")
         except Exception as e:
             error_message = (f"The error raised during the inference process - "
                              f"{traceback.format_exc()}")
             logger.error(error_message)
             self.log_error_queue.put(e)
             raise e
 
-    def train_and_infer(self):
+    def set_monitoring(self):
         """
-        Launch a model training and data generation
+        Reset the progress bar and set up the logger
         """
         self.progress_handler.reset_instance()
         self.set_logger()
+
+    def train_and_infer(self):
+        """
+        Launch a model training and data generation
+        """
+        self.set_monitoring()
         self.train_model()
         self.infer_model()
 
     @staticmethod
-    def generate_button(label, path_to_file, download_name):
+    def generate_button(label: str, path_to_file: str, download_name: str):
         """
         Generate a download button
         """
         if os.path.exists(path_to_file):
             with open(path_to_file, "rb") as f:
                 st.download_button(
                     label,
```

### Comparing `syngen-0.8.2/src/syngen/streamlit_app/img/favicon.svg` & `syngen-0.8.3/src/syngen/streamlit_app/img/favicon.svg`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/streamlit_app/img/logo.svg` & `syngen-0.8.3/src/syngen/streamlit_app/img/logo.svg`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/streamlit_app/run.py` & `syngen-0.8.3/src/syngen/streamlit_app/run.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,155 +1,166 @@
-from threading import Thread
-import time
 import os
+import time
+from threading import Thread
 
 import streamlit as st
 from streamlit_option_menu import option_menu
 
 from syngen.streamlit_app.handlers import StreamlitHandler
 from syngen.streamlit_app.utils import (
     show_data,
     get_running_status,
     set_session_state,
     cleanup_artifacts
 )
 from syngen import __version__
 
 
-def setup_ui():
-    """
-    Set up the UI for the Streamlit app
-    """
-    path_to_logo = f"{os.path.join(os.path.dirname(__file__))}/img/logo.svg"
-    path_to_logo_img = f"{os.path.join(os.path.dirname(__file__))}/img/favicon.svg"
-    st.set_page_config(
-        page_title="SynGen UI",
-        page_icon=path_to_logo_img
-    )
-    st.sidebar.image(path_to_logo, use_column_width=True)
-    st.markdown(
-        f"""
-        <style>
-        {"".join(open(f"{os.path.join(os.path.dirname(__file__))}/css/style.css").readlines())}
-        </style>
-        """, unsafe_allow_html=True
-    )
-
-    st.title(
-        "SynGen UI",
-        help=f"The current version of syngen library is {__version__}"
-    )
-
-
-def handle_cross_icon():
-    """
-    Handle the behavior of disabling of the cross icon
-    """
-    running_status = get_running_status()
-
-    display_status = "none" if running_status else "block"
-
-    css = f"""
-    <style>
-        div[data-testid="fileDeleteBtn"] {{
-        display: {display_status};
-        }}
-    </style>
-    """
-    st.markdown(css, unsafe_allow_html=True)
-
-
-def run_basic_page():
-    """
-    Run the basic page of the Streamlit app
-    """
-    set_session_state()
-    uploaded_file = st.file_uploader(
-        "Upload a CSV file",
-        type="csv",
-        accept_multiple_files=False,
-        disabled=get_running_status(),
-    )
-    handle_cross_icon()
-    if not uploaded_file:
-        cleanup_artifacts()
-        st.warning("Please upload a CSV file to proceed")
-    if uploaded_file:
-        show_data(uploaded_file)
-        epochs = st.number_input(
-            "Epochs",
-            min_value=1,
-            value=1,
-            help="- The larger number of epochs is set the better training result is.\n"
-                 "- The larger number of epochs is set the longer time for training "
-                 "will be required.\n"
-                 "- Actual number of epochs can be smaller that the one that was set here. "
-                 "Once training stops improving the model, further training is not needed.",
-            disabled=get_running_status()
+class StreamlitApp:
+
+    @staticmethod
+    def setup_ui():
+        """
+        Set up the UI for the Streamlit app
+        """
+        path_to_logo = f"{os.path.join(os.path.dirname(__file__))}/img/logo.svg"
+        path_to_logo_img = f"{os.path.join(os.path.dirname(__file__))}/img/favicon.svg"
+        st.set_page_config(
+            page_title="SynGen UI",
+            page_icon=path_to_logo_img
+        )
+        st.sidebar.image(path_to_logo, use_column_width=True)
+        st.markdown(
+            f"""
+                <style>
+                {"".join(open(f"{os.path.join(os.path.dirname(__file__))}/css/style.css").readlines())}
+                </style>
+                """, unsafe_allow_html=True
         )
-        size_limit = st.number_input(
-            "Rows to generate",
-            min_value=1,
-            max_value=None,
-            value=1000,
-            disabled=get_running_status()
+
+        st.title(
+            "SynGen UI",
+            help=f"The current version of syngen library is {__version__}"
         )
-        print_report = st.checkbox(
-            "Create an accuracy report",
-            value=False,
-            key="print_report",
-            disabled=get_running_status()
+
+    @staticmethod
+    def handle_cross_icon():
+        """
+        Handle the behavior of disabling of the cross icon
+        """
+        running_status = get_running_status()
+
+        display_status = "none" if running_status else "block"
+
+        css = f"""
+            <style>
+                div[data-testid="fileDeleteBtn"] {{
+                display: {display_status};
+                }}
+            </style>
+            """
+        st.markdown(css, unsafe_allow_html=True)
+
+    @staticmethod
+    def _get_streamlit_handler(epochs, size_limit, print_report, uploaded_file):
+        """
+        Get the Streamlit handler
+        """
+        return StreamlitHandler(epochs, size_limit, print_report, uploaded_file)
+
+    def run_basic_page(self):
+        """
+        Run the basic page of the Streamlit app
+        """
+        set_session_state()
+        uploaded_file = st.file_uploader(
+            "Upload a CSV file",
+            type="csv",
+            accept_multiple_files=False,
+            disabled=get_running_status(),
         )
-        app = StreamlitHandler(epochs, size_limit, print_report, uploaded_file)
-        if st.button(
-                "Generate data", type="primary", key="gen_button", disabled=get_running_status()
-        ):
-            runner = Thread(name="train_and_infer", target=app.train_and_infer)
-            runner.start()
-            current_progress = 0
-            prg = st.progress(current_progress)
-
-            while runner.is_alive():
-                with st.expander("Logs"):
-                    while True:
-                        if not app.log_queue.empty():
-                            with st.code("logs", language="log"):
-                                log = app.log_queue.get()
-                                st.text(log)
-                                current_progress, message = app.progress_handler.info
-                                prg.progress(value=current_progress, text=message)
-                        elif not app.log_error_queue.empty():
-                            runner.join()
-                            break
-                        elif not runner.is_alive():
-                            break
-                        time.sleep(0.001)
-            if not app.log_error_queue.empty() and not runner.is_alive():
-                st.exception(app.log_error_queue.get())
-            elif app.log_queue.empty() and not runner.is_alive():
-                prg.progress(100)
-                st.success("Data generation completed")
-
-        with st.container():
-            app.generate_buttons()
-
-
-def run():
-    """
-    Run the Streamlit app
-    """
-    setup_ui()
-    with st.sidebar:
-        selected = option_menu("", ["Basic"],
-                               icons=["'play'"],
-                               default_index=0,
-                               menu_icon=None,
-                               styles={
-                                   "container": {"font-family": "Open Sans"}
-                               }
-                               )
-    if selected == "Basic":
-        run_basic_page()
+        self.handle_cross_icon()
+        if not uploaded_file:
+            cleanup_artifacts()
+            st.warning("Please upload a CSV file to proceed")
+        if uploaded_file:
+            show_data(uploaded_file)
+            epochs = st.number_input(
+                "Epochs",
+                min_value=1,
+                value=1,
+                help="- The larger number of epochs is set the better training result is.\n"
+                     "- The larger number of epochs is set the longer time for training "
+                     "will be required.\n"
+                     "- Actual number of epochs can be smaller that the one that was set here. "
+                     "Once training stops improving the model, further training is not needed.",
+                disabled=get_running_status()
+            )
+            size_limit = st.number_input(
+                "Rows to generate",
+                min_value=1,
+                max_value=None,
+                value=1000,
+                disabled=get_running_status()
+            )
+            print_report = st.checkbox(
+                "Create an accuracy report",
+                value=False,
+                key="print_report",
+                disabled=get_running_status()
+            )
+            handler = self._get_streamlit_handler(epochs, size_limit, print_report, uploaded_file)
+            if st.button(
+                    "Generate data",
+                    type="primary",
+                    key="gen_button",
+                    disabled=get_running_status()
+            ):
+                runner = Thread(name="train_and_infer", target=handler.train_and_infer)
+                runner.start()
+                current_progress = 0
+                prg = st.progress(current_progress)
+
+                while runner.is_alive():
+                    with st.expander("Logs"):
+                        while True:
+                            if not handler.log_queue.empty():
+                                with st.code("logs", language="log"):
+                                    log = handler.log_queue.get()
+                                    st.text(log)
+                                    current_progress, message = handler.progress_handler.info
+                                    prg.progress(value=current_progress, text=message)
+                            elif not handler.log_error_queue.empty():
+                                runner.join()
+                                break
+                            elif not runner.is_alive():
+                                break
+                            time.sleep(0.001)
+                if not handler.log_error_queue.empty() and not runner.is_alive():
+                    st.exception(handler.log_error_queue.get())
+                elif handler.log_queue.empty() and not runner.is_alive():
+                    prg.progress(100)
+                    st.success("Data generation completed")
+
+            with st.container():
+                handler.generate_buttons()
+
+    def run(self):
+        """
+        Run the Streamlit app
+        """
+        self.setup_ui()
+        with st.sidebar:
+            selected = option_menu("", ["Basic"],
+                                   icons=["'play'"],
+                                   default_index=0,
+                                   menu_icon=None,
+                                   styles={
+                                       "container": {"font-family": "Open Sans"}
+                                   }
+                                   )
+        if selected == "Basic":
+            self.run_basic_page()
 
 
 if __name__ == "__main__":
-    run()
+    StreamlitApp().run()
```

### Comparing `syngen-0.8.2/src/syngen/streamlit_app/start.py` & `syngen-0.8.3/src/syngen/streamlit_app/start.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/streamlit_app/utils/utils.py` & `syngen-0.8.3/src/syngen/streamlit_app/utils/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen/train.py` & `syngen-0.8.3/src/syngen/train.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen.egg-info/PKG-INFO` & `syngen-0.8.3/src/syngen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.8.2
+Version: 0.8.3
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,15 +51,14 @@
 Requires-Dist: tqdm==4.64.*
 Requires-Dist: Werkzeug==3.0.1
 Requires-Dist: xlrd
 Requires-Dist: xlwt
 Provides-Extra: ui
 Requires-Dist: streamlit==1.31.*; extra == "ui"
 Requires-Dist: streamlit_option_menu; extra == "ui"
-Requires-Dist: altair>5; extra == "ui"
 
 [![CI/CD](https://github.com/tdspora/syngen/actions/workflows/action-build-deploy.yml/badge.svg?branch=main)](https://github.com/tdspora/syngen/actions/workflows/action-build-deploy.yml)
 
 # EPAM Syngen
 
 EPAM Syngen is an unsupervised tabular data generation tool. It is useful for generation of test data with a given table as a template. Most datatypes including floats, integers, datetime, text, categorical, binary are supported. The linked tables i.e., tables sharing a key can also be generated using the simple statistical approach.
 The source of data might be in CSV, Avro and Excel format and should be located locally and be in UTF-8 encoding.
```

### Comparing `syngen-0.8.2/src/syngen.egg-info/SOURCES.txt` & `syngen-0.8.3/src/syngen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syngen-0.8.2/src/syngen.egg-info/requires.txt` & `syngen-0.8.3/src/syngen.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -34,8 +34,7 @@
 Werkzeug==3.0.1
 xlrd
 xlwt
 
 [ui]
 streamlit==1.31.*
 streamlit_option_menu
-altair>5
```

