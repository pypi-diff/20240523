# Comparing `tmp/cleaner_panda-0.1.4.tar.gz` & `tmp/cleaner_panda-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleaner_panda-0.1.4.tar", last modified: Tue May 21 16:52:12 2024, max compression
+gzip compressed data, was "cleaner_panda-0.1.5.tar", last modified: Thu May 23 14:02:51 2024, max compression
```

## Comparing `cleaner_panda-0.1.4.tar` & `cleaner_panda-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 16:52:12.665317 cleaner_panda-0.1.4/
--rw-rw-rw-   0        0        0    35803 2024-05-20 15:24:41.000000 cleaner_panda-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     2928 2024-05-21 16:52:12.666333 cleaner_panda-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2310 2024-05-21 13:52:39.000000 cleaner_panda-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 16:52:12.603645 cleaner_panda-0.1.4/cleaner_panda/
--rw-rw-rw-   0        0        0      534 2024-05-21 16:51:13.000000 cleaner_panda-0.1.4/cleaner_panda/__init__.py
--rw-rw-rw-   0        0        0     1263 2024-05-21 12:25:42.000000 cleaner_panda-0.1.4/cleaner_panda/categorical_encoder.py
--rw-rw-rw-   0        0        0      652 2024-05-21 10:46:50.000000 cleaner_panda-0.1.4/cleaner_panda/data_type_converter.py
--rw-rw-rw-   0        0        0     3440 2024-05-21 13:52:39.000000 cleaner_panda-0.1.4/cleaner_panda/date_time_handler.py
--rw-rw-rw-   0        0        0     3623 2024-05-21 14:33:42.000000 cleaner_panda-0.1.4/cleaner_panda/missing_value_handler.py
--rw-rw-rw-   0        0        0     2671 2024-05-20 15:42:21.000000 cleaner_panda-0.1.4/cleaner_panda/outlier_handler.py
--rw-rw-rw-   0        0        0     1681 2024-05-21 10:47:33.000000 cleaner_panda-0.1.4/cleaner_panda/scaler.py
--rw-rw-rw-   0        0        0     3224 2024-05-21 10:47:33.000000 cleaner_panda-0.1.4/cleaner_panda/text_cleaner.py
-drwxrwxrwx   0        0        0        0 2024-05-21 16:52:12.638560 cleaner_panda-0.1.4/cleaner_panda.egg-info/
--rw-rw-rw-   0        0        0     2928 2024-05-21 16:52:12.000000 cleaner_panda-0.1.4/cleaner_panda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      713 2024-05-21 16:52:12.000000 cleaner_panda-0.1.4/cleaner_panda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 16:52:12.000000 cleaner_panda-0.1.4/cleaner_panda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-05-21 16:52:12.000000 cleaner_panda-0.1.4/cleaner_panda.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-21 16:52:12.000000 cleaner_panda-0.1.4/cleaner_panda.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-21 16:52:12.669856 cleaner_panda-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1024 2024-05-21 16:51:56.000000 cleaner_panda-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 16:52:12.663314 cleaner_panda-0.1.4/tests/
--rw-rw-rw-   0        0        0        0 2024-05-20 15:24:41.000000 cleaner_panda-0.1.4/tests/__init__.py
--rw-rw-rw-   0        0        0     1894 2024-05-21 14:31:59.000000 cleaner_panda-0.1.4/tests/test_categorical_encoder.py
--rw-rw-rw-   0        0        0     1343 2024-05-21 14:29:20.000000 cleaner_panda-0.1.4/tests/test_data_type_converter.py
--rw-rw-rw-   0        0        0     3973 2024-05-21 14:31:58.000000 cleaner_panda-0.1.4/tests/test_date_time_handler.py
--rw-rw-rw-   0        0        0     3853 2024-05-21 14:34:15.000000 cleaner_panda-0.1.4/tests/test_missing_value_handler.py
--rw-rw-rw-   0        0        0     2743 2024-05-21 14:33:33.000000 cleaner_panda-0.1.4/tests/test_outlier_handler.py
--rw-rw-rw-   0        0        0     3701 2024-05-21 14:33:31.000000 cleaner_panda-0.1.4/tests/test_scaler.py
--rw-rw-rw-   0        0        0     4451 2024-05-21 14:33:30.000000 cleaner_panda-0.1.4/tests/test_text_cleaner.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:02:51.179863 cleaner_panda-0.1.5/
+-rw-rw-rw-   0        0        0    35802 2024-05-09 22:17:47.000000 cleaner_panda-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     2959 2024-05-23 14:02:51.178863 cleaner_panda-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2182 2024-05-23 14:02:48.000000 cleaner_panda-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 14:02:51.161821 cleaner_panda-0.1.5/cleaner_panda/
+-rw-rw-rw-   0        0        0      508 2024-05-23 13:46:42.000000 cleaner_panda-0.1.5/cleaner_panda/__init__.py
+-rw-rw-rw-   0        0        0     1263 2024-05-21 14:18:40.000000 cleaner_panda-0.1.5/cleaner_panda/categorical_encoder.py
+-rw-rw-rw-   0        0        0      652 2024-05-21 14:18:40.000000 cleaner_panda-0.1.5/cleaner_panda/data_type_converter.py
+-rw-rw-rw-   0        0        0     3440 2024-05-21 14:18:40.000000 cleaner_panda-0.1.5/cleaner_panda/date_time_handler.py
+-rw-rw-rw-   0        0        0     3553 2024-05-23 13:46:42.000000 cleaner_panda-0.1.5/cleaner_panda/missing_value_handler.py
+-rw-rw-rw-   0        0        0     2671 2024-05-21 14:18:40.000000 cleaner_panda-0.1.5/cleaner_panda/outlier_handler.py
+-rw-rw-rw-   0        0        0     1681 2024-05-21 14:18:40.000000 cleaner_panda-0.1.5/cleaner_panda/scaler.py
+-rw-rw-rw-   0        0        0     3224 2024-05-21 14:18:40.000000 cleaner_panda-0.1.5/cleaner_panda/text_cleaner.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:02:51.177860 cleaner_panda-0.1.5/cleaner_panda.egg-info/
+-rw-rw-rw-   0        0        0     2959 2024-05-23 14:02:51.000000 cleaner_panda-0.1.5/cleaner_panda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2024-05-23 14:02:51.000000 cleaner_panda-0.1.5/cleaner_panda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 14:02:51.000000 cleaner_panda-0.1.5/cleaner_panda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-05-23 14:02:51.000000 cleaner_panda-0.1.5/cleaner_panda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-23 14:02:51.000000 cleaner_panda-0.1.5/cleaner_panda.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-23 14:02:51.179863 cleaner_panda-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1024 2024-05-23 13:55:28.000000 cleaner_panda-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:02:51.175334 cleaner_panda-0.1.5/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-18 10:16:31.000000 cleaner_panda-0.1.5/tests/__init__.py
+-rw-rw-rw-   0        0        0     1896 2024-05-23 13:46:42.000000 cleaner_panda-0.1.5/tests/test_categorical_encoder.py
+-rw-rw-rw-   0        0        0     1343 2024-05-21 14:22:32.000000 cleaner_panda-0.1.5/tests/test_data_type_converter.py
+-rw-rw-rw-   0        0        0     3973 2024-05-21 18:53:13.000000 cleaner_panda-0.1.5/tests/test_date_time_handler.py
+-rw-rw-rw-   0        0        0     3853 2024-05-21 14:27:08.000000 cleaner_panda-0.1.5/tests/test_missing_value_handler.py
+-rw-rw-rw-   0        0        0     2743 2024-05-21 18:53:13.000000 cleaner_panda-0.1.5/tests/test_outlier_handler.py
+-rw-rw-rw-   0        0        0     3701 2024-05-21 18:53:13.000000 cleaner_panda-0.1.5/tests/test_scaler.py
+-rw-rw-rw-   0        0        0     4451 2024-05-21 18:53:13.000000 cleaner_panda-0.1.5/tests/test_text_cleaner.py
```

### Comparing `cleaner_panda-0.1.4/LICENSE` & `cleaner_panda-0.1.5/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -667,8 +667,8 @@
 <https://www.gnu.org/licenses/>.
 
   The GNU General Public License does not permit incorporating your program
 into proprietary programs.  If your program is a subroutine library, you
 may consider it more useful to permit linking proprietary applications with
 the library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `cleaner_panda-0.1.4/PKG-INFO` & `cleaner_panda-0.1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,31 @@
-Metadata-Version: 2.1
-Name: cleaner_panda
-Version: 0.1.4
-Summary: A package for handling various data preprocessing tasks
-Home-page: https://github.com/EmirhanSyl/cleaner-panda
-Author: asimtarik & emirs
-Author-email: support@cleanpanda.com
-License: UNKNOWN
-Download-URL: https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.4.tar.gz
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Cleaner Panda
  Programming For Data Engineering course final project
- https://chat.openai.com/share/87c82e00-50af-446b-ac63-e82d9d35021a
+
+![logo.jpg](logo.jpg)
+
+ https://pypi.org/project/cleaner-panda/
+
+ ## Installation
+ `pip install cleaner-panda`
+
+
+## Modules
+
 
 ### Missing Value Handler
 - `strategy enum {MEAN, MEDIAN, CONSTANT, REMOVE_ROW, REMOVE_COLUMN, FORWARD_BACKWARD}`
 - `cont_int = 0, const_str =”none”, const_date=01.01.2024…`
-- `replace_missing_values(dataFrame, strategy=”strategy.MEAN”, column=0)` -> Replaces missing values on the “column” parameter according to the selected strategy. The “column” can be an index or column name as str.
+- `replace_missing_values(dataFrame, strategy=”strategy.MEAN”, column=0)`
 - `replace_mean(dataframe, column)`
 - `replace_median(dataframe, column)`
 - `replace_constant(dataframe, column, constant)`
 - `replace_remove_row(dataframe, column)`
 - `replace_remove_column(dataframe, column)`
-- `replace_forward_backward(dataframe, column)` // fill missing value with previous/next value
+- `replace_forward_backward(dataframe, column)`
 
 ### Outlier Handler
 - `identify_outliers_iqr(data, threshold=1.5)`
 - `handle_outliers_iqr(data, threshold=1.5, replacement=None)` //replacement: Value to replace outliers with (e.g., median, mean) or None to remove outliers
 
 
 ### Scaler
@@ -68,9 +61,7 @@
 - `convert_date_to_strings(dataframe column)`
 - `extract_components(dataframe, column)`
 - `reformat_date(dataframe, column)`
 - `calculate_datetime_differences()`
 - `convert_datetime_to_different_timezones`
 - `shift_time()`
 - `handle_irregular_time_intervals()`
-
-
```

### Comparing `cleaner_panda-0.1.4/cleaner_panda/categorical_encoder.py` & `cleaner_panda-0.1.5/cleaner_panda/categorical_encoder.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.4/cleaner_panda/data_type_converter.py` & `cleaner_panda-0.1.5/cleaner_panda/data_type_converter.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.4/cleaner_panda/date_time_handler.py` & `cleaner_panda-0.1.5/cleaner_panda/date_time_handler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.4/cleaner_panda/missing_value_handler.py` & `cleaner_panda-0.1.5/cleaner_panda/missing_value_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,44 +35,44 @@
             return self.replace_forward_backward(dataframe, column)
         else:
             raise ValueError("Invalid strategy")
 
     def replace_mean(self, dataframe: pd.DataFrame, column: Union[int, str]) -> pd.DataFrame:
         if pd.api.types.is_numeric_dtype(dataframe[column]):
             mean_value = dataframe[column].mean()
-            dataframe[column].fillna(mean_value, inplace=True)
+            dataframe[column].fillna(mean_value)
         else:
             raise ValueError(f"Column '{column}' is not numeric. Skipping mean replacement...")
         
         return dataframe
 
     def replace_median(self, dataframe: pd.DataFrame, column: Union[int, str]) -> pd.DataFrame:
         if pd.api.types.is_numeric_dtype(dataframe[column]):
             median_value = dataframe[column].median()
-            dataframe[column].fillna(median_value, inplace=True)
+            dataframe[column].fillna(median_value)
         else:
             raise ValueError(f"Column '{column}' is not numeric. Skipping median replacement.")
         return dataframe
 
     def replace_constant(self, dataframe: pd.DataFrame, column: Union[int, str]) -> pd.DataFrame:
         if pd.api.types.is_numeric_dtype(dataframe[column]):
             const_value = self.const_int
         elif pd.api.types.is_string_dtype(dataframe[column]):
             const_value = self.const_str
         elif pd.api.types.is_datetime64_any_dtype(dataframe[column]):
             const_value = self.const_date
         else:
             raise ValueError(f"Unsupported column type for column '{column}'")
         
-        dataframe[column].fillna(const_value, inplace=True)
+        dataframe[column].fillna(const_value)
         return dataframe
 
     def replace_remove_row(self, dataframe: pd.DataFrame, column: Union[int, str]) -> pd.DataFrame:
         return dataframe.dropna(subset=[column])
 
     def replace_remove_column(self, dataframe: pd.DataFrame, column: Union[int, str]) -> pd.DataFrame:
         return dataframe.drop(columns=[column])
 
     def replace_forward_backward(self, dataframe: pd.DataFrame, column: Union[int, str]) -> pd.DataFrame:
-        dataframe[column].fillna(method='ffill', inplace=True)
-        dataframe[column].fillna(method='bfill', inplace=True)
+        dataframe[column].fillna(method='ffill')
+        dataframe[column].fillna(method='bfill')
         return dataframe
```

### Comparing `cleaner_panda-0.1.4/cleaner_panda/outlier_handler.py` & `cleaner_panda-0.1.5/cleaner_panda/outlier_handler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.4/cleaner_panda/scaler.py` & `cleaner_panda-0.1.5/cleaner_panda/scaler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.4/cleaner_panda/text_cleaner.py` & `cleaner_panda-0.1.5/cleaner_panda/text_cleaner.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.4/cleaner_panda.egg-info/PKG-INFO` & `cleaner_panda-0.1.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,54 @@
 Metadata-Version: 2.1
-Name: cleaner-panda
-Version: 0.1.4
+Name: cleaner_panda
+Version: 0.1.5
 Summary: A package for handling various data preprocessing tasks
 Home-page: https://github.com/EmirhanSyl/cleaner-panda
+Download-URL: https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.5.tar.gz
 Author: asimtarik & emirs
 Author-email: support@cleanpanda.com
-License: UNKNOWN
-Download-URL: https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.4.tar.gz
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: scikit-learn
+Requires-Dist: nltk
+Requires-Dist: category_encoders
+Requires-Dist: scipy
+Requires-Dist: bs4
+Requires-Dist: contractions
 
 # Cleaner Panda
  Programming For Data Engineering course final project
- https://chat.openai.com/share/87c82e00-50af-446b-ac63-e82d9d35021a
+
+![logo.jpg](logo.jpg)
+
+ https://pypi.org/project/cleaner-panda/
+
+ ## Installation
+ `pip install cleaner-panda`
+
+
+## Modules
+
 
 ### Missing Value Handler
 - `strategy enum {MEAN, MEDIAN, CONSTANT, REMOVE_ROW, REMOVE_COLUMN, FORWARD_BACKWARD}`
 - `cont_int = 0, const_str =”none”, const_date=01.01.2024…`
-- `replace_missing_values(dataFrame, strategy=”strategy.MEAN”, column=0)` -> Replaces missing values on the “column” parameter according to the selected strategy. The “column” can be an index or column name as str.
+- `replace_missing_values(dataFrame, strategy=”strategy.MEAN”, column=0)`
 - `replace_mean(dataframe, column)`
 - `replace_median(dataframe, column)`
 - `replace_constant(dataframe, column, constant)`
 - `replace_remove_row(dataframe, column)`
 - `replace_remove_column(dataframe, column)`
-- `replace_forward_backward(dataframe, column)` // fill missing value with previous/next value
+- `replace_forward_backward(dataframe, column)`
 
 ### Outlier Handler
 - `identify_outliers_iqr(data, threshold=1.5)`
 - `handle_outliers_iqr(data, threshold=1.5, replacement=None)` //replacement: Value to replace outliers with (e.g., median, mean) or None to remove outliers
 
 
 ### Scaler
@@ -68,9 +84,7 @@
 - `convert_date_to_strings(dataframe column)`
 - `extract_components(dataframe, column)`
 - `reformat_date(dataframe, column)`
 - `calculate_datetime_differences()`
 - `convert_datetime_to_different_timezones`
 - `shift_time()`
 - `handle_irregular_time_intervals()`
-
-
```

### Comparing `cleaner_panda-0.1.4/cleaner_panda.egg-info/SOURCES.txt` & `cleaner_panda-0.1.5/cleaner_panda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.4/setup.py` & `cleaner_panda-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 from setuptools import setup, find_packages
 
 setup(
     name='cleaner_panda',
-    version='0.1.4',
+    version='0.1.5',
     description='A package for handling various data preprocessing tasks',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='asimtarik & emirs',
     author_email='support@cleanpanda.com',
     url='https://github.com/EmirhanSyl/cleaner-panda',
-    download_url='https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.4.tar.gz',
+    download_url='https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.5.tar.gz',
     packages=find_packages(),
     install_requires=[
         'pandas',
         'numpy',
         'scikit-learn',
         'nltk',
         'category_encoders',
```

### Comparing `cleaner_panda-0.1.4/tests/test_categorical_encoder.py` & `cleaner_panda-0.1.5/tests/test_categorical_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,9 +58,10 @@
         print(df)
         
         result = target_encoding(df, 'color', 'price')
         
         print("\nAfter target encoding:\n")
         print(result)
 
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cleaner_panda-0.1.4/tests/test_data_type_converter.py` & `cleaner_panda-0.1.5/tests/test_data_type_converter.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.4/tests/test_date_time_handler.py` & `cleaner_panda-0.1.5/tests/test_date_time_handler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.4/tests/test_missing_value_handler.py` & `cleaner_panda-0.1.5/tests/test_missing_value_handler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.4/tests/test_outlier_handler.py` & `cleaner_panda-0.1.5/tests/test_outlier_handler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.4/tests/test_scaler.py` & `cleaner_panda-0.1.5/tests/test_scaler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.4/tests/test_text_cleaner.py` & `cleaner_panda-0.1.5/tests/test_text_cleaner.py`

 * *Files identical despite different names*

