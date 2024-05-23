# Comparing `tmp/exchange_calendars_extensions_api-0.4.0.tar.gz` & `tmp/exchange_calendars_extensions_api-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchange_calendars_extensions_api-0.4.0.tar", max compression
+gzip compressed data, was "exchange_calendars_extensions_api-0.4.1.tar", max compression
```

## Comparing `exchange_calendars_extensions_api-0.4.0.tar` & `exchange_calendars_extensions_api-0.4.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-05-08 14:21:37.825068 exchange_calendars_extensions_api-0.4.0/LICENSE
--rw-r--r--   0        0        0      761 2024-05-08 14:21:37.825068 exchange_calendars_extensions_api-0.4.0/README.md
--rw-r--r--   0        0        0      530 2024-05-08 14:21:37.825068 exchange_calendars_extensions_api-0.4.0/exchange_calendars_extensions/api/__init__.py
--rw-r--r--   0        0        0    17849 2024-05-08 14:21:37.825068 exchange_calendars_extensions_api-0.4.0/exchange_calendars_extensions/api/changes.py
--rw-r--r--   0        0        0       18 2024-05-08 14:21:50.113000 exchange_calendars_extensions_api-0.4.0/exchange_calendars_extensions/api/version.py
--rw-r--r--   0        0        0     2719 2024-05-08 14:21:50.049000 exchange_calendars_extensions_api-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 exchange_calendars_extensions_api-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-23 14:23:50.295657 exchange_calendars_extensions_api-0.4.1/LICENSE
+-rw-r--r--   0        0        0      761 2024-05-23 14:23:50.295657 exchange_calendars_extensions_api-0.4.1/README.md
+-rw-r--r--   0        0        0      530 2024-05-23 14:23:50.295657 exchange_calendars_extensions_api-0.4.1/exchange_calendars_extensions/api/__init__.py
+-rw-r--r--   0        0        0    18798 2024-05-23 14:23:50.295657 exchange_calendars_extensions_api-0.4.1/exchange_calendars_extensions/api/changes.py
+-rw-r--r--   0        0        0       18 2024-05-23 14:24:01.583822 exchange_calendars_extensions_api-0.4.1/exchange_calendars_extensions/api/version.py
+-rw-r--r--   0        0        0     2719 2024-05-23 14:24:01.515821 exchange_calendars_extensions_api-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 exchange_calendars_extensions_api-0.4.1/PKG-INFO
```

### Comparing `exchange_calendars_extensions_api-0.4.0/LICENSE` & `exchange_calendars_extensions_api-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions_api-0.4.0/README.md` & `exchange_calendars_extensions_api-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions_api-0.4.0/exchange_calendars_extensions/api/__init__.py` & `exchange_calendars_extensions_api-0.4.1/exchange_calendars_extensions/api/__init__.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions_api-0.4.0/exchange_calendars_extensions/api/changes.py` & `exchange_calendars_extensions_api-0.4.1/exchange_calendars_extensions/api/changes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 import datetime as dt
 import functools
 from collections import OrderedDict
 from enum import Enum, unique
 from typing import Union, Annotated, Callable
 
 import pandas as pd
-from pydantic import BaseModel, Field, RootModel, model_validator, validate_call
-from pydantic.functional_validators import BeforeValidator, AfterValidator
+from pydantic import (
+    BaseModel,
+    Field,
+    RootModel,
+    model_validator,
+    validate_call,
+    WithJsonSchema,
+    BeforeValidator,
+    AfterValidator,
+)
 from typing_extensions import (
     Literal,
     Any,
     Self,
     Concatenate,
     ParamSpec,
     TypeVar,
@@ -96,42 +104,56 @@
     """
 
     # Remove timezone information and normalize to midnight.
     return value.tz_localize(None).normalize()
 
 
 # A type alias for pd.Timestamp that allows initialisation from suitably formatted string values.
-TimestampLike = Annotated[pd.Timestamp, BeforeValidator(_to_timestamp)]
+TimestampLike = Annotated[
+    pd.Timestamp,
+    BeforeValidator(_to_timestamp),
+    WithJsonSchema({"type": "string", "format": "date-time"}),
+    Field(examples=["2020-01-01T00:00:00Z"]),
+]
 
 # A type alias for TimestampLike that normalizes the timestamp to a date-like value.
 #
 # Date-like means that the timestamp is timezone-naive and normalized to the date boundary, i.e. midnight of the day it
 # represents. If the input converts to a valid pd.Timestamp, any timezone information, if present, is discarded. If the
 # result is not aligned with a date boundary, it is normalized to midnight of the same day.
-DateLike = Annotated[TimestampLike, AfterValidator(_to_date)]
+DateLike = Annotated[
+    TimestampLike,
+    AfterValidator(_to_date),
+    WithJsonSchema({"type": "string", "format": "date"}),
+    Field(examples=["2020-01-01"]),
+]
 
 
 class AbstractDayProps(
     BaseModel, arbitrary_types_allowed=True, validate_assignment=True, extra="forbid"
 ):
     """
     Abstract base class for special day properties.
     """
 
-    name: str  # The name of the day.
+    name: str = Field(
+        examples=["Holiday", "Ad-hoc Holiday", "Special Close Day", "Special Open Day"]
+    )  # The name of the day.
 
 
 class DayProps(AbstractDayProps):
     """
     Vanilla special day specification.
     """
 
-    type: Literal[
-        DayType.HOLIDAY, DayType.MONTHLY_EXPIRY, DayType.QUARTERLY_EXPIRY
-    ]  # The type of the special day.
+    type: Literal[DayType.HOLIDAY, DayType.MONTHLY_EXPIRY, DayType.QUARTERLY_EXPIRY] = (
+        Field(
+            examples=[DayType.HOLIDAY, DayType.MONTHLY_EXPIRY, DayType.QUARTERLY_EXPIRY]
+        )
+    )  # The type of the special day.
 
     def __str__(self):
         return f'{{type={self.type.name}, name="{self.name}"}}'
 
 
 def _to_time(value: Union[dt.time, str]):
     """
@@ -164,15 +186,20 @@
         if not isinstance(value, dt.time):
             raise ValueError(f"Failed to convert {value} to {dt.time}.")
 
     return value
 
 
 # A type alias for dt.time that allows initialisation from suitably formatted string values.
-TimeLike = Annotated[dt.time, BeforeValidator(_to_time)]
+TimeLike = Annotated[
+    dt.time,
+    BeforeValidator(_to_time),
+    WithJsonSchema({"type": "string", "format": "time"}),
+    Field(examples=["09:00", "16:30"]),
+]
 
 
 class DayPropsWithTime(AbstractDayProps):
     """
     Special day specification that requires a (open/close) time.
     """
 
@@ -184,29 +211,32 @@
     def __str__(self):
         return f'{{type={self.type.name}, name="{self.name}", time={self.time}}}'
 
 
 # Type alias for valid day properties.
 DayPropsLike = Annotated[Union[DayProps, DayPropsWithTime], Field(discriminator="type")]
 
-Tags = Union[list[str], Union[tuple[str], Union[set[str], None]]]
+Tags = Annotated[
+    Union[list[str], Union[tuple[str], Union[set[str], None]]],
+    Field(examples=[["tag1", "tag2"]]),
+]
 
 
 class DayMeta(
     BaseModel, arbitrary_types_allowed=True, validate_assignment=True, extra="forbid"
 ):
     """
     Metadata for a single date.
     """
 
     # Collection of tags.
     tags: Tags = []
 
     # Free-form comment.
-    comment: Union[str, None] = None
+    comment: Union[str, None] = Field(default=None, examples=["This is a comment."])
 
     @model_validator(mode="after")
     def _canonicalize(self) -> "DayMeta":
         # Sort tags alphabetically and remove duplicates.
         self.__dict__["tags"] = sorted(set(self.tags or []))
 
         # Strip comment of whitespace and set to None if empty.
@@ -292,17 +322,25 @@
     special opens) as a day to remove. Now, if the changeset is applied to the original calendar, 2020-01-01 will no
     longer be a holiday and therefore no longer conflict with the new special open day. This form of sanitization
     ensures that a consistent changeset can be applied safely to any exchange calendar. Effectively, normalization
     ensures that adding a new day for a given day type becomes an upsert operation, i.e. the day is added if it does not
     already exist in any day type category, and updated/moved to the new day type if it does.
     """
 
-    add: dict[DateLike, DayPropsLike] = Field(default_factory=dict)
-    remove: list[DateLike] = Field(default_factory=list)
-    meta: dict[DateLike, DayMeta] = Field(default_factory=dict)
+    add: dict[DateLike, DayPropsLike] = Field(
+        default_factory=dict,
+        examples=[{"2020-01-01": {"type": "holiday", "name": "New Year's Day"}}],
+    )
+    remove: list[DateLike] = Field(default_factory=list, examples=["2020-01-01"])
+    meta: dict[DateLike, DayMeta] = Field(
+        default_factory=dict,
+        examples=[
+            {"2020-01-01": {"tags": ["tag1", "tag2"], "comment": "This is a comment."}}
+        ],
+    )
 
     @model_validator(mode="after")
     def _canonicalize(self) -> "ChangeSet":
         # Sort days to add by date.
         add = OrderedDict(sorted(self.add.items(), key=lambda i: i[0]))
 
         # Sort days to remove by date and remove duplicates.
@@ -548,15 +586,15 @@
 
         # Return as sorted tuple.
         return tuple(sorted(dates))
 
 
 # A type alias for a dictionary of changesets, mapping exchange key to a corresponding change set.
 class ChangeSetDict(RootModel):
-    root: dict[str, ChangeSet]
+    root: dict[str, ChangeSet] = Field(default_factory=dict)
 
     # Delegate all dictionary-typical methods to the root dictionary.
     def __getitem__(self, key):
         return self.root[key]
 
     def __setitem__(self, key, value):
         self.root[key] = value
```

### Comparing `exchange_calendars_extensions_api-0.4.0/pyproject.toml` & `exchange_calendars_extensions_api-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "exchange-calendars-extensions-api"
-version = "0.4.0"
+version = "0.4.1"
 description = "A package that defines parts of the API of the exchange-calendars-extensions package."
 license = "Apache-2.0"
 authors = ["Jens Keiner <jens.keiner@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jenskeiner/exchange_calendars_extensions_api/"
 repository = "https://github.com/jenskeiner/exchange_calendars_extensions_api/"
 documentation = "https://github.com/jenskeiner/exchange_calendars_extensions_api/tree/main/docs/"
```

### Comparing `exchange_calendars_extensions_api-0.4.0/PKG-INFO` & `exchange_calendars_extensions_api-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchange-calendars-extensions-api
-Version: 0.4.0
+Version: 0.4.1
 Summary: A package that defines parts of the API of the exchange-calendars-extensions package.
 Home-page: https://github.com/jenskeiner/exchange_calendars_extensions_api/
 License: Apache-2.0
 Keywords: keywords...
 Author: Jens Keiner
 Author-email: jens.keiner@gmail.com
 Requires-Python: >=3.9,<4.0
```

