# Comparing `tmp/django_custom_jsonfield-1.2.tar.gz` & `tmp/django_custom_jsonfield-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_custom_jsonfield-1.2.tar", last modified: Mon May 20 15:29:24 2024, max compression
+gzip compressed data, was "django_custom_jsonfield-1.3.tar", last modified: Thu May 23 18:34:40 2024, max compression
```

## Comparing `django_custom_jsonfield-1.2.tar` & `django_custom_jsonfield-1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:29:24.184542 django_custom_jsonfield-1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:29:24.176542 django_custom_jsonfield-1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:29:24.180542 django_custom_jsonfield-1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-20 15:29:15.000000 django_custom_jsonfield-1.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-20 15:29:15.000000 django_custom_jsonfield-1.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-20 15:29:15.000000 django_custom_jsonfield-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-20 15:29:24.184542 django_custom_jsonfield-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-20 15:29:15.000000 django_custom_jsonfield-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:29:24.180542 django_custom_jsonfield-1.2/django_custom_jsonfield/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 15:29:15.000000 django_custom_jsonfield-1.2/django_custom_jsonfield/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-20 15:29:15.000000 django_custom_jsonfield-1.2/django_custom_jsonfield/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:29:24.184542 django_custom_jsonfield-1.2/django_custom_jsonfield/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-20 15:29:15.000000 django_custom_jsonfield-1.2/django_custom_jsonfield/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-20 15:29:15.000000 django_custom_jsonfield-1.2/django_custom_jsonfield/rest_framework/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-20 15:29:15.000000 django_custom_jsonfield-1.2/django_custom_jsonfield/rest_framework/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:29:24.184542 django_custom_jsonfield-1.2/django_custom_jsonfield.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-20 15:29:24.000000 django_custom_jsonfield-1.2/django_custom_jsonfield.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-20 15:29:24.000000 django_custom_jsonfield-1.2/django_custom_jsonfield.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:29:24.000000 django_custom_jsonfield-1.2/django_custom_jsonfield.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:29:23.000000 django_custom_jsonfield-1.2/django_custom_jsonfield.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-20 15:29:24.000000 django_custom_jsonfield-1.2/django_custom_jsonfield.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-20 15:29:24.000000 django_custom_jsonfield-1.2/django_custom_jsonfield.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-20 15:29:15.000000 django_custom_jsonfield-1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-20 15:29:15.000000 django_custom_jsonfield-1.2/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-20 15:29:15.000000 django_custom_jsonfield-1.2/runtests.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 15:29:24.184542 django_custom_jsonfield-1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:29:24.184542 django_custom_jsonfield-1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:29:15.000000 django_custom_jsonfield-1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-20 15:29:15.000000 django_custom_jsonfield-1.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-20 15:29:15.000000 django_custom_jsonfield-1.2/tests/test_model_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-20 15:29:15.000000 django_custom_jsonfield-1.2/tests/test_openapi_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-20 15:29:15.000000 django_custom_jsonfield-1.2/tests/test_serializer_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-20 15:29:15.000000 django_custom_jsonfield-1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:34:40.079950 django_custom_jsonfield-1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:34:40.071950 django_custom_jsonfield-1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:34:40.075950 django_custom_jsonfield-1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-23 18:34:35.000000 django_custom_jsonfield-1.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-23 18:34:35.000000 django_custom_jsonfield-1.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-23 18:34:35.000000 django_custom_jsonfield-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-23 18:34:40.079950 django_custom_jsonfield-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-23 18:34:35.000000 django_custom_jsonfield-1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:34:40.075950 django_custom_jsonfield-1.3/django_custom_jsonfield/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-23 18:34:35.000000 django_custom_jsonfield-1.3/django_custom_jsonfield/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-23 18:34:35.000000 django_custom_jsonfield-1.3/django_custom_jsonfield/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:34:40.075950 django_custom_jsonfield-1.3/django_custom_jsonfield/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-23 18:34:35.000000 django_custom_jsonfield-1.3/django_custom_jsonfield/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-23 18:34:35.000000 django_custom_jsonfield-1.3/django_custom_jsonfield/rest_framework/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-23 18:34:35.000000 django_custom_jsonfield-1.3/django_custom_jsonfield/rest_framework/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:34:40.075950 django_custom_jsonfield-1.3/django_custom_jsonfield.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-23 18:34:40.000000 django_custom_jsonfield-1.3/django_custom_jsonfield.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-23 18:34:40.000000 django_custom_jsonfield-1.3/django_custom_jsonfield.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:34:40.000000 django_custom_jsonfield-1.3/django_custom_jsonfield.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:34:39.000000 django_custom_jsonfield-1.3/django_custom_jsonfield.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-23 18:34:40.000000 django_custom_jsonfield-1.3/django_custom_jsonfield.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 18:34:40.000000 django_custom_jsonfield-1.3/django_custom_jsonfield.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-23 18:34:35.000000 django_custom_jsonfield-1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 18:34:35.000000 django_custom_jsonfield-1.3/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-23 18:34:35.000000 django_custom_jsonfield-1.3/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:34:40.079950 django_custom_jsonfield-1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:34:40.075950 django_custom_jsonfield-1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:34:35.000000 django_custom_jsonfield-1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-23 18:34:35.000000 django_custom_jsonfield-1.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-23 18:34:35.000000 django_custom_jsonfield-1.3/tests/test_model_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-23 18:34:35.000000 django_custom_jsonfield-1.3/tests/test_openapi_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-23 18:34:35.000000 django_custom_jsonfield-1.3/tests/test_serializer_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-23 18:34:35.000000 django_custom_jsonfield-1.3/tox.ini
```

### Comparing `django_custom_jsonfield-1.2/.github/workflows/publish.yml` & `django_custom_jsonfield-1.3/.github/workflows/publish.yml`

 * *Files 12% similar despite different names*

```diff
@@ -8,16 +8,14 @@
   contents: read
   id-token: write
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
-    - name: Clean Workspace
-      uses: AutoModality/action-clean@v1.1.0
     - uses: actions/checkout@v4
     - name: Set up Python
       uses: actions/setup-python@v3
       with:
         python-version: '3.10'
     - name: Install dependencies
       run: |
```

### Comparing `django_custom_jsonfield-1.2/.github/workflows/test.yml` & `django_custom_jsonfield-1.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django_custom_jsonfield-1.2/LICENSE` & `django_custom_jsonfield-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_custom_jsonfield-1.2/PKG-INFO` & `django_custom_jsonfield-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django_custom_jsonfield
-Version: 1.2
-Summary: Custom
+Version: 1.3
+Summary: An extended JSON field for Django and DRF with validation support using jsonschema.
 License: MIT
 Project-URL: Homepage, https://github.com/AlexPetul/django_custom_jsonfield
 Project-URL: Code, https://github.com/AlexPetul/django_custom_jsonfield
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `django_custom_jsonfield-1.2/README.md` & `django_custom_jsonfield-1.3/README.md`

 * *Files identical despite different names*

### Comparing `django_custom_jsonfield-1.2/django_custom_jsonfield/fields.py` & `django_custom_jsonfield-1.3/django_custom_jsonfield/fields.py`

 * *Files identical despite different names*

### Comparing `django_custom_jsonfield-1.2/django_custom_jsonfield/rest_framework/openapi.py` & `django_custom_jsonfield-1.3/django_custom_jsonfield/rest_framework/openapi.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,23 +35,25 @@
             "string": OpenApiTypes.STR,
             "number": OpenApiTypes.NUMBER,
             "integer": OpenApiTypes.INT,
             "boolean": OpenApiTypes.BOOL,
             "null": OpenApiTypes.NONE,
         }
 
-        schema_type = schema["type"]
-        if schema_type not in basic_type_mapping:
-            raise KeyError(f"Unknown schema type: {schema_type}")
-
-        return build_basic_type(basic_type_mapping[schema_type])
+        return build_basic_type(basic_type_mapping[schema["type"]])
 
     def map_serializer_field(self, auto_schema, direction):
         schema = self.target.schema
 
+        if "const" in schema:
+            if schema["const"] is None:
+                return None
+
+            return {"enum": [schema["const"]]}
+
         try:
             if schema["type"] == "object":
                 return self.build_object_schema(schema)
             elif schema["type"] == "array":
                 return self.build_array_schema(schema)
             else:
                 return self.build_basic_schema(schema)
```

### Comparing `django_custom_jsonfield-1.2/django_custom_jsonfield/rest_framework/serializers.py` & `django_custom_jsonfield-1.3/django_custom_jsonfield/rest_framework/serializers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import jsonschema
 from django.utils.translation import gettext_lazy as _
+from jsonschema import validators
 from rest_framework import serializers
 
 
 class CustomJSONField(serializers.JSONField):
     default_error_messages = {
         "invalid_data": _("Value does not match the JSON schema."),
+        "invalid_schema": _("Invalid JSON schema."),
     }
 
     def __init__(self, schema: dict, **kwargs):
         self.schema = schema
         super().__init__(**kwargs)
+
+        validator = validators.validator_for(self.schema)
+        try:
+            validator.check_schema(self.schema)
+        except jsonschema.exceptions.SchemaError:
+            self.fail("invalid_schema")
+
         self.validators.append(self._validate_data)
 
     def _validate_data(self, value):
         """Validate value against JSON schema."""
         try:
             jsonschema.validate(value, self.schema)
         except jsonschema.exceptions.ValidationError:
-            raise serializers.ValidationError(
-                self.error_messages["invalid_data"],
-                code="invalid_data",
-            )
+            self.fail("invalid_data")
```

### Comparing `django_custom_jsonfield-1.2/django_custom_jsonfield.egg-info/PKG-INFO` & `django_custom_jsonfield-1.3/django_custom_jsonfield.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django_custom_jsonfield
-Version: 1.2
-Summary: Custom
+Version: 1.3
+Summary: An extended JSON field for Django and DRF with validation support using jsonschema.
 License: MIT
 Project-URL: Homepage, https://github.com/AlexPetul/django_custom_jsonfield
 Project-URL: Code, https://github.com/AlexPetul/django_custom_jsonfield
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `django_custom_jsonfield-1.2/django_custom_jsonfield.egg-info/SOURCES.txt` & `django_custom_jsonfield-1.3/django_custom_jsonfield.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_custom_jsonfield-1.2/pyproject.toml` & `django_custom_jsonfield-1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools>=61", "wheel", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django_custom_jsonfield"
 license = {text = "MIT"}
-description = "Custom"
+description = "An extended JSON field for Django and DRF with validation support using jsonschema."
 requires-python = ">=3.8"
-version = "1.2"
+version = "1.3"
 dependencies = [
     "django>=4.0,<5.1",
     "jsonschema>=4.0,<5",
 ]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -71,8 +71,8 @@
 branch = true
 
 [tool.coverage.report]
 precision = 2
 exclude_lines = [
     "pragma: no cover",
     "raise NotImplementedError",
-]
+]
```

### Comparing `django_custom_jsonfield-1.2/tests/test_model_field.py` & `django_custom_jsonfield-1.3/tests/test_model_field.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     [
         {"minItems": "1"},
         {"properties": 1},
         {"pattern": "*invalid.regex"},
     ],
 )
 def test_json_schema_invalid(schema: dict):
+    """Test Django returns errors if JSON schema is invalid."""
+
     class FakeModel(models.Model):
         json_field = CustomJSONField(schema=schema)
 
         class Meta:
             app_label = "test_app"
 
     instance = FakeModel()
@@ -48,23 +50,24 @@
             },
         )
 
         class Meta:
             app_label = "test_app"
 
     instance = FakeModel()
-
     assert instance.check() == []
 
 
 @pytest.mark.parametrize(
     "schema",
     [10, 10.00, list(), tuple(), set(), "", b"", True, None],
 )
 def test_schema_type_invalid(schema: Any):
+    """Test Django raises exception if JSON schema is not typed correctly."""
+
     with pytest.raises(ValueError) as e:
         CustomJSONField(schema=schema)
 
     assert e.value.args[0] == "The schema parameter must be a dictionary."
 
 
 @pytest.mark.parametrize(
@@ -74,17 +77,25 @@
             {"name": "John"},
             {
                 "type": "object",
                 "properties": {"name": {"type": "string"}, "age": {"type": "integer"}},
                 "required": ["name", "age"],
             },
         ),
+        (
+            "invalid_string",
+            {
+                "const": "custom_string",
+            },
+        ),
     ],
 )
-def test_validate_value_against_schema(value, schema):
+def test_validate_value_against_schema(value: Any, schema: Any):
+    """Test Django raises exception if value doesn't match JSON schema."""
+
     class FakeModel(models.Model):
         json_field = CustomJSONField(schema=schema)
 
         class Meta:
             app_label = "test_app"
 
     instance = FakeModel()
```

### Comparing `django_custom_jsonfield-1.2/tox.ini` & `django_custom_jsonfield-1.3/tox.ini`

 * *Files identical despite different names*

