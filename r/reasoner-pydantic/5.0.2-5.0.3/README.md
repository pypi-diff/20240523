# Comparing `tmp/reasoner-pydantic-5.0.2.tar.gz` & `tmp/reasoner-pydantic-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner-pydantic-5.0.2.tar", last modified: Mon Apr 15 16:09:00 2024, max compression
+gzip compressed data, was "reasoner-pydantic-5.0.3.tar", last modified: Thu May 23 20:21:52 2024, max compression
```

## Comparing `reasoner-pydantic-5.0.2.tar` & `reasoner-pydantic-5.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:09:00.662257 reasoner-pydantic-5.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-15 16:09:00.662257 reasoner-pydantic-5.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:09:00.658257 reasoner-pydantic-5.0.2/reasoner_pydantic/
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/reasoner_pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/reasoner_pydantic/auxgraphs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/reasoner_pydantic/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/reasoner_pydantic/kgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/reasoner_pydantic/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/reasoner_pydantic/metakg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/reasoner_pydantic/qgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/reasoner_pydantic/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/reasoner_pydantic/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/reasoner_pydantic/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/reasoner_pydantic/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:09:00.662257 reasoner-pydantic-5.0.2/reasoner_pydantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-15 16:09:00.000000 reasoner-pydantic-5.0.2/reasoner_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-15 16:09:00.000000 reasoner-pydantic-5.0.2/reasoner_pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:09:00.000000 reasoner-pydantic-5.0.2/reasoner_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:09:00.000000 reasoner-pydantic-5.0.2/reasoner_pydantic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 16:09:00.000000 reasoner-pydantic-5.0.2/reasoner_pydantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 16:09:00.000000 reasoner-pydantic-5.0.2/reasoner_pydantic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 16:09:00.662257 reasoner-pydantic-5.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:21:52.189895 reasoner-pydantic-5.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-23 20:21:52.189895 reasoner-pydantic-5.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-23 20:21:49.000000 reasoner-pydantic-5.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:21:52.189895 reasoner-pydantic-5.0.3/reasoner_pydantic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-23 20:21:49.000000 reasoner-pydantic-5.0.3/reasoner_pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-23 20:21:49.000000 reasoner-pydantic-5.0.3/reasoner_pydantic/auxgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-23 20:21:49.000000 reasoner-pydantic-5.0.3/reasoner_pydantic/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-23 20:21:49.000000 reasoner-pydantic-5.0.3/reasoner_pydantic/kgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-05-23 20:21:49.000000 reasoner-pydantic-5.0.3/reasoner_pydantic/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-23 20:21:49.000000 reasoner-pydantic-5.0.3/reasoner_pydantic/metakg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-05-23 20:21:49.000000 reasoner-pydantic-5.0.3/reasoner_pydantic/qgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-05-23 20:21:49.000000 reasoner-pydantic-5.0.3/reasoner_pydantic/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-23 20:21:49.000000 reasoner-pydantic-5.0.3/reasoner_pydantic/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-23 20:21:49.000000 reasoner-pydantic-5.0.3/reasoner_pydantic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12224 2024-05-23 20:21:49.000000 reasoner-pydantic-5.0.3/reasoner_pydantic/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:21:52.189895 reasoner-pydantic-5.0.3/reasoner_pydantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-23 20:21:52.000000 reasoner-pydantic-5.0.3/reasoner_pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-23 20:21:52.000000 reasoner-pydantic-5.0.3/reasoner_pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:21:52.000000 reasoner-pydantic-5.0.3/reasoner_pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:21:52.000000 reasoner-pydantic-5.0.3/reasoner_pydantic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 20:21:52.000000 reasoner-pydantic-5.0.3/reasoner_pydantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 20:21:52.000000 reasoner-pydantic-5.0.3/reasoner_pydantic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 20:21:52.189895 reasoner-pydantic-5.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-23 20:21:49.000000 reasoner-pydantic-5.0.3/setup.py
```

### Comparing `reasoner-pydantic-5.0.2/PKG-INFO` & `reasoner-pydantic-5.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 5.0.2
+Version: 5.0.3
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Abrar Mesbah
 Author-email: amesbah@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-5.0.2/README.md` & `reasoner-pydantic-5.0.3/README.md`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.2/reasoner_pydantic/__init__.py` & `reasoner-pydantic-5.0.3/reasoner_pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.2/reasoner_pydantic/auxgraphs.py` & `reasoner-pydantic-5.0.3/reasoner_pydantic/auxgraphs.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.2/reasoner_pydantic/base_model.py` & `reasoner-pydantic-5.0.3/reasoner_pydantic/base_model.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.2/reasoner_pydantic/kgraph.py` & `reasoner-pydantic-5.0.3/reasoner_pydantic/kgraph.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.2/reasoner_pydantic/message.py` & `reasoner-pydantic-5.0.3/reasoner_pydantic/message.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.2/reasoner_pydantic/metakg.py` & `reasoner-pydantic-5.0.3/reasoner_pydantic/metakg.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.2/reasoner_pydantic/qgraph.py` & `reasoner-pydantic-5.0.3/reasoner_pydantic/qgraph.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,19 +98,24 @@
         None,
         title="categories",
         nullable=True,
     )
     _nonzero_categories = validator("categories", allow_reuse=True)(nonzero_validator)
 
     set_interpretation: Optional[SetInterpretationEnum] = Field("BATCH", nullable=True)
+
     constraints: Optional[HashableSequence[AttributeConstraint]] = Field(
         default=HashableSequence[AttributeConstraint](__root__=[]),
         title="attribute constraints",
     )
 
+    member_ids: Optional[HashableSequence[CURIE]] = Field(
+        default=HashableSequence[CURIE](__root__=[]), title="set member ids"
+    )
+
     class Config:
         title = "query-graph node"
         extra = "allow"
         allow_population_by_field_name = True
 
 
 class QEdge(BaseModel):
```

### Comparing `reasoner-pydantic-5.0.2/reasoner_pydantic/results.py` & `reasoner-pydantic-5.0.3/reasoner_pydantic/results.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.2/reasoner_pydantic/shared.py` & `reasoner-pydantic-5.0.3/reasoner_pydantic/shared.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.2/reasoner_pydantic/utils.py` & `reasoner-pydantic-5.0.3/reasoner_pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.2/reasoner_pydantic/workflow.py` & `reasoner-pydantic-5.0.3/reasoner_pydantic/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,14 +298,22 @@
     id: constant("lookup")
     parameters: Optional[Any]
 
     class Config:
         extra = "forbid"
 
 
+class OperationLookupAndScore(BaseOperation):
+    id: constant("lookup_and_score")
+    parameters: Optional[Any]
+
+    class Config:
+        extra = "forbid"
+
+
 class OperationOverlay(BaseOperation):
     id: constant("overlay")
     parameters: Optional[Any]
 
     class Config:
         extra = "forbid"
 
@@ -446,14 +454,15 @@
     OperationFilterKgraphOrphans,
     OperationFilterKgraphPercentile,
     OperationFilterKgraphStdDev,
     OperationFilterKgraphTopN,
     OperationFilterResults,
     OperationFilterResultsTopN,
     OperationLookup,
+    OperationLookupAndScore,
     OperationOverlay,
     OperationOverlayComputeJaccard,
     OperationOverlayComputeNgd,
     OperationOverlayConnectKnodes,
     OperationOverlayFisherExactTest,
     OperationRestate,
     OperationScore,
@@ -480,14 +489,15 @@
         OperationFilterKgraphOrphans,
         OperationFilterKgraphPercentile,
         OperationFilterKgraphStdDev,
         OperationFilterKgraphTopN,
         OperationFilterResults,
         OperationFilterResultsTopN,
         OperationLookup,
+        OperationLookupAndScore,
         OperationOverlay,
         OperationOverlayComputeJaccard,
         OperationOverlayComputeNgd,
         OperationOverlayConnectKnodes,
         OperationOverlayFisherExactTest,
         OperationRestate,
         OperationScore,
```

### Comparing `reasoner-pydantic-5.0.2/reasoner_pydantic.egg-info/PKG-INFO` & `reasoner-pydantic-5.0.3/reasoner_pydantic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 5.0.2
+Version: 5.0.3
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Abrar Mesbah
 Author-email: amesbah@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-5.0.2/reasoner_pydantic.egg-info/SOURCES.txt` & `reasoner-pydantic-5.0.3/reasoner_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.2/setup.py` & `reasoner-pydantic-5.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="reasoner-pydantic",
-    version="5.0.2",
+    version="5.0.3",
     author="Abrar Mesbah",
     author_email="amesbah@covar.com",
     url="https://github.com/TranslatorSRI/reasoner-pydantic",
     description="Pydantic models for the Reasoner API data formats",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["reasoner_pydantic"],
```

