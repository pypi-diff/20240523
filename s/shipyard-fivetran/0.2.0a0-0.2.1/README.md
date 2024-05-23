# Comparing `tmp/shipyard_fivetran-0.2.0a0.tar.gz` & `tmp/shipyard_fivetran-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_fivetran-0.2.0a0.tar", max compression
+gzip compressed data, was "shipyard_fivetran-0.2.1.tar", max compression
```

## Comparing `shipyard_fivetran-0.2.0a0.tar` & `shipyard_fivetran-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      708 2024-05-13 20:59:25.581677 shipyard_fivetran-0.2.0a0/pyproject.toml
--rw-r--r--   0        0        0       37 2023-06-21 19:54:18.755231 shipyard_fivetran-0.2.0a0/shipyard_fivetran/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 20:53:35.435162 shipyard_fivetran-0.2.0a0/shipyard_fivetran/cli/__init__.py
--rw-r--r--   0        0        0      297 2024-02-05 20:53:35.435768 shipyard_fivetran-0.2.0a0/shipyard_fivetran/cli/authtest.py
--rw-r--r--   0        0        0     3049 2024-05-13 21:05:14.273052 shipyard_fivetran-0.2.0a0/shipyard_fivetran/cli/sync.py
--rw-r--r--   0        0        0     2188 2024-05-13 21:05:14.262784 shipyard_fivetran-0.2.0a0/shipyard_fivetran/cli/update_connector.py
--rw-r--r--   0        0        0     9916 2024-05-13 21:05:14.268379 shipyard_fivetran-0.2.0a0/shipyard_fivetran/fivetran.py
--rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 shipyard_fivetran-0.2.0a0/PKG-INFO
+-rw-r--r--   0        0        0      510 2024-05-23 14:49:04.633898 shipyard_fivetran-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-06-21 19:54:18.755231 shipyard_fivetran-0.2.1/shipyard_fivetran/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 20:53:35.435162 shipyard_fivetran-0.2.1/shipyard_fivetran/cli/__init__.py
+-rw-r--r--   0        0        0      297 2024-02-05 20:53:35.435768 shipyard_fivetran-0.2.1/shipyard_fivetran/cli/authtest.py
+-rw-r--r--   0        0        0     3163 2024-05-23 14:49:04.634351 shipyard_fivetran-0.2.1/shipyard_fivetran/cli/sync.py
+-rw-r--r--   0        0        0     2418 2024-05-20 15:55:29.094574 shipyard_fivetran-0.2.1/shipyard_fivetran/cli/update_connector.py
+-rw-r--r--   0        0        0     9916 2024-05-20 15:55:29.086248 shipyard_fivetran-0.2.1/shipyard_fivetran/fivetran.py
+-rw-r--r--   0        0        0      641 1970-01-01 00:00:00.000000 shipyard_fivetran-0.2.1/PKG-INFO
```

### Comparing `shipyard_fivetran-0.2.0a0/shipyard_fivetran/cli/sync.py` & `shipyard_fivetran-0.2.1/shipyard_fivetran/cli/sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import argparse
 import datetime
 import os
 import sys
 
 import pytz
 import shipyard_utils as shipyard
-from shipyard_templates import ExitCodeException, ShipyardLogger
+from shipyard_templates import ExitCodeException, ShipyardLogger, Etl
 
 from shipyard_fivetran import FivetranClient
 
 logger = ShipyardLogger.get_logger()
 
-EXIT_CODE_INVALID_POKE_INTERVAL = 101
-
 
 def create_pickle(connector_id):
     base_folder_name = shipyard.logs.determine_base_artifact_folder("fivetran")
     artifact_subfolder_paths = shipyard.logs.determine_artifact_subfolders(
         base_folder_name
     )
     shipyard.logs.create_artifacts_folders(artifact_subfolder_paths)
@@ -64,38 +62,37 @@
     force_sync = force_sync.upper() == "TRUE"
     poke_interval = args.interval
 
     fivetran_client = FivetranClient(
         access_token=args.api_key, api_secret=args.api_secret
     )
     if (
-            not wait_for_completion
-            and int(os.environ.get("SHIPYARD_FLEET_DOWNSTREAM_COUNT")) > 0
+        not wait_for_completion
+        and int(os.environ.get("SHIPYARD_FLEET_DOWNSTREAM_COUNT")) > 0
     ):
         # This function is to support the legacy check status functionality
         create_pickle(args.connector_id)
     poke_interval = int(poke_interval) if poke_interval else 0
     if wait_for_completion:
         if 0 < poke_interval <= 60:
-            logger.info(
-                f"Setting poke interval to {poke_interval} minute(s)"
-            )
+            logger.info(f"Setting poke interval to {poke_interval} minute(s)")
             poke_interval = poke_interval
         else:
-            logger.error(
-                "Poke interval must be between 1 and 60 minutes"
-            )
-            sys.exit(EXIT_CODE_INVALID_POKE_INTERVAL)
+            logger.error("Poke interval must be between 1 and 60 minutes")
+            sys.exit(fivetran_client.EXIT_CODE_SYNC_INVALID_POKE_INTERVAL)
     try:
         fivetran_client.trigger_sync(
             args.connector_id,
             force=force_sync,
             wait_for_completion=wait_for_completion,
             poke_interval=poke_interval * 60,
         )
     except ExitCodeException as e:
-        logger.error(e)
+        f"An error occurred when attempting to trigger sync: {e}"
         sys.exit(e.exit_code)
+    except Exception as e:
+        logger.error(f"An error occurred when attempting to trigger sync: {e}")
+        sys.exit(Etl.EXIT_CODE_UNKNOWN_ERROR)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_fivetran-0.2.0a0/shipyard_fivetran/cli/update_connector.py` & `shipyard_fivetran-0.2.1/shipyard_fivetran/cli/update_connector.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import sys
 import json
 
 from shipyard_fivetran import FivetranClient
-from shipyard_templates import ExitCodeException, ShipyardLogger
+from shipyard_templates import ExitCodeException, ShipyardLogger, Etl
 
 logger = ShipyardLogger.get_logger()
 
 
 def get_args():
     parser = argparse.ArgumentParser(
         description="Update a connector using FivetranClient"
@@ -59,13 +59,16 @@
 
     try:
         fivetran_client.update_connector(
             connector_id,
             **args_dict,
         )
     except ExitCodeException as e:
-        logger.error(e)
+        logger.error(f"An error occurred when attempting to update the connector: {e}")
         sys.exit(e.exit_code)
+    except Exception as e:
+        logger.error(f"An error occurred when attempting to update the connector: {e}")
+        sys.exit(Etl.EXIT_CODE_UNKNOWN_ERROR)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_fivetran-0.2.0a0/shipyard_fivetran/fivetran.py` & `shipyard_fivetran-0.2.1/shipyard_fivetran/fivetran.py`

 * *Files identical despite different names*

### Comparing `shipyard_fivetran-0.2.0a0/PKG-INFO` & `shipyard_fivetran-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-fivetran
-Version: 0.2.0a0
+Version: 0.2.1
 Summary: A local client for connecting and working with Fivetran
 License: Apache 2.0
 Author: JR
 Author-email: johnathan.rodriguez@shipyardapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

