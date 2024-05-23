# Comparing `tmp/ng_data_pipelines_sdk-1.4.0.tar.gz` & `tmp/ng_data_pipelines_sdk-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-1.4.0.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-1.4.1.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-1.4.0.tar` & `ng_data_pipelines_sdk-1.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-05-23 13:49:21.485014 ng_data_pipelines_sdk-1.4.0/README.md
--rw-r--r--   0        0        0        0 2024-05-23 13:49:21.520014 ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     9155 2024-05-23 13:49:21.485014 ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-05-23 13:49:21.485014 ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    26638 2024-05-23 13:49:21.485014 ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0    20613 2024-05-23 13:49:21.486014 ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     5406 2024-05-23 13:49:21.486014 ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     4780 2024-05-23 13:49:21.486014 ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      838 2024-05-23 13:49:21.489014 ng_data_pipelines_sdk-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-05-23 13:51:32.379240 ng_data_pipelines_sdk-1.4.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 13:51:32.415240 ng_data_pipelines_sdk-1.4.1/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     9155 2024-05-23 13:51:32.379240 ng_data_pipelines_sdk-1.4.1/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-05-23 13:51:32.379240 ng_data_pipelines_sdk-1.4.1/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    26638 2024-05-23 13:51:32.379240 ng_data_pipelines_sdk-1.4.1/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0    20557 2024-05-23 13:51:32.379240 ng_data_pipelines_sdk-1.4.1/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     5406 2024-05-23 13:51:32.380240 ng_data_pipelines_sdk-1.4.1/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     4780 2024-05-23 13:51:32.380240 ng_data_pipelines_sdk-1.4.1/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      838 2024-05-23 13:51:32.383240 ng_data_pipelines_sdk-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-1.4.1/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/aws_interface.py` & `ng_data_pipelines_sdk-1.4.1/ng_data_pipelines_sdk/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-1.4.1/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/interfaces.py` & `ng_data_pipelines_sdk-1.4.1/ng_data_pipelines_sdk/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,14 @@
 
 class ReadDateParams(BaseModelJsonDumps):
     """
     Represents the parameters for reading dates in a data pipeline.
     Attributes:
         read_dates (Union[List[datetime], datetime, Literal["{{processing_date}}"], Literal["{{processing_date_previous}}"]]):
             The dates to be read. It can be a list of datetimes, a single datetime, or special placeholders for processing dates.
-            The default value is "{{processing_date}}".
         processing_date_offset_days (int):
             The offset to be applied to the processing date. It represents the number of days to add or subtract from the processing date.
             The default value is 0.
         date_partitions (dict[DatePartition, str]):
             A dictionary that maps DatePartition enum values to their corresponding string representations.
             The default value is:
             {
```

### Comparing `ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/spark_manager.py` & `ng_data_pipelines_sdk-1.4.1/ng_data_pipelines_sdk/spark_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/utils.py` & `ng_data_pipelines_sdk-1.4.1/ng_data_pipelines_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.4.0/pyproject.toml` & `ng_data_pipelines_sdk-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ng-data-pipelines-sdk"
-version = "1.4.0"
+version = "1.4.1"
 description = "A library for interacting with data from Amazon S3 through PySpark. Read, write and tranform data using a powerful and intuitive API with strong consistency and type checking, thanks to Pydantic. Compatible with Amazon MWAA running Airflow 2.7.2 and 2.8.1."
 authors = ["ng.cash"]
 readme = "README.md"
 exclude = [".git/", ".gitignore", "tests/", "docs/", "*.yml", "__pycache__/", "*.pyc", "*.ipynb", "playground/", "poetry.lock", "dist/", "build/"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

### Comparing `ng_data_pipelines_sdk-1.4.0/PKG-INFO` & `ng_data_pipelines_sdk-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ng-data-pipelines-sdk
-Version: 1.4.0
+Version: 1.4.1
 Summary: A library for interacting with data from Amazon S3 through PySpark. Read, write and tranform data using a powerful and intuitive API with strong consistency and type checking, thanks to Pydantic. Compatible with Amazon MWAA running Airflow 2.7.2 and 2.8.1.
 Author: ng.cash
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

