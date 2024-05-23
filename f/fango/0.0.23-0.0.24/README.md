# Comparing `tmp/fango-0.0.23.tar.gz` & `tmp/fango-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fango-0.0.23.tar", max compression
+gzip compressed data, was "fango-0.0.24.tar", max compression
```

## Comparing `fango-0.0.23.tar` & `fango-0.0.24.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      645 2024-04-28 12:17:49.759751 fango-0.0.23/README.md
--rw-r--r--   0        0        0     7506 2024-04-28 16:45:48.360417 fango-0.0.23/fango/adapters/pydantic.py
--rw-r--r--   0        0        0      848 2024-04-28 16:45:48.360676 fango-0.0.23/fango/adapters/types.py
--rw-r--r--   0        0        0     2681 2024-04-28 16:45:48.361040 fango-0.0.23/fango/auth.py
--rw-r--r--   0        0        0     4845 2024-04-28 16:45:48.361360 fango-0.0.23/fango/filters.py
--rw-r--r--   0        0        0      310 2024-04-28 16:45:48.361630 fango-0.0.23/fango/generics.py
--rw-r--r--   0        0        0     1907 2024-04-28 16:45:48.361901 fango-0.0.23/fango/log.py
--rw-r--r--   0        0        0        0 2024-04-28 16:45:48.362194 fango-0.0.23/fango/middleware/__init__.py
--rw-r--r--   0        0        0      586 2024-04-28 16:45:48.363645 fango-0.0.23/fango/middleware/common.py
--rw-r--r--   0        0        0     6639 2024-04-28 16:45:48.364090 fango-0.0.23/fango/pagination.py
--rw-r--r--   0        0        0     2403 2024-04-28 16:45:48.364376 fango-0.0.23/fango/permissions.py
--rw-r--r--   0        0        0      440 2024-04-28 16:45:48.364632 fango-0.0.23/fango/routing.py
--rw-r--r--   0        0        0     2879 2024-04-28 16:45:48.364871 fango-0.0.23/fango/schemas.py
--rw-r--r--   0        0        0      284 2024-04-28 16:45:48.368897 fango-0.0.23/fango/tests/client.py
--rw-r--r--   0        0        0      723 2024-04-28 16:45:48.369141 fango-0.0.23/fango/tests/fixtures.py
--rw-r--r--   0        0        0     3062 2024-04-28 16:45:48.369484 fango-0.0.23/fango/utils.py
--rw-r--r--   0        0        0     7259 2024-04-28 16:45:48.369760 fango-0.0.23/fango/viewsets.py
--rw-r--r--   0        0        0      536 2024-04-28 16:45:52.482910 fango-0.0.23/pyproject.toml
--rw-r--r--   0        0        0     1491 1970-01-01 00:00:00.000000 fango-0.0.23/PKG-INFO
+-rw-r--r--   0        0        0      645 2024-04-28 12:17:49.759751 fango-0.0.24/README.md
+-rw-r--r--   0        0        0     7655 2024-05-23 20:00:26.982873 fango-0.0.24/fango/adapters/pydantic.py
+-rw-r--r--   0        0        0      848 2024-05-23 20:00:26.983305 fango-0.0.24/fango/adapters/types.py
+-rw-r--r--   0        0        0     2681 2024-05-23 20:00:26.983720 fango-0.0.24/fango/auth.py
+-rw-r--r--   0        0        0     4845 2024-05-23 20:00:26.984372 fango-0.0.24/fango/filters.py
+-rw-r--r--   0        0        0      310 2024-05-23 20:00:26.984956 fango-0.0.24/fango/generics.py
+-rw-r--r--   0        0        0     1907 2024-05-23 20:00:26.985337 fango-0.0.24/fango/log.py
+-rw-r--r--   0        0        0        0 2024-05-23 20:00:26.985673 fango-0.0.24/fango/middleware/__init__.py
+-rw-r--r--   0        0        0      586 2024-05-23 20:00:26.987257 fango-0.0.24/fango/middleware/common.py
+-rw-r--r--   0        0        0     6639 2024-05-23 20:00:26.987606 fango-0.0.24/fango/pagination.py
+-rw-r--r--   0        0        0     2403 2024-05-23 20:00:26.988002 fango-0.0.24/fango/permissions.py
+-rw-r--r--   0        0        0      440 2024-05-23 20:00:26.988297 fango-0.0.24/fango/routing.py
+-rw-r--r--   0        0        0     3374 2024-05-23 20:00:26.988676 fango-0.0.24/fango/schemas.py
+-rw-r--r--   0        0        0      284 2024-05-23 20:00:26.992901 fango-0.0.24/fango/tests/client.py
+-rw-r--r--   0        0        0      723 2024-05-23 20:00:26.993335 fango-0.0.24/fango/tests/fixtures.py
+-rw-r--r--   0        0        0     3062 2024-05-23 20:00:26.993649 fango-0.0.24/fango/utils.py
+-rw-r--r--   0        0        0     7259 2024-05-23 20:00:26.994691 fango-0.0.24/fango/viewsets.py
+-rw-r--r--   0        0        0      536 2024-05-23 20:01:59.099553 fango-0.0.24/pyproject.toml
+-rw-r--r--   0        0        0     1491 1970-01-01 00:00:00.000000 fango-0.0.24/PKG-INFO
```

### Comparing `fango-0.0.23/README.md` & `fango-0.0.24/README.md`

 * *Files identical despite different names*

### Comparing `fango-0.0.23/fango/adapters/pydantic.py` & `fango-0.0.24/fango/adapters/pydantic.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     OneToOneRel,
 )
 from fastapi import HTTPException
 from pydantic import BaseModel
 
 from fango.adapters.types import PK
 from fango.log import log_params
-from fango.schemas import CRUDAdapter, UnlinkAdapter
+from fango.schemas import CRUDAdapter, LinkAdapter
 
 __all__ = ["PydanticAdapter"]
 
 ForwardRel = ForeignKey | OneToOneField | OneToOneRel
 MultipleRel = ManyToOneRel | ManyToManyField
 
 
@@ -40,18 +40,16 @@
     def save_from_schema(cls, schema_instance: BaseModel, pk: PK | None = None) -> Model:
         """
         Creates or updates a Django model instance from a Pydantic schema.
 
         """
         try:
             return _save_orm_instance(cls, schema_instance, pk=pk)
-        except ObjectDoesNotExist as e:
-            raise HTTPException(status_code=400, detail=str(e))
-        except ValidationError as e:
-            raise HTTPException(status_code=400, detail=e.message)
+        except (ObjectDoesNotExist, ValidationError) as exc:
+            raise HTTPException(status_code=400, detail=getattr(exc, "message", str(exc)))
 
     class Meta:
         abstract = True
 
 
 @log_params("PoetryAdapter")
 def _save_orm_instance(
@@ -166,16 +164,16 @@
                 relation_set.clear()
             except AttributeError:
                 relation_set.all().delete()
 
     elif isinstance(value, CRUDAdapter):
         _handle_crud_adapter(instance, field, key, value)
 
-    elif isinstance(value, UnlinkAdapter):
-        _handle_unlink_adapter(instance, key, value)
+    elif isinstance(value, LinkAdapter):
+        _handle_link_adapter(instance, field, key, value)
 
     elif isinstance(value, list):
         data = []
         for item in value:
             data.append(_get_or_create_relation(instance, field, key, item))
 
         try:
@@ -196,24 +194,21 @@
 
     """
     if value is None:
         return None
 
     elif isinstance(value, BaseModel):
         if isinstance(field, ForwardRel):
-            rel = getattr(value, "id", None)
-
             if rel := getattr(instance, key, None):
                 rel_pk = rel.pk
             else:
                 rel_pk = None
 
         elif isinstance(field, MultipleRel):
             rel_pk = getattr(value, "id", None)
-
         else:
             raise AdapterError
 
         return _save_orm_instance(
             model=field.related_model,
             schema_instance=value,
             remote_field=field.remote_field,
@@ -223,50 +218,61 @@
 
     elif isinstance(value, PK) or key.endswith("_id"):
         return field.related_model.objects.get(pk=value)
 
     elif isinstance(value, Model):
         value.clean()
         value.save()
-        getattr(instance, field.name).add(value)
+
+        try:
+            getattr(instance, field.name).add(value)
+        except AttributeError:
+            setattr(instance, field.name, value)
+
         return value
 
     else:
         raise AdapterError
 
 
 @log_params("PoetryAdapter")
 def _handle_crud_adapter(instance: Model, field: MultipleRel, key: str, value: Any) -> None:
     """
     Manages CRUD adapter.
 
     """
-    relation_set = getattr(instance, key, None)
+    relation_set = getattr(instance, key)
 
     for item in value.create:
         if item.id:
             raise ValidationError(f"Attribute {key}.create data has id.")
 
         _get_or_create_relation(instance, field, key, item)
 
     for item in value.update:
         if not item.id:
             raise ValidationError(f"Attribute {key}.update data has no id.")
 
         _get_or_create_relation(instance, field, key, item)
 
-    for item in value.delete:
-        relation = relation_set.get(pk=item)
+    for pk in value.delete:
+        relation = relation_set.get(pk=pk)
         relation.delete()
 
 
 @log_params("PoetryAdapter")
-def _handle_unlink_adapter(instance: Model, key: str, value: Any) -> None:
+def _handle_link_adapter(instance: Model, field: ForwardRel | MultipleRel, key: str, value: Any) -> None:
     """
-    Manages Unlink adapter.
+    Manages Link adapter.
 
     """
-    relation_set = getattr(instance, key, None)
+    relation_set = getattr(instance, key)
 
-    for pk in value.unlink:
+    for pk in value.add:
+        relation_set.add(pk)
+
+    for pk in value.remove:
         relation = relation_set.get(pk=pk)
-        setattr(relation, relation_set.field.name, None)
+        try:
+            relation_set.remove(pk)
+        except AttributeError:
+            setattr(relation, relation_set.field.name, None)
```

### Comparing `fango-0.0.23/fango/adapters/types.py` & `fango-0.0.24/fango/adapters/types.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.23/fango/auth.py` & `fango-0.0.24/fango/auth.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.23/fango/filters.py` & `fango-0.0.24/fango/filters.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.23/fango/log.py` & `fango-0.0.24/fango/log.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.23/fango/middleware/common.py` & `fango-0.0.24/fango/middleware/common.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.23/fango/pagination.py` & `fango-0.0.24/fango/pagination.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.23/fango/permissions.py` & `fango-0.0.24/fango/permissions.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.23/fango/schemas.py` & `fango-0.0.24/fango/schemas.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from dataclasses import dataclass
+from enum import Enum
+from types import UnionType
 from typing import Generic, TypedDict, TypeVar, get_args
 
 from django.db.models import IntegerChoices, Manager
 from pydantic import BaseModel, ConfigDict, field_validator, model_validator
 from typing_extensions import NotRequired
 
 from fango.adapters.types import PK
@@ -12,15 +14,15 @@
     "Page",
     "Entry",
     "ChoicesItem",
     "FangoModel",
     "ActionClasses",
     "Multiselect",
     "CRUDAdapter",
-    "UnlinkAdapter",
+    "LinkAdapter",
     "DBModel",
 ]
 
 T = TypeVar("T")
 
 
 @dataclass
@@ -38,16 +40,17 @@
 
 class CRUDAdapter(BaseModel, Generic[T]):
     create: list[T] = []
     update: list[T] = []
     delete: list[PK]
 
 
-class UnlinkAdapter(BaseModel, Generic[T]):
-    unlink: list[PK]
+class LinkAdapter(BaseModel, Generic[T]):
+    add: list[PK]
+    remove: list[PK]
 
 
 class Entry(BaseModel, Generic[T]):
     title: str | None = None
     status: str | None = None
     results: T
 
@@ -57,40 +60,46 @@
     name: str | None
 
 
 class FangoModel(BaseModel):
     model_config = ConfigDict(from_attributes=True)
 
     @field_validator("*", mode="before")
-    def model_manager(cls, value):
+    def model_manager(cls, value, info):
         if isinstance(value, Manager):
-            return value.all()
+            if PK in get_args(cls.model_fields[info.field_name].annotation):
+                return value.values_list("pk", flat=True)
+            else:
+                return value.all()
         return value
 
     @model_validator(mode="before")
     @classmethod
     def choices_label(cls, data):
         from fango.utils import get_choices_label
 
         for key, field in cls.model_fields.items():
             value = data.get(key, field.default) if isinstance(data, dict) else getattr(data, key, field.default)
-            for enum in get_args(field.annotation):
-
-                if issubclass(enum, IntegerChoices):
-                    label = get_choices_label(enum, value)
-                    data.update({key: label}) if isinstance(data, dict) else setattr(data, key, label)
-
-                elif metadata := getattr(enum, "__pydantic_generic_metadata__", None):
-                    if metadata["origin"] is ChoicesItem:
-                        label = get_choices_label(metadata["args"][0], value)
-                        (
-                            data.update({key: {"id": value, "name": label}})
-                            if isinstance(data, dict)
-                            else setattr(data, key, {"id": value, "name": label})
-                        )
+            for arg in get_args(field.annotation):
+                if not isinstance(arg, UnionType):
+                    if issubclass(arg, IntegerChoices):
+                        label = get_choices_label(arg, value)
+                        data.update({key: label}) if isinstance(data, dict) else setattr(data, key, label)
+
+                    elif issubclass(arg, Enum):
+                        data.update({key: label}) if isinstance(data, dict) else setattr(data, key, label)
+
+                    elif metadata := getattr(arg, "__pydantic_generic_metadata__", None):
+                        if metadata["origin"] is ChoicesItem and value is not None:
+                            label = get_choices_label(metadata["args"][0], value)
+                            (
+                                data.update({key: {"id": value, "name": label}})
+                                if isinstance(data, dict)
+                                else setattr(data, key, {"id": value, "name": label})
+                            )
 
         return data
 
 
 class Multiselect(FangoModel):
     id: int
     name: str | None = None
```

### Comparing `fango-0.0.23/fango/tests/fixtures.py` & `fango-0.0.24/fango/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.23/fango/utils.py` & `fango-0.0.24/fango/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             argdefs=method.__defaults__,
             closure=method.__closure__,
         ),
         method.__self__,
     )
 
 
-def get_choices_label(enum: type[Choices], value: int) -> str:
+def get_choices_label(enum: type[Choices], value: int) -> str | None:
     """
     Function returns choices text.
 
     """
 
-    choices_dict = {k:v for k,v in enum.choices}
-    return choices_dict[value]
+    choices_dict = dict(enum.choices)
+    return choices_dict.get(value)
```

### Comparing `fango-0.0.23/fango/viewsets.py` & `fango-0.0.24/fango/viewsets.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.23/pyproject.toml` & `fango-0.0.24/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fango"
-version = "0.0.23"
+version = "0.0.24"
 description = "Metaframework for web with combined FastAPI and Django"
 repository = "https://github.com/egorgam/fango"
 keywords = ["fastapi", "django", "fango"]
 authors = ["Egor Gamazin <egorgamazin@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `fango-0.0.23/PKG-INFO` & `fango-0.0.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fango
-Version: 0.0.23
+Version: 0.0.24
 Summary: Metaframework for web with combined FastAPI and Django
 Home-page: https://github.com/egorgam/fango
 License: MIT
 Keywords: fastapi,django,fango
 Author: Egor Gamazin
 Author-email: egorgamazin@yandex.ru
 Requires-Python: >=3.10,<4.0
```

