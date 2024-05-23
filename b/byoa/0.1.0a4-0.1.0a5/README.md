# Comparing `tmp/byoa-0.1.0a4.tar.gz` & `tmp/byoa-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byoa-0.1.0a4.tar", max compression
+gzip compressed data, was "byoa-0.1.0a5.tar", max compression
```

## Comparing `byoa-0.1.0a4.tar` & `byoa-0.1.0a5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1050 2024-03-28 14:43:47.389162 byoa-0.1.0a4/LICENSE
--rw-r--r--   0        0        0     2410 2024-03-28 14:43:47.389162 byoa-0.1.0a4/README.md
--rw-r--r--   0        0        0     1333 2024-03-28 14:43:47.389162 byoa-0.1.0a4/pyproject.toml
--rw-r--r--   0        0        0       73 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/__init__.py
--rw-r--r--   0        0        0       82 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/__main__.py
--rw-r--r--   0        0        0      818 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/cli/__init__.py
--rw-r--r--   0        0        0     1759 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/cli/build.py
--rw-r--r--   0        0        0      941 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/cli/context.py
--rw-r--r--   0        0        0     1962 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/cli/delete.py
--rw-r--r--   0        0        0     4109 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/cli/deploy.py
--rw-r--r--   0        0        0     2413 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/cli/init.py
--rw-r--r--   0        0        0      455 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/cli/manifest.py
--rw-r--r--   0        0        0     1744 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/cli/run.py
--rw-r--r--   0        0        0       52 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/cloud_storage/__init__.py
--rw-r--r--   0        0        0     2678 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/cloud_storage/aws_s3.py
--rw-r--r--   0        0        0     4092 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/cloud_storage/azure_blob_storage.py
--rw-r--r--   0        0        0      153 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/config/__init__.py
--rw-r--r--   0        0        0     1793 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/config/context.py
--rw-r--r--   0        0        0     2901 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/config/manifest.py
--rw-r--r--   0        0        0     1126 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/exceptions.py
--rw-r--r--   0        0        0      547 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/importer.py
--rw-r--r--   0        0        0     1029 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/models.py
--rw-r--r--   0        0        0       73 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/telemetry/__init__.py
--rw-r--r--   0        0        0       42 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/telemetry/log_manager/__init__.py
--rw-r--r--   0        0        0     2505 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/telemetry/log_manager/log_manager.py
--rw-r--r--   0        0        0      801 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/telemetry/log_manager/trace_formatter.py
--rw-r--r--   0        0        0       44 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/telemetry/trace_manager/__init__.py
--rw-r--r--   0        0        0     2654 2024-03-28 14:43:47.393162 byoa-0.1.0a4/src/byoa/telemetry/trace_manager/trace_manager.py
--rw-r--r--   0        0        0     3184 1970-01-01 00:00:00.000000 byoa-0.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1050 2024-05-23 13:06:00.354528 byoa-0.1.0a5/LICENSE
+-rw-r--r--   0        0        0     2410 2024-05-23 13:06:00.354528 byoa-0.1.0a5/README.md
+-rw-r--r--   0        0        0     1333 2024-05-23 13:06:00.358528 byoa-0.1.0a5/pyproject.toml
+-rw-r--r--   0        0        0       73 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/__init__.py
+-rw-r--r--   0        0        0       82 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/__main__.py
+-rw-r--r--   0        0        0      818 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/cli/__init__.py
+-rw-r--r--   0        0        0     1759 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/cli/build.py
+-rw-r--r--   0        0        0      941 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/cli/context.py
+-rw-r--r--   0        0        0     1962 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/cli/delete.py
+-rw-r--r--   0        0        0     4109 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/cli/deploy.py
+-rw-r--r--   0        0        0     2413 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/cli/init.py
+-rw-r--r--   0        0        0      455 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/cli/manifest.py
+-rw-r--r--   0        0        0     1744 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/cli/run.py
+-rw-r--r--   0        0        0       52 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/cloud_storage/__init__.py
+-rw-r--r--   0        0        0     3781 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/cloud_storage/aws_s3.py
+-rw-r--r--   0        0        0     4092 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/cloud_storage/azure_blob_storage.py
+-rw-r--r--   0        0        0      153 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/config/__init__.py
+-rw-r--r--   0        0        0     1793 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/config/context.py
+-rw-r--r--   0        0        0     2901 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/config/manifest.py
+-rw-r--r--   0        0        0     1126 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/exceptions.py
+-rw-r--r--   0        0        0      547 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/importer.py
+-rw-r--r--   0        0        0     1029 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/models.py
+-rw-r--r--   0        0        0       73 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/telemetry/__init__.py
+-rw-r--r--   0        0        0       42 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/telemetry/log_manager/__init__.py
+-rw-r--r--   0        0        0     2505 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/telemetry/log_manager/log_manager.py
+-rw-r--r--   0        0        0      801 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/telemetry/log_manager/trace_formatter.py
+-rw-r--r--   0        0        0       44 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/telemetry/trace_manager/__init__.py
+-rw-r--r--   0        0        0     2654 2024-05-23 13:06:00.358528 byoa-0.1.0a5/src/byoa/telemetry/trace_manager/trace_manager.py
+-rw-r--r--   0        0        0     3184 1970-01-01 00:00:00.000000 byoa-0.1.0a5/PKG-INFO
```

### Comparing `byoa-0.1.0a4/LICENSE` & `byoa-0.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `byoa-0.1.0a4/README.md` & `byoa-0.1.0a5/README.md`

 * *Files identical despite different names*

### Comparing `byoa-0.1.0a4/pyproject.toml` & `byoa-0.1.0a5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "byoa"
-version = "0.1.0a4"
+version = "0.1.0a5"
 description = ""
 authors = [
     "ada-geosys <ada@geosys.com>",
     "kls <kls@geosys.com>",
     "jpn <jpn@geosys.com>",
 ]
 readme = "README.md"
```

### Comparing `byoa-0.1.0a4/src/byoa/cli/__init__.py` & `byoa-0.1.0a5/src/byoa/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `byoa-0.1.0a4/src/byoa/cli/build.py` & `byoa-0.1.0a5/src/byoa/cli/build.py`

 * *Files identical despite different names*

### Comparing `byoa-0.1.0a4/src/byoa/cli/context.py` & `byoa-0.1.0a5/src/byoa/cli/context.py`

 * *Files identical despite different names*

### Comparing `byoa-0.1.0a4/src/byoa/cli/delete.py` & `byoa-0.1.0a5/src/byoa/cli/delete.py`

 * *Files identical despite different names*

### Comparing `byoa-0.1.0a4/src/byoa/cli/deploy.py` & `byoa-0.1.0a5/src/byoa/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `byoa-0.1.0a4/src/byoa/cli/init.py` & `byoa-0.1.0a5/src/byoa/cli/init.py`

 * *Files identical despite different names*

### Comparing `byoa-0.1.0a4/src/byoa/cli/run.py` & `byoa-0.1.0a5/src/byoa/cli/run.py`

 * *Files identical despite different names*

### Comparing `byoa-0.1.0a4/src/byoa/cloud_storage/aws_s3.py` & `byoa-0.1.0a5/src/byoa/cloud_storage/aws_s3.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """AWS S3 helper functions"""
 
 import os
 
 import boto3
 from boto3.exceptions import Boto3Error
+from botocore.client import Config
 
 
 def upload_file(local_file_path: str, bucket_name: str) -> bool:
     """Upload a file to AWS S3 Bucket.
 
     Args:
       local_file_path(str): The local file path to upload.
@@ -65,25 +66,59 @@
         except Boto3Error as error:
             print(f"Error while uploading folder to AWS S3: {error}")
             return False
     else:
         return False
 
 
-def get_s3_uri_path(local_path: str, bucket_name: str) -> str:
+def get_s3_uri_path(
+    local_path: str, bucket_name: str, presigned_url: bool = False, expiration: int = 3600
+) -> str:
     """Get the s3 path of the uploaded element (file or folder)
 
     Args:
       local_path(str): The local path of the uploaded folder/file on s3
       bucket_name(str): The bucket name set to store the file on s3
+      presigned_url(bool): Option to presign URL,
+      expiration(int): expiration time in second to access presigned urls
 
     Returns:
       str: the s3 uri of the uploaded folder/file
     """
     # get bucket name
     if bucket_name is None:
         raise ValueError("bucket_name cannot be 'None'")
 
     s3_key = os.path.basename(local_path)
-    s3_uri = f"s3://{bucket_name}/{s3_key}"
 
-    return s3_uri
+    # get the region of the bucket to generate presigned url
+    region = get_bucket_region(bucket_name)
+
+    s3_client = boto3.client("s3", config=Config(signature_version="s3v4"), region_name=region)
+    if presigned_url:
+        s3_uri = s3_client.generate_presigned_url(
+            "get_object",
+            Params={"Bucket": bucket_name, "Key": s3_key},
+            ExpiresIn=expiration,
+            HttpMethod="GET",
+        )
+        return s3_uri
+
+    return f"s3://{bucket_name}/{s3_key}"
+
+
+def get_bucket_region(bucket_name):
+    """
+    Get the region of an S3 bucket.
+
+    Args:
+    - bucket_name (str): The name of the S3 bucket.
+
+    Returns:
+    - str: The region of the bucket.
+    """
+    s3 = boto3.client("s3")
+    response = s3.get_bucket_location(Bucket=bucket_name)
+    region = response.get(
+        "LocationConstraint", "us-east-1"
+    )  # Default to 'us-east-1' if no location constraint is specified
+    return region
```

### Comparing `byoa-0.1.0a4/src/byoa/cloud_storage/azure_blob_storage.py` & `byoa-0.1.0a5/src/byoa/cloud_storage/azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `byoa-0.1.0a4/src/byoa/config/context.py` & `byoa-0.1.0a5/src/byoa/config/context.py`

 * *Files identical despite different names*

### Comparing `byoa-0.1.0a4/src/byoa/config/manifest.py` & `byoa-0.1.0a5/src/byoa/config/manifest.py`

 * *Files identical despite different names*

### Comparing `byoa-0.1.0a4/src/byoa/exceptions.py` & `byoa-0.1.0a5/src/byoa/exceptions.py`

 * *Files identical despite different names*

### Comparing `byoa-0.1.0a4/src/byoa/importer.py` & `byoa-0.1.0a5/src/byoa/importer.py`

 * *Files identical despite different names*

### Comparing `byoa-0.1.0a4/src/byoa/models.py` & `byoa-0.1.0a5/src/byoa/models.py`

 * *Files identical despite different names*

### Comparing `byoa-0.1.0a4/src/byoa/telemetry/log_manager/log_manager.py` & `byoa-0.1.0a5/src/byoa/telemetry/log_manager/log_manager.py`

 * *Files identical despite different names*

### Comparing `byoa-0.1.0a4/src/byoa/telemetry/log_manager/trace_formatter.py` & `byoa-0.1.0a5/src/byoa/telemetry/log_manager/trace_formatter.py`

 * *Files identical despite different names*

### Comparing `byoa-0.1.0a4/src/byoa/telemetry/trace_manager/trace_manager.py` & `byoa-0.1.0a5/src/byoa/telemetry/trace_manager/trace_manager.py`

 * *Files identical despite different names*

### Comparing `byoa-0.1.0a4/PKG-INFO` & `byoa-0.1.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byoa
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: 
 Author: ada-geosys
 Author-email: ada@geosys.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

