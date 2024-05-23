# Comparing `tmp/omnikeeper_client-6.0.1-py3-none-any.whl.zip` & `tmp/omnikeeper_client-6.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 23086 bytes, number of entries: 17
+Zip file size: 23161 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat     1434 b- defN 24-May-22 08:24 omnikeeper_client/__init__.py
 -rw-rw-rw-  2.0 fat     2045 b- defN 24-May-21 12:56 omnikeeper_client/apiclient.py
 -rw-rw-rw-  2.0 fat     5211 b- defN 24-May-21 12:56 omnikeeper_client/ci.py
 -rw-rw-rw-  2.0 fat     3907 b- defN 24-May-21 12:56 omnikeeper_client/dataframes.py
 -rw-rw-rw-  2.0 fat     1206 b- defN 24-May-22 07:59 omnikeeper_client/issues.py
 -rw-rw-rw-  2.0 fat     3354 b- defN 24-May-21 12:56 omnikeeper_client/layer.py
 -rw-rw-rw-  2.0 fat     2854 b- defN 24-May-21 12:56 omnikeeper_client/pyd.py
 -rw-rw-rw-  2.0 fat    10855 b- defN 24-May-21 12:56 omnikeeper_client/simple_traits.py
 -rw-rw-rw-  2.0 fat     4717 b- defN 24-May-21 12:56 omnikeeper_client/trait.py
--rw-rw-rw-  2.0 fat    26923 b- defN 24-May-22 08:24 omnikeeper_client/traitentities.py
+-rw-rw-rw-  2.0 fat    27264 b- defN 24-May-23 11:14 omnikeeper_client/traitentities.py
 -rw-rw-rw-  2.0 fat     5439 b- defN 24-May-21 12:56 omnikeeper_client/typing.py
 -rw-rw-rw-  2.0 fat      950 b- defN 24-May-21 12:56 omnikeeper_client/util.py
--rw-rw-rw-  2.0 fat    11558 b- defN 24-May-22 08:25 omnikeeper_client-6.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      543 b- defN 24-May-22 08:25 omnikeeper_client-6.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-22 08:25 omnikeeper_client-6.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 24-May-22 08:25 omnikeeper_client-6.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1457 b- defN 24-May-22 08:25 omnikeeper_client-6.0.1.dist-info/RECORD
-17 files, 82563 bytes uncompressed, 20682 bytes compressed:  75.0%
+-rw-rw-rw-  2.0 fat    11558 b- defN 24-May-23 11:15 omnikeeper_client-6.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      543 b- defN 24-May-23 11:15 omnikeeper_client-6.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 11:15 omnikeeper_client-6.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 24-May-23 11:15 omnikeeper_client-6.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1457 b- defN 24-May-23 11:15 omnikeeper_client-6.0.2.dist-info/RECORD
+17 files, 82904 bytes uncompressed, 20757 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: omnikeeper_client/typing.py
 Comment: 
 
 Filename: omnikeeper_client/util.py
 Comment: 
 
-Filename: omnikeeper_client-6.0.1.dist-info/LICENSE
+Filename: omnikeeper_client-6.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: omnikeeper_client-6.0.1.dist-info/METADATA
+Filename: omnikeeper_client-6.0.2.dist-info/METADATA
 Comment: 
 
-Filename: omnikeeper_client-6.0.1.dist-info/WHEEL
+Filename: omnikeeper_client-6.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: omnikeeper_client-6.0.1.dist-info/top_level.txt
+Filename: omnikeeper_client-6.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: omnikeeper_client-6.0.1.dist-info/RECORD
+Filename: omnikeeper_client-6.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## omnikeeper_client/traitentities.py

```diff
@@ -182,15 +182,19 @@
 
         result = session.execute(query, variable_values={"layers": layers})
 
         data_list = result['traitEntities'][prefixed_escaped_trait_id]['all']
         for data in data_list:
             data.update(data.pop('entity'))
 
-        return data_list
+        def unescape_trait_attribute_name(name: str) -> str:
+            return name.replace("__", ".")
+        final_output = [{unescape_trait_attribute_name(k): v for k, v in d.items()} for d in data_list]
+        
+        return final_output
     
   
 def get_all_traitentities(ok_api_client: okc.OkApiClient, trait_id: str, layers: List[str]) -> List[Dict[str,Any]]:
     """
     Returns all traitentites
 
     Parameters
@@ -507,16 +511,18 @@
             writeLayer: $writeLayer
             input: $input
         ) {{
             success
         }}
         }}
         """)
-        
-    final_input = [{"ciid": d["ciid"], "attributes": {k: v for k, v in d.items() if k != "ciid"}} for d in input]
+
+    def escape_trait_attribute_name(name: str) -> str:
+        return name.replace(".", "__")
+    final_input = [{"ciid": d["ciid"], "attributes": {escape_trait_attribute_name(k): v for k, v in d.items() if k != "ciid"}} for d in input]
         
     if read_layers is None:
         read_layers = [write_layer]
     result = ok_api_client.execute_graphql(query, variables=dict(
         writeLayer=write_layer, 
         readLayers=read_layers, 
         input=final_input
```

## Comparing `omnikeeper_client-6.0.1.dist-info/LICENSE` & `omnikeeper_client-6.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `omnikeeper_client-6.0.1.dist-info/METADATA` & `omnikeeper_client-6.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnikeeper-client
-Version: 6.0.1
+Version: 6.0.2
 Summary: Python library containing helper functions for implementing omnikeeper clients
 Author: Maximilian Csuk
 License: Apache 2.0
 License-File: LICENSE
 Requires-Dist: appengine-python-standard ~=1.1
 Requires-Dist: gql ~=3.4
 Requires-Dist: oauthlib ~=3.2
```

## Comparing `omnikeeper_client-6.0.1.dist-info/RECORD` & `omnikeeper_client-6.0.2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 omnikeeper_client/ci.py,sha256=c_P-_uLvInTALzJvC06n8HJ6iCgS14RZ2pKee91AMKI,5211
 omnikeeper_client/dataframes.py,sha256=0snXt4Io2HBxlsGc28OI6OnTm-Qyj06nyk0AA-P-sh4,3907
 omnikeeper_client/issues.py,sha256=gFjc5PhniIMUQIthBoMG1s3enG8ExWeoRhBcZcZrQJo,1206
 omnikeeper_client/layer.py,sha256=9r928gw20H_0TYFfPv972cLAiX4B-HdCny3j_F9L-vc,3354
 omnikeeper_client/pyd.py,sha256=h2Va7Gd4-I0p6X6Yizv2ebExgsukDKIjYCxjCOddCi4,2854
 omnikeeper_client/simple_traits.py,sha256=HkPV4Rkf70oDXUwhSSA9dVEHCxtI5K3uGd4XmRQaUaA,10855
 omnikeeper_client/trait.py,sha256=RU312IWCCKpwso2xn1X4LumZzwnKga53UTxnHBtufxU,4717
-omnikeeper_client/traitentities.py,sha256=41wmOWW-TWKpHzq0_juigYxzRxSRwftoVath8B_eFtg,26923
+omnikeeper_client/traitentities.py,sha256=iyT_ppXlVYl4OBnCB4DAVvzKGUS789DnSs7n-Oe9BB0,27264
 omnikeeper_client/typing.py,sha256=ULabK159CSXDtdjnIAapygV5uewbORVpIU7DCCuCIUM,5439
 omnikeeper_client/util.py,sha256=Cl9HnU5nc4XXmg8I5wUeirt50lLkGKiLnUHhKZeYtCE,950
-omnikeeper_client-6.0.1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-omnikeeper_client-6.0.1.dist-info/METADATA,sha256=EFCS9skMaXMR_9B0eTb9E2SoL6ep_4_J2nRrA1GHhn0,543
-omnikeeper_client-6.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-omnikeeper_client-6.0.1.dist-info/top_level.txt,sha256=3VgpRS-e1mbaX1mKkPt9Mszwazf6tc1Tk3GORBV6ijk,18
-omnikeeper_client-6.0.1.dist-info/RECORD,,
+omnikeeper_client-6.0.2.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+omnikeeper_client-6.0.2.dist-info/METADATA,sha256=EH29tN4VkbTccMYnGQYFHHmm8zUjtYS2VsYXa25Zc4U,543
+omnikeeper_client-6.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+omnikeeper_client-6.0.2.dist-info/top_level.txt,sha256=3VgpRS-e1mbaX1mKkPt9Mszwazf6tc1Tk3GORBV6ijk,18
+omnikeeper_client-6.0.2.dist-info/RECORD,,
```

