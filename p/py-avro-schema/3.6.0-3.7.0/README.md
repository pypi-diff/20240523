# Comparing `tmp/py-avro-schema-3.6.0.tar.gz` & `tmp/py_avro_schema-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-avro-schema-3.6.0.tar", last modified: Tue Mar 26 12:16:04 2024, max compression
+gzip compressed data, was "py_avro_schema-3.7.0.tar", last modified: Thu May 23 12:00:48 2024, max compression
```

## Comparing `py-avro-schema-3.6.0.tar` & `py_avro_schema-3.7.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:16:04.515553 py-avro-schema-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:16:04.507553 py-avro-schema-3.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:16:04.507553 py-avro-schema-3.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/.github/workflows/release-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/.github/workflows/test-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/LICENSE_HEADER.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15052 2024-03-26 12:16:04.515553 py-avro-schema-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:16:04.511553 py-avro-schema-3.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/docs/py_avro_schema.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/docs/types.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 12:16:04.515553 py-avro-schema-3.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:16:04.507553 py-avro-schema-3.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:16:04.511553 py-avro-schema-3.6.0/src/py_avro_schema/
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/src/py_avro_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40662 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/src/py_avro_schema/_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/src/py_avro_schema/_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/src/py_avro_schema/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/src/py_avro_schema/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:16:04.515553 py-avro-schema-3.6.0/src/py_avro_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15052 2024-03-26 12:16:04.000000 py-avro-schema-3.6.0/src/py_avro_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-26 12:16:04.000000 py-avro-schema-3.6.0/src/py_avro_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 12:16:04.000000 py-avro-schema-3.6.0/src/py_avro_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-26 12:16:04.000000 py-avro-schema-3.6.0/src/py_avro_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-26 12:16:04.000000 py-avro-schema-3.6.0/src/py_avro_schema.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:16:04.515553 py-avro-schema-3.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/tests/test_avro_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    21362 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/tests/test_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/tests/test_logicals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/tests/test_plain_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/tests/test_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)    16038 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/tests/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/tests/test_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-03-26 12:15:58.000000 py-avro-schema-3.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:00:48.128196 py_avro_schema-3.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:00:48.120196 py_avro_schema-3.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:00:48.120196 py_avro_schema-3.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/.github/workflows/release-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/.github/workflows/test-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/LICENSE_HEADER.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15052 2024-05-23 12:00:48.128196 py_avro_schema-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:00:48.124196 py_avro_schema-3.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/docs/py_avro_schema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/docs/types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 12:00:48.128196 py_avro_schema-3.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:00:48.120196 py_avro_schema-3.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:00:48.124196 py_avro_schema-3.7.0/src/py_avro_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/src/py_avro_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41744 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/src/py_avro_schema/_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/src/py_avro_schema/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/src/py_avro_schema/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/src/py_avro_schema/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:00:48.124196 py_avro_schema-3.7.0/src/py_avro_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15052 2024-05-23 12:00:48.000000 py_avro_schema-3.7.0/src/py_avro_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-23 12:00:48.000000 py_avro_schema-3.7.0/src/py_avro_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 12:00:48.000000 py_avro_schema-3.7.0/src/py_avro_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-23 12:00:48.000000 py_avro_schema-3.7.0/src/py_avro_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 12:00:48.000000 py_avro_schema-3.7.0/src/py_avro_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:00:48.124196 py_avro_schema-3.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/tests/test_avro_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21362 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/tests/test_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/tests/test_logicals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/tests/test_plain_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/tests/test_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16924 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/tests/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/tests/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-23 12:00:43.000000 py_avro_schema-3.7.0/tox.ini
```

### Comparing `py-avro-schema-3.6.0/.flake8` & `py_avro_schema-3.7.0/.flake8`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/.github/workflows/release-package.yml` & `py_avro_schema-3.7.0/.github/workflows/release-package.yml`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/.github/workflows/test-package.yml` & `py_avro_schema-3.7.0/.github/workflows/test-package.yml`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/.gitignore` & `py_avro_schema-3.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/.pre-commit-config.yaml` & `py_avro_schema-3.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/LICENSE` & `py_avro_schema-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/LICENSE_HEADER.txt` & `py_avro_schema-3.7.0/LICENSE_HEADER.txt`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/PKG-INFO` & `py_avro_schema-3.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-avro-schema
-Version: 3.6.0
+Version: 3.7.0
 Summary: Generate Apache Avro schemas for Python types including standard library data-classes and Pydantic data models.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `py-avro-schema-3.6.0/README.md` & `py_avro_schema-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/docs/conf.py` & `py_avro_schema-3.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/docs/index.rst` & `py_avro_schema-3.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/docs/tutorial.rst` & `py_avro_schema-3.7.0/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/docs/types.rst` & `py_avro_schema-3.7.0/docs/types.rst`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/pyproject.toml` & `py_avro_schema-3.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/src/py_avro_schema/__init__.py` & `py_avro_schema-3.7.0/src/py_avro_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/src/py_avro_schema/_schemas.py` & `py_avro_schema-3.7.0/src/py_avro_schema/_schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import abc
 import collections.abc
 import dataclasses
 import datetime
 import decimal
 import enum
 import inspect
+import re
 import sys
 import types
 import uuid
 from typing import (
     TYPE_CHECKING,
     Annotated,
     Any,
@@ -104,16 +105,22 @@
 
     #: Automatically populate namespaces using full (dotted) module names instead of top-level package names.
     AUTO_NAMESPACE_MODULE = enum.auto()
 
     #: Do not populate ``doc`` schema attributes based on Python docstrings
     NO_DOC = enum.auto()
 
-    #: Use the alias specified in a classes ``Field`` instead of the field's name.
-    #: This currently only affects Pydantic Models
+    #: Use an alias specified as part of a class instead of the class name itself.
+    #: This currently affects Pydantic models only.
+    #: See https://docs.pydantic.dev/dev/api/config/#pydantic.config.ConfigDict.title
+    USE_CLASS_ALIAS = enum.auto()
+
+    #: Use the alias specified in a class field instead of the field/attribute name itself.
+    #: This currently affects Pydantic models only.
+    #: See https://docs.pydantic.dev/dev/api/fields/#pydantic.fields.Field
     USE_FIELD_ALIAS = enum.auto()
 
 
 JSON_OPTIONS = [opt for opt in Option if opt.name and opt.name.startswith("JSON_")]
 
 
 def schema(
@@ -158,14 +165,25 @@
         # Find the first schema class that handles py_type
         schema_obj = schema_class(py_type, namespace=namespace, options=options)  # type: ignore
         if schema_obj:
             return schema_obj
     raise TypeNotSupportedError(f"Cannot generate Avro schema for Python type {py_type}")
 
 
+# See https://avro.apache.org/docs/1.11.1/specification/#names
+_AVRO_NAME_PATTERN = re.compile(r"^[A-Za-z]([A-Za-z0-9_])*$")
+
+
+def validate_name(value: str) -> str:
+    """Validate (and return) whether a given string is a valid Avro name"""
+    if not re.match(_AVRO_NAME_PATTERN, value):
+        raise ValueError(f"'{value}' is not a valid Avro name")
+    return value
+
+
 class Schema(abc.ABC):
     """Schema base"""
 
     def __new__(cls, py_type: Type, namespace: Optional[str] = None, options: Option = Option(0)):
         """
         Create an instance of this schema class if it handles py_type
 
@@ -687,14 +705,24 @@
         self.name = py_type.__name__
 
     def __str__(self):
         """Human rendering of the schema"""
         return self.fullname
 
     @property
+    def name(self):
+        """Return the schema name"""
+        return self._name
+
+    @name.setter
+    def name(self, value: str):
+        """Validate and set the schema name"""
+        self._name = validate_name(value)
+
+    @property
     def fullname(self):
         """The schema's full name including the namespace if set"""
         if self.namespace:
             return ".".join((self.namespace, self.name))
         else:
             return self.name
 
@@ -893,14 +921,16 @@
         An Avro record schema for a given Pydantic model class
 
         :param py_type:   The Python class to generate a schema for.
         :param namespace: The Avro namespace to add to schemas.
         :param options:   Schema generation options.
         """
         super().__init__(py_type, namespace=namespace, options=options)
+        if Option.USE_CLASS_ALIAS in self.options:
+            self.name = py_type.model_config.get("title") or self.name
         self.py_fields = py_type.model_fields
         self.record_fields = [self._record_field(name, field) for name, field in self.py_fields.items()]
 
     def _record_field(self, name: str, py_field: pydantic.fields.FieldInfo) -> RecordField:
         """Return an Avro record field object for a given Pydantic model field"""
         default = dataclasses.MISSING if py_field.is_required() else py_field.get_default(call_default_factory=True)
         py_type = self._annotation(name)
```

### Comparing `py-avro-schema-3.6.0/src/py_avro_schema/_testing.py` & `py_avro_schema-3.7.0/src/py_avro_schema/_testing.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/src/py_avro_schema/_typing.py` & `py_avro_schema-3.7.0/src/py_avro_schema/_typing.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/src/py_avro_schema.egg-info/PKG-INFO` & `py_avro_schema-3.7.0/src/py_avro_schema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-avro-schema
-Version: 3.6.0
+Version: 3.7.0
 Summary: Generate Apache Avro schemas for Python types including standard library data-classes and Pydantic data models.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `py-avro-schema-3.6.0/src/py_avro_schema.egg-info/SOURCES.txt` & `py_avro_schema-3.7.0/src/py_avro_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/tests/test_avro_schema.py` & `py_avro_schema-3.7.0/tests/test_avro_schema.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/tests/test_dataclass.py` & `py_avro_schema-3.7.0/tests/test_dataclass.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/tests/test_logicals.py` & `py_avro_schema-3.7.0/tests/test_logicals.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/tests/test_plain_class.py` & `py_avro_schema-3.7.0/tests/test_plain_class.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/tests/test_primitives.py` & `py_avro_schema-3.7.0/tests/test_primitives.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/tests/test_pydantic.py` & `py_avro_schema-3.7.0/tests/test_pydantic.py`

 * *Files 5% similar despite different names*

```diff
@@ -422,29 +422,61 @@
     assert_schema(PyType, expected, options=pas.Option.USE_FIELD_ALIAS)
 
 
 def test_field_alias_generator():
     class PyType(pydantic.BaseModel):
         field_a: str
 
-        model_config = {"alias_generator": lambda x: x.upper()}
+        model_config = pydantic.ConfigDict(alias_generator=lambda x: x.upper())
 
     expected = {
         "type": "record",
         "name": "PyType",
         "fields": [
             {
                 "name": "FIELD_A",
                 "type": "string",
             }
         ],
     }
     assert_schema(PyType, expected, options=pas.Option.USE_FIELD_ALIAS)
 
 
+def test_class_title():
+    class PyType(pydantic.BaseModel):
+        model_config = pydantic.ConfigDict(title="PyTitle")
+
+    expected = {
+        "type": "record",
+        "name": "PyTitle",
+        "fields": [],
+    }
+    assert_schema(PyType, expected, options=pas.Option.USE_CLASS_ALIAS)
+
+
+def test_class_title_not_set():
+    class PyType(pydantic.BaseModel):
+        model_config = pydantic.ConfigDict()
+
+    expected = {
+        "type": "record",
+        "name": "PyType",
+        "fields": [],
+    }
+    assert_schema(PyType, expected, options=pas.Option.USE_CLASS_ALIAS)
+
+
+def test_class_title_with_space():
+    class PyType(pydantic.BaseModel):
+        model_config = pydantic.ConfigDict(title="Py Title")
+
+    with pytest.raises(ValueError, match="'Py Title' is not a valid Avro name"):
+        assert_schema(PyType, {}, options=pas.Option.USE_CLASS_ALIAS)
+
+
 def test_annotated_decimal():
     class PyType(pydantic.BaseModel):
         field_a: Annotated[
             decimal.Decimal, pas.DecimalMeta(precision=3, scale=2), pydantic.BeforeValidator(lambda x: x)
         ]
 
     expected = {
```

### Comparing `py-avro-schema-3.6.0/tests/test_typing.py` & `py_avro_schema-3.7.0/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-3.6.0/tox.ini` & `py_avro_schema-3.7.0/tox.ini`

 * *Files identical despite different names*

