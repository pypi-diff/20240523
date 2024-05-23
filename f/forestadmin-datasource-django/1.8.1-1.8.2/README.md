# Comparing `tmp/forestadmin_datasource_django-1.8.1.tar.gz` & `tmp/forestadmin_datasource_django-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_datasource_django-1.8.1.tar", max compression
+gzip compressed data, was "forestadmin_datasource_django-1.8.2.tar", max compression
```

## Comparing `forestadmin_datasource_django-1.8.1.tar` & `forestadmin_datasource_django-1.8.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2024-05-14 13:52:42.014771 forestadmin_datasource_django-1.8.1/README.md
--rw-r--r--   0        0        0        0 2024-05-14 13:52:42.014771 forestadmin_datasource_django-1.8.1/forestadmin/datasource_django/__init__.py
--rw-r--r--   0        0        0     3010 2024-05-14 13:52:42.014771 forestadmin_datasource_django-1.8.1/forestadmin/datasource_django/collection.py
--rw-r--r--   0        0        0      589 2024-05-14 13:52:42.014771 forestadmin_datasource_django-1.8.1/forestadmin/datasource_django/datasource.py
--rw-r--r--   0        0        0      217 2024-05-14 13:52:42.014771 forestadmin_datasource_django-1.8.1/forestadmin/datasource_django/exception.py
--rw-r--r--   0        0        0      365 2024-05-14 13:52:42.014771 forestadmin_datasource_django-1.8.1/forestadmin/datasource_django/interface.py
--rw-r--r--   0        0        0        0 2024-05-14 13:52:42.014771 forestadmin_datasource_django-1.8.1/forestadmin/datasource_django/utils/__init__.py
--rw-r--r--   0        0        0     8327 2024-05-14 13:52:42.014771 forestadmin_datasource_django-1.8.1/forestadmin/datasource_django/utils/model_introspection.py
--rw-r--r--   0        0        0     2177 2024-05-14 13:52:42.014771 forestadmin_datasource_django-1.8.1/forestadmin/datasource_django/utils/native_driver_wrapper.py
--rw-r--r--   0        0        0    14254 2024-05-14 13:52:42.014771 forestadmin_datasource_django-1.8.1/forestadmin/datasource_django/utils/query_factory.py
--rw-r--r--   0        0        0      916 2024-05-14 13:52:42.014771 forestadmin_datasource_django-1.8.1/forestadmin/datasource_django/utils/record_serializer.py
--rw-r--r--   0        0        0     4178 2024-05-14 13:52:42.014771 forestadmin_datasource_django-1.8.1/forestadmin/datasource_django/utils/type_converter.py
--rw-r--r--   0        0        0     1881 2024-05-14 13:52:57.994775 forestadmin_datasource_django-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     1071 1970-01-01 00:00:00.000000 forestadmin_datasource_django-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-23 09:47:35.916587 forestadmin_datasource_django-1.8.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 09:47:35.916587 forestadmin_datasource_django-1.8.2/forestadmin/datasource_django/__init__.py
+-rw-r--r--   0        0        0     3010 2024-05-23 09:47:35.916587 forestadmin_datasource_django-1.8.2/forestadmin/datasource_django/collection.py
+-rw-r--r--   0        0        0      589 2024-05-23 09:47:35.916587 forestadmin_datasource_django-1.8.2/forestadmin/datasource_django/datasource.py
+-rw-r--r--   0        0        0      217 2024-05-23 09:47:35.916587 forestadmin_datasource_django-1.8.2/forestadmin/datasource_django/exception.py
+-rw-r--r--   0        0        0      365 2024-05-23 09:47:35.916587 forestadmin_datasource_django-1.8.2/forestadmin/datasource_django/interface.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:47:35.916587 forestadmin_datasource_django-1.8.2/forestadmin/datasource_django/utils/__init__.py
+-rw-r--r--   0        0        0     8327 2024-05-23 09:47:35.916587 forestadmin_datasource_django-1.8.2/forestadmin/datasource_django/utils/model_introspection.py
+-rw-r--r--   0        0        0     2177 2024-05-23 09:47:35.916587 forestadmin_datasource_django-1.8.2/forestadmin/datasource_django/utils/native_driver_wrapper.py
+-rw-r--r--   0        0        0    14254 2024-05-23 09:47:35.916587 forestadmin_datasource_django-1.8.2/forestadmin/datasource_django/utils/query_factory.py
+-rw-r--r--   0        0        0      916 2024-05-23 09:47:35.916587 forestadmin_datasource_django-1.8.2/forestadmin/datasource_django/utils/record_serializer.py
+-rw-r--r--   0        0        0     4486 2024-05-23 09:47:35.916587 forestadmin_datasource_django-1.8.2/forestadmin/datasource_django/utils/type_converter.py
+-rw-r--r--   0        0        0     1860 2024-05-23 09:47:52.564649 forestadmin_datasource_django-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0     1037 1970-01-01 00:00:00.000000 forestadmin_datasource_django-1.8.2/PKG-INFO
```

### Comparing `forestadmin_datasource_django-1.8.1/forestadmin/datasource_django/collection.py` & `forestadmin_datasource_django-1.8.2/forestadmin/datasource_django/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_django-1.8.1/forestadmin/datasource_django/datasource.py` & `forestadmin_datasource_django-1.8.2/forestadmin/datasource_django/datasource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_django-1.8.1/forestadmin/datasource_django/utils/model_introspection.py` & `forestadmin_datasource_django-1.8.2/forestadmin/datasource_django/utils/model_introspection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_django-1.8.1/forestadmin/datasource_django/utils/native_driver_wrapper.py` & `forestadmin_datasource_django-1.8.2/forestadmin/datasource_django/utils/native_driver_wrapper.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_django-1.8.1/forestadmin/datasource_django/utils/query_factory.py` & `forestadmin_datasource_django-1.8.2/forestadmin/datasource_django/utils/query_factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_django-1.8.1/forestadmin/datasource_django/utils/record_serializer.py` & `forestadmin_datasource_django-1.8.2/forestadmin/datasource_django/utils/record_serializer.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_django-1.8.1/forestadmin/datasource_django/utils/type_converter.py` & `forestadmin_datasource_django-1.8.2/forestadmin/datasource_django/utils/type_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,43 @@
 from typing import Dict, Tuple
 
-from django.contrib.postgres import fields as postgres_fields
 from django.db import models
 from forestadmin.datasource_django.exception import DjangoDatasourceException
 from forestadmin.datasource_toolkit.interfaces.fields import ColumnAlias, Operator, PrimitiveType
 from forestadmin.datasource_toolkit.utils.operators import BaseFilterOperator
 
 try:
+    # if postgres driver is installed
+    from django.contrib.postgres import fields as postgres_fields
+except ImportError:
+    postgres_fields = None
+
+try:
     # GeneratedField is available since django 5
     from django.db.models import GeneratedField
-except Exception:
+except ImportError:
     GeneratedField = None
 
 
 class ConverterException(DjangoDatasourceException):
     pass
 
 
+if postgres_fields is not None:
+    POSTGRES_TYPE: Dict[type, PrimitiveType] = {
+        # specific postgres fields
+        postgres_fields.CIText: PrimitiveType.STRING,
+        postgres_fields.CIEmailField: PrimitiveType.STRING,
+        postgres_fields.HStoreField: PrimitiveType.JSON,
+        # postgres_fields.RangeField and subclassed ones not handles
+    }
+else:
+    POSTGRES_TYPE: Dict[type, PrimitiveType] = {}
+
+
 class TypeConverter:
     TYPES: Dict[type, PrimitiveType] = {
         # string
         models.CharField: PrimitiveType.STRING,
         models.TextField: PrimitiveType.STRING,
         #
         # number
@@ -52,19 +69,15 @@
         #
         # json
         models.JSONField: PrimitiveType.JSON,
         #
         # uuid
         models.UUIDField: PrimitiveType.UUID,
         #
-        # specific fields
-        postgres_fields.CIText: PrimitiveType.STRING,
-        postgres_fields.CIEmailField: PrimitiveType.STRING,
-        postgres_fields.HStoreField: PrimitiveType.JSON,
-        # postgres_fields.RangeField and subclassed ones not handles
+        **POSTGRES_TYPE,
     }
 
     @classmethod
     def convert(cls, field: models.Field) -> ColumnAlias:
         if field.choices is not None:
             return PrimitiveType.ENUM
 
@@ -73,15 +86,15 @@
 
         if GeneratedField is not None and isinstance(field, GeneratedField):
             return cls.convert(field.output_field)
 
         if field.__class__ in cls.TYPES:
             return cls.TYPES[field.__class__]
 
-        if isinstance(field, postgres_fields.ArrayField):
+        if postgres_fields is not None and isinstance(field, postgres_fields.ArrayField):
             return [cls.convert(field.base_field)]
 
         for model_type, primitive_type in cls.TYPES.items():
             if isinstance(field, model_type):
                 return primitive_type
 
         raise ConverterException(f'Type "{field.__class__}" is unknown')
```

### Comparing `forestadmin_datasource_django-1.8.1/pyproject.toml` & `forestadmin_datasource_django-1.8.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-datasource-django"
-version = "1.8.1"
+version = "1.8.2"
 description = "django datasource for forestadmin python agent"
 authors = [ "Julien Barreau <julien.barreau@forestadmin.com>",]
 readme = "README.md"
 repository = "https://github.com/ForestAdmin/agent-python"
 documentation = "https://docs.forestadmin.com/developer-guide-agents-python/"
 homepage = "https://www.forestadmin.com"
 [[tool.poetry.packages]]
 include = "forestadmin"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
 typing-extensions = "~=4.2"
 django = ">=3.2,<6.0"
-psycopg2 = ">=2.8.4"
-forestadmin-datasource-toolkit = "1.8.1"
-forestadmin-agent-toolkit = "1.8.1"
+forestadmin-datasource-toolkit = "1.8.2"
+forestadmin-agent-toolkit = "1.8.2"
 
 [tool.pytest.ini_options]
 DJANGO_SETTINGS_MODULE = "test_project_datasource.settings"
 pythonpath = "tests/test_project_datasource"
 
 [tool.poetry.dependencies."backports.zoneinfo"]
 version = "~=0.2.1"
```

### Comparing `forestadmin_datasource_django-1.8.1/PKG-INFO` & `forestadmin_datasource_django-1.8.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: forestadmin-datasource-django
-Version: 1.8.1
+Version: 1.8.2
 Summary: django datasource for forestadmin python agent
 Home-page: https://www.forestadmin.com
 Author: Julien Barreau
 Author-email: julien.barreau@forestadmin.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0) ; python_version < "3.9"
 Requires-Dist: django (>=3.2,<6.0)
-Requires-Dist: forestadmin-agent-toolkit (==1.8.1)
-Requires-Dist: forestadmin-datasource-toolkit (==1.8.1)
-Requires-Dist: psycopg2 (>=2.8.4)
+Requires-Dist: forestadmin-agent-toolkit (==1.8.2)
+Requires-Dist: forestadmin-datasource-toolkit (==1.8.2)
 Requires-Dist: typing-extensions (>=4.2,<5.0)
 Project-URL: Documentation, https://docs.forestadmin.com/developer-guide-agents-python/
 Project-URL: Repository, https://github.com/ForestAdmin/agent-python
 Description-Content-Type: text/markdown
```

