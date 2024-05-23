# Comparing `tmp/mdbase-0.3.3.tar.gz` & `tmp/mdbase-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdbase-0.3.3.tar", last modified: Wed Mar 13 16:36:28 2024, max compression
+gzip compressed data, was "mdbase-0.4.tar", last modified: Thu May 23 16:18:19 2024, max compression
```

## Comparing `mdbase-0.3.3.tar` & `mdbase-0.4.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-13 16:36:28.159518 mdbase-0.3.3/
--rw-rw-rw-   0        0        0     1553 2023-11-09 13:12:24.000000 mdbase-0.3.3/LICENCE
--rw-rw-rw-   0        0        0     1855 2024-03-13 16:36:28.158261 mdbase-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     1317 2024-03-12 17:14:38.000000 mdbase-0.3.3/README.md
--rw-rw-rw-   0        0        0      108 2021-08-03 08:03:10.000000 mdbase-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-13 16:36:28.159518 mdbase-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1259 2024-03-12 17:15:17.000000 mdbase-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-13 16:36:28.150616 mdbase-0.3.3/src/
-drwxrwxrwx   0        0        0        0 2024-03-13 16:36:28.155840 mdbase-0.3.3/src/mdbase/
--rw-rw-rw-   0        0        0     1439 2024-03-12 17:11:08.000000 mdbase-0.3.3/src/mdbase/__init__.py
--rw-rw-rw-   0        0        0     3818 2024-03-12 17:11:21.000000 mdbase-0.3.3/src/mdbase/data.py
--rw-rw-rw-   0        0        0     5045 2024-03-12 17:13:10.000000 mdbase-0.3.3/src/mdbase/io.py
--rw-rw-rw-   0        0        0    52537 2024-03-12 21:25:38.000000 mdbase-0.3.3/src/mdbase/stats.py
-drwxrwxrwx   0        0        0        0 2024-03-13 16:36:28.158261 mdbase-0.3.3/src/mdbase.egg-info/
--rw-rw-rw-   0        0        0     1855 2024-03-13 16:36:28.000000 mdbase-0.3.3/src/mdbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2024-03-13 16:36:28.000000 mdbase-0.3.3/src/mdbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-13 16:36:28.000000 mdbase-0.3.3/src/mdbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-03-13 16:36:28.000000 mdbase-0.3.3/src/mdbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 16:18:19.677154 mdbase-0.4/
+-rw-rw-rw-   0        0        0     1553 2023-11-09 13:12:24.000000 mdbase-0.4/LICENCE
+-rw-rw-rw-   0        0        0     1928 2024-05-23 16:18:19.677154 mdbase-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1392 2024-05-23 16:04:30.000000 mdbase-0.4/README.md
+-rw-rw-rw-   0        0        0      108 2021-08-03 08:03:10.000000 mdbase-0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 16:18:19.677154 mdbase-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1259 2024-03-12 17:15:17.000000 mdbase-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:18:19.672098 mdbase-0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 16:18:19.674098 mdbase-0.4/src/mdbase/
+-rw-rw-rw-   0        0        0     1364 2024-05-23 15:44:10.000000 mdbase-0.4/src/mdbase/__init__.py
+-rw-rw-rw-   0        0        0     9843 2024-05-23 15:54:59.000000 mdbase-0.4/src/mdbase/data.py
+-rw-rw-rw-   0        0        0    53382 2024-05-23 15:55:19.000000 mdbase-0.4/src/mdbase/stats.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:18:19.676430 mdbase-0.4/src/mdbase.egg-info/
+-rw-rw-rw-   0        0        0     1928 2024-05-23 16:18:19.000000 mdbase-0.4/src/mdbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2024-05-23 16:18:19.000000 mdbase-0.4/src/mdbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 16:18:19.000000 mdbase-0.4/src/mdbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-23 16:18:19.000000 mdbase-0.4/src/mdbase.egg-info/top_level.txt
```

### Comparing `mdbase-0.3.3/LICENCE` & `mdbase-0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `mdbase-0.3.3/PKG-INFO` & `mdbase-0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdbase
-Version: 0.3.3
+Version: 0.4
 Summary: MDbase :: join + process multiple XLS databases
 Home-page: https://github.com/mirekslouf/mdbase/
 Author: Mirek Slouf
 Author-email: mirek.slouf@gmail.com
 License: MIT
 Project-URL: Documentation, https://mirekslouf.github.io/mdbase/
 Classifier: Programming Language :: Python :: 3
@@ -43,8 +43,10 @@
   [documentation](https://mirekslouf.github.io/mdbase/docs/).
 
 Versions of MDBASE
 ------------------
 * Version 0.1 = complete, working, but without documentation
 * Version 0.2 = several minor improvements + basic documentation
 * Version 0.3 = further improvements in both code and documentation
+* Version 0.4 = updates, corrections, re-arranged modules, updated docs
+
```

### Comparing `mdbase-0.3.3/README.md` & `mdbase-0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -27,8 +27,10 @@
   [documentation](https://mirekslouf.github.io/mdbase/docs/).
 
 Versions of MDBASE
 ------------------
 * Version 0.1 = complete, working, but without documentation
 * Version 0.2 = several minor improvements + basic documentation
 * Version 0.3 = further improvements in both code and documentation
+* Version 0.4 = updates, corrections, re-arranged modules, updated docs
+
```

### Comparing `mdbase-0.3.3/setup.py` & `mdbase-0.4/setup.py`

 * *Files identical despite different names*

### Comparing `mdbase-0.3.3/src/mdbase/__init__.py` & `mdbase-0.4/src/mdbase/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 '''
-mdbase package
+Package: mdbase
 --------------
 Join and proces multiple XLS files.
 
 List of modules:
 
-* mdbase.io = read multiple XLS files into one single pandas.DataFrame
-* mdbase.data = additional, auxiliary functions for data in pandas.DataFrame
-* mdbase.stats = key module; statistical calculations and plotting of the data
+* mdbase.data = read multiple XLS files into one single pandas.DataFrame
+* mdbase.stats = statistical calculations and plotting of the DataFrame data
 
 Simple and minimalistic, but real and working example:
 
 >>> """ MDbase :: correlation plot """
 >>> 
->>> import mdbase.io, mdbase.stats
+>>> import mdbase.data, mdbase.stats
 >>> 
 >>> # Define directory with databases + XLS database files
 >>> DDIR  = r'../../'
 >>> DBASE1 = DDIR + r'DBASE/CZ/database_cz_2024-03-11.xlsm'
 >>> DBASE2 = DDIR + r'DBASE/IT/database_it_2024-03-11.xlsm'
 >>> DBASE3 = DDIR + r'DBASE/ES/database_es_2024-03-11.xlsm'
 >>> 
 >>> # Join all XLS databases into one pandas.DataFrame object
->>> df = mdbase.io.read_multiple_databases(
+>>> df = mdbase.data.read_multiple_databases(
 >>>     excel_files=[DBASE1,DBASE2,DBASE3],
 >>>     sheet_names=['HIPs','KNEEs'])
 >>> 
 >>> # Define properties in the database we want to correlate and plot
 >>> P1,P2 = ('OI_max_W','CI_max_W')
 >>> 
 >>> # Correlation plot, all experimental data + fitting with Power law model
 >>> CPLOT = mdbase.stats.CorrelationPlot(df)
 >>> CPLOT.correlation(P1, P2, marker='rx', label='Experimental data')
 >>> CPLOT.regression(P1, P2, rtype='power', label=r'Model: $y = kx^n$')
 >>> CPLOT.finalize('OI(max,W)', 'CI(max,W)')
 >>> CPLOT.save('corr_oi-ci.py.png')
 '''
 
-__version__ = "0.3.3"
+__version__ = "0.4"
```

### Comparing `mdbase-0.3.3/src/mdbase/stats.py` & `mdbase-0.4/src/mdbase/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-mdbase.stats
-------------
-Statistical calculations and plotting in MDBASE.
+Module: mdbase.stats
+---------------------
+Statistical calculations and plotting in package MDBASE.
 
 * In MDBASE, statistical calculations and plotting are connected.
 * Current version of MDBASE calculates 4 different plot types + statistics:
     - Correlation plot + statistics: Pearson's r, p-values, R2 coefficients
     - Scatterplot matrix graph + statistics: Pearson's r + p-values
     - Scatterplot matrix tables (two heatmaps with Pearson's r + p-values')
     - Boxplots + statistics: p-values quantifying differences among groups
@@ -30,15 +30,15 @@
 
 import os
 import sys
 import numpy as np
 import matplotlib.pyplot as plt
 import scipy.stats, scipy.optimize
 import seaborn as sns
-import mdbase.io as mio
+import mdbase.data
 
 class PlotParameters:
     '''
     Global plot parameters.
     
     * PlotParametrs methods modify global variable matplotlib.pyplot.rcParams.
     * For single plots, the methods are auto-called during plot initialization.
@@ -1119,23 +1119,39 @@
             The width of boxes in the plot.
 
         Returns
         -------
         None.
 
         '''
-        # Boxplot parameters below are somewhat confusing - brief summary:
+        # Create the boxplot
+        # => create boxplot = add boxes = command: sns.boxplot 
+        # => the following commands/functions just fine-tune the boxplot params
+        # -----
+        # Boxplot must be created with pre-processed dataframe
+        # * Example:
+        #   If we want to compare 'EtO' and 'gIRR' sterilizations
+        #   the dataframe must contain ONLY 'EtO' and 'gIRR' values
+        #   in df.Sterilization column (i.e. in the column with x-data).
+        # * This function accepts the pre-processed database.
+        #   The database must be pre-processed in the main script.
+        #   We can use something like: df = df[df[X].isin(CATEGORIES)],
+        #   which will keep only specific CATEGORIES in column X.
+        # -----
+        # Boxplot parameters:
+        # (boxplot parameters are somewhat confusing => described below
         # (boxplots are rather flexible, this is just one of the possibilities
         # X = column in df containing categorical data -> X-axis
         # Y = column in df containing numerical data (such as OI_max) -> Y-axis
         # hue = color of X-data => here: number of colors = number of X-data
-        # legend=False => no legend -> default here, but it is good to specify)
+        # legend=False => no legend -> default, but we set this explicitly
         # order = order of data in X-axis -> here: order = categories order
         # palette = definition of colors -> no of colors = no of categories
         # width, ax = clear: width of columns and ax-object = where to plot
+        # -----
         sns.boxplot(
             data=self.df, x=x, y=y, hue=x, legend=False,
             order=categories, palette=colors, width=0.5, ax=self.ax)
 
     
     def label(self, plot_label, xpos=-0.30, ypos=1.00, fontsize=10):
         '''
@@ -1265,15 +1281,15 @@
         None
             The output is the calculated statistics
             on the screen and in the text file (with name = output_stats).
         '''
         # Name of TXT file with output statistics that corresponds to BoxPlot
         if output_stats == 'default': output_stats = sys.argv[0]+'.txt'
         # Start writing to both standard output and output_stats file
-        logfile = mio.Logger(output_stats)
+        logfile = mdbase.data.Logger(output_stats)
         # Calulate and print statistics
         print('Correlation matrix table (p-values)')
         print('-----------------------------------')
         for category1 in CATS:
             print(f'{category1:12s}', end='')
             for category2 in CATS:
                 xdata = self.df[Y][self.df[X] == category1]
```

### Comparing `mdbase-0.3.3/src/mdbase.egg-info/PKG-INFO` & `mdbase-0.4/src/mdbase.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdbase
-Version: 0.3.3
+Version: 0.4
 Summary: MDbase :: join + process multiple XLS databases
 Home-page: https://github.com/mirekslouf/mdbase/
 Author: Mirek Slouf
 Author-email: mirek.slouf@gmail.com
 License: MIT
 Project-URL: Documentation, https://mirekslouf.github.io/mdbase/
 Classifier: Programming Language :: Python :: 3
@@ -43,8 +43,10 @@
   [documentation](https://mirekslouf.github.io/mdbase/docs/).
 
 Versions of MDBASE
 ------------------
 * Version 0.1 = complete, working, but without documentation
 * Version 0.2 = several minor improvements + basic documentation
 * Version 0.3 = further improvements in both code and documentation
+* Version 0.4 = updates, corrections, re-arranged modules, updated docs
+
```

