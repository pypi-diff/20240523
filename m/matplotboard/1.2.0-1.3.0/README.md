# Comparing `tmp/matplotboard-1.2.0.tar.gz` & `tmp/matplotboard-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotboard-1.2.0.tar", last modified: Tue Oct  5 22:20:02 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `matplotboard-1.2.0.tar` & `matplotboard-1.3.0.tar`

### file list

```diff
@@ -1,54 +1,38 @@
-drwxrwxrwx   0        0        0        0 2021-10-05 22:20:02.269650 matplotboard-1.2.0/
--rw-rw-rw-   0        0        0     1090 2021-10-05 20:01:11.000000 matplotboard-1.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0       66 2021-10-05 20:01:11.000000 matplotboard-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     9766 2021-10-05 22:20:02.268649 matplotboard-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     8774 2021-10-05 20:01:11.000000 matplotboard-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2021-10-05 22:20:02.187650 matplotboard-1.2.0/matplotboard/
--rw-rw-rw-   0        0        0    12874 2021-10-05 22:09:44.000000 matplotboard-1.2.0/matplotboard/__init__.py
--rw-rw-rw-   0        0        0     1016 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/__main__.py
-drwxrwxrwx   0        0        0        0 2021-10-05 22:20:02.176150 matplotboard-1.2.0/matplotboard/static/
-drwxrwxrwx   0        0        0        0 2021-10-05 22:20:02.228148 matplotboard-1.2.0/matplotboard/static/css/
--rw-rw-rw-   0        0        0     4438 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/css/default.css
-drwxrwxrwx   0        0        0        0 2021-10-05 22:20:02.263648 matplotboard-1.2.0/matplotboard/static/icons/
--rw-rw-rw-   0        0        0     9991 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/android-icon-144x144.png
--rw-rw-rw-   0        0        0    13120 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/android-icon-192x192.png
--rw-rw-rw-   0        0        0     2349 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/android-icon-36x36.png
--rw-rw-rw-   0        0        0     3095 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/android-icon-48x48.png
--rw-rw-rw-   0        0        0     4471 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/android-icon-72x72.png
--rw-rw-rw-   0        0        0     6115 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/android-icon-96x96.png
--rw-rw-rw-   0        0        0     7463 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/apple-icon-114x114.png
--rw-rw-rw-   0        0        0     7897 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/apple-icon-120x120.png
--rw-rw-rw-   0        0        0     9991 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/apple-icon-144x144.png
--rw-rw-rw-   0        0        0    10692 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/apple-icon-152x152.png
--rw-rw-rw-   0        0        0    13063 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/apple-icon-180x180.png
--rw-rw-rw-   0        0        0     3549 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/apple-icon-57x57.png
--rw-rw-rw-   0        0        0     3726 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/apple-icon-60x60.png
--rw-rw-rw-   0        0        0     4471 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/apple-icon-72x72.png
--rw-rw-rw-   0        0        0     4763 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/apple-icon-76x76.png
--rw-rw-rw-   0        0        0    13609 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/apple-icon-precomposed.png
--rw-rw-rw-   0        0        0    13609 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/apple-icon.png
--rw-rw-rw-   0        0        0      282 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/browserconfig.xml
--rw-rw-rw-   0        0        0     1236 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/favicon-16x16.png
--rw-rw-rw-   0        0        0     2096 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/favicon-32x32.png
--rw-rw-rw-   0        0        0     6115 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/favicon-96x96.png
--rw-rw-rw-   0        0        0     1150 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/favicon.ico
--rw-rw-rw-   0        0        0      760 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/manifest.json
--rw-rw-rw-   0        0        0     9991 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/ms-icon-144x144.png
--rw-rw-rw-   0        0        0    10511 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/ms-icon-150x150.png
--rw-rw-rw-   0        0        0    26587 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/ms-icon-310x310.png
--rw-rw-rw-   0        0        0     4354 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/static/icons/ms-icon-70x70.png
-drwxrwxrwx   0        0        0        0 2021-10-05 22:20:02.267151 matplotboard-1.2.0/matplotboard/templates/
--rw-rw-rw-   0        0        0     5022 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/templates/base.j2
--rw-rw-rw-   0        0        0     9537 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/templates/dump.j2
--rw-rw-rw-   0        0        0     2654 2021-10-05 20:01:11.000000 matplotboard-1.2.0/matplotboard/templates/report.j2
--rw-rw-rw-   0        0        0       23 2021-10-05 22:14:13.000000 matplotboard-1.2.0/matplotboard/version.py
-drwxrwxrwx   0        0        0        0 2021-10-05 22:20:02.226148 matplotboard-1.2.0/matplotboard.egg-info/
--rw-rw-rw-   0        0        0     9766 2021-10-05 22:20:01.000000 matplotboard-1.2.0/matplotboard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1743 2021-10-05 22:20:02.000000 matplotboard-1.2.0/matplotboard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-10-05 22:20:01.000000 matplotboard-1.2.0/matplotboard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2021-10-05 22:20:01.000000 matplotboard-1.2.0/matplotboard.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      108 2021-10-05 22:20:01.000000 matplotboard-1.2.0/matplotboard.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2021-10-05 22:20:01.000000 matplotboard-1.2.0/matplotboard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      114 2021-10-05 20:01:11.000000 matplotboard-1.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2021-10-05 22:20:02.270151 matplotboard-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     2180 2021-10-05 22:13:59.000000 matplotboard-1.2.0/setup.py
+-rw-r--r--   0        0        0    12882 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/__init__.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/version.py
+-rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/css/default.css
+-rw-r--r--   0        0        0     9991 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/android-icon-144x144.png
+-rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/android-icon-192x192.png
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/android-icon-36x36.png
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/android-icon-48x48.png
+-rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/android-icon-72x72.png
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/android-icon-96x96.png
+-rw-r--r--   0        0        0     7463 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/apple-icon-114x114.png
+-rw-r--r--   0        0        0     7897 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/apple-icon-120x120.png
+-rw-r--r--   0        0        0     9991 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/apple-icon-144x144.png
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/apple-icon-152x152.png
+-rw-r--r--   0        0        0    13063 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/apple-icon-180x180.png
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/apple-icon-57x57.png
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/apple-icon-60x60.png
+-rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/apple-icon-72x72.png
+-rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/apple-icon-76x76.png
+-rw-r--r--   0        0        0    13609 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/apple-icon-precomposed.png
+-rw-r--r--   0        0        0    13609 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/apple-icon.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/browserconfig.xml
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/favicon-16x16.png
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/favicon-32x32.png
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/favicon-96x96.png
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/favicon.ico
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/manifest.json
+-rw-r--r--   0        0        0     9991 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/ms-icon-144x144.png
+-rw-r--r--   0        0        0    10511 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/ms-icon-150x150.png
+-rw-r--r--   0        0        0    26587 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/ms-icon-310x310.png
+-rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/static/icons/ms-icon-70x70.png
+-rw-r--r--   0        0        0     5022 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/templates/base.j2
+-rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/templates/dump.j2
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 matplotboard-1.3.0/matplotboard/templates/report.j2
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 matplotboard-1.3.0/.gitignore
+-rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 matplotboard-1.3.0/README.md
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 matplotboard-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9785 2020-02-02 00:00:00.000000 matplotboard-1.3.0/PKG-INFO
```

### Comparing `matplotboard-1.2.0/PKG-INFO` & `matplotboard-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: matplotboard
-Version: 1.2.0
-Summary: Generate simple HTML dashboards using matplotlib
-Home-page: https://github.com/cfangmeier/matplotboard
-Author: Caleb Fangmeier
-Author-email: caleb@fangmeier.tech
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
-Classifier: Topic :: Software Development :: Documentation
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Processing :: Markup :: HTML
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 ![Matplotboard: For your Health!](https://cfangmeier.github.io/matplotboard/matplotboard.png)
 
 [![Build Status](https://travis-ci.com/cfangmeier/matplotboard.svg?branch=master)](https://travis-ci.com/cfangmeier/matplotboard)
 
 A utility to generate html dashboards using matplotlib. Matplotboard makes it easy to
 wrap your plotting functions and dump the plots into a searchable webpage or a markdown report. This is best
 demonstrated with an example.
@@ -54,15 +30,15 @@
 
 First, we import `numpy` and `matplotlib` for some calculations, and plotting,
 respectively. As well as `matplotboard` itself.
 
 ```python
 import numpy as np
 import matplotlib.pyplot as plt
-import matplotboard as mpb
+from src import matplotboard as mpb
 ```
 
 
 `matplotboard` relies upon `matplotlib` for the underlying rendering engine so
 other plotting libraries are not supported. However, wrappers around
 `matplotlib` such as `seaborn` should work.
 
@@ -264,9 +240,7 @@
 possible by use of a `row` div as shown in the example.
 
 In addition to including generated figures via the `fig::` construct, static
 figures (such as diagrams or photographs) can be included via the `locfig::`
 (think local figure) construct, where instead of the figure name, you specify
 the path to the file. Finally, pictures out on the internet can be specified
 via `extfig::`.
-
-
```

### Comparing `matplotboard-1.2.0/README.md` & `matplotboard-1.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,246 +1,276 @@
-![Matplotboard: For your Health!](https://cfangmeier.github.io/matplotboard/matplotboard.png)
-
-[![Build Status](https://travis-ci.com/cfangmeier/matplotboard.svg?branch=master)](https://travis-ci.com/cfangmeier/matplotboard)
-
-A utility to generate html dashboards using matplotlib. Matplotboard makes it easy to
-wrap your plotting functions and dump the plots into a searchable webpage or a markdown report. This is best
-demonstrated with an example.
-
-
-``` python
-import numpy as np
-import matplotlib.pyplot as plt
-import matplotboard as mpb
-
-@mpb.decl_fig
-def cool_fig():
-    xs = np.linspace(-10, 10, 100)
-    ys = xs**2
-    plt.plot(xs, ys)
-
-if __name__ == '__main__':
-    figures = {
-        'cool_fig': cool_fig(),
-    }
-
-    mpb.render(figures)
-    mpb.generate_report(figures, 'Report')
-```
-You can view the results [here](https://cfangmeier.github.io/matplotboard/example_01/dashboard/report.html). Let's walk through this one part at a time.
-
-First, we import `numpy` and `matplotlib` for some calculations, and plotting,
-respectively. As well as `matplotboard` itself.
-
-```python
-import numpy as np
-import matplotlib.pyplot as plt
-import matplotboard as mpb
-```
-
-
-`matplotboard` relies upon `matplotlib` for the underlying rendering engine so
-other plotting libraries are not supported. However, wrappers around
-`matplotlib` such as `seaborn` should work.
-
-Next, we declare the function that is actually going to do the plotting.
-
-```python
-@mpb.decl_fig
-def cool_fig():
-    xs = np.linspace(-10,10, 100)
-    ys = xs**2
-    plt.plot(xs, ys)
-```
-
-The `decl_fig` decorator modifies the function to work with `matplotboard`. A
-plotting function decorated with `decl_fig` must fulfill the following
-contract:
-
-  - A clean `figure` has been initiated and the function will do any plotting
-    on that figure.
-  - It is free to subdivide the figure into as many axes as required, but
-    shouldn't create additional `Figure` objects.
-  - The function can optionally return Markdown text that will be rendered
-    along with the plot.
-  - The function shouldn't call `savefig`. This is handled by `matplotboard`
-    automatically.
-
-Finally, we declare the actual figures that we want to generate, and tell `matplotboard` to render the figures and assemble them into an interactive webpage.
-
-```python
-if __name__ == '__main__':
-    figures = {
-        'cool_fig': cool_fig(),
-    }
-
-    mpb.render(figures)
-    mpb.generate_report(figures, 'Report')
-```
-
-Both `render`, and `generate_report` take a dictionary as their first argument.
-The dictionary keys are strings that are interpreted as the individual figure
-names, and the dictionary values are the plots we want to generate. Note that
-the function is called before inserting it into the dictionary. Due to the 
-modification of the original function by the decorator, this doesn't actually
-call the function yet, but bundles the function and any arguments together
-into a `Figure` object which it then returns for later processing by `matplotboard`.
-
-By writing plotting functions with arguments, a single function can be reused
-to make many different plots. For example, you may have a dataset that is
-divided into several categories and you would like to plot some variable for
-each category. You could do this by writing one plotting function and calling
-it with different arguments to specify each of the categories.
-
-Try running the example. If everything works, there should be a new folder in
-the current directory called `dashboard`, and within it an html file called
-`report.html`. Open it with your browser to see a dashboard containing a single
-plot. Try clicking on it for a zoomed view!
-
-A single plot is not very interesting. Where `matplotboard` starts to really become useful is when you have lots of plots to generate. Check out the following example.
-
-```python
-from itertools import product
-import numpy as np
-import matplotlib.pyplot as plt
-import matplotboard as mpb
-
-@mpb.decl_fig
-def cool_fig(func, scale, color='b'):
-    xs = np.linspace(-scale, scale, 100)
-    f = {
-        'sin': lambda xs: np.sin(xs),
-        'tan': lambda xs: np.tan(xs),
-        'exp': lambda xs: np.exp(xs),
-    }[func]
-    ys = f(xs)
-    plt.plot(xs, ys, color=color)
-
-if __name__ == '__main__':
-    mpb.configure(multiprocess=True)
-    figures = {}
-
-    for color, function, scale in product('rbgk', ['sin', 'tan', 'exp'], np.linspace(1, 20, 20)):
-        figures[f'{function}_{color}_{scale}'] = cool_fig(function, scale, color=color)
-
-
-    mpb.render(figures)
-    mpb.generate_report(figures, 'Report')
-```
-
-What's changed? You can view the page [here](https://cfangmeier.github.io/matplotboard/example_02/dashboard/report.html)
-
-First of all, the plotting function has been enhanced to take a few arguments
-that modify it's behavior. You can now specify whether you would like to plot
-`sin`, `tan`, or `exp` as well as effectively set the x length scale.
-
-Second, we now are programatically making all combinations of plotting color,
-function, and scale with the `product` function and declaring a plot for each
-combination. This comes down to `4*3*20=240` different plots. To speed things
-up a bit, this example also switches on `matplotboard`'s multiprocessing
-support. Try running this example and open up the resulting web-page just as
-before. Note the pagination feature limiting the number of figures displayed at
-once. Also, try selecting a plot and moving through the figures on the page
-with the arrow keys. Finally, try out the filter box in the top right. A few
-interesting searches may be "sin\_", "\_r\_", or "tan\_g\_9" to search for all
-`sin` plots, all red plots, and just the `tan_g_9` plot, respectively.
-
-For one final example, let's look at the support for writing reports the incorporate generated figures.
-
-```python
-
-from itertools import product
-import numpy as np
-import matplotlib.pyplot as plt
-import matplotboard as mpb
-
-
-@mpb.decl_fig
-def cool_fig(func, scale, color="b"):
-    xs = np.linspace(-scale, scale, 100)
-    f = {
-        "sin": lambda xs: np.sin(xs),
-        "tan": lambda xs: np.tan(xs),
-        "exp": lambda xs: np.exp(xs),
-    }[func]
-    ys = f(xs)
-    plt.plot(xs, ys, color=color)
-
-
-report = """\
-Authors: Will Hunting
-Date: December 2, 1997
-
-# Report On Functions
-
-## Introduction
-
-As we all know, there are many functions. An example is the sine function seen below.
-fig::sin_b_1
-
-## Other Functions
-
-However, there are many other functions such as the tangent or exponential.
-
-<div class="row">
-<div class="col-md-6 row_fig">
-fig::tan_r_1|The rugged tangent function
-</div>
-<div class="col-md-6 row_fig">
-fig::exp_g_2|The majestic exponential function
-</div>
-</div>
-
-The decision of which function is best is up to *you*!
-
-## Local Figures
-
-I happened to have a couple *really* fantastic figures on my computer that I
-want to include as well. How do I include them? It's easy! Just add them to
-the list of figures with the `loc_fig` function and they will be marked to be
-copied to the output directory. Here are a couple examples:
-
-<div class="row">
-<div class="col-md-6 row_fig">
-fig::image8
-</div>
-<div class="col-md-6 row_fig">
-fig::image10
-</div>
-</div>
-"""
-
-if __name__ == "__main__":
-    mpb.configure(multiprocess=True)
-    figures = {}
-
-    for color, function, scale in product(
-        "rbgk", ["sin", "tan", "exp"], np.linspace(1, 5, 5)
-    ):
-        figures[f"{function}_{color}_{int(scale)}"] = cool_fig(
-            function, scale, color=color
-        )
-    figures["image8"] = mpb.loc_fig("figures/image8.png")
-    figures["image10"] = mpb.loc_fig("figures/image10.png")
-
-    mpb.render(figures)
-    mpb.generate_report(figures, "Report", body=report)
-```
-
-See result of this example [here](https://cfangmeier.github.io/matplotboard/example_03/dashboard/report.html).
-
-The `generate_report` function supports an optional `body` argument which
-signals `matplotboard` to render the markdown into a report, rather than making
-a simple plot dump. A special syntax is used for embedding generated figures.
-
-```
-fig::figure_name|Optional Caption
-```
-
-`Bootstrap` is included by default so multiple figures side-by-side are
-possible by use of a `row` div as shown in the example.
-
-In addition to including generated figures via the `fig::` construct, static
-figures (such as diagrams or photographs) can be included via the `locfig::`
-(think local figure) construct, where instead of the figure name, you specify
-the path to the file. Finally, pictures out on the internet can be specified
-via `extfig::`.
+Metadata-Version: 2.3
+Name: matplotboard
+Version: 1.3.0
+Summary: Generate simple HTML dashboards using matplotlib
+Project-URL: Homepage, https://github.com/cfangmeier/matplotboard
+Author-email: Caleb Fangmeier <caleb@fangmeier.tech>
+License-Expression: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Text Processing :: Markup :: HTML
+Requires-Dist: jinja2>=2.10
+Requires-Dist: markdown>=3.0.1
+Requires-Dist: matplotlib>=3.0.3
+Requires-Dist: openssh-wrapper>=0.4
+Requires-Dist: pathos>=0.2.3
+Requires-Dist: python-markdown-math>=0.6
+Provides-Extra: dev
+Requires-Dist: black>=24.0.0; extra == 'dev'
+Description-Content-Type: text/markdown
+
+![Matplotboard: For your Health!](https://cfangmeier.github.io/matplotboard/matplotboard.png)
+
+[![Build Status](https://travis-ci.com/cfangmeier/matplotboard.svg?branch=master)](https://travis-ci.com/cfangmeier/matplotboard)
+
+A utility to generate html dashboards using matplotlib. Matplotboard makes it easy to
+wrap your plotting functions and dump the plots into a searchable webpage or a markdown report. This is best
+demonstrated with an example.
+
+
+``` python
+import numpy as np
+import matplotlib.pyplot as plt
+import matplotboard as mpb
+
+@mpb.decl_fig
+def cool_fig():
+    xs = np.linspace(-10, 10, 100)
+    ys = xs**2
+    plt.plot(xs, ys)
+
+if __name__ == '__main__':
+    figures = {
+        'cool_fig': cool_fig(),
+    }
+
+    mpb.render(figures)
+    mpb.generate_report(figures, 'Report')
+```
+You can view the results [here](https://cfangmeier.github.io/matplotboard/example_01/dashboard/report.html). Let's walk through this one part at a time.
+
+First, we import `numpy` and `matplotlib` for some calculations, and plotting,
+respectively. As well as `matplotboard` itself.
+
+```python
+import numpy as np
+import matplotlib.pyplot as plt
+from src import matplotboard as mpb
+```
+
+
+`matplotboard` relies upon `matplotlib` for the underlying rendering engine so
+other plotting libraries are not supported. However, wrappers around
+`matplotlib` such as `seaborn` should work.
+
+Next, we declare the function that is actually going to do the plotting.
+
+```python
+@mpb.decl_fig
+def cool_fig():
+    xs = np.linspace(-10,10, 100)
+    ys = xs**2
+    plt.plot(xs, ys)
+```
+
+The `decl_fig` decorator modifies the function to work with `matplotboard`. A
+plotting function decorated with `decl_fig` must fulfill the following
+contract:
+
+  - A clean `figure` has been initiated and the function will do any plotting
+    on that figure.
+  - It is free to subdivide the figure into as many axes as required, but
+    shouldn't create additional `Figure` objects.
+  - The function can optionally return Markdown text that will be rendered
+    along with the plot.
+  - The function shouldn't call `savefig`. This is handled by `matplotboard`
+    automatically.
+
+Finally, we declare the actual figures that we want to generate, and tell `matplotboard` to render the figures and assemble them into an interactive webpage.
+
+```python
+if __name__ == '__main__':
+    figures = {
+        'cool_fig': cool_fig(),
+    }
+
+    mpb.render(figures)
+    mpb.generate_report(figures, 'Report')
+```
+
+Both `render`, and `generate_report` take a dictionary as their first argument.
+The dictionary keys are strings that are interpreted as the individual figure
+names, and the dictionary values are the plots we want to generate. Note that
+the function is called before inserting it into the dictionary. Due to the 
+modification of the original function by the decorator, this doesn't actually
+call the function yet, but bundles the function and any arguments together
+into a `Figure` object which it then returns for later processing by `matplotboard`.
+
+By writing plotting functions with arguments, a single function can be reused
+to make many different plots. For example, you may have a dataset that is
+divided into several categories and you would like to plot some variable for
+each category. You could do this by writing one plotting function and calling
+it with different arguments to specify each of the categories.
+
+Try running the example. If everything works, there should be a new folder in
+the current directory called `dashboard`, and within it an html file called
+`report.html`. Open it with your browser to see a dashboard containing a single
+plot. Try clicking on it for a zoomed view!
+
+A single plot is not very interesting. Where `matplotboard` starts to really become useful is when you have lots of plots to generate. Check out the following example.
+
+```python
+from itertools import product
+import numpy as np
+import matplotlib.pyplot as plt
+import matplotboard as mpb
+
+@mpb.decl_fig
+def cool_fig(func, scale, color='b'):
+    xs = np.linspace(-scale, scale, 100)
+    f = {
+        'sin': lambda xs: np.sin(xs),
+        'tan': lambda xs: np.tan(xs),
+        'exp': lambda xs: np.exp(xs),
+    }[func]
+    ys = f(xs)
+    plt.plot(xs, ys, color=color)
+
+if __name__ == '__main__':
+    mpb.configure(multiprocess=True)
+    figures = {}
+
+    for color, function, scale in product('rbgk', ['sin', 'tan', 'exp'], np.linspace(1, 20, 20)):
+        figures[f'{function}_{color}_{scale}'] = cool_fig(function, scale, color=color)
+
+
+    mpb.render(figures)
+    mpb.generate_report(figures, 'Report')
+```
+
+What's changed? You can view the page [here](https://cfangmeier.github.io/matplotboard/example_02/dashboard/report.html)
+
+First of all, the plotting function has been enhanced to take a few arguments
+that modify it's behavior. You can now specify whether you would like to plot
+`sin`, `tan`, or `exp` as well as effectively set the x length scale.
+
+Second, we now are programatically making all combinations of plotting color,
+function, and scale with the `product` function and declaring a plot for each
+combination. This comes down to `4*3*20=240` different plots. To speed things
+up a bit, this example also switches on `matplotboard`'s multiprocessing
+support. Try running this example and open up the resulting web-page just as
+before. Note the pagination feature limiting the number of figures displayed at
+once. Also, try selecting a plot and moving through the figures on the page
+with the arrow keys. Finally, try out the filter box in the top right. A few
+interesting searches may be "sin\_", "\_r\_", or "tan\_g\_9" to search for all
+`sin` plots, all red plots, and just the `tan_g_9` plot, respectively.
+
+For one final example, let's look at the support for writing reports the incorporate generated figures.
+
+```python
+
+from itertools import product
+import numpy as np
+import matplotlib.pyplot as plt
+import matplotboard as mpb
+
+
+@mpb.decl_fig
+def cool_fig(func, scale, color="b"):
+    xs = np.linspace(-scale, scale, 100)
+    f = {
+        "sin": lambda xs: np.sin(xs),
+        "tan": lambda xs: np.tan(xs),
+        "exp": lambda xs: np.exp(xs),
+    }[func]
+    ys = f(xs)
+    plt.plot(xs, ys, color=color)
+
+
+report = """\
+Authors: Will Hunting
+Date: December 2, 1997
+
+# Report On Functions
+
+## Introduction
+
+As we all know, there are many functions. An example is the sine function seen below.
+fig::sin_b_1
+
+## Other Functions
+
+However, there are many other functions such as the tangent or exponential.
+
+<div class="row">
+<div class="col-md-6 row_fig">
+fig::tan_r_1|The rugged tangent function
+</div>
+<div class="col-md-6 row_fig">
+fig::exp_g_2|The majestic exponential function
+</div>
+</div>
+
+The decision of which function is best is up to *you*!
+
+## Local Figures
+
+I happened to have a couple *really* fantastic figures on my computer that I
+want to include as well. How do I include them? It's easy! Just add them to
+the list of figures with the `loc_fig` function and they will be marked to be
+copied to the output directory. Here are a couple examples:
+
+<div class="row">
+<div class="col-md-6 row_fig">
+fig::image8
+</div>
+<div class="col-md-6 row_fig">
+fig::image10
+</div>
+</div>
+"""
+
+if __name__ == "__main__":
+    mpb.configure(multiprocess=True)
+    figures = {}
+
+    for color, function, scale in product(
+        "rbgk", ["sin", "tan", "exp"], np.linspace(1, 5, 5)
+    ):
+        figures[f"{function}_{color}_{int(scale)}"] = cool_fig(
+            function, scale, color=color
+        )
+    figures["image8"] = mpb.loc_fig("figures/image8.png")
+    figures["image10"] = mpb.loc_fig("figures/image10.png")
+
+    mpb.render(figures)
+    mpb.generate_report(figures, "Report", body=report)
+```
+
+See result of this example [here](https://cfangmeier.github.io/matplotboard/example_03/dashboard/report.html).
+
+The `generate_report` function supports an optional `body` argument which
+signals `matplotboard` to render the markdown into a report, rather than making
+a simple plot dump. A special syntax is used for embedding generated figures.
+
+```
+fig::figure_name|Optional Caption
+```
+
+`Bootstrap` is included by default so multiple figures side-by-side are
+possible by use of a `row` div as shown in the example.
+
+In addition to including generated figures via the `fig::` construct, static
+figures (such as diagrams or photographs) can be included via the `locfig::`
+(think local figure) construct, where instead of the figure name, you specify
+the path to the file. Finally, pictures out on the internet can be specified
+via `extfig::`.
```

### Comparing `matplotboard-1.2.0/matplotboard/__init__.py` & `matplotboard-1.3.0/matplotboard/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,17 @@
             txt_raw = ""
         self.html = MD.convert(txt_raw)
         self.argdict = self._fn_call_to_dict(self.render_fn, *self.args, **self.kwargs)
         self.docs = self._process_docs(self.render_fn)
 
     @staticmethod
     def _fn_call_to_dict(fn, *args, **kwargs):
-        from inspect import getargspec
+        from inspect import getfullargspec
 
-        pnames = list(getargspec(fn).args)
+        pnames = list(getfullargspec(fn).args)
         pvals = list(args) + list(kwargs.values())
 
         def escape(s, quote=True):
             s = s.replace("&", "&amp;")  # Must be done first!
             s = s.replace("<", "&lt;")
             s = s.replace(">", "&gt;")
             if quote:
```

### Comparing `matplotboard-1.2.0/matplotboard/__main__.py` & `matplotboard-1.3.0/matplotboard/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from .version import __version__
-
-
 def main():
     from glob import glob
     from os.path import join, split, splitext
     from argparse import ArgumentParser
     from . import render, generate_report, loc_fig, configure
 
     parser = ArgumentParser("mpb", description="Matplotboard Command Line Utility")
```

### Comparing `matplotboard-1.2.0/matplotboard/static/css/default.css` & `matplotboard-1.3.0/matplotboard/static/css/default.css`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/android-icon-144x144.png` & `matplotboard-1.3.0/matplotboard/static/icons/android-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/android-icon-192x192.png` & `matplotboard-1.3.0/matplotboard/static/icons/android-icon-192x192.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/android-icon-36x36.png` & `matplotboard-1.3.0/matplotboard/static/icons/android-icon-36x36.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/android-icon-48x48.png` & `matplotboard-1.3.0/matplotboard/static/icons/android-icon-48x48.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/android-icon-72x72.png` & `matplotboard-1.3.0/matplotboard/static/icons/android-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/android-icon-96x96.png` & `matplotboard-1.3.0/matplotboard/static/icons/android-icon-96x96.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/apple-icon-114x114.png` & `matplotboard-1.3.0/matplotboard/static/icons/apple-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/apple-icon-120x120.png` & `matplotboard-1.3.0/matplotboard/static/icons/apple-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/apple-icon-144x144.png` & `matplotboard-1.3.0/matplotboard/static/icons/apple-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/apple-icon-152x152.png` & `matplotboard-1.3.0/matplotboard/static/icons/apple-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/apple-icon-180x180.png` & `matplotboard-1.3.0/matplotboard/static/icons/apple-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/apple-icon-57x57.png` & `matplotboard-1.3.0/matplotboard/static/icons/apple-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/apple-icon-60x60.png` & `matplotboard-1.3.0/matplotboard/static/icons/apple-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/apple-icon-72x72.png` & `matplotboard-1.3.0/matplotboard/static/icons/apple-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/apple-icon-76x76.png` & `matplotboard-1.3.0/matplotboard/static/icons/apple-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/apple-icon-precomposed.png` & `matplotboard-1.3.0/matplotboard/static/icons/apple-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/apple-icon.png` & `matplotboard-1.3.0/matplotboard/static/icons/apple-icon.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/favicon-16x16.png` & `matplotboard-1.3.0/matplotboard/static/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/favicon-32x32.png` & `matplotboard-1.3.0/matplotboard/static/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/favicon-96x96.png` & `matplotboard-1.3.0/matplotboard/static/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/favicon.ico` & `matplotboard-1.3.0/matplotboard/static/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/manifest.json` & `matplotboard-1.3.0/matplotboard/static/icons/manifest.json`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/ms-icon-144x144.png` & `matplotboard-1.3.0/matplotboard/static/icons/ms-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/ms-icon-150x150.png` & `matplotboard-1.3.0/matplotboard/static/icons/ms-icon-150x150.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/ms-icon-310x310.png` & `matplotboard-1.3.0/matplotboard/static/icons/ms-icon-310x310.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/static/icons/ms-icon-70x70.png` & `matplotboard-1.3.0/matplotboard/static/icons/ms-icon-70x70.png`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/templates/base.j2` & `matplotboard-1.3.0/matplotboard/templates/base.j2`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/templates/dump.j2` & `matplotboard-1.3.0/matplotboard/templates/dump.j2`

 * *Files identical despite different names*

### Comparing `matplotboard-1.2.0/matplotboard/templates/report.j2` & `matplotboard-1.3.0/matplotboard/templates/report.j2`

 * *Files identical despite different names*

