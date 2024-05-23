# Comparing `tmp/cleaner_panda-0.1.5.tar.gz` & `tmp/cleaner_panda-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleaner_panda-0.1.5.tar", last modified: Thu May 23 14:02:51 2024, max compression
+gzip compressed data, was "cleaner_panda-0.1.6.tar", last modified: Thu May 23 14:32:00 2024, max compression
```

## Comparing `cleaner_panda-0.1.5.tar` & `cleaner_panda-0.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 14:02:51.179863 cleaner_panda-0.1.5/
--rw-rw-rw-   0        0        0    35802 2024-05-09 22:17:47.000000 cleaner_panda-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     2959 2024-05-23 14:02:51.178863 cleaner_panda-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2182 2024-05-23 14:02:48.000000 cleaner_panda-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 14:02:51.161821 cleaner_panda-0.1.5/cleaner_panda/
--rw-rw-rw-   0        0        0      508 2024-05-23 13:46:42.000000 cleaner_panda-0.1.5/cleaner_panda/__init__.py
--rw-rw-rw-   0        0        0     1263 2024-05-21 14:18:40.000000 cleaner_panda-0.1.5/cleaner_panda/categorical_encoder.py
--rw-rw-rw-   0        0        0      652 2024-05-21 14:18:40.000000 cleaner_panda-0.1.5/cleaner_panda/data_type_converter.py
--rw-rw-rw-   0        0        0     3440 2024-05-21 14:18:40.000000 cleaner_panda-0.1.5/cleaner_panda/date_time_handler.py
--rw-rw-rw-   0        0        0     3553 2024-05-23 13:46:42.000000 cleaner_panda-0.1.5/cleaner_panda/missing_value_handler.py
--rw-rw-rw-   0        0        0     2671 2024-05-21 14:18:40.000000 cleaner_panda-0.1.5/cleaner_panda/outlier_handler.py
--rw-rw-rw-   0        0        0     1681 2024-05-21 14:18:40.000000 cleaner_panda-0.1.5/cleaner_panda/scaler.py
--rw-rw-rw-   0        0        0     3224 2024-05-21 14:18:40.000000 cleaner_panda-0.1.5/cleaner_panda/text_cleaner.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:02:51.177860 cleaner_panda-0.1.5/cleaner_panda.egg-info/
--rw-rw-rw-   0        0        0     2959 2024-05-23 14:02:51.000000 cleaner_panda-0.1.5/cleaner_panda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      713 2024-05-23 14:02:51.000000 cleaner_panda-0.1.5/cleaner_panda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 14:02:51.000000 cleaner_panda-0.1.5/cleaner_panda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-05-23 14:02:51.000000 cleaner_panda-0.1.5/cleaner_panda.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-23 14:02:51.000000 cleaner_panda-0.1.5/cleaner_panda.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-23 14:02:51.179863 cleaner_panda-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1024 2024-05-23 13:55:28.000000 cleaner_panda-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:02:51.175334 cleaner_panda-0.1.5/tests/
--rw-rw-rw-   0        0        0        0 2024-05-18 10:16:31.000000 cleaner_panda-0.1.5/tests/__init__.py
--rw-rw-rw-   0        0        0     1896 2024-05-23 13:46:42.000000 cleaner_panda-0.1.5/tests/test_categorical_encoder.py
--rw-rw-rw-   0        0        0     1343 2024-05-21 14:22:32.000000 cleaner_panda-0.1.5/tests/test_data_type_converter.py
--rw-rw-rw-   0        0        0     3973 2024-05-21 18:53:13.000000 cleaner_panda-0.1.5/tests/test_date_time_handler.py
--rw-rw-rw-   0        0        0     3853 2024-05-21 14:27:08.000000 cleaner_panda-0.1.5/tests/test_missing_value_handler.py
--rw-rw-rw-   0        0        0     2743 2024-05-21 18:53:13.000000 cleaner_panda-0.1.5/tests/test_outlier_handler.py
--rw-rw-rw-   0        0        0     3701 2024-05-21 18:53:13.000000 cleaner_panda-0.1.5/tests/test_scaler.py
--rw-rw-rw-   0        0        0     4451 2024-05-21 18:53:13.000000 cleaner_panda-0.1.5/tests/test_text_cleaner.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:00.435687 cleaner_panda-0.1.6/
+-rw-rw-rw-   0        0        0    35802 2024-05-09 22:17:47.000000 cleaner_panda-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     3013 2024-05-23 14:32:00.435687 cleaner_panda-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2236 2024-05-23 14:31:35.000000 cleaner_panda-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:00.421733 cleaner_panda-0.1.6/cleaner_panda/
+-rw-rw-rw-   0        0        0      508 2024-05-23 13:46:42.000000 cleaner_panda-0.1.6/cleaner_panda/__init__.py
+-rw-rw-rw-   0        0        0     1263 2024-05-21 14:18:40.000000 cleaner_panda-0.1.6/cleaner_panda/categorical_encoder.py
+-rw-rw-rw-   0        0        0      652 2024-05-21 14:18:40.000000 cleaner_panda-0.1.6/cleaner_panda/data_type_converter.py
+-rw-rw-rw-   0        0        0     3440 2024-05-21 14:18:40.000000 cleaner_panda-0.1.6/cleaner_panda/date_time_handler.py
+-rw-rw-rw-   0        0        0     3785 2024-05-23 14:29:00.000000 cleaner_panda-0.1.6/cleaner_panda/missing_value_handler.py
+-rw-rw-rw-   0        0        0     2671 2024-05-21 14:18:40.000000 cleaner_panda-0.1.6/cleaner_panda/outlier_handler.py
+-rw-rw-rw-   0        0        0     1681 2024-05-21 14:18:40.000000 cleaner_panda-0.1.6/cleaner_panda/scaler.py
+-rw-rw-rw-   0        0        0     3224 2024-05-21 14:18:40.000000 cleaner_panda-0.1.6/cleaner_panda/text_cleaner.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:00.434634 cleaner_panda-0.1.6/cleaner_panda.egg-info/
+-rw-rw-rw-   0        0        0     3013 2024-05-23 14:32:00.000000 cleaner_panda-0.1.6/cleaner_panda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2024-05-23 14:32:00.000000 cleaner_panda-0.1.6/cleaner_panda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 14:32:00.000000 cleaner_panda-0.1.6/cleaner_panda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-05-23 14:32:00.000000 cleaner_panda-0.1.6/cleaner_panda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-23 14:32:00.000000 cleaner_panda-0.1.6/cleaner_panda.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-23 14:32:00.437193 cleaner_panda-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1024 2024-05-23 14:30:41.000000 cleaner_panda-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:00.433503 cleaner_panda-0.1.6/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-18 10:16:31.000000 cleaner_panda-0.1.6/tests/__init__.py
+-rw-rw-rw-   0        0        0     1896 2024-05-23 13:46:42.000000 cleaner_panda-0.1.6/tests/test_categorical_encoder.py
+-rw-rw-rw-   0        0        0     1343 2024-05-21 14:22:32.000000 cleaner_panda-0.1.6/tests/test_data_type_converter.py
+-rw-rw-rw-   0        0        0     3973 2024-05-21 18:53:13.000000 cleaner_panda-0.1.6/tests/test_date_time_handler.py
+-rw-rw-rw-   0        0        0     3853 2024-05-21 14:27:08.000000 cleaner_panda-0.1.6/tests/test_missing_value_handler.py
+-rw-rw-rw-   0        0        0     2743 2024-05-21 18:53:13.000000 cleaner_panda-0.1.6/tests/test_outlier_handler.py
+-rw-rw-rw-   0        0        0     3701 2024-05-21 18:53:13.000000 cleaner_panda-0.1.6/tests/test_scaler.py
+-rw-rw-rw-   0        0        0     4451 2024-05-21 18:53:13.000000 cleaner_panda-0.1.6/tests/test_text_cleaner.py
```

### Comparing `cleaner_panda-0.1.5/LICENSE` & `cleaner_panda-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.5/PKG-INFO` & `cleaner_panda-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cleaner_panda
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for handling various data preprocessing tasks
 Home-page: https://github.com/EmirhanSyl/cleaner-panda
-Download-URL: https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.5.tar.gz
+Download-URL: https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.6.tar.gz
 Author: asimtarik & emirs
 Author-email: support@cleanpanda.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -20,15 +20,15 @@
 Requires-Dist: scipy
 Requires-Dist: bs4
 Requires-Dist: contractions
 
 # Cleaner Panda
  Programming For Data Engineering course final project
 
-![logo.jpg](logo.jpg)
+![https://github.com/EmirhanSyl/cleaner-panda/blob/main/logo.jpg](logo.jpg)
 
  https://pypi.org/project/cleaner-panda/
 
  ## Installation
  `pip install cleaner-panda`
```

### Comparing `cleaner_panda-0.1.5/README.md` & `cleaner_panda-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Cleaner Panda
  Programming For Data Engineering course final project
 
-![logo.jpg](logo.jpg)
+![https://github.com/EmirhanSyl/cleaner-panda/blob/main/logo.jpg](logo.jpg)
 
  https://pypi.org/project/cleaner-panda/
 
  ## Installation
  `pip install cleaner-panda`
```

### Comparing `cleaner_panda-0.1.5/cleaner_panda/categorical_encoder.py` & `cleaner_panda-0.1.6/cleaner_panda/categorical_encoder.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.5/cleaner_panda/data_type_converter.py` & `cleaner_panda-0.1.6/cleaner_panda/data_type_converter.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.5/cleaner_panda/date_time_handler.py` & `cleaner_panda-0.1.6/cleaner_panda/date_time_handler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.5/cleaner_panda/missing_value_handler.py` & `cleaner_panda-0.1.6/cleaner_panda/missing_value_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,46 +33,51 @@
             return self.replace_remove_column(dataframe, column)
         elif strategy == self.Strategy.FORWARD_BACKWARD:
             return self.replace_forward_backward(dataframe, column)
         else:
             raise ValueError("Invalid strategy")
 
     def replace_mean(self, dataframe: pd.DataFrame, column: Union[int, str]) -> pd.DataFrame:
-        if pd.api.types.is_numeric_dtype(dataframe[column]):
-            mean_value = dataframe[column].mean()
-            dataframe[column].fillna(mean_value)
+        df_copy = dataframe.copy()
+        if pd.api.types.is_numeric_dtype(df_copy[column]):
+            mean_value = df_copy[column].mean()
+            df_copy[column].fillna(mean_value, inplace=True)
         else:
             raise ValueError(f"Column '{column}' is not numeric. Skipping mean replacement...")
-        
-        return dataframe
+        return df_copy
 
     def replace_median(self, dataframe: pd.DataFrame, column: Union[int, str]) -> pd.DataFrame:
-        if pd.api.types.is_numeric_dtype(dataframe[column]):
-            median_value = dataframe[column].median()
-            dataframe[column].fillna(median_value)
+        df_copy = dataframe.copy()
+        if pd.api.types.is_numeric_dtype(df_copy[column]):
+            median_value = df_copy[column].median()
+            df_copy[column].fillna(median_value, inplace=True)
         else:
             raise ValueError(f"Column '{column}' is not numeric. Skipping median replacement.")
-        return dataframe
+        return df_copy
 
     def replace_constant(self, dataframe: pd.DataFrame, column: Union[int, str]) -> pd.DataFrame:
-        if pd.api.types.is_numeric_dtype(dataframe[column]):
+        df_copy = dataframe.copy()
+        if pd.api.types.is_numeric_dtype(df_copy[column]):
             const_value = self.const_int
-        elif pd.api.types.is_string_dtype(dataframe[column]):
+        elif pd.api.types.is_string_dtype(df_copy[column]):
             const_value = self.const_str
-        elif pd.api.types.is_datetime64_any_dtype(dataframe[column]):
+        elif pd.api.types.is_datetime64_any_dtype(df_copy[column]):
             const_value = self.const_date
         else:
             raise ValueError(f"Unsupported column type for column '{column}'")
-        
-        dataframe[column].fillna(const_value)
-        return dataframe
+
+        df_copy[column].fillna(const_value, inplace=True)
+        return df_copy
 
     def replace_remove_row(self, dataframe: pd.DataFrame, column: Union[int, str]) -> pd.DataFrame:
-        return dataframe.dropna(subset=[column])
+        df_copy = dataframe.copy()
+        return df_copy.dropna(subset=[column])
 
     def replace_remove_column(self, dataframe: pd.DataFrame, column: Union[int, str]) -> pd.DataFrame:
-        return dataframe.drop(columns=[column])
+        df_copy = dataframe.copy()
+        return df_copy.drop(columns=[column])
 
     def replace_forward_backward(self, dataframe: pd.DataFrame, column: Union[int, str]) -> pd.DataFrame:
-        dataframe[column].fillna(method='ffill')
-        dataframe[column].fillna(method='bfill')
-        return dataframe
+        df_copy = dataframe.copy()
+        df_copy[column].fillna(method='ffill', inplace=True)
+        df_copy[column].fillna(method='bfill', inplace=True)
+        return df_copy
```

### Comparing `cleaner_panda-0.1.5/cleaner_panda/outlier_handler.py` & `cleaner_panda-0.1.6/cleaner_panda/outlier_handler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.5/cleaner_panda/scaler.py` & `cleaner_panda-0.1.6/cleaner_panda/scaler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.5/cleaner_panda/text_cleaner.py` & `cleaner_panda-0.1.6/cleaner_panda/text_cleaner.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.5/cleaner_panda.egg-info/PKG-INFO` & `cleaner_panda-0.1.6/cleaner_panda.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cleaner_panda
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for handling various data preprocessing tasks
 Home-page: https://github.com/EmirhanSyl/cleaner-panda
-Download-URL: https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.5.tar.gz
+Download-URL: https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.6.tar.gz
 Author: asimtarik & emirs
 Author-email: support@cleanpanda.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -20,15 +20,15 @@
 Requires-Dist: scipy
 Requires-Dist: bs4
 Requires-Dist: contractions
 
 # Cleaner Panda
  Programming For Data Engineering course final project
 
-![logo.jpg](logo.jpg)
+![https://github.com/EmirhanSyl/cleaner-panda/blob/main/logo.jpg](logo.jpg)
 
  https://pypi.org/project/cleaner-panda/
 
  ## Installation
  `pip install cleaner-panda`
```

### Comparing `cleaner_panda-0.1.5/cleaner_panda.egg-info/SOURCES.txt` & `cleaner_panda-0.1.6/cleaner_panda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.5/setup.py` & `cleaner_panda-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 from setuptools import setup, find_packages
 
 setup(
     name='cleaner_panda',
-    version='0.1.5',
+    version='0.1.6',
     description='A package for handling various data preprocessing tasks',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='asimtarik & emirs',
     author_email='support@cleanpanda.com',
     url='https://github.com/EmirhanSyl/cleaner-panda',
-    download_url='https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.5.tar.gz',
+    download_url='https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.6.tar.gz',
     packages=find_packages(),
     install_requires=[
         'pandas',
         'numpy',
         'scikit-learn',
         'nltk',
         'category_encoders',
```

### Comparing `cleaner_panda-0.1.5/tests/test_categorical_encoder.py` & `cleaner_panda-0.1.6/tests/test_categorical_encoder.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.5/tests/test_data_type_converter.py` & `cleaner_panda-0.1.6/tests/test_data_type_converter.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.5/tests/test_date_time_handler.py` & `cleaner_panda-0.1.6/tests/test_date_time_handler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.5/tests/test_missing_value_handler.py` & `cleaner_panda-0.1.6/tests/test_missing_value_handler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.5/tests/test_outlier_handler.py` & `cleaner_panda-0.1.6/tests/test_outlier_handler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.5/tests/test_scaler.py` & `cleaner_panda-0.1.6/tests/test_scaler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.5/tests/test_text_cleaner.py` & `cleaner_panda-0.1.6/tests/test_text_cleaner.py`

 * *Files identical despite different names*

