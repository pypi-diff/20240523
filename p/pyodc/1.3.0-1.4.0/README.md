# Comparing `tmp/pyodc-1.3.0.tar.gz` & `tmp/pyodc-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodc-1.3.0.tar", last modified: Wed May 17 13:29:33 2023, max compression
+gzip compressed data, was "pyodc-1.4.0.tar", last modified: Thu May 23 14:04:31 2024, max compression
```

## Comparing `pyodc-1.3.0.tar` & `pyodc-1.4.0.tar`

### file list

```diff
@@ -1,32 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:29:33.162597 pyodc-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1861 2023-05-17 13:29:16.000000 pyodc-1.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-17 13:29:16.000000 pyodc-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-17 13:29:16.000000 pyodc-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-05-17 13:29:33.162597 pyodc-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2923 2023-05-17 13:29:16.000000 pyodc-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:29:33.158597 pyodc-1.3.0/codc/
--rw-r--r--   0 runner    (1001) docker     (122)      240 2023-05-17 13:29:16.000000 pyodc-1.3.0/codc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-05-17 13:29:16.000000 pyodc-1.3.0/codc/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     5119 2023-05-17 13:29:16.000000 pyodc-1.3.0/codc/encoder.py
--rw-r--r--   0 runner    (1001) docker     (122)    11772 2023-05-17 13:29:16.000000 pyodc-1.3.0/codc/frame.py
--rw-r--r--   0 runner    (1001) docker     (122)     4718 2023-05-17 13:29:16.000000 pyodc-1.3.0/codc/lib.py
--rw-r--r--   0 runner    (1001) docker     (122)     5122 2023-05-17 13:29:16.000000 pyodc-1.3.0/codc/processed_odc.h
--rw-r--r--   0 runner    (1001) docker     (122)     2197 2023-05-17 13:29:16.000000 pyodc-1.3.0/codc/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:29:33.162597 pyodc-1.3.0/pyodc/
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-05-17 13:29:16.000000 pyodc-1.3.0/pyodc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15966 2023-05-17 13:29:16.000000 pyodc-1.3.0/pyodc/codec.py
--rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-05-17 13:29:16.000000 pyodc-1.3.0/pyodc/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     6957 2023-05-17 13:29:16.000000 pyodc-1.3.0/pyodc/encoder.py
--rw-r--r--   0 runner    (1001) docker     (122)    13398 2023-05-17 13:29:16.000000 pyodc-1.3.0/pyodc/frame.py
--rw-r--r--   0 runner    (1001) docker     (122)     2630 2023-05-17 13:29:16.000000 pyodc-1.3.0/pyodc/reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     2804 2023-05-17 13:29:16.000000 pyodc-1.3.0/pyodc/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:29:33.162597 pyodc-1.3.0/pyodc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-05-17 13:29:33.000000 pyodc-1.3.0/pyodc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      463 2023-05-17 13:29:33.000000 pyodc-1.3.0/pyodc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 13:29:33.000000 pyodc-1.3.0/pyodc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-17 13:29:33.000000 pyodc-1.3.0/pyodc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-17 13:29:33.000000 pyodc-1.3.0/pyodc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 13:29:33.000000 pyodc-1.3.0/pyodc.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-17 13:29:16.000000 pyodc-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 13:29:33.162597 pyodc-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-05-17 13:29:16.000000 pyodc-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:04:31.421677 pyodc-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-23 14:04:23.000000 pyodc-1.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 14:04:23.000000 pyodc-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-23 14:04:23.000000 pyodc-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-05-23 14:04:31.421677 pyodc-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-05-23 14:04:23.000000 pyodc-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:04:31.417677 pyodc-1.4.0/codc/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-23 14:04:23.000000 pyodc-1.4.0/codc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-23 14:04:23.000000 pyodc-1.4.0/codc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-05-23 14:04:23.000000 pyodc-1.4.0/codc/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-05-23 14:04:23.000000 pyodc-1.4.0/codc/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-23 14:04:23.000000 pyodc-1.4.0/codc/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-23 14:04:23.000000 pyodc-1.4.0/codc/processed_odc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-23 14:04:23.000000 pyodc-1.4.0/codc/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:04:31.417677 pyodc-1.4.0/pyodc/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-23 14:04:23.000000 pyodc-1.4.0/pyodc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16540 2024-05-23 14:04:23.000000 pyodc-1.4.0/pyodc/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-23 14:04:23.000000 pyodc-1.4.0/pyodc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-23 14:04:23.000000 pyodc-1.4.0/pyodc/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-05-23 14:04:23.000000 pyodc-1.4.0/pyodc/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-23 14:04:23.000000 pyodc-1.4.0/pyodc/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-23 14:04:23.000000 pyodc-1.4.0/pyodc/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:04:31.421677 pyodc-1.4.0/pyodc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-05-23 14:04:31.000000 pyodc-1.4.0/pyodc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-23 14:04:31.000000 pyodc-1.4.0/pyodc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:04:31.000000 pyodc-1.4.0/pyodc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 14:04:31.000000 pyodc-1.4.0/pyodc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 14:04:31.000000 pyodc-1.4.0/pyodc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:04:31.000000 pyodc-1.4.0/pyodc.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-23 14:04:23.000000 pyodc-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 14:04:31.421677 pyodc-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-23 14:04:23.000000 pyodc-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:04:31.421677 pyodc-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-05-23 14:04:23.000000 pyodc-1.4.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-23 14:04:23.000000 pyodc-1.4.0/tests/test_column_disambiguation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-23 14:04:23.000000 pyodc-1.4.0/tests/test_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14179 2024-05-23 14:04:23.000000 pyodc-1.4.0/tests/test_end_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-23 14:04:23.000000 pyodc-1.4.0/tests/test_initial_missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-23 14:04:23.000000 pyodc-1.4.0/tests/test_integral_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-23 14:04:23.000000 pyodc-1.4.0/tests/test_pyodc_codc_interop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-23 14:04:23.000000 pyodc-1.4.0/tests/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-23 14:04:23.000000 pyodc-1.4.0/tests/test_string_codecs.py
```

### Comparing `pyodc-1.3.0/CHANGELOG.md` & `pyodc-1.4.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyodc-1.3.0/LICENSE` & `pyodc-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodc-1.3.0/PKG-INFO` & `pyodc-1.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodc
-Version: 1.3.0
+Version: 1.4.0
 Summary: A Python interface to odc for encoding/decoding ODB-2 files.
 Home-page: https://github.com/ecmwf/pyodc
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: odc odb
 Classifier: Development Status :: 4 - Beta
@@ -15,14 +15,17 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cffi
+Requires-Dist: findlibs>=0.0.5
+Requires-Dist: pandas
 
 # pyodc
 
 [![PyPI](https://img.shields.io/pypi/v/pyodc)](https://pypi.org/project/pyodc/)
 [![Build Status](https://img.shields.io/github/workflow/status/ecmwf/pyodc/Continuous%20Integration/develop)](https://github.com/ecmwf/pyodc/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/pyodc/badge/?version=latest)](https://pyodc.readthedocs.io/en/latest/?badge=latest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -46,15 +49,15 @@
 ### Optional
 
 * [odc]
 * [pytest]
 * [pandoc]
 * [Jupyter Notebook]
 
-For `codc` to work, `odc` library must be compiled and installed on the system and made available to Python (through the CFFI mechanism) as a shared library. There are multiple ways to make the library visible to CFFI: it can be installed as a system library, the installation prefix can be passed in `odc_DIR` environment variable, or the library directory can be included in `LD_LIBRARY_PATH`.
+For `codc` to work, `odc` library must be compiled and installed on the system and made available to Python (through the CFFI mechanism) as a shared library. There are multiple ways to make the library visible to CFFI: it can be installed as a system library, the installation prefix can be passed in the `odc_DIR` or `ODC_DIR` environment variables, or the library directory can be included in `LD_LIBRARY_PATH`.
 
 ## Installation
 
 ```sh
 pip install --user pyodc
 ```
```

### Comparing `pyodc-1.3.0/README.md` & `pyodc-1.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ### Optional
 
 * [odc]
 * [pytest]
 * [pandoc]
 * [Jupyter Notebook]
 
-For `codc` to work, `odc` library must be compiled and installed on the system and made available to Python (through the CFFI mechanism) as a shared library. There are multiple ways to make the library visible to CFFI: it can be installed as a system library, the installation prefix can be passed in `odc_DIR` environment variable, or the library directory can be included in `LD_LIBRARY_PATH`.
+For `codc` to work, `odc` library must be compiled and installed on the system and made available to Python (through the CFFI mechanism) as a shared library. There are multiple ways to make the library visible to CFFI: it can be installed as a system library, the installation prefix can be passed in the `odc_DIR` or `ODC_DIR` environment variables, or the library directory can be included in `LD_LIBRARY_PATH`.
 
 ## Installation
 
 ```sh
 pip install --user pyodc
 ```
```

### Comparing `pyodc-1.3.0/codc/encoder.py` & `pyodc-1.4.0/codc/encoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,23 +53,23 @@
             if arr.dtype in ("uint64", "int64"):
                 dtype = INTEGER
             elif arr.dtype == "float64":
                 if not data.isnull().all() and all(pandas.isnull(v) or float(v).is_integer() for v in arr):
                     dtype = INTEGER
                 else:
                     dtype = DOUBLE
-            elif arr.dtype == "object":
+            if arr.dtype == "object" or pandas.api.types.is_string_dtype(arr):
                 if not arr.isnull().all() and all(s is None or isinstance(s, str) for s in arr):
                     dtype = STRING
                 elif arr.isnull().all():
                     dtype = INTEGER
 
         # With an inferred, or supplied column type, massage the data into a form that can be encoded
 
-        if arr.dtype == "object":
+        if arr.dtype == "object" or pandas.api.types.is_string_dtype(arr):
             # Map strings into an array that can be read in C
             if dtype == STRING:
                 return_arr = return_arr.astype("|S{}".format(max(8, 8 * (1 + ((max(len(s) for s in arr) - 1) // 8)))))
             elif dtype == INTEGER or dtype == BITFIELD:
                 return_arr = return_arr.fillna(value=missing_integer).astype("int64")
 
         elif arr.dtype == "float64":
@@ -102,15 +102,15 @@
     # we need to put it somewhere to ensure it stays alive appropriately long.
     data_cache = []
 
     for i, (name, data) in enumerate(df.items()):
         data, dtype = infer_column_type(data, types.get(name, None))
         data_cache.append(data)
 
-        lib.odc_encoder_add_column(encoder, name.encode("utf-8"), dtype)
+        lib.odc_encoder_add_column(encoder, str(name).encode("utf-8"), dtype)
         lib.odc_encoder_column_set_data_array(
             encoder,
             i,
             data.dtype.itemsize,
             data.array.to_numpy().strides[0],
             ffi.cast("void*", data.values.ctypes.data),
         )
```

### Comparing `pyodc-1.3.0/codc/frame.py` & `pyodc-1.4.0/codc/frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .constants import BITFIELD, DOUBLE, INTEGER, REAL, STRING, DataType
+from .constants import BITFIELD, DOUBLE, INTEGER, REAL, STRING, DataType, type_name
 from .lib import ffi, lib, memoize_constant
 
 try:
     from collections.abc import Iterable
 except ImportError:
     from collections import Iterable
 
@@ -60,15 +60,15 @@
             assert all(isinstance(b, ColumnInfo.Bitfield) for b in self.bitfields)
 
     def __str__(self):
         if self.bitfields is not None:
             bitfield_str = "(" + ",".join("{}:{}".format(b.name, b.size) for b in self.bitfields) + ")"
         else:
             bitfield_str = ""
-        return "{}:{}{}".format(self.name, self.dtype, bitfield_str)
+        return "{}:{}{}".format(self.name, type_name(self.dtype), bitfield_str)
 
     def __repr__(self):
         return str(self)
 
 
 class Frame:
     def __init__(self, table):
@@ -173,26 +173,36 @@
     def dataframe(self, columns=None):
         # Are there any bitfield columns we need to consider?
         original_columns = columns
         bitfields = []
 
         if columns is not None:
             final_columns = set()
+            _original_columns = self.column_dict.keys()
+            _original_simple_columns = self.simple_column_dict.keys()
+
             for colname in columns:
-                dotpos = colname.find(".")
-                if dotpos == -1:
+
+                # If the column is already present, then use that one directly.
+                # This ensures that we can handle exploded bitfield columns, and extract bitfields from
+                # existing columns below
+                if colname in _original_columns or colname in _original_simple_columns:
                     final_columns.add(colname)
                 else:
-                    column_name = colname[:dotpos]
-                    sp = colname[dotpos + 1 :].split("@")
-                    bitfield_name = sp[0]
-                    if len(sp) > 1:
-                        column_name += "@" + sp[1]
-                    final_columns.add(column_name)
-                    bitfields.append((bitfield_name, column_name, colname))
+                    dotpos = colname.find(".")
+                    if dotpos == -1:
+                        final_columns.add(colname)
+                    else:
+                        column_name = colname[:dotpos]
+                        sp = colname[dotpos + 1 :].split("@")
+                        bitfield_name = sp[0]
+                        if len(sp) > 1:
+                            column_name += "@" + sp[1]
+                        final_columns.add(column_name)
+                        bitfields.append((bitfield_name, column_name, colname))
             columns = list(final_columns)
 
         df = self._dataframe_internal(columns)
 
         # If there are any bitfields that need extraction, do it here, and remove any temporarily
         # decoded columns as is possible
```

### Comparing `pyodc-1.3.0/codc/lib.py` & `pyodc-1.4.0/codc/lib.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
 import cffi
+import findlibs
 from pkg_resources import parse_version
 
 __odc_version__ = "1.4.0"
 
 ffi = cffi.FFI()
 
 
@@ -40,32 +41,19 @@
     """
 
     __type_names = {}
 
     def __init__(self):
         ffi.cdef(self.__read_header())
 
-        libnames = [
-            "odccore",
-        ]
-        for env_var in ("ODC_DIR", "odc_DIR"):
-            if os.environ.get(env_var):
-                libnames.insert(0, os.path.join(os.environ[env_var], "lib/libodccore"))
-                libnames.insert(0, os.path.join(os.environ[env_var], "lib64/libodccore"))
-                libnames.insert(0, os.path.join(os.environ[env_var], "lib/libodccore.so"))
-                libnames.insert(0, os.path.join(os.environ[env_var], "lib64/libodccore.so"))
-
-        for libname in libnames:
-            try:
-                self.__lib = ffi.dlopen(libname)
-                break
-            except Exception as e:
-                last_exception = e
-        else:
-            raise CFFIModuleLoadFailed() from last_exception
+        library_path = findlibs.find("odccore", pkg_name="odc")
+        if library_path is None:
+            raise RuntimeError("Cannot find the odccore library")
+
+        self.__lib = ffi.dlopen(library_path)
 
         # Todo: Version check against __version__
 
         # All of the executable members of the CFFI-loaded library are functions in the ODC
         # C API. These should be wrapped with the correct error handling. Otherwise forward
         # these on directly.
```

### Comparing `pyodc-1.3.0/codc/processed_odc.h` & `pyodc-1.4.0/codc/processed_odc.h`

 * *Files identical despite different names*

### Comparing `pyodc-1.3.0/codc/reader.py` & `pyodc-1.4.0/codc/reader.py`

 * *Files identical despite different names*

### Comparing `pyodc-1.3.0/pyodc/codec.py` & `pyodc-1.4.0/pyodc/codec.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     def data_size(self):
         """
         Size of the decoded data in bytes.
         """
         return 8
 
     def encode_header(self, stream):
-        stream.encodeString(self.column_name)
+        stream.encodeString(str(self.column_name))
         stream.encodeInt32(self.type)
 
         if self.type == DataType.BITFIELD:
             assert len(self.bitfield_sizes) == len(self.bitfield_names)
             stream.encodeInt32(len(self.bitfield_names))
             for nm in self.bitfield_names:
                 stream.encodeString(nm)
@@ -112,19 +112,35 @@
 
 
 # n.b. The codec names match the class names
 
 
 class Constant(Codec):
     @classmethod
-    def from_dataframe(cls, column_name: str, data: pd.Series, data_type: DataType, bitfields):
+    def from_dataframe(cls, column_name: str, data: pd.Series, data_type: DataType, bitfields: list):
         assert data.nunique() == 1 and not data.hasnans
-        assert not bitfields
         value = next(iter(data))
-        return cls(column_name, value, value, data_type)
+
+        if bitfields:
+            assert data_type == DataType.BITFIELD
+            bitfield_names = [bf if isinstance(bf, str) else bf[0] for bf in bitfields]
+            bitfield_sizes = [1 if isinstance(bf, str) else bf[1] for bf in bitfields]
+        else:
+            bitfield_names = []
+            bitfield_sizes = []
+
+        return cls(
+            column_name,
+            minval=value,
+            maxval=value,
+            data_type=data_type,
+            has_missing=False,
+            bitfield_names=bitfield_names,
+            bitfield_sizes=bitfield_sizes,
+        )
 
     def encode(self, stream, value):
         pass
 
     def decode(self, stream):
         return {DataType.INTEGER: int, DataType.REAL: float, DataType.DOUBLE: float, DataType.BITFIELD: int}[self.type](
             self.min
@@ -428,15 +444,15 @@
         elif data.dtype == "float64":
             if not data.isnull().all() and all(pd.isnull(v) or float(v).is_integer() for v in data):
                 data_type = DataType.INTEGER
             else:
                 data_type = DataType.DOUBLE
         elif data.dtype == "float32":
             data_type = DataType.REAL
-        elif data.dtype == "object":
+        elif data.dtype == "object" or pd.api.types.is_string_dtype(data):
             if not data.isnull().all() and all(s is None or isinstance(s, str) for s in data):
                 data_type = DataType.STRING
 
     if data_type is None:
         raise RuntimeError("Unknown data type {} not supported".format(data.dtype))
 
     # And now the logic for selecting the codec
@@ -477,15 +493,15 @@
             if INTERNAL_REAL_MISSING[0] in data:
                 raise ValueError("Cannot encode a float data series with both internal missing values")
             codec_class = ShortReal
         else:
             codec_class = ShortReal2
 
     elif data_type == DataType.STRING:
-        if data.nunique() == 1 and not data.hasnans:
+        if data.nunique() == 1 and len(data.iloc[0]) <= 8 and not data.hasnans:
             codec_class = ConstantString
         elif data.nunique() <= 256:
             codec_class = Int8String
         else:
             assert data.nunique() <= 32767
             codec_class = Int16String
```

### Comparing `pyodc-1.3.0/pyodc/constants.py` & `pyodc-1.4.0/pyodc/constants.py`

 * *Files identical despite different names*

### Comparing `pyodc-1.3.0/pyodc/encoder.py` & `pyodc-1.4.0/pyodc/encoder.py`

 * *Files identical despite different names*

### Comparing `pyodc-1.3.0/pyodc/frame.py` & `pyodc-1.4.0/pyodc/frame.py`

 * *Files 7% similar despite different names*

```diff
@@ -260,26 +260,37 @@
         # Are there any bitfield columns we need to consider?
 
         original_columns = columns
         bitfields = []
 
         if columns is not None:
             final_columns = set()
+            _original_columns = self.column_dict.keys()
+            _original_simple_columns = self.simple_column_dict.keys()
+
             for colname in columns:
-                dotpos = colname.find(".")
-                if dotpos == -1:
+
+                # If the column is already present, then use that one directly.
+                # This ensures that we can handle exploded bitfield columns, and extract bitfields from
+                # existing columns below
+                if colname in _original_columns or colname in _original_simple_columns:
                     final_columns.add(colname)
                 else:
-                    column_name = colname[:dotpos]
-                    sp = colname[dotpos + 1 :].split("@")
-                    bitfield_name = sp[0]
-                    if len(sp) > 1:
-                        column_name += "@" + sp[1]
-                    final_columns.add(column_name)
-                    bitfields.append((bitfield_name, column_name, colname))
+                    # Once in here, we don't check if the column exists. If it doesn't this will show up later
+                    dotpos = colname.find(".")
+                    if dotpos == -1:
+                        final_columns.add(colname)
+                    else:
+                        column_name = colname[:dotpos]
+                        sp = colname[dotpos + 1 :].split("@")
+                        bitfield_name = sp[0]
+                        if len(sp) > 1:
+                            column_name += "@" + sp[1]
+                        final_columns.add(column_name)
+                        bitfields.append((bitfield_name, column_name, colname))
             columns = list(final_columns)
 
         df = self._dataframe_internal(columns)
 
         # If there are any bitfields that need extraction, do it here, and remove any temporarily
         # decoded columns as is possible
 
@@ -334,23 +345,29 @@
 
         output_cols = [[] for _ in range(self._numberOfColumns)]
 
         # Select the correct output columns. Note we allow selection of fully-qualified
         # names, but we also allow selection of short names of the form <name>@<table> (so
         # long as these names are not ambiguous
         output = {}
+        full_matches = set()
         for codec, output_col in zip(column_codecs, output_cols):
             if columns is None or codec.column_name in columns:
                 output[codec.column_name] = output_col
+                full_matches.add(codec.column_name)
             else:
                 splitname = codec.column_name.split("@")
                 if len(splitname) == 2:
                     name, table = splitname
                     if name in columns:
                         if name in output:
+                            # If we have already matched "foo" against "foo", then "foo" matching "foo@bar" is
+                            # a weaker match, not an ambiguity
+                            if name in full_matches:
+                                continue
                             raise KeyError("Ambiguous short column name '{}' requested".format(name))
                         output[name] = output_col
 
         if columns:
             for name in columns:
                 if name not in output:
                     raise KeyError(f"Requested columns '{name}' not found")
```

### Comparing `pyodc-1.3.0/pyodc/reader.py` & `pyodc-1.4.0/pyodc/reader.py`

 * *Files identical despite different names*

### Comparing `pyodc-1.3.0/pyodc/stream.py` & `pyodc-1.4.0/pyodc/stream.py`

 * *Files identical despite different names*

### Comparing `pyodc-1.3.0/pyodc.egg-info/PKG-INFO` & `pyodc-1.4.0/pyodc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodc
-Version: 1.3.0
+Version: 1.4.0
 Summary: A Python interface to odc for encoding/decoding ODB-2 files.
 Home-page: https://github.com/ecmwf/pyodc
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: odc odb
 Classifier: Development Status :: 4 - Beta
@@ -15,14 +15,17 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cffi
+Requires-Dist: findlibs>=0.0.5
+Requires-Dist: pandas
 
 # pyodc
 
 [![PyPI](https://img.shields.io/pypi/v/pyodc)](https://pypi.org/project/pyodc/)
 [![Build Status](https://img.shields.io/github/workflow/status/ecmwf/pyodc/Continuous%20Integration/develop)](https://github.com/ecmwf/pyodc/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/pyodc/badge/?version=latest)](https://pyodc.readthedocs.io/en/latest/?badge=latest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -46,15 +49,15 @@
 ### Optional
 
 * [odc]
 * [pytest]
 * [pandoc]
 * [Jupyter Notebook]
 
-For `codc` to work, `odc` library must be compiled and installed on the system and made available to Python (through the CFFI mechanism) as a shared library. There are multiple ways to make the library visible to CFFI: it can be installed as a system library, the installation prefix can be passed in `odc_DIR` environment variable, or the library directory can be included in `LD_LIBRARY_PATH`.
+For `codc` to work, `odc` library must be compiled and installed on the system and made available to Python (through the CFFI mechanism) as a shared library. There are multiple ways to make the library visible to CFFI: it can be installed as a system library, the installation prefix can be passed in the `odc_DIR` or `ODC_DIR` environment variables, or the library directory can be included in `LD_LIBRARY_PATH`.
 
 ## Installation
 
 ```sh
 pip install --user pyodc
 ```
```

### Comparing `pyodc-1.3.0/setup.py` & `pyodc-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     license="Apache License Version 2.0",
     url="https://github.com/ecmwf/pyodc",
     packages=["pyodc", "codc"],
     package_data={"": ["*.h"]},
     include_package_data=True,
     install_requires=[
         "cffi",
+        "findlibs>=0.0.5",
         "pandas",
     ],
     extras_require={},
     tests_require=[
         "pytest",
         "pytest-cov",
         "pytest-flakes",
```

