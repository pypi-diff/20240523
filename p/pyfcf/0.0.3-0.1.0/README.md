# Comparing `tmp/pyfcf-0.0.3.tar.gz` & `tmp/pyfcf-0.1.0.tar.gz`

## Comparing `pyfcf-0.0.3.tar` & `pyfcf-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,13 @@
--rwxr-xr-x   0        0        0      487 2020-02-02 00:00:00.000000 pyfcf-0.0.3/examples/single_figure.py
--rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 pyfcf-0.0.3/pyfcf/__init__.py
--rwxr-xr-x   0        0        0     6689 2020-02-02 00:00:00.000000 pyfcf-0.0.3/pyfcf/basic.py
--rwxr-xr-x   0        0        0       29 2020-02-02 00:00:00.000000 pyfcf-0.0.3/.gitignore
--rwxr-xr-x   0        0        0     1058 2020-02-02 00:00:00.000000 pyfcf-0.0.3/LICENSE
--rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 pyfcf-0.0.3/README.md
--rwxr-xr-x   0        0        0      510 2020-02-02 00:00:00.000000 pyfcf-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pyfcf-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 pyfcf-0.1.0/.gitattributes
+-rw-r--r--   0        0        0    49513 2020-02-02 00:00:00.000000 pyfcf-0.1.0/pixi.lock
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 pyfcf-0.1.0/dist_/pyfcf-0.0.3-py3-none-any.whl
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 pyfcf-0.1.0/dist_/pyfcf-0.0.3.tar.gz
+-rwxr-xr-x   0        0        0      757 2020-02-02 00:00:00.000000 pyfcf-0.1.0/examples/single_figure.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 pyfcf-0.1.0/examples/two_panel.py
+-rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 pyfcf-0.1.0/pyfcf/__init__.py
+-rwxr-xr-x   0        0        0     6984 2020-02-02 00:00:00.000000 pyfcf-0.1.0/pyfcf/basic.py
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 pyfcf-0.1.0/.gitignore
+-rwxr-xr-x   0        0        0     1058 2020-02-02 00:00:00.000000 pyfcf-0.1.0/LICENSE
+-rwxr-xr-x   0        0        0      706 2020-02-02 00:00:00.000000 pyfcf-0.1.0/README.md
+-rwxr-xr-x   0        0        0      796 2020-02-02 00:00:00.000000 pyfcf-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 pyfcf-0.1.0/PKG-INFO
```

### Comparing `pyfcf-0.0.3/pyfcf/basic.py` & `pyfcf-0.1.0/pyfcf/basic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,39 @@
+from typing import Union
 import matplotlib.pyplot as plt
 import numpy as np
+from pathlib import Path
 
 __ALL__ = ["FigConfig",  "setup_matplotlib", "axes_setup"]
 
-def setup_matplotlib(font_size:(int, float) =14) -> None:
+def setup_matplotlib(font_size:Union[int, float] =14, **kwargs) -> None:
     plt.rcParams["font.size"] = font_size
-    # font_family = ['DejaVu Sans', 'Garamond', 'Proxima Nova'][1]
-    # plt.rcParams["font.family"] = font_family
     plt.rcParams["axes.formatter.use_mathtext"] = True
     plt.rcParams["mathtext.fontset"] = "cm"
     plt.rcParams["figure.dpi"] = 200
-
+    for key, value in kwargs.items():
+        plt.rcParams[key] = value
 
 def axes_setup(axes):
     axes.spines["left"].set_position(("axes",-0.025))
     axes.spines["top"].set_visible(False)
     axes.spines["right"].set_visible(False)
     return
 
 
 class FigConfig():
     '''
     Class for generating pretty and customized matplotlib figures.
     '''
 
     def __init__(self, nx: int, ny: int,
-                 idx: (float, None) = None, idy: (float, None) = None,
-                 xs: (float, None) = None, ys: (float, None) = None,
+                 idx: Union[float, None] = None, idy: Union[float, None] = None,
+                 xs: Union[float, None] = None, ys: Union[float, None] = None,
                  xm: list = [], ym: list = [],
-                 cbx: float =0, cby: float=0, cpos: (str, None) = None):
+                 cbx: float =0, cby: float=0, cpos: Union[str, None] = None):
         '''
         :param nx: (int) number of sub figures in x dimension
         :param ny: (int) number of sub figure sin y dimension
         :param idx: (float) size of each x sub figure
         :param idy: (float) size of each y sub figure
         :param xs: (float) size of figure in x dimension
         :param ys: (float) size of figure in y dimension
@@ -55,38 +56,44 @@
             self.cpos = cpos.lower()
         else:
             self.cpos = None
         self.cbx = cbx
         self.cby = cby
 
         if idx is not None:
-            self.idx = idx
-            self.xs = idx*self.nx + self.xcm[-1]
+            if isinstance(idx, (float, int)):
+                self.idx = [idx]
+            else:     
+                self.idx = idx
+            self.xs = np.sum(idx) + self.xcm[-1]
             if self.cpos in ['left', 'right']:
                 self.xs += self.cbx
 
         if idy is not None:
-            self.idy = idy
-            self.ys = idy*self.ny + self.ycm[-1]
+            if isinstance(idy, (float, int)):
+                self.idy = [idy]
+            else:     
+                self.idy = idy            
+            self.ys = np.sum(idy) + self.ycm[-1]
             if self.cpos in ['bottom', 'top']:
                 self.ys += self.cby
 
         if xs is not None:
             self.xs = xs
             if self.cpos in ['left', 'right']:
-                self.idx = (self.xs - self.xcm[-1] - self.cbx)/self.nx
+                self.idx = (self.xs - self.xcm[-1] - self.cbx)
             else:
-                self.idx = (self.xs - self.xcm[-1])/self.nx
+                self.idx = (self.xs - self.xcm[-1])
 
         if ys is not None:
             self.ys = ys
             if self.cpos in ['bottom', 'top']:
-                self.idy = (self.ys - self.ycm[-1] - self.cby)/self.ny
+                self.idy = (self.ys - self.ycm[-1] - self.cby)
             else:
-                self.idy = (self.ys - self.ycm[-1])/self.ny
+                self.idy = (self.ys - self.ycm[-1])
 
         # set normalizing factor
         self.set_nrm()
 
         # check for self consistency
         self._check()
 
@@ -111,16 +118,17 @@
         if self.cpos == 'bottom':
             rect = np.array([self.xcm[ix]+ix*self.idx,
                              self.ycm[iy+1]+iy*self.idy+self.cby, self.idx, self.idy])
         elif self.cpos == 'left':
             rect = np.array([self.xcm[ix+1]+ix*self.idx+self.cbx,
                              self.ycm[iy]+iy*self.idy, self.idx, self.idy])
         else:
-            rect = np.array([self.xcm[ix]+ix*self.idx,
-                             self.ycm[iy]+iy*self.idy, self.idx, self.idy])
+            rect = np.array([self.xcm[ix]+np.cumsum(np.concatenate(([0],self.idx)))[ix],
+                             self.ycm[iy]+np.cumsum(np.concatenate(([0],self.idy)))[iy], 
+                             self.idx[ix], self.idy[iy]])
 
         return rect / self.nrm
 
     def get_cax_rect(self):
         '''Colorbar axis position'''
 
         if self.cpos is None:
@@ -142,31 +150,31 @@
                 self.cbx, self.cby])
         else:
             raise ValueError('Do not understand cpos:', self.cpos)
 
         return rect / self.nrm
 
     @staticmethod
-    def axes_setup(ax,
+    def setup_axes(ax,
                    left_position=-0.025, top_visible=False, right_visible=False,
                    ticklabelsize=10):
         ax.spines["left"].set_position(("axes",left_position))
         ax.spines["top"].set_visible(top_visible)
         ax.spines["right"].set_visible(right_visible)
         ax.tick_params(labelsize=ticklabelsize)
 
     @staticmethod
-    def matplotlib_setup(fontsize: (int, float) = 12, fontfamily=None, dpi=200) -> None:
-        if fontfamily is None:
-            fontfamily = ['DejaVu Sans', 'Garamond', 'Proxima Nova'][1]
-        plt.rcParams["font.size"] = fontsize
-        plt.rcParams["font.family"] = fontfamily
+    def setup_matplotlib(font_size: Union[int, float] = 12, dpi=200, **kwargs) -> None:
+        plt.rcParams["font.size"] = font_size
+        # plt.rcParams["font.family"] = fontfamily
         plt.rcParams["axes.formatter.use_mathtext"] = True
         plt.rcParams["mathtext.fontset"] = "cm"
         plt.rcParams["figure.dpi"] = dpi
+        for key, value in kwargs.items():
+            plt.rcParams[key] = value
 
     @staticmethod
     def set_fontsize(fontsize: float):
         plt.rcParams["font.size"] = fontsize
 
     @staticmethod
     def legend(ax, fontsize=10, **kwargs):
@@ -176,8 +184,8 @@
     def get_script_name(p):
         '''
         Returns the name of the path without extension. Useful for attributing figures to the scripts that generate them.
         Example: FigConfig.get_script_name(__file))
         :param p: path of the script
         :return: string without path and extension
         '''
-        return os.path.splitext(os.path.basename(p))[0]
+        return Path(p).stem
```

### Comparing `pyfcf-0.0.3/LICENSE` & `pyfcf-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfcf-0.0.3/PKG-INFO` & `pyfcf-0.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,30 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pyfcf
-Version: 0.0.3
+Version: 0.1.0
 Summary: Package to create standardized, publication quality matplotlib figures
 Author-email: Katherine Rosenfeld <krosenf@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: matplotlib
 Description-Content-Type: text/markdown
 
 README
 ======
-`pyfcf` is a package to create standardized, publication quality matplotlib figures.
+`pyfcf` is a package to create standardized, publication quality matplotlib figures. It is partcularly useful for creating figures where the axis are a specfic size, allowing standardization between figures in e.g., papers, charts, or posters.
 
 # Installation
 
+Requirements:
+
+- maptlotlib
+
 To install:
 
 ```
   pip install pyfcf
 ```
 
 # Examples
@@ -28,7 +32,19 @@
 Initialize basic `matplotlib` settings:
 
 ```
 pyfcf.setup_matplotlib()
 ```
 
 See `examples/` folder.
+
+# Development
+
+You need additional package `build` `wheel` and `twine`. Make sure that everything is up to date and then
+
+```
+  pip install --upgrade build wheel twine
+  python3 -m build
+  python3 -m twine upload --repository testpypi dist/*
+```
+
+
```

