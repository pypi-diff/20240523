# Comparing `tmp/plotguy-1.2.7.tar.gz` & `tmp/plotguy-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotguy-1.2.7.tar", last modified: Wed Aug 23 06:12:15 2023, max compression
+gzip compressed data, was "plotguy-1.2.8.tar", last modified: Thu May 23 13:28:24 2024, max compression
```

## Comparing `plotguy-1.2.7.tar` & `plotguy-1.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-08-23 06:12:15.736512 plotguy-1.2.7/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-08-23 06:12:15.736319 plotguy-1.2.7/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.2.7/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-08-23 06:12:15.735214 plotguy-1.2.7/plotguy/
--rw-r--r--   0 cmw        (501) staff       (20)    26486 2023-08-18 06:36:49.000000 plotguy-1.2.7/plotguy/__init__.py
--rw-r--r--   0 cmw        (501) staff       (20)    16885 2023-06-09 02:59:56.000000 plotguy-1.2.7/plotguy/aggregate.py
--rw-r--r--   0 cmw        (501) staff       (20)    67716 2023-08-23 01:23:18.000000 plotguy-1.2.7/plotguy/components.py
--rw-r--r--   0 cmw        (501) staff       (20)    39678 2023-08-23 06:04:54.000000 plotguy-1.2.7/plotguy/equity_curves.py
--rw-r--r--   0 cmw        (501) staff       (20)    11754 2023-08-18 10:46:13.000000 plotguy-1.2.7/plotguy/signals.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-08-23 06:12:15.736090 plotguy-1.2.7/plotguy.egg-info/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-08-23 06:12:15.000000 plotguy-1.2.7/plotguy.egg-info/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)      279 2023-08-23 06:12:15.000000 plotguy-1.2.7/plotguy.egg-info/SOURCES.txt
--rw-r--r--   0 cmw        (501) staff       (20)        1 2023-08-23 06:12:15.000000 plotguy-1.2.7/plotguy.egg-info/dependency_links.txt
--rw-r--r--   0 cmw        (501) staff       (20)      131 2023-08-23 06:12:15.000000 plotguy-1.2.7/plotguy.egg-info/requires.txt
--rw-r--r--   0 cmw        (501) staff       (20)        8 2023-08-23 06:12:15.000000 plotguy-1.2.7/plotguy.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-08-23 06:12:15.736570 plotguy-1.2.7/setup.cfg
--rw-r--r--   0 cmw        (501) staff       (20)      832 2023-08-23 06:11:53.000000 plotguy-1.2.7/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2024-05-23 13:28:24.797040 plotguy-1.2.8/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2024-05-23 13:28:24.796904 plotguy-1.2.8/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.2.8/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2024-05-23 13:28:24.796030 plotguy-1.2.8/plotguy/
+-rw-r--r--   0 cmw        (501) staff       (20)    26504 2024-05-23 13:26:21.000000 plotguy-1.2.8/plotguy/__init__.py
+-rw-r--r--   0 cmw        (501) staff       (20)    16885 2023-06-09 02:59:56.000000 plotguy-1.2.8/plotguy/aggregate.py
+-rw-r--r--   0 cmw        (501) staff       (20)    67716 2023-08-23 01:23:18.000000 plotguy-1.2.8/plotguy/components.py
+-rw-r--r--   0 cmw        (501) staff       (20)    39678 2023-08-23 06:04:54.000000 plotguy-1.2.8/plotguy/equity_curves.py
+-rw-r--r--   0 cmw        (501) staff       (20)    11754 2023-08-18 10:46:13.000000 plotguy-1.2.8/plotguy/signals.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2024-05-23 13:28:24.796742 plotguy-1.2.8/plotguy.egg-info/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2024-05-23 13:28:21.000000 plotguy-1.2.8/plotguy.egg-info/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)      279 2024-05-23 13:28:21.000000 plotguy-1.2.8/plotguy.egg-info/SOURCES.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        1 2024-05-23 13:28:21.000000 plotguy-1.2.8/plotguy.egg-info/dependency_links.txt
+-rw-r--r--   0 cmw        (501) staff       (20)      140 2024-05-23 13:28:21.000000 plotguy-1.2.8/plotguy.egg-info/requires.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        8 2024-05-23 13:28:21.000000 plotguy-1.2.8/plotguy.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2024-05-23 13:28:24.797091 plotguy-1.2.8/setup.cfg
+-rw-r--r--   0 cmw        (501) staff       (20)      841 2024-05-23 13:26:50.000000 plotguy-1.2.8/setup.py
```

### Comparing `plotguy-1.2.7/plotguy/__init__.py` & `plotguy-1.2.8/plotguy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
     if subchart_settings == {}:  # subchart default setting
         subchart_settings = {
             'histogram_period': [1, 3, 5, 10, 20],
             'subchart_1': ['volume', 'line']
         }
 
     if mode == 'equity_curves':
-        result_df = pd.read_csv('backtest_result.csv', index_col=0)
+        result_df = pd.read_csv('backtest_result.csv', index_col=0, low_memory=False)
         app = equity_curves.Plot(all_para_combination, result_df, subchart_settings, number_of_curves)
 
     if mode == 'aggregate':
         app = aggregate.Aggregate(risk_free_rate)
 
     if mode == 'signal_analysis':
         app = signals.Signals( all_para_combination, generate_filepath, subchart_settings)
```

### Comparing `plotguy-1.2.7/plotguy/aggregate.py` & `plotguy-1.2.8/plotguy/aggregate.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.2.7/plotguy/components.py` & `plotguy-1.2.8/plotguy/components.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.2.7/plotguy/equity_curves.py` & `plotguy-1.2.8/plotguy/equity_curves.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.2.7/plotguy/signals.py` & `plotguy-1.2.8/plotguy/signals.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.2.7/setup.py` & `plotguy-1.2.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="plotguy",
-    version="1.2.7",
+    version="1.2.8",
     author="Plotguy Team",
     author_email="plotguy.info@gmail.com",
     description="Plotguy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[         
         'pandas==1.5.3',  
         'numpy>=1.24.1',  
         'hkfdb>=2.2', 
         'pyarrow',
-        'polars',
+        'polars==0.18.15',
         'lxml',        
         'dash',
         'dash_bootstrap_components',
         'dash_daq',
         'dash_dangerously_set_inner_html',
     ],
     url="https://pypi.org/project/plotguy/",
```

