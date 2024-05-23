# Comparing `tmp/kafka_overwatch-0.4.0.tar.gz` & `tmp/kafka_overwatch-0.5.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka_overwatch-0.4.0.tar", max compression
+gzip compressed data, was "kafka_overwatch-0.5.0.post0.tar", max compression
```

## Comparing `kafka_overwatch-0.4.0.tar` & `kafka_overwatch-0.5.0.post0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0      281 2024-02-14 21:24:07.216496 kafka_overwatch-0.4.0/AUTHORS.rst
--rw-r--r--   0        0        0    16725 2023-12-13 12:48:29.115693 kafka_overwatch-0.4.0/LICENSE
--rw-r--r--   0        0        0     3130 2024-02-14 21:24:07.217496 kafka_overwatch-0.4.0/README.rst
--rw-r--r--   0        0        0      176 2024-04-25 16:37:05.337066 kafka_overwatch-0.4.0/kafka_overwatch/__init__.py
--rw-r--r--   0        0        0     1300 2024-02-15 16:51:43.978241 kafka_overwatch-0.4.0/kafka_overwatch/aws_helpers/__init__.py
--rw-r--r--   0        0        0     2372 2024-03-12 06:50:39.512258 kafka_overwatch-0.4.0/kafka_overwatch/aws_helpers/kafka_client_secrets.py
--rw-r--r--   0        0        0     2862 2024-04-07 20:43:52.705782 kafka_overwatch-0.4.0/kafka_overwatch/aws_helpers/s3.py
--rw-r--r--   0        0        0     2626 2024-02-07 21:36:59.982077 kafka_overwatch-0.4.0/kafka_overwatch/cli/__init__.py
--rw-r--r--   0        0        0     1342 2024-04-17 05:19:40.739040 kafka_overwatch-0.4.0/kafka_overwatch/cli/schema_registry_restore.py
--rw-r--r--   0        0        0     1175 2024-04-07 20:43:52.705782 kafka_overwatch-0.4.0/kafka_overwatch/common/__init__.py
--rw-r--r--   0        0        0      970 2024-01-04 01:27:32.802689 kafka_overwatch-0.4.0/kafka_overwatch/config/__init__.py
--rw-r--r--   0        0        0     3228 2024-04-07 20:43:52.705782 kafka_overwatch-0.4.0/kafka_overwatch/config/config.py
--rw-r--r--   0        0        0     3229 2024-01-01 08:48:18.162847 kafka_overwatch-0.4.0/kafka_overwatch/config/logging.py
--rw-r--r--   0        0        0      250 2024-04-06 19:12:23.350109 kafka_overwatch-0.4.0/kafka_overwatch/config/threads_settings.py
--rw-r--r--   0        0        0     1542 2024-04-07 20:43:52.706782 kafka_overwatch-0.4.0/kafka_overwatch/kafka_resources/__init__.py
--rw-r--r--   0        0        0     7948 2024-04-07 20:43:52.706782 kafka_overwatch-0.4.0/kafka_overwatch/kafka_resources/groups.py
--rw-r--r--   0        0        0     8939 2024-04-07 20:43:52.706782 kafka_overwatch-0.4.0/kafka_overwatch/kafka_resources/topics.py
--rw-r--r--   0        0        0       88 2024-01-02 07:32:22.087588 kafka_overwatch-0.4.0/kafka_overwatch/monitoring/__init__.py
--rw-r--r--   0        0        0     2513 2024-04-07 20:43:52.706782 kafka_overwatch-0.4.0/kafka_overwatch/monitoring/prometheus.py
--rw-r--r--   0        0        0      176 2024-03-11 21:31:12.971386 kafka_overwatch-0.4.0/kafka_overwatch/notifications/__init__.py
--rw-r--r--   0        0        0     5230 2024-04-07 20:43:52.706782 kafka_overwatch-0.4.0/kafka_overwatch/notifications/aws_sns/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 21:31:12.972386 kafka_overwatch-0.4.0/kafka_overwatch/notifications/aws_sns/usage_report/__init__.py
--rw-r--r--   0        0        0       83 2024-03-11 21:31:12.972386 kafka_overwatch-0.4.0/kafka_overwatch/notifications/aws_sns/usage_report/default.j2
--rw-r--r--   0        0        0      484 2024-03-11 21:31:12.972386 kafka_overwatch-0.4.0/kafka_overwatch/notifications/aws_sns/usage_report/email.j2
--rw-r--r--   0        0        0     3496 2024-04-07 20:43:52.706782 kafka_overwatch-0.4.0/kafka_overwatch/overwatch.py
--rw-r--r--   0        0        0       86 2024-01-02 07:32:22.104588 kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/__init__.py
--rw-r--r--   0        0        0    14000 2024-04-07 20:43:52.706782 kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/clusters.py
--rw-r--r--   0        0        0     5026 2024-03-11 06:55:53.345126 kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/groups.py
--rw-r--r--   0        0        0     5171 2024-04-17 05:16:00.917189 kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/schema_registry/__init__.py
--rw-r--r--   0        0        0     2412 2024-04-07 20:43:52.707782 kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/schema_registry/schema.py
--rw-r--r--   0        0        0     3135 2024-04-18 23:09:58.482167 kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/schema_registry/schemas_restore.py
--rw-r--r--   0        0        0      801 2024-04-07 20:43:52.707782 kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/schema_registry/subject.py
--rw-r--r--   0        0        0     7286 2024-04-07 20:43:52.707782 kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/topics.py
--rw-r--r--   0        0        0     1089 2024-04-07 20:43:52.707782 kafka_overwatch-0.4.0/kafka_overwatch/processing/__init__.py
--rw-r--r--   0        0        0     5893 2024-04-07 20:43:52.707782 kafka_overwatch-0.4.0/kafka_overwatch/processing/clusters.py
--rw-r--r--   0        0        0     9011 2024-04-07 20:43:52.707782 kafka_overwatch-0.4.0/kafka_overwatch/processing/schema_registries.py
--rw-r--r--   0        0        0     4793 2024-04-07 20:43:52.707782 kafka_overwatch-0.4.0/kafka_overwatch/reporting/__init__.py
--rw-r--r--   0        0        0       88 2024-02-14 21:24:07.217496 kafka_overwatch-0.4.0/kafka_overwatch/reporting/governance/__init__.py
--rw-r--r--   0        0        0     1364 2024-03-11 06:55:53.346126 kafka_overwatch-0.4.0/kafka_overwatch/reporting/governance/consumer_groups_naming_convention.py
--rw-r--r--   0        0        0     1355 2024-02-14 21:24:07.217496 kafka_overwatch-0.4.0/kafka_overwatch/reporting/governance/topic_naming_convention.py
--rw-r--r--   0        0        0     1128 2024-04-07 20:43:52.707782 kafka_overwatch-0.4.0/kafka_overwatch/reporting/schema_registry.py
--rw-r--r--   0        0        0     1963 2024-03-11 06:55:53.346126 kafka_overwatch-0.4.0/kafka_overwatch/reporting/tools.py
--rw-r--r--   0        0        0     3967 2024-04-07 20:43:52.707782 kafka_overwatch-0.4.0/kafka_overwatch/reporting/topics.py
--rw-r--r--   0        0        0       86 2024-01-02 07:32:22.103588 kafka_overwatch-0.4.0/kafka_overwatch/specs/__init__.py
--rw-r--r--   0        0        0    21799 2024-04-25 16:37:05.671059 kafka_overwatch-0.4.0/kafka_overwatch/specs/config.json
--rw-r--r--   0        0        0    11668 2024-04-07 20:43:52.708782 kafka_overwatch-0.4.0/kafka_overwatch/specs/config.py
--rw-r--r--   0        0        0     6716 2024-04-25 16:37:05.671059 kafka_overwatch-0.4.0/kafka_overwatch/specs/report.json
--rw-r--r--   0        0        0     3249 2024-04-07 20:43:52.708782 kafka_overwatch-0.4.0/kafka_overwatch/specs/report.py
--rw-r--r--   0        0        0     2889 2024-04-25 16:37:05.337066 kafka_overwatch-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4989 1970-01-01 00:00:00.000000 kafka_overwatch-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      281 2024-02-14 21:24:07.216496 kafka_overwatch-0.5.0.post0/AUTHORS.rst
+-rw-r--r--   0        0        0    16725 2023-12-13 12:48:29.115693 kafka_overwatch-0.5.0.post0/LICENSE
+-rw-r--r--   0        0        0     3384 2024-05-23 19:34:20.918118 kafka_overwatch-0.5.0.post0/README.rst
+-rw-r--r--   0        0        0      182 2024-05-23 19:41:34.007551 kafka_overwatch-0.5.0.post0/kafka_overwatch/__init__.py
+-rw-r--r--   0        0        0     1300 2024-02-15 16:51:43.978241 kafka_overwatch-0.5.0.post0/kafka_overwatch/aws_helpers/__init__.py
+-rw-r--r--   0        0        0     2372 2024-03-12 06:50:39.512258 kafka_overwatch-0.5.0.post0/kafka_overwatch/aws_helpers/kafka_client_secrets.py
+-rw-r--r--   0        0        0     2862 2024-05-20 18:13:04.774594 kafka_overwatch-0.5.0.post0/kafka_overwatch/aws_helpers/s3.py
+-rw-r--r--   0        0        0     2950 2024-05-23 19:30:47.507672 kafka_overwatch-0.5.0.post0/kafka_overwatch/cli/__init__.py
+-rw-r--r--   0        0        0     1342 2024-04-17 05:19:40.739040 kafka_overwatch-0.5.0.post0/kafka_overwatch/cli/schema_registry_restore.py
+-rw-r--r--   0        0        0     1289 2024-05-23 19:30:47.507672 kafka_overwatch-0.5.0.post0/kafka_overwatch/common/__init__.py
+-rw-r--r--   0        0        0      970 2024-01-04 01:27:32.802689 kafka_overwatch-0.5.0.post0/kafka_overwatch/config/__init__.py
+-rw-r--r--   0        0        0     3520 2024-05-23 19:30:47.508672 kafka_overwatch-0.5.0.post0/kafka_overwatch/config/config.py
+-rw-r--r--   0        0        0     3229 2024-01-01 08:48:18.162847 kafka_overwatch-0.5.0.post0/kafka_overwatch/config/logging.py
+-rw-r--r--   0        0        0      250 2024-04-06 19:12:23.350109 kafka_overwatch-0.5.0.post0/kafka_overwatch/config/threads_settings.py
+-rw-r--r--   0        0        0     1542 2024-04-07 20:43:52.706782 kafka_overwatch-0.5.0.post0/kafka_overwatch/kafka_resources/__init__.py
+-rw-r--r--   0        0        0     7987 2024-05-23 19:30:47.508672 kafka_overwatch-0.5.0.post0/kafka_overwatch/kafka_resources/groups.py
+-rw-r--r--   0        0        0     7691 2024-05-23 19:30:47.508672 kafka_overwatch-0.5.0.post0/kafka_overwatch/kafka_resources/topics.py
+-rw-r--r--   0        0        0       88 2024-01-02 07:32:22.087588 kafka_overwatch-0.5.0.post0/kafka_overwatch/monitoring/__init__.py
+-rw-r--r--   0        0        0     2513 2024-04-07 20:43:52.706782 kafka_overwatch-0.5.0.post0/kafka_overwatch/monitoring/prometheus.py
+-rw-r--r--   0        0        0      176 2024-03-11 21:31:12.971386 kafka_overwatch-0.5.0.post0/kafka_overwatch/notifications/__init__.py
+-rw-r--r--   0        0        0     5230 2024-04-07 20:43:52.706782 kafka_overwatch-0.5.0.post0/kafka_overwatch/notifications/aws_sns/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-11 21:31:12.972386 kafka_overwatch-0.5.0.post0/kafka_overwatch/notifications/aws_sns/usage_report/__init__.py
+-rw-r--r--   0        0        0       83 2024-03-11 21:31:12.972386 kafka_overwatch-0.5.0.post0/kafka_overwatch/notifications/aws_sns/usage_report/default.j2
+-rw-r--r--   0        0        0      484 2024-03-11 21:31:12.972386 kafka_overwatch-0.5.0.post0/kafka_overwatch/notifications/aws_sns/usage_report/email.j2
+-rw-r--r--   0        0        0     4096 2024-05-23 19:30:47.508672 kafka_overwatch-0.5.0.post0/kafka_overwatch/overwatch.py
+-rw-r--r--   0        0        0       86 2024-01-02 07:32:22.104588 kafka_overwatch-0.5.0.post0/kafka_overwatch/overwatch_resources/__init__.py
+-rw-r--r--   0        0        0    13631 2024-05-23 19:30:47.508672 kafka_overwatch-0.5.0.post0/kafka_overwatch/overwatch_resources/clusters.py
+-rw-r--r--   0        0        0     5026 2024-03-11 06:55:53.345126 kafka_overwatch-0.5.0.post0/kafka_overwatch/overwatch_resources/groups.py
+-rw-r--r--   0        0        0     5340 2024-05-23 19:30:47.508672 kafka_overwatch-0.5.0.post0/kafka_overwatch/overwatch_resources/schema_registry/__init__.py
+-rw-r--r--   0        0        0     2412 2024-04-07 20:43:52.707782 kafka_overwatch-0.5.0.post0/kafka_overwatch/overwatch_resources/schema_registry/schema.py
+-rw-r--r--   0        0        0     3135 2024-04-18 23:09:58.482167 kafka_overwatch-0.5.0.post0/kafka_overwatch/overwatch_resources/schema_registry/schemas_restore.py
+-rw-r--r--   0        0        0      801 2024-04-07 20:43:52.707782 kafka_overwatch-0.5.0.post0/kafka_overwatch/overwatch_resources/schema_registry/subject.py
+-rw-r--r--   0        0        0     7349 2024-05-23 19:30:47.508672 kafka_overwatch-0.5.0.post0/kafka_overwatch/overwatch_resources/topics.py
+-rw-r--r--   0        0        0      915 2024-05-23 19:30:47.508672 kafka_overwatch-0.5.0.post0/kafka_overwatch/processing/__init__.py
+-rw-r--r--   0        0        0     5816 2024-05-23 19:30:47.509672 kafka_overwatch-0.5.0.post0/kafka_overwatch/processing/clusters.py
+-rw-r--r--   0        0        0     8995 2024-05-23 19:30:47.509672 kafka_overwatch-0.5.0.post0/kafka_overwatch/processing/schema_registries.py
+-rw-r--r--   0        0        0      302 2024-05-23 19:30:47.509672 kafka_overwatch-0.5.0.post0/kafka_overwatch/processing/signals.py
+-rw-r--r--   0        0        0     4793 2024-04-07 20:43:52.707782 kafka_overwatch-0.5.0.post0/kafka_overwatch/reporting/__init__.py
+-rw-r--r--   0        0        0       88 2024-02-14 21:24:07.217496 kafka_overwatch-0.5.0.post0/kafka_overwatch/reporting/governance/__init__.py
+-rw-r--r--   0        0        0     1364 2024-03-11 06:55:53.346126 kafka_overwatch-0.5.0.post0/kafka_overwatch/reporting/governance/consumer_groups_naming_convention.py
+-rw-r--r--   0        0        0     1355 2024-02-14 21:24:07.217496 kafka_overwatch-0.5.0.post0/kafka_overwatch/reporting/governance/topic_naming_convention.py
+-rw-r--r--   0        0        0     1128 2024-04-07 20:43:52.707782 kafka_overwatch-0.5.0.post0/kafka_overwatch/reporting/schema_registry.py
+-rw-r--r--   0        0        0     1963 2024-03-11 06:55:53.346126 kafka_overwatch-0.5.0.post0/kafka_overwatch/reporting/tools.py
+-rw-r--r--   0        0        0     3967 2024-04-07 20:43:52.707782 kafka_overwatch-0.5.0.post0/kafka_overwatch/reporting/topics.py
+-rw-r--r--   0        0        0       86 2024-01-02 07:32:22.103588 kafka_overwatch-0.5.0.post0/kafka_overwatch/specs/__init__.py
+-rw-r--r--   0        0        0    21799 2024-05-23 19:41:34.235547 kafka_overwatch-0.5.0.post0/kafka_overwatch/specs/config.json
+-rw-r--r--   0        0        0    11668 2024-04-07 20:43:52.708782 kafka_overwatch-0.5.0.post0/kafka_overwatch/specs/config.py
+-rw-r--r--   0        0        0     6716 2024-05-23 19:41:34.235547 kafka_overwatch-0.5.0.post0/kafka_overwatch/specs/report.json
+-rw-r--r--   0        0        0     3249 2024-04-07 20:43:52.708782 kafka_overwatch-0.5.0.post0/kafka_overwatch/specs/report.py
+-rw-r--r--   0        0        0     2897 2024-05-23 19:41:34.007551 kafka_overwatch-0.5.0.post0/pyproject.toml
+-rw-r--r--   0        0        0     5241 1970-01-01 00:00:00.000000 kafka_overwatch-0.5.0.post0/PKG-INFO
```

### Comparing `kafka_overwatch-0.4.0/LICENSE` & `kafka_overwatch-0.5.0.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/README.rst` & `kafka_overwatch-0.5.0.post0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -27,33 +27,43 @@
 * Exposes metrics via prometheus
 
     * Topics count
     * Partitions count
     * Number of new messages (measured with topic offsets)
 
 * AWS Secret integration for client config values
+* Schema Registry integration
+
+    * Scan schema registries, map 1 to  many kafka clusters
+    * Backup of the schemas, and CLI to restore schemas to existing/new registry.
 
 Upcoming
 ----------
 
-* Schema Registry integration
 * Multi-nodes awareness (split the load with multiple nodes)
 * `cfn-kafka-admin`_ output format
 * topic messages meta-data analysis (i.e are messages compressed?)
 * scripts to perform cleanup
 * Recommendations generated from/based on models
 * Conduktor Gateway vClusters auto-discovery
 
 
 Configuration
 ===============
 
 Whilst a much more comprehensive documentation is yet to be written, please look at ``kafka_overwatch/specs/config.json``
 which is used with `jsonschema`_ to perform validation of the input.
 
+Return codes
+=============
+
+0 - all successful.
+1 - error during execution
+2 - error importing configuration.
+
 Misc
 =====
 
 Thanks
 -------
 
 Thanks to the Apache Kafka OpenSource community for their continuous efforts in making the eco-system great.
```

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/aws_helpers/__init__.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/aws_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/aws_helpers/kafka_client_secrets.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/aws_helpers/kafka_client_secrets.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/aws_helpers/s3.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/aws_helpers/s3.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/cli/__init__.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/cli/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,15 +34,19 @@
 
 
 def profiling_setup() -> Profiler | None:
     if _ATTEMPT_PROFILING:
         _watcher_session = Session()
         try:
             profiler = Profiler(
-                "overwatch", aws_session=_watcher_session, region_name="eu-west-1"
+                environ.get("AWS_CODEGURU_PROFILER_GROUP_NAME", "overwatch"),
+                aws_session=_watcher_session,
+                region_name=environ.get(
+                    "AWS_CODEGURU_PROFILER_TARGET_REGION", "eu-west-1"
+                ),
             )
             return profiler
         except Exception as error:
             print("Failed to start CodeGuru profiler")
             print(error)
             return None
 
@@ -77,19 +81,23 @@
     from kafka_overwatch.config.config import OverwatchConfig
     from kafka_overwatch.overwatch import KafkaOverwatchService
 
     try:
         _overwatch_config: OverwatchConfig = OverwatchConfig(
             _config, prometheus_registry_dir
         )
+    except Exception as error:
+        print("Failed to load up the configuration", error)
+        return 2
+    try:
         watcher = KafkaOverwatchService(_overwatch_config)
         if profiler:
             profiler.start()
         watcher.start()
         return 0
     except Exception as error:
-        print(error)
+        print("Failed to start kafka-overwatch", error)
         return 1
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/cli/schema_registry_restore.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/cli/schema_registry_restore.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/common/__init__.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/common/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,33 +6,36 @@
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from concurrent.futures import Future
 
 import concurrent
 
+from compose_x_common.compose_x_common import keyisset
+
 from kafka_overwatch.config.logging import KAFKA_LOG
-from kafka_overwatch.processing import stop_flag
+from kafka_overwatch.processing.signals import STOP_FLAG
 
 
 def waiting_on_futures(
     executor,
     futures_to_data: list[Future] | dict[Future, Any],
     resource_type: str,
     resource_name: str,
     scan_type: str,
+    stop_flag: dict,
 ):
     _pending = len(futures_to_data)
     KAFKA_LOG.debug(
         "{}: {} | {} to scan: {}".format(
             resource_type, resource_name, scan_type, _pending
         )
     )
     while _pending > 0:
-        if stop_flag.is_set():
+        if STOP_FLAG.is_set() or stop_flag["stop"] is True:
             for _future in futures_to_data:
                 _future.cancel()
             executor.shutdown(wait=False, cancel_futures=True)
             return
         _, other = concurrent.futures.wait(futures_to_data, timeout=5)
         _pending = len([_f for _f in other if not _f.done()])
         KAFKA_LOG.debug(
```

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/config/__init__.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/config/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/config/config.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/config/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,23 +38,30 @@
             config.global_ = from_dict(Global, {"cluster_scan_interval_in_seconds": 30})
         self._config = config
         self._prometheus_registry_dir = prometheus_dir
 
         self.prometheus_registry: CollectorRegistry = CollectorRegistry(
             auto_describe=True,
         )
-        self.prometheus_collectors = set_kafka_cluster_prometheus_registry_collectors(
-            self.prometheus_registry
-        )
-        self.prometheus_collectors.update(
-            set_schema_registry_prometheus_registry_collectors(self.prometheus_registry)
-        )
-        multiprocess.MultiProcessCollector(
-            self.prometheus_registry, path=self._prometheus_registry_dir.name
-        )
+        try:
+            self.prometheus_collectors = (
+                set_kafka_cluster_prometheus_registry_collectors(
+                    self.prometheus_registry
+                )
+            )
+            self.prometheus_collectors.update(
+                set_schema_registry_prometheus_registry_collectors(
+                    self.prometheus_registry
+                )
+            )
+            multiprocess.MultiProcessCollector(
+                self.prometheus_registry, path=self._prometheus_registry_dir.name
+            )
+        except Exception as error:
+            print("Error with prometheus_registry", error)
         self.runtime_key = Fernet.generate_key()
         self.sns_channels: dict[str, SnsChannel] = {}
         self.schema_registries: dict[str, SchemaRegistry] = {}
         self.init_schema_registries()
         self.init_notification_channels()
 
     def __reduce__(self):
@@ -67,14 +74,16 @@
 
     @property
     def prometheus_registry_dir(self) -> TemporaryDirectory:
         return self._prometheus_registry_dir
 
     def init_schema_registries(self):
         """Initializes the Schema Registries client if setup in the configuration"""
+        if not self.input_config.schema_registries:
+            return
         for registry_name, registry in self.input_config.schema_registries.items():
             _registry = SchemaRegistry(registry_name, registry, self.runtime_key)
             self.schema_registries[registry_name] = _registry
 
     def init_notification_channels(self):
         if not self._config.notification_channels:
             return
```

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/config/logging.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/config/logging.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/kafka_resources/__init__.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/kafka_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/kafka_resources/groups.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/kafka_resources/groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         else:
             consumer_group: ConsumerGroup = kafka_cluster.groups[group_desc.group_id]
             consumer_group.members = group_desc.members
             consumer_group.state = group_desc.state
 
 
 def set_update_cluster_consumer_groups(
-    kafka_cluster: KafkaCluster,
+    kafka_cluster: KafkaCluster, stop_flag: dict
 ) -> None:
     """
     Lists all Consumer Groups
     Checks if all the listed CGs were present in the existing cluster CGs. If not, remove.
     Describe all Consumer Groups
     List all Consumer Group Offsets (serial, no support for list of CGs)
     If CG not in the cluster groups, add to it
@@ -138,14 +138,15 @@
         KAFKA_LOG.info(f"Kafka cluster: {kafka_cluster.name} | CGs to scan: {_pending}")
         waiting_on_futures(
             executor,
             futures_to_data,
             "Kafka Cluster",
             kafka_cluster.name,
             "Consumer groups",
+            stop_flag,
         )
 
 
 def describe_update_consumer_group_offsets(
     consumer_group: ConsumerGroup, kafka_cluster: KafkaCluster
 ) -> None:
     """
```

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/kafka_resources/topics.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/kafka_resources/topics.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,56 +9,26 @@
     from confluent_kafka.admin import TopicDescription
     from kafka_overwatch.overwatch_resources.clusters import KafkaCluster
 
 import concurrent.futures
 import re
 from datetime import datetime as dt
 
+from compose_x_common.compose_x_common import keyisset
 from confluent_kafka import TopicCollection, TopicPartition
 from confluent_kafka.admin import AclOperation, ConfigResource, ResourceType
 from confluent_kafka.error import KafkaException
 from retry.api import retry, retry_call
 
 from kafka_overwatch.common import waiting_on_futures
 from kafka_overwatch.config.logging import KAFKA_LOG
 from kafka_overwatch.kafka_resources import wait_for_result
 from kafka_overwatch.overwatch_resources.topics import Partition, Topic
 
 
-def get_filtered_topics_list(cluster: KafkaCluster) -> list[str]:
-    """
-    Lists all topics, returns them based on include and exclude regex.
-    """
-    if not cluster.topics:
-        describe_update_all_topics(cluster)
-    topics_list = list(cluster.topics.keys())
-    final_list: list[str] = []
-    if (
-        not cluster.config.topic_include_regexes
-        or not cluster.config.topic_exclude_regexes
-    ):
-        return topics_list
-    for regex in cluster.config.topic_exclude_regexes:
-        try:
-            topics_list = [topic for topic in topics_list if not re.match(regex, topic)]
-        except Exception as error:
-            KAFKA_LOG.exception(error)
-            KAFKA_LOG.error(f"Failed to parse exclude_regex with regex {regex}")
-
-    for regex in cluster.config.topic_include_regexes:
-        try:
-            for topic in topics_list:
-                if re.match(regex, topic):
-                    final_list.append(topic)
-        except Exception as error:
-            KAFKA_LOG.error(f"Failed to parse include_regex with regex {regex}")
-
-    return final_list
-
-
 @retry((KafkaException,), tries=5)
 def get_topic_descriptions(
     topic_names: list[str], admin_client
 ) -> dict[str, TopicDescription]:
     desc_topics = {
         topic_name: topic_desc.result()
         for topic_name, topic_desc in wait_for_result(
@@ -79,17 +49,15 @@
         )
         return topic_names
     except Exception as error:
         KAFKA_LOG.error(f"{kafka_cluster.name} - Failed to list topics: {error}")
         raise
 
 
-def describe_update_all_topics(
-    kafka_cluster: KafkaCluster,
-) -> None:
+def describe_update_all_topics(kafka_cluster: KafkaCluster, stop_flag: dict) -> None:
     """
     Lists all topics
     """
     topic_names = get_topics_list(kafka_cluster)
     desc_topics = retry_call(
         get_topic_descriptions, fargs=[topic_names, kafka_cluster.get_admin_client()]
     )
@@ -99,30 +67,20 @@
                 f"Topic {_cluster_topic_name} no longer in cluster {kafka_cluster.name} metadata. Clearing"
             )
             _to_clear = kafka_cluster.topics[_cluster_topic_name]
             for _partition in _to_clear.partitions.values():
                 _partition.cleanup()
             del kafka_cluster.topics[_cluster_topic_name]
 
-    if desc_topics:
-        describe_update_topics(kafka_cluster, desc_topics)
+    if desc_topics and not keyisset("stop", stop_flag):
+        describe_update_topics(kafka_cluster, desc_topics, stop_flag)
     else:
         KAFKA_LOG.info(f"No topics matched for {kafka_cluster.name}")
 
 
-def retry_kafka(future, futures_to_data, executor):
-    # get the associated data for the task
-    data = futures_to_data[future]
-    # submit the task again
-    _retry = executor.submit(init_set_partitions, data)
-    # store so we can track the retries
-    futures_to_data[_retry] = data
-    return data
-
-
 def update_set_topic_config(kafka_cluster, topics_configs_resources) -> None:
     if not topics_configs_resources:
         return
     try:
         topics_config = wait_for_result(
             kafka_cluster.get_admin_client().describe_configs(topics_configs_resources)
         )
@@ -169,15 +127,17 @@
             _topic,
             now,
         ]
 
     return topic_jobs, topics_configs_resources
 
 
-def describe_update_topics(kafka_cluster: KafkaCluster, desc_topics: dict) -> None:
+def describe_update_topics(
+    kafka_cluster: KafkaCluster, desc_topics: dict, stop_flag
+) -> None:
     """
     Leverages threads to retrieve the topic offset watermarks which cannot be sent in a single
     call to Kafka.
     """
     topic_jobs, topics_configs_resources = define_topic_jobs(kafka_cluster, desc_topics)
     _tasks = len(topic_jobs)
     with concurrent.futures.ThreadPoolExecutor(
@@ -195,14 +155,15 @@
         )
         waiting_on_futures(
             executor,
             futures_to_data,
             "Kafka Cluster",
             kafka_cluster.name,
             "Topics",
+            stop_flag,
         )
 
     update_set_topic_config(kafka_cluster, topics_configs_resources)
 
 
 @retry((KafkaException,), tries=10, delay=5, backoff=2, jitter=(2, 5), logger=KAFKA_LOG)
 def get_topic_partition_watermarks(consumer_client, topic_name, partition_id):
```

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/monitoring/prometheus.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/monitoring/prometheus.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/notifications/aws_sns/__init__.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/notifications/aws_sns/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/overwatch.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/overwatch.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 #  SPDX-License-Identifier: MPL-2.0
 #  Copyright 2024 John Mille <john@ews-network.net>
 
 from __future__ import annotations
 
+import time
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from kafka_overwatch.config.config import OverwatchConfig
 
 import concurrent.futures
 import signal
+from multiprocessing import Event, Manager
 
 from kafka_overwatch.config.logging import KAFKA_LOG
 from kafka_overwatch.overwatch_resources.clusters import KafkaCluster
-from kafka_overwatch.processing import handle_signals, stop_flag
 from kafka_overwatch.processing.clusters import process_cluster
 from kafka_overwatch.processing.schema_registries import process_schema_registry
 
+STOP_FLAG = Event()
+
+
+def handle_signals(pid, frame, stop_flag):
+    print("Cluster processing received signal to stop", pid, frame)
+    stop_flag["stop"] = True
+    STOP_FLAG.set()
+
 
 class KafkaOverwatchService:
     """
     Main service which starts the prometheus server and the processes for each
     Kafka cluster to be processed independently.
 
     Upon receiving SIGTERM or SIGINT, it will send a SIGTERM to all child processes
@@ -28,52 +37,64 @@
     The prometheus dependency is imported at the last minute to make sure it will take the
     multiprocess folder env var into account.
     """
 
     def __init__(self, config: OverwatchConfig) -> None:
         self._config = config
         self.kafka_clusters: dict[str, KafkaCluster] = {}
-        signal.signal(signal.SIGINT, handle_signals)
-        signal.signal(signal.SIGTERM, handle_signals)
 
     @property
     def config(self) -> OverwatchConfig:
         return self._config
 
-    def init_system(self):
+    def init_prometheus(self):
         """
         Import prometheus_client.start_http_server at the latest point to make sure the
         multiprocess folder env var is taken into account.
         """
         from prometheus_client import start_http_server
 
-        start_http_server(8000, registry=self.config.prometheus_registry)
+        return start_http_server(8000, registry=self.config.prometheus_registry)
 
     def start(self):
         KAFKA_LOG.info("Starting Kafka Overwatch")
-        self.init_system()
+        httpd, _ = self.init_prometheus()
         clusters_jobs = []
+        manager = Manager()
+        stop_flag = manager.dict()
+        stop_flag["stop"] = False
+
+        signal.signal(
+            signal.SIGTERM,
+            lambda signum, frame: handle_signals(signum, frame, stop_flag),
+        )
+        signal.signal(
+            signal.SIGINT,
+            lambda signum, frame: handle_signals(signum, frame, stop_flag),
+        )
+
         self.kafka_clusters.update(
             {
                 name: KafkaCluster(name, config, self.config)
                 for name, config in self.config.input_config.clusters.items()
             }
         )
         sr_jobs: list = [
-            [_sr, self.config.runtime_key, self.config]
+            [_sr, self.config.runtime_key, self.config, stop_flag]
             for _sr in self.config.schema_registries.values()
         ]
         for (
             cluster_name,
             cluster,
         ) in self.kafka_clusters.items():
-            clusters_jobs.append([cluster, self.config])
-        self.multi_clusters_processing(clusters_jobs, sr_jobs)
+            clusters_jobs.append([cluster, self.config, stop_flag])
+        self.multi_clusters_processing(clusters_jobs, sr_jobs, httpd)
 
-    def multi_clusters_processing(self, clusters_jobs: list, sr_jobs: list):
+    @staticmethod
+    def multi_clusters_processing(clusters_jobs: list, sr_jobs: list, httpd):
         with concurrent.futures.ProcessPoolExecutor(
             max_workers=(len(clusters_jobs) + len(sr_jobs))
         ) as executor:
             futures_to_data: dict[concurrent.futures.Future, list] = {}
             if sr_jobs:
                 futures_to_data.update(
                     {
@@ -84,14 +105,16 @@
             futures_to_data.update(
                 {
                     executor.submit(process_cluster, *cluster_job): cluster_job
                     for cluster_job in clusters_jobs
                 }
             )
             try:
-                while not stop_flag.is_set():
+                while not STOP_FLAG.is_set():
                     concurrent.futures.wait(futures_to_data, timeout=10)
             except KeyboardInterrupt:
-                for _future in futures_to_data:
-                    _future.cancel()
                 executor.shutdown(wait=True, cancel_futures=True)
+            finally:
+                executor.shutdown(wait=True, cancel_futures=True)
+                print("Executor has been shut down")
+                httpd.shutdown()
         return
```

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/clusters.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/overwatch_resources/clusters.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 from prometheus_client import Gauge, Summary
 from retry import retry
 
 from kafka_overwatch.aws_helpers.kafka_client_secrets import eval_kafka_client_config
 from kafka_overwatch.aws_helpers.s3 import S3Handler
 from kafka_overwatch.config.logging import KAFKA_LOG
 from kafka_overwatch.kafka_resources import set_admin_client, set_consumer_client
-from kafka_overwatch.kafka_resources.topics import get_filtered_topics_list
 from kafka_overwatch.overwatch_resources.schema_registry import SchemaRegistry
 from kafka_overwatch.processing import ensure_prometheus_multiproc
 from kafka_overwatch.specs.config import (
     ClusterConfiguration,
     ClusterTopicBackupConfig,
     Exports,
 )
@@ -202,23 +201,14 @@
     @property
     def prometheus_collectors(self):
         if hasattr(self, "_prometheus_collectors"):
             return self._prometheus_collectors
         else:
             return self._overwatch_config.prometheus_collectors
 
-    @property
-    def monitored_topics(self) -> dict[str, Topic]:
-        matching_topic_names = get_filtered_topics_list(self)
-        return {
-            topic_name: topic
-            for topic_name, topic in self.topics.items()
-            if topic_name in matching_topic_names
-        }
-
     @retry((KafkaException,), tries=5, logger=KAFKA_LOG)
     def set_cluster_connections(self) -> None:
         client_config = eval_kafka_client_config(self)
         self._admin_client: AdminClient = set_admin_client(client_config)
         self._consumer_client: Consumer = set_consumer_client(client_config)
 
     @retry((KafkaException,), tries=2, logger=KAFKA_LOG)
```

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/groups.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/overwatch_resources/groups.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/schema_registry/__init__.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/overwatch_resources/schema_registry/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from kafka_overwatch.overwatch_resources.clusters import KafkaCluster
     from .subject import Subject
     from .schema import Schema
 
+from datetime import datetime as dt
 from tempfile import TemporaryDirectory
 
 from cryptography.fernet import Fernet
 from kafka_schema_registry_admin import SchemaRegistry as SchemaRegistryClient
 
 from kafka_overwatch.aws_helpers.s3 import S3Handler
 from kafka_overwatch.specs.config import ConfluentSchemaRegistry
@@ -59,40 +60,44 @@
         """Index of subjects in the registry"""
         self.subjects: dict[str, Subject] = {}
         """Index of the schemas in the registry"""
         self.schemas: dict[int, Schema] = {}
         """Kafka clusters this schema registry is linked to"""
         self.kafka_clusters: dict[str, KafkaCluster] = {}
         self._config = registry_config
-        self.s3_backup_handler: S3Handler | None = None
-        if self.config.backup_config and self.config.backup_config.enabled:
-            self.s3_backup_handler = S3Handler(self.config.backup_config.S3)
-
         self.supported_types = ["JSON", "PROTOBUF", "AVRO"]
 
     @property
     def config(self) -> SchemaRegistryConfig:
         return self._config
 
     def __repr__(self):
         return self.name
 
+    def init_backup_handler(self) -> S3Handler:
+        if (
+            self.config.backup_config
+            and self.config.backup_config.S3
+            and self.config.backup_config.enabled
+        ):
+            return S3Handler(self.config.backup_config.S3)
+
     def get_client(self, runtime_key) -> SchemaRegistryClient | None:
         if self.basic_auth:
             kwargs: dict = self.basic_auth.get_sr_creds(runtime_key)
         else:
             kwargs: dict = {}
         if isinstance(self._config.config, ConfluentSchemaRegistry):
             return SchemaRegistryClient(
                 self.config.config.schema_registry_url,
                 **kwargs,
             )
 
-    def backup(self):
-        if not self.s3_backup_handler:
+    def backup(self, s3_backup_handler: S3Handler | None):
+        if not s3_backup_handler:
             return
         process_folder = TemporaryDirectory()
         schemas_folder: TemporaryDirectory = TemporaryDirectory(dir=process_folder.name)
         subjects_index: dict = {}
         for _subject in self.subjects.values():
             if _subject.name not in subjects_index:
                 _subject_index: dict = {}
@@ -111,14 +116,14 @@
         for _subject in subjects_index:
             subjects_index[_subject] = dict(sorted(subjects_index[_subject].items()))
         with open(f"{schemas_folder.name}/index.json", "w") as index_fd:
             index_fd.write(json.dumps(subjects_index, sort_keys=True))
         with tarfile.open(f"{process_folder.name}/schemas.tar.gz", "w:gz") as tar:
             tar.add(schemas_folder.name, arcname=".")
         with open(f"{process_folder.name}/schemas.tar.gz", "rb") as gz_fd:
-            self.s3_backup_handler.upload(
+            s3_backup_handler.upload(
                 body=gz_fd.read(),
-                file_name="schemas.tar.gz",
+                file_name=f'{self.name}/{dt.now().strftime("%Y/%m/%d/%H_%M")}/schemas.tar.gz',
                 mime_type="application/gzip",
             )
         schemas_folder.cleanup()
         process_folder.cleanup()
```

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/schema_registry/schema.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/overwatch_resources/schema_registry/schema.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/schema_registry/schemas_restore.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/overwatch_resources/schema_registry/schemas_restore.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/schema_registry/subject.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/overwatch_resources/schema_registry/subject.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/topics.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/overwatch_resources/topics.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         return {
             "name": self.name,
             "partitions": len(self.partitions),
             "total_messages": sum(
                 _p.total_messages_count for _p in self.partitions.values()
             ),
             "new_messages": new_messages,
-            "eval_elapsed_time": elapsed_time.total_seconds(),
+            "eval_elapsed_time": elapsed_time,
             "consumer_groups": len(self.consumer_groups),
             "active_groups": len(
                 [_cg for _cg in self.consumer_groups.values() if _cg.is_active]
             ),
         }
 
     def generate_kafka_create_topic_command(self):
@@ -199,15 +199,18 @@
 
     def has_new_messages(self) -> bool:
         """Returns True if the topic has new messages by checking if any partition had new messages"""
         return any(
             [_partition.has_new_messages() for _partition in self.partitions.values()]
         )
 
-    def new_messages_count(self) -> tuple[int, td]:
+    def new_messages_count(self) -> tuple[int, int]:
         total_messages: int = 0
+        if not self.partitions:
+            return 0, 0
         elapsed_time = (
             self.partitions[0].end_offset[1] - self.partitions[0].init_start_offset[1]
         )
+
         for partition in self.partitions.values():
             total_messages += partition.get_end_offset_diff()[0]
-        return total_messages, elapsed_time
+        return total_messages, int(elapsed_time.total_seconds())
```

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/processing/__init__.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/processing/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,25 @@
 #  SPDX-License-Identifier: MPL-2.0
 #  Copyright 2024 John Mille <john@ews-network.net>
+
 from __future__ import annotations
 
 import os
 import time
-from threading import Event
-
-FOREVER = 42
-stop_flag = Event()
-
-
-def handle_signals(pid, frame):
-    print("Cluster processing received signal to stop", pid, frame)
-    global stop_flag
-    stop_flag.set()
 
 
-def wait_between_intervals(time_to_wait: int, too_short_desc: str = None) -> None:
+def wait_between_intervals(
+    stop_flag: dict, time_to_wait: int, too_short_desc: str = None
+) -> None:
     if time_to_wait <= 0:
         if too_short_desc is not None:
             print(too_short_desc)
     else:
         for _ in range(1, time_to_wait):
-            if stop_flag.is_set():
+            if stop_flag["stop"] is True:
                 break
             time.sleep(1)
 
 
 def ensure_prometheus_multiproc(prometheus_dir_path: str):
     """
     Just in case the env_var had not propagated among processes,
```

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/processing/clusters.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/processing/clusters.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,31 +6,32 @@
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from pandas import DataFrame
     from prometheus_client import Gauge
     from kafka_overwatch.config.config import OverwatchConfig
 
-import signal
 from datetime import datetime as dt
 from datetime import timedelta as td
 
+from compose_x_common.compose_x_common import keyisset
+
 from kafka_overwatch.config.logging import KAFKA_LOG
 from kafka_overwatch.kafka_resources.groups import (
     set_update_cluster_consumer_groups,
     update_set_consumer_group_topics_partitions_offsets,
 )
 from kafka_overwatch.kafka_resources.topics import describe_update_all_topics
 from kafka_overwatch.overwatch_resources.clusters import (
     KafkaCluster,
     generate_cluster_consumer_groups_pd_dataframe,
     generate_cluster_topics_pd_dataframe,
 )
 
-from . import FOREVER, handle_signals, stop_flag, wait_between_intervals
+from . import wait_between_intervals
 
 
 def measure_consumer_group_lags(
     kafka_cluster: KafkaCluster, consumer_group_lag_gauge: Gauge
 ):
     """
     Evaluates, if consumer groups were retrieved, the consumer groups lags and export metrics
@@ -58,40 +59,37 @@
     ):
         kafka_cluster.render_report(topics_df, groups_df)
         kafka_cluster.next_reporting = dt.utcnow() + td(
             seconds=kafka_cluster.config.reporting_config.evaluation_period_in_seconds
         )
 
 
-def process_cluster(kafka_cluster: KafkaCluster, overwatch_config: OverwatchConfig):
+def process_cluster(
+    kafka_cluster: KafkaCluster, overwatch_config: OverwatchConfig, stop_flag
+):
     """
     Initialize the Kafka cluster monitoring/evaluation loop.
     Creates the cluster, which creates the Kafka clients.
     """
-    signal.signal(signal.SIGINT, handle_signals)
-    signal.signal(signal.SIGTERM, handle_signals)
     kafka_cluster.init_cluster_prometheus_reporting(overwatch_config)
     kafka_cluster.set_reporting_exporters()
     kafka_cluster.set_cluster_connections()
     consumer_group_lag_gauge = overwatch_config.prometheus_collectors[
         "consumer_group_lag"
     ]
-    while FOREVER:
+    print(stop_flag["stop"] is False)
+    while stop_flag["stop"] is False:
+        print("Cluster loop", stop_flag)
         try:
             kafka_cluster.check_replace_kafka_clients()
             kafka_cluster.set_cluster_properties()
-            print(
-                "PROCESSING LOOP - CLIENTS??",
-                hex(id(kafka_cluster._admin_client)),
-                hex(id(kafka_cluster._consumer_client)),
-            )
 
             processing_start = dt.utcnow()
-            if not stop_flag.is_set():
-                process_cluster_resources(kafka_cluster)
+            if not keyisset("stop", stop_flag):
+                process_cluster_resources(kafka_cluster, stop_flag)
             else:
                 break
             topics_df = generate_cluster_topics_pd_dataframe(kafka_cluster)
             groups_df = generate_cluster_consumer_groups_pd_dataframe(kafka_cluster)
             kafka_cluster.cluster_topics_count.set(
                 len(topics_df["name"].values.tolist())
             )
@@ -111,14 +109,15 @@
             print(groups_df.describe())
             measure_consumer_group_lags(kafka_cluster, consumer_group_lag_gauge)
             generate_cluster_report(kafka_cluster, topics_df, groups_df)
             time_to_wait = int(
                 kafka_cluster.config.cluster_scan_interval_in_seconds - elapsed_time
             )
             wait_between_intervals(
+                stop_flag,
                 time_to_wait,
                 (
                     f"{kafka_cluster.name} - interval set to {kafka_cluster.config.cluster_scan_interval_in_seconds}"
                     f", however it takes {elapsed_time}s to complete the scan. Consider changing scan interval"
                 ),
             )
         except Exception as e:
@@ -129,20 +128,20 @@
             except Exception as e:
                 KAFKA_LOG.exception(e)
                 KAFKA_LOG.error(f"{kafka_cluster.name} - {e}")
                 return
     return
 
 
-def process_cluster_resources(kafka_cluster: KafkaCluster):
+def process_cluster_resources(kafka_cluster: KafkaCluster, stop_flag):
     """Makes sure that no signal was received in between each instruction"""
-    if not stop_flag.is_set():
+    if stop_flag["stop"] is False:
         with kafka_cluster.groups_describe_latency.time():
-            set_update_cluster_consumer_groups(kafka_cluster)
-    if not stop_flag.is_set():
+            set_update_cluster_consumer_groups(kafka_cluster, stop_flag)
+    if stop_flag["stop"] is False:
         with kafka_cluster.topics_describe_latency.time():
-            describe_update_all_topics(kafka_cluster)
-    if not stop_flag.is_set():
+            describe_update_all_topics(kafka_cluster, stop_flag)
+    if stop_flag["stop"] is False:
         for consumer_group in kafka_cluster.groups.values():
             update_set_consumer_group_topics_partitions_offsets(
                 kafka_cluster, consumer_group
             )
```

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/processing/schema_registries.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/processing/schema_registries.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,34 +9,35 @@
 if TYPE_CHECKING:
     from kafka_overwatch.overwatch_resources.schema_registry import (
         SchemaRegistry,
     )
     from kafka_overwatch.config.config import OverwatchConfig
 
 import pickle
-import signal
 from datetime import datetime, timedelta, timezone
 
-from compose_x_common.compose_x_common import set_else_none
+from compose_x_common.compose_x_common import keyisset, set_else_none
 from prometheus_client import Gauge
 
 from kafka_overwatch.common import waiting_on_futures
 from kafka_overwatch.config.logging import KAFKA_LOG
 from kafka_overwatch.config.threads_settings import NUM_THREADS
 from kafka_overwatch.overwatch_resources.schema_registry.schema import (
     Schema,
     refresh_subject_metadata,
 )
 from kafka_overwatch.overwatch_resources.schema_registry.subject import Subject
 from kafka_overwatch.processing import ensure_prometheus_multiproc
 
-from . import FOREVER, handle_signals, stop_flag, wait_between_intervals
+from . import wait_between_intervals
 
 
-def retrieve_from_subjects(schema_registry: SchemaRegistry, sr_client) -> None:
+def retrieve_from_subjects(
+    schema_registry: SchemaRegistry, sr_client, stop_flag
+) -> None:
     """
     Much longer way to retrieve all the schemas & subjects, using the subjects endpoints.
     Using threading to speed up the processing, but still slower by an order of magnitude
     than retrieving the schemas directly.
     """
     KAFKA_LOG.info(f"{schema_registry.name} - Retrieving all subjects")
     all_subjects = sr_client.get_all_subjects().json()
@@ -67,14 +68,15 @@
         )
         waiting_on_futures(
             executor,
             futures_to_data,
             "Schema Registry",
             schema_registry.name,
             "Subjects",
+            stop_flag,
         )
 
 
 def retrieve_from_schemas(schema_registry: SchemaRegistry, sr_client) -> None:
     """
     Fastest way, used if /schemas worked
     """
@@ -122,27 +124,27 @@
     schemas_count: Gauge = overwatch_config.prometheus_collectors["schemas_count"]
 
     subjects_count = subjects_count.labels(schema_registry=schema_registry.name)
     schemas_count = schemas_count.labels(schema_registry=schema_registry.name)
     return subjects_count, schemas_count
 
 
-def process_schemas(schema_registry: SchemaRegistry, sr_client) -> None:
+def process_schemas(schema_registry: SchemaRegistry, sr_client, stop_flag) -> None:
     """
     Process all schemas in the schema registry.
     If getting schemas from /schemas fails, fall back to /subjects
     """
     try:
         retrieve_from_schemas(schema_registry, sr_client)
     except Exception as error:
         KAFKA_LOG.exception(error)
         KAFKA_LOG.error(
             f"{schema_registry.name} Failed to retrieve schemas via /schemas"
         )
-        retrieve_from_subjects(schema_registry, sr_client)
+        retrieve_from_subjects(schema_registry, sr_client, stop_flag)
 
 
 def set_prometheus_metrics(
     subjects_count, schemas_count, schema_registry: SchemaRegistry
 ):
     try:
         subjects_count.set(len(schema_registry.subjects))
@@ -154,16 +156,15 @@
             % (schema_registry.name,)
         )
 
 
 def backup_schema_registry_subjects(schema_registry: SchemaRegistry) -> None:
     """Attempts to back up all the subjects and their associated schemas to S3."""
     try:
-        if schema_registry.s3_backup_handler:
-            schema_registry.backup()
+        schema_registry.backup(schema_registry.init_backup_handler())
     except Exception as error:
         KAFKA_LOG.exception(error)
         KAFKA_LOG.error(
             f"Schema Registry: {schema_registry.name} | Failed to backup to S3"
         )
 
 
@@ -181,37 +182,37 @@
         KAFKA_LOG.error(
             "Schema Registry: %s | Failed to write mmap file to %s"
             % (schema_registry.name, schema_registry.mmap_file)
         )
 
 
 def process_schema_registry(
-    schema_registry: SchemaRegistry, runtime_key, overwatch_config: OverwatchConfig
+    schema_registry: SchemaRegistry,
+    runtime_key,
+    overwatch_config: OverwatchConfig,
+    stop_flag,
 ) -> None:
     """Process function for the schema registry. Responsible for
 
     * retrieving all the schemas & subjects
     * backup the subjects & schemas if configured.
 
     """
-    signal.signal(signal.SIGINT, handle_signals)
-    signal.signal(signal.SIGTERM, handle_signals)
     subjects_count, schemas_count = init_schema_registry_prometheus_reporting(
         schema_registry, overwatch_config
     )
     sr_client = schema_registry.get_client(runtime_key)
-    while FOREVER:
-        if stop_flag.is_set():
-            break
+    schema_registry.init_backup_handler()
+    while stop_flag["stop"] is False:
         now = datetime.now(timezone.utc)
         next_scan = now + timedelta(
             seconds=schema_registry.config.schema_registry_scan_interval
         )
         try:
-            process_schemas(schema_registry, sr_client)
+            process_schemas(schema_registry, sr_client, stop_flag)
             set_prometheus_metrics(subjects_count, schemas_count, schema_registry)
             backup_schema_registry_subjects(schema_registry)
             write_schema_registry_mmap(schema_registry)
         except Exception as error:
             KAFKA_LOG.exception(error)
             KAFKA_LOG.error(
                 "Schema registry: %s | Failed to process successfully."
@@ -220,14 +221,15 @@
             schema_registry.temp_bin_dir.cleanup()
             return
         then = datetime.now(timezone.utc)
         delta = int((next_scan - then).total_seconds())
         if delta > 0:
             KAFKA_LOG.info("%s - Waiting %d seconds" % (schema_registry.name, delta))
             wait_between_intervals(
+                stop_flag,
                 delta,
             )
         else:
             KAFKA_LOG.warning(
                 "%s - Interval is %d - yet it took %d to complete processing."
                 % (
                     schema_registry.name,
```

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/reporting/__init__.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/reporting/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/reporting/governance/consumer_groups_naming_convention.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/reporting/governance/consumer_groups_naming_convention.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/reporting/governance/topic_naming_convention.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/reporting/governance/topic_naming_convention.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/reporting/schema_registry.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/reporting/schema_registry.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/reporting/tools.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/reporting/tools.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/reporting/topics.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/reporting/topics.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/specs/config.json` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/specs/config.json`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/specs/config.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/specs/config.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/specs/report.json` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/specs/report.json`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/kafka_overwatch/specs/report.py` & `kafka_overwatch-0.5.0.post0/kafka_overwatch/specs/report.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.4.0/pyproject.toml` & `kafka_overwatch-0.5.0.post0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kafka-overwatch"
-version = "0.4.0"
+version = "0.5.0-post0"
 description = "Continuously monitors Kafka cluster topics & consumer groups"
 authors = ["John \"Preston\" Mille <john@ews-network.net>"]
 maintainers = ["John \"Preston\" Mille <john@ews-network.net>"]
 readme = "README.rst"
 license = "MPL-2.0"
 keywords = ["kafka", "monitoring", "reporting", "usage-analysis", "cost-savings"]
 
@@ -25,24 +25,24 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/JohnPreston/kafka-overwatch/issues"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 confluent-kafka = "^2.3.0"
-compose-x-common = "^1.4.4"
+compose-x-common = "^1.4"
 boto3 = ">=1.26,<2.0"
 dacite = "^1.8.1"
 pyyaml = "^6.0.1"
 aws-cfn-custom-resource-resolve-parser = "^0.3"
 retry2 = "^0.9.5"
 jsonschema = "^4.20.0"
 aws-embedded-metrics = "^3.2.0"
 importlib-resources = "^6.1.1"
-prometheus-client = "^0.19.0"
+prometheus-client = "^0.20"
 jinja2 = "^3.1.2"
 aws-msk-iam-sasl-signer-python = "^1.0.0"
 pandas = "^2.1.4"
 codeguru-profiler-agent = "^1.2.4"
 kafka-schema-registry-admin = ">=0.5"
 cryptography = "^42.0.5"
 
@@ -88,15 +88,15 @@
   "*/cli.py"
 ]
 
 [tool.tbump]
 github_url = "https://github.com/johnpreston/kafka-overwatch"
 
 [tool.tbump.version]
-current = "0.4.0"
+current = "0.5.0-post0"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?:(?P<rc>[\S]+))?
```

### Comparing `kafka_overwatch-0.4.0/PKG-INFO` & `kafka_overwatch-0.5.0.post0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-overwatch
-Version: 0.4.0
+Version: 0.5.0.post0
 Summary: Continuously monitors Kafka cluster topics & consumer groups
 License: MPL-2.0
 Keywords: kafka,monitoring,reporting,usage-analysis,cost-savings
 Author: John "Preston" Mille
 Author-email: john@ews-network.net
 Maintainer: John "Preston" Mille
 Maintainer-email: john@ews-network.net
@@ -21,24 +21,24 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aws-cfn-custom-resource-resolve-parser (>=0.3,<0.4)
 Requires-Dist: aws-embedded-metrics (>=3.2.0,<4.0.0)
 Requires-Dist: aws-msk-iam-sasl-signer-python (>=1.0.0,<2.0.0)
 Requires-Dist: boto3 (>=1.26,<2.0)
 Requires-Dist: codeguru-profiler-agent (>=1.2.4,<2.0.0)
-Requires-Dist: compose-x-common (>=1.4.4,<2.0.0)
+Requires-Dist: compose-x-common (>=1.4,<2.0)
 Requires-Dist: confluent-kafka (>=2.3.0,<3.0.0)
 Requires-Dist: cryptography (>=42.0.5,<43.0.0)
 Requires-Dist: dacite (>=1.8.1,<2.0.0)
 Requires-Dist: importlib-resources (>=6.1.1,<7.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jsonschema (>=4.20.0,<5.0.0)
 Requires-Dist: kafka-schema-registry-admin (>=0.5)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
-Requires-Dist: prometheus-client (>=0.19.0,<0.20.0)
+Requires-Dist: prometheus-client (>=0.20,<0.21)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: retry2 (>=0.9.5,<0.10.0)
 Project-URL: Bug Tracker, https://github.com/JohnPreston/kafka-overwatch/issues
 Description-Content-Type: text/x-rst
 
 ========================================
 kafka-overwatch
@@ -69,33 +69,43 @@
 * Exposes metrics via prometheus
 
     * Topics count
     * Partitions count
     * Number of new messages (measured with topic offsets)
 
 * AWS Secret integration for client config values
+* Schema Registry integration
+
+    * Scan schema registries, map 1 to  many kafka clusters
+    * Backup of the schemas, and CLI to restore schemas to existing/new registry.
 
 Upcoming
 ----------
 
-* Schema Registry integration
 * Multi-nodes awareness (split the load with multiple nodes)
 * `cfn-kafka-admin`_ output format
 * topic messages meta-data analysis (i.e are messages compressed?)
 * scripts to perform cleanup
 * Recommendations generated from/based on models
 * Conduktor Gateway vClusters auto-discovery
 
 
 Configuration
 ===============
 
 Whilst a much more comprehensive documentation is yet to be written, please look at ``kafka_overwatch/specs/config.json``
 which is used with `jsonschema`_ to perform validation of the input.
 
+Return codes
+=============
+
+0 - all successful.
+1 - error during execution
+2 - error importing configuration.
+
 Misc
 =====
 
 Thanks
 -------
 
 Thanks to the Apache Kafka OpenSource community for their continuous efforts in making the eco-system great.
```

