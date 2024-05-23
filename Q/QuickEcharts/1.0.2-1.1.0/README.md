# Comparing `tmp/QuickEcharts-1.0.2.tar.gz` & `tmp/quickecharts-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuickEcharts-1.0.2.tar", last modified: Tue Mar 26 20:37:10 2024, max compression
+gzip compressed data, was "QuickEcharts-1.1.0.tar", last modified: Thu May 23 16:22:02 2024, max compression
```

## Comparing `QuickEcharts-1.0.2.tar` & `quickecharts-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 20:37:10.104676 QuickEcharts-1.0.2/
--rw-rw-rw-   0        0        0    31892 2023-06-03 03:56:56.000000 QuickEcharts-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       78 2024-03-22 23:36:21.000000 QuickEcharts-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0    69552 2024-03-26 20:37:10.104176 QuickEcharts-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-26 20:37:10.086176 QuickEcharts-1.0.2/QuickEcharts/
--rw-rw-rw-   0        0        0   338142 2024-03-26 20:36:26.000000 QuickEcharts-1.0.2/QuickEcharts/Charts.py
-drwxrwxrwx   0        0        0        0 2024-03-26 20:37:10.102676 QuickEcharts-1.0.2/QuickEcharts.egg-info/
--rw-rw-rw-   0        0        0    69552 2024-03-26 20:37:10.000000 QuickEcharts-1.0.2/QuickEcharts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-03-26 20:37:10.000000 QuickEcharts-1.0.2/QuickEcharts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 20:37:10.000000 QuickEcharts-1.0.2/QuickEcharts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-03-26 20:37:10.000000 QuickEcharts-1.0.2/QuickEcharts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 20:37:10.000000 QuickEcharts-1.0.2/QuickEcharts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    69065 2024-03-26 20:36:21.000000 QuickEcharts-1.0.2/README.md
--rw-rw-rw-   0        0        0      693 2024-03-26 19:47:36.000000 QuickEcharts-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       19 2024-03-05 17:52:13.000000 QuickEcharts-1.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-03-26 20:37:10.104676 QuickEcharts-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1046 2024-03-26 20:36:31.000000 QuickEcharts-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:22:02.642511 QuickEcharts-1.1.0/
+-rw-rw-rw-   0        0        0    31892 2023-06-03 03:56:56.000000 QuickEcharts-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       78 2024-03-22 23:36:21.000000 QuickEcharts-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    69628 2024-05-23 16:22:02.642009 QuickEcharts-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 16:22:02.623010 QuickEcharts-1.1.0/QuickEcharts/
+-rw-rw-rw-   0        0        0   340583 2024-05-23 16:19:21.000000 QuickEcharts-1.1.0/QuickEcharts/Charts.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:22:02.640511 QuickEcharts-1.1.0/QuickEcharts.egg-info/
+-rw-rw-rw-   0        0        0    69628 2024-05-23 16:22:02.000000 QuickEcharts-1.1.0/QuickEcharts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-05-23 16:22:02.000000 QuickEcharts-1.1.0/QuickEcharts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 16:22:02.000000 QuickEcharts-1.1.0/QuickEcharts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-23 16:22:02.000000 QuickEcharts-1.1.0/QuickEcharts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 16:22:02.000000 QuickEcharts-1.1.0/QuickEcharts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    69141 2024-05-23 16:21:14.000000 QuickEcharts-1.1.0/README.md
+-rw-rw-rw-   0        0        0      693 2024-03-26 19:47:36.000000 QuickEcharts-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       19 2024-03-05 17:52:13.000000 QuickEcharts-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 16:22:02.642511 QuickEcharts-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1046 2024-05-23 16:19:42.000000 QuickEcharts-1.1.0/setup.py
```

### Comparing `QuickEcharts-1.0.2/LICENSE` & `QuickEcharts-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `QuickEcharts-1.0.2/PKG-INFO` & `QuickEcharts-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuickEcharts
-Version: 1.0.2
+Version: 1.1.0
 Summary: Create Echart plots in a single simple function call, with internal data wrangling via polars
 Home-page: https://github.com/AdrianAntico/QuickEcharts
 Author: ['Adrian Antico']
 Author-email: adrianantico@gmail.com
 License: AGPL >= 3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -18,14 +18,18 @@
 
 QuickEcharts is a Python package that enables one to plot Echarts quickly. It piggybacks off of the pyecharts package that pipes into Apache Echarts. Pyecharts is a great package for fully customizing plots but is quite a challenge to make use of quickly. QuickEcharts solves this with a simple API for defining plotting elements and data, along with automatic data wrangling operations, using polars, to correctly structure data fast.
 
 For the Code Examples below, there is a dataset in the QuickEcharts/datasets folder named FakeBevData.csv that you can download for replication purposes.
 
 # Installation
 ```
+pip install QuickEcharts
+
+or 
+
 pip install git+https://github.com/AdrianAntico/QuickEcharts.git#egg=quickecharts
 ```
 
 <br>
 
 # Code Examples
 
@@ -604,14 +608,15 @@
 # Create Plot in Jupyter Lab
 p1 = Charts.BoxPlot(
   dt = data,
   SampleSize = 100000,
   YVar = 'Daily Liters',
   GroupVar = 'Brand',
   YVarTrans = "logmin",
+  RenderHTML = False,
   Theme = 'dark',
   BackgroundColor = None,
   Width = "1200px",
   Height = "750px",
   ToolBox = True,
   Brush = True,
   DataZoom = True,
@@ -1874,15 +1879,15 @@
 # Pull Data from Package
 FilePath = "..FakeBevData.csv"
 data = pl.read_csv(FilePath)
 
 # Create Plot in Jupyter Lab
 p1 = Charts.Radar(
   dt = data,
-  YVar = 'Daily Liters',
+  YVar = ['Daily Liters', 'Daily Margin'],
   GroupVar = 'Brand',
   AggMethod = 'mean',
   YVarTrans = None,
   RenderHTML = False,
   LabelColor = '#fff',
   LineColors = ["#ed1690", "#8e5fa8", "#00a6fb", "#213f7f", "#22c0df"],
   Theme = 'dark',
```

### Comparing `QuickEcharts-1.0.2/QuickEcharts/Charts.py` & `QuickEcharts-1.1.0/QuickEcharts/Charts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Module: Charts
 # Author: Adrian Antico <adrianantico@gmail.com>
 # License: APGL (>= 3)
-# Release: quickecharts 1.0.2
+# Release: quickecharts 1.1.0
 # Last modified : 2024-03-26
 
 def NumericTransformation(dt, YVar, Trans):
   """
   Parameters
   dt: polars dataframe
   YVar: column to transform
@@ -1645,32 +1645,31 @@
     # Load environment
     from pyecharts import options as opts
     from pyecharts.charts import Boxplot
     import polars as pl
     import math
 
     # SampleSize = 100000
-    # YVar = 'Daily Liters'
-    # GroupVar = 'Brand'
-    # YVarTrans = None
+    # YVar = ['Daily Liters', 'Daily Units']
+    # GroupVar = None # 'Brand'
+    # YVarTrans = [None, 'logmin']
     # XAxisTitle = YVar
     # XAxisNameLocation = 'end'
     # YAxisNameGap = 15
     # XAxisTitle = GroupVar
     # XAxisNameLocation = 'middle'
     # XAxisNameGap = 42
     # AxisPointerType = 'cross' # 'line', 'shadow'
     # RenderHTML = False
     # Title = 'Hist Plot'
     # TitleColor = 'fff'
     # TitleFontSize = 20
     # SubTitle = 'Subtitle'
     # SubTitleColor = 'fff'
     # SubTitleFontSize = 12
-    # YVarTrans = None
     # XVarTrans = None
     # Theme = 'wonderland'
     # Legend = None
     # LegendPosRight = '0%'
     # LegendPosTop = '5%'
     # ToolBox = True
     # Brush = True
@@ -1697,27 +1696,33 @@
         dt1 = dt.clone()
     else:
       dt1 = dt.clone()
 
     # Define Plotting Variable
     if YVar == None:
       return None
+    # YVar and GroupVar Mgt
+    if isinstance(YVar, list):
+      if len(YVar) > 1:
+        GroupVar = None
 
     # Subset Columns
     if GroupVar == None:
       dt1 = dt1.select([pl.col(YVar)])
     else:
       dt1 = dt1.select([pl.col(YVar), pl.col(GroupVar)])
 
     # Transformation
     if not YVarTrans is None:
-      dt1 = NumericTransformation(dt1, YVar, Trans = YVarTrans.lower())
-
-    # Define data elements
-    YVal = [dt1[YVar].to_list()]
+      if isinstance(YVar, list):
+        for i in range(len(YVar)):# i = 1
+          if not YVarTrans[i] is None:
+            dt1 = NumericTransformation(dt1, YVar[i], Trans = YVarTrans[i].lower())
+      else:
+        dt1 = NumericTransformation(dt1, YVar, Trans = YVarTrans.lower())
 
     # Create plot
     InitOptions = {}
     if not Theme is None:
       InitOptions['theme'] = Theme
 
     if not Width is None:
@@ -1748,38 +1753,45 @@
       Buckets.sort()
       bucket_data = []
       c = c.add_xaxis(Buckets)
       for i in Buckets: # i = 'Angel'
         bucket_data.append(dt1.filter(dt1[GroupVar] == i)[YVar].to_list())
       c = c.add_yaxis('YVar', c.prepare_data(bucket_data))
     else:
-      YVal = [dt1[YVar].to_list()]
-      c = c.add_xaxis(['expr1'])
-      c = c.add_yaxis('YVar', c.prepare_data(YVal))
+      if isinstance(YVar, list):
+        c = c.add_xaxis(YVar)
+        bucket_data = []
+        for yvar in YVar:
+          bucket_data.append(dt1[yvar].to_list())
+
+        c = c.add_yaxis('YVar', c.prepare_data(bucket_data))
+      else:
+        YVal = [dt1[YVar].to_list()]
+        c = c.add_yaxis(YVar, c.prepare_data(YVal))
 
     # Global Options
     GlobalOptions = {}
     if Legend == 'right':
       GlobalOptions['legend_opts'] = opts.LegendOpts(pos_right = LegendPosRight, pos_top = LegendPosTop, orient = "vertical", border_width = LegendBorderSize, textstyle_opts = opts.TextStyleOpts(color = LegendTextColor))
     elif Legend == 'top':
       GlobalOptions['legend_opts'] = opts.LegendOpts(pos_top = LegendPosTop, border_width = LegendBorderSize, textstyle_opts = opts.TextStyleOpts(color = LegendTextColor))
     else:
       GlobalOptions['legend_opts'] = opts.LegendOpts(is_show = False)
 
     if not Title is None:
       GlobalOptions['title_opts'] = opts.TitleOpts(
-          title = Title, subtitle = SubTitle,
-          title_textstyle_opts = opts.TextStyleOpts(
-            color = TitleColor,
-            font_size = TitleFontSize,
-          ),
-          subtitle_textstyle_opts = opts.TextStyleOpts(
-            color = SubTitleColor,
-            font_size = SubTitleFontSize,
-          )
+        title = Title, subtitle = SubTitle,
+        title_textstyle_opts = opts.TextStyleOpts(
+          color = TitleColor,
+          font_size = TitleFontSize,
+        ),
+        subtitle_textstyle_opts = opts.TextStyleOpts(
+          color = SubTitleColor,
+          font_size = SubTitleFontSize,
+        )
       )
       
     GlobalOptions['xaxis_opts'] = opts.AxisOpts(name = XAxisTitle, name_location = XAxisNameLocation, name_gap = XAxisNameGap)
     GlobalOptions['yaxis_opts'] = opts.AxisOpts(name = YAxisTitle, name_location = YAxisNameLocation, name_gap = YAxisNameGap)
 
     if ToolBox:
       GlobalOptions['toolbox_opts'] = opts.ToolboxOpts(
@@ -1795,28 +1807,27 @@
     GlobalOptions['tooltip_opts'] = opts.TooltipOpts(trigger = "axis", axis_pointer_type = AxisPointerType)
 
     if Brush:
       GlobalOptions['brush_opts'] = opts.BrushOpts()
 
     if DataZoom and not GroupVar is None:
       GlobalOptions['datazoom_opts'] = [
-          opts.DataZoomOpts(
-            range_start = 0,
-            range_end = 100),
-          opts.DataZoomOpts(
-            type_ = "inside")]
+        opts.DataZoomOpts(
+          range_start = 0,
+          range_end = 100),
+        opts.DataZoomOpts(
+          type_ = "inside")]
     
     # Final Setting of Global Options
     c = c.set_global_opts(**GlobalOptions)
 
     # Series Options
     if not HorizontalLine is None:
       MarkLineDict = {}
       MarkLineDict['data'] = [opts.MarkLineItem(y = HorizontalLine, name = HorizontalLineName)]
-
       c = c.set_series_opts(markline_opts = opts.MarkLineOpts(**MarkLineDict))
 
     # Render html
     if RenderHTML:
       c.render()
   
     return c
@@ -2080,15 +2091,20 @@
       return None
 
     # Subset Columns
     dt1 = dt.select([pl.col(YVar), pl.col(GroupVar)])
 
     # Transformation
     if not YVarTrans is None:
-      dt1 = NumericTransformation(dt1, YVar, Trans = YVarTrans.lower())
+      if isinstance(YVar, list):
+        for i in range(len(YVar)):# i = 0
+          if not YVarTrans[i] is None:
+            dt1 = NumericTransformation(dt1, YVar[i], Trans = YVarTrans[i].lower())
+      else:
+        dt1 = NumericTransformation(dt1, YVar, Trans = YVarTrans.lower())
 
     # Define data elements
     vals_dict = {}
     if not isinstance(YVar, list):
       yVar = [YVar]
     else:
       yVar = YVar
@@ -2359,16 +2375,21 @@
     if not GroupVar is None:
       dt1 = dt.select([pl.col(YVar), pl.col(XVar), pl.col(GroupVar)])
     else:
       dt1 = dt.select([pl.col(YVar), pl.col(XVar)])
 
     # Transformation
     if not YVarTrans is None:
-      dt1 = NumericTransformation(dt1, YVar, Trans = YVarTrans.lower())
-  
+      if isinstance(YVar, list):
+        for i in range(len(YVar)):# i = 0
+          if not YVarTrans[i] is None:
+            dt1 = NumericTransformation(dt1, YVar[i], Trans = YVarTrans[i].lower())
+      else:
+        dt1 = NumericTransformation(dt1, YVar, Trans = YVarTrans.lower())
+
     # Agg Data
     if not PreAgg:
       dt1 = PolarsAggregation(dt1, AggMethod, NumericVariable = YVar, GroupVariable = GroupVar, DateVariable = XVar)
       dt1 = dt1.sort(XVar)
 
     if GroupVar is None:
       yvar_dict = {}
@@ -2874,15 +2895,20 @@
     if not GroupVar is None:
       dt1 = dt.select([pl.col(YVar), pl.col(XVar), pl.col(GroupVar)])
     else:
       dt1 = dt.select([pl.col(YVar), pl.col(XVar)])
 
     # Transformation
     if not YVarTrans is None:
-      dt1 = NumericTransformation(dt1, YVar, Trans = YVarTrans.lower())
+      if isinstance(YVar, list):
+        for i in range(len(YVar)):# i = 0
+          if not YVarTrans[i] is None:
+            dt1 = NumericTransformation(dt1, YVar[i], Trans = YVarTrans[i].lower())
+      else:
+        dt1 = NumericTransformation(dt1, YVar, Trans = YVarTrans.lower())
   
     # Agg Data
     if not PreAgg:
       dt1 = PolarsAggregation(dt1, AggMethod, NumericVariable = YVar, GroupVariable = GroupVar, DateVariable = XVar)
       dt1 = dt1.sort(XVar)
 
     if GroupVar is None:
@@ -3289,15 +3315,20 @@
     if not GroupVar is None:
       dt1 = dt.select([pl.col(YVar), pl.col(XVar), pl.col(GroupVar)])
     else:
       dt1 = dt.select([pl.col(YVar), pl.col(XVar)])
 
     # Transformation
     if not YVarTrans is None:
-      dt1 = NumericTransformation(dt1, YVar, Trans = YVarTrans.lower())
+      if isinstance(YVar, list):
+        for i in range(len(YVar)):# i = 0
+          if not YVarTrans[i] is None:
+            dt1 = NumericTransformation(dt1, YVar[i], Trans = YVarTrans[i].lower())
+      else:
+        dt1 = NumericTransformation(dt1, YVar, Trans = YVarTrans.lower())
   
     # Agg Data
     if not PreAgg:
       dt1 = PolarsAggregation(dt1, AggMethod, NumericVariable = YVar, GroupVariable = GroupVar, DateVariable = XVar)
       dt1 = dt1.sort(XVar)
 
     if GroupVar is None:
@@ -3804,15 +3835,20 @@
     if not GroupVar is None:
       dt1 = dt.select([pl.col(YVar), pl.col(XVar), pl.col(GroupVar)])
     else:
       dt1 = dt.select([pl.col(YVar), pl.col(XVar)])
 
     # Transformation
     if not YVarTrans is None:
-      dt1 = NumericTransformation(dt1, YVar, Trans = YVarTrans.lower())
+      if isinstance(YVar, list):
+        for i in range(len(YVar)):# i = 0
+          if not YVarTrans[i] is None:
+            dt1 = NumericTransformation(dt1, YVar[i], Trans = YVarTrans[i].lower())
+      else:
+        dt1 = NumericTransformation(dt1, YVar, Trans = YVarTrans.lower())
   
     # Agg Data
     if not PreAgg:
       dt1 = PolarsAggregation(dt1, AggMethod, NumericVariable = YVar, GroupVariable = GroupVar, DateVariable = XVar)
       dt1 = dt1.sort(XVar)
 
     if GroupVar is None:
@@ -4250,15 +4286,21 @@
     if not GroupVar is None:
       dt1 = dt.select([pl.col(YVar), pl.col(XVar), pl.col(GroupVar)])
     else:
       dt1 = dt.select([pl.col(YVar), pl.col(XVar)])
 
     # Transformation
     if not YVarTrans is None:
-      dt1 = NumericTransformation(dt1, YVar, Trans = YVarTrans.lower())
+      if isinstance(YVar, list):
+        for i in range(len(YVar)):# i = 0
+          if not YVarTrans[i] is None:
+            dt1 = NumericTransformation(dt1, YVar[i], Trans = YVarTrans[i].lower())
+      else:
+        dt1 = NumericTransformation(dt1, YVar, Trans = YVarTrans.lower())
+
   
     # Agg Data
     if not PreAgg:
       dt1 = PolarsAggregation(dt1, AggMethod, NumericVariable = YVar, GroupVariable = GroupVar, DateVariable = XVar)
       dt1 = dt1.sort(XVar)
 
     # No GroupVar
@@ -4788,15 +4830,20 @@
     if not GroupVar is None:
       dt1 = dt.select([pl.col(YVar), pl.col(XVar), pl.col(GroupVar)])
     else:
       dt1 = dt.select([pl.col(YVar), pl.col(XVar)])
 
     # Transformation
     if not YVarTrans is None:
-      dt1 = NumericTransformation(dt1, YVar, Trans = YVarTrans.lower())
+      if isinstance(YVar, list):
+        for i in range(len(YVar)):# i = 0
+          if not YVarTrans[i] is None:
+            dt1 = NumericTransformation(dt1, YVar[i], Trans = YVarTrans[i].lower())
+      else:
+        dt1 = NumericTransformation(dt1, YVar, Trans = YVarTrans.lower())
   
     # Agg Data
     if not PreAgg:
       dt1 = PolarsAggregation(dt1, AggMethod, NumericVariable = YVar, GroupVariable = GroupVar, DateVariable = XVar)
       dt1 = dt1.sort(XVar)
 
     if GroupVar is None:
@@ -5199,15 +5246,20 @@
     if not GroupVar is None:
       dt1 = dt.select([pl.col(YVar), pl.col(XVar), pl.col(GroupVar)])
     else:
       dt1 = dt.select([pl.col(YVar), pl.col(XVar)])
 
     # Transformation
     if not YVarTrans is None:
-      dt1 = NumericTransformation(dt1, YVar, Trans = YVarTrans.lower())
+      if isinstance(YVar, list):
+        for i in range(len(YVar)):# i = 0
+          if not YVarTrans[i] is None:
+            dt1 = NumericTransformation(dt1, YVar[i], Trans = YVarTrans[i].lower())
+      else:
+        dt1 = NumericTransformation(dt1, YVar, Trans = YVarTrans.lower())
   
     # Agg Data
     if not PreAgg:
       dt1 = PolarsAggregation(dt1, AggMethod, NumericVariable = YVar, GroupVariable = GroupVar, DateVariable = XVar)
       dt1 = dt1.sort(XVar)
 
     # No GroupVar
@@ -5678,15 +5730,20 @@
     if not GroupVar is None:
       dt1 = dt.select([pl.col(YVar), pl.col(XVar), pl.col(GroupVar)])
     else:
       dt1 = dt.select([pl.col(YVar), pl.col(XVar)])
 
     # Transformation
     if not YVarTrans is None:
-      dt1 = NumericTransformation(dt1, YVar, Trans = YVarTrans.lower())
+      if isinstance(YVar, list):
+        for i in range(len(YVar)):# i = 0
+          if not YVarTrans[i] is None:
+            dt1 = NumericTransformation(dt1, YVar[i], Trans = YVarTrans[i].lower())
+      else:
+        dt1 = NumericTransformation(dt1, YVar, Trans = YVarTrans.lower())
   
     # Agg Data
     if not PreAgg:
       dt1 = PolarsAggregation(dt1, AggMethod, NumericVariable = YVar, GroupVariable = GroupVar, DateVariable = XVar)
       dt1 = dt1.sort(XVar)
 
     if GroupVar is None:
@@ -6337,17 +6394,17 @@
     # AnimationDelayUpdate = 0
     # dt = pl.read_csv("C:/Users/Bizon/Documents/GitHub/rappwd/FakeBevData.csv")
 
     # Define Plotting Variable
     if YVar == None:
       return None
 
-    if isinstance(YVar, list):
-      if len(YVar) > 1:
-        GroupVar = None
+    # Define Plotting Variable
+    if XVar == None:
+      return None
 
     # Cap number of records and define dt1
     if SampleSize != None:
       if dt.shape[0] > SampleSize:
         dt1 = dt.sample(n = SampleSize, shuffle = True)
       else:
         dt1 = dt.clone()
@@ -6785,14 +6842,20 @@
     # AnimationEasingUpdate = "cubicOut"
     # AnimationDelayUpdate = 0
     # dt = pl.read_csv("C:/Users/Bizon/Documents/GitHub/rappwd/FakeBevData.csv")
     
     # Define Plotting Variable
     if YVar == None:
       return None
+
+    if XVar == None:
+      return None
+
+    if ZVar == None:
+      return None
     
     # Cap number of records and define dt1
     if SampleSize != None:
       if dt.shape[0] > SampleSize:
         dt1 = dt.sample(n = SampleSize, shuffle = True)
       else:
         dt1 = dt.clone()
@@ -6973,19 +7036,21 @@
     # AnimationEasingUpdate = "cubicOut"
     # AnimationDelayUpdate = 0
     # dt = pl.read_csv("C:/Users/Bizon/Documents/GitHub/rappwd/FakeBevData.csv")
     
     # Define Plotting Variable
     if YVar == None:
       return None
-    
-    if isinstance(YVar, list):
-      if len(YVar) > 1:
-        GroupVar = None
-    
+
+    if XVar == None:
+      return None
+
+    if ZVar == None:
+      return None
+
     # Cap number of records and define dt1
     if SampleSize != None:
       if dt.shape[0] > SampleSize:
         dt1 = dt.sample(n = SampleSize, shuffle = True)
       else:
         dt1 = dt.clone()
     else:
@@ -7246,19 +7311,18 @@
     # AnimationEasingUpdate = "cubicOut"
     # AnimationDelayUpdate = 0
     # dt = pl.read_csv("C:/Users/Bizon/Documents/GitHub/rappwd/FakeBevData.csv")
     
     # Define Plotting Variable
     if YVar == None:
       return None
-    
-    if isinstance(YVar, list):
-      if len(YVar) > 1:
-        GroupVar = None
-    
+
+    if XVar == None:
+      return None
+
     # Cap number of records and define dt1
     if SampleSize != None:
       if dt.shape[0] > SampleSize:
         dt1 = dt.sample(n = SampleSize, shuffle = True)
       else:
         dt1 = dt.clone()
     else:
@@ -8015,15 +8079,14 @@
     # AnimationDelayUpdate = 0
     # dt = pl.read_csv("C:/Users/Bizon/Documents/GitHub/rappwd/FakeBevData.csv")
     
     # Subset Columns
     dt1 = dt.select([pl.col(YVar), pl.col(XVar), pl.col(ZVar)])
     
     # Transformation
-    
     if not ZVarTrans is None:
       dt1 = NumericTransformation(dt1, ZVar, Trans = ZVarTrans.lower())
   
     # Agg Data
     if not PreAgg:
       dt1 = PolarsAggregation(dt1, AggMethod, NumericVariable = ZVar, GroupVariable = [YVar, XVar], DateVariable = None)
       dt1 = dt1.sort(YVar)
@@ -8258,21 +8321,20 @@
 
     dt1 = dt.select(cols)
     if not PreAgg:
       dt1 = PolarsAggregation(dt1, AggMethod, NumericVariable = YVars, GroupVariable = GroupVar, DateVariable = DateVar)
 
     # Transformation
     if not YVarTrans is None:
-      if isinstance(YVars, list):
-        counter = -1
-        for t in YVarTrans:
-          counter += 1
-          dt1 = NumericTransformation(dt1, YVars[counter], Trans = t.lower())
+      if isinstance(YVar, list):
+        for i in range(len(YVar)):# i = 0
+          if not YVarTrans[i] is None:
+            dt1 = NumericTransformation(dt1, YVar[i], Trans = YVarTrans[i].lower())
       else:
-        dt1 = NumericTransformation(dt1, YVars, Trans = YVarTrans.lower())
+        dt1 = NumericTransformation(dt1, YVar, Trans = YVarTrans.lower())
 
     if isinstance(YVars, list):
       if len(YVars) > 1:
         x_data = YVars
         dt2 = dt1.melt(id_vars = DateVar, value_vars = YVars)
         dt2 = dt2.rename({"variable": "Series", "value": "Values"})
         DateVal = dt2[DateVar].to_list()
```

### Comparing `QuickEcharts-1.0.2/QuickEcharts.egg-info/PKG-INFO` & `QuickEcharts-1.1.0/QuickEcharts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuickEcharts
-Version: 1.0.2
+Version: 1.1.0
 Summary: Create Echart plots in a single simple function call, with internal data wrangling via polars
 Home-page: https://github.com/AdrianAntico/QuickEcharts
 Author: ['Adrian Antico']
 Author-email: adrianantico@gmail.com
 License: AGPL >= 3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -18,14 +18,18 @@
 
 QuickEcharts is a Python package that enables one to plot Echarts quickly. It piggybacks off of the pyecharts package that pipes into Apache Echarts. Pyecharts is a great package for fully customizing plots but is quite a challenge to make use of quickly. QuickEcharts solves this with a simple API for defining plotting elements and data, along with automatic data wrangling operations, using polars, to correctly structure data fast.
 
 For the Code Examples below, there is a dataset in the QuickEcharts/datasets folder named FakeBevData.csv that you can download for replication purposes.
 
 # Installation
 ```
+pip install QuickEcharts
+
+or 
+
 pip install git+https://github.com/AdrianAntico/QuickEcharts.git#egg=quickecharts
 ```
 
 <br>
 
 # Code Examples
 
@@ -604,14 +608,15 @@
 # Create Plot in Jupyter Lab
 p1 = Charts.BoxPlot(
   dt = data,
   SampleSize = 100000,
   YVar = 'Daily Liters',
   GroupVar = 'Brand',
   YVarTrans = "logmin",
+  RenderHTML = False,
   Theme = 'dark',
   BackgroundColor = None,
   Width = "1200px",
   Height = "750px",
   ToolBox = True,
   Brush = True,
   DataZoom = True,
@@ -1874,15 +1879,15 @@
 # Pull Data from Package
 FilePath = "..FakeBevData.csv"
 data = pl.read_csv(FilePath)
 
 # Create Plot in Jupyter Lab
 p1 = Charts.Radar(
   dt = data,
-  YVar = 'Daily Liters',
+  YVar = ['Daily Liters', 'Daily Margin'],
   GroupVar = 'Brand',
   AggMethod = 'mean',
   YVarTrans = None,
   RenderHTML = False,
   LabelColor = '#fff',
   LineColors = ["#ed1690", "#8e5fa8", "#00a6fb", "#213f7f", "#22c0df"],
   Theme = 'dark',
```

### Comparing `QuickEcharts-1.0.2/README.md` & `QuickEcharts-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
 QuickEcharts is a Python package that enables one to plot Echarts quickly. It piggybacks off of the pyecharts package that pipes into Apache Echarts. Pyecharts is a great package for fully customizing plots but is quite a challenge to make use of quickly. QuickEcharts solves this with a simple API for defining plotting elements and data, along with automatic data wrangling operations, using polars, to correctly structure data fast.
 
 For the Code Examples below, there is a dataset in the QuickEcharts/datasets folder named FakeBevData.csv that you can download for replication purposes.
 
 # Installation
 ```
+pip install QuickEcharts
+
+or 
+
 pip install git+https://github.com/AdrianAntico/QuickEcharts.git#egg=quickecharts
 ```
 
 <br>
 
 # Code Examples
 
@@ -590,14 +594,15 @@
 # Create Plot in Jupyter Lab
 p1 = Charts.BoxPlot(
   dt = data,
   SampleSize = 100000,
   YVar = 'Daily Liters',
   GroupVar = 'Brand',
   YVarTrans = "logmin",
+  RenderHTML = False,
   Theme = 'dark',
   BackgroundColor = None,
   Width = "1200px",
   Height = "750px",
   ToolBox = True,
   Brush = True,
   DataZoom = True,
@@ -1860,15 +1865,15 @@
 # Pull Data from Package
 FilePath = "..FakeBevData.csv"
 data = pl.read_csv(FilePath)
 
 # Create Plot in Jupyter Lab
 p1 = Charts.Radar(
   dt = data,
-  YVar = 'Daily Liters',
+  YVar = ['Daily Liters', 'Daily Margin'],
   GroupVar = 'Brand',
   AggMethod = 'mean',
   YVarTrans = None,
   RenderHTML = False,
   LabelColor = '#fff',
   LineColors = ["#ed1690", "#8e5fa8", "#00a6fb", "#213f7f", "#22c0df"],
   Theme = 'dark',
```

### Comparing `QuickEcharts-1.0.2/pyproject.toml` & `QuickEcharts-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `QuickEcharts-1.0.2/setup.py` & `QuickEcharts-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 with open(os.path.join(HERE, "requirements.txt")) as f:
     required = f.read().splitlines()
 
 setup(
     name="QuickEcharts",
-    version="1.0.2",
+    version="1.1.0",
     description="Create Echart plots in a single simple function call, with internal data wrangling via polars",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/AdrianAntico/QuickEcharts",
     author=["Adrian Antico"],
     author_email="adrianantico@gmail.com",
     license="AGPL >= 3",
```

