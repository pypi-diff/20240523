# Comparing `tmp/haondt_charon-1.1.0.tar.gz` & `tmp/haondt_charon-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haondt_charon-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "haondt_charon-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `haondt_charon-1.1.0.tar` & `haondt_charon-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       45 2024-05-19 15:19:09.288336 haondt_charon-1.1.0/.gitignore
--rw-r--r--   0        0        0      169 2024-04-29 01:45:23.302231 haondt_charon-1.1.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      206 2024-05-03 22:30:54.865617 haondt_charon-1.1.0/Dockerfile
--rw-r--r--   0        0        0     1081 2024-04-29 01:45:23.302231 haondt_charon-1.1.0/LICENSE
--rw-r--r--   0        0        0     5755 2024-05-03 22:30:54.865617 haondt_charon-1.1.0/README.md
--rw-r--r--   0        0        0     1054 2024-04-29 01:45:23.302231 haondt_charon-1.1.0/charon.yml
--rw-r--r--   0        0        0        0 2024-05-19 15:19:09.352337 haondt_charon-1.1.0/charon/__init__.py
--rw-r--r--   0        0        0     1395 2024-04-29 01:45:23.302231 haondt_charon-1.1.0/charon/__main__.py
--rw-r--r--   0        0        0       45 2024-04-29 01:45:23.302231 haondt_charon-1.1.0/charon/destinations/__init__.py
--rw-r--r--   0        0        0     1794 2024-04-29 01:45:23.302231 haondt_charon-1.1.0/charon/destinations/gcp_bucket.py
--rw-r--r--   0        0        0     1164 2024-04-29 01:45:23.302231 haondt_charon-1.1.0/charon/destinations/local.py
--rw-r--r--   0        0        0       50 2024-04-29 01:45:23.302231 haondt_charon-1.1.0/charon/requirements.txt
--rw-r--r--   0        0        0     2532 2024-04-29 01:45:23.302231 haondt_charon-1.1.0/charon/scheduling.py
--rw-r--r--   0        0        0     2434 2024-05-19 15:19:09.288336 haondt_charon-1.1.0/charon/shared.py
--rw-r--r--   0        0        0      138 2024-05-19 15:19:09.288336 haondt_charon-1.1.0/charon/sources/__init__.py
--rw-r--r--   0        0        0     1901 2024-05-19 15:19:09.288336 haondt_charon-1.1.0/charon/sources/http.py
--rw-r--r--   0        0        0     2431 2024-05-19 15:19:09.288336 haondt_charon-1.1.0/charon/sources/lib.py
--rw-r--r--   0        0        0     1024 2024-05-19 15:19:09.288336 haondt_charon-1.1.0/charon/sources/local.py
--rw-r--r--   0        0        0     1378 2024-05-19 15:19:09.288336 haondt_charon-1.1.0/charon/sources/sqlite.py
--rw-r--r--   0        0        0     1312 2024-04-29 01:45:23.302231 haondt_charon-1.1.0/charon/styx.py
--rw-r--r--   0        0        0      314 2024-04-29 01:45:23.302231 haondt_charon-1.1.0/docker-compose.yml
--rw-r--r--   0        0        0      468 2024-05-03 22:30:54.865617 haondt_charon-1.1.0/pipeline.yml
--rw-r--r--   0        0        0      742 2024-05-19 15:19:10.156346 haondt_charon-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      788 2024-05-19 15:19:09.288336 haondt_charon-1.1.0/tests/charon.test.yml
--rwxr-xr-x   0        0        0      682 2024-05-19 15:19:09.288336 haondt_charon-1.1.0/tests/test.sh
--rwxr-xr-x   0        0        0      923 2024-05-19 15:19:09.288336 haondt_charon-1.1.0/tests/test2.sh
--rwxr-xr-x   0        0        0      948 2024-05-19 15:19:09.288336 haondt_charon-1.1.0/tests/test3.sh
--rw-r--r--   0        0        0     6300 1970-01-01 00:00:00.000000 haondt_charon-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       45 2024-05-19 15:19:09.288336 haondt_charon-1.2.0/.gitignore
+-rw-r--r--   0        0        0      169 2024-04-29 01:45:23.302231 haondt_charon-1.2.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      206 2024-05-03 22:30:54.865617 haondt_charon-1.2.0/Dockerfile
+-rw-r--r--   0        0        0     1081 2024-04-29 01:45:23.302231 haondt_charon-1.2.0/LICENSE
+-rw-r--r--   0        0        0     5873 2024-05-23 12:37:51.764041 haondt_charon-1.2.0/README.md
+-rw-r--r--   0        0        0     1054 2024-04-29 01:45:23.302231 haondt_charon-1.2.0/charon.yml
+-rw-r--r--   0        0        0        0 2024-05-23 12:37:51.852042 haondt_charon-1.2.0/charon/__init__.py
+-rw-r--r--   0        0        0     1586 2024-05-23 12:37:51.764041 haondt_charon-1.2.0/charon/__main__.py
+-rw-r--r--   0        0        0       45 2024-04-29 01:45:23.302231 haondt_charon-1.2.0/charon/destinations/__init__.py
+-rw-r--r--   0        0        0     1869 2024-05-23 12:37:51.764041 haondt_charon-1.2.0/charon/destinations/gcp_bucket.py
+-rw-r--r--   0        0        0     1164 2024-04-29 01:45:23.302231 haondt_charon-1.2.0/charon/destinations/local.py
+-rw-r--r--   0        0        0       50 2024-04-29 01:45:23.302231 haondt_charon-1.2.0/charon/requirements.txt
+-rw-r--r--   0        0        0     2939 2024-05-23 12:37:51.764041 haondt_charon-1.2.0/charon/scheduling.py
+-rw-r--r--   0        0        0     2434 2024-05-19 15:19:09.288336 haondt_charon-1.2.0/charon/shared.py
+-rw-r--r--   0        0        0      138 2024-05-19 15:19:09.288336 haondt_charon-1.2.0/charon/sources/__init__.py
+-rw-r--r--   0        0        0     1901 2024-05-19 15:19:09.288336 haondt_charon-1.2.0/charon/sources/http.py
+-rw-r--r--   0        0        0     2431 2024-05-19 15:19:09.288336 haondt_charon-1.2.0/charon/sources/lib.py
+-rw-r--r--   0        0        0     1024 2024-05-19 15:19:09.288336 haondt_charon-1.2.0/charon/sources/local.py
+-rw-r--r--   0        0        0     1378 2024-05-19 15:19:09.288336 haondt_charon-1.2.0/charon/sources/sqlite.py
+-rw-r--r--   0        0        0     1312 2024-04-29 01:45:23.302231 haondt_charon-1.2.0/charon/styx.py
+-rw-r--r--   0        0        0      314 2024-04-29 01:45:23.302231 haondt_charon-1.2.0/docker-compose.yml
+-rw-r--r--   0        0        0      468 2024-05-03 22:30:54.865617 haondt_charon-1.2.0/pipeline.yml
+-rw-r--r--   0        0        0      742 2024-05-23 12:37:52.548049 haondt_charon-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      788 2024-05-19 15:19:09.288336 haondt_charon-1.2.0/tests/charon.test.yml
+-rwxr-xr-x   0        0        0      682 2024-05-19 15:19:09.288336 haondt_charon-1.2.0/tests/test.sh
+-rwxr-xr-x   0        0        0      923 2024-05-19 15:19:09.288336 haondt_charon-1.2.0/tests/test2.sh
+-rwxr-xr-x   0        0        0      948 2024-05-19 15:19:09.288336 haondt_charon-1.2.0/tests/test3.sh
+-rw-r--r--   0        0        0     6418 1970-01-01 00:00:00.000000 haondt_charon-1.2.0/PKG-INFO
```

### Comparing `haondt_charon-1.1.0/LICENSE` & `haondt_charon-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.1.0/README.md` & `haondt_charon-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -119,14 +119,24 @@
     url: http://example.com/ # url to make request to
     method: get # optional, request method, defaults to get
     ext: json # optional, extension to use for saved file, defaults to txt
     auth:  # optional, authentication configuration
         bearer: eyJhbGc... # optional, bearer token
 ```
 
+**sqlite**
+
+performs a backup on an sqlite3 db
+
+```yml
+source:
+    type: sqlite
+    db_path: /path/to/db_file.db
+```
+
 ## destinations
 
 all destinations will also have some shared fields
 
 ```yml
 destination:
     type: local # determines how to interpret the destination config
```

### Comparing `haondt_charon-1.1.0/charon.yml` & `haondt_charon-1.2.0/charon.yml`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.1.0/charon/__main__.py` & `haondt_charon-1.2.0/charon/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 from .shared import load_config, configure_utils, get_task
 from . import scheduling
 import argparse
 from . import styx
+import logging
+
+_logger = logging.getLogger(__name__)
+LOG_TEMPLATE = '[%(asctime)s] [%(levelname)s] %(name)s: %(message)s'
+logging.basicConfig(format=LOG_TEMPLATE, level=logging.INFO)
 
 DEFAULT_CONFIG_FILE = 'charon.yml'
 
 def serve(args):
     config = load_config(args.file)
     configure_utils(config)
 
@@ -33,14 +38,14 @@
     subparsers = parser.add_subparsers(dest='subcommand')
 
     styx_parser = subparsers.add_parser('styx')
     styx.configure_parser(styx_parser)
 
     args = parser.parse_args()
     if args.subcommand is None:
-        print('running in service mode...')
+        _logger.info('running in service mode...')
         serve(args)
     elif args.subcommand == 'styx':
         styx.execute(args)
 
 if __name__ == '__main__':
     main()
```

### Comparing `haondt_charon-1.1.0/charon/destinations/gcp_bucket.py` & `haondt_charon-1.2.0/charon/destinations/gcp_bucket.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass, field
 from google.cloud import storage
-import os
+import os, logging
 
+_logger = logging.getLogger(__name__)
 
 @dataclass
 class GcpBucketConfigEntry:
     bucket: str
 
 @dataclass
 class GcpBucketConfig:
@@ -31,26 +32,26 @@
     def task(extension: str, input_file: str):
         nonlocal output_name
         nonlocal config
 
         ensureCredentialsEnvVar()
 
         target_path = f"{output_name}.{extension}"
-        print(f'starting upload to gs://{config.bucket}/{target_path}')
+        _logger.info(f'starting upload to gs://{config.bucket}/{target_path}')
         client = storage.Client()
         bucket = client.get_bucket(config.bucket)
         blob = bucket.blob(target_path)
         blob.upload_from_filename(input_file)
-        print(f'finished upload to gs://{config.bucket}/{target_path}')
+        _logger.info(f'finished upload to gs://{config.bucket}/{target_path}')
     return task
 
 def revert(config, extension, output_file_path):
     ensureCredentialsEnvVar()
     output_name = config['name']
     config = _config.entries[config['config']] 
     target_path = f"{output_name}.{extension}"
-    print(f'starting download from gs://{config.bucket}/{target_path}')
+    _logger.info(f'starting download from gs://{config.bucket}/{target_path}')
     client = storage.Client()
     bucket = client.get_bucket(config.bucket)
     blob = bucket.blob(target_path)
     blob.download_to_filename(output_file_path)
-    print(f'finished download from to gs://{config.bucket}/{target_path}')
+    _logger.info(f'finished download from to gs://{config.bucket}/{target_path}')
```

### Comparing `haondt_charon-1.1.0/charon/destinations/local.py` & `haondt_charon-1.2.0/charon/destinations/local.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.1.0/charon/scheduling.py` & `haondt_charon-1.2.0/charon/scheduling.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 import sched, time
 from typing import Callable
 from croniter import croniter
 from dataclasses import dataclass 
 import logging
 from datetime import timedelta
-import re
+import re, signal
 
 _logger = logging.getLogger(__name__)
 
+JOB_TIMEOUT_SECONDS = 30
+
+def timeout_handler(signum, frame):
+    raise Exception(f'Job failed to complete in the maximum allowed timeframe: {JOB_TIMEOUT_SECONDS} seconds')
 
 @dataclass
 class Job:
     name: str
     itr: Callable[[], float]
     task: Callable
     repeat: bool = True
 
     def schedule_next(self, scheduler):
         next = self.itr()
         scheduler.enterabs(next, 1, self.run_and_reschedule, (scheduler,))
 
     def run_and_reschedule(self, scheduler):
+        _logger.info(f"Executing job {self.name}")
+        signal.signal(signal.SIGALRM, timeout_handler)
         try:
-            self.task()
-        except Exception as e:
-            _logger.exception(f"Job {self.name} failed: {e}")
+            signal.alarm(JOB_TIMEOUT_SECONDS)
+            try:
+                self.task()
+            except Exception as e:
+                _logger.exception(f"Job {self.name} failed: {e}")
+        finally:
+            signal.alarm(0)
 
         if self.repeat:
             self.schedule_next(scheduler)
 
 class TimeDeltaIterator:
     def __init__(self, delta: timedelta, base: float):
         self.delta: float = delta.total_seconds()
```

### Comparing `haondt_charon-1.1.0/charon/shared.py` & `haondt_charon-1.2.0/charon/shared.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.1.0/charon/sources/http.py` & `haondt_charon-1.2.0/charon/sources/http.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.1.0/charon/sources/lib.py` & `haondt_charon-1.2.0/charon/sources/lib.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.1.0/charon/sources/local.py` & `haondt_charon-1.2.0/charon/sources/local.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.1.0/charon/sources/sqlite.py` & `haondt_charon-1.2.0/charon/sources/sqlite.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.1.0/charon/styx.py` & `haondt_charon-1.2.0/charon/styx.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.1.0/pyproject.toml` & `haondt_charon-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [ "flit_core >=3.2,<4",]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "haondt_charon"
 classifiers = [ "License :: OSI Approved :: MIT License",]
 description = "charon is a utility for backing up data from one location to another at regular intervals."
-version = "1.1.0"
+version = "1.2.0"
 readme = "README.md"
 keywords = [ "backup", "recovery",]
 dependencies = [ "croniter>=2.0.5", "PyYAML>=6.0.1", "cryptography>=42.0.5", "google-cloud-storage>=2.16.0",]
 [[project.authors]]
 name = "haondt"
 
 [project.license]
```

### Comparing `haondt_charon-1.1.0/tests/charon.test.yml` & `haondt_charon-1.2.0/tests/charon.test.yml`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.1.0/tests/test.sh` & `haondt_charon-1.2.0/tests/test.sh`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.1.0/tests/test2.sh` & `haondt_charon-1.2.0/tests/test2.sh`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.1.0/tests/test3.sh` & `haondt_charon-1.2.0/tests/test3.sh`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.1.0/PKG-INFO` & `haondt_charon-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haondt_charon
-Version: 1.1.0
+Version: 1.2.0
 Summary: charon is a utility for backing up data from one location to another at regular intervals.
 Keywords: backup,recovery
 Author: haondt
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: croniter>=2.0.5
 Requires-Dist: PyYAML>=6.0.1
@@ -134,14 +134,24 @@
     url: http://example.com/ # url to make request to
     method: get # optional, request method, defaults to get
     ext: json # optional, extension to use for saved file, defaults to txt
     auth:  # optional, authentication configuration
         bearer: eyJhbGc... # optional, bearer token
 ```
 
+**sqlite**
+
+performs a backup on an sqlite3 db
+
+```yml
+source:
+    type: sqlite
+    db_path: /path/to/db_file.db
+```
+
 ## destinations
 
 all destinations will also have some shared fields
 
 ```yml
 destination:
     type: local # determines how to interpret the destination config
```

