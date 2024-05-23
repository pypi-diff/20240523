# Comparing `tmp/ng_data_pipelines_sdk-1.0.0.tar.gz` & `tmp/ng_data_pipelines_sdk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-1.0.0.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-1.1.0.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-1.0.0.tar` & `ng_data_pipelines_sdk-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-05-22 20:58:59.906701 ng_data_pipelines_sdk-1.0.0/README.md
--rw-r--r--   0        0        0        0 2024-05-22 20:58:59.939702 ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     9155 2024-05-22 20:58:59.906701 ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-05-22 20:58:59.906701 ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    26078 2024-05-22 20:58:59.906701 ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0    19492 2024-05-22 20:58:59.906701 ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     5406 2024-05-22 20:58:59.906701 ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     4780 2024-05-22 20:58:59.906701 ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      838 2024-05-22 20:58:59.910702 ng_data_pipelines_sdk-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-05-23 12:53:01.549075 ng_data_pipelines_sdk-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 12:53:01.585075 ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     9155 2024-05-23 12:53:01.549075 ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-05-23 12:53:01.549075 ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    26361 2024-05-23 12:53:01.549075 ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0    20490 2024-05-23 12:53:01.549075 ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     5406 2024-05-23 12:53:01.550075 ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     4780 2024-05-23 12:53:01.550075 ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      838 2024-05-23 12:53:01.553075 ng_data_pipelines_sdk-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-1.1.0/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/aws_interface.py` & `ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pyspark.sql.types import StructType
 
 from ng_data_pipelines_sdk.aws_interface import AWSInterface
 from ng_data_pipelines_sdk.custom_logger import logger
 from ng_data_pipelines_sdk.interfaces import (
     DATE_FORMATTER,
     DataFrameDict,
+    DatePartition,
     EmptyDataFrameException,
     FileType,
     FnKind,
     InputDataFrameParams,
     InputDataFrameParamsDict,
     OutputDataFrameParams,
     OutputDataFrameParamsDict,
@@ -145,17 +146,21 @@
                 paths = [
                     f"{bucket_url}/{path}"
                     for path in input_df_params.dataframe_specific_paths
                 ]
             else:
                 paths = f"{bucket_url}/{input_df_params.dataframe_specific_paths}"
         elif input_df_params.read_date_params:
+            date_partitions = input_df_params.read_date_params.date_partitions
             paths = generate_date_paths(
                 base_path=f"{bucket_url}/{input_df_params.dataframe_base_path}",
                 dates=input_df_params.read_date_params.read_dates,
+                year_partition=date_partitions.get(DatePartition.YEAR, "year"),
+                month_partition=date_partitions.get(DatePartition.MONTH, "month"),
+                day_partition=date_partitions.get(DatePartition.DAY, "day"),
             )
         else:
             paths = f"{bucket_url}/{input_df_params.dataframe_base_path}"
 
         if input_df_params.pyspark_schema_struct:
             schema = self.convert_schema_object_to_pyspark_schema(
                 schema_object=input_df_params.pyspark_schema_struct
@@ -487,19 +492,18 @@
         for _, df_params in step_params.input_dataframes_params.items():
             if df_params.read_date_params:
                 df_params.read_date_params.was_offset_applied = False
 
                 if df_params.read_date_params.read_dates == "{{processing_date}}":
                     df_params.read_date_params.read_dates = processing_date
 
-                    if df_params.read_date_params.processing_date_offset_days != 0:
+                    offset = df_params.read_date_params.processing_date_offset_days
+                    if offset and offset != 0:
                         df_params.read_date_params.read_dates
-                        +timedelta(
-                            days=df_params.read_date_params.processing_date_offset_days
-                        )
+                        +timedelta(days=offset)
                         df_params.read_date_params.was_offset_applied = True
 
         if step_params.output_dataframes_params:
             for _, df_params in step_params.output_dataframes_params.items():
                 if (
                     df_params.single_write_date
                     and df_params.single_write_date.single_write_date
```

### Comparing `ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/interfaces.py` & `ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/interfaces.py`

 * *Files 5% similar despite different names*

```diff
@@ -245,67 +245,104 @@
 
         return v
 
 
 class ReadDateParams(BaseModelJsonDumps):
     """
     Represents the parameters for reading dates in a data pipeline.
-
     Attributes:
         read_dates (Union[List[datetime], datetime, Literal["{{processing_date}}"], Literal["{{processing_date_previous}}"]]):
             The dates to be read. It can be a list of datetimes, a single datetime, or special placeholders for processing dates.
             The default value is "{{processing_date}}".
         processing_date_offset_days (int):
             The offset to be applied to the processing date. It represents the number of days to add or subtract from the processing date.
             The default value is 0.
-        date_partitions (List[str]):
-            The date partitions to be included in the read. It is a list of strings representing the desired partitions, such as "year", "month", "day".
-            The default value is ["year", "month", "day"].
-        date_partitions_first (bool):
-            Specifies whether the date partitions should be added as the first columns in the read data.
-            The default value is True.
-        add_all_date_columns (bool):
-            Specifies whether all date columns should be added to the read data.
-            The default value is True.
+        date_partitions (dict[DatePartition, str]):
+            A dictionary that maps DatePartition enum values to their corresponding string representations.
+            The default value is:
+            {
+                DatePartition.YEAR: "year",
+                DatePartition.MONTH: "month",
+                DatePartition.DAY: "day",
+            }
     """
 
     read_dates: Union[
         Sequence[Union[Union[str, datetime], List[Union[str, datetime]]]],
         datetime,
         Literal["{{processing_date}}"],
     ] = "{{processing_date}}"
-    processing_date_offset_days: int = 0
+    processing_date_offset_days: Optional[int] = None
     was_offset_applied: bool = False
-    date_partitions: List[str] = ["year", "month", "day"]
-    date_partitions_first: bool = True
-    add_all_date_columns: bool = True
+    date_partitions: dict[DatePartition, str] = {
+        DatePartition.YEAR: "year",
+        DatePartition.MONTH: "month",
+        DatePartition.DAY: "day",
+    }
+
+    @model_validator(mode="before")
+    def validate_offset_and_read_dates(cls, data):
+        read_dates = data.get("read_dates")
+        processing_date_offset_days = data.get("processing_date_offset_days")
+
+        if processing_date_offset_days is not None:
+            if read_dates != "{{processing_date}}":
+                raise ValueError(
+                    "If 'processing_date_offset_days' is provided, 'read_dates' must be '{{processing_date}}'"
+                )
+
+        return data
+
+    @field_validator("date_partitions")
+    def ensure_all_date_partitions(
+        cls, v: dict[DatePartition, str]
+    ) -> dict[DatePartition, str]:
+        """
+        Ensures that all date partitions are present in the input dictionary.
+
+        Args:
+            v (dict[DatePartition, str]): The input dictionary.
+
+        Returns:
+            dict[DatePartition, str]: The input dictionary.
+
+        Raises:
+            ValueError: If any date partition is missing.
+        """
+        date_partitions = [DatePartition.YEAR, DatePartition.MONTH, DatePartition.DAY]
+
+        for date_partition in date_partitions:
+            if date_partition not in v:
+                raise ValueError(
+                    f"Missing date partition: '{date_partition}'. The dictionary must contain all date partitions: {date_partitions}"
+                )
+
+        return v
 
 
 class InputDataFrameParams(DataFrameBaseParams):
     """
     Parameters for input data frames.
 
     Attributes:
         pyspark_schema_struct (Optional[Dict[str, Any]]): The schema of the input data frame in PySpark StructType format.
         s3_schema_path_params (Optional[S3ReadSchemaParams]): The parameters for reading the schema from an S3 path.
         read_date_params (Optional[ReadDateParams]): The parameters for reading the date from the input data frame.
-        column_partitions (Optional[List[str]]): The list of column names to be used for partitioning the input data frame.
 
     Methods:
         check_schema_mode(cls, data): Check the schema mode and validate the input data.
 
     Raises:
         ValueError: If 'pyspark_schema_struct' and 's3_schema_path_params' are passed together.
     """
 
     dataframe_specific_paths: Optional[Union[List[str], str]] = None
     pyspark_schema_struct: Optional[Dict[str, Any]] = None
     s3_schema_path_params: Optional[S3ReadSchemaParams] = None
     read_date_params: Optional[ReadDateParams] = None
-    column_partitions: Optional[List[str]] = None
 
     @model_validator(mode="before")
     def check_schema_mode(cls, data):
         """
         Check the schema mode and validate the input data.
 
         Args:
```

### Comparing `ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/spark_manager.py` & `ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/spark_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/utils.py` & `ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.0.0/pyproject.toml` & `ng_data_pipelines_sdk-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ng-data-pipelines-sdk"
-version = "1.0.0"
+version = "1.1.0"
 description = "A library for interacting with data from Amazon S3 through PySpark. Read, write and tranform data using a powerful and intuitive API with strong consistency and type checking, thanks to Pydantic. Compatible with Amazon MWAA running Airflow 2.7.2 and 2.8.1."
 authors = ["ng.cash"]
 readme = "README.md"
 exclude = [".git/", ".gitignore", "tests/", "docs/", "*.yml", "__pycache__/", "*.pyc", "*.ipynb", "playground/", "poetry.lock", "dist/", "build/"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

### Comparing `ng_data_pipelines_sdk-1.0.0/PKG-INFO` & `ng_data_pipelines_sdk-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ng-data-pipelines-sdk
-Version: 1.0.0
+Version: 1.1.0
 Summary: A library for interacting with data from Amazon S3 through PySpark. Read, write and tranform data using a powerful and intuitive API with strong consistency and type checking, thanks to Pydantic. Compatible with Amazon MWAA running Airflow 2.7.2 and 2.8.1.
 Author: ng.cash
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

