# Comparing `tmp/stix_shifter_modules_aws_athena-7.0.7-py2.py3-none-any.whl.zip` & `tmp/stix_shifter_modules_aws_athena-7.0.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,41 +1,41 @@
-Zip file size: 84366 bytes, number of entries: 39
--rw-rw-r--  2.0 unx        0 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/__init__.py
--rw-rw-r--  2.0 unx     1374 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/entry_point.py
--rw-rw-r--  2.0 unx   240254 b- defN 24-May-07 18:00 stix_shifter_modules/aws_athena/configuration/config.json
--rw-rw-r--  2.0 unx      229 b- defN 24-May-07 18:00 stix_shifter_modules/aws_athena/configuration/dialects.json
--rw-rw-r--  2.0 unx     5053 b- defN 24-May-07 18:00 stix_shifter_modules/aws_athena/configuration/lang_en.json
--rw-rw-r--  2.0 unx        0 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_translation/__init__.py
--rw-rw-r--  2.0 unx    26842 b- defN 24-May-07 18:00 stix_shifter_modules/aws_athena/stix_translation/json_to_stix_translator.py
--rw-rw-r--  2.0 unx    24044 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_translation/query_constructor.py
--rw-rw-r--  2.0 unx     1024 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_translation/query_translator.py
--rw-rw-r--  2.0 unx     1075 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_translation/transformers.py
--rw-rw-r--  2.0 unx     4765 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_config.json
--rw-rw-r--  2.0 unx     1894 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_from_stix_map.json
--rw-rw-r--  2.0 unx    10146 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_to_stix_map.json
--rw-rw-r--  2.0 unx      139 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_translation/json/hash_algorithm_map.json
--rw-rw-r--  2.0 unx     2439 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_translation/json/network_protocol_map.json
--rw-rw-r--  2.0 unx    18300 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_translation/json/ocsf_from_stix_map.json
--rw-rw-r--  2.0 unx    75601 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_translation/json/ocsf_to_stix_map.json
--rw-rw-r--  2.0 unx      591 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_translation/json/operators.json
--rw-rw-r--  2.0 unx      814 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_from_stix_map.json
--rw-rw-r--  2.0 unx     2350 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_to_stix_map.json
--rw-rw-r--  2.0 unx     1894 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/guardduty_from_stix_map.json
--rw-rw-r--  2.0 unx    18297 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/ocsf_from_stix_map.json
--rw-rw-r--  2.0 unx    93792 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/to_stix_map.json
--rw-rw-r--  2.0 unx      891 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/vpcflow_from_stix_map.json
--rw-rw-r--  2.0 unx        0 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_transmission/__init__.py
--rw-rw-r--  2.0 unx     4021 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_transmission/boto3_client.py
--rw-rw-r--  2.0 unx     1207 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_transmission/delete_connector.py
--rw-rw-r--  2.0 unx     1969 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_transmission/error_mapper.py
--rw-rw-r--  2.0 unx     1370 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_transmission/ping_connector.py
--rw-rw-r--  2.0 unx     7435 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_transmission/post_query_connector_error_handling.py
--rw-rw-r--  2.0 unx    10418 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_transmission/query_connector.py
--rw-rw-r--  2.0 unx    15539 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_transmission/results_connector.py
--rw-rw-r--  2.0 unx     3473 b- defN 24-May-07 17:59 stix_shifter_modules/aws_athena/stix_transmission/status_connector.py
--rw-rw-r--  2.0 unx    12786 b- defN 24-May-07 18:00 stix_shifter_modules_aws_athena-7.0.7.dist-info/LICENSE.md
--rw-rw-r--  2.0 unx     7175 b- defN 24-May-07 18:00 stix_shifter_modules_aws_athena-7.0.7.dist-info/METADATA
--rw-rw-r--  2.0 unx     1418 b- defN 24-May-07 18:00 stix_shifter_modules_aws_athena-7.0.7.dist-info/NOTICE
--rw-rw-r--  2.0 unx      110 b- defN 24-May-07 18:00 stix_shifter_modules_aws_athena-7.0.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx       21 b- defN 24-May-07 18:00 stix_shifter_modules_aws_athena-7.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4837 b- defN 24-May-07 18:00 stix_shifter_modules_aws_athena-7.0.7.dist-info/RECORD
-39 files, 603587 bytes uncompressed, 76034 bytes compressed:  87.4%
+Zip file size: 84368 bytes, number of entries: 39
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/__init__.py
+-rw-rw-r--  2.0 unx     1374 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/entry_point.py
+-rw-rw-r--  2.0 unx   240254 b- defN 24-May-23 19:01 stix_shifter_modules/aws_athena/configuration/config.json
+-rw-rw-r--  2.0 unx      229 b- defN 24-May-23 19:01 stix_shifter_modules/aws_athena/configuration/dialects.json
+-rw-rw-r--  2.0 unx     5053 b- defN 24-May-23 19:01 stix_shifter_modules/aws_athena/configuration/lang_en.json
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_translation/__init__.py
+-rw-rw-r--  2.0 unx    26842 b- defN 24-May-23 19:01 stix_shifter_modules/aws_athena/stix_translation/json_to_stix_translator.py
+-rw-rw-r--  2.0 unx    24044 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_translation/query_constructor.py
+-rw-rw-r--  2.0 unx     1024 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_translation/query_translator.py
+-rw-rw-r--  2.0 unx     1075 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_translation/transformers.py
+-rw-rw-r--  2.0 unx     4765 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_config.json
+-rw-rw-r--  2.0 unx     1894 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_from_stix_map.json
+-rw-rw-r--  2.0 unx    10146 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_to_stix_map.json
+-rw-rw-r--  2.0 unx      139 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_translation/json/hash_algorithm_map.json
+-rw-rw-r--  2.0 unx     2439 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_translation/json/network_protocol_map.json
+-rw-rw-r--  2.0 unx    18300 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_translation/json/ocsf_from_stix_map.json
+-rw-rw-r--  2.0 unx    75601 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_translation/json/ocsf_to_stix_map.json
+-rw-rw-r--  2.0 unx      591 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_translation/json/operators.json
+-rw-rw-r--  2.0 unx      814 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_from_stix_map.json
+-rw-rw-r--  2.0 unx     2350 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_to_stix_map.json
+-rw-rw-r--  2.0 unx     1894 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/guardduty_from_stix_map.json
+-rw-rw-r--  2.0 unx    18297 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/ocsf_from_stix_map.json
+-rw-rw-r--  2.0 unx    93792 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/to_stix_map.json
+-rw-rw-r--  2.0 unx      891 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/vpcflow_from_stix_map.json
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_transmission/__init__.py
+-rw-rw-r--  2.0 unx     4021 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_transmission/boto3_client.py
+-rw-rw-r--  2.0 unx     1207 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_transmission/delete_connector.py
+-rw-rw-r--  2.0 unx     1969 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_transmission/error_mapper.py
+-rw-rw-r--  2.0 unx     1370 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_transmission/ping_connector.py
+-rw-rw-r--  2.0 unx     7435 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_transmission/post_query_connector_error_handling.py
+-rw-rw-r--  2.0 unx    10418 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_transmission/query_connector.py
+-rw-rw-r--  2.0 unx    15539 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_transmission/results_connector.py
+-rw-rw-r--  2.0 unx     3473 b- defN 24-May-23 19:00 stix_shifter_modules/aws_athena/stix_transmission/status_connector.py
+-rw-rw-r--  2.0 unx    12786 b- defN 24-May-23 19:01 stix_shifter_modules_aws_athena-7.0.9.dist-info/LICENSE.md
+-rw-rw-r--  2.0 unx     7175 b- defN 24-May-23 19:01 stix_shifter_modules_aws_athena-7.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx     1418 b- defN 24-May-23 19:01 stix_shifter_modules_aws_athena-7.0.9.dist-info/NOTICE
+-rw-rw-r--  2.0 unx      110 b- defN 24-May-23 19:01 stix_shifter_modules_aws_athena-7.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       21 b- defN 24-May-23 19:01 stix_shifter_modules_aws_athena-7.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4837 b- defN 24-May-23 19:01 stix_shifter_modules_aws_athena-7.0.9.dist-info/RECORD
+39 files, 603587 bytes uncompressed, 76036 bytes compressed:  87.4%
```

## zipnote {}

```diff
@@ -93,26 +93,26 @@
 
 Filename: stix_shifter_modules/aws_athena/stix_transmission/results_connector.py
 Comment: 
 
 Filename: stix_shifter_modules/aws_athena/stix_transmission/status_connector.py
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-7.0.7.dist-info/LICENSE.md
+Filename: stix_shifter_modules_aws_athena-7.0.9.dist-info/LICENSE.md
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-7.0.7.dist-info/METADATA
+Filename: stix_shifter_modules_aws_athena-7.0.9.dist-info/METADATA
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-7.0.7.dist-info/NOTICE
+Filename: stix_shifter_modules_aws_athena-7.0.9.dist-info/NOTICE
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-7.0.7.dist-info/WHEEL
+Filename: stix_shifter_modules_aws_athena-7.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-7.0.7.dist-info/top_level.txt
+Filename: stix_shifter_modules_aws_athena-7.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-7.0.7.dist-info/RECORD
+Filename: stix_shifter_modules_aws_athena-7.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `stix_shifter_modules_aws_athena-7.0.7.dist-info/LICENSE.md` & `stix_shifter_modules_aws_athena-7.0.9.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `stix_shifter_modules_aws_athena-7.0.7.dist-info/METADATA` & `stix_shifter_modules_aws_athena-7.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stix_shifter_modules_aws_athena
-Version: 7.0.7
+Version: 7.0.9
 Summary: Tools and interface to translate STIX formatted results and queries to different data source formats and to set up appropriate connection strings for invoking and triggering actions in openwhisk
 Home-page: https://github.com/opencybersecurityalliance/stix-shifter
 Author: ibm
 Author-email: 
 Project-URL: Source, https://github.com/opencybersecurityalliance/stix-shifter
 Keywords: datasource stix translate transform transmit
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `stix_shifter_modules_aws_athena-7.0.7.dist-info/NOTICE` & `stix_shifter_modules_aws_athena-7.0.9.dist-info/NOTICE`

 * *Files identical despite different names*

## Comparing `stix_shifter_modules_aws_athena-7.0.7.dist-info/RECORD` & `stix_shifter_modules_aws_athena-7.0.9.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -27,13 +27,13 @@
 stix_shifter_modules/aws_athena/stix_transmission/delete_connector.py,sha256=D2A5li6TWgZvqpnDGLXVveLqYHlWI1evVWKYKeXT60M,1207
 stix_shifter_modules/aws_athena/stix_transmission/error_mapper.py,sha256=hKiytRjhZx2BVSP1o13h30krPYLMTRxuWrPa6dij-l0,1969
 stix_shifter_modules/aws_athena/stix_transmission/ping_connector.py,sha256=HkcSFvDlW71v6tBtMTcvAd_jQqit6Uh3YknjBu7YKmw,1370
 stix_shifter_modules/aws_athena/stix_transmission/post_query_connector_error_handling.py,sha256=7py2aaPdr2zFlRlndb42ZFvcZrDHPmO9pU-lt1z3xcc,7435
 stix_shifter_modules/aws_athena/stix_transmission/query_connector.py,sha256=r6em2euPvrgDCod82Lp3TkfVi1nZut-_gokuX1nptug,10418
 stix_shifter_modules/aws_athena/stix_transmission/results_connector.py,sha256=3J_nfleKOrrSbOGyxDYVxs4qWG1dFWY-qnJBR8jwhZY,15539
 stix_shifter_modules/aws_athena/stix_transmission/status_connector.py,sha256=cRsTNP300ggHy5d3wFr3LNP3MWr2vCO3rLr-5ZJ9zUM,3473
-stix_shifter_modules_aws_athena-7.0.7.dist-info/LICENSE.md,sha256=ssGEKMVW69oFTBblVhD1YPolqCOyOCJi4wRDRI7xCnU,12786
-stix_shifter_modules_aws_athena-7.0.7.dist-info/METADATA,sha256=U0Kgwh_wdJwhRTmsNScNuxlBI0gxVwuxQgy0wwGsH-8,7175
-stix_shifter_modules_aws_athena-7.0.7.dist-info/NOTICE,sha256=wx-gWE9vSnLJ7YQkrGlMp9VNXOXG57TTxDDRd9CEdYg,1418
-stix_shifter_modules_aws_athena-7.0.7.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
-stix_shifter_modules_aws_athena-7.0.7.dist-info/top_level.txt,sha256=NX-VgUOr8fI-lMXHt3gtjfsEn1UPaGAVszt6Z_CTp2s,21
-stix_shifter_modules_aws_athena-7.0.7.dist-info/RECORD,,
+stix_shifter_modules_aws_athena-7.0.9.dist-info/LICENSE.md,sha256=ssGEKMVW69oFTBblVhD1YPolqCOyOCJi4wRDRI7xCnU,12786
+stix_shifter_modules_aws_athena-7.0.9.dist-info/METADATA,sha256=zeYtzgLR7-ewIEmSSSDb4ODYhxntyxpI1N_qIB6xKno,7175
+stix_shifter_modules_aws_athena-7.0.9.dist-info/NOTICE,sha256=wx-gWE9vSnLJ7YQkrGlMp9VNXOXG57TTxDDRd9CEdYg,1418
+stix_shifter_modules_aws_athena-7.0.9.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
+stix_shifter_modules_aws_athena-7.0.9.dist-info/top_level.txt,sha256=NX-VgUOr8fI-lMXHt3gtjfsEn1UPaGAVszt6Z_CTp2s,21
+stix_shifter_modules_aws_athena-7.0.9.dist-info/RECORD,,
```

