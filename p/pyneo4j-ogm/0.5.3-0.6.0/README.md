# Comparing `tmp/pyneo4j_ogm-0.5.3.tar.gz` & `tmp/pyneo4j_ogm-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneo4j_ogm-0.5.3.tar", max compression
+gzip compressed data, was "pyneo4j_ogm-0.6.0.tar", max compression
```

## Comparing `pyneo4j_ogm-0.5.3.tar` & `pyneo4j_ogm-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1070 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/LICENSE
--rw-r--r--   0        0        0    22292 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/README.md
--rw-r--r--   0        0        0      415 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/__init__.py
--rw-r--r--   0        0        0    39179 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/core/base.py
--rw-r--r--   0        0        0    33617 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/core/client.py
--rw-r--r--   0        0        0    47837 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/core/node.py
--rw-r--r--   0        0        0    32758 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/core/relationship.py
--rw-r--r--   0        0        0     7053 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/exceptions.py
--rw-r--r--   0        0        0     1864 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/fields/property_options.py
--rw-r--r--   0        0        0    45294 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/fields/relationship_property.py
--rw-r--r--   0        0        0     2025 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/fields/settings.py
--rw-r--r--   0        0        0      749 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/logger.py
--rw-r--r--   0        0        0      203 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/__init__.py
--rw-r--r--   0        0        0     1680 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/actions/create.py
--rw-r--r--   0        0        0     2746 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/actions/down.py
--rw-r--r--   0        0        0     2087 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/actions/init.py
--rw-r--r--   0        0        0     3945 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/actions/status.py
--rw-r--r--   0        0        0     2368 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/actions/up.py
--rw-r--r--   0        0        0     3888 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/cli.py
--rw-r--r--   0        0        0     3718 2024-05-13 10:57:00.249032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/utils/client.py
--rw-r--r--   0        0        0      640 2024-05-13 10:57:00.249032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/utils/defaults.py
--rw-r--r--   0        0        0     3334 2024-05-13 10:57:00.249032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/utils/migration.py
--rw-r--r--   0        0        0     4429 2024-05-13 10:57:00.249032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/utils/models.py
--rw-r--r--   0        0        0     1951 2024-05-13 10:57:00.249032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/pydantic_utils.py
--rw-r--r--   0        0        0    17636 2024-05-13 10:57:00.249032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/queries/operators.py
--rw-r--r--   0        0        0    16707 2024-05-13 10:57:00.249032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/queries/query_builder.py
--rw-r--r--   0        0        0     5945 2024-05-13 10:57:00.249032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/queries/types.py
--rw-r--r--   0        0        0    14993 2024-05-13 10:57:00.249032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/queries/validators.py
--rw-r--r--   0        0        0     2744 2024-05-13 10:57:01.945021 pyneo4j_ogm-0.5.3/pyproject.toml
--rw-r--r--   0        0        0    23595 1970-01-01 00:00:00.000000 pyneo4j_ogm-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-23 09:47:14.054977 pyneo4j_ogm-0.6.0/LICENSE
+-rw-r--r--   0        0        0    22292 2024-05-23 09:47:14.054977 pyneo4j_ogm-0.6.0/README.md
+-rw-r--r--   0        0        0      415 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/__init__.py
+-rw-r--r--   0        0        0    39179 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/core/base.py
+-rw-r--r--   0        0        0    34256 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/core/client.py
+-rw-r--r--   0        0        0    47837 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/core/node.py
+-rw-r--r--   0        0        0    32758 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/core/relationship.py
+-rw-r--r--   0        0        0     6507 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/exceptions.py
+-rw-r--r--   0        0        0     1864 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/fields/property_options.py
+-rw-r--r--   0        0        0    45294 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/fields/relationship_property.py
+-rw-r--r--   0        0        0     2025 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/fields/settings.py
+-rw-r--r--   0        0        0      749 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/logger.py
+-rw-r--r--   0        0        0      203 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/migrations/__init__.py
+-rw-r--r--   0        0        0     1680 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/migrations/actions/create.py
+-rw-r--r--   0        0        0     2746 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/migrations/actions/down.py
+-rw-r--r--   0        0        0     2087 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/migrations/actions/init.py
+-rw-r--r--   0        0        0     3945 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/migrations/actions/status.py
+-rw-r--r--   0        0        0     2368 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/migrations/actions/up.py
+-rw-r--r--   0        0        0     3888 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/migrations/cli.py
+-rw-r--r--   0        0        0     3718 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/migrations/utils/client.py
+-rw-r--r--   0        0        0      640 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/migrations/utils/defaults.py
+-rw-r--r--   0        0        0     3334 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/migrations/utils/migration.py
+-rw-r--r--   0        0        0     4429 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/migrations/utils/models.py
+-rw-r--r--   0        0        0     1951 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/pydantic_utils.py
+-rw-r--r--   0        0        0    17636 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/queries/operators.py
+-rw-r--r--   0        0        0    16707 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/queries/query_builder.py
+-rw-r--r--   0        0        0     5945 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/queries/types.py
+-rw-r--r--   0        0        0    14993 2024-05-23 09:47:14.058977 pyneo4j_ogm-0.6.0/pyneo4j_ogm/queries/validators.py
+-rw-r--r--   0        0        0     2744 2024-05-23 09:47:16.170989 pyneo4j_ogm-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    23595 1970-01-01 00:00:00.000000 pyneo4j_ogm-0.6.0/PKG-INFO
```

### Comparing `pyneo4j_ogm-0.5.3/LICENSE` & `pyneo4j_ogm-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/README.md` & `pyneo4j_ogm-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/core/base.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/core/base.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/core/client.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/core/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 """
 Pyneo4j database client class for running operations on the database.
 """
 
+import importlib.util
+import inspect
 import os
 from enum import Enum
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Type, Union, cast
 
 from neo4j import AsyncDriver, AsyncGraphDatabase, AsyncSession, AsyncTransaction
 from neo4j.exceptions import DatabaseError
 from neo4j.graph import Node, Path, Relationship
 from typing_extensions import LiteralString
 
 from pyneo4j_ogm.core.node import NodeModel
 from pyneo4j_ogm.core.relationship import RelationshipModel
 from pyneo4j_ogm.exceptions import (
-    AlreadyRegistered,
     InvalidBookmark,
     InvalidEntityType,
     InvalidLabelOrType,
     MissingDatabaseURI,
     NotConnectedToDatabase,
     TransactionInProgress,
     UnsupportedNeo4jVersion,
 )
-from pyneo4j_ogm.fields.settings import NodeModelSettings, RelationshipModelSettings
 from pyneo4j_ogm.logger import logger
 from pyneo4j_ogm.pydantic_utils import get_field_type, get_model_fields
 from pyneo4j_ogm.queries.query_builder import QueryBuilder
 
 
 class EntityType(str, Enum):
     """
@@ -135,93 +135,72 @@
         if int(version.split(".")[0]) < 5:
             raise UnsupportedNeo4jVersion()
 
         logger.info("Connected to database")
         return self
 
     @ensure_connection
+    async def register_models_from_directory(self, dir_path: str) -> None:
+        """
+        Registers all models in a directory and all subdirectories.
+        """
+        logger.info("Registering models in directory %s", dir_path)
+        for root, _, files in os.walk(dir_path):
+            # Check all files for models
+            logger.debug("Checking %s files for models", len(files))
+            for file in files:
+                if not file.endswith(".py"):
+                    continue
+
+                filepath = os.path.join(root, file)
+
+                # Load the module
+                logger.debug("Found file %s, importing", filepath)
+                module_name = os.path.splitext(os.path.basename(filepath))[0]
+                spec = importlib.util.spec_from_file_location(module_name, filepath)
+
+                if spec is None or spec.loader is None:
+                    raise ImportError(f"Could not import migration file {filepath}")
+
+                module = importlib.util.module_from_spec(spec)
+                spec.loader.exec_module(module)
+
+                for member in inspect.getmembers(
+                    module,
+                    lambda x: inspect.isclass(x)
+                    and issubclass(x, (NodeModel, RelationshipModel))
+                    and x is not NodeModel
+                    and x is not RelationshipModel,
+                ):
+                    self.models.add(member[1])
+
+        await self._prepare_registered_models()
+
+    @ensure_connection
     async def register_models(self, models: List[Type[Union[NodeModel, RelationshipModel]]]) -> None:
         """
         Registers models which are used with the client to resolve query results to their
         corresponding model instances.
 
         If a model is not registered with the client, it can not be used with model methods and other
         models can not use it with relationship-properties.
 
         Args:
             models (List[Type[NodeModel | RelationshipModel]]): A list of models to register.
         """
         logger.info("Registering models %s with client %s", models, self)
 
         for model in models:
-            for registered_model in self.models:
-                registered_model_settings = registered_model.model_settings()
-                model_settings = model.model_settings()
-
-                if (
-                    isinstance(registered_model_settings, RelationshipModelSettings)
-                    and isinstance(model_settings, RelationshipModelSettings)
-                    and registered_model_settings.type == model_settings.type
-                ):
-                    raise AlreadyRegistered(cast(str, model_settings.type))
-                elif (
-                    isinstance(registered_model_settings, NodeModelSettings)
-                    and isinstance(model_settings, NodeModelSettings)
-                    and set(registered_model_settings.labels) == set(model_settings.labels)
-                ):
-                    raise AlreadyRegistered(cast(str, model_settings.labels))
-
             if issubclass(model, (NodeModel, RelationshipModel)):
                 logger.debug("Found valid mode %s, registering with client", model.__name__)
 
                 # If the model is a valid model, add it to the set of models stored by the client
                 self.models.add(model)
-                setattr(model, "_client", self)
 
-                for property_name, property_definition in get_model_fields(model).items():
-                    entity_type = EntityType.NODE if issubclass(model, NodeModel) else EntityType.RELATIONSHIP
-                    labels_or_type = (
-                        list(getattr(model._settings, "labels"))
-                        if issubclass(model, NodeModel)
-                        else getattr(model._settings, "type")
-                    )
-
-                    # Check if we need to create any constraints
-                    if not self._skip_constraints:
-                        if getattr(get_field_type(property_definition), "_unique", False):
-                            await self.create_uniqueness_constraint(
-                                name=model.__name__,
-                                entity_type=entity_type,
-                                properties=[property_name],
-                                labels_or_type=labels_or_type,
-                            )
-
-                    # Check if we need to create any indexes
-                    if not self._skip_indexes:
-                        if getattr(get_field_type(property_definition), "_range_index", False):
-                            await self.create_range_index(
-                                name=model.__name__,
-                                entity_type=entity_type,
-                                properties=[property_name],
-                                labels_or_type=labels_or_type,
-                            )
-                        if getattr(get_field_type(property_definition), "_point_index", False):
-                            await self.create_point_index(
-                                name=model.__name__,
-                                entity_type=entity_type,
-                                properties=[property_name],
-                                labels_or_type=labels_or_type,
-                            )
-                        if getattr(get_field_type(property_definition), "_text_index", False):
-                            await self.create_text_index(
-                                name=model.__name__,
-                                entity_type=entity_type,
-                                properties=[property_name],
-                                labels_or_type=labels_or_type,
-                            )
+        await self._prepare_registered_models()
 
     @ensure_connection
     async def close(self) -> None:
         """
         Closes the current connection to the database.
         """
         if not self.is_connected:
@@ -760,14 +739,64 @@
 
             logger.debug("No registered model found for query result %s", query_result)
             return None
 
         logger.debug("Query result %s is not a node, relationship, or path, skipping", type(query_result))
         return None
 
+    async def _prepare_registered_models(self) -> None:
+        """
+        Prepares the registered models by setting the client and creating all indexes and constraints.
+        """
+
+        for model in self.models:
+            setattr(model, "_client", self)
+
+            for property_name, property_definition in get_model_fields(model).items():
+                entity_type = EntityType.NODE if issubclass(model, NodeModel) else EntityType.RELATIONSHIP
+                labels_or_type = (
+                    list(getattr(model._settings, "labels"))
+                    if issubclass(model, NodeModel)
+                    else getattr(model._settings, "type")
+                )
+
+                # Check if we need to create any constraints
+                if not self._skip_constraints:
+                    if getattr(get_field_type(property_definition), "_unique", False):
+                        await self.create_uniqueness_constraint(
+                            name=model.__name__,
+                            entity_type=entity_type,
+                            properties=[property_name],
+                            labels_or_type=labels_or_type,
+                        )
+
+                # Check if we need to create any indexes
+                if not self._skip_indexes:
+                    if getattr(get_field_type(property_definition), "_range_index", False):
+                        await self.create_range_index(
+                            name=model.__name__,
+                            entity_type=entity_type,
+                            properties=[property_name],
+                            labels_or_type=labels_or_type,
+                        )
+                    if getattr(get_field_type(property_definition), "_point_index", False):
+                        await self.create_point_index(
+                            name=model.__name__,
+                            entity_type=entity_type,
+                            properties=[property_name],
+                            labels_or_type=labels_or_type,
+                        )
+                    if getattr(get_field_type(property_definition), "_text_index", False):
+                        await self.create_text_index(
+                            name=model.__name__,
+                            entity_type=entity_type,
+                            properties=[property_name],
+                            labels_or_type=labels_or_type,
+                        )
+
     @property
     def is_connected(self) -> bool:
         """
         Returns whether the client is connected to a database or not.
 
         Returns:
             bool: Whether the client is connected to a database or not.
```

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/core/node.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/core/node.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/core/relationship.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/core/relationship.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/exceptions.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Exceptions module for Pyneo4j OGM.
 """
 
-from typing import Any, List, Set, Union
+from typing import Any, List
 
 
 class Pyneo4jException(Exception):
     """
     Base exception for all Pyneo4j exceptions.
     """
 
@@ -211,18 +211,7 @@
 class ListItemNotEncodable(Pyneo4jException):
     """
     A list item is not JSON encodable and can thus not be stored.
     """
 
     def __init__(self, *args: object) -> None:
         super().__init__("List item is not JSON encodable and can not be stored inside the database", *args)
-
-
-class AlreadyRegistered(Pyneo4jException):
-    """
-    Multiple models are using the same labels/type as a already registered model.
-    """
-
-    def __init__(self, labels_or_type: Union[Set[str], str], *args: object) -> None:
-        received = f"[{', '.join(labels_or_type)}]" if isinstance(labels_or_type, set) else f"[{labels_or_type}]"
-        label_or_type = "labels" if isinstance(labels_or_type, set) else "type"
-        super().__init__(f"A model is using the same {label_or_type} as another model. Got {received}", *args)
```

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/fields/property_options.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/fields/property_options.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/fields/relationship_property.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/fields/relationship_property.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/fields/settings.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/fields/settings.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/logger.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/logger.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/actions/create.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/migrations/actions/create.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/actions/down.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/migrations/actions/down.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/actions/init.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/migrations/actions/init.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/actions/status.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/migrations/actions/status.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/actions/up.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/migrations/actions/up.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/cli.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/migrations/cli.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/utils/client.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/migrations/utils/client.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/utils/defaults.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/migrations/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/utils/migration.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/migrations/utils/migration.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/utils/models.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/migrations/utils/models.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/pydantic_utils.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/queries/operators.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/queries/operators.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/queries/query_builder.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/queries/query_builder.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/queries/types.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/queries/types.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyneo4j_ogm/queries/validators.py` & `pyneo4j_ogm-0.6.0/pyneo4j_ogm/queries/validators.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.3/pyproject.toml` & `pyneo4j_ogm-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyneo4j-ogm"
-version = "0.5.3"
+version = "0.6.0"
 description = "Asynchronous Python OGM for Neo4j"
 authors = ["groc-prog <marc.troisner@gmail.com>"]
 maintainers = ["groc-prog <marc.troisner@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 keywords = ["neo4j", "python", "orm", "ogm", "async", "asynchronous", "database", "graph-database", "pydantic"]
 homepage = "https://github.com/groc-prog/pyneo4j-ogm"
```

### Comparing `pyneo4j_ogm-0.5.3/PKG-INFO` & `pyneo4j_ogm-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneo4j-ogm
-Version: 0.5.3
+Version: 0.6.0
 Summary: Asynchronous Python OGM for Neo4j
 Home-page: https://github.com/groc-prog/pyneo4j-ogm
 License: MIT
 Keywords: neo4j,python,orm,ogm,async,asynchronous,database,graph-database,pydantic
 Author: groc-prog
 Author-email: marc.troisner@gmail.com
 Maintainer: groc-prog
```

