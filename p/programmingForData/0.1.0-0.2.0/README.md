# Comparing `tmp/programmingForData-0.1.0.tar.gz` & `tmp/programmingForData-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "programmingForData-0.1.0.tar", last modified: Tue May 21 14:16:21 2024, max compression
+gzip compressed data, was "programmingForData-0.2.0.tar", last modified: Thu May 23 10:46:24 2024, max compression
```

## Comparing `programmingForData-0.1.0.tar` & `programmingForData-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 14:16:21.126256 programmingForData-0.1.0/
--rw-rw-rw-   0        0        0     1089 2024-05-21 13:35:45.000000 programmingForData-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4677 2024-05-21 14:16:21.126256 programmingForData-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4128 2024-05-21 13:26:48.000000 programmingForData-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 14:16:21.124873 programmingForData-0.1.0/programmingForData.egg-info/
--rw-rw-rw-   0        0        0     4677 2024-05-21 14:16:21.000000 programmingForData-0.1.0/programmingForData.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-05-21 14:16:21.000000 programmingForData-0.1.0/programmingForData.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 14:16:21.000000 programmingForData-0.1.0/programmingForData.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-05-21 14:16:21.000000 programmingForData-0.1.0/programmingForData.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 14:16:21.000000 programmingForData-0.1.0/programmingForData.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 14:16:21.127267 programmingForData-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      932 2024-05-21 13:30:05.000000 programmingForData-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 10:46:24.299823 programmingForData-0.2.0/
+-rw-rw-rw-   0        0        0     1089 2024-05-21 13:35:45.000000 programmingForData-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4602 2024-05-23 10:46:24.299823 programmingForData-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4053 2024-05-23 10:44:30.000000 programmingForData-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 10:46:24.290390 programmingForData-0.2.0/programmingForData/
+-rw-rw-rw-   0        0        0      339 2024-05-21 13:10:27.000000 programmingForData-0.2.0/programmingForData/BudgetHandler.py
+-rw-rw-rw-   0        0        0      882 2024-05-21 13:06:30.000000 programmingForData-0.2.0/programmingForData/CategoricalEncoder.py
+-rw-rw-rw-   0        0        0      189 2024-05-21 13:08:22.000000 programmingForData-0.2.0/programmingForData/DataFilter.py
+-rw-rw-rw-   0        0        0      376 2024-05-21 13:09:56.000000 programmingForData-0.2.0/programmingForData/DataTypeConverter.py
+-rw-rw-rw-   0        0        0      393 2024-05-21 13:12:16.000000 programmingForData-0.2.0/programmingForData/DateTimeHandler.py
+-rw-rw-rw-   0        0        0      712 2024-05-23 10:24:32.000000 programmingForData-0.2.0/programmingForData/MissingValueHandler.py
+-rw-rw-rw-   0        0        0      860 2024-05-23 10:24:32.000000 programmingForData-0.2.0/programmingForData/OutlierHandler.py
+-rw-rw-rw-   0        0        0      740 2024-05-21 13:14:50.000000 programmingForData-0.2.0/programmingForData/Scaler.py
+-rw-rw-rw-   0        0        0     5473 2024-05-23 10:25:13.000000 programmingForData-0.2.0/programmingForData/Test.py
+-rw-rw-rw-   0        0        0     1312 2024-05-23 10:24:32.000000 programmingForData-0.2.0/programmingForData/Visualizer.py
+-rw-rw-rw-   0        0        0      608 2024-05-23 10:46:08.000000 programmingForData-0.2.0/programmingForData/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 10:46:24.295649 programmingForData-0.2.0/programmingForData.egg-info/
+-rw-rw-rw-   0        0        0     4602 2024-05-23 10:46:24.000000 programmingForData-0.2.0/programmingForData.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      622 2024-05-23 10:46:24.000000 programmingForData-0.2.0/programmingForData.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 10:46:24.000000 programmingForData-0.2.0/programmingForData.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-05-23 10:46:24.000000 programmingForData-0.2.0/programmingForData.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-23 10:46:24.000000 programmingForData-0.2.0/programmingForData.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 10:46:24.300997 programmingForData-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      932 2024-05-23 09:53:56.000000 programmingForData-0.2.0/setup.py
```

### Comparing `programmingForData-0.1.0/LICENSE` & `programmingForData-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `programmingForData-0.1.0/PKG-INFO` & `programmingForData-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: programmingForData
-Version: 0.1.0
+Version: 0.2.0
 Summary: A comprehensive library for data preprocessing tasks
 Home-page: https://github.com/beyzasevigen/programmingForData
 Author: Beyza Nur Sevigen, Meryem Kilic
 Author-email: beyzanur.sevigen@stu.fsm.edu.tr, meryem.kilic@stu.fsm.edu.tr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,24 +14,24 @@
 
 # Data Preprocessing Library
 
 A comprehensive library for data preprocessing tasks, including data cleaning, transformation, and visualization.
 
 ## Installation
 
-To install the library, use pip:
+To install the updated library, use pip:
 
 
-`pip install data_preprocessing_library`
+`pip install programmingForData==0.2.0`
 
 ### Usage
 #### Outlier Handling
 ```
 import pandas as pd
-from data_preprocessing_library.outlier_handler import OutlierHandler
+from programmingForData.OutlierHandler import OutlierHandler
 
 data = pd.DataFrame({'A': [1, 2, 3, 4, 100]})
 outlier_handler = OutlierHandler()
 
 # Remove outliers using IQR method
 cleaned_data = outlier_handler.iqr_outliers(data, 'A')
 print(cleaned_data)
@@ -41,15 +41,15 @@
 print(data)
 ```
 
 
 #### Scaling
 ```
 import pandas as pd
-from data_preprocessing_library.scaler import Scaler
+from programmingForData.Scaler import Scaler
 
 data = pd.DataFrame({'A': [1, 2, 3, 4, 5]})
 scaler = Scaler()
 
 # Min-Max scaling
 scaled_data = scaler.min_max_scale(data)
 print(scaled_data)
@@ -57,15 +57,15 @@
 # Standard scaling
 standard_scaled_data = scaler.standard_scale(data)
 print(standard_scaled_data)
 ```
 #### Handling Missing Values
 ```
 import pandas as pd
-from data_preprocessing_library.missing_value_handler import MissingValueHandler
+from programmingForData.MissingValueHandler import MissingValueHandler
 
 data = pd.DataFrame({'A': [1, 2, None, 4, 5]})
 missing_value_handler = MissingValueHandler()
 
 # Fill missing values with mean
 data = missing_value_handler.fill_mean(data, ['A'])
 print(data)
@@ -73,15 +73,15 @@
 # Drop rows with missing values
 data = missing_value_handler.drop_missing(data)
 print(data)
 ```
 #### Visualization
 ```
 import pandas as pd
-from data_preprocessing_library.visualizer import Visualizer
+from programmingForData.Visualizer import Visualizer
 
 data = pd.DataFrame({'A': [1, 2, 3, 4, 5], 'B': [5, 4, 3, 2, 1]})
 visualizer = Visualizer()
 
 # Plot histogram
 visualizer.plot_histogram(data, 'A')
 
@@ -93,15 +93,15 @@
 
 # Plot correlation matrix
 visualizer.plot_correlation_matrix(data)
 ```
 #### Filtering Data
 ```
 import pandas as pd
-from data_preprocessing_library.data_filter import DataFilter
+from programmingForData.DataFilter import DataFilter
 
 data = pd.DataFrame({'A': [1, 2, 3, 4, 5], 'B': [5, 4, 3, 2, 1]})
 data_filter = DataFilter()
 
 # Filter data by condition
 filtered_data = data_filter.filter_by_condition(data, 'A > 2')
 print(filtered_data)
@@ -109,15 +109,15 @@
 # Filter specific columns
 filtered_columns = data_filter.filter_by_columns(data, ['A'])
 print(filtered_columns)
 ```
 #### Encoding Categorical Data
 ```
 import pandas as pd
-from data_preprocessing_library.categorical_encoder import CategoricalEncoder
+from programmingForData.CategoricalEncoder import CategoricalEncoder
 
 data = pd.DataFrame({'Category': ['A', 'B', 'A', 'C']})
 encoder = CategoricalEncoder()
 
 # One-hot encoding
 one_hot_encoded_data = encoder.one_hot_encode(data, 'Category')
 print(one_hot_encoded_data)
@@ -125,27 +125,27 @@
 # Label encoding
 label_encoded_data = encoder.label_encode(data, 'Category')
 print(label_encoded_data)
 ```
 #### Budget Categorization
 ```
 import pandas as pd
-from data_preprocessing_library.budget_handler import BudgetHandler
+from programmingForData.BudgetHandler import BudgetHandler
 
 data = pd.DataFrame({'Budget': [500000, 20000000, 300000000]})
 budget_handler = BudgetHandler()
 
 # Categorize budget
 categorized_data = budget_handler.categorize_budget(data, 'Budget')
 print(categorized_data)
 ```
 #### Data Type Conversion
 ```
 import pandas as pd
-from data_preprocessing_library.data_type_converter import DataTypeConverter
+from programmingForData.DataTypeConverter import DataTypeConverter
 
 data = pd.DataFrame({'A': ['1', '2', '3'], 'B': [1, 2, 3]})
 converter = DataTypeConverter()
 
 # Convert to numeric
 numeric_data = converter.convert_to_numeric(data, ['A'])
 print(numeric_data)
@@ -153,15 +153,15 @@
 # Convert to categorical
 categorical_data = converter.convert_to_categorical(data, ['B'])
 print(categorical_data)
 ```
 #### Date and Time Handling
 ```
 import pandas as pd
-from data_preprocessing_library.date_time_handler import DateTimeHandler
+from programmingForData.DateTimeHandler import DateTimeHandler
 
 data = pd.DataFrame({'Date': ['01/01/2020', '02/01/2020', '03/01/2020']})
 date_time_handler = DateTimeHandler()
 
 # Convert to datetime
 datetime_data = date_time_handler.convert_to_datetime(data, 'Date')
 print(datetime_data)
```

### Comparing `programmingForData-0.1.0/README.md` & `programmingForData-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Data Preprocessing Library
 
 A comprehensive library for data preprocessing tasks, including data cleaning, transformation, and visualization.
 
 ## Installation
 
-To install the library, use pip:
+To install the updated library, use pip:
 
 
-`pip install data_preprocessing_library`
+`pip install programmingForData==0.2.0`
 
 ### Usage
 #### Outlier Handling
 ```
 import pandas as pd
-from data_preprocessing_library.outlier_handler import OutlierHandler
+from programmingForData.OutlierHandler import OutlierHandler
 
 data = pd.DataFrame({'A': [1, 2, 3, 4, 100]})
 outlier_handler = OutlierHandler()
 
 # Remove outliers using IQR method
 cleaned_data = outlier_handler.iqr_outliers(data, 'A')
 print(cleaned_data)
@@ -27,15 +27,15 @@
 print(data)
 ```
 
 
 #### Scaling
 ```
 import pandas as pd
-from data_preprocessing_library.scaler import Scaler
+from programmingForData.Scaler import Scaler
 
 data = pd.DataFrame({'A': [1, 2, 3, 4, 5]})
 scaler = Scaler()
 
 # Min-Max scaling
 scaled_data = scaler.min_max_scale(data)
 print(scaled_data)
@@ -43,15 +43,15 @@
 # Standard scaling
 standard_scaled_data = scaler.standard_scale(data)
 print(standard_scaled_data)
 ```
 #### Handling Missing Values
 ```
 import pandas as pd
-from data_preprocessing_library.missing_value_handler import MissingValueHandler
+from programmingForData.MissingValueHandler import MissingValueHandler
 
 data = pd.DataFrame({'A': [1, 2, None, 4, 5]})
 missing_value_handler = MissingValueHandler()
 
 # Fill missing values with mean
 data = missing_value_handler.fill_mean(data, ['A'])
 print(data)
@@ -59,15 +59,15 @@
 # Drop rows with missing values
 data = missing_value_handler.drop_missing(data)
 print(data)
 ```
 #### Visualization
 ```
 import pandas as pd
-from data_preprocessing_library.visualizer import Visualizer
+from programmingForData.Visualizer import Visualizer
 
 data = pd.DataFrame({'A': [1, 2, 3, 4, 5], 'B': [5, 4, 3, 2, 1]})
 visualizer = Visualizer()
 
 # Plot histogram
 visualizer.plot_histogram(data, 'A')
 
@@ -79,15 +79,15 @@
 
 # Plot correlation matrix
 visualizer.plot_correlation_matrix(data)
 ```
 #### Filtering Data
 ```
 import pandas as pd
-from data_preprocessing_library.data_filter import DataFilter
+from programmingForData.DataFilter import DataFilter
 
 data = pd.DataFrame({'A': [1, 2, 3, 4, 5], 'B': [5, 4, 3, 2, 1]})
 data_filter = DataFilter()
 
 # Filter data by condition
 filtered_data = data_filter.filter_by_condition(data, 'A > 2')
 print(filtered_data)
@@ -95,15 +95,15 @@
 # Filter specific columns
 filtered_columns = data_filter.filter_by_columns(data, ['A'])
 print(filtered_columns)
 ```
 #### Encoding Categorical Data
 ```
 import pandas as pd
-from data_preprocessing_library.categorical_encoder import CategoricalEncoder
+from programmingForData.CategoricalEncoder import CategoricalEncoder
 
 data = pd.DataFrame({'Category': ['A', 'B', 'A', 'C']})
 encoder = CategoricalEncoder()
 
 # One-hot encoding
 one_hot_encoded_data = encoder.one_hot_encode(data, 'Category')
 print(one_hot_encoded_data)
@@ -111,27 +111,27 @@
 # Label encoding
 label_encoded_data = encoder.label_encode(data, 'Category')
 print(label_encoded_data)
 ```
 #### Budget Categorization
 ```
 import pandas as pd
-from data_preprocessing_library.budget_handler import BudgetHandler
+from programmingForData.BudgetHandler import BudgetHandler
 
 data = pd.DataFrame({'Budget': [500000, 20000000, 300000000]})
 budget_handler = BudgetHandler()
 
 # Categorize budget
 categorized_data = budget_handler.categorize_budget(data, 'Budget')
 print(categorized_data)
 ```
 #### Data Type Conversion
 ```
 import pandas as pd
-from data_preprocessing_library.data_type_converter import DataTypeConverter
+from programmingForData.DataTypeConverter import DataTypeConverter
 
 data = pd.DataFrame({'A': ['1', '2', '3'], 'B': [1, 2, 3]})
 converter = DataTypeConverter()
 
 # Convert to numeric
 numeric_data = converter.convert_to_numeric(data, ['A'])
 print(numeric_data)
@@ -139,15 +139,15 @@
 # Convert to categorical
 categorical_data = converter.convert_to_categorical(data, ['B'])
 print(categorical_data)
 ```
 #### Date and Time Handling
 ```
 import pandas as pd
-from data_preprocessing_library.date_time_handler import DateTimeHandler
+from programmingForData.DateTimeHandler import DateTimeHandler
 
 data = pd.DataFrame({'Date': ['01/01/2020', '02/01/2020', '03/01/2020']})
 date_time_handler = DateTimeHandler()
 
 # Convert to datetime
 datetime_data = date_time_handler.convert_to_datetime(data, 'Date')
 print(datetime_data)
```

### Comparing `programmingForData-0.1.0/programmingForData.egg-info/PKG-INFO` & `programmingForData-0.2.0/programmingForData.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: programmingForData
-Version: 0.1.0
+Version: 0.2.0
 Summary: A comprehensive library for data preprocessing tasks
 Home-page: https://github.com/beyzasevigen/programmingForData
 Author: Beyza Nur Sevigen, Meryem Kilic
 Author-email: beyzanur.sevigen@stu.fsm.edu.tr, meryem.kilic@stu.fsm.edu.tr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,24 +14,24 @@
 
 # Data Preprocessing Library
 
 A comprehensive library for data preprocessing tasks, including data cleaning, transformation, and visualization.
 
 ## Installation
 
-To install the library, use pip:
+To install the updated library, use pip:
 
 
-`pip install data_preprocessing_library`
+`pip install programmingForData==0.2.0`
 
 ### Usage
 #### Outlier Handling
 ```
 import pandas as pd
-from data_preprocessing_library.outlier_handler import OutlierHandler
+from programmingForData.OutlierHandler import OutlierHandler
 
 data = pd.DataFrame({'A': [1, 2, 3, 4, 100]})
 outlier_handler = OutlierHandler()
 
 # Remove outliers using IQR method
 cleaned_data = outlier_handler.iqr_outliers(data, 'A')
 print(cleaned_data)
@@ -41,15 +41,15 @@
 print(data)
 ```
 
 
 #### Scaling
 ```
 import pandas as pd
-from data_preprocessing_library.scaler import Scaler
+from programmingForData.Scaler import Scaler
 
 data = pd.DataFrame({'A': [1, 2, 3, 4, 5]})
 scaler = Scaler()
 
 # Min-Max scaling
 scaled_data = scaler.min_max_scale(data)
 print(scaled_data)
@@ -57,15 +57,15 @@
 # Standard scaling
 standard_scaled_data = scaler.standard_scale(data)
 print(standard_scaled_data)
 ```
 #### Handling Missing Values
 ```
 import pandas as pd
-from data_preprocessing_library.missing_value_handler import MissingValueHandler
+from programmingForData.MissingValueHandler import MissingValueHandler
 
 data = pd.DataFrame({'A': [1, 2, None, 4, 5]})
 missing_value_handler = MissingValueHandler()
 
 # Fill missing values with mean
 data = missing_value_handler.fill_mean(data, ['A'])
 print(data)
@@ -73,15 +73,15 @@
 # Drop rows with missing values
 data = missing_value_handler.drop_missing(data)
 print(data)
 ```
 #### Visualization
 ```
 import pandas as pd
-from data_preprocessing_library.visualizer import Visualizer
+from programmingForData.Visualizer import Visualizer
 
 data = pd.DataFrame({'A': [1, 2, 3, 4, 5], 'B': [5, 4, 3, 2, 1]})
 visualizer = Visualizer()
 
 # Plot histogram
 visualizer.plot_histogram(data, 'A')
 
@@ -93,15 +93,15 @@
 
 # Plot correlation matrix
 visualizer.plot_correlation_matrix(data)
 ```
 #### Filtering Data
 ```
 import pandas as pd
-from data_preprocessing_library.data_filter import DataFilter
+from programmingForData.DataFilter import DataFilter
 
 data = pd.DataFrame({'A': [1, 2, 3, 4, 5], 'B': [5, 4, 3, 2, 1]})
 data_filter = DataFilter()
 
 # Filter data by condition
 filtered_data = data_filter.filter_by_condition(data, 'A > 2')
 print(filtered_data)
@@ -109,15 +109,15 @@
 # Filter specific columns
 filtered_columns = data_filter.filter_by_columns(data, ['A'])
 print(filtered_columns)
 ```
 #### Encoding Categorical Data
 ```
 import pandas as pd
-from data_preprocessing_library.categorical_encoder import CategoricalEncoder
+from programmingForData.CategoricalEncoder import CategoricalEncoder
 
 data = pd.DataFrame({'Category': ['A', 'B', 'A', 'C']})
 encoder = CategoricalEncoder()
 
 # One-hot encoding
 one_hot_encoded_data = encoder.one_hot_encode(data, 'Category')
 print(one_hot_encoded_data)
@@ -125,27 +125,27 @@
 # Label encoding
 label_encoded_data = encoder.label_encode(data, 'Category')
 print(label_encoded_data)
 ```
 #### Budget Categorization
 ```
 import pandas as pd
-from data_preprocessing_library.budget_handler import BudgetHandler
+from programmingForData.BudgetHandler import BudgetHandler
 
 data = pd.DataFrame({'Budget': [500000, 20000000, 300000000]})
 budget_handler = BudgetHandler()
 
 # Categorize budget
 categorized_data = budget_handler.categorize_budget(data, 'Budget')
 print(categorized_data)
 ```
 #### Data Type Conversion
 ```
 import pandas as pd
-from data_preprocessing_library.data_type_converter import DataTypeConverter
+from programmingForData.DataTypeConverter import DataTypeConverter
 
 data = pd.DataFrame({'A': ['1', '2', '3'], 'B': [1, 2, 3]})
 converter = DataTypeConverter()
 
 # Convert to numeric
 numeric_data = converter.convert_to_numeric(data, ['A'])
 print(numeric_data)
@@ -153,15 +153,15 @@
 # Convert to categorical
 categorical_data = converter.convert_to_categorical(data, ['B'])
 print(categorical_data)
 ```
 #### Date and Time Handling
 ```
 import pandas as pd
-from data_preprocessing_library.date_time_handler import DateTimeHandler
+from programmingForData.DateTimeHandler import DateTimeHandler
 
 data = pd.DataFrame({'Date': ['01/01/2020', '02/01/2020', '03/01/2020']})
 date_time_handler = DateTimeHandler()
 
 # Convert to datetime
 datetime_data = date_time_handler.convert_to_datetime(data, 'Date')
 print(datetime_data)
```

### Comparing `programmingForData-0.1.0/setup.py` & `programmingForData-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='programmingForData',
-    version='0.1.0',
+    version='0.2.0',
     author='Beyza Nur Sevigen, Meryem Kilic',
     author_email='beyzanur.sevigen@stu.fsm.edu.tr, meryem.kilic@stu.fsm.edu.tr',
     description='A comprehensive library for data preprocessing tasks',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/beyzasevigen/programmingForData',
     packages=find_packages(),
```

