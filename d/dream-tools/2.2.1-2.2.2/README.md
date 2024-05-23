# Comparing `tmp/dream-tools-2.2.1.tar.gz` & `tmp/dream-tools-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dream-tools-2.2.1.tar", last modified: Tue May 21 14:04:14 2024, max compression
+gzip compressed data, was "dream-tools-2.2.2.tar", last modified: Thu May 23 13:54:38 2024, max compression
```

## Comparing `dream-tools-2.2.1.tar` & `dream-tools-2.2.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 14:04:14.003780 dream-tools-2.2.1/
--rw-rw-rw-   0        0        0     1093 2020-08-12 11:00:01.000000 dream-tools-2.2.1/LICENSE
--rw-rw-rw-   0        0        0     1454 2024-05-21 14:04:14.000599 dream-tools-2.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      883 2024-05-21 11:37:08.000000 dream-tools-2.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 14:04:13.998193 dream-tools-2.2.1/dream_tools.egg-info/
--rw-rw-rw-   0        0        0     1454 2024-05-21 14:04:13.000000 dream-tools-2.2.1/dream_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1389 2024-05-21 14:04:13.000000 dream-tools-2.2.1/dream_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 14:04:13.000000 dream-tools-2.2.1/dream_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-21 14:04:13.000000 dream-tools-2.2.1/dream_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-21 14:04:13.000000 dream-tools-2.2.1/dream_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-21 14:04:13.923646 dream-tools-2.2.1/dreamtools/
--rw-rw-rw-   0        0        0      729 2024-05-21 13:46:27.000000 dream-tools-2.2.1/dreamtools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:04:13.943218 dream-tools-2.2.1/dreamtools/gamY/
--rw-rw-rw-   0        0        0       19 2024-05-21 09:13:24.000000 dream-tools-2.2.1/dreamtools/gamY/__init__.py
--rw-rw-rw-   0        0        0     3825 2024-05-21 13:53:12.000000 dream-tools-2.2.1/dreamtools/gamY/classes.py
--rw-rw-rw-   0        0        0     4423 2022-12-13 11:41:07.000000 dream-tools-2.2.1/dreamtools/gamY/excel_endo_exo.py
--rw-rw-rw-   0        0        0     2488 2024-05-21 13:53:12.000000 dream-tools-2.2.1/dreamtools/gamY/extract_equations.py
--rw-rw-rw-   0        0        0     1060 2024-05-21 13:53:12.000000 dream-tools-2.2.1/dreamtools/gamY/extract_variables.py
--rw-rw-rw-   0        0        0    54033 2024-05-21 13:59:23.000000 dream-tools-2.2.1/dreamtools/gamY/gamY.py
--rw-rw-rw-   0        0        0     4288 2024-05-21 13:53:12.000000 dream-tools-2.2.1/dreamtools/gamY/gdx_to_excel.py
--rw-rw-rw-   0        0        0     1541 2024-05-21 13:53:12.000000 dream-tools-2.2.1/dreamtools/gamY/gekko_endo_exo.py
--rw-rw-rw-   0        0        0     4996 2024-05-21 13:53:12.000000 dream-tools-2.2.1/dreamtools/gamY/patterns.py
--rw-rw-rw-   0        0        0     1135 2024-05-21 13:53:12.000000 dream-tools-2.2.1/dreamtools/gamY/rename_set.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:04:13.955653 dream-tools-2.2.1/dreamtools/gams_excel/
--rw-rw-rw-   0        0        0       25 2020-01-31 12:41:21.000000 dream-tools-2.2.1/dreamtools/gams_excel/__init__.py
--rw-rw-rw-   0        0        0     3138 2024-04-05 09:32:29.000000 dream-tools-2.2.1/dreamtools/gams_excel/excel_endo_exo.py
--rw-rw-rw-   0        0        0     2666 2020-10-09 09:58:26.000000 dream-tools-2.2.1/dreamtools/gams_excel/gams_excel.py
--rw-rw-rw-   0        0        0     4288 2024-05-17 10:42:49.000000 dream-tools-2.2.1/dreamtools/gams_excel/gdx_to_excel.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:04:13.970551 dream-tools-2.2.1/dreamtools/gams_pandas/
--rw-rw-rw-   0        0        0       89 2023-01-13 09:23:38.000000 dream-tools-2.2.1/dreamtools/gams_pandas/__init__.py
--rw-rw-rw-   0        0        0    17187 2024-04-05 09:32:21.000000 dream-tools-2.2.1/dreamtools/gams_pandas/gams_pandas.py
--rw-rw-rw-   0        0        0     1481 2023-01-13 09:23:38.000000 dream-tools-2.2.1/dreamtools/gams_pandas/gdx.py
--rw-rw-rw-   0        0        0    11969 2023-10-26 19:08:17.000000 dream-tools-2.2.1/dreamtools/gams_pandas/test_gams_pandas.py
--rw-rw-rw-   0        0        0     3321 2023-01-13 09:23:38.000000 dream-tools-2.2.1/dreamtools/gams_pandas/utility.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:04:13.995533 dream-tools-2.2.1/dreamtools/multiindex_plotly/
--rw-rw-rw-   0        0        0      385 2023-03-01 08:59:38.000000 dream-tools-2.2.1/dreamtools/multiindex_plotly/__init__.py
--rw-rw-rw-   0        0        0     2854 2023-01-13 09:23:38.000000 dream-tools-2.2.1/dreamtools/multiindex_plotly/age_plot.py
--rw-rw-rw-   0        0        0     2084 2023-02-24 13:26:37.000000 dream-tools-2.2.1/dreamtools/multiindex_plotly/dream_plotly_template.py
--rw-rw-rw-   0        0        0    22704 2023-01-13 09:23:38.000000 dream-tools-2.2.1/dreamtools/multiindex_plotly/dream_settings.py
--rw-rw-rw-   0        0        0      891 2023-01-13 09:23:38.000000 dream-tools-2.2.1/dreamtools/multiindex_plotly/makro_settings.py
--rw-rw-rw-   0        0        0        3 2023-01-13 09:23:38.000000 dream-tools-2.2.1/dreamtools/multiindex_plotly/plotly_util.py
--rw-rw-rw-   0        0        0     4445 2023-09-14 08:18:26.000000 dream-tools-2.2.1/dreamtools/multiindex_plotly/reporting.py
--rw-rw-rw-   0        0        0     7201 2023-01-13 09:23:38.000000 dream-tools-2.2.1/dreamtools/multiindex_plotly/scratch.py
--rw-rw-rw-   0        0        0     1897 2023-03-01 10:04:19.000000 dream-tools-2.2.1/dreamtools/multiindex_plotly/test_plot.py
--rw-rw-rw-   0        0        0     2330 2023-01-25 09:50:54.000000 dream-tools-2.2.1/dreamtools/multiindex_plotly/test_timeseries_analysis.py
--rw-rw-rw-   0        0        0    10640 2023-03-01 10:03:09.000000 dream-tools-2.2.1/dreamtools/multiindex_plotly/timeseries_analysis.py
--rw-rw-rw-   0        0        0      841 2024-05-21 10:52:06.000000 dream-tools-2.2.1/dreamtools/utils.py
--rw-rw-rw-   0        0        0       42 2024-05-21 14:04:14.004487 dream-tools-2.2.1/setup.cfg
--rw-rw-rw-   0        0        0      843 2024-05-21 11:34:28.000000 dream-tools-2.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:54:38.344344 dream-tools-2.2.2/
+-rw-rw-rw-   0        0        0     1093 2020-08-12 11:00:01.000000 dream-tools-2.2.2/LICENSE
+-rw-rw-rw-   0        0        0     1454 2024-05-23 13:54:38.342344 dream-tools-2.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      883 2024-05-21 11:37:08.000000 dream-tools-2.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 13:54:38.341344 dream-tools-2.2.2/dream_tools.egg-info/
+-rw-rw-rw-   0        0        0     1454 2024-05-23 13:54:38.000000 dream-tools-2.2.2/dream_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1389 2024-05-23 13:54:38.000000 dream-tools-2.2.2/dream_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 13:54:38.000000 dream-tools-2.2.2/dream_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-23 13:54:38.000000 dream-tools-2.2.2/dream_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-23 13:54:38.000000 dream-tools-2.2.2/dream_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 13:54:38.303799 dream-tools-2.2.2/dreamtools/
+-rw-rw-rw-   0        0        0      729 2024-05-23 13:47:30.000000 dream-tools-2.2.2/dreamtools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:54:38.316343 dream-tools-2.2.2/dreamtools/gamY/
+-rw-rw-rw-   0        0        0       19 2024-05-21 09:13:24.000000 dream-tools-2.2.2/dreamtools/gamY/__init__.py
+-rw-rw-rw-   0        0        0     3825 2024-05-21 13:53:12.000000 dream-tools-2.2.2/dreamtools/gamY/classes.py
+-rw-rw-rw-   0        0        0     4423 2022-12-13 11:41:07.000000 dream-tools-2.2.2/dreamtools/gamY/excel_endo_exo.py
+-rw-rw-rw-   0        0        0     2488 2024-05-21 13:53:12.000000 dream-tools-2.2.2/dreamtools/gamY/extract_equations.py
+-rw-rw-rw-   0        0        0     1060 2024-05-21 13:53:12.000000 dream-tools-2.2.2/dreamtools/gamY/extract_variables.py
+-rw-rw-rw-   0        0        0    54073 2024-05-23 13:47:18.000000 dream-tools-2.2.2/dreamtools/gamY/gamY.py
+-rw-rw-rw-   0        0        0     4288 2024-05-21 13:53:12.000000 dream-tools-2.2.2/dreamtools/gamY/gdx_to_excel.py
+-rw-rw-rw-   0        0        0     1541 2024-05-21 13:53:12.000000 dream-tools-2.2.2/dreamtools/gamY/gekko_endo_exo.py
+-rw-rw-rw-   0        0        0     4996 2024-05-21 13:53:12.000000 dream-tools-2.2.2/dreamtools/gamY/patterns.py
+-rw-rw-rw-   0        0        0     1135 2024-05-21 13:53:12.000000 dream-tools-2.2.2/dreamtools/gamY/rename_set.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:54:38.321344 dream-tools-2.2.2/dreamtools/gams_excel/
+-rw-rw-rw-   0        0        0       25 2020-01-31 12:41:21.000000 dream-tools-2.2.2/dreamtools/gams_excel/__init__.py
+-rw-rw-rw-   0        0        0     3138 2024-04-05 09:32:29.000000 dream-tools-2.2.2/dreamtools/gams_excel/excel_endo_exo.py
+-rw-rw-rw-   0        0        0     2666 2020-10-09 09:58:26.000000 dream-tools-2.2.2/dreamtools/gams_excel/gams_excel.py
+-rw-rw-rw-   0        0        0     4288 2024-05-17 10:42:49.000000 dream-tools-2.2.2/dreamtools/gams_excel/gdx_to_excel.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:54:38.327344 dream-tools-2.2.2/dreamtools/gams_pandas/
+-rw-rw-rw-   0        0        0       89 2023-01-13 09:23:38.000000 dream-tools-2.2.2/dreamtools/gams_pandas/__init__.py
+-rw-rw-rw-   0        0        0    17187 2024-04-05 09:32:21.000000 dream-tools-2.2.2/dreamtools/gams_pandas/gams_pandas.py
+-rw-rw-rw-   0        0        0     1481 2023-01-13 09:23:38.000000 dream-tools-2.2.2/dreamtools/gams_pandas/gdx.py
+-rw-rw-rw-   0        0        0    11969 2023-10-26 19:08:17.000000 dream-tools-2.2.2/dreamtools/gams_pandas/test_gams_pandas.py
+-rw-rw-rw-   0        0        0     3321 2023-01-13 09:23:38.000000 dream-tools-2.2.2/dreamtools/gams_pandas/utility.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:54:38.340345 dream-tools-2.2.2/dreamtools/multiindex_plotly/
+-rw-rw-rw-   0        0        0      385 2023-03-01 08:59:38.000000 dream-tools-2.2.2/dreamtools/multiindex_plotly/__init__.py
+-rw-rw-rw-   0        0        0     2854 2023-01-13 09:23:38.000000 dream-tools-2.2.2/dreamtools/multiindex_plotly/age_plot.py
+-rw-rw-rw-   0        0        0     2084 2023-02-24 13:26:37.000000 dream-tools-2.2.2/dreamtools/multiindex_plotly/dream_plotly_template.py
+-rw-rw-rw-   0        0        0    22704 2023-01-13 09:23:38.000000 dream-tools-2.2.2/dreamtools/multiindex_plotly/dream_settings.py
+-rw-rw-rw-   0        0        0      891 2023-01-13 09:23:38.000000 dream-tools-2.2.2/dreamtools/multiindex_plotly/makro_settings.py
+-rw-rw-rw-   0        0        0        3 2023-01-13 09:23:38.000000 dream-tools-2.2.2/dreamtools/multiindex_plotly/plotly_util.py
+-rw-rw-rw-   0        0        0     4445 2023-09-14 08:18:26.000000 dream-tools-2.2.2/dreamtools/multiindex_plotly/reporting.py
+-rw-rw-rw-   0        0        0     7201 2023-01-13 09:23:38.000000 dream-tools-2.2.2/dreamtools/multiindex_plotly/scratch.py
+-rw-rw-rw-   0        0        0     1897 2023-03-01 10:04:19.000000 dream-tools-2.2.2/dreamtools/multiindex_plotly/test_plot.py
+-rw-rw-rw-   0        0        0     2330 2023-01-25 09:50:54.000000 dream-tools-2.2.2/dreamtools/multiindex_plotly/test_timeseries_analysis.py
+-rw-rw-rw-   0        0        0    10640 2023-03-01 10:03:09.000000 dream-tools-2.2.2/dreamtools/multiindex_plotly/timeseries_analysis.py
+-rw-rw-rw-   0        0        0      841 2024-05-21 10:52:06.000000 dream-tools-2.2.2/dreamtools/utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 13:54:38.344344 dream-tools-2.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      843 2024-05-21 11:34:28.000000 dream-tools-2.2.2/setup.py
```

### Comparing `dream-tools-2.2.1/LICENSE` & `dream-tools-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/PKG-INFO` & `dream-tools-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dream-tools
-Version: 2.2.1
+Version: 2.2.2
 Summary: A collection of tools used by the Danish Research Institute for Economic Analysis and Modelling, DREAM (https://dreamgruppen.dk/).
 Home-page: https://github.com/MartinBonde/dream-tools
 Author: Martin Kirk Bonde
 Author-email: martin@bonde.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `dream-tools-2.2.1/README.md` & `dream-tools-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dream_tools.egg-info/PKG-INFO` & `dream-tools-2.2.2/dream_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dream-tools
-Version: 2.2.1
+Version: 2.2.2
 Summary: A collection of tools used by the Danish Research Institute for Economic Analysis and Modelling, DREAM (https://dreamgruppen.dk/).
 Home-page: https://github.com/MartinBonde/dream-tools
 Author: Martin Kirk Bonde
 Author-email: martin@bonde.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `dream-tools-2.2.1/dream_tools.egg-info/SOURCES.txt` & `dream-tools-2.2.2/dream_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/__init__.py` & `dream-tools-2.2.2/dreamtools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .gams_pandas import *
 
-__version__ = "2.2.1"
+__version__ = "2.2.2"
 
 # Global setting controlling the default name of the time index
 X_AXIS_NAME = "t"
 # Default axis position if no level named dt.X_AXIS_NAME is found
 X_AXIS_INDEX = -1 #  (-1 = last index is time)
 
 # Time settings, used for plot and prt functions
```

### Comparing `dream-tools-2.2.1/dreamtools/gamY/classes.py` & `dream-tools-2.2.2/dreamtools/gamY/classes.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/gamY/excel_endo_exo.py` & `dream-tools-2.2.2/dreamtools/gamY/excel_endo_exo.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/gamY/extract_equations.py` & `dream-tools-2.2.2/dreamtools/gamY/extract_equations.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/gamY/extract_variables.py` & `dream-tools-2.2.2/dreamtools/gamY/extract_variables.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/gamY/gamY.py` & `dream-tools-2.2.2/dreamtools/gamY/gamY.py`

 * *Files 0% similar despite different names*

```diff
@@ -1266,18 +1266,18 @@
   return True
 
 
 def find_gams():
     """
     Find GAMS executable
     """
-    gams_path = os.environ.get("GAMS") or os.environ.get("gams") or shutil.which("GAMS") or shutil.which("gams")
+    gams_path = shutil.which("GAMS") or shutil.which("gams") or os.environ.get("GAMS") or os.environ.get("gams")
     
-    if not gams_path:
-      sys.exit("ERROR: gamY could not find GAMS. Set GAMS path as environmental variable with variable name GAMS")
+    if not os.path.isfile(gams_path):
+      sys.exit("ERROR: gamY could not find GAMS. Set path to gams executable as environmental variable with variable name GAMS (or gams)")
     
     return gams_path
 
 
 def run(file_path, r=None, s=None, shell=False, **kwargs):
   """
   Run a GAMS file after precompiling it with optional adjustments.
```

### Comparing `dream-tools-2.2.1/dreamtools/gamY/gdx_to_excel.py` & `dream-tools-2.2.2/dreamtools/gamY/gdx_to_excel.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/gamY/gekko_endo_exo.py` & `dream-tools-2.2.2/dreamtools/gamY/gekko_endo_exo.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/gamY/patterns.py` & `dream-tools-2.2.2/dreamtools/gamY/patterns.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/gamY/rename_set.py` & `dream-tools-2.2.2/dreamtools/gamY/rename_set.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/gams_excel/excel_endo_exo.py` & `dream-tools-2.2.2/dreamtools/gams_excel/excel_endo_exo.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/gams_excel/gams_excel.py` & `dream-tools-2.2.2/dreamtools/gams_excel/gams_excel.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/gams_excel/gdx_to_excel.py` & `dream-tools-2.2.2/dreamtools/gams_excel/gdx_to_excel.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/gams_pandas/gams_pandas.py` & `dream-tools-2.2.2/dreamtools/gams_pandas/gams_pandas.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/gams_pandas/gdx.py` & `dream-tools-2.2.2/dreamtools/gams_pandas/gdx.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/gams_pandas/test_gams_pandas.py` & `dream-tools-2.2.2/dreamtools/gams_pandas/test_gams_pandas.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/gams_pandas/utility.py` & `dream-tools-2.2.2/dreamtools/gams_pandas/utility.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/multiindex_plotly/age_plot.py` & `dream-tools-2.2.2/dreamtools/multiindex_plotly/age_plot.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/multiindex_plotly/dream_plotly_template.py` & `dream-tools-2.2.2/dreamtools/multiindex_plotly/dream_plotly_template.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/multiindex_plotly/dream_settings.py` & `dream-tools-2.2.2/dreamtools/multiindex_plotly/dream_settings.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/multiindex_plotly/makro_settings.py` & `dream-tools-2.2.2/dreamtools/multiindex_plotly/makro_settings.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/multiindex_plotly/reporting.py` & `dream-tools-2.2.2/dreamtools/multiindex_plotly/reporting.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/multiindex_plotly/scratch.py` & `dream-tools-2.2.2/dreamtools/multiindex_plotly/scratch.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/multiindex_plotly/test_plot.py` & `dream-tools-2.2.2/dreamtools/multiindex_plotly/test_plot.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/multiindex_plotly/test_timeseries_analysis.py` & `dream-tools-2.2.2/dreamtools/multiindex_plotly/test_timeseries_analysis.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/multiindex_plotly/timeseries_analysis.py` & `dream-tools-2.2.2/dreamtools/multiindex_plotly/timeseries_analysis.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/dreamtools/utils.py` & `dream-tools-2.2.2/dreamtools/utils.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.2.1/setup.py` & `dream-tools-2.2.2/setup.py`

 * *Files identical despite different names*

