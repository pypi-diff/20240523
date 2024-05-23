# Comparing `tmp/nested_dataclass_serialization-0.1.4.tar.gz` & `tmp/nested_dataclass_serialization-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nested_dataclass_serialization-0.1.4.tar", max compression
+gzip compressed data, was "nested_dataclass_serialization-0.1.5.tar", max compression
```

## Comparing `nested_dataclass_serialization-0.1.4.tar` & `nested_dataclass_serialization-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2024-03-19 15:39:27.952336 nested_dataclass_serialization-0.1.4/LICENSE
--rw-r--r--   0        0        0     2123 2024-03-19 15:39:27.952336 nested_dataclass_serialization-0.1.4/README.md
--rw-r--r--   0        0        0       73 2024-03-19 15:39:27.952336 nested_dataclass_serialization-0.1.4/nested_dataclass_serialization/__init__.py
--rw-r--r--   0        0        0     1369 2024-03-19 15:39:27.952336 nested_dataclass_serialization-0.1.4/nested_dataclass_serialization/dataclass_hashing.py
--rw-r--r--   0        0        0     1207 2024-03-19 15:39:27.952336 nested_dataclass_serialization-0.1.4/nested_dataclass_serialization/dataclass_json_decoding.py
--rw-r--r--   0        0        0     7833 2024-03-19 15:39:27.952336 nested_dataclass_serialization-0.1.4/nested_dataclass_serialization/dataclass_json_encoding.py
--rw-r--r--   0        0        0     3235 2024-03-19 15:39:27.952336 nested_dataclass_serialization-0.1.4/nested_dataclass_serialization/dataclass_serialization.py
--rw-r--r--   0        0        0      977 2024-03-19 15:39:27.952336 nested_dataclass_serialization-0.1.4/nested_dataclass_serialization/dataclass_serialization_omegaconf.py
--rw-r--r--   0        0        0     2606 2024-03-19 15:39:27.952336 nested_dataclass_serialization-0.1.4/nested_dataclass_serialization/dataclass_serialization_utils.py
--rw-r--r--   0        0        0      833 2024-03-19 15:39:27.952336 nested_dataclass_serialization-0.1.4/nested_dataclass_serialization/strange_hack.py
--rw-r--r--   0        0        0      769 2024-03-19 15:39:38.400341 nested_dataclass_serialization-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2721 1970-01-01 00:00:00.000000 nested_dataclass_serialization-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-23 07:35:35.141879 nested_dataclass_serialization-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2123 2024-05-23 07:35:35.141879 nested_dataclass_serialization-0.1.5/README.md
+-rw-r--r--   0        0        0       73 2024-05-23 07:35:35.141879 nested_dataclass_serialization-0.1.5/nested_dataclass_serialization/__init__.py
+-rw-r--r--   0        0        0     1369 2024-05-23 07:35:35.141879 nested_dataclass_serialization-0.1.5/nested_dataclass_serialization/dataclass_hashing.py
+-rw-r--r--   0        0        0     1207 2024-05-23 07:35:35.141879 nested_dataclass_serialization-0.1.5/nested_dataclass_serialization/dataclass_json_decoding.py
+-rw-r--r--   0        0        0     8211 2024-05-23 07:35:35.141879 nested_dataclass_serialization-0.1.5/nested_dataclass_serialization/dataclass_json_encoding.py
+-rw-r--r--   0        0        0     3264 2024-05-23 07:35:35.141879 nested_dataclass_serialization-0.1.5/nested_dataclass_serialization/dataclass_serialization.py
+-rw-r--r--   0        0        0      977 2024-05-23 07:35:35.141879 nested_dataclass_serialization-0.1.5/nested_dataclass_serialization/dataclass_serialization_omegaconf.py
+-rw-r--r--   0        0        0     2926 2024-05-23 07:35:35.141879 nested_dataclass_serialization-0.1.5/nested_dataclass_serialization/dataclass_serialization_utils.py
+-rw-r--r--   0        0        0      833 2024-05-23 07:35:35.141879 nested_dataclass_serialization-0.1.5/nested_dataclass_serialization/strange_hack.py
+-rw-r--r--   0        0        0      769 2024-05-23 07:35:46.149830 nested_dataclass_serialization-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2721 1970-01-01 00:00:00.000000 nested_dataclass_serialization-0.1.5/PKG-INFO
```

### Comparing `nested_dataclass_serialization-0.1.4/LICENSE` & `nested_dataclass_serialization-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nested_dataclass_serialization-0.1.4/README.md` & `nested_dataclass_serialization-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nested_dataclass_serialization-0.1.4/nested_dataclass_serialization/dataclass_hashing.py` & `nested_dataclass_serialization-0.1.5/nested_dataclass_serialization/dataclass_hashing.py`

 * *Files identical despite different names*

### Comparing `nested_dataclass_serialization-0.1.4/nested_dataclass_serialization/dataclass_json_decoding.py` & `nested_dataclass_serialization-0.1.5/nested_dataclass_serialization/dataclass_json_decoding.py`

 * *Files identical despite different names*

### Comparing `nested_dataclass_serialization-0.1.4/nested_dataclass_serialization/dataclass_json_encoding.py` & `nested_dataclass_serialization-0.1.5/nested_dataclass_serialization/dataclass_json_encoding.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,23 @@
 import logging
 import re
 import uuid
 from collections.abc import Callable
 from hashlib import sha1
 from typing import Any
 
+from beartype.door import is_bearable
+
 from nested_dataclass_serialization.dataclass_serialization_utils import (
     CLASS_REF_KEY,
     IDKEY,
     NODE_ID_KEY,
     NODES_KEY,
     Dataclass,
+    JsonLoadsOutput,
     OmegaConfDict,
     OmegaConfList,
     PythonBuiltinData,
 )
 from nested_dataclass_serialization.strange_hack import (
     fix_module_if_class_in_same_file_as_main,
 )
@@ -66,35 +69,37 @@
                 self._object2node_id[obj_id] = node_id
                 self._id2node_[node_id] = dct
             node_dct = {NODE_ID_KEY: node_id}
         else:
             node_dct = dct
         return node_dct
 
-    def default(self, o: Any) -> PythonBuiltinData:
+    def default(self, o: Any) -> JsonLoadsOutput:
         """
         this overwrites json.JSONEncoders default method
         """
         if self.sparse:
             # msg = "if you want it, fix it!"
             # raise NotImplementedError(msg)
             self._object2node_id = {}
             self._id2node_ = {}
         dct = self._obj2dict(
             o,
             dict_factory=self._flat_dag_dict if self.sparse else dict,
         )
         if self.sparse:
+            assert isinstance(dct, dict)
             dct[NODES_KEY] = self._id2node_
-        return dct
+        return dct  # pyright: ignore[reportReturnType]
 
     def _obj2dict(  # noqa: C901, PLR0912, WPS231
         self,
         obj: Any,
         dict_factory: DictFactory,
+        name: str | None = None,
     ) -> PythonBuiltinData:
         if dataclasses.is_dataclass(obj):
             out = self._encode_dataclass(obj, dict_factory)
         elif isinstance(obj, tuple) and hasattr(obj, "_fields"):
             # TODO: this could return any class that implements _fields method! WTF! not what I want!
             raise CannotEncodeError
             # out = type(obj)(*(self._obj2dict(v, dict_factory) for v in obj))
@@ -126,14 +131,16 @@
             #     obj= f"{UNSERIALIZABLE}{id(obj)=}{UNSERIALIZABLE}"
             obj = (
                 obj._to_dict(self.skip_keys)  # noqa: SLF001
                 if hasattr(obj, "_to_dict")
                 else obj
             )
             out = obj
+        if not is_bearable(out, PythonBuiltinData):
+            logger.error(f"cannot encode: {name}: {out=}")
         return out
 
     def _encode_dataclass(self, obj: Dataclass, dict_factory: DictFactory) -> dict:
         result: list[tuple[str, Any]] = []
         module = obj.__class__.__module__
         if module == "__main__":
             module = fix_module_if_class_in_same_file_as_main(obj)
@@ -152,15 +159,17 @@
         skip_this_one = self.skip_keys and k in self.skip_keys
         if not skip_this_one:
             r.append((k, v))
 
     def _fields_to_serialize(self, dict_factory: DictFactory, obj: Any) -> KeyValues:
         def exclude_for_hash(o: Dataclass, f_name: str) -> bool:
             if self.encode_for_hash and hasattr(o, "__exclude_from_hash__"):
-                out = f_name in o.__exclude_from_hash__
+                out = (
+                    f_name in o.__exclude_from_hash__
+                )  # pyright: ignore[reportAttributeAccessIssue]
             else:
                 out = False
             return out
 
         feelds = (
             f
             for f in dataclasses.fields(obj)
@@ -168,15 +177,15 @@
             and hasattr(obj, f.name)
             and not f.name.startswith("_")
             and not exclude_for_hash(obj, f.name)
             and not (self.skip_keys and f.name in self.skip_keys)
         )
         name_values = ((f.name, getattr(obj, f.name)) for f in feelds)
         return [
-            (name, self._obj2dict(value, dict_factory))
+            (name, self._obj2dict(value, dict_factory, name=name))
             for name, value in name_values
             if value.__class__.__name__ != "_UNDEFINED"
             or not self.skip_undefined  # TODO(tilo): hardcoded this UNDEFINED here! think about it! and fix it!
         ]
 
     def _values_of_non_special_properties(self, obj: Any) -> KeyValues:
         # Add values of non-special attributes which are properties.
```

### Comparing `nested_dataclass_serialization-0.1.4/nested_dataclass_serialization/dataclass_serialization.py` & `nested_dataclass_serialization-0.1.5/nested_dataclass_serialization/dataclass_serialization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from typing import Any
 
 from nested_dataclass_serialization.dataclass_json_decoding import (
     DataclassDecoderObjectHook,
 )
 from nested_dataclass_serialization.dataclass_json_encoding import DataclassEncoder
 from nested_dataclass_serialization.dataclass_serialization_utils import (
     CLASS_REF_KEY,
@@ -12,15 +13,15 @@
     Dataclass,
     JsonLoadsOutput,
     NeStr,
 )
 
 
 def decode_dataclass(
-    o: dict | (list | tuple),
+    o: dict[str, Any] | (list[Any] | tuple[Any]),
     class_ref_key: str = CLASS_REF_KEY,
     is_sparse: bool = False,
 ) -> Dataclass | JsonLoadsOutput:
     # TODO:  why did I want this Base64-stuff?
     # o = json.dumps(o) # there must be a better way than, json.dumps twice!
     # o = json.loads(o, cls=Base64Decoder)
     return _json_loads_decode_dataclass(
@@ -87,15 +88,15 @@
 def encode_dataclass(  # noqa: PLR0913
     d: Dataclass | JsonLoadsOutput | tuple,
     class_reference_key: str = CLASS_REF_KEY,
     skip_undefined: bool = True,
     skip_keys: list[str] | None = None,
     sparse: bool = False,
     encode_for_hash: bool = False,
-) -> dict | (list | (tuple | set)):
+) -> JsonLoadsOutput:
     """
     # TODO: bad naming! cause it not only handles Dataclasses but also JsonLoadsOutput
     encode in the sense that the dictionary representation can be decoded to the nested dataclasses object again
     """
     DataclassEncoder.class_reference_key = class_reference_key
     DataclassEncoder.skip_undefined = skip_undefined
     DataclassEncoder.skip_keys = skip_keys
```

### Comparing `nested_dataclass_serialization-0.1.4/nested_dataclass_serialization/dataclass_serialization_omegaconf.py` & `nested_dataclass_serialization-0.1.5/nested_dataclass_serialization/dataclass_serialization_omegaconf.py`

 * *Files identical despite different names*

### Comparing `nested_dataclass_serialization-0.1.4/nested_dataclass_serialization/dataclass_serialization_utils.py` & `nested_dataclass_serialization-0.1.5/nested_dataclass_serialization/dataclass_serialization_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 from beartype.vale import Is
 
 # ------------TODO: move the following upstream to some utils repo?-----------------
 NeStr = Annotated[str, Is[lambda s: len(s) > 0]]
 Dataclass = Annotated[object, Is[lambda o: dataclasses.is_dataclass(o)]]
 JsonLoadsOutput = (
-    dict | list | str | int | float | bool | None
+    dict[str, Any] | list[Any] | str | int | float | bool | None
 )  # forgot anything? set  cannot be handled by json
-PythonBuiltinData = JsonLoadsOutput | tuple | set
+PythonBuiltinData = JsonLoadsOutput | tuple[Any, ...] | set[Any]
 
 
 # -------------------------------------------------------------------------------------
 
 IDKEY = "_id_"
 ID_KEY = IDKEY  # TODO: rename
 CLASS_REF_KEY = "_target_"
@@ -34,15 +34,18 @@
     fullpath: str,
 ) -> Any:
     *module_path, class_name = fullpath.split(".")
     module_reference = ".".join(module_path)
     clazz = getattr(importlib.import_module(module_reference), class_name)
     if hasattr(clazz, "create"):
         out = clazz.create(**d)
-    elif hasattr(clazz, dataclasses._FIELDS):  # noqa: SLF001
+    elif hasattr(
+        clazz,
+        dataclasses._FIELDS,  # pyright: ignore[reportAttributeAccessIssue]  # noqa: SLF001
+    ):
         out = shallow_dataclass_from_dict(clazz, d)
     else:
         out = clazz(**d)
     return out
 
 
 T = TypeVar("T")
@@ -50,25 +53,29 @@
 
 def shallow_dataclass_from_dict(clazz: type[T], dct: dict) -> T:
     """
     NO decoding of nested dicts to nested dataclasses here!!
     is used as a "factory" in instantiate_via_importlib
     dict can contain dataclasses or whatever objects!
     """
+    assert dataclasses.is_dataclass(clazz)  # just for type narrowing
     kwargs = {
         f.name: dct[f.name]
         for f in dataclasses.fields(clazz)
         if (f.init and f.name in dct.keys())
     }
     obj = clazz(**kwargs)
     set_noninit_fields(clazz, dct, obj)
     return obj
 
 
 def set_noninit_fields(cls: Dataclass, dct: dict, obj: Any) -> None:
+    assert dataclasses.is_dataclass(
+        cls,
+    )  # just for type narrowing -> even though beartype checks this, pyright still wants an assert
     state_fields = (
         f for f in dataclasses.fields(cls) if (not f.init and f.name in dct)
     )
     for f in state_fields:
         setattr(obj, f.name, dct[f.name])
```

### Comparing `nested_dataclass_serialization-0.1.4/nested_dataclass_serialization/strange_hack.py` & `nested_dataclass_serialization-0.1.5/nested_dataclass_serialization/strange_hack.py`

 * *Files identical despite different names*

### Comparing `nested_dataclass_serialization-0.1.4/pyproject.toml` & `nested_dataclass_serialization-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nested-dataclass-serialization"
-version = "0.1.4" # see: https://pypi.org/project/poetry-dynamic-versioning/
+version = "0.1.5" # see: https://pypi.org/project/poetry-dynamic-versioning/
 description = ""
 authors = ["Tilo Himmelsbach <dertilo@gmail.com>"]
 repository = "https://github.com/dertilo/nested-dataclass-serialization"
 
 readme = "README.md"
 packages = [{ include = "nested_dataclass_serialization" }]
```

### Comparing `nested_dataclass_serialization-0.1.4/PKG-INFO` & `nested_dataclass_serialization-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nested-dataclass-serialization
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Home-page: https://github.com/dertilo/nested-dataclass-serialization
 Author: Tilo Himmelsbach
 Author-email: dertilo@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

