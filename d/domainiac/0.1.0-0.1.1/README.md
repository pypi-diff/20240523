# Comparing `tmp/domainiac-0.1.0.tar.gz` & `tmp/domainiac-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domainiac-0.1.0.tar", max compression
+gzip compressed data, was "domainiac-0.1.1.tar", max compression
```

## Comparing `domainiac-0.1.0.tar` & `domainiac-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       65 2024-05-17 07:27:52.400529 domainiac-0.1.0/domainiac/__init__.py
--rw-r--r--   0        0        0      174 2024-05-17 07:27:52.400529 domainiac-0.1.0/domainiac/managers/__init__.py
--rw-r--r--   0        0        0     1388 2024-05-17 07:27:52.400529 domainiac-0.1.0/domainiac/managers/masterdata_manager.py
--rw-r--r--   0        0        0      995 2024-05-17 07:27:52.400529 domainiac-0.1.0/domainiac/managers/metering_manager.py
--rw-r--r--   0        0        0     1083 2024-05-17 07:27:52.400529 domainiac-0.1.0/domainiac/managers/plant_manager.py
--rw-r--r--   0        0        0     1085 2024-05-17 07:27:52.400529 domainiac-0.1.0/domainiac/managers/unit_manager.py
--rw-r--r--   0        0        0      685 2024-05-17 07:27:52.400529 domainiac-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      465 1970-01-01 00:00:00.000000 domainiac-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       65 2024-05-23 10:29:07.204609 domainiac-0.1.1/domainiac/__init__.py
+-rw-r--r--   0        0        0      174 2024-05-23 10:29:07.204609 domainiac-0.1.1/domainiac/managers/__init__.py
+-rw-r--r--   0        0        0     1463 2024-05-23 10:29:07.204609 domainiac-0.1.1/domainiac/managers/masterdata_manager.py
+-rw-r--r--   0        0        0      995 2024-05-23 10:29:07.204609 domainiac-0.1.1/domainiac/managers/metering_manager.py
+-rw-r--r--   0        0        0     1823 2024-05-23 10:29:07.204609 domainiac-0.1.1/domainiac/managers/plant_manager.py
+-rw-r--r--   0        0        0     1085 2024-05-23 10:29:07.204609 domainiac-0.1.1/domainiac/managers/unit_manager.py
+-rw-r--r--   0        0        0      685 2024-05-23 10:29:07.204609 domainiac-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      465 1970-01-01 00:00:00.000000 domainiac-0.1.1/PKG-INFO
```

### Comparing `domainiac-0.1.0/domainiac/managers/masterdata_manager.py` & `domainiac-0.1.1/domainiac/managers/masterdata_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,31 +15,38 @@
         resolution: pd.Timedelta,
     ) -> None:
         self.db = db
         self.time_interval = time_interval
         self.resolution = resolution
 
     @typechecked
-    def get_data(
+    def get_operational_entities(
         self,
         table: str,
         filters: dict = {},
-        columns: list = [],
     ) -> pd.DataFrame:
-        """Gets the units for a given unit type.
-        Filters for units valid at the end of time interval.
-        Filters by default for units in operation.
-        """
+        """Gets the operational data for a given table."""
 
         filters["standing_entity_state"] = "InOperation"
         df = self.db.query(table, filters=filters)
 
-        for key in filters.keys():
-            if key not in df.columns:
-                raise KeyError(f"Column {key} not found in {table}")
+        return df
+
+    @typechecked
+    def get_data(
+        self,
+        table: str,
+        filters: dict = {},
+        columns: list = [],
+    ) -> pd.DataFrame:
+        """Gets the data for a given table.
+        Filters for rows valid at the end of time interval.
+        """
+        df = self.get_operational_entities(table, filters)
+
         for column in columns:
             if column not in df.columns:
                 raise KeyError(f"Column {column} not found in {table}")
 
         df = pdz.as_of_time(
             df=df,
             period=("valid_from_date_utc", "valid_to_date_utc"),
```

### Comparing `domainiac-0.1.0/domainiac/managers/metering_manager.py` & `domainiac-0.1.1/domainiac/managers/metering_manager.py`

 * *Files identical despite different names*

### Comparing `domainiac-0.1.0/domainiac/managers/plant_manager.py` & `domainiac-0.1.1/domainiac/managers/unit_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import datamazing.pandas as pdz
 import pandas as pd
 
 from .masterdata_manager import MasterdataManager
 
 
-class PlantManager(MasterdataManager):
+class UnitManager(MasterdataManager):
     """
-    Manager which simplifies the process of getting plants from masterdata.
+    Manager which simplifies the process of getting units from masterdata.
     """
 
     def __init__(
         self,
         db: pdz.Database,
         time_interval: pdz.TimeInterval,
         resolution: pd.Timedelta,
     ) -> None:
         self.db = db
         self.time_interval = time_interval
         self.resolution = resolution
 
-    def get_plants(
+    def get_units(
         self,
         filters: dict = {},
         columns: list = [
-            "plant_id",
             "masterdata_gsrn",
-            "datahub_gsrn_e18",
             "installed_power_MW",
+            "plant_id",
             "price_area",
             "valid_from_date_utc",
             "valid_to_date_utc",
+            "power_system_resource_type",
         ],
     ) -> pd.DataFrame:
-        """Gets the plants for a given plant type.
-        Filters for plants valid at the end of time interval.
-        Filters by default for plants in operation.
+        """Gets the units for a given unit type.
+        Filters for units valid at the end of time interval.
+        Filters by default for units in operation.
         """
-        return self.get_data("masterdataPlant", filters=filters, columns=columns)
+        return self.get_data("masterdataUnit", filters=filters, columns=columns)
```

### Comparing `domainiac-0.1.0/pyproject.toml` & `domainiac-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "domainiac"
-version = "0.1.0"
+version = "0.1.1"
 description = "Package for working with Energinet data, but with specialized functions used for Enigma."
 authors = ["Team Enigma <gridop-enigma@energinet.dk>"]
 packages = [
     { include = "domainiac" },
 ]
 
 [tool.poetry.dependencies]
```

