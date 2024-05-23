# Comparing `tmp/airgradient-0.4.0.tar.gz` & `tmp/airgradient-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airgradient-0.4.0.tar", max compression
+gzip compressed data, was "airgradient-0.4.1.tar", max compression
```

## Comparing `airgradient-0.4.0.tar` & `airgradient-0.4.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-05-09 07:35:10.138172 airgradient-0.4.0/LICENSE.md
--rw-r--r--   0        0        0     4673 2024-05-09 07:35:10.138172 airgradient-0.4.0/README.md
--rw-r--r--   0        0        0     3857 2024-05-09 07:35:20.690251 airgradient-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      540 2024-05-09 07:35:10.138172 airgradient-0.4.0/src/airgradient/__init__.py
--rw-r--r--   0        0        0     3893 2024-05-09 07:35:10.138172 airgradient-0.4.0/src/airgradient/airgradient.py
--rw-r--r--   0        0        0      214 2024-05-09 07:35:10.138172 airgradient-0.4.0/src/airgradient/exceptions.py
--rw-r--r--   0        0        0     2733 2024-05-09 07:35:10.138172 airgradient-0.4.0/src/airgradient/models.py
--rw-r--r--   0        0        0        0 2024-05-09 07:35:10.138172 airgradient-0.4.0/src/airgradient/py.typed
--rw-r--r--   0        0        0     6007 1970-01-01 00:00:00.000000 airgradient-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-23 07:34:37.146370 airgradient-0.4.1/LICENSE.md
+-rw-r--r--   0        0        0     4673 2024-05-23 07:34:37.146370 airgradient-0.4.1/README.md
+-rw-r--r--   0        0        0     3857 2024-05-23 07:34:51.474289 airgradient-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      540 2024-05-23 07:34:37.150370 airgradient-0.4.1/src/airgradient/__init__.py
+-rw-r--r--   0        0        0     3893 2024-05-23 07:34:37.150370 airgradient-0.4.1/src/airgradient/airgradient.py
+-rw-r--r--   0        0        0      214 2024-05-23 07:34:37.150370 airgradient-0.4.1/src/airgradient/exceptions.py
+-rw-r--r--   0        0        0     2728 2024-05-23 07:34:37.150370 airgradient-0.4.1/src/airgradient/models.py
+-rw-r--r--   0        0        0        0 2024-05-23 07:34:37.150370 airgradient-0.4.1/src/airgradient/py.typed
+-rw-r--r--   0        0        0     6007 1970-01-01 00:00:00.000000 airgradient-0.4.1/PKG-INFO
```

### Comparing `airgradient-0.4.0/LICENSE.md` & `airgradient-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `airgradient-0.4.0/README.md` & `airgradient-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `airgradient-0.4.0/pyproject.toml` & `airgradient-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airgradient"
-version = "0.4.0"
+version = "0.4.1"
 description = "Asynchronous Python client for AirGradient."
 authors = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 maintainers = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/airgradienthq/python-airgradient"
 repository = "https://github.com/airgradienthq/python-airgradient"
@@ -32,21 +32,21 @@
 orjson = ">=3.9.0"
 
 [tool.poetry.group.dev.dependencies]
 codespell = "2.2.6"
 covdefaults = "2.3.0"
 coverage = {version = "7.5.1", extras = ["toml"]}
 mypy = "1.10.0"
-pre-commit = "3.7.0"
+pre-commit = "3.7.1"
 pre-commit-hooks = "4.6.0"
 pylint = "3.1.0"
-pytest = "8.2.0"
+pytest = "8.2.1"
 pytest-asyncio = "0.23.6"
 pytest-cov = "5.0.0"
-ruff = "0.4.3"
+ruff = "0.4.4"
 safety = "3.2.0"
 yamllint = "1.35.1"
 syrupy = "4.6.1"
 aioresponses = "0.7.6"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/airgradienthq/python-airgradient/issues"
```

### Comparing `airgradient-0.4.0/src/airgradient/__init__.py` & `airgradient-0.4.1/src/airgradient/__init__.py`

 * *Files identical despite different names*

### Comparing `airgradient-0.4.0/src/airgradient/airgradient.py` & `airgradient-0.4.1/src/airgradient/airgradient.py`

 * *Files identical despite different names*

### Comparing `airgradient-0.4.0/src/airgradient/models.py` & `airgradient-0.4.1/src/airgradient/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,35 +11,35 @@
 
 @dataclass
 class Measures(DataClassORJSONMixin):
     """Measures model."""
 
     signal_strength: int = field(metadata=field_options(alias="wifi"))
     serial_number: str = field(metadata=field_options(alias="serialno"))
-    boot_time: int = field(metadata=field_options(alias="boot"))
-    firmware_version: str = field(metadata=field_options(alias="firmwareVersion"))
-    model: str = field(metadata=field_options(alias="fwMode"))
+    boot_time: int = field(metadata=field_options(alias="bootCount"))
+    firmware_version: str = field(metadata=field_options(alias="firmware"))
+    model: str = field(metadata=field_options(alias="model"))
     rco2: int | None = None
     pm01: int | None = None
     pm02: int | None = None
     pm10: int | None = None
     total_volatile_organic_component_index: int | None = field(
         default=None, metadata=field_options(alias="tvocIndex")
     )
     raw_total_volatile_organic_component: int | None = field(
-        default=None, metadata=field_options(alias="tvoc_raw")
+        default=None, metadata=field_options(alias="tvocRaw")
     )
     pm003_count: int | None = field(
         default=None, metadata=field_options(alias="pm003Count")
     )
     nitrogen_index: int | None = field(
         default=None, metadata=field_options(alias="noxIndex")
     )
     raw_nitrogen: int | None = field(
-        default=None, metadata=field_options(alias="nox_raw")
+        default=None, metadata=field_options(alias="noxRaw")
     )
     ambient_temperature: float | None = field(
         default=None, metadata=field_options(alias="atmp")
     )
     relative_humidity: float | None = field(
         default=None, metadata=field_options(alias="rhum")
     )
```

### Comparing `airgradient-0.4.0/PKG-INFO` & `airgradient-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airgradient
-Version: 0.4.0
+Version: 0.4.1
 Summary: Asynchronous Python client for AirGradient.
 Home-page: https://github.com/airgradienthq/python-airgradient
 License: MIT
 Keywords: Airgradient,api,async,client
 Author: Joost Lekkerkerker
 Author-email: joostlek@outlook.com
 Maintainer: Joost Lekkerkerker
```

