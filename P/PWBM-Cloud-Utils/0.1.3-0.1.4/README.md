# Comparing `tmp/PWBM_Cloud_Utils-0.1.3.tar.gz` & `tmp/pwbm_cloud_utils-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PWBM_Cloud_Utils-0.1.3.tar", last modified: Fri Mar 29 14:06:09 2024, max compression
+gzip compressed data, was "pwbm_cloud_utils-0.1.4.tar", last modified: Thu May 23 15:09:15 2024, max compression
```

## Comparing `PWBM_Cloud_Utils-0.1.3.tar` & `pwbm_cloud_utils-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 14:06:09.474839 PWBM_Cloud_Utils-0.1.3/
--rw-rw-rw-   0        0        0     1091 2023-11-06 14:05:57.000000 PWBM_Cloud_Utils-0.1.3/LICENSE
--rw-rw-rw-   0        0        0    31005 2024-03-29 14:06:09.474839 PWBM_Cloud_Utils-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    30242 2024-03-08 20:11:25.000000 PWBM_Cloud_Utils-0.1.3/README.md
--rw-rw-rw-   0        0        0      722 2024-03-28 21:46:11.000000 PWBM_Cloud_Utils-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-29 14:06:09.474839 PWBM_Cloud_Utils-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-29 14:06:09.396594 PWBM_Cloud_Utils-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2024-03-29 14:06:09.427639 PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils/
--rw-rw-rw-   0        0        0      293 2024-03-21 20:38:35.000000 PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils/__init__.py
--rw-rw-rw-   0        0        0     7238 2024-03-28 21:43:20.000000 PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils/api_functions.py
--rw-rw-rw-   0        0        0     2715 2024-03-28 21:43:20.000000 PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils/cloud_main.py
--rw-rw-rw-   0        0        0      389 2024-03-21 20:33:49.000000 PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils/cloud_utils.py
--rw-rw-rw-   0        0        0     2401 2024-03-28 21:43:20.000000 PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils/entities.py
--rw-rw-rw-   0        0        0     2966 2024-03-28 21:44:54.000000 PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils/io_config.py
--rw-rw-rw-   0        0        0    26147 2024-03-21 19:49:35.000000 PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils/io_reader.py
--rw-rw-rw-   0        0        0    26568 2024-03-21 19:49:35.000000 PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils/io_writer.py
--rw-rw-rw-   0        0        0     2507 2024-03-08 20:43:44.000000 PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils/upload_test_github.py
-drwxrwxrwx   0        0        0        0 2024-03-29 14:06:09.474839 PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils.egg-info/
--rw-rw-rw-   0        0        0    31005 2024-03-29 14:06:09.000000 PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      735 2024-03-29 14:06:09.000000 PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 14:06:09.000000 PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-03-29 14:06:09.000000 PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-03-29 14:06:09.000000 PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-29 14:06:09.459257 PWBM_Cloud_Utils-0.1.3/src/tests/
--rw-rw-rw-   0        0        0        0 2024-03-11 21:18:01.000000 PWBM_Cloud_Utils-0.1.3/src/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 14:06:09.474839 PWBM_Cloud_Utils-0.1.3/src/tests/data/
--rw-rw-rw-   0        0        0      259 2024-03-05 21:23:16.000000 PWBM_Cloud_Utils-0.1.3/src/tests/data/Person.py
--rw-rw-rw-   0        0        0     3540 2024-03-21 19:49:35.000000 PWBM_Cloud_Utils-0.1.3/src/tests/test_cache.py
--rw-rw-rw-   0        0        0     9853 2024-03-08 20:11:25.000000 PWBM_Cloud_Utils-0.1.3/src/tests/test_config.py
--rw-rw-rw-   0        0        0    39613 2024-03-21 19:49:35.000000 PWBM_Cloud_Utils-0.1.3/src/tests/test_local.py
--rw-rw-rw-   0        0        0      496 2024-03-22 19:45:20.000000 PWBM_Cloud_Utils-0.1.3/src/tests/test_main.py
--rw-rw-rw-   0        0        0    41431 2024-03-21 19:49:35.000000 PWBM_Cloud_Utils-0.1.3/src/tests/test_s3.py
+drwxrwxrwx   0        0        0        0 2024-05-23 15:09:15.879534 pwbm_cloud_utils-0.1.4/
+-rw-rw-rw-   0        0        0     1091 2023-11-06 14:05:57.000000 pwbm_cloud_utils-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0    31334 2024-05-23 15:09:15.874534 pwbm_cloud_utils-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    30534 2024-05-07 17:54:10.000000 pwbm_cloud_utils-0.1.4/README.md
+-rw-rw-rw-   0        0        0      751 2024-05-23 15:07:33.000000 pwbm_cloud_utils-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 15:09:15.880532 pwbm_cloud_utils-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 15:09:15.753354 pwbm_cloud_utils-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 15:09:15.800530 pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils/
+-rw-rw-rw-   0        0        0      400 2024-05-07 17:54:10.000000 pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils/__init__.py
+-rw-rw-rw-   0        0        0     7771 2024-05-07 17:55:04.000000 pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils/api_functions.py
+-rw-rw-rw-   0        0        0     2715 2024-03-28 21:43:20.000000 pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils/cloud_main.py
+-rw-rw-rw-   0        0        0      906 2024-04-04 20:17:35.000000 pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils/cloud_utils.py
+-rw-rw-rw-   0        0        0     2415 2024-05-07 17:55:04.000000 pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils/entities.py
+-rw-rw-rw-   0        0        0    18182 2024-05-22 18:07:44.000000 pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils/file_manager.py
+-rw-rw-rw-   0        0        0     5178 2024-05-22 18:07:44.000000 pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils/io_base.py
+-rw-rw-rw-   0        0        0     2214 2024-05-07 17:54:10.000000 pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils/io_config.py
+-rw-rw-rw-   0        0        0    17919 2024-05-22 18:07:44.000000 pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils/io_reader.py
+-rw-rw-rw-   0        0        0    17740 2024-05-22 18:07:44.000000 pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils/io_writer.py
+-rw-rw-rw-   0        0        0    15388 2024-05-22 18:07:44.000000 pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils/scripting_functions.py
+-rw-rw-rw-   0        0        0     2507 2024-03-08 20:43:44.000000 pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils/upload_test_github.py
+drwxrwxrwx   0        0        0        0 2024-05-23 15:09:15.871531 pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils.egg-info/
+-rw-rw-rw-   0        0        0    31334 2024-05-23 15:09:15.000000 pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1111 2024-05-23 15:09:15.000000 pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 15:09:15.000000 pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2024-05-23 15:09:15.000000 pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-23 15:09:15.000000 pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 15:09:15.863533 pwbm_cloud_utils-0.1.4/src/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-11 21:18:01.000000 pwbm_cloud_utils-0.1.4/src/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 15:09:15.866533 pwbm_cloud_utils-0.1.4/src/tests/data/
+-rw-rw-rw-   0        0        0      311 2024-05-22 18:07:44.000000 pwbm_cloud_utils-0.1.4/src/tests/data/Person.py
+-rw-rw-rw-   0        0        0      430 2024-05-22 18:07:44.000000 pwbm_cloud_utils-0.1.4/src/tests/helpers_testing.py
+-rw-rw-rw-   0        0        0     2612 2024-05-22 18:07:44.000000 pwbm_cloud_utils-0.1.4/src/tests/test_cache.py
+-rw-rw-rw-   0        0        0      496 2024-04-10 18:09:11.000000 pwbm_cloud_utils-0.1.4/src/tests/test_cloud_main.py
+-rw-rw-rw-   0        0        0      715 2024-04-05 12:51:45.000000 pwbm_cloud_utils-0.1.4/src/tests/test_cloud_utils.py
+-rw-rw-rw-   0        0        0     3450 2024-05-22 18:07:44.000000 pwbm_cloud_utils-0.1.4/src/tests/test_config.py
+-rw-rw-rw-   0        0        0    11931 2024-05-22 18:07:44.000000 pwbm_cloud_utils-0.1.4/src/tests/test_io_base.py
+-rw-rw-rw-   0        0        0     9666 2024-05-07 17:54:10.000000 pwbm_cloud_utils-0.1.4/src/tests/test_local_file_manager.py
+-rw-rw-rw-   0        0        0    21579 2024-05-22 18:07:44.000000 pwbm_cloud_utils-0.1.4/src/tests/test_local_reader.py
+-rw-rw-rw-   0        0        0    23701 2024-05-22 18:07:44.000000 pwbm_cloud_utils-0.1.4/src/tests/test_local_writer.py
+-rw-rw-rw-   0        0        0    10909 2024-05-07 17:54:10.000000 pwbm_cloud_utils-0.1.4/src/tests/test_s3_file_manager.py
+-rw-rw-rw-   0        0        0    21423 2024-05-22 18:07:44.000000 pwbm_cloud_utils-0.1.4/src/tests/test_s3_reader.py
+-rw-rw-rw-   0        0        0    22423 2024-05-22 18:07:44.000000 pwbm_cloud_utils-0.1.4/src/tests/test_s3_writer.py
+-rw-rw-rw-   0        0        0    16335 2024-05-22 18:07:44.000000 pwbm_cloud_utils-0.1.4/src/tests/test_scripting.py
```

### Comparing `PWBM_Cloud_Utils-0.1.3/LICENSE` & `pwbm_cloud_utils-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PWBM_Cloud_Utils-0.1.3/PKG-INFO` & `pwbm_cloud_utils-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: PWBM_Cloud_Utils
-Version: 0.1.3
+Version: 0.1.4
 Summary: connect to read/write data to s3
 Author-email: "Yunye Jiang, Mariko Paulson, Chris Palenchar" <yunyej@wharton.upenn.edu>
 Project-URL: Homepage, https://github.com/PennWhartonBudgetModel/PWBM_Cloud_Utils
 Project-URL: Bug Tracker, https://github.com/PennWhartonBudgetModel/PWBM_Cloud_Utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3
 Requires-Dist: pandas
 Requires-Dist: python-dotenv
 Requires-Dist: requests
-Requires-Dist: fastparquet
 Requires-Dist: pyarrow
+Requires-Dist: typing-extensions
+Requires-Dist: s3fs>=2023.3.0
 
 # PWBM_Cloud_Utils
 
 ## Introduction
 This Python module provides a convenient interface for handling input/output configurations, reading from different sources (local or cloud), and writing data to cloud storage (Amazon S3) or locally. It is designed to be flexible, supporting various data formats and compression options.
 
+Note that the package officially supports `pyarrow` as the engine to work with parquet
+files. This is because `pandas` is adopting `pyarrow` for more efficient memory
+representation since Version 2.0. The code may still work with `fastparquet`, but
+it will not be supported officially.
+
 ## Installation
 To use this module, ensure that you have the required dependencies installed. You can install them using the following command:
 ```bash
 pip install PWBM_Cloud_Utils
 ```
 or
 ```bash
```

### Comparing `PWBM_Cloud_Utils-0.1.3/README.md` & `pwbm_cloud_utils-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # PWBM_Cloud_Utils
 
 ## Introduction
 This Python module provides a convenient interface for handling input/output configurations, reading from different sources (local or cloud), and writing data to cloud storage (Amazon S3) or locally. It is designed to be flexible, supporting various data formats and compression options.
 
+Note that the package officially supports `pyarrow` as the engine to work with parquet
+files. This is because `pandas` is adopting `pyarrow` for more efficient memory
+representation since Version 2.0. The code may still work with `fastparquet`, but
+it will not be supported officially.
+
 ## Installation
 To use this module, ensure that you have the required dependencies installed. You can install them using the following command:
 ```bash
 pip install PWBM_Cloud_Utils
 ```
 or
 ```bash
```

### Comparing `PWBM_Cloud_Utils-0.1.3/pyproject.toml` & `pwbm_cloud_utils-0.1.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "PWBM_Cloud_Utils"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Yunye Jiang, Mariko Paulson, Chris Palenchar", email="yunyej@wharton.upenn.edu" },
 ]
 description = "connect to read/write data to s3"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -13,14 +13,15 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "boto3",
     "pandas",
     "python-dotenv",
     "requests",
-    "fastparquet",
     "pyarrow",
+    "typing-extensions",
+    "s3fs>=2023.3.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/PennWhartonBudgetModel/PWBM_Cloud_Utils"
 "Bug Tracker" = "https://github.com/PennWhartonBudgetModel/PWBM_Cloud_Utils/issues"
```

### Comparing `PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils/api_functions.py` & `pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils/api_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,16 @@
         Returns:
             dict: The JSON response from the API.
         """
         url = f"{self.base_url}/{endpoint}"
         # The optional parameters are handled by the requests package, whose default values
         # are None in the package. See Session.request() for more information.
         response = requests.request(method, url, json=data, files=files)
+        response.raise_for_status()
+        
         return response.json()
 
 
 class ScenarioAPI(APIClient):
 
     def get_scenario_by_id(self, scenario_id: int) -> ScenarioData:
         """
@@ -60,30 +62,45 @@
         Returns:
             ScenarioData: An instance of ScenarioData containing the retrieved scenario details.
         """
         endpoint = f"scenario/{scenario_id}"
         response_data = self._make_request("GET", endpoint)
         return ScenarioData(**response_data)
 
-    def create_scenario(self, scenario_data: ScenarioUploadData) -> ScenarioData:
+    def create_scenario(self, scenario_data: ScenarioUploadData) -> dict:
         """
         Create a scenario using the provided scenario_data.
 
         Args:
             scenario_data (ScenarioData): An instance of ScenarioData containing the data for the new scenario.
 
         Returns:
             ScenarioData: An instance of ScenarioData containing the created scenario details.
         """
-        endpoint = "scenario/"
-        params = dataclasses.asdict(scenario_data)
-        files = {"file": scenario_data.file} if scenario_data.file else None
-        response_data = self._make_request("PUT", endpoint, data=params, files=files)
-        return ScenarioData(**response_data)
+        parent_id = scenario_data.parent_id if scenario_data.parent_id else 0
+        endpoint = f"scenario/?parent_id={parent_id}&model_id={scenario_data.model_id}"
+
+        files = {"file": (scenario_data.folder_name, scenario_data.file)} if scenario_data.file else None
+
+        response_data = self._make_request("PUT", endpoint, files=files)
+        return response_data
+
+    def execute_scenario(self, scenario_id: int) -> dict:
+        """
+        Retrieve a scenario by its ID on cloud.
 
+        Args:
+            scenario_id: The ID of the scenario.
+
+        Returns:
+            information associated with the run
+        """
+        endpoint = f"scenario/execute/{scenario_id}"
+        response = self._make_request("POST", endpoint)
+        return response
 
 # TODO Currently not in use
 class RunListAPI(APIClient):
     def get_run_list(self, run_list_id):
         return self._make_request("GET", f"run_list/{run_list_id}")
 
     def get_run_list_output_path(self, run_list_id, policy_id):
```

### Comparing `PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils/cloud_main.py` & `pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils/cloud_main.py`

 * *Files identical despite different names*

### Comparing `PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils/entities.py` & `pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,18 @@
     Attributes:
         parent_id : The ID of the parent scenario folder.
         model_id : The ID of the model associated with the scenario.
         folder_name ： The name of the folder containing the scenario files.
         file : The binary content of the scenario file.
     """
 
-    parent_id: int
     model_id: int
     folder_name: str | None
     file: bytes | None
+    parent_id: int | None = None
 
 @dataclass
 class ScenarioData:
     """
     Represents data for a scenario.
 
     Attributes:
```

### Comparing `PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils/io_config.py` & `pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils/io_config.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,28 +9,30 @@
     local_read_basepath: str | None
     local_write_basepath: str | None
     cloud_cache_basepath: str | None
     cloud_execution: bool
 
     def __init__(self):
         """
-        Constructor for IOConfig. IOConfig uses the local .env file to set config settings. Some settings are overridable with the constructor.
+        Constructor for IOConfig. IOConfig uses the local .env file to set config 
+        settings. Some settings are overridable with the constructor.
         """
         load_dotenv(".env")
 
         # TODO: also edit yaml in WITS_API (was CloudData)
         cloud_exec_key = "CLOUD_EXECUTION"
         if cloud_exec_key in os.environ:
             if os.environ[cloud_exec_key].upper() == "TRUE":
                 self.cloud_execution = True
             elif os.environ[cloud_exec_key].upper() == "FALSE":
                 self.cloud_execution = False
             else:
                 raise AssertionError(
-                    f'Environment Variable {cloud_exec_key} value of "{os.environ[cloud_exec_key]}" is not a proper boolean.  Use "True" or "False".'
+                    f'Environment Variable {cloud_exec_key} value of '
+                    f'"{os.environ[cloud_exec_key]}" is not a proper boolean.  Use "True" or "False".'
                 )
         else:
             self.cloud_execution = False
        
         # TODO: also edit yaml in WITS_API (was aws_model_bucket)
         if "CLOUD_READ_BASEPATH" in os.environ:
             self.cloud_read_basepath = os.environ["CLOUD_READ_BASEPATH"]
@@ -52,29 +54,7 @@
         else:
             self.local_write_basepath = None
 
         if "CLOUD_CACHE_BASEPATH" in os.environ:
             self.cloud_cache_basepath = os.environ["CLOUD_CACHE_BASEPATH"]
         else:
             self.cloud_cache_basepath = None
-
-        
-    
-    @staticmethod
-    def parse_s3_path(s3_path: str) -> tuple:
-        """
-        Read given S3 URI path into a tuple with bucket name and path. Returns None if path does not match S3 URI format.
-    
-        Attributes:
-            s3_path: S3 URI path to the file/folder, including file name and extension.
-        
-        Returns:
-            tuple: first item is string bucket name and second item is string path
-        """
-        # Bucket names can consist only of lowercase letters, numbers, dots (.), and hyphens (-).
-        p = re.compile(r'^[sS]3:\/\/(?P<bucket>(\d|[a-z]|-|\.)+)\/(?P<path>.*)$')
-
-        m = p.match(s3_path)
-        if m:
-            return (m.group('bucket'), m.group('path'))
-        else:
-            return None
```

### Comparing `PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils/io_reader.py` & `pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils/io_reader.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,125 +1,82 @@
-import shutil 
 import os
-import io
+import sys
+import tarfile
+import zipfile
 from typing import Any
-import boto3
 import botocore
 import gzip
 import pickle
 import pandas as pd
-import re
-import tempfile
+
+from .io_base import IOBase
 from .io_config import IOConfig
 
-class IOReader:
+class IOReader(IOBase):
     def __init__(
         self, 
         cloud_basepath: str | None = None,
         local_basepath: str | None = None,
     ) -> None:
         """
-        Constructor for IOReader. IOReader allows you to read files from either the cloud_baspath location or the local_basepath, depending on where your code is executing. By default, the basepaths defined in your .env file will be used but you can override those using the constructor arguments.
+        Constructor for IOReader. IOReader allows you to read files from either the 
+        cloud_baspath location or the local_basepath, depending on where your code is executing. 
+        By default, the basepaths defined in your .env file will be used but you can override 
+        those using the constructor arguments.
     
         Attributes:
             cloud_basepath: basepath to use with reader when executing on the cloud.
             local_basepath: basepath to use with reader when executing locally.
         
         """
         config = IOConfig()
-        self.resource = boto3.resource("s3")
-        self.client = boto3.client("s3")
         self.cloud_execution = config.cloud_execution
 
         if config.cloud_execution:
             self.basepath = cloud_basepath
             self.cloud_cache_basepath = config.cloud_cache_basepath
             if self.basepath is None:
                 self.basepath = config.cloud_read_basepath
         else:
             self.basepath = local_basepath
             self.cloud_cache_basepath = None
             if self.basepath is None:
                 self.basepath = config.local_read_basepath
-
-
-    def check_extension(self, path: str, ext: str) -> bool:
-        """
-        Helper for checking if the path has the given extension
-
-        Attributes:
-            path: either an absolute path or a relative path to a file
-            ext: extension you are looking for. should not include leading "." (ie "csv" or "pkl.gz")
-        
-        Returns:
-            bool: True if the path has the extension
-        """
-        if not re.search(r'^\..*', ext):
-            ext = f".{ext}"
-        return re.search(f'.+{ext}$', path) is not None
-
-    def get_absolute_path(self, path: str, *, basepath: str | None = None) -> str:
-        """
-        Gets absolute path by joining the given path to either the IOReader's basepath by default or the given basepath if specified. See IOReader constructor for more info about the basepath.
-    
-        Attributes:
-            path: relative path to a file or a folder. To reference the root of the basepath, either "." or "" accepted.
-            basepath: Optional basepath to override IOReader's basepath. Defaults to None.
-        
-        Returns:
-            str: absolute path from joining path to basepath.
-        """
-        if basepath is None:
-            if self.basepath is None:
-                raise ValueError("No basepath set.")
-            basepath = self.basepath
-        if len(path) > 0 and path[0] == ".":
-            path = path[1:]
-        return os.path.join(basepath, path).replace("\\","/")
     
     def read_bytes(
         self, 
         path: str | None = None, 
         /, *, # before positional, after keyword
         abspath: str | None = None,
         decompress: bool = False,
     ) -> bytes:
         """
         Read file specified by path or abspath and return its contents as a byte string.
     
         Attributes:
-            path: Relative path to the file from within the IOReader's basepath directory, including file name and extension. path ignored if abspath specified, so either specify path or abspath not both. Positional only.
-            abspath: Absolute path to the file, including file name and extension. If file is on S3, use the format "s3://bucket/key". path ignored if abspath specified, so either specify path or abspath not both. Keyword only.
+            path: Relative path to the file from within the IOReader's basepath directory, 
+                  including file name and extension. path ignored if abspath specified, 
+                  so either specify path or abspath not both. Positional only.
+            abspath: Absolute path to the file, including file name and extension. 
+                     If file is on S3, use the format "s3://bucket/key". path ignored 
+                     if abspath specified, so either specify path or abspath not both. 
+                     Keyword only.
             decompress: Whether to decompress file using gzip. By default, False. Keyword only.
         
         Returns:
             bytes: byte string of file contents.
         """
-        if abspath is None:
-            if path is None:
-                raise ValueError("No path or abspath set.")
-            # uses config to build full absolute path
-            abspath = self.get_absolute_path(path)
 
-        # tries to parse S3 info from abspath
-        path_tuple = IOConfig.parse_s3_path(abspath)
+        file_manager = self._get_file_manager(path, abspath=abspath)
+
+        file_obj = file_manager.read_bytes()
+
+        response = file_obj.read()
+        file_obj.close()
 
-        if path_tuple is not None:
-            # data on S3
-            bucket_name = path_tuple[0]
-            path = path_tuple[1]
-
-            response_body = io.BytesIO()
-            self.resource.Object(bucket_name, path.replace("\\","/")).download_fileobj(response_body)
-            response = response_body.getvalue()
-        else:
-            # data on network or local drive
-            with open(abspath, "rb") as f:
-                response = f.read()
-        
         if decompress:
             response = gzip.decompress(response)
         
         return response
 
     def read(
         self, 
@@ -128,16 +85,21 @@
         abspath: str | None = None,
         decompress: bool = False, 
     ) -> str:
         """
         Read file specified by path or abspath and return its contents as a string.
 
         Attributes:
-            path: Relative path to the file from within the IOReader's basepath directory, including file name and extension. path ignored if abspath specified, so either specify path or abspath not both. Positional only.
-            abspath: Absolute path to the file, including file name and extension. If file is on S3, use the format "s3://bucket/key". path ignored if abspath specified, so either specify path or abspath not both. Keyword only.
+            path: Relative path to the file from within the IOReader's basepath directory, 
+                  including file name and extension. path ignored if abspath specified, 
+                  so either specify path or abspath not both. Positional only.
+            abspath: Absolute path to the file, including file name and extension. 
+                     If file is on S3, use the format "s3://bucket/key". path ignored 
+                     if abspath specified, so either specify path or abspath not both. 
+                     Keyword only.
             decompress: Whether to decompress file using gzip. By default, False. Keyword only.
         
         Returns:
             str: string of file contents.
         """
         return self.read_bytes(
             path, 
@@ -149,19 +111,25 @@
         self, 
         path: str | None = None, 
         /, *, # before positional, after keyword
         abspath: str | None = None,
         decompress: bool = False, 
     ) -> list[str]:
         """
-        Read file specified by path or abspath and return its contents as a list of strings with one entry per line.
+        Read file specified by path or abspath and return its contents as a list of 
+        strings with one entry per line.
 
         Attributes:
-            path: Relative path to the file from within the IOReader's basepath directory, including file name and extension. path ignored if abspath specified, so either specify path or abspath not both. Positional only.
-            abspath: Absolute path to the file, including file name and extension. If file is on S3, use the format "s3://bucket/key". path ignored if abspath specified, so either specify path or abspath not both. Keyword only.
+            path: Relative path to the file from within the IOReader's basepath directory, 
+                  including file name and extension. path ignored if abspath specified, 
+                  so either specify path or abspath not both. Positional only.
+            abspath: Absolute path to the file, including file name and extension. 
+                     If file is on S3, use the format "s3://bucket/key". path ignored 
+                     if abspath specified, so either specify path or abspath not both. 
+                     Keyword only.
             decompress: Whether to decompress file using gzip. By default, False. Keyword only.
         
         Returns:
             list[str]: list of strings with one entry per line of file contents.
         """
         return self.read(
             path, 
@@ -173,19 +141,25 @@
         self, 
         path: str | None = None, 
         /, *, # before positional, after keyword
         abspath: str | None = None,
         decompress: bool = False, 
     ) -> Any:
         """
-        Read pickle file specified by path or abspath and return its unpickled contents. Note: if contents is a pandas Dataframe, please use read_df.
+        Read pickle file specified by path or abspath and return its unpickled contents. 
+        Note: if contents is a pandas Dataframe, please use read_df.
     
         Attributes:
-            path: Relative path to the file from within the IOReader's basepath directory, including file name and extension. path ignored if abspath specified, so either specify path or abspath not both. Positional only.
-            abspath: Absolute path to the file, including file name and extension. If file is on S3, use the format "s3://bucket/key". path ignored if abspath specified, so either specify path or abspath not both. Keyword only.
+            path: Relative path to the file from within the IOReader's basepath directory, 
+                  including file name and extension. path ignored if abspath specified, 
+                  so either specify path or abspath not both. Positional only.
+            abspath: Absolute path to the file, including file name and extension. 
+                     If file is on S3, use the format "s3://bucket/key". path ignored 
+                     if abspath specified, so either specify path or abspath not both. 
+                     Keyword only.
             decompress: Whether to decompress file using gzip. By default, False. Keyword only.
         
         Returns:
             Any: unpickled file contents.
         """
         response = self.read_bytes(
             path, 
@@ -197,216 +171,169 @@
     def read_df(
         self, 
         path: str | None = None, 
         /, *, # before positional, after keyword
         abspath: str | None = None,
         decompress: bool = False, 
         filetype: str = "infer",
-        pandas_args: dict = {}
+        pandas_args: dict | None = None
     ) -> pd.DataFrame:
         """
-        Read file specified by path or abspath and return its contents as a pandas Dataframe. File type automatically determined from path. Note: only csv, pickle, and parquet files supported. If another file type needed, please use read_bytes or read_file.
+        Read file specified by path or abspath and return its contents as a pandas Dataframe. 
+        File type automatically determined from path. Note: only csv, pickle, and parquet files supported. 
+        If another file type needed, please use read_bytes or read_file.
     
         Attributes:
-            path: Relative path to the file from within the IOReader's basepath directory, including file name and extension. path ignored if abspath specified, so either specify path or abspath not both. Positional only.
-            abspath: Absolute path to the file, including file name and extension. If file is on S3, use the format "s3://bucket/key". path ignored if abspath specified, so either specify path or abspath not both. Keyword only.
+            path: Relative path to the file from within the IOReader's basepath directory, 
+                  including file name and extension. path ignored if abspath specified, 
+                  so either specify path or abspath not both. Positional only.
+            abspath: Absolute path to the file, including file name and extension. 
+                     If file is on S3, use the format "s3://bucket/key". path ignored 
+                     if abspath specified, so either specify path or abspath not both. 
+                     Keyword only.
             decompress: Whether to decompress file using gzip. By default, False. Keyword only.
-            filetype: File type of file being read. Possible values are: "csv", "pickle", "parquet", and "infer". Defaults to "infer", which means type is inferred from the path. Keyword only.
-            pandas_args: A dictionary of arguments to add when calling pandas function. Defaults to {}. Keyword only.
+            filetype: File type of file being read. Possible values are: "csv", "pickle", "parquet", 
+                      and "infer". Defaults to "infer", which means type is inferred from the path. 
+                      Keyword only.
+            pandas_args: A dictionary of arguments to add when calling pandas function. Defaults to {}. 
+                         Keyword only.
         
         Returns:
             pd.DataFrame: file contents as a pandas Dataframe.
         """
-        pd_args = pandas_args.copy()
+        if pandas_args is None:
+            pd_args = {}
+        else:
+            pd_args = pandas_args.copy()
 
         if abspath is None:
             if path is None:
                 raise ValueError("No path or abspath set.")
             # uses config to build full absolute path
             abspath = self.get_absolute_path(path)
 
-        # tries to parse S3 info from abspath
-        path_tuple = IOConfig.parse_s3_path(abspath)
+        file_manager = self._get_file_manager(abspath=abspath)
+
+        response = file_manager.read_df_target()
 
         if filetype == "pickle" or (
             filetype == "infer" and (
-                self.check_extension(abspath, "pkl") 
-                or self.check_extension(abspath, "pkl.[a-zA-Z0-9]+")
+                IOReader.check_extension(abspath, "pkl") or
+                IOReader.check_extension(abspath, r"pkl\.[a-zA-Z0-9]+")
+                
             )
         ):
-            if decompress or self.check_extension(abspath, ".gz"):
+            if decompress or IOReader.check_extension(abspath, "gz"):
                 pd_args["compression"] = "gzip"
 
-            if path_tuple is not None:
-
-                response = self.read_bytes(abspath=abspath)
-
-                response = io.BytesIO(response)
-                    
-                df = pd.read_pickle(response, **pd_args)
-
-                return df
-            else:
-
-                df = pd.read_pickle(abspath, **pd_args)
-                
-                return df
+            return pd.read_pickle(response, **pd_args)
+        
         elif filetype == "parquet" or (
             filetype == "infer" and (
-                self.check_extension(abspath, "parquet") 
-                or self.check_extension(abspath, "parquet.[a-zA-Z0-9]+") 
-                or self.check_extension(abspath, "pqt") 
-                or self.check_extension(abspath, "pqt.[a-zA-Z0-9]+")
+                IOReader.check_extension(abspath, "parquet") or
+                IOReader.check_extension(abspath, r"parquet\.[a-zA-Z0-9]+") or
+                IOReader.check_extension(abspath, "pqt") or
+                IOReader.check_extension(abspath, r"pqt\.[a-zA-Z0-9]+")
             )
         ):
-            if path_tuple is not None:
-
-                response = self.read_bytes(abspath=abspath)
-
-                response = io.BytesIO(response)
+            
+            return pd.read_parquet(response, **pd_args)
 
-                return pd.read_parquet(response, **pd_args)
-            else:
-                return pd.read_parquet(abspath, **pd_args)
         elif filetype == "csv" or (
             filetype == "infer" and (
-                self.check_extension(abspath, "csv") 
-                or self.check_extension(abspath, "csv.[a-zA-Z0-9]+")
+                IOReader.check_extension(abspath, "csv") or
+                IOReader.check_extension(abspath, r"csv\.[a-zA-Z0-9]+")
             )
         ):
-            if decompress or self.check_extension(abspath, ".gz"):
+            if decompress or IOReader.check_extension(abspath, "gz"):
                 pd_args["compression"] = "gzip"
 
-            if path_tuple is not None:
-
-                response = self.read_bytes(abspath=abspath)
-
-                response = io.BytesIO(response)
-
-                df = pd.read_csv(response, **pd_args)
+            return pd.read_csv(response, **pd_args)
 
-                return df
-            else:
-                df = pd.read_csv(abspath, **pd_args)
-                
-                return df
         else:
-            raise ValueError("Invalid filetype. only csv, pickle, and parquet supported. Try read file or read bytes or explicitly setting filetype.")
+            raise ValueError(
+                "Invalid filetype. only csv, pickle, and parquet supported. "
+                "Try read file or read bytes or explicitly setting filetype."
+            )
 
     def read_file(
         self, 
         dest_path: str,
         src_path: str | None = None, 
         /, *, # before positional, after keyword
         abspath: str | None = None,
         decompress: bool = False, 
     ) -> None:
         """
         Read file specified by src_path or abspath and write it to the dest_path.
 
         Attributes:
-            dest_path: Absolute destination path to read the file to, including file name and extension. Positional only.
-            src_path: Relative path to the source file from within the IOReader's basepath directory, including file name and extension. src_path ignored if abspath specified, so either specify src_path or abspath not both. Positional only.
-            abspath: Absolute path to the source file, including file name and extension. If file is on S3, use the format "s3://bucket/key". src_path ignored if abspath specified, so either specify src_path or abspath not both. Keyword only.
+            dest_path: Absolute destination path to read the file to, including file name 
+                       and extension. Positional only.
+            src_path: Relative path to the source file from within the IOReader's basepath 
+                      directory, including file name and extension. src_path ignored if abspath 
+                      specified, so either specify src_path or abspath not both. Positional only.
+            abspath: Absolute path to the source file, including file name and extension. 
+                     If file is on S3, use the format "s3://bucket/key". src_path ignored if 
+                     abspath specified, so either specify src_path or abspath not both. 
+                     Keyword only.
             decompress: Whether to decompress file using gzip. By default, False. Keyword only.
         """
-        if abspath is None:
-            if src_path is None:
-                raise ValueError("No path or abspath set.")
-            # uses config to build full absolute path
-            abspath = self.get_absolute_path(src_path)
 
-        # tries to parse S3 info from abspath
-        path_tuple = IOConfig.parse_s3_path(abspath)
-
-        if path_tuple is not None:
-            # data on S3
-            if decompress:
-                response = self.read_bytes(
-                    abspath=abspath, 
-                    decompress=decompress
-                )
-
-                if self.check_extension(dest_path, ".gz"):
-                    dest_path = dest_path[:-3]
-
-                if not os.path.exists(os.path.dirname(dest_path)):
-                    os.makedirs(os.path.dirname(dest_path))
-
-                with open(dest_path, 'wb') as f:
-                    f.write(response)
-            else:
-                bucket_name = path_tuple[0]
-                src_path = path_tuple[1]
-
-                bucket = self.resource.Bucket(bucket_name)
+        file_bytes = self.read_bytes(
+            src_path, 
+            abspath=abspath,
+            decompress=decompress,
+        )
 
-                if not os.path.exists(os.path.dirname(dest_path)):
-                    os.makedirs(os.path.dirname(dest_path))
+        if not os.path.exists(os.path.dirname(dest_path)):
+            os.makedirs(os.path.dirname(dest_path))
 
-                bucket.download_file(src_path.replace("\\","/"), dest_path)
-        else:
-            if not os.path.exists(os.path.dirname(dest_path)):
-                os.makedirs(os.path.dirname(dest_path))
-            if decompress:
-                if self.check_extension(dest_path, ".gz"):
-                    dest_path = dest_path[:-3]
-
-                with gzip.open(abspath, 'rb') as f_in:
-                    with open(dest_path, 'wb') as f_out:
-                        shutil.copyfileobj(f_in, f_out)
-            else:
-                shutil.copy(abspath, dest_path)
+        with open(dest_path, 'wb') as f:
+            f.write(file_bytes)
     
     def read_directory(
         self,
         dest_path: str,
         src_path: str | None = None, 
         /, *, # before positional, after keyword
         abspath: str | None = None,
     ) -> None:
         """
         Read directory folder contents specified by src_path or abspath and write them to dest_path.
 
         Attributes:
             dest_path: Absolute destination path to read the directory to. Positional only.
-            src_path: Relative path to the source directory from within the IOReader's basepath directory. src_path ignored if abspath specified, so either specify src_path or abspath not both. Positional only.
-            abspath: Absolute path to the source directory. If directory is on S3, use the format "s3://bucket/key". src_path ignored if abspath specified, so either specify src_path or abspath not both. Keyword only.
+            src_path: Relative path to the source directory from within the IOReader's 
+                      basepath directory. src_path ignored if abspath specified, so either 
+                      specify src_path or abspath not both. Positional only.
+            abspath: Absolute path to the source directory. If directory is on S3, use the format 
+                     "s3://bucket/key". src_path ignored if abspath specified, so either specify 
+                     src_path or abspath not both. Keyword only.
         """
         if not self.exists(src_path, abspath=abspath, is_folder=True):
             raise OSError("Source directory does not exist")
 
         if abspath is None:
             if src_path is None:
                 raise ValueError("No src_path or abspath set.")
             # uses config to build full absolute path
             abspath = self.get_absolute_path(src_path)
 
-        abspath = abspath.replace("\\","/")
-
-        # tries to parse S3 info from abspath
-        path_tuple = IOConfig.parse_s3_path(abspath)
-
-        if path_tuple is not None:
-            if abspath[len(abspath) - 1] == "/":
-                abspath = abspath[:-1]
-
-            for file_abspath in self.list_directory(abspath=abspath):
-                file_relpath = file_abspath.replace(f"{abspath}/", "", 1)
-                self.read_file(os.path.join(dest_path, file_relpath), abspath=file_abspath)
-
-        else:
-            shutil.copytree(abspath, dest_path, dirs_exist_ok=True)
+        for file_abspath in self.list_directory(abspath=abspath):
+            relative_path = os.path.relpath(file_abspath, abspath)
+            self.read_file(os.path.join(dest_path, relative_path), abspath=file_abspath)
 
     def read_in_cache(
         self,
         cache_path: str,
     ) -> None:
         """
-        If executing on the cloud, read in saved cloud cache if one exists and write it to cache_path. If executing locally, it won't do anything.
+        If executing on the cloud, read in saved cloud cache if one exists and write it to cache_path. 
+        If executing locally, it won't do anything.
     
         Attributes:
             cache_path: Absolute destination path to read the cache to.
         """
         if self.cloud_execution:
             try:                
                 cache_name = f"{os.path.basename(cache_path)}.zip"
@@ -416,182 +343,83 @@
                     if not os.path.exists(cache_path):
                         os.makedirs(cache_path)
                 else:
                     self.read_zip_directory(cache_path, abspath=cloud_path)
             except botocore.exceptions.ClientError:
                 if not os.path.exists(cache_path):
                     os.makedirs(cache_path)
-    
+
     def read_zip_directory(
         self,
         dest_path: str,
         src_path: str | None = None,
         /, *, # before positional, after keyword
         abspath: str | None = None,
         format_archive: str="zip",
     ) -> None:
         """
-        Read archived directory folder specified by src_path or abspath, unpack archived directory (aka unzip it), and write it to dest_path.
+        Read archived directory folder specified by src_path or abspath, unpack archived directory 
+        (aka unzip it), and write it to dest_path.
 
         Attributes:
             dest_path: Absolute destination path to read the directory to. Positional only.
-            src_path: Relative path to the source zipped directory/archive from within the IOReader's basepath directory. src_path ignored if abspath specified, so either specify src_path or abspath not both. Positional only.
-            abspath: Absolute path to the source zipped directory/archive. If file is on S3, use the format "s3://bucket/key". src_path ignored if abspath specified, so either specify src_path or abspath not both. Keyword only.
-            format_archive: Format of archived directory. Possible values are: "zip", "tar", "gztar", "bztar", and "xztar". By default, "zip". Keyword only.
+            src_path: Relative path to the source zipped directory/archive from within the IOReader's 
+                      basepath directory. src_path ignored if abspath specified, so either specify 
+                      src_path or abspath not both. Positional only.
+            abspath: Absolute path to the source zipped directory/archive. If file is on S3, 
+                     use the format "s3://bucket/key". src_path ignored if abspath specified, 
+                     so either specify src_path or abspath not both. Keyword only.
+            format_archive: Format of archived directory. Possible values are: "zip", "tar", 
+                            "gztar", "bztar", and "xztar". By default, "zip". Keyword only.
         """
+        # TODO: this code is repeated between read_zip_directory() and write_zip_directory(). 
+        #       Let's reduce the repetition over time.
         if format_archive == "zip" or format_archive == "tar":
-            ext = format_archive
+            ext = ext_regex = format_archive
+            format_abbreviation = ""
         elif format_archive == "gztar":
             ext = "tar.gz"
+            ext_regex = r"tar\.gz"
+            format_abbreviation = 'gz'
         elif format_archive == "bztar":
             ext = "tar.bz2"
+            ext_regex = r"tar\.bz2"
+            format_abbreviation = 'bz2'
         elif format_archive == "xztar":
             ext = "tar.xz"
+            ext_regex = r"tar\.xz"
+            format_abbreviation = 'xz'
         else:
             format_archive = "zip"
-            ext = format_archive
+            ext = ext_regex = format_archive
+            format_abbreviation = ""
 
         if abspath is None:
             if src_path is None:
                 raise ValueError("No src_path or abspath set.")
             # uses config to build full absolute path
             abspath = self.get_absolute_path(src_path)
 
-        abspath = abspath.replace("\\","/")
-
-        if not self.check_extension(abspath, ext):
+        if not IOReader.check_extension(abspath, ext_regex):
             abspath = f"{abspath}.{ext}"
 
         if not self.exists(abspath=abspath):
             raise OSError("Source directory does not exist")
 
-        # tries to parse S3 info from abspath
-        path_tuple = IOConfig.parse_s3_path(abspath)
-
-        if path_tuple is not None:
-            bucket_name = path_tuple[0]
-            src_path = path_tuple[1]
-
-            if not os.path.exists(dest_path):
-                os.makedirs(dest_path)
-
-            with tempfile.TemporaryDirectory() as tmpdirname:
-                self.resource.Object(bucket_name, src_path.replace("\\","/")).download_file(f'{tmpdirname}/tmp.{ext}')
-
-                shutil.unpack_archive(f'{tmpdirname}/tmp.{ext}', dest_path, format_archive)
-
-        else:
-            shutil.unpack_archive(abspath, dest_path, format_archive)
-
-    def list_directory(
-        self, 
-        path: str | None = None, 
-        /, *, # before positional, after keyword
-        abspath: str | None = None,
-        regex_search: str = "",
-    ) -> list[str]:
-        """
-        List all files in directory at specified location, including those in subfolders. Note that only files included in returned list.
-
-        Attributes:
-            path: Relative path to the directory from within the IOReader's basepath directory. path ignored if abspath specified, so either specify path or abspath not both. Positional only.
-            abspath: Absolute path to the directory. If file is on S3, use the format "s3://bucket/key". path ignored if abspath specified, so either specify path or abspath not both. Keyword only.
-            regex_search: only results that match regex pattern will be included. Keyword only.
-        
-        Returns:
-            list[str]: list of files located in the directory and all subdirectories. 
-        """
-        if not self.exists(path, abspath=abspath, is_folder=True):
-
-            raise OSError("Directory does not exist")
+        if not os.path.exists(dest_path):
+            os.makedirs(dest_path)
 
-        if abspath is None:
-            if path is None:
-                raise ValueError("No path or abspath set.")
-            # uses config to build full absolute path
-            abspath = self.get_absolute_path(path)
+        file_manager = self._get_file_manager(abspath=abspath)
 
-        # tries to parse S3 info from abspath
-        path_tuple = IOConfig.parse_s3_path(abspath)
+        file_obj = file_manager.read_bytes()
 
-        if path_tuple is not None:
-            bucket_name = path_tuple[0]
-            path = path_tuple[1]
-
-            # filter by path and substring
-            paginator = self.client.get_paginator('list_objects_v2')
-
-            if path == "." or path == "":
-                pages = paginator.paginate(Bucket=bucket_name)
-            else:
-                path = path.replace("\\","/")
-                # if path doesn't end in slash add one
-                if path[len(path) - 1] != "/":
-                    path = f"{path}/"
-                pages = paginator.paginate(Bucket=bucket_name, Prefix=path)
-
-            file_list = []
-            for page in pages:
-                # filter by path and search_regex
-                file_list += [obj['Key'] for obj in page['Contents'] if re.search(regex_search, obj['Key'])]
-
-            # filter out the folders so only files in list
-            file_list = [ f"s3://{bucket_name}/{f}" for f in file_list if not re.search('^.+/$', f) ]
-            return file_list
+        if format_archive == "zip":
+            with zipfile.ZipFile(file_obj, mode="r") as archive:
+                archive.extractall(dest_path)
         else:
-            file_list = []
-            for dirpath, dirnames, filenames in os.walk(abspath):  
-                for filename in filenames:
-                    curr_path = os.path.join(dirpath, filename).replace("\\","/")
-                    if re.search(regex_search, curr_path):
-                        file_list.append(curr_path)
-            return file_list
-
-    def exists(
-        self, 
-        path: str | None = None, 
-        /, *, # before positional, after keyword
-        abspath: str | None = None,
-        is_folder: bool = False,
-    ) -> bool:
-        """
-        Check if file or directory specified by path exists.
-    
-        Attributes:
-            path: Relative path to the directory from within the IOReader's basepath directory. path ignored if abspath specified, so either specify path or abspath not both. Positional only.
-            abspath: Absolute path to the directory. If file is on S3, use the format "s3://bucket/key". path ignored if abspath specified, so either specify path or abspath not both. Keyword only.
-            is_folder: Whether the given path is to a folder. Keyword only.
-        
-        Returns:
-            bool: True if file or directory exists, otherwise False.
-        """
-        if abspath is None:
-            if path is None:
-                raise ValueError("No path or abspath set.")
-            # uses config to build full absolute path
-            abspath = self.get_absolute_path(path)
-
-        # tries to parse S3 info from abspath
-        path_tuple = IOConfig.parse_s3_path(abspath)
-
-        if path_tuple is not None:
-            bucket_name = path_tuple[0]
-            path = path_tuple[1]
-            if path[len(path) - 1] == "/":
-                is_folder = True
-                path = path[:-1]
-
-            try:
-                if is_folder:
-                    if path == "." or path == "":
-                        self.client.head_bucket(Bucket=bucket_name)
-                        return True
-                    else:
-                        response = self.client.list_objects(Bucket=bucket_name, Prefix=path.replace("\\","/"), Delimiter='/',MaxKeys=2)
-                        return 'CommonPrefixes' in response
+            with tarfile.open(fileobj=file_obj, mode=f"r|{format_abbreviation}") as archive:
+                if sys.version_info >= (3,12):
+                    archive.extractall(dest_path, filter="data")
                 else:
-                    self.resource.Object(bucket_name, path.replace("\\","/")).content_type
-            except botocore.exceptions.ClientError:
-                return False
-            return True
-        else:
-            return os.path.exists(abspath)
+                    archive.extractall(dest_path)
+
+        file_obj.close()
```

### Comparing `PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils/upload_test_github.py` & `pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils/upload_test_github.py`

 * *Files identical despite different names*

### Comparing `PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils.egg-info/PKG-INFO` & `pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: PWBM_Cloud_Utils
-Version: 0.1.3
+Version: 0.1.4
 Summary: connect to read/write data to s3
 Author-email: "Yunye Jiang, Mariko Paulson, Chris Palenchar" <yunyej@wharton.upenn.edu>
 Project-URL: Homepage, https://github.com/PennWhartonBudgetModel/PWBM_Cloud_Utils
 Project-URL: Bug Tracker, https://github.com/PennWhartonBudgetModel/PWBM_Cloud_Utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3
 Requires-Dist: pandas
 Requires-Dist: python-dotenv
 Requires-Dist: requests
-Requires-Dist: fastparquet
 Requires-Dist: pyarrow
+Requires-Dist: typing-extensions
+Requires-Dist: s3fs>=2023.3.0
 
 # PWBM_Cloud_Utils
 
 ## Introduction
 This Python module provides a convenient interface for handling input/output configurations, reading from different sources (local or cloud), and writing data to cloud storage (Amazon S3) or locally. It is designed to be flexible, supporting various data formats and compression options.
 
+Note that the package officially supports `pyarrow` as the engine to work with parquet
+files. This is because `pandas` is adopting `pyarrow` for more efficient memory
+representation since Version 2.0. The code may still work with `fastparquet`, but
+it will not be supported officially.
+
 ## Installation
 To use this module, ensure that you have the required dependencies installed. You can install them using the following command:
 ```bash
 pip install PWBM_Cloud_Utils
 ```
 or
 ```bash
```

### Comparing `PWBM_Cloud_Utils-0.1.3/src/PWBM_Cloud_Utils.egg-info/SOURCES.txt` & `pwbm_cloud_utils-0.1.4/src/PWBM_Cloud_Utils.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -2,23 +2,34 @@
 README.md
 pyproject.toml
 src/PWBM_Cloud_Utils/__init__.py
 src/PWBM_Cloud_Utils/api_functions.py
 src/PWBM_Cloud_Utils/cloud_main.py
 src/PWBM_Cloud_Utils/cloud_utils.py
 src/PWBM_Cloud_Utils/entities.py
+src/PWBM_Cloud_Utils/file_manager.py
+src/PWBM_Cloud_Utils/io_base.py
 src/PWBM_Cloud_Utils/io_config.py
 src/PWBM_Cloud_Utils/io_reader.py
 src/PWBM_Cloud_Utils/io_writer.py
+src/PWBM_Cloud_Utils/scripting_functions.py
 src/PWBM_Cloud_Utils/upload_test_github.py
 src/PWBM_Cloud_Utils.egg-info/PKG-INFO
 src/PWBM_Cloud_Utils.egg-info/SOURCES.txt
 src/PWBM_Cloud_Utils.egg-info/dependency_links.txt
 src/PWBM_Cloud_Utils.egg-info/requires.txt
 src/PWBM_Cloud_Utils.egg-info/top_level.txt
 src/tests/__init__.py
+src/tests/helpers_testing.py
 src/tests/test_cache.py
+src/tests/test_cloud_main.py
+src/tests/test_cloud_utils.py
 src/tests/test_config.py
-src/tests/test_local.py
-src/tests/test_main.py
-src/tests/test_s3.py
+src/tests/test_io_base.py
+src/tests/test_local_file_manager.py
+src/tests/test_local_reader.py
+src/tests/test_local_writer.py
+src/tests/test_s3_file_manager.py
+src/tests/test_s3_reader.py
+src/tests/test_s3_writer.py
+src/tests/test_scripting.py
 src/tests/data/Person.py
```

