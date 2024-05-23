# Comparing `tmp/data_ingestion_lib-1.0.0.tar.gz` & `tmp/data_ingestion_lib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ingestion_lib-1.0.0.tar", max compression
+gzip compressed data, was "data_ingestion_lib-1.0.2.tar", max compression
```

## Comparing `data_ingestion_lib-1.0.0.tar` & `data_ingestion_lib-1.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0        0 2024-05-10 02:19:40.568734 data_ingestion_lib-1.0.0/data_ingestion/aws_services/__init__.py
--rw-r--r--   0        0        0      781 2024-05-14 03:16:33.631281 data_ingestion_lib-1.0.0/data_ingestion/aws_services/eventbridge_service.py
--rw-r--r--   0        0        0     1088 2024-05-14 03:16:33.629923 data_ingestion_lib-1.0.0/data_ingestion/aws_services/s3_service.py
--rw-r--r--   0        0        0     1900 2024-05-14 03:16:33.629459 data_ingestion_lib-1.0.0/data_ingestion/aws_services/scheduler_service.py
--rw-r--r--   0        0        0        0 2024-05-10 02:19:40.572765 data_ingestion_lib-1.0.0/data_ingestion/crud/__init__.py
--rw-r--r--   0        0        0     4036 2024-05-14 03:16:33.630798 data_ingestion_lib-1.0.0/data_ingestion/crud/data_ingestion_metadata_table/DataIngestionConfig.py
--rw-r--r--   0        0        0     4061 2024-05-14 03:16:33.631018 data_ingestion_lib-1.0.0/data_ingestion/crud/data_ingestion_metadata_table/ExportStatus.py
--rw-r--r--   0        0        0        0 2024-05-10 02:19:40.574777 data_ingestion_lib-1.0.0/data_ingestion/crud/data_ingestion_metadata_table/__init__.py
--rw-r--r--   0        0        0     1627 2024-05-14 03:16:33.630393 data_ingestion_lib-1.0.0/data_ingestion/database/SetupDB.py
--rw-r--r--   0        0        0        0 2024-05-10 02:19:40.575725 data_ingestion_lib-1.0.0/data_ingestion/database/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 02:19:40.576195 data_ingestion_lib-1.0.0/data_ingestion/model/__init__.py
--rw-r--r--   0        0        0     1798 2024-05-10 02:19:40.576944 data_ingestion_lib-1.0.0/data_ingestion/model/data_ingestion_metadata_table/DataIngestionConfig.py
--rw-r--r--   0        0        0     3511 2024-05-10 02:19:40.577636 data_ingestion_lib-1.0.0/data_ingestion/model/data_ingestion_metadata_table/ExportStatus.py
--rw-r--r--   0        0        0        0 2024-05-10 02:19:40.577757 data_ingestion_lib-1.0.0/data_ingestion/model/data_ingestion_metadata_table/__init__.py
--rw-r--r--   0        0        0      816 2024-05-15 03:02:49.214003 data_ingestion_lib-1.0.0/data_ingestion/settings.py
--rw-r--r--   0        0        0        0 2024-05-10 02:19:40.579065 data_ingestion_lib-1.0.0/data_ingestion/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 02:19:40.579671 data_ingestion_lib-1.0.0/data_ingestion/tests/aws_services/__init__.py
--rw-r--r--   0        0        0     2126 2024-05-15 10:02:06.051740 data_ingestion_lib-1.0.0/data_ingestion/tests/aws_services/test_s3_service.py
--rw-r--r--   0        0        0     2048 2024-05-14 03:16:33.630598 data_ingestion_lib-1.0.0/data_ingestion/tests/aws_services/test_scheduler_service.py
--rw-r--r--   0        0        0     4456 2024-05-15 08:38:37.510139 data_ingestion_lib-1.0.0/data_ingestion/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-05-10 02:19:40.582037 data_ingestion_lib-1.0.0/data_ingestion/tests/crud/__init__.py
--rw-r--r--   0        0        0     2965 2024-05-14 03:16:33.631470 data_ingestion_lib-1.0.0/data_ingestion/tests/crud/test_data_ingestion_metadata_table.py
--rw-r--r--   0        0        0     2357 2024-05-14 03:16:33.630134 data_ingestion_lib-1.0.0/data_ingestion/tests/crud/test_export_status.py
--rw-r--r--   0        0        0        0 2024-05-15 04:43:31.911804 data_ingestion_lib-1.0.0/data_ingestion/tests/utils/__init__.py
--rw-r--r--   0        0        0     1535 2024-05-15 08:44:04.658150 data_ingestion_lib-1.0.0/data_ingestion/tests/utils/test_data_ingestion_utils.py
--rw-r--r--   0        0        0        0 2024-05-10 02:19:40.584861 data_ingestion_lib-1.0.0/data_ingestion/utils/__init__.py
--rw-r--r--   0        0        0      261 2024-05-14 03:16:33.570438 data_ingestion_lib-1.0.0/data_ingestion/utils/aws_session.py
--rw-r--r--   0        0        0      544 2024-05-10 02:19:40.586519 data_ingestion_lib-1.0.0/data_ingestion/utils/common.py
--rw-r--r--   0        0        0      484 2024-05-10 02:19:40.587179 data_ingestion_lib-1.0.0/data_ingestion/utils/datetime_util.py
--rw-r--r--   0        0        0      440 2024-05-14 03:16:33.530748 data_ingestion_lib-1.0.0/data_ingestion/utils/dynamodb_client.py
--rw-r--r--   0        0        0      235 2024-05-14 03:16:33.551322 data_ingestion_lib-1.0.0/data_ingestion/utils/eventbridge_client.py
--rw-r--r--   0        0        0       43 2024-05-10 02:19:40.589877 data_ingestion_lib-1.0.0/data_ingestion/utils/exception.py
--rw-r--r--   0        0        0     1726 2024-05-10 02:19:40.590541 data_ingestion_lib-1.0.0/data_ingestion/utils/logger.py
--rw-r--r--   0        0        0      404 2024-05-14 03:16:33.570572 data_ingestion_lib-1.0.0/data_ingestion/utils/s3_client.py
--rw-r--r--   0        0        0      239 2024-05-14 03:16:33.570644 data_ingestion_lib-1.0.0/data_ingestion/utils/scheduler_client.py
--rw-r--r--   0        0        0      221 2024-05-14 03:16:33.528683 data_ingestion_lib-1.0.0/data_ingestion/utils/sqs_client.py
--rw-r--r--   0        0        0      457 2024-05-14 03:16:33.529198 data_ingestion_lib-1.0.0/data_ingestion/utils/step_function_client.py
--rw-r--r--   0        0        0      188 2024-05-22 07:26:57.272077 data_ingestion_lib-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      747 1970-01-01 00:00:00.000000 data_ingestion_lib-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-22 08:36:12.337511 data_ingestion_lib-1.0.2/data_ingestion/aws_services/__init__.py
+-rw-r--r--   0        0        0      781 2024-05-22 08:36:12.338115 data_ingestion_lib-1.0.2/data_ingestion/aws_services/eventbridge_service.py
+-rw-r--r--   0        0        0     1088 2024-05-22 08:36:12.338469 data_ingestion_lib-1.0.2/data_ingestion/aws_services/s3_service.py
+-rw-r--r--   0        0        0     1900 2024-05-22 08:36:12.338806 data_ingestion_lib-1.0.2/data_ingestion/aws_services/scheduler_service.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:36:12.338915 data_ingestion_lib-1.0.2/data_ingestion/crud/__init__.py
+-rw-r--r--   0        0        0     4036 2024-05-22 08:36:12.339430 data_ingestion_lib-1.0.2/data_ingestion/crud/data_ingestion_metadata_table/DataIngestionConfig.py
+-rw-r--r--   0        0        0     4061 2024-05-22 08:36:12.339790 data_ingestion_lib-1.0.2/data_ingestion/crud/data_ingestion_metadata_table/ExportStatus.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:36:12.339882 data_ingestion_lib-1.0.2/data_ingestion/crud/data_ingestion_metadata_table/__init__.py
+-rw-r--r--   0        0        0     1627 2024-05-22 08:36:12.340374 data_ingestion_lib-1.0.2/data_ingestion/database/SetupDB.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:36:12.340461 data_ingestion_lib-1.0.2/data_ingestion/database/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:36:12.340726 data_ingestion_lib-1.0.2/data_ingestion/model/__init__.py
+-rw-r--r--   0        0        0     1798 2024-05-22 08:36:12.341214 data_ingestion_lib-1.0.2/data_ingestion/model/data_ingestion_metadata_table/DataIngestionConfig.py
+-rw-r--r--   0        0        0     3511 2024-05-22 08:36:12.341549 data_ingestion_lib-1.0.2/data_ingestion/model/data_ingestion_metadata_table/ExportStatus.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:36:12.341636 data_ingestion_lib-1.0.2/data_ingestion/model/data_ingestion_metadata_table/__init__.py
+-rw-r--r--   0        0        0      816 2024-05-22 08:36:12.342104 data_ingestion_lib-1.0.2/data_ingestion/settings.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:36:12.342211 data_ingestion_lib-1.0.2/data_ingestion/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:36:12.342475 data_ingestion_lib-1.0.2/data_ingestion/tests/aws_services/__init__.py
+-rw-r--r--   0        0        0     2126 2024-05-22 08:36:12.342968 data_ingestion_lib-1.0.2/data_ingestion/tests/aws_services/test_s3_service.py
+-rw-r--r--   0        0        0     2048 2024-05-22 08:36:12.343292 data_ingestion_lib-1.0.2/data_ingestion/tests/aws_services/test_scheduler_service.py
+-rw-r--r--   0        0        0     4456 2024-05-22 08:36:12.343642 data_ingestion_lib-1.0.2/data_ingestion/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:36:12.343771 data_ingestion_lib-1.0.2/data_ingestion/tests/crud/__init__.py
+-rw-r--r--   0        0        0     2965 2024-05-22 08:36:12.344603 data_ingestion_lib-1.0.2/data_ingestion/tests/crud/test_data_ingestion_metadata_table.py
+-rw-r--r--   0        0        0     2357 2024-05-22 08:36:12.345085 data_ingestion_lib-1.0.2/data_ingestion/tests/crud/test_export_status.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:36:12.345253 data_ingestion_lib-1.0.2/data_ingestion/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1535 2024-05-22 08:36:12.346753 data_ingestion_lib-1.0.2/data_ingestion/tests/utils/test_data_ingestion_utils.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:36:12.346960 data_ingestion_lib-1.0.2/data_ingestion/utils/__init__.py
+-rw-r--r--   0        0        0      261 2024-05-22 08:36:12.347768 data_ingestion_lib-1.0.2/data_ingestion/utils/aws_session.py
+-rw-r--r--   0        0        0      544 2024-05-22 08:36:12.348347 data_ingestion_lib-1.0.2/data_ingestion/utils/common.py
+-rw-r--r--   0        0        0      484 2024-05-22 08:36:12.348937 data_ingestion_lib-1.0.2/data_ingestion/utils/datetime_util.py
+-rw-r--r--   0        0        0      440 2024-05-22 08:36:12.349454 data_ingestion_lib-1.0.2/data_ingestion/utils/dynamodb_client.py
+-rw-r--r--   0        0        0      235 2024-05-22 08:36:12.349969 data_ingestion_lib-1.0.2/data_ingestion/utils/eventbridge_client.py
+-rw-r--r--   0        0        0       43 2024-05-22 08:36:12.350473 data_ingestion_lib-1.0.2/data_ingestion/utils/exception.py
+-rw-r--r--   0        0        0     1726 2024-05-22 08:36:12.351000 data_ingestion_lib-1.0.2/data_ingestion/utils/logger.py
+-rw-r--r--   0        0        0      404 2024-05-22 08:36:12.351503 data_ingestion_lib-1.0.2/data_ingestion/utils/s3_client.py
+-rw-r--r--   0        0        0      239 2024-05-22 08:36:12.352026 data_ingestion_lib-1.0.2/data_ingestion/utils/scheduler_client.py
+-rw-r--r--   0        0        0      221 2024-05-22 08:36:12.352543 data_ingestion_lib-1.0.2/data_ingestion/utils/sqs_client.py
+-rw-r--r--   0        0        0      457 2024-05-22 08:36:12.353085 data_ingestion_lib-1.0.2/data_ingestion/utils/step_function_client.py
+-rw-r--r--   0        0        0      361 2024-05-23 06:43:32.165645 data_ingestion_lib-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 data_ingestion_lib-1.0.2/PKG-INFO
```

### Comparing `data_ingestion_lib-1.0.0/data_ingestion/aws_services/eventbridge_service.py` & `data_ingestion_lib-1.0.2/data_ingestion/aws_services/eventbridge_service.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.0/data_ingestion/aws_services/s3_service.py` & `data_ingestion_lib-1.0.2/data_ingestion/aws_services/s3_service.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.0/data_ingestion/aws_services/scheduler_service.py` & `data_ingestion_lib-1.0.2/data_ingestion/aws_services/scheduler_service.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.0/data_ingestion/crud/data_ingestion_metadata_table/DataIngestionConfig.py` & `data_ingestion_lib-1.0.2/data_ingestion/crud/data_ingestion_metadata_table/DataIngestionConfig.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.0/data_ingestion/crud/data_ingestion_metadata_table/ExportStatus.py` & `data_ingestion_lib-1.0.2/data_ingestion/crud/data_ingestion_metadata_table/ExportStatus.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.0/data_ingestion/database/SetupDB.py` & `data_ingestion_lib-1.0.2/data_ingestion/database/SetupDB.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.0/data_ingestion/model/data_ingestion_metadata_table/DataIngestionConfig.py` & `data_ingestion_lib-1.0.2/data_ingestion/model/data_ingestion_metadata_table/DataIngestionConfig.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.0/data_ingestion/model/data_ingestion_metadata_table/ExportStatus.py` & `data_ingestion_lib-1.0.2/data_ingestion/model/data_ingestion_metadata_table/ExportStatus.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.0/data_ingestion/settings.py` & `data_ingestion_lib-1.0.2/data_ingestion/settings.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.0/data_ingestion/tests/aws_services/test_s3_service.py` & `data_ingestion_lib-1.0.2/data_ingestion/tests/aws_services/test_s3_service.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.0/data_ingestion/tests/aws_services/test_scheduler_service.py` & `data_ingestion_lib-1.0.2/data_ingestion/tests/aws_services/test_scheduler_service.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.0/data_ingestion/tests/conftest.py` & `data_ingestion_lib-1.0.2/data_ingestion/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.0/data_ingestion/tests/crud/test_data_ingestion_metadata_table.py` & `data_ingestion_lib-1.0.2/data_ingestion/tests/crud/test_data_ingestion_metadata_table.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.0/data_ingestion/tests/crud/test_export_status.py` & `data_ingestion_lib-1.0.2/data_ingestion/tests/crud/test_export_status.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.0/data_ingestion/tests/utils/test_data_ingestion_utils.py` & `data_ingestion_lib-1.0.2/data_ingestion/tests/utils/test_data_ingestion_utils.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.0/data_ingestion/utils/common.py` & `data_ingestion_lib-1.0.2/data_ingestion/utils/common.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.0/data_ingestion/utils/logger.py` & `data_ingestion_lib-1.0.2/data_ingestion/utils/logger.py`

 * *Files identical despite different names*

### Comparing `data_ingestion_lib-1.0.0/PKG-INFO` & `data_ingestion_lib-1.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: data-ingestion-lib
-Version: 1.0.0
+Version: 1.0.2
 Summary: Data ingestion module 
 Author: Dat Nguyen
 Author-email: dat.nguyen2@tyme.com
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: boto3 (>=1.34,<2.0)
+Requires-Dist: moto (==4.2.9)
+Requires-Dist: mypy_boto3_dynamodb (>=1.34,<2.0)
+Requires-Dist: mypy_boto3_s3 (>=1.34,<2.0)
+Requires-Dist: pytest (>=7.2,<8.0)
+Requires-Dist: python-json-logger (>=2.0,<3.0)
```

