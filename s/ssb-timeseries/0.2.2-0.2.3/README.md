# Comparing `tmp/ssb_timeseries-0.2.2.tar.gz` & `tmp/ssb_timeseries-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_timeseries-0.2.2.tar", max compression
+gzip compressed data, was "ssb_timeseries-0.2.3.tar", max compression
```

## Comparing `ssb_timeseries-0.2.2.tar` & `ssb_timeseries-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1073 2024-05-14 10:57:41.047234 ssb_timeseries-0.2.2/LICENSE
--rw-r--r--   0        0        0    10072 2024-05-14 10:57:41.047234 ssb_timeseries-0.2.2/README.md
--rw-r--r--   0        0        0     4508 2024-05-14 10:57:51.599631 ssb_timeseries-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      452 2024-05-14 10:57:41.047234 ssb_timeseries-0.2.2/src/ssb_timeseries/__init__.py
--rw-r--r--   0        0        0      739 2024-05-14 10:57:41.047234 ssb_timeseries-0.2.2/src/ssb_timeseries/__main__.py
--rw-r--r--   0        0        0     7585 2024-05-14 10:57:41.047234 ssb_timeseries-0.2.2/src/ssb_timeseries/config.py
--rw-r--r--   0        0        0    36878 2024-05-14 10:57:51.599631 ssb_timeseries-0.2.2/src/ssb_timeseries/dataset.py
--rw-r--r--   0        0        0     8028 2024-05-14 10:57:41.047234 ssb_timeseries-0.2.2/src/ssb_timeseries/dates.py
--rw-r--r--   0        0        0     9990 2024-05-14 10:57:41.051234 ssb_timeseries-0.2.2/src/ssb_timeseries/fs.py
--rw-r--r--   0        0        0    15170 2024-05-14 10:57:41.051234 ssb_timeseries-0.2.2/src/ssb_timeseries/io.py
--rw-r--r--   0        0        0     4242 2024-05-14 10:57:41.051234 ssb_timeseries-0.2.2/src/ssb_timeseries/logging.py
--rw-r--r--   0        0        0    11842 2024-05-14 10:57:41.051234 ssb_timeseries-0.2.2/src/ssb_timeseries/meta.py
--rw-r--r--   0        0        0     5963 2024-05-14 10:57:41.051234 ssb_timeseries-0.2.2/src/ssb_timeseries/properties.py
--rw-r--r--   0        0        0        0 2024-05-14 10:57:41.051234 ssb_timeseries-0.2.2/src/ssb_timeseries/py.typed
--rw-r--r--   0        0        0     5786 2024-05-14 10:57:41.051234 ssb_timeseries-0.2.2/src/ssb_timeseries/sample_data.py
--rw-r--r--   0        0        0     1203 2024-05-14 10:57:41.051234 ssb_timeseries-0.2.2/src/ssb_timeseries/sample_metadata.py
--rw-r--r--   0        0        0     1451 2024-05-14 10:57:41.051234 ssb_timeseries-0.2.2/src/ssb_timeseries/setup.py
--rw-r--r--   0        0        0      411 2024-05-14 10:57:41.051234 ssb_timeseries-0.2.2/src/ssb_timeseries/types.py
--rw-r--r--   0        0        0    11240 1970-01-01 00:00:00.000000 ssb_timeseries-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-23 09:04:33.695865 ssb_timeseries-0.2.3/LICENSE
+-rw-r--r--   0        0        0    10072 2024-05-23 09:04:33.695865 ssb_timeseries-0.2.3/README.md
+-rw-r--r--   0        0        0     4508 2024-05-23 09:04:43.532018 ssb_timeseries-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      452 2024-05-23 09:04:33.699865 ssb_timeseries-0.2.3/src/ssb_timeseries/__init__.py
+-rw-r--r--   0        0        0      739 2024-05-23 09:04:33.699865 ssb_timeseries-0.2.3/src/ssb_timeseries/__main__.py
+-rw-r--r--   0        0        0     9527 2024-05-23 09:04:43.532018 ssb_timeseries-0.2.3/src/ssb_timeseries/config.py
+-rw-r--r--   0        0        0    36528 2024-05-23 09:04:43.532018 ssb_timeseries-0.2.3/src/ssb_timeseries/dataset.py
+-rw-r--r--   0        0        0     8038 2024-05-23 09:04:43.532018 ssb_timeseries-0.2.3/src/ssb_timeseries/dates.py
+-rw-r--r--   0        0        0     9053 2024-05-23 09:04:43.532018 ssb_timeseries-0.2.3/src/ssb_timeseries/fs.py
+-rw-r--r--   0        0        0    15424 2024-05-23 09:04:43.532018 ssb_timeseries-0.2.3/src/ssb_timeseries/io.py
+-rw-r--r--   0        0        0     4286 2024-05-23 09:04:43.532018 ssb_timeseries-0.2.3/src/ssb_timeseries/logging.py
+-rw-r--r--   0        0        0    11842 2024-05-23 09:04:33.699865 ssb_timeseries-0.2.3/src/ssb_timeseries/meta.py
+-rw-r--r--   0        0        0     5963 2024-05-23 09:04:33.699865 ssb_timeseries-0.2.3/src/ssb_timeseries/properties.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:04:33.699865 ssb_timeseries-0.2.3/src/ssb_timeseries/py.typed
+-rw-r--r--   0        0        0     5786 2024-05-23 09:04:33.699865 ssb_timeseries-0.2.3/src/ssb_timeseries/sample_data.py
+-rw-r--r--   0        0        0     1203 2024-05-23 09:04:33.699865 ssb_timeseries-0.2.3/src/ssb_timeseries/sample_metadata.py
+-rw-r--r--   0        0        0     1451 2024-05-23 09:04:33.699865 ssb_timeseries-0.2.3/src/ssb_timeseries/setup.py
+-rw-r--r--   0        0        0      253 2024-05-23 09:04:43.532018 ssb_timeseries-0.2.3/src/ssb_timeseries/types.py
+-rw-r--r--   0        0        0    11240 1970-01-01 00:00:00.000000 ssb_timeseries-0.2.3/PKG-INFO
```

### Comparing `ssb_timeseries-0.2.2/LICENSE` & `ssb_timeseries-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_timeseries-0.2.2/README.md` & `ssb_timeseries-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ssb_timeseries-0.2.2/pyproject.toml` & `ssb_timeseries-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-timeseries"
-version = "0.2.2"
+version = "0.2.3"
 description = "SSB Timeseries"
 authors = ["Bernhard Ryeng <bernhard.ryeng@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/ssb-timeseries"
 repository = "https://github.com/statisticsnorway/ssb-timeseries"
 documentation = "https://statisticsnorway.github.io/ssb-timeseries"
```

### Comparing `ssb_timeseries-0.2.2/src/ssb_timeseries/__main__.py` & `ssb_timeseries-0.2.3/src/ssb_timeseries/__main__.py`

 * *Files identical despite different names*

### Comparing `ssb_timeseries-0.2.2/src/ssb_timeseries/config.py` & `ssb_timeseries-0.2.3/src/ssb_timeseries/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,77 @@
-# from dataclasses import dataclass
 import json
 import os
 import sys
+from dataclasses import dataclass
 from pathlib import Path
 
+from typing_extensions import Self
+
 from ssb_timeseries import fs
 from ssb_timeseries.types import PathStr
 
 # mypy: disable-error-code="assignment, arg-type"
 
 
 GCS = "gs://ssb-prod-dapla-felles-data-delt/poc-tidsserier"
 JOVYAN = "/home/jovyan"
 HOME = str(Path.home())
+LOGFILE = "timeseries.log"
 
 DEFAULT_BUCKET = HOME
 DEFAULT_TIMESERIES_LOCATION = os.path.join(HOME, "series_data")
 DEFAULT_CONFIG_LOCATION = os.path.join(HOME, "timeseries_config.json")
-DEFAULT_LOG_FILE_LOCATION: str = os.path.join(HOME, "logs", "timeseries.log")
-TIMESERIES_CONFIG: str = os.getenv("TIMESERIES_CONFIG", DEFAULT_CONFIG_LOCATION)
+DEFAULT_LOG_FILE_LOCATION: str = os.path.join(HOME, "logs", LOGFILE)
+CONFIGURATION_FILE: str = os.getenv("TIMESERIES_CONFIG", DEFAULT_CONFIG_LOCATION)
+
+
+@dataclass(slots=True)
+class Cfg:
+    """Configuration class."""
+
+    configuration_file: str = CONFIGURATION_FILE
+    repository: str = DEFAULT_TIMESERIES_LOCATION
+    log_file: str = DEFAULT_LOG_FILE_LOCATION
+    bucket: str = DEFAULT_BUCKET
+    product: str = ""
+
+    def __str__(self) -> str:
+        """Return timeseries configurations as JSON string."""
+        return json.dumps(self, default=lambda o: o.__dict__, sort_keys=True, indent=4)
+
+    def save(self, path: PathStr = CONFIGURATION_FILE) -> None:
+        """Saves configurations to JSON file and set environment variable TIMESERIES_CONFIG to the location of the file.
+
+        Args:
+            path (PathStr): Full path of the JSON file to save to. Defaults to the value of the environment variable TIMESERIES_CONFIG.
+        """
+        fs.write_json(content=str(self), path=path)
+        if HOME == JOVYAN:
+            # For some reason `os.environ["TIMESERIES_CONFIG"] = path` does not work:
+            cmd = f"export TIMESERIES_CONFIG={CONFIGURATION_FILE}"
+            os.system(cmd)
+            # os.system(f"echo '{cmd}' >> ~/.bashrc")
+        else:
+            os.environ["TIMESERIES_CONFIG"] = path
+
+    @classmethod
+    def load(cls, path: PathStr) -> Self:
+        """Read the properties from a JSON file into a Config object."""
+        if path:
+            json_file = json.loads(fs.read_json(path))
+
+            return cls(
+                configuration_file=str(path),
+                bucket=json_file.get("bucket"),
+                repository=json_file.get("timeseries_root"),
+                product=json_file.get("product"),
+                log_file=json_file.get("log_file"),
+            )
+        else:
+            raise ValueError("cfg_from_file was called with an empty or invalid path.")
 
 
 class Config:
     """Timeseries configurations: bucket, product, timeseries_root, log_file."""
 
     def __init__(self, configuration_file: str = "", **kwargs: str) -> None:
         """Create or retrieve configurations.
@@ -36,27 +85,27 @@
         Kwargs:
             - bucket              - The "production bucket" location. Sharing and snapshots typically go in the sub directories hee, depending on configs.
             - product             - Optional sub directory for "production bucket".
             - timeseries_root     - Series data are stored in tree underneath. Defaults to '$HOME/series_data/'
             - log_file            - Exactly that. Defaults to '$HOME/series_data/'
         """
         if fs.exists(configuration_file):
-            self.load(configuration_file)
+            # self = Cfg.load(configuration_file) # NOSONAR # TODO: switch to Cfg class to simplify code
             self.configuration_file = configuration_file
             os.environ["TIMESERIES_CONFIG"] = configuration_file
         elif configuration_file:
-            if fs.exists(TIMESERIES_CONFIG):
-                self.load(TIMESERIES_CONFIG)
+            if fs.exists(CONFIGURATION_FILE):
+                self.load(CONFIGURATION_FILE)
                 self.save(configuration_file)
             else:
                 self.__set_default_config()
 
-        elif fs.exists(TIMESERIES_CONFIG):
-            self.load(TIMESERIES_CONFIG)
-            self.configuration_file = TIMESERIES_CONFIG
+        elif fs.exists(CONFIGURATION_FILE):
+            self.load(CONFIGURATION_FILE)
+            self.configuration_file = CONFIGURATION_FILE
 
         if kwargs:
             log_file = kwargs.get("log_file", "")
             if log_file:
                 self.log_file = log_file
             elif not self.log_file:
                 self.log_file = DEFAULT_LOG_FILE_LOCATION
@@ -106,38 +155,41 @@
             self.bucket = read_from_file.get("bucket")
             self.timeseries_root = read_from_file.get("timeseries_root")
             self.product = read_from_file.get("product", "")
             self.log_file = read_from_file.get("log_file", "")
         else:
             raise ValueError("Config.load(<path>) was called with an empty path.")
 
-    def save(self, path: PathStr = TIMESERIES_CONFIG) -> None:
+    def save(self, path: PathStr = CONFIGURATION_FILE) -> None:
         """Saves configurations to JSON file and set environment variable TIMESERIES_CONFIG to the location of the file.
 
         Args:
             path (PathStr): Full path of the JSON file to save to. Defaults to the value of the environment variable TIMESERIES_CONFIG.
         """
         fs.write_json(content=self.to_json(), path=path)
         if HOME == JOVYAN:
             # For some reason `os.environ["TIMESERIES_CONFIG"] = path` does not work:
-            cmd = f"export TIMESERIES_CONFIG={TIMESERIES_CONFIG}"
+            cmd = f"export TIMESERIES_CONFIG={CONFIGURATION_FILE}"
             os.system(cmd)
             # os.system(f"echo '{cmd}' >> ~/.bashrc")
         else:
             os.environ["TIMESERIES_CONFIG"] = path
 
     def __set_default_config(self) -> None:
         self.bucket = DEFAULT_BUCKET
         self.configuration_file = DEFAULT_CONFIG_LOCATION
         self.log_file = DEFAULT_LOG_FILE_LOCATION
         self.product = ""
         self.timeseries_root = DEFAULT_TIMESERIES_LOCATION
         fs.touch(self.log_file)
 
 
+CONFIG = Config(configuration_file=CONFIGURATION_FILE)
+
+
 def main(*args: str | PathStr) -> None:
     """Set configurations to predefined defaults when run from command line.
 
     Use:
         ```
         poetry run timeseries-config <option>
         ```
@@ -173,19 +225,19 @@
         case "home":
             bucket = HOME
             timeseries_root = os.path.join(HOME, "series_data")
             log_file = DEFAULT_LOG_FILE_LOCATION
         case "gcs":
             bucket = GCS
             timeseries_root = os.path.join(GCS, "series_data")
-            log_file = os.path.join(HOME, "logs", "timeseries.log")
+            log_file = os.path.join(HOME, "logs", LOGFILE)
         case "jovyan":
             bucket = JOVYAN
             timeseries_root = os.path.join(JOVYAN, "series_data")
-            log_file = os.path.join(JOVYAN, "logs", "timeseries.log")
+            log_file = os.path.join(JOVYAN, "logs", LOGFILE)
         case _:
             raise ValueError(
                 f"Unrecognised named configuration preset '{named_config}'."
             )
 
     cfg = Config(
         configuration_file=TIMESERIES_CONFIG,
```

### Comparing `ssb_timeseries-0.2.2/src/ssb_timeseries/dataset.py` & `ssb_timeseries-0.2.3/src/ssb_timeseries/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,16 +106,16 @@
         elif load_data and self.data_type.versioning == properties.Versioning.AS_OF:
             self.data = self.io.read_data(self.as_of_utc)
         else:
             self.data = pd.DataFrame()
 
         kwarg_data: pd.DataFrame = kwargs.get("data", pd.DataFrame())
         if not kwarg_data.empty:
-            # TODO: if kwarg_data overlap data from file, overwrite with kwarg_data
-            # ... for all versioning types? Think it through!
+            # if kwarg_data overlaps data from file, overwrite with kwarg_data
+            # ... does this make sense for all versioning types? Verify!
             self.data = kwarg_data
             # self.data.set_index(self.datetime_columns())
             # will not work for valid_from_to
             # self.data.set_index(self.datetime_columns()).to_period()
             ts_logger.debug(
                 f"DATASET {self.name}: Merged {kwarg_data.size} datapoints:\n{self.data}"
             )
@@ -141,19 +141,22 @@
                 for n in self.numeric_columns()
             }
 
             name_pattern = kwargs.get("name_pattern", "")
             if name_pattern:
                 for s in self.tags["series"]:
                     name_parts = s.split("_")
-                    # [self.tags['series'][s][attribute] = value for attribute,  value in zip(name_pattern, name_parts)]
                     for attribute, value in zip(name_pattern, name_parts, strict=False):
                         self.tags["series"][s][attribute] = value
 
-                    # [self.tags.series[k] = for k, a in zip(self.numeric_columns(), name_pattern]
+            series_tags = kwargs.get("series_tags", {})
+            if series_tags:
+                for s in self.tags["series"]:
+                    for attribute, value in series_tags.items():
+                        self.tags["series"][s][attribute] = value
 
         self.product: str = kwargs.get("product", "")
         self.process_stage: str = kwargs.get("process_stage", "")
         self.sharing: dict[str, str] = kwargs.get("sharing", {})
 
     def copy(self, new_name: str, **kwargs: Any) -> Self:
         """Create a copy of the Dataset.
@@ -168,20 +171,19 @@
         out.rename(new_name)
         return out
 
     def rename(self, new_name: str) -> None:
         """Rename the Dataset.
 
         For use by .copy, and on very rare other occasions. Does not move or rename any previously stored data.
-
-        TODO: Fix that?
         """
+        # TODO: Fix that?
         self.name = new_name
 
-        self.tags["dataset"] = new_name
+        self.tags["name"] = new_name
         for _, v in self.tags["series"].items():
             v["dataset"] = new_name
 
     def save(self, as_of_tz: datetime = None) -> None:
         """Persist the Dataset.
 
         Args:
@@ -216,46 +218,41 @@
             product=self.product,
             process_stage=self.process_stage,
             sharing=self.sharing,
             period_from=date_from,
             period_to=date_to,
         )
 
-    def series(self, what: str = "names") -> Any:
-        """Get series names (default) or tags."""
-        if what.lower() == "names":
-            return self.data.columns
-        elif what.lower() == "tags":
-            return self.tags["series"]
-        else:
-            raise ValueError(f"Unrecognised return type {what}")
+    @property
+    def series(self) -> list[str]:
+        """Get series names."""
+        return self.numeric_columns()
 
-    def series_tags(self, series_name: str | list[str] = "") -> Any:  # remove this?
+    @property
+    def series_tags(self) -> dict[str, str | list[str]]:
         """Get series tags."""
-        if series_name:
-            return self.tags["series"][series_name]
-        else:
-            return self.tags["series"]
+        return self.tags["series"]  # type: ignore
 
     def tag_set(self, tags: dict[str, str] = None, **kwargs: str | list[str]) -> None:
         """Tag the set.
 
         Tags may be provided as dictionary of tags, or as kwargs.
 
         In both cases they take the form of attribute-value pairs.
 
         Attribute (str): Attribute identifier.
         Ideally attributes relies on KLASS, ie a KLASS taxonomy defines the possible attribute values.
 
         Value (str): Element identifier, unique within the taxonomy. Ideally KLASS code.
         """
+        # TODO: Implement this:
         if tags:
-            raise NotImplementedError("Not (yet) implemented. Planned for later.")
+            raise NotImplementedError()
         elif kwargs:
-            raise NotImplementedError("Not (yet) implemented. Planned for later.")
+            raise NotImplementedError()
             # if value not in self[attribute]:
             # self[attribute].append(value)
         else:
             raise ValueError("Must provide either tags or kwargs.")
 
     def tag_series(
         self, identifiers: str | list[str], tags: dict[str, str] = None, **kwargs: str
@@ -267,26 +264,27 @@
         In both cases they take the form of attribute-value pairs.
 
         Attribute (str): Attribute identifier.
         Ideally attributes relies on KLASS, ie a KLASS taxonomy defines the possible attribute values.
 
         Value (str): Element identifier, unique within the taxonomy. Ideally KLASS code.
         """
-        if tags:
-            raise NotImplementedError("Not (yet) implemented. Planned for later.")
-        elif kwargs:
-            raise NotImplementedError("Not (yet) implemented. Planned for later.")
-            # if value not in self[attribute]:
-            # self[attribute].append(value)
-        else:
-            raise ValueError("Must provide either tags or kwargs.")
-        # should handle different datatypes for "item" :
-        # name, int index, List of name or index
-        # if value not in self.series[item][attribute]:
-        #    self.series[attribute].append(value)
+        if not tags:
+            tags = {}
+
+        tags.update(kwargs)
+
+        if not identifiers:
+            identifiers = self.series
+
+        for s in self[identifiers]:
+            if s in self.series:
+                self.tags["series"][s].update(tags)
+            else:
+                raise ValueError(f"{s} not in {self.series}.")
 
     @no_type_check
     def filter(
         self,
         pattern: str = "",
         tags: dict[Any, Any] = None,
         regex: str = "",
@@ -317,16 +315,18 @@
             matching_series = df.columns
 
         if pattern:
             df = self.data.filter(like=pattern).copy(deep=True)
             matching_series = df.columns
 
         if tags:
-            series_tags = self.series_tags()
-            # ts_logger.debug(f"DATASET.filter()\ntags to find:\n\t{tags}\ntags in series:\n\t{series_tags}")
+            series_tags = self.series_tags
+            ts_logger.warning(
+                f"DATASET.filter()\ntags to find:\n\t{tags}\ntags in series:\n\t{series_tags}"
+            )
             matching_series = [
                 name
                 for name, s_tags in series_tags.items()
                 if all(s_tags[k] in v for k, v in tags.items())
             ]
             ts_logger.debug(f"DATASET.filter(tags) matched series:\n{matching_series} ")
             df = self.data[matching_series].copy(deep=True)
@@ -392,15 +392,16 @@
             raise TypeError("Dataset.filter() did not return a Dataset type.")
 
     def plot(self, *args: Any, **kwargs: Any) -> Any:
         """Plot dataset data.
 
         Convenience wrapper around Dataframe.plot() with sensible defaults.
         """
-        xlabels = self.datetime_columns()
+        xlabels = self.datetime_columns()[0]
+        ts_logger.debug(f"DATASET.plot(): x labels = {xlabels}")
         ts_logger.debug(f"Dataset.plot({args!r}, {kwargs!r}) x-labels {xlabels}")
         return self.data.plot(  # type: ignore[call-overload]
             xlabels,
             *args,
             legend=len(self.data.columns) < 9,
             title=self.name,
             figsize=(12, 4),
@@ -568,23 +569,26 @@
         """Get names of datetime columns (valid_at, valid_from, valid_to).
 
         Args:
             *comparisons (Self | pd.DataFrame): Objects to compare with. If provided, returns the intersection of self and all comparisons.
 
         Returns:
             list[str]: The (common) datetime column names of self (and comparisons).
+
+        Raises:
+            ValueError: If comparisons are not of type Self or pd.DataFrame.
         """
         intersect = set(self.data.columns) & {"valid_at", "valid_from", "valid_to"}
         for c in comparisons:
             if isinstance(c, Dataset):
                 intersect = set(c.data.columns) & intersect
             elif isinstance(c, pd.DataFrame):
                 intersect = set(c.columns) & intersect
             else:
-                pass
+                raise ValueError(f"Unsupported type: {type(c)}")
 
         return list(intersect)
 
     @no_type_check
     def math(
         self,
         other: Self | pd.DataFrame | pd.Series | int | float,
@@ -788,17 +792,15 @@
             aggregate_function (str | list[str]): Optional function name (or list) of the function names to apply (mean | count | sum | ...). Defaults to `sum`.
 
         Returns:
             Self: A dataset object with the aggregated data.
             If the taxonomy object has hierarchical structure, aggregate series are calculated for parent nodes at all levels.
             If the taxonomy is a flat list, only a single 'total' aggregate series is calculated.
         """
-        if isinstance(taxonomy, Taxonomy):
-            pass
-        else:
+        if not isinstance(taxonomy, Taxonomy):
             taxonomy = Taxonomy(taxonomy)
 
         if isinstance(aggregate_function, str):
             aggregate_function = [aggregate_function]
 
         df = self.data.copy().drop(columns=self.numeric_columns())
         for node in taxonomy.parent_nodes():
```

### Comparing `ssb_timeseries-0.2.2/src/ssb_timeseries/dates.py` & `ssb_timeseries-0.2.3/src/ssb_timeseries/dates.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# type: ignore
+# type: ignore #NOSONAR
 # ruff: noqa
 """Date and time utilities."""
 
 from datetime import datetime as dt, tzinfo
 from typing import Any
 from zoneinfo import ZoneInfo
 
 from dateutil import parser
 
 from ssb_timeseries.logging import ts_logger
 
 MAX_TIME_PRECISION = "second"
+DEFAULT_TIMESPEC = "seconds"
 DEFAULT_TZ = ZoneInfo("Europe/Oslo")  # Will shift between CET and CEST
 UTC = ZoneInfo("UTC")
 
 
 def date_utc(some_date: dt | str | None, **kwargs) -> dt:
     """Convert date to UTC.
 
@@ -36,15 +37,14 @@
     """Convert date to Europe/Oslo timezone; ie shifting between CET and CEST.
 
     If the date has no timezone information, the data is assumed to be in Oslo timezone.
 
     The output will be rounded to the precision specified by kwarg 'rounding'. Default precision 'minute' will be used if none is provided.
     """
     dt_type = ensure_datetime(some_date, tz=DEFAULT_TZ)
-    # correct_tz = dt_type.astimezone(tz=DEFAULT_TZ)
     return date_round(dt_type, **kwargs)
 
 
 def date_round(d: dt, **kwargs) -> dt:
     """Round date to specified by kwarg 'rounding' or default precision.
 
     Rounding can take the values 'none', 'day', 'd', 'hour', 'h', 'minute', 'min', 'm', 'second', 'sec', or 's'.
@@ -122,22 +122,22 @@
 
 def now_cet(**kwargs) -> dt:
     """Return now in CET."""
     t = dt.now(tz=UTC)
     return date_round(t, **kwargs)
 
 
-def utc_iso(d: Any, timespec: str = "seconds") -> str:
+def utc_iso(d: Any, timespec: str = DEFAULT_TIMESPEC) -> str:
     """Convert date to UTC and return as an ISO formatted string."""
     return date_utc(d).isoformat(timespec=timespec)
 
 
-def utc_iso_no_colon(d: dt, timespec: str = "seconds") -> str:
+def utc_iso_no_colon(d: dt, timespec: str = DEFAULT_TIMESPEC) -> str:
     """Convert date to UTC and return as an ISO formatted string without the colons."""
-    return utc_iso(d).replace(":", "")
+    return utc_iso(d, timespec=timespec).replace(":", "")
 
 
 class Interval:
     def __init__(self, f=None, t=None, **kwargs) -> None:
         """Interval(date_from, date_to)
         or a number of variations of named parameters: start/stop, begin/end, as_of, as_of_from/as_of_to, valid_from, valid_to -
         If only "as_of" is provided, start/stop are both set to this date.
@@ -156,15 +156,15 @@
         date_from = kwargs.get("date_from")
         date_to = kwargs.get("date_to")
         from_date = kwargs.get("from_date")
         to_date = kwargs.get("to_date")
         begin = kwargs.get("begin")
         end = kwargs.get("end")
 
-        MAX_TIME_precision: str = kwargs.get("MAX_TIME_precision")
+        precision: str = kwargs.get("precision", MAX_TIME_PRECISION)
 
         ts_logger.debug(f"Interval.__init__ with kwargs:\n{kwargs}")
 
         self.start = (
             f
             or as_of
             or start
@@ -185,17 +185,17 @@
             or date_to
             or to_date
             or valid_to
             or end
             or dt.max
         )
 
-        if MAX_TIME_precision:
+        if precision:
             # "round" to MAX_TIME_precision if provided
-            pass
+            ...
 
         ts_logger.debug(f"Interval.__init__ returns self:\n{self}")
 
     def includes(self, *args: dt | list[dt]):
         ts_logger.debug(f"Interval.include args: {args}")
         if len(args) == 1:
             ts_logger.debug("Interval.include - single input")
```

### Comparing `ssb_timeseries-0.2.2/src/ssb_timeseries/fs.py` & `ssb_timeseries-0.2.3/src/ssb_timeseries/fs.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,36 +6,34 @@
 
 import pandas
 import pyarrow
 from dapla import FileClient
 
 from ssb_timeseries.types import PathStr
 
-# from ssb_timeseries.logging import ts_logger  # , log_start_stop
-
 """This is an abstraction that allows file based io regardless of whether involved file systems are local or gcs.
 """
 
 # ruff: noqa: ANN002, ANN003
 # mypy: disable-error-code="arg-type, type-arg, no-any-return, no-untyped-def, import-untyped, attr-defined, type-var, index"
 
 
 def remove_prefix(path: PathStr) -> str:
     """Helper function to compensate for some os.* functions shorten gs://<path> to gs:/<path>."""
     return path.replace("//", "/").replace("gs:/", "")
 
 
 def is_gcs(path: PathStr) -> bool:
     """Check if path is on GCS."""
-    return str(path)[:4] == "gs:/"
+    return str(path).startswith("gs:/")
 
 
 def is_local(path: PathStr) -> bool:
     """Check if path is local."""
-    return str(path)[:4] != "gs:/"
+    return not str(path).startswith("gs:/")
 
 
 def fs_type(path: PathStr) -> str:
     """Check filesystem type (local or GCS) for a given path."""
     out = ""
     types = {"gcs": is_gcs(path), "local": is_local(path)}
     out = list(types.keys())[list(types.values()).index(True)]
@@ -49,30 +47,14 @@
     elif is_gcs(path):
         fs = FileClient.get_gcs_file_system()
         return fs.exists(path)
     else:
         return Path(path).exists()
 
 
-# def existing_subpath(path: PathStr) -> str:
-#     """Return the existing part of a path on local or GCS file system."""
-#     out = ""
-#     # TODO: redo this with pathlib
-#     parts = str(path).split(os.sep)
-#     pp = ""
-#     for p in parts:
-#         if p:
-#             pp = os.sep.join([pp, p])
-#         if exists(pp):
-#             out = pp
-
-#     return out
-
-
-# redo above w pathlib
 def existing_subpath(path: PathStr) -> str:
     """Return the existing part of a path on local or GCS file system."""
     if Path(path).exists():
         return str(path)
     else:
         p = Path(path).parent
         while not p.exists():
@@ -86,43 +68,32 @@
         fs = FileClient.get_gcs_file_system()
         fs.touch(path)
     else:
         mk_parent_dir(path)
         Path(path).touch()
 
 
-# def dir_name(path: PathStr):
-#     basename = os.path.basename(path)
-#     parts = os.path.splitext(basename)
-#     if len(parts) > 1:
-#         d = os.path.dirname(path)
-#     else:
-#         d = path
-
-#     return d  # os.path.normpath(d)
-
-
 def mkdir(path: PathStr) -> None:
     """Make directory regardless of filesystem is local or GCS."""
     # not good enough .. it is hard to distinguish between dirs and files that do not exist yet
     if is_local(path):
         os.makedirs(path, exist_ok=True)
     else:
-        pass
+        ...
 
 
 def mk_parent_dir(path: PathStr) -> None:
     """Ensure a parent directory exists. ... regardless of wether fielsystem is local or GCS."""
     # wanted a mkdir that could work with both file and directory paths,
     # but it is hard to distinguish between dirs and files that do not exist yet
     # --> use this to create parent directory for files, mkdir() when the last part of path is a directory
     if is_local(path):
         os.makedirs(os.path.dirname(path), exist_ok=True)
     else:
-        pass
+        ...
 
 
 def file_count(path: PathStr, create: bool = False) -> int:
     """Count files in path. Should work regardless of wether source and target location is local fs or GCS to local."""
     return len(ls(path, create=create))
 
 
@@ -175,29 +146,31 @@
             fs.put(from_path, to_path)
         case ("gcs", "local"):
             fs.get(from_path, to_path)
         case ("gcs", "gcs"):
             fs.move(from_path, to_path)
 
 
-def rm(path: PathStr, *args) -> None:
+def rm(path: PathStr) -> None:
     """Remove file from local or GCS filesystem."""
     if is_gcs(path):
-        pass
+        ...
         # TO DO: implement this (but recursive)
         # fs = FileClient.get_gcs_file_system()
         # fs.rm(path)
     else:
         os.remove(path)
 
 
-def rmtree(path: str, *args) -> None:
+def rmtree(
+    path: str,
+) -> None:
     """Remove all directory and all its files and subdirectories regardless of local or GCS filesystem."""
     if is_gcs(path):
-        pass
+        ...
         # TO DO: implement this (but recursive)
         # fs = FileClient.get_gcs_file_system()
         # fs.rm(path)
     else:
         shutil.rmtree(path)
 
 
@@ -205,30 +178,40 @@
     """Return common part of path, for two or more files. Files must be on same file system, but the file system can be either local or GCS."""
     # TO DO: add support for Windows style paths?
     # ... regex along the lines of: [A-Z\:|\\\\]
     paths = [a.replace("gs:/", "") for a in args]
     return os.path.commonpath(paths)
 
 
-def find(path: PathStr, pattern: str = "", *args, **kwargs) -> list[str]:
+def find(
+    path: PathStr,
+    pattern: str = "",
+    full_path: bool = False,
+    replace_root: bool = False,
+) -> list[str]:
     """Find files and subdirectories with names matching pattern. Should work for both local and GCS filesystems."""
     if pattern:
         pattern = f"*{pattern}*"
     else:
         pattern = "*"
-
+    search_str = os.path.join(path, "*", pattern)
     if is_gcs(path):
         fs = FileClient.get_gcs_file_system()
-        return fs.glob(os.path.join(path, pattern))
+        found = fs.glob(search_str)
     else:
-        search_str = os.path.join(path, "*", pattern)
-        dirs = glob.glob(search_str)
-        search_results = [d.replace(path, "root").split(os.path.sep) for d in dirs]
+        found = glob.glob(search_str)
 
-        return [f[2] for f in search_results]
+    if replace_root:
+        # may be necessary if not returning full path? -> TODO: add tests
+        found = [f.replace(path, "root").split(os.path.sep) for f in found]
+
+    if full_path:
+        return found
+    else:
+        return [f[-1] for f in found]
 
 
 def read_parquet(path: PathStr) -> None:
     """TODO: Add faster pyarrrow implementations enforcing type based schemas."""
     pass
 
 
@@ -240,16 +223,14 @@
 ) -> None:
     """TODO: Add faster pyarrrow implementations enforcing type based schemas."""
     pass
 
 
 def pandas_read_parquet(
     path: PathStr,
-    *args,
-    **kwargs,
 ) -> pandas.DataFrame:
     """Quick and dirty --> replace later."""
     if is_gcs(path):
         fs = FileClient.get_gcs_file_system()
         with fs.open(path, "rb") as file:
             df = pandas.read_parquet(file)
     else:
@@ -281,32 +262,25 @@
     else:
         with open(path) as file:
             return json.load(file)
 
 
 def write_json(path: PathStr, content: str | dict) -> None:
     """Write json file to path on either local fs or GCS."""
-    # Code does not make sense, but is not invoked:
-    # if not isinstance(path, str):
-    #     path = json.loads(path)
-    # more reasonable would be somehting like -->
-    # if not isinstance(content, str):
-    #     content = json.loads(content)
-    # ... but that caauses an error. --> Code is "too clever"?
-
     if is_gcs(path):
         fs = FileClient.get_gcs_file_system()
         with fs.open(path, "w") as file:
             json.dump(content, file, indent=4, ensure_ascii=False)
     else:
         os.makedirs(os.path.dirname(path), exist_ok=True)
         with open(path, "w") as file:
             json.dump(content, file, indent=4, ensure_ascii=False)
 
 
+# nosonar: disable comment
 # from pyarrow import fs
 # local = fs.LocalFileSystem()
 # with local.open_output_stream('/tmp/pyarrowtest.dat') as stream:
 #         stream.write(b'data')
 # 4
 # with local.open_input_stream('/tmp/pyarrowtest.dat') as stream:
 #         print(stream.readall())
@@ -315,13 +289,7 @@
 # # creating an fsspec-based filesystem object for Google Cloud Storage
 # import gcsfs
 # fs = gcsfs.GCSFileSystem(project='my-google-project')
 
 # # using this to read a partitioned dataset
 # import pyarrow.dataset as ds
 # ds.dataset("data/", filesystem=fs)
-
-
-# @staticmethod
-# def funcname(parameter_list):
-#     """Docstring"""
-#     pass
```

### Comparing `ssb_timeseries-0.2.2/src/ssb_timeseries/io.py` & `ssb_timeseries-0.2.3/src/ssb_timeseries/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,46 @@
-"""The IO module provides abstractions for READ and WRITE operations so that `Dataset` does not have to care avbout the mechanics.
-
-TO DO: turn Dataset.io into a Protocol class?
-
-Essential configs:
-    TIMESERIES_CONFIG: str = os.environ.get("TIMESERIES_CONFIG")
-    CONFIG = config.Config(configuration_file=TIMESERIES_CONFIG)
-
-Default configs may be created by running
-    `poetry run timeseries-config {home | jovyan | gcs}`
-
-See `config` module docs for details.
-"""
-
 import glob
 import os
 import re
 from datetime import datetime
 from typing import NamedTuple
 
 import pandas
 
-from ssb_timeseries import config
 from ssb_timeseries import fs
 from ssb_timeseries import properties
+from ssb_timeseries.config import CONFIG
 from ssb_timeseries.dates import Interval
 from ssb_timeseries.dates import utc_iso_no_colon
 from ssb_timeseries.logging import ts_logger
 from ssb_timeseries.types import PathStr
 
+"""The IO module provides abstractions for READ and WRITE operations so that `Dataset` does not have to care avbout the mechanics.
+
+TO DO: turn Dataset.io into a Protocol class?
+
+Essential configs:
+    TIMESERIES_CONFIG: str = os.environ.get("TIMESERIES_CONFIG")
+    CONFIG = config.Config(configuration_file=TIMESERIES_CONFIG)
+
+Default configs may be created by running
+    `poetry run timeseries-config {home | jovyan | gcs}`
+
+See `config` module docs for details.
+"""
+
+# consider:
 # from ssb_timeseries.types import F
 # from abc import ABC, abstractmethod
 # from typing import Protocol
 # import contextlib
 
 # mypy: disable-error-code="type-var, arg-type, type-arg, return-value, attr-defined, union-attr, operator, assignment,import-untyped, "
 
 
-TIMESERIES_CONFIG: str = os.environ.get("TIMESERIES_CONFIG")
-CONFIG = config.Config(configuration_file=TIMESERIES_CONFIG)
-
-
 class SearchResult(NamedTuple):
     """Result item for search."""
 
     name: str
     type_directory: str
 
 
@@ -65,16 +62,16 @@
         """
         self.set_name = set_name
         self.data_type = set_type
         self.process_stage = process_stage
         self.sharing = sharing
 
         if as_of_utc is None:
-            pass
-            # exception if not
+            ...
+            # exception if type is AS_OF
         else:
             self.as_of_utc: datetime = utc_iso_no_colon(as_of_utc)
 
     @property
     def root(self) -> str:
         """The root path is the basis for all other paths."""
         ts_root = CONFIG.timeseries_root
@@ -101,15 +98,15 @@
         if "AS_OF" in self.set_type_dir:
             file_name = f"{self.set_name}-as_of_{self.as_of_utc}-data.parquet"
         elif "NONE" in self.set_type_dir:
             file_name = f"{self.set_name}-latest-data.parquet"
         elif "NAMED" in self.set_type_dir:
             file_name = f"{self.set_name}-NAMED-data.parquet"
         else:
-            raise Exception("Unhandled versioning.")
+            raise ValueError("Unhandled versioning.")
 
         ts_logger.debug(file_name)
         return file_name
 
     @property
     def data_dir(self) -> str:
         """The data directory for the dataset. This is a subdirectory under the type path."""
@@ -241,17 +238,15 @@
 
     def last_version(self, directory: str, pattern: str = "*.parquet") -> str:
         """Check directory and get max version number from files matching regex pattern."""
         files = fs.ls(directory, pattern=pattern)
         number_of_files = len(files)
 
         # TODO: mypy --> error: Item "None" of "Match[str] | None" has no attribute "group"  [union-attr]
-        vs = sorted(
-            [int(re.search("(_v)([0-9]+)(.parquet)", f).group(2)) for f in files]
-        )
+        vs = sorted([int(re.search("(_v)(\d+)(.parquet)", f).group(2)) for f in files])
         ts_logger.debug(
             f"DATASET {self.set_name}: io.last_version regex identified versions {vs} in {directory}."
         )
         if vs:
             read_from_filenames = max(vs)
             out = read_from_filenames
         else:
@@ -301,35 +296,32 @@
             return dt.isoformat().replace(":", "")
 
         if as_of_utc:
             out = f"{self.set_name}_p{iso_no_colon(period_from)}_p{iso_no_colon(period_to)}_v{iso_no_colon(as_of_utc)}_v{next_vs}"
         else:
             out = f"{self.set_name}_p{iso_no_colon(period_from)}_p{iso_no_colon(period_to)}_v{next_vs}"
 
-            #  to comply with the naming standard we need to stuff about the data
+            #  to comply with the naming standard we need to know some things about the data
             ts_logger.debug(
                 f"DATASET last version {next_vs} from {period_from} to {period_to}.')"
             )
         return out
 
-    def sharing_directory(
-        self,
-        team: str,
-        bucket: str,
-    ) -> PathStr:
+    def sharing_directory(self, bucket: str, team: str = "") -> PathStr:
         """Get name of sharing directory based on dataset parameters and configuration.
 
         Creates the directory if it does not exist.
         """
-        # if team:
-        #     dir = os.path.join(bucket, team, self.set_name)
-        # else:
-        #     dir = os.path.join(bucket, self.set_name)
+        fix_test_cases_before_taking_this_approach = False
+        if team and fix_test_cases_before_taking_this_approach:
+            # allowing this breaks tests! --> TODO: adapt test cases
+            directory = os.path.join(bucket, team, self.set_name)
+        else:
+            directory = os.path.join(bucket, self.set_name)
 
-        directory = os.path.join(bucket, self.set_name)
         ts_logger.warning(f"DATASET.IO.SHARING_DIRECTORY: {directory}")
         fs.mkdir(directory)
         return directory
 
     def snapshot(
         self,
         product: str,
@@ -365,15 +357,15 @@
         data_publish_path = os.path.join(directory, f"{snapshot_name}.parquet")
         meta_publish_path = os.path.join(directory, f"{snapshot_name}.json")
 
         fs.cp(self.data_fullpath, data_publish_path)
         fs.cp(self.metadata_fullpath, meta_publish_path)
 
         if sharing:
-            ts_logger.debug(f"Sharing configs: {sharing}")
+            ts_logger.warning(f"Sharing configs: {sharing}")
             for s in sharing:
                 ts_logger.debug(f"Sharing: {s}")
                 fs.cp(
                     data_publish_path,
                     self.sharing_directory(bucket=s["path"], team=s["team"]),
                 )
                 fs.cp(
@@ -398,29 +390,36 @@
             raise DatasetIoException(
                 f"Directory {path} must be below {ts_root} in file tree."
             )
         return path
 
 
 def find_datasets(
-    pattern: str | PathStr = "", as_of: datetime | None = None
+    pattern: str | PathStr = "",  # as_of: datetime | None = None
 ) -> list[SearchResult]:
     """Search for files in under timeseries root."""
     if pattern:
         pattern = f"*{pattern}*"
     else:
         pattern = "*"
 
-    search_str = os.path.join(CONFIG.timeseries_root, "*", pattern)
-    dirs = glob.glob(search_str)
-    ts_logger.debug(f"DATASET.IO.SEARCH: {search_str} dirs{dirs}")
+    dirs_old = glob.glob(os.path.join(CONFIG.timeseries_root, "*", pattern))
+    search_results_old = [
+        d.replace(CONFIG.timeseries_root, "root").split(os.path.sep) for d in dirs_old
+    ]
+    dirs = fs.find(CONFIG.timeseries_root, pattern, full_path=True)
+    ts_logger.warning(
+        f"DATASET.IO.SEARCH: {pattern}:\n\t--> dirs\n\tnew: {dirs}\n\told: {dirs_old}"
+    )
     search_results = [
         d.replace(CONFIG.timeseries_root, "root").split(os.path.sep) for d in dirs
     ]
-    ts_logger.debug(f"DATASET.IO.SEARCH: search_results{search_results}")
+    ts_logger.warning(
+        f"DATASET.IO.SEARCH: results:\n\tnew: {search_results}\n\told: {search_results_old}"
+    )
 
     return [SearchResult(f[2], f[1]) for f in search_results]
 
 
 class DatasetIoException(Exception):
     """Exception for dataset io errors."""
```

### Comparing `ssb_timeseries-0.2.2/src/ssb_timeseries/logging.py` & `ssb_timeseries-0.2.3/src/ssb_timeseries/logging.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Time series should make use of standardised messaging and logging.
 
 These are features that may warrant their own shared Dapla libraries. This module separates out code that could go into such a library.
 """
 
 import functools
 import logging
-import os
 from datetime import datetime
 
 from typing_extensions import Self
 
-from ssb_timeseries import config
+from ssb_timeseries.config import CONFIG
+from ssb_timeseries.config import CONFIGURATION_FILE
 from ssb_timeseries.types import F
 
+# nosonar: disable comment
 # import uuid
 # automatic cloud logging config
 # import google.cloud.logging
 # client = google.cloud.logging.Client()
 # client.setup_logging()
 
 # mypy: disable-error-code="operator, no-untyped-def, return-value, import-untyped, arg-type"
@@ -26,52 +27,41 @@
 log_string = logging.Formatter(
     "%(name)s | %(levelname)s | %(asctime)s | %(message)s \n"
 )
 log_json = logging.Formatter(
     '{"name": "%(name)s"; "level": %(levelname)s; "timestamp": %(asctime)s; "message": "%(message)s" }'
 )
 
-TIMESERIES_CONFIG = os.environ.get("TIMESERIES_CONFIG")
-CONFIG = config.Config(configuration_file=TIMESERIES_CONFIG)
+# nosonar: disable comment
+# CONFIGURATION_FILE = str(os.environ.get("TIMESERIES_CONFIG"))
+# CONFIG = Config(configuration_file=CONFIGURATION_FILE)
+LOG_FILE = str(CONFIG.log_file)
+
+# investigating conftest import error
+print(f"Configuration: {CONFIGURATION_FILE}. Log file: {LOG_FILE}")
+assert LOG_FILE != ""
 
-file_handler = logging.FileHandler(CONFIG.log_file)
+file_handler = logging.FileHandler(LOG_FILE)
 file_handler.setFormatter(log_json)
 file_handler.setLevel(logging.INFO)
 ts_logger.addHandler(file_handler)
 
 # Also log to console.
 console = logging.StreamHandler()
 console.setFormatter(log_string)  # BUG: format does not take effect in console?
 console.setLevel(logging.WARNING)
 ts_logger.addHandler(console)
 
+# nosonar: disable comment
 # Google Cloud logging:
 # from google.cloud.logging.handlers import CloudLoggingHandler
 # cloud_handler = CloudLoggingHandler(client)
 # ts_logger.addHandler(cloud_handler)
 
 
-# def warn(message: str) -> None:
-#     ts_logger.warning(message)
-#     # print(message)
-
-
-# def info(message: str) -> None:
-#     ts_logger.info(message)
-#     # print(message)
-
-
-# def debug(message: str) -> None:
-#     ts_logger.debug(message)
-#     # print(message)
-
-
-# F = TypeVar("F", bound=Callable[..., Any])
-
-
 class EnterExitLog:
     """Class supporting decorator to log on enter and exit."""
 
     def __init__(self, name: str) -> None:
         """Enter/exit template for workflow process."""
         self.name = name
 
@@ -88,63 +78,58 @@
         ts_logger.info(
             f"FINISH: {self.name}. Completed in: {self.elapsed_time} seconds."
         )
 
 
 def log_start_stop(func: F) -> F:
     """Log start and stop of decorated function."""
-    # TODO: generalise: pass in functions to enter/exit?
+    # nosonar  TODO: generalise: pass in functions to enter/exit?
 
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         with EnterExitLog(func.__name__):
             out = func(*args, **kwargs)
 
         return out
 
     return wrapper
 
 
+# nosonar disable comment
 # def debug(func):  # ANN001, ANN201
 #     """Print the function signature and return value."""
 
 #     @functools.wraps(func)
 #     def wrapper_debug(*args, **kwargs):
 #         args_repr = [repr(a) for a in args]  # 1
 #         kwargs_repr = [f"{k}={v!r}" for k, v in kwargs.items()]  # 2
 #         signature = ", ".join(args_repr + kwargs_repr)  # 3
 #         print(f"Calling {func.__name__}({signature})")
 #         value = func(*args, **kwargs)
 #         print(f"{func.__name__!r} returned {value!r}")  # 4
 #         return value
-
 #     return wrapper_debug
-
-
-"""
-
-# @wraps??
-class Timer:
-    def __init__(self, name: str):
-        self.name: str = name
-
-    def __enter__(self):
-        self.init_time = datetime.now()
-        ts_logger.info("Started: {self.name}.")
-        return self
-
-    def __exit__(self, type, value, tb):
-        self.end_time = datetime.now()
-        self.elapsed_time = self.end_time - self.init_time
-        ts_logger.info("Finished: {self.name} in: {self.elapsed_time} seconds.")
-
-
-def funcion_timer(func) -> Callable[..., Function]:
-    @functools.wraps(func)
-    def wrapper(*args, **kwargs) -> Function:
-        with Timer(func.__name__):
-            return func(*args, **kwargs)
-
-    return wrapper
-
-
-"""
+# """
+#
+# # @wraps??
+# class Timer:
+#     def __init__(self, name: str):
+#         self.name: str = name
+#
+#     def __enter__(self):
+#         self.init_time = datetime.now()
+#         ts_logger.info("Started: {self.name}.")
+#         return self
+#
+#     def __exit__(self, type, value, tb):
+#         self.end_time = datetime.now()
+#         self.elapsed_time = self.end_time - self.init_time
+#         ts_logger.info("Finished: {self.name} in: {self.elapsed_time} seconds.")
+#
+# def funcion_timer(func) -> Callable[..., Function]:
+#     @functools.wraps(func)
+#     def wrapper(*args, **kwargs) -> Function:
+#         with Timer(func.__name__):
+#             return func(*args, **kwargs)
+#
+#     return wrapper
+# """
```

### Comparing `ssb_timeseries-0.2.2/src/ssb_timeseries/meta.py` & `ssb_timeseries-0.2.3/src/ssb_timeseries/meta.py`

 * *Files identical despite different names*

### Comparing `ssb_timeseries-0.2.2/src/ssb_timeseries/properties.py` & `ssb_timeseries-0.2.3/src/ssb_timeseries/properties.py`

 * *Files identical despite different names*

### Comparing `ssb_timeseries-0.2.2/src/ssb_timeseries/sample_data.py` & `ssb_timeseries-0.2.3/src/ssb_timeseries/sample_data.py`

 * *Files identical despite different names*

### Comparing `ssb_timeseries-0.2.2/src/ssb_timeseries/sample_metadata.py` & `ssb_timeseries-0.2.3/src/ssb_timeseries/sample_metadata.py`

 * *Files identical despite different names*

### Comparing `ssb_timeseries-0.2.2/src/ssb_timeseries/setup.py` & `ssb_timeseries-0.2.3/src/ssb_timeseries/setup.py`

 * *Files identical despite different names*

### Comparing `ssb_timeseries-0.2.2/PKG-INFO` & `ssb_timeseries-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-timeseries
-Version: 0.2.2
+Version: 0.2.3
 Summary: SSB Timeseries
 Home-page: https://github.com/statisticsnorway/ssb-timeseries
 License: MIT
 Author: Bernhard Ryeng
 Author-email: bernhard.ryeng@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

