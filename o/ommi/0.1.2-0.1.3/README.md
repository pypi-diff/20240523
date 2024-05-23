# Comparing `tmp/ommi-0.1.2.tar.gz` & `tmp/ommi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ommi-0.1.2.tar", max compression
+gzip compressed data, was "ommi-0.1.3.tar", max compression
```

## Comparing `ommi-0.1.2.tar` & `ommi-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0     1076 2024-05-02 21:27:51.195847 ommi-0.1.2/LICENSE
--rw-r--r--   0        0        0     3723 2024-05-02 21:27:51.195847 ommi-0.1.2/README.md
--rw-r--r--   0        0        0      195 2024-05-02 21:27:51.195847 ommi-0.1.2/ommi/__init__.py
--rw-r--r--   0        0        0      943 2024-05-02 21:27:51.195847 ommi-0.1.2/ommi/contextual_method.py
--rw-r--r--   0        0        0      677 2024-05-02 21:27:51.195847 ommi-0.1.2/ommi/driver_context.py
--rw-r--r--   0        0        0     4676 2024-05-02 21:27:51.195847 ommi-0.1.2/ommi/drivers.py
--rw-r--r--   0        0        0     6148 2024-05-02 21:27:51.195847 ommi-0.1.2/ommi/ext/.DS_Store
--rw-r--r--   0        0        0    13048 2024-05-02 21:27:51.195847 ommi-0.1.2/ommi/ext/drivers/sqlite.py
--rw-r--r--   0        0        0     4596 2024-05-02 21:27:51.195847 ommi-0.1.2/ommi/field_metadata.py
--rw-r--r--   0        0        0      210 2024-05-02 21:27:51.195847 ommi-0.1.2/ommi/model_collections.py
--rw-r--r--   0        0        0     7707 2024-05-02 21:27:51.195847 ommi-0.1.2/ommi/models.py
--rw-r--r--   0        0        0     9718 2024-05-02 21:27:51.195847 ommi-0.1.2/ommi/query_ast.py
--rw-r--r--   0        0        0     1279 2024-05-02 21:27:51.195847 ommi-0.1.2/ommi/statuses.py
--rw-r--r--   0        0        0      767 2024-05-02 21:28:08.888096 ommi-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4535 1970-01-01 00:00:00.000000 ommi-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-23 15:31:01.150359 ommi-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4001 2024-05-23 15:31:01.150359 ommi-0.1.3/README.md
+-rw-r--r--   0        0        0      195 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/__init__.py
+-rw-r--r--   0        0        0      943 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/contextual_method.py
+-rw-r--r--   0        0        0      677 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/driver_context.py
+-rw-r--r--   0        0        0     4676 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/drivers.py
+-rw-r--r--   0        0        0     6148 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/ext/.DS_Store
+-rw-r--r--   0        0        0     8295 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/ext/drivers/mongodb.py
+-rw-r--r--   0        0        0    13214 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/ext/drivers/postgresql.py
+-rw-r--r--   0        0        0    12398 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/ext/drivers/sqlite.py
+-rw-r--r--   0        0        0     4605 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/field_metadata.py
+-rw-r--r--   0        0        0      350 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/model_collections.py
+-rw-r--r--   0        0        0     8755 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/models.py
+-rw-r--r--   0        0        0     9955 2024-05-23 15:31:01.150359 ommi-0.1.3/ommi/query_ast.py
+-rw-r--r--   0        0        0     1279 2024-05-23 15:31:01.154359 ommi-0.1.3/ommi/statuses.py
+-rw-r--r--   0        0        0      170 2024-05-23 15:31:01.154359 ommi-0.1.3/ommi/utils/get_first.py
+-rw-r--r--   0        0        0      837 2024-05-23 15:31:18.422281 ommi-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4813 1970-01-01 00:00:00.000000 ommi-0.1.3/PKG-INFO
```

### Comparing `ommi-0.1.2/LICENSE` & `ommi-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ommi-0.1.2/README.md` & `ommi-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,28 @@
 - [Pydantic](https://docs.pydantic.dev/latest/)
 
 ### Included Database Support
 
 #### SQLite3
 
 - Table creation from models
-- Select, Insert, Update, Delete
+- Select, Insert, Update, Delete, Count
+- No relationships or joins
+
+#### PostgreSQL
+
+- Table creation from models
+- Select, Insert, Update, Delete, Count
+- No relationships or joins
+
+#### MongoDB
+
+- Collection creation from models
+- Fetch, Insert, Update, Delete, Count
+- No relationships or nested documents
 
 ## Usage
 
 ### Defining Models
 
 All models that support Ommi database drivers need to use the `ommi_model` class decorator.
 
@@ -126,8 +139,8 @@
 #### Update
 
 Update takes any number of model instances and syncs their changes to the database.
 
 ```python
 user.name = "Bob"
 await db.update(user).or_raise()
-```
+```
```

### Comparing `ommi-0.1.2/ommi/contextual_method.py` & `ommi-0.1.3/ommi/contextual_method.py`

 * *Files identical despite different names*

### Comparing `ommi-0.1.2/ommi/driver_context.py` & `ommi-0.1.3/ommi/driver_context.py`

 * *Files identical despite different names*

### Comparing `ommi-0.1.2/ommi/drivers.py` & `ommi-0.1.3/ommi/drivers.py`

 * *Files identical despite different names*

### Comparing `ommi-0.1.2/ommi/ext/.DS_Store` & `ommi-0.1.3/ommi/ext/.DS_Store`

 * *Files identical despite different names*

### Comparing `ommi-0.1.2/ommi/ext/drivers/sqlite.py` & `ommi-0.1.3/ommi/ext/drivers/sqlite.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,16 +75,18 @@
 
     @property
     def connected(self) -> bool:
         return self._connected
 
     @database_action
     async def connect(self) -> "SQLiteDriver":
-        self._db = sqlite3.connect(self.config.filename)
-        self._connected = True
+        if not self._connected:
+            self._db = sqlite3.connect(self.config.filename)
+            self._connected = True
+
         return self
 
     @database_action
     async def disconnect(self) -> "SQLiteDriver":
         self._db.close()
         self._connected = False
         return self
@@ -254,47 +256,23 @@
     ) -> dict[str, ResultOrdering]:
         return {
             f"{ref.model.__model_name__}.{ref.field.name}": ref.ordering
             for ref in sorting
         }
 
     def _create_table(self, model: Type[OmmiModel], session: sqlite3.Cursor):
-        pk = self._find_primary_key(model)
+        pk = model.get_primary_key_field().get("store_as")
         columns = ", ".join(
             self._build_column(field, field.get("store_as") == pk)
             for field in model.__ommi_metadata__.fields.values()
         )
         session.execute(
             f"CREATE TABLE IF NOT EXISTS {model.__ommi_metadata__.model_name} ({columns});"
         )
 
-    def _find_primary_key(self, model: Type[OmmiModel]) -> str:
-        if not model.__ommi_metadata__.fields:
-            raise Exception(f"No fields defined on {model}")
-
-        fields = list(model.__ommi_metadata__.fields.values())
-        if name := next(
-            (
-                f.get("store_as")
-                for f in fields
-                if f.get("store_as", f.get("field_name")).lower() == "id"
-            ),
-            None,
-        ):
-            return name
-
-        for field in fields:
-            if (
-                field.get("field_type") is int
-                or field.get("store_as").casefold() == "id"
-            ):
-                return field.get("store_as")
-
-        return next(iter(fields)).get("store_as")
-
     def _insert(self, item: OmmiModel, session: sqlite3.Cursor):
         fields = list(item.__ommi_metadata__.fields.values())
         data = {
             field.get("store_as"): getattr(item, field.get("field_name"))
             for field in fields
         }
         qs = ", ".join(["?"] * len(data))
@@ -307,15 +285,15 @@
 
     def _update_rows(
         self,
         model: Type[OmmiModel],
         items: list[OmmiModel],
         session: sqlite3.Cursor,
     ):
-        pk = self._find_primary_key(model)
+        pk = model.get_primary_key_field().get("store_as")
         fields = list(model.__ommi_metadata__.fields.values())
         for item in items:
             values = (
                 getattr(item, field.get("field_name"))
                 for field in fields
                 if field.get("store_as") != pk
             )
@@ -331,15 +309,15 @@
 
     def _delete_rows(
         self,
         model: Type[OmmiModel],
         items: list[OmmiModel],
         session: sqlite3.Cursor,
     ):
-        pk = self._find_primary_key(model)
+        pk = model.get_primary_key_field().get("store_as")
         keys = [getattr(item, pk) for item in items]
         qs = ", ".join(["?"] * len(items))
         session.execute(
             f"DELETE FROM {model.__ommi_metadata__.model_name} WHERE {pk} IN ({qs});",
             keys,
         )
 
@@ -412,10 +390,10 @@
 
             if query.offset > 0:
                 query_builder.append(f"OFFSET {query.offset}")
 
         return " ".join(query_builder) + ";"
 
     def _sync_with_last_inserted(self, item: OmmiModel, session: sqlite3.Cursor):
-        pk = self._find_primary_key(type(item))
+        pk = item.get_primary_key_field().get("store_as")
         result = session.execute("SELECT last_insert_rowid();").fetchone()
         setattr(item, pk, result[0])
```

### Comparing `ommi-0.1.2/ommi/field_metadata.py` & `ommi-0.1.3/ommi/field_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,16 @@
             raise NotImplementedError
 
         self._add_field(other)
         return self
 
     def _add_field(self, field: "FieldMetadata") -> None:
         """Adds field metadata to the aggregate metadata. This is done in a non-destructive way so as to prevent changes
-        made to the aggregate metadata mapping from propagating to the the aggregated field metadata instances."""
+        made to the aggregate metadata mapping from propagating to the the aggregated field metadata instances.
+        """
         self._fields.append(field)
         self.metadata.maps.append(field.metadata)
 
     def matches(self, metadata: "FieldMetadata | Type[FieldMetadata]") -> bool:
         return any(f.matches(metadata) for f in self._fields)
```

### Comparing `ommi-0.1.2/ommi/models.py` & `ommi-0.1.3/ommi/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,46 @@
 from dataclasses import dataclass, field as dc_field
 from inspect import get_annotations
-from typing import Callable, overload, Type, TypeVar, Any, Generator, get_origin, Annotated, get_args, Awaitable
+from pyexpat import model
+from typing import (
+    Callable,
+    overload,
+    Type,
+    TypeVar,
+    Any,
+    Generator,
+    get_origin,
+    Annotated,
+    get_args,
+    Awaitable,
+)
 from tramp.results import Result
 
 import ommi.drivers as drivers
 import ommi.query_ast as query_ast
-from ommi.field_metadata import FieldMetadata, AggregateMetadata, FieldType, StoreAs, create_metadata_type
+from ommi.field_metadata import (
+    FieldMetadata,
+    AggregateMetadata,
+    FieldType,
+    StoreAs,
+    create_metadata_type, Key,
+)
+from ommi.utils.get_first import first
 from ommi.statuses import DatabaseStatus
 from ommi.contextual_method import contextual_method
 from ommi.driver_context import active_driver
 import ommi.model_collections
 
-
 T = TypeVar("T", bound=Type)
 
 DRIVER_DUNDER_NAME = "__ommi_driver__"
 MODEL_NAME_DUNDER_NAME = "__ommi_model_name__"
 MODEL_NAME_CLASS_PARAM = "name"
 METADATA_DUNDER_NAME = "__ommi_metadata__"
 
-
 _global_collection = None
 
 
 def get_global_collection() -> "ommi.model_collections.ModelCollection":
     global _global_collection
     if not _global_collection:
         _global_collection = ommi.model_collections.ModelCollection()
@@ -80,18 +97,22 @@
     @contextual_method
     def get_driver(
         self, driver: "drivers.DatabaseDrivers | None" = None
     ) -> "drivers.DatabaseDriver | None":
         return driver or type(self).get_driver()
 
     @get_driver.classmethod
-    def get_driver(cls, driver: "drivers.DatabaseDrivers | None" = None) -> "drivers.DatabaseDriver | None":
+    def get_driver(
+        cls, driver: "drivers.DatabaseDrivers | None" = None
+    ) -> "drivers.DatabaseDriver | None":
         return driver or active_driver.get(None)
 
-    def add(self) -> "drivers.DatabaseAction[DatabaseStatus[OmmiModel]] | Awaitable[DatabaseStatus[OmmiModel]]":
+    def add(
+        self,
+    ) -> "drivers.DatabaseAction[DatabaseStatus[OmmiModel]] | Awaitable[DatabaseStatus[OmmiModel]]":
         return self.get_driver().add(self)
 
     @contextual_method
     def delete(
         self, driver: "drivers.DatabaseDriver | None" = None
     ) -> "drivers.DatabaseAction[DatabaseStatus[drivers.DatabaseDriver]] | Awaitable[DatabaseStatus[drivers.DatabaseDriver]]":
         return self.get_driver(driver).delete(self)
@@ -116,22 +137,44 @@
     @classmethod
     def fetch(
         cls,
         *predicates: "ASTGroupNode | DatabaseModel | bool",
         driver: "drivers.DatabaseDriver | None" = None,
         **columns: Any,
     ) -> "drivers.DatabaseAction[DatabaseStatus[list[OmmiModel]]] | Awaitable[DatabaseStatus[list[OmmiModel]]]":
-        return cls.get_driver(driver).fetch(cls, *predicates, *cls._build_column_predicates(columns))
+        return cls.get_driver(driver).fetch(
+            cls, *predicates, *cls._build_column_predicates(columns)
+        )
 
     def sync(
         self, driver: "drivers.DatabaseDriver | None" = None
     ) -> "drivers.DatabaseAction[DatabaseStatus[drivers.DatabaseDriver]] | Awaitable[DatabaseStatus[drivers.DatabaseDriver]]":
         return self.get_driver(driver).update(self)
 
     @classmethod
+    def get_primary_key_field(cls) -> OmmiField:
+        fields = cls.__ommi_metadata__.fields
+        if not fields:
+            raise Exception(f"No fields defined on {cls}")
+
+        def find_field_where(predicate):
+            return first(f for f in fields.values() if predicate(f))
+
+        if field := find_field_where(lambda f: f.matches(Key)):
+            return field
+
+        if field := find_field_where(lambda f: f.get("store_as") in {"id", "_id"}):
+            return field
+
+        if field := find_field_where(lambda f: issubclass(f.get("field_type"), int)):
+            return field
+
+        return first(fields.values())
+
+    @classmethod
     def _build_column_predicates(
         cls, columns: dict[str, Any]
     ) -> "Generator[query_ast.ASTComparisonNode | bool, None, None]":
         if not columns:
             return
 
         for name, value in columns.items():
@@ -139,49 +182,56 @@
                 raise ValueError(f"Invalid column {name!r} for model {cls.__name__}")
 
             yield getattr(cls, name) == value
 
 
 @overload
 def ommi_model(
-    cls: None = None, *, collection: "ommi.model_collections.ModelCollection | None" = None
-) -> Callable[[T], T | Type[OmmiModel]]:
-    ...
+    cls: None = None,
+    *,
+    collection: "ommi.model_collections.ModelCollection | None" = None,
+) -> Callable[[T], T | Type[OmmiModel]]: ...
 
 
 @overload
-def ommi_model(cls: T) -> T | Type[OmmiModel]:
-    ...
+def ommi_model(cls: T) -> T | Type[OmmiModel]: ...
 
 
 def ommi_model(
     cls: T | None = None, /, **kwargs
 ) -> T | Type[OmmiModel] | Callable[[T], T | Type[OmmiModel]]:
     def wrap_model(c: T) -> T | Type[OmmiModel]:
         model = _create_model(c, **kwargs)
-        _register_model(model, Result.Value(kwargs["collection"]) if "collection" in kwargs else Result.Nothing)
+        _register_model(
+            model,
+            (
+                Result.Value(kwargs["collection"])
+                if "collection" in kwargs
+                else Result.Nothing
+            ),
+        )
         return model
 
     return wrap_model if cls is None else wrap_model(cls)
 
 
 def _create_model(c: T, **kwargs) -> T | Type[OmmiModel]:
     metadata_factory = (
-        c.__ommi_metadata__.clone
-        if hasattr(c, METADATA_DUNDER_NAME)
-        else OmmiMetadata
+        c.__ommi_metadata__.clone if hasattr(c, METADATA_DUNDER_NAME) else OmmiMetadata
     )
 
     fields = _get_fields(get_annotations(c))
     return type.__new__(
         type(c),
         f"OmmiModel_{c.__name__}",
         (c, OmmiModel),
         {
-            name: QueryableFieldDescriptor(fields[name].get("store_as"), getattr(c, name, None))
+            name: QueryableFieldDescriptor(
+                fields[name].get("store_as"), getattr(c, name, None)
+            )
             for name in get_annotations(c)
             if not name.startswith("_")
         }
         | {
             METADATA_DUNDER_NAME: metadata_factory(
                 model_name=_get_value(
                     kwargs,
@@ -192,23 +242,29 @@
                 ),
                 fields=fields,
             )
         },
     )
 
 
-def _register_model(model: Type[OmmiModel], collection: "Result[ommi.model_collections.ModelCollection]"):
+def _register_model(
+    model: Type[OmmiModel], collection: "Result[ommi.model_collections.ModelCollection]"
+):
     get_collection(collection, model).add(model)
 
 
 def get_collection(
-        collection: "Result[ommi.model_collections.ModelCollection]",
-        model: Type[OmmiModel] | None = None,
+    collection: "Result[ommi.model_collections.ModelCollection]",
+    model: Type[OmmiModel] | None = None,
 ) -> "ommi.model_collections.ModelCollection":
-    return collection.value_or(getattr(model, METADATA_DUNDER_NAME).collection if model else get_global_collection())
+    return collection.value_or(
+        getattr(model, METADATA_DUNDER_NAME).collection
+        if model
+        else get_global_collection()
+    )
 
 
 def _get_fields(fields: dict[str, Any]) -> dict[str, FieldMetadata]:
     ommi_fields = {}
     for name, hint in fields.items():
         ommi_fields[name] = AggregateMetadata()
         if get_origin(hint) == Annotated:
@@ -219,19 +275,23 @@
                     case FieldMetadata():
                         ommi_fields[name] |= annotation
 
                     case _:
                         _annotations.append(annotation)
 
             if _annotations:
-                field_type = Annotated.__class_getitem__(field_type, *_annotations)  # Hack to support 3.10
+                field_type = Annotated.__class_getitem__(
+                    field_type, *_annotations
+                )  # Hack to support 3.10
 
         else:
             field_type = hint
 
         ommi_fields[name] |= FieldType(field_type)
         if not ommi_fields[name].matches(StoreAs):
             ommi_fields[name] |= StoreAs(name)
 
-        ommi_fields[name] |= create_metadata_type("FieldMetadata", field_name=name, field_type=field_type)()
+        ommi_fields[name] |= create_metadata_type(
+            "FieldMetadata", field_name=name, field_type=field_type
+        )()
 
     return ommi_fields
```

### Comparing `ommi-0.1.2/ommi/query_ast.py` & `ommi-0.1.3/ommi/query_ast.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,21 @@
 
     def limit(self, limit: int, page: int = 0) -> Self:
         self.max_results = limit
         self.results_page = page
         return self
 
     def sort(self, *on_fields: "ASTReferenceNode") -> Self:
-        self.sorting.extend(field for field in on_fields if field not in self.sorting)
+        # Gotta jump through some hoops to compare ASTReferenceNodes and maintain ordering
+        unique = set(on_fields) | set(self.sorting)
+        for field in on_fields:
+            if field in unique:
+                self.sorting.append(field)
+                unique.remove(field)
+
         return self
 
     def __eq__(self, other):
         if not isinstance(other, ASTGroupNode):
             return NotImplemented
 
         return self._compare_items(other)
@@ -222,15 +228,15 @@
     def __init__(self, field, model, ordering=ResultOrdering.ASCENDING):
         super().__init__(ASTGroupNode())
         self._field = field
         self._model = model
         self._ordering = ordering
 
     def _eq(self, other):
-        return self.field == other.field and self.model == other.model
+        return self.field == other.field and self.model == other.model and self.ordering == other.ordering
 
     def __iter__(self):
         yield from (self._field, self._model)
 
     @property
     def field(self):
         return self._field
```

### Comparing `ommi-0.1.2/ommi/statuses.py` & `ommi-0.1.3/ommi/statuses.py`

 * *Files identical despite different names*

### Comparing `ommi-0.1.2/pyproject.toml` & `ommi-0.1.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ommi"
-version = "0.1.2"
+version = "0.1.3"
 description = "A portable object model mapper that can work with any database and model library (dataclasses, Attrs, Pydantic, etc.). It is designed for the general case to support the largest possible number of databases."
 authors = ["Zech Zimmerman <hi@zech.codes>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ZechCodes/Ommi"
 keywords = ["database", "orm", "object model mapper", "dataclasses", "attrs", "pydantic", "sqlite"]
 
@@ -13,11 +13,13 @@
 tramp = "^0.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pydantic = "^2.5.3"
 attrs = "^23.2.0"
 pytest = "^7.4.4"
 pytest-asyncio = "^0.23.4"
+motor = "^3.4.0"
+psycopg = {extras = ["binary"], version = "^3.1.19"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ommi-0.1.2/PKG-INFO` & `ommi-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ommi
-Version: 0.1.2
+Version: 0.1.3
 Summary: A portable object model mapper that can work with any database and model library (dataclasses, Attrs, Pydantic, etc.). It is designed for the general case to support the largest possible number of databases.
 Home-page: https://github.com/ZechCodes/Ommi
 License: MIT
 Keywords: database,orm,object model mapper,dataclasses,attrs,pydantic,sqlite
 Author: Zech Zimmerman
 Author-email: hi@zech.codes
 Requires-Python: >=3.10,<4.0
@@ -39,15 +39,28 @@
 - [Pydantic](https://docs.pydantic.dev/latest/)
 
 ### Included Database Support
 
 #### SQLite3
 
 - Table creation from models
-- Select, Insert, Update, Delete
+- Select, Insert, Update, Delete, Count
+- No relationships or joins
+
+#### PostgreSQL
+
+- Table creation from models
+- Select, Insert, Update, Delete, Count
+- No relationships or joins
+
+#### MongoDB
+
+- Collection creation from models
+- Fetch, Insert, Update, Delete, Count
+- No relationships or nested documents
 
 ## Usage
 
 ### Defining Models
 
 All models that support Ommi database drivers need to use the `ommi_model` class decorator.
 
@@ -145,7 +158,8 @@
 
 Update takes any number of model instances and syncs their changes to the database.
 
 ```python
 user.name = "Bob"
 await db.update(user).or_raise()
 ```
+
```

