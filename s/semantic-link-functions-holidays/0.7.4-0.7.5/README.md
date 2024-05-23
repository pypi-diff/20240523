# Comparing `tmp/semantic_link_functions_holidays-0.7.4-py3-none-any.whl.zip` & `tmp/semantic_link_functions_holidays-0.7.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 4212 bytes, number of entries: 7
--rw-rw-r--  2.0 unx       90 b- defN 24-May-15 07:53 sempy_functions_holidays/__init__.py
--rw-rw-r--  2.0 unx     2287 b- defN 24-May-15 07:53 sempy_functions_holidays/_holiday.py
--rw-rw-r--  2.0 unx     1141 b- defN 24-May-15 07:56 semantic_link_functions_holidays-0.7.4.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     1796 b- defN 24-May-15 07:56 semantic_link_functions_holidays-0.7.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-15 07:56 semantic_link_functions_holidays-0.7.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       25 b- defN 24-May-15 07:56 semantic_link_functions_holidays-0.7.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      699 b- defN 24-May-15 07:56 semantic_link_functions_holidays-0.7.4.dist-info/RECORD
+-rw-rw-r--  2.0 unx       90 b- defN 24-May-23 15:17 sempy_functions_holidays/__init__.py
+-rw-rw-r--  2.0 unx     2287 b- defN 24-May-23 15:17 sempy_functions_holidays/_holiday.py
+-rw-rw-r--  2.0 unx     1141 b- defN 24-May-23 15:21 semantic_link_functions_holidays-0.7.5.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     1796 b- defN 24-May-23 15:21 semantic_link_functions_holidays-0.7.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-23 15:21 semantic_link_functions_holidays-0.7.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       25 b- defN 24-May-23 15:21 semantic_link_functions_holidays-0.7.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      699 b- defN 24-May-23 15:21 semantic_link_functions_holidays-0.7.5.dist-info/RECORD
 7 files, 6130 bytes uncompressed, 2938 bytes compressed:  52.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: sempy_functions_holidays/__init__.py
 Comment: 
 
 Filename: sempy_functions_holidays/_holiday.py
 Comment: 
 
-Filename: semantic_link_functions_holidays-0.7.4.dist-info/LICENSE.txt
+Filename: semantic_link_functions_holidays-0.7.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: semantic_link_functions_holidays-0.7.4.dist-info/METADATA
+Filename: semantic_link_functions_holidays-0.7.5.dist-info/METADATA
 Comment: 
 
-Filename: semantic_link_functions_holidays-0.7.4.dist-info/WHEEL
+Filename: semantic_link_functions_holidays-0.7.5.dist-info/WHEEL
 Comment: 
 
-Filename: semantic_link_functions_holidays-0.7.4.dist-info/top_level.txt
+Filename: semantic_link_functions_holidays-0.7.5.dist-info/top_level.txt
 Comment: 
 
-Filename: semantic_link_functions_holidays-0.7.4.dist-info/RECORD
+Filename: semantic_link_functions_holidays-0.7.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `semantic_link_functions_holidays-0.7.4.dist-info/LICENSE.txt` & `semantic_link_functions_holidays-0.7.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `semantic_link_functions_holidays-0.7.4.dist-info/METADATA` & `semantic_link_functions_holidays-0.7.5.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: semantic-link-functions-holidays
-Version: 0.7.4
+Version: 0.7.5
 Summary: Semantic link functions for holidays package. Enables enrichment of FabricDataFrame with public holidays.
 Home-page: https://github.com/microsoft/semantic-link-functions
 Author: Microsoft
 Author-email: semanticdatascience@service.microsoft.com
 License: MIT License
 Platform: Microsoft Fabric
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: ../LICENSE.txt
 Requires-Dist: holidays
-Requires-Dist: semantic-link-sempy ==0.7.4
+Requires-Dist: semantic-link-sempy ==0.7.5
 
 FabricDataFrames dynamically expose semantic functions based on logic defined by each function. For example, the is_holiday function shows up in the autocomplete suggestions when you're working on a FabricDataFrame containing both a datetime column and a country column.
 
 Each semantic function uses information about the data types, metadata (such as Power BI data categories), and the data in a FabricDataFrame or FabricSeries to determine its relevance to the particular data on which you're working.
 
 Semantic functions are automatically discovered when annotated with the @semantic_function decorator. You can think of semantic functions as being similar to C# extension methods applied to the popular DataFrame concept.
```

## Comparing `semantic_link_functions_holidays-0.7.4.dist-info/RECORD` & `semantic_link_functions_holidays-0.7.5.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 sempy_functions_holidays/__init__.py,sha256=VYW6G1u2CuOQQaNwEQ67FNsjBH3Ttu304K8eQrbdznM,90
 sempy_functions_holidays/_holiday.py,sha256=XRNAzKqm85avi0GT8mx5p3--0nYapu2w-YPcB3_yzE8,2287
-semantic_link_functions_holidays-0.7.4.dist-info/LICENSE.txt,sha256=ws_MuBL-SCEBqPBFl9_FqZkaaydIJmxHrJG2parhU4M,1141
-semantic_link_functions_holidays-0.7.4.dist-info/METADATA,sha256=1YYbOukxSC0IqisjQz0QNWj6EdzwE2rFZZ6MbmKwu14,1796
-semantic_link_functions_holidays-0.7.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-semantic_link_functions_holidays-0.7.4.dist-info/top_level.txt,sha256=KW2UCFjobepwGduVHOIPecVWV87HuJqoaOXMjMr-cvA,25
-semantic_link_functions_holidays-0.7.4.dist-info/RECORD,,
+semantic_link_functions_holidays-0.7.5.dist-info/LICENSE.txt,sha256=ws_MuBL-SCEBqPBFl9_FqZkaaydIJmxHrJG2parhU4M,1141
+semantic_link_functions_holidays-0.7.5.dist-info/METADATA,sha256=0w_sjCQs-GBWosorwsPrHP5RTBLIhrpHdzaWCZ72igw,1796
+semantic_link_functions_holidays-0.7.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+semantic_link_functions_holidays-0.7.5.dist-info/top_level.txt,sha256=KW2UCFjobepwGduVHOIPecVWV87HuJqoaOXMjMr-cvA,25
+semantic_link_functions_holidays-0.7.5.dist-info/RECORD,,
```

