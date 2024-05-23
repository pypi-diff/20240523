# Comparing `tmp/pycatflow-0.0.8.tar.gz` & `tmp/pycatflow-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatflow-0.0.8.tar", last modified: Mon Sep 27 08:30:45 2021, max compression
+gzip compressed data, was "pycatflow-0.0.9.tar", last modified: Thu May 23 15:55:03 2024, max compression
```

## Comparing `pycatflow-0.0.8.tar` & `pycatflow-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 bumatic    (501) staff       (20)        0 2021-09-27 08:30:45.835116 pycatflow-0.0.8/
--rw-r--r--   0 bumatic    (501) staff       (20)     3081 2021-09-27 08:30:45.830436 pycatflow-0.0.8/PKG-INFO
--rw-r--r--   0 bumatic    (501) staff       (20)     2159 2021-09-21 11:25:56.000000 pycatflow-0.0.8/README.md
-drwxr-xr-x   0 bumatic    (501) staff       (20)        0 2021-09-27 08:30:45.829371 pycatflow-0.0.8/pycatflow/
--rw-r--r--   0 bumatic    (501) staff       (20)       40 2021-09-21 07:50:42.000000 pycatflow-0.0.8/pycatflow/__init__.py
--rw-r--r--   0 bumatic    (501) staff       (20)     9068 2021-09-27 08:20:24.000000 pycatflow-0.0.8/pycatflow/input.py
--rw-r--r--   0 bumatic    (501) staff       (20)    27937 2021-09-27 06:07:53.000000 pycatflow-0.0.8/pycatflow/viz.py
-drwxr-xr-x   0 bumatic    (501) staff       (20)        0 2021-09-27 08:30:45.830231 pycatflow-0.0.8/pycatflow.egg-info/
--rw-r--r--   0 bumatic    (501) staff       (20)     3081 2021-09-27 08:30:45.000000 pycatflow-0.0.8/pycatflow.egg-info/PKG-INFO
--rw-r--r--   0 bumatic    (501) staff       (20)      255 2021-09-27 08:30:45.000000 pycatflow-0.0.8/pycatflow.egg-info/SOURCES.txt
--rw-r--r--   0 bumatic    (501) staff       (20)        1 2021-09-27 08:30:45.000000 pycatflow-0.0.8/pycatflow.egg-info/dependency_links.txt
--rw-r--r--   0 bumatic    (501) staff       (20)       19 2021-09-27 08:30:45.000000 pycatflow-0.0.8/pycatflow.egg-info/requires.txt
--rw-r--r--   0 bumatic    (501) staff       (20)       10 2021-09-27 08:30:45.000000 pycatflow-0.0.8/pycatflow.egg-info/top_level.txt
--rw-r--r--   0 bumatic    (501) staff       (20)      108 2021-09-21 07:50:42.000000 pycatflow-0.0.8/pyproject.toml
--rw-r--r--   0 bumatic    (501) staff       (20)       38 2021-09-27 08:30:45.835188 pycatflow-0.0.8/setup.cfg
--rw-r--r--   0 bumatic    (501) staff       (20)      784 2021-09-27 08:30:25.000000 pycatflow-0.0.8/setup.py
+drwxr-xr-x   0 bumatic    (501) staff       (20)        0 2024-05-23 15:55:03.252790 pycatflow-0.0.9/
+-rw-r--r--   0 bumatic    (501) staff       (20)     1077 2024-05-23 13:28:20.000000 pycatflow-0.0.9/LICENSE
+-rw-r--r--   0 bumatic    (501) staff       (20)     3308 2024-05-23 15:55:03.206320 pycatflow-0.0.9/PKG-INFO
+-rw-r--r--   0 bumatic    (501) staff       (20)     2844 2024-05-23 13:28:20.000000 pycatflow-0.0.9/README.md
+drwxr-xr-x   0 bumatic    (501) staff       (20)        0 2024-05-23 15:55:03.122018 pycatflow-0.0.9/pycatflow/
+-rw-r--r--   0 bumatic    (501) staff       (20)       40 2024-05-23 13:28:20.000000 pycatflow-0.0.9/pycatflow/__init__.py
+-rw-r--r--   0 bumatic    (501) staff       (20)     9068 2024-05-23 13:28:20.000000 pycatflow-0.0.9/pycatflow/input.py
+-rw-r--r--   0 bumatic    (501) staff       (20)    27971 2024-05-23 15:40:16.000000 pycatflow-0.0.9/pycatflow/viz.py
+drwxr-xr-x   0 bumatic    (501) staff       (20)        0 2024-05-23 15:55:03.200569 pycatflow-0.0.9/pycatflow.egg-info/
+-rw-r--r--   0 bumatic    (501) staff       (20)     3308 2024-05-23 15:55:03.000000 pycatflow-0.0.9/pycatflow.egg-info/PKG-INFO
+-rw-r--r--   0 bumatic    (501) staff       (20)      263 2024-05-23 15:55:03.000000 pycatflow-0.0.9/pycatflow.egg-info/SOURCES.txt
+-rw-r--r--   0 bumatic    (501) staff       (20)        1 2024-05-23 15:55:03.000000 pycatflow-0.0.9/pycatflow.egg-info/dependency_links.txt
+-rw-r--r--   0 bumatic    (501) staff       (20)       29 2024-05-23 15:55:03.000000 pycatflow-0.0.9/pycatflow.egg-info/requires.txt
+-rw-r--r--   0 bumatic    (501) staff       (20)       10 2024-05-23 15:55:03.000000 pycatflow-0.0.9/pycatflow.egg-info/top_level.txt
+-rw-r--r--   0 bumatic    (501) staff       (20)      108 2024-05-23 13:28:20.000000 pycatflow-0.0.9/pyproject.toml
+-rw-r--r--   0 bumatic    (501) staff       (20)       38 2024-05-23 15:55:03.253193 pycatflow-0.0.9/setup.cfg
+-rw-r--r--   0 bumatic    (501) staff       (20)      794 2024-05-23 15:39:27.000000 pycatflow-0.0.9/setup.py
```

### Comparing `pycatflow-0.0.8/README.md` & `pycatflow-0.0.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5531785.svg)](https://doi.org/10.5281/zenodo.5531785)
+
 # PyCatFlow
 
-This package is a visualization tool which allows the representation of temporal developments, based on categorical data.
+This package is a visualization tool which allows the representation of temporal developments, based on categorical data. I wrote a short [article on Medium](https://medium.com/@bumatic/pycatflow-visualizing-categorical-data-over-time-b344102bcce2) in which I outline the basic idea of PyCatFlow and provide a Tutorial for non-programmers based on a [Jupyter Notebook with interactive widgets that can be run online](https://mybinder.org/v2/gist/bumatic/83c3423595cde010da7ad059c6b8b2f5/HEAD).
 
 ## Install 
 
 PyCatFlow is available on PyPi:
 
 ```Shell
 $ pip3 install pycatflow
@@ -52,12 +54,14 @@
 Running the above code creates this visualization:
 
 ![Sample Visualization](https://raw.githubusercontent.com/bumatic/PyCatFlow/main/example/sample_viz.svg)
 
 
 ## Credits & License
 
-PyCatFlow was conceptualized by Marcus Burkhardt and implemented by Herbert Natta ([@herbertmn](https://github.com/herbertmn)). It is inspired by the Rankflow visualization tool develped by Bernhard Rieder. 
+PyCatFlow was conceptualized by Marcus Burkhardt and implemented in collaboration with Herbert Natta ([@herbertmn](https://github.com/herbertmn)). It is inspired by the Rankflow visualization tool develped by Bernhard Rieder. 
+
+**Cite as:** Marcus Burkhardt, and Herbert Natta. 2021. “PyCatFlow: A Python Package for Visualizing Categorical Data over Time”. Zenodo. https://doi.org/10.5281/zenodo.5531785.
 
 The package is released under MIT License.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pycatflow-0.0.8/pycatflow/input.py` & `pycatflow-0.0.9/pycatflow/input.py`

 * *Files identical despite different names*

### Comparing `pycatflow-0.0.8/pycatflow/viz.py` & `pycatflow-0.0.9/pycatflow/viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import drawSvg as draw
-from matplotlib import cm,colors
+import drawsvg as draw
+from matplotlib import colormaps,colors
 import pycatflow as pcf
 import math
 import copy
 
 debug_legend = False
 
 class Node:
@@ -187,24 +187,24 @@
     elif height is None:
         height = spacing * 4 + max([x.y for x in points]) + ((sum([x.size for x in points]) / len(points)) * len(set([x.category for x in points])))
     elif width is None:
         width = spacing * 4 + max([x.x for x in points])
 
     # COLORS
     if palette is not None:
-        palette = cm.get_cmap(palette[0], palette[1]).colors
+        palette = colormaps.get_cmap(palette[0]).colors[:palette[1]]
         count = 0
         category_colors = {}
         for e in set([n.category for n in points]):
             if count < len(palette):
                 count += 1
             category_colors[e] = colors.to_hex(palette[count])
     else:
         # DEFAULT PALETTE: the number of colors is set in relation to the length of the category list
-        palette = cm.get_cmap("tab20c", len(set([n.category for n in points])) + 1).colors
+        palette = colormaps.get_cmap("tab20c").colors[:(len(set([n.category for n in points])) + 1)]
         count = 0
         category_colors = {}
         for e in set([n.category for n in points]):
             if count < len(palette)-1:
                 count += 1
             category_colors[e] = colors.to_hex(palette[count])
 
@@ -225,28 +225,28 @@
         l = label_size
         if label_shortening == "resize":
             while len(h)*(l/2) > n2+points[0].size-(n2/8) and l > 1:
                 if x != max(h_x_shift):
                     l -= 1
                 else:
                     break
-            d.append(draw.Text(h, x=x, y=height - spacing, fontSize=l, font_family=label_font, fill=label_color))
+            d.append(draw.Text(h, x=x, y=height - spacing, font_size=l, font_family=label_font, fill=label_color))
         elif label_shortening == "clip":
             clip = draw.ClipPath()
             clip.append(draw.Rectangle(x, height - spacing, n2, label_size))
-            d.append(draw.Text(h, x=x, y=height - spacing, fontSize=l, font_family=label_font, clip_path=clip, fill=label_color))
+            d.append(draw.Text(h, x=x, y=height - spacing, font_size=l, font_family=label_font, clip_path=clip, fill=label_color))
         elif label_shortening == "new_line":
             if len(h)*(label_size/2) > n2+points[0].size-(n2/8):
                 margin = int((n2+points[0].size-(n2/8))/(label_size/2))
                 txt = [h[x:x+margin] for x in range(0, len(h), margin)]
                 while len(txt)*l > (l+n2/5) and l > 1:
                     l -= 1
             else:
                 txt = h
-            d.append(draw.Text(txt, x=x, y=height-spacing, fontSize=l, font_family=label_font, fill=label_color))
+            d.append(draw.Text(txt, x=x, y=height-spacing, font_size=l, font_family=label_font, fill=label_color))
     
     # lines
     for n in sequence.items():        
         if len(n[1]) > 1:
             for k in n[1][:-1]:
                 if color_categories:
                     color = category_colors[points[k].category]
@@ -419,37 +419,37 @@
                         l -= 1
 
             label_pos_y = height - node.y + (node.size/2) - (l/2)
             if label_position == "start_end":
                 if node.label not in [n.label for n in points][:node.index] or node.label not in [n.label for n in points][node.index+1:] and node.index < len(points) and node.x != max([n.x for n in points]):
                     if label_shortening == "clip":
                         label = draw.Text(txt, x=node.x+node.width+(n2/8), y=label_pos_y,
-                                          fontSize=l, font_family=label_font, fill=label_color, clip_path=clip)
+                                          font_size=l, font_family=label_font, fill=label_color, clip_path=clip)
                     else:
                         label = draw.Text(txt, x=node.x-(n2/8), y=label_pos_y,
-                                          fontSize=l, font_family=label_font, fill=label_color, text_anchor="end")
+                                          font_size=l, font_family=label_font, fill=label_color, text_anchor="end")
 
             elif label_position == "nodes":
                 if label_shortening == "clip":
                     label = draw.Text(txt, x=node.x+node.width+(n2/8), y=label_pos_y,
-                                      fontSize=l, font_family=label_font, fill=label_color, clip_path=clip)
+                                      font_size=l, font_family=label_font, fill=label_color, clip_path=clip)
                 else:
                     label = draw.Text(txt, x=node.x + node.width+(n2/8), y=label_pos_y,
-                                      fontSize=l, font_family=label_font, fill=label_color)
+                                      font_size=l, font_family=label_font, fill=label_color)
             d.append(label)
     
     # Add legend to canvas
     if color_categories and legend:
         offset = 5  # Alternative: offset = spacing
         spacing_bottom = 5  # Alternative: spacing_bottom = spacing
         symbol_size = sum([x.size for x in points])/len(points)
         
         legend_height = (symbol_size+offset) * len(category_colors)
         legend_header_y = legend_height + symbol_size + spacing_bottom + (offset)
-        legend_header = draw.Text("Legend", x=points[0].x, y=legend_header_y, fontSize=label_size,
+        legend_header = draw.Text("Legend", x=points[0].x, y=legend_header_y, font_size=label_size,
                                   font_family=label_font, fill=label_color)
 
         if debug_legend:
             print('Legend Title')
             print('legend_height: {}'.format(legend_height))
             print('legend_header_y: {}'.format(legend_header_y))
             print('points[0].x: {}'.format(points[0].x))
@@ -471,15 +471,15 @@
                 print('points[0].x: {}'.format(points[0].x))
                 print('spacing_bottom+legend_height-offset-symbol_y_shift: {}'.format(spacing_bottom+legend_height-offset-symbol_y_shift))
                 print('points[0].width: {}'.format(points[0].width))
                 print('symbol_size: {}'.format(symbol_size))
                 print()
 
             name = draw.Text(e[0], x=points[0].x+node.width+(n2/12), y=legend_label_y,
-                             fontSize=label_size, fill=label_color)
+                             font_size=label_size, fill=label_color)
             d.append(symbol)
             d.append(name)
             if spacing_bottom+legend_height-(offset)-symbol_y_shift > spacing_bottom:
                 symbol_y_shift += offset+symbol_size
             else:
                 symbol_y_shift = 0
```

### Comparing `pycatflow-0.0.8/setup.py` & `pycatflow-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pycatflow", 
-    version="0.0.8",
+    version="0.0.9",
     author="Marcus Burkhardt",
     author_email="marcus.burkhardt@gmail.com",
     description="A tool for visualizing categorical data over time.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bumatic/PyCatFlow",
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(),
     python_requires=">=3.6",
-    install_requires=['drawSVG', 'matplotlib']
+    install_requires=['drawsvg[all]>=2.0', 'matplotlib']
 )
```

