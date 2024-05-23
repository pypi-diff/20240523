# Comparing `tmp/ng_data_pipelines_sdk-1.1.0.tar.gz` & `tmp/ng_data_pipelines_sdk-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-1.1.0.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-1.2.0.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-1.1.0.tar` & `ng_data_pipelines_sdk-1.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-05-23 12:53:01.549075 ng_data_pipelines_sdk-1.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-23 12:53:01.585075 ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     9155 2024-05-23 12:53:01.549075 ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-05-23 12:53:01.549075 ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    26361 2024-05-23 12:53:01.549075 ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0    20490 2024-05-23 12:53:01.549075 ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     5406 2024-05-23 12:53:01.550075 ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     4780 2024-05-23 12:53:01.550075 ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      838 2024-05-23 12:53:01.553075 ng_data_pipelines_sdk-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-05-23 13:28:14.223469 ng_data_pipelines_sdk-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 13:28:14.255469 ng_data_pipelines_sdk-1.2.0/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     9155 2024-05-23 13:28:14.223469 ng_data_pipelines_sdk-1.2.0/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-05-23 13:28:14.223469 ng_data_pipelines_sdk-1.2.0/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    26588 2024-05-23 13:28:14.223469 ng_data_pipelines_sdk-1.2.0/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0    20740 2024-05-23 13:28:14.223469 ng_data_pipelines_sdk-1.2.0/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     5406 2024-05-23 13:28:14.223469 ng_data_pipelines_sdk-1.2.0/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     4780 2024-05-23 13:28:14.224469 ng_data_pipelines_sdk-1.2.0/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      838 2024-05-23 13:28:14.226469 ng_data_pipelines_sdk-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-1.2.0/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/aws_interface.py` & `ng_data_pipelines_sdk-1.2.0/ng_data_pipelines_sdk/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-1.2.0/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,16 @@
             df_params (InputDataFrameParams): The parameters for reading the DataFrame.
 
         Returns:
             DataFrame: The read DataFrame.
 
         """
         bucket_url = self._get_bucket_url(input_df_params.dataframe_bucket_params)
+        full_base_path = f"{bucket_url}/{input_df_params.dataframe_base_path}"
+
         if input_df_params.dataframe_specific_paths:
             if isinstance(input_df_params.dataframe_specific_paths, list):
                 paths = [
                     f"{bucket_url}/{path}"
                     for path in input_df_params.dataframe_specific_paths
                 ]
             else:
@@ -154,14 +156,19 @@
             paths = generate_date_paths(
                 base_path=f"{bucket_url}/{input_df_params.dataframe_base_path}",
                 dates=input_df_params.read_date_params.read_dates,
                 year_partition=date_partitions.get(DatePartition.YEAR, "year"),
                 month_partition=date_partitions.get(DatePartition.MONTH, "month"),
                 day_partition=date_partitions.get(DatePartition.DAY, "day"),
             )
+
+            # Prevent pyspark from adding date columns to the DataFrame
+            if not input_df_params.read_date_params.add_all_date_columns:
+                full_base_path = None
+
         else:
             paths = f"{bucket_url}/{input_df_params.dataframe_base_path}"
 
         if input_df_params.pyspark_schema_struct:
             schema = self.convert_schema_object_to_pyspark_schema(
                 schema_object=input_df_params.pyspark_schema_struct
             )
@@ -173,15 +180,15 @@
         if verbose:
             logger.info("Starting read operation.")
 
         df = self.spark_manager.read(
             env=input_df_params.dataframe_bucket_params.env,
             paths=paths,
             file_type=input_df_params.dataframe_file_type,
-            base_path=f"{bucket_url}/{input_df_params.dataframe_base_path}",
+            base_path=full_base_path,
             schema=schema,
             cache=cache,
         )
 
         if verbose:
             logger.info("Read operation completed successfully.\n")
```

### Comparing `ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/interfaces.py` & `ng_data_pipelines_sdk-1.2.0/ng_data_pipelines_sdk/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,28 +260,32 @@
             A dictionary that maps DatePartition enum values to their corresponding string representations.
             The default value is:
             {
                 DatePartition.YEAR: "year",
                 DatePartition.MONTH: "month",
                 DatePartition.DAY: "day",
             }
+        add_all_date_columns (bool):
+            Whether to add all date columns to the DataFrame. If set to True, the DataFrame will have columns for year, month, and day.
+            The default value is True.
     """
 
     read_dates: Union[
         Sequence[Union[Union[str, datetime], List[Union[str, datetime]]]],
         datetime,
         Literal["{{processing_date}}"],
     ] = "{{processing_date}}"
     processing_date_offset_days: Optional[int] = None
     was_offset_applied: bool = False
     date_partitions: dict[DatePartition, str] = {
         DatePartition.YEAR: "year",
         DatePartition.MONTH: "month",
         DatePartition.DAY: "day",
     }
+    add_all_date_columns: bool = True
 
     @model_validator(mode="before")
     def validate_offset_and_read_dates(cls, data):
         read_dates = data.get("read_dates")
         processing_date_offset_days = data.get("processing_date_offset_days")
 
         if processing_date_offset_days is not None:
```

### Comparing `ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/spark_manager.py` & `ng_data_pipelines_sdk-1.2.0/ng_data_pipelines_sdk/spark_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.1.0/ng_data_pipelines_sdk/utils.py` & `ng_data_pipelines_sdk-1.2.0/ng_data_pipelines_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-1.1.0/pyproject.toml` & `ng_data_pipelines_sdk-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ng-data-pipelines-sdk"
-version = "1.1.0"
+version = "1.2.0"
 description = "A library for interacting with data from Amazon S3 through PySpark. Read, write and tranform data using a powerful and intuitive API with strong consistency and type checking, thanks to Pydantic. Compatible with Amazon MWAA running Airflow 2.7.2 and 2.8.1."
 authors = ["ng.cash"]
 readme = "README.md"
 exclude = [".git/", ".gitignore", "tests/", "docs/", "*.yml", "__pycache__/", "*.pyc", "*.ipynb", "playground/", "poetry.lock", "dist/", "build/"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

### Comparing `ng_data_pipelines_sdk-1.1.0/PKG-INFO` & `ng_data_pipelines_sdk-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ng-data-pipelines-sdk
-Version: 1.1.0
+Version: 1.2.0
 Summary: A library for interacting with data from Amazon S3 through PySpark. Read, write and tranform data using a powerful and intuitive API with strong consistency and type checking, thanks to Pydantic. Compatible with Amazon MWAA running Airflow 2.7.2 and 2.8.1.
 Author: ng.cash
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

