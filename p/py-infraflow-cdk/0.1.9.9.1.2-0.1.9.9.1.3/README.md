# Comparing `tmp/py_infraflow_cdk-0.1.9.9.1.2.tar.gz` & `tmp/py_infraflow_cdk-0.1.9.9.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_infraflow_cdk-0.1.9.9.1.2.tar", max compression
+gzip compressed data, was "py_infraflow_cdk-0.1.9.9.1.3.tar", max compression
```

## Comparing `py_infraflow_cdk-0.1.9.9.1.2.tar` & `py_infraflow_cdk-0.1.9.9.1.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      337 2024-01-24 18:03:42.816211 py_infraflow_cdk-0.1.9.9.1.2/README.md
--rw-r--r--   0        0        0        0 2024-01-22 17:24:55.856613 py_infraflow_cdk-0.1.9.9.1.2/infraflow/__init__.py
--rw-r--r--   0        0        0      240 2024-01-22 17:24:55.856719 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/__init__.py
--rw-r--r--   0        0        0        0 2024-01-22 17:24:55.856794 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/_step_functions/__init__.py
--rw-r--r--   0        0        0     1329 2024-01-22 17:24:55.856883 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/_step_functions/core.py
--rw-r--r--   0        0        0     1261 2024-01-22 17:24:55.856942 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/_step_functions/patterns.py
--rw-r--r--   0        0        0      280 2024-01-22 17:24:55.857004 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/api_gateway.py
--rw-r--r--   0        0        0     7399 2024-05-10 16:34:36.118206 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/app_patterns/express_default_dlq_processor.py
--rw-r--r--   0        0        0    12703 2024-04-24 21:30:34.435023 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/app_patterns/standard.py
--rw-r--r--   0        0        0      156 2024-01-22 17:24:55.857163 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/arns.py
--rw-r--r--   0        0        0        0 2024-01-22 17:24:55.857224 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/core/__init__.py
--rw-r--r--   0        0        0      364 2024-01-22 17:24:55.857292 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/core/component_service.py
--rw-r--r--   0        0        0      316 2024-01-22 17:24:55.857349 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/core/construct.py
--rw-r--r--   0        0        0     5168 2024-03-20 16:31:56.831033 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/core/environment.py
--rw-r--r--   0        0        0     1020 2024-01-24 18:03:42.816662 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/core/service_stage.py
--rw-r--r--   0        0        0      367 2024-02-19 16:57:57.498391 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/core/utils.py
--rw-r--r--   0        0        0    10397 2024-05-08 20:06:25.481166 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/docker.py
--rw-r--r--   0        0        0     9235 2024-05-10 16:52:15.747978 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/events.py
--rw-r--r--   0        0        0      139 2024-01-22 17:24:55.857712 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/iam/__init__.py
--rw-r--r--   0        0        0   533095 2024-01-24 18:03:42.817968 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/iam/_actions.py
--rw-r--r--   0        0        0   249582 2024-01-22 17:24:55.859417 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/iam/action_groups.py
--rw-r--r--   0        0        0   108710 2024-01-22 17:24:55.859750 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/iam/actions
--rw-r--r--   0        0        0     4943 2024-01-22 17:24:55.859832 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/iam/base.py
--rw-r--r--   0        0        0        0 2024-03-20 16:31:56.831151 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/instrumentation/__init__.py
--rw-r--r--   0        0        0     1376 2024-04-11 23:31:09.973506 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/instrumentation/alarms.py
--rw-r--r--   0        0        0     5976 2024-04-24 21:59:03.929389 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/instrumentation/docker.py
--rw-r--r--   0        0        0     7347 2024-04-25 19:01:22.356096 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/instrumentation/lambdas.py
--rw-r--r--   0        0        0     1704 2024-04-11 23:31:09.974803 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/instrumentation/metrics.py
--rw-r--r--   0        0        0     4435 2024-04-11 23:31:09.975272 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/instrumentation/queues.py
--rw-r--r--   0        0        0     6252 2024-05-08 20:23:06.969174 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/lambdas.py
--rw-r--r--   0        0        0      349 2024-02-28 20:32:26.259456 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/queue.py
--rw-r--r--   0        0        0        0 2024-01-22 17:24:55.859986 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/sg/__init__.py
--rw-r--r--   0        0        0     3481 2024-01-24 18:03:42.818220 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/sg/patterns.py
--rw-r--r--   0        0        0      715 2024-01-24 18:03:42.818283 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/sg/ports.py
--rw-r--r--   0        0        0      629 2024-01-22 17:24:55.860118 py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/sg/tier_maps.py
--rw-r--r--   0        0        0      141 2024-01-24 18:03:42.818392 py_infraflow_cdk-0.1.9.9.1.2/infraflow/priv_utils/__init__.py
--rw-r--r--   0        0        0      154 2024-01-22 17:24:55.860264 py_infraflow_cdk-0.1.9.9.1.2/infraflow/util.py
--rw-r--r--   0        0        0      687 2024-05-10 16:52:22.531324 py_infraflow_cdk-0.1.9.9.1.2/pyproject.toml
--rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 py_infraflow_cdk-0.1.9.9.1.2/PKG-INFO
+-rw-r--r--   0        0        0      337 2024-01-24 18:03:42.816211 py_infraflow_cdk-0.1.9.9.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-01-22 17:24:55.856613 py_infraflow_cdk-0.1.9.9.1.3/infraflow/__init__.py
+-rw-r--r--   0        0        0      240 2024-01-22 17:24:55.856719 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-22 17:24:55.856794 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/_step_functions/__init__.py
+-rw-r--r--   0        0        0     1329 2024-01-22 17:24:55.856883 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/_step_functions/core.py
+-rw-r--r--   0        0        0     1261 2024-01-22 17:24:55.856942 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/_step_functions/patterns.py
+-rw-r--r--   0        0        0      280 2024-01-22 17:24:55.857004 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/api_gateway.py
+-rw-r--r--   0        0        0     7399 2024-05-22 22:22:01.944518 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/app_patterns/express_default_dlq_processor.py
+-rw-r--r--   0        0        0    12829 2024-05-22 22:26:07.349206 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/app_patterns/standard.py
+-rw-r--r--   0        0        0      156 2024-01-22 17:24:55.857163 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/arns.py
+-rw-r--r--   0        0        0        0 2024-01-22 17:24:55.857224 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/core/__init__.py
+-rw-r--r--   0        0        0      364 2024-01-22 17:24:55.857292 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/core/component_service.py
+-rw-r--r--   0        0        0      316 2024-01-22 17:24:55.857349 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/core/construct.py
+-rw-r--r--   0        0        0     5168 2024-03-20 16:31:56.831033 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/core/environment.py
+-rw-r--r--   0        0        0     1020 2024-01-24 18:03:42.816662 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/core/service_stage.py
+-rw-r--r--   0        0        0      367 2024-02-19 16:57:57.498391 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/core/utils.py
+-rw-r--r--   0        0        0    10397 2024-05-08 20:06:25.481166 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/docker.py
+-rw-r--r--   0        0        0     9235 2024-05-10 16:52:15.747978 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/events.py
+-rw-r--r--   0        0        0      139 2024-01-22 17:24:55.857712 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/iam/__init__.py
+-rw-r--r--   0        0        0   533095 2024-01-24 18:03:42.817968 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/iam/_actions.py
+-rw-r--r--   0        0        0   249582 2024-01-22 17:24:55.859417 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/iam/action_groups.py
+-rw-r--r--   0        0        0   108710 2024-01-22 17:24:55.859750 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/iam/actions
+-rw-r--r--   0        0        0     4943 2024-01-22 17:24:55.859832 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/iam/base.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:31:56.831151 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/instrumentation/__init__.py
+-rw-r--r--   0        0        0     1376 2024-04-11 23:31:09.973506 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/instrumentation/alarms.py
+-rw-r--r--   0        0        0     5976 2024-04-24 21:59:03.929389 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/instrumentation/docker.py
+-rw-r--r--   0        0        0     7347 2024-04-25 19:01:22.356096 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/instrumentation/lambdas.py
+-rw-r--r--   0        0        0     1704 2024-04-11 23:31:09.974803 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/instrumentation/metrics.py
+-rw-r--r--   0        0        0     4435 2024-04-11 23:31:09.975272 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/instrumentation/queues.py
+-rw-r--r--   0        0        0     6482 2024-05-22 22:26:07.349492 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/lambdas.py
+-rw-r--r--   0        0        0      349 2024-02-28 20:32:26.259456 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/queue.py
+-rw-r--r--   0        0        0        0 2024-01-22 17:24:55.859986 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/sg/__init__.py
+-rw-r--r--   0        0        0     3481 2024-01-24 18:03:42.818220 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/sg/patterns.py
+-rw-r--r--   0        0        0      715 2024-01-24 18:03:42.818283 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/sg/ports.py
+-rw-r--r--   0        0        0      629 2024-01-22 17:24:55.860118 py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/sg/tier_maps.py
+-rw-r--r--   0        0        0      141 2024-01-24 18:03:42.818392 py_infraflow_cdk-0.1.9.9.1.3/infraflow/priv_utils/__init__.py
+-rw-r--r--   0        0        0      154 2024-01-22 17:24:55.860264 py_infraflow_cdk-0.1.9.9.1.3/infraflow/util.py
+-rw-r--r--   0        0        0      687 2024-05-22 22:26:07.349713 py_infraflow_cdk-0.1.9.9.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 py_infraflow_cdk-0.1.9.9.1.3/PKG-INFO
```

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/_step_functions/core.py` & `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/_step_functions/core.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/_step_functions/patterns.py` & `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/_step_functions/patterns.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/app_patterns/express_default_dlq_processor.py` & `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/app_patterns/express_default_dlq_processor.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/app_patterns/standard.py` & `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/app_patterns/standard.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,26 +29,28 @@
     # noinspection PyDefaultArgument
     def __init__(self,
                  app: App,
                  service_name: str,
                  stage_name: str,
                  env: EnvConfig,
                  src_path: str = "src",
+                 excluded_code=None,
                  db_ports=[],
                  python_version: aws_lambda.Runtime = aws_lambda.Runtime.PYTHON_3_9,
                  vpc_endpoint_services: list[InterfaceVpcEndpointAwsService] = DEFAULT_INTERFACE_SERVICES,
                  **kwargs):
         super().__init__(app, service_name, stage_name, env, **kwargs)
         self.db_ports = db_ports
         self.vpc_endpoint_services = vpc_endpoint_services
         self._ecs_execution_role = None
         self._app_role = None
         self._event_publish_policy = None
         self.python_version = python_version
         self.src_path = src_path
+        self.excluded_code = excluded_code
         self._lambda_context: Optional[LambdaContext] = None
         self._api: Optional[apigateway.IRestApi] = None
         self._event_bridge_bus_cdk: Optional[aws_events.IEventBus] = None
         self._events: Optional[EventBridgeEvents] = None
         self._ecs_cluster: Optional[EcsCluster] = None
         self._sns_bus_cdk: Optional[aws_sns.Topic] = None
         self.security_groups: Tiered = Tiered(self, db_ports=db_ports)
@@ -108,15 +110,16 @@
             self.managed_policy("LambdaAllowENIManagement", name="AWSLambdaENIManagementAccess")
         )
 
         self._lambda_context = self._lambda_context or LambdaContext(
             self,
             path=self.src_path,
             role=self.app_role,
-            runtime=self.python_version
+            runtime=self.python_version,
+            excluded_code=self.excluded_code
         )
 
     def managed_policy(self, id, *, arn=None, name=None):
         if not arn:
             arn = f"arn:aws:iam::aws:policy/service-role/{name}"
         self._managed_policies[id] = self._managed_policies.get(id) or ManagedPolicy.from_managed_policy_arn(
             scope=self,
```

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/core/environment.py` & `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/core/environment.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/core/service_stage.py` & `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/core/service_stage.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/docker.py` & `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/docker.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/events.py` & `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/events.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/iam/_actions.py` & `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/iam/_actions.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/iam/action_groups.py` & `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/iam/action_groups.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/iam/actions` & `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/iam/actions`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/iam/base.py` & `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/iam/base.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/instrumentation/alarms.py` & `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/instrumentation/alarms.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/instrumentation/docker.py` & `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/instrumentation/docker.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/instrumentation/lambdas.py` & `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/instrumentation/lambdas.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/instrumentation/metrics.py` & `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/instrumentation/metrics.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/instrumentation/queues.py` & `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/instrumentation/queues.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/lambdas.py` & `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/lambdas.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,28 +26,30 @@
     def __init__(self,
                  stage: ServiceStageStack,
                  path: str,
                  role: IRole = None,
                  runtime: aws_lambda.Runtime = aws_lambda.Runtime.PYTHON_3_9,
                  vpc: bool = True,
                  subnet_type: SubnetType = SubnetType.PRIVATE_WITH_EGRESS,
-                 tracing=aws_lambda.Tracing.ACTIVE
+                 tracing=aws_lambda.Tracing.ACTIVE,
+                 excluded_code=None
                  ):
         self.vpc = vpc
         self.tracing = tracing
         self.subnet_type = subnet_type
         self.role = role
         self.runtime = runtime
         self.path = path
         self.stage = stage
         self.default_sg = stage.default_sg
         self.queues: list[aws_sqs.Queue] = []
         self.functions: list[aws_lambda.Function] = []
         self.queue_instrumentation: dict[aws_sqs.Queue, QueueInstrumentation] = {}
         self.lambda_instrumentation: dict[aws_lambda.Function, LambdaInstrumentation] = {}
+        self.excluded_code = excluded_code
 
     # def to_cdk(self):
     #     return dict(
     #         scope=self.scope,
     #         code=aws_lambda.Code.from_asset(self.path),
     #         runtime=self.runtime
     #     )
@@ -62,15 +64,15 @@
             timeout: Union[datetime.timedelta, Duration, int]=datetime.timedelta(minutes=5)
     ):
         constructed_name = self.construct_name(handler, name, suffix)
         func = aws_lambda.Function(
                 id=constructed_name,
                 handler=handler,
                 scope=scope_override or self.stage,
-                code=aws_lambda.Code.from_asset(self.path),
+                code=aws_lambda.Code.from_asset(self.path, {'exclude': self.excluded_code}), ## TODO SH here we can have an exclude pattern
                 runtime=self.runtime,
                 reserved_concurrent_executions=max_concurrency,
                 timeout=to_duration(timeout),
                 security_groups=[
                     self.stage.security_groups.get_group(target=SecurityGroupTarget(
                         scope_override or self.stage,
                         id=constructed_name,
@@ -105,15 +107,21 @@
             timeout: Union[datetime.timedelta, Duration, int]=datetime.timedelta(minutes=5),
             **queue_config
     ):
         constructed_name = self.construct_name(handler, name, suffix)
         queued_function = QueueFunctionConstruct(self.stage, constructed_name)
         queue = aws_sqs.Queue(queued_function, 'Queue', visibility_timeout=to_duration(timeout), **queue_config)
         self.queue_instrumentation[queue] = QueueInstrumentation(queue)
-        func = self.function(handler, 'Function', scope_override=queued_function, max_concurrency=max_concurrency, timeout=timeout)
+        func = self.function(
+            handler,
+            'Function',
+            scope_override=queued_function,
+            max_concurrency=max_concurrency,
+            timeout=timeout
+        )
         func.add_event_source(sources.SqsEventSource(queue, batch_size=batch_size))
         queued_function.queue = queue
         queued_function.function = func
         return queued_function
 
     def scheduled_function(self, handler, schedule: Union[Schedule, Duration, datetime.timedelta], name=None, suffix=None):
         schedule = Duration.seconds(schedule.total_seconds()) if isinstance(schedule, datetime.timedelta) else None
```

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/sg/patterns.py` & `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/sg/patterns.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/sg/ports.py` & `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/sg/ports.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/infraflow/cdk/sg/tier_maps.py` & `py_infraflow_cdk-0.1.9.9.1.3/infraflow/cdk/sg/tier_maps.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/pyproject.toml` & `py_infraflow_cdk-0.1.9.9.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-infraflow-cdk"
-version = "0.1.9.9.1.2"
+version = "0.1.9.9.1.3"
 description = "Build Event Based and Microservice infrastructure and connections using these reusable AWS CDK patterns"
 authors = ["Matthew Beatty <infraflow@upcontent.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "infraflow"}]
 
 [tool.poetry.dependencies]
```

### Comparing `py_infraflow_cdk-0.1.9.9.1.2/PKG-INFO` & `py_infraflow_cdk-0.1.9.9.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-infraflow-cdk
-Version: 0.1.9.9.1.2
+Version: 0.1.9.9.1.3
 Summary: Build Event Based and Microservice infrastructure and connections using these reusable AWS CDK patterns
 License: MIT
 Author: Matthew Beatty
 Author-email: infraflow@upcontent.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

