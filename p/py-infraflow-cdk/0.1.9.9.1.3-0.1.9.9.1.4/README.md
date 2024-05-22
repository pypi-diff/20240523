# Comparing `tmp/py_infraflow_cdk-0.1.9.9.1.3.tar.gz` & `tmp/py_infraflow_cdk-0.1.9.9.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_infraflow_cdk-0.1.9.9.1.3.tar", max compression
+gzip compressed data, was "py_infraflow_cdk-0.1.9.9.1.4.tar", max compression
```

## Comparing `py_infraflow_cdk-0.1.9.9.1.3.tar` & `py_infraflow_cdk-0.1.9.9.1.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      337 2024-01-24 18:03:42.816211 py_infraflow_cdk-0.1.9.9.1.3/README.md
--rw-r--r--   0        0        0        0 2024-01-22 17:24:55.856613 py_infraflow_cdk-0.1.9.9.1.3/infraflow/__init__.py
--rw-r--r--   0        0        0      240 2024-01-22 17:24:55.856719 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/__init__.py
--rw-r--r--   0        0        0        0 2024-01-22 17:24:55.856794 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/_step_functions/__init__.py
--rw-r--r--   0        0        0     1329 2024-01-22 17:24:55.856883 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/_step_functions/core.py
--rw-r--r--   0        0        0     1261 2024-01-22 17:24:55.856942 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/_step_functions/patterns.py
--rw-r--r--   0        0        0      280 2024-01-22 17:24:55.857004 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/api_gateway.py
--rw-r--r--   0        0        0     7399 2024-05-22 22:22:01.944518 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/app_patterns/express_default_dlq_processor.py
--rw-r--r--   0        0        0    12829 2024-05-22 22:26:07.349206 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/app_patterns/standard.py
--rw-r--r--   0        0        0      156 2024-01-22 17:24:55.857163 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/arns.py
--rw-r--r--   0        0        0        0 2024-01-22 17:24:55.857224 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/core/__init__.py
--rw-r--r--   0        0        0      364 2024-01-22 17:24:55.857292 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/core/component_service.py
--rw-r--r--   0        0        0      316 2024-01-22 17:24:55.857349 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/core/construct.py
--rw-r--r--   0        0        0     5168 2024-03-20 16:31:56.831033 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/core/environment.py
--rw-r--r--   0        0        0     1020 2024-01-24 18:03:42.816662 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/core/service_stage.py
--rw-r--r--   0        0        0      367 2024-02-19 16:57:57.498391 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/core/utils.py
--rw-r--r--   0        0        0    10397 2024-05-08 20:06:25.481166 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/docker.py
--rw-r--r--   0        0        0     9235 2024-05-10 16:52:15.747978 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/events.py
--rw-r--r--   0        0        0      139 2024-01-22 17:24:55.857712 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/iam/__init__.py
--rw-r--r--   0        0        0   533095 2024-01-24 18:03:42.817968 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/iam/_actions.py
--rw-r--r--   0        0        0   249582 2024-01-22 17:24:55.859417 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/iam/action_groups.py
--rw-r--r--   0        0        0   108710 2024-01-22 17:24:55.859750 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/iam/actions
--rw-r--r--   0        0        0     4943 2024-01-22 17:24:55.859832 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/iam/base.py
--rw-r--r--   0        0        0        0 2024-03-20 16:31:56.831151 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/instrumentation/__init__.py
--rw-r--r--   0        0        0     1376 2024-04-11 23:31:09.973506 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/instrumentation/alarms.py
--rw-r--r--   0        0        0     5976 2024-04-24 21:59:03.929389 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/instrumentation/docker.py
--rw-r--r--   0        0        0     7347 2024-04-25 19:01:22.356096 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/instrumentation/lambdas.py
--rw-r--r--   0        0        0     1704 2024-04-11 23:31:09.974803 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/instrumentation/metrics.py
--rw-r--r--   0        0        0     4435 2024-04-11 23:31:09.975272 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/instrumentation/queues.py
--rw-r--r--   0        0        0     6482 2024-05-22 22:26:07.349492 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/lambdas.py
--rw-r--r--   0        0        0      349 2024-02-28 20:32:26.259456 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/queue.py
--rw-r--r--   0        0        0        0 2024-01-22 17:24:55.859986 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/sg/__init__.py
--rw-r--r--   0        0        0     3481 2024-01-24 18:03:42.818220 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/sg/patterns.py
--rw-r--r--   0        0        0      715 2024-01-24 18:03:42.818283 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/sg/ports.py
--rw-r--r--   0        0        0      629 2024-01-22 17:24:55.860118 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/sg/tier_maps.py
--rw-r--r--   0        0        0      141 2024-01-24 18:03:42.818392 py_infraflow_cdk-0.1.9.9.1.3/infraflow/priv_utils/__init__.py
--rw-r--r--   0        0        0      154 2024-01-22 17:24:55.860264 py_infraflow_cdk-0.1.9.9.1.3/infraflow/util.py
--rw-r--r--   0        0        0      687 2024-05-22 22:26:07.349713 py_infraflow_cdk-0.1.9.9.1.3/pyproject.toml
--rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 py_infraflow_cdk-0.1.9.9.1.3/PKG-INFO
+-rw-r--r--   0        0        0      337 2024-01-24 18:03:42.816211 py_infraflow_cdk-0.1.9.9.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-01-22 17:24:55.856613 py_infraflow_cdk-0.1.9.9.1.4/infraflow/__init__.py
+-rw-r--r--   0        0        0      240 2024-01-22 17:24:55.856719 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-22 17:24:55.856794 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/_step_functions/__init__.py
+-rw-r--r--   0        0        0     1329 2024-01-22 17:24:55.856883 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/_step_functions/core.py
+-rw-r--r--   0        0        0     1261 2024-01-22 17:24:55.856942 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/_step_functions/patterns.py
+-rw-r--r--   0        0        0      280 2024-01-22 17:24:55.857004 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/api_gateway.py
+-rw-r--r--   0        0        0     7399 2024-05-22 22:22:01.944518 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/app_patterns/express_default_dlq_processor.py
+-rw-r--r--   0        0        0    12829 2024-05-22 22:26:07.349206 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/app_patterns/standard.py
+-rw-r--r--   0        0        0      156 2024-01-22 17:24:55.857163 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/arns.py
+-rw-r--r--   0        0        0        0 2024-01-22 17:24:55.857224 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/core/__init__.py
+-rw-r--r--   0        0        0      364 2024-01-22 17:24:55.857292 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/core/component_service.py
+-rw-r--r--   0        0        0      316 2024-01-22 17:24:55.857349 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/core/construct.py
+-rw-r--r--   0        0        0     5168 2024-03-20 16:31:56.831033 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/core/environment.py
+-rw-r--r--   0        0        0     1020 2024-01-24 18:03:42.816662 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/core/service_stage.py
+-rw-r--r--   0        0        0      367 2024-02-19 16:57:57.498391 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/core/utils.py
+-rw-r--r--   0        0        0    10397 2024-05-08 20:06:25.481166 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/docker.py
+-rw-r--r--   0        0        0     9235 2024-05-10 16:52:15.747978 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/events.py
+-rw-r--r--   0        0        0      139 2024-01-22 17:24:55.857712 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/iam/__init__.py
+-rw-r--r--   0        0        0   533095 2024-01-24 18:03:42.817968 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/iam/_actions.py
+-rw-r--r--   0        0        0   249582 2024-01-22 17:24:55.859417 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/iam/action_groups.py
+-rw-r--r--   0        0        0   108710 2024-01-22 17:24:55.859750 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/iam/actions
+-rw-r--r--   0        0        0     4943 2024-01-22 17:24:55.859832 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/iam/base.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:31:56.831151 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/instrumentation/__init__.py
+-rw-r--r--   0        0        0     1376 2024-04-11 23:31:09.973506 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/instrumentation/alarms.py
+-rw-r--r--   0        0        0     5976 2024-04-24 21:59:03.929389 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/instrumentation/docker.py
+-rw-r--r--   0        0        0     7347 2024-04-25 19:01:22.356096 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/instrumentation/lambdas.py
+-rw-r--r--   0        0        0     1704 2024-04-11 23:31:09.974803 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/instrumentation/metrics.py
+-rw-r--r--   0        0        0     4435 2024-04-11 23:31:09.975272 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/instrumentation/queues.py
+-rw-r--r--   0        0        0     6551 2024-05-22 22:43:51.284271 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/lambdas.py
+-rw-r--r--   0        0        0      349 2024-02-28 20:32:26.259456 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/queue.py
+-rw-r--r--   0        0        0        0 2024-01-22 17:24:55.859986 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/sg/__init__.py
+-rw-r--r--   0        0        0     3481 2024-01-24 18:03:42.818220 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/sg/patterns.py
+-rw-r--r--   0        0        0      715 2024-01-24 18:03:42.818283 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/sg/ports.py
+-rw-r--r--   0        0        0      629 2024-01-22 17:24:55.860118 py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/sg/tier_maps.py
+-rw-r--r--   0        0        0      141 2024-01-24 18:03:42.818392 py_infraflow_cdk-0.1.9.9.1.4/infraflow/priv_utils/__init__.py
+-rw-r--r--   0        0        0      154 2024-01-22 17:24:55.860264 py_infraflow_cdk-0.1.9.9.1.4/infraflow/util.py
+-rw-r--r--   0        0        0      687 2024-05-22 22:43:51.284474 py_infraflow_cdk-0.1.9.9.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 py_infraflow_cdk-0.1.9.9.1.4/PKG-INFO
```

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/_step_functions/core.py` & `py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/_step_functions/core.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/_step_functions/patterns.py` & `py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/_step_functions/patterns.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/app_patterns/express_default_dlq_processor.py` & `py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/app_patterns/express_default_dlq_processor.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/app_patterns/standard.py` & `py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/app_patterns/standard.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/core/environment.py` & `py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/core/environment.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/core/service_stage.py` & `py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/core/service_stage.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/docker.py` & `py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/docker.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/events.py` & `py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/events.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/iam/_actions.py` & `py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/iam/_actions.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/iam/action_groups.py` & `py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/iam/action_groups.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/iam/actions` & `py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/iam/actions`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/iam/base.py` & `py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/iam/base.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/instrumentation/alarms.py` & `py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/instrumentation/alarms.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/instrumentation/docker.py` & `py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/instrumentation/docker.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/instrumentation/lambdas.py` & `py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/instrumentation/lambdas.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/instrumentation/metrics.py` & `py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/instrumentation/metrics.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/instrumentation/queues.py` & `py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/instrumentation/queues.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/lambdas.py` & `py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/lambdas.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from aws_cdk import aws_sqs
 from aws_cdk import aws_lambda_event_sources as sources
 from aws_cdk.aws_ec2 import SubnetType, SubnetSelection, Subnet
 from aws_cdk.aws_events import Rule, Schedule
 from aws_cdk.aws_events_targets import LambdaFunction
 from aws_cdk.aws_iam import IRole
 from aws_cdk.aws_lambda import IEventSource
+from aws_cdk.aws_s3_assets import AssetOptions
 from constructs import Construct, IConstruct
 
 from infraflow.cdk.core.service_stage import ServiceStageStack
 from infraflow.cdk.core.utils import to_duration
 from infraflow.cdk.iam import PolicyBuilder, action_groups
 from infraflow.cdk.instrumentation.queues import QueueInstrumentation
 from infraflow.cdk.sg.patterns import SecurityGroupTarget
@@ -64,15 +65,15 @@
             timeout: Union[datetime.timedelta, Duration, int]=datetime.timedelta(minutes=5)
     ):
         constructed_name = self.construct_name(handler, name, suffix)
         func = aws_lambda.Function(
                 id=constructed_name,
                 handler=handler,
                 scope=scope_override or self.stage,
-                code=aws_lambda.Code.from_asset(self.path, {'exclude': self.excluded_code}), ## TODO SH here we can have an exclude pattern
+                code=aws_lambda.Code.from_asset(path=self.path, options=AssetOptions(exclude=self.excluded_code)), ## TODO SH here we can have an exclude pattern
                 runtime=self.runtime,
                 reserved_concurrent_executions=max_concurrency,
                 timeout=to_duration(timeout),
                 security_groups=[
                     self.stage.security_groups.get_group(target=SecurityGroupTarget(
                         scope_override or self.stage,
                         id=constructed_name,
```

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/sg/patterns.py` & `py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/sg/patterns.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/sg/ports.py` & `py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/sg/ports.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/sg/tier_maps.py` & `py_infraflow_cdk-0.1.9.9.1.4/infraflow/cdk/sg/tier_maps.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/pyproject.toml` & `py_infraflow_cdk-0.1.9.9.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-infraflow-cdk"
-version = "0.1.9.9.1.3"
+version = "0.1.9.9.1.4"
 description = "Build Event Based and Microservice infrastructure and connections using these reusable AWS CDK patterns"
 authors = ["Matthew Beatty <infraflow@upcontent.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "infraflow"}]
 
 [tool.poetry.dependencies]
```

### Comparing `py_infraflow_cdk-0.1.9.9.1.3/PKG-INFO` & `py_infraflow_cdk-0.1.9.9.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-infraflow-cdk
-Version: 0.1.9.9.1.3
+Version: 0.1.9.9.1.4
 Summary: Build Event Based and Microservice infrastructure and connections using these reusable AWS CDK patterns
 License: MIT
 Author: Matthew Beatty
 Author-email: infraflow@upcontent.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

