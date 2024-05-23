# Comparing `tmp/unic-0.4.6.tar.gz` & `tmp/unic-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unic-0.4.6.tar", max compression
+gzip compressed data, was "unic-0.4.7.tar", max compression
```

## Comparing `unic-0.4.6.tar` & `unic-0.4.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1064 2023-08-02 13:34:57.957684 unic-0.4.6/LICENSE
--rw-r--r--   0        0        0      888 2024-05-17 15:00:39.830539 unic-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     2398 2024-05-03 12:41:18.395441 unic-0.4.6/README.md
--rw-r--r--   0        0        0      897 2023-12-11 12:31:51.919297 unic-0.4.6/unic/__init__.py
--rw-r--r--   0        0        0      912 2023-12-11 13:01:08.512829 unic-0.4.6/unic/configs/metirc_system/settings.toml
--rw-r--r--   0        0        0      244 2023-08-02 13:34:57.987478 unic-0.4.6/unic/configs/timeunit/settings.toml
--rw-r--r--   0        0        0     2232 2023-08-02 13:34:57.987478 unic-0.4.6/unic/configs/timezone/settings.toml
--rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-0.4.6/unic/length_unit/metric_system/__init__.py
--rw-r--r--   0        0        0      751 2024-05-16 14:57:00.498671 unic-0.4.6/unic/length_unit/metric_system/metric_system_model.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.4.6/unic/length_unit/validators/__init__.py
--rw-r--r--   0        0        0     1279 2024-05-10 14:36:03.640060 unic-0.4.6/unic/length_unit/validators/validators.py
--rw-r--r--   0        0        0        0 2023-08-08 15:37:47.030079 unic-0.4.6/unic/time_unit/datetime/__init__.py
--rw-r--r--   0        0        0     1377 2024-05-16 14:49:57.983327 unic-0.4.6/unic/time_unit/datetime/datetime_model.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-0.4.6/unic/time_unit/time/__init__.py
--rw-r--r--   0        0        0      728 2024-05-16 14:56:54.023059 unic-0.4.6/unic/time_unit/time/time_model.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:58.002017 unic-0.4.6/unic/time_unit/unixtime/__init__.py
--rw-r--r--   0        0        0     1094 2024-05-16 14:56:45.186999 unic-0.4.6/unic/time_unit/unixtime/unixtime_model.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.4.6/unic/time_unit/validators/__init__.py
--rw-r--r--   0        0        0     2557 2024-05-10 14:33:34.102958 unic-0.4.6/unic/time_unit/validators/validators.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.4.6/unic/utils/__init__.py
--rw-r--r--   0        0        0      399 2024-05-14 16:00:12.297440 unic-0.4.6/unic/utils/config_parser.py
--rw-r--r--   0        0        0     3096 1970-01-01 00:00:00.000000 unic-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-02 13:34:57.957684 unic-0.4.7/LICENSE
+-rw-r--r--   0        0        0      888 2024-05-23 15:12:17.186843 unic-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     2398 2024-05-03 12:41:18.395441 unic-0.4.7/README.md
+-rw-r--r--   0        0        0      897 2023-12-11 12:31:51.919297 unic-0.4.7/unic/__init__.py
+-rw-r--r--   0        0        0      912 2023-12-11 13:01:08.512829 unic-0.4.7/unic/configs/metirc_system/settings.toml
+-rw-r--r--   0        0        0      244 2023-08-02 13:34:57.987478 unic-0.4.7/unic/configs/timeunit/settings.toml
+-rw-r--r--   0        0        0     2232 2023-08-02 13:34:57.987478 unic-0.4.7/unic/configs/timezone/settings.toml
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-0.4.7/unic/length_unit/metric_system/__init__.py
+-rw-r--r--   0        0        0      865 2024-05-23 14:56:09.193757 unic-0.4.7/unic/length_unit/metric_system/metric_system_model.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.4.7/unic/length_unit/validators/__init__.py
+-rw-r--r--   0        0        0     1279 2024-05-10 14:36:03.640060 unic-0.4.7/unic/length_unit/validators/validators.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:37:47.030079 unic-0.4.7/unic/time_unit/datetime/__init__.py
+-rw-r--r--   0        0        0     1377 2024-05-16 14:49:57.983327 unic-0.4.7/unic/time_unit/datetime/datetime_model.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-0.4.7/unic/time_unit/time/__init__.py
+-rw-r--r--   0        0        0      834 2024-05-23 14:53:33.455521 unic-0.4.7/unic/time_unit/time/time_model.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:58.002017 unic-0.4.7/unic/time_unit/unixtime/__init__.py
+-rw-r--r--   0        0        0     1303 2024-05-23 14:11:24.862341 unic-0.4.7/unic/time_unit/unixtime/unixtime_model.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.4.7/unic/time_unit/validators/__init__.py
+-rw-r--r--   0        0        0     2795 2024-05-21 15:45:17.999751 unic-0.4.7/unic/time_unit/validators/validators.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.4.7/unic/utils/__init__.py
+-rw-r--r--   0        0        0      399 2024-05-14 16:00:12.297440 unic-0.4.7/unic/utils/config_parser.py
+-rw-r--r--   0        0        0     3096 1970-01-01 00:00:00.000000 unic-0.4.7/PKG-INFO
```

### Comparing `unic-0.4.6/LICENSE` & `unic-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `unic-0.4.6/pyproject.toml` & `unic-0.4.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unic"
-version = "0.4.6"
+version = "0.4.7"
 description = "Python package for converting various units."
 authors = ["Subretu"]
 maintainers = ["Subretu"]
 license = "MIT"
 readme = 'README.md'
 repository = 'https://github.com/subretu/unic'
 keywords = ['unit', 'convert', 'time', 'timestamp', 'length']
@@ -23,12 +23,12 @@
 python = "^3.8"
 pydantic = "^2.1"
 tomli = "^2.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 mypy = "^1.4.1"
-black = "^23.7.0"
+black = "^24.4.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `unic-0.4.6/README.md` & `unic-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `unic-0.4.6/unic/__init__.py` & `unic-0.4.7/unic/__init__.py`

 * *Files identical despite different names*

### Comparing `unic-0.4.6/unic/configs/metirc_system/settings.toml` & `unic-0.4.7/unic/configs/metirc_system/settings.toml`

 * *Files identical despite different names*

### Comparing `unic-0.4.6/unic/configs/timezone/settings.toml` & `unic-0.4.7/unic/configs/timezone/settings.toml`

 * *Files identical despite different names*

### Comparing `unic-0.4.6/unic/length_unit/metric_system/metric_system_model.py` & `unic-0.4.7/unic/length_unit/metric_system/metric_system_model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from pydantic import ValidationError
 from unic.utils import config_parser
 from unic.length_unit.validators import validators
 from fractions import Fraction
 
 
 class MetricSystemModel:
+    def __init__(self):
+        self.metric_system_parameter = config_parser.parse_toml("metirc_system")
+
     def convert(self, data: int, *, from_unit: str, to_unit: str) -> int:
         try:
             input_data = validators.MetricSystemModelValidator(
                 data=data, from_unit=from_unit, to_unit=to_unit
             )
         except ValidationError as e:
             error_messages = "; ".join(err["msg"] for err in e.errors())
             raise ValueError(error_messages)
 
-        parameter = config_parser.parse_toml("metirc_system")
-        data = float(input_data.data * Fraction(parameter[from_unit][to_unit]))
+        parameter = self.metric_system_parameter.get(from_unit, {}).get(to_unit, None)
+        data = float(input_data.data * Fraction(parameter))
 
         return data
```

### Comparing `unic-0.4.6/unic/length_unit/validators/validators.py` & `unic-0.4.7/unic/length_unit/validators/validators.py`

 * *Files identical despite different names*

### Comparing `unic-0.4.6/unic/time_unit/datetime/datetime_model.py` & `unic-0.4.7/unic/time_unit/datetime/datetime_model.py`

 * *Files identical despite different names*

### Comparing `unic-0.4.6/unic/time_unit/validators/validators.py` & `unic-0.4.7/unic/time_unit/validators/validators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 from pydantic import BaseModel, StrictFloat, field_validator, StrictInt, StrictStr
 from typing import Union
 from datetime import datetime
 from unic.utils import config_parser
-import math
+
+
+class TimezoneConfigCache:
+    _timezone_cache = None
+
+    @classmethod
+    def get_valid_timezones(cls):
+        if cls._timezone_cache is None:
+            cls._timezone_cache = config_parser.parse_toml("timezone")
+        return cls._timezone_cache
 
 
 class ValidatorMixin:
     @classmethod
     def validate_units(cls, v, valid_units, parameter):
         if v not in valid_units:
             raise ValueError(
                 f"{v} is invalid value for parameter: {parameter}. Allowed values are {valid_units}."
             )
         return v
 
     @classmethod
     def validate_timezone(cls, v):
-        valid_timezones = config_parser.parse_toml("timezone")
+        valid_timezones = TimezoneConfigCache.get_valid_timezones()
         if v not in valid_timezones.keys() and v is not None:
             raise ValueError(f"{v} is invalid value for parameter: tz.")
         return v
 
 
 class TimeModelValidator(BaseModel, ValidatorMixin):
     data: Union[StrictInt, StrictFloat]
@@ -39,15 +48,15 @@
 class DatetimeModelValidator(BaseModel, ValidatorMixin):
     data: StrictInt
     format: StrictStr
     tz: Union[StrictStr, None]
 
     @field_validator("data")
     def data_check(cls, v):
-        digits = math.floor(math.log10(abs(v))) + 1
+        digits = len(str(abs(v)))
         if digits == 10:
             return v
         if digits == 13:
             return v / 1000
         else:
             raise ValueError("Unixtime digits is 10 or 13.")
```

### Comparing `unic-0.4.6/PKG-INFO` & `unic-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unic
-Version: 0.4.6
+Version: 0.4.7
 Summary: Python package for converting various units.
 Home-page: https://github.com/subretu/unic
 License: MIT
 Keywords: unit,convert,time,timestamp,length
 Author: Subretu
 Maintainer: Subretu
 Requires-Python: >=3.8,<4.0
```

