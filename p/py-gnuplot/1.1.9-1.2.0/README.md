# Comparing `tmp/py-gnuplot-1.1.9.tar.gz` & `tmp/py-gnuplot-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-gnuplot-1.1.9.tar", last modified: Fri Feb  2 10:59:59 2024, max compression
+gzip compressed data, was "py-gnuplot-1.2.0.tar", last modified: Tue Feb  6 15:46:17 2024, max compression
```

## Comparing `py-gnuplot-1.1.9.tar` & `py-gnuplot-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 test1     (1000) test1     (1000)        0 2024-02-02 10:59:59.530785 py-gnuplot-1.1.9/
--rw-r--r--   0 test1     (1000) test1     (1000)       36 2024-02-02 07:06:20.000000 py-gnuplot-1.1.9/CHANGELOG.txt
--rw-r--r--   0 test1     (1000) test1     (1000)     1418 2024-02-02 07:06:20.000000 py-gnuplot-1.1.9/LICENSE.txt
--rw-r--r--   0 test1     (1000) test1     (1000)       96 2024-02-02 07:06:20.000000 py-gnuplot-1.1.9/MANIFEST.in
--rw-rw-r--   0 test1     (1000) test1     (1000)    58226 2024-02-02 10:59:59.530785 py-gnuplot-1.1.9/PKG-INFO
--rw-r--r--   0 test1     (1000) test1     (1000)    57911 2024-02-02 10:59:41.000000 py-gnuplot-1.1.9/README.rst
-drwxrwxr-x   0 test1     (1000) test1     (1000)        0 2024-02-02 10:59:59.530785 py-gnuplot-1.1.9/py_gnuplot.egg-info/
--rw-rw-r--   0 test1     (1000) test1     (1000)    58226 2024-02-02 10:59:59.000000 py-gnuplot-1.1.9/py_gnuplot.egg-info/PKG-INFO
--rw-rw-r--   0 test1     (1000) test1     (1000)      299 2024-02-02 10:59:59.000000 py-gnuplot-1.1.9/py_gnuplot.egg-info/SOURCES.txt
--rw-rw-r--   0 test1     (1000) test1     (1000)        1 2024-02-02 10:59:59.000000 py-gnuplot-1.1.9/py_gnuplot.egg-info/dependency_links.txt
--rw-rw-r--   0 test1     (1000) test1     (1000)        7 2024-02-02 10:59:59.000000 py-gnuplot-1.1.9/py_gnuplot.egg-info/requires.txt
--rw-rw-r--   0 test1     (1000) test1     (1000)       10 2024-02-02 10:59:59.000000 py-gnuplot-1.1.9/py_gnuplot.egg-info/top_level.txt
-drwxrwxr-x   0 test1     (1000) test1     (1000)        0 2024-02-02 10:59:59.530785 py-gnuplot-1.1.9/pygnuplot/
--rw-r--r--   0 test1     (1000) test1     (1000)      348 2024-02-02 07:06:20.000000 py-gnuplot-1.1.9/pygnuplot/__init__.py
--rw-r--r--   0 test1     (1000) test1     (1000)    12251 2024-02-02 10:55:09.000000 py-gnuplot-1.1.9/pygnuplot/gnuplot.py
--rw-r--r--   0 test1     (1000) test1     (1000)     4425 2024-02-02 07:06:20.000000 py-gnuplot-1.1.9/pygnuplot/pyplot.py
--rw-r--r--   0 test1     (1000) test1     (1000)       38 2024-02-02 10:59:59.530785 py-gnuplot-1.1.9/setup.cfg
--rw-r--r--   0 test1     (1000) test1     (1000)      612 2024-02-02 10:55:09.000000 py-gnuplot-1.1.9/setup.py
+drwxrwxr-x   0 test1     (1000) test1     (1000)        0 2024-02-06 15:46:17.297607 py-gnuplot-1.2.0/
+-rw-r--r--   0 test1     (1000) test1     (1000)       36 2020-05-17 10:24:41.000000 py-gnuplot-1.2.0/CHANGELOG.txt
+-rw-r--r--   0 test1     (1000) test1     (1000)     1418 2021-06-11 15:51:50.000000 py-gnuplot-1.2.0/LICENSE.txt
+-rw-r--r--   0 test1     (1000) test1     (1000)       96 2020-05-25 11:57:26.000000 py-gnuplot-1.2.0/MANIFEST.in
+-rw-rw-r--   0 test1     (1000) test1     (1000)    42012 2024-02-06 15:46:17.297607 py-gnuplot-1.2.0/PKG-INFO
+-rw-r--r--   0 test1     (1000) test1     (1000)    41697 2024-02-06 15:44:49.000000 py-gnuplot-1.2.0/README.rst
+drwxrwxr-x   0 test1     (1000) test1     (1000)        0 2024-02-06 15:46:17.293607 py-gnuplot-1.2.0/py_gnuplot.egg-info/
+-rw-rw-r--   0 test1     (1000) test1     (1000)    42012 2024-02-06 15:46:17.000000 py-gnuplot-1.2.0/py_gnuplot.egg-info/PKG-INFO
+-rw-rw-r--   0 test1     (1000) test1     (1000)      289 2024-02-06 15:46:17.000000 py-gnuplot-1.2.0/py_gnuplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 test1     (1000) test1     (1000)        1 2024-02-06 15:46:17.000000 py-gnuplot-1.2.0/py_gnuplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 test1     (1000) test1     (1000)        7 2024-02-06 15:46:17.000000 py-gnuplot-1.2.0/py_gnuplot.egg-info/requires.txt
+-rw-rw-r--   0 test1     (1000) test1     (1000)       10 2024-02-06 15:46:17.000000 py-gnuplot-1.2.0/py_gnuplot.egg-info/top_level.txt
+drwxrwxr-x   0 test1     (1000) test1     (1000)        0 2024-02-06 15:46:17.293607 py-gnuplot-1.2.0/pygnuplot/
+-rw-r--r--   0 test1     (1000) test1     (1000)      342 2024-02-03 02:48:08.000000 py-gnuplot-1.2.0/pygnuplot/__init__.py
+-rw-r--r--   0 test1     (1000) test1     (1000)    12261 2024-02-06 14:33:33.000000 py-gnuplot-1.2.0/pygnuplot/gnuplot.py
+-rw-r--r--   0 test1     (1000) test1     (1000)     4425 2020-06-02 02:23:31.000000 py-gnuplot-1.2.0/pygnuplot/pyplot.py
+-rw-rw-r--   0 test1     (1000) test1     (1000)       38 2024-02-06 15:46:17.297607 py-gnuplot-1.2.0/setup.cfg
+-rw-r--r--   0 test1     (1000) test1     (1000)      612 2024-02-06 15:45:36.000000 py-gnuplot-1.2.0/setup.py
```

### Comparing `py-gnuplot-1.1.9/LICENSE.txt` & `py-gnuplot-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py-gnuplot-1.1.9/PKG-INFO` & `py-gnuplot-1.2.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,1315 +1,840 @@
-Metadata-Version: 2.1
-Name: py-gnuplot
-Version: 1.1.9
-Summary: py-gnuplot is a python plot tools based on gnuplot.
-Home-page: http://www.gnuplot.info
-Author: Yongping Guo
-Author-email: guoyoooping@163.com
-License: GPLv3
-Keywords: gnuplot,pandas
-Platform: UNKNOWN
-Requires-Python: >=3.6
-License-File: LICENSE.txt
-
 .. meta::
    :description: gnuplot plotting backend for python.
    :keywords: gnuplot, py-gnuplot, pandas, python, plot
 
-Gnuplot is a portable command-line driven graphing utility for many
-platforms. To leverage the powful gnuplot to plot beautiful image in
-efficicent way in python, we port gnuplot to python. Let's see an example
-at first:
-
-..
-    cmd2img:: python3
-    :image: simple.1.png
+Gnuplot is a powerful command-line driven graphing utility for many platforms.
+To leverage the powful gnuplot to plot beautiful image in efficicent way in
+python, we port gnuplot to python. 
+
+We develop **set()/unset()** function to set or unset gnuplot plotting style,
+**plot()/splot()** to operate gnuplot plot or splot command, **cmd()** to
+execute any commands that coulnd't be done by the above functions. They are
+intuative and gnuplot users can swith to py-gnuplot naturally. By this means we
+can do what gnuplot do.
+
+.. image:: https://gnuplot.sourceforge.net/demo_6.0/transparent.2.png
+    :align: right
+    :width: 300
+
+But for plotting python generated data the above functions are not enough. We
+develop **plot_data()/splot_data()** to plot data generated in
+python.
+
+Here is a quick examples to generate the right image with only basic functions,
+more examples which plot python generated data are coming in later sections.
+
+.. _sphinx-plot-directive: https://pypi.org/project/sphinx-plot-directive
 
+.. _quick_example.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
 
-    gnuplot.plot('[-10:10] sin(x)',
-           'atan(x)',
-           'cos(atan(x))',
-           terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400',
-           output = '"simple.1.png"',
-           key = 'fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid',
-           samples = '50, 50',
-           title = '"Simple Plots" font ",20" textcolor lt -1 norotate',
-           xrange = '[ * : * ] noreverse writeback',
-           x2range = '[ * : * ] noreverse writeback',
-           yrange = '[ * : * ] noreverse writeback',
-           y2range = '[ * : * ] noreverse writeback',
-           zrange = '[ * : * ] noreverse writeback',
-           cbrange = '[ * : * ] noreverse writeback',
-           rrange = '[ * : * ] noreverse writeback',
-           colorbox = 'vertical origin screen 0.9, 0.2 size screen 0.05, 0.6 front noinvert bdefault',
-           #NO_ANIMATION = '1', #I don't know what's this. Who know? please tell me. Thanks.
-           )
-
-From the example we can see, we plot the function with plot() function, with
-all the options as the function parameters. It's easy to understand and comply
-with both gnuplot and python's grammer. The generated image is as below:
-
-.. figure:: http://gnuplot.sourceforge.net/demo/simple.1.png 
-   :width: 350
+    #py-gnuplot: A quick demo
 
-   figure 1. pygnuplot demo 1: simple function
+    #Ceate a gnuplot context. with "log = True" to print the gnuplot execute log.
+    g = gnuplot.Gnuplot(log = True)
 
-Let's see the detail in the below:
+    #Set plotting style
+    g.set(terminal = 'pngcairo transparent enhanced font "arial,8" fontscale 1.0 size 512, 280 ',
+            output = '"quick_example.png"',
+            style = ["fill transparent solid 0.50 noborder", "data lines", "function filledcurves y1=0"],
+            key = 'title "Gaussian Distribution" center fixed left top vertical Left reverse enhanced autotitle nobox noinvert samplen 1 spacing 1 width 0 height 0',
+            title = '"Transparent filled curves"',
+            xrange = '[ -5.00000 : 5.00000 ] noreverse nowriteback',
+            yrange = '[ 0.00000 : 1.00000 ] noreverse nowriteback')
 
-.. contents:: [Contents]
-   :depth: 3
+    #Expressions and caculations
+    g.cmd('Gauss(x,mu,sigma) = 1./(sigma*sqrt(2*pi)) * exp( -(x-mu)**2 / (2*sigma**2) )',
+            'd1(x) = Gauss(x, 0.5, 0.5)',
+            'd2(x) = Gauss(x,  2.,  1.)',
+            'd3(x) = Gauss(x, -1.,  2.)')
 
-1. Introduction and examples list
-===================================
+    #Plotting
+    g.plot('d1(x) fs solid 1.0 lc rgb "forest-green" title "μ =  0.5 σ = 0.5"',
+            'd2(x) lc rgb "gold" title "μ =  2.0 σ = 1.0"',
+            'd3(x) lc rgb "dark-violet" title "μ = -1.0 σ = 2.0"')
 
-As we know Gnuplot is a portable and powerful command-line driven graphing
-utility for many platforms. To leverage the power of Gnuplot, We develop
-the py-gnuplot in a easy understand way.
-
-**py-python only support python3** since the function dictionary paramaters in
-python2 is not in order.
-
-This package has an object-oriented design as well as direct function call to
-allows the user flexibility to set plot options and to run multiple gnuplot
-sessions simultaneously. So in this document, every examples are rendered in
-two way: quick plot mode and object-oriented. Either mode works and you can
-choose which way you like.
-
-We will introduce it in detail in the following chapter and here list the
-exaples used in this article as below:
-
-.. _Table1:
-
-.. list-table:: Table1 : A demostration of pygnuplot.gnuplot script
-   :widths: 15, 20, 20, 70
-   :header-rows: 1
-
-   * - gnuplot demo script
-     - object-oriented interface script
-     - direct function call script
-     - All the script produce the same image
-   * - `simple.dem`_
-     - simple2.py_
-     - simple3.py_
-     - |simple.1.png|
-   * - `surface2.dem`_
-     - surface1.py_
-     - surface2.py_
-     - |surface2.9.png|
-   * - `iterate.dem`_
-     - whale1.py_
-     - whale2.py_
-     - |whale.png|
+more examples:
 
-.. _Table2:
+.. _simple.1.gnu: http://gnuplot.sourceforge.net/demo/simple.1.gnu
+.. _surface2.9.gnu: http://gnuplot.sourceforge.net/demo/surface2.9.gnu
+.. _histograms.1.gnu: http://gnuplot.sourceforge.net/demo/histograms.1.gnu
+.. _iterate.2.gnu: http://gnuplot.sourceforge.net/demo/iterate.2.gnu
+.. _finance.13.gnu: http://gnuplot.sourceforge.net/demo/finance.13.gnu
 
-.. list-table:: Table 2: A demostration of plot() and plot_data()
-   :widths: 15, 20, 20, 70
-   :header-rows: 1
-
-   * - gnuplot demo script
-     - object-oriented interface script
-     - direct function call script
-     - All the script produce the same image
-   * - `histo.1.gnu`_
-     - histo.1.py_
-     - histo.2.py_
-     - |histograms.1.png|
-   * - `finance.dem`_
-     - finance1.py_
-     - finance1.py_
-     - |finance.13.png|
-
-.. list-table:: Table 3: Examples porting from Matplotlib
-   :widths: 35, 35, 35, 35
-   :header-rows: 0
-
-   * - `3.2.1 Stacked bar chart`_ |sphx_glr_bar_stacked_001.png|
-     - `3.2.2 Grouped bar chart with labels`_ |sphx_glr_barchart_001.png|
-     - `3.2.3 Multiplot Axes Demo`_ |sphx_glr_axes_demo_001.png|
-     - `3.2.4 control view and zoom`_ |sphx_glr_axes_margins_001.png|
-   * - `3.2.5 Rendering math equation using TeX`_ |sphx_glr_tex_demo_001.png|
-     - `3.2.6 Basic pie chart`_ |sphx_glr_pie_features_0011.png|
-     - 
-     - 
-
-.. _simple.dem: http://gnuplot.sourceforge.net/demo/simple.1.gnu
-.. _surface2.dem: http://gnuplot.sourceforge.net/demo/surface2.9.gnu
-.. _histo.1.gnu: http://gnuplot.sourceforge.net/demo/histograms.1.gnu
-.. _iterate.dem: http://gnuplot.sourceforge.net/demo/iterate.2.gnu
-.. _finance.dem: http://gnuplot.sourceforge.net/demo/finance.13.gnu
 .. |simple.1.png| image:: http://gnuplot.sourceforge.net/demo/simple.1.png
-   :width: 180
+   :width: 350
 .. |surface2.9.png| image:: http://gnuplot.sourceforge.net/demo/surface2.9.png
-   :width: 180
+   :width: 350
 .. |finance.13.png| image:: http://gnuplot.sourceforge.net/demo/finance.13.png
-   :width: 180
+   :width: 350
 .. |iterate.2.png| image:: http://gnuplot.sourceforge.net/demo/iterate.2.png
-   :width: 180
+   :width: 350
 .. |whale.png| image:: http://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.png
-   :width: 180
-.. |histograms.1.png| image:: http://gnuplot.sourceforge.net/demo/histograms.1.png
-   :width: 180
+   :width: 350
+.. |histograms.2.png| image:: http://gnuplot.sourceforge.net/demo/histograms.2.png
+   :width: 350
 .. |sphx_glr_bar_stacked_001.png| image:: https://matplotlib.org/_images/sphx_glr_bar_stacked_001.png
-   :width: 180
+   :width: 350
 .. |sphx_glr_barchart_001.png| image:: https://matplotlib.org/_images/sphx_glr_barchart_001.png
-   :width: 180
+   :width: 350
 .. |sphx_glr_axes_demo_001.png| image:: https://matplotlib.org/_images/sphx_glr_axes_demo_001.png
-   :width: 180
+   :width: 350
 .. |sphx_glr_pie_features_0011.png| image:: https://matplotlib.org/_images/sphx_glr_pie_features_0011.png
-   :width: 180
+   :width: 350
 .. |sphx_glr_tex_demo_001.png| image:: https://matplotlib.org/_images/sphx_glr_tex_demo_001.png
-   :width: 180
+   :width: 350
 .. |sphx_glr_axes_margins_001.png| image:: https://matplotlib.org/_images/sphx_glr_axes_margins_001.png
-   :width: 180
+   :width: 350
+
+.. list-table:: Table1 : plot examples with different script
 
-2. Plot elements in py-gnuplot
-=================================
+   * - examples
+     - plot function
+     - plot file
+     - splot function
+     - splot file
+     - multiplot
+   * - figure
+     - |simple.1.png|
+     - |histograms.2.png|
+     - |surface2.9.png|
+     - |whale.png|
+     - |finance.13.png|
+   * - gnuplot script
+     - `simple.1.gnu`_
+     - `histograms.1.gnu`_
+     - `surface2.9.gnu`_
+     - `iterate.2.gnu`_
+     - `finance.13.gnu`_
+   * - py-gnuplot script
+     - `simple.1.py`_
+     - `histograms.2.py`_
+     - `surface.9.py`_
+     - `whale.py`_
+     - `finance.13.py`_
+   * - py-gnuplot quick mode
+     - `simple2.1.py`_
+     - `histograms2.2.py`_
+     - `surface2.9.py`_
+     - `whale2.py`_
+     -  N/A(too complicated)
+   * - py-gnuplot data generated in python
+     - N/A
+     - `histograms3.2.py`_
+     - N/A
+     - N/A
+     - `finance3.13.py`_
+
+.. list-table:: Table2 : examples porting from matplotlib
+   :widths: 30,30,30
+
+   * - `sphx_glr_bar_stacked_001.py`_ |sphx_glr_bar_stacked_001.png|
+     - `sphx_glr_barchart_001.py`_ |sphx_glr_barchart_001.png|
+     - `sphx_glr_axes_demo_001.py`_ |sphx_glr_axes_demo_001.png|
+   * - `sphx_glr_axes_margins_001.py`_ |sphx_glr_axes_margins_001.png|
+     - `sphx_glr_tex_demo_001.py`_ |sphx_glr_tex_demo_001.png|
+     - `sphx_glr_pie_features_0011.py`_ |sphx_glr_pie_features_0011.png|
 
-As we know, gnuplot use commands to plot all kinds of image, we port almost all
-the useful commands as functions in py-gnuplot.
+Let's see the detail.
 
-In `2.1 member functions port from Gnuplot`_ we introduce the member
-functions that we can plot all what Gnuplot could do, The limitation is
-it's not so easy to plot the python generated data with the those existing
-command.
+.. contents:: [Contents]
+   :depth: 2
 
-To plot the data generated in python, we develop additional functions as
-below, ::
+1. Introduction
+=================
 
-    plot_data(self, data, *items, **kwargs):
-    splot_data(self, data, *items, **kwargs)
+As we know, to plot a image in gnuplot we do:
 
-they are almost the same as the original plot()/splot(), the difference is
-we pass the data as the first parameter, you don't give the filename in the
-plot command, see detail in `2.2 new developed member functions for python
-generated data`_ .
+    1) Enter gnuplot conext;
+    2) Set plotting style;
+    3) Define some expressions;
+    4) Plotting.
 
-Sometime we only need simple plot and don't want to allocate a Gnuplot
-instance, we develop the quick way to plot: `2.3 new developed global
-class-less function call`_ and you can plot the image in a easy way with
-global class-less function call.
+We translate gnuplot's main function into python ones, and each one do the same
+thing as gnuplot. As in `quick_example.py`_ we also have 4 steps to plot an
+image::
 
-2.1 member functions port from Gnuplot
----------------------------------------
+    #Constructor
+    g = gnuplot.Gnuplot()
+    #Set plotting style
+    g.set()
+    #Expressions and caculations
+    g.cmd()
+    #Plotting
+    g.plot()
 
-The principle is if you can write Gnuplot script, you can write py-gnuplot.
-There is 1-1 mapping between almost all Gnuplot command and python
-function;
+1.1 constructor
+----------------
 
-2.1.1 The constructor
-+++++++++++++++++++++
+Defenition:
 
 .. code-block:: python
 
     def __init__(self, *args, log = False, **kwargs):
         '''
         *args: The flag parameter in gnuplot
         log: If print the gnuplot log
         **kwargs: the flag that need to be set. You can also set them in the set() function.
         '''
 
-When create the Gnuplot instance, you can pass some parameter to it, you
-can also set them when you call set() or plot(), they are the same.
-
-The "log" parameter is a new added flag to indicate if we print the gnuplot
-execution log when run. For example:
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-    #See original gnuplot script here:
-    #http://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.html
-    g = gnuplot.Gnuplot(log = True,
-            term = 'pngcairo size 480,480',
-            out = '"whale.png"',
-            pm3d = 'depth hidden3d ls 100',
-            cbrange = '[-0.5:0.5]',
-            palette = 'rgb -3,-3,-3',
-            colorbox = None,
-            border = None,
-            key = None,
-            zrange = '[-2:2]',
-            tics = None,
-            view = '60,185,1.5')
-    g.splot('"examples/whale.dat" w pm3d')
-
-This is the script output with the log=True::
-
-    [py-gnuplot] set term pngcairo size 480,480
-    [py-gnuplot] set out "whale.png"
-    [py-gnuplot] set pm3d depth hidden3d ls 100
-    [py-gnuplot] set cbrange [-0.5:0.5]
-    [py-gnuplot] set palette rgb -3,-3,-3
-    [py-gnuplot] unset colorbox
-    [py-gnuplot] unset border
-    [py-gnuplot] unset key
-    [py-gnuplot] set zrange [-2:2]
-    [py-gnuplot] unset tics
-    [py-gnuplot] set view 60,185,1.5
-    [py-gnuplot] splot "examples/whale.dat" w pm3d
-
-And this is the image output: |small_whale.png|
-
-.. |small_whale.png| image:: http://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.png
-   :width: 50
-
-2.1.2 cmd()
-+++++++++++
-
-.. code-block:: python
-
-    def cmd(self, *args):
-        '''
-        *args: all the line that need to pass to gnuplot. It could be a
-        list of lines, or a paragraph; Lines starting with "#" would be
-        omitted. Every line should be a clause that could be executed in
-        gnuplot.
-        '''
-
-We implemented the function cmd() and pass the command to call Gnuplot to plot
-the data, Thus we could do everything with the only one simple function:
+We call g = gnuplot.Gnuplot(log = True) to get a gnuplot context. Here log = True means to print the gnuplot log when call gnuplot functions.::
 
-.. _simple1.1.py:
-..
-    cmd2img:: python3
-    :image: simple.1.png
+    #Ceate a gnuplot context. with "log = True" to print the gnuplot execute log.
+    g = gnuplot.Gnuplot(log = True)
 
-.. code-block:: python
+1.2 Set()/unset()
+------------------
 
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-    # Illustration of object-oriented interface, you can see we only wrap the
-    # gnuplot script by g.cmd('...') and it's simple and straitfoward if you
-    # are familar with Gnuplot.
-    g = gnuplot.Gnuplot()
-    g.cmd('set terminal pngcairo font "arial,10" fontscale 1.0 size 600, 400')
-    g.cmd('set output "simple.1.png"')
-    g.cmd('set key fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid')
-    g.cmd('set samples 50, 50')
-    g.cmd('set title "Simple Plots" ')
-    g.cmd('set title  font ",20" norotate')
-    g.cmd('plot [-10:10] sin(x),atan(x),cos(atan(x))')
-
-Or you can even pass the Gnuplot command as a string list or a text paragraph:
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-    # Illustration of cmd(), you can see we only wrap the
-    # gnuplot script by g.cmd('...') and it's simple and straitfoward if you
-    # are familar with Gnuplot.
-    g = gnuplot.Gnuplot()
-
-    # Take all the Gnuplot command as a list of command:
-    g.cmd('set terminal pngcairo font "arial,10" fontscale 1.0 size 600, 400',
-    'set output "simple.1.png"',
-    'set key fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid',
-    'set samples 50, 50',
-    'set title "Simple Plots" ',
-    'set title  font ",20" norotate',
-    'plot [-10:10] sin(x),atan(x),cos(atan(x))')
-
-    # Another means, take all the Gnuplot command as a script paragraph,
-    #uncomment the following code block to have a try.
-    #plot_cmd = '''
-    #set terminal pngcairo font "arial,10" fontscale 1.0 size 600, 400
-    #set output "simple.1.png"
-    #set key fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid
-    #set samples 50, 50
-    #set title "Simple Plots
-    #set title  font ",20" norotate
-    #plot [-10:10] sin(x),atan(x),cos(atan(x))'''
-    #g.cmd(plot_cmd)
-
-This is the image output: |small_simple.png|
-
-.. |small_simple.png| image:: http://gnuplot.sourceforge.net/demo/simple.1.png
-   :width: 50
-
-By this means we can do everything that Gnuplot can do and cannot do what
-Gnuplot itself can't do. It's the exact way that the Gnuplot do it. and we
-don't get any benifit besides we can call Gnuplot in python. So we develop
-many other functions as below:
-
-2.1.3 set()
-+++++++++++
+Defenition:
 
 .. code-block:: python
 
     def set(self, *args, **kwargs):
         '''
         *args: options without value
         *kwargs: options with value. The set and unset commands may optionally
                  contain an iteration clause, so the arg could be list.
         '''
+    def unset(self, *items):
+        '''
+        *args: options that need to be unset
+        '''
 
-The set command can be used to set lots of options. The set and unset
-commands may optionally contain an iteration clause, so the arg could be
-list. For examples:
-
-We set the options before plot and then call plot to render the image. It's
-equivalent to example in `2.1.2 cmd()`_ but seems muck like a python script.
-
-.. _simple2.py:
-
-..
-    cmd2img:: python3
-    :image: simple.1.png
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
+After enter gnuplot context, normally we need to set the plotting style. For
+example we need to set the terminal and output at first in gnuplt as following::
 
-    # Gnuplot lines:
-    #set terminal pngcairo font "arial,10" fontscale 1.0 size 600, 400
-    #set output "simple.1.png"
-    #set key fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid
-    #set samples 50, 50
-    #set title "Simple Plots" font ",20" norotate
+    set terminal pngcairo  transparent enhanced font "arial,8" fontscale 1.0 size 512, 280 
+    set output 'transparent.2.png'
 
-    g = gnuplot.Gnuplot()
-    g.set(terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400',
-            output = '"simple.1.png"',
-            key = 'fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid',
-            samples = '50, 50',
-            title = '"Simple Plots" font ",20" norotate')
-    g.plot('[-10:10] sin(x),atan(x),cos(atan(x))')
-
-set() is flexible but indeed set() functions is not necessary. We could
-pass the options as parameter in the constructor and plot(). For examples
-the following script act equally with the above:
-
-.. code-block:: python
+Then we translate the set into set() function as following, please not that all
+the elment are stirng, so must add extra quoto and it would be passed to
+gnuplot without any change. Pleae note that all the parameters must be string
+since it would be passed to gnuplot without any change. You need to change them
+to string if they are not::
+
+    #Set plotting style
+    g.set(terminal = 'pngcairo transparent enhanced font "arial,8" fontscale 1.0 size 512, 280 ',
+            output = '"quick_example.png"',
+            ...
+            )
 
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
+For unset we have flexible ways to do that, for exampes the following ways are
+the same::
 
-    # py-python lines:
-    g = gnuplot.Gnuplot(terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400',
-            output = '"test.png"',
-            boxwidth = '0.9 relative',
-            style = 'fill solid 1.0',
-            label = ['"y=x" at 1,2',
-                '2 "S" at graph 0.5,0.5 center font "Symbol,24"',
-                '3 "y=x^2" at 2,3,4 right'])
-            g.plot('"file.dat" with boxes')
+    #gnuplot unset
+    unset colorbox
 
-We can also write it as the following, they are all the same:
+    #py-gnuplot means1
+    g.unset(colorbox)
 
-.. code-block:: python
+    #py-gnuplot means2
+    g.set(colorbox = None)
 
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
+    #py-gnuplot means3
+    g.set(nocolorbox = "")
 
-    # py-python lines:
-    g = gnuplot.Gnuplot()
-    g.plot('"file.dat" with boxes',
-           terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400',
-           output = '"test.png"',
-           boxwidth = '0.9 relative',
-           style = 'fill solid 1.0',
-           label = ['"y=x" at 1,2',
-                    '2 "S" at graph 0.5,0.5 center font "Symbol,24"',
-                    '3 "y=x^2" at 2,3,4 right'])
+1.3 cmd()
+----------
 
-2.1.4 unset()
-+++++++++++++++
+Defenition:
 
 .. code-block:: python
 
-    def unset(self, *items):
+    def cmd(self, *args):
         '''
-        *args: options that need to be unset
+        *args: all the line that need to pass to gnuplot. It could be a
+        list of lines, or a paragraph; Lines starting with "#" would be
+        omitted. Every line should be a clause that could be executed in
+        gnuplot.
         '''
 
-Options set using the set() function may be returned to their default state by
-the corresponding unset() function:
-
-.. code-block:: python
+Sometimes before plot we need define some variable or caculations, call cmd() functions to do::
 
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-    # py-python lines:
-    g = gnuplot.Gnuplot(terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400', output = '"test.png"')
-    g.unset('xlabel', 'ylabel', 'xrange', 'yrange')
-    g.plot('sin(x) with lp')
-
-unset command could be replaced as set, for example the above example could
-also be writen as:
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
+    #gnuplot
+    Gauss(x,mu,sigma) = 1./(sigma*sqrt(2*pi)) * exp( -(x-mu)**2 / (2*sigma**2) )
+    d1(x) = Gauss(x, 0.5, 0.5)
+    d2(x) = Gauss(x,  2.,  1.)
+    d3(x) = Gauss(x, -1.,  2.)
+
+    #py-gnuplot
+    g.cmd('Gauss(x,mu,sigma) = 1./(sigma*sqrt(2*pi)) * exp( -(x-mu)**2 / (2*sigma**2) )',
+            'd1(x) = Gauss(x, 0.5, 0.5)',
+            'd2(x) = Gauss(x,  2.,  1.)',
+            'd3(x) = Gauss(x, -1.,  2.)')
 
-    # Another means to unset options:
-    g = gnuplot.Gnuplot(terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400', output = '"test.png"')
-    g.set('noxlabel', 'noylabel', 'noxrange', 'noyrange')
-    g.plot('sin(x) with lp')
+As we see, all statement in cmd() would be translated the same statement in
+gnuplot. By this way we can execute any gnuplot statement.
 
-    # Another means to unset options:
-    g = gnuplot.Gnuplot()
-    g.set(xlabel = None,
-          ylabel = None,
-          xrange = None,
-          yrange = None)
-    g.plot('sin(x) with lp')
+1.4 plot()/splot()
+------------------
 
-2.1.5 plot()
-++++++++++++
+Definition:
 
 .. code-block:: python
 
     def plot(self, *items, **kwargs):
         '''
         *items: The list of plot command;
         **kwargs: The options that would be set before the plot command.
         '''
-
-plot is the primary command for drawing plots with gnuplot, We port it as a
-function in py-python. As description, the plot-element is passed as
-variable parameters, and options are passed as dictionary parameter. please
-be noted that the plot-element should be in the single quotes:
-
-Note that the plot()/splot() only plot the gnuplot functions and file, if
-you'd like to plot data generated in python, you should call the new added
-functions: `2.2.1 plot_data()`_ and `2.2.2 splot_data()`_ .
-
-for example plot the gnuplot function or datafile we use pygnuplot.gnuplot:
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-    g = gnuplot.Gnuplot()
-    g.plot('[-10:10] sin(x)',
-           'atan(x)',
-           'cos(atan(x))',
-           terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400',
-           output = '"simple.1.png"',
-           key = 'fixed left top vertical Right lt black linewidth 1.000 dashtype solid',
-           samples = '50, 50',
-           title = '"Simple Plots" font ",20" norotate')
-
-If we plot the python generated data we use plot_data() and splot_data():
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-    # usage examples, please note that we didn't give the output so could only
-    # see the image flash on the screen. Will introduce how to output the
-    # image to files.
-    df = pd.DataFrame(data = {'col1': [1, 2],
-                              'col2': [3, 4],
-                              'col3': [5, 6]})
-    g = gnuplot.Gnuplot()
-    g.plot_data(df, 'using 1:2 with lines', 'using 1:3 with points')
-
-As we stated in `2.1.3 set()`_ , we can use parameter to replace
-set()/unset() in plot() function, here is something we need to know when
-using parameter to replace set()/unset():
-
-1) If it's flag parameter, for example::
-
-    set grid
-    set hidden3d
-
-we can pass it as a empty value:
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-
-    # Examples of gnuplot.plot()
-    g = gnuplot.Gnuplot()
-    g.plot('sin(x)',
-           'cos(x)',
-           ...,
-           grid = '',
-           hidden3d = '',
-           ...)
-
-    # Examples of plot_data()
-    df = pd.DataFrame(data = {'col1': [1, 2],
-                              'col2': [3, 4],
-                              'col3': [5, 6]})
-    g = gnuplot.Gnuplot()
-    g.plot_data(df, 'using 1:2 with lines', 'using 1:3 with points',
-           grid = '')
-
-2) We have two means to pass "unset" command, one is the no-xxx option and
-   the other is xxx = None, for examples we'd like to unset the grid and
-   xrange::
-
-    unset grid
-    unset xrange
-
-We can do that in py-gnuplot by:
-
-.. code-block:: python
-
-    g = gnuplot.Gnuplot()
-    # Example of use no-xxx to unset the flag
-    g.plot(df, 'using 0:2:3:4:5 notitle with financebars lt 8',
-            ...,
-            nogrid = '',
-            noxlabel = '',
-            ...)
-
-    # Example of use None to unset the flag
-    g.plot(df, 'using 0:2:3:4:5 notitle with financebars lt 8',
-            ...,
-            grid = None,
-            xlabel = None,
-            ...)
-
-3) If there is multiple lines for one options, for exampe in gnuplot it
-   is::
-
-    set arrow from 5,-5,-1.2 to 5,5,-1.2 lt -1
-    set arrow from 5,6,-1 to 5,5,-1 lt -1
-    set arrow from 5,6,sinc(5,5) to 5,5,sinc(5,5) lt -1
-
-We pass them by a list of options:
-
-.. code-block:: python
-
-    g = gnuplot.Gnuplot()
-    g.plot(df,
-           'using 0:2:3:4:5 notitle with financebars lt 8',
-           ...,
-           arrow = ['from 5,-5,-1.2 to 5,5,-1.2 lt -1',
-                    'from 5,6,-1 to 5,5,-1 lt -1',
-                    'from 5,6,sinc(5,5) to 5,5,sinc(5,5) lt -1'],
-           ...,
-           ...)
-
-2.1.6 splot()
-+++++++++++++
-
-.. code-block:: python
-
     def splot(self, *items, **kwargs):
         '''
         *items: The list of plot command;
         **kwargs: The options that would be set before the plot command.
         '''
 
-The usage of splot() is exactly the same as plot().
+Every plot/splot command would be a parameter in plot()/splot() functions. Like
+set()/unset(), all the parameters must be string since it would be pas sed to
+gnuplot without any change. You need to change them to string if they are not::
+
+    #gnplot
+    plot d1(x) fs solid 1.0 lc rgb "forest-green" title "μ =  0.5 σ = 0.5", \
+     d2(x) lc rgb "gold" title "μ =  2.0 σ = 1.0", \
+     d3(x) lc rgb "dark-violet" title "μ = -1.0 σ = 2.0"
+
+    #py-gnplot
+    g.plot('d1(x) fs solid 1.0 lc rgb "forest-green" title "μ =  0.5 σ = 0.5"',
+            'd2(x) lc rgb "gold" title "μ =  2.0 σ = 1.0"',
+            'd3(x) lc rgb "dark-violet" title "μ = -1.0 σ = 2.0"')
 
-2.2 new developed member functions for python generated data
---------------------------------------------------------------
+1.5 plot_data()/splot_data()
+--------------------------------------
 
-We develop the following memember functions, they are very familar with the
-orignal plot() and splot(), the only difference is that , in the new
-developed function, we pass the python generated data as the first
-parameter and remove the corresponding element in the plot command.
+.. Note:: in older release, they are called plot_data()/splot_data(), I'd like to chnage them to the new name since they are more intuitive.
 
-2.2.1 plot_data()
-+++++++++++++++++
+Definition:
 
 .. code-block:: python
 
     def plot_data(self, data, *items, **kwargs):
         '''
         data: The data that need to be plotted. It's either the string of list
         or the Pnadas Dataframe, if it's Pnadas Dataframe it would be converted
         to string by data.to_csv(). Note that we will execut a extra command
         "set datafile separator "," to fit the data format of csv.
         *items: The list of plot command;
         **kwargs: The options that would be set before the plot command.
         '''
-
-The usage is the same as in `2.1.5 plot()`_ except that you should pass the
-data(string or pandas Dataframe format) as the first parameter, and remove
-the corresponding filename in every plot line. Moreover, the defaulst
-seperator now is "," for easy use with csv file:
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-    # usage examples, please note that we didn't give the output so could only
-    # see the image flash on the screen. Will introduce how to output the
-    # image to files.
-    df = pd.DataFrame(data = {'col1': [1, 2],
-                              'col2': [3, 4],
-                              'col3': [5, 6]})
-    g = gnuplot.Gnuplot()
-    # Note that the first parameter is df and there is no "data.file" in
-    # the following commmand.
-    g.plot_data(df,
-                'using 1:2 with lines',
-                'using 1:3 with points')
-
-2.2.2 splot_data()
-++++++++++++++++++
-
-.. code-block:: python
-
     def splot_data(self, data, *items, **kwargs):
         '''
         data: The data that need to be plotted. It's either the string of list
         or the Pnadas Dataframe, if it's Pnadas Dataframe it would be converted
         to string by data.to_csv(). Note that we will execut a extra command
         "set datafile separator "," to fit the data format of csv.
         *items: The list of plot command;
         **kwargs: The options that would be set before the plot command.
         '''
 
-The usage is the same as in `2.2.1 plot_data()`_ .
+With above functions: constructor, Set()/unset(), plot()/splot(), we can do
+what gnuplot do, but it cannot plot python generated data. It's hard to
+implement the new functions with the existing gnuplot command, so we develop
+two new functions: plot_data()/splot_data(). They are much like
+plot()/splot(), the only difference is:
+
+    * plot()/splot() take function(filename) in every plot command.
+    * plot_data()/splot_data() take the dataframe as the first
+      parameter, while remove function(filename) in every plot commmand
+
+for examples::
+
+    #plot(): 'finance.dat' is in plot command
+    g.plot("'finance.dat' using 0:($6/10000) notitle with impulses lt 3",
+           "'finance.dat' using 0:($7/10000) notitle with lines lt 1")
 
-2.3 new developed global class-less function call
-----------------------------------------------------
+    #plot_data(): the first parameter must be dataframe, every plot
+    #command doesn't take the data.
+    g.plot_data(df,
+            'using 0:($6/10000) notitle with impulses lt 3',
+            'using 0:($7/10000) notitle with lines lt 1')
 
-We can plot the image just by the above object-oriented interface, but
-sometimes we want to quick plot an image in quick mode, we can call the
-global class-less function call:
+See `histograms.2.py`_ and `histograms.2.py`_ for differences.
 
-2.3.1 plot()
-++++++++++++
+1.6 multiplot
+------------------
 
-.. code-block:: python
+To plot multiplot, you must set multiplot at first as in gnuplot. Here is examples.
 
-    #submodule gnuplot
-    def plot(*args, **kwargs):
-        '''
-        *items: The list of plot command;
-        **kwargs: The options that would be set before the plot command.
-        '''
+1.7 quick mode
+------------------
 
-The usage is the same as in `2.1.5 plot()`_ except that you needn't
-allocate a Gnuplot() instance at first:.
+For some easy case, we can combine the following step into one.
 
-.. _simple3.py:
+    1) Enter gnuplot conext;
+    2) Set plotting style;
+    3) Define some expressions;
+    4) Plotting.
 
-..
-    cmd2img:: python3
-    :image: simple.1.png
+For examples:
 
+.. _simple2.1.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
 
     gnuplot.plot('[-10:10] sin(x)',
            'atan(x)',
            'cos(atan(x))',
            terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400',
            output = '"simple.1.png"',
-           key = 'fixed left top vertical Right lt black linewidth 1.000 dashtype solid',
+           key = 'fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid',
            samples = '50, 50',
-           title = '"Simple Plots" font ",20" norotate')
-
-2.3.2 splot()
-++++++++++++++
-
-.. code-block:: python
-
-    #submodule gnuplot
-    def splot(*args, **kwargs):
-        '''
-        *items: The list of plot command;
-        **kwargs: The options that would be set before the plot command.
-        '''
-
-The usage is the same as in `2.1.6 splot()`_ except that you needn't
-allocate a Gnuplot() instance at first:
-
-2.3.3 plot_data()
-+++++++++++++++++
-
-.. code-block:: python
-
-    def plot_data(data, *items, **kwargs):
-        '''
-        data: The data that need to be plotted. It's either the string of list
-        or the Pnadas Dataframe, if it's Pnadas Dataframe it would be converted
-        to string by data.to_csv()
-        *items: The list of plot command;
-        **kwargs: The options that would be set before the plot command.
-        '''
-
-The usage is the same as in `2.2.1 plot_data()`_ except that you needn't
-allocate a Gnuplot() instance at first:
+           title = '"Simple Plots" font ",20" textcolor lt -1 norotate',
+           xrange = '[ * : * ] noreverse writeback',
+           x2range = '[ * : * ] noreverse writeback',
+           yrange = '[ * : * ] noreverse writeback',
+           y2range = '[ * : * ] noreverse writeback',
+           zrange = '[ * : * ] noreverse writeback',
+           cbrange = '[ * : * ] noreverse writeback',
+           rrange = '[ * : * ] noreverse writeback',
+           colorbox = 'vertical origin screen 0.9, 0.2 size screen 0.05, 0.6 front noinvert bdefault')
 
+.. _whale2.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
+    import pandas as pd
 
-    df = pd.DataFrame(data = {'col1': [1, 2],
-                              'col2': [3, 4],
-                              'col3': [5, 6]})
-    gnuplot.plot_data(df,
-                      'using 1:2 with lines',
-                      'using 1:3 with points')
-
-2.3.4 splot_data()
-++++++++++++++++++
-
-.. code-block:: python
-
-    class gnuplot.Gnuplot(object):
-
-        def splot(self, *items, **kwargs):
-            '''
-            *items: The list of plot command;
-            **kwargs: The options that would be set before the plot command.
-            '''
-
-The usage is the same as in `2.2.2 splot_data()`_ except that you needn't
-allocate a Gnuplot() instance at first:
-
-2.3.5 multiplot()
-+++++++++++++++++
-
-Since we don't allocate the Gnuplot instance, there is a little trick to
-plot the multiplot image. To solve the issue we create 3 brand new function
-to implement that.
-
-.. code-block:: python
-
-    def multiplot(\*args, \*\*kwargs):
-        @args: the subplot object list;
-        @kwargs: the setting options that need to be set before call plot;
-
-    def make_plot(\*args, \*\*kwargs)
-        The parameter definition is the same as plot(), but it doesn't plot
-        the data really, it only return the plot dictionary for later
-        multiplot() use.
-
-    def make_splot(\*args, \*\*kwargs)
-        The parameter definition is the same as splot(), but it doesn't plot
-        the data really, it only return the plot dictionary for later
-        multiplot() use.
-
-    def make_plot_data (data, \*args, \*\*kwargs)
-        The parameter definition is the same as plot_data(), but it doesn't
-        plot the data really, it only return the plot dictionary for later
-        multiplot() use.
-
-    def make_splot_data (data, \*args, \*\*kwargs)
-        The parameter definition is the same as splot_data(), but it
-        doesn't plot the data really, it only return the plot dictionary
-        for later multiplot() use.
-
-Before call multiplot() we must generate the subplot object by calling
-make_plot()/make_splot(), It is much like mplfinance.make_addplot(), it only
-add the subplot command for further call:
+    #https://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.html
+    gnuplot.splot('"examples/whale.dat" w pm3d',
+            term = 'pngcairo size 480,480',
+            out = '"whale.png"',
+            style = 'line 100 lw 0.1 lc "black"',
+            pm3d = 'depth hidden3d ls 100',
+            cbrange = '[-0.5:0.5]',
+            palette = 'rgb -3,-3,-3',
+            colorbox = None,
+            border = None,
+            key = None,
+            zrange = '[-2:2]',
+            tics = None,
+            view = '60,185,1.5')
 
+.. _histograms2.2.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
+    import pandas as pd
 
-    sub1 = gnuplot.make_plot('sin(x)', ylabel = 'ylabel')
-    sub2 = gnuplot.make_plot('cos(x)', xlabel = 'xlabel')
-    sub3 = gnuplot.make_plot('sin(2*x)', noxlabel = '', ylabel = '')
-    sub4 = gnuplot.make_plot('cos(2*x)', xlabel = 'xlabel')
-    gnuplot.multiplot(sub1, sub2, sub3, sub4,
-                      output = '"sample.multiplot.png"',
-                      term = 'pngcairo size 900,600 font ",11"',
-                      multiplot  = 'layout 2,2 columnsfirst margins 0.1,0.9,0.1,0.9 spacing 0.1')
-
-A example in reality:
-
-.. _finance2.py:
-
-..
-    cmd2img:: python3
-    :image: finance.13.png
+    df = pd.read_csv('examples/immigration.dat', index_col = 0, sep='\t', comment='#')
+    gnuplot.plot_data(df,
+            'using 2:xtic(1), for [i=3:22] "" using i ',
+            terminal = 'pngcairo transparent enhanced font "arial,10" fontscale 1.0 size 600, 400 ',
+            output = '"histograms.1.png"',
+            key = 'fixed right top vertical Right noreverse noenhanced autotitle nobox',
+            style = 'data linespoints',
+            datafile = ' missing "-"',
+            xtics = 'border in scale 1,0.5 nomirror rotate by -45 autojustify norangelimit',
+            title = '"US immigration from Europe by decade"')
 
+.. _surface2.9.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
-    import pandas as pd
-
-    # A demostration to generate pandas data frame data in python.
-    df = pd.read_csv('examples/finance.dat',
-            sep='\t',
-            index_col = 0,
-            parse_dates = True,
-            names = ['date', 'open','high','low','close', 'volume','volume_m50',
-                'intensity','close_ma20','upper','lower '])
-
-    # make subplot at first, now there is still no real plot.
-    sub1 = gnuplot.make_plot_data(df,
-            'using 0:2:3:4:5 notitle with candlesticks lt 8',
-            'using 0:9 notitle with lines lt 3',
-            'using 0:10 notitle with lines lt 1',
-            'using 0:11 notitle with lines lt 2',
-            'using 0:8 axes x1y2 notitle with lines lt 4',
-            title = '"Change to candlesticks"',
-            logscale = 'y',
-            xrange = '[50:253]',
-            yrange = '[75:105]',
-            format = 'x ""',
-            xtics = '(66, 87, 109, 130, 151, 174, 193, 215, 235)',
-            ytics = '(105, 100, 95, 90, 85, 80)',
-            lmargin = '9',
-            rmargin = '2',
-            bmargin = '0',
-            origin = '0, 0.3',
-            size = ' 1, 0.7',
-            grid = 'xtics ytics',
-            ylabel = '"price" offset 1',
-            label = ['1 "Acme Widgets" at graph 0.5, graph 0.9 center front',
-                '2 "Courtesy of Bollinger Capital" at graph 0.01, 0.07',
-                '3 "  www.BollingerBands.com" at graph 0.01, 0.03']
-            )
 
-    sub2 = gnuplot.make_plot_data(df,
-            'using 0:($6/10000) notitle with impulses lt 3',
-            'using 0:($7/10000) notitle with lines lt 1',
-            ytics = '500',
-            xtics = '("6/03" 66, "7/03" 87, "8/03" 109, "9/03" 130, "10/03" 151, "11/03" 174, "12/03" 193, "1/04" 215, "2/04" 235)',
-            ylabel = '"volume (0000)" offset 1',
-            nologscale = 'y',
-            autoscale = 'y',
-            size = '1.0, 0.3',
-            origin = '0.0, 0.0',
-            bmargin = '',
-            tmargin = '0',
-            format = ['x', 'y "%1.0f"'])
+    #py-gnuplot: https://gnuplot.sourceforge.net/demo/surface2.9.gnu
+    gnuplot.splot('cos(u)+.5*cos(u)*cos(v),sin(u)+.5*sin(u)*cos(v),.5*sin(v) with lines',
+            '1+cos(u)+.5*cos(u)*cos(v),.5*sin(v),sin(u)+.5*sin(u)*cos(v) with lines',
+            terminal = 'pngcairo enhanced font "arial,10" fontscale 1.0 size 600, 400 ',
+            output = '"surface2.9.png"',
+            dummy = 'u, v',
+            key = 'bmargin center horizontal Right noreverse enhanced autotitle nobox',
+            style = ['data lines'],
+            parametric = '',
+            view = '50, 30, 1, 1',
+            isosamples = '50, 20',
+            hidden3d = 'back offset 1 trianglepattern 3 undefined 1 altdiagonal bentover',
+            xyplane = 'relative 0',
+            title = '"Interlocking Tori" ',
+            urange = '[ -3.14159 : 3.14159 ] noreverse nowriteback',
+            vrange = '[ -3.14159 : 3.14159 ] noreverse nowriteback')
 
-    # plot at one time.
-    gnuplot.multiplot(sub1, sub2,
-            output = '"finance.13.png"',
-            term = 'pngcairo font "arial,10" fontscale 1.0 size 900, 600')
+2. Examples
+=============
 
-.. _3 Multiplot Axes Demo2:
+2.1 plot/splot function
+-------------------------------
 
+.. _simple.1.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
-    import pandas as pd
-    import numpy as np
-
-    #https://matplotlib.org/gallery/subplots_axes_and_figures/axes_demo.html#sphx-glr-gallery-subplots-axes-and-figures-axes-demo-py
-    #http://gnuplot.sourceforge.net/demo_5.2/bins.html
-
-    # 1) create some data to use for the plot
-    np.random.seed(19680801) # Fixing random state for reproducibility
-    dt = 0.001
-    t = np.arange(0.0, 10.0, dt)
-    r = np.exp(-t / 0.05)  # impulse response
-    x = np.random.randn(len(t))
-    s = np.convolve(x, r)[:len(x)] * dt  # colored noise
-    df = pd.DataFrame({'r': r, 'x': x, 's': s}, index = t)
-    df.index.name = 't'
-    #print(df.tail().to_csv())
-
-    # 2) Plot the data
-    main = gnuplot.make_plot_data(df.iloc[:1000],
-            'using 1:4 with line lw 2 lc "web-blue"',
-            title = '"Gaussian colored noise"',
-            xlabel = '"time (s)"',
-            ylabel = '"current (nA)"',
-            xrange = '[0:1]',
-            yrange = '[-0.015:0.03]',
-            key = None,
-            size = ' 1, 1',
-            origin = '0, 0')
-    right = gnuplot.make_plot_data(df,
-            'using 4 bins=400 with boxes title "20 bins" lw 2 lc "web-blue"',
-            title = '"Probability"',
-            xlabel = None,
-            ylabel = None,
-            tics = None,
-            xrange = None,
-            yrange = None,
-            origin = '0.65, 0.56',
-            size = '0.24, 0.32',
-            object = 'rectangle from graph 0,0 to graph 1,1 behind fc "black" fillstyle solid 1.0')
-    left = gnuplot.make_plot_data(df,
-            'using 1:2 with line lw 2 lc "web-blue"',
-            title = '"Impulse response"',
-            xrange = '[0:0.2]',
-            origin = '0.15, 0.56',
-            size = '0.24, 0.32')
 
-    gnuplot.multiplot(main, right, left,
-            output = '"sphx_glr_axes_demo_001.png"',
-            term = 'pngcairo font "arial,10" fontscale 1.0 size 640, 480',
-            key = '')
+    #py-gnuplot: https://gnuplot.sourceforge.net/demo_6.0/simple.html
 
-3. examples
-============
+    #Ceate a gnuplot context. with "log = True" to print the gnuplot execute log.
+    g = gnuplot.Gnuplot(log = True)
 
-3.1 examples port from gnuplot
-------------------------------
+    #Set plotting style
+    g.set(terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400',
+           output = '"simple.1.png"',
+           key = 'fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid',
+           samples = '50, 50',
+           title = '"Simple Plots" font ",20" textcolor lt -1 norotate',
+           xrange = '[ * : * ] noreverse writeback',
+           x2range = '[ * : * ] noreverse writeback',
+           yrange = '[ * : * ] noreverse writeback',
+           y2range = '[ * : * ] noreverse writeback',
+           zrange = '[ * : * ] noreverse writeback',
+           cbrange = '[ * : * ] noreverse writeback',
+           rrange = '[ * : * ] noreverse writeback',
+           colorbox = 'vertical origin screen 0.9, 0.2 size screen 0.05, 0.6 front  noinvert bdefault')
 
-3.1.1 finance
-+++++++++++++
+    #Expressions and caculations
+    g.cmd("NO_ANIMATION = 1")
 
-example with object-oriented interface call:
+    #Plotting
+    g.plot("[-10:10] sin(x)", "atan(x)", "cos(atan(x))")
 
-.. _finance1.py:
+This is the output: 
 
-..
-    cmd2img:: python3
-    :image: finance.13.png
+|simple.1.png|
 
+.. _surface.9.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
-    import pandas as pd
-
-    # A demostration to generate pandas data frame data in python.
-    df = pd.read_csv('examples/finance.dat',
-            sep='\t',
-            index_col = 0,
-            parse_dates = True,
-            names = ['date', 'open','high','low','close', 'volume','volume_m50',
-                'intensity','close_ma20','upper','lower '])
-
-    # Create a Gnuplot instance and set the options at first;
-    g = gnuplot.Gnuplot(log = True,
-            output = '"finance.13.png"',
-            term = 'pngcairo font "arial,10" fontscale 1.0 size 900, 600',
-            multiplot = True)
-
-    g.plot_data(df,
-            'using 0:2:3:4:5 notitle with candlesticks lt 8',
-            'using 0:9 notitle with lines lt 3',
-            'using 0:10 notitle with lines lt 1',
-            'using 0:11 notitle with lines lt 2',
-            'using 0:8 axes x1y2 notitle with lines lt 4',
-            title = '"Change to candlesticks"',
-            logscale = 'y',
-            xrange = '[50:253]',
-            yrange = '[75:105]',
-            format = 'x ""',
-            xtics = '(66, 87, 109, 130, 151, 174, 193, 215, 235)',
-            ytics = '(105, 100, 95, 90, 85, 80)',
-            lmargin = '9',
-            rmargin = '2',
-            bmargin = '0',
-            origin = '0, 0.3',
-            size = ' 1, 0.7',
-            grid = 'xtics ytics',
-            ylabel = '"price" offset 1',
-            label = ['1 "Acme Widgets" at graph 0.5, graph 0.9 center front',
-                '2 "Courtesy of Bollinger Capital" at graph 0.01, 0.07',
-                '3 "  www.BollingerBands.com" at graph 0.01, 0.03'],
-            )
 
-    g.plot_data(df,
-            'using 0:($6/10000) notitle with impulses lt 3',
-            'using 0:($7/10000) notitle with lines lt 1',
-            bmargin = '',
-            size = '1.0, 0.3',
-            origin = '0.0, 0.0',
-            tmargin = '0',
-            nologscale = 'y',
-            autoscale = 'y',
-            format = ['x', 'y "%1.0f"'],
-            ytics = '500',
-            xtics = '("6/03" 66, "7/03" 87, "8/03" 109, "9/03" 130, "10/03" 151, "11/03" 174, "12/03" 193, "1/04" 215, "2/04" 235)',
-            ylabel = '"volume (0000)" offset 1')
-
-Since it enable the log options, I attach the execution log as below::
+    #py-gnuplot: https://gnuplot.sourceforge.net/demo_6.0/simple.html
 
-    [py-gnuplot 19:35:26] set output "finance.13.png"
-    [py-gnuplot 19:35:26] set term pngcairo font "arial,10" fontscale 1.0 size 900, 600
-    [py-gnuplot 19:35:26] set multiplot
-    [py-gnuplot 19:35:26] set datafile separator ","
-    [py-gnuplot 19:35:26] set title "Change to candlesticks"
-    [py-gnuplot 19:35:26] set logscale y
-    [py-gnuplot 19:35:26] set xrange [50:253]
-    [py-gnuplot 19:35:26] set yrange [75:105]
-    [py-gnuplot 19:35:26] set format x ""
-    [py-gnuplot 19:35:26] set xtics (66, 87, 109, 130, 151, 174, 193, 215, 235)
-    [py-gnuplot 19:35:26] set ytics (105, 100, 95, 90, 85, 80)
-    [py-gnuplot 19:35:26] set lmargin 9
-    [py-gnuplot 19:35:26] set rmargin 2
-    [py-gnuplot 19:35:26] set bmargin 0
-    [py-gnuplot 19:35:26] set origin 0, 0.3
-    [py-gnuplot 19:35:26] set size  1, 0.7
-    [py-gnuplot 19:35:26] set grid xtics ytics
-    [py-gnuplot 19:35:26] set ylabel "price" offset 1
-    [py-gnuplot 19:35:26] set label 1 "Acme Widgets" at graph 0.5, graph 0.9 center front
-    [py-gnuplot 19:35:26] set label 2 "Courtesy of Bollinger Capital" at graph 0.01, 0.07
-    [py-gnuplot 19:35:26] set label 3 "  www.BollingerBands.com" at graph 0.01, 0.03
-    [py-gnuplot 19:35:26] plot $DataFrame using 0:2:3:4:5 notitle with candlesticks lt 8,\
-    [py-gnuplot 19:35:26] $DataFrame using 0:9 notitle with lines lt 3,\
-    [py-gnuplot 19:35:26] $DataFrame using 0:10 notitle with lines lt 1,\
-    [py-gnuplot 19:35:26] $DataFrame using 0:11 notitle with lines lt 2,\
-    [py-gnuplot 19:35:26] $DataFrame using 0:8 axes x1y2 notitle with lines lt 4
-    [py-gnuplot 19:35:26] unset for [i=1:200] label i
-    [py-gnuplot 19:35:26] set datafile separator ","
-    [py-gnuplot 19:35:26] set bmargin
-    [py-gnuplot 19:35:26] set size 1.0, 0.3
-    [py-gnuplot 19:35:26] set origin 0.0, 0.0
-    [py-gnuplot 19:35:26] set tmargin 0
-    [py-gnuplot 19:35:26] set nologscale y
-    [py-gnuplot 19:35:26] set autoscale y
-    [py-gnuplot 19:35:26] set format x
-    [py-gnuplot 19:35:26] set format y "%1.0f"
-    [py-gnuplot 19:35:26] set ytics 500
-    [py-gnuplot 19:35:26] set xtics ("6/03" 66, "7/03" 87, "8/03" 109, "9/03" 130, "10/03" 151, "11/03" 174, "12/03" 193, "1/04" 215, "2/04" 235)
-    [py-gnuplot 19:35:26] set ylabel "volume (0000)" offset 1
-    [py-gnuplot 19:35:26] plot $DataFrame using 0:($6/10000) notitle with impulses lt 3,\
-    [py-gnuplot 19:35:26] $DataFrame using 0:($7/10000) notitle with lines lt 1
-    [py-gnuplot 19:35:26] unset for [i=1:200] label i
+    #Ceate a gnuplot context. with "log = True" to print the gnuplot execute log.
+    g = gnuplot.Gnuplot(log = True)
 
-And the generated output is as following:
+    #Set plotting style
+    g.set(terminal = 'pngcairo  transparent enhanced font "arial,10" fontscale 1.0 size 600, 400',
+            output = "'surface2.9.png'",
+            dummy = 'u, v',
+            key = 'bmargin center horizontal Right noreverse enhanced autotitle nobox',
+            parametric = '',
+            view = '50, 30, 1, 1',
+            isosamples = '50, 20',
+            hidden3d = 'back offset 1 trianglepattern 3 undefined 1 altdiagonal bentover',
+            style = ['data lines'],
+            xyplane = 'relative 0',
+            title = '"Interlocking Tori" ',
+            urange = '[ -3.14159 : 3.14159 ] noreverse nowriteback',
+            vrange = '[ -3.14159 : 3.14159 ] noreverse nowriteback',
+            colorbox = 'vertical origin screen 0.9, 0.2 size screen 0.05, 0.6 front  noinvert bdefault')
 
-.. image:: http://gnuplot.sourceforge.net/demo/finance.13.png
-   :width: 350
+    #Expressions and caculations
+    g.cmd("NO_ANIMATION = 1")
 
-3.1.2 histogram
-+++++++++++++++
+    #Plotting
+    g.splot("cos(u)+.5*cos(u)*cos(v)",
+            "sin(u)+.5*sin(u)*cos(v)",
+            ".5*sin(v) with lines",
+            "1+cos(u)+.5*cos(u)*cos(v)",
+            ".5*sin(v),sin(u)+.5*sin(u)*cos(v) with lines",
+            )
 
-.. _histo.1.py:
+This is the output: 
 
-..
-    cmd2img:: python3
-    :image: histograms.1.png
+|surface2.9.png|
 
-Plot with member functions:
+2.2 plot/splot file
+-------------------------------
 
+.. _histograms.2.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
 
-    df = pd.read_csv('examples/immigration.dat', index_col = 0, sep='\t', comment='#')
-    g = gnuplot.Gnuplot()
-    g.set(terminal = 'pngcairo transparent enhanced font "arial,10" fontscale 1.0 size 600, 400 ',
-            output = '"histograms.1.png"',
-            key = 'fixed right top vertical Right noreverse noenhanced autotitle nobox',
-            style = 'data linespoints',
-            datafile = ' missing "-"',
-            xtics = 'border in scale 1,0.5 nomirror rotate by -45 autojustify norangelimit',
-            title = '"US immigration from Europe by decade"')
-    g.plot_data(df, 'using 2:xtic(1), for [i=3:22] "" using i ')
-
-Since it's simple, we can plot it quick way:
-
-.. _histo.2.py:
-
-..
-    cmd2img:: python3
-    :image: histograms.1.png
+    #Histograms demo example comes from
+    #https://gnuplot.sourceforge.net/demo_6.0/histograms.2.gnu
 
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-    import pandas as pd
+    #1) Ceate a gnuplot context
+    g = gnuplot.Gnuplot(log = True)
 
-    df = pd.read_csv('examples/immigration.dat', index_col = 0, sep='\t', comment='#')
-    gnuplot.plot_data(df,
-            'using 2:xtic(1), for [i=3:22] "" using i ',
-            terminal = 'pngcairo transparent enhanced font "arial,10" fontscale 1.0 size 600, 400 ',
-            output = '"histograms.1.png"',
+    #2) Set plotting style
+    g.set(terminal = 'pngcairo  transparent enhanced font "arial,10" fontscale 1.0 size 600, 400',
+            output = "'histograms.2.png'",
+            boxwidth = '0.9 absolute',
+            style = ['fill   solid 1.00 border lt -1',
+                'histogram clustered gap 1 title textcolor lt -1',
+                'data histograms' ],
             key = 'fixed right top vertical Right noreverse noenhanced autotitle nobox',
-            style = 'data linespoints',
-            datafile = ' missing "-"',
-            xtics = 'border in scale 1,0.5 nomirror rotate by -45 autojustify norangelimit',
-            title = '"US immigration from Europe by decade"')
+            datafile = "missing '-'",
+            xtics = ["border in scale 0,0 nomirror rotate by -45  autojustify",
+                "norangelimit ",
+                " ()"],
+            title = '"US immigration from Northern Europe\\nPlot selected data columns as histogram of clustered boxes"',
+            xrange = '[ * : * ] noreverse writeback',
+            x2range = '[ * : * ] noreverse writeback',
+            yrange  = '[ 0.00000 : 300000. ] noreverse writeback',
+            y2range = '[ * : * ] noreverse writeback',
+            zrange = '[ * : * ] noreverse writeback',
+            cbrange = '[ * : * ] noreverse writeback',
+            rrange = '[ * : * ] noreverse writeback',
+            colorbox = 'vertical origin screen 0.9, 0.2 size screen 0.05, 0.6 front  noinvert bdefault')
 
-And the generated output is as following:
+    #3) Expressions and caculations
+    g.cmd("NO_ANIMATION = 1")
 
-.. image:: http://gnuplot.sourceforge.net/demo/histograms.1.png
-   :width: 350
+    #4) Plotting
+    g.plot("'examples/immigration.dat' using 6:xtic(1) ti col",
+            "'' u 12 ti col",
+            "'' u 13 ti col",
+            "'' u 14 ti col")
 
-3.1.3 splot
-+++++++++++
+This is the output: 
 
-.. _surface1.py:
+|histograms.2.png|
 
-..
-    cmd2img:: python3
-    :image: surface2.9.png
-
-object-oriented function call:
+Another example is to splot a pm3d image:
 
+.. _whale.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
 
-    g = gnuplot.Gnuplot(output = '"surface2.9.png"',
-            terminal = 'pngcairo enhanced font "arial,10" fontscale 1.0 size 600, 400 ',
-            title = '"Interlocking Tori" ',
-            dummy = 'u, v',
-            key = 'bmargin center horizontal Right noreverse enhanced autotitle nobox',
-            style = ['increment default','data lines'],
-            parametric = '',
-            view = '50, 30, 1, 1',
-            isosamples = '50, 20',
-            hidden3d = 'back offset 1 trianglepattern 3 undefined 1 altdiagonal bentover',
-            xyplane = 'relative 0',
-            urange = '[ -3.14159 : 3.14159 ] noreverse nowriteback',
-            vrange = '[ -3.14159 : 3.14159 ] noreverse nowriteback')
-    g.splot('cos(u)+.5*cos(u)*cos(v),sin(u)+.5*sin(u)*cos(v),.5*sin(v) with lines',
-            '1+cos(u)+.5*cos(u)*cos(v),.5*sin(v),sin(u)+.5*sin(u)*cos(v) with lines')
+    #Whale example comes from
+    #https://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.html
 
-.. _surface2.py:
+    #Ceate a gnuplot context
+    g = gnuplot.Gnuplot(log = True)
 
-Direct function call example:
+    #Set plotting style
+    g.set(term = 'pngcairo size 480,480',
+            output = '"whale.png"',
+            style = 'line 100 lw 0.1 lc "black"',
+            pm3d = 'depth hidden3d ls 100',
+            cbrange = '[-0.5:0.5]',
+            palette = 'rgb -3,-3,-3',
+            colorbox = None,
+            border   = None,
+            key = None,
+            zrange = '[-2:2]',
+            tics  = None,
+            view = '60,185,1.5')
 
-..
-    cmd2img:: python3
-    :image: surface2.9.png
+    #No Expressions
 
+    #Plotting
+    g.splot('"examples/whale.dat" w pm3d')
+
+The generated image is as below:
+
+|whale.png|
+
+2.3 plot/splot python generated data
+----------------------------------------------
+
+.. _histograms3.2.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
+    import pandas as pd
 
-    gnuplot.splot('cos(u)+.5*cos(u)*cos(v),sin(u)+.5*sin(u)*cos(v),.5*sin(v) with lines',
-            '1+cos(u)+.5*cos(u)*cos(v),.5*sin(v),sin(u)+.5*sin(u)*cos(v) with lines',
-            terminal = 'pngcairo enhanced font "arial,10" fontscale 1.0 size 600, 400 ',
-            output = '"surface2.9.png"',
-            dummy = 'u, v',
-            key = 'bmargin center horizontal Right noreverse enhanced autotitle nobox',
-            style = ['data lines'],
-            parametric = '',
-            view = '50, 30, 1, 1',
-            isosamples = '50, 20',
-            hidden3d = 'back offset 1 trianglepattern 3 undefined 1 altdiagonal bentover',
-            xyplane = 'relative 0',
-            title = '"Interlocking Tori" ',
-            urange = '[ -3.14159 : 3.14159 ] noreverse nowriteback',
-            vrange = '[ -3.14159 : 3.14159 ] noreverse nowriteback')
+    #Histograms demo example comes from
+    #https://gnuplot.sourceforge.net/demo_6.0/histograms.2.gnu
 
-And the generated output is as following:
+    #1) Ceate a gnuplot context
+    g = gnuplot.Gnuplot(log = True)
 
-.. image:: http://gnuplot.sourceforge.net/demo/surface2.9.png
-   :width: 350
+    #2) Set plotting style
+    g.set(terminal = 'pngcairo  transparent enhanced font "arial,10" fontscale 1.0 size 600, 400',
+            output = "'histograms.2.png'",
+            boxwidth = '0.9 absolute',
+            style = ['fill   solid 1.00 border lt -1',
+                'histogram clustered gap 1 title textcolor lt -1',
+                'data histograms' ],
+            key = 'fixed right top vertical Right noreverse noenhanced autotitle nobox',
+            datafile = "missing '-'",
+            xtics = ["border in scale 0,0 nomirror rotate by -45  autojustify",
+                "norangelimit ",
+                " ()"],
+            title = '"US immigration from Northern Europe\\nPlot selected data columns as histogram of clustered boxes"',
+            xrange = '[ * : * ] noreverse writeback',
+            x2range = '[ * : * ] noreverse writeback',
+            yrange  = '[ 0.00000 : 300000. ] noreverse writeback',
+            y2range = '[ * : * ] noreverse writeback',
+            zrange = '[ * : * ] noreverse writeback',
+            cbrange = '[ * : * ] noreverse writeback',
+            rrange = '[ * : * ] noreverse writeback',
+            colorbox = 'vertical origin screen 0.9, 0.2 size screen 0.05, 0.6 front  noinvert bdefault')
+
+    #3) Expressions and caculations
+    g.cmd("NO_ANIMATION = 1")
+    #The original example is plotting file, it's easy. To demonstrate plotting
+    #data generated in python, we transform the data into df for demonstration.
+    df = pd.read_csv('examples/immigration.dat', index_col = 0, sep='\t', comment='#')
 
-3.1.4 pm3d
-++++++++++
+    #4) Plotting
+    g.plot_data(df,
+            'using 6:xtic(1) ti col',
+            'u 12 ti col',
+            'u 13 ti col',
+            'u 14 ti col')
 
-iterate.dem
+The generated image is as below:
 
-.. _whale1.py:
+|histograms.2.png|
 
-..
-    cmd2img:: python3
-    :image: whale.png
+2.4 multiplot examples
+------------------------------
 
+.. _finance.13.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
+    import pandas as pd
 
-    #http://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.html
-    g = gnuplot.Gnuplot()
-    # Black and white version
-    g.splot('"examples/whale.dat" w pm3d',
-            term = 'pngcairo size 480,480',
-            out = '"whale.png"',
-            style = 'line 100 lw 0.1 lc "black"',
-            pm3d = 'depth hidden3d ls 100',
-            cbrange = '[-0.5:0.5]',
-            palette = 'rgb -3,-3,-3',
-            colorbox = None,
-            border = None,
-            key = None,
-            zrange = '[-2:2]',
-            tics = None,
-            view = '60,185,1.5')
+    #Transparent demo example comes from
+    #https://gnuplot.sourceforge.net/demo_6.0/finance.html
 
+    #Ceate a gnuplot context
+    g = gnuplot.Gnuplot(log = True)
 
-.. _whale2.py:
+    #Set plotting style
+    g.set(output = "'finance.13.png'",
+            term = 'pngcairo  transparent enhanced font "arial,8" fontscale 1.0 size 660, 320',
+            label = ['1 "Acme Widgets" at graph 0.5, graph 0.9 center front',
+                '2 "Courtesy of Bollinger Capital" at graph 0.01, 0.07',
+                '3 "  www.BollingerBands.com" at graph 0.01, 0.03'],
+            logscale = 'y',
+            yrange = '[75:105]',
+            ytics = '(105, 100, 95, 90, 85, 80)',
+            xrange = '[50:253]',
+            grid = '',
+            lmargin = '9',
+            rmargin = '2',
+            format = 'x ""',
+            xtics = '(66, 87, 109, 130, 151, 174, 193, 215, 235)',
+            multiplot = True)
 
-..
-    cmd2img:: python3
-    :image: whale.png
+    #3) Expressions and caculations
 
+    #4) Plotting: Since multiplot = True, we plot two subplot
+    g.plot("'finance.dat' using 0:2:3:4:5 notitle with candlesticks lt 8",
+            "'finance.dat' using 0:9 notitle with lines lt 3",
+            "'finance.dat' using 0:10 notitle with lines lt 1",
+            "'finance.dat' using 0:11 notitle with lines lt 2",
+            "'finance.dat' using 0:8 axes x1y2 notitle with lines lt 4",
+            title = '"Change to candlesticks"',
+            size = ' 1, 0.7',
+            origin = '0, 0.3',
+            bmargin = '0',
+            ylabel = '"price" offset 1')
+    g.plot("'finance.dat' using 0:($6/10000) notitle with impulses lt 3",
+            "'finance.dat' using 0:($7/10000) notitle with lines lt 1",
+            bmargin = '',
+            format = ['x', 'y "%1.0f"'],
+            size = '1.0, 0.3',
+            origin = '0.0, 0.0',
+            tmargin = '0',
+            nologscale = 'y',
+            autoscale = 'y',
+            ytics = '500',
+            xtics = '("6/03" 66, "7/03" 87, "8/03" 109, "9/03" 130, "10/03" 151, "11/03" 174, "12/03" 193, "1/04" 215, "2/04" 235)',
+            ylabel = '"volume (0000)" offset 1')
+
+.. _finance3.13.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
 
-    # Black and white version
-    gnuplot.splot('"examples/whale.dat" w pm3d',
-            term = 'pngcairo size 480,480',
-            out = '"whale.png"',
-            style = 'line 100 lw 0.1 lc "black"',
-            pm3d = 'depth hidden3d ls 100',
-            cbrange = '[-0.5:0.5]',
-            palette = 'rgb -3,-3,-3',
-            colorbox = None,
-            border = None,
-            key = None,
-            zrange = '[-2:2]',
-            tics = None,
-            view = '60,185,1.5')
+    #Transparent demo example comes from
+    #https://gnuplot.sourceforge.net/demo_6.0/finance.html
 
-And the generated output is as following:
+    #Ceate a gnuplot context
+    g = gnuplot.Gnuplot(log = True)
 
-.. http://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.html
-.. image http://gnuplot.sourceforge.net/demo/iterate.2.png
-.. image:: http://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.png
-   :width: 350
+    #Set plotting style
+    g.set(output = "'finance.13.png'",
+            term = 'pngcairo  transparent enhanced font "arial,8" fontscale 1.0 size 660, 320',
+            label = ['1 "Acme Widgets" at graph 0.5, graph 0.9 center front',
+                '2 "Courtesy of Bollinger Capital" at graph 0.01, 0.07',
+                '3 "  www.BollingerBands.com" at graph 0.01, 0.03'],
+            logscale = 'y',
+            yrange = '[75:105]',
+            ytics = '(105, 100, 95, 90, 85, 80)',
+            xrange = '[50:253]',
+            grid = '',
+            lmargin = '9',
+            rmargin = '2',
+            format = 'x ""',
+            xtics = '(66, 87, 109, 130, 151, 174, 193, 215, 235)',
+            multiplot = True)
 
-3.2 Examples port from matplotlib
----------------------------------
+    #3) Expressions and caculations
+    #A demostration to generate pandas data frame data in python.
+    df = pd.read_csv('examples/finance.dat',
+            sep='\t',
+            index_col = 0,
+            parse_dates = True,
+            names = ['date', 'open','high','low','close', 'volume','volume_m50',
+                'intensity','close_ma20','upper','lower '])
+
+    #4) Plotting: Since multiplot = True, we plot two subplot
+    g.plot_data(df,
+            'using 0:2:3:4:5 notitle with candlesticks lt 8',
+            'using 0:9 notitle with lines lt 3',
+            'using 0:10 notitle with lines lt 1',
+            'using 0:11 notitle with lines lt 2',
+            'using 0:8 axes x1y2 notitle with lines lt 4',
+            title = '"Change to candlesticks"',
+            size = ' 1, 0.7',
+            origin = '0, 0.3',
+            bmargin = '0',
+            ylabel = '"price" offset 1')
+    g.plot_data(df,
+            'using 0:($6/10000) notitle with impulses lt 3',
+            'using 0:($7/10000) notitle with lines lt 1',
+            bmargin = '',
+            format = ['x', 'y "%1.0f"'],
+            size = '1.0, 0.3',
+            origin = '0.0, 0.0',
+            tmargin = '0',
+            nologscale = 'y',
+            autoscale = 'y',
+            ytics = '500',
+            xtics = '("6/03" 66, "7/03" 87, "8/03" 109, "9/03" 130, "10/03" 151, "11/03" 174, "12/03" 193, "1/04" 215, "2/04" 235)',
+            ylabel = '"volume (0000)" offset 1')
+
+Both script generate the same output image:
+
+|finance.13.png|
+
+2.5 Examples port from matplotlib
+-----------------------------------
 
 Just for fun, I translate some examples in matplotlib to py-gnuplot:
 
-3.2.1 Stacked bar chart
+2.5.1 Stacked bar chart
 +++++++++++++++++++++++
 
-..
-    .. cmd2img:: python3
-        :image: sphx_glr_bar_stacked_001.png
-
+.. _sphx_glr_bar_stacked_001.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
 
@@ -1335,27 +860,22 @@
             boxwidth = '%s' %(width),
             xrange = '[0.5:5.5]',
             ylabel = '"Scores"',
             title = '"Scores by group and gender"',
             output = '"sphx_glr_bar_stacked_001.png"',
             terminal = 'pngcairo size 640, 480')
 
-Refer to the original script: `Stacked bar chart`_ and the original image:
+This is the output:
 
-.. _Stacked bar chart: https://matplotlib.org/gallery/lines_bars_and_markers/bar_stacked.html#sphx-glr-gallery-lines-bars-and-markers-bar-stacked-py
-.. image:: https://matplotlib.org/_images/sphx_glr_bar_stacked_001.png
-   :width: 350
+|sphx_glr_bar_stacked_001.png|
 
-3.2.2 Grouped bar chart with labels
+2.5.2 Grouped bar chart with labels
 +++++++++++++++++++++++++++++++++++
 
-..
-    cmd2img:: python3
-            :image: sphx_glr_barchart_001.png
-
+.. _sphx_glr_barchart_001.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
 
@@ -1382,27 +902,22 @@
             style = ['data histogram',
                      'histogram cluster gap 1',
                      'fill solid border -1',
                      'textbox transparent'],
             output = '"sphx_glr_barchart_001.png"',
             terminal = 'pngcairo size 640, 480')
 
-Refer to the original script: `Grouped bar chart with labels`_ and the original image:
+This is the output:
 
-.. _Grouped bar chart with labels: https://matplotlib.org/gallery/lines_bars_and_markers/barchart.html#sphx-glr-gallery-lines-bars-and-markers-barchart-py
-.. image:: https://matplotlib.org/_images/sphx_glr_barchart_001.png
-   :width: 350
+|sphx_glr_barchart_001.png|
 
-3.2.3 Multiplot Axes Demo
+2.5.3 Multiplot Axes Demo
 +++++++++++++++++++++++++
 
-..
-    cmd2img:: python3
-            :image: sphx_glr_axes_demo_001.png
-
+.. _sphx_glr_axes_demo_001.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
     import numpy as np
@@ -1451,27 +966,22 @@
     g.plot_data(df,
             'using 1:2 with line lw 2 lc "web-blue"',
             title = '"Impulse response"',
             xrange = '[0:0.2]',
             origin = '0.15, 0.56',
             size = '0.24, 0.32')
 
-Refer to the original script: `Multiplot Axes Demo`_ and the original image:
+This is the output:
 
-.. _Multiplot Axes Demo: https://matplotlib.org/gallery/subplots_axes_and_figures/axes_demo.html#sphx-glr-gallery-subplots-axes-and-figures-axes-demo-py
-.. image:: https://matplotlib.org/_images/sphx_glr_axes_demo_001.png
-   :width: 350
+|sphx_glr_axes_demo_001.png|
 
-3.2.4 control view and zoom 
+2.5.4 control view and zoom 
 ++++++++++++++++++++++++++++
 
-..
-    cmd2img:: python3
-            :image: sphx_glr_axes_margins_001.png
-
+.. _sphx_glr_axes_margins_001.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
 
@@ -1506,79 +1016,69 @@
             xrange = '[0: 3]',
             yrange = '[-0.7: 1]',
             xtics = '0, 0.5, 3',
             ytics = '-0.5, 0.5, 1',
             origin = '0, 0',
             size = '1, 0.5')
 
-Refer to the original script: `axes_margins.py`_ and the original image:
+This is the output:
 
-.. _axes_margins.py: https://matplotlib.org/_downloads/4d3bc54481c3ff3a1ac6712bc2904875/axes_margins.py
-.. image:: https://matplotlib.org/_images/sphx_glr_axes_margins_001.png
-   :width: 350
+|sphx_glr_axes_margins_001.png|
 
-3.2.5 Rendering math equation using TeX
+2.5.5 Rendering math equation using TeX
 +++++++++++++++++++++++++++++++++++++++
 
 We can embed the TeX math equation into the gnuplot generated image by setting
 the epslatex terminal, it would be rendered as a .tex file, you can import it
 directly or you can convert it to .pdf file and then .png file if needed. this
 is the example:
 
-..
-    cmd2img:: python3
-    :image: pygnuplot_tex_demo.tex
-
+.. _sphx_glr_tex_demo_001.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
 
     # https://matplotlib.org/gallery/text_labels_and_annotations/tex_demo.html#sphx-glr-gallery-text-labels-and-annotations-tex-demo-py
     # http://wap.sciencenet.cn/blog-373392-500657.html
     # https://www.thinbug.com/q/17593917
     g = gnuplot.Gnuplot(log = True,
-            output = '"pygnuplot_tex_demo.tex"',
+            output = '"sphx_glr_tex_demo_001.tex"',
             term = 'epslatex standalone lw 2 color colortext')
 
     # NOTE: In the following example, we need to escape the "\", that means we
     # should use '\\' or "\\\\" for \
     g.plot('cos(4*pi*x) + 2',
             xlabel = "'\\textbf{time (s)}'",
             ylabel = "'\\textit{Velocity (\N{DEGREE SIGN}/sec)}'",
             title = "'\\TeX\\ is Number $\\displaystyle\\sum_{n=1}^\\infty\\frac{-e^{i\\pi}}{2^n}$!' tc 'red'",
             key = None,
             xrange = '[0: 1]')
 
+This is the output:
+
+|sphx_glr_tex_demo_001.png|
+
 I list the script output since it's with the log=True::
 
-    [py-gnuplot 14:56:13] set output "pygnuplot_tex_demo.tex"
+    [py-gnuplot 14:56:13] set output "sphx_glr_tex_demo_001.tex"
     [py-gnuplot 14:56:13] set term epslatex standalone lw 2 color colortext
     [py-gnuplot 14:56:13] set xlabel '\textbf{time (s)}'
     [py-gnuplot 14:56:13] set ylabel '\textit{Velocity (°/sec)}'
     [py-gnuplot 14:56:13] set title '\TeX\ is Number $\displaystyle\sum_{n=1}^\infty\frac{-e^{i\pi}}{2^n}$!' tc 'red'
     [py-gnuplot 14:56:13] unset key
     [py-gnuplot 14:56:13] set xrange [0: 1]
     [py-gnuplot 14:56:13] plot cos(4*pi*x) + 2
 
-Refer to the original script: `Rendering math equation using TeX`_ and the original image:
-
-.. _Rendering math equation using TeX: https://matplotlib.org/gallery/text_labels_and_annotations/tex_demo.html#sphx-glr-gallery-text-labels-and-annotations-tex-demo-py
-.. image:: https://matplotlib.org/_images/sphx_glr_tex_demo_001.png
-   :width: 350
-
-3.2.6 Basic pie chart
+2.5.6 Basic pie chart
 +++++++++++++++++++++
 
-..
-    cmd2img:: python3
-    :image: sphx_glr_pie_features_0011.png
-
+.. _sphx_glr_pie_features_0011.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
     import math
@@ -1601,60 +1101,55 @@
     df = df.fillna(startangle)
     #print(df)
 
     pie_shade = []
     pie_graph = []
 
     shade_offset = 0.03
+    g = gnuplot.Gnuplot(log = True,
+            output = '"sphx_glr_pie_features_0011.png"',
+            term = 'pngcairo size 640, 480',
+            key = None,
+            parametric = "",
+            border = "",
+            tics = "",
+            multiplot = True)
+
     for k, v in df.iterrows():
         #print(k,v)
         cos = math.cos((v['start']+v['end'])/2)
         sin = math.sin((v['start']+v['end'])/2)
 
         # If we'd like explode the piece, ad the dx/dy to move the origi point.
         dx = v['explode'] * cos
         dy = v['explode'] * sin
 
         # make the shade for each piece
-        piece = gnuplot.make_plot('cos(t)+%f, sin(t)+%f with filledcurves xy=%f,%f lc "grey80"'
-                    %(dx-shade_offset, dy-shade_offset, dx-shade_offset, dy-shade_offset),
+        g.plot('cos(t)+%f, sin(t)+%f with filledcurves xy=%f,%f lc "grey80"'
+                %(dx-shade_offset, dy-shade_offset, dx-shade_offset, dy-shade_offset),
                 trange = '[%f:%f]' %(v['start'], v['end']),
                 xrange = '[-1.5:1.5]',
                 yrange = '[-1.5:1.5]')
-        pie_shade.append(piece)
 
         # make the pie and label
-        piece = gnuplot.make_plot('cos(t)+%f, sin(t)+%f with filledcurve xy=%f,%f  lt %d'
-                    %(dx, dy, dx, dy, k+3),
+        g.plot('cos(t)+%f, sin(t)+%f with filledcurve xy=%f,%f  lt %d'
+                %(dx, dy, dx, dy, k+3),
                 trange = '[%f:%f]' %(v['start'], v['end']),
                 xrange = '[-1.5:1.5]',
                 yrange = '[-1.5:1.5]',
-                label = ['1 "%s" at %f, %f center front' %(v['labels'], 1.2*cos+dx, 1.2*sin+dy),
-                    '2 "%.1f%%" at %f, %f center front' %(v['percentage']*100, 0.6*cos, 0.6*sin)])
-        pie_graph.append(piece)
+                label = ['1 "%s" at %f, %f center front' %(v['labels'], 1.2*cos+dx, 1.2*sin+dy), '2 "%.1f%%" at %f, %f center front' %(v['percentage']*100, 0.6*cos, 0.6*sin)])
 
-    gnuplot.multiplot(*pie_shade, *pie_graph,
-            output = '"sphx_glr_pie_features_0011.png"',
-            terminal = 'pngcairo size 640, 480',
-            key = None,
-            parametric = '',
-            border = '',
-            tics = '',
-            multiplot = True)
-
-Refer to the original script: `Basic pie chart`_ and the original image:
+This is the output:
 
-.. _Basic pie chart: https://matplotlib.org/gallery/pie_and_polar_charts/pie_features.html#sphx-glr-gallery-pie-and-polar-charts-pie-features-py
-.. image:: https://matplotlib.org/_images/sphx_glr_pie_features_0011.png
-   :width: 350
+|sphx_glr_pie_features_0011.png|
 
-4. Q/A
+3. Q/A
 =======
 
-5. CHANGLOG
+4. CHANGLOG
 =============
 
 1.0 Initial upload;
 
 1.0.3 Now Gnuplot().plot()/splot() supplot set options as parameters.
 
 1.0.7 The pyplot.plot() now can accept both string and pandas.Dataframe as the
@@ -1675,12 +1170,15 @@
 1.1.2 Enhancement: If it's multiplot mode, automatically call the following
 Gnuplot to unset the label:
 
     g.unset('for [i=1:200] label i')
 
 1.1.3 Enhancement: When plotting the python generated data, we set the
 seperator to "," for easy using it in csv file.
+
 1.1.5 Bug fix: on some case it exit exceptionally.
+
 1.1.8 Remove some Chinese comments to remove the "UnicodeDecodeError" for some users.
-1.1.9 1) Run and update the examples in gnuplot6.0.0. 2) If you'd like enable multiplot, you shuld use  multimplot = True to replace multimplot = "".
 
+1.1.9 1) Run and update the examples in gnuplot6.0.0. 2) If you'd like enable multiplot, you shuld use  multimplot = True to replace multimplot = "".
 
+1.1.13 Document update.
```

### Comparing `py-gnuplot-1.1.9/README.rst` & `py-gnuplot-1.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,1302 +1,853 @@
+Metadata-Version: 2.1
+Name: py-gnuplot
+Version: 1.2.0
+Summary: py-gnuplot is a python plot tools based on gnuplot.
+Home-page: http://www.gnuplot.info
+Author: Yongping Guo
+Author-email: guoyoooping@163.com
+License: GPLv3
+Keywords: gnuplot,pandas
+Platform: UNKNOWN
+Requires-Python: >=3.6
+License-File: LICENSE.txt
+
 .. meta::
    :description: gnuplot plotting backend for python.
    :keywords: gnuplot, py-gnuplot, pandas, python, plot
 
-Gnuplot is a portable command-line driven graphing utility for many
-platforms. To leverage the powful gnuplot to plot beautiful image in
-efficicent way in python, we port gnuplot to python. Let's see an example
-at first:
-
-..
-    cmd2img:: python3
-    :image: simple.1.png
+Gnuplot is a powerful command-line driven graphing utility for many platforms.
+To leverage the powful gnuplot to plot beautiful image in efficicent way in
+python, we port gnuplot to python. 
+
+We develop **set()/unset()** function to set or unset gnuplot plotting style,
+**plot()/splot()** to operate gnuplot plot or splot command, **cmd()** to
+execute any commands that coulnd't be done by the above functions. They are
+intuative and gnuplot users can swith to py-gnuplot naturally. By this means we
+can do what gnuplot do.
+
+.. image:: https://gnuplot.sourceforge.net/demo_6.0/transparent.2.png
+    :align: right
+    :width: 300
+
+But for plotting python generated data the above functions are not enough. We
+develop **plot_data()/splot_data()** to plot data generated in
+python.
+
+Here is a quick examples to generate the right image with only basic functions,
+more examples which plot python generated data are coming in later sections.
+
+.. _sphinx-plot-directive: https://pypi.org/project/sphinx-plot-directive
 
+.. _quick_example.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
 
-    gnuplot.plot('[-10:10] sin(x)',
-           'atan(x)',
-           'cos(atan(x))',
-           terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400',
-           output = '"simple.1.png"',
-           key = 'fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid',
-           samples = '50, 50',
-           title = '"Simple Plots" font ",20" textcolor lt -1 norotate',
-           xrange = '[ * : * ] noreverse writeback',
-           x2range = '[ * : * ] noreverse writeback',
-           yrange = '[ * : * ] noreverse writeback',
-           y2range = '[ * : * ] noreverse writeback',
-           zrange = '[ * : * ] noreverse writeback',
-           cbrange = '[ * : * ] noreverse writeback',
-           rrange = '[ * : * ] noreverse writeback',
-           colorbox = 'vertical origin screen 0.9, 0.2 size screen 0.05, 0.6 front noinvert bdefault',
-           #NO_ANIMATION = '1', #I don't know what's this. Who know? please tell me. Thanks.
-           )
-
-From the example we can see, we plot the function with plot() function, with
-all the options as the function parameters. It's easy to understand and comply
-with both gnuplot and python's grammer. The generated image is as below:
+    #py-gnuplot: A quick demo
 
-.. figure:: http://gnuplot.sourceforge.net/demo/simple.1.png 
-   :width: 350
+    #Ceate a gnuplot context. with "log = True" to print the gnuplot execute log.
+    g = gnuplot.Gnuplot(log = True)
 
-   figure 1. pygnuplot demo 1: simple function
+    #Set plotting style
+    g.set(terminal = 'pngcairo transparent enhanced font "arial,8" fontscale 1.0 size 512, 280 ',
+            output = '"quick_example.png"',
+            style = ["fill transparent solid 0.50 noborder", "data lines", "function filledcurves y1=0"],
+            key = 'title "Gaussian Distribution" center fixed left top vertical Left reverse enhanced autotitle nobox noinvert samplen 1 spacing 1 width 0 height 0',
+            title = '"Transparent filled curves"',
+            xrange = '[ -5.00000 : 5.00000 ] noreverse nowriteback',
+            yrange = '[ 0.00000 : 1.00000 ] noreverse nowriteback')
 
-Let's see the detail in the below:
+    #Expressions and caculations
+    g.cmd('Gauss(x,mu,sigma) = 1./(sigma*sqrt(2*pi)) * exp( -(x-mu)**2 / (2*sigma**2) )',
+            'd1(x) = Gauss(x, 0.5, 0.5)',
+            'd2(x) = Gauss(x,  2.,  1.)',
+            'd3(x) = Gauss(x, -1.,  2.)')
 
-.. contents:: [Contents]
-   :depth: 3
-
-1. Introduction and examples list
-===================================
+    #Plotting
+    g.plot('d1(x) fs solid 1.0 lc rgb "forest-green" title "μ =  0.5 σ = 0.5"',
+            'd2(x) lc rgb "gold" title "μ =  2.0 σ = 1.0"',
+            'd3(x) lc rgb "dark-violet" title "μ = -1.0 σ = 2.0"')
 
-As we know Gnuplot is a portable and powerful command-line driven graphing
-utility for many platforms. To leverage the power of Gnuplot, We develop
-the py-gnuplot in a easy understand way.
-
-**py-python only support python3** since the function dictionary paramaters in
-python2 is not in order.
-
-This package has an object-oriented design as well as direct function call to
-allows the user flexibility to set plot options and to run multiple gnuplot
-sessions simultaneously. So in this document, every examples are rendered in
-two way: quick plot mode and object-oriented. Either mode works and you can
-choose which way you like.
-
-We will introduce it in detail in the following chapter and here list the
-exaples used in this article as below:
-
-.. _Table1:
-
-.. list-table:: Table1 : A demostration of pygnuplot.gnuplot script
-   :widths: 15, 20, 20, 70
-   :header-rows: 1
-
-   * - gnuplot demo script
-     - object-oriented interface script
-     - direct function call script
-     - All the script produce the same image
-   * - `simple.dem`_
-     - simple2.py_
-     - simple3.py_
-     - |simple.1.png|
-   * - `surface2.dem`_
-     - surface1.py_
-     - surface2.py_
-     - |surface2.9.png|
-   * - `iterate.dem`_
-     - whale1.py_
-     - whale2.py_
-     - |whale.png|
+more examples:
 
-.. _Table2:
+.. _simple.1.gnu: http://gnuplot.sourceforge.net/demo/simple.1.gnu
+.. _surface2.9.gnu: http://gnuplot.sourceforge.net/demo/surface2.9.gnu
+.. _histograms.1.gnu: http://gnuplot.sourceforge.net/demo/histograms.1.gnu
+.. _iterate.2.gnu: http://gnuplot.sourceforge.net/demo/iterate.2.gnu
+.. _finance.13.gnu: http://gnuplot.sourceforge.net/demo/finance.13.gnu
 
-.. list-table:: Table 2: A demostration of plot() and plot_data()
-   :widths: 15, 20, 20, 70
-   :header-rows: 1
-
-   * - gnuplot demo script
-     - object-oriented interface script
-     - direct function call script
-     - All the script produce the same image
-   * - `histo.1.gnu`_
-     - histo.1.py_
-     - histo.2.py_
-     - |histograms.1.png|
-   * - `finance.dem`_
-     - finance1.py_
-     - finance1.py_
-     - |finance.13.png|
-
-.. list-table:: Table 3: Examples porting from Matplotlib
-   :widths: 35, 35, 35, 35
-   :header-rows: 0
-
-   * - `3.2.1 Stacked bar chart`_ |sphx_glr_bar_stacked_001.png|
-     - `3.2.2 Grouped bar chart with labels`_ |sphx_glr_barchart_001.png|
-     - `3.2.3 Multiplot Axes Demo`_ |sphx_glr_axes_demo_001.png|
-     - `3.2.4 control view and zoom`_ |sphx_glr_axes_margins_001.png|
-   * - `3.2.5 Rendering math equation using TeX`_ |sphx_glr_tex_demo_001.png|
-     - `3.2.6 Basic pie chart`_ |sphx_glr_pie_features_0011.png|
-     - 
-     - 
-
-.. _simple.dem: http://gnuplot.sourceforge.net/demo/simple.1.gnu
-.. _surface2.dem: http://gnuplot.sourceforge.net/demo/surface2.9.gnu
-.. _histo.1.gnu: http://gnuplot.sourceforge.net/demo/histograms.1.gnu
-.. _iterate.dem: http://gnuplot.sourceforge.net/demo/iterate.2.gnu
-.. _finance.dem: http://gnuplot.sourceforge.net/demo/finance.13.gnu
 .. |simple.1.png| image:: http://gnuplot.sourceforge.net/demo/simple.1.png
-   :width: 180
+   :width: 350
 .. |surface2.9.png| image:: http://gnuplot.sourceforge.net/demo/surface2.9.png
-   :width: 180
+   :width: 350
 .. |finance.13.png| image:: http://gnuplot.sourceforge.net/demo/finance.13.png
-   :width: 180
+   :width: 350
 .. |iterate.2.png| image:: http://gnuplot.sourceforge.net/demo/iterate.2.png
-   :width: 180
+   :width: 350
 .. |whale.png| image:: http://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.png
-   :width: 180
-.. |histograms.1.png| image:: http://gnuplot.sourceforge.net/demo/histograms.1.png
-   :width: 180
+   :width: 350
+.. |histograms.2.png| image:: http://gnuplot.sourceforge.net/demo/histograms.2.png
+   :width: 350
 .. |sphx_glr_bar_stacked_001.png| image:: https://matplotlib.org/_images/sphx_glr_bar_stacked_001.png
-   :width: 180
+   :width: 350
 .. |sphx_glr_barchart_001.png| image:: https://matplotlib.org/_images/sphx_glr_barchart_001.png
-   :width: 180
+   :width: 350
 .. |sphx_glr_axes_demo_001.png| image:: https://matplotlib.org/_images/sphx_glr_axes_demo_001.png
-   :width: 180
+   :width: 350
 .. |sphx_glr_pie_features_0011.png| image:: https://matplotlib.org/_images/sphx_glr_pie_features_0011.png
-   :width: 180
+   :width: 350
 .. |sphx_glr_tex_demo_001.png| image:: https://matplotlib.org/_images/sphx_glr_tex_demo_001.png
-   :width: 180
+   :width: 350
 .. |sphx_glr_axes_margins_001.png| image:: https://matplotlib.org/_images/sphx_glr_axes_margins_001.png
-   :width: 180
+   :width: 350
 
-2. Plot elements in py-gnuplot
-=================================
+.. list-table:: Table1 : plot examples with different script
 
-As we know, gnuplot use commands to plot all kinds of image, we port almost all
-the useful commands as functions in py-gnuplot.
+   * - examples
+     - plot function
+     - plot file
+     - splot function
+     - splot file
+     - multiplot
+   * - figure
+     - |simple.1.png|
+     - |histograms.2.png|
+     - |surface2.9.png|
+     - |whale.png|
+     - |finance.13.png|
+   * - gnuplot script
+     - `simple.1.gnu`_
+     - `histograms.1.gnu`_
+     - `surface2.9.gnu`_
+     - `iterate.2.gnu`_
+     - `finance.13.gnu`_
+   * - py-gnuplot script
+     - `simple.1.py`_
+     - `histograms.2.py`_
+     - `surface.9.py`_
+     - `whale.py`_
+     - `finance.13.py`_
+   * - py-gnuplot quick mode
+     - `simple2.1.py`_
+     - `histograms2.2.py`_
+     - `surface2.9.py`_
+     - `whale2.py`_
+     -  N/A(too complicated)
+   * - py-gnuplot data generated in python
+     - N/A
+     - `histograms3.2.py`_
+     - N/A
+     - N/A
+     - `finance3.13.py`_
+
+.. list-table:: Table2 : examples porting from matplotlib
+   :widths: 30,30,30
+
+   * - `sphx_glr_bar_stacked_001.py`_ |sphx_glr_bar_stacked_001.png|
+     - `sphx_glr_barchart_001.py`_ |sphx_glr_barchart_001.png|
+     - `sphx_glr_axes_demo_001.py`_ |sphx_glr_axes_demo_001.png|
+   * - `sphx_glr_axes_margins_001.py`_ |sphx_glr_axes_margins_001.png|
+     - `sphx_glr_tex_demo_001.py`_ |sphx_glr_tex_demo_001.png|
+     - `sphx_glr_pie_features_0011.py`_ |sphx_glr_pie_features_0011.png|
+
+Let's see the detail.
 
-In `2.1 member functions port from Gnuplot`_ we introduce the member
-functions that we can plot all what Gnuplot could do, The limitation is
-it's not so easy to plot the python generated data with the those existing
-command.
+.. contents:: [Contents]
+   :depth: 2
 
-To plot the data generated in python, we develop additional functions as
-below, ::
+1. Introduction
+=================
 
-    plot_data(self, data, *items, **kwargs):
-    splot_data(self, data, *items, **kwargs)
+As we know, to plot a image in gnuplot we do:
 
-they are almost the same as the original plot()/splot(), the difference is
-we pass the data as the first parameter, you don't give the filename in the
-plot command, see detail in `2.2 new developed member functions for python
-generated data`_ .
+    1) Enter gnuplot conext;
+    2) Set plotting style;
+    3) Define some expressions;
+    4) Plotting.
 
-Sometime we only need simple plot and don't want to allocate a Gnuplot
-instance, we develop the quick way to plot: `2.3 new developed global
-class-less function call`_ and you can plot the image in a easy way with
-global class-less function call.
+We translate gnuplot's main function into python ones, and each one do the same
+thing as gnuplot. As in `quick_example.py`_ we also have 4 steps to plot an
+image::
 
-2.1 member functions port from Gnuplot
----------------------------------------
+    #Constructor
+    g = gnuplot.Gnuplot()
+    #Set plotting style
+    g.set()
+    #Expressions and caculations
+    g.cmd()
+    #Plotting
+    g.plot()
 
-The principle is if you can write Gnuplot script, you can write py-gnuplot.
-There is 1-1 mapping between almost all Gnuplot command and python
-function;
+1.1 constructor
+----------------
 
-2.1.1 The constructor
-+++++++++++++++++++++
+Defenition:
 
 .. code-block:: python
 
     def __init__(self, *args, log = False, **kwargs):
         '''
         *args: The flag parameter in gnuplot
         log: If print the gnuplot log
         **kwargs: the flag that need to be set. You can also set them in the set() function.
         '''
 
-When create the Gnuplot instance, you can pass some parameter to it, you
-can also set them when you call set() or plot(), they are the same.
-
-The "log" parameter is a new added flag to indicate if we print the gnuplot
-execution log when run. For example:
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-    #See original gnuplot script here:
-    #http://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.html
-    g = gnuplot.Gnuplot(log = True,
-            term = 'pngcairo size 480,480',
-            out = '"whale.png"',
-            pm3d = 'depth hidden3d ls 100',
-            cbrange = '[-0.5:0.5]',
-            palette = 'rgb -3,-3,-3',
-            colorbox = None,
-            border = None,
-            key = None,
-            zrange = '[-2:2]',
-            tics = None,
-            view = '60,185,1.5')
-    g.splot('"examples/whale.dat" w pm3d')
-
-This is the script output with the log=True::
-
-    [py-gnuplot] set term pngcairo size 480,480
-    [py-gnuplot] set out "whale.png"
-    [py-gnuplot] set pm3d depth hidden3d ls 100
-    [py-gnuplot] set cbrange [-0.5:0.5]
-    [py-gnuplot] set palette rgb -3,-3,-3
-    [py-gnuplot] unset colorbox
-    [py-gnuplot] unset border
-    [py-gnuplot] unset key
-    [py-gnuplot] set zrange [-2:2]
-    [py-gnuplot] unset tics
-    [py-gnuplot] set view 60,185,1.5
-    [py-gnuplot] splot "examples/whale.dat" w pm3d
+We call g = gnuplot.Gnuplot(log = True) to get a gnuplot context. Here log = True means to print the gnuplot log when call gnuplot functions.::
 
-And this is the image output: |small_whale.png|
+    #Ceate a gnuplot context. with "log = True" to print the gnuplot execute log.
+    g = gnuplot.Gnuplot(log = True)
 
-.. |small_whale.png| image:: http://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.png
-   :width: 50
+1.2 Set()/unset()
+------------------
 
-2.1.2 cmd()
-+++++++++++
-
-.. code-block:: python
-
-    def cmd(self, *args):
-        '''
-        *args: all the line that need to pass to gnuplot. It could be a
-        list of lines, or a paragraph; Lines starting with "#" would be
-        omitted. Every line should be a clause that could be executed in
-        gnuplot.
-        '''
-
-We implemented the function cmd() and pass the command to call Gnuplot to plot
-the data, Thus we could do everything with the only one simple function:
-
-.. _simple1.1.py:
-..
-    cmd2img:: python3
-    :image: simple.1.png
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-    # Illustration of object-oriented interface, you can see we only wrap the
-    # gnuplot script by g.cmd('...') and it's simple and straitfoward if you
-    # are familar with Gnuplot.
-    g = gnuplot.Gnuplot()
-    g.cmd('set terminal pngcairo font "arial,10" fontscale 1.0 size 600, 400')
-    g.cmd('set output "simple.1.png"')
-    g.cmd('set key fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid')
-    g.cmd('set samples 50, 50')
-    g.cmd('set title "Simple Plots" ')
-    g.cmd('set title  font ",20" norotate')
-    g.cmd('plot [-10:10] sin(x),atan(x),cos(atan(x))')
-
-Or you can even pass the Gnuplot command as a string list or a text paragraph:
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-    # Illustration of cmd(), you can see we only wrap the
-    # gnuplot script by g.cmd('...') and it's simple and straitfoward if you
-    # are familar with Gnuplot.
-    g = gnuplot.Gnuplot()
-
-    # Take all the Gnuplot command as a list of command:
-    g.cmd('set terminal pngcairo font "arial,10" fontscale 1.0 size 600, 400',
-    'set output "simple.1.png"',
-    'set key fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid',
-    'set samples 50, 50',
-    'set title "Simple Plots" ',
-    'set title  font ",20" norotate',
-    'plot [-10:10] sin(x),atan(x),cos(atan(x))')
-
-    # Another means, take all the Gnuplot command as a script paragraph,
-    #uncomment the following code block to have a try.
-    #plot_cmd = '''
-    #set terminal pngcairo font "arial,10" fontscale 1.0 size 600, 400
-    #set output "simple.1.png"
-    #set key fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid
-    #set samples 50, 50
-    #set title "Simple Plots
-    #set title  font ",20" norotate
-    #plot [-10:10] sin(x),atan(x),cos(atan(x))'''
-    #g.cmd(plot_cmd)
-
-This is the image output: |small_simple.png|
-
-.. |small_simple.png| image:: http://gnuplot.sourceforge.net/demo/simple.1.png
-   :width: 50
-
-By this means we can do everything that Gnuplot can do and cannot do what
-Gnuplot itself can't do. It's the exact way that the Gnuplot do it. and we
-don't get any benifit besides we can call Gnuplot in python. So we develop
-many other functions as below:
-
-2.1.3 set()
-+++++++++++
+Defenition:
 
 .. code-block:: python
 
     def set(self, *args, **kwargs):
         '''
         *args: options without value
         *kwargs: options with value. The set and unset commands may optionally
                  contain an iteration clause, so the arg could be list.
         '''
+    def unset(self, *items):
+        '''
+        *args: options that need to be unset
+        '''
 
-The set command can be used to set lots of options. The set and unset
-commands may optionally contain an iteration clause, so the arg could be
-list. For examples:
-
-We set the options before plot and then call plot to render the image. It's
-equivalent to example in `2.1.2 cmd()`_ but seems muck like a python script.
-
-.. _simple2.py:
-
-..
-    cmd2img:: python3
-    :image: simple.1.png
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-
-    # Gnuplot lines:
-    #set terminal pngcairo font "arial,10" fontscale 1.0 size 600, 400
-    #set output "simple.1.png"
-    #set key fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid
-    #set samples 50, 50
-    #set title "Simple Plots" font ",20" norotate
+After enter gnuplot context, normally we need to set the plotting style. For
+example we need to set the terminal and output at first in gnuplt as following::
 
-    g = gnuplot.Gnuplot()
-    g.set(terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400',
-            output = '"simple.1.png"',
-            key = 'fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid',
-            samples = '50, 50',
-            title = '"Simple Plots" font ",20" norotate')
-    g.plot('[-10:10] sin(x),atan(x),cos(atan(x))')
-
-set() is flexible but indeed set() functions is not necessary. We could
-pass the options as parameter in the constructor and plot(). For examples
-the following script act equally with the above:
+    set terminal pngcairo  transparent enhanced font "arial,8" fontscale 1.0 size 512, 280 
+    set output 'transparent.2.png'
 
-.. code-block:: python
+Then we translate the set into set() function as following, please not that all
+the elment are stirng, so must add extra quoto and it would be passed to
+gnuplot without any change. Pleae note that all the parameters must be string
+since it would be passed to gnuplot without any change. You need to change them
+to string if they are not::
+
+    #Set plotting style
+    g.set(terminal = 'pngcairo transparent enhanced font "arial,8" fontscale 1.0 size 512, 280 ',
+            output = '"quick_example.png"',
+            ...
+            )
 
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
+For unset we have flexible ways to do that, for exampes the following ways are
+the same::
 
-    # py-python lines:
-    g = gnuplot.Gnuplot(terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400',
-            output = '"test.png"',
-            boxwidth = '0.9 relative',
-            style = 'fill solid 1.0',
-            label = ['"y=x" at 1,2',
-                '2 "S" at graph 0.5,0.5 center font "Symbol,24"',
-                '3 "y=x^2" at 2,3,4 right'])
-            g.plot('"file.dat" with boxes')
+    #gnuplot unset
+    unset colorbox
 
-We can also write it as the following, they are all the same:
+    #py-gnuplot means1
+    g.unset(colorbox)
 
-.. code-block:: python
+    #py-gnuplot means2
+    g.set(colorbox = None)
 
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
+    #py-gnuplot means3
+    g.set(nocolorbox = "")
 
-    # py-python lines:
-    g = gnuplot.Gnuplot()
-    g.plot('"file.dat" with boxes',
-           terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400',
-           output = '"test.png"',
-           boxwidth = '0.9 relative',
-           style = 'fill solid 1.0',
-           label = ['"y=x" at 1,2',
-                    '2 "S" at graph 0.5,0.5 center font "Symbol,24"',
-                    '3 "y=x^2" at 2,3,4 right'])
+1.3 cmd()
+----------
 
-2.1.4 unset()
-+++++++++++++++
+Defenition:
 
 .. code-block:: python
 
-    def unset(self, *items):
+    def cmd(self, *args):
         '''
-        *args: options that need to be unset
+        *args: all the line that need to pass to gnuplot. It could be a
+        list of lines, or a paragraph; Lines starting with "#" would be
+        omitted. Every line should be a clause that could be executed in
+        gnuplot.
         '''
 
-Options set using the set() function may be returned to their default state by
-the corresponding unset() function:
+Sometimes before plot we need define some variable or caculations, call cmd() functions to do::
 
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-    # py-python lines:
-    g = gnuplot.Gnuplot(terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400', output = '"test.png"')
-    g.unset('xlabel', 'ylabel', 'xrange', 'yrange')
-    g.plot('sin(x) with lp')
-
-unset command could be replaced as set, for example the above example could
-also be writen as:
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
+    #gnuplot
+    Gauss(x,mu,sigma) = 1./(sigma*sqrt(2*pi)) * exp( -(x-mu)**2 / (2*sigma**2) )
+    d1(x) = Gauss(x, 0.5, 0.5)
+    d2(x) = Gauss(x,  2.,  1.)
+    d3(x) = Gauss(x, -1.,  2.)
+
+    #py-gnuplot
+    g.cmd('Gauss(x,mu,sigma) = 1./(sigma*sqrt(2*pi)) * exp( -(x-mu)**2 / (2*sigma**2) )',
+            'd1(x) = Gauss(x, 0.5, 0.5)',
+            'd2(x) = Gauss(x,  2.,  1.)',
+            'd3(x) = Gauss(x, -1.,  2.)')
 
-    # Another means to unset options:
-    g = gnuplot.Gnuplot(terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400', output = '"test.png"')
-    g.set('noxlabel', 'noylabel', 'noxrange', 'noyrange')
-    g.plot('sin(x) with lp')
+As we see, all statement in cmd() would be translated the same statement in
+gnuplot. By this way we can execute any gnuplot statement.
 
-    # Another means to unset options:
-    g = gnuplot.Gnuplot()
-    g.set(xlabel = None,
-          ylabel = None,
-          xrange = None,
-          yrange = None)
-    g.plot('sin(x) with lp')
+1.4 plot()/splot()
+------------------
 
-2.1.5 plot()
-++++++++++++
+Definition:
 
 .. code-block:: python
 
     def plot(self, *items, **kwargs):
         '''
         *items: The list of plot command;
         **kwargs: The options that would be set before the plot command.
         '''
-
-plot is the primary command for drawing plots with gnuplot, We port it as a
-function in py-python. As description, the plot-element is passed as
-variable parameters, and options are passed as dictionary parameter. please
-be noted that the plot-element should be in the single quotes:
-
-Note that the plot()/splot() only plot the gnuplot functions and file, if
-you'd like to plot data generated in python, you should call the new added
-functions: `2.2.1 plot_data()`_ and `2.2.2 splot_data()`_ .
-
-for example plot the gnuplot function or datafile we use pygnuplot.gnuplot:
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-    g = gnuplot.Gnuplot()
-    g.plot('[-10:10] sin(x)',
-           'atan(x)',
-           'cos(atan(x))',
-           terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400',
-           output = '"simple.1.png"',
-           key = 'fixed left top vertical Right lt black linewidth 1.000 dashtype solid',
-           samples = '50, 50',
-           title = '"Simple Plots" font ",20" norotate')
-
-If we plot the python generated data we use plot_data() and splot_data():
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-    # usage examples, please note that we didn't give the output so could only
-    # see the image flash on the screen. Will introduce how to output the
-    # image to files.
-    df = pd.DataFrame(data = {'col1': [1, 2],
-                              'col2': [3, 4],
-                              'col3': [5, 6]})
-    g = gnuplot.Gnuplot()
-    g.plot_data(df, 'using 1:2 with lines', 'using 1:3 with points')
-
-As we stated in `2.1.3 set()`_ , we can use parameter to replace
-set()/unset() in plot() function, here is something we need to know when
-using parameter to replace set()/unset():
-
-1) If it's flag parameter, for example::
-
-    set grid
-    set hidden3d
-
-we can pass it as a empty value:
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-
-    # Examples of gnuplot.plot()
-    g = gnuplot.Gnuplot()
-    g.plot('sin(x)',
-           'cos(x)',
-           ...,
-           grid = '',
-           hidden3d = '',
-           ...)
-
-    # Examples of plot_data()
-    df = pd.DataFrame(data = {'col1': [1, 2],
-                              'col2': [3, 4],
-                              'col3': [5, 6]})
-    g = gnuplot.Gnuplot()
-    g.plot_data(df, 'using 1:2 with lines', 'using 1:3 with points',
-           grid = '')
-
-2) We have two means to pass "unset" command, one is the no-xxx option and
-   the other is xxx = None, for examples we'd like to unset the grid and
-   xrange::
-
-    unset grid
-    unset xrange
-
-We can do that in py-gnuplot by:
-
-.. code-block:: python
-
-    g = gnuplot.Gnuplot()
-    # Example of use no-xxx to unset the flag
-    g.plot(df, 'using 0:2:3:4:5 notitle with financebars lt 8',
-            ...,
-            nogrid = '',
-            noxlabel = '',
-            ...)
-
-    # Example of use None to unset the flag
-    g.plot(df, 'using 0:2:3:4:5 notitle with financebars lt 8',
-            ...,
-            grid = None,
-            xlabel = None,
-            ...)
-
-3) If there is multiple lines for one options, for exampe in gnuplot it
-   is::
-
-    set arrow from 5,-5,-1.2 to 5,5,-1.2 lt -1
-    set arrow from 5,6,-1 to 5,5,-1 lt -1
-    set arrow from 5,6,sinc(5,5) to 5,5,sinc(5,5) lt -1
-
-We pass them by a list of options:
-
-.. code-block:: python
-
-    g = gnuplot.Gnuplot()
-    g.plot(df,
-           'using 0:2:3:4:5 notitle with financebars lt 8',
-           ...,
-           arrow = ['from 5,-5,-1.2 to 5,5,-1.2 lt -1',
-                    'from 5,6,-1 to 5,5,-1 lt -1',
-                    'from 5,6,sinc(5,5) to 5,5,sinc(5,5) lt -1'],
-           ...,
-           ...)
-
-2.1.6 splot()
-+++++++++++++
-
-.. code-block:: python
-
     def splot(self, *items, **kwargs):
         '''
         *items: The list of plot command;
         **kwargs: The options that would be set before the plot command.
         '''
 
-The usage of splot() is exactly the same as plot().
+Every plot/splot command would be a parameter in plot()/splot() functions. Like
+set()/unset(), all the parameters must be string since it would be pas sed to
+gnuplot without any change. You need to change them to string if they are not::
+
+    #gnplot
+    plot d1(x) fs solid 1.0 lc rgb "forest-green" title "μ =  0.5 σ = 0.5", \
+     d2(x) lc rgb "gold" title "μ =  2.0 σ = 1.0", \
+     d3(x) lc rgb "dark-violet" title "μ = -1.0 σ = 2.0"
+
+    #py-gnplot
+    g.plot('d1(x) fs solid 1.0 lc rgb "forest-green" title "μ =  0.5 σ = 0.5"',
+            'd2(x) lc rgb "gold" title "μ =  2.0 σ = 1.0"',
+            'd3(x) lc rgb "dark-violet" title "μ = -1.0 σ = 2.0"')
 
-2.2 new developed member functions for python generated data
---------------------------------------------------------------
+1.5 plot_data()/splot_data()
+--------------------------------------
 
-We develop the following memember functions, they are very familar with the
-orignal plot() and splot(), the only difference is that , in the new
-developed function, we pass the python generated data as the first
-parameter and remove the corresponding element in the plot command.
+.. Note:: in older release, they are called plot_data()/splot_data(), I'd like to chnage them to the new name since they are more intuitive.
 
-2.2.1 plot_data()
-+++++++++++++++++
+Definition:
 
 .. code-block:: python
 
     def plot_data(self, data, *items, **kwargs):
         '''
         data: The data that need to be plotted. It's either the string of list
         or the Pnadas Dataframe, if it's Pnadas Dataframe it would be converted
         to string by data.to_csv(). Note that we will execut a extra command
         "set datafile separator "," to fit the data format of csv.
         *items: The list of plot command;
         **kwargs: The options that would be set before the plot command.
         '''
-
-The usage is the same as in `2.1.5 plot()`_ except that you should pass the
-data(string or pandas Dataframe format) as the first parameter, and remove
-the corresponding filename in every plot line. Moreover, the defaulst
-seperator now is "," for easy use with csv file:
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-    # usage examples, please note that we didn't give the output so could only
-    # see the image flash on the screen. Will introduce how to output the
-    # image to files.
-    df = pd.DataFrame(data = {'col1': [1, 2],
-                              'col2': [3, 4],
-                              'col3': [5, 6]})
-    g = gnuplot.Gnuplot()
-    # Note that the first parameter is df and there is no "data.file" in
-    # the following commmand.
-    g.plot_data(df,
-                'using 1:2 with lines',
-                'using 1:3 with points')
-
-2.2.2 splot_data()
-++++++++++++++++++
-
-.. code-block:: python
-
     def splot_data(self, data, *items, **kwargs):
         '''
         data: The data that need to be plotted. It's either the string of list
         or the Pnadas Dataframe, if it's Pnadas Dataframe it would be converted
         to string by data.to_csv(). Note that we will execut a extra command
         "set datafile separator "," to fit the data format of csv.
         *items: The list of plot command;
         **kwargs: The options that would be set before the plot command.
         '''
 
-The usage is the same as in `2.2.1 plot_data()`_ .
+With above functions: constructor, Set()/unset(), plot()/splot(), we can do
+what gnuplot do, but it cannot plot python generated data. It's hard to
+implement the new functions with the existing gnuplot command, so we develop
+two new functions: plot_data()/splot_data(). They are much like
+plot()/splot(), the only difference is:
+
+    * plot()/splot() take function(filename) in every plot command.
+    * plot_data()/splot_data() take the dataframe as the first
+      parameter, while remove function(filename) in every plot commmand
+
+for examples::
+
+    #plot(): 'finance.dat' is in plot command
+    g.plot("'finance.dat' using 0:($6/10000) notitle with impulses lt 3",
+           "'finance.dat' using 0:($7/10000) notitle with lines lt 1")
 
-2.3 new developed global class-less function call
-----------------------------------------------------
+    #plot_data(): the first parameter must be dataframe, every plot
+    #command doesn't take the data.
+    g.plot_data(df,
+            'using 0:($6/10000) notitle with impulses lt 3',
+            'using 0:($7/10000) notitle with lines lt 1')
 
-We can plot the image just by the above object-oriented interface, but
-sometimes we want to quick plot an image in quick mode, we can call the
-global class-less function call:
+See `histograms.2.py`_ and `histograms.2.py`_ for differences.
 
-2.3.1 plot()
-++++++++++++
+1.6 multiplot
+------------------
 
-.. code-block:: python
+To plot multiplot, you must set multiplot at first as in gnuplot. Here is examples.
 
-    #submodule gnuplot
-    def plot(*args, **kwargs):
-        '''
-        *items: The list of plot command;
-        **kwargs: The options that would be set before the plot command.
-        '''
+1.7 quick mode
+------------------
 
-The usage is the same as in `2.1.5 plot()`_ except that you needn't
-allocate a Gnuplot() instance at first:.
+For some easy case, we can combine the following step into one.
 
-.. _simple3.py:
+    1) Enter gnuplot conext;
+    2) Set plotting style;
+    3) Define some expressions;
+    4) Plotting.
 
-..
-    cmd2img:: python3
-    :image: simple.1.png
+For examples:
 
+.. _simple2.1.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
 
     gnuplot.plot('[-10:10] sin(x)',
            'atan(x)',
            'cos(atan(x))',
            terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400',
            output = '"simple.1.png"',
-           key = 'fixed left top vertical Right lt black linewidth 1.000 dashtype solid',
+           key = 'fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid',
            samples = '50, 50',
-           title = '"Simple Plots" font ",20" norotate')
-
-2.3.2 splot()
-++++++++++++++
-
-.. code-block:: python
-
-    #submodule gnuplot
-    def splot(*args, **kwargs):
-        '''
-        *items: The list of plot command;
-        **kwargs: The options that would be set before the plot command.
-        '''
-
-The usage is the same as in `2.1.6 splot()`_ except that you needn't
-allocate a Gnuplot() instance at first:
-
-2.3.3 plot_data()
-+++++++++++++++++
-
-.. code-block:: python
-
-    def plot_data(data, *items, **kwargs):
-        '''
-        data: The data that need to be plotted. It's either the string of list
-        or the Pnadas Dataframe, if it's Pnadas Dataframe it would be converted
-        to string by data.to_csv()
-        *items: The list of plot command;
-        **kwargs: The options that would be set before the plot command.
-        '''
-
-The usage is the same as in `2.2.1 plot_data()`_ except that you needn't
-allocate a Gnuplot() instance at first:
+           title = '"Simple Plots" font ",20" textcolor lt -1 norotate',
+           xrange = '[ * : * ] noreverse writeback',
+           x2range = '[ * : * ] noreverse writeback',
+           yrange = '[ * : * ] noreverse writeback',
+           y2range = '[ * : * ] noreverse writeback',
+           zrange = '[ * : * ] noreverse writeback',
+           cbrange = '[ * : * ] noreverse writeback',
+           rrange = '[ * : * ] noreverse writeback',
+           colorbox = 'vertical origin screen 0.9, 0.2 size screen 0.05, 0.6 front noinvert bdefault')
 
+.. _whale2.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
+    import pandas as pd
 
-    df = pd.DataFrame(data = {'col1': [1, 2],
-                              'col2': [3, 4],
-                              'col3': [5, 6]})
-    gnuplot.plot_data(df,
-                      'using 1:2 with lines',
-                      'using 1:3 with points')
-
-2.3.4 splot_data()
-++++++++++++++++++
-
-.. code-block:: python
-
-    class gnuplot.Gnuplot(object):
-
-        def splot(self, *items, **kwargs):
-            '''
-            *items: The list of plot command;
-            **kwargs: The options that would be set before the plot command.
-            '''
-
-The usage is the same as in `2.2.2 splot_data()`_ except that you needn't
-allocate a Gnuplot() instance at first:
-
-2.3.5 multiplot()
-+++++++++++++++++
-
-Since we don't allocate the Gnuplot instance, there is a little trick to
-plot the multiplot image. To solve the issue we create 3 brand new function
-to implement that.
-
-.. code-block:: python
-
-    def multiplot(\*args, \*\*kwargs):
-        @args: the subplot object list;
-        @kwargs: the setting options that need to be set before call plot;
-
-    def make_plot(\*args, \*\*kwargs)
-        The parameter definition is the same as plot(), but it doesn't plot
-        the data really, it only return the plot dictionary for later
-        multiplot() use.
-
-    def make_splot(\*args, \*\*kwargs)
-        The parameter definition is the same as splot(), but it doesn't plot
-        the data really, it only return the plot dictionary for later
-        multiplot() use.
-
-    def make_plot_data (data, \*args, \*\*kwargs)
-        The parameter definition is the same as plot_data(), but it doesn't
-        plot the data really, it only return the plot dictionary for later
-        multiplot() use.
-
-    def make_splot_data (data, \*args, \*\*kwargs)
-        The parameter definition is the same as splot_data(), but it
-        doesn't plot the data really, it only return the plot dictionary
-        for later multiplot() use.
-
-Before call multiplot() we must generate the subplot object by calling
-make_plot()/make_splot(), It is much like mplfinance.make_addplot(), it only
-add the subplot command for further call:
+    #https://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.html
+    gnuplot.splot('"examples/whale.dat" w pm3d',
+            term = 'pngcairo size 480,480',
+            out = '"whale.png"',
+            style = 'line 100 lw 0.1 lc "black"',
+            pm3d = 'depth hidden3d ls 100',
+            cbrange = '[-0.5:0.5]',
+            palette = 'rgb -3,-3,-3',
+            colorbox = None,
+            border = None,
+            key = None,
+            zrange = '[-2:2]',
+            tics = None,
+            view = '60,185,1.5')
 
+.. _histograms2.2.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
+    import pandas as pd
 
-    sub1 = gnuplot.make_plot('sin(x)', ylabel = 'ylabel')
-    sub2 = gnuplot.make_plot('cos(x)', xlabel = 'xlabel')
-    sub3 = gnuplot.make_plot('sin(2*x)', noxlabel = '', ylabel = '')
-    sub4 = gnuplot.make_plot('cos(2*x)', xlabel = 'xlabel')
-    gnuplot.multiplot(sub1, sub2, sub3, sub4,
-                      output = '"sample.multiplot.png"',
-                      term = 'pngcairo size 900,600 font ",11"',
-                      multiplot  = 'layout 2,2 columnsfirst margins 0.1,0.9,0.1,0.9 spacing 0.1')
-
-A example in reality:
-
-.. _finance2.py:
-
-..
-    cmd2img:: python3
-    :image: finance.13.png
+    df = pd.read_csv('examples/immigration.dat', index_col = 0, sep='\t', comment='#')
+    gnuplot.plot_data(df,
+            'using 2:xtic(1), for [i=3:22] "" using i ',
+            terminal = 'pngcairo transparent enhanced font "arial,10" fontscale 1.0 size 600, 400 ',
+            output = '"histograms.1.png"',
+            key = 'fixed right top vertical Right noreverse noenhanced autotitle nobox',
+            style = 'data linespoints',
+            datafile = ' missing "-"',
+            xtics = 'border in scale 1,0.5 nomirror rotate by -45 autojustify norangelimit',
+            title = '"US immigration from Europe by decade"')
 
+.. _surface2.9.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
-    import pandas as pd
-
-    # A demostration to generate pandas data frame data in python.
-    df = pd.read_csv('examples/finance.dat',
-            sep='\t',
-            index_col = 0,
-            parse_dates = True,
-            names = ['date', 'open','high','low','close', 'volume','volume_m50',
-                'intensity','close_ma20','upper','lower '])
-
-    # make subplot at first, now there is still no real plot.
-    sub1 = gnuplot.make_plot_data(df,
-            'using 0:2:3:4:5 notitle with candlesticks lt 8',
-            'using 0:9 notitle with lines lt 3',
-            'using 0:10 notitle with lines lt 1',
-            'using 0:11 notitle with lines lt 2',
-            'using 0:8 axes x1y2 notitle with lines lt 4',
-            title = '"Change to candlesticks"',
-            logscale = 'y',
-            xrange = '[50:253]',
-            yrange = '[75:105]',
-            format = 'x ""',
-            xtics = '(66, 87, 109, 130, 151, 174, 193, 215, 235)',
-            ytics = '(105, 100, 95, 90, 85, 80)',
-            lmargin = '9',
-            rmargin = '2',
-            bmargin = '0',
-            origin = '0, 0.3',
-            size = ' 1, 0.7',
-            grid = 'xtics ytics',
-            ylabel = '"price" offset 1',
-            label = ['1 "Acme Widgets" at graph 0.5, graph 0.9 center front',
-                '2 "Courtesy of Bollinger Capital" at graph 0.01, 0.07',
-                '3 "  www.BollingerBands.com" at graph 0.01, 0.03']
-            )
 
-    sub2 = gnuplot.make_plot_data(df,
-            'using 0:($6/10000) notitle with impulses lt 3',
-            'using 0:($7/10000) notitle with lines lt 1',
-            ytics = '500',
-            xtics = '("6/03" 66, "7/03" 87, "8/03" 109, "9/03" 130, "10/03" 151, "11/03" 174, "12/03" 193, "1/04" 215, "2/04" 235)',
-            ylabel = '"volume (0000)" offset 1',
-            nologscale = 'y',
-            autoscale = 'y',
-            size = '1.0, 0.3',
-            origin = '0.0, 0.0',
-            bmargin = '',
-            tmargin = '0',
-            format = ['x', 'y "%1.0f"'])
+    #py-gnuplot: https://gnuplot.sourceforge.net/demo/surface2.9.gnu
+    gnuplot.splot('cos(u)+.5*cos(u)*cos(v),sin(u)+.5*sin(u)*cos(v),.5*sin(v) with lines',
+            '1+cos(u)+.5*cos(u)*cos(v),.5*sin(v),sin(u)+.5*sin(u)*cos(v) with lines',
+            terminal = 'pngcairo enhanced font "arial,10" fontscale 1.0 size 600, 400 ',
+            output = '"surface2.9.png"',
+            dummy = 'u, v',
+            key = 'bmargin center horizontal Right noreverse enhanced autotitle nobox',
+            style = ['data lines'],
+            parametric = '',
+            view = '50, 30, 1, 1',
+            isosamples = '50, 20',
+            hidden3d = 'back offset 1 trianglepattern 3 undefined 1 altdiagonal bentover',
+            xyplane = 'relative 0',
+            title = '"Interlocking Tori" ',
+            urange = '[ -3.14159 : 3.14159 ] noreverse nowriteback',
+            vrange = '[ -3.14159 : 3.14159 ] noreverse nowriteback')
 
-    # plot at one time.
-    gnuplot.multiplot(sub1, sub2,
-            output = '"finance.13.png"',
-            term = 'pngcairo font "arial,10" fontscale 1.0 size 900, 600')
+2. Examples
+=============
 
-.. _3 Multiplot Axes Demo2:
+2.1 plot/splot function
+-------------------------------
 
+.. _simple.1.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
-    import pandas as pd
-    import numpy as np
-
-    #https://matplotlib.org/gallery/subplots_axes_and_figures/axes_demo.html#sphx-glr-gallery-subplots-axes-and-figures-axes-demo-py
-    #http://gnuplot.sourceforge.net/demo_5.2/bins.html
-
-    # 1) create some data to use for the plot
-    np.random.seed(19680801) # Fixing random state for reproducibility
-    dt = 0.001
-    t = np.arange(0.0, 10.0, dt)
-    r = np.exp(-t / 0.05)  # impulse response
-    x = np.random.randn(len(t))
-    s = np.convolve(x, r)[:len(x)] * dt  # colored noise
-    df = pd.DataFrame({'r': r, 'x': x, 's': s}, index = t)
-    df.index.name = 't'
-    #print(df.tail().to_csv())
-
-    # 2) Plot the data
-    main = gnuplot.make_plot_data(df.iloc[:1000],
-            'using 1:4 with line lw 2 lc "web-blue"',
-            title = '"Gaussian colored noise"',
-            xlabel = '"time (s)"',
-            ylabel = '"current (nA)"',
-            xrange = '[0:1]',
-            yrange = '[-0.015:0.03]',
-            key = None,
-            size = ' 1, 1',
-            origin = '0, 0')
-    right = gnuplot.make_plot_data(df,
-            'using 4 bins=400 with boxes title "20 bins" lw 2 lc "web-blue"',
-            title = '"Probability"',
-            xlabel = None,
-            ylabel = None,
-            tics = None,
-            xrange = None,
-            yrange = None,
-            origin = '0.65, 0.56',
-            size = '0.24, 0.32',
-            object = 'rectangle from graph 0,0 to graph 1,1 behind fc "black" fillstyle solid 1.0')
-    left = gnuplot.make_plot_data(df,
-            'using 1:2 with line lw 2 lc "web-blue"',
-            title = '"Impulse response"',
-            xrange = '[0:0.2]',
-            origin = '0.15, 0.56',
-            size = '0.24, 0.32')
 
-    gnuplot.multiplot(main, right, left,
-            output = '"sphx_glr_axes_demo_001.png"',
-            term = 'pngcairo font "arial,10" fontscale 1.0 size 640, 480',
-            key = '')
+    #py-gnuplot: https://gnuplot.sourceforge.net/demo_6.0/simple.html
 
-3. examples
-============
+    #Ceate a gnuplot context. with "log = True" to print the gnuplot execute log.
+    g = gnuplot.Gnuplot(log = True)
 
-3.1 examples port from gnuplot
-------------------------------
+    #Set plotting style
+    g.set(terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400',
+           output = '"simple.1.png"',
+           key = 'fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid',
+           samples = '50, 50',
+           title = '"Simple Plots" font ",20" textcolor lt -1 norotate',
+           xrange = '[ * : * ] noreverse writeback',
+           x2range = '[ * : * ] noreverse writeback',
+           yrange = '[ * : * ] noreverse writeback',
+           y2range = '[ * : * ] noreverse writeback',
+           zrange = '[ * : * ] noreverse writeback',
+           cbrange = '[ * : * ] noreverse writeback',
+           rrange = '[ * : * ] noreverse writeback',
+           colorbox = 'vertical origin screen 0.9, 0.2 size screen 0.05, 0.6 front  noinvert bdefault')
 
-3.1.1 finance
-+++++++++++++
+    #Expressions and caculations
+    g.cmd("NO_ANIMATION = 1")
 
-example with object-oriented interface call:
+    #Plotting
+    g.plot("[-10:10] sin(x)", "atan(x)", "cos(atan(x))")
 
-.. _finance1.py:
+This is the output: 
 
-..
-    cmd2img:: python3
-    :image: finance.13.png
+|simple.1.png|
 
+.. _surface.9.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
-    import pandas as pd
-
-    # A demostration to generate pandas data frame data in python.
-    df = pd.read_csv('examples/finance.dat',
-            sep='\t',
-            index_col = 0,
-            parse_dates = True,
-            names = ['date', 'open','high','low','close', 'volume','volume_m50',
-                'intensity','close_ma20','upper','lower '])
-
-    # Create a Gnuplot instance and set the options at first;
-    g = gnuplot.Gnuplot(log = True,
-            output = '"finance.13.png"',
-            term = 'pngcairo font "arial,10" fontscale 1.0 size 900, 600',
-            multiplot = True)
-
-    g.plot_data(df,
-            'using 0:2:3:4:5 notitle with candlesticks lt 8',
-            'using 0:9 notitle with lines lt 3',
-            'using 0:10 notitle with lines lt 1',
-            'using 0:11 notitle with lines lt 2',
-            'using 0:8 axes x1y2 notitle with lines lt 4',
-            title = '"Change to candlesticks"',
-            logscale = 'y',
-            xrange = '[50:253]',
-            yrange = '[75:105]',
-            format = 'x ""',
-            xtics = '(66, 87, 109, 130, 151, 174, 193, 215, 235)',
-            ytics = '(105, 100, 95, 90, 85, 80)',
-            lmargin = '9',
-            rmargin = '2',
-            bmargin = '0',
-            origin = '0, 0.3',
-            size = ' 1, 0.7',
-            grid = 'xtics ytics',
-            ylabel = '"price" offset 1',
-            label = ['1 "Acme Widgets" at graph 0.5, graph 0.9 center front',
-                '2 "Courtesy of Bollinger Capital" at graph 0.01, 0.07',
-                '3 "  www.BollingerBands.com" at graph 0.01, 0.03'],
-            )
-
-    g.plot_data(df,
-            'using 0:($6/10000) notitle with impulses lt 3',
-            'using 0:($7/10000) notitle with lines lt 1',
-            bmargin = '',
-            size = '1.0, 0.3',
-            origin = '0.0, 0.0',
-            tmargin = '0',
-            nologscale = 'y',
-            autoscale = 'y',
-            format = ['x', 'y "%1.0f"'],
-            ytics = '500',
-            xtics = '("6/03" 66, "7/03" 87, "8/03" 109, "9/03" 130, "10/03" 151, "11/03" 174, "12/03" 193, "1/04" 215, "2/04" 235)',
-            ylabel = '"volume (0000)" offset 1')
 
-Since it enable the log options, I attach the execution log as below::
+    #py-gnuplot: https://gnuplot.sourceforge.net/demo_6.0/simple.html
 
-    [py-gnuplot 19:35:26] set output "finance.13.png"
-    [py-gnuplot 19:35:26] set term pngcairo font "arial,10" fontscale 1.0 size 900, 600
-    [py-gnuplot 19:35:26] set multiplot
-    [py-gnuplot 19:35:26] set datafile separator ","
-    [py-gnuplot 19:35:26] set title "Change to candlesticks"
-    [py-gnuplot 19:35:26] set logscale y
-    [py-gnuplot 19:35:26] set xrange [50:253]
-    [py-gnuplot 19:35:26] set yrange [75:105]
-    [py-gnuplot 19:35:26] set format x ""
-    [py-gnuplot 19:35:26] set xtics (66, 87, 109, 130, 151, 174, 193, 215, 235)
-    [py-gnuplot 19:35:26] set ytics (105, 100, 95, 90, 85, 80)
-    [py-gnuplot 19:35:26] set lmargin 9
-    [py-gnuplot 19:35:26] set rmargin 2
-    [py-gnuplot 19:35:26] set bmargin 0
-    [py-gnuplot 19:35:26] set origin 0, 0.3
-    [py-gnuplot 19:35:26] set size  1, 0.7
-    [py-gnuplot 19:35:26] set grid xtics ytics
-    [py-gnuplot 19:35:26] set ylabel "price" offset 1
-    [py-gnuplot 19:35:26] set label 1 "Acme Widgets" at graph 0.5, graph 0.9 center front
-    [py-gnuplot 19:35:26] set label 2 "Courtesy of Bollinger Capital" at graph 0.01, 0.07
-    [py-gnuplot 19:35:26] set label 3 "  www.BollingerBands.com" at graph 0.01, 0.03
-    [py-gnuplot 19:35:26] plot $DataFrame using 0:2:3:4:5 notitle with candlesticks lt 8,\
-    [py-gnuplot 19:35:26] $DataFrame using 0:9 notitle with lines lt 3,\
-    [py-gnuplot 19:35:26] $DataFrame using 0:10 notitle with lines lt 1,\
-    [py-gnuplot 19:35:26] $DataFrame using 0:11 notitle with lines lt 2,\
-    [py-gnuplot 19:35:26] $DataFrame using 0:8 axes x1y2 notitle with lines lt 4
-    [py-gnuplot 19:35:26] unset for [i=1:200] label i
-    [py-gnuplot 19:35:26] set datafile separator ","
-    [py-gnuplot 19:35:26] set bmargin
-    [py-gnuplot 19:35:26] set size 1.0, 0.3
-    [py-gnuplot 19:35:26] set origin 0.0, 0.0
-    [py-gnuplot 19:35:26] set tmargin 0
-    [py-gnuplot 19:35:26] set nologscale y
-    [py-gnuplot 19:35:26] set autoscale y
-    [py-gnuplot 19:35:26] set format x
-    [py-gnuplot 19:35:26] set format y "%1.0f"
-    [py-gnuplot 19:35:26] set ytics 500
-    [py-gnuplot 19:35:26] set xtics ("6/03" 66, "7/03" 87, "8/03" 109, "9/03" 130, "10/03" 151, "11/03" 174, "12/03" 193, "1/04" 215, "2/04" 235)
-    [py-gnuplot 19:35:26] set ylabel "volume (0000)" offset 1
-    [py-gnuplot 19:35:26] plot $DataFrame using 0:($6/10000) notitle with impulses lt 3,\
-    [py-gnuplot 19:35:26] $DataFrame using 0:($7/10000) notitle with lines lt 1
-    [py-gnuplot 19:35:26] unset for [i=1:200] label i
+    #Ceate a gnuplot context. with "log = True" to print the gnuplot execute log.
+    g = gnuplot.Gnuplot(log = True)
 
-And the generated output is as following:
+    #Set plotting style
+    g.set(terminal = 'pngcairo  transparent enhanced font "arial,10" fontscale 1.0 size 600, 400',
+            output = "'surface2.9.png'",
+            dummy = 'u, v',
+            key = 'bmargin center horizontal Right noreverse enhanced autotitle nobox',
+            parametric = '',
+            view = '50, 30, 1, 1',
+            isosamples = '50, 20',
+            hidden3d = 'back offset 1 trianglepattern 3 undefined 1 altdiagonal bentover',
+            style = ['data lines'],
+            xyplane = 'relative 0',
+            title = '"Interlocking Tori" ',
+            urange = '[ -3.14159 : 3.14159 ] noreverse nowriteback',
+            vrange = '[ -3.14159 : 3.14159 ] noreverse nowriteback',
+            colorbox = 'vertical origin screen 0.9, 0.2 size screen 0.05, 0.6 front  noinvert bdefault')
 
-.. image:: http://gnuplot.sourceforge.net/demo/finance.13.png
-   :width: 350
+    #Expressions and caculations
+    g.cmd("NO_ANIMATION = 1")
 
-3.1.2 histogram
-+++++++++++++++
+    #Plotting
+    g.splot("cos(u)+.5*cos(u)*cos(v)",
+            "sin(u)+.5*sin(u)*cos(v)",
+            ".5*sin(v) with lines",
+            "1+cos(u)+.5*cos(u)*cos(v)",
+            ".5*sin(v),sin(u)+.5*sin(u)*cos(v) with lines",
+            )
 
-.. _histo.1.py:
+This is the output: 
 
-..
-    cmd2img:: python3
-    :image: histograms.1.png
+|surface2.9.png|
 
-Plot with member functions:
+2.2 plot/splot file
+-------------------------------
 
+.. _histograms.2.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
 
-    df = pd.read_csv('examples/immigration.dat', index_col = 0, sep='\t', comment='#')
-    g = gnuplot.Gnuplot()
-    g.set(terminal = 'pngcairo transparent enhanced font "arial,10" fontscale 1.0 size 600, 400 ',
-            output = '"histograms.1.png"',
-            key = 'fixed right top vertical Right noreverse noenhanced autotitle nobox',
-            style = 'data linespoints',
-            datafile = ' missing "-"',
-            xtics = 'border in scale 1,0.5 nomirror rotate by -45 autojustify norangelimit',
-            title = '"US immigration from Europe by decade"')
-    g.plot_data(df, 'using 2:xtic(1), for [i=3:22] "" using i ')
-
-Since it's simple, we can plot it quick way:
-
-.. _histo.2.py:
-
-..
-    cmd2img:: python3
-    :image: histograms.1.png
-
-.. code-block:: python
+    #Histograms demo example comes from
+    #https://gnuplot.sourceforge.net/demo_6.0/histograms.2.gnu
 
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-    import pandas as pd
+    #1) Ceate a gnuplot context
+    g = gnuplot.Gnuplot(log = True)
 
-    df = pd.read_csv('examples/immigration.dat', index_col = 0, sep='\t', comment='#')
-    gnuplot.plot_data(df,
-            'using 2:xtic(1), for [i=3:22] "" using i ',
-            terminal = 'pngcairo transparent enhanced font "arial,10" fontscale 1.0 size 600, 400 ',
-            output = '"histograms.1.png"',
+    #2) Set plotting style
+    g.set(terminal = 'pngcairo  transparent enhanced font "arial,10" fontscale 1.0 size 600, 400',
+            output = "'histograms.2.png'",
+            boxwidth = '0.9 absolute',
+            style = ['fill   solid 1.00 border lt -1',
+                'histogram clustered gap 1 title textcolor lt -1',
+                'data histograms' ],
             key = 'fixed right top vertical Right noreverse noenhanced autotitle nobox',
-            style = 'data linespoints',
-            datafile = ' missing "-"',
-            xtics = 'border in scale 1,0.5 nomirror rotate by -45 autojustify norangelimit',
-            title = '"US immigration from Europe by decade"')
+            datafile = "missing '-'",
+            xtics = ["border in scale 0,0 nomirror rotate by -45  autojustify",
+                "norangelimit ",
+                " ()"],
+            title = '"US immigration from Northern Europe\\nPlot selected data columns as histogram of clustered boxes"',
+            xrange = '[ * : * ] noreverse writeback',
+            x2range = '[ * : * ] noreverse writeback',
+            yrange  = '[ 0.00000 : 300000. ] noreverse writeback',
+            y2range = '[ * : * ] noreverse writeback',
+            zrange = '[ * : * ] noreverse writeback',
+            cbrange = '[ * : * ] noreverse writeback',
+            rrange = '[ * : * ] noreverse writeback',
+            colorbox = 'vertical origin screen 0.9, 0.2 size screen 0.05, 0.6 front  noinvert bdefault')
 
-And the generated output is as following:
-
-.. image:: http://gnuplot.sourceforge.net/demo/histograms.1.png
-   :width: 350
+    #3) Expressions and caculations
+    g.cmd("NO_ANIMATION = 1")
 
-3.1.3 splot
-+++++++++++
+    #4) Plotting
+    g.plot("'examples/immigration.dat' using 6:xtic(1) ti col",
+            "'' u 12 ti col",
+            "'' u 13 ti col",
+            "'' u 14 ti col")
 
-.. _surface1.py:
+This is the output: 
 
-..
-    cmd2img:: python3
-    :image: surface2.9.png
+|histograms.2.png|
 
-object-oriented function call:
+Another example is to splot a pm3d image:
 
+.. _whale.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
 
-    g = gnuplot.Gnuplot(output = '"surface2.9.png"',
-            terminal = 'pngcairo enhanced font "arial,10" fontscale 1.0 size 600, 400 ',
-            title = '"Interlocking Tori" ',
-            dummy = 'u, v',
-            key = 'bmargin center horizontal Right noreverse enhanced autotitle nobox',
-            style = ['increment default','data lines'],
-            parametric = '',
-            view = '50, 30, 1, 1',
-            isosamples = '50, 20',
-            hidden3d = 'back offset 1 trianglepattern 3 undefined 1 altdiagonal bentover',
-            xyplane = 'relative 0',
-            urange = '[ -3.14159 : 3.14159 ] noreverse nowriteback',
-            vrange = '[ -3.14159 : 3.14159 ] noreverse nowriteback')
-    g.splot('cos(u)+.5*cos(u)*cos(v),sin(u)+.5*sin(u)*cos(v),.5*sin(v) with lines',
-            '1+cos(u)+.5*cos(u)*cos(v),.5*sin(v),sin(u)+.5*sin(u)*cos(v) with lines')
+    #Whale example comes from
+    #https://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.html
 
-.. _surface2.py:
+    #Ceate a gnuplot context
+    g = gnuplot.Gnuplot(log = True)
 
-Direct function call example:
+    #Set plotting style
+    g.set(term = 'pngcairo size 480,480',
+            output = '"whale.png"',
+            style = 'line 100 lw 0.1 lc "black"',
+            pm3d = 'depth hidden3d ls 100',
+            cbrange = '[-0.5:0.5]',
+            palette = 'rgb -3,-3,-3',
+            colorbox = None,
+            border   = None,
+            key = None,
+            zrange = '[-2:2]',
+            tics  = None,
+            view = '60,185,1.5')
 
-..
-    cmd2img:: python3
-    :image: surface2.9.png
+    #No Expressions
+
+    #Plotting
+    g.splot('"examples/whale.dat" w pm3d')
 
+The generated image is as below:
+
+|whale.png|
+
+2.3 plot/splot python generated data
+----------------------------------------------
+
+.. _histograms3.2.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
+    import pandas as pd
 
-    gnuplot.splot('cos(u)+.5*cos(u)*cos(v),sin(u)+.5*sin(u)*cos(v),.5*sin(v) with lines',
-            '1+cos(u)+.5*cos(u)*cos(v),.5*sin(v),sin(u)+.5*sin(u)*cos(v) with lines',
-            terminal = 'pngcairo enhanced font "arial,10" fontscale 1.0 size 600, 400 ',
-            output = '"surface2.9.png"',
-            dummy = 'u, v',
-            key = 'bmargin center horizontal Right noreverse enhanced autotitle nobox',
-            style = ['data lines'],
-            parametric = '',
-            view = '50, 30, 1, 1',
-            isosamples = '50, 20',
-            hidden3d = 'back offset 1 trianglepattern 3 undefined 1 altdiagonal bentover',
-            xyplane = 'relative 0',
-            title = '"Interlocking Tori" ',
-            urange = '[ -3.14159 : 3.14159 ] noreverse nowriteback',
-            vrange = '[ -3.14159 : 3.14159 ] noreverse nowriteback')
+    #Histograms demo example comes from
+    #https://gnuplot.sourceforge.net/demo_6.0/histograms.2.gnu
 
-And the generated output is as following:
+    #1) Ceate a gnuplot context
+    g = gnuplot.Gnuplot(log = True)
 
-.. image:: http://gnuplot.sourceforge.net/demo/surface2.9.png
-   :width: 350
+    #2) Set plotting style
+    g.set(terminal = 'pngcairo  transparent enhanced font "arial,10" fontscale 1.0 size 600, 400',
+            output = "'histograms.2.png'",
+            boxwidth = '0.9 absolute',
+            style = ['fill   solid 1.00 border lt -1',
+                'histogram clustered gap 1 title textcolor lt -1',
+                'data histograms' ],
+            key = 'fixed right top vertical Right noreverse noenhanced autotitle nobox',
+            datafile = "missing '-'",
+            xtics = ["border in scale 0,0 nomirror rotate by -45  autojustify",
+                "norangelimit ",
+                " ()"],
+            title = '"US immigration from Northern Europe\\nPlot selected data columns as histogram of clustered boxes"',
+            xrange = '[ * : * ] noreverse writeback',
+            x2range = '[ * : * ] noreverse writeback',
+            yrange  = '[ 0.00000 : 300000. ] noreverse writeback',
+            y2range = '[ * : * ] noreverse writeback',
+            zrange = '[ * : * ] noreverse writeback',
+            cbrange = '[ * : * ] noreverse writeback',
+            rrange = '[ * : * ] noreverse writeback',
+            colorbox = 'vertical origin screen 0.9, 0.2 size screen 0.05, 0.6 front  noinvert bdefault')
+
+    #3) Expressions and caculations
+    g.cmd("NO_ANIMATION = 1")
+    #The original example is plotting file, it's easy. To demonstrate plotting
+    #data generated in python, we transform the data into df for demonstration.
+    df = pd.read_csv('examples/immigration.dat', index_col = 0, sep='\t', comment='#')
 
-3.1.4 pm3d
-++++++++++
+    #4) Plotting
+    g.plot_data(df,
+            'using 6:xtic(1) ti col',
+            'u 12 ti col',
+            'u 13 ti col',
+            'u 14 ti col')
 
-iterate.dem
+The generated image is as below:
 
-.. _whale1.py:
+|histograms.2.png|
 
-..
-    cmd2img:: python3
-    :image: whale.png
+2.4 multiplot examples
+------------------------------
 
+.. _finance.13.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
+    import pandas as pd
 
-    #http://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.html
-    g = gnuplot.Gnuplot()
-    # Black and white version
-    g.splot('"examples/whale.dat" w pm3d',
-            term = 'pngcairo size 480,480',
-            out = '"whale.png"',
-            style = 'line 100 lw 0.1 lc "black"',
-            pm3d = 'depth hidden3d ls 100',
-            cbrange = '[-0.5:0.5]',
-            palette = 'rgb -3,-3,-3',
-            colorbox = None,
-            border = None,
-            key = None,
-            zrange = '[-2:2]',
-            tics = None,
-            view = '60,185,1.5')
+    #Transparent demo example comes from
+    #https://gnuplot.sourceforge.net/demo_6.0/finance.html
 
+    #Ceate a gnuplot context
+    g = gnuplot.Gnuplot(log = True)
 
-.. _whale2.py:
+    #Set plotting style
+    g.set(output = "'finance.13.png'",
+            term = 'pngcairo  transparent enhanced font "arial,8" fontscale 1.0 size 660, 320',
+            label = ['1 "Acme Widgets" at graph 0.5, graph 0.9 center front',
+                '2 "Courtesy of Bollinger Capital" at graph 0.01, 0.07',
+                '3 "  www.BollingerBands.com" at graph 0.01, 0.03'],
+            logscale = 'y',
+            yrange = '[75:105]',
+            ytics = '(105, 100, 95, 90, 85, 80)',
+            xrange = '[50:253]',
+            grid = '',
+            lmargin = '9',
+            rmargin = '2',
+            format = 'x ""',
+            xtics = '(66, 87, 109, 130, 151, 174, 193, 215, 235)',
+            multiplot = True)
+
+    #3) Expressions and caculations
 
-..
-    cmd2img:: python3
-    :image: whale.png
+    #4) Plotting: Since multiplot = True, we plot two subplot
+    g.plot("'finance.dat' using 0:2:3:4:5 notitle with candlesticks lt 8",
+            "'finance.dat' using 0:9 notitle with lines lt 3",
+            "'finance.dat' using 0:10 notitle with lines lt 1",
+            "'finance.dat' using 0:11 notitle with lines lt 2",
+            "'finance.dat' using 0:8 axes x1y2 notitle with lines lt 4",
+            title = '"Change to candlesticks"',
+            size = ' 1, 0.7',
+            origin = '0, 0.3',
+            bmargin = '0',
+            ylabel = '"price" offset 1')
+    g.plot("'finance.dat' using 0:($6/10000) notitle with impulses lt 3",
+            "'finance.dat' using 0:($7/10000) notitle with lines lt 1",
+            bmargin = '',
+            format = ['x', 'y "%1.0f"'],
+            size = '1.0, 0.3',
+            origin = '0.0, 0.0',
+            tmargin = '0',
+            nologscale = 'y',
+            autoscale = 'y',
+            ytics = '500',
+            xtics = '("6/03" 66, "7/03" 87, "8/03" 109, "9/03" 130, "10/03" 151, "11/03" 174, "12/03" 193, "1/04" 215, "2/04" 235)',
+            ylabel = '"volume (0000)" offset 1')
 
+.. _finance3.13.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
 
-    # Black and white version
-    gnuplot.splot('"examples/whale.dat" w pm3d',
-            term = 'pngcairo size 480,480',
-            out = '"whale.png"',
-            style = 'line 100 lw 0.1 lc "black"',
-            pm3d = 'depth hidden3d ls 100',
-            cbrange = '[-0.5:0.5]',
-            palette = 'rgb -3,-3,-3',
-            colorbox = None,
-            border = None,
-            key = None,
-            zrange = '[-2:2]',
-            tics = None,
-            view = '60,185,1.5')
+    #Transparent demo example comes from
+    #https://gnuplot.sourceforge.net/demo_6.0/finance.html
 
-And the generated output is as following:
+    #Ceate a gnuplot context
+    g = gnuplot.Gnuplot(log = True)
 
-.. http://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.html
-.. image http://gnuplot.sourceforge.net/demo/iterate.2.png
-.. image:: http://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.png
-   :width: 350
+    #Set plotting style
+    g.set(output = "'finance.13.png'",
+            term = 'pngcairo  transparent enhanced font "arial,8" fontscale 1.0 size 660, 320',
+            label = ['1 "Acme Widgets" at graph 0.5, graph 0.9 center front',
+                '2 "Courtesy of Bollinger Capital" at graph 0.01, 0.07',
+                '3 "  www.BollingerBands.com" at graph 0.01, 0.03'],
+            logscale = 'y',
+            yrange = '[75:105]',
+            ytics = '(105, 100, 95, 90, 85, 80)',
+            xrange = '[50:253]',
+            grid = '',
+            lmargin = '9',
+            rmargin = '2',
+            format = 'x ""',
+            xtics = '(66, 87, 109, 130, 151, 174, 193, 215, 235)',
+            multiplot = True)
+
+    #3) Expressions and caculations
+    #A demostration to generate pandas data frame data in python.
+    df = pd.read_csv('examples/finance.dat',
+            sep='\t',
+            index_col = 0,
+            parse_dates = True,
+            names = ['date', 'open','high','low','close', 'volume','volume_m50',
+                'intensity','close_ma20','upper','lower '])
+
+    #4) Plotting: Since multiplot = True, we plot two subplot
+    g.plot_data(df,
+            'using 0:2:3:4:5 notitle with candlesticks lt 8',
+            'using 0:9 notitle with lines lt 3',
+            'using 0:10 notitle with lines lt 1',
+            'using 0:11 notitle with lines lt 2',
+            'using 0:8 axes x1y2 notitle with lines lt 4',
+            title = '"Change to candlesticks"',
+            size = ' 1, 0.7',
+            origin = '0, 0.3',
+            bmargin = '0',
+            ylabel = '"price" offset 1')
+    g.plot_data(df,
+            'using 0:($6/10000) notitle with impulses lt 3',
+            'using 0:($7/10000) notitle with lines lt 1',
+            bmargin = '',
+            format = ['x', 'y "%1.0f"'],
+            size = '1.0, 0.3',
+            origin = '0.0, 0.0',
+            tmargin = '0',
+            nologscale = 'y',
+            autoscale = 'y',
+            ytics = '500',
+            xtics = '("6/03" 66, "7/03" 87, "8/03" 109, "9/03" 130, "10/03" 151, "11/03" 174, "12/03" 193, "1/04" 215, "2/04" 235)',
+            ylabel = '"volume (0000)" offset 1')
+
+Both script generate the same output image:
 
-3.2 Examples port from matplotlib
----------------------------------
+|finance.13.png|
+
+2.5 Examples port from matplotlib
+-----------------------------------
 
 Just for fun, I translate some examples in matplotlib to py-gnuplot:
 
-3.2.1 Stacked bar chart
+2.5.1 Stacked bar chart
 +++++++++++++++++++++++
 
-..
-    .. cmd2img:: python3
-        :image: sphx_glr_bar_stacked_001.png
-
+.. _sphx_glr_bar_stacked_001.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
 
@@ -1322,27 +873,22 @@
             boxwidth = '%s' %(width),
             xrange = '[0.5:5.5]',
             ylabel = '"Scores"',
             title = '"Scores by group and gender"',
             output = '"sphx_glr_bar_stacked_001.png"',
             terminal = 'pngcairo size 640, 480')
 
-Refer to the original script: `Stacked bar chart`_ and the original image:
+This is the output:
 
-.. _Stacked bar chart: https://matplotlib.org/gallery/lines_bars_and_markers/bar_stacked.html#sphx-glr-gallery-lines-bars-and-markers-bar-stacked-py
-.. image:: https://matplotlib.org/_images/sphx_glr_bar_stacked_001.png
-   :width: 350
+|sphx_glr_bar_stacked_001.png|
 
-3.2.2 Grouped bar chart with labels
+2.5.2 Grouped bar chart with labels
 +++++++++++++++++++++++++++++++++++
 
-..
-    cmd2img:: python3
-            :image: sphx_glr_barchart_001.png
-
+.. _sphx_glr_barchart_001.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
 
@@ -1369,27 +915,22 @@
             style = ['data histogram',
                      'histogram cluster gap 1',
                      'fill solid border -1',
                      'textbox transparent'],
             output = '"sphx_glr_barchart_001.png"',
             terminal = 'pngcairo size 640, 480')
 
-Refer to the original script: `Grouped bar chart with labels`_ and the original image:
+This is the output:
 
-.. _Grouped bar chart with labels: https://matplotlib.org/gallery/lines_bars_and_markers/barchart.html#sphx-glr-gallery-lines-bars-and-markers-barchart-py
-.. image:: https://matplotlib.org/_images/sphx_glr_barchart_001.png
-   :width: 350
+|sphx_glr_barchart_001.png|
 
-3.2.3 Multiplot Axes Demo
+2.5.3 Multiplot Axes Demo
 +++++++++++++++++++++++++
 
-..
-    cmd2img:: python3
-            :image: sphx_glr_axes_demo_001.png
-
+.. _sphx_glr_axes_demo_001.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
     import numpy as np
@@ -1438,27 +979,22 @@
     g.plot_data(df,
             'using 1:2 with line lw 2 lc "web-blue"',
             title = '"Impulse response"',
             xrange = '[0:0.2]',
             origin = '0.15, 0.56',
             size = '0.24, 0.32')
 
-Refer to the original script: `Multiplot Axes Demo`_ and the original image:
+This is the output:
 
-.. _Multiplot Axes Demo: https://matplotlib.org/gallery/subplots_axes_and_figures/axes_demo.html#sphx-glr-gallery-subplots-axes-and-figures-axes-demo-py
-.. image:: https://matplotlib.org/_images/sphx_glr_axes_demo_001.png
-   :width: 350
+|sphx_glr_axes_demo_001.png|
 
-3.2.4 control view and zoom 
+2.5.4 control view and zoom 
 ++++++++++++++++++++++++++++
 
-..
-    cmd2img:: python3
-            :image: sphx_glr_axes_margins_001.png
-
+.. _sphx_glr_axes_margins_001.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
 
@@ -1493,79 +1029,69 @@
             xrange = '[0: 3]',
             yrange = '[-0.7: 1]',
             xtics = '0, 0.5, 3',
             ytics = '-0.5, 0.5, 1',
             origin = '0, 0',
             size = '1, 0.5')
 
-Refer to the original script: `axes_margins.py`_ and the original image:
+This is the output:
 
-.. _axes_margins.py: https://matplotlib.org/_downloads/4d3bc54481c3ff3a1ac6712bc2904875/axes_margins.py
-.. image:: https://matplotlib.org/_images/sphx_glr_axes_margins_001.png
-   :width: 350
+|sphx_glr_axes_margins_001.png|
 
-3.2.5 Rendering math equation using TeX
+2.5.5 Rendering math equation using TeX
 +++++++++++++++++++++++++++++++++++++++
 
 We can embed the TeX math equation into the gnuplot generated image by setting
 the epslatex terminal, it would be rendered as a .tex file, you can import it
 directly or you can convert it to .pdf file and then .png file if needed. this
 is the example:
 
-..
-    cmd2img:: python3
-    :image: pygnuplot_tex_demo.tex
-
+.. _sphx_glr_tex_demo_001.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
 
     # https://matplotlib.org/gallery/text_labels_and_annotations/tex_demo.html#sphx-glr-gallery-text-labels-and-annotations-tex-demo-py
     # http://wap.sciencenet.cn/blog-373392-500657.html
     # https://www.thinbug.com/q/17593917
     g = gnuplot.Gnuplot(log = True,
-            output = '"pygnuplot_tex_demo.tex"',
+            output = '"sphx_glr_tex_demo_001.tex"',
             term = 'epslatex standalone lw 2 color colortext')
 
     # NOTE: In the following example, we need to escape the "\", that means we
     # should use '\\' or "\\\\" for \
     g.plot('cos(4*pi*x) + 2',
             xlabel = "'\\textbf{time (s)}'",
             ylabel = "'\\textit{Velocity (\N{DEGREE SIGN}/sec)}'",
             title = "'\\TeX\\ is Number $\\displaystyle\\sum_{n=1}^\\infty\\frac{-e^{i\\pi}}{2^n}$!' tc 'red'",
             key = None,
             xrange = '[0: 1]')
 
+This is the output:
+
+|sphx_glr_tex_demo_001.png|
+
 I list the script output since it's with the log=True::
 
-    [py-gnuplot 14:56:13] set output "pygnuplot_tex_demo.tex"
+    [py-gnuplot 14:56:13] set output "sphx_glr_tex_demo_001.tex"
     [py-gnuplot 14:56:13] set term epslatex standalone lw 2 color colortext
     [py-gnuplot 14:56:13] set xlabel '\textbf{time (s)}'
     [py-gnuplot 14:56:13] set ylabel '\textit{Velocity (°/sec)}'
     [py-gnuplot 14:56:13] set title '\TeX\ is Number $\displaystyle\sum_{n=1}^\infty\frac{-e^{i\pi}}{2^n}$!' tc 'red'
     [py-gnuplot 14:56:13] unset key
     [py-gnuplot 14:56:13] set xrange [0: 1]
     [py-gnuplot 14:56:13] plot cos(4*pi*x) + 2
 
-Refer to the original script: `Rendering math equation using TeX`_ and the original image:
-
-.. _Rendering math equation using TeX: https://matplotlib.org/gallery/text_labels_and_annotations/tex_demo.html#sphx-glr-gallery-text-labels-and-annotations-tex-demo-py
-.. image:: https://matplotlib.org/_images/sphx_glr_tex_demo_001.png
-   :width: 350
-
-3.2.6 Basic pie chart
+2.5.6 Basic pie chart
 +++++++++++++++++++++
 
-..
-    cmd2img:: python3
-    :image: sphx_glr_pie_features_0011.png
-
+.. _sphx_glr_pie_features_0011.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
     import math
@@ -1588,60 +1114,55 @@
     df = df.fillna(startangle)
     #print(df)
 
     pie_shade = []
     pie_graph = []
 
     shade_offset = 0.03
+    g = gnuplot.Gnuplot(log = True,
+            output = '"sphx_glr_pie_features_0011.png"',
+            term = 'pngcairo size 640, 480',
+            key = None,
+            parametric = "",
+            border = "",
+            tics = "",
+            multiplot = True)
+
     for k, v in df.iterrows():
         #print(k,v)
         cos = math.cos((v['start']+v['end'])/2)
         sin = math.sin((v['start']+v['end'])/2)
 
         # If we'd like explode the piece, ad the dx/dy to move the origi point.
         dx = v['explode'] * cos
         dy = v['explode'] * sin
 
         # make the shade for each piece
-        piece = gnuplot.make_plot('cos(t)+%f, sin(t)+%f with filledcurves xy=%f,%f lc "grey80"'
-                    %(dx-shade_offset, dy-shade_offset, dx-shade_offset, dy-shade_offset),
+        g.plot('cos(t)+%f, sin(t)+%f with filledcurves xy=%f,%f lc "grey80"'
+                %(dx-shade_offset, dy-shade_offset, dx-shade_offset, dy-shade_offset),
                 trange = '[%f:%f]' %(v['start'], v['end']),
                 xrange = '[-1.5:1.5]',
                 yrange = '[-1.5:1.5]')
-        pie_shade.append(piece)
 
         # make the pie and label
-        piece = gnuplot.make_plot('cos(t)+%f, sin(t)+%f with filledcurve xy=%f,%f  lt %d'
-                    %(dx, dy, dx, dy, k+3),
+        g.plot('cos(t)+%f, sin(t)+%f with filledcurve xy=%f,%f  lt %d'
+                %(dx, dy, dx, dy, k+3),
                 trange = '[%f:%f]' %(v['start'], v['end']),
                 xrange = '[-1.5:1.5]',
                 yrange = '[-1.5:1.5]',
-                label = ['1 "%s" at %f, %f center front' %(v['labels'], 1.2*cos+dx, 1.2*sin+dy),
-                    '2 "%.1f%%" at %f, %f center front' %(v['percentage']*100, 0.6*cos, 0.6*sin)])
-        pie_graph.append(piece)
+                label = ['1 "%s" at %f, %f center front' %(v['labels'], 1.2*cos+dx, 1.2*sin+dy), '2 "%.1f%%" at %f, %f center front' %(v['percentage']*100, 0.6*cos, 0.6*sin)])
 
-    gnuplot.multiplot(*pie_shade, *pie_graph,
-            output = '"sphx_glr_pie_features_0011.png"',
-            terminal = 'pngcairo size 640, 480',
-            key = None,
-            parametric = '',
-            border = '',
-            tics = '',
-            multiplot = True)
+This is the output:
 
-Refer to the original script: `Basic pie chart`_ and the original image:
+|sphx_glr_pie_features_0011.png|
 
-.. _Basic pie chart: https://matplotlib.org/gallery/pie_and_polar_charts/pie_features.html#sphx-glr-gallery-pie-and-polar-charts-pie-features-py
-.. image:: https://matplotlib.org/_images/sphx_glr_pie_features_0011.png
-   :width: 350
-
-4. Q/A
+3. Q/A
 =======
 
-5. CHANGLOG
+4. CHANGLOG
 =============
 
 1.0 Initial upload;
 
 1.0.3 Now Gnuplot().plot()/splot() supplot set options as parameters.
 
 1.0.7 The pyplot.plot() now can accept both string and pandas.Dataframe as the
@@ -1662,10 +1183,17 @@
 1.1.2 Enhancement: If it's multiplot mode, automatically call the following
 Gnuplot to unset the label:
 
     g.unset('for [i=1:200] label i')
 
 1.1.3 Enhancement: When plotting the python generated data, we set the
 seperator to "," for easy using it in csv file.
+
 1.1.5 Bug fix: on some case it exit exceptionally.
+
 1.1.8 Remove some Chinese comments to remove the "UnicodeDecodeError" for some users.
+
 1.1.9 1) Run and update the examples in gnuplot6.0.0. 2) If you'd like enable multiplot, you shuld use  multimplot = True to replace multimplot = "".
+
+1.1.13 Document update.
+
+
```

### Comparing `py-gnuplot-1.1.9/py_gnuplot.egg-info/PKG-INFO` & `py-gnuplot-1.2.0/py_gnuplot.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,1315 +1,853 @@
 Metadata-Version: 2.1
 Name: py-gnuplot
-Version: 1.1.9
+Version: 1.2.0
 Summary: py-gnuplot is a python plot tools based on gnuplot.
 Home-page: http://www.gnuplot.info
 Author: Yongping Guo
 Author-email: guoyoooping@163.com
 License: GPLv3
 Keywords: gnuplot,pandas
 Platform: UNKNOWN
 Requires-Python: >=3.6
 License-File: LICENSE.txt
 
 .. meta::
    :description: gnuplot plotting backend for python.
    :keywords: gnuplot, py-gnuplot, pandas, python, plot
 
-Gnuplot is a portable command-line driven graphing utility for many
-platforms. To leverage the powful gnuplot to plot beautiful image in
-efficicent way in python, we port gnuplot to python. Let's see an example
-at first:
-
-..
-    cmd2img:: python3
-    :image: simple.1.png
+Gnuplot is a powerful command-line driven graphing utility for many platforms.
+To leverage the powful gnuplot to plot beautiful image in efficicent way in
+python, we port gnuplot to python. 
 
+We develop **set()/unset()** function to set or unset gnuplot plotting style,
+**plot()/splot()** to operate gnuplot plot or splot command, **cmd()** to
+execute any commands that coulnd't be done by the above functions. They are
+intuative and gnuplot users can swith to py-gnuplot naturally. By this means we
+can do what gnuplot do.
+
+.. image:: https://gnuplot.sourceforge.net/demo_6.0/transparent.2.png
+    :align: right
+    :width: 300
+
+But for plotting python generated data the above functions are not enough. We
+develop **plot_data()/splot_data()** to plot data generated in
+python.
+
+Here is a quick examples to generate the right image with only basic functions,
+more examples which plot python generated data are coming in later sections.
+
+.. _sphinx-plot-directive: https://pypi.org/project/sphinx-plot-directive
+
+.. _quick_example.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
 
-    gnuplot.plot('[-10:10] sin(x)',
-           'atan(x)',
-           'cos(atan(x))',
-           terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400',
-           output = '"simple.1.png"',
-           key = 'fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid',
-           samples = '50, 50',
-           title = '"Simple Plots" font ",20" textcolor lt -1 norotate',
-           xrange = '[ * : * ] noreverse writeback',
-           x2range = '[ * : * ] noreverse writeback',
-           yrange = '[ * : * ] noreverse writeback',
-           y2range = '[ * : * ] noreverse writeback',
-           zrange = '[ * : * ] noreverse writeback',
-           cbrange = '[ * : * ] noreverse writeback',
-           rrange = '[ * : * ] noreverse writeback',
-           colorbox = 'vertical origin screen 0.9, 0.2 size screen 0.05, 0.6 front noinvert bdefault',
-           #NO_ANIMATION = '1', #I don't know what's this. Who know? please tell me. Thanks.
-           )
-
-From the example we can see, we plot the function with plot() function, with
-all the options as the function parameters. It's easy to understand and comply
-with both gnuplot and python's grammer. The generated image is as below:
-
-.. figure:: http://gnuplot.sourceforge.net/demo/simple.1.png 
-   :width: 350
+    #py-gnuplot: A quick demo
 
-   figure 1. pygnuplot demo 1: simple function
+    #Ceate a gnuplot context. with "log = True" to print the gnuplot execute log.
+    g = gnuplot.Gnuplot(log = True)
 
-Let's see the detail in the below:
+    #Set plotting style
+    g.set(terminal = 'pngcairo transparent enhanced font "arial,8" fontscale 1.0 size 512, 280 ',
+            output = '"quick_example.png"',
+            style = ["fill transparent solid 0.50 noborder", "data lines", "function filledcurves y1=0"],
+            key = 'title "Gaussian Distribution" center fixed left top vertical Left reverse enhanced autotitle nobox noinvert samplen 1 spacing 1 width 0 height 0',
+            title = '"Transparent filled curves"',
+            xrange = '[ -5.00000 : 5.00000 ] noreverse nowriteback',
+            yrange = '[ 0.00000 : 1.00000 ] noreverse nowriteback')
 
-.. contents:: [Contents]
-   :depth: 3
+    #Expressions and caculations
+    g.cmd('Gauss(x,mu,sigma) = 1./(sigma*sqrt(2*pi)) * exp( -(x-mu)**2 / (2*sigma**2) )',
+            'd1(x) = Gauss(x, 0.5, 0.5)',
+            'd2(x) = Gauss(x,  2.,  1.)',
+            'd3(x) = Gauss(x, -1.,  2.)')
 
-1. Introduction and examples list
-===================================
+    #Plotting
+    g.plot('d1(x) fs solid 1.0 lc rgb "forest-green" title "μ =  0.5 σ = 0.5"',
+            'd2(x) lc rgb "gold" title "μ =  2.0 σ = 1.0"',
+            'd3(x) lc rgb "dark-violet" title "μ = -1.0 σ = 2.0"')
 
-As we know Gnuplot is a portable and powerful command-line driven graphing
-utility for many platforms. To leverage the power of Gnuplot, We develop
-the py-gnuplot in a easy understand way.
-
-**py-python only support python3** since the function dictionary paramaters in
-python2 is not in order.
-
-This package has an object-oriented design as well as direct function call to
-allows the user flexibility to set plot options and to run multiple gnuplot
-sessions simultaneously. So in this document, every examples are rendered in
-two way: quick plot mode and object-oriented. Either mode works and you can
-choose which way you like.
-
-We will introduce it in detail in the following chapter and here list the
-exaples used in this article as below:
-
-.. _Table1:
-
-.. list-table:: Table1 : A demostration of pygnuplot.gnuplot script
-   :widths: 15, 20, 20, 70
-   :header-rows: 1
-
-   * - gnuplot demo script
-     - object-oriented interface script
-     - direct function call script
-     - All the script produce the same image
-   * - `simple.dem`_
-     - simple2.py_
-     - simple3.py_
-     - |simple.1.png|
-   * - `surface2.dem`_
-     - surface1.py_
-     - surface2.py_
-     - |surface2.9.png|
-   * - `iterate.dem`_
-     - whale1.py_
-     - whale2.py_
-     - |whale.png|
+more examples:
 
-.. _Table2:
+.. _simple.1.gnu: http://gnuplot.sourceforge.net/demo/simple.1.gnu
+.. _surface2.9.gnu: http://gnuplot.sourceforge.net/demo/surface2.9.gnu
+.. _histograms.1.gnu: http://gnuplot.sourceforge.net/demo/histograms.1.gnu
+.. _iterate.2.gnu: http://gnuplot.sourceforge.net/demo/iterate.2.gnu
+.. _finance.13.gnu: http://gnuplot.sourceforge.net/demo/finance.13.gnu
 
-.. list-table:: Table 2: A demostration of plot() and plot_data()
-   :widths: 15, 20, 20, 70
-   :header-rows: 1
-
-   * - gnuplot demo script
-     - object-oriented interface script
-     - direct function call script
-     - All the script produce the same image
-   * - `histo.1.gnu`_
-     - histo.1.py_
-     - histo.2.py_
-     - |histograms.1.png|
-   * - `finance.dem`_
-     - finance1.py_
-     - finance1.py_
-     - |finance.13.png|
-
-.. list-table:: Table 3: Examples porting from Matplotlib
-   :widths: 35, 35, 35, 35
-   :header-rows: 0
-
-   * - `3.2.1 Stacked bar chart`_ |sphx_glr_bar_stacked_001.png|
-     - `3.2.2 Grouped bar chart with labels`_ |sphx_glr_barchart_001.png|
-     - `3.2.3 Multiplot Axes Demo`_ |sphx_glr_axes_demo_001.png|
-     - `3.2.4 control view and zoom`_ |sphx_glr_axes_margins_001.png|
-   * - `3.2.5 Rendering math equation using TeX`_ |sphx_glr_tex_demo_001.png|
-     - `3.2.6 Basic pie chart`_ |sphx_glr_pie_features_0011.png|
-     - 
-     - 
-
-.. _simple.dem: http://gnuplot.sourceforge.net/demo/simple.1.gnu
-.. _surface2.dem: http://gnuplot.sourceforge.net/demo/surface2.9.gnu
-.. _histo.1.gnu: http://gnuplot.sourceforge.net/demo/histograms.1.gnu
-.. _iterate.dem: http://gnuplot.sourceforge.net/demo/iterate.2.gnu
-.. _finance.dem: http://gnuplot.sourceforge.net/demo/finance.13.gnu
 .. |simple.1.png| image:: http://gnuplot.sourceforge.net/demo/simple.1.png
-   :width: 180
+   :width: 350
 .. |surface2.9.png| image:: http://gnuplot.sourceforge.net/demo/surface2.9.png
-   :width: 180
+   :width: 350
 .. |finance.13.png| image:: http://gnuplot.sourceforge.net/demo/finance.13.png
-   :width: 180
+   :width: 350
 .. |iterate.2.png| image:: http://gnuplot.sourceforge.net/demo/iterate.2.png
-   :width: 180
+   :width: 350
 .. |whale.png| image:: http://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.png
-   :width: 180
-.. |histograms.1.png| image:: http://gnuplot.sourceforge.net/demo/histograms.1.png
-   :width: 180
+   :width: 350
+.. |histograms.2.png| image:: http://gnuplot.sourceforge.net/demo/histograms.2.png
+   :width: 350
 .. |sphx_glr_bar_stacked_001.png| image:: https://matplotlib.org/_images/sphx_glr_bar_stacked_001.png
-   :width: 180
+   :width: 350
 .. |sphx_glr_barchart_001.png| image:: https://matplotlib.org/_images/sphx_glr_barchart_001.png
-   :width: 180
+   :width: 350
 .. |sphx_glr_axes_demo_001.png| image:: https://matplotlib.org/_images/sphx_glr_axes_demo_001.png
-   :width: 180
+   :width: 350
 .. |sphx_glr_pie_features_0011.png| image:: https://matplotlib.org/_images/sphx_glr_pie_features_0011.png
-   :width: 180
+   :width: 350
 .. |sphx_glr_tex_demo_001.png| image:: https://matplotlib.org/_images/sphx_glr_tex_demo_001.png
-   :width: 180
+   :width: 350
 .. |sphx_glr_axes_margins_001.png| image:: https://matplotlib.org/_images/sphx_glr_axes_margins_001.png
-   :width: 180
+   :width: 350
 
-2. Plot elements in py-gnuplot
-=================================
+.. list-table:: Table1 : plot examples with different script
+
+   * - examples
+     - plot function
+     - plot file
+     - splot function
+     - splot file
+     - multiplot
+   * - figure
+     - |simple.1.png|
+     - |histograms.2.png|
+     - |surface2.9.png|
+     - |whale.png|
+     - |finance.13.png|
+   * - gnuplot script
+     - `simple.1.gnu`_
+     - `histograms.1.gnu`_
+     - `surface2.9.gnu`_
+     - `iterate.2.gnu`_
+     - `finance.13.gnu`_
+   * - py-gnuplot script
+     - `simple.1.py`_
+     - `histograms.2.py`_
+     - `surface.9.py`_
+     - `whale.py`_
+     - `finance.13.py`_
+   * - py-gnuplot quick mode
+     - `simple2.1.py`_
+     - `histograms2.2.py`_
+     - `surface2.9.py`_
+     - `whale2.py`_
+     -  N/A(too complicated)
+   * - py-gnuplot data generated in python
+     - N/A
+     - `histograms3.2.py`_
+     - N/A
+     - N/A
+     - `finance3.13.py`_
+
+.. list-table:: Table2 : examples porting from matplotlib
+   :widths: 30,30,30
+
+   * - `sphx_glr_bar_stacked_001.py`_ |sphx_glr_bar_stacked_001.png|
+     - `sphx_glr_barchart_001.py`_ |sphx_glr_barchart_001.png|
+     - `sphx_glr_axes_demo_001.py`_ |sphx_glr_axes_demo_001.png|
+   * - `sphx_glr_axes_margins_001.py`_ |sphx_glr_axes_margins_001.png|
+     - `sphx_glr_tex_demo_001.py`_ |sphx_glr_tex_demo_001.png|
+     - `sphx_glr_pie_features_0011.py`_ |sphx_glr_pie_features_0011.png|
 
-As we know, gnuplot use commands to plot all kinds of image, we port almost all
-the useful commands as functions in py-gnuplot.
+Let's see the detail.
 
-In `2.1 member functions port from Gnuplot`_ we introduce the member
-functions that we can plot all what Gnuplot could do, The limitation is
-it's not so easy to plot the python generated data with the those existing
-command.
+.. contents:: [Contents]
+   :depth: 2
 
-To plot the data generated in python, we develop additional functions as
-below, ::
+1. Introduction
+=================
 
-    plot_data(self, data, *items, **kwargs):
-    splot_data(self, data, *items, **kwargs)
+As we know, to plot a image in gnuplot we do:
 
-they are almost the same as the original plot()/splot(), the difference is
-we pass the data as the first parameter, you don't give the filename in the
-plot command, see detail in `2.2 new developed member functions for python
-generated data`_ .
+    1) Enter gnuplot conext;
+    2) Set plotting style;
+    3) Define some expressions;
+    4) Plotting.
 
-Sometime we only need simple plot and don't want to allocate a Gnuplot
-instance, we develop the quick way to plot: `2.3 new developed global
-class-less function call`_ and you can plot the image in a easy way with
-global class-less function call.
+We translate gnuplot's main function into python ones, and each one do the same
+thing as gnuplot. As in `quick_example.py`_ we also have 4 steps to plot an
+image::
 
-2.1 member functions port from Gnuplot
----------------------------------------
+    #Constructor
+    g = gnuplot.Gnuplot()
+    #Set plotting style
+    g.set()
+    #Expressions and caculations
+    g.cmd()
+    #Plotting
+    g.plot()
 
-The principle is if you can write Gnuplot script, you can write py-gnuplot.
-There is 1-1 mapping between almost all Gnuplot command and python
-function;
+1.1 constructor
+----------------
 
-2.1.1 The constructor
-+++++++++++++++++++++
+Defenition:
 
 .. code-block:: python
 
     def __init__(self, *args, log = False, **kwargs):
         '''
         *args: The flag parameter in gnuplot
         log: If print the gnuplot log
         **kwargs: the flag that need to be set. You can also set them in the set() function.
         '''
 
-When create the Gnuplot instance, you can pass some parameter to it, you
-can also set them when you call set() or plot(), they are the same.
-
-The "log" parameter is a new added flag to indicate if we print the gnuplot
-execution log when run. For example:
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-    #See original gnuplot script here:
-    #http://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.html
-    g = gnuplot.Gnuplot(log = True,
-            term = 'pngcairo size 480,480',
-            out = '"whale.png"',
-            pm3d = 'depth hidden3d ls 100',
-            cbrange = '[-0.5:0.5]',
-            palette = 'rgb -3,-3,-3',
-            colorbox = None,
-            border = None,
-            key = None,
-            zrange = '[-2:2]',
-            tics = None,
-            view = '60,185,1.5')
-    g.splot('"examples/whale.dat" w pm3d')
-
-This is the script output with the log=True::
-
-    [py-gnuplot] set term pngcairo size 480,480
-    [py-gnuplot] set out "whale.png"
-    [py-gnuplot] set pm3d depth hidden3d ls 100
-    [py-gnuplot] set cbrange [-0.5:0.5]
-    [py-gnuplot] set palette rgb -3,-3,-3
-    [py-gnuplot] unset colorbox
-    [py-gnuplot] unset border
-    [py-gnuplot] unset key
-    [py-gnuplot] set zrange [-2:2]
-    [py-gnuplot] unset tics
-    [py-gnuplot] set view 60,185,1.5
-    [py-gnuplot] splot "examples/whale.dat" w pm3d
-
-And this is the image output: |small_whale.png|
-
-.. |small_whale.png| image:: http://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.png
-   :width: 50
-
-2.1.2 cmd()
-+++++++++++
-
-.. code-block:: python
-
-    def cmd(self, *args):
-        '''
-        *args: all the line that need to pass to gnuplot. It could be a
-        list of lines, or a paragraph; Lines starting with "#" would be
-        omitted. Every line should be a clause that could be executed in
-        gnuplot.
-        '''
-
-We implemented the function cmd() and pass the command to call Gnuplot to plot
-the data, Thus we could do everything with the only one simple function:
+We call g = gnuplot.Gnuplot(log = True) to get a gnuplot context. Here log = True means to print the gnuplot log when call gnuplot functions.::
 
-.. _simple1.1.py:
-..
-    cmd2img:: python3
-    :image: simple.1.png
+    #Ceate a gnuplot context. with "log = True" to print the gnuplot execute log.
+    g = gnuplot.Gnuplot(log = True)
 
-.. code-block:: python
+1.2 Set()/unset()
+------------------
 
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-    # Illustration of object-oriented interface, you can see we only wrap the
-    # gnuplot script by g.cmd('...') and it's simple and straitfoward if you
-    # are familar with Gnuplot.
-    g = gnuplot.Gnuplot()
-    g.cmd('set terminal pngcairo font "arial,10" fontscale 1.0 size 600, 400')
-    g.cmd('set output "simple.1.png"')
-    g.cmd('set key fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid')
-    g.cmd('set samples 50, 50')
-    g.cmd('set title "Simple Plots" ')
-    g.cmd('set title  font ",20" norotate')
-    g.cmd('plot [-10:10] sin(x),atan(x),cos(atan(x))')
-
-Or you can even pass the Gnuplot command as a string list or a text paragraph:
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-    # Illustration of cmd(), you can see we only wrap the
-    # gnuplot script by g.cmd('...') and it's simple and straitfoward if you
-    # are familar with Gnuplot.
-    g = gnuplot.Gnuplot()
-
-    # Take all the Gnuplot command as a list of command:
-    g.cmd('set terminal pngcairo font "arial,10" fontscale 1.0 size 600, 400',
-    'set output "simple.1.png"',
-    'set key fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid',
-    'set samples 50, 50',
-    'set title "Simple Plots" ',
-    'set title  font ",20" norotate',
-    'plot [-10:10] sin(x),atan(x),cos(atan(x))')
-
-    # Another means, take all the Gnuplot command as a script paragraph,
-    #uncomment the following code block to have a try.
-    #plot_cmd = '''
-    #set terminal pngcairo font "arial,10" fontscale 1.0 size 600, 400
-    #set output "simple.1.png"
-    #set key fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid
-    #set samples 50, 50
-    #set title "Simple Plots
-    #set title  font ",20" norotate
-    #plot [-10:10] sin(x),atan(x),cos(atan(x))'''
-    #g.cmd(plot_cmd)
-
-This is the image output: |small_simple.png|
-
-.. |small_simple.png| image:: http://gnuplot.sourceforge.net/demo/simple.1.png
-   :width: 50
-
-By this means we can do everything that Gnuplot can do and cannot do what
-Gnuplot itself can't do. It's the exact way that the Gnuplot do it. and we
-don't get any benifit besides we can call Gnuplot in python. So we develop
-many other functions as below:
-
-2.1.3 set()
-+++++++++++
+Defenition:
 
 .. code-block:: python
 
     def set(self, *args, **kwargs):
         '''
         *args: options without value
         *kwargs: options with value. The set and unset commands may optionally
                  contain an iteration clause, so the arg could be list.
         '''
+    def unset(self, *items):
+        '''
+        *args: options that need to be unset
+        '''
 
-The set command can be used to set lots of options. The set and unset
-commands may optionally contain an iteration clause, so the arg could be
-list. For examples:
-
-We set the options before plot and then call plot to render the image. It's
-equivalent to example in `2.1.2 cmd()`_ but seems muck like a python script.
-
-.. _simple2.py:
-
-..
-    cmd2img:: python3
-    :image: simple.1.png
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-
-    # Gnuplot lines:
-    #set terminal pngcairo font "arial,10" fontscale 1.0 size 600, 400
-    #set output "simple.1.png"
-    #set key fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid
-    #set samples 50, 50
-    #set title "Simple Plots" font ",20" norotate
+After enter gnuplot context, normally we need to set the plotting style. For
+example we need to set the terminal and output at first in gnuplt as following::
 
-    g = gnuplot.Gnuplot()
-    g.set(terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400',
-            output = '"simple.1.png"',
-            key = 'fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid',
-            samples = '50, 50',
-            title = '"Simple Plots" font ",20" norotate')
-    g.plot('[-10:10] sin(x),atan(x),cos(atan(x))')
-
-set() is flexible but indeed set() functions is not necessary. We could
-pass the options as parameter in the constructor and plot(). For examples
-the following script act equally with the above:
+    set terminal pngcairo  transparent enhanced font "arial,8" fontscale 1.0 size 512, 280 
+    set output 'transparent.2.png'
 
-.. code-block:: python
+Then we translate the set into set() function as following, please not that all
+the elment are stirng, so must add extra quoto and it would be passed to
+gnuplot without any change. Pleae note that all the parameters must be string
+since it would be passed to gnuplot without any change. You need to change them
+to string if they are not::
+
+    #Set plotting style
+    g.set(terminal = 'pngcairo transparent enhanced font "arial,8" fontscale 1.0 size 512, 280 ',
+            output = '"quick_example.png"',
+            ...
+            )
 
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
+For unset we have flexible ways to do that, for exampes the following ways are
+the same::
 
-    # py-python lines:
-    g = gnuplot.Gnuplot(terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400',
-            output = '"test.png"',
-            boxwidth = '0.9 relative',
-            style = 'fill solid 1.0',
-            label = ['"y=x" at 1,2',
-                '2 "S" at graph 0.5,0.5 center font "Symbol,24"',
-                '3 "y=x^2" at 2,3,4 right'])
-            g.plot('"file.dat" with boxes')
+    #gnuplot unset
+    unset colorbox
 
-We can also write it as the following, they are all the same:
+    #py-gnuplot means1
+    g.unset(colorbox)
 
-.. code-block:: python
+    #py-gnuplot means2
+    g.set(colorbox = None)
 
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
+    #py-gnuplot means3
+    g.set(nocolorbox = "")
 
-    # py-python lines:
-    g = gnuplot.Gnuplot()
-    g.plot('"file.dat" with boxes',
-           terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400',
-           output = '"test.png"',
-           boxwidth = '0.9 relative',
-           style = 'fill solid 1.0',
-           label = ['"y=x" at 1,2',
-                    '2 "S" at graph 0.5,0.5 center font "Symbol,24"',
-                    '3 "y=x^2" at 2,3,4 right'])
+1.3 cmd()
+----------
 
-2.1.4 unset()
-+++++++++++++++
+Defenition:
 
 .. code-block:: python
 
-    def unset(self, *items):
+    def cmd(self, *args):
         '''
-        *args: options that need to be unset
+        *args: all the line that need to pass to gnuplot. It could be a
+        list of lines, or a paragraph; Lines starting with "#" would be
+        omitted. Every line should be a clause that could be executed in
+        gnuplot.
         '''
 
-Options set using the set() function may be returned to their default state by
-the corresponding unset() function:
+Sometimes before plot we need define some variable or caculations, call cmd() functions to do::
 
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-    # py-python lines:
-    g = gnuplot.Gnuplot(terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400', output = '"test.png"')
-    g.unset('xlabel', 'ylabel', 'xrange', 'yrange')
-    g.plot('sin(x) with lp')
-
-unset command could be replaced as set, for example the above example could
-also be writen as:
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
+    #gnuplot
+    Gauss(x,mu,sigma) = 1./(sigma*sqrt(2*pi)) * exp( -(x-mu)**2 / (2*sigma**2) )
+    d1(x) = Gauss(x, 0.5, 0.5)
+    d2(x) = Gauss(x,  2.,  1.)
+    d3(x) = Gauss(x, -1.,  2.)
+
+    #py-gnuplot
+    g.cmd('Gauss(x,mu,sigma) = 1./(sigma*sqrt(2*pi)) * exp( -(x-mu)**2 / (2*sigma**2) )',
+            'd1(x) = Gauss(x, 0.5, 0.5)',
+            'd2(x) = Gauss(x,  2.,  1.)',
+            'd3(x) = Gauss(x, -1.,  2.)')
 
-    # Another means to unset options:
-    g = gnuplot.Gnuplot(terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400', output = '"test.png"')
-    g.set('noxlabel', 'noylabel', 'noxrange', 'noyrange')
-    g.plot('sin(x) with lp')
+As we see, all statement in cmd() would be translated the same statement in
+gnuplot. By this way we can execute any gnuplot statement.
 
-    # Another means to unset options:
-    g = gnuplot.Gnuplot()
-    g.set(xlabel = None,
-          ylabel = None,
-          xrange = None,
-          yrange = None)
-    g.plot('sin(x) with lp')
+1.4 plot()/splot()
+------------------
 
-2.1.5 plot()
-++++++++++++
+Definition:
 
 .. code-block:: python
 
     def plot(self, *items, **kwargs):
         '''
         *items: The list of plot command;
         **kwargs: The options that would be set before the plot command.
         '''
-
-plot is the primary command for drawing plots with gnuplot, We port it as a
-function in py-python. As description, the plot-element is passed as
-variable parameters, and options are passed as dictionary parameter. please
-be noted that the plot-element should be in the single quotes:
-
-Note that the plot()/splot() only plot the gnuplot functions and file, if
-you'd like to plot data generated in python, you should call the new added
-functions: `2.2.1 plot_data()`_ and `2.2.2 splot_data()`_ .
-
-for example plot the gnuplot function or datafile we use pygnuplot.gnuplot:
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-    g = gnuplot.Gnuplot()
-    g.plot('[-10:10] sin(x)',
-           'atan(x)',
-           'cos(atan(x))',
-           terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400',
-           output = '"simple.1.png"',
-           key = 'fixed left top vertical Right lt black linewidth 1.000 dashtype solid',
-           samples = '50, 50',
-           title = '"Simple Plots" font ",20" norotate')
-
-If we plot the python generated data we use plot_data() and splot_data():
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-    # usage examples, please note that we didn't give the output so could only
-    # see the image flash on the screen. Will introduce how to output the
-    # image to files.
-    df = pd.DataFrame(data = {'col1': [1, 2],
-                              'col2': [3, 4],
-                              'col3': [5, 6]})
-    g = gnuplot.Gnuplot()
-    g.plot_data(df, 'using 1:2 with lines', 'using 1:3 with points')
-
-As we stated in `2.1.3 set()`_ , we can use parameter to replace
-set()/unset() in plot() function, here is something we need to know when
-using parameter to replace set()/unset():
-
-1) If it's flag parameter, for example::
-
-    set grid
-    set hidden3d
-
-we can pass it as a empty value:
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-
-    # Examples of gnuplot.plot()
-    g = gnuplot.Gnuplot()
-    g.plot('sin(x)',
-           'cos(x)',
-           ...,
-           grid = '',
-           hidden3d = '',
-           ...)
-
-    # Examples of plot_data()
-    df = pd.DataFrame(data = {'col1': [1, 2],
-                              'col2': [3, 4],
-                              'col3': [5, 6]})
-    g = gnuplot.Gnuplot()
-    g.plot_data(df, 'using 1:2 with lines', 'using 1:3 with points',
-           grid = '')
-
-2) We have two means to pass "unset" command, one is the no-xxx option and
-   the other is xxx = None, for examples we'd like to unset the grid and
-   xrange::
-
-    unset grid
-    unset xrange
-
-We can do that in py-gnuplot by:
-
-.. code-block:: python
-
-    g = gnuplot.Gnuplot()
-    # Example of use no-xxx to unset the flag
-    g.plot(df, 'using 0:2:3:4:5 notitle with financebars lt 8',
-            ...,
-            nogrid = '',
-            noxlabel = '',
-            ...)
-
-    # Example of use None to unset the flag
-    g.plot(df, 'using 0:2:3:4:5 notitle with financebars lt 8',
-            ...,
-            grid = None,
-            xlabel = None,
-            ...)
-
-3) If there is multiple lines for one options, for exampe in gnuplot it
-   is::
-
-    set arrow from 5,-5,-1.2 to 5,5,-1.2 lt -1
-    set arrow from 5,6,-1 to 5,5,-1 lt -1
-    set arrow from 5,6,sinc(5,5) to 5,5,sinc(5,5) lt -1
-
-We pass them by a list of options:
-
-.. code-block:: python
-
-    g = gnuplot.Gnuplot()
-    g.plot(df,
-           'using 0:2:3:4:5 notitle with financebars lt 8',
-           ...,
-           arrow = ['from 5,-5,-1.2 to 5,5,-1.2 lt -1',
-                    'from 5,6,-1 to 5,5,-1 lt -1',
-                    'from 5,6,sinc(5,5) to 5,5,sinc(5,5) lt -1'],
-           ...,
-           ...)
-
-2.1.6 splot()
-+++++++++++++
-
-.. code-block:: python
-
     def splot(self, *items, **kwargs):
         '''
         *items: The list of plot command;
         **kwargs: The options that would be set before the plot command.
         '''
 
-The usage of splot() is exactly the same as plot().
+Every plot/splot command would be a parameter in plot()/splot() functions. Like
+set()/unset(), all the parameters must be string since it would be pas sed to
+gnuplot without any change. You need to change them to string if they are not::
+
+    #gnplot
+    plot d1(x) fs solid 1.0 lc rgb "forest-green" title "μ =  0.5 σ = 0.5", \
+     d2(x) lc rgb "gold" title "μ =  2.0 σ = 1.0", \
+     d3(x) lc rgb "dark-violet" title "μ = -1.0 σ = 2.0"
+
+    #py-gnplot
+    g.plot('d1(x) fs solid 1.0 lc rgb "forest-green" title "μ =  0.5 σ = 0.5"',
+            'd2(x) lc rgb "gold" title "μ =  2.0 σ = 1.0"',
+            'd3(x) lc rgb "dark-violet" title "μ = -1.0 σ = 2.0"')
 
-2.2 new developed member functions for python generated data
---------------------------------------------------------------
+1.5 plot_data()/splot_data()
+--------------------------------------
 
-We develop the following memember functions, they are very familar with the
-orignal plot() and splot(), the only difference is that , in the new
-developed function, we pass the python generated data as the first
-parameter and remove the corresponding element in the plot command.
+.. Note:: in older release, they are called plot_data()/splot_data(), I'd like to chnage them to the new name since they are more intuitive.
 
-2.2.1 plot_data()
-+++++++++++++++++
+Definition:
 
 .. code-block:: python
 
     def plot_data(self, data, *items, **kwargs):
         '''
         data: The data that need to be plotted. It's either the string of list
         or the Pnadas Dataframe, if it's Pnadas Dataframe it would be converted
         to string by data.to_csv(). Note that we will execut a extra command
         "set datafile separator "," to fit the data format of csv.
         *items: The list of plot command;
         **kwargs: The options that would be set before the plot command.
         '''
-
-The usage is the same as in `2.1.5 plot()`_ except that you should pass the
-data(string or pandas Dataframe format) as the first parameter, and remove
-the corresponding filename in every plot line. Moreover, the defaulst
-seperator now is "," for easy use with csv file:
-
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-
-    # usage examples, please note that we didn't give the output so could only
-    # see the image flash on the screen. Will introduce how to output the
-    # image to files.
-    df = pd.DataFrame(data = {'col1': [1, 2],
-                              'col2': [3, 4],
-                              'col3': [5, 6]})
-    g = gnuplot.Gnuplot()
-    # Note that the first parameter is df and there is no "data.file" in
-    # the following commmand.
-    g.plot_data(df,
-                'using 1:2 with lines',
-                'using 1:3 with points')
-
-2.2.2 splot_data()
-++++++++++++++++++
-
-.. code-block:: python
-
     def splot_data(self, data, *items, **kwargs):
         '''
         data: The data that need to be plotted. It's either the string of list
         or the Pnadas Dataframe, if it's Pnadas Dataframe it would be converted
         to string by data.to_csv(). Note that we will execut a extra command
         "set datafile separator "," to fit the data format of csv.
         *items: The list of plot command;
         **kwargs: The options that would be set before the plot command.
         '''
 
-The usage is the same as in `2.2.1 plot_data()`_ .
+With above functions: constructor, Set()/unset(), plot()/splot(), we can do
+what gnuplot do, but it cannot plot python generated data. It's hard to
+implement the new functions with the existing gnuplot command, so we develop
+two new functions: plot_data()/splot_data(). They are much like
+plot()/splot(), the only difference is:
+
+    * plot()/splot() take function(filename) in every plot command.
+    * plot_data()/splot_data() take the dataframe as the first
+      parameter, while remove function(filename) in every plot commmand
+
+for examples::
+
+    #plot(): 'finance.dat' is in plot command
+    g.plot("'finance.dat' using 0:($6/10000) notitle with impulses lt 3",
+           "'finance.dat' using 0:($7/10000) notitle with lines lt 1")
 
-2.3 new developed global class-less function call
-----------------------------------------------------
+    #plot_data(): the first parameter must be dataframe, every plot
+    #command doesn't take the data.
+    g.plot_data(df,
+            'using 0:($6/10000) notitle with impulses lt 3',
+            'using 0:($7/10000) notitle with lines lt 1')
 
-We can plot the image just by the above object-oriented interface, but
-sometimes we want to quick plot an image in quick mode, we can call the
-global class-less function call:
+See `histograms.2.py`_ and `histograms.2.py`_ for differences.
 
-2.3.1 plot()
-++++++++++++
+1.6 multiplot
+------------------
 
-.. code-block:: python
+To plot multiplot, you must set multiplot at first as in gnuplot. Here is examples.
 
-    #submodule gnuplot
-    def plot(*args, **kwargs):
-        '''
-        *items: The list of plot command;
-        **kwargs: The options that would be set before the plot command.
-        '''
+1.7 quick mode
+------------------
 
-The usage is the same as in `2.1.5 plot()`_ except that you needn't
-allocate a Gnuplot() instance at first:.
+For some easy case, we can combine the following step into one.
 
-.. _simple3.py:
+    1) Enter gnuplot conext;
+    2) Set plotting style;
+    3) Define some expressions;
+    4) Plotting.
 
-..
-    cmd2img:: python3
-    :image: simple.1.png
+For examples:
 
+.. _simple2.1.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
 
     gnuplot.plot('[-10:10] sin(x)',
            'atan(x)',
            'cos(atan(x))',
            terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400',
            output = '"simple.1.png"',
-           key = 'fixed left top vertical Right lt black linewidth 1.000 dashtype solid',
+           key = 'fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid',
            samples = '50, 50',
-           title = '"Simple Plots" font ",20" norotate')
-
-2.3.2 splot()
-++++++++++++++
-
-.. code-block:: python
-
-    #submodule gnuplot
-    def splot(*args, **kwargs):
-        '''
-        *items: The list of plot command;
-        **kwargs: The options that would be set before the plot command.
-        '''
-
-The usage is the same as in `2.1.6 splot()`_ except that you needn't
-allocate a Gnuplot() instance at first:
-
-2.3.3 plot_data()
-+++++++++++++++++
-
-.. code-block:: python
-
-    def plot_data(data, *items, **kwargs):
-        '''
-        data: The data that need to be plotted. It's either the string of list
-        or the Pnadas Dataframe, if it's Pnadas Dataframe it would be converted
-        to string by data.to_csv()
-        *items: The list of plot command;
-        **kwargs: The options that would be set before the plot command.
-        '''
-
-The usage is the same as in `2.2.1 plot_data()`_ except that you needn't
-allocate a Gnuplot() instance at first:
+           title = '"Simple Plots" font ",20" textcolor lt -1 norotate',
+           xrange = '[ * : * ] noreverse writeback',
+           x2range = '[ * : * ] noreverse writeback',
+           yrange = '[ * : * ] noreverse writeback',
+           y2range = '[ * : * ] noreverse writeback',
+           zrange = '[ * : * ] noreverse writeback',
+           cbrange = '[ * : * ] noreverse writeback',
+           rrange = '[ * : * ] noreverse writeback',
+           colorbox = 'vertical origin screen 0.9, 0.2 size screen 0.05, 0.6 front noinvert bdefault')
 
+.. _whale2.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
+    import pandas as pd
 
-    df = pd.DataFrame(data = {'col1': [1, 2],
-                              'col2': [3, 4],
-                              'col3': [5, 6]})
-    gnuplot.plot_data(df,
-                      'using 1:2 with lines',
-                      'using 1:3 with points')
-
-2.3.4 splot_data()
-++++++++++++++++++
-
-.. code-block:: python
-
-    class gnuplot.Gnuplot(object):
-
-        def splot(self, *items, **kwargs):
-            '''
-            *items: The list of plot command;
-            **kwargs: The options that would be set before the plot command.
-            '''
-
-The usage is the same as in `2.2.2 splot_data()`_ except that you needn't
-allocate a Gnuplot() instance at first:
-
-2.3.5 multiplot()
-+++++++++++++++++
-
-Since we don't allocate the Gnuplot instance, there is a little trick to
-plot the multiplot image. To solve the issue we create 3 brand new function
-to implement that.
-
-.. code-block:: python
-
-    def multiplot(\*args, \*\*kwargs):
-        @args: the subplot object list;
-        @kwargs: the setting options that need to be set before call plot;
-
-    def make_plot(\*args, \*\*kwargs)
-        The parameter definition is the same as plot(), but it doesn't plot
-        the data really, it only return the plot dictionary for later
-        multiplot() use.
-
-    def make_splot(\*args, \*\*kwargs)
-        The parameter definition is the same as splot(), but it doesn't plot
-        the data really, it only return the plot dictionary for later
-        multiplot() use.
-
-    def make_plot_data (data, \*args, \*\*kwargs)
-        The parameter definition is the same as plot_data(), but it doesn't
-        plot the data really, it only return the plot dictionary for later
-        multiplot() use.
-
-    def make_splot_data (data, \*args, \*\*kwargs)
-        The parameter definition is the same as splot_data(), but it
-        doesn't plot the data really, it only return the plot dictionary
-        for later multiplot() use.
-
-Before call multiplot() we must generate the subplot object by calling
-make_plot()/make_splot(), It is much like mplfinance.make_addplot(), it only
-add the subplot command for further call:
+    #https://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.html
+    gnuplot.splot('"examples/whale.dat" w pm3d',
+            term = 'pngcairo size 480,480',
+            out = '"whale.png"',
+            style = 'line 100 lw 0.1 lc "black"',
+            pm3d = 'depth hidden3d ls 100',
+            cbrange = '[-0.5:0.5]',
+            palette = 'rgb -3,-3,-3',
+            colorbox = None,
+            border = None,
+            key = None,
+            zrange = '[-2:2]',
+            tics = None,
+            view = '60,185,1.5')
 
+.. _histograms2.2.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
+    import pandas as pd
 
-    sub1 = gnuplot.make_plot('sin(x)', ylabel = 'ylabel')
-    sub2 = gnuplot.make_plot('cos(x)', xlabel = 'xlabel')
-    sub3 = gnuplot.make_plot('sin(2*x)', noxlabel = '', ylabel = '')
-    sub4 = gnuplot.make_plot('cos(2*x)', xlabel = 'xlabel')
-    gnuplot.multiplot(sub1, sub2, sub3, sub4,
-                      output = '"sample.multiplot.png"',
-                      term = 'pngcairo size 900,600 font ",11"',
-                      multiplot  = 'layout 2,2 columnsfirst margins 0.1,0.9,0.1,0.9 spacing 0.1')
-
-A example in reality:
-
-.. _finance2.py:
-
-..
-    cmd2img:: python3
-    :image: finance.13.png
+    df = pd.read_csv('examples/immigration.dat', index_col = 0, sep='\t', comment='#')
+    gnuplot.plot_data(df,
+            'using 2:xtic(1), for [i=3:22] "" using i ',
+            terminal = 'pngcairo transparent enhanced font "arial,10" fontscale 1.0 size 600, 400 ',
+            output = '"histograms.1.png"',
+            key = 'fixed right top vertical Right noreverse noenhanced autotitle nobox',
+            style = 'data linespoints',
+            datafile = ' missing "-"',
+            xtics = 'border in scale 1,0.5 nomirror rotate by -45 autojustify norangelimit',
+            title = '"US immigration from Europe by decade"')
 
+.. _surface2.9.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
-    import pandas as pd
 
-    # A demostration to generate pandas data frame data in python.
-    df = pd.read_csv('examples/finance.dat',
-            sep='\t',
-            index_col = 0,
-            parse_dates = True,
-            names = ['date', 'open','high','low','close', 'volume','volume_m50',
-                'intensity','close_ma20','upper','lower '])
-
-    # make subplot at first, now there is still no real plot.
-    sub1 = gnuplot.make_plot_data(df,
-            'using 0:2:3:4:5 notitle with candlesticks lt 8',
-            'using 0:9 notitle with lines lt 3',
-            'using 0:10 notitle with lines lt 1',
-            'using 0:11 notitle with lines lt 2',
-            'using 0:8 axes x1y2 notitle with lines lt 4',
-            title = '"Change to candlesticks"',
-            logscale = 'y',
-            xrange = '[50:253]',
-            yrange = '[75:105]',
-            format = 'x ""',
-            xtics = '(66, 87, 109, 130, 151, 174, 193, 215, 235)',
-            ytics = '(105, 100, 95, 90, 85, 80)',
-            lmargin = '9',
-            rmargin = '2',
-            bmargin = '0',
-            origin = '0, 0.3',
-            size = ' 1, 0.7',
-            grid = 'xtics ytics',
-            ylabel = '"price" offset 1',
-            label = ['1 "Acme Widgets" at graph 0.5, graph 0.9 center front',
-                '2 "Courtesy of Bollinger Capital" at graph 0.01, 0.07',
-                '3 "  www.BollingerBands.com" at graph 0.01, 0.03']
-            )
-
-    sub2 = gnuplot.make_plot_data(df,
-            'using 0:($6/10000) notitle with impulses lt 3',
-            'using 0:($7/10000) notitle with lines lt 1',
-            ytics = '500',
-            xtics = '("6/03" 66, "7/03" 87, "8/03" 109, "9/03" 130, "10/03" 151, "11/03" 174, "12/03" 193, "1/04" 215, "2/04" 235)',
-            ylabel = '"volume (0000)" offset 1',
-            nologscale = 'y',
-            autoscale = 'y',
-            size = '1.0, 0.3',
-            origin = '0.0, 0.0',
-            bmargin = '',
-            tmargin = '0',
-            format = ['x', 'y "%1.0f"'])
+    #py-gnuplot: https://gnuplot.sourceforge.net/demo/surface2.9.gnu
+    gnuplot.splot('cos(u)+.5*cos(u)*cos(v),sin(u)+.5*sin(u)*cos(v),.5*sin(v) with lines',
+            '1+cos(u)+.5*cos(u)*cos(v),.5*sin(v),sin(u)+.5*sin(u)*cos(v) with lines',
+            terminal = 'pngcairo enhanced font "arial,10" fontscale 1.0 size 600, 400 ',
+            output = '"surface2.9.png"',
+            dummy = 'u, v',
+            key = 'bmargin center horizontal Right noreverse enhanced autotitle nobox',
+            style = ['data lines'],
+            parametric = '',
+            view = '50, 30, 1, 1',
+            isosamples = '50, 20',
+            hidden3d = 'back offset 1 trianglepattern 3 undefined 1 altdiagonal bentover',
+            xyplane = 'relative 0',
+            title = '"Interlocking Tori" ',
+            urange = '[ -3.14159 : 3.14159 ] noreverse nowriteback',
+            vrange = '[ -3.14159 : 3.14159 ] noreverse nowriteback')
 
-    # plot at one time.
-    gnuplot.multiplot(sub1, sub2,
-            output = '"finance.13.png"',
-            term = 'pngcairo font "arial,10" fontscale 1.0 size 900, 600')
+2. Examples
+=============
 
-.. _3 Multiplot Axes Demo2:
+2.1 plot/splot function
+-------------------------------
 
+.. _simple.1.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
-    import pandas as pd
-    import numpy as np
-
-    #https://matplotlib.org/gallery/subplots_axes_and_figures/axes_demo.html#sphx-glr-gallery-subplots-axes-and-figures-axes-demo-py
-    #http://gnuplot.sourceforge.net/demo_5.2/bins.html
-
-    # 1) create some data to use for the plot
-    np.random.seed(19680801) # Fixing random state for reproducibility
-    dt = 0.001
-    t = np.arange(0.0, 10.0, dt)
-    r = np.exp(-t / 0.05)  # impulse response
-    x = np.random.randn(len(t))
-    s = np.convolve(x, r)[:len(x)] * dt  # colored noise
-    df = pd.DataFrame({'r': r, 'x': x, 's': s}, index = t)
-    df.index.name = 't'
-    #print(df.tail().to_csv())
-
-    # 2) Plot the data
-    main = gnuplot.make_plot_data(df.iloc[:1000],
-            'using 1:4 with line lw 2 lc "web-blue"',
-            title = '"Gaussian colored noise"',
-            xlabel = '"time (s)"',
-            ylabel = '"current (nA)"',
-            xrange = '[0:1]',
-            yrange = '[-0.015:0.03]',
-            key = None,
-            size = ' 1, 1',
-            origin = '0, 0')
-    right = gnuplot.make_plot_data(df,
-            'using 4 bins=400 with boxes title "20 bins" lw 2 lc "web-blue"',
-            title = '"Probability"',
-            xlabel = None,
-            ylabel = None,
-            tics = None,
-            xrange = None,
-            yrange = None,
-            origin = '0.65, 0.56',
-            size = '0.24, 0.32',
-            object = 'rectangle from graph 0,0 to graph 1,1 behind fc "black" fillstyle solid 1.0')
-    left = gnuplot.make_plot_data(df,
-            'using 1:2 with line lw 2 lc "web-blue"',
-            title = '"Impulse response"',
-            xrange = '[0:0.2]',
-            origin = '0.15, 0.56',
-            size = '0.24, 0.32')
 
-    gnuplot.multiplot(main, right, left,
-            output = '"sphx_glr_axes_demo_001.png"',
-            term = 'pngcairo font "arial,10" fontscale 1.0 size 640, 480',
-            key = '')
+    #py-gnuplot: https://gnuplot.sourceforge.net/demo_6.0/simple.html
 
-3. examples
-============
+    #Ceate a gnuplot context. with "log = True" to print the gnuplot execute log.
+    g = gnuplot.Gnuplot(log = True)
 
-3.1 examples port from gnuplot
-------------------------------
+    #Set plotting style
+    g.set(terminal = 'pngcairo font "arial,10" fontscale 1.0 size 600, 400',
+           output = '"simple.1.png"',
+           key = 'fixed left top vertical Right noreverse enhanced autotitle box lt black linewidth 1.000 dashtype solid',
+           samples = '50, 50',
+           title = '"Simple Plots" font ",20" textcolor lt -1 norotate',
+           xrange = '[ * : * ] noreverse writeback',
+           x2range = '[ * : * ] noreverse writeback',
+           yrange = '[ * : * ] noreverse writeback',
+           y2range = '[ * : * ] noreverse writeback',
+           zrange = '[ * : * ] noreverse writeback',
+           cbrange = '[ * : * ] noreverse writeback',
+           rrange = '[ * : * ] noreverse writeback',
+           colorbox = 'vertical origin screen 0.9, 0.2 size screen 0.05, 0.6 front  noinvert bdefault')
 
-3.1.1 finance
-+++++++++++++
+    #Expressions and caculations
+    g.cmd("NO_ANIMATION = 1")
 
-example with object-oriented interface call:
+    #Plotting
+    g.plot("[-10:10] sin(x)", "atan(x)", "cos(atan(x))")
 
-.. _finance1.py:
+This is the output: 
 
-..
-    cmd2img:: python3
-    :image: finance.13.png
+|simple.1.png|
 
+.. _surface.9.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
-    import pandas as pd
-
-    # A demostration to generate pandas data frame data in python.
-    df = pd.read_csv('examples/finance.dat',
-            sep='\t',
-            index_col = 0,
-            parse_dates = True,
-            names = ['date', 'open','high','low','close', 'volume','volume_m50',
-                'intensity','close_ma20','upper','lower '])
-
-    # Create a Gnuplot instance and set the options at first;
-    g = gnuplot.Gnuplot(log = True,
-            output = '"finance.13.png"',
-            term = 'pngcairo font "arial,10" fontscale 1.0 size 900, 600',
-            multiplot = True)
-
-    g.plot_data(df,
-            'using 0:2:3:4:5 notitle with candlesticks lt 8',
-            'using 0:9 notitle with lines lt 3',
-            'using 0:10 notitle with lines lt 1',
-            'using 0:11 notitle with lines lt 2',
-            'using 0:8 axes x1y2 notitle with lines lt 4',
-            title = '"Change to candlesticks"',
-            logscale = 'y',
-            xrange = '[50:253]',
-            yrange = '[75:105]',
-            format = 'x ""',
-            xtics = '(66, 87, 109, 130, 151, 174, 193, 215, 235)',
-            ytics = '(105, 100, 95, 90, 85, 80)',
-            lmargin = '9',
-            rmargin = '2',
-            bmargin = '0',
-            origin = '0, 0.3',
-            size = ' 1, 0.7',
-            grid = 'xtics ytics',
-            ylabel = '"price" offset 1',
-            label = ['1 "Acme Widgets" at graph 0.5, graph 0.9 center front',
-                '2 "Courtesy of Bollinger Capital" at graph 0.01, 0.07',
-                '3 "  www.BollingerBands.com" at graph 0.01, 0.03'],
-            )
 
-    g.plot_data(df,
-            'using 0:($6/10000) notitle with impulses lt 3',
-            'using 0:($7/10000) notitle with lines lt 1',
-            bmargin = '',
-            size = '1.0, 0.3',
-            origin = '0.0, 0.0',
-            tmargin = '0',
-            nologscale = 'y',
-            autoscale = 'y',
-            format = ['x', 'y "%1.0f"'],
-            ytics = '500',
-            xtics = '("6/03" 66, "7/03" 87, "8/03" 109, "9/03" 130, "10/03" 151, "11/03" 174, "12/03" 193, "1/04" 215, "2/04" 235)',
-            ylabel = '"volume (0000)" offset 1')
-
-Since it enable the log options, I attach the execution log as below::
+    #py-gnuplot: https://gnuplot.sourceforge.net/demo_6.0/simple.html
 
-    [py-gnuplot 19:35:26] set output "finance.13.png"
-    [py-gnuplot 19:35:26] set term pngcairo font "arial,10" fontscale 1.0 size 900, 600
-    [py-gnuplot 19:35:26] set multiplot
-    [py-gnuplot 19:35:26] set datafile separator ","
-    [py-gnuplot 19:35:26] set title "Change to candlesticks"
-    [py-gnuplot 19:35:26] set logscale y
-    [py-gnuplot 19:35:26] set xrange [50:253]
-    [py-gnuplot 19:35:26] set yrange [75:105]
-    [py-gnuplot 19:35:26] set format x ""
-    [py-gnuplot 19:35:26] set xtics (66, 87, 109, 130, 151, 174, 193, 215, 235)
-    [py-gnuplot 19:35:26] set ytics (105, 100, 95, 90, 85, 80)
-    [py-gnuplot 19:35:26] set lmargin 9
-    [py-gnuplot 19:35:26] set rmargin 2
-    [py-gnuplot 19:35:26] set bmargin 0
-    [py-gnuplot 19:35:26] set origin 0, 0.3
-    [py-gnuplot 19:35:26] set size  1, 0.7
-    [py-gnuplot 19:35:26] set grid xtics ytics
-    [py-gnuplot 19:35:26] set ylabel "price" offset 1
-    [py-gnuplot 19:35:26] set label 1 "Acme Widgets" at graph 0.5, graph 0.9 center front
-    [py-gnuplot 19:35:26] set label 2 "Courtesy of Bollinger Capital" at graph 0.01, 0.07
-    [py-gnuplot 19:35:26] set label 3 "  www.BollingerBands.com" at graph 0.01, 0.03
-    [py-gnuplot 19:35:26] plot $DataFrame using 0:2:3:4:5 notitle with candlesticks lt 8,\
-    [py-gnuplot 19:35:26] $DataFrame using 0:9 notitle with lines lt 3,\
-    [py-gnuplot 19:35:26] $DataFrame using 0:10 notitle with lines lt 1,\
-    [py-gnuplot 19:35:26] $DataFrame using 0:11 notitle with lines lt 2,\
-    [py-gnuplot 19:35:26] $DataFrame using 0:8 axes x1y2 notitle with lines lt 4
-    [py-gnuplot 19:35:26] unset for [i=1:200] label i
-    [py-gnuplot 19:35:26] set datafile separator ","
-    [py-gnuplot 19:35:26] set bmargin
-    [py-gnuplot 19:35:26] set size 1.0, 0.3
-    [py-gnuplot 19:35:26] set origin 0.0, 0.0
-    [py-gnuplot 19:35:26] set tmargin 0
-    [py-gnuplot 19:35:26] set nologscale y
-    [py-gnuplot 19:35:26] set autoscale y
-    [py-gnuplot 19:35:26] set format x
-    [py-gnuplot 19:35:26] set format y "%1.0f"
-    [py-gnuplot 19:35:26] set ytics 500
-    [py-gnuplot 19:35:26] set xtics ("6/03" 66, "7/03" 87, "8/03" 109, "9/03" 130, "10/03" 151, "11/03" 174, "12/03" 193, "1/04" 215, "2/04" 235)
-    [py-gnuplot 19:35:26] set ylabel "volume (0000)" offset 1
-    [py-gnuplot 19:35:26] plot $DataFrame using 0:($6/10000) notitle with impulses lt 3,\
-    [py-gnuplot 19:35:26] $DataFrame using 0:($7/10000) notitle with lines lt 1
-    [py-gnuplot 19:35:26] unset for [i=1:200] label i
+    #Ceate a gnuplot context. with "log = True" to print the gnuplot execute log.
+    g = gnuplot.Gnuplot(log = True)
 
-And the generated output is as following:
+    #Set plotting style
+    g.set(terminal = 'pngcairo  transparent enhanced font "arial,10" fontscale 1.0 size 600, 400',
+            output = "'surface2.9.png'",
+            dummy = 'u, v',
+            key = 'bmargin center horizontal Right noreverse enhanced autotitle nobox',
+            parametric = '',
+            view = '50, 30, 1, 1',
+            isosamples = '50, 20',
+            hidden3d = 'back offset 1 trianglepattern 3 undefined 1 altdiagonal bentover',
+            style = ['data lines'],
+            xyplane = 'relative 0',
+            title = '"Interlocking Tori" ',
+            urange = '[ -3.14159 : 3.14159 ] noreverse nowriteback',
+            vrange = '[ -3.14159 : 3.14159 ] noreverse nowriteback',
+            colorbox = 'vertical origin screen 0.9, 0.2 size screen 0.05, 0.6 front  noinvert bdefault')
 
-.. image:: http://gnuplot.sourceforge.net/demo/finance.13.png
-   :width: 350
+    #Expressions and caculations
+    g.cmd("NO_ANIMATION = 1")
 
-3.1.2 histogram
-+++++++++++++++
+    #Plotting
+    g.splot("cos(u)+.5*cos(u)*cos(v)",
+            "sin(u)+.5*sin(u)*cos(v)",
+            ".5*sin(v) with lines",
+            "1+cos(u)+.5*cos(u)*cos(v)",
+            ".5*sin(v),sin(u)+.5*sin(u)*cos(v) with lines",
+            )
 
-.. _histo.1.py:
+This is the output: 
 
-..
-    cmd2img:: python3
-    :image: histograms.1.png
+|surface2.9.png|
 
-Plot with member functions:
+2.2 plot/splot file
+-------------------------------
 
+.. _histograms.2.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
 
-    df = pd.read_csv('examples/immigration.dat', index_col = 0, sep='\t', comment='#')
-    g = gnuplot.Gnuplot()
-    g.set(terminal = 'pngcairo transparent enhanced font "arial,10" fontscale 1.0 size 600, 400 ',
-            output = '"histograms.1.png"',
-            key = 'fixed right top vertical Right noreverse noenhanced autotitle nobox',
-            style = 'data linespoints',
-            datafile = ' missing "-"',
-            xtics = 'border in scale 1,0.5 nomirror rotate by -45 autojustify norangelimit',
-            title = '"US immigration from Europe by decade"')
-    g.plot_data(df, 'using 2:xtic(1), for [i=3:22] "" using i ')
-
-Since it's simple, we can plot it quick way:
-
-.. _histo.2.py:
-
-..
-    cmd2img:: python3
-    :image: histograms.1.png
+    #Histograms demo example comes from
+    #https://gnuplot.sourceforge.net/demo_6.0/histograms.2.gnu
 
-.. code-block:: python
-
-    #!/usr/bin/env python3
-    #coding=utf8
-    from pygnuplot import gnuplot
-    import pandas as pd
+    #1) Ceate a gnuplot context
+    g = gnuplot.Gnuplot(log = True)
 
-    df = pd.read_csv('examples/immigration.dat', index_col = 0, sep='\t', comment='#')
-    gnuplot.plot_data(df,
-            'using 2:xtic(1), for [i=3:22] "" using i ',
-            terminal = 'pngcairo transparent enhanced font "arial,10" fontscale 1.0 size 600, 400 ',
-            output = '"histograms.1.png"',
+    #2) Set plotting style
+    g.set(terminal = 'pngcairo  transparent enhanced font "arial,10" fontscale 1.0 size 600, 400',
+            output = "'histograms.2.png'",
+            boxwidth = '0.9 absolute',
+            style = ['fill   solid 1.00 border lt -1',
+                'histogram clustered gap 1 title textcolor lt -1',
+                'data histograms' ],
             key = 'fixed right top vertical Right noreverse noenhanced autotitle nobox',
-            style = 'data linespoints',
-            datafile = ' missing "-"',
-            xtics = 'border in scale 1,0.5 nomirror rotate by -45 autojustify norangelimit',
-            title = '"US immigration from Europe by decade"')
+            datafile = "missing '-'",
+            xtics = ["border in scale 0,0 nomirror rotate by -45  autojustify",
+                "norangelimit ",
+                " ()"],
+            title = '"US immigration from Northern Europe\\nPlot selected data columns as histogram of clustered boxes"',
+            xrange = '[ * : * ] noreverse writeback',
+            x2range = '[ * : * ] noreverse writeback',
+            yrange  = '[ 0.00000 : 300000. ] noreverse writeback',
+            y2range = '[ * : * ] noreverse writeback',
+            zrange = '[ * : * ] noreverse writeback',
+            cbrange = '[ * : * ] noreverse writeback',
+            rrange = '[ * : * ] noreverse writeback',
+            colorbox = 'vertical origin screen 0.9, 0.2 size screen 0.05, 0.6 front  noinvert bdefault')
 
-And the generated output is as following:
+    #3) Expressions and caculations
+    g.cmd("NO_ANIMATION = 1")
 
-.. image:: http://gnuplot.sourceforge.net/demo/histograms.1.png
-   :width: 350
+    #4) Plotting
+    g.plot("'examples/immigration.dat' using 6:xtic(1) ti col",
+            "'' u 12 ti col",
+            "'' u 13 ti col",
+            "'' u 14 ti col")
 
-3.1.3 splot
-+++++++++++
+This is the output: 
 
-.. _surface1.py:
+|histograms.2.png|
 
-..
-    cmd2img:: python3
-    :image: surface2.9.png
-
-object-oriented function call:
+Another example is to splot a pm3d image:
 
+.. _whale.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
 
-    g = gnuplot.Gnuplot(output = '"surface2.9.png"',
-            terminal = 'pngcairo enhanced font "arial,10" fontscale 1.0 size 600, 400 ',
-            title = '"Interlocking Tori" ',
-            dummy = 'u, v',
-            key = 'bmargin center horizontal Right noreverse enhanced autotitle nobox',
-            style = ['increment default','data lines'],
-            parametric = '',
-            view = '50, 30, 1, 1',
-            isosamples = '50, 20',
-            hidden3d = 'back offset 1 trianglepattern 3 undefined 1 altdiagonal bentover',
-            xyplane = 'relative 0',
-            urange = '[ -3.14159 : 3.14159 ] noreverse nowriteback',
-            vrange = '[ -3.14159 : 3.14159 ] noreverse nowriteback')
-    g.splot('cos(u)+.5*cos(u)*cos(v),sin(u)+.5*sin(u)*cos(v),.5*sin(v) with lines',
-            '1+cos(u)+.5*cos(u)*cos(v),.5*sin(v),sin(u)+.5*sin(u)*cos(v) with lines')
+    #Whale example comes from
+    #https://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.html
 
-.. _surface2.py:
+    #Ceate a gnuplot context
+    g = gnuplot.Gnuplot(log = True)
 
-Direct function call example:
+    #Set plotting style
+    g.set(term = 'pngcairo size 480,480',
+            output = '"whale.png"',
+            style = 'line 100 lw 0.1 lc "black"',
+            pm3d = 'depth hidden3d ls 100',
+            cbrange = '[-0.5:0.5]',
+            palette = 'rgb -3,-3,-3',
+            colorbox = None,
+            border   = None,
+            key = None,
+            zrange = '[-2:2]',
+            tics  = None,
+            view = '60,185,1.5')
 
-..
-    cmd2img:: python3
-    :image: surface2.9.png
+    #No Expressions
 
+    #Plotting
+    g.splot('"examples/whale.dat" w pm3d')
+
+The generated image is as below:
+
+|whale.png|
+
+2.3 plot/splot python generated data
+----------------------------------------------
+
+.. _histograms3.2.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
+    import pandas as pd
 
-    gnuplot.splot('cos(u)+.5*cos(u)*cos(v),sin(u)+.5*sin(u)*cos(v),.5*sin(v) with lines',
-            '1+cos(u)+.5*cos(u)*cos(v),.5*sin(v),sin(u)+.5*sin(u)*cos(v) with lines',
-            terminal = 'pngcairo enhanced font "arial,10" fontscale 1.0 size 600, 400 ',
-            output = '"surface2.9.png"',
-            dummy = 'u, v',
-            key = 'bmargin center horizontal Right noreverse enhanced autotitle nobox',
-            style = ['data lines'],
-            parametric = '',
-            view = '50, 30, 1, 1',
-            isosamples = '50, 20',
-            hidden3d = 'back offset 1 trianglepattern 3 undefined 1 altdiagonal bentover',
-            xyplane = 'relative 0',
-            title = '"Interlocking Tori" ',
-            urange = '[ -3.14159 : 3.14159 ] noreverse nowriteback',
-            vrange = '[ -3.14159 : 3.14159 ] noreverse nowriteback')
+    #Histograms demo example comes from
+    #https://gnuplot.sourceforge.net/demo_6.0/histograms.2.gnu
 
-And the generated output is as following:
+    #1) Ceate a gnuplot context
+    g = gnuplot.Gnuplot(log = True)
 
-.. image:: http://gnuplot.sourceforge.net/demo/surface2.9.png
-   :width: 350
+    #2) Set plotting style
+    g.set(terminal = 'pngcairo  transparent enhanced font "arial,10" fontscale 1.0 size 600, 400',
+            output = "'histograms.2.png'",
+            boxwidth = '0.9 absolute',
+            style = ['fill   solid 1.00 border lt -1',
+                'histogram clustered gap 1 title textcolor lt -1',
+                'data histograms' ],
+            key = 'fixed right top vertical Right noreverse noenhanced autotitle nobox',
+            datafile = "missing '-'",
+            xtics = ["border in scale 0,0 nomirror rotate by -45  autojustify",
+                "norangelimit ",
+                " ()"],
+            title = '"US immigration from Northern Europe\\nPlot selected data columns as histogram of clustered boxes"',
+            xrange = '[ * : * ] noreverse writeback',
+            x2range = '[ * : * ] noreverse writeback',
+            yrange  = '[ 0.00000 : 300000. ] noreverse writeback',
+            y2range = '[ * : * ] noreverse writeback',
+            zrange = '[ * : * ] noreverse writeback',
+            cbrange = '[ * : * ] noreverse writeback',
+            rrange = '[ * : * ] noreverse writeback',
+            colorbox = 'vertical origin screen 0.9, 0.2 size screen 0.05, 0.6 front  noinvert bdefault')
+
+    #3) Expressions and caculations
+    g.cmd("NO_ANIMATION = 1")
+    #The original example is plotting file, it's easy. To demonstrate plotting
+    #data generated in python, we transform the data into df for demonstration.
+    df = pd.read_csv('examples/immigration.dat', index_col = 0, sep='\t', comment='#')
 
-3.1.4 pm3d
-++++++++++
+    #4) Plotting
+    g.plot_data(df,
+            'using 6:xtic(1) ti col',
+            'u 12 ti col',
+            'u 13 ti col',
+            'u 14 ti col')
 
-iterate.dem
+The generated image is as below:
 
-.. _whale1.py:
+|histograms.2.png|
 
-..
-    cmd2img:: python3
-    :image: whale.png
+2.4 multiplot examples
+------------------------------
 
+.. _finance.13.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
+    import pandas as pd
 
-    #http://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.html
-    g = gnuplot.Gnuplot()
-    # Black and white version
-    g.splot('"examples/whale.dat" w pm3d',
-            term = 'pngcairo size 480,480',
-            out = '"whale.png"',
-            style = 'line 100 lw 0.1 lc "black"',
-            pm3d = 'depth hidden3d ls 100',
-            cbrange = '[-0.5:0.5]',
-            palette = 'rgb -3,-3,-3',
-            colorbox = None,
-            border = None,
-            key = None,
-            zrange = '[-2:2]',
-            tics = None,
-            view = '60,185,1.5')
+    #Transparent demo example comes from
+    #https://gnuplot.sourceforge.net/demo_6.0/finance.html
 
+    #Ceate a gnuplot context
+    g = gnuplot.Gnuplot(log = True)
 
-.. _whale2.py:
+    #Set plotting style
+    g.set(output = "'finance.13.png'",
+            term = 'pngcairo  transparent enhanced font "arial,8" fontscale 1.0 size 660, 320',
+            label = ['1 "Acme Widgets" at graph 0.5, graph 0.9 center front',
+                '2 "Courtesy of Bollinger Capital" at graph 0.01, 0.07',
+                '3 "  www.BollingerBands.com" at graph 0.01, 0.03'],
+            logscale = 'y',
+            yrange = '[75:105]',
+            ytics = '(105, 100, 95, 90, 85, 80)',
+            xrange = '[50:253]',
+            grid = '',
+            lmargin = '9',
+            rmargin = '2',
+            format = 'x ""',
+            xtics = '(66, 87, 109, 130, 151, 174, 193, 215, 235)',
+            multiplot = True)
 
-..
-    cmd2img:: python3
-    :image: whale.png
+    #3) Expressions and caculations
 
+    #4) Plotting: Since multiplot = True, we plot two subplot
+    g.plot("'finance.dat' using 0:2:3:4:5 notitle with candlesticks lt 8",
+            "'finance.dat' using 0:9 notitle with lines lt 3",
+            "'finance.dat' using 0:10 notitle with lines lt 1",
+            "'finance.dat' using 0:11 notitle with lines lt 2",
+            "'finance.dat' using 0:8 axes x1y2 notitle with lines lt 4",
+            title = '"Change to candlesticks"',
+            size = ' 1, 0.7',
+            origin = '0, 0.3',
+            bmargin = '0',
+            ylabel = '"price" offset 1')
+    g.plot("'finance.dat' using 0:($6/10000) notitle with impulses lt 3",
+            "'finance.dat' using 0:($7/10000) notitle with lines lt 1",
+            bmargin = '',
+            format = ['x', 'y "%1.0f"'],
+            size = '1.0, 0.3',
+            origin = '0.0, 0.0',
+            tmargin = '0',
+            nologscale = 'y',
+            autoscale = 'y',
+            ytics = '500',
+            xtics = '("6/03" 66, "7/03" 87, "8/03" 109, "9/03" 130, "10/03" 151, "11/03" 174, "12/03" 193, "1/04" 215, "2/04" 235)',
+            ylabel = '"volume (0000)" offset 1')
+
+.. _finance3.13.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
 
-    # Black and white version
-    gnuplot.splot('"examples/whale.dat" w pm3d',
-            term = 'pngcairo size 480,480',
-            out = '"whale.png"',
-            style = 'line 100 lw 0.1 lc "black"',
-            pm3d = 'depth hidden3d ls 100',
-            cbrange = '[-0.5:0.5]',
-            palette = 'rgb -3,-3,-3',
-            colorbox = None,
-            border = None,
-            key = None,
-            zrange = '[-2:2]',
-            tics = None,
-            view = '60,185,1.5')
+    #Transparent demo example comes from
+    #https://gnuplot.sourceforge.net/demo_6.0/finance.html
 
-And the generated output is as following:
+    #Ceate a gnuplot context
+    g = gnuplot.Gnuplot(log = True)
 
-.. http://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.html
-.. image http://gnuplot.sourceforge.net/demo/iterate.2.png
-.. image:: http://ayapin-film.sakura.ne.jp/Gnuplot/Pm3d/Part1/whale.png
-   :width: 350
+    #Set plotting style
+    g.set(output = "'finance.13.png'",
+            term = 'pngcairo  transparent enhanced font "arial,8" fontscale 1.0 size 660, 320',
+            label = ['1 "Acme Widgets" at graph 0.5, graph 0.9 center front',
+                '2 "Courtesy of Bollinger Capital" at graph 0.01, 0.07',
+                '3 "  www.BollingerBands.com" at graph 0.01, 0.03'],
+            logscale = 'y',
+            yrange = '[75:105]',
+            ytics = '(105, 100, 95, 90, 85, 80)',
+            xrange = '[50:253]',
+            grid = '',
+            lmargin = '9',
+            rmargin = '2',
+            format = 'x ""',
+            xtics = '(66, 87, 109, 130, 151, 174, 193, 215, 235)',
+            multiplot = True)
 
-3.2 Examples port from matplotlib
----------------------------------
+    #3) Expressions and caculations
+    #A demostration to generate pandas data frame data in python.
+    df = pd.read_csv('examples/finance.dat',
+            sep='\t',
+            index_col = 0,
+            parse_dates = True,
+            names = ['date', 'open','high','low','close', 'volume','volume_m50',
+                'intensity','close_ma20','upper','lower '])
+
+    #4) Plotting: Since multiplot = True, we plot two subplot
+    g.plot_data(df,
+            'using 0:2:3:4:5 notitle with candlesticks lt 8',
+            'using 0:9 notitle with lines lt 3',
+            'using 0:10 notitle with lines lt 1',
+            'using 0:11 notitle with lines lt 2',
+            'using 0:8 axes x1y2 notitle with lines lt 4',
+            title = '"Change to candlesticks"',
+            size = ' 1, 0.7',
+            origin = '0, 0.3',
+            bmargin = '0',
+            ylabel = '"price" offset 1')
+    g.plot_data(df,
+            'using 0:($6/10000) notitle with impulses lt 3',
+            'using 0:($7/10000) notitle with lines lt 1',
+            bmargin = '',
+            format = ['x', 'y "%1.0f"'],
+            size = '1.0, 0.3',
+            origin = '0.0, 0.0',
+            tmargin = '0',
+            nologscale = 'y',
+            autoscale = 'y',
+            ytics = '500',
+            xtics = '("6/03" 66, "7/03" 87, "8/03" 109, "9/03" 130, "10/03" 151, "11/03" 174, "12/03" 193, "1/04" 215, "2/04" 235)',
+            ylabel = '"volume (0000)" offset 1')
+
+Both script generate the same output image:
+
+|finance.13.png|
+
+2.5 Examples port from matplotlib
+-----------------------------------
 
 Just for fun, I translate some examples in matplotlib to py-gnuplot:
 
-3.2.1 Stacked bar chart
+2.5.1 Stacked bar chart
 +++++++++++++++++++++++
 
-..
-    .. cmd2img:: python3
-        :image: sphx_glr_bar_stacked_001.png
-
+.. _sphx_glr_bar_stacked_001.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
 
@@ -1335,27 +873,22 @@
             boxwidth = '%s' %(width),
             xrange = '[0.5:5.5]',
             ylabel = '"Scores"',
             title = '"Scores by group and gender"',
             output = '"sphx_glr_bar_stacked_001.png"',
             terminal = 'pngcairo size 640, 480')
 
-Refer to the original script: `Stacked bar chart`_ and the original image:
+This is the output:
 
-.. _Stacked bar chart: https://matplotlib.org/gallery/lines_bars_and_markers/bar_stacked.html#sphx-glr-gallery-lines-bars-and-markers-bar-stacked-py
-.. image:: https://matplotlib.org/_images/sphx_glr_bar_stacked_001.png
-   :width: 350
+|sphx_glr_bar_stacked_001.png|
 
-3.2.2 Grouped bar chart with labels
+2.5.2 Grouped bar chart with labels
 +++++++++++++++++++++++++++++++++++
 
-..
-    cmd2img:: python3
-            :image: sphx_glr_barchart_001.png
-
+.. _sphx_glr_barchart_001.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
 
@@ -1382,27 +915,22 @@
             style = ['data histogram',
                      'histogram cluster gap 1',
                      'fill solid border -1',
                      'textbox transparent'],
             output = '"sphx_glr_barchart_001.png"',
             terminal = 'pngcairo size 640, 480')
 
-Refer to the original script: `Grouped bar chart with labels`_ and the original image:
+This is the output:
 
-.. _Grouped bar chart with labels: https://matplotlib.org/gallery/lines_bars_and_markers/barchart.html#sphx-glr-gallery-lines-bars-and-markers-barchart-py
-.. image:: https://matplotlib.org/_images/sphx_glr_barchart_001.png
-   :width: 350
+|sphx_glr_barchart_001.png|
 
-3.2.3 Multiplot Axes Demo
+2.5.3 Multiplot Axes Demo
 +++++++++++++++++++++++++
 
-..
-    cmd2img:: python3
-            :image: sphx_glr_axes_demo_001.png
-
+.. _sphx_glr_axes_demo_001.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
     import numpy as np
@@ -1451,27 +979,22 @@
     g.plot_data(df,
             'using 1:2 with line lw 2 lc "web-blue"',
             title = '"Impulse response"',
             xrange = '[0:0.2]',
             origin = '0.15, 0.56',
             size = '0.24, 0.32')
 
-Refer to the original script: `Multiplot Axes Demo`_ and the original image:
+This is the output:
 
-.. _Multiplot Axes Demo: https://matplotlib.org/gallery/subplots_axes_and_figures/axes_demo.html#sphx-glr-gallery-subplots-axes-and-figures-axes-demo-py
-.. image:: https://matplotlib.org/_images/sphx_glr_axes_demo_001.png
-   :width: 350
+|sphx_glr_axes_demo_001.png|
 
-3.2.4 control view and zoom 
+2.5.4 control view and zoom 
 ++++++++++++++++++++++++++++
 
-..
-    cmd2img:: python3
-            :image: sphx_glr_axes_margins_001.png
-
+.. _sphx_glr_axes_margins_001.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
 
@@ -1506,79 +1029,69 @@
             xrange = '[0: 3]',
             yrange = '[-0.7: 1]',
             xtics = '0, 0.5, 3',
             ytics = '-0.5, 0.5, 1',
             origin = '0, 0',
             size = '1, 0.5')
 
-Refer to the original script: `axes_margins.py`_ and the original image:
+This is the output:
 
-.. _axes_margins.py: https://matplotlib.org/_downloads/4d3bc54481c3ff3a1ac6712bc2904875/axes_margins.py
-.. image:: https://matplotlib.org/_images/sphx_glr_axes_margins_001.png
-   :width: 350
+|sphx_glr_axes_margins_001.png|
 
-3.2.5 Rendering math equation using TeX
+2.5.5 Rendering math equation using TeX
 +++++++++++++++++++++++++++++++++++++++
 
 We can embed the TeX math equation into the gnuplot generated image by setting
 the epslatex terminal, it would be rendered as a .tex file, you can import it
 directly or you can convert it to .pdf file and then .png file if needed. this
 is the example:
 
-..
-    cmd2img:: python3
-    :image: pygnuplot_tex_demo.tex
-
+.. _sphx_glr_tex_demo_001.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
 
     # https://matplotlib.org/gallery/text_labels_and_annotations/tex_demo.html#sphx-glr-gallery-text-labels-and-annotations-tex-demo-py
     # http://wap.sciencenet.cn/blog-373392-500657.html
     # https://www.thinbug.com/q/17593917
     g = gnuplot.Gnuplot(log = True,
-            output = '"pygnuplot_tex_demo.tex"',
+            output = '"sphx_glr_tex_demo_001.tex"',
             term = 'epslatex standalone lw 2 color colortext')
 
     # NOTE: In the following example, we need to escape the "\", that means we
     # should use '\\' or "\\\\" for \
     g.plot('cos(4*pi*x) + 2',
             xlabel = "'\\textbf{time (s)}'",
             ylabel = "'\\textit{Velocity (\N{DEGREE SIGN}/sec)}'",
             title = "'\\TeX\\ is Number $\\displaystyle\\sum_{n=1}^\\infty\\frac{-e^{i\\pi}}{2^n}$!' tc 'red'",
             key = None,
             xrange = '[0: 1]')
 
+This is the output:
+
+|sphx_glr_tex_demo_001.png|
+
 I list the script output since it's with the log=True::
 
-    [py-gnuplot 14:56:13] set output "pygnuplot_tex_demo.tex"
+    [py-gnuplot 14:56:13] set output "sphx_glr_tex_demo_001.tex"
     [py-gnuplot 14:56:13] set term epslatex standalone lw 2 color colortext
     [py-gnuplot 14:56:13] set xlabel '\textbf{time (s)}'
     [py-gnuplot 14:56:13] set ylabel '\textit{Velocity (°/sec)}'
     [py-gnuplot 14:56:13] set title '\TeX\ is Number $\displaystyle\sum_{n=1}^\infty\frac{-e^{i\pi}}{2^n}$!' tc 'red'
     [py-gnuplot 14:56:13] unset key
     [py-gnuplot 14:56:13] set xrange [0: 1]
     [py-gnuplot 14:56:13] plot cos(4*pi*x) + 2
 
-Refer to the original script: `Rendering math equation using TeX`_ and the original image:
-
-.. _Rendering math equation using TeX: https://matplotlib.org/gallery/text_labels_and_annotations/tex_demo.html#sphx-glr-gallery-text-labels-and-annotations-tex-demo-py
-.. image:: https://matplotlib.org/_images/sphx_glr_tex_demo_001.png
-   :width: 350
-
-3.2.6 Basic pie chart
+2.5.6 Basic pie chart
 +++++++++++++++++++++
 
-..
-    cmd2img:: python3
-    :image: sphx_glr_pie_features_0011.png
-
+.. _sphx_glr_pie_features_0011.py:
 .. code-block:: python
 
     #!/usr/bin/env python3
     #coding=utf8
     from pygnuplot import gnuplot
     import pandas as pd
     import math
@@ -1601,60 +1114,55 @@
     df = df.fillna(startangle)
     #print(df)
 
     pie_shade = []
     pie_graph = []
 
     shade_offset = 0.03
+    g = gnuplot.Gnuplot(log = True,
+            output = '"sphx_glr_pie_features_0011.png"',
+            term = 'pngcairo size 640, 480',
+            key = None,
+            parametric = "",
+            border = "",
+            tics = "",
+            multiplot = True)
+
     for k, v in df.iterrows():
         #print(k,v)
         cos = math.cos((v['start']+v['end'])/2)
         sin = math.sin((v['start']+v['end'])/2)
 
         # If we'd like explode the piece, ad the dx/dy to move the origi point.
         dx = v['explode'] * cos
         dy = v['explode'] * sin
 
         # make the shade for each piece
-        piece = gnuplot.make_plot('cos(t)+%f, sin(t)+%f with filledcurves xy=%f,%f lc "grey80"'
-                    %(dx-shade_offset, dy-shade_offset, dx-shade_offset, dy-shade_offset),
+        g.plot('cos(t)+%f, sin(t)+%f with filledcurves xy=%f,%f lc "grey80"'
+                %(dx-shade_offset, dy-shade_offset, dx-shade_offset, dy-shade_offset),
                 trange = '[%f:%f]' %(v['start'], v['end']),
                 xrange = '[-1.5:1.5]',
                 yrange = '[-1.5:1.5]')
-        pie_shade.append(piece)
 
         # make the pie and label
-        piece = gnuplot.make_plot('cos(t)+%f, sin(t)+%f with filledcurve xy=%f,%f  lt %d'
-                    %(dx, dy, dx, dy, k+3),
+        g.plot('cos(t)+%f, sin(t)+%f with filledcurve xy=%f,%f  lt %d'
+                %(dx, dy, dx, dy, k+3),
                 trange = '[%f:%f]' %(v['start'], v['end']),
                 xrange = '[-1.5:1.5]',
                 yrange = '[-1.5:1.5]',
-                label = ['1 "%s" at %f, %f center front' %(v['labels'], 1.2*cos+dx, 1.2*sin+dy),
-                    '2 "%.1f%%" at %f, %f center front' %(v['percentage']*100, 0.6*cos, 0.6*sin)])
-        pie_graph.append(piece)
+                label = ['1 "%s" at %f, %f center front' %(v['labels'], 1.2*cos+dx, 1.2*sin+dy), '2 "%.1f%%" at %f, %f center front' %(v['percentage']*100, 0.6*cos, 0.6*sin)])
 
-    gnuplot.multiplot(*pie_shade, *pie_graph,
-            output = '"sphx_glr_pie_features_0011.png"',
-            terminal = 'pngcairo size 640, 480',
-            key = None,
-            parametric = '',
-            border = '',
-            tics = '',
-            multiplot = True)
-
-Refer to the original script: `Basic pie chart`_ and the original image:
+This is the output:
 
-.. _Basic pie chart: https://matplotlib.org/gallery/pie_and_polar_charts/pie_features.html#sphx-glr-gallery-pie-and-polar-charts-pie-features-py
-.. image:: https://matplotlib.org/_images/sphx_glr_pie_features_0011.png
-   :width: 350
+|sphx_glr_pie_features_0011.png|
 
-4. Q/A
+3. Q/A
 =======
 
-5. CHANGLOG
+4. CHANGLOG
 =============
 
 1.0 Initial upload;
 
 1.0.3 Now Gnuplot().plot()/splot() supplot set options as parameters.
 
 1.0.7 The pyplot.plot() now can accept both string and pandas.Dataframe as the
@@ -1675,12 +1183,17 @@
 1.1.2 Enhancement: If it's multiplot mode, automatically call the following
 Gnuplot to unset the label:
 
     g.unset('for [i=1:200] label i')
 
 1.1.3 Enhancement: When plotting the python generated data, we set the
 seperator to "," for easy using it in csv file.
+
 1.1.5 Bug fix: on some case it exit exceptionally.
+
 1.1.8 Remove some Chinese comments to remove the "UnicodeDecodeError" for some users.
+
 1.1.9 1) Run and update the examples in gnuplot6.0.0. 2) If you'd like enable multiplot, you shuld use  multimplot = True to replace multimplot = "".
 
+1.1.13 Document update.
+
```

### Comparing `py-gnuplot-1.1.9/pygnuplot/gnuplot.py` & `py-gnuplot-1.2.0/pygnuplot/gnuplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     for v in args:
         subplot["cmd"].append(v)
     for k,v in kwargs.items():
         subplot["attribute"][k] = v
     return subplot
 
 def multiplot(*args, **kwargs):
-    g = Gnuplot()
+    g = Gnuplot(log = True)
 
     g.set(**kwargs)
     if 'multiplot' not in kwargs.keys():
         g.cmd('set multiplot')
 
     for subplot in args:
 
@@ -290,14 +290,26 @@
         cmd = c.rstrip(',')
         self.cmd(cmd + '\n')
 
         # unset the label if it's in multiplot mode.
         if self.isMultiplot:
             self.unset('for [i=1:200] label i')
 
+    def splot(self, *items, **kwargs):
+        self.set(**kwargs)
+        c = 'splot'
+        for item in items:
+            c = c + " " + item + ","
+        cmd = c.rstrip(',')
+        self.cmd(cmd + '\n')
+
+        # unset the label if it's in multiplot mode.
+        if self.isMultiplot:
+            self.unset('for [i=1:200] label i')
+
     def plot_data(self, data, *items, **kwargs):
         '''
         data: The data that need to be plotted. It's either the string of list
         or the Pnadas Dataframe, if it's Pnadas Dataframe it would be converted
         to string by data.to_csv(). Note that we will execut a extra command
         "set datafile separator "," to fit the data format of csv.
         *items: The list of plot command;
@@ -354,26 +366,14 @@
         cmd = c.rstrip(',')
         self.cmd(cmd + '\n')
 
         # unset the label if it's in multiplot mode.
         if self.isMultiplot:
             self.unset('for [i=1:200] label i')
 
-    def splot(self, *items, **kwargs):
-        self.set(**kwargs)
-        c = 'splot'
-        for item in items:
-            c = c + " " + item + ","
-        cmd = c.rstrip(',')
-        self.cmd(cmd + '\n')
-
-        # unset the label if it's in multiplot mode.
-        if self.isMultiplot:
-            self.unset('for [i=1:200] label i')
-
 
     def evaluate(self, cmd):
         self.cmd('evaluate %s' %(cmd))
 
     def exit(self):
         self.cmd('exit')
```

### Comparing `py-gnuplot-1.1.9/pygnuplot/pyplot.py` & `py-gnuplot-1.2.0/pygnuplot/pyplot.py`

 * *Files identical despite different names*

### Comparing `py-gnuplot-1.1.9/setup.py` & `py-gnuplot-1.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(name='py-gnuplot',
-      version='1.1.9',
+      version='1.2.0',
       keywords = ["gnuplot", "pandas"],
       author='Yongping Guo',
       author_email='guoyoooping@163.com',
       description='py-gnuplot is a python plot tools based on gnuplot.',
       long_description=open('README.rst').read(),
       install_requires = ["pandas"],
       url='http://www.gnuplot.info',
```

