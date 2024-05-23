# Comparing `tmp/datacleanerpandas-0.1.0.tar.gz` & `tmp/datacleanerpandas-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datacleanerpandas-0.1.0.tar", last modified: Tue May 21 20:16:11 2024, max compression
+gzip compressed data, was "datacleanerpandas-0.1.1.tar", last modified: Thu May 23 11:50:06 2024, max compression
```

## Comparing `datacleanerpandas-0.1.0.tar` & `datacleanerpandas-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 20:16:11.282072 datacleanerpandas-0.1.0/
--rw-rw-rw-   0        0        0      669 2024-05-21 20:16:11.278074 datacleanerpandas-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4530 2024-05-21 16:12:00.000000 datacleanerpandas-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 20:16:11.209073 datacleanerpandas-0.1.0/dataPreprocessing/
--rw-rw-rw-   0        0        0      367 2024-05-21 10:30:34.000000 datacleanerpandas-0.1.0/dataPreprocessing/__init__.py
--rw-rw-rw-   0        0        0     1049 2024-05-21 12:20:38.000000 datacleanerpandas-0.1.0/dataPreprocessing/categorical_encoder.py
--rw-rw-rw-   0        0        0     1045 2024-05-21 10:30:34.000000 datacleanerpandas-0.1.0/dataPreprocessing/data_type_converter.py
--rw-rw-rw-   0        0        0     2488 2024-05-21 10:30:34.000000 datacleanerpandas-0.1.0/dataPreprocessing/datetime_handler.py
--rw-rw-rw-   0        0        0     1255 2024-05-21 10:30:34.000000 datacleanerpandas-0.1.0/dataPreprocessing/feature_engineer.py
--rw-rw-rw-   0        0        0     2501 2024-05-21 10:30:34.000000 datacleanerpandas-0.1.0/dataPreprocessing/missing_value_handler.py
--rw-rw-rw-   0        0        0     2234 2024-05-21 10:30:34.000000 datacleanerpandas-0.1.0/dataPreprocessing/outlier_handler.py
--rw-rw-rw-   0        0        0      839 2024-05-21 10:30:34.000000 datacleanerpandas-0.1.0/dataPreprocessing/scaler.py
--rw-rw-rw-   0        0        0     1749 2024-05-21 11:53:06.000000 datacleanerpandas-0.1.0/dataPreprocessing/text_cleaner.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:16:11.273070 datacleanerpandas-0.1.0/datacleanerpandas.egg-info/
--rw-rw-rw-   0        0        0      669 2024-05-21 20:16:11.000000 datacleanerpandas-0.1.0/datacleanerpandas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      814 2024-05-21 20:16:11.000000 datacleanerpandas-0.1.0/datacleanerpandas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 20:16:11.000000 datacleanerpandas-0.1.0/datacleanerpandas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-21 20:16:11.000000 datacleanerpandas-0.1.0/datacleanerpandas.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-21 20:16:11.000000 datacleanerpandas-0.1.0/datacleanerpandas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 20:16:11.282072 datacleanerpandas-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      814 2024-05-21 20:15:37.000000 datacleanerpandas-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:16:11.271070 datacleanerpandas-0.1.0/tests/
--rw-rw-rw-   0        0        0       32 2024-05-21 10:30:34.000000 datacleanerpandas-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1399 2024-05-21 11:22:00.000000 datacleanerpandas-0.1.0/tests/test_categorical_encoder.py
--rw-rw-rw-   0        0        0     1737 2024-05-21 10:30:34.000000 datacleanerpandas-0.1.0/tests/test_data_type_converter.py
--rw-rw-rw-   0        0        0     2271 2024-05-21 10:30:34.000000 datacleanerpandas-0.1.0/tests/test_datetime_handler.py
--rw-rw-rw-   0        0        0     1836 2024-05-21 19:12:01.000000 datacleanerpandas-0.1.0/tests/test_feature_engineer.py
--rw-rw-rw-   0        0        0     3903 2024-05-21 10:30:34.000000 datacleanerpandas-0.1.0/tests/test_missing_value_handler.py
--rw-rw-rw-   0        0        0     2237 2024-05-21 10:30:34.000000 datacleanerpandas-0.1.0/tests/test_outlier_handler.py
--rw-rw-rw-   0        0        0     1443 2024-05-21 10:30:34.000000 datacleanerpandas-0.1.0/tests/test_scaler.py
--rw-rw-rw-   0        0        0     1427 2024-05-21 11:53:06.000000 datacleanerpandas-0.1.0/tests/test_text_cleaner.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:50:06.463901 datacleanerpandas-0.1.1/
+-rw-rw-rw-   0        0        0      669 2024-05-23 11:50:06.462901 datacleanerpandas-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4436 2024-05-23 07:18:58.000000 datacleanerpandas-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 11:50:06.439772 datacleanerpandas-0.1.1/dataPreprocessing/
+-rw-rw-rw-   0        0        0      359 2024-05-23 07:18:59.000000 datacleanerpandas-0.1.1/dataPreprocessing/__init__.py
+-rw-rw-rw-   0        0        0      682 2024-05-23 07:49:13.000000 datacleanerpandas-0.1.1/dataPreprocessing/categorical_encoder.py
+-rw-rw-rw-   0        0        0      493 2024-05-23 07:50:09.000000 datacleanerpandas-0.1.1/dataPreprocessing/data_type_converter.py
+-rw-rw-rw-   0        0        0     1678 2024-05-23 10:25:56.000000 datacleanerpandas-0.1.1/dataPreprocessing/datetime_handler.py
+-rw-rw-rw-   0        0        0      550 2024-05-23 07:56:04.000000 datacleanerpandas-0.1.1/dataPreprocessing/feature_engineer.py
+-rw-rw-rw-   0        0        0     1401 2024-05-23 10:43:32.000000 datacleanerpandas-0.1.1/dataPreprocessing/missing_value_handler.py
+-rw-rw-rw-   0        0        0     1010 2024-05-23 07:59:41.000000 datacleanerpandas-0.1.1/dataPreprocessing/outlier_handler.py
+-rw-rw-rw-   0        0        0      813 2024-05-23 07:18:59.000000 datacleanerpandas-0.1.1/dataPreprocessing/scaler.py
+-rw-rw-rw-   0        0        0     1131 2024-05-23 08:00:32.000000 datacleanerpandas-0.1.1/dataPreprocessing/text_cleaner.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:50:06.449896 datacleanerpandas-0.1.1/datacleanerpandas.egg-info/
+-rw-rw-rw-   0        0        0      669 2024-05-23 11:50:06.000000 datacleanerpandas-0.1.1/datacleanerpandas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      814 2024-05-23 11:50:06.000000 datacleanerpandas-0.1.1/datacleanerpandas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 11:50:06.000000 datacleanerpandas-0.1.1/datacleanerpandas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-23 11:50:06.000000 datacleanerpandas-0.1.1/datacleanerpandas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-23 11:50:06.000000 datacleanerpandas-0.1.1/datacleanerpandas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 11:50:06.463901 datacleanerpandas-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      790 2024-05-23 11:43:34.000000 datacleanerpandas-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:50:06.461902 datacleanerpandas-0.1.1/tests/
+-rw-rw-rw-   0        0        0       31 2024-05-23 07:19:00.000000 datacleanerpandas-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      956 2024-05-23 08:00:44.000000 datacleanerpandas-0.1.1/tests/test_categorical_encoder.py
+-rw-rw-rw-   0        0        0     1165 2024-05-23 08:00:53.000000 datacleanerpandas-0.1.1/tests/test_data_type_converter.py
+-rw-rw-rw-   0        0        0     1489 2024-05-23 10:25:56.000000 datacleanerpandas-0.1.1/tests/test_datetime_handler.py
+-rw-rw-rw-   0        0        0     1229 2024-05-23 08:01:10.000000 datacleanerpandas-0.1.1/tests/test_feature_engineer.py
+-rw-rw-rw-   0        0        0     2816 2024-05-23 08:01:31.000000 datacleanerpandas-0.1.1/tests/test_missing_value_handler.py
+-rw-rw-rw-   0        0        0     1550 2024-05-23 08:01:49.000000 datacleanerpandas-0.1.1/tests/test_outlier_handler.py
+-rw-rw-rw-   0        0        0     1398 2024-05-23 07:19:00.000000 datacleanerpandas-0.1.1/tests/test_scaler.py
+-rw-rw-rw-   0        0        0     1386 2024-05-23 07:19:00.000000 datacleanerpandas-0.1.1/tests/test_text_cleaner.py
```

### Comparing `datacleanerpandas-0.1.0/PKG-INFO` & `datacleanerpandas-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: datacleanerpandas
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for handling various data preprocessing tasks
 Home-page: https://github.com/baharkarakas/datacleanerpandas
-Download-URL: https://github.com/baharkarakas/datacleanerpandas/archive/refs/tags/v0.1.0.tar.gz
+Download-URL: https://github.com/baharkarakas/datacleanerpandas/archive/refs/tags/v0.1.1.tar.gz
 Author: baharkarakas & AlperCna
 Author-email: support@pandasdatacleaner.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Requires-Dist: pandas
```

### Comparing `datacleanerpandas-0.1.0/dataPreprocessing/scaler.py` & `datacleanerpandas-0.1.1/dataPreprocessing/scaler.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from sklearn.preprocessing import StandardScaler, MinMaxScaler
-
-class Scaler:
-    def __init__(self, method="standard"):
-        if method == "standard":
-            self.scaler = StandardScaler()
-        elif method == "minmax":
-            self.scaler = MinMaxScaler()
-        else:
-            raise ValueError("Invalid method: choose 'standard' or 'minmax'")
-        self.columns = None
-
-    def fit(self, X):
-        numeric_cols = X.select_dtypes(include=['number'])
-        self.columns = numeric_cols.columns
-        self.scaler.fit(numeric_cols)
-        return self
-
-    def transform(self, X):
-        X_copy = X.copy()
-        X_copy[self.columns] = self.scaler.transform(X_copy[self.columns])
-        return X_copy
-
-    def fit_transform(self, X):
-        self.fit(X)
-        return self.transform(X)
+from sklearn.preprocessing import StandardScaler, MinMaxScaler
+
+class Scaler:
+    def __init__(self, method="standard"):
+        if method == "standard":
+            self.scaler = StandardScaler()
+        elif method == "minmax":
+            self.scaler = MinMaxScaler()
+        else:
+            raise ValueError("Invalid method: choose 'standard' or 'minmax'")
+        self.columns = None
+
+    def fit(self, X):
+        numeric_cols = X.select_dtypes(include=['number'])
+        self.columns = numeric_cols.columns
+        self.scaler.fit(numeric_cols)
+        return self
+
+    def transform(self, X):
+        X_copy = X.copy()
+        X_copy[self.columns] = self.scaler.transform(X_copy[self.columns])
+        return X_copy
+
+    def fit_transform(self, X):
+        self.fit(X)
+        return self.transform(X)
```

### Comparing `datacleanerpandas-0.1.0/datacleanerpandas.egg-info/PKG-INFO` & `datacleanerpandas-0.1.1/datacleanerpandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: datacleanerpandas
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for handling various data preprocessing tasks
 Home-page: https://github.com/baharkarakas/datacleanerpandas
-Download-URL: https://github.com/baharkarakas/datacleanerpandas/archive/refs/tags/v0.1.0.tar.gz
+Download-URL: https://github.com/baharkarakas/datacleanerpandas/archive/refs/tags/v0.1.1.tar.gz
 Author: baharkarakas & AlperCna
 Author-email: support@pandasdatacleaner.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Requires-Dist: pandas
```

### Comparing `datacleanerpandas-0.1.0/datacleanerpandas.egg-info/SOURCES.txt` & `datacleanerpandas-0.1.1/datacleanerpandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datacleanerpandas-0.1.0/tests/test_data_type_converter.py` & `datacleanerpandas-0.1.1/tests/test_data_type_converter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,32 @@
-import unittest
-import pandas as pd
-from dataPreprocessing.data_type_converter import DataTypeConverter
-
-
-class TestDataTypeConverter(unittest.TestCase):
-    """
-    TestDataTypeConverter is a test class for the DataTypeConverter class, ensuring the correct functionality of data type conversions.
-
-    Methods:
-        setUp():
-            Initializes a sample DataFrame for testing.
-
-        test_to_numeric():
-            Tests the conversion of a column to numeric values.
-
-        test_to_categorical():
-            Tests the conversion of a column to categorical values.
-
-        test_to_datetime():
-            Tests the conversion of a column to datetime objects.
-    """
-
-    def setUp(self):
-        self.data = pd.DataFrame({
-            'numeric_str': ['1', '2', '3', 'invalid'],
-            'categorical_str': ['A', 'B', 'A', 'C'],
-            'date_str': ['2023-05-19', '2024-05-19', 'invalid', '2025-05-19']
-        })
-
-    def test_to_numeric(self):
-        df = DataTypeConverter.to_numeric(self.data.copy(), 'numeric_str')
-        self.assertTrue(pd.api.types.is_numeric_dtype(df['numeric_str']))
-        self.assertTrue(df['numeric_str'].isna().iloc[3])
-
-    def test_to_categorical(self):
-        df = DataTypeConverter.to_categorical(self.data.copy(), 'categorical_str')
-        self.assertTrue(isinstance(df['categorical_str'].dtype, pd.CategoricalDtype))
-
-    def test_to_datetime(self):
-        df = DataTypeConverter.to_datetime(self.data.copy(), 'date_str', date_format='%Y-%m-%d')
-        self.assertTrue(pd.api.types.is_datetime64_any_dtype(df['date_str']))
-        self.assertTrue(df['date_str'].isna().iloc[2])
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+import pandas as pd
+from dataPreprocessing.data_type_converter import DataTypeConverter
+
+
+class TestDataTypeConverter(unittest.TestCase):
+
+
+    def setUp(self):
+        self.data = pd.DataFrame({
+            'numeric_str': ['1', '2', '3', 'invalid'],
+            'categorical_str': ['A', 'B', 'A', 'C'],
+            'date_str': ['2023-05-19', '2024-05-19', 'invalid', '2025-05-19']
+        })
+
+    def test_to_numeric(self):
+        df = DataTypeConverter.to_numeric(self.data.copy(), 'numeric_str')
+        self.assertTrue(pd.api.types.is_numeric_dtype(df['numeric_str']))
+        self.assertTrue(df['numeric_str'].isna().iloc[3])
+
+    def test_to_categorical(self):
+        df = DataTypeConverter.to_categorical(self.data.copy(), 'categorical_str')
+        self.assertTrue(isinstance(df['categorical_str'].dtype, pd.CategoricalDtype))
+
+    def test_to_datetime(self):
+        df = DataTypeConverter.to_datetime(self.data.copy(), 'date_str', date_format='%Y-%m-%d')
+        self.assertTrue(pd.api.types.is_datetime64_any_dtype(df['date_str']))
+        self.assertTrue(df['date_str'].isna().iloc[2])
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `datacleanerpandas-0.1.0/tests/test_datetime_handler.py` & `datacleanerpandas-0.1.1/tests/test_datetime_handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,40 @@
-import unittest
-import pandas as pd
-from datetime import datetime
-
-from dataPreprocessing.datetime_handler import DateTimeHandler
-
-
-class TestDateTimeHandler(unittest.TestCase):
-    """
-    TestDateTimeHandler is a test class for the DateTimeHandler class, ensuring the correct functionality of date and time manipulations.
-
-    Methods:
-        setUp():
-            Initializes a sample DataFrame with datetime data for testing.
-
-        test_convert_to_datetime():
-            Tests the conversion of a column to datetime objects.
-
-        test_extract_date_component():
-            Tests the extraction of specific date components from a datetime column.
-
-        test_calculate_date_difference():
-            Tests the calculation of the difference between two datetime columns.
-
-        test_add_to_date():
-            Tests the addition of a specified amount of time to a datetime column.
-    """
-
-    def setUp(self):
-        self.data = pd.DataFrame({
-            'date1': ['2023-05-19', '2024-05-19', '2025-05-19'],
-            'date2': ['2023-04-19', '2023-05-19', '2023-06-19']
-        })
-        self.data = DateTimeHandler.convert_to_datetime(self.data, 'date1')
-        self.data = DateTimeHandler.convert_to_datetime(self.data, 'date2')
-
-    def test_convert_to_datetime(self):
-        df = pd.DataFrame({'date': ['2023-05-19', '2024-05-19', '2025-05-19']})
-        df = DateTimeHandler.convert_to_datetime(df, 'date')
-        self.assertTrue(pd.api.types.is_datetime64_any_dtype(df['date']))
-
-    def test_extract_date_component(self):
-        df = DateTimeHandler.extract_date_component(self.data, 'date1', 'year')
-        self.assertIn('date1_year', df.columns)
-        self.assertEqual(df['date1_year'].iloc[0], 2023)
-
-    def test_calculate_date_difference(self):
-        df = DateTimeHandler.calculate_date_difference(self.data, 'date1', 'date2')
-        self.assertIn('date1_vs_date2_diff', df.columns)
-        self.assertEqual(df['date1_vs_date2_diff'].iloc[0], 30)
-
-    def test_add_to_date(self):
-        df = DateTimeHandler.add_to_date(self.data, 'date1', 10, 'days')
-        self.assertEqual(df['date1'].iloc[0], datetime(2023, 5, 29))
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+import pandas as pd
+from datetime import datetime
+
+from dataPreprocessing.datetime_handler import DateTimeHandler
+
+
+class TestDateTimeHandler(unittest.TestCase):
+
+
+    def setUp(self):
+        self.data = pd.DataFrame({
+            'date1': ['2023-05-19', '2024-05-19', '2025-05-19'],
+            'date2': ['2023-04-19', '2023-05-19', '2023-06-19']
+        })
+        self.data = DateTimeHandler.convert_to_datetime(self.data, 'date1')
+        self.data = DateTimeHandler.convert_to_datetime(self.data, 'date2')
+
+    def test_convert_to_datetime(self):
+        df = pd.DataFrame({'date': ['2023-05-19', '2024-05-19', '2025-05-19']})
+        df = DateTimeHandler.convert_to_datetime(df, 'date')
+        self.assertTrue(pd.api.types.is_datetime64_any_dtype(df['date']))
+
+    def test_extract_date_component(self):
+        df = DateTimeHandler.extract_date_component(self.data, 'date1', 'year')
+        self.assertIn('date1_year', df.columns)
+        self.assertEqual(df['date1_year'].iloc[0], 2023)
+
+    def test_calculate_date_difference(self):
+        df = DateTimeHandler.calculate_date_difference(self.data, 'date1', 'date2')
+        self.assertIn('date1_vs_date2_diff', df.columns)
+        self.assertEqual(df['date1_vs_date2_diff'].iloc[0], 30)
+
+    def test_add_to_date(self):
+        df = DateTimeHandler.add_to_date(self.data, 'date1', 10, 'days')
+        self.assertEqual(df['date1'].iloc[0], datetime(2023, 5, 29))
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `datacleanerpandas-0.1.0/tests/test_feature_engineer.py` & `datacleanerpandas-0.1.1/tests/test_feature_engineer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,37 @@
-import unittest
-import pandas as pd
-from dataPreprocessing.feature_engineer import FeatureEngineer
-
-
-class TestFeatureEngineer(unittest.TestCase):
-    """
-    TestFeatureEngineer is a test class for the FeatureEngineer class, ensuring the correct functionality of feature engineering.
-
-    Methods:
-        setUp():
-            Initializes a sample DataFrame for testing.
-
-        test_add_difference():
-            Tests the addition of a difference column.
-
-        test_add_product():
-            Tests the addition of a product column.
-
-        test_add_sum():
-            Tests the addition of a sum column.
-
-        test_add_square():
-            Tests the addition of a square column.
-    """
-
-    def setUp(self):
-        self.data = pd.DataFrame({
-            'A': [1, 2, 3, 4],
-            'B': [4, 3, 2, 1]
-        })
-
-    def test_add_difference(self):
-        df = FeatureEngineer.add_difference(self.data.copy(), 'A', 'B', 'A_minus_B')
-        self.assertIn('A_minus_B', df.columns)
-        self.assertListEqual(list(df['A_minus_B']), [-3, -1, 1, 3])
-
-    def test_add_product(self):
-        df = FeatureEngineer.add_product(self.data.copy(), 'A', 'B', 'A_times_B')
-        self.assertIn('A_times_B', df.columns)
-        self.assertListEqual(list(df['A_times_B']), [4, 6, 6, 4])
-
-    def test_add_sum(self):
-        df = FeatureEngineer.add_sum(self.data.copy(), 'A', 'B', 'A_plus_B')
-        self.assertIn('A_plus_B', df.columns)
-        self.assertListEqual(list(df['A_plus_B']), [5, 5, 5, 5])
-
-    def test_add_square(self):
-        df = FeatureEngineer.add_square(self.data.copy(), 'A', 'A_squared')
-        self.assertIn('A_squared', df.columns)
-        self.assertListEqual(list(df['A_squared']), [1, 4, 9, 16])
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+import pandas as pd
+from dataPreprocessing.feature_engineer import FeatureEngineer
+
+
+class TestFeatureEngineer(unittest.TestCase):
+
+
+    def setUp(self):
+        self.data = pd.DataFrame({
+            'A': [1, 2, 3, 4],
+            'B': [4, 3, 2, 1]
+        })
+
+    def test_add_difference(self):
+        df = FeatureEngineer.add_difference(self.data.copy(), 'A', 'B', 'A_minus_B')
+        self.assertIn('A_minus_B', df.columns)
+        self.assertListEqual(list(df['A_minus_B']), [-3, -1, 1, 3])
+
+    def test_add_product(self):
+        df = FeatureEngineer.add_product(self.data.copy(), 'A', 'B', 'A_times_B')
+        self.assertIn('A_times_B', df.columns)
+        self.assertListEqual(list(df['A_times_B']), [4, 6, 6, 4])
+
+    def test_add_sum(self):
+        df = FeatureEngineer.add_sum(self.data.copy(), 'A', 'B', 'A_plus_B')
+        self.assertIn('A_plus_B', df.columns)
+        self.assertListEqual(list(df['A_plus_B']), [5, 5, 5, 5])
+
+    def test_add_square(self):
+        df = FeatureEngineer.add_square(self.data.copy(), 'A', 'A_squared')
+        self.assertIn('A_squared', df.columns)
+        self.assertListEqual(list(df['A_squared']), [1, 4, 9, 16])
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `datacleanerpandas-0.1.0/tests/test_outlier_handler.py` & `datacleanerpandas-0.1.1/tests/test_outlier_handler.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,44 @@
-import unittest
-import pandas as pd
-from dataPreprocessing.outlier_handler import OutlierHandler
-
-class TestOutlierHandler(unittest.TestCase):
-    """
-    TestOutlierHandler is a test class for the OutlierHandler class, ensuring the correct functionality of outlier detection and handling.
-
-    Methods:
-        setUp():
-            Initializes a sample DataFrame with potential outliers for testing.
-
-        test_outlier_removal():
-            Tests the outlier removal functionality using the default IQR method and a threshold of 1.5.
-
-        test_invalid_method():
-            Tests that an invalid method raises a ValueError.
-
-        test_custom_threshold():
-            Tests the outlier removal functionality using a custom threshold for the IQR method.
-    """
-
-    def setUp(self):
-        self.data = pd.DataFrame({
-            'A': [1, 2, 3, 4, 100],
-            'B': [1, 2, 3, 4, 5]
-        })
-
-    def test_outlier_removal(self):
-        handler = OutlierHandler(method="iqr", threshold=1.5)
-        transformed = handler.fit_transform(self.data)
-        expected = pd.DataFrame({
-            'A': [1, 2, 3, 4, 7],
-            'B': [1, 2, 3, 4, 5]
-        })
-        # Ensure expected types match the original DataFrame
-        expected['A'] = expected['A'].astype(self.data['A'].dtype)
-        expected['B'] = expected['B'].astype(self.data['B'].dtype)
-        pd.testing.assert_frame_equal(transformed, expected)
-
-    def test_invalid_method(self):
-        with self.assertRaises(ValueError):
-            handler = OutlierHandler(method="invalid_method")
-            handler.fit(self.data)
-
-    def test_custom_threshold(self):
-        handler = OutlierHandler(method="iqr", threshold=3)
-        transformed = handler.fit_transform(self.data)
-        expected = pd.DataFrame({
-            'A': [1, 2, 3, 4, 10],
-            'B': [1, 2, 3, 4, 5]
-        })
-        # Ensure expected types match the original DataFrame
-        expected['A'] = expected['A'].astype(self.data['A'].dtype)
-        expected['B'] = expected['B'].astype(self.data['B'].dtype)
-        pd.testing.assert_frame_equal(transformed, expected)
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+import pandas as pd
+from dataPreprocessing.outlier_handler import OutlierHandler
+
+class TestOutlierHandler(unittest.TestCase):
+
+
+    def setUp(self):
+        self.data = pd.DataFrame({
+            'A': [1, 2, 3, 4, 100],
+            'B': [1, 2, 3, 4, 5]
+        })
+
+    def test_outlier_removal(self):
+        handler = OutlierHandler(method="iqr", threshold=1.5)
+        transformed = handler.fit_transform(self.data)
+        expected = pd.DataFrame({
+            'A': [1, 2, 3, 4, 7],
+            'B': [1, 2, 3, 4, 5]
+        })
+        # Ensure expected types match the original DataFrame
+        expected['A'] = expected['A'].astype(self.data['A'].dtype)
+        expected['B'] = expected['B'].astype(self.data['B'].dtype)
+        pd.testing.assert_frame_equal(transformed, expected)
+
+    def test_invalid_method(self):
+        with self.assertRaises(ValueError):
+            handler = OutlierHandler(method="invalid_method")
+            handler.fit(self.data)
+
+    def test_custom_threshold(self):
+        handler = OutlierHandler(method="iqr", threshold=3)
+        transformed = handler.fit_transform(self.data)
+        expected = pd.DataFrame({
+            'A': [1, 2, 3, 4, 10],
+            'B': [1, 2, 3, 4, 5]
+        })
+        # Ensure expected types match the original DataFrame
+        expected['A'] = expected['A'].astype(self.data['A'].dtype)
+        expected['B'] = expected['B'].astype(self.data['B'].dtype)
+        pd.testing.assert_frame_equal(transformed, expected)
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `datacleanerpandas-0.1.0/tests/test_scaler.py` & `datacleanerpandas-0.1.1/tests/test_scaler.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-# tests/test_scaler.py
-
-import unittest
-import pandas as pd
-
-from dataPreprocessing.scaler import Scaler
-
-
-class TestScaler(unittest.TestCase):
-
-    def setUp(self):
-        self.data = pd.DataFrame({
-            'A': [1, 2, 3, 4, 5],
-            'B': [10, 20, 30, 40, 50]
-        })
-
-    def test_minmax_scaler(self):
-        scaler = Scaler(method="minmax")
-        transformed = scaler.fit_transform(self.data)
-        expected = pd.DataFrame({
-            'A': [0.0, 0.25, 0.5, 0.75, 1.0],
-            'B': [0.0, 0.25, 0.5, 0.75, 1.0]
-        })
-        pd.testing.assert_frame_equal(pd.DataFrame(transformed, columns=self.data.columns), expected)
-
-    def test_standard_scaler(self):
-        scaler = Scaler(method="standard")
-        transformed = scaler.fit_transform(self.data)
-        expected = pd.DataFrame({
-            'A': [-1.414214, -0.707107, 0.000000, 0.707107, 1.414214],
-            'B': [-1.414214, -0.707107, 0.000000, 0.707107, 1.414214]
-        })
-        pd.testing.assert_frame_equal(
-            pd.DataFrame(transformed, columns=self.data.columns),
-            expected,
-            check_dtype=False, # Skipping the "checking for given data type"
-            atol=1e-5 # Mutlak tolerans
-        )
-
-    def test_invalid_method(self):
-        with self.assertRaises(ValueError):
-            Scaler(method="invalid_method")
-
-if __name__ == '__main__':
-    unittest.main()
+# tests/test_scaler.py
+
+import unittest
+import pandas as pd
+
+from dataPreprocessing.scaler import Scaler
+
+
+class TestScaler(unittest.TestCase):
+
+    def setUp(self):
+        self.data = pd.DataFrame({
+            'A': [1, 2, 3, 4, 5],
+            'B': [10, 20, 30, 40, 50]
+        })
+
+    def test_minmax_scaler(self):
+        scaler = Scaler(method="minmax")
+        transformed = scaler.fit_transform(self.data)
+        expected = pd.DataFrame({
+            'A': [0.0, 0.25, 0.5, 0.75, 1.0],
+            'B': [0.0, 0.25, 0.5, 0.75, 1.0]
+        })
+        pd.testing.assert_frame_equal(pd.DataFrame(transformed, columns=self.data.columns), expected)
+
+    def test_standard_scaler(self):
+        scaler = Scaler(method="standard")
+        transformed = scaler.fit_transform(self.data)
+        expected = pd.DataFrame({
+            'A': [-1.414214, -0.707107, 0.000000, 0.707107, 1.414214],
+            'B': [-1.414214, -0.707107, 0.000000, 0.707107, 1.414214]
+        })
+        pd.testing.assert_frame_equal(
+            pd.DataFrame(transformed, columns=self.data.columns),
+            expected,
+            check_dtype=False, # Skipping the "checking for given data type"
+            atol=1e-5 # Mutlak tolerans
+        )
+
+    def test_invalid_method(self):
+        with self.assertRaises(ValueError):
+            Scaler(method="invalid_method")
+
+if __name__ == '__main__':
+    unittest.main()
```

