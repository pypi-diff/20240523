# Comparing `tmp/osml-model-runner-2.1.0.tar.gz` & `tmp/osml_model_runner-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osml-model-runner-2.1.0.tar", last modified: Tue Apr  2 22:15:20 2024, max compression
+gzip compressed data, was "osml_model_runner-2.1.1.tar", last modified: Thu May 23 18:48:23 2024, max compression
```

## Comparing `osml-model-runner-2.1.0.tar` & `osml_model_runner-2.1.1.tar`

### file list

```diff
@@ -1,85 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.901538 osml-model-runner-2.1.0/
--rwxr-xr-x   0 runner    (1001) docker     (127)      946 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-04-02 22:15:20.901538 osml-model-runner-2.1.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     6895 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      547 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2318 2024-04-02 22:15:20.905538 osml-model-runner-2.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.889538 osml-model-runner-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.889538 osml-model-runner-2.1.0/src/aws/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.889538 osml-model-runner-2.1.0/src/aws/osml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.889538 osml-model-runner-2.1.0/src/aws/osml/model_runner/
--rwxr-xr-x   0 runner    (1001) docker     (127)      209 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.893538 osml-model-runner-2.1.0/src/aws/osml/model_runner/api/
--rwxr-xr-x   0 runner    (1001) docker     (127)      531 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/api/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      188 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/api/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9708 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/api/image_request.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      405 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/api/inference.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2384 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/api/region_request.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1884 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/api/request_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      525 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/api/sink.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    53228 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/app.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5206 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/app_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.893538 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1462 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      221 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/auto_string_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      906 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/credentials_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3621 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/endpoint_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      196 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/log_context.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      425 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/metrics_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7544 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/mr_post_processing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4421 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/security_classification.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2623 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/timer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1518 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.893538 osml-model-runner-2.1.0/src/aws/osml/model_runner/database/
--rwxr-xr-x   0 runner    (1001) docker     (127)      784 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/database/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10583 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/database/ddb_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4487 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/database/endpoint_statistics_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      711 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/database/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11027 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/database/feature_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9202 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/database/job_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6210 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/database/region_request_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      634 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.897538 osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/
--rwxr-xr-x   0 runner    (1001) docker     (127)      493 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1462 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/endpoint_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/endpoint_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      267 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9513 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/feature_selection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11901 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7608 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/http_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/sm_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.897538 osml-model-runner-2.1.0/src/aws/osml/model_runner/queue/
--rwxr-xr-x   0 runner    (1001) docker     (127)      250 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/queue/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3553 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/queue/request_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.897538 osml-model-runner-2.1.0/src/aws/osml/model_runner/sink/
--rwxr-xr-x   0 runner    (1001) docker     (127)      337 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/sink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/sink/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4404 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/sink/kinesis_sink.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3522 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/sink/s3_sink.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1176 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/sink/sink.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1859 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/sink/sink_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.901538 osml-model-runner-2.1.0/src/aws/osml/model_runner/status/
--rwxr-xr-x   0 runner    (1001) docker     (127)      414 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/status/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      180 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/status/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1810 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/status/image_request_status.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2244 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/status/sns_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3772 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/status/status_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.901538 osml-model-runner-2.1.0/src/aws/osml/model_runner/tile_worker/
--rwxr-xr-x   0 runner    (1001) docker     (127)      327 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/tile_worker/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      189 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/tile_worker/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9898 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/tile_worker/tile_worker.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13353 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/tile_worker/tile_worker_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.901538 osml-model-runner-2.1.0/src/osml_model_runner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-04-02 22:15:20.000000 osml-model-runner-2.1.0/src/osml_model_runner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-02 22:15:20.000000 osml-model-runner-2.1.0/src/osml_model_runner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:15:20.000000 osml-model-runner-2.1.0/src/osml_model_runner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:15:20.000000 osml-model-runner-2.1.0/src/osml_model_runner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-02 22:15:20.000000 osml-model-runner-2.1.0/src/osml_model_runner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 22:15:20.000000 osml-model-runner-2.1.0/src/osml_model_runner.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.901538 osml-model-runner-2.1.0/test/
--rwxr-xr-x   0 runner    (1001) docker     (127)    12851 2024-04-02 22:15:11.000000 osml-model-runner-2.1.0/test/test_api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    30059 2024-04-02 22:15:11.000000 osml-model-runner-2.1.0/test/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:48:23.111686 osml_model_runner-2.1.1/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      946 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-05-23 18:48:23.111686 osml_model_runner-2.1.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6895 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      547 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2318 2024-05-23 18:48:23.111686 osml_model_runner-2.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:48:23.099686 osml_model_runner-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:48:23.095686 osml_model_runner-2.1.1/src/aws/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:48:23.095686 osml_model_runner-2.1.1/src/aws/osml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:48:23.099686 osml_model_runner-2.1.1/src/aws/osml/model_runner/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      209 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:48:23.099686 osml_model_runner-2.1.1/src/aws/osml/model_runner/api/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      531 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/api/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      188 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/api/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9708 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/api/image_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      405 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/api/inference.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2384 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/api/region_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1884 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/api/request_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      525 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/api/sink.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    53228 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5206 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/app_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:48:23.103686 osml_model_runner-2.1.1/src/aws/osml/model_runner/common/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1279 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/common/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      221 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/common/auto_string_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      906 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/common/credentials_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3621 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/common/endpoint_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      138 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/common/feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/common/log_context.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      425 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/common/metrics_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7544 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/common/mr_post_processing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2623 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/common/timer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1518 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/common/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:48:23.103686 osml_model_runner-2.1.1/src/aws/osml/model_runner/database/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      784 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/database/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10583 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/database/ddb_helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4487 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/database/endpoint_statistics_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      711 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/database/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11027 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/database/feature_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9146 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/database/job_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6210 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/database/region_request_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      634 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:48:23.103686 osml_model_runner-2.1.1/src/aws/osml/model_runner/inference/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      493 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/inference/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1462 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/inference/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/inference/endpoint_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/inference/endpoint_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      267 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/inference/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9513 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/inference/feature_selection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11481 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/inference/feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7608 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/inference/http_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/inference/sm_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:48:23.107686 osml_model_runner-2.1.1/src/aws/osml/model_runner/queue/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      250 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/queue/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3553 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/queue/request_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:48:23.107686 osml_model_runner-2.1.1/src/aws/osml/model_runner/sink/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      337 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/sink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/sink/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4404 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/sink/kinesis_sink.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3522 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/sink/s3_sink.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1176 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/sink/sink.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1859 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/sink/sink_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:48:23.107686 osml_model_runner-2.1.1/src/aws/osml/model_runner/status/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      414 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/status/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      180 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/status/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1810 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/status/image_request_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2244 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/status/sns_helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3772 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/status/status_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:48:23.107686 osml_model_runner-2.1.1/src/aws/osml/model_runner/tile_worker/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      327 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/tile_worker/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      189 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/tile_worker/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9898 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/tile_worker/tile_worker.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13353 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/src/aws/osml/model_runner/tile_worker/tile_worker_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:48:23.111686 osml_model_runner-2.1.1/src/osml_model_runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-05-23 18:48:23.000000 osml_model_runner-2.1.1/src/osml_model_runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-23 18:48:23.000000 osml_model_runner-2.1.1/src/osml_model_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:48:23.000000 osml_model_runner-2.1.1/src/osml_model_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:48:22.000000 osml_model_runner-2.1.1/src/osml_model_runner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-23 18:48:23.000000 osml_model_runner-2.1.1/src/osml_model_runner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-23 18:48:23.000000 osml_model_runner-2.1.1/src/osml_model_runner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:48:23.107686 osml_model_runner-2.1.1/test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12851 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/test/test_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30009 2024-05-23 18:48:19.000000 osml_model_runner-2.1.1/test/test_app.py
```

### Comparing `osml-model-runner-2.1.0/LICENSE` & `osml_model_runner-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/PKG-INFO` & `osml_model_runner-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osml-model-runner
-Version: 2.1.0
+Version: 2.1.1
 Summary: Application to run large scale imagery against AI/ML models
 Author: Amazon Web Services
 Author-email: aws-osml-admin@amazon.com
 License: 
         MIT No Attribution
         
         Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
```

### Comparing `osml-model-runner-2.1.0/README.md` & `osml_model_runner-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/pyproject.toml` & `osml_model_runner-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/setup.cfg` & `osml_model_runner-2.1.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = osml-model-runner
-version = 2.1.0
+version = 2.1.1
 description = Application to run large scale imagery against AI/ML models
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Amazon Web Services
 author_email = aws-osml-admin@amazon.com
 license = 
 	MIT No Attribution
```

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/api/__init__.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/api/__init__.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/api/image_request.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/api/image_request.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/api/region_request.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/api/region_request.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/api/request_utils.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/api/request_utils.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/api/sink.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/api/sink.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/app.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/app.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/app_config.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/app_config.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/common/__init__.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/common/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Telling flake8 to not flag errors in this file. It is normal that these classes are imported but not used in an
 # __init__.py file.
 # flake8: noqa
 
 from .auto_string_enum import AutoStringEnum
 from .credentials_utils import get_credentials_for_assumed_role
 from .endpoint_utils import EndpointUtils
-from .exceptions import InvalidAssumedRoleException, InvalidClassificationException
+from .exceptions import InvalidAssumedRoleException
 from .feature_utils import get_feature_image_bounds
 from .log_context import ThreadingLocalContextFilter
 from .metrics_utils import build_embedded_metrics_config
 from .mr_post_processing import (
     FeatureDistillationAlgorithm,
     FeatureDistillationAlgorithmType,
     FeatureDistillationDeserializer,
@@ -21,20 +21,14 @@
     MRPostProcessingAlgorithm,
     MRPostProcessingAlgorithmType,
     MRPostProcessingDeserializer,
     MRPostprocessingStep,
     deserialize_post_processing_list,
     mr_post_processing_options_factory,
 )
-from .security_classification import (
-    Classification,
-    ClassificationLevel,
-    classification_asdict_factory,
-    get_image_classification,
-)
 from .timer import Timer
 from .typing import (
     VALID_IMAGE_COMPRESSION,
     VALID_IMAGE_FORMATS,
     GeojsonDetectionField,
     ImageCompression,
     ImageCoord,
```

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/common/credentials_utils.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/common/credentials_utils.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/common/endpoint_utils.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/common/endpoint_utils.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/common/feature_utils.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/common/feature_utils.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/common/log_context.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/common/log_context.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/common/mr_post_processing.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/common/mr_post_processing.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/common/timer.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/common/timer.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/common/typing.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/common/typing.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/database/__init__.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/database/__init__.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/database/ddb_helper.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/database/ddb_helper.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/database/endpoint_statistics_table.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/database/endpoint_statistics_table.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/database/exceptions.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/database/exceptions.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/database/feature_table.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/database/feature_table.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/database/job_table.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/database/job_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     extents: Optional[str] = None
     tile_size: Optional[str] = None
     tile_overlap: Optional[str] = None
     model_name: Optional[str] = None
     outputs: Optional[str] = None
     processing_time: Optional[Decimal] = None
     feature_properties: Optional[str] = None
-    image_security_classification: Optional[str] = None
     feature_distillation_option: Optional[str] = None
 
     def __post_init__(self):
         self.ddb_key = DDBKey(hash_key="image_id", hash_value=self.image_id)
 
 
 class JobTable(DDBHelper):
```

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/database/region_request_table.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/database/region_request_table.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/exceptions.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/exceptions.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/detector.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/inference/detector.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/endpoint_builder.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/inference/endpoint_builder.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/endpoint_factory.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/inference/endpoint_factory.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/feature_selection.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/inference/feature_selection.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/feature_utils.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/inference/feature_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
 import shapely
 from geojson import Feature, FeatureCollection, LineString, MultiLineString, MultiPoint, MultiPolygon, Point, Polygon, loads
 from osgeo import gdal
 from shapely.geometry.base import BaseGeometry
 
-from aws.osml.model_runner.common import Classification, ImageDimensions, get_image_classification
+from aws.osml.model_runner.common import ImageDimensions
 from aws.osml.photogrammetry import GeodeticWorldCoordinate, SensorModel
 
 
 def features_to_image_shapes(sensor_model: SensorModel, features: List[Feature]) -> List[BaseGeometry]:
     """
     Convert geojson objects/shapes to shapely shapes
 
@@ -228,30 +228,24 @@
             source_id = metadata.get("NITF_FTITLE", None)
             # Format of datetime string follows 14 digit spec in MIL-STD-2500C for NITFs
             source_dt = (
                 datetime.strptime(metadata.get("NITF_IDATIM"), "%Y%m%d%H%M%S").isoformat(timespec="seconds") + "Z"
                 if metadata.get("NITF_IDATIM")
                 else None
             )
-            # Determine the image classification from the metadata
-            source_classification = get_image_classification(dataset)
-            source_classification_str = (
-                source_classification.classification if isinstance(source_classification, Classification) else None
-            )
 
             # Build a source property for features
             source_property = {
                 "sourceMetadata": [
                     {
                         "location": image_location,
                         "format": "NITF",
                         "category": data_type,
                         "sourceId": source_id,
                         "sourceDT": source_dt,
-                        "classification": source_classification_str,
                     }
                 ]
             }
 
             return source_property
         except Exception as err:
             logging.warning(f"Source metadata not available for {image_extension} image extension! {err}")
```

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/http_detector.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/inference/http_detector.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/sm_detector.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/inference/sm_detector.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/queue/request_queue.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/queue/request_queue.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/sink/kinesis_sink.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/sink/kinesis_sink.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/sink/s3_sink.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/sink/s3_sink.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/sink/sink.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/sink/sink.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/sink/sink_factory.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/sink/sink_factory.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/status/image_request_status.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/status/image_request_status.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/status/sns_helper.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/status/sns_helper.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/status/status_monitor.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/status/status_monitor.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/tile_worker/tile_worker.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/tile_worker/tile_worker.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/aws/osml/model_runner/tile_worker/tile_worker_utils.py` & `osml_model_runner-2.1.1/src/aws/osml/model_runner/tile_worker/tile_worker_utils.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/src/osml_model_runner.egg-info/PKG-INFO` & `osml_model_runner-2.1.1/src/osml_model_runner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osml-model-runner
-Version: 2.1.0
+Version: 2.1.1
 Summary: Application to run large scale imagery against AI/ML models
 Author: Amazon Web Services
 Author-email: aws-osml-admin@amazon.com
 License: 
         MIT No Attribution
         
         Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
```

### Comparing `osml-model-runner-2.1.0/src/osml_model_runner.egg-info/SOURCES.txt` & `osml_model_runner-2.1.1/src/osml_model_runner.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 src/aws/osml/model_runner/common/credentials_utils.py
 src/aws/osml/model_runner/common/endpoint_utils.py
 src/aws/osml/model_runner/common/exceptions.py
 src/aws/osml/model_runner/common/feature_utils.py
 src/aws/osml/model_runner/common/log_context.py
 src/aws/osml/model_runner/common/metrics_utils.py
 src/aws/osml/model_runner/common/mr_post_processing.py
-src/aws/osml/model_runner/common/security_classification.py
 src/aws/osml/model_runner/common/timer.py
 src/aws/osml/model_runner/common/typing.py
 src/aws/osml/model_runner/database/__init__.py
 src/aws/osml/model_runner/database/ddb_helper.py
 src/aws/osml/model_runner/database/endpoint_statistics_table.py
 src/aws/osml/model_runner/database/exceptions.py
 src/aws/osml/model_runner/database/feature_table.py
```

### Comparing `osml-model-runner-2.1.0/test/test_api.py` & `osml_model_runner-2.1.1/test/test_api.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.1.0/test/test_app.py` & `osml_model_runner-2.1.1/test/test_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,14 @@
         self.test_feature_source_property = [
             {
                 "location": TEST_IMAGE_FILE,
                 "format": "NITF",
                 "category": "VIS",
                 "sourceId": "Checks an uncompressed 1024x1024 8 bit mono image with GEOcentric data. Airfield",
                 "sourceDT": "1996-12-17T10:26:30Z",
-                "classification": "UNCLASSIFIED",
             }
         ]
 
         self.region_request = RegionRequest(
             {
                 "tile_size": (10, 10),
                 "tile_overlap": (1, 1),
```

