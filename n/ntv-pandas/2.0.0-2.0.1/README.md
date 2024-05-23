# Comparing `tmp/ntv_pandas-2.0.0.tar.gz` & `tmp/ntv_pandas-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntv_pandas-2.0.0.tar", last modified: Mon May  6 16:35:33 2024, max compression
+gzip compressed data, was "ntv_pandas-2.0.1.tar", last modified: Thu May 23 13:19:38 2024, max compression
```

## Comparing `ntv_pandas-2.0.0.tar` & `ntv_pandas-2.0.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 16:35:33.581950 ntv_pandas-2.0.0/
--rw-rw-rw-   0        0        0    11713 2024-05-06 16:35:33.581453 ntv_pandas-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    10847 2024-05-06 12:53:21.000000 ntv_pandas-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 16:35:33.569502 ntv_pandas-2.0.0/ntv_pandas/
--rw-rw-rw-   0        0        0     1273 2024-05-06 16:25:44.000000 ntv_pandas-2.0.0/ntv_pandas/__init__.py
--rw-rw-rw-   0        0        0     4567 2024-05-06 16:24:28.000000 ntv_pandas-2.0.0/ntv_pandas/accessors.py
--rw-rw-rw-   0        0        0     4309 2023-09-18 21:58:13.000000 ntv_pandas-2.0.0/ntv_pandas/ntv_pandas.ini
--rw-rw-rw-   0        0        0     3521 2023-10-07 19:49:27.000000 ntv_pandas-2.0.0/ntv_pandas/ntv_table.ini
--rw-rw-rw-   0        0        0    31621 2024-05-06 14:34:01.000000 ntv_pandas-2.0.0/ntv_pandas/pandas_ntv_connector.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:35:33.580457 ntv_pandas-2.0.0/ntv_pandas.egg-info/
--rw-rw-rw-   0        0        0    11713 2024-05-06 16:35:33.000000 ntv_pandas-2.0.0/ntv_pandas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2024-05-06 16:35:33.000000 ntv_pandas-2.0.0/ntv_pandas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 16:35:33.000000 ntv_pandas-2.0.0/ntv_pandas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-05-06 16:35:33.000000 ntv_pandas-2.0.0/ntv_pandas.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-06 16:35:33.000000 ntv_pandas-2.0.0/ntv_pandas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-05-06 16:35:33.582448 ntv_pandas-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1265 2024-05-06 14:10:16.000000 ntv_pandas-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:35:33.579461 ntv_pandas-2.0.0/tests/
--rw-rw-rw-   0        0        0    10601 2024-05-06 09:49:35.000000 ntv_pandas-2.0.0/tests/tests_ntv_pandas.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:19:38.830758 ntv_pandas-2.0.1/
+-rw-rw-rw-   0        0        0    11700 2024-05-23 13:19:38.830758 ntv_pandas-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10833 2024-05-21 09:06:20.000000 ntv_pandas-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 13:19:38.810845 ntv_pandas-2.0.1/ntv_pandas/
+-rw-rw-rw-   0        0        0     1413 2024-05-21 12:44:04.000000 ntv_pandas-2.0.1/ntv_pandas/__init__.py
+-rw-rw-rw-   0        0        0     4284 2024-05-21 09:06:20.000000 ntv_pandas-2.0.1/ntv_pandas/ntv_pandas.ini
+-rw-rw-rw-   0        0        0     3519 2024-05-21 09:06:20.000000 ntv_pandas-2.0.1/ntv_pandas/ntv_table.ini
+-rw-rw-rw-   0        0        0     4518 2024-05-21 09:06:21.000000 ntv_pandas-2.0.1/ntv_pandas/pandas_accessors.py
+-rw-rw-rw-   0        0        0    32264 2024-05-21 09:06:21.000000 ntv_pandas-2.0.1/ntv_pandas/pandas_ntv_connector.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:19:38.829765 ntv_pandas-2.0.1/ntv_pandas.egg-info/
+-rw-rw-rw-   0        0        0    11700 2024-05-23 13:19:38.000000 ntv_pandas-2.0.1/ntv_pandas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2024-05-23 13:19:38.000000 ntv_pandas-2.0.1/ntv_pandas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 13:19:38.000000 ntv_pandas-2.0.1/ntv_pandas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-05-23 13:19:38.000000 ntv_pandas-2.0.1/ntv_pandas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-23 13:19:38.000000 ntv_pandas-2.0.1/ntv_pandas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      368 2024-05-21 08:07:05.000000 ntv_pandas-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2024-05-23 13:19:38.831756 ntv_pandas-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1345 2024-05-23 12:41:49.000000 ntv_pandas-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:19:38.827277 ntv_pandas-2.0.1/tests/
+-rw-rw-rw-   0        0        0    14485 2024-05-21 09:06:21.000000 ntv_pandas-2.0.1/tests/tests_ntv_pandas.py
```

### Comparing `ntv_pandas-2.0.0/PKG-INFO` & `ntv_pandas-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ntv_pandas
-Version: 2.0.0
+Version: 2.0.1
 Summary: NTV-pandas : A tabular analyzer and a semantic, compact and reversible converter
 Home-page: https://github.com/loco-philippe/ntv-pandas/blob/main/README.md
 Author: Philippe Thomy
 Author-email: philippe@loco-labs.io
 Keywords: pandas,JSON-NTV,semantic JSON,development,environmental data
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9, <4
+Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 Requires-Dist: ntv_numpy
 Requires-Dist: tab_analysis
 Requires-Dist: tab_dataset
 Requires-Dist: json_ntv
 Requires-Dist: numpy
 Requires-Dist: pandas
@@ -66,38 +66,38 @@
 The DataFrame resulting from these conversions are identical to the initial DataFrame (reversibility).
 
 ```python
 In [1]: import pandas as pd
         import ntv_pandas as npd
 
 In [2]: fruits = {'plants':      ['fruit', 'fruit', 'fruit', 'fruit', 'vegetable', 'vegetable', 'vegetable', 'vegetable'],
-                  'plts':        ['fr', 'fr', 'fr', 'fr', 've', 've', 've', 've'], 
+                  'plts':        ['fr', 'fr', 'fr', 'fr', 've', 've', 've', 've'],
                   'quantity':    ['1 kg', '10 kg', '1 kg', '10 kg', '1 kg', '10 kg', '1 kg', '10 kg'],
                   'product':     ['apple', 'apple', 'orange', 'orange', 'peppers', 'peppers', 'carrot', 'carrot'],
                   'price':       [1, 10, 2, 20, 1.5, 15, 1.5, 20],
                   'price level': ['low', 'low', 'high', 'high', 'low', 'low', 'high', 'high'],
                   'group':       ['fruit 1', 'fruit 10', 'fruit 1', 'veget', 'veget', 'veget', 'veget', 'veget'],
                   'id':          [1001, 1002, 1003, 1004, 1005, 1006, 1007, 1008],
                   'supplier':    ["sup1", "sup1", "sup1", "sup2", "sup2", "sup2", "sup2", "sup1"],
                   'location':    ["fr", "gb", "es", "ch", "gb", "fr", "es", "ch"],
-                  'valid':       ["ok", "ok", "ok", "ok", "ok", "ok", "ok", "ok"]} 
+                  'valid':       ["ok", "ok", "ok", "ok", "ok", "ok", "ok", "ok"]}
         df_fruits = pd.DataFrame(fruits)
         df_fruits.npd.analysis(distr=True).partitions()   # return the list of partitions (a partition is a list of dimensions)
-Out[2]: 
+Out[2]:
         [['plants', 'quantity', 'price level'],
          ['quantity', 'price level', 'supplier'],
          ['plants', 'location'],
          ['quantity', 'product'],
          ['supplier', 'location'],
          ['id']]
 
 In [3]: kwargs = {'dims':['product', 'quantity'], 'datagroup': False, 'ntv_type': False, 'json_name': False}
         xd_fruits = df_fruits.npd.to_xarray(**kwargs)
         xd_fruits
-Out[3]: 
+Out[3]:
         <xarray.Dataset> Size: 976B
         Dimensions:      (product: 4, quantity: 2)
         Coordinates:
         * product      (product) <U7 112B 'apple' 'carrot' 'orange' 'peppers'
         * quantity     (quantity) <U5 40B '1 kg' '10 kg'
         plants       (product) <U9 144B 'fruit' 'vegetable' 'fruit' 'vegetable'
         plts         (product) <U2 32B 'fr' 've' 'fr' 've'
@@ -108,47 +108,47 @@
         id           (product, quantity) int64 64B 1001 1002 1007 ... 1004 1005 1006
         location     (product, quantity) <U2 64B 'fr' 'gb' 'es' ... 'ch' 'gb' 'fr'
         price        (product, quantity) float64 64B 1.0 10.0 1.5 ... 20.0 1.5 15.0
         supplier     (product, quantity) <U4 128B 'sup1' 'sup1' ... 'sup2' 'sup2'
 
 In [4]: sc_fruits = df_fruits.npd.to_scipp(**kwargs)
         sc_fruits
-Out[4]: 
+Out[4]:
         <scipp.Dataset>
         Dimensions: Sizes[product:4, quantity:2, ]
         Coordinates:
         * plants                     string  [dimensionless]  (product)  ["fruit", "vegetable", "fruit", "vegetable"]
         * plts                       string  [dimensionless]  (product)  ["fr", "ve", "fr", "ve"]
         * price level                string  [dimensionless]  (product)  ["low", "high", "high", "low"]
         * product                    string  [dimensionless]  (product)  ["apple", "carrot", "orange", "peppers"]
         * quantity                   string  [dimensionless]  (quantity) ["1 kg", "10 kg"]
         * valid                      string  [dimensionless]  ()  "ok"
         Data:
           group                      string  [dimensionless]  (product, quantity)  ["fruit 1", "fruit 10", ..., "veget", "veget"]
           id                          int64  [dimensionless]  (product, quantity)  [1001, 1002, ..., 1005, 1006]
           location                   string  [dimensionless]  (product, quantity)  ["fr", "gb", ..., "gb", "fr"]
           price                     float64  [dimensionless]  (product, quantity)  [1, 10, ..., 1.5, 15]
-          supplier                   string  [dimensionless]  (product, quantity)  ["sup1", "sup1", ..., "sup2", "sup2"]       
+          supplier                   string  [dimensionless]  (product, quantity)  ["sup1", "sup1", ..., "sup2", "sup2"]
 ```
 
 Reversibility:
 
 ```python
 In [5]: df_fruits_xd = npd.from_xarray(xd_fruits, **kwargs)
         df_fruits_xd_sort = df_fruits_xd.reset_index()[list(df_fruits.columns)].sort_values(list(df_fruits.columns)).reset_index(drop=True)
         df_fruits_sort = df_fruits.sort_values(list(df_fruits.columns)).reset_index(drop=True)
         df_fruits_xd_sort.equals(df_fruits_sort)
-Out[5]: 
+Out[5]:
         True
 
 In [6]: df_fruits_sc = npd.from_scipp(sc_fruits, **kwargs)
         df_fruits_sc_sort = df_fruits_sc.reset_index()[list(df_fruits.columns)].sort_values(list(df_fruits.columns)).reset_index(drop=True)
         df_fruits_sort = df_fruits.sort_values(list(df_fruits.columns)).reset_index(drop=True)
         df_fruits_sc_sort.equals(df_fruits_sort)
-Out[6]: 
+Out[6]:
         True
 ```
 
 ## JSON converter example
 
 In the example below, a DataFrame with multiple data types is converted to JSON (first to NTV format and then to Table Schema format).
```

### Comparing `ntv_pandas-2.0.0/README.md` & `ntv_pandas-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,38 +43,38 @@
 The DataFrame resulting from these conversions are identical to the initial DataFrame (reversibility).
 
 ```python
 In [1]: import pandas as pd
         import ntv_pandas as npd
 
 In [2]: fruits = {'plants':      ['fruit', 'fruit', 'fruit', 'fruit', 'vegetable', 'vegetable', 'vegetable', 'vegetable'],
-                  'plts':        ['fr', 'fr', 'fr', 'fr', 've', 've', 've', 've'], 
+                  'plts':        ['fr', 'fr', 'fr', 'fr', 've', 've', 've', 've'],
                   'quantity':    ['1 kg', '10 kg', '1 kg', '10 kg', '1 kg', '10 kg', '1 kg', '10 kg'],
                   'product':     ['apple', 'apple', 'orange', 'orange', 'peppers', 'peppers', 'carrot', 'carrot'],
                   'price':       [1, 10, 2, 20, 1.5, 15, 1.5, 20],
                   'price level': ['low', 'low', 'high', 'high', 'low', 'low', 'high', 'high'],
                   'group':       ['fruit 1', 'fruit 10', 'fruit 1', 'veget', 'veget', 'veget', 'veget', 'veget'],
                   'id':          [1001, 1002, 1003, 1004, 1005, 1006, 1007, 1008],
                   'supplier':    ["sup1", "sup1", "sup1", "sup2", "sup2", "sup2", "sup2", "sup1"],
                   'location':    ["fr", "gb", "es", "ch", "gb", "fr", "es", "ch"],
-                  'valid':       ["ok", "ok", "ok", "ok", "ok", "ok", "ok", "ok"]} 
+                  'valid':       ["ok", "ok", "ok", "ok", "ok", "ok", "ok", "ok"]}
         df_fruits = pd.DataFrame(fruits)
         df_fruits.npd.analysis(distr=True).partitions()   # return the list of partitions (a partition is a list of dimensions)
-Out[2]: 
+Out[2]:
         [['plants', 'quantity', 'price level'],
          ['quantity', 'price level', 'supplier'],
          ['plants', 'location'],
          ['quantity', 'product'],
          ['supplier', 'location'],
          ['id']]
 
 In [3]: kwargs = {'dims':['product', 'quantity'], 'datagroup': False, 'ntv_type': False, 'json_name': False}
         xd_fruits = df_fruits.npd.to_xarray(**kwargs)
         xd_fruits
-Out[3]: 
+Out[3]:
         <xarray.Dataset> Size: 976B
         Dimensions:      (product: 4, quantity: 2)
         Coordinates:
         * product      (product) <U7 112B 'apple' 'carrot' 'orange' 'peppers'
         * quantity     (quantity) <U5 40B '1 kg' '10 kg'
         plants       (product) <U9 144B 'fruit' 'vegetable' 'fruit' 'vegetable'
         plts         (product) <U2 32B 'fr' 've' 'fr' 've'
@@ -85,47 +85,47 @@
         id           (product, quantity) int64 64B 1001 1002 1007 ... 1004 1005 1006
         location     (product, quantity) <U2 64B 'fr' 'gb' 'es' ... 'ch' 'gb' 'fr'
         price        (product, quantity) float64 64B 1.0 10.0 1.5 ... 20.0 1.5 15.0
         supplier     (product, quantity) <U4 128B 'sup1' 'sup1' ... 'sup2' 'sup2'
 
 In [4]: sc_fruits = df_fruits.npd.to_scipp(**kwargs)
         sc_fruits
-Out[4]: 
+Out[4]:
         <scipp.Dataset>
         Dimensions: Sizes[product:4, quantity:2, ]
         Coordinates:
         * plants                     string  [dimensionless]  (product)  ["fruit", "vegetable", "fruit", "vegetable"]
         * plts                       string  [dimensionless]  (product)  ["fr", "ve", "fr", "ve"]
         * price level                string  [dimensionless]  (product)  ["low", "high", "high", "low"]
         * product                    string  [dimensionless]  (product)  ["apple", "carrot", "orange", "peppers"]
         * quantity                   string  [dimensionless]  (quantity) ["1 kg", "10 kg"]
         * valid                      string  [dimensionless]  ()  "ok"
         Data:
           group                      string  [dimensionless]  (product, quantity)  ["fruit 1", "fruit 10", ..., "veget", "veget"]
           id                          int64  [dimensionless]  (product, quantity)  [1001, 1002, ..., 1005, 1006]
           location                   string  [dimensionless]  (product, quantity)  ["fr", "gb", ..., "gb", "fr"]
           price                     float64  [dimensionless]  (product, quantity)  [1, 10, ..., 1.5, 15]
-          supplier                   string  [dimensionless]  (product, quantity)  ["sup1", "sup1", ..., "sup2", "sup2"]       
+          supplier                   string  [dimensionless]  (product, quantity)  ["sup1", "sup1", ..., "sup2", "sup2"]
 ```
 
 Reversibility:
 
 ```python
 In [5]: df_fruits_xd = npd.from_xarray(xd_fruits, **kwargs)
         df_fruits_xd_sort = df_fruits_xd.reset_index()[list(df_fruits.columns)].sort_values(list(df_fruits.columns)).reset_index(drop=True)
         df_fruits_sort = df_fruits.sort_values(list(df_fruits.columns)).reset_index(drop=True)
         df_fruits_xd_sort.equals(df_fruits_sort)
-Out[5]: 
+Out[5]:
         True
 
 In [6]: df_fruits_sc = npd.from_scipp(sc_fruits, **kwargs)
         df_fruits_sc_sort = df_fruits_sc.reset_index()[list(df_fruits.columns)].sort_values(list(df_fruits.columns)).reset_index(drop=True)
         df_fruits_sort = df_fruits.sort_values(list(df_fruits.columns)).reset_index(drop=True)
         df_fruits_sc_sort.equals(df_fruits_sort)
-Out[6]: 
+Out[6]:
         True
 ```
 
 ## JSON converter example
 
 In the example below, a DataFrame with multiple data types is converted to JSON (first to NTV format and then to Table Schema format).
```

### Comparing `ntv_pandas-2.0.0/ntv_pandas/__init__.py` & `ntv_pandas-2.0.1/ntv_pandas/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,19 +16,29 @@
     - `ntv-pandas.ntv_pandas.pandas_ntv_connector.to_json`
     - `ntv-pandas.ntv_pandas.pandas_ntv_connector.read_json`
     - `ntv-pandas.ntv_pandas.pandas_ntv_connector.analysis`
     - `ntv-pandas.ntv_pandas.pandas_ntv_connector.as_def_type`
     - `ntv-pandas.ntv_pandas.pandas_ntv_connector.equals`
 
 - `ntv-pandas.ntv_pandas.accessors` :
-    
+
     - `ntv-pandas.ntv_pandas.accessors.NpdSeriesAccessor`
-    - `ntv-pandas.ntv_pandas.accessors.NpdDataFrameAccessor`  
+    - `ntv-pandas.ntv_pandas.accessors.NpdDataFrameAccessor`
 """
+
 from ntv_pandas.pandas_ntv_connector import DataFrameConnec, SeriesConnec, read_json
 from ntv_pandas.pandas_ntv_connector import to_json, as_def_type, equals, to_analysis
 from ntv_pandas.pandas_ntv_connector import from_xarray, from_scipp
-import ntv_pandas.accessors
-
-#path = Path(ntv_pandas.pandas_ntv_connector.__file__).parent
+import ntv_pandas.pandas_accessors as pandas_accessors
 
-#print('package :', __package__)
+__all__ = [
+    "DataFrameConnec",
+    "SeriesConnec",
+    "read_json",
+    "to_json",
+    "as_def_type",
+    "equals",
+    "to_analysis",
+    "from_xarray",
+    "from_scipp",
+    "pandas_accessors",
+]
```

### Comparing `ntv_pandas-2.0.0/ntv_pandas/accessors.py` & `ntv_pandas-2.0.1/ntv_pandas/pandas_accessors.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Created on Sun Oct 8 2023
 
 @author: philippe@loco-labs.io
 
 
 Accessor methods bound to pd.Series.npd, pd.DataFrame.npd
 """
+
 import pandas as pd
 from tab_analysis import AnaDataset
 from ntv_numpy import Xdataset
 from ntv_pandas.pandas_ntv_connector import to_json, as_def_type, equals
 from ntv_pandas.pandas_ntv_connector import to_analysis, check_relation
 
 try:
@@ -29,16 +30,16 @@
 
     def analysis(self, distr=False):
         """Accessor for method `tab_analysis.AnaDataset` applied with
         `pandas_ntv_connector.to_analysis` invoked as `pd.DataFrame.npd.analysis`"""
         return AnaDataset(to_analysis(self._obj, distr))
 
     def check_relation(self, parent, child, typecoupl, value=True):
-        ''' Accessor for method `pandas_ntv_connector.check_relation` invoket as
-        `pd.DataFrame.npd.check_relation`'''
+        """Accessor for method `pandas_ntv_connector.check_relation` invoket as
+        `pd.DataFrame.npd.check_relation`"""
         return check_relation(self._obj, parent, child, typecoupl, value)
 
     def to_json(self, **kwargs):
         """Accessor for method `pandas_ntv_connector.to_json` invoked as
         `pd.DataFrame.npd.to_json`
 
         *parameters*
@@ -64,31 +65,30 @@
     def to_xarray(self, **kwargs):
         """Accessor for method `Xdataset.from_dataframe.to_xarray` invoked as
         `pd.DataFrame.npd.to_xarray`.
 
         *Parameters*
 
         - **dims**: list of string (default None) - order of dimensions to apply
-        - **dataset**: Boolean (default True) - if False and a single data_var,
-        return a sc.DataArray
-        - **datagroup**: Boolean (default True) - if True, return a sc.DataGroup
-        which contains the sc.DataArray/sc.Dataset and the other data else only
-        sc.DataArray/sc.Dataset"""
+        - **dataset** : Boolean (default True) - if False and a single data_var,
+        return a xr.DataArray
+        - **info** : Boolean (default True) - if True, add json representation
+        of 'relative' Xndarrays and 'data_arrays' Xndarrays in attrs"""
         return Xdataset.from_dataframe(self._obj, **kwargs).to_xarray(**kwargs)
 
     def to_scipp(self, **kwargs):
         """Accessor for method `Xdataset.from_dataframe.to_scipp` invoked as
         `pd.DataFrame.npd.to_scipp`.
 
         *Parameters*
 
         - **dims**: list of string (default None) - order of dimensions to apply
         - **dataset**: Boolean (default True) - if False and a single data_var,
         return a DataArray
-        - **datagroup**: Boolean (default True) - if True return a DataGroup with
+        - **info**: Boolean (default True) - if True return a DataGroup with
         metadata and data_arrays
         - **ntv_type**: Boolean (default True) - if True add ntv-type to the name"""
         return Xdataset.from_dataframe(self._obj, **kwargs).to_scipp(**kwargs)
 
 
 try:
     # delete the accessor to avoid warning
```

### Comparing `ntv_pandas-2.0.0/ntv_pandas/ntv_pandas.ini` & `ntv_pandas-2.0.1/ntv_pandas/ntv_pandas.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,270 +1,268 @@
 00000000: 5b64 6174 615d 0d0a 0d0a 2320 6465 6669  [data]....# defi
 00000010: 6e65 2074 6865 2063 6174 6567 6f72 6965  ne the categorie
 00000020: 7320 6f66 2064 6174 6120 6465 6669 6e65  s of data define
 00000030: 6420 696e 2027 7479 7065 270d 0a63 6f6c  d in 'type'..col
-00000040: 756d 6e20 3d20 5b0d 0a20 2020 200d 0a20  umn = [..    .. 
-00000050: 2020 2023 2027 6e74 765f 7479 7065 2720     # 'ntv_type' 
-00000060: 6973 2074 6865 2074 7970 6520 6f66 2074  is the type of t
-00000070: 6865 2064 6174 6120 0d0a 2020 2020 226e  he data ..    "n
-00000080: 7476 5f74 7970 6522 2c20 0d0a 2020 2020  tv_type", ..    
-00000090: 0d0a 2020 2020 2320 276e 616d 655f 7479  ..    # 'name_ty
-000000a0: 7065 2720 6973 2074 6865 2064 6174 6120  pe' is the data 
-000000b0: 6164 6465 6420 746f 2074 6865 2053 6572  added to the Ser
-000000c0: 6965 7320 6e61 6d65 0d0a 2020 2020 226e  ies name..    "n
-000000d0: 616d 655f 7479 7065 222c 200d 0a20 2020  ame_type", ..   
-000000e0: 200d 0a20 2020 2023 2027 6474 7970 6527   ..    # 'dtype'
-000000f0: 2069 7320 7573 6564 2074 6f20 6465 6669   is used to defi
-00000100: 6e65 2074 6865 2064 7479 7065 206f 6620  ne the dtype of 
-00000110: 7468 6520 5365 7269 6573 2c20 6966 2027  the Series, if '
-00000120: 6e75 6c6c 2720 7061 6e64 6173 2063 686f  null' pandas cho
-00000130: 6f73 6520 7468 6520 6474 7970 650d 0a20  ose the dtype.. 
-00000140: 2020 2022 6474 7970 6522 5d0d 0a0d 0a23     "dtype"]....#
-00000150: 2064 6566 696e 6520 7468 6520 7479 7065   define the type
-00000160: 7320 7769 7468 2061 2070 616e 6461 7320  s with a pandas 
-00000170: 636f 6e76 6572 7369 6f6e 0d0a 7479 7065  conversion..type
-00000180: 2020 203d 205b 0d0a 0d0a 2020 2020 2320     = [....    # 
-00000190: 7769 7468 6f75 7420 6e74 765f 7479 7065  without ntv_type
-000001a0: 200d 0a20 2020 2023 2020 2020 2064 7479   ..    #     dty
-000001b0: 7065 203a 2027 696e 7436 3427 2c20 2766  pe : 'int64', 'f
-000001c0: 6c6f 6174 3634 272c 2027 626f 6f6c 6561  loat64', 'boolea
-000001d0: 6e27 2c20 0d0a 2020 2020 2320 2020 2020  n', ..    #     
-000001e0: 2020 2020 2020 2020 276f 626a 6563 7420          'object 
-000001f0: 286a 736f 6e2d 6172 7261 792c 206a 736f  (json-array, jso
-00000200: 6e2d 6f62 6a65 6374 2927 0d0a 2020 2020  n-object)'..    
-00000210: 5b22 222c 0909 2020 2020 6e75 6c6c 2c20  ["",..    null, 
-00000220: 2020 2020 2020 6e75 6c6c 2020 2020 2020        null      
-00000230: 2020 2020 2020 2020 2020 5d2c 0d0a 0d0a            ],....
-00000240: 2020 2020 2320 7769 7468 206e 7476 5f74      # with ntv_t
-00000250: 7970 6520 6f6e 6c79 2069 6e20 6a73 6f6e  ype only in json
-00000260: 2064 6174 6120 286e 6f74 206e 756d 6265   data (not numbe
-00000270: 7273 2920 2020 200d 0a20 2020 205b 2264  rs)    ..    ["d
-00000280: 7572 6174 696f 6e22 2c09 6e75 6c6c 2c09  uration",.null,.
-00000290: 2020 2020 2274 696d 6564 656c 7461 3634      "timedelta64
-000002a0: 5b6e 735d 2220 2020 5d2c 0d0a 2020 2020  [ns]"   ],..    
-000002b0: 5b22 6461 7465 7469 6d65 222c 096e 756c  ["datetime",.nul
-000002c0: 6c2c 0920 2020 2022 6461 7465 7469 6d65  l,.    "datetime
-000002d0: 3634 5b6e 735d 2220 2020 205d 2c0d 0a20  64[ns]"    ],.. 
-000002e0: 2020 205b 2273 7472 696e 6722 2c09 2020     ["string",.  
-000002f0: 2020 6e75 6c6c 2c09 2020 2020 2273 7472    null,.    "str
-00000300: 696e 6722 2020 2020 2020 2020 2020 2020  ing"            
-00000310: 5d2c 0d0a 2020 2020 5b22 6a73 6f6e 222c  ],..    ["json",
-00000320: 0920 2020 206e 756c 6c2c 2009 2020 2020  .    null, .    
-00000330: 6e75 6c6c 2020 2020 2020 2020 2020 2020  null            
-00000340: 2020 2020 5d2c 0d0a 0d0a 2020 2020 2320      ],....    # 
-00000350: 7769 7468 206e 7476 5f74 7970 6520 6f6e  with ntv_type on
-00000360: 6c79 2069 6e20 6a73 6f6e 2064 6174 6120  ly in json data 
-00000370: 286e 756d 6265 7273 2920 2020 200d 0a20  (numbers)    .. 
-00000380: 2020 205b 2266 6c6f 6174 3136 222c 0920     ["float16",. 
-00000390: 2020 206e 756c 6c2c 0920 2020 2022 466c     null,.    "Fl
-000003a0: 6f61 7431 3622 2020 2020 2020 2020 2020  oat16"          
-000003b0: 205d 2c0d 0a20 2020 205b 2266 6c6f 6174   ],..    ["float
-000003c0: 3332 222c 0920 2020 206e 756c 6c2c 0920  32",.    null,. 
-000003d0: 2020 2022 466c 6f61 7433 3222 2020 2020     "Float32"    
-000003e0: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
-000003f0: 2275 696e 7438 222c 0920 2020 206e 756c  "uint8",.    nul
-00000400: 6c2c 0920 2020 2022 5549 6e74 3822 2020  l,.    "UInt8"  
-00000410: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
-00000420: 2020 205b 2275 696e 7431 3622 2c09 2020     ["uint16",.  
-00000430: 2020 6e75 6c6c 2c09 2020 2020 2255 496e    null,.    "UIn
-00000440: 7431 3622 2020 2020 2020 2020 2020 2020  t16"            
-00000450: 5d2c 0d0a 2020 2020 5b22 7569 6e74 3332  ],..    ["uint32
-00000460: 222c 0920 2020 206e 756c 6c2c 0920 2020  ",.    null,.   
-00000470: 2022 5549 6e74 3332 2220 2020 2020 2020   "UInt32"       
-00000480: 2020 2020 205d 2c0d 0a20 2020 205b 2275       ],..    ["u
-00000490: 696e 7436 3422 2c09 2020 2020 6e75 6c6c  int64",.    null
-000004a0: 2c20 0920 2020 2022 5549 6e74 3634 2220  , .    "UInt64" 
-000004b0: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
-000004c0: 2020 205b 2269 6e74 3822 2c09 2020 2020     ["int8",.    
-000004d0: 6e75 6c6c 2c09 2020 2020 2249 6e74 3822  null,.    "Int8"
-000004e0: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
-000004f0: 0d0a 2020 2020 5b22 696e 7431 3622 2c09  ..    ["int16",.
-00000500: 2020 2020 6e75 6c6c 2c09 2020 2020 2249      null,.    "I
-00000510: 6e74 3136 2220 2020 2020 2020 2020 2020  nt16"           
-00000520: 2020 5d2c 0d0a 2020 2020 5b22 696e 7433    ],..    ["int3
-00000530: 3222 2c09 2020 2020 6e75 6c6c 2c09 2020  2",.    null,.  
-00000540: 2020 2249 6e74 3332 2220 2020 2020 2020    "Int32"       
-00000550: 2020 2020 2020 5d2c 0d0a 0d0a 2020 2020        ],....    
-00000560: 2320 7769 7468 206e 7476 5f74 7970 6520  # with ntv_type 
-00000570: 696e 2053 6572 6965 7320 6e61 6d65 2061  in Series name a
-00000580: 6e64 2069 6e20 6a73 6f6e 2064 6174 6120  nd in json data 
-00000590: 286e 756d 6265 7273 290d 0a20 2020 205b  (numbers)..    [
-000005a0: 2269 6e74 222c 0920 2020 2020 2020 2022  "int",.        "
-000005b0: 696e 7422 2c09 2020 2020 2249 6e74 3634  int",.    "Int64
-000005c0: 2220 2020 2020 2020 2020 2020 2020 5d2c  "             ],
-000005d0: 0d0a 2020 2020 5b22 666c 6f61 7422 2c09  ..    ["float",.
-000005e0: 2020 2020 2266 6c6f 6174 222c 0922 466c      "float",."Fl
-000005f0: 6f61 7436 3422 2020 2020 2020 2020 2020  oat64"          
-00000600: 205d 2c0d 0a20 2020 205b 226e 756d 6265   ],..    ["numbe
-00000610: 7222 2c09 2020 2020 226e 756d 6265 7222  r",.    "number"
-00000620: 2c09 2246 6c6f 6174 3634 2220 2020 2020  ,."Float64"     
-00000630: 2020 2020 2020 5d2c 0d0a 2020 2020 5b22        ],..    ["
-00000640: 696e 7436 3422 2c20 2020 2020 2020 2269  int64",       "i
-00000650: 6e74 3634 222c 0922 496e 7436 3422 2020  nt64",."Int64"  
-00000660: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
-00000670: 2020 205b 2266 6c6f 6174 3634 222c 0920     ["float64",. 
-00000680: 2020 2022 666c 6f61 7436 3422 2c09 2246     "float64",."F
-00000690: 6c6f 6174 3634 2220 2020 2020 2020 2020  loat64"         
-000006a0: 2020 5d2c 0d0a 2020 2020 5b22 626f 6f6c    ],..    ["bool
-000006b0: 6561 6e22 2c09 2020 2020 2262 6f6f 6c65  ean",.    "boole
-000006c0: 616e 222c 0922 626f 6f6c 6561 6e22 2020  an",."boolean"  
-000006d0: 2020 2020 2020 2020 205d 2c0d 0a0d 0a20           ],.... 
-000006e0: 2020 2023 2077 6974 6820 6e74 765f 7479     # with ntv_ty
-000006f0: 7065 2069 6e20 5365 7269 6573 206e 616d  pe in Series nam
-00000700: 6520 616e 6420 696e 206a 736f 6e20 6461  e and in json da
-00000710: 7461 2028 6e6f 7420 6e75 6d62 6572 7329  ta (not numbers)
-00000720: 0d0a 2020 2020 5b22 6172 7261 7922 2c09  ..    ["array",.
-00000730: 2020 2020 2261 7272 6179 222c 0922 6f62      "array",."ob
-00000740: 6a65 6374 2220 2020 2020 2020 2020 2020  ject"           
-00000750: 205d 2c0d 0a20 2020 205b 226f 626a 6563   ],..    ["objec
-00000760: 7422 2c09 2020 2020 226f 626a 6563 7422  t",.    "object"
-00000770: 2c09 226f 626a 6563 7422 2020 2020 2020  ,."object"      
-00000780: 2020 2020 2020 5d2c 0d0a 2020 2020 5b22        ],..    ["
-00000790: 6e75 6c6c 222c 0920 2020 2022 6e75 6c6c  null",.    "null
-000007a0: 222c 2009 226f 626a 6563 7422 2020 2020  ", ."object"    
-000007b0: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
-000007c0: 5b22 7065 7269 6f64 222c 0920 2020 2022  ["period",.    "
-000007d0: 7065 7269 6f64 222c 0922 7374 7269 6e67  period",."string
-000007e0: 2220 2020 2020 2020 2020 2020 205d 2c0d  "            ],.
-000007f0: 0a20 2020 205b 2275 7269 222c 0920 2020  .    ["uri",.   
-00000800: 2020 2020 2022 7572 6922 2c09 2020 2020       "uri",.    
-00000810: 2273 7472 696e 6722 2020 2020 2020 2020  "string"        
-00000820: 2020 2020 5d2c 0d0a 2020 2020 5b22 656d      ],..    ["em
-00000830: 6169 6c22 2c09 2020 2020 2265 6d61 696c  ail",.    "email
-00000840: 222c 0922 7374 7269 6e67 2220 2020 2020  ",."string"     
-00000850: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
-00000860: 2266 696c 6522 2c09 2020 2020 2266 696c  "file",.    "fil
-00000870: 6522 2c09 2020 2020 2273 7472 696e 6722  e",.    "string"
-00000880: 2020 2020 2020 2020 2020 2020 5d2c 0d0a              ],..
-00000890: 0d0a 2020 2020 2320 7769 7468 206e 7476  ..    # with ntv
-000008a0: 5f74 7970 6520 636f 6e76 6572 7465 6420  _type converted 
-000008b0: 696e 206f 626a 6563 7420 6474 7970 650d  in object dtype.
-000008c0: 0a20 2020 205b 2264 6174 6522 2c09 2020  .    ["date",.  
-000008d0: 2020 2264 6174 6522 2c09 2020 2020 226f    "date",.    "o
-000008e0: 626a 6563 7422 2020 2020 2020 2020 2020  bject"          
-000008f0: 2020 5d2c 200d 0a20 2020 205b 2274 696d    ], ..    ["tim
-00000900: 6522 2c09 2020 2020 2274 696d 6522 2c09  e",.    "time",.
-00000910: 2020 2020 226f 626a 6563 7422 2020 2020      "object"    
-00000920: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
-00000930: 5b22 706f 696e 7422 2c09 2020 2020 2270  ["point",.    "p
-00000940: 6f69 6e74 222c 0922 6f62 6a65 6374 2220  oint",."object" 
-00000950: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
-00000960: 2020 205b 226c 696e 6522 2c09 2020 2020     ["line",.    
-00000970: 226c 696e 6522 2c09 2020 2020 226f 626a  "line",.    "obj
-00000980: 6563 7422 2020 2020 2020 2020 2020 2020  ect"            
-00000990: 5d2c 0d0a 2020 2020 5b22 706f 6c79 676f  ],..    ["polygo
-000009a0: 6e22 2c09 2020 2020 2270 6f6c 7967 6f6e  n",.    "polygon
-000009b0: 222c 0922 6f62 6a65 6374 2220 2020 2020  ",."object"     
-000009c0: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
-000009d0: 2267 656f 6d65 7472 7922 2c20 2020 2022  "geometry",    "
-000009e0: 6765 6f6d 6574 7279 222c 0922 6f62 6a65  geometry",."obje
-000009f0: 6374 2220 2020 2020 2020 2020 2020 205d  ct"            ]
-00000a00: 2c0d 0a20 2020 205b 2267 656f 6a73 6f6e  ,..    ["geojson
-00000a10: 222c 0920 2020 2022 6765 6f6a 736f 6e22  ",.    "geojson"
-00000a20: 2c09 226f 626a 6563 7422 2020 2020 2020  ,."object"      
-00000a30: 2020 2020 2020 5d2c 0d0a 0d0a 2020 2020        ],....    
-00000a40: 2320 7769 7468 206e 7476 5f74 7970 6520  # with ntv_type 
-00000a50: 756e 6b6e 6f77 6e20 696e 2070 616e 6461  unknown in panda
-00000a60: 730d 0a20 2020 205b 226d 6f6e 7468 222c  s..    ["month",
-00000a70: 0920 2020 2022 6d6f 6e74 6822 2c09 6e75  .    "month",.nu
-00000a80: 6c6c 2020 2020 2020 2020 2020 2020 2020  ll              
-00000a90: 2020 5d2c 0d0a 2020 2020 5b22 7965 6172    ],..    ["year
-00000aa0: 222c 0920 2020 2022 7965 6172 222c 0920  ",.    "year",. 
-00000ab0: 2020 206e 756c 6c20 2020 2020 2020 2020     null         
-00000ac0: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
-00000ad0: 2264 6179 222c 0920 2020 2020 2020 2022  "day",.        "
-00000ae0: 6461 7922 2c09 2020 2020 6e75 6c6c 2020  day",.    null  
-00000af0: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
-00000b00: 0d0a 2020 2020 5b22 7764 6179 222c 0920  ..    ["wday",. 
-00000b10: 2020 2022 7764 6179 222c 0920 2020 206e     "wday",.    n
-00000b20: 756c 6c20 2020 2020 2020 2020 2020 2020  ull             
-00000b30: 2020 205d 2c0d 0a20 2020 205b 2279 6461     ],..    ["yda
-00000b40: 7922 2c09 2020 2020 2279 6461 7922 2c09  y",.    "yday",.
-00000b50: 2020 2020 6e75 6c6c 2020 2020 2020 2020      null        
-00000b60: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
-00000b70: 5b22 7765 656b 222c 0920 2020 2022 7765  ["week",.    "we
-00000b80: 656b 222c 0920 2020 206e 756c 6c20 2020  ek",.    null   
-00000b90: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
-00000ba0: 0a20 2020 205b 2268 6f75 7222 2c09 2020  .    ["hour",.  
-00000bb0: 2020 2268 6f75 7222 2c09 2020 2020 6e75    "hour",.    nu
-00000bc0: 6c6c 2020 2020 2020 2020 2020 2020 2020  ll              
-00000bd0: 2020 5d2c 0d0a 2020 2020 5b22 6d69 6e75    ],..    ["minu
-00000be0: 7465 222c 0920 2020 2022 6d69 6e75 7465  te",.    "minute
-00000bf0: 222c 096e 756c 6c20 2020 2020 2020 2020  ",.null         
-00000c00: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
-00000c10: 2273 6563 6f6e 6422 2c09 2020 2020 2273  "second",.    "s
-00000c20: 6563 6f6e 6422 2c09 6e75 6c6c 2020 2020  econd",.null    
-00000c30: 2020 2020 2020 2020 2020 2020 5d0d 0a20              ].. 
-00000c40: 2020 205d 0d0a 0d0a 2320 6465 6669 6e65     ]....# define
-00000c50: 2074 6865 2074 7970 6573 2077 6974 6820   the types with 
-00000c60: 6120 4e54 5620 636f 6e76 6572 7369 6f6e  a NTV conversion
-00000c70: 2028 276f 7468 6572 7479 7065 2720 6973   ('othertype' is
-00000c80: 206e 6f74 2075 7365 6429 0d0a 6f74 6865   not used)..othe
-00000c90: 7274 7970 6520 3d20 5b0d 0a20 2020 205b  rtype = [..    [
-00000ca0: 2264 6174 222c 0920 2020 2020 2020 2020  "dat",.         
-00000cb0: 2020 2022 6461 7422 2c09 2020 2020 2020     "dat",.      
-00000cc0: 2020 226f 626a 6563 7422 2020 2020 5d2c    "object"    ],
-00000cd0: 0d0a 2020 2020 5b22 6d75 6c74 6970 6f69  ..    ["multipoi
-00000ce0: 6e74 222c 0920 2020 2022 6d75 6c74 6970  nt",.    "multip
-00000cf0: 6f69 6e74 222c 2020 2022 6f62 6a65 6374  oint",   "object
-00000d00: 2220 2020 205d 2c0d 0a20 2020 205b 226d  "    ],..    ["m
-00000d10: 756c 7469 6c69 6e65 222c 0920 2020 2022  ultiline",.    "
-00000d20: 6d75 6c74 696c 696e 6522 2c20 2020 2022  multiline",    "
-00000d30: 6f62 6a65 6374 2220 2020 205d 2c0d 0a20  object"    ],.. 
-00000d40: 2020 205b 226d 756c 7469 706f 6c79 676f     ["multipolygo
-00000d50: 6e22 2c09 226d 756c 7469 706f 6c79 676f  n",."multipolygo
-00000d60: 6e22 2c09 226f 626a 6563 7422 2020 2020  n",."object"    
-00000d70: 5d2c 0d0a 2020 2020 5b22 626f 7822 2c09  ],..    ["box",.
-00000d80: 2020 2020 2020 2020 2020 2020 2262 6f78              "box
-00000d90: 222c 0920 2020 2020 2020 2022 6f62 6a65  ",.        "obje
-00000da0: 6374 2220 2020 205d 2c0d 0a20 2020 205b  ct"    ],..    [
-00000db0: 2263 6f64 656f 6c63 222c 0920 2020 2020  "codeolc",.     
-00000dc0: 2020 2022 636f 6465 6f6c 6322 2c09 2020     "codeolc",.  
-00000dd0: 2020 226f 626a 6563 7422 2020 2020 5d2c    "object"    ],
-00000de0: 0d0a 2020 2020 5b22 726f 7722 2c09 2020  ..    ["row",.  
-00000df0: 2020 2020 2020 2020 2020 2272 6f77 222c            "row",
-00000e00: 0920 2020 2020 2020 2022 6f62 6a65 6374  .        "object
-00000e10: 2220 2020 205d 2c0d 0a20 2020 205b 2266  "    ],..    ["f
-00000e20: 6965 6c64 222c 0920 2020 2020 2020 2022  ield",.        "
-00000e30: 6669 656c 6422 2c09 2020 2020 226f 626a  field",.    "obj
-00000e40: 6563 7422 2020 2020 5d2c 0d0a 2020 2020  ect"    ],..    
-00000e50: 5b22 7461 6222 2c09 2020 2020 2020 2020  ["tab",.        
-00000e60: 2020 2020 2274 6162 222c 0920 2020 2020      "tab",.     
-00000e70: 2020 2022 6f62 6a65 6374 2220 2020 205d     "object"    ]
-00000e80: 2c0d 0a20 2020 205b 226e 7476 222c 0920  ,..    ["ntv",. 
-00000e90: 2020 2020 2020 2020 2020 2022 6e74 7622             "ntv"
-00000ea0: 2c09 2020 2020 2020 2020 226f 626a 6563  ,.        "objec
-00000eb0: 7422 2020 2020 5d0d 0a20 2020 205d 0d0a  t"    ]..    ]..
-00000ec0: 0d0a 2320 6465 6669 6e65 2063 6f6e 7665  ..# define conve
-00000ed0: 7273 696f 6e20 6265 7477 6565 6e20 6465  rsion between de
-00000ee0: 6661 756c 7420 6474 7970 6520 616e 6420  fault dtype and 
-00000ef0: 616c 6961 7320 6474 7970 650d 0a61 7374  alias dtype..ast
-00000f00: 7970 6520 3d20 7b0d 0a0d 0a20 2020 2023  ype = {....    #
-00000f10: 2074 6865 2027 7661 6c75 6527 2069 7320   the 'value' is 
-00000f20: 7468 6520 616c 6961 7320 6474 7970 6520  the alias dtype 
-00000f30: 6f66 2074 6865 2027 6b65 7927 2064 7479  of the 'key' dty
-00000f40: 7065 0d0a 2020 2020 2275 696e 7438 223a  pe..    "uint8":
-00000f50: 2020 2020 2020 2020 2255 496e 7438 222c          "UInt8",
-00000f60: 0d0a 2020 2020 2275 696e 7431 3622 3a20  ..    "uint16": 
-00000f70: 2020 2020 2020 2255 496e 7431 3622 2c0d        "UInt16",.
-00000f80: 0a20 2020 2022 7569 6e74 3332 223a 2020  .    "uint32":  
-00000f90: 2020 2020 2022 5549 6e74 3332 222c 0d0a       "UInt32",..
-00000fa0: 2020 2020 2275 696e 7436 3422 3a20 2020      "uint64":   
-00000fb0: 2020 2020 2255 496e 7436 3422 2c0d 0a20      "UInt64",.. 
-00000fc0: 2020 2022 696e 7438 223a 2020 2020 2020     "int8":      
-00000fd0: 2020 2022 496e 7438 222c 0d0a 2020 2020     "Int8",..    
-00000fe0: 2269 6e74 3136 223a 2020 2020 2020 2020  "int16":        
-00000ff0: 2249 6e74 3136 222c 0d0a 2020 2020 2269  "Int16",..    "i
-00001000: 6e74 3332 223a 2020 2020 2020 2020 2249  nt32":        "I
-00001010: 6e74 3332 222c 0d0a 2020 2020 2269 6e74  nt32",..    "int
-00001020: 3634 223a 2020 2020 2020 2020 2249 6e74  64":        "Int
-00001030: 3634 222c 0d0a 2020 2020 2266 6c6f 6174  64",..    "float
-00001040: 3136 223a 2020 2020 2020 2246 6c6f 6174  16":      "Float
-00001050: 3136 222c 0d0a 2020 2020 2266 6c6f 6174  16",..    "float
-00001060: 3332 223a 2020 2020 2020 2246 6c6f 6174  32":      "Float
-00001070: 3332 222c 0d0a 2020 2020 2266 6c6f 6174  32",..    "float
-00001080: 3634 223a 2020 2020 2020 2246 6c6f 6174  64":      "Float
-00001090: 3634 222c 0d0a 2020 2020 2262 6f6f 6c22  64",..    "bool"
-000010a0: 3a20 2020 2020 2020 2020 2262 6f6f 6c65  :         "boole
-000010b0: 616e 220d 0a20 2020 207d 0d0a 0d0a 2320  an"..    }....# 
-000010c0: 7265 7061 6365 2028 5c77 2b29 202d 3e20  repace (\w+) -> 
-000010d0: 2224 3122 2c                             "$1",
+00000040: 756d 6e20 3d20 5b0d 0a0d 0a20 2020 2023  umn = [....    #
+00000050: 2027 6e74 765f 7479 7065 2720 6973 2074   'ntv_type' is t
+00000060: 6865 2074 7970 6520 6f66 2074 6865 2064  he type of the d
+00000070: 6174 610d 0a20 2020 2022 6e74 765f 7479  ata..    "ntv_ty
+00000080: 7065 222c 0d0a 0d0a 2020 2020 2320 276e  pe",....    # 'n
+00000090: 616d 655f 7479 7065 2720 6973 2074 6865  ame_type' is the
+000000a0: 2064 6174 6120 6164 6465 6420 746f 2074   data added to t
+000000b0: 6865 2053 6572 6965 7320 6e61 6d65 0d0a  he Series name..
+000000c0: 2020 2020 226e 616d 655f 7479 7065 222c      "name_type",
+000000d0: 0d0a 0d0a 2020 2020 2320 2764 7479 7065  ....    # 'dtype
+000000e0: 2720 6973 2075 7365 6420 746f 2064 6566  ' is used to def
+000000f0: 696e 6520 7468 6520 6474 7970 6520 6f66  ine the dtype of
+00000100: 2074 6865 2053 6572 6965 732c 2069 6620   the Series, if 
+00000110: 276e 756c 6c27 2070 616e 6461 7320 6368  'null' pandas ch
+00000120: 6f6f 7365 2074 6865 2064 7479 7065 0d0a  oose the dtype..
+00000130: 2020 2020 2264 7479 7065 225d 0d0a 0d0a      "dtype"]....
+00000140: 2320 6465 6669 6e65 2074 6865 2074 7970  # define the typ
+00000150: 6573 2077 6974 6820 6120 7061 6e64 6173  es with a pandas
+00000160: 2063 6f6e 7665 7273 696f 6e0d 0a74 7970   conversion..typ
+00000170: 6520 2020 3d20 5b0d 0a0d 0a20 2020 2023  e   = [....    #
+00000180: 2077 6974 686f 7574 206e 7476 5f74 7970   without ntv_typ
+00000190: 650d 0a20 2020 2023 2020 2020 2064 7479  e..    #     dty
+000001a0: 7065 203a 2027 696e 7436 3427 2c20 2766  pe : 'int64', 'f
+000001b0: 6c6f 6174 3634 272c 2027 626f 6f6c 6561  loat64', 'boolea
+000001c0: 6e27 2c0d 0a20 2020 2023 2020 2020 2020  n',..    #      
+000001d0: 2020 2020 2020 2027 6f62 6a65 6374 2028         'object (
+000001e0: 6a73 6f6e 2d61 7272 6179 2c20 6a73 6f6e  json-array, json
+000001f0: 2d6f 626a 6563 7429 270d 0a20 2020 205b  -object)'..    [
+00000200: 2222 2c09 0920 2020 206e 756c 6c2c 2020  "",..    null,  
+00000210: 2020 2020 206e 756c 6c20 2020 2020 2020       null       
+00000220: 2020 2020 2020 2020 205d 2c0d 0a0d 0a20           ],.... 
+00000230: 2020 2023 2077 6974 6820 6e74 765f 7479     # with ntv_ty
+00000240: 7065 206f 6e6c 7920 696e 206a 736f 6e20  pe only in json 
+00000250: 6461 7461 2028 6e6f 7420 6e75 6d62 6572  data (not number
+00000260: 7329 0d0a 2020 2020 5b22 6475 7261 7469  s)..    ["durati
+00000270: 6f6e 222c 096e 756c 6c2c 0920 2020 2022  on",.null,.    "
+00000280: 7469 6d65 6465 6c74 6136 345b 6e73 5d22  timedelta64[ns]"
+00000290: 2020 205d 2c0d 0a20 2020 205b 2264 6174     ],..    ["dat
+000002a0: 6574 696d 6522 2c09 6e75 6c6c 2c09 2020  etime",.null,.  
+000002b0: 2020 2264 6174 6574 696d 6536 345b 6e73    "datetime64[ns
+000002c0: 5d22 2020 2020 5d2c 0d0a 2020 2020 5b22  ]"    ],..    ["
+000002d0: 7374 7269 6e67 222c 0920 2020 206e 756c  string",.    nul
+000002e0: 6c2c 0920 2020 2022 7374 7269 6e67 2220  l,.    "string" 
+000002f0: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
+00000300: 2020 205b 226a 736f 6e22 2c09 2020 2020     ["json",.    
+00000310: 6e75 6c6c 2c20 0920 2020 206e 756c 6c20  null, .    null 
+00000320: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00000330: 2c0d 0a0d 0a20 2020 2023 2077 6974 6820  ,....    # with 
+00000340: 6e74 765f 7479 7065 206f 6e6c 7920 696e  ntv_type only in
+00000350: 206a 736f 6e20 6461 7461 2028 6e75 6d62   json data (numb
+00000360: 6572 7329 0d0a 2020 2020 5b22 666c 6f61  ers)..    ["floa
+00000370: 7431 3622 2c09 2020 2020 6e75 6c6c 2c09  t16",.    null,.
+00000380: 2020 2020 2246 6c6f 6174 3136 2220 2020      "Float16"   
+00000390: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
+000003a0: 5b22 666c 6f61 7433 3222 2c09 2020 2020  ["float32",.    
+000003b0: 6e75 6c6c 2c09 2020 2020 2246 6c6f 6174  null,.    "Float
+000003c0: 3332 2220 2020 2020 2020 2020 2020 5d2c  32"           ],
+000003d0: 0d0a 2020 2020 5b22 7569 6e74 3822 2c09  ..    ["uint8",.
+000003e0: 2020 2020 6e75 6c6c 2c09 2020 2020 2255      null,.    "U
+000003f0: 496e 7438 2220 2020 2020 2020 2020 2020  Int8"           
+00000400: 2020 5d2c 0d0a 2020 2020 5b22 7569 6e74    ],..    ["uint
+00000410: 3136 222c 0920 2020 206e 756c 6c2c 0920  16",.    null,. 
+00000420: 2020 2022 5549 6e74 3136 2220 2020 2020     "UInt16"     
+00000430: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
+00000440: 2275 696e 7433 3222 2c09 2020 2020 6e75  "uint32",.    nu
+00000450: 6c6c 2c09 2020 2020 2255 496e 7433 3222  ll,.    "UInt32"
+00000460: 2020 2020 2020 2020 2020 2020 5d2c 0d0a              ],..
+00000470: 2020 2020 5b22 7569 6e74 3634 222c 0920      ["uint64",. 
+00000480: 2020 206e 756c 6c2c 2009 2020 2020 2255     null, .    "U
+00000490: 496e 7436 3422 2020 2020 2020 2020 2020  Int64"          
+000004a0: 2020 5d2c 0d0a 2020 2020 5b22 696e 7438    ],..    ["int8
+000004b0: 222c 0920 2020 206e 756c 6c2c 0920 2020  ",.    null,.   
+000004c0: 2022 496e 7438 2220 2020 2020 2020 2020   "Int8"         
+000004d0: 2020 2020 205d 2c0d 0a20 2020 205b 2269       ],..    ["i
+000004e0: 6e74 3136 222c 0920 2020 206e 756c 6c2c  nt16",.    null,
+000004f0: 0920 2020 2022 496e 7431 3622 2020 2020  .    "Int16"    
+00000500: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
+00000510: 205b 2269 6e74 3332 222c 0920 2020 206e   ["int32",.    n
+00000520: 756c 6c2c 0920 2020 2022 496e 7433 3222  ull,.    "Int32"
+00000530: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
+00000540: 0a0d 0a20 2020 2023 2077 6974 6820 6e74  ...    # with nt
+00000550: 765f 7479 7065 2069 6e20 5365 7269 6573  v_type in Series
+00000560: 206e 616d 6520 616e 6420 696e 206a 736f   name and in jso
+00000570: 6e20 6461 7461 2028 6e75 6d62 6572 7329  n data (numbers)
+00000580: 0d0a 2020 2020 5b22 696e 7422 2c09 2020  ..    ["int",.  
+00000590: 2020 2020 2020 2269 6e74 222c 0920 2020        "int",.   
+000005a0: 2022 496e 7436 3422 2020 2020 2020 2020   "Int64"        
+000005b0: 2020 2020 205d 2c0d 0a20 2020 205b 2266       ],..    ["f
+000005c0: 6c6f 6174 222c 0920 2020 2022 666c 6f61  loat",.    "floa
+000005d0: 7422 2c09 2246 6c6f 6174 3634 2220 2020  t",."Float64"   
+000005e0: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
+000005f0: 5b22 6e75 6d62 6572 222c 0920 2020 2022  ["number",.    "
+00000600: 6e75 6d62 6572 222c 0922 466c 6f61 7436  number",."Float6
+00000610: 3422 2020 2020 2020 2020 2020 205d 2c0d  4"           ],.
+00000620: 0a20 2020 205b 2269 6e74 3634 222c 2020  .    ["int64",  
+00000630: 2020 2020 2022 696e 7436 3422 2c09 2249       "int64",."I
+00000640: 6e74 3634 2220 2020 2020 2020 2020 2020  nt64"           
+00000650: 2020 5d2c 0d0a 2020 2020 5b22 666c 6f61    ],..    ["floa
+00000660: 7436 3422 2c09 2020 2020 2266 6c6f 6174  t64",.    "float
+00000670: 3634 222c 0922 466c 6f61 7436 3422 2020  64",."Float64"  
+00000680: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
+00000690: 205b 2262 6f6f 6c65 616e 222c 0920 2020   ["boolean",.   
+000006a0: 2022 626f 6f6c 6561 6e22 2c09 2262 6f6f   "boolean",."boo
+000006b0: 6c65 616e 2220 2020 2020 2020 2020 2020  lean"           
+000006c0: 5d2c 0d0a 0d0a 2020 2020 2320 7769 7468  ],....    # with
+000006d0: 206e 7476 5f74 7970 6520 696e 2053 6572   ntv_type in Ser
+000006e0: 6965 7320 6e61 6d65 2061 6e64 2069 6e20  ies name and in 
+000006f0: 6a73 6f6e 2064 6174 6120 286e 6f74 206e  json data (not n
+00000700: 756d 6265 7273 290d 0a20 2020 205b 2261  umbers)..    ["a
+00000710: 7272 6179 222c 0920 2020 2022 6172 7261  rray",.    "arra
+00000720: 7922 2c09 226f 626a 6563 7422 2020 2020  y",."object"    
+00000730: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
+00000740: 5b22 6f62 6a65 6374 222c 0920 2020 2022  ["object",.    "
+00000750: 6f62 6a65 6374 222c 0922 6f62 6a65 6374  object",."object
+00000760: 2220 2020 2020 2020 2020 2020 205d 2c0d  "            ],.
+00000770: 0a20 2020 205b 226e 756c 6c22 2c09 2020  .    ["null",.  
+00000780: 2020 226e 756c 6c22 2c20 0922 6f62 6a65    "null", ."obje
+00000790: 6374 2220 2020 2020 2020 2020 2020 205d  ct"            ]
+000007a0: 2c0d 0a20 2020 205b 2270 6572 696f 6422  ,..    ["period"
+000007b0: 2c09 2020 2020 2270 6572 696f 6422 2c09  ,.    "period",.
+000007c0: 2273 7472 696e 6722 2020 2020 2020 2020  "string"        
+000007d0: 2020 2020 5d2c 0d0a 2020 2020 5b22 7572      ],..    ["ur
+000007e0: 6922 2c09 2020 2020 2020 2020 2275 7269  i",.        "uri
+000007f0: 222c 0920 2020 2022 7374 7269 6e67 2220  ",.    "string" 
+00000800: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
+00000810: 2020 205b 2265 6d61 696c 222c 0920 2020     ["email",.   
+00000820: 2022 656d 6169 6c22 2c09 2273 7472 696e   "email",."strin
+00000830: 6722 2020 2020 2020 2020 2020 2020 5d2c  g"            ],
+00000840: 0d0a 2020 2020 5b22 6669 6c65 222c 0920  ..    ["file",. 
+00000850: 2020 2022 6669 6c65 222c 0920 2020 2022     "file",.    "
+00000860: 7374 7269 6e67 2220 2020 2020 2020 2020  string"         
+00000870: 2020 205d 2c0d 0a0d 0a20 2020 2023 2077     ],....    # w
+00000880: 6974 6820 6e74 765f 7479 7065 2063 6f6e  ith ntv_type con
+00000890: 7665 7274 6564 2069 6e20 6f62 6a65 6374  verted in object
+000008a0: 2064 7479 7065 0d0a 2020 2020 5b22 6461   dtype..    ["da
+000008b0: 7465 222c 0920 2020 2022 6461 7465 222c  te",.    "date",
+000008c0: 0920 2020 2022 6f62 6a65 6374 2220 2020  .    "object"   
+000008d0: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
+000008e0: 205b 2274 696d 6522 2c09 2020 2020 2274   ["time",.    "t
+000008f0: 696d 6522 2c09 2020 2020 226f 626a 6563  ime",.    "objec
+00000900: 7422 2020 2020 2020 2020 2020 2020 5d2c  t"            ],
+00000910: 0d0a 2020 2020 5b22 706f 696e 7422 2c09  ..    ["point",.
+00000920: 2020 2020 2270 6f69 6e74 222c 0922 6f62      "point",."ob
+00000930: 6a65 6374 2220 2020 2020 2020 2020 2020  ject"           
+00000940: 205d 2c0d 0a20 2020 205b 226c 696e 6522   ],..    ["line"
+00000950: 2c09 2020 2020 226c 696e 6522 2c09 2020  ,.    "line",.  
+00000960: 2020 226f 626a 6563 7422 2020 2020 2020    "object"      
+00000970: 2020 2020 2020 5d2c 0d0a 2020 2020 5b22        ],..    ["
+00000980: 706f 6c79 676f 6e22 2c09 2020 2020 2270  polygon",.    "p
+00000990: 6f6c 7967 6f6e 222c 0922 6f62 6a65 6374  olygon",."object
+000009a0: 2220 2020 2020 2020 2020 2020 205d 2c0d  "            ],.
+000009b0: 0a20 2020 205b 2267 656f 6d65 7472 7922  .    ["geometry"
+000009c0: 2c20 2020 2022 6765 6f6d 6574 7279 222c  ,    "geometry",
+000009d0: 0922 6f62 6a65 6374 2220 2020 2020 2020  ."object"       
+000009e0: 2020 2020 205d 2c0d 0a20 2020 205b 2267       ],..    ["g
+000009f0: 656f 6a73 6f6e 222c 0920 2020 2022 6765  eojson",.    "ge
+00000a00: 6f6a 736f 6e22 2c09 226f 626a 6563 7422  ojson",."object"
+00000a10: 2020 2020 2020 2020 2020 2020 5d2c 0d0a              ],..
+00000a20: 0d0a 2020 2020 2320 7769 7468 206e 7476  ..    # with ntv
+00000a30: 5f74 7970 6520 756e 6b6e 6f77 6e20 696e  _type unknown in
+00000a40: 2070 616e 6461 730d 0a20 2020 205b 226d   pandas..    ["m
+00000a50: 6f6e 7468 222c 0920 2020 2022 6d6f 6e74  onth",.    "mont
+00000a60: 6822 2c09 6e75 6c6c 2020 2020 2020 2020  h",.null        
+00000a70: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
+00000a80: 5b22 7965 6172 222c 0920 2020 2022 7965  ["year",.    "ye
+00000a90: 6172 222c 0920 2020 206e 756c 6c20 2020  ar",.    null   
+00000aa0: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
+00000ab0: 0a20 2020 205b 2264 6179 222c 0920 2020  .    ["day",.   
+00000ac0: 2020 2020 2022 6461 7922 2c09 2020 2020       "day",.    
+00000ad0: 6e75 6c6c 2020 2020 2020 2020 2020 2020  null            
+00000ae0: 2020 2020 5d2c 0d0a 2020 2020 5b22 7764      ],..    ["wd
+00000af0: 6179 222c 0920 2020 2022 7764 6179 222c  ay",.    "wday",
+00000b00: 0920 2020 206e 756c 6c20 2020 2020 2020  .    null       
+00000b10: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
+00000b20: 205b 2279 6461 7922 2c09 2020 2020 2279   ["yday",.    "y
+00000b30: 6461 7922 2c09 2020 2020 6e75 6c6c 2020  day",.    null  
+00000b40: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
+00000b50: 0d0a 2020 2020 5b22 7765 656b 222c 0920  ..    ["week",. 
+00000b60: 2020 2022 7765 656b 222c 0920 2020 206e     "week",.    n
+00000b70: 756c 6c20 2020 2020 2020 2020 2020 2020  ull             
+00000b80: 2020 205d 2c0d 0a20 2020 205b 2268 6f75     ],..    ["hou
+00000b90: 7222 2c09 2020 2020 2268 6f75 7222 2c09  r",.    "hour",.
+00000ba0: 2020 2020 6e75 6c6c 2020 2020 2020 2020      null        
+00000bb0: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
+00000bc0: 5b22 6d69 6e75 7465 222c 0920 2020 2022  ["minute",.    "
+00000bd0: 6d69 6e75 7465 222c 096e 756c 6c20 2020  minute",.null   
+00000be0: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
+00000bf0: 0a20 2020 205b 2273 6563 6f6e 6422 2c09  .    ["second",.
+00000c00: 2020 2020 2273 6563 6f6e 6422 2c09 6e75      "second",.nu
+00000c10: 6c6c 2020 2020 2020 2020 2020 2020 2020  ll              
+00000c20: 2020 5d0d 0a20 2020 205d 0d0a 0d0a 2320    ]..    ]....# 
+00000c30: 6465 6669 6e65 2074 6865 2074 7970 6573  define the types
+00000c40: 2077 6974 6820 6120 4e54 5620 636f 6e76   with a NTV conv
+00000c50: 6572 7369 6f6e 2028 276f 7468 6572 7479  ersion ('otherty
+00000c60: 7065 2720 6973 206e 6f74 2075 7365 6429  pe' is not used)
+00000c70: 0d0a 6f74 6865 7274 7970 6520 3d20 5b0d  ..othertype = [.
+00000c80: 0a20 2020 205b 2264 6174 222c 0920 2020  .    ["dat",.   
+00000c90: 2020 2020 2020 2020 2022 6461 7422 2c09           "dat",.
+00000ca0: 2020 2020 2020 2020 226f 626a 6563 7422          "object"
+00000cb0: 2020 2020 5d2c 0d0a 2020 2020 5b22 6d75      ],..    ["mu
+00000cc0: 6c74 6970 6f69 6e74 222c 0920 2020 2022  ltipoint",.    "
+00000cd0: 6d75 6c74 6970 6f69 6e74 222c 2020 2022  multipoint",   "
+00000ce0: 6f62 6a65 6374 2220 2020 205d 2c0d 0a20  object"    ],.. 
+00000cf0: 2020 205b 226d 756c 7469 6c69 6e65 222c     ["multiline",
+00000d00: 0920 2020 2022 6d75 6c74 696c 696e 6522  .    "multiline"
+00000d10: 2c20 2020 2022 6f62 6a65 6374 2220 2020  ,    "object"   
+00000d20: 205d 2c0d 0a20 2020 205b 226d 756c 7469   ],..    ["multi
+00000d30: 706f 6c79 676f 6e22 2c09 226d 756c 7469  polygon",."multi
+00000d40: 706f 6c79 676f 6e22 2c09 226f 626a 6563  polygon",."objec
+00000d50: 7422 2020 2020 5d2c 0d0a 2020 2020 5b22  t"    ],..    ["
+00000d60: 626f 7822 2c09 2020 2020 2020 2020 2020  box",.          
+00000d70: 2020 2262 6f78 222c 0920 2020 2020 2020    "box",.       
+00000d80: 2022 6f62 6a65 6374 2220 2020 205d 2c0d   "object"    ],.
+00000d90: 0a20 2020 205b 2263 6f64 656f 6c63 222c  .    ["codeolc",
+00000da0: 0920 2020 2020 2020 2022 636f 6465 6f6c  .        "codeol
+00000db0: 6322 2c09 2020 2020 226f 626a 6563 7422  c",.    "object"
+00000dc0: 2020 2020 5d2c 0d0a 2020 2020 5b22 726f      ],..    ["ro
+00000dd0: 7722 2c09 2020 2020 2020 2020 2020 2020  w",.            
+00000de0: 2272 6f77 222c 0920 2020 2020 2020 2022  "row",.        "
+00000df0: 6f62 6a65 6374 2220 2020 205d 2c0d 0a20  object"    ],.. 
+00000e00: 2020 205b 2266 6965 6c64 222c 0920 2020     ["field",.   
+00000e10: 2020 2020 2022 6669 656c 6422 2c09 2020       "field",.  
+00000e20: 2020 226f 626a 6563 7422 2020 2020 5d2c    "object"    ],
+00000e30: 0d0a 2020 2020 5b22 7461 6222 2c09 2020  ..    ["tab",.  
+00000e40: 2020 2020 2020 2020 2020 2274 6162 222c            "tab",
+00000e50: 0920 2020 2020 2020 2022 6f62 6a65 6374  .        "object
+00000e60: 2220 2020 205d 2c0d 0a20 2020 205b 226e  "    ],..    ["n
+00000e70: 7476 222c 0920 2020 2020 2020 2020 2020  tv",.           
+00000e80: 2022 6e74 7622 2c09 2020 2020 2020 2020   "ntv",.        
+00000e90: 226f 626a 6563 7422 2020 2020 5d0d 0a20  "object"    ].. 
+00000ea0: 2020 205d 0d0a 0d0a 2320 6465 6669 6e65     ]....# define
+00000eb0: 2063 6f6e 7665 7273 696f 6e20 6265 7477   conversion betw
+00000ec0: 6565 6e20 6465 6661 756c 7420 6474 7970  een default dtyp
+00000ed0: 6520 616e 6420 616c 6961 7320 6474 7970  e and alias dtyp
+00000ee0: 650d 0a61 7374 7970 6520 3d20 7b0d 0a0d  e..astype = {...
+00000ef0: 0a20 2020 2023 2074 6865 2027 7661 6c75  .    # the 'valu
+00000f00: 6527 2069 7320 7468 6520 616c 6961 7320  e' is the alias 
+00000f10: 6474 7970 6520 6f66 2074 6865 2027 6b65  dtype of the 'ke
+00000f20: 7927 2064 7479 7065 0d0a 2020 2020 2275  y' dtype..    "u
+00000f30: 696e 7438 223a 2020 2020 2020 2020 2255  int8":        "U
+00000f40: 496e 7438 222c 0d0a 2020 2020 2275 696e  Int8",..    "uin
+00000f50: 7431 3622 3a20 2020 2020 2020 2255 496e  t16":       "UIn
+00000f60: 7431 3622 2c0d 0a20 2020 2022 7569 6e74  t16",..    "uint
+00000f70: 3332 223a 2020 2020 2020 2022 5549 6e74  32":       "UInt
+00000f80: 3332 222c 0d0a 2020 2020 2275 696e 7436  32",..    "uint6
+00000f90: 3422 3a20 2020 2020 2020 2255 496e 7436  4":       "UInt6
+00000fa0: 3422 2c0d 0a20 2020 2022 696e 7438 223a  4",..    "int8":
+00000fb0: 2020 2020 2020 2020 2022 496e 7438 222c           "Int8",
+00000fc0: 0d0a 2020 2020 2269 6e74 3136 223a 2020  ..    "int16":  
+00000fd0: 2020 2020 2020 2249 6e74 3136 222c 0d0a        "Int16",..
+00000fe0: 2020 2020 2269 6e74 3332 223a 2020 2020      "int32":    
+00000ff0: 2020 2020 2249 6e74 3332 222c 0d0a 2020      "Int32",..  
+00001000: 2020 2269 6e74 3634 223a 2020 2020 2020    "int64":      
+00001010: 2020 2249 6e74 3634 222c 0d0a 2020 2020    "Int64",..    
+00001020: 2266 6c6f 6174 3136 223a 2020 2020 2020  "float16":      
+00001030: 2246 6c6f 6174 3136 222c 0d0a 2020 2020  "Float16",..    
+00001040: 2266 6c6f 6174 3332 223a 2020 2020 2020  "float32":      
+00001050: 2246 6c6f 6174 3332 222c 0d0a 2020 2020  "Float32",..    
+00001060: 2266 6c6f 6174 3634 223a 2020 2020 2020  "float64":      
+00001070: 2246 6c6f 6174 3634 222c 0d0a 2020 2020  "Float64",..    
+00001080: 2262 6f6f 6c22 3a20 2020 2020 2020 2020  "bool":         
+00001090: 2262 6f6f 6c65 616e 220d 0a20 2020 207d  "boolean"..    }
+000010a0: 0d0a 0d0a 2320 7265 7061 6365 2028 5c77  ....# repace (\w
+000010b0: 2b29 202d 3e20 2224 3122 2c0a            +) -> "$1",.
```

### Comparing `ntv_pandas-2.0.0/ntv_pandas/ntv_table.ini` & `ntv_pandas-2.0.1/ntv_pandas/ntv_table.ini`

 * *Files 4% similar despite different names*

```diff
@@ -2,220 +2,219 @@
 00000010: 6e65 2074 6865 2063 6174 6567 6f72 6965  ne the categorie
 00000020: 7320 6f66 2064 6174 6120 6465 6669 6e65  s of data define
 00000030: 6420 696e 2027 7479 7065 270d 0a63 6f6c  d in 'type'..col
 00000040: 756d 6e20 3d20 5b22 6e74 765f 7479 7065  umn = ["ntv_type
 00000050: 222c 2022 666f 726d 6174 222c 2022 7479  ", "format", "ty
 00000060: 7065 225d 0d0a 2020 2020 2320 276e 7476  pe"]..    # 'ntv
 00000070: 5f74 7970 6527 2069 7320 7468 6520 7479  _type' is the ty
-00000080: 7065 206f 6620 7468 6520 6461 7461 200d  pe of the data .
-00000090: 0a20 2020 2023 2027 666f 726d 6174 2720  .    # 'format' 
-000000a0: 6973 2064 6566 696e 6564 2069 6e20 5461  is defined in Ta
-000000b0: 626c 6553 6368 656d 6120 7370 6563 6966  bleSchema specif
-000000c0: 6963 6174 696f 6e0d 0a20 2020 2023 2027  ication..    # '
-000000d0: 7479 7065 2720 6973 2064 6566 696e 6564  type' is defined
-000000e0: 2069 6e20 5461 626c 6553 6368 656d 6120   in TableSchema 
-000000f0: 7370 6563 6966 6963 6174 696f 6e0d 0a0d  specification...
-00000100: 0a23 206d 6170 7069 6e67 2062 6574 7765  .# mapping betwe
-00000110: 656e 204e 5456 7479 7065 2061 6e64 2054  en NTVtype and T
-00000120: 6162 6c65 5363 6865 6d61 0d0a 6d61 7070  ableSchema..mapp
-00000130: 696e 6720 3d20 5b0d 0a20 2020 2023 206e  ing = [..    # n
-00000140: 756d 6572 6963 616c 0d0a 2020 2020 5b22  umerical..    ["
-00000150: 696e 7422 2c09 2020 2020 2020 2020 2264  int",.        "d
-00000160: 6566 6175 6c74 222c 0920 2020 2022 696e  efault",.    "in
-00000170: 7465 6765 7222 2020 2020 5d2c 0d0a 2020  teger"    ],..  
-00000180: 2020 5b22 6e75 6d62 6572 222c 0920 2020    ["number",.   
-00000190: 2022 6465 6661 756c 7422 2c09 2020 2020   "default",.    
-000001a0: 226e 756d 6265 7222 2020 2020 205d 2c0d  "number"     ],.
-000001b0: 0a20 2020 205b 2262 6f6f 6c65 616e 222c  .    ["boolean",
-000001c0: 0920 2020 2022 6465 6661 756c 7422 2c09  .    "default",.
-000001d0: 2020 2020 2262 6f6f 6c65 616e 2220 2020      "boolean"   
-000001e0: 205d 2c0d 0a20 2020 2023 206a 736f 6e0d   ],..    # json.
-000001f0: 0a20 2020 205b 2273 7472 696e 6722 2c09  .    ["string",.
-00000200: 2020 2020 2264 6566 6175 6c74 222c 0920      "default",. 
-00000210: 2020 2022 7374 7269 6e67 2220 2020 2020     "string"     
-00000220: 5d2c 0d0a 2020 2020 5b22 7572 6922 2c09  ],..    ["uri",.
-00000230: 2020 2020 2020 2020 2275 7269 222c 0920          "uri",. 
-00000240: 2020 2020 2020 2022 7374 7269 6e67 2220         "string" 
-00000250: 2020 2020 5d2c 0d0a 2020 2020 5b22 656d      ],..    ["em
-00000260: 6169 6c22 2c09 2020 2020 2265 6d61 696c  ail",.    "email
-00000270: 222c 0920 2020 2022 7374 7269 6e67 2220  ",.    "string" 
-00000280: 2020 2020 5d2c 0d0a 2020 2020 5b22 6a73      ],..    ["js
-00000290: 6f6e 222c 0920 2020 2022 6465 6661 756c  on",.    "defaul
-000002a0: 7422 2c20 0920 2020 2022 6f62 6a65 6374  t", .    "object
-000002b0: 2220 2020 2020 5d2c 0d0a 2020 2020 5b22  "     ],..    ["
-000002c0: 6172 7261 7922 2c09 2020 2020 2264 6566  array",.    "def
-000002d0: 6175 6c74 222c 0920 2020 2022 6172 7261  ault",.    "arra
-000002e0: 7922 2020 2020 2020 5d2c 0d0a 2020 2020  y"      ],..    
-000002f0: 2320 6461 7461 7469 6f6e 0d0a 2020 2020  # datation..    
-00000300: 5b22 6475 7261 7469 6f6e 222c 0922 6465  ["duration",."de
-00000310: 6661 756c 7422 2c09 2020 2020 2264 7572  fault",.    "dur
-00000320: 6174 696f 6e22 2020 205d 2c0d 0a20 2020  ation"   ],..   
-00000330: 205b 2264 6174 6574 696d 6522 2c09 2264   ["datetime",."d
-00000340: 6566 6175 6c74 222c 0920 2020 2022 6461  efault",.    "da
-00000350: 7465 7469 6d65 2220 2020 5d2c 0d0a 2020  tetime"   ],..  
-00000360: 2020 5b22 6461 7465 222c 0920 2020 2022    ["date",.    "
-00000370: 6465 6661 756c 7422 2c09 2020 2020 2264  default",.    "d
-00000380: 6174 6522 2020 2020 2020 205d 2c20 0d0a  ate"       ], ..
-00000390: 2020 2020 5b22 7469 6d65 222c 0920 2020      ["time",.   
-000003a0: 2022 6465 6661 756c 7422 2c09 2020 2020   "default",.    
-000003b0: 2274 696d 6522 2020 2020 2020 205d 2c0d  "time"       ],.
-000003c0: 0a20 2020 205b 226d 6f6e 7468 222c 0920  .    ["month",. 
-000003d0: 2020 2022 6465 6661 756c 7422 2c09 2020     "default",.  
-000003e0: 2020 2279 6561 726d 6f6e 7468 2220 205d    "yearmonth"  ]
-000003f0: 2c0d 0a20 2020 205b 2279 6561 7222 2c09  ,..    ["year",.
-00000400: 2020 2020 2264 6566 6175 6c74 222c 0920      "default",. 
-00000410: 2020 2022 7965 6172 2220 2020 2020 2020     "year"       
-00000420: 5d2c 0d0a 2020 2020 2320 6c6f 6361 7469  ],..    # locati
-00000430: 6f6e 0d0a 2020 2020 5b22 706f 696e 7422  on..    ["point"
-00000440: 2c09 2020 2020 2261 7272 6179 222c 0920  ,.    "array",. 
-00000450: 2020 2022 6765 6f70 6f69 6e74 2220 2020     "geopoint"   
-00000460: 5d2c 0d0a 2020 2020 5b22 6765 6f6a 736f  ],..    ["geojso
-00000470: 6e22 2c09 2020 2020 2264 6566 6175 6c74  n",.    "default
-00000480: 222c 2020 0922 6765 6f6a 736f 6e22 2020  ",  ."geojson"  
-00000490: 2020 5d2c 0d0a 0d0a 2020 2020 2320 7479    ],....    # ty
-000004a0: 7065 7320 7769 7468 6f75 7420 5461 626c  pes without Tabl
-000004b0: 6553 6368 656d 6120 7370 6563 6966 6963  eSchema specific
-000004c0: 6174 696f 6e0d 0a20 2020 2023 206e 756d  ation..    # num
-000004d0: 6572 6963 616c 200d 0a20 2020 205b 2266  erical ..    ["f
-000004e0: 6c6f 6174 3634 222c 0920 2020 2022 666c  loat64",.    "fl
-000004f0: 6f61 7436 3422 2c09 226e 756d 6265 7222  oat64",."number"
-00000500: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-00000510: 205b 2266 6c6f 6174 222c 0920 2020 2022   ["float",.    "
-00000520: 666c 6f61 7422 2c09 226e 756d 6265 7222  float",."number"
-00000530: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-00000540: 205b 2266 6c6f 6174 3136 222c 0920 2020   ["float16",.   
-00000550: 2022 666c 6f61 7431 3622 2c09 226e 756d   "float16",."num
-00000560: 6265 7222 2020 2020 2020 2020 205d 2c0d  ber"         ],.
-00000570: 0a20 2020 205b 2266 6c6f 6174 3332 222c  .    ["float32",
-00000580: 0920 2020 2022 666c 6f61 7433 3222 2c09  .    "float32",.
-00000590: 226e 756d 6265 7222 2020 2020 2020 2020  "number"        
-000005a0: 205d 2c0d 0a20 2020 205b 2275 696e 7438   ],..    ["uint8
-000005b0: 222c 0920 2020 2022 7569 6e74 3822 2c09  ",.    "uint8",.
-000005c0: 2269 6e74 6567 6572 2220 2020 2020 2020  "integer"       
-000005d0: 205d 2c0d 0a20 2020 205b 2275 696e 7431   ],..    ["uint1
-000005e0: 3622 2c09 2020 2020 2275 696e 7431 3622  6",.    "uint16"
-000005f0: 2c09 2269 6e74 6567 6572 2220 2020 2020  ,."integer"     
-00000600: 2020 205d 2c0d 0a20 2020 205b 2275 696e     ],..    ["uin
-00000610: 7433 3222 2c09 2020 2020 2275 696e 7433  t32",.    "uint3
-00000620: 3222 2c09 2269 6e74 6567 6572 2220 2020  2",."integer"   
-00000630: 2020 2020 205d 2c0d 0a20 2020 205b 2275       ],..    ["u
-00000640: 696e 7436 3422 2c09 2020 2020 2275 696e  int64",.    "uin
-00000650: 7436 3422 2c20 0922 696e 7465 6765 7222  t64", ."integer"
-00000660: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
-00000670: 5b22 696e 7438 222c 0920 2020 2022 696e  ["int8",.    "in
-00000680: 7438 222c 0920 2020 2022 696e 7465 6765  t8",.    "intege
-00000690: 7222 2020 2020 2020 2020 5d2c 0d0a 2020  r"        ],..  
-000006a0: 2020 5b22 696e 7431 3622 2c09 2020 2020    ["int16",.    
-000006b0: 2269 6e74 3136 222c 0922 696e 7465 6765  "int16",."intege
-000006c0: 7222 2020 2020 2020 2020 5d2c 0d0a 2020  r"        ],..  
-000006d0: 2020 5b22 696e 7433 3222 2c09 2020 2020    ["int32",.    
-000006e0: 2269 6e74 3332 222c 0922 696e 7465 6765  "int32",."intege
-000006f0: 7222 2020 2020 2020 2020 5d2c 0d0a 2020  r"        ],..  
-00000700: 2020 5b22 696e 7436 3422 2c20 2020 2020    ["int64",     
-00000710: 2020 2269 6e74 3634 222c 0922 696e 7465    "int64",."inte
-00000720: 6765 7222 2020 2020 2020 2020 5d2c 0d0a  ger"        ],..
-00000730: 2020 2020 2320 6a73 6f6e 0d0a 2020 2020      # json..    
-00000740: 5b22 6669 6c65 222c 0920 2020 2022 6669  ["file",.    "fi
-00000750: 6c65 222c 0920 2020 2022 7374 7269 6e67  le",.    "string
-00000760: 2220 2020 2020 2020 2020 5d2c 0d0a 2020  "         ],..  
-00000770: 2020 5b22 6e75 6c6c 222c 0920 2020 2022    ["null",.    "
-00000780: 6e75 6c6c 222c 2009 226f 626a 6563 7422  null", ."object"
-00000790: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-000007a0: 205b 226f 626a 6563 7422 2c09 2020 2020   ["object",.    
-000007b0: 226f 626a 6563 7422 2c09 226f 626a 6563  "object",."objec
-000007c0: 7422 2020 2020 2020 2020 205d 2c0d 0a20  t"         ],.. 
-000007d0: 2020 2023 2064 6174 6174 696f 6e0d 0a20     # datation.. 
-000007e0: 2020 205b 2264 6179 222c 0920 2020 2020     ["day",.     
-000007f0: 2020 2022 6461 7922 2c09 2020 2020 2264     "day",.    "d
-00000800: 6174 6522 2020 2020 2020 2020 2020 205d  ate"           ]
-00000810: 2c0d 0a20 2020 205b 2277 6461 7922 2c09  ,..    ["wday",.
-00000820: 2020 2020 2277 6461 7922 2c09 2020 2020      "wday",.    
-00000830: 2264 6174 6522 2020 2020 2020 2020 2020  "date"          
-00000840: 205d 2c0d 0a20 2020 205b 2279 6461 7922   ],..    ["yday"
-00000850: 2c09 2020 2020 2279 6461 7922 2c09 2020  ,.    "yday",.  
-00000860: 2020 2264 6174 6522 2020 2020 2020 2020    "date"        
-00000870: 2020 205d 2c0d 0a20 2020 205b 2277 6565     ],..    ["wee
-00000880: 6b22 2c09 2020 2020 2277 6565 6b22 2c09  k",.    "week",.
-00000890: 2020 2020 2264 6174 6522 2020 2020 2020      "date"      
-000008a0: 2020 2020 205d 2c0d 0a20 2020 205b 2268       ],..    ["h
-000008b0: 6f75 7222 2c09 2020 2020 2268 6f75 7222  our",.    "hour"
-000008c0: 2c09 2020 2020 2274 696d 6522 2020 2020  ,.    "time"    
-000008d0: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
-000008e0: 226d 696e 7574 6522 2c09 2020 2020 226d  "minute",.    "m
-000008f0: 696e 7574 6522 2c09 2274 696d 6522 2020  inute",."time"  
-00000900: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-00000910: 205b 2273 6563 6f6e 6422 2c09 2020 2020   ["second",.    
-00000920: 2273 6563 6f6e 6422 2c09 2274 696d 6522  "second",."time"
-00000930: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
-00000940: 2020 2023 5b22 7065 7269 6f64 222c 0920     #["period",. 
-00000950: 2020 2022 7065 7269 6f64 222c 0922 6475     "period",."du
-00000960: 7261 7469 6f6e 2220 2020 2020 2020 5d2c  ration"       ],
-00000970: 0d0a 2020 2020 2320 6c6f 6361 7469 6f6e  ..    # location
-00000980: 0d0a 2020 2020 5b22 6765 6f6d 6574 7279  ..    ["geometry
-00000990: 222c 2020 2020 2267 656f 6d65 7472 7922  ",    "geometry"
-000009a0: 2c09 2267 656f 6a73 6f6e 2220 2020 2020  ,."geojson"     
-000009b0: 2020 205d 2c0d 0a20 2020 205b 2270 6f6c     ],..    ["pol
-000009c0: 7967 6f6e 222c 0920 2020 2022 706f 6c79  ygon",.    "poly
-000009d0: 676f 6e22 2c09 2267 656f 6a73 6f6e 2220  gon",."geojson" 
-000009e0: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
-000009f0: 226c 696e 6522 2c09 2020 2020 226c 696e  "line",.    "lin
-00000a00: 6522 2c09 2020 2020 2267 656f 6a73 6f6e  e",.    "geojson
-00000a10: 2220 2020 2020 2020 205d 0d0a 2020 2020  "        ]..    
-00000a20: 5d0d 0a0d 0a23 2073 7065 6369 6669 6320  ]....# specific 
-00000a30: 6e74 765f 7479 7065 2069 6620 6e61 6d65  ntv_type if name
-00000a40: 5f74 7970 6520 6973 206e 756c 6c0d 0a63  _type is null..c
-00000a50: 6f6c 5f74 7970 6520 3d20 5b20 226e 7476  ol_type = [ "ntv
-00000a60: 5f74 7970 6522 2c20 226e 616d 655f 7479  _type", "name_ty
-00000a70: 7065 222c 2022 6474 7970 6522 205d 0d0a  pe", "dtype" ]..
-00000a80: 7479 7065 2020 203d 205b 0d0a 2020 2020  type   = [..    
-00000a90: 5b22 696e 7422 2c09 2020 2020 2020 2020  ["int",.        
-00000aa0: 6e75 6c6c 2c09 2020 2020 2269 6e74 3634  null,.    "int64
-00000ab0: 2220 2020 2020 2020 2020 205d 2c0d 0a20  "          ],.. 
-00000ac0: 2020 205b 226a 736f 6e22 2c09 2020 2020     ["json",.    
-00000ad0: 6e75 6c6c 2c09 2020 2020 226f 626a 6563  null,.    "objec
-00000ae0: 7422 2020 2020 2020 2020 205d 2c0d 0a20  t"         ],.. 
-00000af0: 2020 205b 2262 6f6f 6c65 616e 222c 0920     ["boolean",. 
-00000b00: 2020 206e 756c 6c2c 0920 2020 2022 626f     null,.    "bo
-00000b10: 6f6c 6561 6e22 2020 2020 2020 2020 5d2c  olean"        ],
-00000b20: 0d0a 2020 2020 5b22 6e75 6d62 6572 222c  ..    ["number",
-00000b30: 0920 2020 206e 756c 6c2c 0920 2020 2022  .    null,.    "
-00000b40: 666c 6f61 7436 3422 2020 2020 2020 2020  float64"        
-00000b50: 5d0d 0a20 2020 205d 0d0a 0d0a 2320 6465  ]..    ]....# de
-00000b60: 6669 6e65 2074 6865 2074 7970 6573 2077  fine the types w
-00000b70: 6974 686f 7574 2054 6162 6c65 5363 6865  ithout TableSche
-00000b80: 6d61 2073 7065 6369 6669 6361 7469 6f6e  ma specification
-00000b90: 0d0a 6f74 6865 7274 7970 6520 3d20 5b0d  ..othertype = [.
-00000ba0: 0a20 2020 205b 2264 6174 222c 0920 2020  .    ["dat",.   
-00000bb0: 2020 2020 2020 2020 2022 6461 7422 2c09           "dat",.
-00000bc0: 2020 2020 2020 2020 226f 626a 6563 7422          "object"
-00000bd0: 205d 2c0d 0a20 2020 205b 226d 756c 7469   ],..    ["multi
-00000be0: 706f 696e 7422 2c09 2020 2020 226d 756c  point",.    "mul
-00000bf0: 7469 706f 696e 7422 2c20 2020 226f 626a  tipoint",   "obj
-00000c00: 6563 7422 205d 2c0d 0a20 2020 205b 226d  ect" ],..    ["m
-00000c10: 756c 7469 6c69 6e65 222c 0920 2020 2022  ultiline",.    "
-00000c20: 6d75 6c74 696c 696e 6522 2c20 2020 2022  multiline",    "
-00000c30: 6f62 6a65 6374 2220 5d2c 0d0a 2020 2020  object" ],..    
-00000c40: 5b22 6d75 6c74 6970 6f6c 7967 6f6e 222c  ["multipolygon",
-00000c50: 0922 6d75 6c74 6970 6f6c 7967 6f6e 222c  ."multipolygon",
-00000c60: 0922 6f62 6a65 6374 2220 5d2c 0d0a 2020  ."object" ],..  
-00000c70: 2020 5b22 626f 7822 2c09 2020 2020 2020    ["box",.      
-00000c80: 2020 2020 2020 2262 6f78 222c 0920 2020        "box",.   
-00000c90: 2020 2020 2022 6f62 6a65 6374 2220 5d2c       "object" ],
-00000ca0: 0d0a 2020 2020 5b22 636f 6465 6f6c 6322  ..    ["codeolc"
-00000cb0: 2c09 2020 2020 2020 2020 2263 6f64 656f  ,.        "codeo
-00000cc0: 6c63 222c 0920 2020 2022 6f62 6a65 6374  lc",.    "object
-00000cd0: 2220 5d2c 0d0a 2020 2020 5b22 726f 7722  " ],..    ["row"
-00000ce0: 2c09 2020 2020 2020 2020 2020 2020 2272  ,.            "r
-00000cf0: 6f77 222c 0920 2020 2020 2020 2022 6f62  ow",.        "ob
-00000d00: 6a65 6374 2220 5d2c 0d0a 2020 2020 5b22  ject" ],..    ["
-00000d10: 6669 656c 6422 2c09 2020 2020 2020 2020  field",.        
-00000d20: 2266 6965 6c64 222c 0920 2020 2022 6f62  "field",.    "ob
-00000d30: 6a65 6374 2220 5d2c 0d0a 2020 2020 5b22  ject" ],..    ["
-00000d40: 7461 6222 2c09 2020 2020 2020 2020 2020  tab",.          
-00000d50: 2020 2274 6162 222c 0920 2020 2020 2020    "tab",.       
-00000d60: 2022 6f62 6a65 6374 2220 5d2c 0d0a 2020   "object" ],..  
-00000d70: 2020 5b22 6e74 7622 2c09 2020 2020 2020    ["ntv",.      
-00000d80: 2020 2020 2020 226e 7476 222c 0920 2020        "ntv",.   
-00000d90: 2020 2020 2022 6f62 6a65 6374 2220 5d0d       "object" ].
-00000da0: 0a20 2020 205d 0d0a 0d0a 2320 7265 7061  .    ]....# repa
-00000db0: 6365 2028 5c77 2b29 202d 3e20 2224 3122  ce (\w+) -> "$1"
-00000dc0: 2c                                       ,
+00000080: 7065 206f 6620 7468 6520 6461 7461 0d0a  pe of the data..
+00000090: 2020 2020 2320 2766 6f72 6d61 7427 2069      # 'format' i
+000000a0: 7320 6465 6669 6e65 6420 696e 2054 6162  s defined in Tab
+000000b0: 6c65 5363 6865 6d61 2073 7065 6369 6669  leSchema specifi
+000000c0: 6361 7469 6f6e 0d0a 2020 2020 2320 2774  cation..    # 't
+000000d0: 7970 6527 2069 7320 6465 6669 6e65 6420  ype' is defined 
+000000e0: 696e 2054 6162 6c65 5363 6865 6d61 2073  in TableSchema s
+000000f0: 7065 6369 6669 6361 7469 6f6e 0d0a 0d0a  pecification....
+00000100: 2320 6d61 7070 696e 6720 6265 7477 6565  # mapping betwee
+00000110: 6e20 4e54 5674 7970 6520 616e 6420 5461  n NTVtype and Ta
+00000120: 626c 6553 6368 656d 610d 0a6d 6170 7069  bleSchema..mappi
+00000130: 6e67 203d 205b 0d0a 2020 2020 2320 6e75  ng = [..    # nu
+00000140: 6d65 7269 6361 6c0d 0a20 2020 205b 2269  merical..    ["i
+00000150: 6e74 222c 0920 2020 2020 2020 2022 6465  nt",.        "de
+00000160: 6661 756c 7422 2c09 2020 2020 2269 6e74  fault",.    "int
+00000170: 6567 6572 2220 2020 205d 2c0d 0a20 2020  eger"    ],..   
+00000180: 205b 226e 756d 6265 7222 2c09 2020 2020   ["number",.    
+00000190: 2264 6566 6175 6c74 222c 0920 2020 2022  "default",.    "
+000001a0: 6e75 6d62 6572 2220 2020 2020 5d2c 0d0a  number"     ],..
+000001b0: 2020 2020 5b22 626f 6f6c 6561 6e22 2c09      ["boolean",.
+000001c0: 2020 2020 2264 6566 6175 6c74 222c 0920      "default",. 
+000001d0: 2020 2022 626f 6f6c 6561 6e22 2020 2020     "boolean"    
+000001e0: 5d2c 0d0a 2020 2020 2320 6a73 6f6e 0d0a  ],..    # json..
+000001f0: 2020 2020 5b22 7374 7269 6e67 222c 0920      ["string",. 
+00000200: 2020 2022 6465 6661 756c 7422 2c09 2020     "default",.  
+00000210: 2020 2273 7472 696e 6722 2020 2020 205d    "string"     ]
+00000220: 2c0d 0a20 2020 205b 2275 7269 222c 0920  ,..    ["uri",. 
+00000230: 2020 2020 2020 2022 7572 6922 2c09 2020         "uri",.  
+00000240: 2020 2020 2020 2273 7472 696e 6722 2020        "string"  
+00000250: 2020 205d 2c0d 0a20 2020 205b 2265 6d61     ],..    ["ema
+00000260: 696c 222c 0920 2020 2022 656d 6169 6c22  il",.    "email"
+00000270: 2c09 2020 2020 2273 7472 696e 6722 2020  ,.    "string"  
+00000280: 2020 205d 2c0d 0a20 2020 205b 226a 736f     ],..    ["jso
+00000290: 6e22 2c09 2020 2020 2264 6566 6175 6c74  n",.    "default
+000002a0: 222c 2009 2020 2020 226f 626a 6563 7422  ", .    "object"
+000002b0: 2020 2020 205d 2c0d 0a20 2020 205b 2261       ],..    ["a
+000002c0: 7272 6179 222c 0920 2020 2022 6465 6661  rray",.    "defa
+000002d0: 756c 7422 2c09 2020 2020 2261 7272 6179  ult",.    "array
+000002e0: 2220 2020 2020 205d 2c0d 0a20 2020 2023  "      ],..    #
+000002f0: 2064 6174 6174 696f 6e0d 0a20 2020 205b   datation..    [
+00000300: 2264 7572 6174 696f 6e22 2c09 2264 6566  "duration",."def
+00000310: 6175 6c74 222c 0920 2020 2022 6475 7261  ault",.    "dura
+00000320: 7469 6f6e 2220 2020 5d2c 0d0a 2020 2020  tion"   ],..    
+00000330: 5b22 6461 7465 7469 6d65 222c 0922 6465  ["datetime",."de
+00000340: 6661 756c 7422 2c09 2020 2020 2264 6174  fault",.    "dat
+00000350: 6574 696d 6522 2020 205d 2c0d 0a20 2020  etime"   ],..   
+00000360: 205b 2264 6174 6522 2c09 2020 2020 2264   ["date",.    "d
+00000370: 6566 6175 6c74 222c 0920 2020 2022 6461  efault",.    "da
+00000380: 7465 2220 2020 2020 2020 5d2c 0d0a 2020  te"       ],..  
+00000390: 2020 5b22 7469 6d65 222c 0920 2020 2022    ["time",.    "
+000003a0: 6465 6661 756c 7422 2c09 2020 2020 2274  default",.    "t
+000003b0: 696d 6522 2020 2020 2020 205d 2c0d 0a20  ime"       ],.. 
+000003c0: 2020 205b 226d 6f6e 7468 222c 0920 2020     ["month",.   
+000003d0: 2022 6465 6661 756c 7422 2c09 2020 2020   "default",.    
+000003e0: 2279 6561 726d 6f6e 7468 2220 205d 2c0d  "yearmonth"  ],.
+000003f0: 0a20 2020 205b 2279 6561 7222 2c09 2020  .    ["year",.  
+00000400: 2020 2264 6566 6175 6c74 222c 0920 2020    "default",.   
+00000410: 2022 7965 6172 2220 2020 2020 2020 5d2c   "year"       ],
+00000420: 0d0a 2020 2020 2320 6c6f 6361 7469 6f6e  ..    # location
+00000430: 0d0a 2020 2020 5b22 706f 696e 7422 2c09  ..    ["point",.
+00000440: 2020 2020 2261 7272 6179 222c 0920 2020      "array",.   
+00000450: 2022 6765 6f70 6f69 6e74 2220 2020 5d2c   "geopoint"   ],
+00000460: 0d0a 2020 2020 5b22 6765 6f6a 736f 6e22  ..    ["geojson"
+00000470: 2c09 2020 2020 2264 6566 6175 6c74 222c  ,.    "default",
+00000480: 2020 0922 6765 6f6a 736f 6e22 2020 2020    ."geojson"    
+00000490: 5d2c 0d0a 0d0a 2020 2020 2320 7479 7065  ],....    # type
+000004a0: 7320 7769 7468 6f75 7420 5461 626c 6553  s without TableS
+000004b0: 6368 656d 6120 7370 6563 6966 6963 6174  chema specificat
+000004c0: 696f 6e0d 0a20 2020 2023 206e 756d 6572  ion..    # numer
+000004d0: 6963 616c 0d0a 2020 2020 5b22 666c 6f61  ical..    ["floa
+000004e0: 7436 3422 2c09 2020 2020 2266 6c6f 6174  t64",.    "float
+000004f0: 3634 222c 0922 6e75 6d62 6572 2220 2020  64",."number"   
+00000500: 2020 2020 2020 5d2c 0d0a 2020 2020 5b22        ],..    ["
+00000510: 666c 6f61 7422 2c09 2020 2020 2266 6c6f  float",.    "flo
+00000520: 6174 222c 0922 6e75 6d62 6572 2220 2020  at",."number"   
+00000530: 2020 2020 2020 5d2c 0d0a 2020 2020 5b22        ],..    ["
+00000540: 666c 6f61 7431 3622 2c09 2020 2020 2266  float16",.    "f
+00000550: 6c6f 6174 3136 222c 0922 6e75 6d62 6572  loat16",."number
+00000560: 2220 2020 2020 2020 2020 5d2c 0d0a 2020  "         ],..  
+00000570: 2020 5b22 666c 6f61 7433 3222 2c09 2020    ["float32",.  
+00000580: 2020 2266 6c6f 6174 3332 222c 0922 6e75    "float32",."nu
+00000590: 6d62 6572 2220 2020 2020 2020 2020 5d2c  mber"         ],
+000005a0: 0d0a 2020 2020 5b22 7569 6e74 3822 2c09  ..    ["uint8",.
+000005b0: 2020 2020 2275 696e 7438 222c 0922 696e      "uint8",."in
+000005c0: 7465 6765 7222 2020 2020 2020 2020 5d2c  teger"        ],
+000005d0: 0d0a 2020 2020 5b22 7569 6e74 3136 222c  ..    ["uint16",
+000005e0: 0920 2020 2022 7569 6e74 3136 222c 0922  .    "uint16",."
+000005f0: 696e 7465 6765 7222 2020 2020 2020 2020  integer"        
+00000600: 5d2c 0d0a 2020 2020 5b22 7569 6e74 3332  ],..    ["uint32
+00000610: 222c 0920 2020 2022 7569 6e74 3332 222c  ",.    "uint32",
+00000620: 0922 696e 7465 6765 7222 2020 2020 2020  ."integer"      
+00000630: 2020 5d2c 0d0a 2020 2020 5b22 7569 6e74    ],..    ["uint
+00000640: 3634 222c 0920 2020 2022 7569 6e74 3634  64",.    "uint64
+00000650: 222c 2009 2269 6e74 6567 6572 2220 2020  ", ."integer"   
+00000660: 2020 2020 205d 2c0d 0a20 2020 205b 2269       ],..    ["i
+00000670: 6e74 3822 2c09 2020 2020 2269 6e74 3822  nt8",.    "int8"
+00000680: 2c09 2020 2020 2269 6e74 6567 6572 2220  ,.    "integer" 
+00000690: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
+000006a0: 2269 6e74 3136 222c 0920 2020 2022 696e  "int16",.    "in
+000006b0: 7431 3622 2c09 2269 6e74 6567 6572 2220  t16",."integer" 
+000006c0: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
+000006d0: 2269 6e74 3332 222c 0920 2020 2022 696e  "int32",.    "in
+000006e0: 7433 3222 2c09 2269 6e74 6567 6572 2220  t32",."integer" 
+000006f0: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
+00000700: 2269 6e74 3634 222c 2020 2020 2020 2022  "int64",       "
+00000710: 696e 7436 3422 2c09 2269 6e74 6567 6572  int64",."integer
+00000720: 2220 2020 2020 2020 205d 2c0d 0a20 2020  "        ],..   
+00000730: 2023 206a 736f 6e0d 0a20 2020 205b 2266   # json..    ["f
+00000740: 696c 6522 2c09 2020 2020 2266 696c 6522  ile",.    "file"
+00000750: 2c09 2020 2020 2273 7472 696e 6722 2020  ,.    "string"  
+00000760: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
+00000770: 226e 756c 6c22 2c09 2020 2020 226e 756c  "null",.    "nul
+00000780: 6c22 2c20 0922 6f62 6a65 6374 2220 2020  l", ."object"   
+00000790: 2020 2020 2020 5d2c 0d0a 2020 2020 5b22        ],..    ["
+000007a0: 6f62 6a65 6374 222c 0920 2020 2022 6f62  object",.    "ob
+000007b0: 6a65 6374 222c 0922 6f62 6a65 6374 2220  ject",."object" 
+000007c0: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
+000007d0: 2320 6461 7461 7469 6f6e 0d0a 2020 2020  # datation..    
+000007e0: 5b22 6461 7922 2c09 2020 2020 2020 2020  ["day",.        
+000007f0: 2264 6179 222c 0920 2020 2022 6461 7465  "day",.    "date
+00000800: 2220 2020 2020 2020 2020 2020 5d2c 0d0a  "           ],..
+00000810: 2020 2020 5b22 7764 6179 222c 0920 2020      ["wday",.   
+00000820: 2022 7764 6179 222c 0920 2020 2022 6461   "wday",.    "da
+00000830: 7465 2220 2020 2020 2020 2020 2020 5d2c  te"           ],
+00000840: 0d0a 2020 2020 5b22 7964 6179 222c 0920  ..    ["yday",. 
+00000850: 2020 2022 7964 6179 222c 0920 2020 2022     "yday",.    "
+00000860: 6461 7465 2220 2020 2020 2020 2020 2020  date"           
+00000870: 5d2c 0d0a 2020 2020 5b22 7765 656b 222c  ],..    ["week",
+00000880: 0920 2020 2022 7765 656b 222c 0920 2020  .    "week",.   
+00000890: 2022 6461 7465 2220 2020 2020 2020 2020   "date"         
+000008a0: 2020 5d2c 0d0a 2020 2020 5b22 686f 7572    ],..    ["hour
+000008b0: 222c 0920 2020 2022 686f 7572 222c 0920  ",.    "hour",. 
+000008c0: 2020 2022 7469 6d65 2220 2020 2020 2020     "time"       
+000008d0: 2020 2020 5d2c 0d0a 2020 2020 5b22 6d69      ],..    ["mi
+000008e0: 6e75 7465 222c 0920 2020 2022 6d69 6e75  nute",.    "minu
+000008f0: 7465 222c 0922 7469 6d65 2220 2020 2020  te",."time"     
+00000900: 2020 2020 2020 5d2c 0d0a 2020 2020 5b22        ],..    ["
+00000910: 7365 636f 6e64 222c 0920 2020 2022 7365  second",.    "se
+00000920: 636f 6e64 222c 0922 7469 6d65 2220 2020  cond",."time"   
+00000930: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
+00000940: 235b 2270 6572 696f 6422 2c09 2020 2020  #["period",.    
+00000950: 2270 6572 696f 6422 2c09 2264 7572 6174  "period",."durat
+00000960: 696f 6e22 2020 2020 2020 205d 2c0d 0a20  ion"       ],.. 
+00000970: 2020 2023 206c 6f63 6174 696f 6e0d 0a20     # location.. 
+00000980: 2020 205b 2267 656f 6d65 7472 7922 2c20     ["geometry", 
+00000990: 2020 2022 6765 6f6d 6574 7279 222c 0922     "geometry",."
+000009a0: 6765 6f6a 736f 6e22 2020 2020 2020 2020  geojson"        
+000009b0: 5d2c 0d0a 2020 2020 5b22 706f 6c79 676f  ],..    ["polygo
+000009c0: 6e22 2c09 2020 2020 2270 6f6c 7967 6f6e  n",.    "polygon
+000009d0: 222c 0922 6765 6f6a 736f 6e22 2020 2020  ",."geojson"    
+000009e0: 2020 2020 5d2c 0d0a 2020 2020 5b22 6c69      ],..    ["li
+000009f0: 6e65 222c 0920 2020 2022 6c69 6e65 222c  ne",.    "line",
+00000a00: 0920 2020 2022 6765 6f6a 736f 6e22 2020  .    "geojson"  
+00000a10: 2020 2020 2020 5d0d 0a20 2020 205d 0d0a        ]..    ]..
+00000a20: 0d0a 2320 7370 6563 6966 6963 206e 7476  ..# specific ntv
+00000a30: 5f74 7970 6520 6966 206e 616d 655f 7479  _type if name_ty
+00000a40: 7065 2069 7320 6e75 6c6c 0d0a 636f 6c5f  pe is null..col_
+00000a50: 7479 7065 203d 205b 2022 6e74 765f 7479  type = [ "ntv_ty
+00000a60: 7065 222c 2022 6e61 6d65 5f74 7970 6522  pe", "name_type"
+00000a70: 2c20 2264 7479 7065 2220 5d0d 0a74 7970  , "dtype" ]..typ
+00000a80: 6520 2020 3d20 5b0d 0a20 2020 205b 2269  e   = [..    ["i
+00000a90: 6e74 222c 0920 2020 2020 2020 206e 756c  nt",.        nul
+00000aa0: 6c2c 0920 2020 2022 696e 7436 3422 2020  l,.    "int64"  
+00000ab0: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
+00000ac0: 5b22 6a73 6f6e 222c 0920 2020 206e 756c  ["json",.    nul
+00000ad0: 6c2c 0920 2020 2022 6f62 6a65 6374 2220  l,.    "object" 
+00000ae0: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
+00000af0: 5b22 626f 6f6c 6561 6e22 2c09 2020 2020  ["boolean",.    
+00000b00: 6e75 6c6c 2c09 2020 2020 2262 6f6f 6c65  null,.    "boole
+00000b10: 616e 2220 2020 2020 2020 205d 2c0d 0a20  an"        ],.. 
+00000b20: 2020 205b 226e 756d 6265 7222 2c09 2020     ["number",.  
+00000b30: 2020 6e75 6c6c 2c09 2020 2020 2266 6c6f    null,.    "flo
+00000b40: 6174 3634 2220 2020 2020 2020 205d 0d0a  at64"        ]..
+00000b50: 2020 2020 5d0d 0a0d 0a23 2064 6566 696e      ]....# defin
+00000b60: 6520 7468 6520 7479 7065 7320 7769 7468  e the types with
+00000b70: 6f75 7420 5461 626c 6553 6368 656d 6120  out TableSchema 
+00000b80: 7370 6563 6966 6963 6174 696f 6e0d 0a6f  specification..o
+00000b90: 7468 6572 7479 7065 203d 205b 0d0a 2020  thertype = [..  
+00000ba0: 2020 5b22 6461 7422 2c09 2020 2020 2020    ["dat",.      
+00000bb0: 2020 2020 2020 2264 6174 222c 0920 2020        "dat",.   
+00000bc0: 2020 2020 2022 6f62 6a65 6374 2220 5d2c       "object" ],
+00000bd0: 0d0a 2020 2020 5b22 6d75 6c74 6970 6f69  ..    ["multipoi
+00000be0: 6e74 222c 0920 2020 2022 6d75 6c74 6970  nt",.    "multip
+00000bf0: 6f69 6e74 222c 2020 2022 6f62 6a65 6374  oint",   "object
+00000c00: 2220 5d2c 0d0a 2020 2020 5b22 6d75 6c74  " ],..    ["mult
+00000c10: 696c 696e 6522 2c09 2020 2020 226d 756c  iline",.    "mul
+00000c20: 7469 6c69 6e65 222c 2020 2020 226f 626a  tiline",    "obj
+00000c30: 6563 7422 205d 2c0d 0a20 2020 205b 226d  ect" ],..    ["m
+00000c40: 756c 7469 706f 6c79 676f 6e22 2c09 226d  ultipolygon",."m
+00000c50: 756c 7469 706f 6c79 676f 6e22 2c09 226f  ultipolygon",."o
+00000c60: 626a 6563 7422 205d 2c0d 0a20 2020 205b  bject" ],..    [
+00000c70: 2262 6f78 222c 0920 2020 2020 2020 2020  "box",.         
+00000c80: 2020 2022 626f 7822 2c09 2020 2020 2020     "box",.      
+00000c90: 2020 226f 626a 6563 7422 205d 2c0d 0a20    "object" ],.. 
+00000ca0: 2020 205b 2263 6f64 656f 6c63 222c 0920     ["codeolc",. 
+00000cb0: 2020 2020 2020 2022 636f 6465 6f6c 6322         "codeolc"
+00000cc0: 2c09 2020 2020 226f 626a 6563 7422 205d  ,.    "object" ]
+00000cd0: 2c0d 0a20 2020 205b 2272 6f77 222c 0920  ,..    ["row",. 
+00000ce0: 2020 2020 2020 2020 2020 2022 726f 7722             "row"
+00000cf0: 2c09 2020 2020 2020 2020 226f 626a 6563  ,.        "objec
+00000d00: 7422 205d 2c0d 0a20 2020 205b 2266 6965  t" ],..    ["fie
+00000d10: 6c64 222c 0920 2020 2020 2020 2022 6669  ld",.        "fi
+00000d20: 656c 6422 2c09 2020 2020 226f 626a 6563  eld",.    "objec
+00000d30: 7422 205d 2c0d 0a20 2020 205b 2274 6162  t" ],..    ["tab
+00000d40: 222c 0920 2020 2020 2020 2020 2020 2022  ",.            "
+00000d50: 7461 6222 2c09 2020 2020 2020 2020 226f  tab",.        "o
+00000d60: 626a 6563 7422 205d 2c0d 0a20 2020 205b  bject" ],..    [
+00000d70: 226e 7476 222c 0920 2020 2020 2020 2020  "ntv",.         
+00000d80: 2020 2022 6e74 7622 2c09 2020 2020 2020     "ntv",.      
+00000d90: 2020 226f 626a 6563 7422 205d 0d0a 2020    "object" ]..  
+00000da0: 2020 5d0d 0a0d 0a23 2072 6570 6163 6520    ]....# repace 
+00000db0: 285c 772b 2920 2d3e 2022 2431 222c 0a    (\w+) -> "$1",.
```

### Comparing `ntv_pandas-2.0.0/ntv_pandas/pandas_ntv_connector.py` & `ntv_pandas-2.0.1/ntv_pandas/pandas_ntv_connector.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 - an utility class with static methods : `PdUtil`
 
 The functions `to_json`, `to_analysis`, `check_relation`, `as_def_type` and
 `equals` are used with the `npd` accessor.
 
 """
+
 import os
 import datetime
 import json
 import configparser
 from pathlib import Path
 from collections import Counter
 from io import StringIO
@@ -48,86 +49,94 @@
 from tab_dataset.cfield import Cfield
 from ntv_numpy import Xdataset
 
 path_ntv_pandas = Path(os.path.abspath(__file__)).parent
 
 
 def as_def_type(pd_array):
-    '''convert a Series or DataFrame with default dtype'''
+    """convert a Series or DataFrame with default dtype"""
     if isinstance(pd_array, (pd.Series, pd.Index)):
-        return pd_array.astype(SeriesConnec.deftype.get(pd_array.dtype.name, pd_array.dtype.name))
+        return pd_array.astype(
+            SeriesConnec.deftype.get(pd_array.dtype.name, pd_array.dtype.name)
+        )
     return pd.DataFrame({col: as_def_type(pd_array[col]) for col in pd_array.columns})
 
 
 def check_relation(pd_df, parent, child, typecoupl, value=True):
-    ''' Accessor for method `cdataset.Cdataset.check_relation` invoket as
+    """Accessor for method `cdataset.Cdataset.check_relation` invoket as
     `pd.DataFrame.npd.check_relation`.
     Get the inconsistent records for a relationship.
 
      *Parameters*
 
     - **child** : str - name of the child Series involved in the relation
     - **parent**: str - name of the parent Series involved in the relation
     - **typecoupl**: str - relationship to check ('derived' or 'coupled')
     - **value**: boolean (default True) - if True return a dict with inconsistent
     values of the Series, else a tuple with index of records)
 
     *Returns* :
 
     - dict with inconsistent values of the Series
-    - or a tuple with row of records'''
+    - or a tuple with row of records"""
     parent_idx = SeriesConnec.to_idx(pd_df[parent])
-    parent_field = Cfield(parent_idx['codec'], parent, parent_idx['keys'])
+    parent_field = Cfield(parent_idx["codec"], parent, parent_idx["keys"])
     child_idx = SeriesConnec.to_idx(pd_df[child])
-    child_field = Cfield(child_idx['codec'], child, child_idx['keys'])
+    child_field = Cfield(child_idx["codec"], child, child_idx["keys"])
     return Cfield.check_relation(parent_field, child_field, typecoupl, value)
 
 
 def equals(pdself, pdother):
-    '''return True if pd.equals is True and names are equal and dtype of categories are equal'''
+    """return True if pd.equals is True and names are equal and dtype of categories are equal"""
     if isinstance(pdself, pd.Series) and isinstance(pdother, pd.Series):
         return SeriesConnec.equals(pdself, pdother)
     if isinstance(pdself, pd.DataFrame) and isinstance(pdother, pd.DataFrame):
         return DataFrameConnec.equals(pdself, pdother)
     return False
 
 
 def read_json(jsn, **kwargs):
-    ''' convert JSON text or JSON Value to pandas Series or Dataframe.
+    """convert JSON text or JSON Value to pandas Series or Dataframe.
 
     *parameters*
 
     - **jsn** : JSON text or JSON value to convert
     - **extkeys**: list (default None) - keys to use if not present in ntv_value
     - **decode_str**: boolean (default False) - if True, string values are converted
     in object values
     - **leng**: integer (default None) - leng of the Series (used with single codec value)
     - **alias**: boolean (default False) - if True, convert dtype in alias dtype
     - **annotated**: boolean (default False) - if True, ntv_codec names are ignored
     - **series**: boolean (default False) - used only without header. If True
     JSON data is converted into Series else DataFrame
-    '''
-    option = {'extkeys': None, 'decode_str': False, 'leng': None, 'alias': False,
-              'annotated': False, 'series': False} | kwargs
+    """
+    option = {
+        "extkeys": None,
+        "decode_str": False,
+        "leng": None,
+        "alias": False,
+        "annotated": False,
+        "series": False,
+    } | kwargs
     jso = json.loads(jsn) if isinstance(jsn, str) else jsn
-    if 'schema' in jso:
+    if "schema" in jso:
         return PdUtil.to_obj_table(jso, **option)
     ntv = Ntv.from_obj(jso)
-    if ntv.type_str == 'field':
+    if ntv.type_str == "field":
         return SeriesConnec.to_obj_ntv(ntv.ntv_value, **option)
-    if ntv.type_str == 'tab':
+    if ntv.type_str == "tab":
         return DataFrameConnec.to_obj_ntv(ntv.ntv_value, **option)
-    if option['series']:
+    if option["series"]:
         return SeriesConnec.to_obj_ntv(ntv, **option)
     return DataFrameConnec.to_obj_ntv(ntv.ntv_value, **option)
 
 
 def _dist(key1, key2, distr=False):
-    '''return default coupling codec between two keys list and optionaly if
-    the relationship is distributed'''
+    """return default coupling codec between two keys list and optionaly if
+    the relationship is distributed"""
     if not key1 or not key2:
         return 0
     k1k2 = [tuple((v1, v2)) for v1, v2 in zip(key1, key2)]
     dist = len(list(dict.fromkeys(k1k2)))
     if not distr:
         return dist
     distrib = False
@@ -135,391 +144,446 @@
         distrib = max(Counter(k1k2).values()) == len(key1) // dist
         # distrib = min(sum(map(lambda x: (x + i) % (max(a) + 1), a)) == sum(a)
         # for i in range(1, max(a)+1))
     return [dist, distrib]
 
 
 def to_analysis(pd_df, distr=False):
-    '''return a dict with data used in AnaDataset module'''
+    """return a dict with data used in AnaDataset module"""
 
-    keys = [list(pd_df[col].astype('category').cat.codes)
-            for col in pd_df.columns]
+    keys = [list(pd_df[col].astype("category").cat.codes) for col in pd_df.columns]
     lencodec = [len(set(key)) for key in keys]
     if distr:
-        dist = [[_dist(keys[i], keys[j], distr) for j in range(i+1, len(keys))]
-                for i in range(len(keys)-1)]
+        dist = [
+            [_dist(keys[i], keys[j], distr) for j in range(i + 1, len(keys))]
+            for i in range(len(keys) - 1)
+        ]
     else:
-        dist = [[len(set(zip(keys[i], keys[j]))) for j in range(i+1, len(keys))]
-                for i in range(len(keys)-1)]
-    return {'fields': [{'lencodec': lencodec[ind], 'id': pd_df.columns[ind],
-                        'mincodec': lencodec[ind]}
-                       for ind in range(len(pd_df.columns))],
-            'name': None, 'length': len(pd_df),
-            'relations': {pd_df.columns[i]: {pd_df.columns[j+i+1]: dist[i][j]
-                          for j in range(len(dist[i]))} for i in range(len(dist))}}
+        dist = [
+            [len(set(zip(keys[i], keys[j]))) for j in range(i + 1, len(keys))]
+            for i in range(len(keys) - 1)
+        ]
+    return {
+        "fields": [
+            {
+                "lencodec": lencodec[ind],
+                "id": pd_df.columns[ind],
+                "mincodec": lencodec[ind],
+            }
+            for ind in range(len(pd_df.columns))
+        ],
+        "name": None,
+        "length": len(pd_df),
+        "relations": {
+            pd_df.columns[i]: {
+                pd_df.columns[j + i + 1]: dist[i][j] for j in range(len(dist[i]))
+            }
+            for i in range(len(dist))
+        },
+    }
 
 
 def to_json(pd_array, **kwargs):
-    ''' convert pandas Series or Dataframe to JSON text or JSON Value.
+    """convert pandas Series or Dataframe to JSON text or JSON Value.
 
     *parameters*
 
     - **pd_array** : Series or Dataframe to convert
     - **encoded** : boolean (default: False) - if True return a JSON text else a JSON value
     - **header** : boolean (default: True) - if True the JSON data is included as
     value in a {key:value} object where key is ':field' for Series or ':tab' for DataFrame
     - **table** : boolean (default False) - if True return TableSchema format
     - **index** : boolean (default True) - if True the index Series is included
-    '''
-    option = {'encoded': False, 'header': True,
-              'table': False, 'index': True} | kwargs
-    option['header'] = False if option['table'] else option['header']
+    """
+    option = {"encoded": False, "header": True, "table": False, "index": True} | kwargs
+    option["header"] = False if option["table"] else option["header"]
     if isinstance(pd_array, pd.Series):
-        jsn = SeriesConnec.to_json_ntv(pd_array, table=option['table'])[0]
-        head = ':field'
+        jsn = SeriesConnec.to_json_ntv(pd_array, table=option["table"])[0]
+        head = ":field"
     else:
-        jsn = DataFrameConnec.to_json_ntv(pd_array, table=option['table'],
-                                          index=option['index'])[0]
-        head = ':tab'
-    if option['header']:
+        jsn = DataFrameConnec.to_json_ntv(
+            pd_array, table=option["table"], index=option["index"]
+        )[0]
+        head = ":tab"
+    if option["header"]:
         jsn = {head: jsn}
-    if option['encoded']:
+    if option["encoded"]:
         return json.dumps(jsn)
     return jsn
 
 
 def from_xarray(xdt, **kwargs):
-    ''' convert xarray.Dataset to pandas DataFrame.
+    """convert xarray.Dataset to pandas DataFrame.
 
     *Parameters*
 
-    - **json_name**: Boolean (default True) - if False use full_name else json_name
+    - **ntv_type**: Boolean (default True) - if False use full_name else json_name
     - **info**: Boolean (default True) - if True add xdt.info in DataFrame.attrs
     - **dims**: list of string (default None) - order of dimensions full_name to apply
-    '''
+    """
     return Xdataset.from_xarray(xdt).to_dataframe(**kwargs)
 
 
 def from_scipp(sci, **kwargs):
-    ''' convert scipp.Dataset / scipp.DataArray / scipp.DataGroup to pandas DataFrame.
+    """convert scipp.Dataset / scipp.DataArray / scipp.DataGroup to pandas DataFrame.
 
     *Parameters*
 
-    - **json_name**: Boolean (default True) - if False use full_name else json_name
+    - **ntv_type**: Boolean (default True) - if False use full_name else json_name
     - **info**: Boolean (default True) - if True add xdt.info in DataFrame.attrs
     - **dims**: list of string (default None) - order of dimensions full_name to apply
-    '''
+    """
     return Xdataset.from_scipp(sci).to_dataframe(**kwargs)
 
 
 class DataFrameConnec(NtvConnector):
-
-    '''NTV connector for pandas DataFrame.
+    """NTV connector for pandas DataFrame.
 
     One static methods is included:
 
     - to_listidx: convert a DataFrame in categorical data
-    '''
+    """
 
-    clas_obj = 'DataFrame'
-    clas_typ = 'tab'
+    clas_obj = "DataFrame"
+    clas_typ = "tab"
 
     @staticmethod
     def to_obj_ntv(ntv_value, **kwargs):  # reindex=True, decode_str=False):
-        ''' convert json ntv_value into a DataFrame.
+        """convert json ntv_value into a DataFrame.
 
         *Parameters*
 
         - **index** : list (default None) - list of index values,
         - **alias** : boolean (default False) - if True, alias dtype else default dtype
-        - **annotated** : boolean (default False) - if True, NTV names are not included.'''
+        - **annotated** : boolean (default False) - if True, NTV names are not included."""
         series = SeriesConnec.to_series
 
         ntv = Ntv.fast(ntv_value)
-        lidx = [list(NtvUtil.decode_ntv_tab(ntvf, PdUtil.decode_ntv_to_val))
-                for ntvf in ntv]
+        lidx = [
+            list(NtvUtil.decode_ntv_tab(ntvf, PdUtil.decode_ntv_to_val)) for ntvf in ntv
+        ]
         leng = max([idx[6] for idx in lidx])
-        option = kwargs | {'leng': leng}
+        option = kwargs | {"leng": leng}
         no_keys = []
         for ind, lind in enumerate(lidx):
             no_keys.append(not lind[3] and not lind[4] and not lind[5])
             NtvConnector.init_ntv_keys(ind, lidx, leng)
-            lind[2] = Ntv.fast(Ntv.obj_ntv(
-                lind[2], typ=lind[1], single=len(lind[2]) == 1))
-        list_series = [series(lidx[ind][2], lidx[ind][0], None if no_keys[ind]
-                              else lidx[ind][4], **option) for ind in range(len(lidx))]
+            lind[2] = Ntv.fast(
+                Ntv.obj_ntv(lind[2], typ=lind[1], single=len(lind[2]) == 1)
+            )
+        list_series = [
+            series(
+                lidx[ind][2],
+                lidx[ind][0],
+                None if no_keys[ind] else lidx[ind][4],
+                **option,
+            )
+            for ind in range(len(lidx))
+        ]
         dfr = pd.DataFrame({ser.name: ser for ser in list_series})
         return PdUtil.pd_index(dfr)
 
     @staticmethod
     def to_json_ntv(value, name=None, typ=None, **kwargs):
-        ''' convert a DataFrame (value, name, type) into NTV json (json-value, name, type).
+        """convert a DataFrame (value, name, type) into NTV json (json-value, name, type).
 
         *Parameters*
 
         - **typ** : string (default None) - type of the NTV object,
         - **name** : string (default None) - name of the NTV object
         - **value** : DataFrame values
         - **table** : boolean (default False) - if True return TableSchema format
         - **index** : boolean (default True) - if True the index Series is included
-        '''
-        table = kwargs.get('table', False)
-        index = kwargs.get('index', True)
+        """
+        table = kwargs.get("table", False)
+        index = kwargs.get("index", True)
         if not table:
             df2 = value.reset_index() if index else value
-            jsn = Ntv.obj([SeriesConnec.to_json_ntv(PdUtil.unic(df2[col]))[0]
-                           for col in df2.columns]).to_obj()
+            jsn = Ntv.obj(
+                [
+                    SeriesConnec.to_json_ntv(PdUtil.unic(df2[col]))[0]
+                    for col in df2.columns
+                ]
+            ).to_obj()
             return (jsn, name, DataFrameConnec.clas_typ if not typ else typ)
-        df2 = pd.DataFrame({NtvUtil.from_obj_name(col)[0]: PdUtil.convert(
-            SeriesConnec.to_json_ntv(value[col], table=True, no_val=True)[1],
-            value[col]) for col in value.columns})
-        table_val = json.loads(df2.to_json(orient='table',
-                                           date_format='iso', default_handler=str))
+        df2 = pd.DataFrame(
+            {
+                NtvUtil.from_obj_name(col)[0]: PdUtil.convert(
+                    SeriesConnec.to_json_ntv(value[col], table=True, no_val=True)[1],
+                    value[col],
+                )
+                for col in value.columns
+            }
+        )
+        table_val = json.loads(
+            df2.to_json(orient="table", date_format="iso", default_handler=str)
+        )
         for nam in value.columns:
             ntv_name, ntv_type = SeriesConnec.to_json_ntv(
-                value[nam], table=True, no_val=True)
-            table_val['schema'] = PdUtil.table_schema(table_val['schema'],
-                                                      ntv_name, ntv_type)
+                value[nam], table=True, no_val=True
+            )
+            table_val["schema"] = PdUtil.table_schema(
+                table_val["schema"], ntv_name, ntv_type
+            )
         return (table_val, name, DataFrameConnec.clas_typ if not typ else typ)
 
     @staticmethod
     def to_listidx(dtf):
-        ''' convert a DataFrame in categorical data
+        """convert a DataFrame in categorical data
 
         *Return: tuple with:*
 
         - **list** of dict (keys : 'codec', 'name, 'keys') for each column
-        - **lenght** of the DataFrame'''
+        - **lenght** of the DataFrame"""
         return ([SeriesConnec.to_idx(ser) for name, ser in dtf.items()], len(dtf))
 
     @staticmethod
     def equals(pdself, pdother):
-        '''return True if columns are equals'''
+        """return True if columns are equals"""
         if not (isinstance(pdself, pd.DataFrame) and isinstance(pdother, pd.DataFrame)):
             return False
         if len(pdself.columns) != len(pdother.columns):
             return False
         for cself, cother in zip(pdself, pdother):
             if not SeriesConnec.equals(pdself[cself], pdother[cother]):
                 return False
         return True
 
 
 class SeriesConnec(NtvConnector):
-    '''NTV connector for pandas Series
+    """NTV connector for pandas Series
 
     Two static methods are included:
 
     - to_idx: convert a Series in categorical data
     - to_series: return a Series from Field data
-    '''
-    clas_obj = 'Series'
-    clas_typ = 'field'
+    """
+
+    clas_obj = "Series"
+    clas_typ = "field"
     config = configparser.ConfigParser()
-    config.read(path_ntv_pandas.joinpath('ntv_pandas.ini'))
-    types = pd.DataFrame(json.loads(config['data']['type']),
-                         columns=json.loads(config['data']['column']))
-    astype = json.loads(config['data']['astype'])
+    config.read(path_ntv_pandas.joinpath("ntv_pandas.ini"))
+    types = pd.DataFrame(
+        json.loads(config["data"]["type"]), columns=json.loads(config["data"]["column"])
+    )
+    astype = json.loads(config["data"]["astype"])
     deftype = {val: key for key, val in astype.items()}
     config = configparser.ConfigParser()
-    config.read(path_ntv_pandas.joinpath('ntv_table.ini'))
-    table = pd.DataFrame(json.loads(config['data']['mapping']),
-                         columns=json.loads(config['data']['column']))
-    typtab = pd.DataFrame(json.loads(config['data']['type']),
-                          columns=json.loads(config['data']['col_type']))
+    config.read(path_ntv_pandas.joinpath("ntv_table.ini"))
+    table = pd.DataFrame(
+        json.loads(config["data"]["mapping"]),
+        columns=json.loads(config["data"]["column"]),
+    )
+    typtab = pd.DataFrame(
+        json.loads(config["data"]["type"]),
+        columns=json.loads(config["data"]["col_type"]),
+    )
 
     @staticmethod
     def to_obj_ntv(ntv_value, **kwargs):
-        '''Generate a Series Object from a Ntv field object
+        """Generate a Series Object from a Ntv field object
 
         *Parameters*
 
         - **ntv_value**: Ntv object or Ntv value - value to convert in Series
 
         *parameters (kwargs)*
 
         - **extkeys**: list (default None) - keys to use if not present in ntv_value
         - **decode_str**: boolean (default False) - if True, string values are converted
         in object values
         - **index**: list (default None) - if present, add the index in Series
         - **leng**: integer (default None) - leng of the Series (used with single codec value)
         - **alias**: boolean (default False) - if True, convert dtype in alias dtype
         - **annotated**: boolean (default False) - if True, ntv_codec names are ignored
-        '''
-        option = {'extkeys': None, 'decode_str': False, 'leng': None,
-                  'annotated': False} | kwargs
+        """
+        option = {
+            "extkeys": None,
+            "decode_str": False,
+            "leng": None,
+            "annotated": False,
+        } | kwargs
         if ntv_value is None:
             return None
-        ntv = Ntv.obj(ntv_value, decode_str=option['decode_str'])
+        ntv = Ntv.obj(ntv_value, decode_str=option["decode_str"])
 
-        ntv_name, typ, codec, parent, ntv_keys, coef, leng_field = \
+        ntv_name, typ, codec, parent, ntv_keys, coef, leng_field = (
             NtvUtil.decode_ntv_tab(ntv, PdUtil.decode_ntv_to_val)
-        if parent and not option['extkeys']:
+        )
+        if parent and not option["extkeys"]:
             return None
         if coef:
             ntv_keys = NtvConnector.keysfromcoef(
-                coef, leng_field//coef, option['leng'])
-        elif option['extkeys'] and parent:
-            ntv_keys = NtvConnector.keysfromderkeys(
-                option['extkeys'], ntv_keys)
-        elif option['extkeys'] and not parent:
-            ntv_keys = option['extkeys']
-        ntv_codec = Ntv.fast(Ntv.obj_ntv(
-            codec, typ=typ, single=len(codec) == 1))
+                coef, leng_field // coef, option["leng"]
+            )
+        elif option["extkeys"] and parent:
+            ntv_keys = NtvConnector.keysfromderkeys(option["extkeys"], ntv_keys)
+        elif option["extkeys"] and not parent:
+            ntv_keys = option["extkeys"]
+        ntv_codec = Ntv.fast(Ntv.obj_ntv(codec, typ=typ, single=len(codec) == 1))
         return SeriesConnec.to_series(ntv_codec, ntv_name, ntv_keys, **option)
 
     @staticmethod
     def to_json_ntv(value, name=None, typ=None, **kwargs):
-        ''' convert a Series (value, name, type) into NTV json (json-value, name, type).
+        """convert a Series (value, name, type) into NTV json (json-value, name, type).
 
         *Parameters*
 
         - **typ** : string (default None) - type of the NTV object,
         - **name** : string (default None) - name of the NTV object
         - **value** : Series values
         - **table** : boolean (default False) - if True return (ntv_value, ntv_name, ntv_type)
-        - **no_val** : boolean (default False) - if True return (ntv_name, ntv_type)'''
+        - **no_val** : boolean (default False) - if True return (ntv_name, ntv_type)"""
 
-        table = kwargs.get('table', False)
-        no_val = kwargs.get('no_val', False)
-        srs = value.astype(SeriesConnec.astype.get(
-            value.dtype.name, value.dtype.name))
-        sr_name = srs.name if srs.name else ''
+        table = kwargs.get("table", False)
+        no_val = kwargs.get("no_val", False)
+        srs = value.astype(SeriesConnec.astype.get(value.dtype.name, value.dtype.name))
+        sr_name = srs.name if srs.name else ""
         ntv_name, name_type = NtvUtil.from_obj_name(sr_name)[:2]
 
         if table:
             ntv_type = PdUtil.ntv_type(name_type, srs.dtype.name, table=True)
             ntv_value = PdUtil.table_val(ntv_type, ntv_name, srs)
             if no_val:
                 return (ntv_name, ntv_type)
             return (ntv_value, ntv_name, ntv_type)
-        if srs.dtype.name == 'category':
+        if srs.dtype.name == "category":
             cdc = pd.Series(srs.cat.categories)
             ntv_type = PdUtil.ntv_type(name_type, cdc.dtype.name)
             cat_value = PdUtil.ntv_val(ntv_type, cdc)
             cat_value = NtvList(cat_value, ntv_type=ntv_type)
             cod_value = list(srs.cat.codes)
             coef = NtvConnector.encode_coef(cod_value)
-            ntv_value = [cat_value, NtvList(
-                [coef]) if coef else NtvList(cod_value)]
+            ntv_value = [cat_value, NtvList([coef]) if coef else NtvList(cod_value)]
             ntv_type = None
         else:
             ntv_type = PdUtil.ntv_type(name_type, srs.dtype.name)
-            ntv_value = Ntv.from_obj(PdUtil.ntv_val(ntv_type, srs),
-                                     def_type=ntv_type).ntv_value
+            ntv_value = Ntv.from_obj(
+                PdUtil.ntv_val(ntv_type, srs), def_type=ntv_type
+            ).ntv_value
         if len(ntv_value) == 1:
             ntv_value[0].set_name(ntv_name)
-            return (ntv_value[0].to_obj(), name,
-                    SeriesConnec.clas_typ if not typ else typ)
-        return (NtvList(ntv_value, ntv_name, ntv_type).to_obj(), name,
-                SeriesConnec.clas_typ if not typ else typ)
+            return (
+                ntv_value[0].to_obj(),
+                name,
+                SeriesConnec.clas_typ if not typ else typ,
+            )
+        return (
+            NtvList(ntv_value, ntv_name, ntv_type).to_obj(),
+            name,
+            SeriesConnec.clas_typ if not typ else typ,
+        )
 
     @staticmethod
     def to_idx(ser):
-        ''' convert a Series in categorical data
+        """convert a Series in categorical data
 
         *return (dict)*
 
         { 'codec': 'list of pandas categories',
           'name': 'name of the series',
           'keys': 'list of pandas codes' }
-        '''
-        idx = ser.astype('category')
+        """
+        idx = ser.astype("category")
         lis = list(idx.cat.categories)
         if lis and isinstance(lis[0], pd._libs.tslibs.timestamps.Timestamp):
-            lis = [ts.to_pydatetime().astimezone(datetime.timezone.utc)
-                   for ts in lis]
-        return {'codec': lis, 'name': ser.name, 'keys': list(idx.cat.codes)}
+            lis = [ts.to_pydatetime().astimezone(datetime.timezone.utc) for ts in lis]
+        return {"codec": lis, "name": ser.name, "keys": list(idx.cat.codes)}
 
     @staticmethod
     def to_series(ntv_codec, ntv_name, ntv_keys, **kwargs):
-        ''' return a pd.Series from Field data (codec, name, keys)
+        """return a pd.Series from Field data (codec, name, keys)
 
         *Parameters*
 
         - **ntv_codec**: Ntv object - codec value to convert in Series values
         - **ntv_type**: string - default type to apply to convert in dtype
         - **ntv_name**: string - name of the Series
 
         *parameters (kwargs)*
 
         - **index**: list (default None) - if present, add the index in Series
         - **leng**: integer (default None) - leng of the Series (used with single codec value)
         - **alias**: boolean (default False) - if True, convert dtype in alias dtype
         - **annotated**: boolean (default False) - if True, ntv_codec names are ignored
-        '''
-        option = {'index': None, 'leng': None, 'alias': False,
-                  'annotated': False} | kwargs
-        types = SeriesConnec.types.set_index('ntv_type')
+        """
+        option = {
+            "index": None,
+            "leng": None,
+            "alias": False,
+            "annotated": False,
+        } | kwargs
+        types = SeriesConnec.types.set_index("ntv_type")
         astype = SeriesConnec.astype
-        leng = option['leng']
+        leng = option["leng"]
 
         ntv_type = ntv_codec.type_str
         len_unique = leng if len(ntv_codec) == 1 and leng else 1
         pd_convert = ntv_type in types.index
 
-        pd_name, name_type, dtype = PdUtil.pd_name(
-            ntv_name, ntv_type, pd_convert)
-        ntv_obj = PdUtil.ntv_obj(ntv_codec, name_type if pd_convert else ntv_type,
-                                 option['annotated'], pd_convert)
+        pd_name, name_type, dtype = PdUtil.pd_name(ntv_name, ntv_type, pd_convert)
+        ntv_obj = PdUtil.ntv_obj(
+            ntv_codec,
+            name_type if pd_convert else ntv_type,
+            option["annotated"],
+            pd_convert,
+        )
         if ntv_keys:
-            if pd_convert and name_type != 'array':
+            if pd_convert and name_type != "array":
                 categ = SeriesConnec._from_json(ntv_obj, dtype, ntv_type)
                 cat_type = categ.dtype.name
                 categories = categ.astype(astype.get(cat_type, cat_type))
             else:
-                categories = pd.Series(ntv_obj, dtype='object')
+                categories = pd.Series(ntv_obj, dtype="object")
             cat = pd.CategoricalDtype(categories=categories)
             data = pd.Categorical.from_codes(codes=ntv_keys, dtype=cat)
-            srs = pd.Series(data, name=pd_name,
-                            index=option['index'], dtype='category')
+            srs = pd.Series(data, name=pd_name, index=option["index"], dtype="category")
         else:
             data = ntv_obj * len_unique
             if pd_convert:
                 srs = SeriesConnec._from_json(data, dtype, ntv_type, pd_name)
             else:
                 srs = pd.Series(data, name=pd_name, dtype=dtype)
 
-        if option['alias']:
+        if option["alias"]:
             return srs.astype(astype.get(srs.dtype.name, srs.dtype.name))
         return srs.astype(SeriesConnec.deftype.get(srs.dtype.name, srs.dtype.name))
 
     @staticmethod
     def _from_json(data, dtype, ntv_type, pd_name=None):
-        '''return a Series from a Json data.
+        """return a Series from a Json data.
 
         *Parameters*
 
         - **data**: Json-value - data to convert in a Series
         - **dtype**: string - dtype of the Series
         - **ntv_type**: string - default type to apply to convert in dtype
         - **pd_name**: string - name of the Series including ntv_type
 
-        NTVvalue and a ntv_type'''
-        srs = pd.read_json(StringIO(json.dumps(data)),
-                           dtype=dtype, typ='series')
-        if not pd_name is None:
+        NTVvalue and a ntv_type"""
+        srs = pd.read_json(StringIO(json.dumps(data)), dtype=dtype, typ="series")
+        if pd_name is not None:
             srs = srs.rename(pd_name)
         return PdUtil.convert(ntv_type, srs, tojson=False)
 
     @staticmethod
     def equals(pdself, pdother):
-        '''return True if pd.equals is True and names are equal and dtype of categories are equal'''
+        """return True if pd.equals is True and names are equal and dtype of categories are equal"""
         if not (isinstance(pdself, pd.Series) and isinstance(pdother, pd.Series)):
             return False
         if pdself.name != pdother.name:
             return False
-        type_cat = str(pdself.dtype) == str(pdother.dtype) == 'category'
+        type_cat = str(pdself.dtype) == str(pdother.dtype) == "category"
         if type_cat:
             return SeriesConnec.equals(pdself.cat.categories, pdother.cat.categories)
         return as_def_type(pdself).equals(as_def_type(pdother))
 
 
 class PdUtil:
-    '''ntv-pandas utilities.
+    """ntv-pandas utilities.
 
     This class includes static methods:
 
     Ntv and pandas
     - **ntv_type**: return NTVtype from name_type and dtype of a Series
     - **convert**: convert Series with external NTVtype
     - **ntv_val**: convert a simple Series into NTV json-value
@@ -531,201 +595,224 @@
     TableSchema
     - **to_obj_table**: convert json TableSchema data into a DataFrame or a Series
     - **name_table**: return a list of non index field's names from a json Table
     - **ntvtype_table**: return a list of non index field's ntv_type from a json Table
     - **table_schema**: add 'format' and 'type' keys in a Json TableSchema
     - **table_val**: convert a Series into TableSchema json-value
     - **ntv_table**: return NTVtype from the TableSchema data
-    '''
+    """
+
     @staticmethod
     def to_obj_table(jsn, **kwargs):
-        ''' convert json TableSchema data into a DataFrame or a Series'''
-        ntv_type = PdUtil.ntvtype_table(jsn['schema']['fields'])
-        name = PdUtil.name_table(jsn['schema']['fields'])
-        pd_name = [PdUtil.pd_name(nam, ntvtyp, table=True)[0]
-                   for nam, ntvtyp in zip(name, ntv_type)]
-        pd_dtype = [PdUtil.pd_name(nam, ntvtyp, table=True)[2]
-                    for nam, ntvtyp in zip(name, ntv_type)]
-        dfr = pd.read_json(StringIO(json.dumps(jsn['data'])), orient='record')
+        """convert json TableSchema data into a DataFrame or a Series"""
+        ntv_type = PdUtil.ntvtype_table(jsn["schema"]["fields"])
+        name = PdUtil.name_table(jsn["schema"]["fields"])
+        pd_name = [
+            PdUtil.pd_name(nam, ntvtyp, table=True)[0]
+            for nam, ntvtyp in zip(name, ntv_type)
+        ]
+        pd_dtype = [
+            PdUtil.pd_name(nam, ntvtyp, table=True)[2]
+            for nam, ntvtyp in zip(name, ntv_type)
+        ]
+        dfr = pd.read_json(StringIO(json.dumps(jsn["data"])), orient="record")
         dfr = PdUtil.pd_index(dfr)
-        dfr = pd.DataFrame({col: PdUtil.convert(ntv_type[ind], dfr[col], tojson=False)
-                            for ind, col in enumerate(dfr.columns)})
-        dfr = dfr.astype({col: pd_dtype[ind]
-                         for ind, col in enumerate(dfr.columns)})
+        dfr = pd.DataFrame(
+            {
+                col: PdUtil.convert(ntv_type[ind], dfr[col], tojson=False)
+                for ind, col in enumerate(dfr.columns)
+            }
+        )
+        dfr = dfr.astype({col: pd_dtype[ind] for ind, col in enumerate(dfr.columns)})
         dfr.columns = pd_name
         if len(dfr.columns) == 1:
             return dfr[dfr.columns[0]]
         return dfr
 
     @staticmethod
     def decode_ntv_to_val(ntv):
-        ''' return a value from a ntv_field'''
+        """return a value from a ntv_field"""
         if isinstance(ntv, NtvSingle):
             return ntv.to_obj(simpleval=True)
         return [ntv_val.to_obj() for ntv_val in ntv]
 
     @staticmethod
     def name_table(fields):
-        '''return a list of non index field's names from a json Table'''
-        names = [field.get('name', None) for field in fields
-                 if field.get('name', None) != 'index']
-        return [None if name == 'values' else name for name in names]
+        """return a list of non index field's names from a json Table"""
+        names = [
+            field.get("name", None)
+            for field in fields
+            if field.get("name", None) != "index"
+        ]
+        return [None if name == "values" else name for name in names]
 
     @staticmethod
     def ntvtype_table(fields):
-        '''return a list of non index field's ntv_type from a json Table'''
-        return [PdUtil.ntv_table(field.get('format', 'default'),
-                field.get('type', None)) for field in fields
-                if field.get('name', None) != 'index']
+        """return a list of non index field's ntv_type from a json Table"""
+        return [
+            PdUtil.ntv_table(field.get("format", "default"), field.get("type", None))
+            for field in fields
+            if field.get("name", None) != "index"
+        ]
 
     @staticmethod
     def table_schema(schema, name, ntv_type):
-        '''convert 'ntv_type' in 'format' and 'type' keys in a Json TableSchema
-        for the field defined by 'name' '''
-        ind = [field['name'] for field in schema['fields']].index(name)
-        tabletype = SeriesConnec.table.set_index('ntv_type').loc[ntv_type]
-        if tabletype['format'] == 'default':
-            schema['fields'][ind].pop('format', None)
+        """convert 'ntv_type' in 'format' and 'type' keys in a Json TableSchema
+        for the field defined by 'name'"""
+        ind = [field["name"] for field in schema["fields"]].index(name)
+        tabletype = SeriesConnec.table.set_index("ntv_type").loc[ntv_type]
+        if tabletype["format"] == "default":
+            schema["fields"][ind].pop("format", None)
         else:
-            schema['fields'][ind]['format'] = tabletype['format']
-        schema['fields'][ind]['type'] = tabletype['type']
-        schema['fields'][ind].pop('extDtype', None)
+            schema["fields"][ind]["format"] = tabletype["format"]
+        schema["fields"][ind]["type"] = tabletype["type"]
+        schema["fields"][ind].pop("extDtype", None)
         return schema
 
     @staticmethod
     def table_val(ntv_type, ntv_name, srs):
-        '''convert a Series into TableSchema json-value.
+        """convert a Series into TableSchema json-value.
 
         *Parameters*
 
         - **ntv_type** : string - NTVtype deduced from the Series name_type and dtype,
         - **ntv_name**: string - name of the Series
-        - **srs** : Series to be converted.'''
+        - **srs** : Series to be converted."""
         srs = PdUtil.convert(ntv_type, srs)
         srs.name = ntv_name
-        tab_val = json.loads(srs.to_json(orient='table',
-                                         date_format='iso', default_handler=str))
-        name = 'values' if srs.name is None else srs.name
-        tab_val['schema'] = PdUtil.table_schema(
-            tab_val['schema'], name, ntv_type)
+        tab_val = json.loads(
+            srs.to_json(orient="table", date_format="iso", default_handler=str)
+        )
+        name = "values" if srs.name is None else srs.name
+        tab_val["schema"] = PdUtil.table_schema(tab_val["schema"], name, ntv_type)
         return tab_val
 
     @staticmethod
     def convert(ntv_type, srs, tojson=True):
-        ''' convert Series with external NTVtype.
+        """convert Series with external NTVtype.
 
         *Parameters*
 
         - **ntv_type** : string - NTVtype deduced from the Series name_type and dtype,
         - **srs** : Series to be converted.
-        - **tojson** : boolean (default True) - apply to json function'''
+        - **tojson** : boolean (default True) - apply to json function"""
         if tojson:
-            if ntv_type in ['point', 'line', 'polygon', 'geometry']:
+            if ntv_type in ["point", "line", "polygon", "geometry"]:
                 return srs.apply(ShapelyConnec.to_coord)
-            if ntv_type == 'geojson':
+            if ntv_type == "geojson":
                 return srs.apply(ShapelyConnec.to_geojson)
-            if ntv_type == 'date':
+            if ntv_type == "date":
                 return srs.astype(str)
             return srs
-        if ntv_type in ['point', 'line', 'polygon', 'geometry']:
+        if ntv_type in ["point", "line", "polygon", "geometry"]:
             return srs.apply(ShapelyConnec.to_geometry)
-        if ntv_type == 'geojson':
+        if ntv_type == "geojson":
             return srs.apply(ShapelyConnec.from_geojson)
-        if ntv_type == 'datetime':
+        if ntv_type == "datetime":
             return pd.to_datetime(srs)
-        if ntv_type == 'date':
+        if ntv_type == "date":
             return pd.to_datetime(srs).dt.date
-        if ntv_type == 'time':
-            return pd.to_datetime(srs, format='mixed').dt.time
+        if ntv_type == "time":
+            return pd.to_datetime(srs, format="mixed").dt.time
         return srs
 
     @staticmethod
     def ntv_type(name_type, dtype, table=False):
-        ''' return NTVtype from name_type and dtype of a Series .
+        """return NTVtype from name_type and dtype of a Series .
 
         *Parameters*
 
         - **name_type** : string - type included in the Series name,
         - **dtype** : string - dtype of the Series.
         - **table** : boolean (default False) - True if Table Schema conversion
-        '''
+        """
         if not name_type:
-            types_none = SeriesConnec.types.set_index('name_type').loc[None]
+            types_none = SeriesConnec.types.set_index("name_type").loc[None]
             if dtype in types_none.dtype.values:
-                return types_none.set_index('dtype').loc[dtype].ntv_type
+                return types_none.set_index("dtype").loc[dtype].ntv_type
             if not table:
                 return None
-            typtab = SeriesConnec.typtab.set_index('name_type').loc[None]
-            return typtab.set_index('dtype').loc[dtype.lower()].ntv_type
+            typtab = SeriesConnec.typtab.set_index("name_type").loc[None]
+            return typtab.set_index("dtype").loc[dtype.lower()].ntv_type
         return name_type
 
     @staticmethod
     def ntv_val(ntv_type, srs):
-        ''' convert a simple Series into NTV json-value.
+        """convert a simple Series into NTV json-value.
 
         *Parameters*
 
         - **ntv_type** : string - NTVtype deduced from the Series name_type and dtype,
-        - **srs** : Series to be converted.'''
+        - **srs** : Series to be converted."""
         srs = PdUtil.convert(ntv_type, srs)
-        if ntv_type in ['point', 'line', 'polygon', 'geometry', 'geojson']:
+        if ntv_type in ["point", "line", "polygon", "geometry", "geojson"]:
             return srs.to_list()
-        if srs.dtype.name == 'object':
+        if srs.dtype.name == "object":
             return srs.to_list()
-        return json.loads(srs.to_json(orient='records',
-                                      date_format='iso', default_handler=str))
+        return json.loads(
+            srs.to_json(orient="records", date_format="iso", default_handler=str)
+        )
 
     @staticmethod
     def ntv_obj(ntv_codec, name_type, annotated, pd_convert):
-        '''return a list of values to convert in a Series'''
+        """return a list of values to convert in a Series"""
         if pd_convert:
-            if name_type == 'array':
-                return ntv_codec.to_obj(format='obj', simpleval=True)
-            ntv_obj = ntv_codec.obj_value(simpleval=annotated, json_array=False,
-                                          def_type=ntv_codec.type_str, fast=True)
+            if name_type == "array":
+                return ntv_codec.to_obj(format="obj", simpleval=True)
+            ntv_obj = ntv_codec.obj_value(
+                simpleval=annotated,
+                json_array=False,
+                def_type=ntv_codec.type_str,
+                fast=True,
+            )
             return ntv_obj if isinstance(ntv_obj, list) else [ntv_obj]
-        return ntv_codec.to_obj(format='obj', simpleval=True, def_type=name_type)
+        return ntv_codec.to_obj(format="obj", simpleval=True, def_type=name_type)
 
     @staticmethod
     def ntv_table(table_format, table_type):
-        ''' return NTVtype from the TableSchema data.
+        """return NTVtype from the TableSchema data.
 
         *Parameters*
 
         - **table_format** : string - TableSchema format,
-        - **table_type** : string - TableSchema type'''
-        return SeriesConnec.table.set_index(['type', 'format']).loc[
-            (table_type, table_format)].values[0]
+        - **table_type** : string - TableSchema type"""
+        return (
+            SeriesConnec.table.set_index(["type", "format"])
+            .loc[(table_type, table_format)]
+            .values[0]
+        )
 
     @staticmethod
     def pd_index(dfr):
-        '''return a DataFrame with index'''
-        if 'index' in dfr.columns:
-            dfr = dfr.set_index('index')
+        """return a DataFrame with index"""
+        if "index" in dfr.columns:
+            dfr = dfr.set_index("index")
             dfr.index.rename(None, inplace=True)
         return dfr
 
     @staticmethod
     def pd_name(ntv_name, ntv_type, pd_convert=True, table=False):
-        '''return a tuple with the name of the Series, the type deduced from
-        the name and the dtype'''
-        ntv_name = '' if ntv_name is None else ntv_name
-        typtab = SeriesConnec.typtab.set_index('ntv_type')
-        types = SeriesConnec.types.set_index('ntv_type')
+        """return a tuple with the name of the Series, the type deduced from
+        the name and the dtype"""
+        ntv_name = "" if ntv_name is None else ntv_name
+        typtab = SeriesConnec.typtab.set_index("ntv_type")
+        types = SeriesConnec.types.set_index("ntv_type")
         if table and ntv_type.lower() in typtab.index:
-            name_type = typtab.loc[ntv_type.lower()]['name_type']
-            dtype = typtab.loc[ntv_type.lower()]['dtype']
+            name_type = typtab.loc[ntv_type.lower()]["name_type"]
+            dtype = typtab.loc[ntv_type.lower()]["dtype"]
         elif pd_convert or table:
-            name_type = types.loc[ntv_type]['name_type'] if ntv_type != '' else ''
-            dtype = types.loc[ntv_type]['dtype']
+            name_type = types.loc[ntv_type]["name_type"] if ntv_type != "" else ""
+            dtype = types.loc[ntv_type]["dtype"]
         else:
-            return (ntv_name + '::' + ntv_type, ntv_type, 'object')
+            return (ntv_name + "::" + ntv_type, ntv_type, "object")
         dtype = SeriesConnec.deftype.get(dtype, dtype)  # ajout
-        pd_name = ntv_name + '::' + name_type if name_type else ntv_name
+        pd_name = ntv_name + "::" + name_type if name_type else ntv_name
         return (pd_name if pd_name else None, name_type, dtype)
 
     @staticmethod
     def unic(srs):
-        ''' return simple value if the Series contains a single value'''
-        if str(srs.dtype) == 'category':
+        """return simple value if the Series contains a single value"""
+        if str(srs.dtype) == "category":
             return srs
-        return srs[:1] if np.array_equal(srs.values, [srs.values[0]] * len(srs)) else srs
+        return (
+            srs[:1] if np.array_equal(srs.values, [srs.values[0]] * len(srs)) else srs
+        )
```

### Comparing `ntv_pandas-2.0.0/ntv_pandas.egg-info/PKG-INFO` & `ntv_pandas-2.0.1/ntv_pandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ntv_pandas
-Version: 2.0.0
+Version: 2.0.1
 Summary: NTV-pandas : A tabular analyzer and a semantic, compact and reversible converter
 Home-page: https://github.com/loco-philippe/ntv-pandas/blob/main/README.md
 Author: Philippe Thomy
 Author-email: philippe@loco-labs.io
 Keywords: pandas,JSON-NTV,semantic JSON,development,environmental data
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9, <4
+Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 Requires-Dist: ntv_numpy
 Requires-Dist: tab_analysis
 Requires-Dist: tab_dataset
 Requires-Dist: json_ntv
 Requires-Dist: numpy
 Requires-Dist: pandas
@@ -66,38 +66,38 @@
 The DataFrame resulting from these conversions are identical to the initial DataFrame (reversibility).
 
 ```python
 In [1]: import pandas as pd
         import ntv_pandas as npd
 
 In [2]: fruits = {'plants':      ['fruit', 'fruit', 'fruit', 'fruit', 'vegetable', 'vegetable', 'vegetable', 'vegetable'],
-                  'plts':        ['fr', 'fr', 'fr', 'fr', 've', 've', 've', 've'], 
+                  'plts':        ['fr', 'fr', 'fr', 'fr', 've', 've', 've', 've'],
                   'quantity':    ['1 kg', '10 kg', '1 kg', '10 kg', '1 kg', '10 kg', '1 kg', '10 kg'],
                   'product':     ['apple', 'apple', 'orange', 'orange', 'peppers', 'peppers', 'carrot', 'carrot'],
                   'price':       [1, 10, 2, 20, 1.5, 15, 1.5, 20],
                   'price level': ['low', 'low', 'high', 'high', 'low', 'low', 'high', 'high'],
                   'group':       ['fruit 1', 'fruit 10', 'fruit 1', 'veget', 'veget', 'veget', 'veget', 'veget'],
                   'id':          [1001, 1002, 1003, 1004, 1005, 1006, 1007, 1008],
                   'supplier':    ["sup1", "sup1", "sup1", "sup2", "sup2", "sup2", "sup2", "sup1"],
                   'location':    ["fr", "gb", "es", "ch", "gb", "fr", "es", "ch"],
-                  'valid':       ["ok", "ok", "ok", "ok", "ok", "ok", "ok", "ok"]} 
+                  'valid':       ["ok", "ok", "ok", "ok", "ok", "ok", "ok", "ok"]}
         df_fruits = pd.DataFrame(fruits)
         df_fruits.npd.analysis(distr=True).partitions()   # return the list of partitions (a partition is a list of dimensions)
-Out[2]: 
+Out[2]:
         [['plants', 'quantity', 'price level'],
          ['quantity', 'price level', 'supplier'],
          ['plants', 'location'],
          ['quantity', 'product'],
          ['supplier', 'location'],
          ['id']]
 
 In [3]: kwargs = {'dims':['product', 'quantity'], 'datagroup': False, 'ntv_type': False, 'json_name': False}
         xd_fruits = df_fruits.npd.to_xarray(**kwargs)
         xd_fruits
-Out[3]: 
+Out[3]:
         <xarray.Dataset> Size: 976B
         Dimensions:      (product: 4, quantity: 2)
         Coordinates:
         * product      (product) <U7 112B 'apple' 'carrot' 'orange' 'peppers'
         * quantity     (quantity) <U5 40B '1 kg' '10 kg'
         plants       (product) <U9 144B 'fruit' 'vegetable' 'fruit' 'vegetable'
         plts         (product) <U2 32B 'fr' 've' 'fr' 've'
@@ -108,47 +108,47 @@
         id           (product, quantity) int64 64B 1001 1002 1007 ... 1004 1005 1006
         location     (product, quantity) <U2 64B 'fr' 'gb' 'es' ... 'ch' 'gb' 'fr'
         price        (product, quantity) float64 64B 1.0 10.0 1.5 ... 20.0 1.5 15.0
         supplier     (product, quantity) <U4 128B 'sup1' 'sup1' ... 'sup2' 'sup2'
 
 In [4]: sc_fruits = df_fruits.npd.to_scipp(**kwargs)
         sc_fruits
-Out[4]: 
+Out[4]:
         <scipp.Dataset>
         Dimensions: Sizes[product:4, quantity:2, ]
         Coordinates:
         * plants                     string  [dimensionless]  (product)  ["fruit", "vegetable", "fruit", "vegetable"]
         * plts                       string  [dimensionless]  (product)  ["fr", "ve", "fr", "ve"]
         * price level                string  [dimensionless]  (product)  ["low", "high", "high", "low"]
         * product                    string  [dimensionless]  (product)  ["apple", "carrot", "orange", "peppers"]
         * quantity                   string  [dimensionless]  (quantity) ["1 kg", "10 kg"]
         * valid                      string  [dimensionless]  ()  "ok"
         Data:
           group                      string  [dimensionless]  (product, quantity)  ["fruit 1", "fruit 10", ..., "veget", "veget"]
           id                          int64  [dimensionless]  (product, quantity)  [1001, 1002, ..., 1005, 1006]
           location                   string  [dimensionless]  (product, quantity)  ["fr", "gb", ..., "gb", "fr"]
           price                     float64  [dimensionless]  (product, quantity)  [1, 10, ..., 1.5, 15]
-          supplier                   string  [dimensionless]  (product, quantity)  ["sup1", "sup1", ..., "sup2", "sup2"]       
+          supplier                   string  [dimensionless]  (product, quantity)  ["sup1", "sup1", ..., "sup2", "sup2"]
 ```
 
 Reversibility:
 
 ```python
 In [5]: df_fruits_xd = npd.from_xarray(xd_fruits, **kwargs)
         df_fruits_xd_sort = df_fruits_xd.reset_index()[list(df_fruits.columns)].sort_values(list(df_fruits.columns)).reset_index(drop=True)
         df_fruits_sort = df_fruits.sort_values(list(df_fruits.columns)).reset_index(drop=True)
         df_fruits_xd_sort.equals(df_fruits_sort)
-Out[5]: 
+Out[5]:
         True
 
 In [6]: df_fruits_sc = npd.from_scipp(sc_fruits, **kwargs)
         df_fruits_sc_sort = df_fruits_sc.reset_index()[list(df_fruits.columns)].sort_values(list(df_fruits.columns)).reset_index(drop=True)
         df_fruits_sort = df_fruits.sort_values(list(df_fruits.columns)).reset_index(drop=True)
         df_fruits_sc_sort.equals(df_fruits_sort)
-Out[6]: 
+Out[6]:
         True
 ```
 
 ## JSON converter example
 
 In the example below, a DataFrame with multiple data types is converted to JSON (first to NTV format and then to Table Schema format).
```

### Comparing `ntv_pandas-2.0.0/setup.py` & `ntv_pandas-2.0.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,26 +7,35 @@
 from setuptools import setup, find_packages
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ntv_pandas",
-    version="2.0.0",
+    version="2.0.1",
     description="NTV-pandas : A tabular analyzer and a semantic, compact and reversible converter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/loco-philippe/ntv-pandas/blob/main/README.md",
     author="Philippe Thomy",
     author_email="philippe@loco-labs.io",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3"],
+        "Programming Language :: Python :: 3",
+    ],
     keywords="pandas, JSON-NTV, semantic JSON, development, environmental data",
-    packages=find_packages(include=['ntv_pandas', 'ntv_pandas.*']),
-    package_data={'ntv_pandas': ['*.ini']},
-    python_requires=">=3.9, <4",
-    install_requires=['ntv_numpy', 'tab_analysis', 'tab_dataset', 'json_ntv', 'numpy', 'pandas', 'shapely']
+    packages=find_packages(include=["ntv_pandas", "ntv_pandas.*"]),
+    package_data={"ntv_pandas": ["*.ini"]},
+    python_requires=">=3.10, <4",
+    install_requires=[
+        "ntv_numpy",
+        "tab_analysis",
+        "tab_dataset",
+        "json_ntv",
+        "numpy",
+        "pandas",
+        "shapely",
+    ],
 )
```

