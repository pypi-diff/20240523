# Comparing `tmp/ng_data_pipelines_sdk-1.3.0.tar.gz` & `tmp/ng_data_pipelines_sdk-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-1.3.0.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-1.4.0.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-1.3.0.tar` & `ng_data_pipelines_sdk-1.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-05-23 13:43:24.184311 ng_data_pipelines_sdk-1.3.0/README.md
--rw-r--r--   0        0        0        0 2024-05-23 13:43:24.219311 ng_data_pipelines_sdk-1.3.0/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     9155 2024-05-23 13:43:24.184311 ng_data_pipelines_sdk-1.3.0/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-05-23 13:43:24.184311 ng_data_pipelines_sdk-1.3.0/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    26638 2024-05-23 13:43:24.184311 ng_data_pipelines_sdk-1.3.0/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0    20730 2024-05-23 13:43:24.184311 ng_data_pipelines_sdk-1.3.0/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     5406 2024-05-23 13:43:24.184311 ng_data_pipelines_sdk-1.3.0/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     4780 2024-05-23 13:43:24.185312 ng_data_pipelines_sdk-1.3.0/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      838 2024-05-23 13:43:24.188311 ng_data_pipelines_sdk-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-05-23 13:49:21.485014 ng_data_pipelines_sdk-1.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 13:49:21.520014 ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     9155 2024-05-23 13:49:21.485014 ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-05-23 13:49:21.485014 ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    26638 2024-05-23 13:49:21.485014 ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0    20613 2024-05-23 13:49:21.486014 ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     5406 2024-05-23 13:49:21.486014 ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     4780 2024-05-23 13:49:21.486014 ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      838 2024-05-23 13:49:21.489014 ng_data_pipelines_sdk-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-1.4.0/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-1.3.0/ng_data_pipelines_sdk/aws_interface.py` & `ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.3.0/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.3.0/ng_data_pipelines_sdk/interfaces.py` & `ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,15 @@
             The default value is True.
     """
 
     read_dates: Union[
         Sequence[Union[Union[str, datetime], List[Union[str, datetime]]]],
         datetime,
         Literal["{{processing_date}}"],
-    ] = "{{processing_date}}"
+    ]
     processing_date_offset_days: Optional[int] = None
     was_offset_applied: bool = False
     date_partitions: dict[DatePartition, str] = {
         DatePartition.YEAR: "year",
         DatePartition.MONTH: "month",
         DatePartition.DAY: "day",
     }
@@ -414,17 +414,15 @@
     Attributes:
         single_write_date (Union[datetime, Literal["{{processing_date}}"]]):
             The single write date. It can be either a datetime object or the string "{{processing_date}}".
         single_write_date_partitions (List[str]):
             The list of partitions to be used for the single write date. Defaults to ["year", "month", "day"].
     """
 
-    single_write_date: Union[datetime, Literal["{{processing_date}}"]] = (
-        "{{processing_date}}"
-    )
+    single_write_date: Union[datetime, Literal["{{processing_date}}"]]
     single_write_date_partitions: dict[DatePartition, str] = {
         DatePartition.YEAR: "year",
         DatePartition.MONTH: "month",
         DatePartition.DAY: "day",
     }
 
     @field_validator("single_write_date_partitions")
@@ -464,15 +462,14 @@
         single_write_date (Optional[SingleWriteDateParams]): Parameters for single write date.
         partition_by (List[str]): List of columns to partition the data by.
     """
 
     dataframe_specific_path: Optional[str] = None
     write_schema_on_s3: bool = False
     overwrite: bool = False
-    dataframe_file_type: FileType = FileType.PARQUET
     single_write_date: Optional[SingleWriteDateParams] = None
     partition_by: Optional[List[str]] = None
 
     @model_validator(mode="before")
     def xor_specific_path_and_dataframe_base_path(cls, data):
         dataframe_specific_path = data.get("dataframe_specific_path")
         dataframe_base_path = data.get("dataframe_base_path")
```

### Comparing `ng_data_pipelines_sdk-1.3.0/ng_data_pipelines_sdk/spark_manager.py` & `ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/spark_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.3.0/ng_data_pipelines_sdk/utils.py` & `ng_data_pipelines_sdk-1.4.0/ng_data_pipelines_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.3.0/pyproject.toml` & `ng_data_pipelines_sdk-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ng-data-pipelines-sdk"
-version = "1.3.0"
+version = "1.4.0"
 description = "A library for interacting with data from Amazon S3 through PySpark. Read, write and tranform data using a powerful and intuitive API with strong consistency and type checking, thanks to Pydantic. Compatible with Amazon MWAA running Airflow 2.7.2 and 2.8.1."
 authors = ["ng.cash"]
 readme = "README.md"
 exclude = [".git/", ".gitignore", "tests/", "docs/", "*.yml", "__pycache__/", "*.pyc", "*.ipynb", "playground/", "poetry.lock", "dist/", "build/"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

### Comparing `ng_data_pipelines_sdk-1.3.0/PKG-INFO` & `ng_data_pipelines_sdk-1.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ng-data-pipelines-sdk
-Version: 1.3.0
+Version: 1.4.0
 Summary: A library for interacting with data from Amazon S3 through PySpark. Read, write and tranform data using a powerful and intuitive API with strong consistency and type checking, thanks to Pydantic. Compatible with Amazon MWAA running Airflow 2.7.2 and 2.8.1.
 Author: ng.cash
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

