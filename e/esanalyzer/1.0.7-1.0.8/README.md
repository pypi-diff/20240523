# Comparing `tmp/esanalyzer-1.0.7-py3-none-any.whl.zip` & `tmp/esanalyzer-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 7959 bytes, number of entries: 6
+Zip file size: 8004 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat    23353 b- defN 24-May-22 12:18 esanalyzer.py
--rw-rw-rw-  2.0 fat     1074 b- defN 24-May-22 12:18 esanalyzer-1.0.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1806 b- defN 24-May-22 12:18 esanalyzer-1.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-22 12:18 esanalyzer-1.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 24-May-22 12:18 esanalyzer-1.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      472 b- defN 24-May-22 12:18 esanalyzer-1.0.7.dist-info/RECORD
-6 files, 26808 bytes uncompressed, 7107 bytes compressed:  73.5%
+-rw-rw-rw-  2.0 fat     1074 b- defN 24-May-22 12:53 esanalyzer-1.0.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1976 b- defN 24-May-22 12:53 esanalyzer-1.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-22 12:53 esanalyzer-1.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-May-22 12:53 esanalyzer-1.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      472 b- defN 24-May-22 12:53 esanalyzer-1.0.8.dist-info/RECORD
+6 files, 26978 bytes uncompressed, 7152 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: esanalyzer.py
 Comment: 
 
-Filename: esanalyzer-1.0.7.dist-info/LICENSE
+Filename: esanalyzer-1.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: esanalyzer-1.0.7.dist-info/METADATA
+Filename: esanalyzer-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: esanalyzer-1.0.7.dist-info/WHEEL
+Filename: esanalyzer-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: esanalyzer-1.0.7.dist-info/top_level.txt
+Filename: esanalyzer-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: esanalyzer-1.0.7.dist-info/RECORD
+Filename: esanalyzer-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `esanalyzer-1.0.7.dist-info/LICENSE` & `esanalyzer-1.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `esanalyzer-1.0.7.dist-info/METADATA` & `esanalyzer-1.0.8.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: esanalyzer
-Version: 1.0.7
+Version: 1.0.8
 Summary: Emotion("fear", "anger", "surprise", "sadness", "disgust", "joy") and Sentiment("Positive","Negative") Analysis
-Home-page: https://github.com/ajaysingh111444/python/tree/esanalyzer/esanalyzer/version/1.0.7
+Home-page: https://github.com/ajaysingh111444/python/tree/esanalyzer/esanalyzer/version/1.0.8
 Author: Ajay Singh Rajput
-Requires-Python: >=3.6
+Requires-Python: >=3.12.3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nrclex ==3.0.0
 Requires-Dist: datasets ==2.16.1
 Requires-Dist: scikit-learn ==1.3.2
 Requires-Dist: pandas ==2.1.4
 Requires-Dist: numpy ==1.26.3
 Requires-Dist: googletrans ==4.0.0-rc1
 Requires-Dist: transformers ==4.36.2
 Requires-Dist: nltk ==3.8.1
+Requires-Dist: torch ==2.3.0
+Requires-Dist: torchvision ==0.18.0
+Requires-Dist: torchaudio ==2.3.0
+Requires-Dist: tensorflow ==2.16.1
+Requires-Dist: flax ==0.8.3
 
 # esanalyzer
 
     The Python Emotion Analysis and Sentiment Analysis library you've been looking for.
 
     ## Services
     - Emotion Analysis("fear", "anger", "surprise", "sadness", "disgust", "joy")
```

