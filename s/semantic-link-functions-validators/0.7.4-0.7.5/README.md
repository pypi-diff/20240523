# Comparing `tmp/semantic_link_functions_validators-0.7.4-py3-none-any.whl.zip` & `tmp/semantic_link_functions_validators-0.7.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 4748 bytes, number of entries: 7
--rw-rw-r--  2.0 unx      200 b- defN 24-May-15 07:53 sempy_functions_validators/__init__.py
--rw-rw-r--  2.0 unx     9440 b- defN 24-May-15 07:53 sempy_functions_validators/_validators.py
--rw-rw-r--  2.0 unx     1141 b- defN 24-May-15 07:56 semantic_link_functions_validators-0.7.4.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     1837 b- defN 24-May-15 07:56 semantic_link_functions_validators-0.7.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-15 07:56 semantic_link_functions_validators-0.7.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       27 b- defN 24-May-15 07:56 semantic_link_functions_validators-0.7.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      717 b- defN 24-May-15 07:56 semantic_link_functions_validators-0.7.4.dist-info/RECORD
+-rw-rw-r--  2.0 unx      200 b- defN 24-May-23 15:17 sempy_functions_validators/__init__.py
+-rw-rw-r--  2.0 unx     9440 b- defN 24-May-23 15:17 sempy_functions_validators/_validators.py
+-rw-rw-r--  2.0 unx     1141 b- defN 24-May-23 15:21 semantic_link_functions_validators-0.7.5.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     1837 b- defN 24-May-23 15:21 semantic_link_functions_validators-0.7.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-23 15:21 semantic_link_functions_validators-0.7.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       27 b- defN 24-May-23 15:21 semantic_link_functions_validators-0.7.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      717 b- defN 24-May-23 15:21 semantic_link_functions_validators-0.7.5.dist-info/RECORD
 7 files, 13454 bytes uncompressed, 3440 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: sempy_functions_validators/__init__.py
 Comment: 
 
 Filename: sempy_functions_validators/_validators.py
 Comment: 
 
-Filename: semantic_link_functions_validators-0.7.4.dist-info/LICENSE.txt
+Filename: semantic_link_functions_validators-0.7.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: semantic_link_functions_validators-0.7.4.dist-info/METADATA
+Filename: semantic_link_functions_validators-0.7.5.dist-info/METADATA
 Comment: 
 
-Filename: semantic_link_functions_validators-0.7.4.dist-info/WHEEL
+Filename: semantic_link_functions_validators-0.7.5.dist-info/WHEEL
 Comment: 
 
-Filename: semantic_link_functions_validators-0.7.4.dist-info/top_level.txt
+Filename: semantic_link_functions_validators-0.7.5.dist-info/top_level.txt
 Comment: 
 
-Filename: semantic_link_functions_validators-0.7.4.dist-info/RECORD
+Filename: semantic_link_functions_validators-0.7.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `semantic_link_functions_validators-0.7.4.dist-info/LICENSE.txt` & `semantic_link_functions_validators-0.7.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `semantic_link_functions_validators-0.7.4.dist-info/METADATA` & `semantic_link_functions_validators-0.7.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: semantic-link-functions-validators
-Version: 0.7.4
+Version: 0.7.5
 Summary: Semantic link functions for validators package. Enables validation of email addresses, credit card numbers, ... in FabricDataFrames.
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
 Requires-Dist: validators
-Requires-Dist: semantic-link-sempy ==0.7.4
+Requires-Dist: semantic-link-sempy ==0.7.5
 
 FabricDataFrames dynamically expose semantic functions based on logic defined by each function. For example, the is_holiday function shows up in the autocomplete suggestions when you're working on a FabricDataFrame containing both a datetime column and a country column.
 
 Each semantic function uses information about the data types, metadata (such as Power BI data categories), and the data in a FabricDataFrame or FabricSeries to determine its relevance to the particular data on which you're working.
 
 Semantic functions are automatically discovered when annotated with the @semantic_function decorator. You can think of semantic functions as being similar to C# extension methods applied to the popular DataFrame concept.
```

## Comparing `semantic_link_functions_validators-0.7.4.dist-info/RECORD` & `semantic_link_functions_validators-0.7.5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 sempy_functions_validators/__init__.py,sha256=SB-WAvpV7T1_hb8YRjTFhEdkE1cQ0t4oxTTDE7qsTrw,200
 sempy_functions_validators/_validators.py,sha256=ZYq3OFZHA_N9uj4T26Y9UW8m9Ln6F69xGorWdmTdUbY,9440
-semantic_link_functions_validators-0.7.4.dist-info/LICENSE.txt,sha256=ws_MuBL-SCEBqPBFl9_FqZkaaydIJmxHrJG2parhU4M,1141
-semantic_link_functions_validators-0.7.4.dist-info/METADATA,sha256=69ZvQ7V_sMnCNRdxymBNlhE7Cb_CuHMuEJ4ImPP0W48,1837
-semantic_link_functions_validators-0.7.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-semantic_link_functions_validators-0.7.4.dist-info/top_level.txt,sha256=yJOwEenUV6QBleak2Kw3aX9RFn9iqXL9UTGl8QFQnHY,27
-semantic_link_functions_validators-0.7.4.dist-info/RECORD,,
+semantic_link_functions_validators-0.7.5.dist-info/LICENSE.txt,sha256=ws_MuBL-SCEBqPBFl9_FqZkaaydIJmxHrJG2parhU4M,1141
+semantic_link_functions_validators-0.7.5.dist-info/METADATA,sha256=g0ALyftkwI43-F1VgvdiI0MYa2v_z1GR4V-WXw06k9k,1837
+semantic_link_functions_validators-0.7.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+semantic_link_functions_validators-0.7.5.dist-info/top_level.txt,sha256=yJOwEenUV6QBleak2Kw3aX9RFn9iqXL9UTGl8QFQnHY,27
+semantic_link_functions_validators-0.7.5.dist-info/RECORD,,
```

