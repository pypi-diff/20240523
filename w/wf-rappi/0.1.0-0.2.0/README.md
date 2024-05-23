# Comparing `tmp/wf_rappi-0.1.0.tar.gz` & `tmp/wf_rappi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf_rappi-0.1.0.tar", last modified: Mon May 20 22:47:18 2024, max compression
+gzip compressed data, was "wf_rappi-0.2.0.tar", last modified: Thu May 23 03:23:04 2024, max compression
```

## Comparing `wf_rappi-0.1.0.tar` & `wf_rappi-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 22:47:18.200599 wf_rappi-0.1.0/
--rw-rw-rw-   0        0        0     2723 2024-05-20 22:47:18.194165 wf_rappi-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-20 22:47:18.201856 wf_rappi-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1398 2024-05-20 22:37:50.000000 wf_rappi-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-20 22:47:18.122619 wf_rappi-0.1.0/wf_rappi/
--rw-rw-rw-   0        0        0       56 2024-05-20 14:07:52.000000 wf_rappi-0.1.0/wf_rappi/__init__.py
--rw-rw-rw-   0        0        0     4322 2024-05-17 02:48:37.000000 wf_rappi-0.1.0/wf_rappi/data_processing.py
--rw-rw-rw-   0        0        0     1396 2024-04-18 19:54:58.000000 wf_rappi-0.1.0/wf_rappi/dbconn.py
--rw-rw-rw-   0        0        0       70 2024-05-15 21:58:33.000000 wf_rappi-0.1.0/wf_rappi/export.py
--rw-rw-rw-   0        0        0    10931 2024-05-02 14:33:49.000000 wf_rappi-0.1.0/wf_rappi/fetch_data.py
--rw-rw-rw-   0        0        0     2471 2024-05-17 02:56:42.000000 wf_rappi-0.1.0/wf_rappi/main.py
--rw-rw-rw-   0        0        0     1610 2024-05-17 02:48:28.000000 wf_rappi-0.1.0/wf_rappi/modeling.py
--rw-rw-rw-   0        0        0     5612 2024-05-20 20:51:43.000000 wf_rappi-0.1.0/wf_rappi/order_distribution.py
--rw-rw-rw-   0        0        0     2748 2024-04-19 03:22:08.000000 wf_rappi-0.1.0/wf_rappi/wfm_functions.py
-drwxrwxrwx   0        0        0        0 2024-05-20 22:47:18.182608 wf_rappi-0.1.0/wf_rappi.egg-info/
--rw-rw-rw-   0        0        0     2723 2024-05-20 22:47:17.000000 wf_rappi-0.1.0/wf_rappi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2024-05-20 22:47:17.000000 wf_rappi-0.1.0/wf_rappi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 22:47:17.000000 wf_rappi-0.1.0/wf_rappi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-05-20 22:47:17.000000 wf_rappi-0.1.0/wf_rappi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      571 2024-05-20 22:47:17.000000 wf_rappi-0.1.0/wf_rappi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-20 22:47:17.000000 wf_rappi-0.1.0/wf_rappi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 03:23:04.263980 wf_rappi-0.2.0/
+-rw-rw-rw-   0        0        0     2194 2024-05-23 03:23:04.237169 wf_rappi-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-23 03:23:04.285411 wf_rappi-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      933 2024-05-23 03:22:55.000000 wf_rappi-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:23:03.984575 wf_rappi-0.2.0/wf_rappi/
+-rw-rw-rw-   0        0        0       56 2024-05-20 14:07:52.000000 wf_rappi-0.2.0/wf_rappi/__init__.py
+-rw-rw-rw-   0        0        0     6455 2024-05-22 23:36:42.000000 wf_rappi-0.2.0/wf_rappi/data_processing.py
+-rw-rw-rw-   0        0        0     1396 2024-04-18 19:54:58.000000 wf_rappi-0.2.0/wf_rappi/dbconn.py
+-rw-rw-rw-   0        0        0       70 2024-05-15 21:58:33.000000 wf_rappi-0.2.0/wf_rappi/export.py
+-rw-rw-rw-   0        0        0    12003 2024-05-22 13:51:17.000000 wf_rappi-0.2.0/wf_rappi/fetch_data.py
+-rw-rw-rw-   0        0        0     2582 2024-05-22 15:27:04.000000 wf_rappi-0.2.0/wf_rappi/main.py
+-rw-rw-rw-   0        0        0     1610 2024-05-17 02:48:28.000000 wf_rappi-0.2.0/wf_rappi/modeling.py
+-rw-rw-rw-   0        0        0     8092 2024-05-23 03:12:09.000000 wf_rappi-0.2.0/wf_rappi/order_distribution.py
+-rw-rw-rw-   0        0        0     2748 2024-04-19 03:22:08.000000 wf_rappi-0.2.0/wf_rappi/wfm_functions.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:23:04.193941 wf_rappi-0.2.0/wf_rappi.egg-info/
+-rw-rw-rw-   0        0        0     2194 2024-05-23 03:23:02.000000 wf_rappi-0.2.0/wf_rappi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2024-05-23 03:23:03.000000 wf_rappi-0.2.0/wf_rappi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 03:23:02.000000 wf_rappi-0.2.0/wf_rappi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-23 03:23:02.000000 wf_rappi-0.2.0/wf_rappi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      298 2024-05-23 03:23:02.000000 wf_rappi-0.2.0/wf_rappi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-23 03:23:02.000000 wf_rappi-0.2.0/wf_rappi.egg-info/top_level.txt
```

### Comparing `wf_rappi-0.1.0/setup.py` & `wf_rappi-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,33 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="wf_rappi",
-    version="0.1.0",
+    version="0.2.0",
     packages=find_packages(),
     install_requires=[
         'numpy>=1.11.1',
         'pandas>=1.0',
-        'aiohttp==3.9.1',
-        'holidays==0.10.5',
-        'linkify-it-py==2.0.2',
         'matplotlib==3.8.3',
-        'matplotlib-inline==0.1.6',
-        'numpy==1.26.4',
         'openpyxl==3.1.2',
         'packaging==23.2',
-        'pandas==2.1.4',
         'pillow==10.2.0',
-        'pkginfo==1.10.0',
-        'platformdirs==3.11.0',
-        'pluggy==1.3.0',
-        'prison==0.2.1',
-        'prophet==1.1.5',
         'psycopg2==2.9.9',
         'pyarrow==15.0.0',
         'pydantic==2.5.3',
         'pydantic-core==2.14.6',
         'requests==2.31.0',
         'scikit-learn==1.3.2',
-        'scipy==1.12.0',
-        'seaborn==0.13.2',
-        'skforecast==0.11.0',
         'snowflake-connector-python==3.7.1',
         'snowflake-snowpark-python==1.13.0',
         'SQLAlchemy==1.4.51',
-        'tqdm==4.66.2',
-        'twine==5.1.0',
-        'typing-extensions==4.9.0'
+        'twine==5.1.0'
     ],
     entry_points={
         "console_scripts": [
             "wf-rappi = wf_rappi.main:distribute_orders",
         ],
     },
     long_description=description,
```

### Comparing `wf_rappi-0.1.0/wf_rappi/dbconn.py` & `wf_rappi-0.2.0/wf_rappi/dbconn.py`

 * *Files identical despite different names*

### Comparing `wf_rappi-0.1.0/wf_rappi/fetch_data.py` & `wf_rappi-0.2.0/wf_rappi/fetch_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass, field
 from typing import List
 from functools import lru_cache
 import pandas as pd
+import os
 
 
 @dataclass(frozen=True, order=True) # Instances of this class will be immutable and orderable based on their fields
 class Orders:
     service_user_types: List[str] = field(
         default_factory=lambda: ['User', 'RT', 'Rest'])
     segment_types: List[str] = field(
@@ -205,15 +206,15 @@
     # Execute the query with the parameters
     with conn.cursor() as cur:
         cur.execute(query, params)
         result = cur.fetch_pandas_all()
 
     return result
 
-##############3
+##############
 def fetch_special_days(conn, countries=None, region=None, date_range=None, interval=False) -> pd.DataFrame:
     
     """
     Function to fetch specia days from the database
     :param conn: Snowflake connection object
     :param countries: List of countries to filter the data
     :param region: Region to filter the data
@@ -290,7 +291,31 @@
 
     # Execute the query with the parameters
     with conn.cursor() as cur:
         cur.execute(query)
         result = cur.fetch_pandas_all()
 
     return result
+
+import json
+def get_project_settings(import_filepath="settings.json"):
+    """
+    Function to import settings from settings.json
+    :param import_filepath: path to settings.json
+    :return: settings as a dictionary object
+    """
+    if os.path.exists(import_filepath):
+        try:
+            with open(import_filepath, "r") as f:
+                content = f.read().strip()
+                if not content:
+                    raise ImportError(f"Error reading {import_filepath}: File is empty")
+                project_settings = json.loads(content)
+            return project_settings
+        except FileNotFoundError:
+            raise ImportError(f"File not found: {import_filepath}")
+        except json.JSONDecodeError as e:
+            raise ImportError(f"Error decoding JSON from {import_filepath}: {e}")
+        except Exception as e:
+            raise ImportError(f"Unexpected error reading {import_filepath}: {e}")
+    else:
+        raise ImportError(f"settings.json does not exist at provided location: {import_filepath}")
```

### Comparing `wf_rappi-0.1.0/wf_rappi/main.py` & `wf_rappi-0.2.0/wf_rappi/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from data_processing import *
 from modeling import *
 from export import *
 from order_distribution import distribute_orders
 from order_distribution import create_ordenes_financieras, create_curva_ordenes
 
 # Path to the Parquet file containing order data
-# parquet_path = "C:/Users/jonathan.marin/Documents/GitHub/rappi/wfm/libreria/one_year_and_a_half.parquet.gzip"
-date_range=['2024-04-01', '2024-04-10']
-
+# file_path = "C:/Users/jonathan.marin/Documents/GitHub/rappi/wfm/libreria/one_year_and_a_half.parquet.gzip"
+date_range = ['2024-01-01', '2024-04-30']
+service = "SS"
 # Path to the CSV file containing special dates
-csv_path = "C:/Users/jonathan.marin/Documents/GitHub/rappi/wfm/Calendario Rappi - BD_Feriados.csv"
+#file_path_sp = "C:/Users/jonathan.marin/Documents/GitHub/rappi/wfm/Calendario Rappi - BD_Feriados.csv"
 
 # Start date for the dataset
 startdate = "2024-01-01"
 
 # Read and sort order data
 df_ordered = read_and_sort_orders(date_range)
 
 # Preprocess special dates
-special_days = preprocess_special_dates(csv_path)
+special_days = preprocess_special_dates(date_range)
 
 # Filter special dates from the ordered dataframe
 df_filtered = filter_special_dates(df_ordered, special_days)
 
 # Pivot the filtered dataframe to get orders by region and day
-orders = pivot_orders(df_filtered)
+orders = pivot_orders(df_filtered, service=service)
 
 # Set the index of orders dataframe to "FECHA" column
 data = orders.set_index("FECHA")
 
 # Split the data into training and testing sets
 train, test = split_train_test_data(data, startdate)
 
 # Create time series features for training and testing sets
 train = create_features(train)
 test = create_features(test)
 
 # Features and target variable
 FEATURES = ['dayofweek', 'quarter', 'month', 'year', 'dayofyear', 'dayofmonth', 'weekofyear']
-TARGET = "SS"
+TARGET = service
 
 # Extract features and target variable for training and testing sets
 X_train = train[FEATURES]
 y_train = train[TARGET]
 
 X_test = test[FEATURES]
 y_test = test[TARGET]
@@ -55,19 +55,19 @@
 
 # Add predictions to the test dataframe
 test['prediction'] = predictions
 
 # Calculate RMSE score
 score = calculate_rmse(y_test, predictions)
 
-# Select data for April
-abril = test[test.index >= '2024-04-01']
+# Select data for next month
+month_to_predict = test[test.index >= '2024-04-01']
 
 # Create financial orders based on predicted values and average daily weights
-ordenes_financieras = create_ordenes_financieras(df_ordered, abril)
+ordenes_financieras = create_ordenes_financieras(df_ordered, month_to_predict,service=service, ordenes_aprobadas=14000000)
 
 # Create an order curve based on order distribution throughout the week
 curva_ordenes = create_curva_ordenes(df_ordered)
 
 # Distribute financial orders according to the order curve
 df3 = distribute_orders(ordenes_financieras, curva_ordenes)
 print(df3.head())
```

### Comparing `wf_rappi-0.1.0/wf_rappi/modeling.py` & `wf_rappi-0.2.0/wf_rappi/modeling.py`

 * *Files identical despite different names*

### Comparing `wf_rappi-0.1.0/wf_rappi/wfm_functions.py` & `wf_rappi-0.2.0/wf_rappi/wfm_functions.py`

 * *Files identical despite different names*

