# Comparing `tmp/numpydantic-1.0.0.tar.gz` & `tmp/numpydantic-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpydantic-1.0.0.tar", last modified: Thu May 23 07:29:21 2024, max compression
+gzip compressed data, was "numpydantic-1.0.0rc1.tar", last modified: Sat May 18 01:21:16 2024, max compression
```

## Comparing `numpydantic-1.0.0.tar` & `numpydantic-1.0.0rc1.tar`

### file list

```diff
@@ -1,36 +1,34 @@
--rw-r--r--   0        0        0     1071 2024-02-02 01:53:21.226339 numpydantic-1.0.0/LICENSE
--rw-r--r--   0        0        0    12440 2024-05-21 04:28:07.895951 numpydantic-1.0.0/README.md
--rw-r--r--   0        0        0     2238 2024-05-23 07:29:21.580436 numpydantic-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-04-04 03:21:40.424457 numpydantic-1.0.0/src/numpydantic/.DS_Store
--rw-r--r--   0        0        0      316 2024-04-23 02:35:29.607872 numpydantic-1.0.0/src/numpydantic/__init__.py
--rw-r--r--   0        0        0     2778 2024-05-23 06:28:37.793982 numpydantic-1.0.0/src/numpydantic/dtype.py
--rw-r--r--   0        0        0      197 2024-04-23 02:36:10.489339 numpydantic-1.0.0/src/numpydantic/exceptions.py
--rw-r--r--   0        0        0      520 2024-05-21 00:48:54.719182 numpydantic-1.0.0/src/numpydantic/interface/__init__.py
--rw-r--r--   0        0        0     1543 2024-05-18 00:28:09.845192 numpydantic-1.0.0/src/numpydantic/interface/dask.py
--rw-r--r--   0        0        0     6497 2024-05-18 00:28:27.564833 numpydantic-1.0.0/src/numpydantic/interface/hdf5.py
--rw-r--r--   0        0        0     6302 2024-05-18 01:08:19.698258 numpydantic-1.0.0/src/numpydantic/interface/interface.py
--rw-r--r--   0        0        0     1550 2024-05-18 00:53:46.935649 numpydantic-1.0.0/src/numpydantic/interface/numpy.py
--rw-r--r--   0        0        0     8212 2024-05-21 04:20:56.136256 numpydantic-1.0.0/src/numpydantic/interface/video.py
--rw-r--r--   0        0        0       47 2024-04-23 02:47:24.151838 numpydantic-1.0.0/src/numpydantic/interface/xarray.py
--rw-r--r--   0        0        0     4153 2024-05-18 00:34:12.796438 numpydantic-1.0.0/src/numpydantic/interface/zarr.py
--rw-r--r--   0        0        0     1470 2024-05-18 01:05:09.799203 numpydantic-1.0.0/src/numpydantic/maps.py
--rw-r--r--   0        0        0     2117 2024-05-18 01:15:56.425468 numpydantic-1.0.0/src/numpydantic/meta.py
--rw-r--r--   0        0        0     2138 2024-05-15 21:39:17.388265 numpydantic-1.0.0/src/numpydantic/monkeypatch.py
--rw-r--r--   0        0        0     4707 2024-05-23 07:26:11.702629 numpydantic-1.0.0/src/numpydantic/ndarray.py
--rw-r--r--   0        0        0      662 2024-05-23 04:31:36.720708 numpydantic-1.0.0/src/numpydantic/ndarray.pyi
--rw-r--r--   0        0        0     8724 2024-05-23 05:21:54.834499 numpydantic-1.0.0/src/numpydantic/schema.py
--rw-r--r--   0        0        0      678 2024-05-09 03:26:26.479741 numpydantic-1.0.0/src/numpydantic/types.py
--rw-r--r--   0        0        0        0 2024-04-03 22:50:41.167226 numpydantic-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     4836 2024-05-17 23:36:02.073010 numpydantic-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0     4021 2024-05-16 03:05:17.922915 numpydantic-1.0.0/tests/fixtures.py
--rw-r--r--   0        0        0        0 2024-04-09 00:54:38.999742 numpydantic-1.0.0/tests/test_interface/__init__.py
--rw-r--r--   0        0        0     1043 2024-05-09 05:06:59.486862 numpydantic-1.0.0/tests/test_interface/conftest.py
--rw-r--r--   0        0        0     1379 2024-05-14 22:28:23.749257 numpydantic-1.0.0/tests/test_interface/test_dask.py
--rw-r--r--   0        0        0     3249 2024-05-17 23:51:17.657048 numpydantic-1.0.0/tests/test_interface/test_hdf5.py
--rw-r--r--   0        0        0     2853 2024-05-18 01:13:40.285516 numpydantic-1.0.0/tests/test_interface/test_interface.py
--rw-r--r--   0        0        0      870 2024-05-17 23:59:26.685569 numpydantic-1.0.0/tests/test_interface/test_numpy.py
--rw-r--r--   0        0        0     5786 2024-05-21 04:20:57.765894 numpydantic-1.0.0/tests/test_interface/test_video.py
--rw-r--r--   0        0        0     3912 2024-05-18 02:04:19.887104 numpydantic-1.0.0/tests/test_interface/test_zarr.py
--rw-r--r--   0        0        0      881 2024-05-16 05:26:37.839232 numpydantic-1.0.0/tests/test_meta.py
--rw-r--r--   0        0        0     6724 2024-05-21 04:15:49.520841 numpydantic-1.0.0/tests/test_ndarray.py
--rw-r--r--   0        0        0    14228 1970-01-01 00:00:00.000000 numpydantic-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-02-02 01:53:21.226339 numpydantic-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     3919 2024-04-03 23:31:57.506716 numpydantic-1.0.0rc1/README.md
+-rw-r--r--   0        0        0     2056 2024-05-18 01:21:16.860265 numpydantic-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-04-04 03:21:40.424457 numpydantic-1.0.0rc1/src/numpydantic/.DS_Store
+-rw-r--r--   0        0        0      316 2024-04-23 02:35:29.607872 numpydantic-1.0.0rc1/src/numpydantic/__init__.py
+-rw-r--r--   0        0        0     2759 2024-05-16 05:09:35.686033 numpydantic-1.0.0rc1/src/numpydantic/dtype.py
+-rw-r--r--   0        0        0      197 2024-04-23 02:36:10.489339 numpydantic-1.0.0rc1/src/numpydantic/exceptions.py
+-rw-r--r--   0        0        0      443 2024-05-09 05:06:59.484309 numpydantic-1.0.0rc1/src/numpydantic/interface/__init__.py
+-rw-r--r--   0        0        0     1543 2024-05-18 00:28:09.845192 numpydantic-1.0.0rc1/src/numpydantic/interface/dask.py
+-rw-r--r--   0        0        0     6497 2024-05-18 00:28:27.564833 numpydantic-1.0.0rc1/src/numpydantic/interface/hdf5.py
+-rw-r--r--   0        0        0     6302 2024-05-18 01:08:19.698258 numpydantic-1.0.0rc1/src/numpydantic/interface/interface.py
+-rw-r--r--   0        0        0     1550 2024-05-18 00:53:46.935649 numpydantic-1.0.0rc1/src/numpydantic/interface/numpy.py
+-rw-r--r--   0        0        0       47 2024-04-23 02:47:24.151838 numpydantic-1.0.0rc1/src/numpydantic/interface/xarray.py
+-rw-r--r--   0        0        0     4153 2024-05-18 00:34:12.796438 numpydantic-1.0.0rc1/src/numpydantic/interface/zarr.py
+-rw-r--r--   0        0        0     1470 2024-05-18 01:05:09.799203 numpydantic-1.0.0rc1/src/numpydantic/maps.py
+-rw-r--r--   0        0        0     2117 2024-05-18 01:15:56.425468 numpydantic-1.0.0rc1/src/numpydantic/meta.py
+-rw-r--r--   0        0        0     2138 2024-05-15 21:39:17.388265 numpydantic-1.0.0rc1/src/numpydantic/monkeypatch.py
+-rw-r--r--   0        0        0     4919 2024-05-18 00:33:09.966148 numpydantic-1.0.0rc1/src/numpydantic/ndarray.py
+-rw-r--r--   0        0        0      542 2024-05-18 01:13:43.173698 numpydantic-1.0.0rc1/src/numpydantic/ndarray.pyi
+-rw-r--r--   0        0        0     6693 2024-05-18 01:03:52.283638 numpydantic-1.0.0rc1/src/numpydantic/schema.py
+-rw-r--r--   0        0        0      678 2024-05-09 03:26:26.479741 numpydantic-1.0.0rc1/src/numpydantic/types.py
+-rw-r--r--   0        0        0        0 2024-04-03 22:50:41.167226 numpydantic-1.0.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0     4836 2024-05-17 23:36:02.073010 numpydantic-1.0.0rc1/tests/conftest.py
+-rw-r--r--   0        0        0     4021 2024-05-16 03:05:17.922915 numpydantic-1.0.0rc1/tests/fixtures.py
+-rw-r--r--   0        0        0        0 2024-04-09 00:54:38.999742 numpydantic-1.0.0rc1/tests/test_interface/__init__.py
+-rw-r--r--   0        0        0     1043 2024-05-09 05:06:59.486862 numpydantic-1.0.0rc1/tests/test_interface/conftest.py
+-rw-r--r--   0        0        0     1379 2024-05-14 22:28:23.749257 numpydantic-1.0.0rc1/tests/test_interface/test_dask.py
+-rw-r--r--   0        0        0     3249 2024-05-17 23:51:17.657048 numpydantic-1.0.0rc1/tests/test_interface/test_hdf5.py
+-rw-r--r--   0        0        0     2853 2024-05-18 01:13:40.285516 numpydantic-1.0.0rc1/tests/test_interface/test_interface.py
+-rw-r--r--   0        0        0      870 2024-05-17 23:59:26.685569 numpydantic-1.0.0rc1/tests/test_interface/test_numpy.py
+-rw-r--r--   0        0        0     3912 2024-05-18 00:39:30.448720 numpydantic-1.0.0rc1/tests/test_interface/test_zarr.py
+-rw-r--r--   0        0        0      881 2024-05-16 05:26:37.839232 numpydantic-1.0.0rc1/tests/test_meta.py
+-rw-r--r--   0        0        0     5714 2024-05-18 01:05:33.062349 numpydantic-1.0.0rc1/tests/test_ndarray.py
+-rw-r--r--   0        0        0     5564 1970-01-01 00:00:00.000000 numpydantic-1.0.0rc1/PKG-INFO
```

### Comparing `numpydantic-1.0.0/LICENSE` & `numpydantic-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0/pyproject.toml` & `numpydantic-1.0.0rc1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 [project]
 name = "numpydantic"
-version = "1.0.0"
+version = "1.0.0.rc1"
 description = "Type and shape validation and serialization for numpy arrays in pydantic models"
 authors = [
     { name = "sneakers-the-rat", email = "sneakers-the-rat@protonmail.com" },
 ]
 dependencies = [
     "pydantic>=2.3.0",
     "nptyping>=2.5.0",
     "numpy>=1.24.0",
 ]
-homepage = "https://numpydantic.readthedocs.io"
 requires-python = "<4.0,>=3.9"
 readme = "README.md"
-repository = "https://github.com/p2p-ld/numpydantic"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 dask = [
     "dask>=2024.4.0",
 ]
 hdf5 = [
     "h5py>=3.10.0",
 ]
-video = [
-    "opencv-python>=4.9.0.80",
-]
 zarr = [
     "zarr>=2.17.2",
 ]
 arrays = [
-    "numpydantic[dask,hdf5,zarr,video]",
+    "numpydantic[dask,hdf5,zarr]",
 ]
 tests = [
     "numpydantic[arrays]",
     "pytest>=7.4.0",
     "pytest-depends<2.0.0,>=1.0.1",
     "coverage>=6.1.1",
     "pytest-cov<5.0.0,>=4.1.0",
@@ -45,15 +40,14 @@
 ]
 docs = [
     "sphinx<8.0.0,>=7.2.6",
     "furo>=2024.1.29",
     "myst-parser<3.0.0,>=2.0.0",
     "autodoc-pydantic<3.0.0,>=2.0.1",
     "sphinx-design<1.0.0,>=0.5.0",
-    "sphinxcontrib-mermaid>=0.9.2",
 ]
 dev = [
     "numpydantic[tests,docs]",
     "sphinx-autobuild>=2021.3.14",
     "black<25.0.0,>=24.1.1",
     "ruff<1.0.0,>=0.2.0",
 ]
```

### Comparing `numpydantic-1.0.0/src/numpydantic/.DS_Store` & `numpydantic-1.0.0rc1/src/numpydantic/.DS_Store`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0/src/numpydantic/dtype.py` & `numpydantic-1.0.0rc1/src/numpydantic/dtype.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 control of dtype specifications - like different precision modes, etc.
 and allow for abstract specifications of dtype that can be checked across
 interfaces.
 
 This module also allows for convenient access to all abstract dtypes in a single
 module, rather than needing to import each individually.
 
-Some types like `Integer` are compound types - tuples of multiple dtypes.
+Some types like :ref:`Integer` are compound types - tuples of multiple dtypes.
 Check these using ``in`` rather than ``==``. This interface will develop in future
 versions to allow a single dtype check.
 """
 
 import sys
 from typing import Tuple, Union
 
@@ -55,15 +55,14 @@
 UInt = np.uint
 ULongLong = np.ulonglong
 LongLong = np.longlong
 Timedelta64 = np.timedelta64
 SignedInteger = (np.int8, np.int16, np.int32, np.int64, np.short)
 UnsignedInteger = (np.uint8, np.uint16, np.uint32, np.uint64, np.ushort)
 Integer = tuple([*SignedInteger, *UnsignedInteger])
-"""All integer types"""
 Int = Integer  # Int should translate to the "generic" int type.
 
 Float16 = np.float16
 Float32 = np.float32
 Float64 = np.float64
 Half = np.half
 Single = np.single
```

### Comparing `numpydantic-1.0.0/src/numpydantic/interface/dask.py` & `numpydantic-1.0.0rc1/src/numpydantic/interface/dask.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0/src/numpydantic/interface/hdf5.py` & `numpydantic-1.0.0rc1/src/numpydantic/interface/hdf5.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0/src/numpydantic/interface/interface.py` & `numpydantic-1.0.0rc1/src/numpydantic/interface/interface.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0/src/numpydantic/interface/numpy.py` & `numpydantic-1.0.0rc1/src/numpydantic/interface/numpy.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0/src/numpydantic/interface/zarr.py` & `numpydantic-1.0.0rc1/src/numpydantic/interface/zarr.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0/src/numpydantic/maps.py` & `numpydantic-1.0.0rc1/src/numpydantic/maps.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0/src/numpydantic/meta.py` & `numpydantic-1.0.0rc1/src/numpydantic/meta.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0/src/numpydantic/monkeypatch.py` & `numpydantic-1.0.0rc1/src/numpydantic/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0/src/numpydantic/ndarray.py` & `numpydantic-1.0.0rc1/src/numpydantic/ndarray.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     those all belong in :mod:`numpydantic.schema` .
 
     Keeping with nptyping's style, NDArrayMeta is in this module even if it's
     excluded from the type stub.
 
 """
 
-from typing import Any, Tuple
+from typing import TYPE_CHECKING, Any, Tuple
 
 import numpy as np
 from nptyping.error import InvalidArgumentsError
 from nptyping.ndarray import NDArrayMeta as _NDArrayMeta
 from nptyping.nptyping_type import NPTypingType
 from nptyping.structure import Structure
 from nptyping.structure_expression import check_type_names
@@ -33,14 +33,21 @@
     _handler_type,
     _jsonize_array,
     get_validate_interface,
     make_json_schema,
 )
 from numpydantic.types import DtypeType, ShapeType
 
+if TYPE_CHECKING:  # pragma: no cover
+    pass
+
+"""
+python types that pydantic/json schema can't support (and Any will be used instead)
+"""
+
 
 class NDArrayMeta(_NDArrayMeta, implementation="NDArray"):
     """
     Hooking into nptyping's array metaclass to override methods pending
     completion of the transition away from nptyping
     """
 
@@ -79,17 +86,20 @@
 
 
 class NDArray(NPTypingType, metaclass=NDArrayMeta):
     """
     Constrained array type allowing npytyping syntax for dtype and shape validation
     and serialization.
 
-    This class is not intended to be instantiated or used for type checking, it
-    implements the ``__get_pydantic_core_schema__` method to invoke
-    the relevant :ref:`interface <Interfaces>` for validation and serialization.
+    Integrates with pydantic such that
+    - JSON schema for list of list encoding
+    - Serialized as LoL, with automatic compression for large arrays
+    - Automatic coercion from lists on instantiation
+
+    Also supports validation on :class:`.NDArrayProxy` types for lazy loading.
 
     References:
         - https://docs.pydantic.dev/latest/usage/types/custom/#handling-third-party-types
     """
 
     __args__: Tuple[ShapeType, DtypeType] = (Any, Any)
```

### Comparing `numpydantic-1.0.0/src/numpydantic/ndarray.pyi` & `numpydantic-1.0.0rc1/src/numpydantic/ndarray.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from dask.array.core import Array as DaskArrayCoreArray
 from numpydantic.interface.hdf5 import H5ArrayPath
 from typing import typing.Tuple[typing.Union[pathlib.Path, str], str]
 from pathlib import Path as PathlibPath
-from cv2 import VideoCapture as Cv2VideoCapture
-from pathlib import Path as PathlibPath
 from zarr.core import Array as ZarrCoreArray
 from numpydantic.interface.zarr import ZarrArrayPath
 from numpy import ndarray as Numpyndarray
 import typing
 import pathlib
-NDArray = DaskArrayCoreArray | H5ArrayPath | typing.Tuple[typing.Union[pathlib.Path, str], str] | PathlibPath | Cv2VideoCapture | PathlibPath | ZarrCoreArray | ZarrArrayPath | Numpyndarray
+NDArray = DaskArrayCoreArray | H5ArrayPath | typing.Tuple[typing.Union[pathlib.Path, str], str] | PathlibPath | ZarrCoreArray | ZarrArrayPath | Numpyndarray
```

### Comparing `numpydantic-1.0.0/src/numpydantic/schema.py` & `numpydantic-1.0.0rc1/src/numpydantic/schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """
 Helper functions for use with :class:`~numpydantic.NDArray` - see the note in
 :mod:`~numpydantic.ndarray` for why these are separated.
 """
 
-import hashlib
-import json
-from typing import Any, Callable, Optional, Union
+from typing import Any, Callable, Union
 
 import nptyping.structure
 import numpy as np
 from nptyping import Shape
 from pydantic import SerializationInfo
 from pydantic_core import CoreSchema, core_schema
 from pydantic_core.core_schema import ListSchema, ValidationInfo
@@ -122,77 +120,22 @@
 
         # make a label annotation, if we have one
         metadata = {"name": label} if label is not None else None
 
         # make the current level list schema, accounting for shape
         if arg == "*":
             list_schema = core_schema.list_schema(inner_schema, metadata=metadata)
-        elif arg == "...":
-            list_schema = _unbounded_shape(inner_schema, metadata=metadata)
         else:
-            try:
-                arg = int(arg)
-            except ValueError as e:
-                raise ValueError(
-                    "Array shapes must be integers, wildcards, or ellipses. "
-                    "Shape variables (for declaring that one dimension must be the "
-                    "same size as another) are not supported because it is "
-                    "impossible to express dynamic minItems/maxItems in JSON Schema. "
-                    "See: https://github.com/orgs/json-schema-org/discussions/730"
-                ) from e
+            arg = int(arg)
             list_schema = core_schema.list_schema(
                 inner_schema, min_length=arg, max_length=arg, metadata=metadata
             )
     return list_schema
 
 
-def _hash_schema(schema: CoreSchema) -> str:
-    """
-    Make a hex-encoded 8-byte blake2b hash from a pydantic core schema.
-    Collisions are really not important or likely here, but we do want the same schema
-    to produce the same hash.
-    """
-    schema_str = json.dumps(
-        schema, sort_keys=True, indent=None, separators=(",", ":")
-    ).encode("utf-8")
-    hasher = hashlib.blake2b(digest_size=8)
-    hasher.update(schema_str)
-    return hasher.hexdigest()
-
-
-def _unbounded_shape(
-    inner_type: CoreSchema, metadata: Optional[dict] = None
-) -> core_schema.DefinitionsSchema:
-    """
-    Make a recursive schema that refers to itself using a hashed version of the inner
-    type
-    """
-
-    schema_hash = _hash_schema(inner_type)
-    array_ref = f"any-shape-array-{schema_hash}"
-
-    schema = core_schema.definitions_schema(
-        core_schema.list_schema(
-            core_schema.definition_reference_schema(array_ref), metadata=metadata
-        ),
-        [
-            core_schema.union_schema(
-                [
-                    core_schema.list_schema(
-                        core_schema.definition_reference_schema(array_ref)
-                    ),
-                    inner_type,
-                ],
-                ref=array_ref,
-            )
-        ],
-    )
-    return schema
-
-
 def make_json_schema(
     shape: ShapeType, dtype: DtypeType, _handler: _handler_type
 ) -> ListSchema:
     """
     Make a list of list JSON schema from a shape and a dtype.
 
     First resolves the dtype into a pydantic ``CoreSchema`` ,
@@ -207,16 +150,15 @@
     Returns:
         :class:`pydantic_core.core_schema.ListSchema`
     """
     dtype_schema = _lol_dtype(dtype, _handler)
 
     # get the names of the shape constraints, if any
     if shape is Any:
-        list_schema = _unbounded_shape(dtype_schema)
-        # list_schema = core_schema.list_schema(core_schema.any_schema())
+        list_schema = core_schema.list_schema(core_schema.any_schema())
     else:
         list_schema = list_of_lists_schema(shape, dtype_schema)
 
     return list_schema
 
 
 def get_validate_interface(shape: ShapeType, dtype: DtypeType) -> Callable:
```

### Comparing `numpydantic-1.0.0/src/numpydantic/types.py` & `numpydantic-1.0.0rc1/src/numpydantic/types.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0/tests/conftest.py` & `numpydantic-1.0.0rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0/tests/fixtures.py` & `numpydantic-1.0.0rc1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0/tests/test_interface/conftest.py` & `numpydantic-1.0.0rc1/tests/test_interface/conftest.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0/tests/test_interface/test_dask.py` & `numpydantic-1.0.0rc1/tests/test_interface/test_dask.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0/tests/test_interface/test_hdf5.py` & `numpydantic-1.0.0rc1/tests/test_interface/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0/tests/test_interface/test_interface.py` & `numpydantic-1.0.0rc1/tests/test_interface/test_interface.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0/tests/test_interface/test_numpy.py` & `numpydantic-1.0.0rc1/tests/test_interface/test_numpy.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0/tests/test_interface/test_zarr.py` & `numpydantic-1.0.0rc1/tests/test_interface/test_zarr.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0/tests/test_meta.py` & `numpydantic-1.0.0rc1/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `numpydantic-1.0.0/tests/test_ndarray.py` & `numpydantic-1.0.0rc1/tests/test_ndarray.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 from nptyping import Shape, Number
 
 from numpydantic import NDArray
 from numpydantic.exceptions import ShapeError, DtypeError
 from numpydantic import dtype
 
 
+# from .fixtures import tmp_output_dir_func
+
+
 def test_ndarray_type():
     class Model(BaseModel):
         array: NDArray[Shape["2 x, * y"], Number]
         array_any: Optional[NDArray[Any, Any]] = None
 
     schema = Model.model_json_schema()
     assert schema["properties"]["array"]["items"] == {
@@ -179,47 +182,21 @@
     inner_type = schema["properties"]["array"]["items"]["items"]
     if expected == "any":
         assert inner_type == {}
     else:
         assert inner_type["type"] == expected
 
 
-def _recursive_array(schema):
-    assert "$defs" in schema
-    # get the key uses for the array
-    array_key = list(schema["$defs"].keys())[0]
-
-    # the array property should be a ref to the recursive array
-    # get the innermost part of the field schema
-    field_schema = schema["properties"]["array"]
-    while "items" in field_schema:
-        field_schema = field_schema["items"]
-    assert field_schema["$ref"] == f"#/$defs/{array_key}"
-
-    # and the recursive array should indeed be recursive...
-    # specifically it should be an array whose items can be itself or
-    # of the type specified by the dtype
-    any_of = schema["$defs"][array_key]["anyOf"]
-    assert any_of[0]["items"]["$ref"] == f"#/$defs/{array_key}"
-    assert any_of[0]["type"] == "array"
-    # here we are just assuming that it's a uint8 array..
-    assert any_of[1]["type"] == "integer"
-    assert any_of[1]["maximum"] == 255
-    assert any_of[1]["minimum"] == 0
+@pytest.mark.skip("Not implemented yet")
+def test_json_schema_wildcard():
+    """
+    NDarray types should generate a JSON schema without shape constraints
+    """
+    pass
 
 
+@pytest.mark.skip("Not implemented yet")
 def test_json_schema_ellipsis():
     """
     NDArray types should create a recursive JSON schema for any-shaped arrays
     """
-
-    class AnyShape(BaseModel):
-        array: NDArray[Shape["*, ..."], np.uint8]
-
-    schema = AnyShape.model_json_schema()
-    _recursive_array(schema)
-
-    class ConstrainedAnyShape(BaseModel):
-        array: NDArray[Shape["3, 4, ..."], np.uint8]
-
-    schema = ConstrainedAnyShape.model_json_schema()
-    _recursive_array(schema)
+    pass
```

