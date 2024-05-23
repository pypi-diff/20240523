# Comparing `tmp/pydantic_to_pyarrow-0.1.2.tar.gz` & `tmp/pydantic_to_pyarrow-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_to_pyarrow-0.1.2.tar", max compression
+gzip compressed data, was "pydantic_to_pyarrow-0.1.3.tar", max compression
```

## Comparing `pydantic_to_pyarrow-0.1.2.tar` & `pydantic_to_pyarrow-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1062 2024-03-05 15:00:36.142359 pydantic_to_pyarrow-0.1.2/LICENSE
--rw-r--r--   0        0        0     3881 2024-03-05 15:00:36.142359 pydantic_to_pyarrow-0.1.2/README.md
--rw-r--r--   0        0        0     3221 2024-03-05 15:00:36.142359 pydantic_to_pyarrow-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      170 2024-03-05 15:00:36.146359 pydantic_to_pyarrow-0.1.2/src/pydantic_to_pyarrow/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 15:00:36.146359 pydantic_to_pyarrow-0.1.2/src/pydantic_to_pyarrow/py.typed
--rw-r--r--   0        0        0     7341 2024-03-05 15:00:36.146359 pydantic_to_pyarrow-0.1.2/src/pydantic_to_pyarrow/schema.py
--rw-r--r--   0        0        0     5490 1970-01-01 00:00:00.000000 pydantic_to_pyarrow-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-23 13:59:19.117635 pydantic_to_pyarrow-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4356 2024-05-23 13:59:19.117635 pydantic_to_pyarrow-0.1.3/README.md
+-rw-r--r--   0        0        0     3221 2024-05-23 13:59:19.117635 pydantic_to_pyarrow-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      170 2024-05-23 13:59:19.117635 pydantic_to_pyarrow-0.1.3/src/pydantic_to_pyarrow/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 13:59:19.117635 pydantic_to_pyarrow-0.1.3/src/pydantic_to_pyarrow/py.typed
+-rw-r--r--   0        0        0     8982 2024-05-23 13:59:19.117635 pydantic_to_pyarrow-0.1.3/src/pydantic_to_pyarrow/schema.py
+-rw-r--r--   0        0        0     5965 1970-01-01 00:00:00.000000 pydantic_to_pyarrow-0.1.3/PKG-INFO
```

### Comparing `pydantic_to_pyarrow-0.1.2/LICENSE` & `pydantic_to_pyarrow-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_to_pyarrow-0.1.2/README.md` & `pydantic_to_pyarrow-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -60,44 +60,54 @@
 datetime.datetime | pa.timestamp("ms", tz=None) ONLY if param allow_losing_tz=True |
 pydantic.types.NaiveDatetime | pa.timestamp("ms", tz=None) |
 pydantic.types.AwareDatetime | pa.timestamp("ms", tz=None) ONLY if param allow_losing_tz=True |
 . | .
 Optional[...] | The pyarrow field is nullable |
 Pydantic Model | pa.struct() |
 List[...] | pa.list_(...) |
+Dict[..., ...] | pa.map_(pa key_type, pa value_type) |
 Enum of str | pa.dictionary(pa.int32(), pa.string()) | 
 Enum of int | pa.int64() |
 
+If a field is marked as exclude, (`Field(exclude=True)`), then it will be excluded
+from the pyarrow schema if exclude_fields is set to True.
+
 ## An Example
 
 ```py
-from typing import List, Optional
+from typing import Dict, List, Optional
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 from pydantic_to_pyarrow import get_pyarrow_schema
 
 class NestedModel(BaseModel):
     str_field: str
 
 
 class MyModel(BaseModel):
     int_field: int
     opt_str_field: Optional[str]
     py310_opt_str_field: str | None
     nested: List[NestedModel]
+    dict_field: Dict[str, int]
+    excluded_field: str = Field(exclude=True)
 
 
 pa_schema = get_pyarrow_schema(MyModel)
 print(pa_schema)
 #> int_field: int64 not null
 #> opt_str_field: string
 #> py310_opt_str_field: string
 #> nested: list<item: struct<str_field: string not null>> not null
 #>   child 0, item: struct<str_field: string not null>
 #>       child 0, str_field: string not null
+#> dict_field: map<string, int64> not null
+#>   child 0, entries: struct<key: string not null, value: int64> not null
+#>       child 0, key: string not null
+#>       child 1, value: int64
 ```
 
 ## Development
 
 Prerequisites:
 
 - Any Python 3.8 through 3.11
```

### Comparing `pydantic_to_pyarrow-0.1.2/pyproject.toml` & `pydantic_to_pyarrow-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "pydantic_to_pyarrow"
-version = "0.1.2"
+version = "0.1.3"
 description = "Conversion from pydantic models to pyarrow schemas"
 authors = ["Simon Wicks <simw@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/simw/pydantic-to-pyarrow"
 license = "MIT"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `pydantic_to_pyarrow-0.1.2/src/pydantic_to_pyarrow/schema.py` & `pydantic_to_pyarrow-0.1.3/src/pydantic_to_pyarrow/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -70,55 +70,90 @@
 TYPES_WITH_METADATA = {
     Decimal: _get_decimal_type,
     int: _get_int_type,
 }
 
 
 def _get_literal_type(
-    field_type: Type[Any], _metadata: List[Any], _allow_losing_tz: bool
+    field_type: Type[Any],
+    _metadata: List[Any],
+    _allow_losing_tz: bool,
+    _exclude_fields: bool,
 ) -> pa.DataType:
     values = get_args(field_type)
     if all(isinstance(value, str) for value in values):
         return pa.dictionary(pa.int32(), pa.string())
     elif all(isinstance(value, int) for value in values):
         # Dictionary of (int, int) is converted to just int when
         # written into parquet.
         return pa.int64()
     else:
         msg = "Literal type is only supported with all int or string values. "
         raise SchemaCreationError(msg)
 
 
 def _get_list_type(
-    field_type: Type[Any], metadata: List[Any], allow_losing_tz: bool
+    field_type: Type[Any],
+    metadata: List[Any],
+    allow_losing_tz: bool,
+    _exclude_fields: bool,
 ) -> pa.DataType:
     sub_type = get_args(field_type)[0]
     if _is_optional(sub_type):
         # pyarrow lists can have null elements in them
         sub_type = list(set(get_args(sub_type)) - {type(None)})[0]
-    return pa.list_(_get_pyarrow_type(sub_type, metadata, allow_losing_tz))
+    return pa.list_(
+        _get_pyarrow_type(sub_type, metadata, allow_losing_tz, _exclude_fields)
+    )
 
 
 def _get_annotated_type(
-    field_type: Type[Any], metadata: List[Any], allow_losing_tz: bool
+    field_type: Type[Any],
+    metadata: List[Any],
+    allow_losing_tz: bool,
+    exclude_fields: bool,
 ) -> pa.DataType:
     # TODO: fix / clean up / understand why / if this works in all cases
     args = get_args(field_type)[1:]
     metadatas = [
         item.metadata if hasattr(item, "metadata") else [item] for item in args
     ]
     metadata = [item for sublist in metadatas for item in sublist]
     field_type = cast(Type[Any], get_args(field_type)[0])
-    return _get_pyarrow_type(field_type, metadata, allow_losing_tz)
+    return _get_pyarrow_type(field_type, metadata, allow_losing_tz, exclude_fields)
+
+
+def _get_dict_type(
+    field_type: Type[Any],
+    metadata: List[Any],
+    allow_losing_tz: bool,
+    _exclude_fields: bool,
+) -> pa.DataType:
+    key_type, value_type = get_args(field_type)
+    return pa.map_(
+        _get_pyarrow_type(
+            key_type,
+            metadata,
+            allow_losing_tz=allow_losing_tz,
+            exclude_fields=_exclude_fields,
+        ),
+        _get_pyarrow_type(
+            value_type,
+            metadata,
+            allow_losing_tz=allow_losing_tz,
+            exclude_fields=_exclude_fields,
+        ),
+    )
 
 
 FIELD_TYPES = {
     Literal: _get_literal_type,
     list: _get_list_type,
     Annotated: _get_annotated_type,
+    dict: _get_dict_type,
 }
 
 
 def _get_enum_type(field_type: Type[Any]) -> pa.DataType:
     is_str = [isinstance(enum_value.value, str) for enum_value in field_type]
     if all(is_str):
         return pa.dictionary(pa.int32(), pa.string())
@@ -139,15 +174,18 @@
     if not is_python_39_union and not is_python_310_union:
         return False
 
     return type(None) in get_args(field_type)
 
 
 def _get_pyarrow_type(
-    field_type: Type[Any], metadata: List[Any], allow_losing_tz: bool
+    field_type: Type[Any],
+    metadata: List[Any],
+    allow_losing_tz: bool,
+    exclude_fields: bool,
 ) -> pa.DataType:
     if field_type in FIELD_MAP:
         return FIELD_MAP[field_type]
 
     if allow_losing_tz and field_type in LOSING_TZ_TYPES:
         return LOSING_TZ_TYPES[field_type]
 
@@ -160,32 +198,37 @@
         return _get_enum_type(field_type)
 
     if field_type in TYPES_WITH_METADATA:
         return TYPES_WITH_METADATA[field_type](metadata)
 
     if get_origin(field_type) in FIELD_TYPES:
         return FIELD_TYPES[get_origin(field_type)](
-            field_type, metadata, allow_losing_tz
+            field_type, metadata, allow_losing_tz, exclude_fields
         )
 
     # isinstance(filed_type, type) checks whether it's a class
     # otherwise eg Deque[int] would casue an exception on issubclass
     if isinstance(field_type, type) and issubclass(field_type, BaseModel):
-        return _get_pyarrow_schema(field_type, allow_losing_tz, as_schema=False)
+        return _get_pyarrow_schema(
+            field_type, allow_losing_tz, exclude_fields, as_schema=False
+        )
 
     raise SchemaCreationError(f"Unknown type: {field_type}")
 
 
 def _get_pyarrow_schema(
     pydantic_class: Type[BaseModelType],
     allow_losing_tz: bool,
+    exclude_fields: bool,
     as_schema: bool = True,
 ) -> pa.Schema:
     fields = []
     for name, field_info in pydantic_class.model_fields.items():
+        if field_info.exclude and exclude_fields:
+            continue
         field_type = field_info.annotation
         metadata = field_info.metadata
 
         if field_type is None:
             # Not sure how to get here through pydantic, hence nocover
             raise SchemaCreationError(
                 f"Missing type for field {name}"
@@ -196,25 +239,45 @@
             if _is_optional(field_type):
                 nullable = True
                 types_under_union = list(set(get_args(field_type)) - {type(None)})
                 # mypy infers field_type as Type[Any] | None here, hence casting
                 field_type = cast(Type[Any], types_under_union[0])
 
             pa_field = _get_pyarrow_type(
-                field_type, metadata, allow_losing_tz=allow_losing_tz
+                field_type,
+                metadata,
+                allow_losing_tz=allow_losing_tz,
+                exclude_fields=exclude_fields,
             )
         except Exception as err:  # noqa: BLE001 - ignore blind exception
             raise SchemaCreationError(
                 f"Error processing field {name}: {field_type}, {err}"
             ) from err
 
         fields.append(pa.field(name, pa_field, nullable=nullable))
 
     if as_schema:
         return pa.schema(fields)
     return pa.struct(fields)
 
 
 def get_pyarrow_schema(
-    pydantic_class: Type[BaseModelType], allow_losing_tz: bool = False
+    pydantic_class: Type[BaseModelType],
+    allow_losing_tz: bool = False,
+    exclude_fields: bool = False,
 ) -> pa.Schema:
-    return _get_pyarrow_schema(pydantic_class, allow_losing_tz)
+    """
+    Converts a Pydantic model into a PyArrow schema.
+
+    Args:
+        pydantic_class (Type[BaseModelType]): The Pydantic model class to convert.
+        allow_losing_tz (bool, optional): Whether to allow losing timezone information
+        when converting datetime fields. Defaults to False.
+        exclude_fields (bool, optional): If True, will exclude fields in the pydantic
+        model that have `Field(exclude=True)`. Defaults to False.
+
+    Returns:
+        pa.Schema: The PyArrow schema representing the Pydantic model.
+    """
+    return _get_pyarrow_schema(
+        pydantic_class, allow_losing_tz, exclude_fields=exclude_fields
+    )
```

### Comparing `pydantic_to_pyarrow-0.1.2/PKG-INFO` & `pydantic_to_pyarrow-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic_to_pyarrow
-Version: 0.1.2
+Version: 0.1.3
 Summary: Conversion from pydantic models to pyarrow schemas
 Home-page: https://github.com/simw/pydantic-to-pyarrow
 License: MIT
 Author: Simon Wicks
 Author-email: simw@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -95,44 +95,54 @@
 datetime.datetime | pa.timestamp("ms", tz=None) ONLY if param allow_losing_tz=True |
 pydantic.types.NaiveDatetime | pa.timestamp("ms", tz=None) |
 pydantic.types.AwareDatetime | pa.timestamp("ms", tz=None) ONLY if param allow_losing_tz=True |
 . | .
 Optional[...] | The pyarrow field is nullable |
 Pydantic Model | pa.struct() |
 List[...] | pa.list_(...) |
+Dict[..., ...] | pa.map_(pa key_type, pa value_type) |
 Enum of str | pa.dictionary(pa.int32(), pa.string()) | 
 Enum of int | pa.int64() |
 
+If a field is marked as exclude, (`Field(exclude=True)`), then it will be excluded
+from the pyarrow schema if exclude_fields is set to True.
+
 ## An Example
 
 ```py
-from typing import List, Optional
+from typing import Dict, List, Optional
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 from pydantic_to_pyarrow import get_pyarrow_schema
 
 class NestedModel(BaseModel):
     str_field: str
 
 
 class MyModel(BaseModel):
     int_field: int
     opt_str_field: Optional[str]
     py310_opt_str_field: str | None
     nested: List[NestedModel]
+    dict_field: Dict[str, int]
+    excluded_field: str = Field(exclude=True)
 
 
 pa_schema = get_pyarrow_schema(MyModel)
 print(pa_schema)
 #> int_field: int64 not null
 #> opt_str_field: string
 #> py310_opt_str_field: string
 #> nested: list<item: struct<str_field: string not null>> not null
 #>   child 0, item: struct<str_field: string not null>
 #>       child 0, str_field: string not null
+#> dict_field: map<string, int64> not null
+#>   child 0, entries: struct<key: string not null, value: int64> not null
+#>       child 0, key: string not null
+#>       child 1, value: int64
 ```
 
 ## Development
 
 Prerequisites:
 
 - Any Python 3.8 through 3.11
```

