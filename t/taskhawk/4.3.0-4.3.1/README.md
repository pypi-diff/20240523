# Comparing `tmp/taskhawk-4.3.0.tar.gz` & `tmp/taskhawk-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskhawk-4.3.0.tar", last modified: Wed Jul  5 18:36:58 2023, max compression
+gzip compressed data, was "taskhawk-4.3.1.tar", last modified: Thu May 23 17:54:16 2024, max compression
```

## Comparing `taskhawk-4.3.0.tar` & `taskhawk-4.3.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-05 18:36:58.789808 taskhawk-4.3.0/
--rw-r--r--   0 maru       (501) staff       (20)      348 2020-03-12 19:54:19.000000 taskhawk-4.3.0/CONTRIBUTORS.txt
--rw-r--r--   0 maru       (501) staff       (20)    11342 2021-07-30 00:29:32.000000 taskhawk-4.3.0/LICENSE.md
--rw-r--r--   0 maru       (501) staff       (20)      162 2020-03-12 19:54:19.000000 taskhawk-4.3.0/MANIFEST.in
--rw-r--r--   0 maru       (501) staff       (20)     5395 2023-07-05 18:36:58.789857 taskhawk-4.3.0/PKG-INFO
--rw-r--r--   0 maru       (501) staff       (20)     4432 2021-07-30 00:29:32.000000 taskhawk-4.3.0/README.rst
--rw-r--r--   0 maru       (501) staff       (20)      244 2020-03-12 19:54:19.000000 taskhawk-4.3.0/pyproject.toml
--rw-r--r--   0 maru       (501) staff       (20)      316 2023-07-05 18:36:58.790067 taskhawk-4.3.0/setup.cfg
--rw-r--r--   0 maru       (501) staff       (20)     3197 2022-11-29 05:20:56.000000 taskhawk-4.3.0/setup.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-05 18:36:58.785872 taskhawk-4.3.0/taskhawk/
--rw-r--r--   0 maru       (501) staff       (20)      632 2023-07-05 18:36:57.000000 taskhawk-4.3.0/taskhawk/__init__.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-05 18:36:58.787693 taskhawk-4.3.0/taskhawk/backends/
--rw-r--r--   0 maru       (501) staff       (20)        0 2020-03-12 19:54:19.000000 taskhawk-4.3.0/taskhawk/backends/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)     9886 2023-06-03 00:08:40.000000 taskhawk-4.3.0/taskhawk/backends/aws.py
--rw-r--r--   0 maru       (501) staff       (20)     6936 2023-07-05 18:34:53.000000 taskhawk-4.3.0/taskhawk/backends/base.py
--rw-r--r--   0 maru       (501) staff       (20)      343 2020-03-12 19:54:19.000000 taskhawk-4.3.0/taskhawk/backends/exceptions.py
--rw-r--r--   0 maru       (501) staff       (20)    11745 2023-07-05 18:34:53.000000 taskhawk-4.3.0/taskhawk/backends/gcp.py
--rw-r--r--   0 maru       (501) staff       (20)      567 2020-03-12 19:54:19.000000 taskhawk-4.3.0/taskhawk/backends/import_utils.py
--rw-r--r--   0 maru       (501) staff       (20)     1121 2020-03-12 19:54:19.000000 taskhawk-4.3.0/taskhawk/backends/utils.py
--rw-r--r--   0 maru       (501) staff       (20)      809 2022-11-29 05:20:56.000000 taskhawk-4.3.0/taskhawk/commands.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-05 18:36:58.787853 taskhawk-4.3.0/taskhawk/conf/
--rw-r--r--   0 maru       (501) staff       (20)     7020 2023-07-05 18:34:53.000000 taskhawk-4.3.0/taskhawk/conf/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)     2983 2022-11-29 05:20:56.000000 taskhawk-4.3.0/taskhawk/consumer.py
--rw-r--r--   0 maru       (501) staff       (20)      980 2022-11-28 19:50:36.000000 taskhawk-4.3.0/taskhawk/exceptions.py
--rw-r--r--   0 maru       (501) staff       (20)     9359 2022-11-29 05:20:56.000000 taskhawk-4.3.0/taskhawk/models.py
--rw-r--r--   0 maru       (501) staff       (20)      525 2022-11-29 05:20:56.000000 taskhawk-4.3.0/taskhawk/publisher.py
--rw-r--r--   0 maru       (501) staff       (20)     7975 2022-04-13 05:43:22.000000 taskhawk-4.3.0/taskhawk/task_manager.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-05 18:36:58.786511 taskhawk-4.3.0/taskhawk.egg-info/
--rw-r--r--   0 maru       (501) staff       (20)     5395 2023-07-05 18:36:58.000000 taskhawk-4.3.0/taskhawk.egg-info/PKG-INFO
--rw-r--r--   0 maru       (501) staff       (20)      959 2023-07-05 18:36:58.000000 taskhawk-4.3.0/taskhawk.egg-info/SOURCES.txt
--rw-r--r--   0 maru       (501) staff       (20)        1 2023-07-05 18:36:58.000000 taskhawk-4.3.0/taskhawk.egg-info/dependency_links.txt
--rw-r--r--   0 maru       (501) staff       (20)      478 2023-07-05 18:36:58.000000 taskhawk-4.3.0/taskhawk.egg-info/requires.txt
--rw-r--r--   0 maru       (501) staff       (20)        9 2023-07-05 18:36:58.000000 taskhawk-4.3.0/taskhawk.egg-info/top_level.txt
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-05 18:36:58.789197 taskhawk-4.3.0/tests/
--rw-r--r--   0 maru       (501) staff       (20)        0 2020-03-12 19:54:19.000000 taskhawk-4.3.0/tests/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)     4363 2022-11-29 05:20:56.000000 taskhawk-4.3.0/tests/conftest.py
--rw-r--r--   0 maru       (501) staff       (20)      201 2020-03-12 19:54:19.000000 taskhawk-4.3.0/tests/settings.py
--rw-r--r--   0 maru       (501) staff       (20)      661 2021-07-06 19:19:15.000000 taskhawk-4.3.0/tests/tasks.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-05 18:36:58.789689 taskhawk-4.3.0/tests/test_backends/
--rw-r--r--   0 maru       (501) staff       (20)        0 2020-03-12 19:54:19.000000 taskhawk-4.3.0/tests/test_backends/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)    12649 2020-03-12 19:54:19.000000 taskhawk-4.3.0/tests/test_backends/test_aws.py
--rw-r--r--   0 maru       (501) staff       (20)    10558 2021-07-06 19:19:15.000000 taskhawk-4.3.0/tests/test_backends/test_base.py
--rw-r--r--   0 maru       (501) staff       (20)    13090 2023-07-05 18:34:53.000000 taskhawk-4.3.0/tests/test_backends/test_gcp.py
--rw-r--r--   0 maru       (501) staff       (20)      481 2020-03-12 19:54:19.000000 taskhawk-4.3.0/tests/test_commands.py
--rw-r--r--   0 maru       (501) staff       (20)     1101 2022-11-28 19:50:36.000000 taskhawk-4.3.0/tests/test_consumer.py
--rw-r--r--   0 maru       (501) staff       (20)     5851 2020-03-12 19:54:19.000000 taskhawk-4.3.0/tests/test_models.py
--rw-r--r--   0 maru       (501) staff       (20)      383 2020-03-12 19:54:19.000000 taskhawk-4.3.0/tests/test_publisher.py
--rw-r--r--   0 maru       (501) staff       (20)      607 2020-03-12 19:54:19.000000 taskhawk-4.3.0/tests/test_settings.py
--rw-r--r--   0 maru       (501) staff       (20)     8474 2020-03-12 19:54:19.000000 taskhawk-4.3.0/tests/test_task_manager.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2024-05-23 17:54:16.367785 taskhawk-4.3.1/
+-rw-r--r--   0 maru       (501) staff       (20)      348 2020-03-12 19:54:19.000000 taskhawk-4.3.1/CONTRIBUTORS.txt
+-rw-r--r--   0 maru       (501) staff       (20)    11342 2021-07-30 00:29:32.000000 taskhawk-4.3.1/LICENSE.md
+-rw-r--r--   0 maru       (501) staff       (20)      162 2020-03-12 19:54:19.000000 taskhawk-4.3.1/MANIFEST.in
+-rw-r--r--   0 maru       (501) staff       (20)     5395 2024-05-23 17:54:16.367850 taskhawk-4.3.1/PKG-INFO
+-rw-r--r--   0 maru       (501) staff       (20)     4432 2021-07-30 00:29:32.000000 taskhawk-4.3.1/README.rst
+-rw-r--r--   0 maru       (501) staff       (20)      244 2020-03-12 19:54:19.000000 taskhawk-4.3.1/pyproject.toml
+-rw-r--r--   0 maru       (501) staff       (20)      316 2024-05-23 17:54:16.368078 taskhawk-4.3.1/setup.cfg
+-rw-r--r--   0 maru       (501) staff       (20)     3197 2022-11-29 05:20:56.000000 taskhawk-4.3.1/setup.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2024-05-23 17:54:16.364260 taskhawk-4.3.1/taskhawk/
+-rw-r--r--   0 maru       (501) staff       (20)      632 2024-05-23 17:54:12.000000 taskhawk-4.3.1/taskhawk/__init__.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2024-05-23 17:54:16.365879 taskhawk-4.3.1/taskhawk/backends/
+-rw-r--r--   0 maru       (501) staff       (20)        0 2020-03-12 19:54:19.000000 taskhawk-4.3.1/taskhawk/backends/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)    10178 2024-05-23 17:53:16.000000 taskhawk-4.3.1/taskhawk/backends/aws.py
+-rw-r--r--   0 maru       (501) staff       (20)     7169 2024-05-23 17:53:16.000000 taskhawk-4.3.1/taskhawk/backends/base.py
+-rw-r--r--   0 maru       (501) staff       (20)      343 2020-03-12 19:54:19.000000 taskhawk-4.3.1/taskhawk/backends/exceptions.py
+-rw-r--r--   0 maru       (501) staff       (20)    12165 2024-05-23 17:53:16.000000 taskhawk-4.3.1/taskhawk/backends/gcp.py
+-rw-r--r--   0 maru       (501) staff       (20)      567 2020-03-12 19:54:19.000000 taskhawk-4.3.1/taskhawk/backends/import_utils.py
+-rw-r--r--   0 maru       (501) staff       (20)     1121 2020-03-12 19:54:19.000000 taskhawk-4.3.1/taskhawk/backends/utils.py
+-rw-r--r--   0 maru       (501) staff       (20)      809 2022-11-29 05:20:56.000000 taskhawk-4.3.1/taskhawk/commands.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2024-05-23 17:54:16.366016 taskhawk-4.3.1/taskhawk/conf/
+-rw-r--r--   0 maru       (501) staff       (20)     7020 2023-07-05 18:34:53.000000 taskhawk-4.3.1/taskhawk/conf/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)     2983 2022-11-29 05:20:56.000000 taskhawk-4.3.1/taskhawk/consumer.py
+-rw-r--r--   0 maru       (501) staff       (20)      980 2022-11-28 19:50:36.000000 taskhawk-4.3.1/taskhawk/exceptions.py
+-rw-r--r--   0 maru       (501) staff       (20)     9359 2022-11-29 05:20:56.000000 taskhawk-4.3.1/taskhawk/models.py
+-rw-r--r--   0 maru       (501) staff       (20)      525 2022-11-29 05:20:56.000000 taskhawk-4.3.1/taskhawk/publisher.py
+-rw-r--r--   0 maru       (501) staff       (20)     8126 2023-08-03 23:02:56.000000 taskhawk-4.3.1/taskhawk/task_manager.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2024-05-23 17:54:16.364974 taskhawk-4.3.1/taskhawk.egg-info/
+-rw-r--r--   0 maru       (501) staff       (20)     5395 2024-05-23 17:54:16.000000 taskhawk-4.3.1/taskhawk.egg-info/PKG-INFO
+-rw-r--r--   0 maru       (501) staff       (20)      959 2024-05-23 17:54:16.000000 taskhawk-4.3.1/taskhawk.egg-info/SOURCES.txt
+-rw-r--r--   0 maru       (501) staff       (20)        1 2024-05-23 17:54:16.000000 taskhawk-4.3.1/taskhawk.egg-info/dependency_links.txt
+-rw-r--r--   0 maru       (501) staff       (20)      478 2024-05-23 17:54:16.000000 taskhawk-4.3.1/taskhawk.egg-info/requires.txt
+-rw-r--r--   0 maru       (501) staff       (20)        9 2024-05-23 17:54:16.000000 taskhawk-4.3.1/taskhawk.egg-info/top_level.txt
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2024-05-23 17:54:16.367244 taskhawk-4.3.1/tests/
+-rw-r--r--   0 maru       (501) staff       (20)        0 2020-03-12 19:54:19.000000 taskhawk-4.3.1/tests/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)     4363 2022-11-29 05:20:56.000000 taskhawk-4.3.1/tests/conftest.py
+-rw-r--r--   0 maru       (501) staff       (20)      201 2020-03-12 19:54:19.000000 taskhawk-4.3.1/tests/settings.py
+-rw-r--r--   0 maru       (501) staff       (20)      661 2021-07-06 19:19:15.000000 taskhawk-4.3.1/tests/tasks.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2024-05-23 17:54:16.367675 taskhawk-4.3.1/tests/test_backends/
+-rw-r--r--   0 maru       (501) staff       (20)        0 2020-03-12 19:54:19.000000 taskhawk-4.3.1/tests/test_backends/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)    12649 2020-03-12 19:54:19.000000 taskhawk-4.3.1/tests/test_backends/test_aws.py
+-rw-r--r--   0 maru       (501) staff       (20)    10725 2024-05-23 17:53:16.000000 taskhawk-4.3.1/tests/test_backends/test_base.py
+-rw-r--r--   0 maru       (501) staff       (20)    13090 2023-07-05 18:34:53.000000 taskhawk-4.3.1/tests/test_backends/test_gcp.py
+-rw-r--r--   0 maru       (501) staff       (20)      481 2020-03-12 19:54:19.000000 taskhawk-4.3.1/tests/test_commands.py
+-rw-r--r--   0 maru       (501) staff       (20)     1101 2022-11-28 19:50:36.000000 taskhawk-4.3.1/tests/test_consumer.py
+-rw-r--r--   0 maru       (501) staff       (20)     5851 2020-03-12 19:54:19.000000 taskhawk-4.3.1/tests/test_models.py
+-rw-r--r--   0 maru       (501) staff       (20)      383 2020-03-12 19:54:19.000000 taskhawk-4.3.1/tests/test_publisher.py
+-rw-r--r--   0 maru       (501) staff       (20)      607 2020-03-12 19:54:19.000000 taskhawk-4.3.1/tests/test_settings.py
+-rw-r--r--   0 maru       (501) staff       (20)     8773 2023-08-03 22:59:53.000000 taskhawk-4.3.1/tests/test_task_manager.py
```

### Comparing `taskhawk-4.3.0/LICENSE.md` & `taskhawk-4.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `taskhawk-4.3.0/PKG-INFO` & `taskhawk-4.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskhawk
-Version: 4.3.0
+Version: 4.3.1
 Summary: Taskhawk Python Library
 Home-page: https://github.com/cloudchacho/taskhawk-python
 Author: Automatic Labs
 Maintainer: Aniruddha Maru
 Maintainer-email: aniruddhamaru@gmail.com
 License: Apache Software License (Apache License 2.0)
 Keywords: python taskhawk
```

### Comparing `taskhawk-4.3.0/README.rst` & `taskhawk-4.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `taskhawk-4.3.0/setup.py` & `taskhawk-4.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.3.0/taskhawk/__init__.py` & `taskhawk-4.3.1/taskhawk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ~~~~~~~~
 
 :copyright: (c) 2013-2017 by the Automatic Labs.
 """
 
 
 # semantic versioning (http://semver.org/)
-VERSION = '4.3.0'
+VERSION = '4.3.1'
 
 
 try:
     from .backends.aws import AWSMetadata  # noqa
 except ImportError:
     pass
 try:
```

### Comparing `taskhawk-4.3.0/taskhawk/backends/aws.py` & `taskhawk-4.3.1/taskhawk/backends/aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,18 @@
         message_json = queue_message.body
         receipt = queue_message.receipt_handle
         self.message_handler(message_json, AWSMetadata(receipt))
 
     def delete_message(self, queue_message) -> None:
         queue_message.delete()
 
+    def nack_message(self, queue_message) -> None:
+        # should operate like a nack https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/sqs-visibility-timeout.html#terminating-message-visibility-timeout
+        queue_message.change_visibility(VisibilityTimeout=0)
+
     def extend_visibility_timeout(self, visibility_timeout_s: int, metadata: AWSMetadata) -> None:
         """
         Extends visibility timeout of a message on a given priority queue for long running tasks.
         """
         receipt = metadata.receipt
         queue_url = self.sqs_client.get_queue_url(QueueName=self.queue_name)['QueueUrl']
         self.sqs_client.change_message_visibility(
```

### Comparing `taskhawk-4.3.0/taskhawk/backends/base.py` & `taskhawk-4.3.1/taskhawk/backends/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,21 +103,24 @@
             try:
                 self.process_message(queue_message)
             except IgnoreException:
                 logger.info('Ignoring task', extra={'queue_message': queue_message})
             except LoggingException as e:
                 # log with message and extra
                 logger.exception(str(e), extra=e.extra)
+                self.nack_message(queue_message)
                 continue
             except RetryException:
                 # Retry without logging exception
                 logger.info('Retrying due to exception')
+                self.nack_message(queue_message)
                 continue
             except Exception:
                 logger.exception('Exception while processing message')
+                self.nack_message(queue_message)
                 continue
 
             try:
                 settings.TASKHAWK_POST_PROCESS_HOOK(**self.post_process_hook_kwargs(queue_message))
             except Exception:
                 logger.exception('Exception in post process hook for message', extra={'queue_message': queue_message})
                 continue
@@ -154,14 +157,17 @@
     def process_messages(self, lambda_event) -> None:
         # for lambda backend
         raise NotImplementedError
 
     def delete_message(self, queue_message) -> None:
         raise NotImplementedError
 
+    def nack_message(self, queue_message) -> None:
+        raise NotImplementedError
+
     @staticmethod
     def _build_message(message_json: str, provider_metadata) -> Message:
         try:
             message = Message(json.loads(message_json))
             message.metadata.provider_metadata = provider_metadata
             return message
         except (ValidationError, ValueError):
```

### Comparing `taskhawk-4.3.0/taskhawk/backends/gcp.py` & `taskhawk-4.3.1/taskhawk/backends/gcp.py`

 * *Files 3% similar despite different names*

```diff
@@ -224,14 +224,21 @@
             queue_message.message.data.decode(),
             GoogleMetadata(queue_message.ack_id, queue_message.message.publish_time, queue_message.delivery_attempt),
         )
 
     def delete_message(self, queue_message: ReceivedMessage) -> None:
         self.subscriber.acknowledge(subscription=self._subscription_path, ack_ids=[queue_message.ack_id])
 
+    def nack_message(self, queue_message: ReceivedMessage) -> None:
+        # https://cloud.google.com/pubsub/docs/reference/rest/v1/projects.subscriptions/pull#receivedmessage
+        # A NACK is any call to subscriptions.modifyAckDeadline with a 0 deadline
+        self.subscriber.modify_ack_deadline(
+            subscription=self._subscription_path, ack_ids=[queue_message.ack_id], ack_deadline_seconds=0
+        )
+
     @staticmethod
     def pre_process_hook_kwargs(queue_message: ReceivedMessage) -> dict:
         return {'google_pubsub_message': queue_message}
 
     @staticmethod
     def post_process_hook_kwargs(queue_message: ReceivedMessage) -> dict:
         return {'google_pubsub_message': queue_message}
```

### Comparing `taskhawk-4.3.0/taskhawk/backends/import_utils.py` & `taskhawk-4.3.1/taskhawk/backends/import_utils.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.3.0/taskhawk/backends/utils.py` & `taskhawk-4.3.1/taskhawk/backends/utils.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.3.0/taskhawk/commands.py` & `taskhawk-4.3.1/taskhawk/commands.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.3.0/taskhawk/conf/__init__.py` & `taskhawk-4.3.1/taskhawk/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.3.0/taskhawk/consumer.py` & `taskhawk-4.3.1/taskhawk/consumer.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.3.0/taskhawk/exceptions.py` & `taskhawk-4.3.1/taskhawk/exceptions.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.3.0/taskhawk/models.py` & `taskhawk-4.3.1/taskhawk/models.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.3.0/taskhawk/publisher.py` & `taskhawk-4.3.1/taskhawk/publisher.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.3.0/taskhawk/task_manager.py` & `taskhawk-4.3.1/taskhawk/task_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import copy
 import inspect
 import typing
 from concurrent.futures import Future
+from typing import Optional
 
 from taskhawk.conf import settings
 from taskhawk.exceptions import ConfigurationError, TaskNotFound
 from taskhawk.models import Metadata, Message, Priority
 from taskhawk.publisher import publish
 
 
@@ -132,15 +133,19 @@
             # if **kwargs is specified, just pass all things by default since function can always inspect arg names
             if p.kind == inspect.Parameter.VAR_KEYWORD:
                 self._accepts_metadata = self._accepts_headers = True
             elif p.kind == inspect.Parameter.VAR_POSITIONAL:
                 # disallow use of *args
                 raise ConfigurationError("Use of *args is not allowed")
             elif p.name == "metadata":
-                if p.annotation is not inspect.Signature.empty and p.annotation is not Metadata:
+                if (
+                    p.annotation is not inspect.Signature.empty
+                    and p.annotation is not Metadata
+                    and p.annotation is not Optional[Metadata]
+                ):
                     raise ConfigurationError(f"Signature for 'metadata' param must be Metadata, not {p.annotation}")
                 self._accepts_metadata = True
             elif p.name == "headers":
                 if p.annotation is not inspect.Signature.empty and p.annotation is not dict:
                     raise ConfigurationError("Signature for 'headers' param must be dict")
                 self._accepts_headers = True
```

### Comparing `taskhawk-4.3.0/taskhawk.egg-info/PKG-INFO` & `taskhawk-4.3.1/taskhawk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskhawk
-Version: 4.3.0
+Version: 4.3.1
 Summary: Taskhawk Python Library
 Home-page: https://github.com/cloudchacho/taskhawk-python
 Author: Automatic Labs
 Maintainer: Aniruddha Maru
 Maintainer-email: aniruddhamaru@gmail.com
 License: Apache Software License (Apache License 2.0)
 Keywords: python taskhawk
```

### Comparing `taskhawk-4.3.0/taskhawk.egg-info/SOURCES.txt` & `taskhawk-4.3.1/taskhawk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taskhawk-4.3.0/tests/conftest.py` & `taskhawk-4.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.3.0/tests/tasks.py` & `taskhawk-4.3.1/tests/tasks.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.3.0/tests/test_backends/test_aws.py` & `taskhawk-4.3.1/tests/test_backends/test_aws.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.3.0/tests/test_backends/test_base.py` & `taskhawk-4.3.1/tests/test_backends/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,18 +90,20 @@
         )
 
     def test_preserves_messages(self, consumer_backend):
         consumer_backend.pull_messages = mock.MagicMock()
         consumer_backend.pull_messages.return_value = [mock.MagicMock()]
         consumer_backend.process_message = mock.MagicMock()
         consumer_backend.process_message.side_effect = Exception
+        consumer_backend.nack_message = mock.MagicMock()
 
         consumer_backend.fetch_and_process_messages()
 
         consumer_backend.pull_messages.return_value[0].delete.assert_not_called()
+        consumer_backend.nack_message.assert_called_once_with(consumer_backend.pull_messages.return_value[0])
 
     def test_ignore_delete_error(self, consumer_backend):
         queue_message = mock.MagicMock()
         consumer_backend.pull_messages = mock.MagicMock(return_value=[queue_message])
         consumer_backend.process_message = mock.MagicMock()
         consumer_backend.delete_message = mock.MagicMock(side_effect=Exception)
```

### Comparing `taskhawk-4.3.0/tests/test_backends/test_gcp.py` & `taskhawk-4.3.1/tests/test_backends/test_gcp.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.3.0/tests/test_consumer.py` & `taskhawk-4.3.1/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.3.0/tests/test_models.py` & `taskhawk-4.3.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.3.0/tests/test_settings.py` & `taskhawk-4.3.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.3.0/tests/test_task_manager.py` & `taskhawk-4.3.1/tests/test_task_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from typing import Optional
 from unittest import mock
 import uuid
 
 import pytest
 
+import taskhawk
 from taskhawk.task_manager import _ALL_TASKS, Task, task, AsyncInvocation
 from taskhawk.models import Priority
 from taskhawk.exceptions import ConfigurationError, TaskNotFound
 from .tasks import send_email
 
 
 def test_task_decorator():
@@ -144,14 +146,18 @@
         pass
 
     @staticmethod
     def f_args(a, b, *args, **kwargs):
         pass
 
     @staticmethod
+    def f_valid_annotation(a, b, metadata: Optional[taskhawk.Metadata] = None):
+        pass
+
+    @staticmethod
     def f_invalid_annotation(a, b, metadata: int):
         pass
 
     @staticmethod
     def f_invalid_annotation2(a, b, headers: int):
         pass
 
@@ -179,14 +185,18 @@
         assert task_obj._accepts_metadata is True
         assert task_obj._accepts_headers is True
 
     def test_constructor_disallow_args(self):
         with pytest.raises(ConfigurationError):
             Task(TestTask.f_args, Priority.default, 'name')
 
+    def test_constructor_good_annotation(self):
+        # shouldn't raise
+        Task(TestTask.f_valid_annotation, Priority.default, 'name')
+
     def test_constructor_bad_annotation(self):
         with pytest.raises(ConfigurationError):
             Task(TestTask.f_invalid_annotation, Priority.default, 'name')
 
     def test_constructor_bad_annotation2(self):
         with pytest.raises(ConfigurationError):
             Task(TestTask.f_invalid_annotation2, Priority.default, 'name')
```

