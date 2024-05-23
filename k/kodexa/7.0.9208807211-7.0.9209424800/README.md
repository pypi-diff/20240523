# Comparing `tmp/kodexa-7.0.9208807211.tar.gz` & `tmp/kodexa-7.0.9209424800.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-7.0.9208807211.tar", max compression
+gzip compressed data, was "kodexa-7.0.9209424800.tar", max compression
```

## Comparing `kodexa-7.0.9208807211.tar` & `kodexa-7.0.9209424800.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    11357 2024-05-23 13:21:48.683934 kodexa-7.0.9208807211/LICENSE
--rw-r--r--   0        0        0     2178 2024-05-23 13:21:48.683934 kodexa-7.0.9208807211/README.md
--rw-r--r--   0        0        0      957 2024-05-23 13:21:48.687934 kodexa-7.0.9208807211/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2024-05-23 13:21:48.687934 kodexa-7.0.9208807211/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    14663 2024-05-23 13:21:48.687934 kodexa-7.0.9208807211/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      328 2024-05-23 13:21:48.687934 kodexa-7.0.9208807211/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0    10413 2024-05-23 13:21:48.687934 kodexa-7.0.9208807211/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      796 2024-05-23 13:21:48.687934 kodexa-7.0.9208807211/kodexa/model/__init__.py
--rw-r--r--   0        0        0      521 2024-05-23 13:21:48.687934 kodexa-7.0.9208807211/kodexa/model/base.py
--rw-r--r--   0        0        0        0 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/model/entities/__init__.py
--rw-r--r--   0        0        0     3526 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/model/entities/product.py
--rw-r--r--   0        0        0     3810 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/model/entities/product_subscription.py
--rw-r--r--   0        0        0   115561 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/model/model.py
--rw-r--r--   0        0        0   174335 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/model/objects.py
--rw-r--r--   0        0        0    62032 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    25221 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   220924 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/platform/client.py
--rw-r--r--   0        0        0     1055 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/platform/interaction.py
--rw-r--r--   0        0        0    34024 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13269 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3691 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3447 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     3155 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       61 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7068 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       61 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    71452 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       61 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    30564 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     5975 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    44214 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      179 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/steps/__init__.py
--rw-r--r--   0        0        0    10428 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/steps/common.py
--rw-r--r--   0        0        0      323 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/testing/__init__.py
--rw-r--r--   0        0        0     1052 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    14021 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 13:21:48.691933 kodexa-7.0.9208807211/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1373 2024-05-23 13:22:01.803954 kodexa-7.0.9208807211/pyproject.toml
--rw-r--r--   0        0        0     3486 1970-01-01 00:00:00.000000 kodexa-7.0.9208807211/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-23 14:03:19.503305 kodexa-7.0.9209424800/LICENSE
+-rw-r--r--   0        0        0     2178 2024-05-23 14:03:19.503305 kodexa-7.0.9209424800/README.md
+-rw-r--r--   0        0        0      957 2024-05-23 14:03:19.507305 kodexa-7.0.9209424800/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2024-05-23 14:03:19.507305 kodexa-7.0.9209424800/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    14663 2024-05-23 14:03:19.507305 kodexa-7.0.9209424800/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      328 2024-05-23 14:03:19.507305 kodexa-7.0.9209424800/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0    10413 2024-05-23 14:03:19.507305 kodexa-7.0.9209424800/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      796 2024-05-23 14:03:19.507305 kodexa-7.0.9209424800/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      521 2024-05-23 14:03:19.507305 kodexa-7.0.9209424800/kodexa/model/base.py
+-rw-r--r--   0        0        0        0 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/model/entities/__init__.py
+-rw-r--r--   0        0        0     3526 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/model/entities/product.py
+-rw-r--r--   0        0        0     3810 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/model/entities/product_subscription.py
+-rw-r--r--   0        0        0   115561 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/model/model.py
+-rw-r--r--   0        0        0   174417 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/model/objects.py
+-rw-r--r--   0        0        0    62032 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    25221 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   220924 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/platform/client.py
+-rw-r--r--   0        0        0     1055 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/platform/interaction.py
+-rw-r--r--   0        0        0    34024 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13269 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3691 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3447 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     3155 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       61 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7068 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       61 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    71452 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       61 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    30564 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     5975 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    44214 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      179 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0    10428 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/steps/common.py
+-rw-r--r--   0        0        0      323 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0     1052 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    14021 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 14:03:19.511305 kodexa-7.0.9209424800/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1373 2024-05-23 14:03:31.391191 kodexa-7.0.9209424800/pyproject.toml
+-rw-r--r--   0        0        0     3486 1970-01-01 00:00:00.000000 kodexa-7.0.9209424800/PKG-INFO
```

### Comparing `kodexa-7.0.9208807211/LICENSE` & `kodexa-7.0.9209424800/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/README.md` & `kodexa-7.0.9209424800/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/__init__.py` & `kodexa-7.0.9209424800/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/assistant/assistant.py` & `kodexa-7.0.9209424800/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/connectors/connectors.py` & `kodexa-7.0.9209424800/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/model/__init__.py` & `kodexa-7.0.9209424800/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/model/base.py` & `kodexa-7.0.9209424800/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/model/entities/product.py` & `kodexa-7.0.9209424800/kodexa/model/entities/product.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/model/entities/product_subscription.py` & `kodexa-7.0.9209424800/kodexa/model/entities/product_subscription.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/model/model.py` & `kodexa-7.0.9209424800/kodexa/model/model.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/model/objects.py` & `kodexa-7.0.9209424800/kodexa/model/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1728,14 +1728,15 @@
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
     taxonomy_refs: Optional[List[str]] = Field(None, alias="taxonomyRefs")
     store_refs: Optional[List[str]] = Field(None, alias="storeRefs")
     dashboard_refs: Optional[List[str]] = Field(None, alias="dashboardRefs")
     data_form_refs: Optional[List[str]] = Field(None, alias="dataFormRefs")
+    guidance_set_refs: Optional[List[str]] = Field(None, alias="guidanceSetRefs")
 
 
 class Role1(Enum):
     """
 
     """
     owner = "OWNER"
```

### Comparing `kodexa-7.0.9208807211/kodexa/model/persistence.py` & `kodexa-7.0.9209424800/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/pipeline/pipeline.py` & `kodexa-7.0.9209424800/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/platform/client.py` & `kodexa-7.0.9209424800/kodexa/platform/client.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/platform/interaction.py` & `kodexa-7.0.9209424800/kodexa/platform/interaction.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/platform/kodexa.py` & `kodexa-7.0.9209424800/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/selectors/ast.py` & `kodexa-7.0.9209424800/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/selectors/core.py` & `kodexa-7.0.9209424800/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/selectors/lexrules.py` & `kodexa-7.0.9209424800/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/selectors/lextab.py` & `kodexa-7.0.9209424800/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/selectors/parserules.py` & `kodexa-7.0.9209424800/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/selectors/parsetab.py` & `kodexa-7.0.9209424800/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/spatial/azure_models.py` & `kodexa-7.0.9209424800/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/spatial/bbox_common.py` & `kodexa-7.0.9209424800/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/spatial/table_form_common.py` & `kodexa-7.0.9209424800/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/steps/common.py` & `kodexa-7.0.9209424800/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/testing/test_components.py` & `kodexa-7.0.9209424800/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/kodexa/testing/test_utils.py` & `kodexa-7.0.9209424800/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9208807211/pyproject.toml` & `kodexa-7.0.9209424800/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "7.0.09208807211"
+version = "7.0.09209424800"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-7.0.9208807211/PKG-INFO` & `kodexa-7.0.9209424800/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 7.0.9208807211
+Version: 7.0.9209424800
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

