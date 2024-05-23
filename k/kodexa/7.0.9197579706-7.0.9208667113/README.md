# Comparing `tmp/kodexa-7.0.9197579706.tar.gz` & `tmp/kodexa-7.0.9208667113.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-7.0.9197579706.tar", max compression
+gzip compressed data, was "kodexa-7.0.9208667113.tar", max compression
```

## Comparing `kodexa-7.0.9197579706.tar` & `kodexa-7.0.9208667113.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    11357 2024-05-22 19:57:34.516972 kodexa-7.0.9197579706/LICENSE
--rw-r--r--   0        0        0     2178 2024-05-22 19:57:34.516972 kodexa-7.0.9197579706/README.md
--rw-r--r--   0        0        0      957 2024-05-22 19:57:34.520973 kodexa-7.0.9197579706/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2024-05-22 19:57:34.520973 kodexa-7.0.9197579706/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    14663 2024-05-22 19:57:34.520973 kodexa-7.0.9197579706/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      328 2024-05-22 19:57:34.520973 kodexa-7.0.9197579706/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0    10413 2024-05-22 19:57:34.520973 kodexa-7.0.9197579706/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      796 2024-05-22 19:57:34.520973 kodexa-7.0.9197579706/kodexa/model/__init__.py
--rw-r--r--   0        0        0      521 2024-05-22 19:57:34.520973 kodexa-7.0.9197579706/kodexa/model/base.py
--rw-r--r--   0        0        0        0 2024-05-22 19:57:34.520973 kodexa-7.0.9197579706/kodexa/model/entities/__init__.py
--rw-r--r--   0        0        0     3526 2024-05-22 19:57:34.520973 kodexa-7.0.9197579706/kodexa/model/entities/product.py
--rw-r--r--   0        0        0     3810 2024-05-22 19:57:34.520973 kodexa-7.0.9197579706/kodexa/model/entities/product_subscription.py
--rw-r--r--   0        0        0   115561 2024-05-22 19:57:34.520973 kodexa-7.0.9197579706/kodexa/model/model.py
--rw-r--r--   0        0        0   174335 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/model/objects.py
--rw-r--r--   0        0        0    62032 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    25221 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   218354 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/platform/client.py
--rw-r--r--   0        0        0     1055 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/platform/interaction.py
--rw-r--r--   0        0        0    34024 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13269 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3691 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3447 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     3155 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       61 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7068 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       61 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    71452 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       61 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    30564 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     5975 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    44214 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      179 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/steps/__init__.py
--rw-r--r--   0        0        0    10428 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/steps/common.py
--rw-r--r--   0        0        0      323 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/testing/__init__.py
--rw-r--r--   0        0        0     1052 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    14021 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 19:57:34.524973 kodexa-7.0.9197579706/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1373 2024-05-22 19:57:46.661052 kodexa-7.0.9197579706/pyproject.toml
--rw-r--r--   0        0        0     3486 1970-01-01 00:00:00.000000 kodexa-7.0.9197579706/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-23 13:13:09.556251 kodexa-7.0.9208667113/LICENSE
+-rw-r--r--   0        0        0     2178 2024-05-23 13:13:09.556251 kodexa-7.0.9208667113/README.md
+-rw-r--r--   0        0        0      957 2024-05-23 13:13:09.564251 kodexa-7.0.9208667113/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2024-05-23 13:13:09.564251 kodexa-7.0.9208667113/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    14663 2024-05-23 13:13:09.564251 kodexa-7.0.9208667113/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      328 2024-05-23 13:13:09.564251 kodexa-7.0.9208667113/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0    10413 2024-05-23 13:13:09.564251 kodexa-7.0.9208667113/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      796 2024-05-23 13:13:09.564251 kodexa-7.0.9208667113/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      521 2024-05-23 13:13:09.564251 kodexa-7.0.9208667113/kodexa/model/base.py
+-rw-r--r--   0        0        0        0 2024-05-23 13:13:09.564251 kodexa-7.0.9208667113/kodexa/model/entities/__init__.py
+-rw-r--r--   0        0        0     3526 2024-05-23 13:13:09.564251 kodexa-7.0.9208667113/kodexa/model/entities/product.py
+-rw-r--r--   0        0        0     3810 2024-05-23 13:13:09.564251 kodexa-7.0.9208667113/kodexa/model/entities/product_subscription.py
+-rw-r--r--   0        0        0   115561 2024-05-23 13:13:09.564251 kodexa-7.0.9208667113/kodexa/model/model.py
+-rw-r--r--   0        0        0   174335 2024-05-23 13:13:09.564251 kodexa-7.0.9208667113/kodexa/model/objects.py
+-rw-r--r--   0        0        0    62032 2024-05-23 13:13:09.564251 kodexa-7.0.9208667113/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    25221 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   219663 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/platform/client.py
+-rw-r--r--   0        0        0     1055 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/platform/interaction.py
+-rw-r--r--   0        0        0    34024 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13269 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3691 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3447 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     3155 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       61 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7068 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       61 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    71452 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       61 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    30564 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     5975 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    44214 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      179 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0    10428 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/steps/common.py
+-rw-r--r--   0        0        0      323 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0     1052 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    14021 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 13:13:09.568251 kodexa-7.0.9208667113/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1373 2024-05-23 13:13:22.812435 kodexa-7.0.9208667113/pyproject.toml
+-rw-r--r--   0        0        0     3486 1970-01-01 00:00:00.000000 kodexa-7.0.9208667113/PKG-INFO
```

### Comparing `kodexa-7.0.9197579706/LICENSE` & `kodexa-7.0.9208667113/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/README.md` & `kodexa-7.0.9208667113/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/__init__.py` & `kodexa-7.0.9208667113/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/assistant/assistant.py` & `kodexa-7.0.9208667113/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/connectors/connectors.py` & `kodexa-7.0.9208667113/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/model/__init__.py` & `kodexa-7.0.9208667113/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/model/base.py` & `kodexa-7.0.9208667113/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/model/entities/product.py` & `kodexa-7.0.9208667113/kodexa/model/entities/product.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/model/entities/product_subscription.py` & `kodexa-7.0.9208667113/kodexa/model/entities/product_subscription.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/model/model.py` & `kodexa-7.0.9208667113/kodexa/model/model.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/model/objects.py` & `kodexa-7.0.9208667113/kodexa/model/objects.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/model/persistence.py` & `kodexa-7.0.9208667113/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/pipeline/pipeline.py` & `kodexa-7.0.9208667113/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/platform/client.py` & `kodexa-7.0.9208667113/kodexa/platform/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2077,14 +2077,46 @@
 
         Returns:
             DocumentStoreEndpoint: The instance class of the project document stores endpoint.
         """
         return DocumentStoreEndpoint
 
 
+class ProjectDashboardsEndpoint(ProjectResourceEndpoint):
+    """Represents a project dashboards endpoint.
+
+    This class is used to represent a project document stores endpoint in the system.
+    """
+
+    """Represents a project document stores endpoint"""
+
+    def get_type(self) -> str:
+        """Get the type of the endpoint.
+
+        This method is used to get the type of the endpoint.
+
+        Returns:
+            str: The type of the endpoint.
+        """
+        return "dashboards"
+
+    def get_instance_class(self, object_dict=None):
+        """Get the instance class of the project document stores endpoint.
+
+        This method is used to get the instance class of the project document stores endpoint.
+
+        Args:
+            object_dict (dict, optional): The object dictionary. Defaults to None.
+
+        Returns:
+            DocumentStoreEndpoint: The instance class of the project document stores endpoint.
+        """
+        return DashboardEndpoint
+
+
 class GuidanceSetEndpoint(ComponentInstanceEndpoint, GuidanceSet):
 
     def get_type(self) -> str:
         """
         Get the type of the endpoint.
 
         Returns:
@@ -2514,14 +2546,23 @@
 
         self.client.put(
             f"/api/projects/{self.id}/resources",
             body=json.loads(project_resources_update.json(by_alias=True)),
         )
 
     @property
+    def dashboards(self) -> ProjectDashboardsEndpoint:
+        """Get the document stores endpoint of the project.
+
+        Returns:
+            ProjectDocumentStoresEndpoint: The document stores endpoint of the project.
+        """
+        return ProjectDashboardsEndpoint().set_client(self.client).set_project(self)
+
+    @property
     def document_stores(self) -> ProjectDocumentStoresEndpoint:
         """Get the document stores endpoint of the project.
 
         Returns:
             ProjectDocumentStoresEndpoint: The document stores endpoint of the project.
         """
         return ProjectDocumentStoresEndpoint().set_client(self.client).set_project(self)
@@ -2592,15 +2633,14 @@
         response = self.client.put(
             f"/api/projects/{self.id}/tags",
             body=[tag.model_dump(by_alias=True) for tag in tags],
         )
         return [ProjectTag.model_validate(tag) for tag in response.json()]
 
 
-
 class MessagesEndpoint(EntitiesEndpoint):
     """Represents a message endpoint"""
 
     def get_type(self) -> str:
         """
         Get the type of the endpoint.
```

### Comparing `kodexa-7.0.9197579706/kodexa/platform/interaction.py` & `kodexa-7.0.9208667113/kodexa/platform/interaction.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/platform/kodexa.py` & `kodexa-7.0.9208667113/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/selectors/ast.py` & `kodexa-7.0.9208667113/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/selectors/core.py` & `kodexa-7.0.9208667113/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/selectors/lexrules.py` & `kodexa-7.0.9208667113/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/selectors/lextab.py` & `kodexa-7.0.9208667113/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/selectors/parserules.py` & `kodexa-7.0.9208667113/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/selectors/parsetab.py` & `kodexa-7.0.9208667113/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/spatial/azure_models.py` & `kodexa-7.0.9208667113/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/spatial/bbox_common.py` & `kodexa-7.0.9208667113/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/spatial/table_form_common.py` & `kodexa-7.0.9208667113/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/steps/common.py` & `kodexa-7.0.9208667113/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/testing/test_components.py` & `kodexa-7.0.9208667113/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/kodexa/testing/test_utils.py` & `kodexa-7.0.9208667113/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9197579706/pyproject.toml` & `kodexa-7.0.9208667113/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "7.0.09197579706"
+version = "7.0.09208667113"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-7.0.9197579706/PKG-INFO` & `kodexa-7.0.9208667113/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 7.0.9197579706
+Version: 7.0.9208667113
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```
